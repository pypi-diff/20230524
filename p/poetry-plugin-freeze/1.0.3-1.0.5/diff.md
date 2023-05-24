# Comparing `tmp/poetry_plugin_freeze-1.0.3.tar.gz` & `tmp/poetry_plugin_freeze-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_freeze-1.0.3.tar", max compression
+gzip compressed data, was "poetry_plugin_freeze-1.0.5.tar", max compression
```

## Comparing `poetry_plugin_freeze-1.0.3.tar` & `poetry_plugin_freeze-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,22 @@
--rw-r--r--   0        0        0     3073 2023-03-27 17:22:29.557376 poetry_plugin_freeze-1.0.3/README.md
--rw-r--r--   0        0        0      946 2023-03-27 17:22:29.561376 poetry_plugin_freeze-1.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-27 17:22:29.561376 poetry_plugin_freeze-1.0.3/src/poetry_plugin_freeze/__init__.py
--rw-r--r--   0        0        0     8214 2023-03-27 17:22:29.561376 poetry_plugin_freeze-1.0.3/src/poetry_plugin_freeze/app.py
--rw-r--r--   0        0        0      317 2023-03-27 17:22:29.561376 poetry_plugin_freeze-1.0.3/tests/conftest.py
--rw-r--r--   0        0        0        2 2023-03-27 17:22:29.561376 poetry_plugin_freeze-1.0.3/tests/fixtures/nested_packages/app_b/__init__.py
--rw-r--r--   0        0        0     1027 2023-03-27 17:22:29.561376 poetry_plugin_freeze-1.0.3/tests/fixtures/nested_packages/dist/app_b-0.1-py3-none-any.whl
--rw-r--r--   0        0        0        0 2023-03-27 17:22:29.561376 poetry_plugin_freeze-1.0.3/tests/fixtures/nested_packages/others/app_c/app_c/__init__.py
--rw-r--r--   0        0        0     1025 2023-03-27 17:22:29.561376 poetry_plugin_freeze-1.0.3/tests/fixtures/nested_packages/others/app_c/dist/app_c-0.2-py3-none-any.whl
--rw-r--r--   0        0        0    14149 2023-03-27 17:22:29.561376 poetry_plugin_freeze-1.0.3/tests/fixtures/nested_packages/others/app_c/poetry.lock
--rw-r--r--   0        0        0      415 2023-03-27 17:22:29.561376 poetry_plugin_freeze-1.0.3/tests/fixtures/nested_packages/others/app_c/pyproject.toml
--rw-r--r--   0        0        0     7605 2023-03-27 17:22:29.561376 poetry_plugin_freeze-1.0.3/tests/fixtures/nested_packages/poetry.lock
--rw-r--r--   0        0        0      405 2023-03-27 17:22:29.561376 poetry_plugin_freeze-1.0.3/tests/fixtures/nested_packages/pyproject.toml
--rw-r--r--   0        0        0     2312 2023-03-27 17:22:29.561376 poetry_plugin_freeze-1.0.3/tests/fixtures/whl_info/METADATA
--rw-r--r--   0        0        0     4010 2023-03-27 17:22:29.561376 poetry_plugin_freeze-1.0.3/tests/fixtures/whl_info/RECORD
--rw-r--r--   0        0        0     4146 2023-03-27 17:22:29.561376 poetry_plugin_freeze-1.0.3/tests/test_freeze.py
--rw-r--r--   0        0        0     3866 1970-01-01 00:00:00.000000 poetry_plugin_freeze-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     4650 2023-05-24 12:20:35.866163 poetry_plugin_freeze-1.0.5/README.md
+-rw-r--r--   0        0        0      946 2023-05-24 12:20:35.866163 poetry_plugin_freeze-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 12:20:35.866163 poetry_plugin_freeze-1.0.5/src/poetry_plugin_freeze/__init__.py
+-rw-r--r--   0        0        0    11958 2023-05-24 12:20:35.866163 poetry_plugin_freeze-1.0.5/src/poetry_plugin_freeze/app.py
+-rw-r--r--   0        0        0      317 2023-05-24 12:20:35.866163 poetry_plugin_freeze-1.0.5/tests/conftest.py
+-rw-r--r--   0        0        0        2 2023-05-24 12:20:35.866163 poetry_plugin_freeze-1.0.5/tests/fixtures/nested_packages/app_b/__init__.py
+-rw-r--r--   0        0        0     1027 2023-05-24 12:20:35.870163 poetry_plugin_freeze-1.0.5/tests/fixtures/nested_packages/dist/app_b-0.1-py3-none-any.whl
+-rw-r--r--   0        0        0        0 2023-05-24 12:20:35.870163 poetry_plugin_freeze-1.0.5/tests/fixtures/nested_packages/others/app_c/app_c/__init__.py
+-rw-r--r--   0        0        0     1025 2023-05-24 12:20:35.870163 poetry_plugin_freeze-1.0.5/tests/fixtures/nested_packages/others/app_c/dist/app_c-0.2-py3-none-any.whl
+-rw-r--r--   0        0        0    14149 2023-05-24 12:20:35.870163 poetry_plugin_freeze-1.0.5/tests/fixtures/nested_packages/others/app_c/poetry.lock
+-rw-r--r--   0        0        0      415 2023-05-24 12:20:35.870163 poetry_plugin_freeze-1.0.5/tests/fixtures/nested_packages/others/app_c/pyproject.toml
+-rw-r--r--   0        0        0       82 2023-05-24 12:20:35.870163 poetry_plugin_freeze-1.0.5/tests/fixtures/nested_packages/others/app_with_extras/README.md
+-rw-r--r--   0        0        0        0 2023-05-24 12:20:35.870163 poetry_plugin_freeze-1.0.5/tests/fixtures/nested_packages/others/app_with_extras/app_with_extras/__init__.py
+-rw-r--r--   0        0        0     1326 2023-05-24 12:20:35.870163 poetry_plugin_freeze-1.0.5/tests/fixtures/nested_packages/others/app_with_extras/dist/app_with_extras-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0    16277 2023-05-24 12:20:35.870163 poetry_plugin_freeze-1.0.5/tests/fixtures/nested_packages/others/app_with_extras/poetry.lock
+-rw-r--r--   0        0        0      654 2023-05-24 12:20:35.870163 poetry_plugin_freeze-1.0.5/tests/fixtures/nested_packages/others/app_with_extras/pyproject.toml
+-rw-r--r--   0        0        0     7605 2023-05-24 12:20:35.870163 poetry_plugin_freeze-1.0.5/tests/fixtures/nested_packages/poetry.lock
+-rw-r--r--   0        0        0      405 2023-05-24 12:20:35.870163 poetry_plugin_freeze-1.0.5/tests/fixtures/nested_packages/pyproject.toml
+-rw-r--r--   0        0        0     2312 2023-05-24 12:20:35.870163 poetry_plugin_freeze-1.0.5/tests/fixtures/whl_info/METADATA
+-rw-r--r--   0        0        0     4010 2023-05-24 12:20:35.870163 poetry_plugin_freeze-1.0.5/tests/fixtures/whl_info/RECORD
+-rw-r--r--   0        0        0     5575 2023-05-24 12:20:35.870163 poetry_plugin_freeze-1.0.5/tests/test_freeze.py
+-rw-r--r--   0        0        0     5443 1970-01-01 00:00:00.000000 poetry_plugin_freeze-1.0.5/PKG-INFO
```

### Comparing `poetry_plugin_freeze-1.0.3/pyproject.toml` & `poetry_plugin_freeze-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-freeze"
-version = "1.0.3"
+version = "1.0.5"
 description = "Poetry plugin to freeze a wheel's dependencies per lock file"
 license = "Apache-2.0"
 authors = ["Kapil Thangavelu <kapilt@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/cloud-custodian/poetry-plugin-freeze"
 
 packages = [
```

### Comparing `poetry_plugin_freeze-1.0.3/src/poetry_plugin_freeze/app.py` & `poetry_plugin_freeze-1.0.5/src/poetry_plugin_freeze/app.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from base64 import urlsafe_b64encode
 import csv
 from email.parser import Parser
+from functools import lru_cache
 import hashlib
 from io import StringIO, TextIOWrapper
 from pathlib import Path
 import shutil
 import os
 import tempfile
 import zipfile
 
 from cleo.helpers import option
 from poetry.console.commands.command import Command
 from poetry.core.packages.dependency_group import MAIN_GROUP
+from poetry.core.version.markers import MultiMarker, SingleMarker
 from poetry.packages import DependencyPackage
 from poetry.core.masonry.metadata import Metadata
 from poetry.core.masonry.utils.helpers import distribution_name
+from poetry.core.version.markers import union as marker_union
 from poetry.factory import Factory
 from poetry.plugins.application_plugin import ApplicationPlugin
 
-from poetry_plugin_export.walker import get_project_dependency_packages
+from poetry_plugin_export.walker import get_project_dependency_packages, walk_dependencies
 
 
 class FreezeCommand(Command):
     name = "freeze-wheel"
 
     options = [option("wheel-dir", None, "Sub-directory containing wheels")]
 
@@ -117,23 +120,98 @@
 
         dep_packages = list(
             get_project_dependency_packages(
                 self.poetry.locker,
                 project_requires=root_package.all_requires,
                 root_package_name=root_package.name,
                 project_python_marker=root_package.python_marker,
+                extras=root_package.extras,
             )
         )
         return {p.package.name: p for p in dep_packages}
 
+    @lru_cache(maxsize=None)
+    def get_dependency_sources(self):
+        """Determine the root source of each locked dependency
+
+        For each locked dependency, determine whether it came
+        as a base requirement or part of one or more extras.
+        """
+
+        def _with_python_marker(requirements, root_package):
+            """Augment requirements with the root package's python marker"""
+            marked_requirements = []
+            for require in requirements:
+                require = require.clone()
+                require.marker = require.marker.intersect(root_package.python_marker)
+                marked_requirements.append(require)
+            return marked_requirements
+
+        repository = self.poetry.locker.locked_repository()
+        root_package = self.poetry.package
+        locked_packages_by_name = {p.name: [p] for p in repository.packages}
+        dependency_sources = {}
+        base_requires = [
+            dep
+            for dep in root_package.requires
+            if not dep.is_optional() or set(dep.in_extras) <= root_package.features
+        ]
+
+        # Identify nested dependencies that don't require extra selections.
+        base_nested_dependencies = walk_dependencies(
+            _with_python_marker(base_requires, root_package),
+            packages_by_name=locked_packages_by_name,
+            root_package_name=root_package.name,
+        )
+        for d in base_nested_dependencies:
+            dependency_sources.setdefault(d.name, set()).add("base")
+
+        # Identify nested dependencies that come from one or more extra
+        # selections.
+        for extra in root_package.extras:
+            extra_nested_dependencies = walk_dependencies(
+                _with_python_marker(root_package.extras[extra], root_package),
+                packages_by_name=locked_packages_by_name,
+                root_package_name=root_package.name,
+            )
+            for d in extra_nested_dependencies:
+                dependency_sources.setdefault(d.name, set()).add(extra)
+        return dependency_sources
+
+    def compact_markers(self, dependency):
+        """Update a dependency to consolidate its markers.
+
+        This avoids duplication when there are multiple markers
+        (for sets of python versions, for example). It also records
+        extra dependency markers which are lost in the conversion
+        from installed package to dependency.
+        """
+        dep_sources = self.get_dependency_sources().get(dependency.name, set())
+
+        # Record extra markers only if a dependency is not included
+        # in the base requirement set.
+        new_marker = dependency.marker.without_extras()
+        in_base = "base" in dep_sources
+        in_extras = dep_sources - {"base"}
+        if in_extras and not in_base:
+            extra_markers = marker_union(*(SingleMarker("extra", extra) for extra in in_extras))
+            new_marker = MultiMarker(new_marker, extra_markers)
+        dependency.marker = new_marker
+
     def get_frozen_deps(self, dep_packages):
         lines = []
+        dependency_sources = self.get_dependency_sources()
         for pkg_name, dep_package in dep_packages.items():
+            self.compact_markers(dep_package.dependency)
             require_dist = "%s (==%s)" % (pkg_name, dep_package.package.version)
-            requirement = dep_package.dependency.to_pep_508(with_extras=False)
+            # Freeze extra markers for dependencies which were pulled in via extras
+            # Don't freeze markers if a dependency is also part of the base
+            # dependency tree.
+            freeze_extras = "base" not in dependency_sources.get(dep_package.dependency.name, set())
+            requirement = dep_package.dependency.to_pep_508(with_extras=freeze_extras)
             if ";" in requirement:
                 markers = requirement.split(";", 1)[1].strip()
                 require_dist += f" ; {markers}"
             lines.append(require_dist)
         return lines
 
     def replace_deps(self, dist_meta, dep_lines):
@@ -153,20 +231,21 @@
         package_deps = {}
         group = self.poetry.package.dependency_group(group)
         for dep in group.dependencies:
             if not (dep.is_file() or dep.is_directory()):
                 continue
             if dep.is_vcs() or dep.is_url():
                 continue
-            assert dep.name in self.fridge, f"Unknown path dependency {dep.name}"
-            iced = self.fridge[dep.name]
-            package_deps[dep.name] = DependencyPackage(
-                dependency=iced.poetry.package.to_dependency(), package=iced.poetry.package
-            )
-            package_deps.update(iced.get_dep_packages())
+            iced = IcedPoet(dep.full_path)
+            # Carry markers from the root package dependency through to the iced package
+            self.compact_markers(dep)
+            iced_dep = iced.poetry.package.to_dependency()
+            iced_dep.marker = MultiMarker(dep.marker, iced_dep.marker)
+            package_dep = DependencyPackage(dependency=iced_dep, package=iced.poetry.package)
+            package_deps[dep.name] = package_dep
         return package_deps
 
     def freeze_record(self, records_fh, dist_meta, md_path):
         hash_digest = get_sha256_digest(str(dist_meta).encode("utf8"))
         output = StringIO()
         csv_params = {
             "delimiter": csv.excel.delimiter,
@@ -192,15 +271,15 @@
         md_path = f"{dist_info}/METADATA"
         record_path = f"{dist_info}/RECORD"
 
         with zipfile.ZipFile(wheel_path) as source_whl:
             # freeze deps in metadata and update records
             md_text = source_whl.open(md_path).read().decode("utf8")
             dist_meta = Parser().parsestr(md_text)
-            deps = self.get_path_deps()
+            deps = self.get_path_deps(MAIN_GROUP)
             deps.update(dep_packages)
             dep_lines = self.get_frozen_deps(deps)
             self.replace_deps(dist_meta, dep_lines)
 
             with source_whl.open(record_path) as record_fh:
                 record_text = self.freeze_record(record_fh, dist_meta, md_path)
```

### Comparing `poetry_plugin_freeze-1.0.3/tests/fixtures/nested_packages/dist/app_b-0.1-py3-none-any.whl` & `poetry_plugin_freeze-1.0.5/tests/fixtures/nested_packages/dist/app_b-0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_plugin_freeze-1.0.3/tests/fixtures/nested_packages/others/app_c/dist/app_c-0.2-py3-none-any.whl` & `poetry_plugin_freeze-1.0.5/tests/fixtures/nested_packages/others/app_c/dist/app_c-0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_plugin_freeze-1.0.3/tests/fixtures/nested_packages/others/app_c/poetry.lock` & `poetry_plugin_freeze-1.0.5/tests/fixtures/nested_packages/others/app_c/poetry.lock`

 * *Files identical despite different names*

### Comparing `poetry_plugin_freeze-1.0.3/tests/fixtures/nested_packages/poetry.lock` & `poetry_plugin_freeze-1.0.5/tests/fixtures/nested_packages/poetry.lock`

 * *Files identical despite different names*

### Comparing `poetry_plugin_freeze-1.0.3/tests/fixtures/whl_info/METADATA` & `poetry_plugin_freeze-1.0.5/tests/fixtures/whl_info/METADATA`

 * *Files identical despite different names*

### Comparing `poetry_plugin_freeze-1.0.3/tests/fixtures/whl_info/RECORD` & `poetry_plugin_freeze-1.0.5/tests/fixtures/whl_info/RECORD`

 * *Files identical despite different names*

### Comparing `poetry_plugin_freeze-1.0.3/PKG-INFO` & `poetry_plugin_freeze-1.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-freeze
-Version: 1.0.3
+Version: 1.0.5
 Summary: Poetry plugin to freeze a wheel's dependencies per lock file
 Home-page: https://github.com/cloud-custodian/poetry-plugin-freeze
 License: Apache-2.0
 Author: Kapil Thangavelu
 Author-email: kapilt@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -34,14 +34,42 @@
 
 A post build / pre publish command to allow for creating wheels with frozen dependencies. Basically we update wheel metadata for Requires-Dist to replace the pyproject.toml based version specification to a frozen (ie. ==version) one based on the version from the poetry lock information.
 
 
 Note we can't use poetry to publish because the frozen wheel because it uses metadata from pyproject.toml instead
 of frozen wheel metadata.
 
+### Optional Dependencies
+
+Frozen wheel metadata will contain [Provides-Extra](https://packaging.python.org/en/latest/specifications/core-metadata/#provides-extra-multiple-use) entries for any [extra / optional dependencies](https://packaging.python.org/en/latest/specifications/declaring-project-metadata/#dependencies-optional-dependencies). Frozen [Requires-Dist](https://packaging.python.org/en/latest/specifications/core-metadata/#core-metadata-requires-dist) lines will specify `extra` names _for packages that appear only in the optional/extra dependency graph.
+
+If a package appears as both a nested "main" dependency and also as an "extra" dependency, its `Requires-Dist` entry in the frozen wheel _will not_ specify an extra name.
+
+To define this behavior in relation to poetry's [export plugin](https://github.com/python-poetry/poetry-plugin-export/), these two flows should result in the same installed package set:
+
+```console
+# Export Flow
+poetry export -f requirements.txt > requirements.txt && pip install -r requirements.txt
+
+# Freeze-wheel Flow
+poetry build && poetry freeze-wheel && pip install my_frozen_wheel
+```
+
+And introducing extras:
+
+```console
+# Export Flow
+poetry export --extras gcp -f requirements.txt && pip install -r requirements.txt
+
+# Freeze-wheel Flow
+poetry build && poetry freeze-wheel && pip install my_frozen_wheel[gcp]
+```
+
+The difference is in when to choose which extras to install - `export` does that at freeze time. `freeze-wheel` embeds the extra _context_ at freeze time, but defers the actual extra selection until install time.
+
 ## Usage
 
 ```shell
 # install plugin
 poetry self add poetry-plugin-freeze
 
 # build per normal
@@ -55,20 +83,11 @@
 
 # publish per normal
 twine upload dist/*.whl
 ```
 
 ## Mono-Repo Support
 
-To support mono repos consisting of multiple libraries/applications, when creating a frozen wheel, dev dependencies specified by path can be optionally substituted out for references to their release artifact versions.
+To support mono repos consisting of multiple libraries/applications, when creating a frozen wheel, main group dependencies specified by path can be optionally substituted out for references to their release artifact versions.
 
 This assumes automation to run build and publish across the various subpackages, ie typically via make or just.
 
-
-
-
-
-
-
-
-
-
```

