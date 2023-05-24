# Comparing `tmp/fastapi_keycloak-1.0.6.tar.gz` & `tmp/fastapi_keycloak-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_keycloak-1.0.6.tar", last modified: Thu Jun 16 13:31:53 2022, max compression
+gzip compressed data, was "fastapi_keycloak-1.0.7.tar", last modified: Sun Jul 24 08:07:20 2022, max compression
```

## Comparing `fastapi_keycloak-1.0.6.tar` & `fastapi_keycloak-1.0.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      711 2021-12-22 13:15:56.130204 fastapi_keycloak-1.0.6/.github/FUNDING.yml
--rw-r--r--   0        0        0     1298 2022-05-18 19:51:01.947488 fastapi_keycloak-1.0.6/.github/workflows/testing.yaml
--rw-r--r--   0        0        0     1849 2022-03-22 13:04:51.310339 fastapi_keycloak-1.0.6/.gitignore
--rw-r--r--   0        0        0    11363 2022-04-20 10:53:17.924267 fastapi_keycloak-1.0.6/LICENSE
--rw-r--r--   0        0        0     2631 2022-05-18 19:51:01.947878 fastapi_keycloak-1.0.6/README.md
--rw-r--r--   0        0        0       23 2022-04-20 10:53:17.925346 fastapi_keycloak-1.0.6/codecov.yaml
--rw-r--r--   0        0        0       36 2022-03-22 13:01:36.237253 fastapi_keycloak-1.0.6/documentation/docs/CNAME
--rw-r--r--   0        0        0      464 2022-03-22 13:03:08.325253 fastapi_keycloak-1.0.6/documentation/docs/apple-m1.md
--rw-r--r--   0        0        0      212 2022-03-22 13:09:11.601295 fastapi_keycloak-1.0.6/documentation/docs/css/styles.css
--rw-r--r--   0        0        0    74518 2022-04-20 10:53:17.931883 fastapi_keycloak-1.0.6/documentation/docs/downloads/realm-export.json
--rw-r--r--   0        0        0     6411 2022-06-16 13:29:04.107491 fastapi_keycloak-1.0.6/documentation/docs/full_example.md
--rw-r--r--   0        0        0     1344 2022-03-22 13:07:41.343593 fastapi_keycloak-1.0.6/documentation/docs/img/favicon.svg
--rw-r--r--   0        0        0     5713 2022-03-22 13:07:35.562473 fastapi_keycloak-1.0.6/documentation/docs/img/logo.png
--rw-r--r--   0        0        0     2215 2022-03-22 12:57:41.238321 fastapi_keycloak-1.0.6/documentation/docs/index.md
--rw-r--r--   0        0        0      771 2022-03-22 13:03:45.709009 fastapi_keycloak-1.0.6/documentation/docs/keycloak_configuration.md
--rw-r--r--   0        0        0     3752 2022-03-22 13:01:33.790846 fastapi_keycloak-1.0.6/documentation/docs/quick_start.md
--rw-r--r--   0        0        0      143 2022-03-22 13:04:17.606185 fastapi_keycloak-1.0.6/documentation/docs/reference.md
--rw-r--r--   0        0        0     2067 2022-03-22 12:57:41.240604 fastapi_keycloak-1.0.6/documentation/mkdocs.yaml
--rw-r--r--   0        0        0      745 2022-06-16 13:29:16.560647 fastapi_keycloak-1.0.6/fastapi_keycloak/__init__.py
--rw-r--r--   0        0        0    42347 2022-06-16 13:29:04.108133 fastapi_keycloak-1.0.6/fastapi_keycloak/api.py
--rw-r--r--   0        0        0     2235 2022-04-20 10:53:17.932737 fastapi_keycloak-1.0.6/fastapi_keycloak/exceptions.py
--rw-r--r--   0        0        0     5383 2022-06-16 13:29:04.108462 fastapi_keycloak-1.0.6/fastapi_keycloak/model.py
--rw-r--r--   0        0        0      335 2022-04-20 10:53:17.933395 fastapi_keycloak-1.0.6/fastapi_keycloak/requirements.txt
--rw-r--r--   0        0        0     1545 2022-04-20 10:53:17.933569 fastapi_keycloak-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      752 2021-12-22 13:15:56.135150 fastapi_keycloak-1.0.6/requirements.txt
--rw-r--r--   0        0        0       26 2022-04-20 10:53:17.933846 fastapi_keycloak-1.0.6/tests/.coveragerc
--rw-r--r--   0        0        0      469 2022-04-20 10:53:17.933999 fastapi_keycloak-1.0.6/tests/__init__.py
--rw-r--r--   0        0        0     6413 2022-06-16 13:29:04.108623 fastapi_keycloak-1.0.6/tests/app.py
--rwxr-xr-x   0        0        0      170 2022-05-18 19:51:01.948845 fastapi_keycloak-1.0.6/tests/build_keycloak_m1.sh
--rw-r--r--   0        0        0      269 2022-03-25 08:20:51.575556 fastapi_keycloak-1.0.6/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-03-27 19:27:29.214338 fastapi_keycloak-1.0.6/tests/coverage.xml
--rw-r--r--   0        0        0     1086 2022-04-20 10:53:17.934719 fastapi_keycloak-1.0.6/tests/keycloak_postgres.yaml
--rw-r--r--   0        0        0      154 2022-04-20 10:53:17.934920 fastapi_keycloak-1.0.6/tests/pytest.ini
--rw-r--r--   0        0        0    74192 2022-04-20 10:53:17.935288 fastapi_keycloak-1.0.6/tests/realm-export.json
--rwxr-xr-x   0        0        0       47 2022-03-27 19:23:14.661797 fastapi_keycloak-1.0.6/tests/start_infra.sh
--rwxr-xr-x   0        0        0       46 2022-04-20 10:53:17.935538 fastapi_keycloak-1.0.6/tests/stop_infra.sh
--rw-r--r--   0        0        0    15835 2022-04-20 10:53:17.935744 fastapi_keycloak-1.0.6/tests/test_functional.py
--rw-r--r--   0        0        0     2663 2022-06-16 13:29:04.108760 fastapi_keycloak-1.0.6/tests/test_integration.py
--rw-r--r--   0        0        0      414 2022-05-18 19:51:01.949276 fastapi_keycloak-1.0.6/tests/wait_for_service.sh
--rw-r--r--   0        0        0     4324 1970-01-01 00:00:00.000000 fastapi_keycloak-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      711 2022-05-02 21:05:06.860849 fastapi_keycloak-1.0.7/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1298 2022-07-24 08:06:50.800551 fastapi_keycloak-1.0.7/.github/workflows/testing.yaml
+-rw-r--r--   0        0        0     1849 2022-05-02 21:05:06.861048 fastapi_keycloak-1.0.7/.gitignore
+-rw-r--r--   0        0        0    11363 2022-05-02 21:05:06.861163 fastapi_keycloak-1.0.7/LICENSE
+-rw-r--r--   0        0        0     2631 2022-05-18 20:14:24.529104 fastapi_keycloak-1.0.7/README.md
+-rw-r--r--   0        0        0       23 2022-05-02 21:05:06.861308 fastapi_keycloak-1.0.7/codecov.yaml
+-rw-r--r--   0        0        0       36 2022-05-02 21:05:06.861441 fastapi_keycloak-1.0.7/documentation/docs/CNAME
+-rw-r--r--   0        0        0      464 2022-05-02 21:05:06.861508 fastapi_keycloak-1.0.7/documentation/docs/apple-m1.md
+-rw-r--r--   0        0        0      212 2022-05-02 21:05:06.861607 fastapi_keycloak-1.0.7/documentation/docs/css/styles.css
+-rw-r--r--   0        0        0    74518 2022-05-02 21:05:06.862088 fastapi_keycloak-1.0.7/documentation/docs/downloads/realm-export.json
+-rw-r--r--   0        0        0     6411 2022-07-13 20:13:08.995634 fastapi_keycloak-1.0.7/documentation/docs/full_example.md
+-rw-r--r--   0        0        0     1344 2022-05-02 21:05:06.862322 fastapi_keycloak-1.0.7/documentation/docs/img/favicon.svg
+-rw-r--r--   0        0        0     5713 2022-05-02 21:05:06.862420 fastapi_keycloak-1.0.7/documentation/docs/img/logo.png
+-rw-r--r--   0        0        0     2215 2022-05-02 21:05:06.862501 fastapi_keycloak-1.0.7/documentation/docs/index.md
+-rw-r--r--   0        0        0      771 2022-05-02 21:05:06.862575 fastapi_keycloak-1.0.7/documentation/docs/keycloak_configuration.md
+-rw-r--r--   0        0        0     3752 2022-05-02 21:05:06.862659 fastapi_keycloak-1.0.7/documentation/docs/quick_start.md
+-rw-r--r--   0        0        0      143 2022-05-02 21:05:06.862725 fastapi_keycloak-1.0.7/documentation/docs/reference.md
+-rw-r--r--   0        0        0     2067 2022-05-02 21:05:06.862815 fastapi_keycloak-1.0.7/documentation/mkdocs.yaml
+-rw-r--r--   0        0        0      745 2022-07-24 07:54:35.699786 fastapi_keycloak-1.0.7/fastapi_keycloak/__init__.py
+-rw-r--r--   0        0        0    42399 2022-07-24 07:54:35.694829 fastapi_keycloak-1.0.7/fastapi_keycloak/api.py
+-rw-r--r--   0        0        0     2639 2022-07-24 07:54:35.695438 fastapi_keycloak-1.0.7/fastapi_keycloak/exceptions.py
+-rw-r--r--   0        0        0     5617 2022-07-24 07:54:35.695696 fastapi_keycloak-1.0.7/fastapi_keycloak/model.py
+-rw-r--r--   0        0        0      335 2022-05-02 21:05:06.863387 fastapi_keycloak-1.0.7/fastapi_keycloak/requirements.txt
+-rw-r--r--   0        0        0     1545 2022-05-02 21:05:06.863474 fastapi_keycloak-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      752 2022-05-02 21:05:06.863544 fastapi_keycloak-1.0.7/requirements.txt
+-rw-r--r--   0        0        0       26 2022-05-02 21:05:06.863634 fastapi_keycloak-1.0.7/tests/.coveragerc
+-rw-r--r--   0        0        0      469 2022-07-23 20:42:16.669187 fastapi_keycloak-1.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     6413 2022-07-23 20:43:33.110159 fastapi_keycloak-1.0.7/tests/app.py
+-rwxr-xr-x   0        0        0      170 2022-05-18 20:14:24.529678 fastapi_keycloak-1.0.7/tests/build_keycloak_m1.sh
+-rw-r--r--   0        0        0      269 2022-05-02 21:05:06.863934 fastapi_keycloak-1.0.7/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-05-02 21:05:06.863963 fastapi_keycloak-1.0.7/tests/coverage.xml
+-rw-r--r--   0        0        0     1086 2022-05-02 21:05:06.864051 fastapi_keycloak-1.0.7/tests/keycloak_postgres.yaml
+-rw-r--r--   0        0        0      154 2022-07-24 08:06:50.800747 fastapi_keycloak-1.0.7/tests/pytest.ini
+-rw-r--r--   0        0        0    74192 2022-05-02 21:05:06.864236 fastapi_keycloak-1.0.7/tests/realm-export.json
+-rwxr-xr-x   0        0        0       47 2022-05-02 21:05:06.864323 fastapi_keycloak-1.0.7/tests/start_infra.sh
+-rwxr-xr-x   0        0        0       46 2022-05-02 21:05:06.864392 fastapi_keycloak-1.0.7/tests/stop_infra.sh
+-rw-r--r--   0        0        0    16086 2022-07-24 07:54:35.695986 fastapi_keycloak-1.0.7/tests/test_functional.py
+-rw-r--r--   0        0        0     2667 2022-07-24 08:06:50.800941 fastapi_keycloak-1.0.7/tests/test_integration.py
+-rw-r--r--   0        0        0      414 2022-05-18 20:14:24.530097 fastapi_keycloak-1.0.7/tests/wait_for_service.sh
+-rw-r--r--   0        0        0     4324 1970-01-01 00:00:00.000000 fastapi_keycloak-1.0.7/PKG-INFO
```

### Comparing `fastapi_keycloak-1.0.6/.github/FUNDING.yml` & `fastapi_keycloak-1.0.7/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak-1.0.6/.github/workflows/testing.yaml` & `fastapi_keycloak-1.0.7/.github/workflows/testing.yaml`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak-1.0.6/.gitignore` & `fastapi_keycloak-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak-1.0.6/LICENSE` & `fastapi_keycloak-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak-1.0.6/README.md` & `fastapi_keycloak-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak-1.0.6/documentation/docs/downloads/realm-export.json` & `fastapi_keycloak-1.0.7/documentation/docs/downloads/realm-export.json`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak-1.0.6/documentation/docs/full_example.md` & `fastapi_keycloak-1.0.7/documentation/docs/full_example.md`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak-1.0.6/documentation/docs/img/favicon.svg` & `fastapi_keycloak-1.0.7/documentation/docs/img/favicon.svg`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak-1.0.6/documentation/docs/img/logo.png` & `fastapi_keycloak-1.0.7/documentation/docs/img/logo.png`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak-1.0.6/documentation/docs/index.md` & `fastapi_keycloak-1.0.7/documentation/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak-1.0.6/documentation/docs/keycloak_configuration.md` & `fastapi_keycloak-1.0.7/documentation/docs/keycloak_configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak-1.0.6/documentation/docs/quick_start.md` & `fastapi_keycloak-1.0.7/documentation/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak-1.0.6/documentation/mkdocs.yaml` & `fastapi_keycloak-1.0.7/documentation/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak-1.0.6/fastapi_keycloak/__init__.py` & `fastapi_keycloak-1.0.7/fastapi_keycloak/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Keycloak API Client for integrating authentication and authorization with FastAPI"""
 
-__version__ = "1.0.6"
+__version__ = "1.0.7"
 
 from fastapi_keycloak.api import FastAPIKeycloak
 from fastapi_keycloak.model import (HTTPMethod, KeycloakError, KeycloakGroup,
                                     KeycloakIdentityProvider, KeycloakRole,
                                     KeycloakToken, KeycloakUser, OIDCUser,
                                     UsernamePassword)
```

### Comparing `fastapi_keycloak-1.0.6/fastapi_keycloak/api.py` & `fastapi_keycloak-1.0.7/fastapi_keycloak/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import functools
 import json
 from json import JSONDecodeError
-from typing import Any, List, Type, Union
+from typing import Any, Callable, List, Type, Union
 from urllib.parse import urlencode
 
 import requests
 from fastapi import Depends, FastAPI, HTTPException, status
 from fastapi.security import OAuth2PasswordBearer
 from jose import ExpiredSignatureError, JWTError, jwt
 from jose.exceptions import JWTClaimsError
@@ -17,14 +17,15 @@
 from fastapi_keycloak.exceptions import (
     ConfigureTOTPException,
     KeycloakError,
     MandatoryActionException,
     UpdatePasswordException,
     UpdateProfileException,
     UpdateUserLocaleException,
+    UserNotFound,
     VerifyEmailException,
 )
 from fastapi_keycloak.model import (
     HTTPMethod,
     KeycloakGroup,
     KeycloakIdentityProvider,
     KeycloakRole,
@@ -217,24 +218,24 @@
         """Returns the auth scheme to register the endpoints with swagger
 
         Returns:
             OAuth2PasswordBearer: Auth scheme for swagger
         """
         return OAuth2PasswordBearer(tokenUrl=self.token_uri)
 
-    def get_current_user(self, required_roles: List[str] = None, extra_fields: List[str] = None) -> OIDCUser:
+    def get_current_user(self, required_roles: List[str] = None, extra_fields: List[str] = None) -> Callable[OAuth2PasswordBearer, OIDCUser]:
         """Returns the current user based on an access token in the HTTP-header. Optionally verifies roles are possessed
         by the user
 
         Args:
             required_roles List[str]: List of role names required for this endpoint
             extra_fields List[str]: The names of the additional fields you need that are encoded in JWT
 
         Returns:
-            OIDCUser: Decoded JWT content
+            Callable[OAuth2PasswordBearer, OIDCUser]: Dependency method which returns the decoded JWT content
 
         Raises:
             ExpiredSignatureError: If the token is expired (exp > datetime.now())
             JWTError: If decoding fails or the signature is invalid
             JWTClaimsError: If any claim is invalid
             HTTPException: If any role required is not contained within the roles of the users
         """
@@ -255,19 +256,14 @@
                 JWTError: If decoding fails or the signature is invalid
                 JWTClaimsError: If any claim is invalid
                 HTTPException: If any role required is not contained within the roles of the users
             """
             decoded_token = self._decode_token(token=token, audience="account")
             user = OIDCUser.parse_obj(decoded_token)
             if required_roles:
-                if not user.realm_access:  # in cases where there are no roles in realm accessing
-                    raise HTTPException(
-                        status_code=status.HTTP_403_FORBIDDEN,
-                        detail=f"Role(s) {', '.join(required_roles)} is required to perform this action",
-                    )
                 for role in required_roles:
                     if role not in user.roles:
                         raise HTTPException(
                             status_code=status.HTTP_403_FORBIDDEN,
                             detail=f'Role "{role}" is required to perform this action',
                         )
 
@@ -845,14 +841,19 @@
                 url=f"{self.users_uri}?{query}", method=HTTPMethod.GET
             )
             return KeycloakUser(**response.json()[0])
         else:
             response = self._admin_request(
                 url=f"{self.users_uri}/{user_id}", method=HTTPMethod.GET
             )
+            if response.status_code == status.HTTP_404_NOT_FOUND:
+                raise UserNotFound(
+                    status_code = status.HTTP_404_NOT_FOUND,
+                    reason=f"User with user_id[{user_id}] was not found"
+                )
             return KeycloakUser(**response.json())
 
     @result_or_error(response_model=KeycloakUser)
     def update_user(self, user: KeycloakUser):
         """Updates a user. Requires the whole object.
 
         Args:
```

### Comparing `fastapi_keycloak-1.0.6/fastapi_keycloak/exceptions.py` & `fastapi_keycloak-1.0.7/fastapi_keycloak/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,25 @@
     """
 
     def __init__(self, status_code: int, reason: str):
         self.status_code = status_code
         self.reason = reason
         super().__init__(f"HTTP {status_code}: {reason}")
 
+class UserNotFound(Exception):
+    """Thrown when a user lookup fails.
+
+    Attributes:
+        status_code (int): The status code of the response received
+        reason (str): The reason why the requests did fail
+    """
+    def __init__(self, status_code: int, reason: str):
+        self.status_code = status_code
+        self.reason = reason
+        super().__init__(f"HTTP {status_code}: {reason}")
 
 class MandatoryActionException(HTTPException):
     """Throw if the exchange of username and password for an access token fails"""
 
     def __init__(self, detail: str) -> None:
         super().__init__(status_code=400, detail=detail)
```

### Comparing `fastapi_keycloak-1.0.6/fastapi_keycloak/model.py` & `fastapi_keycloak-1.0.7/fastapi_keycloak/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 from typing import List, Optional
 
-from pydantic import BaseModel, SecretStr
+from pydantic import BaseModel, SecretStr, Field
 
 from fastapi_keycloak.exceptions import KeycloakError
 
 
 class HTTPMethod(Enum):
     """Represents the basic HTTP verbs
 
@@ -105,23 +105,28 @@
     name: Optional[str]
     given_name: Optional[str]
     family_name: Optional[str]
     email: Optional[str]
     preferred_username: Optional[str]
     realm_access: Optional[dict]
     resource_access: Optional[dict]
-    extra_fields: Optional[dict]
+    extra_fields: dict = Field(default_factory=dict)
 
     @property
     def roles(self) -> List[str]:
         """Returns the roles of the user
 
         Returns:
             List[str]: If the realm access dict contains roles
         """
+        if not self.realm_access:
+            raise KeycloakError(
+                status_code=404,
+                reason="The 'realm_access' section of the provided access token is missing",
+            )
         try:
             return self.realm_access["roles"]
         except KeyError as e:
             raise KeycloakError(
                 status_code=404,
                 reason="The 'realm_access' section of the provided access token did not contain any 'roles'",
             ) from e
```

### Comparing `fastapi_keycloak-1.0.6/pyproject.toml` & `fastapi_keycloak-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak-1.0.6/requirements.txt` & `fastapi_keycloak-1.0.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak-1.0.6/tests/app.py` & `fastapi_keycloak-1.0.7/tests/app.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak-1.0.6/tests/keycloak_postgres.yaml` & `fastapi_keycloak-1.0.7/tests/keycloak_postgres.yaml`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak-1.0.6/tests/realm-export.json` & `fastapi_keycloak-1.0.7/tests/realm-export.json`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak-1.0.6/tests/test_functional.py` & `fastapi_keycloak-1.0.7/tests/test_functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from fastapi_keycloak import KeycloakError
 from fastapi_keycloak.exceptions import (
     ConfigureTOTPException,
     UpdatePasswordException,
     UpdateProfileException,
     UpdateUserLocaleException,
+    UserNotFound,
     VerifyEmailException,
 )
 from fastapi_keycloak.model import (
     KeycloakGroup,
     KeycloakRole,
     KeycloakToken,
     KeycloakUser,
@@ -441,7 +442,14 @@
         user: KeycloakUser = idp.update_user(user=user)  # Save the change
         assert idp.user_login(
             username=user.username, password=TEST_PASSWORD
         )  # Login possible again
 
         # Clean up
         idp.delete_user(user_id=user.id)
+
+    def test_user_not_found_exception(self, idp):
+
+        with pytest.raises(
+            UserNotFound
+        ):  # Expect the get to fail due to anon existant user
+            u = idp.get_user(user_id="some_non_existant_user_id")
```

### Comparing `fastapi_keycloak-1.0.6/tests/test_integration.py` & `fastapi_keycloak-1.0.7/tests/test_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         assert type(response.json()) == dict
 
     def test_timeout(self, idp):
         timeout = 0.0001
         idp.timeout = timeout
         try:
             idp.proxy(relative_path="/realms/Test", method=HTTPMethod.GET)
-            sleep(timeout)
+            sleep(1.0+timeout)
             assert False
         except ReadTimeout:
             assert True
 
     def test_get_all_roles_and_get_roles(self, idp):
         roles: List[KeycloakRole] = idp.get_all_roles()
         assert roles
```

### Comparing `fastapi_keycloak-1.0.6/PKG-INFO` & `fastapi_keycloak-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_keycloak
-Version: 1.0.6
+Version: 1.0.7
 Summary: Keycloak API Client for integrating authentication and authorization with FastAPI
 Keywords: Keycloak,FastAPI,Authentication,Authorization
 Author-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Maintainer-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
```

