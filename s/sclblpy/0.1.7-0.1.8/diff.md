# Comparing `tmp/sclblpy-0.1.7.tar.gz` & `tmp/sclblpy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sclblpy-0.1.7.tar", last modified: Sun May  9 07:29:23 2021, max compression
+gzip compressed data, was "dist/sclblpy-0.1.8.tar", last modified: Thu May 12 08:52:40 2022, max compression
```

## Comparing `sclblpy-0.1.7.tar` & `sclblpy-0.1.8.tar`

### file list

```diff
@@ -1,33 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-09 07:29:23.000000 sclblpy-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2021-05-09 07:29:20.000000 sclblpy-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-05-09 07:29:20.000000 sclblpy-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    17511 2021-05-09 07:29:23.000000 sclblpy-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14023 2021-05-09 07:29:20.000000 sclblpy-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       99 2021-05-09 07:29:20.000000 sclblpy-0.1.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-09 07:29:23.000000 sclblpy-0.1.7/sclblpy/
--rw-r--r--   0 runner    (1001) docker     (121)      766 2021-05-09 07:29:20.000000 sclblpy-0.1.7/sclblpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      325 2021-05-09 07:29:20.000000 sclblpy-0.1.7/sclblpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3389 2021-05-09 07:29:20.000000 sclblpy-0.1.7/sclblpy/_bundle.py
--rw-r--r--   0 runner    (1001) docker     (121)     1439 2021-05-09 07:29:20.000000 sclblpy-0.1.7/sclblpy/_globals.py
--rw-r--r--   0 runner    (1001) docker     (121)    10611 2021-05-09 07:29:20.000000 sclblpy-0.1.7/sclblpy/_jwt.py
--rw-r--r--   0 runner    (1001) docker     (121)     8141 2021-05-09 07:29:20.000000 sclblpy-0.1.7/sclblpy/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    25017 2021-05-09 07:29:20.000000 sclblpy-0.1.7/sclblpy/appdirs.py
--rw-r--r--   0 runner    (1001) docker     (121)      807 2021-05-09 07:29:20.000000 sclblpy-0.1.7/sclblpy/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    70437 2021-05-09 07:29:20.000000 sclblpy-0.1.7/sclblpy/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2021-05-09 07:29:20.000000 sclblpy-0.1.7/sclblpy/supported_models.json
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-05-09 07:29:20.000000 sclblpy-0.1.7/sclblpy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-09 07:29:23.000000 sclblpy-0.1.7/sclblpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    17511 2021-05-09 07:29:23.000000 sclblpy-0.1.7/sclblpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      537 2021-05-09 07:29:23.000000 sclblpy-0.1.7/sclblpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-09 07:29:23.000000 sclblpy-0.1.7/sclblpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-05-09 07:29:23.000000 sclblpy-0.1.7/sclblpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-05-09 07:29:23.000000 sclblpy-0.1.7/sclblpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-09 07:29:23.000000 sclblpy-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      905 2021-05-09 07:29:20.000000 sclblpy-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-09 07:29:23.000000 sclblpy-0.1.7/test/
--rw-r--r--   0 runner    (1001) docker     (121)    21798 2021-05-09 07:29:20.000000 sclblpy-0.1.7/test/test_all_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-05-09 07:29:20.000000 sclblpy-0.1.7/test/test_bundle.py
--rw-r--r--   0 runner    (1001) docker     (121)     3086 2021-05-09 07:29:20.000000 sclblpy-0.1.7/test/test_jwt.py
--rw-r--r--   0 runner    (1001) docker     (121)     8847 2021-05-09 07:29:20.000000 sclblpy-0.1.7/test/test_main.py
--rw-r--r--   0 runner    (1001) docker     (121)     3816 2021-05-09 07:29:20.000000 sclblpy-0.1.7/test/test_run.py
--rw-r--r--   0 runner    (1001) docker     (121)     3260 2021-05-09 07:29:20.000000 sclblpy-0.1.7/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-12 08:52:40.000000 sclblpy-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-05-12 08:52:34.000000 sclblpy-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-05-12 08:52:34.000000 sclblpy-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     8404 2022-05-12 08:52:40.000000 sclblpy-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7930 2022-05-12 08:52:34.000000 sclblpy-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2022-05-12 08:52:34.000000 sclblpy-0.1.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-12 08:52:40.000000 sclblpy-0.1.8/sclblpy/
+-rw-r--r--   0 runner    (1001) docker     (121)      700 2022-05-12 08:52:34.000000 sclblpy-0.1.8/sclblpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      325 2022-05-12 08:52:34.000000 sclblpy-0.1.8/sclblpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3389 2022-05-12 08:52:34.000000 sclblpy-0.1.8/sclblpy/_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-05-12 08:52:34.000000 sclblpy-0.1.8/sclblpy/_globals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10554 2022-05-12 08:52:34.000000 sclblpy-0.1.8/sclblpy/_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-05-12 08:52:34.000000 sclblpy-0.1.8/sclblpy/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25017 2022-05-12 08:52:34.000000 sclblpy-0.1.8/sclblpy/appdirs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      807 2022-05-12 08:52:34.000000 sclblpy-0.1.8/sclblpy/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44001 2022-05-12 08:52:34.000000 sclblpy-0.1.8/sclblpy/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-05-12 08:52:34.000000 sclblpy-0.1.8/sclblpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-12 08:52:40.000000 sclblpy-0.1.8/sclblpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8404 2022-05-12 08:52:40.000000 sclblpy-0.1.8/sclblpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2022-05-12 08:52:40.000000 sclblpy-0.1.8/sclblpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-12 08:52:40.000000 sclblpy-0.1.8/sclblpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-05-12 08:52:40.000000 sclblpy-0.1.8/sclblpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-05-12 08:52:40.000000 sclblpy-0.1.8/sclblpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-12 08:52:40.000000 sclblpy-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      874 2022-05-12 08:52:34.000000 sclblpy-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-12 08:52:40.000000 sclblpy-0.1.8/test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-12 08:52:34.000000 sclblpy-0.1.8/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-05-12 08:52:34.000000 sclblpy-0.1.8/test/test_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3052 2022-05-12 08:52:34.000000 sclblpy-0.1.8/test/test_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7165 2022-05-12 08:52:34.000000 sclblpy-0.1.8/test/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (121)      907 2022-05-12 08:52:34.000000 sclblpy-0.1.8/test/test_utils.py
```

### Comparing `sclblpy-0.1.7/LICENSE` & `sclblpy-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sclblpy-0.1.7/sclblpy/__init__.py` & `sclblpy-0.1.8/sclblpy/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import sys
 
 if sys.version_info < (3, 0):
     print('Sclblpy requires Python 3, while Python ' + str(sys.version[0] + ' was detected. Terminating... '))
     sys.exit(1)
 
 from .main import welcome, \
-    upload, upload_sklearn, upload_onnx, update, update_sklearn, update_onnx, update_docs, \
+    upload_onnx, update_onnx, update_docs, \
     endpoints, delete_endpoint, models, delete_model, \
     devices, delete_device, assignments, assign, delete_assignment, \
-    run, remove_credentials, list_models, \
+    remove_credentials, \
     stop_print, start_print, \
     _set_toolchain_URL, _set_usermanager_URL, _set_taskmanager_URL
 from .version import __version__
```

### Comparing `sclblpy-0.1.7/sclblpy/_bundle.py` & `sclblpy-0.1.8/sclblpy/_bundle.py`

 * *Files identical despite different names*

### Comparing `sclblpy-0.1.7/sclblpy/_globals.py` & `sclblpy-0.1.8/sclblpy/_globals.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # Global variables for the sclblpy package.
 import os
 from sclblpy.appdirs import AppDirs
 
 # servers:
-USER_MANAGER_URL: str = "https://usermanager.sclbl.net:8008"  # Location of the user manager.
-TOOLCHAIN_URL: str = "https://toolchain.sclbl.net:8010"  # Location of the toolchain server.
-TASK_MANAGER_URL: str = "https://taskmanager.sclbl.net:8080"  # Location of the taskmanager.
+USER_MANAGER_URL: str = "https://usermanager.sclbl.net"  # Location of the user manager.
+TOOLCHAIN_URL: str = "https://toolchain.sclbl.net"  # Location of the toolchain server.
+TASK_MANAGER_URL: str = "https://taskmanager.sclbl.net"  # Location of the taskmanager.
 
 # control printing:
 SILENT: bool = False  # Boolean indicating whether user feedback should be suppressed.
 DEBUG: bool = False  # Boolean indicating whether using the package in debug mode; if so, it will raise exceptions.
 
 # Storage locations:
 dirs = AppDirs("sclblpy", "sclbl")
 USER_CREDENTIALS: str = dirs.user_config_dir + "/.creds.json"  # Location of json file to store user credentials
 GZIP_BUNDLE: str = dirs.user_data_dir + "/model_bundle.gzip"  # Location where a save model is (temporarily) stored
-MODELS_JSON: str = os.path.dirname(os.path.realpath(__file__)) + "/supported_models.json"  # Location of the json with supported models
 
 # JWT necessities:
 JWT_TOKEN: str = ""  # JWT token.
 JWT_USER_ID: str = ""  # Scailable user id.
 JWT_TIMESTAMP: float = 0.0  # Timestamp in seconds.
 
 # Available models:
```

### Comparing `sclblpy-0.1.7/sclblpy/_jwt.py` & `sclblpy-0.1.8/sclblpy/_jwt.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     Checks whether a valid JWT string is present. If so,
     checks whether the JWT string needs refreshing (more than 2 mins old)
     and refreshes if necessary. Returns True when a valid and
     fresh JWT string is located.
 
     Note, if no JWT string is present, or the JWT string has expired,
     the function tries to
-    a. Read username and pass from file
-    b. Prompt user for username and pass
+    a. Read email and pass from file
+    b. Prompt user for email and pass
     and subsequently sign in.
 
     Args:
         seconds_refresh: int, seconds before a refresh is attempted. Default 120.
         seconds_renew: int, seconds before a renew is attempted. Default 280.
 
     Returns:
@@ -37,15 +37,15 @@
     now: float = time.time()
     time_refresh: float = now - seconds_refresh
     time_renew: float = now - seconds_renew
 
     if not glob.JWT_TOKEN or glob.JWT_TIMESTAMP < time_renew:
         user_details: dict = _get_user_details()
         try:
-            if _sign_in(user_details['username'], user_details['password']):
+            if _sign_in(user_details['email'], user_details['password']):
                 return True
             else:
                 return False
         except LoginError as e:
             if not glob.SILENT:
                 print("JWT error: sign in failed:" + str(e))
             if glob.DEBUG:
@@ -69,42 +69,42 @@
     if glob.JWT_TOKEN:
         return True
     else:
         # Edge case; JWT token empty:
         return False
 
 
-def _sign_in(username: str, password: str, _remove_file=True) -> bool:
+def _sign_in(email: str, password: str, _remove_file=True) -> bool:
     """Performs the sign in of a user.
 
     The function sign in performs a sign in of a user based
-    on the username (str) and password (str). It returns
+    on the email (str) and password (str). It returns
     a boolean value indicating whether the sign in was successful.
 
     Args:
-        username: A string (email) to login the user
+        email: A string (email) to login the user
         password: A string (password for login
         _remove_file: A bool indicating if the credentials should be removed on failed login. Default True.
 
     Returns:
         True if sign in is successful.
 
     Raises:
         LoginError: if unable to login.
     """
-    if len(username) < 1 or len(password) < 1:
+    if len(email) < 1 or len(password) < 1:
         if not glob.SILENT:
-            print("JWT error: no username and password provided.")
+            print("JWT error: no email and password provided.")
         if glob.DEBUG:
-            raise LoginError("No username or password provided.")
+            raise LoginError("No email or password provided.")
         return False
 
     url: str = glob.USER_MANAGER_URL + "/user/signin/"
     data: dict = {
-        'email': username,
+        'email': email,
         'pwd': password
     }
     headers: dict = {
         'Content-Type': 'text/plain'
     }
 
     # Try connecting to server:
@@ -157,47 +157,47 @@
             print("JWT error: Unable to connect to scailable servers.")
         if glob.DEBUG:
             raise LoginError("Unable to connect to Scailable servers.")
         return False
 
 
 def _get_user_details() -> dict:
-    """Gets the username and password from a user.
+    """Gets the email and password from a user.
 
     Function tries to
-    a. Retrieve username and password from .creds.json file.
-    b. Retrieve username and password by prompting the user.
+    a. Retrieve email and password from .creds.json file.
+    b. Retrieve email and password by prompting the user.
 
     If user responds 'y' to prompt to save the function we will store the user credentials.
 
     Args:
 
     Returns:
         A dict containing the fields
-            'username' String
+            'email' String
             'password' String
 
     Raises (in debug mode):
         LoginError
     """
 
     details: dict = {}
     try:
         with open(glob.USER_CREDENTIALS, "r") as f:
             details = json.load(f)
             return details
     except FileNotFoundError:
         pass
 
-    username: str = input("Please provide your username: ")
+    email: str = input("Please provide your email: ")
     with warnings.catch_warnings():
         warnings.simplefilter('ignore', GetPassWarning)
         password = getpass('Please type your password: ')
 
-    details['username'] = username
+    details['email'] = email
     details['password'] = password
 
     while True:
         query = input('Would you like us to store your user credentials (y/n)? ')
         answer = query[0].lower()
         if query == '' or not answer in ['y', 'n']:
             print('Please answer with yes or no')
@@ -301,15 +301,15 @@
             if not glob.SILENT:
                 print("JWT delete error: Unable to remove your credentials.")
             if glob.DEBUG:
                 raise JWTError("JWT delete error: Unable to remove credentials: " + str(e))
             return False
         if not glob.SILENT:
             print("Your stored user credentials have been removed. \n"
-                  "You will have to re-enter your username and password next time.")
+                  "You will have to re-enter your email and password next time.")
 
         return True
     else:
         return False
 
 
 if __name__ == '__main__':
```

### Comparing `sclblpy-0.1.7/sclblpy/appdirs.py` & `sclblpy-0.1.8/sclblpy/appdirs.py`

 * *Files identical despite different names*

### Comparing `sclblpy-0.1.7/sclblpy/errors.py` & `sclblpy-0.1.8/sclblpy/errors.py`

 * *Files identical despite different names*

### Comparing `sclblpy-0.1.7/sclblpy/main.py` & `sclblpy-0.1.8/sclblpy/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,98 +1,29 @@
 # File contains all public methods of the scblpy package
 import json
 import urllib
 import requests
 import sclblpy._globals as glob
 from sclblpy._bundle import _gzip_save, _gzip_delete
 from sclblpy._jwt import _check_jwt, _remove_credentials
-from sclblpy._utils import _get_model_name, _get_system_info, _predict, _get_model_package, _load_supported_models, \
-    _check_model
+from sclblpy._utils import  _get_system_info
 from sclblpy.errors import UserManagerError, JWTError, UploadModelError, RunTaskError, CreateAssignmentError
 from sclblpy.version import __version__
 
 
 # welcome just prints a simple welcome message:
 def welcome():
     """ Welcome simply prints a welcome message.
     """
     print("\n*** Thanks for importing sclblpy! ***")
     print("You can use the 'upload()' function to upload your models.")
     print("To inspect your currently uploaded models, use `endpoints()`.")
     print("Check the docs at https://pypi.org/project/sclblpy/ for more info. \n")
 
 
-# upload is a wrapper for upload_onnx and upload_sklearn to provide backwards compatibility:
-def upload(mod, features, docs={}, email=True, model_type="sklearn", _keep=False) -> bool:
-    """upload uploads a trained AI/ML model to Scailable.
-
-    The upload function is the main workhorse of the sclblpy package but effectively provides a
-    wrapper to choose between the
-     - upload_sklearn(mod, feature_vector, docs={}, email=True, _keep=False)
-     - upload_onnx(path, docs={}, email=True)
-    functions.
-
-    The function checks the type, and if type = "sklearn" (default) calls the upload_sklearn() function.
-    If type = "onnx" it calls the upload_onnx() function.
-
-    Behavior:
-    If type = "onnx"
-        - The function first checks if the supplied path indeed references a .onnx file
-        - Next, the docs are checked; if none are provided a warning is issued and a simple
-        name is provided based on the model type.
-        - Finally the onnx file and the supporting docs are uploaded to the toolchain.
-
-    If type = "sklearn"
-        - The function first checks whether the supplied model is ok (part of the list and fitted).
-        - Next, it checks whether an example row is provided and if so it creates the example
-        input and output .json objects.
-        - Next, the docs are checked; if none are provided a warning is issued and a simple
-        name is provided based on the model type.
-        - Subsequently, we package the whole thing, including details of the user system, into a
-        gzipped file that is stored on disc.
-        - Finally the whole package is uploaded to the toolchain.
-
-    Note: This method prints user-feedback by default. This feedback can be suppressed by calling the
-        stop_print() method.
-
-    Args:
-        mod: The model to be uploaded (type="sklearn" OR the path to the stored ONNX file (type="onnx").
-        features:
-            - An example feature_vector for your model (type="sklearn" only).
-            (i.e., the first row of your training data X obtained using row = X[0,:])
-            - The input str (binary) to the onnx model (type="onnx" only). Can be an empty string.
-        docs: A dict{} containing the fields 'name' and 'documentation'.
-        email: Bool indicating whether a confirmation email of a successful conversion should be send. Default True.
-        model_type: String indicating the type of model. Currently with options "sklearn" or "onnx". Default "sklearn"
-        _keep: Bool indicating whether the .gzipped file should be retained (type="sklearn" only). Default False.
-
-    Returns:
-        False if upload failed, true otherwise
-
-    Raises  (in debug mode):
-        UploadModelError if unable to successfully bundle and upload the model.
-    """
-    if model_type == "sklearn":
-        if features == "":
-            if not glob.SILENT:
-                print("FATAL: You cannot upload a sklearn model with an empty string as feature vector.")
-            if glob.DEBUG:
-                raise UploadModelError("Cannot upload sklearn model with empty string as feature vector.")
-            return False
-        if not upload_sklearn(mod, features, docs, email, _keep):
-            return False
-    elif model_type == "onnx":
-        if not upload_onnx(mod, features, docs, email):
-            return False
-    else:
-        if glob.DEBUG:
-            raise UploadModelError("Please specify a valid model type.")
-        return False
-
-    return True
 
 
 # upload_onnx uploads an onnx file to the toolchain-server
 def upload_onnx(path, example="", docs={}, email=True) -> bool:
     """upload_onnx uploads a fitted onnx model to Scailable.
 
     - The function first checks if the supplied path indeed references a .onnx file
@@ -196,15 +127,15 @@
 
         # Do the request
         try:
             response = requests.post(url, headers=headers, data=payload, files=files)
         except Exception as e:
             if not glob.SILENT:
                 print("FATAL: Unable to carry out the upload request: the toolchain is not available. \n"
-                      "Your model has not been uploaded. \n")
+                      "Your model has not been uploaded. PLACE 1 URL: {url}\n")
             if glob.DEBUG:
                 raise UploadModelError("We were unable to obtain JWT authorization: " + str(e))
             return False
 
         # Error handling
         try:
             response_data = json.loads(response.text)
@@ -237,264 +168,16 @@
 
         return True
 
     else:
         return False
 
 
-# upload_sklearn uploads a fitted sklearn model to the toolchain server
-def upload_sklearn(mod, feature_vector, docs={}, email=True, _keep=False) -> bool:
-    """upload_sklearn uploads a fitted sklearn model to Scailable.
-
-    - The function first checks whether the supplied model is ok (part of the list and fitted).
-    - Next, it checks whether an example row is provided and if so it creates the example
-    input and output .json objects.
-    - Next, the docs are checked; if none are provided a warning is issued and a simple
-    name is provided based on the model type.
-    - Subsequently, we package the whole thing, including details of the user system, into a
-    gzipped file that is stored on disc.
-    - Finally the whole package is uploaded to the toolchain.
-
-    Note: This method prints user-feedback by default. This feedback can be suppressed by calling the
-        stop_print() method.
-
-    Args:
-        mod: The model to be uploaded.
-        feature_vector: An example feature_vector for your model.
-            (i.e., the first row of your training data X obtained using row = X[0,:])
-        docs: A dict{} containing the fields 'name' and 'documentation'
-        email: Bool indicating whether a confirmation email of a successful conversion should be send. Default True.
-        _keep: Bool indicating whether the .gzipped file should be retained. Default False.
-
-    Returns:
-        False if upload failed, true otherwise
-
-    Raises  (in debug mode):
-        UploadModelError if unable to successfully bundle and upload the model.
-    """
-    if glob.DEBUG:
-        print("We are checking your uploaded sklearn model...")
-
-    bundle = {}
-
-    # Check model:
-    if not _check_model(mod):
-        if not glob.SILENT:
-            print("FATAL: The model you are trying to upload is not (yet) supported or has not been fitted. \n"
-                  "Please see README.md for a list of supported models. \n"
-                  "Your models has not been uploaded. \n")
-        if glob.DEBUG:
-            raise UploadModelError("The uploaded model is not supported.")
-        return False
-    bundle['fitted_model'] = mod
-
-    # check input vector and generate an example:
-    bundle['example'] = {}
-    if feature_vector.any():
-        # try prediction
-        try:
-            output = _predict(mod, feature_vector)  # predict raises error if unable to generate predcition
-        except Exception as e:
-            if not glob.SILENT:
-                print("FATAL: We were unable to create an example inference. \n"
-                      "Your model has not been uploaded. \n")
-            if glob.DEBUG:
-                raise UploadModelError("Unable to generate prediction: " + str(e))
-            return False
-        # format data:
-        input_str: str = '[[%s]]' % ', '.join([str(i) for i in feature_vector.tolist()])
-        example = {'input': input_str, "output": json.dumps(output)}
-        bundle['example'] = example
-    else:
-        if not glob.SILENT:
-            print("FATAL: You did not provide a required example instance. (see docs). \n"
-                  "Your model has not been uploaded. \n")
-        return False
-
-    # check the docs:
-    bundle['docs'] = {}
-    if docs:
-        bundle['docs'] = docs
-    else:
-        try:  # This should work, but catching the exception just in case:
-            name = _get_model_name(mod)
-        except Exception:
-            name = "NAMELESS MODEL"
-        bundle['docs']['name'] = name
-        bundle['docs']['documentation'] = "-- EMPTY --"
-        if not glob.SILENT:
-            print("WARNING: You did not provide any documentation. \n"
-                  "We will simply use " + name + " as its name without further documentation.")
-
-    # check authorization:
-    auth = _check_jwt()
-    if not auth:
-        if not glob.SILENT:
-            print("FATAL: We were unable to obtain JWT authorization for your account. \n"
-                  "Your model has not been uploaded. \n")
-        if glob.DEBUG:
-            raise UploadModelError("We were unable to obtain JWT authorization.")
-        return False
-
-    # get system information
-    bundle['system_info'] = _get_system_info()
-
-    # gzip the bundle
-    if not _gzip_save(bundle):
-        if not glob.SILENT:
-            print("FATAL: We were unable to gzip your model bundle. \n"
-                  "Your model has not been uploaded. \n")
-        if glob.DEBUG:
-            raise UploadModelError("We were unable to save the bundle.")
-        return False
-
-    # all ok, upload:
-    if auth:
-
-        url = glob.TOOLCHAIN_URL + "/upload/" + glob.JWT_USER_ID
-
-        # Map python package to the right toolchain:
-        pkg_name = _get_model_package(mod)
-        toolchain_name = ""
-        if pkg_name == "sklearn":
-            toolchain_name = "sklearn"
-        elif pkg_name == "statsmodels":
-            toolchain_name = "sklearn"
-        elif pkg_name == "xgboost":
-            toolchain_name = "sklearn"
-        elif pkg_name == "lightgbm":
-            toolchain_name = "sklearn"
-
-        # Setup the actual request
-        data: dict = {
-            'email': email,
-            'package': __version__,
-            'toolchain': toolchain_name,
-            'name': bundle['docs'].get('name', "No name found."),
-            'docs': bundle['docs'].get('documentation', "No docs provided."),
-            'exampleInput': bundle['example'].get('input', "[]"),
-            'exampleOutput': bundle['example'].get('output', "[]")
-        }
-        payload: dict = {
-            'data': json.dumps(data)
-        }
-
-        files = [('bundle', open(glob.GZIP_BUNDLE, 'rb'))]
-        headers = {
-            'Authorization': glob.JWT_TOKEN,
-        }
-
-        # Do the request (and make sure to delete the gzip if errors occur)
-        try:
-            response = requests.post(url, headers=headers, data=payload, files=files)
-        except Exception as e:
-            if not glob.SILENT:
-                print("FATAL: Unable to carry out the upload request: the toolchain is not available. \n"
-                      "Your model has not been uploaded. \n")
-            if not _keep:
-                _gzip_delete()
-            if glob.DEBUG:
-                raise UploadModelError("We were unable to obtain JWT authorization: " + str(e))
-            return False
-
-        # Error handling
-        try:
-            response_data = json.loads(response.text)
-        except Exception as e:
-            if not glob.SILENT:
-                print("FATAL: We did not receive a valid JSON response from the toolchain-server. \n"
-                      "Your model has not been uploaded. \n")
-            if not _keep:
-                _gzip_delete()
-            if glob.DEBUG:
-                raise UploadModelError("We did not receive a valid response from the server: " + str(e))
-            return False
-
-        if response_data['error']:
-            if not glob.SILENT:
-                print("FATAL: An error was returned by the toolchain-server. \n"
-                      "Your model has not been uploaded. \n")
-            if not _keep:
-                _gzip_delete()
-            if glob.DEBUG:
-                raise UploadModelError("We did not receive a valid response from the server: " + response_data['error'])
-            return False
-
-        if glob.DEBUG:
-            print("The following content has been send to the toolchain server:")
-            print(bundle)
-
-        # user feedback:
-        if not glob.SILENT:
-            print("Your model was successfully uploaded to Scailable!")
-            print("NOTE: After transpiling, we will send you an email and your model will be available at "
-                  "https://admin.sclbl.net.")
-            print("Or, alternatively, you can use the 'endpoints()' function to list all your uploaded models. \n")
-
-        # remove bundle:
-        if not _keep:
-            _gzip_delete()
-
-        return True
-
-    else:
-        return False
-
-
-# update updates an existing model
-def update(mod, features, cfid, docs={}, email=True, model_type="sklearn", _keep=False) -> bool:
-    """Updates an already existing model.
 
-    The update function is similar to the upload function in most respects (so, see its docs),
-    but instead of creating a new endpoint it overwrites the docs and model of an already exisitng
-    endpoint. Thus, there is an additional argument "cfid" providing the computeFunction Id
-    of the endpoint that needs to be updated. Use sp.list_models() to get a list of your already
-    existing endpoints. Just like the upload function, update is a wrapper for:
-     - update_sklearn(mod, feature_vector, cfid, docs={}, email=True, _keep=False)
-     - update_onnx(path, cfid, example="", docs={}, email=True)
 
-    Note: If you solely want to change the documentation of an endpoint, you can either use the
-        update_docs() function or the online admin interface at https://admin.sclble.net.
-
-    Args:
-        mod: The model to be uploaded (type="sklearn" OR the path to the stored ONNX file (type="onnx").
-        features:
-            - An example feature_vector for your model (type="sklearn" only).
-            (i.e., the first row of your training data X obtained using row = X[0,:])
-            - The input str (binary) to the onnx model (type="onnx" only). Can be an empty string.
-        cfid: a string with a valid computeFunction ID.
-        docs: A dict{} containing the fields 'name' and 'documentation'.
-        email: Bool indicating whether a confirmation email of a successful conversion should be send. Default True.
-        model_type: String indicating the type of model. Currently with options "sklearn" or "onnx". Default "sklearn"
-        _keep: Bool indicating whether the .gzipped file should be retained (type="sklearn" only). Default False.
-
-    Returns:
-        False if upload failed, true otherwise
-
-    Raises  (in debug mode):
-        UploadModelError if unable to successfully bundle and upload the model.
-    """
-    if model_type == "sklearn":
-        if features == "":
-            if not glob.SILENT:
-                print("FATAL: You cannot upload a sklearn model with an empty string as feature vector.")
-            if glob.DEBUG:
-                raise UploadModelError("Cannot upload sklearn model with empty string as feature vector.")
-            return False
-        if not update_sklearn(mod, features, cfid, docs=docs, email=email, _keep=_keep):
-            return False
-    elif model_type == "onnx":
-        if not update_onnx(mod, cfid, example=features, docs=docs, email=email):
-            return False
-    else:
-        if glob.DEBUG:
-            raise UploadModelError("Please specify a valid model type.")
-        return False
-
-    return True
 
 
 # update_onnx updates an onnx model
 def update_onnx(path, cfid, example="", docs={}, email=True) -> bool:
     """upload_onnx updates a fitted onnx model to Scailable.
 
     The update function is similar to the upload function in most respects (so, see its docs),
@@ -600,16 +283,16 @@
             'Authorization': glob.JWT_TOKEN,
         }
 
         try:
             response = requests.put(url, headers=headers, data=payload, files=files)
         except Exception as e:
             if not glob.SILENT:
-                print("FATAL: Unable to carry out the update request: the toolchain is not available. \n"
-                      "Your model has not been updated. \n")
+                print(f"FATAL: Unable to carry out the update request: the toolchain is not available. \n"
+                      f"Your model has not been updated. {url}, user id: {glob.JWT_USER_ID}, cfid:  {cfid}\n")
             if glob.DEBUG:
                 raise UploadModelError("We were unable to obtain JWT authorization: " + str(e))
             return False
 
         # Error handling
         try:
             response_data = json.loads(response.text)
@@ -639,205 +322,14 @@
 
         return True
 
     else:
         return False
 
 
-# update_sklearn updates an sklearn model
-def update_sklearn(mod, feature_vector, cfid, docs={}, email=True, _keep=False) -> bool:
-    """Updates an already existing sklearn model.
-
-    The update function is similar to the upload function in most respects (so, see its docs),
-    but instead of creating a new endpoint it overwrites the docs and model of an already existing
-    endpoint. Thus, there is an additional argument "cfid" providing the computeFunction Id
-    of the endpoint that needs to be updated. Use sp.list_models() to get a list of your already
-    existing endpoints.
-
-    Note: If you solely want to change the documentation of an endpoint, you can either use the
-        update_docs() function or the online admin interface at https://admin.sclble.net.
-
-    Args:
-        mod: The model to be uploaded.
-        feature_vector: An example feature_vector for your model.
-            (i.e., the first row of your training data X obtained using row = X[0,:])
-        cfid: a string with a valid computeFunction ID.
-        docs: A dict{} containing the fields 'name' and 'documentation'. Default {}.
-        email: Bool indicating whether a confirmation email of a successful conversion should be send. Default True.
-        _keep: Bool indicating whether the .gzipped file should be retained. Default False.
-
-    Returns:
-        False if upload failed, true otherwise
-
-    Raises  (in debug mode):
-        UploadModelError if unable to successfully bundle and upload the model.
-    """
-    if glob.DEBUG:
-        print("We are checking your updated sklearn model...")
-
-    bundle = {}
-
-    # Check model:
-    if not _check_model(mod):
-        if not glob.SILENT:
-            print("FATAL: The model you are trying to upload is not (yet) supported or has not been fitted. \n"
-                  "Please see README.md for a list of supported models. \n"
-                  "Your models has not been uploaded. \n")
-        if glob.DEBUG:
-            raise UploadModelError("The submitted model is not supported.")
-        return False
-    bundle['fitted_model'] = mod
-
-    # check input vector and generate an example:
-    bundle['example'] = {}
-    if feature_vector.any():
-        # try prediction
-        try:
-            output = _predict(mod, feature_vector)  # predict raises error if unable to generate predcition
-        except Exception as e:
-            if not glob.SILENT:
-                print("FATAL: We were unable to create an example inference. \n"
-                      "Your model has not been updated. \n")
-            if glob.DEBUG:
-                raise UploadModelError("Unable to generate prediction: " + str(e))
-            return False
-        # format data:
-        input_str: str = '[[%s]]' % ', '.join([str(i) for i in feature_vector.tolist()])
-        example = {'input': input_str, "output": json.dumps(output)}
-        bundle['example'] = example
-    else:
-        if not glob.SILENT:
-            print("FATAL: You did not provide a required example instance. (see docs). \n"
-                  "Your model has not been updated. \n")
-        return False
-
-    # check the docs:
-    bundle['docs'] = {}
-    docs_update = True
-    if docs:
-        bundle['docs'] = docs
-    else:
-        docs_update = False
-        if not glob.SILENT:
-            print("WARNING: You did not provide any documentation. \n"
-                  "We will only update the .wasm model, not the documentation.")
-
-    # check authorization:
-    auth = _check_jwt()
-    if not auth:
-        if not glob.SILENT:
-            print("FATAL: We were unable to obtain JWT authorization for your account. \n"
-                  "Your model has not been updated. \n")
-        if glob.DEBUG:
-            raise UploadModelError("We were unable to obtain JWT authorization.")
-        return False
-
-    # get system information
-    bundle['system_info'] = _get_system_info()
-
-    # gzip the bundle
-    if not _gzip_save(bundle):
-        if not glob.SILENT:
-            print("FATAL: We were unable to gzip your model bundle. \n"
-                  "Your model has not been updated. \n")
-        if glob.DEBUG:
-            raise UploadModelError("We were unable to save the bundle.")
-        return False
-
-    # all ok, upload:
-    if auth:
-
-        url = glob.TOOLCHAIN_URL + "/upload/" + glob.JWT_USER_ID + "/" + cfid
-
-        # Map python package to the right toolchain:
-        pkg_name = _get_model_package(mod)
-        toolchain_name = ""
-        if pkg_name == "sklearn":
-            toolchain_name = "sklearn"
-        elif pkg_name == "statsmodels":
-            toolchain_name = "sklearn"
-        elif pkg_name == "xgboost":
-            toolchain_name = "sklearn"
-        elif pkg_name == "lightgbm":
-            toolchain_name = "sklearn"
-
-        # Setup the actual request
-        data: dict = {
-            'email': email,
-            'package': __version__,
-            'toolchain': toolchain_name,
-            'name': bundle['docs'].get('name', ""),
-            'docs': bundle['docs'].get('documentation', ""),
-            'updateDocs': docs_update,
-            'exampleInput': bundle['example'].get('input', "[]"),
-            'exampleOutput': bundle['example'].get('output', "[]")
-        }
-        payload: dict = {
-            'data': json.dumps(data)
-        }
-
-        files = [('bundle', open(glob.GZIP_BUNDLE, 'rb'))]
-        headers = {
-            'Authorization': glob.JWT_TOKEN
-        }
-
-        # Do the request (and make sure to delete the gzip if errors occur)
-        try:
-            response = requests.put(url, headers=headers, data=payload, files=files)
-        except Exception as e:
-            if not glob.SILENT:
-                print("FATAL: Unable to carry out the upload request: the toolchain is not available. \n"
-                      "Your model has not been updated. \n")
-            if not _keep:
-                _gzip_delete()
-            if glob.DEBUG:
-                raise UploadModelError("We were unable to obtain JWT authorization: " + str(e))
-            return False
-
-        # Error handling
-        try:
-            response_data = json.loads(response.text)
-        except Exception as e:
-            if not glob.SILENT:
-                print("FATAL: We did not receive a valid JSON response from the toolchain-server. \n"
-                      "Your model has not been updated. \n")
-            if not _keep:
-                _gzip_delete()
-            if glob.DEBUG:
-                raise UploadModelError("We did not receive a valid response from the server: " + str(e))
-            return False
-
-        if response_data['error']:
-            if not glob.SILENT:
-                print("FATAL: An error was returned by the server. \n"
-                      "Your model has not been updated. \n")
-            if not _keep:
-                _gzip_delete()
-            if glob.DEBUG:
-                raise UploadModelError("We did not receive a valid response from the server: " + response_data['error'])
-            return False
-
-        if glob.DEBUG:
-            print("The following content has been send to the toolchain server:")
-            print(bundle)
-
-        # user feedback:
-        if not glob.SILENT:
-            print("Your model was successfully submitted for an update. \n")
-
-        # remove bundle:
-        if not _keep:
-            _gzip_delete()
-
-        return True
-
-    else:
-        return False
-
-
 # update_docs updates the docs of a given model (but not the model itself:
 def update_docs(cfid, docs) -> bool:
     """Updates the documentation of an already existing model
 
     The update_docs function can be used to upload the documentation of an already existing model
     by simply providing the cfid and the new docs object.
 
@@ -849,14 +341,15 @@
         False if upload failed, true otherwise
 
     Raises  (in debug mode):
         UploadModelError if unable to successfully bundle and upload the model.
     """
 
     # check the docs:
+    print(docs)
     name = docs.get('name', "")
     if name == "":
         print("FATAL: Please make sure to add a name to your documentation (using the 'name') field \n"
               "Your model documentation has not been updated. \n")
         return False
     documentation = docs.get('documentation', "")
     if documentation == "":
@@ -898,16 +391,17 @@
         }
 
         # Do the request (and make sure to delete the gzip if errors occur)
         try:
             response = requests.put(url, headers=headers, data=payload, files=files)
         except Exception as e:
             if not glob.SILENT:
-                print("FATAL: Unable to carry out the upload request: the toolchain is not available. \n"
-                      "Your model documentation has not been updated. \n")
+                print(f"FATAL: Unable to carry out the upload request: the toolchain is not available. \n"
+                      "Your model documentation has not been updated. PLACE 2 URL: {url} \n")
+                print(url)
             if glob.DEBUG:
                 raise UploadModelError("We were unable to obtain JWT authorization: " + str(e))
             return False
 
         # Error handling
         try:
             response_data = json.loads(response.text)
@@ -1269,145 +763,14 @@
         return False
 
     if glob.DEBUG:
         print(result)
 
     return True
 
-
-# run generates inference for a sklearn model
-def run(cfid, feature_vector, fv_type="auto") -> dict:
-    """run a sklearn model that has previously been uploaded to Scailable.
-
-    The run function allows a user to execute a sklearn task that has been uploaded to Scailable and
-    for which a REST endpoint is thus available.
-
-    The user specifies the compute-function id, and the desired input, and receives the resulting output
-    (often the inference generated by a model)
-
-    Note: This function returns the result of the following code which can be embedded in any python project
-    to consume a Scailable REST endpoint without including the sclblpy package:
-
-    # import requests
-    #
-    # url = "https://taskmanager.sclbl.net:8080/task/" + cfid
-    #
-    # data = ",".join(map(str, feature_vector))
-    #
-    # payload = "{\"input\":
-    #   {\"content-type\":\"json\",
-    #   \"location\":\"embedded\",
-    #   \"data\":\"{
-    #       \\\"input\\\": [[" + data + "]]}\"},
-    #   \"output\":{
-    #       \"content-type\":\"json\",
-    #       \"location\":\"echo\"},
-    #       \"control\":1,
-    #       \"properties\":{\"language\":\"WASM\"}}"
-    #
-    # headers = {
-    #     'Content-Type': 'application/x-www-form-urlencoded'
-    # }
-    #
-    # response = requests.request("POST", url, headers=headers, data=payload)
-    #
-
-    Args:
-        cfid: String containing the compute-function ID of an existing Scailable endpoint
-        feature_vector: The input for the compute-function
-            (i.e., the a single row of data X obtained using row = X[0,:]).
-        fv_type: String indicating the type of input ("csv", "pb", or "raw"). Default is "auto".
-            (when set to "auto" the function will try to determine the input type).
-
-
-    Returns:
-        False if the call fails, a dict containing the server response otherwise.
-
-    Raises  (in debug mode):
-        RunTaskError if unable to run the compute function.
-    """
-
-    # Check the cfid:
-    if not cfid:
-        if not glob.SILENT:
-            print("Please provide a valid cfid. Abort.")
-        return False
-
-    # Create the ednpoint url:
-    url = glob.TASK_MANAGER_URL + "/task/" + cfid
-
-    # Determine the input vector type:
-    if fv_type == "auto":
-        fv_type = _check_input_type(feature_vector)
-
-    if not fv_type or fv_type not in ["csv", "pb", "raw"]:
-        if not glob.SILENT:
-            print("Your feature_vector input type is invalid or cannot be determined. Abort.")
-        return False
-
-    # Run:
-    response = ""
-    if fv_type == "csv":
-        try:
-            response = _run_csv(url, feature_vector)
-        except Exception as e:
-            if not glob.SILENT:
-                print("Run csv error: " + str(e))
-            if glob.DEBUG:
-                raise RunTaskError("Run csv error:" + str(e))
-            return False
-    elif fv_type == "raw":
-        try:
-            response = _run_raw(url, feature_vector)
-        except Exception as e:
-            if not glob.SILENT:
-                print("Run raw error: " + str(e))
-            if glob.DEBUG:
-                raise RunTaskError("Run raw error:" + str(e))
-            return False
-    elif fv_type == "pb":
-        try:
-            response = _run_pb(url, feature_vector)
-        except Exception as e:
-            if not glob.SILENT:
-                print("Run pb error: " + str(e))
-            if glob.DEBUG:
-                raise RunTaskError("Run pb error:" + str(e))
-            return False
-
-    # Check:
-    if response == "":
-        if not glob.SILENT:
-            print("An error occurred while running, the response is empty.")
-        if glob.DEBUG:
-            raise RunTaskError("An error occurred while running, the response is empty.")
-        return False
-
-    # Parse:
-    try:
-        json_string = response.text
-    except Exception as e:
-        if not glob.SILENT:
-            print("We were unable to parse server response to output. " + str(e))
-        if glob.DEBUG:
-            raise RunTaskError("We were unable to parse server response to output. " + str(e))
-        return False
-
-    try:
-        output = json.loads(json_string)
-    except Exception as e:
-        if not glob.SILENT:
-            print("We were unable to parse server response to json. " + str(e))
-        if glob.DEBUG:
-            raise RunTaskError("We were unable to parse server response to json. " + str(e))
-        return False
-
-    return output
-
-
 # models lists the models / endpoints for the current user.
 def models(offset=0, limit=20, _verbose=True, _return=False) -> dict:
     """ Print or return the endpoints available for the current user.
 
     Simple wrapper for the endpoints() function.
 
     Args:
@@ -1654,30 +1017,14 @@
 
     """
     print("Printing user feedback set to 'True'.")
     glob.SILENT = False
     return True
 
 
-# list_models lists all supported sklearn models
-def list_models() -> dict:
-    """Print or return a list of all supported models.
-
-    Returns:
-        A dictionary detailing the supported models
-    """
-    if not glob.SUPPORTED_MODELS:
-        _load_supported_models()
-
-    if not glob.SILENT:
-        print("Currently supported models:")
-        print(json.dumps(glob.SUPPORTED_MODELS, sort_keys=True, indent=4))
-
-    return glob.SUPPORTED_MODELS
-
 
 # _set_toolchain_URL sets the location of the toolchain (for local testing)
 def _set_toolchain_URL(url: str) -> str:
     """Change the location of the toolchain server.
 
     This function is internal and should not be used by average users of the package. However,
     it is useful for trouble-shooting the package either locally or on development servers.
```

### Comparing `sclblpy-0.1.7/setup.py` & `sclblpy-0.1.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,26 +7,25 @@
 exec(open('sclblpy/version.py').read())
 
 setuptools.setup(
     name="sclblpy",
     version=__version__,
     author="Maurits Kaptein",
     author_email="maurits.kaptein@scailable.net",
-    description="Python package for uploading sklearn and onnx models to Scailable toolchain.",
+    description="Python package for uploading onnx models to Scailable toolchain.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="https://github.com/scailable/sclblpy/",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'numpy',
         'requests',
         'uuid',
-        'sklearn',
       ],
     python_requires='>=3.7',
 )
```

### Comparing `sclblpy-0.1.7/test/test_bundle.py` & `sclblpy-0.1.8/test/test_bundle.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Simple unit tests for _bundly.py
 from sclblpy._bundle import _gzip_save, _gzip_load, _gzip_delete
 
 # Script settings:
 from sclblpy.main import _toggle_debug_mode, stop_print
 
-RUN_TESTS = False  # Prevent unintended testing
-DEBUG = False  # Set to debug mode; if true it will raise exceptions
-PRINTING = False  # Toggle printing on and off.
+RUN_TESTS = 1  # Prevent unintended testing
+DEBUG = 1  # Set to debug mode; if true it will raise exceptions
+PRINTING = 1  # Toggle printing on and off.
 
 def test_gzip_save():
     """Test gzip save. """
     obj = {}
     obj["model_fit"] = "adfsdlafalskdf"
     obj["example"] = "model"
```

### Comparing `sclblpy-0.1.7/test/test_jwt.py` & `sclblpy-0.1.8/test/test_jwt.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 from sclblpy import _set_toolchain_URL, _set_usermanager_URL, stop_print
 from sclblpy._jwt import _check_jwt, _sign_in, _remove_credentials, _get_user_details
 from sclblpy.errors import JWTError
 from sclblpy.main import _toggle_debug_mode
 
 # Script settings:
-RUN_TESTS = False  # Prevent unintended testing
-DEBUG = False  # Set to debug mode; if true it will raise exceptions
-PRINTING = True  # Toggle printing on and off.
-ADMIN_URL = "http://localhost:8008"  # Location of admin for this test
-TOOLCHAIN_URL = "http://localhost:8010"  # Location of toolchain for this test
-
-# For the tests to pass we need a valid username and password:
-USERNAME = "maurits@mauritskaptein.com"
-PASSWORD = "test"
+RUN_TESTS = 1  # Prevent unintended testing
+DEBUG = 0  # Set to debug mode; if true it will raise exceptions
+PRINTING = 1  # Toggle printing on and off.
+ADMIN_URL = "https://usermanager.sclbl.net"  # Location of admin for this test
+TOOLCHAIN_URL = "https://toolchain.sclbl.net"  # Location of toolchain for this test
+
+# For the tests to pass we need a valid email and password:
+EMAIL = "email-here"
+PASSWORD = "password-here"
 
 
 def test_JWT():
     """ Test __check_jwt() function """
 
     assert _check_jwt(seconds_refresh=2, seconds_renew=3) is True, "This should be true with the right credentials"
 
@@ -35,27 +35,27 @@
     assert _check_jwt(seconds_refresh=2, seconds_renew=3) is True, "This should be true with the right credentials"
 
 
 def test_signin():
     """Test __signin() function"""
 
     # Try empty
-    username: str = ""
+    email: str = ""
     password: str = ""
-    assert _sign_in(username, password) is False, "This should not log in"
+    assert _sign_in(email, password) is False, "This should not log in"
 
     # Try invalid
-    username = "blabla@blabla.com"
+    email = "blabla@blabla.com"
     password = "not-a-valid-password"
-    assert _sign_in(username, password) is False, "This should not log in 2"
+    assert _sign_in(email, password) is False, "This should not log in 2"
 
     # Try valid
-    username = USERNAME
+    email = EMAIL
     password = PASSWORD
-    assert _sign_in(username, password) is True, "This should sign in (if the username and pass indeed exist)."
+    assert _sign_in(email, password) is True, "This should sign in (if the email and pass indeed exist)."
 
 
 def test_get_user_details():
     """ Test of get user details"""
     assert type(_get_user_details()) is dict, "This should be a dict"
     assert _remove_credentials() is True, "This should be True"
     assert type(_get_user_details()) is dict, "This should be a dict"
```

### Comparing `sclblpy-0.1.7/test/test_main.py` & `sclblpy-0.1.8/test/test_main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,95 +1,56 @@
-import os
 import time
 
-from sclblpy._bundle import _gzip_load, _gzip_delete
 from sclblpy._jwt import _get_user_details
-from sclblpy.main import remove_credentials, upload, endpoints, delete_endpoint, _set_toolchain_URL, \
-    _set_usermanager_URL, list_models, start_print, stop_print, _toggle_debug_mode, update, update_docs, run, \
+from sclblpy.main import remove_credentials, upload_onnx, endpoints, delete_endpoint, _set_toolchain_URL, \
+    _set_usermanager_URL, update_onnx, stop_print, _toggle_debug_mode, update_docs, run, \
     _set_taskmanager_URL, models, devices, delete_device, assignments, assign, delete_assignment, delete_model
 
-import sclblpy._globals as glob
 
-import numpy as np
-from sklearn import svm
-from sklearn import datasets
-
-# Script settings:
-RUN_TESTS = False  # Prevent unintended testing
+RUN_TESTS = True  # Prevent unintended testing
 DEBUG = True  # Set to debug mode; if true it will raise exceptions
 PRINTING = True  # Toggle printing on and off.
-ADMIN_URL = "http://localhost:8008"  # Location of admin for this test
-TOOLCHAIN_URL = "http://localhost:8010"  # Location of toolchain for this test
-TASKMANAGER_URL = "http://localhost:8080"
-
+ADMIN_URL = "https://usermanager.sclbl.net"  # Location of admin for this test
+TOOLCHAIN_URL = "https://toolchain.sclbl.net"  # Location of toolchain for this test
 
-def test_upload():
-    """ Test the upload function (sklearn and onnx"""
-
-    # Start fitting a simple model, no feature vecto
-    clf = svm.SVC()
-    X, y = datasets.load_iris(return_X_y=True)
-    clf.fit(X, y)
-    assert upload(clf, np.empty(0)) is False, "No valid feature vector."
 
+def test_upload_onnx():
+    """ Test the upload function (onnx)"""
     # Add docs
     docs = {}
-    docs['name'] = "Name of model"
-    docs['documentation'] = "A long .md thing...."
-    assert upload(clf, np.empty(0), docs=docs) is False, "No valid feature vector."
-
-    # Valid
-    row = X[130, :]
-    assert upload(clf, row, docs=docs) is True, "SKlearn upload test failed."
 
     # ONNX
     docs['name'] = "Name of ONNX model"
     docs['documentation'] = "A long .md thing...."
-    check = upload("../test/files/model.onnx", "", docs, model_type="onnx")
+    check = upload_onnx("../test/files/model.onnx", "", docs)
     assert check is True, "ONNX upload test failed."
 
 
 def test_update():
-    """ Test the update function (sklearn & onnx"""
-
-    # Start fitting a simple model, no feature vecto
-    clf = svm.SVC()
-    X, y = datasets.load_iris(return_X_y=True)
-    clf.fit(X, y)
+    """ Test the update function (onnx)"""
 
     # Add and feature vector
     docs = {}
     docs['name'] = "Name of model - UPDATED"
     docs['documentation'] = "A long .md thing.... UPDATED"
-    row = X[130, :]
 
     # Get an existing endpoint to update
-    try:
-        cfid = endpoints(_verbose=False, _return=True)[0]["cfid"]
-    except Exception as e:
-        print("No endpoint to overwrite found")
-        assert False is True, "No endpoint found for overwrite test."
-
-    print("Updating: " + cfid)
+    print(endpoints(_verbose=False, _return=True))
 
-    # Overwrite without docs
-    result = update(clf, row, cfid, docs={})
-    assert result is True, "Sklearn update failed."
-
-    # Get another endpoint to update
-    try:
-        cfid = endpoints(_verbose=False, _return=True)[1]["cfid"]
-    except Exception as e:
-        print("No endpoint to overwrite found 2")
-        assert False == True, "no endpoint found for overwrite test 2"
+    # try except is a bit unusual in a test (as any fail in e.g. endpoints or the indexing will lead to the same output)
+    #try:
+    cfid = endpoints(_verbose=False, _return=True)[0]["cfid"]
+    #except Exception as e:
+    #    print("No endpoint to overwrite found")
+    #    assert False is True, "No endpoint found for overwrite test."
 
     print("Updating: " + cfid)
 
     # Overwrite with valid docs:
-    result = update("../test/files/model.onnx", "", cfid, docs=docs, model_type="onnx")
+    result = update_onnx("../test/files/model.onnx", cfid=cfid,example="", docs=docs) #
     assert result is True, "ONNX update failed."
 
 
 def test_update_docs():
     """ Test the update docs function """
 
     # Get an existing endpoint to update
@@ -159,24 +120,14 @@
     except Exception as e:
         # Effectively there was no endpoint...
         print("No endpoints to remove; test not run.")
 
     if cfid:
         assert delete_endpoint(cfid) is True, "Should be able to delete an endpoint."
 
-    # delete model
-    ep = endpoints(_return=True)
-    try:
-        cfid = ep[0]['cfid']
-    except Exception as e:
-        # Effectively there was no model...
-        print("No endpoints to remove; test not run.")
-
-    if cfid:
-        assert delete_model(cfid) is True, "Should be able to delete a model."
 
 
 def test_devices_functions():
     """ test get, delete for devices """
 
     # Get existing devices
     device_list = devices(_return=True)
@@ -196,51 +147,29 @@
 
     # check counts:
     device_list2 = devices(_return=True)
     count2 = len(device_list2)
     assert (count2 == (count-1)) is True, "The deleted device count is not correct."
 
 
-# More obscure tests / please read docstrings and make sure settings are correct.
-def test_run():
-    """ Test running an endpoint
-    Note: Only works with valid existing cfid and compatible fv.
-    """
-    cfid = "e871d8e5-b2e2-11ea-a47d-9600004e79cc"
-
-    fv = [1, 2]
-
-    result = run(cfid, fv)
 
-    assert result is not False, "Error in running test; are the cfid and feature_vector ok?"
-    print(result)
-
-    if result['statusCode'] == 1:
-        print(result['result'])
 
 
 def test_remove_credentials():  # Also tested in JWT.
     """ Test of get user details"""
     assert type(_get_user_details()) is dict, "This should be a dict."
     assert remove_credentials(True) is True, "This should return true if removed."
 
 
 def test_setting_URLs():
     """ Test url setters: """
     _set_toolchain_URL(TOOLCHAIN_URL)
     _set_usermanager_URL(ADMIN_URL)
-    _set_taskmanager_URL(TASKMANAGER_URL)
 
 
-def test_user_utils():
-    start_print()
-    list_models()
-    stop_print()
-    list_models()
-    start_print()
 
 
 # Run tests
 if __name__ == '__main__':
 
     if not RUN_TESTS:
         print("Not running tests.")
@@ -254,24 +183,39 @@
 
     if DEBUG:
         _toggle_debug_mode()  # serves as test
 
     print("Running simple functional tests of main.py")
     print("===============================")
 
-    test_upload()  # upload sklearn and onnx test
+    test_upload_onnx()  # upload an onnx test
 
     print("Wait, toolchain needs to finish....")
-    time.sleep(10)
+    time.sleep(25)
+    print(" waited for 25 seconds")
 
-    test_update()  # update sklearn and onnx test
+    print('testing update \n\n')
+    test_update()  # update an onnx test
+    print('testing update docs \n\n')
     test_update_docs()  # update only docs test
+    print('testing assign functions \n\n')
     test_assign_functions()  # test creating and removing assignments
+
+
+    # The test below deletes the device registration, so it's commented out to keep the tests repeatable
+
+    print('testing endpoint functions \n\n')
+    print(endpoints(_return=True))
     test_endpoints_functions()  # test getting and deleting models
-    test_devices_functions()  # test device get and delete
+
+    #print('testing device functions \n\n')
+    #test_devices_functions()  # test device get and delete
+
+
+    ## MISSSING: REMOVE THE CREATED MODELS!!!
 
     # More obscure tests, not run by default / commented out
     #test_user_utils()
     #test_remove_credentials()
     #test_run()
 
     print("===============================")
```

