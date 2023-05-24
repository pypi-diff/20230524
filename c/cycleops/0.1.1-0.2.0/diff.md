# Comparing `tmp/cycleops-0.1.1.tar.gz` & `tmp/cycleops-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycleops-0.1.1.tar", max compression
+gzip compressed data, was "cycleops-0.2.0.tar", max compression
```

## Comparing `cycleops-0.1.1.tar` & `cycleops-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1069 2023-05-09 10:17:07.975552 cycleops-0.1.1/LICENSE
--rw-r--r--   0        0        0     3487 2023-05-09 10:17:07.975552 cycleops-0.1.1/README.md
--rw-r--r--   0        0        0     1125 2023-05-09 10:17:07.975552 cycleops-0.1.1/cycleops/__main__.py
--rw-r--r--   0        0        0      414 2023-05-09 10:17:07.975552 cycleops-0.1.1/cycleops/auth.py
--rw-r--r--   0        0        0     5468 2023-05-09 10:17:07.975552 cycleops-0.1.1/cycleops/client.py
--rw-r--r--   0        0        0     1113 2023-05-09 10:17:07.975552 cycleops-0.1.1/cycleops/exceptions.py
--rw-r--r--   0        0        0     6626 2023-05-09 10:17:07.975552 cycleops-0.1.1/cycleops/services.py
--rw-r--r--   0        0        0     4249 2023-05-09 10:17:07.975552 cycleops-0.1.1/cycleops/setups.py
--rw-r--r--   0        0        0     3047 2023-05-09 10:17:07.975552 cycleops-0.1.1/cycleops/stacks.py
--rw-r--r--   0        0        0      869 2023-05-09 10:17:07.975552 cycleops-0.1.1/cycleops/units.py
--rw-r--r--   0        0        0      972 2023-05-09 10:17:07.975552 cycleops-0.1.1/cycleops/utils.py
--rw-r--r--   0        0        0      556 2023-05-09 10:17:07.975552 cycleops-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4012 1970-01-01 00:00:00.000000 cycleops-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-24 07:58:30.141776 cycleops-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3994 2023-05-24 07:58:30.141776 cycleops-0.2.0/README.md
+-rw-r--r--   0        0        0     1125 2023-05-24 07:58:30.141776 cycleops-0.2.0/cycleops/__main__.py
+-rw-r--r--   0        0        0      414 2023-05-24 07:58:30.141776 cycleops-0.2.0/cycleops/auth.py
+-rw-r--r--   0        0        0     5468 2023-05-24 07:58:30.141776 cycleops-0.2.0/cycleops/client.py
+-rw-r--r--   0        0        0     1113 2023-05-24 07:58:30.141776 cycleops-0.2.0/cycleops/exceptions.py
+-rw-r--r--   0        0        0    12554 2023-05-24 07:58:30.141776 cycleops-0.2.0/cycleops/services.py
+-rw-r--r--   0        0        0     4249 2023-05-24 07:58:30.141776 cycleops-0.2.0/cycleops/setups.py
+-rw-r--r--   0        0        0     3047 2023-05-24 07:58:30.141776 cycleops-0.2.0/cycleops/stacks.py
+-rw-r--r--   0        0        0      869 2023-05-24 07:58:30.141776 cycleops-0.2.0/cycleops/units.py
+-rw-r--r--   0        0        0      972 2023-05-24 07:58:30.141776 cycleops-0.2.0/cycleops/utils.py
+-rw-r--r--   0        0        0      556 2023-05-24 07:58:30.145776 cycleops-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4519 1970-01-01 00:00:00.000000 cycleops-0.2.0/PKG-INFO
```

### Comparing `cycleops-0.1.1/LICENSE` & `cycleops-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cycleops-0.1.1/README.md` & `cycleops-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -76,14 +76,26 @@
 
 #### Delete a service
 
 ```
 cycleops services delete <service_id>
 ```
 
+#### Create a Container
+
+```
+cycleops services create-container <service_id> <container_name> --image <image_name>:<image_tag> --ports <ports>,<ports> --volumes <volume>,<volume>,<volume> --env-file <env_file_path> --command <command>
+```
+
+#### Update a Container
+
+```
+cycleops services update-container <service_id> <container_name> --name <new_container_name> --image <image_name>:<image_tag> --ports <ports>,<ports> --volumes <volume>,<volume>,<volume> --env-file <env_file_path> --command <command>
+```
+
 ### Stacks
 
 #### List your stacks
 
 ```
 cycleops stacks list
 ```
@@ -156,15 +168,15 @@
 
 ```yml
  deploy:
     runs-on: ubuntu-latest
     env:
       CYCLEOPS_API_KEY: ${{ secrets.CYCLEOPS_API_KEY }}
     steps:
-        run: pipx install cycleops
+        run: pip install cycleops
         run: cycleops services update <service_id> --variable containers.0.image=<image_name>
         run: cycleops setups deploy <setup_id>
 ```
 
 ## Example
 
 You can update a service's image and deploy a setup as follows:
```

### Comparing `cycleops-0.1.1/cycleops/__main__.py` & `cycleops-0.2.0/cycleops/__main__.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.1.1/cycleops/client.py` & `cycleops-0.2.0/cycleops/client.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.1.1/cycleops/exceptions.py` & `cycleops-0.2.0/cycleops/exceptions.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.1.1/cycleops/setups.py` & `cycleops-0.2.0/cycleops/setups.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.1.1/cycleops/stacks.py` & `cycleops-0.2.0/cycleops/stacks.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.1.1/cycleops/units.py` & `cycleops-0.2.0/cycleops/units.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.1.1/cycleops/utils.py` & `cycleops-0.2.0/cycleops/utils.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.1.1/pyproject.toml` & `cycleops-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycleops"
-version = "0.1.1"
+version = "0.2.0"
 description = "The official command line interface for Cycleops"
 authors = ["George Margaritis <george@withlogic.co>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `cycleops-0.1.1/PKG-INFO` & `cycleops-0.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycleops
-Version: 0.1.1
+Version: 0.2.0
 Summary: The official command line interface for Cycleops
 License: MIT
 Author: George Margaritis
 Author-email: george@withlogic.co
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -92,14 +92,26 @@
 
 #### Delete a service
 
 ```
 cycleops services delete <service_id>
 ```
 
+#### Create a Container
+
+```
+cycleops services create-container <service_id> <container_name> --image <image_name>:<image_tag> --ports <ports>,<ports> --volumes <volume>,<volume>,<volume> --env-file <env_file_path> --command <command>
+```
+
+#### Update a Container
+
+```
+cycleops services update-container <service_id> <container_name> --name <new_container_name> --image <image_name>:<image_tag> --ports <ports>,<ports> --volumes <volume>,<volume>,<volume> --env-file <env_file_path> --command <command>
+```
+
 ### Stacks
 
 #### List your stacks
 
 ```
 cycleops stacks list
 ```
@@ -172,15 +184,15 @@
 
 ```yml
  deploy:
     runs-on: ubuntu-latest
     env:
       CYCLEOPS_API_KEY: ${{ secrets.CYCLEOPS_API_KEY }}
     steps:
-        run: pipx install cycleops
+        run: pip install cycleops
         run: cycleops services update <service_id> --variable containers.0.image=<image_name>
         run: cycleops setups deploy <setup_id>
 ```
 
 ## Example
 
 You can update a service's image and deploy a setup as follows:
```

