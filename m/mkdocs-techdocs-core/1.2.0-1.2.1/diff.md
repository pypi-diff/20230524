# Comparing `tmp/mkdocs-techdocs-core-1.2.0.tar.gz` & `tmp/mkdocs-techdocs-core-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mkdocs-techdocs-core-1.2.0.tar", last modified: Wed Mar 29 11:34:17 2023, max compression
+gzip compressed data, was "dist/mkdocs-techdocs-core-1.2.1.tar", last modified: Wed May 24 13:00:22 2023, max compression
```

## Comparing `mkdocs-techdocs-core-1.2.0.tar` & `mkdocs-techdocs-core-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:34:17.000000 mkdocs-techdocs-core-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18905 2023-03-29 11:34:17.000000 mkdocs-techdocs-core-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15399 2023-03-29 11:34:12.000000 mkdocs-techdocs-core-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:34:17.000000 mkdocs-techdocs-core-1.2.0/mkdocs_techdocs_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18905 2023-03-29 11:34:17.000000 mkdocs-techdocs-core-1.2.0/mkdocs_techdocs_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-29 11:34:17.000000 mkdocs-techdocs-core-1.2.0/mkdocs_techdocs_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 11:34:17.000000 mkdocs-techdocs-core-1.2.0/mkdocs_techdocs_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-29 11:34:17.000000 mkdocs-techdocs-core-1.2.0/mkdocs_techdocs_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-29 11:34:17.000000 mkdocs-techdocs-core-1.2.0/mkdocs_techdocs_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-29 11:34:17.000000 mkdocs-techdocs-core-1.2.0/mkdocs_techdocs_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 11:34:17.000000 mkdocs-techdocs-core-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-29 11:34:12.000000 mkdocs-techdocs-core-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:34:17.000000 mkdocs-techdocs-core-1.2.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 11:34:12.000000 mkdocs-techdocs-core-1.2.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-03-29 11:34:12.000000 mkdocs-techdocs-core-1.2.0/src/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-03-29 11:34:12.000000 mkdocs-techdocs-core-1.2.0/src/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:00:22.000000 mkdocs-techdocs-core-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    19079 2023-05-24 13:00:22.000000 mkdocs-techdocs-core-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15549 2023-05-24 13:00:17.000000 mkdocs-techdocs-core-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:00:22.000000 mkdocs-techdocs-core-1.2.1/mkdocs_techdocs_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19079 2023-05-24 13:00:22.000000 mkdocs-techdocs-core-1.2.1/mkdocs_techdocs_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-24 13:00:22.000000 mkdocs-techdocs-core-1.2.1/mkdocs_techdocs_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:00:22.000000 mkdocs-techdocs-core-1.2.1/mkdocs_techdocs_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-24 13:00:22.000000 mkdocs-techdocs-core-1.2.1/mkdocs_techdocs_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-24 13:00:22.000000 mkdocs-techdocs-core-1.2.1/mkdocs_techdocs_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-24 13:00:22.000000 mkdocs-techdocs-core-1.2.1/mkdocs_techdocs_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 13:00:22.000000 mkdocs-techdocs-core-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-24 13:00:17.000000 mkdocs-techdocs-core-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:00:22.000000 mkdocs-techdocs-core-1.2.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:00:17.000000 mkdocs-techdocs-core-1.2.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-05-24 13:00:17.000000 mkdocs-techdocs-core-1.2.1/src/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-24 13:00:17.000000 mkdocs-techdocs-core-1.2.1/src/test_core.py
```

### Comparing `mkdocs-techdocs-core-1.2.0/PKG-INFO` & `mkdocs-techdocs-core-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-techdocs-core
-Version: 1.2.0
+Version: 1.2.1
 Summary: The core MkDocs plugin used by Backstage's TechDocs as a wrapper around multiple MkDocs plugins and Python Markdown extensions
 Home-page: https://github.com/backstage/mkdocs-techdocs-core
 Author: TechDocs Core
 Author-email: pulp-fiction@spotify.com
 License: Apache-2.0
 Description: # mkdocs-techdocs-core
         
@@ -150,14 +150,17 @@
         
         We only use `material-mkdocs` as base styles because Backstage also uses the `Material UI` on the client-side. We don't expect people to use themes other than `Material UI` to maintain consistency across all Backstage pages (in other words, documentation pages have the same look and feel as any other Backstage page) and so we use the `BackstageTheme` configured in Front-end application as the source of truth for all application design tokens like colors, typography and etc. So here you can [see](https://github.com/backstage/backstage/blob/master/plugins/techdocs/src/reader/components/TechDocsReaderPageContent/dom.tsx#L160-L692) that some styles will always be overridden regardless of the `mkdocs-material` plugin theme settings and this can cause unexpected behavior for those who override the theme setting in a `mkdocs.yaml` file.
         
         ## Changelog
         
         ### Unreleased
         
+        ### 1.2.1
+         - Use latest version of `pymdown-extensions` which contains [security fixes](https://github.com/backstage/mkdocs-techdocs-core/pull/123).
+        
         ### 1.2.0
          - Updated `mkdocs-material` (and its dependencies) from `8.1.11` to `9.1.3` causing a few changes:
            -  Some `mkdocs-material` features were made opt-in v9. In order to preserve compatibility, they are now hardcoded as enabled by `mkdocs-techdocs-core`. The features are
               -  `navigation.footer`
               -  `content.action.edit`
            -  `theme.palette` is now hardcoded to `""` to preserve previous behavior. Without hardcoding the palette, it gets the value `default`, causing unwanted visual changes. 
            -  Some components e.g. admonitions have a slightly different look.
```

### Comparing `mkdocs-techdocs-core-1.2.0/README.md` & `mkdocs-techdocs-core-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,17 @@
 
 We only use `material-mkdocs` as base styles because Backstage also uses the `Material UI` on the client-side. We don't expect people to use themes other than `Material UI` to maintain consistency across all Backstage pages (in other words, documentation pages have the same look and feel as any other Backstage page) and so we use the `BackstageTheme` configured in Front-end application as the source of truth for all application design tokens like colors, typography and etc. So here you can [see](https://github.com/backstage/backstage/blob/master/plugins/techdocs/src/reader/components/TechDocsReaderPageContent/dom.tsx#L160-L692) that some styles will always be overridden regardless of the `mkdocs-material` plugin theme settings and this can cause unexpected behavior for those who override the theme setting in a `mkdocs.yaml` file.
 
 ## Changelog
 
 ### Unreleased
 
+### 1.2.1
+ - Use latest version of `pymdown-extensions` which contains [security fixes](https://github.com/backstage/mkdocs-techdocs-core/pull/123).
+
 ### 1.2.0
  - Updated `mkdocs-material` (and its dependencies) from `8.1.11` to `9.1.3` causing a few changes:
    -  Some `mkdocs-material` features were made opt-in v9. In order to preserve compatibility, they are now hardcoded as enabled by `mkdocs-techdocs-core`. The features are
       -  `navigation.footer`
       -  `content.action.edit`
    -  `theme.palette` is now hardcoded to `""` to preserve previous behavior. Without hardcoding the palette, it gets the value `default`, causing unwanted visual changes. 
    -  Some components e.g. admonitions have a slightly different look.
```

### Comparing `mkdocs-techdocs-core-1.2.0/mkdocs_techdocs_core.egg-info/PKG-INFO` & `mkdocs-techdocs-core-1.2.1/mkdocs_techdocs_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-techdocs-core
-Version: 1.2.0
+Version: 1.2.1
 Summary: The core MkDocs plugin used by Backstage's TechDocs as a wrapper around multiple MkDocs plugins and Python Markdown extensions
 Home-page: https://github.com/backstage/mkdocs-techdocs-core
 Author: TechDocs Core
 Author-email: pulp-fiction@spotify.com
 License: Apache-2.0
 Description: # mkdocs-techdocs-core
         
@@ -150,14 +150,17 @@
         
         We only use `material-mkdocs` as base styles because Backstage also uses the `Material UI` on the client-side. We don't expect people to use themes other than `Material UI` to maintain consistency across all Backstage pages (in other words, documentation pages have the same look and feel as any other Backstage page) and so we use the `BackstageTheme` configured in Front-end application as the source of truth for all application design tokens like colors, typography and etc. So here you can [see](https://github.com/backstage/backstage/blob/master/plugins/techdocs/src/reader/components/TechDocsReaderPageContent/dom.tsx#L160-L692) that some styles will always be overridden regardless of the `mkdocs-material` plugin theme settings and this can cause unexpected behavior for those who override the theme setting in a `mkdocs.yaml` file.
         
         ## Changelog
         
         ### Unreleased
         
+        ### 1.2.1
+         - Use latest version of `pymdown-extensions` which contains [security fixes](https://github.com/backstage/mkdocs-techdocs-core/pull/123).
+        
         ### 1.2.0
          - Updated `mkdocs-material` (and its dependencies) from `8.1.11` to `9.1.3` causing a few changes:
            -  Some `mkdocs-material` features were made opt-in v9. In order to preserve compatibility, they are now hardcoded as enabled by `mkdocs-techdocs-core`. The features are
               -  `navigation.footer`
               -  `content.action.edit`
            -  `theme.palette` is now hardcoded to `""` to preserve previous behavior. Without hardcoding the palette, it gets the value `default`, causing unwanted visual changes. 
            -  Some components e.g. admonitions have a slightly different look.
```

### Comparing `mkdocs-techdocs-core-1.2.0/setup.py` & `mkdocs-techdocs-core-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 # Read the contents of the requirements.txt file
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="mkdocs-techdocs-core",
-    version="1.2.0",
+    version="1.2.1",
     description="The core MkDocs plugin used by Backstage's TechDocs as a wrapper around "
     "multiple MkDocs plugins and Python Markdown extensions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="mkdocs",
     url="https://github.com/backstage/mkdocs-techdocs-core",
     author="TechDocs Core",
```

### Comparing `mkdocs-techdocs-core-1.2.0/src/core.py` & `mkdocs-techdocs-core-1.2.1/src/core.py`

 * *Files identical despite different names*

### Comparing `mkdocs-techdocs-core-1.2.0/src/test_core.py` & `mkdocs-techdocs-core-1.2.1/src/test_core.py`

 * *Files identical despite different names*

