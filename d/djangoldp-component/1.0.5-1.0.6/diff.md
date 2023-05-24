# Comparing `tmp/djangoldp_component-1.0.5.tar.gz` & `tmp/djangoldp_component-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_component-1.0.5.tar", last modified: Fri May 19 16:05:51 2023, max compression
+gzip compressed data, was "dist/djangoldp_component-1.0.6.tar", last modified: Wed May 24 10:29:13 2023, max compression
```

## Comparing `djangoldp_component-1.0.5.tar` & `djangoldp_component-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:05:51.000000 djangoldp_component-1.0.5/
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-05-19 16:05:33.000000 djangoldp_component-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:05:51.000000 djangoldp_component-1.0.5/djangoldp_component.egg-info/
--rw-r--r--   0 root         (0) root         (0)      294 2023-05-19 16:05:51.000000 djangoldp_component-1.0.5/djangoldp_component.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 16:05:51.000000 djangoldp_component-1.0.5/djangoldp_component.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      599 2023-05-19 16:05:51.000000 djangoldp_component-1.0.5/djangoldp_component.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-19 16:05:51.000000 djangoldp_component-1.0.5/djangoldp_component.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 16:05:51.000000 djangoldp_component-1.0.5/djangoldp_component.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-19 16:05:33.000000 djangoldp_component-1.0.5/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-05-19 16:05:51.000000 djangoldp_component-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      294 2023-05-19 16:05:51.000000 djangoldp_component-1.0.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:05:51.000000 djangoldp_component-1.0.5/djangoldp_component/
--rw-rw-rw-   0 root         (0) root         (0)     9635 2023-05-19 16:05:33.000000 djangoldp_component-1.0.5/djangoldp_component/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1654 2023-05-19 16:05:33.000000 djangoldp_component-1.0.5/djangoldp_component/admin.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-05-19 16:05:49.000000 djangoldp_component-1.0.5/djangoldp_component/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-19 16:05:33.000000 djangoldp_component-1.0.5/djangoldp_component/apps.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-19 16:05:33.000000 djangoldp_component-1.0.5/djangoldp_component/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:05:51.000000 djangoldp_component-1.0.5/djangoldp_component/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    12897 2023-05-19 16:05:33.000000 djangoldp_component-1.0.5/djangoldp_component/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      517 2023-05-19 16:05:33.000000 djangoldp_component-1.0.5/djangoldp_component/migrations/0003_component_auto_menu.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 16:05:33.000000 djangoldp_component-1.0.5/djangoldp_component/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-05-19 16:05:33.000000 djangoldp_component-1.0.5/djangoldp_component/migrations/0002_delete_dependency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:29:13.000000 djangoldp_component-1.0.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-05-24 10:28:53.000000 djangoldp_component-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:29:13.000000 djangoldp_component-1.0.6/djangoldp_component.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      294 2023-05-24 10:29:13.000000 djangoldp_component-1.0.6/djangoldp_component.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 10:29:13.000000 djangoldp_component-1.0.6/djangoldp_component.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      599 2023-05-24 10:29:13.000000 djangoldp_component-1.0.6/djangoldp_component.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-24 10:29:13.000000 djangoldp_component-1.0.6/djangoldp_component.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 10:29:13.000000 djangoldp_component-1.0.6/djangoldp_component.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-24 10:28:53.000000 djangoldp_component-1.0.6/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-05-24 10:29:13.000000 djangoldp_component-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      294 2023-05-24 10:29:13.000000 djangoldp_component-1.0.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:29:13.000000 djangoldp_component-1.0.6/djangoldp_component/
+-rw-rw-rw-   0 root         (0) root         (0)     9713 2023-05-24 10:28:53.000000 djangoldp_component-1.0.6/djangoldp_component/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1654 2023-05-24 10:28:53.000000 djangoldp_component-1.0.6/djangoldp_component/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-05-24 10:29:11.000000 djangoldp_component-1.0.6/djangoldp_component/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-24 10:28:53.000000 djangoldp_component-1.0.6/djangoldp_component/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-24 10:28:53.000000 djangoldp_component-1.0.6/djangoldp_component/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:29:13.000000 djangoldp_component-1.0.6/djangoldp_component/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    12897 2023-05-24 10:28:53.000000 djangoldp_component-1.0.6/djangoldp_component/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      517 2023-05-24 10:28:53.000000 djangoldp_component-1.0.6/djangoldp_component/migrations/0003_component_auto_menu.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 10:28:53.000000 djangoldp_component-1.0.6/djangoldp_component/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-05-24 10:28:53.000000 djangoldp_component-1.0.6/djangoldp_component/migrations/0002_delete_dependency.py
```

### Comparing `djangoldp_component-1.0.5/README.md` & `djangoldp_component-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_component-1.0.5/djangoldp_component.egg-info/SOURCES.txt` & `djangoldp_component-1.0.6/djangoldp_component.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_component-1.0.5/setup.cfg` & `djangoldp_component-1.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp_component-1.0.5/djangoldp_component/models.py` & `djangoldp_component-1.0.6/djangoldp_component/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,25 +49,25 @@
         container_path = "/components/"
         depth = 1  # Do not serialize user
         lookup_field = "slug"
         nested_fields = ["parameters", "script_tags"]
         ordering = ["slug"]
         owner_field = "creator"
         owner_perms = ["inherit", "change", "delete"]
-        rdf_context = {
-            "friendly_name": "sib:friendlyName",
-            "name": "sib:tag",
-            "short_description": "sib:shortDescription",
-            "preferred_route": "sib:route",
-            "auto_import": "sib:componentAutoImport",
-            "auto_menu": "sib:componentAutoMenu",
-            "creator": "foaf:user",
-            "parameters": "ldp:Container",
-            "script_tags": "ldp:Container",
-        }
+        # rdf_context = {
+        #     "friendly_name": "sib:friendlyName",
+        #     "name": "sib:tag",
+        #     "short_description": "sib:shortDescription",
+        #     "preferred_route": "sib:route",
+        #     "auto_import": "sib:componentAutoImport",
+        #     "auto_menu": "sib:componentAutoMenu",
+        #     "creator": "foaf:user",
+        #     "parameters": "ldp:Container",
+        #     "script_tags": "ldp:Container",
+        # }
         rdf_type = "sib:component"
         serializer_fields = [
             "@id",
             "friendly_name",
             "name",
             "short_description",
             "preferred_route",
@@ -102,20 +102,20 @@
 
     class Meta(Model.Meta):
         anonymous_perms = ["view"]
         authenticated_perms = ["inherit"]
         container_path = "script-tags/"
         owner_field = "component__creator"
         owner_perms = ["inherit", "change", "delete"]
-        rdf_context = {
-            "component": "sib:component",
-            "friendly_name": "sib:friendlyName",
-            "src": "sib:componentScriptTagSrc",
-            "integrity": "sib:componentScriptTagIntegrity",
-        }
+        # rdf_context = {
+        #     "component": "sib:component",
+        #     "friendly_name": "sib:friendlyName",
+        #     "src": "sib:componentScriptTagSrc",
+        #     "integrity": "sib:componentScriptTagIntegrity",
+        # }
         rdf_type = "sib:scriptTag"
         serializer_fields = ["@id", "friendly_name", "src", "integrity"]
         superuser_perms = ["inherit"]
         verbose_name = _("script tag")
         verbose_name_plural = _("script tags")
 
 
@@ -142,21 +142,21 @@
 
     class Meta(Model.Meta):
         anonymous_perms = ["view"]
         authenticated_perms = ["inherit"]
         container_path = "parameters/"
         owner_field = "component__creator"
         owner_perms = ["inherit", "change", "delete"]
-        rdf_context = {
-            "friendly_name": "sib:friendlyName",
-            "description": "sib:description",
-            "component": "sib:component",
-            "key": "sib:key",
-            "default": "sib:value",
-        }
+        # rdf_context = {
+        #     "friendly_name": "sib:friendlyName",
+        #     "description": "sib:description",
+        #     "component": "sib:component",
+        #     "key": "sib:key",
+        #     "default": "sib:value",
+        # }
         rdf_type = "sib:parameter"
         serializer_fields = ["@id", "friendly_name", "description", "key", "default"]
         superuser_perms = ["inherit"]
         verbose_name = _("parameter")
         verbose_name_plural = _("parameters")
 
 
@@ -187,22 +187,22 @@
         container_path = "/packages/"
         depth = 0
         lookup_field = "slug"
         nested_fields = ["parameters"]
         ordering = ["slug"]
         owner_field = "creator"
         owner_perms = ["inherit", "change", "delete"]
-        rdf_context = {
-            "friendly_name": "sib:friendlyName",
-            "short_description": "sib:shortDescription",
-            "creator": "foaf:user",
-            "distribution": "sib:distribution",
-            "module": "sib:module",
-            "parameters": "ldp:Container",
-        }
+        # rdf_context = {
+        #     "friendly_name": "sib:friendlyName",
+        #     "short_description": "sib:shortDescription",
+        #     "creator": "foaf:user",
+        #     "distribution": "sib:distribution",
+        #     "module": "sib:module",
+        #     "parameters": "ldp:Container",
+        # }
         rdf_type = "sib:package"
         serializer_fields = [
             "@id",
             "friendly_name",
             "short_description",
             "creator",
             "distribution",
@@ -237,21 +237,21 @@
 
     class Meta(Model.Meta):
         anonymous_perms = ["view"]
         authenticated_perms = ["inherit"]
         container_path = "server-parameters/"
         owner_field = "package__creator"
         owner_perms = ["inherit", "change", "delete"]
-        rdf_context = {
-            "friendly_name": "sib:friendlyName",
-            "description": "sib:description",
-            "package": "sib:package",
-            "key": "sib:key",
-            "default": "sib:value",
-        }
+        # rdf_context = {
+        #     "friendly_name": "sib:friendlyName",
+        #     "description": "sib:description",
+        #     "package": "sib:package",
+        #     "key": "sib:key",
+        #     "default": "sib:value",
+        # }
         rdf_type = "sib:parameter"
         serializer_fields = ["@id", "friendly_name", "description", "key", "default"]
         superuser_perms = ["inherit"]
         verbose_name = _("server parameter")
         verbose_name_plural = _("server parameters")
```

### Comparing `djangoldp_component-1.0.5/djangoldp_component/admin.py` & `djangoldp_component-1.0.6/djangoldp_component/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_component-1.0.5/djangoldp_component/migrations/0001_initial.py` & `djangoldp_component-1.0.6/djangoldp_component/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_component-1.0.5/djangoldp_component/migrations/0003_component_auto_menu.py` & `djangoldp_component-1.0.6/djangoldp_component/migrations/0003_component_auto_menu.py`

 * *Files identical despite different names*

