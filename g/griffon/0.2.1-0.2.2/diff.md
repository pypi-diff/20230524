# Comparing `tmp/griffon-0.2.1.tar.gz` & `tmp/griffon-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griffon-0.2.1.tar", last modified: Tue May 23 07:05:16 2023, max compression
+gzip compressed data, was "griffon-0.2.2.tar", last modified: Wed May 24 08:00:20 2023, max compression
```

## Comparing `griffon-0.2.1.tar` & `griffon-0.2.2.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:16.290184 griffon-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-23 07:04:57.000000 griffon-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-23 07:05:16.290184 griffon-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-23 07:04:57.000000 griffon-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:16.282184 griffon-0.2.1/griffon/
--rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:16.282184 griffon-0.2.1/griffon/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/autocomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:16.282184 griffon-0.2.1/griffon/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:16.286184 griffon-0.2.1/griffon/commands/entities/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26909 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/entities/community_component_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    27264 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/entities/corgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/entities/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/entities/osidb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/plugin_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:16.286184 griffon-0.2.1/griffon/commands/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/plugins/cve_mitre.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/plugins/cvelib.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/plugins/fcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/plugins/go_vuln.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/plugins/osv.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/plugins/semgrep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/process.py
--rw-r--r--   0 runner    (1001) docker     (123)    24381 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    41808 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:16.286184 griffon-0.2.1/griffon/services/
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/services/core_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    36478 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/services/core_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    20730 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/services/core_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:16.286184 griffon-0.2.1/griffon/static/
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/static/default_griffonrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:16.282184 griffon-0.2.1/griffon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-23 07:05:16.000000 griffon-0.2.1/griffon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-23 07:05:16.000000 griffon-0.2.1/griffon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 07:05:16.000000 griffon-0.2.1/griffon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-23 07:05:16.000000 griffon-0.2.1/griffon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 07:05:16.000000 griffon-0.2.1/griffon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-23 07:05:16.000000 griffon-0.2.1/griffon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-23 07:04:57.000000 griffon-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 07:05:16.290184 griffon-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-23 07:04:57.000000 griffon-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:16.290184 griffon-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-23 07:04:57.000000 griffon-0.2.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-23 07:04:57.000000 griffon-0.2.1/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-23 07:04:57.000000 griffon-0.2.1/tests/test_manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-23 07:04:57.000000 griffon-0.2.1/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-23 07:04:57.000000 griffon-0.2.1/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-23 07:04:57.000000 griffon-0.2.1/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-23 07:04:57.000000 griffon-0.2.1/tests/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-23 07:04:57.000000 griffon-0.2.1/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:00:20.137890 griffon-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-24 08:00:01.000000 griffon-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-24 08:00:20.137890 griffon-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-24 08:00:01.000000 griffon-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:00:20.129890 griffon-0.2.2/griffon/
+-rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:00:20.133890 griffon-0.2.2/griffon/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/autocomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:00:20.133890 griffon-0.2.2/griffon/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/commands/docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:00:20.133890 griffon-0.2.2/griffon/commands/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/commands/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26909 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/commands/entities/community_component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27264 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/commands/entities/corgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/commands/entities/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/commands/entities/osidb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/commands/plugin_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:00:20.133890 griffon-0.2.2/griffon/commands/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/commands/plugins/bugzilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/commands/plugins/cve_mitre.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/commands/plugins/cvelib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/commands/plugins/fcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/commands/plugins/go_vuln.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/commands/plugins/osv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/commands/plugins/semgrep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/commands/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24381 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/commands/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/commands/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45932 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:00:20.133890 griffon-0.2.2/griffon/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/services/core_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36767 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/services/core_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20730 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/services/core_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:00:20.133890 griffon-0.2.2/griffon/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-24 08:00:01.000000 griffon-0.2.2/griffon/static/default_griffonrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:00:20.133890 griffon-0.2.2/griffon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-24 08:00:20.000000 griffon-0.2.2/griffon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-24 08:00:20.000000 griffon-0.2.2/griffon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 08:00:20.000000 griffon-0.2.2/griffon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-24 08:00:20.000000 griffon-0.2.2/griffon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-24 08:00:20.000000 griffon-0.2.2/griffon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-24 08:00:20.000000 griffon-0.2.2/griffon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-24 08:00:01.000000 griffon-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 08:00:20.137890 griffon-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-24 08:00:01.000000 griffon-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:00:20.137890 griffon-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-24 08:00:01.000000 griffon-0.2.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-24 08:00:01.000000 griffon-0.2.2/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-24 08:00:01.000000 griffon-0.2.2/tests/test_manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-24 08:00:01.000000 griffon-0.2.2/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-24 08:00:01.000000 griffon-0.2.2/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-24 08:00:01.000000 griffon-0.2.2/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-24 08:00:01.000000 griffon-0.2.2/tests/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-24 08:00:01.000000 griffon-0.2.2/tests/test_unit.py
```

### Comparing `griffon-0.2.1/LICENSE` & `griffon-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/PKG-INFO` & `griffon-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griffon
-Version: 0.2.1
+Version: 0.2.2
 Summary: Red Hat Product Security CLI
 Home-page: https://github.com/RedHatProductSecurity/griffon
 Author: James Fuller, Red Hat Product Security
 License: MIT
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `griffon-0.2.1/README.md` & `griffon-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/griffon/__init__.py` & `griffon-0.2.2/griffon/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import osidb_bindings
 from osidb_bindings.bindings.python_client.models import Affect, Flaw, Tracker
 from pkg_resources import resource_filename  # type: ignore
 from rich.logging import RichHandler
 
 from griffon.output import console
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 if "CORGI_API_URL" not in os.environ:
     print("Must set CORGI_API_URL environment variable.")
     exit(1)
 CORGI_API_URL = os.environ["CORGI_API_URL"]
 
 if "OSIDB_API_URL" not in os.environ:
```

### Comparing `griffon-0.2.1/griffon/autocomplete/__init__.py` & `griffon-0.2.2/griffon/autocomplete/__init__.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/griffon/cli.py` & `griffon-0.2.2/griffon/cli.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/griffon/commands/configure.py` & `griffon-0.2.2/griffon/commands/configure.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/griffon/commands/docs.py` & `griffon-0.2.2/griffon/commands/docs.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 
 @click.group(name="docs", help="Links to useful docs.")
 @click.pass_context
 def docs_grp(ctx):
     pass
 
 
+@docs_grp.command(name="public-manifests", help="published SPDX sbom (BETA)")
+def public_manifests():
+    click.launch("https://access.redhat.com/security/data/sbom/beta/spdx/")
+
+
 @docs_grp.group(name="service", help="Links to coarse grained data services.")
 @click.pass_context
 def service_grp(ctx):
     pass
 
 
 @service_grp.command()
```

### Comparing `griffon-0.2.1/griffon/commands/entities/__init__.py` & `griffon-0.2.2/griffon/commands/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/griffon/commands/entities/community_component_registry.py` & `griffon-0.2.2/griffon/commands/entities/community_component_registry.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/griffon/commands/entities/corgi.py` & `griffon-0.2.2/griffon/commands/entities/corgi.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/griffon/commands/entities/helpers.py` & `griffon-0.2.2/griffon/commands/entities/helpers.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/griffon/commands/entities/osidb.py` & `griffon-0.2.2/griffon/commands/entities/osidb.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/griffon/commands/plugin_commands.py` & `griffon-0.2.2/griffon/commands/plugin_commands.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/griffon/commands/plugins/cve_mitre.py` & `griffon-0.2.2/griffon/commands/plugins/cve_mitre.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/griffon/commands/plugins/go_vuln.py` & `griffon-0.2.2/griffon/commands/plugins/go_vuln.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/griffon/commands/plugins/osv.py` & `griffon-0.2.2/griffon/commands/plugins/osv.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/griffon/commands/plugins/semgrep.py` & `griffon-0.2.2/griffon/commands/plugins/semgrep.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     pass
 
 
 try:
     # ensure semgrep is installed
     import semgrep  # noqa
 
-    @plugins.command(help="Run this first, installs semgrep")
+    @plugins.command(help="semgrep scan")
     @click.argument("scan_dir", required=False, type=click.Path(exists=True))
     @click.pass_context
     def scan(ctx, scan_dir):
         if not scan_dir:
             scan_dir = click.prompt("Please enter a valid directory path to scan")
         subprocess.run(["semgrep", "--config", "auto", scan_dir])
```

### Comparing `griffon-0.2.1/griffon/commands/process.py` & `griffon-0.2.2/griffon/commands/process.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/griffon/commands/queries.py` & `griffon-0.2.2/griffon/commands/queries.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/griffon/commands/reports.py` & `griffon-0.2.2/griffon/commands/reports.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/griffon/output.py` & `griffon-0.2.2/griffon/output.py`

 * *Files 3% similar despite different names*

```diff
@@ -189,14 +189,15 @@
                                 "name": item.get("name"),
                                 "nvr": item.get("nvr"),
                                 "type": item.get("type"),
                                 "arch": item.get("arch"),
                                 "related_url": item.get("related_url"),
                                 "purl": item.get("purl"),
                                 "sources": item.get("sources"),
+                                "upstreams": item.get("upstreams"),
                             }
                             if "software_build" in item:
                                 c["build_source_url"] = item["software_build"].get("source")
                             normalised_results.append(c)
         product_versions = sorted(
             list(set([item["product_version"] for item in normalised_results]))
         )
@@ -310,34 +311,54 @@
                                     related_url = ""
                                     if result_tree[pv][ps][cn][nvr]["related_url"]:
                                         related_url = re.sub(
                                             search_component_name,
                                             f"[b]{search_component_name}[/b]",
                                             result_tree[pv][ps][cn][nvr]["related_url"],
                                         )
-                                    if result_tree[pv][ps][cn][nvr]["sources"]:
-                                        source_component_names = list(
-                                            set(
-                                                [
-                                                    source["name"]
-                                                    for source in result_tree[pv][ps][cn][nvr][
-                                                        "sources"
-                                                    ]
+                                    upstream_component_names = list(
+                                        set(
+                                            [
+                                                source["name"]
+                                                for source in result_tree[pv][ps][cn][nvr][
+                                                    "upstreams"
                                                 ]
-                                            )
+                                            ]
                                         )
-                                        for source_name in source_component_names:
-                                            console.print(
-                                                Text(ps, style="magenta b u"),
-                                                source_name,
-                                                dep,
-                                                f"([grey]{related_url}[/grey])",
-                                                no_wrap=False,
-                                            )
-                                    else:
+                                    )
+                                    if upstream_component_names:
+                                        console.print(
+                                            Text(ps, style="magenta b u"),
+                                            f"[cyan]{upstream_component_names[0]} (and {len(upstream_component_names)} more)[/cyan]",  # noqa
+                                            dep,
+                                            f"([grey]{related_url}[/grey])",
+                                            no_wrap=False,
+                                        )
+                                    source_component_names = list(
+                                        set(
+                                            [
+                                                source["name"]
+                                                for source in result_tree[pv][ps][cn][nvr][
+                                                    "sources"
+                                                ]
+                                            ]
+                                        )
+                                    )
+                                    if source_component_names:
+                                        console.print(
+                                            Text(ps, style="magenta b u"),
+                                            f"[light_blue]{source_component_names[0]} (and {len(source_component_names)} more)[/light_blue]",  # noqa
+                                            dep,
+                                            f"([grey]{related_url}[/grey])",
+                                            no_wrap=False,
+                                        )
+                                    if (
+                                        not result_tree[pv][ps][cn][nvr]["upstreams"]
+                                        and not result_tree[pv][ps][cn][nvr]["sources"]
+                                    ):
                                         console.print(
                                             Text(ps, style="magenta b u"),
                                             dep,
                                             f"([grey]{related_url}[/grey])",
                                             no_wrap=False,
                                         )
             if ctx.obj["VERBOSE"] == 2:  # product_stream X nvr x related_url x build_source_url
@@ -360,84 +381,132 @@
                                             result_tree[pv][ps][cn][nvr]["related_url"],
                                         )
                                     build_source_url = ""
                                     if result_tree[pv][ps][cn][nvr]["build_source_url"]:
                                         build_source_url = result_tree[pv][ps][cn][nvr][
                                             "build_source_url"
                                         ]
-                                    if result_tree[pv][ps][cn][nvr]["sources"]:
-                                        source_component_names = list(
-                                            set(
-                                                [
-                                                    source["name"]
-                                                    for source in result_tree[pv][ps][cn][nvr][
-                                                        "sources"
-                                                    ]
+                                    upstream_component_names = list(
+                                        set(
+                                            [
+                                                source["name"]
+                                                for source in result_tree[pv][ps][cn][nvr][
+                                                    "upstreams"
+                                                ]
+                                            ]
+                                        )
+                                    )
+                                    if upstream_component_names:
+                                        console.print(
+                                            Text(ps, style="magenta b u"),
+                                            f"[cyan]{upstream_component_names[0]} (and {len(upstream_component_names)} more)[/cyan]",  # noqa
+                                            dep,
+                                            f"([grey]{related_url}[/grey])",
+                                            no_wrap=False,
+                                        )
+                                    source_component_names = list(
+                                        set(
+                                            [
+                                                source["name"]
+                                                for source in result_tree[pv][ps][cn][nvr][
+                                                    "sources"
                                                 ]
-                                            )
+                                            ]
                                         )
-                                        for source_name in source_component_names:
-                                            console.print(
-                                                Text(ps, style="magenta b u"),
-                                                source_name,
-                                                dep,
-                                                f"([grey]{related_url}[/grey])",
-                                                no_wrap=False,
-                                            )
-                                    else:
+                                    )
+                                    if source_component_names:
+                                        console.print(
+                                            Text(ps, style="magenta b u"),
+                                            f"[light_blue]{source_component_names[0]} (and {len(source_component_names)} more)[/light_blue]",  # noqa
+                                            dep,
+                                            f"([grey]{related_url}[/grey])",
+                                            no_wrap=False,
+                                        )
+                                    if (
+                                        not result_tree[pv][ps][cn][nvr]["upstreams"]
+                                        and not result_tree[pv][ps][cn][nvr]["sources"]
+                                    ):
                                         console.print(
                                             Text(ps, style="magenta b u"),
                                             dep,
                                             f"([grey]{related_url}[/grey])",
                                             f"([grey]{build_source_url}[/grey])",
                                             no_wrap=False,
                                         )
-            if ctx.obj["VERBOSE"] > 2:  # product_stream X purl x related_url x build_source_url
+            if (
+                ctx.obj["VERBOSE"] > 2
+            ):  # product_stream X nvr (full source/upstreams) x related_url x build_source_url
                 for pv in result_tree.keys():
                     for ps in result_tree[pv].keys():
                         for cn in result_tree[pv][ps].keys():
                             if not any([match in cn for match in exclude_components]):
                                 for nvr in result_tree[pv][ps][cn].keys():
-                                    purl = result_tree[pv][ps][cn][nvr]["purl"]
-                                    dep = f"[grey93]{purl}[/grey93]"
+                                    dep_name = re.sub(
+                                        search_component_name,
+                                        f"[b]{search_component_name}[/b]",
+                                        nvr,
+                                    )
+                                    dep = f"[grey93]{dep_name}[/grey93]"
                                     related_url = ""
                                     if result_tree[pv][ps][cn][nvr]["related_url"]:
                                         related_url = re.sub(
                                             search_component_name,
                                             f"[b]{search_component_name}[/b]",
                                             result_tree[pv][ps][cn][nvr]["related_url"],
                                         )
                                     build_source_url = ""
                                     if result_tree[pv][ps][cn][nvr]["build_source_url"]:
                                         build_source_url = result_tree[pv][ps][cn][nvr][
                                             "build_source_url"
                                         ]
-                                    if result_tree[pv][ps][cn][nvr]["sources"]:
-                                        source_component_names = list(
-                                            set(
-                                                [
-                                                    source["name"]
-                                                    for source in result_tree[pv][ps][cn][nvr][
-                                                        "sources"
-                                                    ]
+                                    upstream_component_names = list(
+                                        set(
+                                            [
+                                                source["name"]
+                                                for source in result_tree[pv][ps][cn][nvr][
+                                                    "upstreams"
+                                                ]
+                                            ]
+                                        )
+                                    )
+                                    for upstream_name in upstream_component_names:
+                                        console.print(
+                                            Text(ps, style="magenta b u"),
+                                            f"[cyan]{upstream_name}[/cyan]",
+                                            dep,
+                                            f"([grey]{related_url}[/grey])",
+                                            f"([grey]{build_source_url}[/grey])",
+                                            no_wrap=False,
+                                        )
+                                    source_component_names = list(
+                                        set(
+                                            [
+                                                source["name"]
+                                                for source in result_tree[pv][ps][cn][nvr][
+                                                    "sources"
                                                 ]
-                                            )
+                                            ]
+                                        )
+                                    )
+                                    for source_name in source_component_names:
+                                        console.print(
+                                            Text(ps, style="magenta b u"),
+                                            f"[light_blue]{source_name}[/light_blue]",
+                                            dep,
+                                            f"([grey]{related_url}[/grey])",
+                                            f"([grey]{build_source_url}[/grey])",
+                                            no_wrap=False,
                                         )
-                                        for source_name in source_component_names:
-                                            console.print(
-                                                Text(ps, style="magenta b u"),
-                                                source_name,
-                                                dep,
-                                                f"([grey]{related_url}[/grey])",
-                                                no_wrap=False,
-                                            )
-                                    else:
+                                    if (
+                                        not result_tree[pv][ps][cn][nvr]["upstreams"]
+                                        and not result_tree[pv][ps][cn][nvr]["sources"]
+                                    ):
                                         console.print(
                                             Text(ps, style="magenta b u"),
-                                            f"[white]{purl}[/white]",
+                                            dep,
                                             f"([grey]{related_url}[/grey])",
                                             f"([grey]{build_source_url}[/grey])",
                                             no_wrap=False,
                                         )
 
         ctx.exit()
 
@@ -614,15 +683,15 @@
 
 
 def text_output_component_flaws(ctx, output, format):
     ordered_components = sorted(output["results"], key=lambda d: d["name"])
     for item in ordered_components:
         component_name = item["name"]
         # sorting should work when there is no title or cve-id key
-        ordered_affects = sorted(item["affects"], key=lambda d: (d["title"] is None, d["title"]))
+        ordered_affects = sorted(item["affects"], key=lambda d: d["flaw_cve_id"])
         for affect in ordered_affects:
             flaw_cve_id = "Vulnerability"
             if affect["flaw_cve_id"]:
                 flaw_cve_id = affect["flaw_cve_id"]
             if ctx.obj["VERBOSE"] == 0:
                 console.print(
                     Text(flaw_cve_id, style="magenta"),
```

### Comparing `griffon-0.2.1/griffon/services/__init__.py` & `griffon-0.2.2/griffon/services/__init__.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/griffon/services/core_process.py` & `griffon-0.2.2/griffon/services/core_process.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/griffon/services/core_queries.py` & `griffon-0.2.2/griffon/services/core_queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
     components = list()
     if component_cnt < 120:
         components.extend(components_initial.results)
     elif component_cnt > 120:
         components.extend(components_initial.results)
         with concurrent.futures.ThreadPoolExecutor() as executor:
             futures = []
-            for batch in range(120, 600, 120):
+            for batch in range(120, 1200, 120):
                 futures.append(
                     executor.submit(
                         corgi_session.components.retrieve_list,
                         **params,
                         offset=batch,
                         limit=120,  # noqa
                     )
@@ -318,32 +318,34 @@
                 self.corgi_session, params, component_initial, component_initial.count
             )
             results.extend(latest_components)
 
         if self.search_related_url:
             # Note: related_url filter has no concept of strict
             params["related_url"] = self.component_name
-            params["namespace"] = "REDHAT"
+            if self.ns:
+                params["namespace"] = self.ns
             if self.component_type:
                 params["type"] = self.component_type
 
             component_initial = self.corgi_session.components.retrieve_list(limit=120, **params)
             related_url_components: list = async_retrieve_components(
                 self.corgi_session, params, component_initial, component_initial.count
             )
             results.extend(related_url_components)
 
         if self.search_all:
-            # params["type"] ="RPM"
             if not self.strict_name_search:
                 params["re_name"] = self.component_name
             else:
                 params["name"] = self.component_name
             if self.component_type:
                 params["type"] = self.component_type
+            if self.ns:
+                params["namespace"] = self.ns
 
             all_component_initial = self.corgi_session.components.retrieve_list(limit=120, **params)
             all_components: list = async_retrieve_components(
                 self.corgi_session,
                 params,
                 all_component_initial,
                 all_component_initial.count,
@@ -353,14 +355,16 @@
         if self.search_all_roots:
             params["type"] = "RPM"
             params["arch"] = "src"
             if not self.strict_name_search:
                 params["re_name"] = self.component_name
             else:
                 params["name"] = self.component_name
+            if self.ns:
+                params["namespace"] = self.ns
 
             all_src_component_initial = self.corgi_session.components.retrieve_list(
                 limit=120, **params
             )
             all_src_components: list = async_retrieve_components(
                 self.corgi_session,
                 params,
@@ -443,14 +447,18 @@
             self.community_session = CommunityComponentService.create_session()
             params["type"] = "RPM"
             params["arch"] = "src"
             if not self.strict_name_search:
                 params["re_name"] = self.component_name
             else:
                 params["name"] = self.component_name
+            if self.search_upstreams:
+                params["namespace"] = "UPSTREAM"
+            if self.ns:
+                params["namespace"] = self.ns
 
             if self.component_type:
                 params["type"] = self.component_type
 
             component_initial = self.community_session.components.retrieve_list(limit=120, **params)
             commmunity_src_components: list = async_retrieve_components(
                 self.community_session, params, component_initial, component_initial.count
```

### Comparing `griffon-0.2.1/griffon/services/core_reports.py` & `griffon-0.2.2/griffon/services/core_reports.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/griffon/static/default_griffonrc` & `griffon-0.2.2/griffon/static/default_griffonrc`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/griffon.egg-info/PKG-INFO` & `griffon-0.2.2/griffon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griffon
-Version: 0.2.1
+Version: 0.2.2
 Summary: Red Hat Product Security CLI
 Home-page: https://github.com/RedHatProductSecurity/griffon
 Author: James Fuller, Red Hat Product Security
 License: MIT
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `griffon-0.2.1/griffon.egg-info/SOURCES.txt` & `griffon-0.2.2/griffon.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 griffon/commands/queries.py
 griffon/commands/reports.py
 griffon/commands/entities/__init__.py
 griffon/commands/entities/community_component_registry.py
 griffon/commands/entities/corgi.py
 griffon/commands/entities/helpers.py
 griffon/commands/entities/osidb.py
+griffon/commands/plugins/bugzilla.py
 griffon/commands/plugins/cve_mitre.py
 griffon/commands/plugins/cvelib.py
 griffon/commands/plugins/fcc.py
 griffon/commands/plugins/go_vuln.py
 griffon/commands/plugins/osv.py
 griffon/commands/plugins/semgrep.py
 griffon/services/__init__.py
```

### Comparing `griffon-0.2.1/pyproject.toml` & `griffon-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/setup.py` & `griffon-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/tests/test_cli.py` & `griffon-0.2.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/tests/test_entities.py` & `griffon-0.2.2/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/tests/test_manage.py` & `griffon-0.2.2/tests/test_manage.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/tests/test_plugins.py` & `griffon-0.2.2/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/tests/test_process.py` & `griffon-0.2.2/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/tests/test_queries.py` & `griffon-0.2.2/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/tests/test_reports.py` & `griffon-0.2.2/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.1/tests/test_unit.py` & `griffon-0.2.2/tests/test_unit.py`

 * *Files identical despite different names*

