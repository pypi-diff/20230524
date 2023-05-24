# Comparing `tmp/jupyterhub_ltiauthenticator-1.5.0.tar.gz` & `tmp/jupyterhub_ltiauthenticator-1.5.1.tar.gz`

## Comparing `jupyterhub_ltiauthenticator-1.5.0.tar` & `jupyterhub_ltiauthenticator-1.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/_version.py
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/lti11/__init__.py
--rw-r--r--   0        0        0     6792 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/lti11/auth.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/lti11/constants.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/lti11/handlers.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/lti11/templates.py
--rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/lti11/validator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/lti13/__init__.py
--rw-r--r--   0        0        0     6984 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/lti13/auth.py
--rw-r--r--   0        0        0    14762 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/lti13/constants.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/lti13/error.py
--rw-r--r--   0        0        0    16831 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/lti13/handlers.py
--rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/lti13/validator.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.0/.gitignore
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.0/LICENSE
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.0/README.md
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/_version.py
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti11/__init__.py
+-rw-r--r--   0        0        0     6792 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti11/auth.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti11/constants.py
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti11/handlers.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti11/templates.py
+-rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti11/validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti13/__init__.py
+-rw-r--r--   0        0        0     6984 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti13/auth.py
+-rw-r--r--   0        0        0    14762 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti13/constants.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti13/error.py
+-rw-r--r--   0        0        0    17269 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti13/handlers.py
+-rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti13/validator.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/.gitignore
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/LICENSE
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/README.md
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/PKG-INFO
```

### Comparing `jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/utils.py` & `jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/utils.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/lti11/auth.py` & `jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti11/auth.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/lti11/constants.py` & `jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti11/constants.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/lti11/handlers.py` & `jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti11/handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,21 @@
 
     def set_login_cookie(self, user):
         super().set_login_cookie(user)
 
         # Make sure that hub cookie is always set, even if the user was already logged in
         self.set_hub_cookie(user)
 
+    def check_xsrf_cookie(self):
+        """
+        Do not attempt to check for xsrf parameter in POST requests. LTI requests are
+        meant to be cross-site, so it must not be verified.
+        """
+        return
+
     @gen.coroutine
     def post(self):
         """
         Technical reference of relevance to understand this function
         ------------------------------------------------------------
         1. Class dependencies
            - jupyterhub.handlers.BaseHandler: https://github.com/jupyterhub/jupyterhub/blob/abb93ad799865a4b27f677e126ab917241e1af72/jupyterhub/handlers/base.py#L69
```

### Comparing `jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/lti11/templates.py` & `jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti11/templates.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/lti11/validator.py` & `jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti11/validator.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/lti13/auth.py` & `jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti13/auth.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/lti13/constants.py` & `jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti13/constants.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/lti13/error.py` & `jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti13/error.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/lti13/handlers.py` & `jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti13/handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,14 +127,21 @@
 
 class LTI13LoginInitHandler(OAuthLoginHandler):
     """
     Handles JupyterHub authentication requests according to the
     LTI 1.3 standard.
     """
 
+    def check_xsrf_cookie(self):
+        """
+        Do not attempt to check for xsrf parameter in POST requests. LTI requests are
+        meant to be cross-site, so it must not be verified.
+        """
+        return
+
     def authorize_redirect(
         self,
         redirect_uri: str,
         login_hint: str,
         nonce: str,
         client_id: str,
         state: str,
@@ -319,14 +326,21 @@
     References:
     https://www.imsglobal.org/spec/security/v1p0/#step-3-authentication-response
     https://www.imsglobal.org/spec/security/v1p0/#step-4-resource-is-displayed
     """
 
     _nonce_state_cookie = None
 
+    def check_xsrf_cookie(self):
+        """
+        Do not attempt to check for xsrf parameter in POST requests. LTI requests are
+        meant to be cross-site, so it must not be verified.
+        """
+        return
+
     async def get(self):
         """Overrides the upstream get handler and always raise HTTPError 405."""
         raise HTTPError(405, "GET method is not allowed for launch requests")
 
     async def post(self):
         """
         Overrides the upstream post handler.
```

### Comparing `jupyterhub_ltiauthenticator-1.5.0/ltiauthenticator/lti13/validator.py` & `jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti13/validator.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_ltiauthenticator-1.5.0/.gitignore` & `jupyterhub_ltiauthenticator-1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterhub_ltiauthenticator-1.5.0/LICENSE` & `jupyterhub_ltiauthenticator-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub_ltiauthenticator-1.5.0/README.md` & `jupyterhub_ltiauthenticator-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterhub_ltiauthenticator-1.5.0/pyproject.toml` & `jupyterhub_ltiauthenticator-1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "escapism>=1.0.1",
     "jupyterhub>=1.2",
     "oauthenticator>=15.1.0",
     "oauthlib>=3.2.2",
-    "PyJWT[crypto]>=2.6.0",
+    "PyJWT[crypto]>=2.7.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
     "pre-commit",
 ]
@@ -121,15 +121,15 @@
 #
 # ref: https://github.com/your-tools/tbump#readme
 #
 [tool.tbump]
 github_url = "https://github.com/jupyterhub/ltiauthenticator"
 
 [tool.tbump.version]
-current = "1.5.0"
+current = "1.5.1"
 regex = '''
     (?P<major>\d+)
     \.
     (?P<minor>\d+)
     \.
     (?P<patch>\d+)
     (?P<pre>((a|b|rc)\d+)|)
```

### Comparing `jupyterhub_ltiauthenticator-1.5.0/PKG-INFO` & `jupyterhub_ltiauthenticator-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-ltiauthenticator
-Version: 1.5.0
+Version: 1.5.1
 Summary: JupyterHub authenticator implementing LTI v1.1 and LTI v1.3
 Project-URL: Documentation, https://ltiauthenticator.readthedocs.io
 Project-URL: Source, https://github.com/jupyterhub/ltiauthenticator
 Project-URL: Issues, https://github.com/jupyterhub/ltiauthenticator/issues
 Author-email: Yuvi Panda <yuvipanda@gmail.com>, Jupyter Contributors <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
@@ -40,15 +40,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: escapism>=1.0.1
 Requires-Dist: jupyterhub>=1.2
 Requires-Dist: oauthenticator>=15.1.0
 Requires-Dist: oauthlib>=3.2.2
-Requires-Dist: pyjwt[crypto]>=2.6.0
+Requires-Dist: pyjwt[crypto]>=2.7.0
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
```

