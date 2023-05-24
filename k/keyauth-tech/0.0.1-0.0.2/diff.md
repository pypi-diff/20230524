# Comparing `tmp/keyauth-tech-0.0.1.tar.gz` & `tmp/keyauth-tech-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyauth-tech-0.0.1.tar", last modified: Wed May 24 11:21:23 2023, max compression
+gzip compressed data, was "keyauth-tech-0.0.2.tar", last modified: Wed May 24 11:27:01 2023, max compression
```

## Comparing `keyauth-tech-0.0.1.tar` & `keyauth-tech-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-05-24 11:21:23.674823 keyauth-tech-0.0.1/
--rw-r--r--   0 ecom       (502) staff       (20)       77 2023-05-24 11:05:53.000000 keyauth-tech-0.0.1/CHANGELOG.txt
--rw-r--r--   0 ecom       (502) staff       (20)     1046 2023-05-24 11:06:49.000000 keyauth-tech-0.0.1/LICENSE.txt
--rw-r--r--   0 ecom       (502) staff       (20)       25 2023-05-24 11:06:11.000000 keyauth-tech-0.0.1/MANIFEST.in
--rw-r--r--   0 ecom       (502) staff       (20)      798 2023-05-24 11:21:23.674683 keyauth-tech-0.0.1/PKG-INFO
--rw-r--r--   0 ecom       (502) staff       (20)      116 2023-05-24 11:09:48.000000 keyauth-tech-0.0.1/README.txt
-drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-05-24 11:21:23.673665 keyauth-tech-0.0.1/keyauth/
--rw-r--r--   0 ecom       (502) staff       (20)     2342 2023-05-24 11:03:49.000000 keyauth-tech-0.0.1/keyauth/__init__.py
-drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-05-24 11:21:23.674483 keyauth-tech-0.0.1/keyauth_tech.egg-info/
--rw-r--r--   0 ecom       (502) staff       (20)      798 2023-05-24 11:21:23.000000 keyauth-tech-0.0.1/keyauth_tech.egg-info/PKG-INFO
--rw-r--r--   0 ecom       (502) staff       (20)      256 2023-05-24 11:21:23.000000 keyauth-tech-0.0.1/keyauth_tech.egg-info/SOURCES.txt
--rw-r--r--   0 ecom       (502) staff       (20)        1 2023-05-24 11:21:23.000000 keyauth-tech-0.0.1/keyauth_tech.egg-info/dependency_links.txt
--rw-r--r--   0 ecom       (502) staff       (20)       38 2023-05-24 11:21:23.000000 keyauth-tech-0.0.1/keyauth_tech.egg-info/requires.txt
--rw-r--r--   0 ecom       (502) staff       (20)        8 2023-05-24 11:21:23.000000 keyauth-tech-0.0.1/keyauth_tech.egg-info/top_level.txt
--rw-r--r--   0 ecom       (502) staff       (20)       38 2023-05-24 11:21:23.674865 keyauth-tech-0.0.1/setup.cfg
--rw-r--r--   0 ecom       (502) staff       (20)      837 2023-05-24 11:20:51.000000 keyauth-tech-0.0.1/setup.py
+drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-05-24 11:27:01.348130 keyauth-tech-0.0.2/
+-rw-r--r--   0 ecom       (502) staff       (20)       94 2023-05-24 11:26:55.000000 keyauth-tech-0.0.2/CHANGELOG.txt
+-rw-r--r--   0 ecom       (502) staff       (20)     1046 2023-05-24 11:06:49.000000 keyauth-tech-0.0.2/LICENSE.txt
+-rw-r--r--   0 ecom       (502) staff       (20)       25 2023-05-24 11:06:11.000000 keyauth-tech-0.0.2/MANIFEST.in
+-rw-r--r--   0 ecom       (502) staff       (20)      815 2023-05-24 11:27:01.347980 keyauth-tech-0.0.2/PKG-INFO
+-rw-r--r--   0 ecom       (502) staff       (20)      116 2023-05-24 11:09:48.000000 keyauth-tech-0.0.2/README.txt
+drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-05-24 11:27:01.347071 keyauth-tech-0.0.2/keyauth/
+-rw-r--r--   0 ecom       (502) staff       (20)     2342 2023-05-24 11:03:49.000000 keyauth-tech-0.0.2/keyauth/__init__.py
+drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-05-24 11:27:01.347766 keyauth-tech-0.0.2/keyauth_tech.egg-info/
+-rw-r--r--   0 ecom       (502) staff       (20)      815 2023-05-24 11:27:01.000000 keyauth-tech-0.0.2/keyauth_tech.egg-info/PKG-INFO
+-rw-r--r--   0 ecom       (502) staff       (20)      264 2023-05-24 11:27:01.000000 keyauth-tech-0.0.2/keyauth_tech.egg-info/SOURCES.txt
+-rw-r--r--   0 ecom       (502) staff       (20)        1 2023-05-24 11:27:01.000000 keyauth-tech-0.0.2/keyauth_tech.egg-info/dependency_links.txt
+-rw-r--r--   0 ecom       (502) staff       (20)       18 2023-05-24 11:27:01.000000 keyauth-tech-0.0.2/keyauth_tech.egg-info/requires.txt
+-rw-r--r--   0 ecom       (502) staff       (20)        8 2023-05-24 11:27:01.000000 keyauth-tech-0.0.2/keyauth_tech.egg-info/top_level.txt
+-rw-r--r--   0 ecom       (502) staff       (20)     2102 2023-05-24 11:25:21.000000 keyauth-tech-0.0.2/req.txt
+-rw-r--r--   0 ecom       (502) staff       (20)       38 2023-05-24 11:27:01.348170 keyauth-tech-0.0.2/setup.cfg
+-rw-r--r--   0 ecom       (502) staff       (20)      811 2023-05-24 11:26:34.000000 keyauth-tech-0.0.2/setup.py
```

### Comparing `keyauth-tech-0.0.1/LICENSE.txt` & `keyauth-tech-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `keyauth-tech-0.0.1/PKG-INFO` & `keyauth-tech-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyauth-tech
-Version: 0.0.1
+Version: 0.0.2
 Summary: An Authentication Tool for Authenticating Users, HWIDs and Licenses to keep your Code secure from malicious actions.
 Home-page: https://keyauth.tech
 Author: Collin Stokes
 Author-email: rehan009a@outlook.com
 License: MIT
 Keywords: authentication
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,10 +15,10 @@
 License-File: LICENSE.txt
 
 An Authentication Tool for Authenticating Users, HWIDs and Licenses to keep your Code secure from malicious actions.
 
 Change Log
 ==========
 
-0.0.1 (24/05/2023)
+0.0.2 (24/05/2023)
 -------------------
-- First Release
+- Fixed Bugs & Issues Installing
```

### Comparing `keyauth-tech-0.0.1/keyauth/__init__.py` & `keyauth-tech-0.0.2/keyauth/__init__.py`

 * *Files identical despite different names*

### Comparing `keyauth-tech-0.0.1/keyauth_tech.egg-info/PKG-INFO` & `keyauth-tech-0.0.2/keyauth_tech.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyauth-tech
-Version: 0.0.1
+Version: 0.0.2
 Summary: An Authentication Tool for Authenticating Users, HWIDs and Licenses to keep your Code secure from malicious actions.
 Home-page: https://keyauth.tech
 Author: Collin Stokes
 Author-email: rehan009a@outlook.com
 License: MIT
 Keywords: authentication
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,10 +15,10 @@
 License-File: LICENSE.txt
 
 An Authentication Tool for Authenticating Users, HWIDs and Licenses to keep your Code secure from malicious actions.
 
 Change Log
 ==========
 
-0.0.1 (24/05/2023)
+0.0.2 (24/05/2023)
 -------------------
-- First Release
+- Fixed Bugs & Issues Installing
```

### Comparing `keyauth-tech-0.0.1/setup.py` & `keyauth-tech-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,19 +6,19 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='keyauth-tech',
-  version='0.0.1',
+  version='0.0.2',
   description='An Authentication Tool for Authenticating Users, HWIDs and Licenses to keep your Code secure from malicious actions.',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='https://keyauth.tech',  
   author='Collin Stokes',
   author_email='rehan009a@outlook.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='authentication', 
   packages=find_packages(),
-  install_requires=['subprocess', 'requests', 'platform', 'colorama'] 
+  install_requires=['requests', 'colorama'] 
 )
```

