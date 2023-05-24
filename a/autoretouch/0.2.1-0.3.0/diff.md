# Comparing `tmp/autoretouch-0.2.1.tar.gz` & `tmp/autoretouch-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoretouch-0.2.1.tar", last modified: Tue May 23 13:06:00 2023, max compression
+gzip compressed data, was "autoretouch-0.3.0.tar", last modified: Wed May 24 18:16:29 2023, max compression
```

## Comparing `autoretouch-0.2.1.tar` & `autoretouch-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 tlorentzen   (501) staff       (20)        0 2023-05-23 13:06:00.683531 autoretouch-0.2.1/
--rw-r--r--   0 tlorentzen   (501) staff       (20)      644 2021-10-06 09:14:54.000000 autoretouch-0.2.1/LICENSE
--rw-r--r--   0 tlorentzen   (501) staff       (20)     5205 2023-05-23 13:06:00.683030 autoretouch-0.2.1/PKG-INFO
--rw-r--r--   0 tlorentzen   (501) staff       (20)     4859 2023-03-21 14:15:18.000000 autoretouch-0.2.1/README.md
-drwxr-xr-x   0 tlorentzen   (501) staff       (20)        0 2023-05-23 13:06:00.676695 autoretouch-0.2.1/autoretouch/
--rw-r--r--   0 tlorentzen   (501) staff       (20)      695 2022-07-29 09:51:42.000000 autoretouch-0.2.1/autoretouch/.autoretouch-complete.fish
--rw-r--r--   0 tlorentzen   (501) staff       (20)     1002 2022-07-29 09:51:42.000000 autoretouch-0.2.1/autoretouch/.autoretouch-complete.zsh
--rw-r--r--   0 tlorentzen   (501) staff       (20)        0 2022-07-29 09:51:42.000000 autoretouch-0.2.1/autoretouch/__init__.py
-drwxr-xr-x   0 tlorentzen   (501) staff       (20)        0 2023-05-23 13:06:00.680203 autoretouch-0.2.1/autoretouch/api_client/
--rw-r--r--   0 tlorentzen   (501) staff       (20)        0 2022-07-29 09:51:42.000000 autoretouch-0.2.1/autoretouch/api_client/__init__.py
--rw-r--r--   0 tlorentzen   (501) staff       (20)     4889 2022-07-29 09:51:42.000000 autoretouch-0.2.1/autoretouch/api_client/authenticator.py
--rw-r--r--   0 tlorentzen   (501) staff       (20)    25812 2023-05-23 12:06:14.000000 autoretouch-0.2.1/autoretouch/api_client/client.py
--rw-r--r--   0 tlorentzen   (501) staff       (20)     2615 2022-07-29 09:51:42.000000 autoretouch-0.2.1/autoretouch/api_client/model.py
-drwxr-xr-x   0 tlorentzen   (501) staff       (20)        0 2023-05-23 13:06:00.681231 autoretouch-0.2.1/autoretouch/cli/
--rw-r--r--   0 tlorentzen   (501) staff       (20)        0 2022-07-29 09:51:42.000000 autoretouch-0.2.1/autoretouch/cli/__init__.py
--rw-r--r--   0 tlorentzen   (501) staff       (20)     8530 2022-07-29 09:51:42.000000 autoretouch-0.2.1/autoretouch/cli/commands.py
-drwxr-xr-x   0 tlorentzen   (501) staff       (20)        0 2023-05-23 13:06:00.678562 autoretouch-0.2.1/autoretouch.egg-info/
--rw-r--r--   0 tlorentzen   (501) staff       (20)     5205 2023-05-23 13:06:00.000000 autoretouch-0.2.1/autoretouch.egg-info/PKG-INFO
--rw-r--r--   0 tlorentzen   (501) staff       (20)      597 2023-05-23 13:06:00.000000 autoretouch-0.2.1/autoretouch.egg-info/SOURCES.txt
--rw-r--r--   0 tlorentzen   (501) staff       (20)        1 2023-05-23 13:06:00.000000 autoretouch-0.2.1/autoretouch.egg-info/dependency_links.txt
--rw-r--r--   0 tlorentzen   (501) staff       (20)       73 2023-05-23 13:06:00.000000 autoretouch-0.2.1/autoretouch.egg-info/entry_points.txt
--rw-r--r--   0 tlorentzen   (501) staff       (20)       39 2023-05-23 13:06:00.000000 autoretouch-0.2.1/autoretouch.egg-info/requires.txt
--rw-r--r--   0 tlorentzen   (501) staff       (20)       12 2023-05-23 13:06:00.000000 autoretouch-0.2.1/autoretouch.egg-info/top_level.txt
--rw-r--r--   0 tlorentzen   (501) staff       (20)       85 2022-07-29 09:51:42.000000 autoretouch-0.2.1/pyproject.toml
--rw-r--r--   0 tlorentzen   (501) staff       (20)       38 2023-05-23 13:06:00.683666 autoretouch-0.2.1/setup.cfg
--rw-r--r--   0 tlorentzen   (501) staff       (20)     3695 2023-05-23 12:07:17.000000 autoretouch-0.2.1/setup.py
-drwxr-xr-x   0 tlorentzen   (501) staff       (20)        0 2023-05-23 13:06:00.682338 autoretouch-0.2.1/test/
--rw-r--r--   0 tlorentzen   (501) staff       (20)     3073 2023-05-16 15:12:01.000000 autoretouch-0.2.1/test/test_authenticator.py
--rw-r--r--   0 tlorentzen   (501) staff       (20)    11415 2023-05-17 08:43:20.000000 autoretouch-0.2.1/test/test_client.py
+drwxr-xr-x   0 tlorentzen   (501) staff       (20)        0 2023-05-24 18:16:29.829039 autoretouch-0.3.0/
+-rw-r--r--   0 tlorentzen   (501) staff       (20)      644 2021-10-06 09:14:54.000000 autoretouch-0.3.0/LICENSE
+-rw-r--r--   0 tlorentzen   (501) staff       (20)     5205 2023-05-24 18:16:29.828641 autoretouch-0.3.0/PKG-INFO
+-rw-r--r--   0 tlorentzen   (501) staff       (20)     4859 2023-03-21 14:15:18.000000 autoretouch-0.3.0/README.md
+drwxr-xr-x   0 tlorentzen   (501) staff       (20)        0 2023-05-24 18:16:29.816969 autoretouch-0.3.0/autoretouch/
+-rw-r--r--   0 tlorentzen   (501) staff       (20)      695 2022-07-29 09:51:42.000000 autoretouch-0.3.0/autoretouch/.autoretouch-complete.fish
+-rw-r--r--   0 tlorentzen   (501) staff       (20)     1002 2022-07-29 09:51:42.000000 autoretouch-0.3.0/autoretouch/.autoretouch-complete.zsh
+-rw-r--r--   0 tlorentzen   (501) staff       (20)        0 2022-07-29 09:51:42.000000 autoretouch-0.3.0/autoretouch/__init__.py
+drwxr-xr-x   0 tlorentzen   (501) staff       (20)        0 2023-05-24 18:16:29.824783 autoretouch-0.3.0/autoretouch/api_client/
+-rw-r--r--   0 tlorentzen   (501) staff       (20)        0 2022-07-29 09:51:42.000000 autoretouch-0.3.0/autoretouch/api_client/__init__.py
+-rw-r--r--   0 tlorentzen   (501) staff       (20)     4889 2022-07-29 09:51:42.000000 autoretouch-0.3.0/autoretouch/api_client/authenticator.py
+-rw-r--r--   0 tlorentzen   (501) staff       (20)    25938 2023-05-24 18:14:12.000000 autoretouch-0.3.0/autoretouch/api_client/client.py
+-rw-r--r--   0 tlorentzen   (501) staff       (20)     2615 2022-07-29 09:51:42.000000 autoretouch-0.3.0/autoretouch/api_client/model.py
+drwxr-xr-x   0 tlorentzen   (501) staff       (20)        0 2023-05-24 18:16:29.825923 autoretouch-0.3.0/autoretouch/cli/
+-rw-r--r--   0 tlorentzen   (501) staff       (20)        0 2022-07-29 09:51:42.000000 autoretouch-0.3.0/autoretouch/cli/__init__.py
+-rw-r--r--   0 tlorentzen   (501) staff       (20)     8530 2022-07-29 09:51:42.000000 autoretouch-0.3.0/autoretouch/cli/commands.py
+drwxr-xr-x   0 tlorentzen   (501) staff       (20)        0 2023-05-24 18:16:29.822106 autoretouch-0.3.0/autoretouch.egg-info/
+-rw-r--r--   0 tlorentzen   (501) staff       (20)     5205 2023-05-24 18:16:29.000000 autoretouch-0.3.0/autoretouch.egg-info/PKG-INFO
+-rw-r--r--   0 tlorentzen   (501) staff       (20)      597 2023-05-24 18:16:29.000000 autoretouch-0.3.0/autoretouch.egg-info/SOURCES.txt
+-rw-r--r--   0 tlorentzen   (501) staff       (20)        1 2023-05-24 18:16:29.000000 autoretouch-0.3.0/autoretouch.egg-info/dependency_links.txt
+-rw-r--r--   0 tlorentzen   (501) staff       (20)       73 2023-05-24 18:16:29.000000 autoretouch-0.3.0/autoretouch.egg-info/entry_points.txt
+-rw-r--r--   0 tlorentzen   (501) staff       (20)       39 2023-05-24 18:16:29.000000 autoretouch-0.3.0/autoretouch.egg-info/requires.txt
+-rw-r--r--   0 tlorentzen   (501) staff       (20)       12 2023-05-24 18:16:29.000000 autoretouch-0.3.0/autoretouch.egg-info/top_level.txt
+-rw-r--r--   0 tlorentzen   (501) staff       (20)       85 2022-07-29 09:51:42.000000 autoretouch-0.3.0/pyproject.toml
+-rw-r--r--   0 tlorentzen   (501) staff       (20)       38 2023-05-24 18:16:29.829177 autoretouch-0.3.0/setup.cfg
+-rw-r--r--   0 tlorentzen   (501) staff       (20)     3695 2023-05-24 18:15:10.000000 autoretouch-0.3.0/setup.py
+drwxr-xr-x   0 tlorentzen   (501) staff       (20)        0 2023-05-24 18:16:29.827482 autoretouch-0.3.0/test/
+-rw-r--r--   0 tlorentzen   (501) staff       (20)     3073 2023-05-16 15:12:01.000000 autoretouch-0.3.0/test/test_authenticator.py
+-rw-r--r--   0 tlorentzen   (501) staff       (20)    11415 2023-05-17 08:43:20.000000 autoretouch-0.3.0/test/test_client.py
```

### Comparing `autoretouch-0.2.1/LICENSE` & `autoretouch-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autoretouch-0.2.1/PKG-INFO` & `autoretouch-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoretouch
-Version: 0.2.1
+Version: 0.3.0
 Summary: cli and python package to communicate with the autoRetouch API
 Author: ['Antoine Daurat <antoine@autoretouch.com>', 'Oliver Allweyer <oliver@autoretouch.com>', 'Till Lorentzen <till@autoretouch.com>']
 License: BSD Zero
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # autoRetouch client
```

### Comparing `autoretouch-0.2.1/README.md` & `autoretouch-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `autoretouch-0.2.1/autoretouch/.autoretouch-complete.fish` & `autoretouch-0.3.0/autoretouch/.autoretouch-complete.fish`

 * *Files identical despite different names*

### Comparing `autoretouch-0.2.1/autoretouch/.autoretouch-complete.zsh` & `autoretouch-0.3.0/autoretouch/.autoretouch-complete.zsh`

 * *Files identical despite different names*

### Comparing `autoretouch-0.2.1/autoretouch/api_client/authenticator.py` & `autoretouch-0.3.0/autoretouch/api_client/authenticator.py`

 * *Files identical despite different names*

### Comparing `autoretouch-0.2.1/autoretouch/api_client/client.py` & `autoretouch-0.3.0/autoretouch/api_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,14 +358,15 @@
             workflow_id: UUID,
             image_content_hash: str,
             image_name: str,
             labels: Optional[Dict[str, str]] = None,
             workflow_version_id: Optional[UUID] = None,
             organization_id: Optional[UUID] = None,
             settings: Optional[dict] = None,
+            webhooks: Optional[List[str]] = None,
     ) -> UUID:
         logger.info("creating workflow execution for image reference...")
         self.authenticated()
         organization_id = self._get_organization_id(organization_id)
         version_str = f"&version={workflow_version_id}" if workflow_version_id else ""
         url = (
             f"{self.api_config.BASE_API_URL_CURRENT}/workflow/execution/create"
@@ -380,14 +381,16 @@
                 "name": image_name,
                 "contentHash": image_content_hash,
                 "contentType": mimetype,
             },
             **({"labels": labels} if labels else {}),
             "settings": settings if settings else {}
         }
+        if webhooks is not None:
+            payload["webhooks"] = webhooks
 
         response = requests.post(url=url, headers=headers, data=json.dumps(payload))
         logger.debug(f"{url} answered with status {response.status_code}")
         response.raise_for_status()
         return UUID(response.content.decode(response.encoding))
 
     def get_workflow_execution_details(
```

### Comparing `autoretouch-0.2.1/autoretouch/api_client/model.py` & `autoretouch-0.3.0/autoretouch/api_client/model.py`

 * *Files identical despite different names*

### Comparing `autoretouch-0.2.1/autoretouch/cli/commands.py` & `autoretouch-0.3.0/autoretouch/cli/commands.py`

 * *Files identical despite different names*

### Comparing `autoretouch-0.2.1/autoretouch.egg-info/PKG-INFO` & `autoretouch-0.3.0/autoretouch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoretouch
-Version: 0.2.1
+Version: 0.3.0
 Summary: cli and python package to communicate with the autoRetouch API
 Author: ['Antoine Daurat <antoine@autoretouch.com>', 'Oliver Allweyer <oliver@autoretouch.com>', 'Till Lorentzen <till@autoretouch.com>']
 License: BSD Zero
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # autoRetouch client
```

### Comparing `autoretouch-0.2.1/autoretouch.egg-info/SOURCES.txt` & `autoretouch-0.3.0/autoretouch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autoretouch-0.2.1/setup.py` & `autoretouch-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 
 with open("README.md", "r") as f:
     README = f.read()
 
 setup(
     name="autoretouch",
-    version="0.2.1",
+    version="0.3.0",
     author=[
         "Antoine Daurat <antoine@autoretouch.com>",
         "Oliver Allweyer <oliver@autoretouch.com>",
         "Till Lorentzen <till@autoretouch.com>"
     ],
     description="cli and python package to communicate with the autoRetouch API",
     long_description=README,
```

### Comparing `autoretouch-0.2.1/test/test_authenticator.py` & `autoretouch-0.3.0/test/test_authenticator.py`

 * *Files identical despite different names*

### Comparing `autoretouch-0.2.1/test/test_client.py` & `autoretouch-0.3.0/test/test_client.py`

 * *Files identical despite different names*

