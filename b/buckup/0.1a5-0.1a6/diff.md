# Comparing `tmp/buckup-0.1a5.tar.gz` & `tmp/buckup-0.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buckup-0.1a5.tar", last modified: Wed Mar 29 13:56:12 2023, max compression
+gzip compressed data, was "buckup-0.1a6.tar", last modified: Wed May 24 09:50:40 2023, max compression
```

## Comparing `buckup-0.1a5.tar` & `buckup-0.1a6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jake      (1000) jake       (975)        0 2023-03-29 13:56:12.442809 buckup-0.1a5/
--rw-r--r--   0 jake      (1000) jake       (975)     1494 2023-03-15 10:25:28.000000 buckup-0.1a5/LICENSE
--rw-r--r--   0 jake      (1000) jake       (975)     3760 2023-03-29 13:56:12.442809 buckup-0.1a5/PKG-INFO
--rw-r--r--   0 jake      (1000) jake       (975)     2852 2023-03-15 10:25:28.000000 buckup-0.1a5/README.rst
-drwxr-xr-x   0 jake      (1000) jake       (975)        0 2023-03-29 13:56:12.436143 buckup-0.1a5/buckup/
--rw-r--r--   0 jake      (1000) jake       (975)        0 2023-03-29 13:51:29.000000 buckup-0.1a5/buckup/__init__.py
--rw-r--r--   0 jake      (1000) jake       (975)     9648 2023-03-29 13:51:34.000000 buckup-0.1a5/buckup/bucket_creator.py
--rw-r--r--   0 jake      (1000) jake       (975)     8537 2023-03-29 13:51:29.000000 buckup-0.1a5/buckup/command_line.py
--rw-r--r--   0 jake      (1000) jake       (975)      351 2023-03-15 10:25:28.000000 buckup-0.1a5/buckup/exceptions.py
--rw-r--r--   0 jake      (1000) jake       (975)      807 2023-03-15 10:25:28.000000 buckup-0.1a5/buckup/utils.py
-drwxr-xr-x   0 jake      (1000) jake       (975)        0 2023-03-29 13:56:12.442809 buckup-0.1a5/buckup.egg-info/
--rw-r--r--   0 jake      (1000) jake       (975)     3760 2023-03-29 13:56:12.000000 buckup-0.1a5/buckup.egg-info/PKG-INFO
--rw-r--r--   0 jake      (1000) jake       (975)      323 2023-03-29 13:56:12.000000 buckup-0.1a5/buckup.egg-info/SOURCES.txt
--rw-r--r--   0 jake      (1000) jake       (975)        1 2023-03-29 13:56:12.000000 buckup-0.1a5/buckup.egg-info/dependency_links.txt
--rw-r--r--   0 jake      (1000) jake       (975)       52 2023-03-29 13:56:12.000000 buckup-0.1a5/buckup.egg-info/entry_points.txt
--rw-r--r--   0 jake      (1000) jake       (975)        6 2023-03-29 13:56:12.000000 buckup-0.1a5/buckup.egg-info/requires.txt
--rw-r--r--   0 jake      (1000) jake       (975)        7 2023-03-29 13:56:12.000000 buckup-0.1a5/buckup.egg-info/top_level.txt
--rw-r--r--   0 jake      (1000) jake       (975)      981 2023-03-29 13:56:12.446143 buckup-0.1a5/setup.cfg
--rw-r--r--   0 jake      (1000) jake       (975)      130 2023-03-15 10:25:28.000000 buckup-0.1a5/setup.py
+drwxr-xr-x   0 jake      (1000) jake       (975)        0 2023-05-24 09:50:40.232460 buckup-0.1a6/
+-rw-r--r--   0 jake      (1000) jake       (975)     1494 2023-03-15 10:25:28.000000 buckup-0.1a6/LICENSE
+-rw-r--r--   0 jake      (1000) jake       (975)     3943 2023-05-24 09:50:40.232460 buckup-0.1a6/PKG-INFO
+-rw-r--r--   0 jake      (1000) jake       (975)     3035 2023-05-24 09:41:31.000000 buckup-0.1a6/README.rst
+drwxr-xr-x   0 jake      (1000) jake       (975)        0 2023-05-24 09:50:40.229127 buckup-0.1a6/buckup/
+-rw-r--r--   0 jake      (1000) jake       (975)       78 2023-05-24 09:42:01.000000 buckup-0.1a6/buckup/__init__.py
+-rw-r--r--   0 jake      (1000) jake       (975)     9687 2023-05-24 09:41:31.000000 buckup-0.1a6/buckup/bucket_creator.py
+-rw-r--r--   0 jake      (1000) jake       (975)     8995 2023-05-24 09:42:01.000000 buckup-0.1a6/buckup/command_line.py
+-rw-r--r--   0 jake      (1000) jake       (975)      351 2023-03-15 10:25:28.000000 buckup-0.1a6/buckup/exceptions.py
+-rw-r--r--   0 jake      (1000) jake       (975)      807 2023-03-15 10:25:28.000000 buckup-0.1a6/buckup/utils.py
+drwxr-xr-x   0 jake      (1000) jake       (975)        0 2023-05-24 09:50:40.232460 buckup-0.1a6/buckup.egg-info/
+-rw-r--r--   0 jake      (1000) jake       (975)     3943 2023-05-24 09:50:40.000000 buckup-0.1a6/buckup.egg-info/PKG-INFO
+-rw-r--r--   0 jake      (1000) jake       (975)      323 2023-05-24 09:50:40.000000 buckup-0.1a6/buckup.egg-info/SOURCES.txt
+-rw-r--r--   0 jake      (1000) jake       (975)        1 2023-05-24 09:50:40.000000 buckup-0.1a6/buckup.egg-info/dependency_links.txt
+-rw-r--r--   0 jake      (1000) jake       (975)       52 2023-05-24 09:50:40.000000 buckup-0.1a6/buckup.egg-info/entry_points.txt
+-rw-r--r--   0 jake      (1000) jake       (975)        6 2023-05-24 09:50:40.000000 buckup-0.1a6/buckup.egg-info/requires.txt
+-rw-r--r--   0 jake      (1000) jake       (975)        7 2023-05-24 09:50:40.000000 buckup-0.1a6/buckup.egg-info/top_level.txt
+-rw-r--r--   0 jake      (1000) jake       (975)      981 2023-05-24 09:50:40.235794 buckup-0.1a6/setup.cfg
+-rw-r--r--   0 jake      (1000) jake       (975)      130 2023-03-15 10:25:28.000000 buckup-0.1a6/setup.py
```

### Comparing `buckup-0.1a5/LICENSE` & `buckup-0.1a6/LICENSE`

 * *Files identical despite different names*

### Comparing `buckup-0.1a5/PKG-INFO` & `buckup-0.1a6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buckup
-Version: 0.1a5
+Version: 0.1a6
 Summary: Create S3 buckets in seconds from your command line to use on your website.
 Home-page: https://github.com/torchbox/buckup
 Author: Tomasz Knapik
 Author-email: tomasz.knapik@torchbox.com
 Maintainer: Torchbox
 Maintainer-email: info@torchbox.com
 License: BSD 3-Clause License
@@ -69,14 +69,24 @@
 .. code:: sh
 
    cd /tmp
    git clone https://aur.archlinux.org/buckup.git
    cd buckup
    makepkg -si
 
+Homebrew
+~~~~~~~~
+
+Buckup can be installed from Torchbox's `Homebrew tap <https://github.com/torchbox/homebrew-tap>`_.
+
+.. code:: sh
+
+   brew tap torchbox/tap
+   brew install buckup
+
 Development build
 ~~~~~~~~~~~~~~~~~
 
 You can easily install buckup inside a virtual environment and work on it
 there, e.g.
 
 .. code:: sh
```

### Comparing `buckup-0.1a5/README.rst` & `buckup-0.1a6/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,24 @@
 .. code:: sh
 
    cd /tmp
    git clone https://aur.archlinux.org/buckup.git
    cd buckup
    makepkg -si
 
+Homebrew
+~~~~~~~~
+
+Buckup can be installed from Torchbox's `Homebrew tap <https://github.com/torchbox/homebrew-tap>`_.
+
+.. code:: sh
+
+   brew tap torchbox/tap
+   brew install buckup
+
 Development build
 ~~~~~~~~~~~~~~~~~
 
 You can easily install buckup inside a virtual environment and work on it
 there, e.g.
 
 .. code:: sh
```

### Comparing `buckup-0.1a5/buckup/bucket_creator.py` & `buckup-0.1a6/buckup/bucket_creator.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
     def commit(self, data):
         bucket = self.create_bucket(data['bucket_name'], data['region'])
         user = self.create_user(bucket, data['user_name'])
         self.set_bucket_policy(
             bucket,
             user,
+            allow_public_acls=data["allow_public_acls"],
             public_get_object_paths=data.get('public_get_object_paths')
         )
         if data.get('cors_origins'):
             self.set_cors(bucket, data['cors_origins'])
         if data.get('enable_versioning'):
             self.enable_versioning(bucket)
 
@@ -90,15 +91,15 @@
             },
             "Action": "s3:*",
             "Resource": "arn:aws:s3:::{bucket_name}/*".format(
                 bucket_name=bucket.name
             )
         }
 
-    def set_bucket_policy(self, bucket, user, public_get_object_paths=None):
+    def set_bucket_policy(self, bucket, user, allow_public_acls, public_get_object_paths=None):
         policy_statement = []
         public_access = bool(public_get_object_paths)
 
         if public_access:
             policy_statement.append(
                 self.get_bucket_policy_statement_for_get_object(
                     bucket, public_get_object_paths
@@ -121,27 +122,27 @@
                     time.sleep(5)
                     continue
                 raise e
             else:
                 break
         print('Bucket policy set.')
 
-        if public_access:
-            # NB: This API doesn't exist on a `Bucket`
-            self.s3_client.put_public_access_block(
-                Bucket=bucket.name,
-                # Allow policies to provide access to objects, but not ACLs
-                PublicAccessBlockConfiguration={
-                    "BlockPublicAcls": True,
-                    "IgnorePublicAcls": True,
-                    "BlockPublicPolicy": False,
-                    "RestrictPublicBuckets": False
-                }
-            )
-            print('Enabled public access to the bucket.')
+        # NB: This API doesn't exist on a `Bucket`
+        self.s3_client.put_public_access_block(
+            Bucket=bucket.name,
+            PublicAccessBlockConfiguration={
+                "BlockPublicAcls": not allow_public_acls,
+                "IgnorePublicAcls": not allow_public_acls,
+                "BlockPublicPolicy": not public_access,
+                "RestrictPublicBuckets": not public_access
+            }
+        )
+
+        if public_access or allow_public_acls:
+            print('Configured public access to bucket.')
 
     def create_bucket(self, name, region):
         """
         Create bucket of name in the given region.
         """
         create_bucket_kwargs = {}
         create_bucket_config = {}
```

### Comparing `buckup-0.1a5/buckup/command_line.py` & `buckup-0.1a6/buckup/command_line.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .bucket_creator import BucketCreator
 from .exceptions import (
     BucketNameAlreadyInUse, CannotGetCurrentUser, CannotListAccountAliases,
     CredentialsNotFound, InvalidBucketName, InvalidUserName, UserNameTaken
 )
 
 from .utils import CommandLineInterface
+from . import __version__
 
 
 USER_NAME_FORMAT = '{bucket_name}-s3-owner'
 
 
 class BuckupCommandLineInterface(CommandLineInterface):
     def __init__(self, boto3_profile=None, boto3_region=None):
@@ -163,14 +164,20 @@
                 print('If you specify a wildcard, you should not specify '
                       'other paths.\n')
                 continue
             elif paths:
                 break
         self.data['public_get_object_paths'] = paths
 
+    def ask_public_acl(self):
+        self.data['allow_public_acls'] = self.ask_yes_no(
+            'Do you want to allow public ACLs on objects?\n'
+            'This allows access to individual objects to be controlled separately from the bucket policy.'
+        )
+
     def ask_cors(self):
         cors_origins = self.ask(
             'Specify a comma separated list of origins whitelisted for the '
             'CORS,\ne.g. "https://example.com" (not required)'
         ).strip().split(',')
         self.data['cors_origins'] = []
         for origin in cors_origins:
@@ -195,25 +202,32 @@
         self.print_separator()
         self.print_account_information()
         self.print_separator()
         self.ask_bucket_name()
         self.ask_user_name()
         self.ask_enable_versioning()
         self.ask_public_get_object()
+        self.ask_public_acl()
         self.ask_cors()
         self.print_separator()
         if self.ask_summary():
             self.print_separator()
             self.create_bucket()
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
         description='Create S3 bucket with user ready to use on your website.'
     )
+    parser.add_argument(
+        "--version",
+        help="Show version",
+        action="version",
+        version=__version__
+    )
     parser.add_argument('--profile', type=str,
                         help='AWS CLI profile you want to use')
     parser.add_argument('--region', type=str,
                         help='In which region you want to host. It will use '
                              'your default region from the local session if '
                              'not specified.')
     return parser.parse_args()
```

### Comparing `buckup-0.1a5/buckup/utils.py` & `buckup-0.1a6/buckup/utils.py`

 * *Files identical despite different names*

### Comparing `buckup-0.1a5/buckup.egg-info/PKG-INFO` & `buckup-0.1a6/buckup.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buckup
-Version: 0.1a5
+Version: 0.1a6
 Summary: Create S3 buckets in seconds from your command line to use on your website.
 Home-page: https://github.com/torchbox/buckup
 Author: Tomasz Knapik
 Author-email: tomasz.knapik@torchbox.com
 Maintainer: Torchbox
 Maintainer-email: info@torchbox.com
 License: BSD 3-Clause License
@@ -69,14 +69,24 @@
 .. code:: sh
 
    cd /tmp
    git clone https://aur.archlinux.org/buckup.git
    cd buckup
    makepkg -si
 
+Homebrew
+~~~~~~~~
+
+Buckup can be installed from Torchbox's `Homebrew tap <https://github.com/torchbox/homebrew-tap>`_.
+
+.. code:: sh
+
+   brew tap torchbox/tap
+   brew install buckup
+
 Development build
 ~~~~~~~~~~~~~~~~~
 
 You can easily install buckup inside a virtual environment and work on it
 there, e.g.
 
 .. code:: sh
```

### Comparing `buckup-0.1a5/setup.cfg` & `buckup-0.1a6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = buckup
-version = 0.1a5
+version = 0.1a6
 description = Create S3 buckets in seconds from your command line to use on your website.
 long-description = file: README.rst
 maintainer = Torchbox
 maintainer_email = info@torchbox.com
 author = Tomasz Knapik
 author_email = tomasz.knapik@torchbox.com
 url = https://github.com/torchbox/buckup
```

