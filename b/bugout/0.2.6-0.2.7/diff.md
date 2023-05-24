# Comparing `tmp/bugout-0.2.6.tar.gz` & `tmp/bugout-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bugout-0.2.6.tar", last modified: Mon Feb 13 16:54:20 2023, max compression
+gzip compressed data, was "bugout-0.2.7.tar", last modified: Wed May 24 12:48:23 2023, max compression
```

## Comparing `bugout-0.2.6.tar` & `bugout-0.2.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 16:54:20.216929 bugout-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-13 16:54:03.000000 bugout-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-02-13 16:54:20.216929 bugout-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-02-13 16:54:03.000000 bugout-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 16:54:20.212929 bugout-0.2.6/bugout/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-02-13 16:54:03.000000 bugout-0.2.6/bugout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-02-13 16:54:03.000000 bugout-0.2.6/bugout/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31213 2023-02-13 16:54:03.000000 bugout-0.2.6/bugout/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-02-13 16:54:03.000000 bugout-0.2.6/bugout/calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-02-13 16:54:03.000000 bugout-0.2.6/bugout/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-02-13 16:54:03.000000 bugout-0.2.6/bugout/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-02-13 16:54:03.000000 bugout-0.2.6/bugout/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-02-13 16:54:03.000000 bugout-0.2.6/bugout/humbug.py
--rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-02-13 16:54:03.000000 bugout-0.2.6/bugout/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23739 2023-02-13 16:54:03.000000 bugout-0.2.6/bugout/journal.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 16:54:03.000000 bugout-0.2.6/bugout/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-02-13 16:54:03.000000 bugout-0.2.6/bugout/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-02-13 16:54:03.000000 bugout-0.2.6/bugout/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-02-13 16:54:03.000000 bugout-0.2.6/bugout/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 16:54:20.216929 bugout-0.2.6/bugout.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-02-13 16:54:20.000000 bugout-0.2.6/bugout.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-02-13 16:54:20.000000 bugout-0.2.6/bugout.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 16:54:20.000000 bugout-0.2.6/bugout.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-13 16:54:20.000000 bugout-0.2.6/bugout.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 16:54:19.000000 bugout-0.2.6/bugout.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-13 16:54:20.000000 bugout-0.2.6/bugout.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-13 16:54:20.000000 bugout-0.2.6/bugout.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 16:54:20.216929 bugout-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-02-13 16:54:03.000000 bugout-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:48:23.644303 bugout-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-24 12:48:09.000000 bugout-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-24 12:48:23.644303 bugout-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-24 12:48:09.000000 bugout-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:48:23.644303 bugout-0.2.7/bugout/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32500 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/humbug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23739 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/journal.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:48:23.644303 bugout-0.2.7/bugout.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-24 12:48:23.000000 bugout-0.2.7/bugout.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-24 12:48:23.000000 bugout-0.2.7/bugout.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:48:23.000000 bugout-0.2.7/bugout.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-24 12:48:23.000000 bugout-0.2.7/bugout.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:48:15.000000 bugout-0.2.7/bugout.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-24 12:48:23.000000 bugout-0.2.7/bugout.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 12:48:23.000000 bugout-0.2.7/bugout.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 12:48:23.644303 bugout-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-24 12:48:09.000000 bugout-0.2.7/setup.py
```

### Comparing `bugout-0.2.6/LICENSE` & `bugout-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bugout-0.2.6/PKG-INFO` & `bugout-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bugout
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python client library for Bugout API
 Home-page: https://github.com/bugout-dev/bugout-python
 Author: Bugout
 Author-email: engineering@bugout.dev
 License: MIT
 Platform: all
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `bugout-0.2.6/README.md` & `bugout-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `bugout-0.2.6/bugout/__main__.py` & `bugout-0.2.7/bugout/__main__.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.6/bugout/app.py` & `bugout-0.2.7/bugout/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -407,14 +407,47 @@
         token: Union[str, uuid.UUID],
         resource_id: Union[str, uuid.UUID],
         timeout: float = REQUESTS_TIMEOUT,
     ) -> data.BugoutResource:
         self.resource.timeout = timeout
         return self.resource.delete_resource(token=token, resource_id=resource_id)
 
+    def get_resource_holders(
+        self,
+        token: Union[str, uuid.UUID],
+        resource_id: Union[str, uuid.UUID],
+        timeout: float = REQUESTS_TIMEOUT,
+    ) -> data.BugoutResourceHolders:
+        self.resource.timeout = timeout
+        return self.resource.get_resource_holders(token=token, resource_id=resource_id)
+
+    def add_resource_holder_permissions(
+        self,
+        token: Union[str, uuid.UUID],
+        resource_id: Union[str, uuid.UUID],
+        holder_permissions: data.BugoutResourceHolder,
+        timeout: float = REQUESTS_TIMEOUT,
+    ) -> data.BugoutResourceHolders:
+        self.resource.timeout = timeout
+        return self.resource.add_resource_holder_permissions(
+            token=token, resource_id=resource_id, holder_permissions=holder_permissions
+        )
+
+    def delete_resource_holder_permissions(
+        self,
+        token: Union[str, uuid.UUID],
+        resource_id: Union[str, uuid.UUID],
+        holder_permissions: data.BugoutResourceHolder,
+        timeout: float = REQUESTS_TIMEOUT,
+    ) -> data.BugoutResourceHolders:
+        self.resource.timeout = timeout
+        return self.resource.delete_resource_holder_permissions(
+            token=token, resource_id=resource_id, holder_permissions=holder_permissions
+        )
+
     # Journal scopes handlers
     def list_scopes(
         self, token: Union[str, uuid.UUID], api: str, timeout: float = REQUESTS_TIMEOUT
     ) -> data.BugoutScopes:
         self.journal.timeout = timeout
         return self.journal.list_scopes(token=token, api=api)
```

### Comparing `bugout-0.2.6/bugout/calls.py` & `bugout-0.2.7/bugout/calls.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.6/bugout/data.py` & `bugout-0.2.7/bugout/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,14 +29,22 @@
 
 @unique
 class HolderType(Enum):
     user = "user"
     group = "group"
 
 
+class ResourcePermissions(Enum):
+    ADMIN = "admin"
+    CREATE = "create"
+    READ = "read"
+    UPDATE = "update"
+    DELETE = "delete"
+
+
 class AuthType(Enum):
     bearer = "Bearer"
     web3 = "Web3"
 
 
 class JournalTypes(Enum):
     DEFAULT = "default"
@@ -123,14 +131,30 @@
     updated_at: datetime
 
 
 class BugoutResources(BaseModel):
     resources: List[BugoutResource]
 
 
+class BugoutResourceHolder(BaseModel):
+    id: uuid.UUID = Field(alias="holder_id")
+    holder_type: HolderType
+    permissions: List[ResourcePermissions] = Field(default_factory=list)
+
+    class Config:
+        # Required configuration because in Brood we use "holder_id" instead of "id"
+        # during creation and deletion of new permissions for holder
+        allow_population_by_field_name = True
+
+
+class BugoutResourceHolders(BaseModel):
+    resource_id: uuid.UUID
+    holders: List[BugoutResourceHolder] = Field(default_factory=list)
+
+
 class BugoutJournalPermission(BaseModel):
     holder_type: HolderType
     holder_id: str
     permissions: List[str] = Field(default_factory=list)
 
 
 class BugoutJournalPermissions(BaseModel):
```

### Comparing `bugout-0.2.6/bugout/exceptions.py` & `bugout-0.2.7/bugout/exceptions.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.6/bugout/group.py` & `bugout-0.2.7/bugout/group.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.6/bugout/humbug.py` & `bugout-0.2.7/bugout/humbug.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.6/bugout/jobs.py` & `bugout-0.2.7/bugout/jobs.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.6/bugout/journal.py` & `bugout-0.2.7/bugout/journal.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.6/bugout/settings.py` & `bugout-0.2.7/bugout/settings.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.6/bugout/user.py` & `bugout-0.2.7/bugout/user.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.6/bugout.egg-info/PKG-INFO` & `bugout-0.2.7/bugout.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bugout
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python client library for Bugout API
 Home-page: https://github.com/bugout-dev/bugout-python
 Author: Bugout
 Author-email: engineering@bugout.dev
 License: MIT
 Platform: all
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `bugout-0.2.6/setup.py` & `bugout-0.2.7/setup.py`

 * *Files identical despite different names*

