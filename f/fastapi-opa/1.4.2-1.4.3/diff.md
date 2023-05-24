# Comparing `tmp/fastapi-opa-1.4.2.tar.gz` & `tmp/fastapi-opa-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-opa-1.4.2.tar", max compression
+gzip compressed data, was "fastapi-opa-1.4.3.tar", max compression
```

## Comparing `fastapi-opa-1.4.2.tar` & `fastapi-opa-1.4.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2021-09-02 22:01:36.628310 fastapi-opa-1.4.2/LICENSE
--rw-r--r--   0        0        0     7834 2022-12-18 13:54:02.811870 fastapi-opa-1.4.2/README.md
--rw-r--r--   0        0        0      122 2021-09-02 22:01:36.631644 fastapi-opa-1.4.2/fastapi_opa/__init__.py
--rw-r--r--   0        0        0      124 2021-09-02 22:01:36.631644 fastapi-opa-1.4.2/fastapi_opa/auth/__init__.py
--rw-r--r--   0        0        0     1019 2022-12-18 13:54:02.811870 fastapi-opa-1.4.2/fastapi_opa/auth/auth_api_key.py
--rw-r--r--   0        0        0      709 2021-09-02 22:01:36.631644 fastapi-opa-1.4.2/fastapi_opa/auth/auth_interface.py
--rw-r--r--   0        0        0     8788 2022-12-18 13:54:02.811870 fastapi-opa-1.4.2/fastapi_opa/auth/auth_oidc.py
--rw-r--r--   0        0        0     5435 2021-09-02 22:01:36.631644 fastapi-opa-1.4.2/fastapi_opa/auth/auth_saml.py
--rw-r--r--   0        0        0      328 2021-09-02 22:01:36.631644 fastapi-opa-1.4.2/fastapi_opa/auth/exceptions.py
--rw-r--r--   0        0        0        0 2021-09-02 22:01:36.631644 fastapi-opa-1.4.2/fastapi_opa/opa/__init__.py
--rw-r--r--   0        0        0        0 2021-09-02 22:01:36.631644 fastapi-opa-1.4.2/fastapi_opa/opa/enrichment/__init__.py
--rw-r--r--   0        0        0     3771 2022-12-18 13:54:02.811870 fastapi-opa-1.4.2/fastapi_opa/opa/enrichment/graphql_enrichment.py
--rw-r--r--   0        0        0     1107 2022-12-18 13:54:02.811870 fastapi-opa-1.4.2/fastapi_opa/opa/opa_config.py
--rw-r--r--   0        0        0     5458 2022-12-18 13:54:02.811870 fastapi-opa-1.4.2/fastapi_opa/opa/opa_middleware.py
--rw-r--r--   0        0        0     1563 2023-01-02 14:45:05.866551 fastapi-opa-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     9067 2023-01-02 14:47:22.388898 fastapi-opa-1.4.2/setup.py
--rw-r--r--   0        0        0     9018 2023-01-02 14:47:22.389351 fastapi-opa-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-09-02 22:01:36.628310 fastapi-opa-1.4.3/LICENSE
+-rw-r--r--   0        0        0     7438 2023-03-01 05:51:53.140409 fastapi-opa-1.4.3/README.md
+-rw-r--r--   0        0        0      122 2021-09-02 22:01:36.631644 fastapi-opa-1.4.3/fastapi_opa/__init__.py
+-rw-r--r--   0        0        0      124 2021-09-02 22:01:36.631644 fastapi-opa-1.4.3/fastapi_opa/auth/__init__.py
+-rw-r--r--   0        0        0     1019 2022-12-18 13:54:02.811870 fastapi-opa-1.4.3/fastapi_opa/auth/auth_api_key.py
+-rw-r--r--   0        0        0      709 2021-09-02 22:01:36.631644 fastapi-opa-1.4.3/fastapi_opa/auth/auth_interface.py
+-rw-r--r--   0        0        0     8788 2022-12-18 13:54:02.811870 fastapi-opa-1.4.3/fastapi_opa/auth/auth_oidc.py
+-rw-r--r--   0        0        0     5433 2023-03-01 06:30:47.831112 fastapi-opa-1.4.3/fastapi_opa/auth/auth_saml.py
+-rw-r--r--   0        0        0      328 2021-09-02 22:01:36.631644 fastapi-opa-1.4.3/fastapi_opa/auth/exceptions.py
+-rw-r--r--   0        0        0        0 2021-09-02 22:01:36.631644 fastapi-opa-1.4.3/fastapi_opa/opa/__init__.py
+-rw-r--r--   0        0        0        0 2021-09-02 22:01:36.631644 fastapi-opa-1.4.3/fastapi_opa/opa/enrichment/__init__.py
+-rw-r--r--   0        0        0     3771 2022-12-18 13:54:02.811870 fastapi-opa-1.4.3/fastapi_opa/opa/enrichment/graphql_enrichment.py
+-rw-r--r--   0        0        0     1107 2022-12-18 13:54:02.811870 fastapi-opa-1.4.3/fastapi_opa/opa/opa_config.py
+-rw-r--r--   0        0        0     5457 2023-03-01 06:30:47.831112 fastapi-opa-1.4.3/fastapi_opa/opa/opa_middleware.py
+-rw-r--r--   0        0        0     1438 2023-03-01 06:30:47.831112 fastapi-opa-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     8637 2023-03-01 06:30:59.721123 fastapi-opa-1.4.3/setup.py
+-rw-r--r--   0        0        0     8562 2023-03-01 06:30:59.723420 fastapi-opa-1.4.3/PKG-INFO
```

### Comparing `fastapi-opa-1.4.2/LICENSE` & `fastapi-opa-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-opa-1.4.2/README.md` & `fastapi-opa-1.4.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,56 @@
-# Open Policy Agent Middleware for FastAPI
+Metadata-Version: 2.1
+Name: fastapi-opa
+Version: 1.4.3
+Summary: Fastapi OPA middleware incl. auth flow.
+Home-page: https://github.com/busykoala/fastapi-opa
+License: GPL-3.0-or-later
+Keywords: fastapi,oidc,authentication,authorization,saml
+Author: Matthias Osswald
+Author-email: info@busykoala.io
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: graphql
+Provides-Extra: saml
+Requires-Dist: PyJWT[crypto] (>=2.4)
+Requires-Dist: fastapi (>=0.65.2)
+Requires-Dist: graphene (>=2,<3); extra == "graphql"
+Requires-Dist: importlib-metadata (<5.0)
+Requires-Dist: itsdangerous
+Requires-Dist: python-multipart; extra == "saml"
+Requires-Dist: python3-saml; extra == "saml"
+Requires-Dist: requests
+Project-URL: Repository, https://github.com/busykoala/fastapi-opa
+Description-Content-Type: text/markdown
 
-## Table of Contents
+# Open Policy Agent middleware for FastAPI
+
+## Table of contents
 - [Contributors](#contributors)
 - [What does fastapi-opa do](#about)
 - [Installation](#installation)
 - [How to get started](#getting-started)
 - [Open Policy Agent](#opa)
-- [Authentication Flow](#auth-flow)
-  - [API Key Authentication](#api-key-auth)
-  - [OIDC Authentication](#oidc-auth)
-  - [SAML Authentication](#saml-auth)
-- [Custom Payload Enrichment](#custom-payload-enrichment)
-  - [Graphql Enrichment](#gql-enrichment)
+- [Authentication flow](#auth-flow)
+  - [API key authentication](#api-key-auth)
+  - [OIDC authentication](#oidc-auth)
+  - [SAML authentication](#saml-auth)
+- [Custom payload enrichment](#custom-payload-enrichment)
+  - [GraphQL enrichment](#gql-enrichment)
 
 <a name="contributors"/>
 
 ## Contributors
 
-Thanks to all our contributors! There is no specific order and hopefully nobody was left out.
+Thanks to all the contributors below. Furthermore thanks for raising issues.
 
 <a href="https://github.com/morestanna">
   <img src="https://avatars.githubusercontent.com/morestanna" width="60" height="60" />
 </a>
 <a href="https://github.com/busykoala">
   <img src="https://avatars.githubusercontent.com/busykoala" width="60" height="60" />
 </a>
@@ -35,53 +64,50 @@
   <img src="https://avatars.githubusercontent.com/ejsyx" width="60" height="60" />
 </a>
 
 <a name="about"/>
 
 ## What does fastapi-opa do
 
-`fastapi-opa` is an extension to FastAPI that allows you to add a login flow
-to your application within minutes using open policy agent and your favourite
-identity provider.
+The FastAPI extension `fastapi-opa` allows to add login flows and integrates
+Open Policy Agent to your app.
 
 ![Flow Diagram](https://raw.githubusercontent.com/busykoala/fastapi-opa/master/assets/diagram.png)
 
-When a user tries to get a response from an endpoint he/she will be redirected
-to the identity provider for authorization.
-After the authentication the app validates the token provided. Once it was
-validated the user information is used to get an OPA decision whether
-the user is allowed to get any information from the endpoint.
+The middleware redirects the request to the identity provider. After the
+authentication it validates the token. Using the token, Open Policy Agent
+decides if the response has success or failure status.
 
 <a name="installation"/>
 
 ## Installation
 
 ```bash
 poetry add [--extras "graphql"] [--extras "saml"] fastapi-opa 
 ```
 
 <a name="getting-started"/>
 
 ## How to get started
 
-:bulb: Checkout the wiki for a complete environment setup with Keycloak and Open Policy Agent:  
+:bulb: checkout the wiki for an environment setup with Keycloak and Open Policy Agent:  
 [Getting Started with FastAPI app with Authentication and Authorization](https://github.com/busykoala/fastapi-opa/wiki#dev-setup)
 
-The package provides a very easy way to integrate authentication and
-authorization. We can decide what authentication flow we inject into the
-OPAMiddleware to be able choosing between different flows.
-
-There are 
- - one example for oidc : fastapi_opa.example_oidc.py,
- - one example for saml: fastapi_opa.example_saml.py
+The package combines authentication and authorization with FastAPI. You can
+customize the `OPAMiddleware` depending on your authentication flow.
+
+Check out these examples for the most common flows:
+- OIDC: `fastapi_opa.example_oidc.py`
+- SAML: `fastapi_opa.example_saml.py`
 
 ## Open Policy Agent
 
-The (validated/authenticated) user token is sent to the Open Policy Agent
-with the additional attributes `request_method` and `request_path`.
+The middleware sends the validated and authenticated user token to Open
+Policy Agent. It adds the extra attributes `request_method` and
+`request_path`.
 
 ```json
 {
     "input": {
         "exp": 1617466243,
         "iat": 1617465943,
         "auth_time": 1617465663,
@@ -101,19 +127,20 @@
         "subordinates": [],
         "request_method": "GET",
         "request_path": ["finance", "salary", "david"]
     }
 }
 ```
 
-In open policy agent you can now easily create policies using user roles,
-routes, or request methods etc.
+In Open Policy Agent you can create policies using user roles,
+routes, request methods etc.
 
-An example policy (from [the official OPA docs](https://www.openpolicyagent.org/docs/v0.11.0/http-api-authorization/))
-for this setup could be like:
+An example policy (from [the official Open Policy Agent
+docs](https://www.openpolicyagent.org/docs/v0.11.0/http-api-authorization/))
+for this setup could look like this:
 
 ```rego
 package httpapi.authz
 
 # bob is alice's manager, and betty is charlie's.
 subordinates = {"alice": [], "charlie": [], "bob": ["alice"], "betty": ["charlie"]}
 
@@ -137,57 +164,58 @@
   input.request_path = ["finance", "salary", username]
   subordinates[input.user][_] == username
 }
 ```
 
 <a name="auth-flow"/>
 
-## Authentication Flow
+## Authentication flow
 
-There is an interface provided to easily implement the desired authentication
-flow and inject it into OPAMiddleware
-(`fastapi_opa.auth.auth_interface.AuthInterface`), or you can open a pull
-request if you would like to contribute to the package.
+Use the provided interface to set up your desired authentication flow. Then
+insert it into `OPAMiddleware` (`fastapi_opa.auth.auth_interface.AuthInterface`).
+Consider submitting a pull request with new flows.
 
-Also there are implementations ready to use.
+You can also use these ready-to-go implementations:
 
 <a name="api-key-auth"/>
 
-### API Key Authentication
+### API key authentication
+
+In the API key authentication a request header needs to match a given value.
 
-The API key authentication is the simplest authentication system where you simply needs to match
-a given value in the request header:
 ```python
 # Configure API keys
 api_key_config = APIKeyConfig(
     header_key="test",
     api_key="1234"
 )
 api_key_auth = APIKeyAuthentication(api_key_config)
 ```
-Here sending a request with the `header["test"] = "1234"` would be considered as a successful authentication.
-For OPA, the user is `APIKey` and the variable `client` is set with the client address.
+
+In the example the header `header["test"] = "1234"` authenticates the request.
+For Open Policy Agent, set user to `APIKey` and the variable `client` to the
+client address.
 
 <a name="oidc-auth"/>
 
-### OIDC Authentication
+### OIDC authentication
 
 The example in [How to get started](#getting-started) provides an example for
 the implementation of the OIDC Authentication.
 
 <a name="saml-auth"/>
 
-### SAML Authentication
+### SAML authentication
 
 For the saml implementation create your certs using
 `openssl req -new -x509 -days 3652 -nodes -out sp.crt -keyout sp.key` and
 add the keys to the sp section of your `settings.json`. Checkout the test
-settings to get an idea (`tests/test_data/saml/*.json`). The path to your
-own `settings.json` and `advanced_settings.json` has to be provided in the
-`SAMLAuthConfig` like in the example below (do not use the test data in
+settings to get an idea (`tests/test_data/saml/*.json`).
+Provide the path to your own `settings.json` and `advanced_settings.json`
+in the `SAMLAuthConfig` like in the example below (don't use the test data in
 production).
 
 ```python
 from fastapi_opa import OPAConfig
 from fastapi_opa.auth.auth_saml import SAMLAuthentication
 from fastapi_opa.auth.auth_saml import SAMLConfig
 
@@ -196,51 +224,50 @@
 saml_config = SAMLConfig(settings_directory="./tests/test_data/saml")
 saml_auth = SAMLAuthentication(saml_config)
 
 opa_config = OPAConfig(authentication=saml_auth, opa_host=opa_host,
                        accepted_methods=["id_token", "access_token"])
 ```
 
-The cert has to be uploaded to your identity provider. Using Keycloak as an
-idp you need to configure `encrypt assertion`, `client signature required`,
-`force POST bindings` on creating the client.
+Upload the certificate to your identity provider. Using Keycloak as an
+identity provider you need to configure `encrypt assertion`,
+`client signature required`, `force POST bindings` on creating the client.
 Also configure: `Client Scopes` -> `role_list (saml)` -> `Mappers tab` ->
 `role list` -> `Single Role Attribute`
 
 <a name="custom-payload-enrichment"/>
 
-## Custom Payload Enrichment
+## Custom payload enrichment
 
-In `fastapi_opa.opa.opa_config.Injectable` an interface is provided to add
-more information to the payload sent to OPA.
+Use the interface `fastapi_opa.opa.opa_config.Injectable` to add
+more information to the payload sent to Open Policy Agent.
 
-The injectables can be added to the `OPAConfig`. Let's look at an example:
+Configure the injectables in the `OPAConfig`:
 
 ```python
 class FancyInjectable(Injectable):
     async def extract(self, request: Request) -> List:
         return ["some", "custom", "stuff"]
 
 fancy_inj = FancyInjectable("fancy_key", skip_endpoints=["/health", "/api/[^/]*/test])
 
 opa_config = OPAConfig(
     authentication=oidc_auth, opa_host=opa_host, injectables=[fancy_inj]
 )
 ```
 
-With `skip_endpoints`, you can define some endpoints where the injectable
-will not be applied. The endpoints can be defined either directly or through some
-regex.
-
+Use `skip_endpoints` to choose which endpoints the injectable shouldn't affect.
+To define an endpoint, specify an exact string or a regular expression.
 
 <a name="gql-enrichment"/>
 
-### Graphql Enrichment
+### GraphQL enrichment
 
-For GraphQL there is a ready to use injectable:
+For GraphQL you can use the ready to go injectable:
 
 ```python
 from fastapi_opa.opa.enrichment.graphql_enrichment import GraphQLInjectable`
 
 graphql = GraphQLInjectable("gql_injectable")
 opa_config = OPAConfig(authentication=oidc_auth, opa_host=opa_host, injectables=[graphql])
 ```
+
```

### Comparing `fastapi-opa-1.4.2/fastapi_opa/auth/auth_api_key.py` & `fastapi-opa-1.4.3/fastapi_opa/auth/auth_api_key.py`

 * *Files identical despite different names*

### Comparing `fastapi-opa-1.4.2/fastapi_opa/auth/auth_interface.py` & `fastapi-opa-1.4.3/fastapi_opa/auth/auth_interface.py`

 * *Files identical despite different names*

### Comparing `fastapi-opa-1.4.2/fastapi_opa/auth/auth_oidc.py` & `fastapi-opa-1.4.3/fastapi_opa/auth/auth_oidc.py`

 * *Files identical despite different names*

### Comparing `fastapi-opa-1.4.2/fastapi_opa/auth/auth_saml.py` & `fastapi-opa-1.4.3/fastapi_opa/auth/auth_saml.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,16 @@
         elif "sso2" in request.query_params:
             logger.debug("--sso2--")
             return_to = "%sattrs/" % request.base_url
             return await self.single_sign_on(auth, return_to)
 
         elif "acs" in request.query_params:
             logger.debug("--acs--")
-            return await (
-                self.assertion_consumer_service(auth, request_args, request)
+            return await self.assertion_consumer_service(
+                auth, request_args, request
             )
 
         elif "slo" in request.query_params:
             logger.debug("--slo--")
             return await self.single_log_out(auth)
 
         elif "sls" in request.query_params:
```

### Comparing `fastapi-opa-1.4.2/fastapi_opa/opa/enrichment/graphql_enrichment.py` & `fastapi-opa-1.4.3/fastapi_opa/opa/enrichment/graphql_enrichment.py`

 * *Files identical despite different names*

### Comparing `fastapi-opa-1.4.2/fastapi_opa/opa/opa_config.py` & `fastapi-opa-1.4.3/fastapi_opa/opa/opa_config.py`

 * *Files identical despite different names*

### Comparing `fastapi-opa-1.4.2/fastapi_opa/opa/opa_middleware.py` & `fastapi-opa-1.4.3/fastapi_opa/opa/opa_middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,14 @@
         self.config = config
         self.app = app
         self.skip_endpoints = [re.compile(skip) for skip in skip_endpoints]
 
     async def __call__(
         self, scope: Scope, receive: Receive, send: Send
     ) -> None:
-
         if scope["type"] == "lifespan":
             return await self.app(scope, receive, send)
 
         # Small hack to ensure that later we can still receive the body
         own_receive = OwnReceive(receive)
         request = Request(scope, own_receive, send)
```

### Comparing `fastapi-opa-1.4.2/pyproject.toml` & `fastapi-opa-1.4.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "fastapi-opa"
-version = "1.4.2"
+version = "1.4.3"
 description = "Fastapi OPA middleware incl. auth flow."
-authors = ["Matthias Osswald <m@osswald.li>"]
+authors = ["Matthias Osswald <info@busykoala.io>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/busykoala/fastapi-opa"
 keywords = ["fastapi", "oidc", "authentication", "authorization", "saml"]
 exclude = ["fastapi_opa/example_oidc.py", "fastapi_opa/example_saml.py"]
 
 [tool.poetry.dependencies]
@@ -15,16 +15,14 @@
 itsdangerous = "*"
 requests = "*"
 PyJWT = {extras = ["crypto"], version = ">= 2.4"}
 graphene = {version = "^2", optional = true}
 python3-saml = {version = "*", optional = true}
 python-multipart = {version = "*", optional = true}
 # transitive overrides
-lxml = ">= 4.9.1"  # https://github.com/advisories/GHSA-wrxv-2j5q-m38w
-gitpython = "> 3.1.29"  # https://github.com/advisories/GHSA-hcpj-qp55-gfph
 importlib-metadata = "< 5.0"  # https://importlib-metadata.readthedocs.io/en/latest/history.html
 
 
 [tool.poetry.dev-dependencies]
 flake9 = "*"
 black = "*"
 isort = "*"
@@ -33,14 +31,15 @@
 pytest-mock = "*"
 mock = "*"
 freezegun = "*"
 Authlib = "*"
 pytest-asyncio = "*"
 nest-asyncio = "*"
 httpx = "*"
+vale = "^2.20.2"
 
 [tool.poetry.extras]
 graphql = ["graphene"]
 saml = ["python3-saml", "python-multipart"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `fastapi-opa-1.4.2/setup.py` & `fastapi-opa-1.4.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,30 +9,28 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyJWT[crypto]>=2.4',
  'fastapi>=0.65.2',
- 'gitpython>3.1.29',
  'importlib-metadata<5.0',
  'itsdangerous',
- 'lxml>=4.9.1',
  'requests']
 
 extras_require = \
 {'graphql': ['graphene>=2,<3'], 'saml': ['python3-saml', 'python-multipart']}
 
 setup_kwargs = {
     'name': 'fastapi-opa',
-    'version': '1.4.2',
+    'version': '1.4.3',
     'description': 'Fastapi OPA middleware incl. auth flow.',
-    'long_description': '# Open Policy Agent Middleware for FastAPI\n\n## Table of Contents\n- [Contributors](#contributors)\n- [What does fastapi-opa do](#about)\n- [Installation](#installation)\n- [How to get started](#getting-started)\n- [Open Policy Agent](#opa)\n- [Authentication Flow](#auth-flow)\n  - [API Key Authentication](#api-key-auth)\n  - [OIDC Authentication](#oidc-auth)\n  - [SAML Authentication](#saml-auth)\n- [Custom Payload Enrichment](#custom-payload-enrichment)\n  - [Graphql Enrichment](#gql-enrichment)\n\n<a name="contributors"/>\n\n## Contributors\n\nThanks to all our contributors! There is no specific order and hopefully nobody was left out.\n\n<a href="https://github.com/morestanna">\n  <img src="https://avatars.githubusercontent.com/morestanna" width="60" height="60" />\n</a>\n<a href="https://github.com/busykoala">\n  <img src="https://avatars.githubusercontent.com/busykoala" width="60" height="60" />\n</a>\n<a href="https://github.com/TracyWR">\n  <img src="https://avatars.githubusercontent.com/TracyWR" width="60" height="60" />\n</a>\n<a href="https://github.com/loikki">\n  <img src="https://avatars.githubusercontent.com/loikki" width="60" height="60" />\n</a>\n<a href="https://github.com/ejsyx">\n  <img src="https://avatars.githubusercontent.com/ejsyx" width="60" height="60" />\n</a>\n\n<a name="about"/>\n\n## What does fastapi-opa do\n\n`fastapi-opa` is an extension to FastAPI that allows you to add a login flow\nto your application within minutes using open policy agent and your favourite\nidentity provider.\n\n![Flow Diagram](https://raw.githubusercontent.com/busykoala/fastapi-opa/master/assets/diagram.png)\n\nWhen a user tries to get a response from an endpoint he/she will be redirected\nto the identity provider for authorization.\nAfter the authentication the app validates the token provided. Once it was\nvalidated the user information is used to get an OPA decision whether\nthe user is allowed to get any information from the endpoint.\n\n<a name="installation"/>\n\n## Installation\n\n```bash\npoetry add [--extras "graphql"] [--extras "saml"] fastapi-opa \n```\n\n<a name="getting-started"/>\n\n## How to get started\n\n:bulb: Checkout the wiki for a complete environment setup with Keycloak and Open Policy Agent:  \n[Getting Started with FastAPI app with Authentication and Authorization](https://github.com/busykoala/fastapi-opa/wiki#dev-setup)\n\nThe package provides a very easy way to integrate authentication and\nauthorization. We can decide what authentication flow we inject into the\nOPAMiddleware to be able choosing between different flows.\n\nThere are \n - one example for oidc : fastapi_opa.example_oidc.py,\n - one example for saml: fastapi_opa.example_saml.py\n\n## Open Policy Agent\n\nThe (validated/authenticated) user token is sent to the Open Policy Agent\nwith the additional attributes `request_method` and `request_path`.\n\n```json\n{\n    "input": {\n        "exp": 1617466243,\n        "iat": 1617465943,\n        "auth_time": 1617465663,\n        "jti": "9aacb638-70c6-4f0a-b0c8-dbc67f92e3d1",\n        "iss": "http://localhost:8080/auth/realms/example-realm",\n        "aud": "example-client",\n        "sub": "ccf78dc0-e1d6-4606-99d4-9009e74e3ab4",\n        "typ": "ID",\n        "azp": "david",\n        "session_state": "41640fe7-39d2-44bc-818c-a3360b36fb87",\n        "at_hash": "2IGw-B9f5910Sll1tnfQRg",\n        "acr": "0",\n        "email_verified": false,\n        "hr": "true",\n        "preferred_username": "david",\n        "user": "david",\n        "subordinates": [],\n        "request_method": "GET",\n        "request_path": ["finance", "salary", "david"]\n    }\n}\n```\n\nIn open policy agent you can now easily create policies using user roles,\nroutes, or request methods etc.\n\nAn example policy (from [the official OPA docs](https://www.openpolicyagent.org/docs/v0.11.0/http-api-authorization/))\nfor this setup could be like:\n\n```rego\npackage httpapi.authz\n\n# bob is alice\'s manager, and betty is charlie\'s.\nsubordinates = {"alice": [], "charlie": [], "bob": ["alice"], "betty": ["charlie"]}\n\n# HTTP API request\nimport input\n\ndefault allow = false\n\n# Allow users to get their own salaries.\nallow {\n  some username\n  input.request_method == "GET"\n  input.request_path = ["finance", "salary", username]\n  input.user == username\n}\n\n# Allow managers to get their subordinates\' salaries.\nallow {\n  some username\n  input.request_method == "GET"\n  input.request_path = ["finance", "salary", username]\n  subordinates[input.user][_] == username\n}\n```\n\n<a name="auth-flow"/>\n\n## Authentication Flow\n\nThere is an interface provided to easily implement the desired authentication\nflow and inject it into OPAMiddleware\n(`fastapi_opa.auth.auth_interface.AuthInterface`), or you can open a pull\nrequest if you would like to contribute to the package.\n\nAlso there are implementations ready to use.\n\n<a name="api-key-auth"/>\n\n### API Key Authentication\n\nThe API key authentication is the simplest authentication system where you simply needs to match\na given value in the request header:\n```python\n# Configure API keys\napi_key_config = APIKeyConfig(\n    header_key="test",\n    api_key="1234"\n)\napi_key_auth = APIKeyAuthentication(api_key_config)\n```\nHere sending a request with the `header["test"] = "1234"` would be considered as a successful authentication.\nFor OPA, the user is `APIKey` and the variable `client` is set with the client address.\n\n<a name="oidc-auth"/>\n\n### OIDC Authentication\n\nThe example in [How to get started](#getting-started) provides an example for\nthe implementation of the OIDC Authentication.\n\n<a name="saml-auth"/>\n\n### SAML Authentication\n\nFor the saml implementation create your certs using\n`openssl req -new -x509 -days 3652 -nodes -out sp.crt -keyout sp.key` and\nadd the keys to the sp section of your `settings.json`. Checkout the test\nsettings to get an idea (`tests/test_data/saml/*.json`). The path to your\nown `settings.json` and `advanced_settings.json` has to be provided in the\n`SAMLAuthConfig` like in the example below (do not use the test data in\nproduction).\n\n```python\nfrom fastapi_opa import OPAConfig\nfrom fastapi_opa.auth.auth_saml import SAMLAuthentication\nfrom fastapi_opa.auth.auth_saml import SAMLConfig\n\nopa_host = "http://localhost:8181"\n\nsaml_config = SAMLConfig(settings_directory="./tests/test_data/saml")\nsaml_auth = SAMLAuthentication(saml_config)\n\nopa_config = OPAConfig(authentication=saml_auth, opa_host=opa_host,\n                       accepted_methods=["id_token", "access_token"])\n```\n\nThe cert has to be uploaded to your identity provider. Using Keycloak as an\nidp you need to configure `encrypt assertion`, `client signature required`,\n`force POST bindings` on creating the client.\nAlso configure: `Client Scopes` -> `role_list (saml)` -> `Mappers tab` ->\n`role list` -> `Single Role Attribute`\n\n<a name="custom-payload-enrichment"/>\n\n## Custom Payload Enrichment\n\nIn `fastapi_opa.opa.opa_config.Injectable` an interface is provided to add\nmore information to the payload sent to OPA.\n\nThe injectables can be added to the `OPAConfig`. Let\'s look at an example:\n\n```python\nclass FancyInjectable(Injectable):\n    async def extract(self, request: Request) -> List:\n        return ["some", "custom", "stuff"]\n\nfancy_inj = FancyInjectable("fancy_key", skip_endpoints=["/health", "/api/[^/]*/test])\n\nopa_config = OPAConfig(\n    authentication=oidc_auth, opa_host=opa_host, injectables=[fancy_inj]\n)\n```\n\nWith `skip_endpoints`, you can define some endpoints where the injectable\nwill not be applied. The endpoints can be defined either directly or through some\nregex.\n\n\n<a name="gql-enrichment"/>\n\n### Graphql Enrichment\n\nFor GraphQL there is a ready to use injectable:\n\n```python\nfrom fastapi_opa.opa.enrichment.graphql_enrichment import GraphQLInjectable`\n\ngraphql = GraphQLInjectable("gql_injectable")\nopa_config = OPAConfig(authentication=oidc_auth, opa_host=opa_host, injectables=[graphql])\n```\n',
+    'long_description': '# Open Policy Agent middleware for FastAPI\n\n## Table of contents\n- [Contributors](#contributors)\n- [What does fastapi-opa do](#about)\n- [Installation](#installation)\n- [How to get started](#getting-started)\n- [Open Policy Agent](#opa)\n- [Authentication flow](#auth-flow)\n  - [API key authentication](#api-key-auth)\n  - [OIDC authentication](#oidc-auth)\n  - [SAML authentication](#saml-auth)\n- [Custom payload enrichment](#custom-payload-enrichment)\n  - [GraphQL enrichment](#gql-enrichment)\n\n<a name="contributors"/>\n\n## Contributors\n\nThanks to all the contributors below. Furthermore thanks for raising issues.\n\n<a href="https://github.com/morestanna">\n  <img src="https://avatars.githubusercontent.com/morestanna" width="60" height="60" />\n</a>\n<a href="https://github.com/busykoala">\n  <img src="https://avatars.githubusercontent.com/busykoala" width="60" height="60" />\n</a>\n<a href="https://github.com/TracyWR">\n  <img src="https://avatars.githubusercontent.com/TracyWR" width="60" height="60" />\n</a>\n<a href="https://github.com/loikki">\n  <img src="https://avatars.githubusercontent.com/loikki" width="60" height="60" />\n</a>\n<a href="https://github.com/ejsyx">\n  <img src="https://avatars.githubusercontent.com/ejsyx" width="60" height="60" />\n</a>\n\n<a name="about"/>\n\n## What does fastapi-opa do\n\nThe FastAPI extension `fastapi-opa` allows to add login flows and integrates\nOpen Policy Agent to your app.\n\n![Flow Diagram](https://raw.githubusercontent.com/busykoala/fastapi-opa/master/assets/diagram.png)\n\nThe middleware redirects the request to the identity provider. After the\nauthentication it validates the token. Using the token, Open Policy Agent\ndecides if the response has success or failure status.\n\n<a name="installation"/>\n\n## Installation\n\n```bash\npoetry add [--extras "graphql"] [--extras "saml"] fastapi-opa \n```\n\n<a name="getting-started"/>\n\n## How to get started\n\n:bulb: checkout the wiki for an environment setup with Keycloak and Open Policy Agent:  \n[Getting Started with FastAPI app with Authentication and Authorization](https://github.com/busykoala/fastapi-opa/wiki#dev-setup)\n\nThe package combines authentication and authorization with FastAPI. You can\ncustomize the `OPAMiddleware` depending on your authentication flow.\n\nCheck out these examples for the most common flows:\n- OIDC: `fastapi_opa.example_oidc.py`\n- SAML: `fastapi_opa.example_saml.py`\n\n## Open Policy Agent\n\nThe middleware sends the validated and authenticated user token to Open\nPolicy Agent. It adds the extra attributes `request_method` and\n`request_path`.\n\n```json\n{\n    "input": {\n        "exp": 1617466243,\n        "iat": 1617465943,\n        "auth_time": 1617465663,\n        "jti": "9aacb638-70c6-4f0a-b0c8-dbc67f92e3d1",\n        "iss": "http://localhost:8080/auth/realms/example-realm",\n        "aud": "example-client",\n        "sub": "ccf78dc0-e1d6-4606-99d4-9009e74e3ab4",\n        "typ": "ID",\n        "azp": "david",\n        "session_state": "41640fe7-39d2-44bc-818c-a3360b36fb87",\n        "at_hash": "2IGw-B9f5910Sll1tnfQRg",\n        "acr": "0",\n        "email_verified": false,\n        "hr": "true",\n        "preferred_username": "david",\n        "user": "david",\n        "subordinates": [],\n        "request_method": "GET",\n        "request_path": ["finance", "salary", "david"]\n    }\n}\n```\n\nIn Open Policy Agent you can create policies using user roles,\nroutes, request methods etc.\n\nAn example policy (from [the official Open Policy Agent\ndocs](https://www.openpolicyagent.org/docs/v0.11.0/http-api-authorization/))\nfor this setup could look like this:\n\n```rego\npackage httpapi.authz\n\n# bob is alice\'s manager, and betty is charlie\'s.\nsubordinates = {"alice": [], "charlie": [], "bob": ["alice"], "betty": ["charlie"]}\n\n# HTTP API request\nimport input\n\ndefault allow = false\n\n# Allow users to get their own salaries.\nallow {\n  some username\n  input.request_method == "GET"\n  input.request_path = ["finance", "salary", username]\n  input.user == username\n}\n\n# Allow managers to get their subordinates\' salaries.\nallow {\n  some username\n  input.request_method == "GET"\n  input.request_path = ["finance", "salary", username]\n  subordinates[input.user][_] == username\n}\n```\n\n<a name="auth-flow"/>\n\n## Authentication flow\n\nUse the provided interface to set up your desired authentication flow. Then\ninsert it into `OPAMiddleware` (`fastapi_opa.auth.auth_interface.AuthInterface`).\nConsider submitting a pull request with new flows.\n\nYou can also use these ready-to-go implementations:\n\n<a name="api-key-auth"/>\n\n### API key authentication\n\nIn the API key authentication a request header needs to match a given value.\n\n```python\n# Configure API keys\napi_key_config = APIKeyConfig(\n    header_key="test",\n    api_key="1234"\n)\napi_key_auth = APIKeyAuthentication(api_key_config)\n```\n\nIn the example the header `header["test"] = "1234"` authenticates the request.\nFor Open Policy Agent, set user to `APIKey` and the variable `client` to the\nclient address.\n\n<a name="oidc-auth"/>\n\n### OIDC authentication\n\nThe example in [How to get started](#getting-started) provides an example for\nthe implementation of the OIDC Authentication.\n\n<a name="saml-auth"/>\n\n### SAML authentication\n\nFor the saml implementation create your certs using\n`openssl req -new -x509 -days 3652 -nodes -out sp.crt -keyout sp.key` and\nadd the keys to the sp section of your `settings.json`. Checkout the test\nsettings to get an idea (`tests/test_data/saml/*.json`).\nProvide the path to your own `settings.json` and `advanced_settings.json`\nin the `SAMLAuthConfig` like in the example below (don\'t use the test data in\nproduction).\n\n```python\nfrom fastapi_opa import OPAConfig\nfrom fastapi_opa.auth.auth_saml import SAMLAuthentication\nfrom fastapi_opa.auth.auth_saml import SAMLConfig\n\nopa_host = "http://localhost:8181"\n\nsaml_config = SAMLConfig(settings_directory="./tests/test_data/saml")\nsaml_auth = SAMLAuthentication(saml_config)\n\nopa_config = OPAConfig(authentication=saml_auth, opa_host=opa_host,\n                       accepted_methods=["id_token", "access_token"])\n```\n\nUpload the certificate to your identity provider. Using Keycloak as an\nidentity provider you need to configure `encrypt assertion`,\n`client signature required`, `force POST bindings` on creating the client.\nAlso configure: `Client Scopes` -> `role_list (saml)` -> `Mappers tab` ->\n`role list` -> `Single Role Attribute`\n\n<a name="custom-payload-enrichment"/>\n\n## Custom payload enrichment\n\nUse the interface `fastapi_opa.opa.opa_config.Injectable` to add\nmore information to the payload sent to Open Policy Agent.\n\nConfigure the injectables in the `OPAConfig`:\n\n```python\nclass FancyInjectable(Injectable):\n    async def extract(self, request: Request) -> List:\n        return ["some", "custom", "stuff"]\n\nfancy_inj = FancyInjectable("fancy_key", skip_endpoints=["/health", "/api/[^/]*/test])\n\nopa_config = OPAConfig(\n    authentication=oidc_auth, opa_host=opa_host, injectables=[fancy_inj]\n)\n```\n\nUse `skip_endpoints` to choose which endpoints the injectable shouldn\'t affect.\nTo define an endpoint, specify an exact string or a regular expression.\n\n<a name="gql-enrichment"/>\n\n### GraphQL enrichment\n\nFor GraphQL you can use the ready to go injectable:\n\n```python\nfrom fastapi_opa.opa.enrichment.graphql_enrichment import GraphQLInjectable`\n\ngraphql = GraphQLInjectable("gql_injectable")\nopa_config = OPAConfig(authentication=oidc_auth, opa_host=opa_host, injectables=[graphql])\n```\n',
     'author': 'Matthias Osswald',
-    'author_email': 'm@osswald.li',
+    'author_email': 'info@busykoala.io',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/busykoala/fastapi-opa',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
```

#### html2text {}

```diff
@@ -1,113 +1,109 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['fastapi_opa', 'fastapi_opa.auth', 'fastapi_opa.opa',
 'fastapi_opa.opa.enrichment'] package_data = \ {'': ['*']} install_requires = \
-['PyJWT[crypto]>=2.4', 'fastapi>=0.65.2', 'gitpython>3.1.29', 'importlib-
-metadata<5.0', 'itsdangerous', 'lxml>=4.9.1', 'requests'] extras_require = \
-{'graphql': ['graphene>=2,<3'], 'saml': ['python3-saml', 'python-multipart']}
-setup_kwargs = { 'name': 'fastapi-opa', 'version': '1.4.2', 'description':
-'Fastapi OPA middleware incl. auth flow.', 'long_description': '# Open Policy
-Agent Middleware for FastAPI\n\n## Table of Contents\n- [Contributors]
-(#contributors)\n- [What does fastapi-opa do](#about)\n- [Installation]
-(#installation)\n- [How to get started](#getting-started)\n- [Open Policy
-Agent](#opa)\n- [Authentication Flow](#auth-flow)\n - [API Key Authentication]
-(#api-key-auth)\n - [OIDC Authentication](#oidc-auth)\n - [SAML Authentication]
-(#saml-auth)\n- [Custom Payload Enrichment](#custom-payload-enrichment)\n -
-[Graphql Enrichment](#gql-enrichment)\n\n\n\n## Contributors\n\nThanks to all
-our contributors! There is no specific order and hopefully nobody was left
-out.\n\n\n_[https://avatars.githubusercontent.com/morestanna]\n\n\n_[https://
+['PyJWT[crypto]>=2.4', 'fastapi>=0.65.2', 'importlib-metadata<5.0',
+'itsdangerous', 'requests'] extras_require = \ {'graphql': ['graphene>=2,<3'],
+'saml': ['python3-saml', 'python-multipart']} setup_kwargs = { 'name':
+'fastapi-opa', 'version': '1.4.3', 'description': 'Fastapi OPA middleware incl.
+auth flow.', 'long_description': '# Open Policy Agent middleware for
+FastAPI\n\n## Table of contents\n- [Contributors](#contributors)\n- [What does
+fastapi-opa do](#about)\n- [Installation](#installation)\n- [How to get
+started](#getting-started)\n- [Open Policy Agent](#opa)\n- [Authentication
+flow](#auth-flow)\n - [API key authentication](#api-key-auth)\n - [OIDC
+authentication](#oidc-auth)\n - [SAML authentication](#saml-auth)\n- [Custom
+payload enrichment](#custom-payload-enrichment)\n - [GraphQL enrichment](#gql-
+enrichment)\n\n\n\n## Contributors\n\nThanks to all the contributors below.
+Furthermore thanks for raising issues.\n\n\n_[https://
+avatars.githubusercontent.com/morestanna]\n\n\n_[https://
 avatars.githubusercontent.com/busykoala]\n\n\n_[https://
 avatars.githubusercontent.com/TracyWR]\n\n\n_[https://
 avatars.githubusercontent.com/loikki]\n\n\n_[https://
 avatars.githubusercontent.com/ejsyx]\n\n\n\n\n## What does fastapi-opa
-do\n\n`fastapi-opa` is an extension to FastAPI that allows you to add a login
-flow\nto your application within minutes using open policy agent and your
-favourite\nidentity provider.\n\n![Flow Diagram](https://
+do\n\nThe FastAPI extension `fastapi-opa` allows to add login flows and
+integrates\nOpen Policy Agent to your app.\n\n![Flow Diagram](https://
 raw.githubusercontent.com/busykoala/fastapi-opa/master/assets/
-diagram.png)\n\nWhen a user tries to get a response from an endpoint he/she
-will be redirected\nto the identity provider for authorization.\nAfter the
-authentication the app validates the token provided. Once it was\nvalidated the
-user information is used to get an OPA decision whether\nthe user is allowed to
-get any information from the endpoint.\n\n\n\n##
+diagram.png)\n\nThe middleware redirects the request to the identity provider.
+After the\nauthentication it validates the token. Using the token, Open Policy
+Agent\ndecides if the response has success or failure status.\n\n\n\n##
 Installation\n\n```bash\npoetry add [--extras "graphql"] [--extras "saml"]
-fastapi-opa \n```\n\n\n\n## How to get started\n\n:bulb: Checkout the wiki for
-a complete environment setup with Keycloak and Open Policy Agent: \n[Getting
-Started with FastAPI app with Authentication and Authorization](https://
-github.com/busykoala/fastapi-opa/wiki#dev-setup)\n\nThe package provides a very
-easy way to integrate authentication and\nauthorization. We can decide what
-authentication flow we inject into the\nOPAMiddleware to be able choosing
-between different flows.\n\nThere are \n - one example for oidc :
-fastapi_opa.example_oidc.py,\n - one example for saml:
-fastapi_opa.example_saml.py\n\n## Open Policy Agent\n\nThe (validated/
-authenticated) user token is sent to the Open Policy Agent\nwith the additional
-attributes `request_method` and `request_path`.\n\n```json\n{\n "input": {\n
-"exp": 1617466243,\n "iat": 1617465943,\n "auth_time": 1617465663,\n "jti":
+fastapi-opa \n```\n\n\n\n## How to get started\n\n:bulb: checkout the wiki for
+an environment setup with Keycloak and Open Policy Agent: \n[Getting Started
+with FastAPI app with Authentication and Authorization](https://github.com/
+busykoala/fastapi-opa/wiki#dev-setup)\n\nThe package combines authentication
+and authorization with FastAPI. You can\ncustomize the `OPAMiddleware`
+depending on your authentication flow.\n\nCheck out these examples for the most
+common flows:\n- OIDC: `fastapi_opa.example_oidc.py`\n- SAML:
+`fastapi_opa.example_saml.py`\n\n## Open Policy Agent\n\nThe middleware sends
+the validated and authenticated user token to Open\nPolicy Agent. It adds the
+extra attributes `request_method` and\n`request_path`.\n\n```json\n{\n "input":
+{\n "exp": 1617466243,\n "iat": 1617465943,\n "auth_time": 1617465663,\n "jti":
 "9aacb638-70c6-4f0a-b0c8-dbc67f92e3d1",\n "iss": "http://localhost:8080/auth/
 realms/example-realm",\n "aud": "example-client",\n "sub": "ccf78dc0-e1d6-4606-
 99d4-9009e74e3ab4",\n "typ": "ID",\n "azp": "david",\n "session_state":
 "41640fe7-39d2-44bc-818c-a3360b36fb87",\n "at_hash": "2IGw-
 B9f5910Sll1tnfQRg",\n "acr": "0",\n "email_verified": false,\n "hr": "true",\n
 "preferred_username": "david",\n "user": "david",\n "subordinates": [],\n
 "request_method": "GET",\n "request_path": ["finance", "salary", "david"]\n
-}\n}\n```\n\nIn open policy agent you can now easily create policies using user
-roles,\nroutes, or request methods etc.\n\nAn example policy (from [the
-official OPA docs](https://www.openpolicyagent.org/docs/v0.11.0/http-api-
-authorization/))\nfor this setup could be like:\n\n```rego\npackage
+}\n}\n```\n\nIn Open Policy Agent you can create policies using user
+roles,\nroutes, request methods etc.\n\nAn example policy (from [the official
+Open Policy Agent\ndocs](https://www.openpolicyagent.org/docs/v0.11.0/http-api-
+authorization/))\nfor this setup could look like this:\n\n```rego\npackage
 httpapi.authz\n\n# bob is alice\'s manager, and betty is
 charlie\'s.\nsubordinates = {"alice": [], "charlie": [], "bob": ["alice"],
 "betty": ["charlie"]}\n\n# HTTP API request\nimport input\n\ndefault allow =
 false\n\n# Allow users to get their own salaries.\nallow {\n some username\n
 input.request_method == "GET"\n input.request_path = ["finance", "salary",
 username]\n input.user == username\n}\n\n# Allow managers to get their
 subordinates\' salaries.\nallow {\n some username\n input.request_method ==
 "GET"\n input.request_path = ["finance", "salary", username]\n subordinates
-[input.user][_] == username\n}\n```\n\n\n\n## Authentication Flow\n\nThere is
-an interface provided to easily implement the desired authentication\nflow and
-inject it into OPAMiddleware\n
-(`fastapi_opa.auth.auth_interface.AuthInterface`), or you can open a
-pull\nrequest if you would like to contribute to the package.\n\nAlso there are
-implementations ready to use.\n\n\n\n### API Key Authentication\n\nThe API key
-authentication is the simplest authentication system where you simply needs to
-match\na given value in the request header:\n```python\n# Configure API
+[input.user][_] == username\n}\n```\n\n\n\n## Authentication flow\n\nUse the
+provided interface to set up your desired authentication flow. Then\ninsert it
+into `OPAMiddleware`
+(`fastapi_opa.auth.auth_interface.AuthInterface`).\nConsider submitting a pull
+request with new flows.\n\nYou can also use these ready-to-go implementations:
+\n\n\n\n### API key authentication\n\nIn the API key authentication a request
+header needs to match a given value.\n\n```python\n# Configure API
 keys\napi_key_config = APIKeyConfig(\n header_key="test",\n
 api_key="1234"\n)\napi_key_auth = APIKeyAuthentication
-(api_key_config)\n```\nHere sending a request with the `header["test"] =
-"1234"` would be considered as a successful authentication.\nFor OPA, the user
-is `APIKey` and the variable `client` is set with the client
-address.\n\n\n\n### OIDC Authentication\n\nThe example in [How to get started]
-(#getting-started) provides an example for\nthe implementation of the OIDC
-Authentication.\n\n\n\n### SAML Authentication\n\nFor the saml implementation
-create your certs using\n`openssl req -new -x509 -days 3652 -nodes -out sp.crt
--keyout sp.key` and\nadd the keys to the sp section of your `settings.json`.
-Checkout the test\nsettings to get an idea (`tests/test_data/saml/*.json`). The
-path to your\nown `settings.json` and `advanced_settings.json` has to be
-provided in the\n`SAMLAuthConfig` like in the example below (do not use the
-test data in\nproduction).\n\n```python\nfrom fastapi_opa import
-OPAConfig\nfrom fastapi_opa.auth.auth_saml import SAMLAuthentication\nfrom
-fastapi_opa.auth.auth_saml import SAMLConfig\n\nopa_host = "http://localhost:
-8181"\n\nsaml_config = SAMLConfig(settings_directory="./tests/test_data/
-saml")\nsaml_auth = SAMLAuthentication(saml_config)\n\nopa_config = OPAConfig
-(authentication=saml_auth, opa_host=opa_host,\n accepted_methods=["id_token",
-"access_token"])\n```\n\nThe cert has to be uploaded to your identity provider.
-Using Keycloak as an\nidp you need to configure `encrypt assertion`, `client
-signature required`,\n`force POST bindings` on creating the client.\nAlso
-configure: `Client Scopes` -> `role_list (saml)` -> `Mappers tab` ->\n`role
-list` -> `Single Role Attribute`\n\n\n\n## Custom Payload Enrichment\n\nIn
-`fastapi_opa.opa.opa_config.Injectable` an interface is provided to add\nmore
-information to the payload sent to OPA.\n\nThe injectables can be added to the
-`OPAConfig`. Let\'s look at an example:\n\n```python\nclass FancyInjectable
+(api_key_config)\n```\n\nIn the example the header `header["test"] = "1234"`
+authenticates the request.\nFor Open Policy Agent, set user to `APIKey` and the
+variable `client` to the\nclient address.\n\n\n\n### OIDC authentication\n\nThe
+example in [How to get started](#getting-started) provides an example for\nthe
+implementation of the OIDC Authentication.\n\n\n\n### SAML
+authentication\n\nFor the saml implementation create your certs using\n`openssl
+req -new -x509 -days 3652 -nodes -out sp.crt -keyout sp.key` and\nadd the keys
+to the sp section of your `settings.json`. Checkout the test\nsettings to get
+an idea (`tests/test_data/saml/*.json`).\nProvide the path to your own
+`settings.json` and `advanced_settings.json`\nin the `SAMLAuthConfig` like in
+the example below (don\'t use the test data in\nproduction).\n\n```python\nfrom
+fastapi_opa import OPAConfig\nfrom fastapi_opa.auth.auth_saml import
+SAMLAuthentication\nfrom fastapi_opa.auth.auth_saml import
+SAMLConfig\n\nopa_host = "http://localhost:8181"\n\nsaml_config = SAMLConfig
+(settings_directory="./tests/test_data/saml")\nsaml_auth = SAMLAuthentication
+(saml_config)\n\nopa_config = OPAConfig(authentication=saml_auth,
+opa_host=opa_host,\n accepted_methods=["id_token",
+"access_token"])\n```\n\nUpload the certificate to your identity provider.
+Using Keycloak as an\nidentity provider you need to configure `encrypt
+assertion`,\n`client signature required`, `force POST bindings` on creating the
+client.\nAlso configure: `Client Scopes` -> `role_list (saml)` -> `Mappers tab`
+->\n`role list` -> `Single Role Attribute`\n\n\n\n## Custom payload
+enrichment\n\nUse the interface `fastapi_opa.opa.opa_config.Injectable` to
+add\nmore information to the payload sent to Open Policy Agent.\n\nConfigure
+the injectables in the `OPAConfig`:\n\n```python\nclass FancyInjectable
 (Injectable):\n async def extract(self, request: Request) -> List:\n return
 ["some", "custom", "stuff"]\n\nfancy_inj = FancyInjectable("fancy_key",
 skip_endpoints=["/health", "/api/[^/]*/test])\n\nopa_config = OPAConfig(\n
 authentication=oidc_auth, opa_host=opa_host, injectables=
-[fancy_inj]\n)\n```\n\nWith `skip_endpoints`, you can define some endpoints
-where the injectable\nwill not be applied. The endpoints can be defined either
-directly or through some\nregex.\n\n\n\n\n### Graphql Enrichment\n\nFor GraphQL
-there is a ready to use injectable:\n\n```python\nfrom
+[fancy_inj]\n)\n```\n\nUse `skip_endpoints` to choose which endpoints the
+injectable shouldn\'t affect.\nTo define an endpoint, specify an exact string
+or a regular expression.\n\n\n\n### GraphQL enrichment\n\nFor GraphQL you can
+use the ready to go injectable:\n\n```python\nfrom
 fastapi_opa.opa.enrichment.graphql_enrichment import
 GraphQLInjectable`\n\ngraphql = GraphQLInjectable("gql_injectable")\nopa_config
 = OPAConfig(authentication=oidc_auth, opa_host=opa_host, injectables=
 [graphql])\n```\n', 'author': 'Matthias Osswald', 'author_email':
-'m@osswald.li', 'maintainer': None, 'maintainer_email': None, 'url': 'https://
-github.com/busykoala/fastapi-opa', 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'extras_require':
-extras_require, 'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
+'info@busykoala.io', 'maintainer': None, 'maintainer_email': None, 'url':
+'https://github.com/busykoala/fastapi-opa', 'packages': packages,
+'package_data': package_data, 'install_requires': install_requires,
+'extras_require': extras_require, 'python_requires': '>=3.7,<4.0', } setup
+(**setup_kwargs)
```

