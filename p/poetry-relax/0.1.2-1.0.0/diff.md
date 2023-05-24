# Comparing `tmp/poetry-relax-0.1.2.tar.gz` & `tmp/poetry_relax-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry-relax-0.1.2.tar", max compression
+gzip compressed data, was "poetry_relax-1.0.0.tar", max compression
```

## Comparing `poetry-relax-0.1.2.tar` & `poetry_relax-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-05-23 15:47:55.953304 poetry-relax-0.1.2/LICENSE
--rw-r--r--   0        0        0     6496 2023-05-23 15:47:55.953304 poetry-relax-0.1.2/README.md
--rw-r--r--   0        0        0     1411 2023-05-23 15:48:35.935095 poetry-relax-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      434 2023-05-23 15:47:55.953304 poetry-relax-0.1.2/src/poetry_relax/__init__.py
--rw-r--r--   0        0        0     7559 2023-05-23 15:47:55.953304 poetry-relax-0.1.2/src/poetry_relax/_core.py
--rw-r--r--   0        0        0     7830 2023-05-23 15:47:55.953304 poetry-relax-0.1.2/src/poetry_relax/command.py
--rw-r--r--   0        0        0        0 2023-05-23 15:47:55.953304 poetry-relax-0.1.2/src/poetry_relax/py.typed
--rw-r--r--   0        0        0     7484 1970-01-01 00:00:00.000000 poetry-relax-0.1.2/setup.py
--rw-r--r--   0        0        0     7892 1970-01-01 00:00:00.000000 poetry-relax-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-24 01:01:19.675124 poetry_relax-1.0.0/LICENSE
+-rw-r--r--   0        0        0     7715 2023-05-24 01:01:19.675124 poetry_relax-1.0.0/README.md
+-rw-r--r--   0        0        0     1412 2023-05-24 01:01:44.396923 poetry_relax-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      434 2023-05-24 01:01:19.675124 poetry_relax-1.0.0/src/poetry_relax/__init__.py
+-rw-r--r--   0        0        0     8033 2023-05-24 01:01:19.675124 poetry_relax-1.0.0/src/poetry_relax/_core.py
+-rw-r--r--   0        0        0    11925 2023-05-24 01:01:19.675124 poetry_relax-1.0.0/src/poetry_relax/command.py
+-rw-r--r--   0        0        0        0 2023-05-24 01:01:19.675124 poetry_relax-1.0.0/src/poetry_relax/py.typed
+-rw-r--r--   0        0        0     8862 1970-01-01 00:00:00.000000 poetry_relax-1.0.0/PKG-INFO
```

### Comparing `poetry-relax-0.1.2/LICENSE` & `poetry_relax-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry-relax-0.1.2/pyproject.toml` & `poetry_relax-1.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-relax"
-version = "0.1.2"
+version = "1.0.0"
 repository = "https://github.com/madkinsz/poetry-relax"
 description = "Plugin for Poetry to relax upper version pins"
 authors = ["Zanie <contact@zanie.dev>"]
 readme = "README.md"
 keywords = ["poetry", "plugin", "versioning", "version"]
 packages = [{ include = "poetry_relax", from = "src" }]
 classifiers = [
@@ -35,12 +35,12 @@
 
 [tool.poetry.group.dev.dependencies]
 black = ">=7.1.3"
 isort = ">=2.5.0"
 pytest = ">=7.1.3"
 pytest-xdist = ">=2.5.0"
 mypy = ">=0.971"
-types-setuptools = "^67.6.0.5"
+types-setuptools = ">=67.6.0.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `poetry-relax-0.1.2/src/poetry_relax/_core.py` & `poetry_relax-1.0.0/src/poetry_relax/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,25 @@
 Core utilities for the `poetry relax` functionality.
 """
 import contextlib
 import functools
 import re
 import sys
 from copy import copy
-from typing import TYPE_CHECKING, Any, Callable, Iterable, Optional
+from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable, Optional
 
 import packaging.version
+from poetry.core.packages.dependency_group import MAIN_GROUP
+
+if TYPE_CHECKING:
+    # See https://github.com/python-poetry/cleo/pull/254 for ignore
+    from cleo.io.io import IO  # type: ignore
+    from poetry.core.packages.dependency import Dependency
+    from poetry.installation.installer import Installer
+    from poetry.poetry import Poetry
 
 if sys.version_info < (3, 8):  # Python 3.7 support
     import pkg_resources
 
     POETRY_VERSION = packaging.version.Version(
         pkg_resources.get_distribution("poetry").version
     )
@@ -23,22 +31,24 @@
 
 
 if POETRY_VERSION < packaging.version.Version("1.3.0"):
     from poetry.core.semver.version_range import VersionRange
 else:
     from poetry.core.constraints.version import VersionRange
 
-from poetry.core.packages.dependency_group import MAIN_GROUP
 
-if TYPE_CHECKING:
-    # See https://github.com/python-poetry/cleo/pull/254 for ignore
-    from cleo.io.io import IO  # type: ignore
-    from poetry.core.packages.dependency import Dependency
-    from poetry.installation.installer import Installer
-    from poetry.poetry import Poetry
+if POETRY_VERSION < packaging.version.Version("1.3.0"):
+    # Poetry 1.2.x defined a different name for Cleo 1.x
+    # isort: off
+    from poetry.console.exceptions import (  # type: ignore
+        PoetrySimpleConsoleException as PoetryConsoleError,
+    )
+else:
+    from poetry.console.exceptions import PoetryConsoleError  # noqa: F401
+
 
 # Regular expressions derived from `poetry.core.semver.helpers.parse_constraint`
 # These are used to parse complex constraint strings into single constraints
 AND_CONSTRAINT_SEPARATORS = re.compile(
     r"((?<!^)(?<![~=>< ,]) *(?<!-)[, ](?!-) *(?!,|$))"
 )
 OR_CONSTRAINT_SEPARATORS = re.compile(r"(\s*\|\|?\s*)")
@@ -62,44 +72,45 @@
         io.write_line = write_line  # type: ignore
         io.write = write  # type:ignore
 
 
 def run_installer_update(
     poetry: "Poetry",
     installer: "Installer",
-    dependencies: Iterable["Dependency"],
-    dependency_group_name: str,
+    dependencies_by_group: Dict[str, Iterable["Dependency"]],
     poetry_config: dict,
     dry_run: bool,
     lockfile_only: bool,
     verbose: bool,
     silent: bool,
 ) -> int:
     """
     Run an installer update.
 
-    Ensures that any existing dependencies in the given group are replaced with the new
+    Ensures that any existing dependencies in the given groups are replaced with the new
     dependencies if their names match.
 
     New dependencies are also whitelisted to be updated during locking.
     """
-    group = poetry.package.dependency_group(dependency_group_name)
 
-    # Ensure if we are given a generator that we can consume it more than once
-    dependencies = list(dependencies)
+    for group_name, dependencies in dependencies_by_group.items():
+        group = poetry.package.dependency_group(group_name)
 
-    for dependency in dependencies:
-        with contextlib.suppress(ValueError):
-            group.remove_dependency(dependency.name)
-        group.add_dependency(dependency)
+        # Ensure if we are given a generator that we can consume it more than once
+        dependencies = list(dependencies)
+
+        for dependency in dependencies:
+            with contextlib.suppress(ValueError):
+                group.remove_dependency(dependency.name)
+            group.add_dependency(dependency)
 
     # Refresh the locker
     poetry.set_locker(poetry.locker.__class__(poetry.locker.lock, poetry_config))
     installer.set_locker(poetry.locker)
-
+    installer.only_groups(dependencies_by_group.keys())
     installer.set_package(poetry.package)
     installer.dry_run(dry_run)
     installer.verbose(verbose)
     installer.update()
 
     if lockfile_only:
         installer.lock()
```

### Comparing `poetry-relax-0.1.2/src/poetry_relax/command.py` & `poetry_relax-1.0.0/src/poetry_relax/command.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,72 @@
-from typing import Any
+from collections import defaultdict
+from typing import Any, Dict, List, Set, Tuple
 
 # cleo is not PEP 561 compliant must be ignored
 # See https://github.com/python-poetry/cleo/pull/254
 from cleo.helpers import option  # type: ignore
+from packaging.version import Version
 from poetry.console.commands.init import InitCommand
 from poetry.console.commands.installer_command import InstallerCommand
 from poetry.core.factory import Factory
-from poetry.core.packages.dependency_group import MAIN_GROUP
+from poetry.core.packages.dependency import Dependency
 from tomlkit.toml_document import TOMLDocument
 
 from poetry_relax._core import (
+    POETRY_VERSION,
+    PoetryConsoleError,
     drop_caret_bound_from_dependency,
     extract_dependency_config_for_group,
     run_installer_update,
 )
 
 
+def _pretty_group(group: str) -> str:
+    return f" in group <c1>{group!r}</c1>"
+
+
 class RelaxCommand(InitCommand, InstallerCommand):
     """
     Implementation of `poetry relax`.
     """
 
     # This inherits from `InitCommand` and `InstallerCommand` for access to internal
     # utilities
 
     name = "relax"
     description = "Relax project dependencies."
     options = [
         option(
+            "only",
+            description=(
+                "A group to relax constraints in. If not provided, all groups are used"
+                "; including optional groups."
+                # If a group is specified, it is treated like the Poetry `--only` flag.
+            ),
+            flag=False,
+            default=None,
+            multiple=True,
+        ),
+        option(
             "group",
             "-G",
-            description="The group relax constraints in.",
             flag=False,
-            default=MAIN_GROUP,
+            default=None,
+            description=(
+                "A group to relax constraints in."
+                " (<warning>Deprecated; use `--only` instead.</warning>)"
+            ),
+            multiple=True,
+        ),
+        option(
+            "without",
+            description="A group to exclude from relaxing constraints.",
+            flag=False,
+            default=None,
+            multiple=True,
         ),
         option(
             "dry-run",
             None,
             description=("Output the operations but do not execute anything."),
         ),
         option(
@@ -57,14 +87,26 @@
         ),
     ]
     help = (
         "The <c1>relax</> command removes upper version constraints designated by "
         "carets (<c2>^</>)."
     )
 
+    def _get_only_group_option(self):
+        only = self.option("only")
+        deprecated_groups = self.option("group")
+
+        if deprecated_groups:
+            self.line(
+                "<warning>The `--group` option is deprecated; use `--only` instead."
+                "</warning>"
+            )
+
+        return set(only + deprecated_groups)
+
     def handle(self) -> int:
         """
         The plugin entrypoint for the `poetry relax` command.
         """
 
         # The following implemention relies heavily on internal Poetry objects and
         # is based on the `poetry add` implementation which is available under the MIT
@@ -72,67 +114,106 @@
 
         # Read poetry file as a dictionary
         if self.io.is_verbose():
             self.line(f"Using poetry file at {self.poetry.file.path}")
         pyproject_config: dict[str, Any] = self.poetry.file.read()
         poetry_config = pyproject_config["tool"]["poetry"]
 
-        # Load dependencies in the given group
-        group = self.option("group")
-        pretty_group = f" in group <c1>{group!r}</c1>" if group != MAIN_GROUP else ""
-
-        self.info(f"Checking dependencies{pretty_group} for relaxable constraints...")
-
-        dependency_config = extract_dependency_config_for_group(group, poetry_config)
-        if dependency_config is None:
-            self.line(f"No dependencies found{pretty_group}.")
-            # Return a bad status code as the user likely provided a bad group
+        # Validate given groups using Poetry's internal handler
+        self._validate_group_options(
+            {opt: (self.option(opt) or set()) for opt in {"only", "without", "group"}}
+        )
+
+        groups = [
+            str(group)
+            for group in (
+                self._get_only_group_option()
+                # Use all groups by default, including optional groups
+                or sorted(
+                    self.poetry.package.dependency_group_names(include_optional=True)
+                )
+            )
+            # Exclude groups specified by the `--without` option
+            if group not in self.option("without")
+        ]
+
+        if not groups:
+            self.info("No groups to relax.")
             return 1
 
-        # Parse the dependencies
-        target_dependencies = [
-            Factory.create_dependency(name, constraints)
-            for name, constraints in dependency_config.items()
-            if name != "python"
-        ]
+        updated_dependencies: Dict[
+            str, List[Tuple[str, Dependency]]
+        ] = {}  # Dependencies updated per group
+
+        for group in groups:
+            # Load dependencies in the given group
+            pretty_group = _pretty_group(group)
+            self.info(
+                f"Checking dependencies{pretty_group} for relaxable constraints..."
+            )
 
-        if not target_dependencies:
-            self.line("No dependencies to relax{pretty_group}.")
-            return 0
+            dependency_config = extract_dependency_config_for_group(
+                group, poetry_config
+            )
+            if dependency_config is None:
+                self.line(f"No dependencies found{pretty_group}.")
+                continue
+
+            # Parse the dependencies
+            target_dependencies = [
+                Factory.create_dependency(name, constraints)
+                for name, constraints in dependency_config.items()
+                if name != "python"
+            ]
+
+            if not target_dependencies:
+                self.line(f"No dependencies to relax{pretty_group}.")
+                updated_dependencies[group] = []
+                continue
 
-        if self.io.is_verbose():
-            self.line(f"Found {len(target_dependencies)} dependencies{pretty_group}.")
+            if self.io.is_verbose():
+                self.line(
+                    f"Found {len(target_dependencies)} dependencies{pretty_group}."
+                )
 
-        # Construct new dependency objects with the max constraint removed
-        new_dependencies = [
-            drop_caret_bound_from_dependency(d) for d in target_dependencies
-        ]
+            # Construct new dependency objects with the max constraint removed
+            new_dependencies = [
+                drop_caret_bound_from_dependency(d) for d in target_dependencies
+            ]
+
+            updated_dependencies[group] = [
+                (old.pretty_constraint, new)
+                for old, new in zip(target_dependencies, new_dependencies)
+                # We use the pretty constraint in updates to retain the user's string
+                if old.pretty_constraint != new.pretty_constraint
+            ]
 
-        updated_dependencies = [
-            (old.pretty_constraint, new)
-            for old, new in zip(target_dependencies, new_dependencies)
-            # We use the pretty constraint in updates to retain the user's string
-            if old.pretty_constraint != new.pretty_constraint
-        ]
+            if self.io.is_verbose():
+                self.line(
+                    f"Proposing updates to {len(updated_dependencies[group])} "
+                    f"dependencies{pretty_group}."
+                )
 
-        if not updated_dependencies:
+        updated_count = sum(len(deps) for deps in updated_dependencies.values())
+        if not updated_count:
             self.info("No dependency constraints to relax.")
             return 0
 
-        if self.io.is_verbose():
-            self.line(f"Proposing updates to {len(updated_dependencies)} dependencies.")
+        self.line(f"Proposing updates to {updated_count} dependencies.")
 
         # Validate that the update is valid by running the installer
         if self.option("update") or self.option("check") or self.option("lock"):
             if self.io.is_verbose():
-                for old_constraint, dependency in updated_dependencies:
-                    self.info(
-                        f"Proposing update for <c1>{dependency.name}</> constraint from "
-                        f"<c2>{old_constraint}</> to <c2>{dependency.pretty_constraint}</>"
-                    )
+                for group in groups:
+                    for old_constraint, dependency in updated_dependencies[group]:
+                        self.info(
+                            f"Proposing update for <c1>{dependency.name}</> constraint from "
+                            f"<c2>{old_constraint}</> to <c2>{dependency.pretty_constraint}</>"
+                            f"{_pretty_group(group)}"
+                        )
 
             should_not_update = self.option("dry-run") or not (
                 self.option("update") or self.option("lock")
             )
             if should_not_update:
                 self.info("Checking new dependencies can be solved...")
             else:
@@ -150,16 +231,18 @@
                 return 1
 
             try:
                 status = run_installer_update(
                     poetry=self.poetry,
                     installer=self.installer,
                     lockfile_only=self.option("lock"),
-                    dependencies=(d for _, d in updated_dependencies),
-                    dependency_group_name=group,
+                    dependencies_by_group={
+                        group: (d for _, d in deps)
+                        for group, deps in updated_dependencies.items()
+                    },
                     poetry_config=poetry_config,
                     dry_run=should_not_update,
                     verbose=self.io.is_verbose(),
                     silent=(
                         # Do not display installer output by default, it's confusing
                         should_not_update
                         and not self.io.is_verbose()
@@ -176,27 +259,35 @@
                 self.info("Skipping check for valid versions.")
 
             status = 0
 
         # Cosmetic new line
         self.line("")
 
-        for old_constraint, dependency in updated_dependencies:
-            # Mutate the dependency config (and consequently the pyproject config)
-            name = dependency.name
-            if isinstance(dependency_config[name], dict):
-                dependency_config[name]["version"] = dependency.pretty_constraint
-            else:
-                dependency_config[name] = dependency.pretty_constraint
-
-            # Display the final updates since they can be buried by the installer update
-            self.info(
-                f"Updated <c1>{dependency.pretty_name}</> constraint from "
-                f"<c2>{old_constraint}</> to <c2>{dependency.pretty_constraint}</>"
+        for group in groups:
+            dependency_config = extract_dependency_config_for_group(
+                group, poetry_config
             )
+            if dependency_config is None:
+                continue
+
+            for old_constraint, dependency in updated_dependencies[group]:
+                # Mutate the dependency config (and consequently the pyproject config)
+                name = dependency.name
+                if isinstance(dependency_config[name], dict):
+                    dependency_config[name]["version"] = dependency.pretty_constraint
+                else:
+                    dependency_config[name] = dependency.pretty_constraint
+
+                # Display the final updates since they can be buried by the installer update
+                self.info(
+                    f"Updated <c1>{dependency.pretty_name}</> constraint from "
+                    f"<c2>{old_constraint}</> to <c2>{dependency.pretty_constraint}</>"
+                    f"{_pretty_group(group)}"
+                )
 
         if status == 0 and not self.option("dry-run"):
             assert isinstance(pyproject_config, TOMLDocument)
             self.poetry.file.write(pyproject_config)
             self.info("Updated config file with relaxed constraints.")
 
         elif status != 0:
@@ -204,7 +295,31 @@
                 "Aborted relax due to failure during dependency update.",
                 style="fg=red;options=bold",
             )
         else:
             self.info("Skipped update of config file due to dry-run flag.")
 
         return status
+
+    def _validate_group_options(self, group_options: Dict[str, Set[str]]) -> None:
+        """
+        Raises en error if it detects that a group is not part of pyproject.toml
+        """
+        if POETRY_VERSION >= Version("1.5.0"):
+            return super()._validate_group_options(group_options)
+
+        # Backport of the validation logic from Poetry 1.5.x
+
+        invalid_options = defaultdict(set)
+        for opt, groups in group_options.items():
+            for group in groups:
+                if not self.poetry.package.has_dependency_group(group):
+                    invalid_options[group].add(opt)
+        if invalid_options:
+            message_parts = []
+            for group in sorted(invalid_options):
+                opts = ", ".join(
+                    f"<fg=yellow;options=bold>--{opt}</>"
+                    for opt in sorted(invalid_options[group])
+                )
+                message_parts.append(f"{group} (via {opts})")
+            raise PoetryConsoleError(f"Group(s) not found: {', '.join(message_parts)}")
```

### Comparing `poetry-relax-0.1.2/setup.py` & `poetry_relax-1.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,468 +1,483 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 655f 6469  etup..package_di
-00000040: 7220 3d20 5c0a 7b27 273a 2027 7372 6327  r = \.{'': 'src'
-00000050: 7d0a 0a70 6163 6b61 6765 7320 3d20 5c0a  }..packages = \.
-00000060: 5b27 706f 6574 7279 5f72 656c 6178 275d  ['poetry_relax']
-00000070: 0a0a 7061 636b 6167 655f 6461 7461 203d  ..package_data =
-00000080: 205c 0a7b 2727 3a20 5b27 2a27 5d7d 0a0a   \.{'': ['*']}..
-00000090: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-000000a0: 203d 205c 0a5b 2770 6f65 7472 793e 3d31   = \.['poetry>=1
-000000b0: 2e32 275d 0a0a 656e 7472 795f 706f 696e  .2']..entry_poin
-000000c0: 7473 203d 205c 0a7b 2770 6f65 7472 792e  ts = \.{'poetry.
-000000d0: 6170 706c 6963 6174 696f 6e2e 706c 7567  application.plug
-000000e0: 696e 273a 205b 2772 656c 6178 203d 2070  in': ['relax = p
-000000f0: 6f65 7472 795f 7265 6c61 783a 5265 6c61  oetry_relax:Rela
-00000100: 7850 6c75 6769 6e27 5d7d 0a0a 7365 7475  xPlugin']}..setu
-00000110: 705f 6b77 6172 6773 203d 207b 0a20 2020  p_kwargs = {.   
-00000120: 2027 6e61 6d65 273a 2027 706f 6574 7279   'name': 'poetry
-00000130: 2d72 656c 6178 272c 0a20 2020 2027 7665  -relax',.    've
-00000140: 7273 696f 6e27 3a20 2730 2e31 2e32 272c  rsion': '0.1.2',
-00000150: 0a20 2020 2027 6465 7363 7269 7074 696f  .    'descriptio
-00000160: 6e27 3a20 2750 6c75 6769 6e20 666f 7220  n': 'Plugin for 
-00000170: 506f 6574 7279 2074 6f20 7265 6c61 7820  Poetry to relax 
-00000180: 7570 7065 7220 7665 7273 696f 6e20 7069  upper version pi
-00000190: 6e73 272c 0a20 2020 2027 6c6f 6e67 5f64  ns',.    'long_d
-000001a0: 6573 6372 6970 7469 6f6e 273a 2022 2320  escription': "# 
-000001b0: 706f 6574 7279 2d72 656c 6178 5c6e 5c6e  poetry-relax\n\n
-000001c0: 4120 5b50 6f65 7472 795d 2868 7474 7073  A [Poetry](https
-000001d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7079  ://github.com/py
-000001e0: 7468 6f6e 2d70 6f65 7472 792f 706f 6574  thon-poetry/poet
-000001f0: 7279 2920 706c 7567 696e 2074 6f20 7265  ry) plugin to re
-00000200: 6c61 7820 6465 7065 6e64 656e 6379 2076  lax dependency v
-00000210: 6572 7369 6f6e 7320 7768 656e 2070 7562  ersions when pub
-00000220: 6c69 7368 696e 6720 6c69 6272 6172 6965  lishing librarie
-00000230: 732e 2052 656c 6178 2079 6f75 7220 7072  s. Relax your pr
-00000240: 6f6a 6563 7427 7320 6465 7065 6e64 656e  oject's dependen
-00000250: 6369 6573 2066 726f 6d20 6066 6f6f 6261  cies from `fooba
-00000260: 725e 322e 302e 3060 2074 6f20 6066 6f6f  r^2.0.0` to `foo
-00000270: 6261 723e 3d32 2e30 2e30 602e 5c6e 5c6e  bar>=2.0.0`.\n\n
-00000280: 4279 2064 6566 6175 6c74 2c20 506f 6574  By default, Poet
-00000290: 7279 2075 7365 7320 6361 7265 7420 636f  ry uses caret co
-000002a0: 6e73 7472 6169 6e74 7320 7768 6963 6820  nstraints which 
-000002b0: 776f 756c 6420 6c69 6d69 7420 6066 6f6f  would limit `foo
-000002c0: 6261 7260 2076 6572 7369 6f6e 7320 746f  bar` versions to
-000002d0: 2060 3c33 2e30 602e 5c6e 2a2a 706f 6574   `<3.0`.\n**poet
-000002e0: 7279 2d72 656c 6178 2a2a 2020 7265 6d6f  ry-relax**  remo
-000002f0: 7665 7320 7468 6573 6520 7570 7065 7220  ves these upper 
-00000300: 7665 7273 696f 6e20 626f 756e 6473 2c20  version bounds, 
-00000310: 616c 6c6f 7769 6e67 2064 6570 656e 6465  allowing depende
-00000320: 6e63 6965 7320 746f 2062 6520 7570 6772  ncies to be upgr
-00000330: 6164 6564 2e5c 6e5c 6e52 656d 6f76 696e  aded.\n\nRemovin
-00000340: 6720 7570 7065 7220 7665 7273 696f 6e20  g upper version 
-00000350: 626f 756e 6473 2069 7320 696d 706f 7274  bounds is import
-00000360: 616e 7420 7768 656e 2070 7562 6c69 7368  ant when publish
-00000370: 696e 6720 6c69 6272 6172 6965 732e 5c6e  ing libraries.\n
-00000380: 5768 656e 2073 6561 7263 6869 6e67 2066  When searching f
-00000390: 6f72 2076 6572 7369 6f6e 7320 6f66 2064  or versions of d
-000003a0: 6570 656e 6465 6e63 6965 7320 746f 2069  ependencies to i
-000003b0: 6e73 7461 6c6c 2c20 7468 6520 7265 736f  nstall, the reso
-000003c0: 6c76 6572 2028 652e 672e 2060 7069 7060  lver (e.g. `pip`
-000003d0: 2920 6d75 7374 2072 6573 7065 6374 2074  ) must respect t
-000003e0: 6865 2062 6f75 6e64 7320 796f 7572 206c  he bounds your l
-000003f0: 6962 7261 7279 2073 7065 6369 6669 6573  ibrary specifies
-00000400: 2e5c 6e57 6865 6e20 6120 6e65 7720 7665  .\nWhen a new ve
-00000410: 7273 696f 6e20 6f66 2074 6865 2064 6570  rsion of the dep
-00000420: 656e 6465 6e63 7920 6973 2072 656c 6561  endency is relea
-00000430: 7365 642c 2063 6f6e 7375 6d65 7273 206f  sed, consumers o
-00000440: 6620 796f 7572 206c 6962 7261 7279 205f  f your library _
-00000450: 6361 6e6e 6f74 5f20 696e 7374 616c 6c20  cannot_ install 
-00000460: 6974 2075 6e6c 6573 7320 6120 6e65 7720  it unless a new 
-00000470: 7665 7273 696f 6e20 6f66 2079 6f75 7220  version of your 
-00000480: 6c69 6272 6172 7920 6973 2061 6c73 6f20  library is also 
-00000490: 7265 6c65 6173 6564 2e5c 6e5c 6e49 7420  released.\n\nIt 
-000004a0: 6973 206e 6f74 2066 6561 7369 626c 6520  is not feasible 
-000004b0: 746f 2072 656c 6561 7365 2070 6174 6368  to release patch
-000004c0: 6573 2066 6f72 2065 7665 7279 2070 7265  es for every pre
-000004d0: 7669 6f75 7320 7665 7273 696f 6e20 6f66  vious version of
-000004e0: 206d 6f73 7420 6c69 6272 6172 6965 732c   most libraries,
-000004f0: 2077 6869 6368 2066 6f72 6365 7320 7573   which forces us
-00000500: 6572 7320 746f 2075 7365 2074 6865 206d  ers to use the m
-00000510: 6f73 7420 7265 6365 6e74 2076 6572 7369  ost recent versi
-00000520: 6f6e 206f 6620 7468 6520 6c69 6272 6172  on of the librar
-00000530: 7920 6f72 2062 6520 7374 7563 6b20 7769  y or be stuck wi
-00000540: 7468 6f75 7420 7468 6520 6e65 7720 7665  thout the new ve
-00000550: 7273 696f 6e20 6f66 2074 6865 2064 6570  rsion of the dep
-00000560: 656e 6465 6e63 792e 5c6e 5768 656e 206d  endency.\nWhen m
-00000570: 616e 7920 6c69 6272 6172 6965 7320 636f  any libraries co
-00000580: 6e74 6169 6e20 7570 7065 7220 7665 7273  ntain upper vers
-00000590: 696f 6e20 626f 756e 6473 2c20 7468 6520  ion bounds, the 
-000005a0: 6465 7065 6e64 656e 6369 6573 2063 616e  dependencies can
-000005b0: 2065 6173 696c 7920 6265 636f 6d65 205f   easily become _
-000005c0: 756e 736f 6c76 6162 6c65 5f20 e280 9420  unsolvable_ ... 
-000005d0: 7768 6572 6520 6c69 6272 6172 6965 7320  where libraries 
-000005e0: 6861 7665 2069 6e63 6f6d 7061 7469 626c  have incompatibl
-000005f0: 6520 6465 7065 6e64 656e 6379 2076 6572  e dependency ver
-00000600: 7369 6f6e 2072 6571 7569 7265 6d65 6e74  sion requirement
-00000610: 732e 5c6e 4279 2072 656d 6f76 696e 6720  s.\nBy removing 
-00000620: 7570 7065 7220 7665 7273 696f 6e20 626f  upper version bo
-00000630: 756e 6473 2066 726f 6d20 796f 7572 206c  unds from your l
-00000640: 6962 7261 7279 2c20 636f 6e74 726f 6c20  ibrary, control 
-00000650: 6973 2072 6574 7572 6e65 6420 746f 2074  is returned to t
-00000660: 6865 2075 7365 722e 5c6e 5c6e 506f 6574  he user.\n\nPoet
-00000670: 7279 2773 2064 6566 6175 6c74 2062 6568  ry's default beh
-00000680: 6176 696f 7220 6973 2074 6f20 696e 636c  avior is to incl
-00000690: 7564 6520 7570 7065 7220 7665 7273 696f  ude upper versio
-000006a0: 6e20 626f 756e 6473 2e20 4d61 6e79 2070  n bounds. Many p
-000006b0: 656f 706c 6520 6861 7665 2073 706f 6b65  eople have spoke
-000006c0: 6e20 7570 2061 6761 696e 7374 2074 6869  n up against thi
-000006d0: 7320 7374 796c 6520 6f66 2064 6570 656e  s style of depen
-000006e0: 6465 6e63 7920 6d61 6e61 6765 6d65 6e74  dency management
-000006f0: 2069 6e20 7468 6520 5079 7468 6f6e 2065   in the Python e
-00000700: 636f 7379 7374 656d 2c20 696e 636c 7564  cosystem, includ
-00000710: 696e 6720 6d65 6d62 6572 7320 6f66 2074  ing members of t
-00000720: 6865 2050 7974 686f 6e20 636f 7265 2064  he Python core d
-00000730: 6576 656c 6f70 6d65 6e74 2074 6561 6d2e  evelopment team.
-00000740: 2053 6565 205b 7468 6520 626f 7474 6f6d   See [the bottom
-00000750: 206f 6620 7468 6520 7265 6164 6d65 5d28   of the readme](
-00000760: 2372 6566 6572 656e 6365 7329 2066 6f72  #references) for
-00000770: 206c 696e 6b73 2061 6e64 2061 6464 6974   links and addit
-00000780: 696f 6e61 6c20 636f 6e74 6578 742e 5c6e  ional context.\n
-00000790: 5c6e 5369 6e63 6520 7468 6520 506f 6574  \nSince the Poet
-000007a0: 7279 2070 726f 6a65 6374 2077 696c 6c20  ry project will 
-000007b0: 6e6f 7420 616c 6c6f 7720 7468 6973 2062  not allow this b
-000007c0: 6568 6176 696f 7220 746f 2062 6520 636f  ehavior to be co
-000007d0: 6e66 6967 7572 6564 2c20 6d61 696e 7461  nfigured, mainta
-000007e0: 696e 6572 7320 6861 7665 2072 6573 6f72  iners have resor
-000007f0: 7465 6420 746f 206d 616e 7561 6c20 6564  ted to manual ed
-00000800: 6974 696e 6720 6f66 2064 6570 656e 6465  iting of depende
-00000810: 6e63 7920 636f 6e73 7472 6169 6e74 7320  ncy constraints 
-00000820: 6166 7465 7220 6164 6469 6e67 2e20 2a2a  after adding. **
-00000830: 706f 6574 7279 2d72 656c 6178 2a2a 2061  poetry-relax** a
-00000840: 696d 7320 746f 2061 7574 6f6d 6174 6520  ims to automate 
-00000850: 616e 6420 7369 6d70 6c69 6679 2074 6869  and simplify thi
-00000860: 7320 7072 6f63 6573 732e 5c6e 5c6e 2a2a  s process.\n\n**
-00000870: 706f 6574 7279 2d72 656c 6178 2a2a 2070  poetry-relax** p
-00000880: 726f 7669 6465 733a 5c6e 2d20 4175 746f  rovides:\n- Auto
-00000890: 6d61 7465 6420 7265 6d6f 7661 6c20 6f66  mated removal of
-000008a0: 2075 7070 6572 2062 6f75 6e64 2063 6f6e   upper bound con
-000008b0: 7374 7261 696e 7473 2073 7065 6369 6669  straints specifi
-000008c0: 6564 2077 6974 6820 605e 605c 6e2d 2053  ed with `^`\n- S
-000008d0: 6166 6574 7920 6368 6563 6b20 6966 2070  afety check if p
-000008e0: 6163 6b61 6765 2072 6571 7569 7265 6d65  ackage requireme
-000008f0: 6e74 7320 6172 6520 7374 696c 6c20 736f  nts are still so
-00000900: 6c76 6162 6c65 2061 6674 6572 2072 656c  lvable after rel
-00000910: 6178 696e 6720 636f 6e73 7472 6169 6e74  axing constraint
-00000920: 735c 6e2d 2055 7067 7261 6465 206f 6620  s\n- Upgrade of 
-00000930: 6465 7065 6e64 656e 6369 6573 2061 6674  dependencies aft
-00000940: 6572 2072 656c 6178 696e 6720 636f 6e73  er relaxing cons
-00000950: 7472 6169 6e74 735c 6e2d 2055 7064 6174  traints\n- Updat
-00000960: 6520 6f66 2074 6865 206c 6f63 6b20 6669  e of the lock fi
-00000970: 6c65 2077 6974 686f 7574 2075 7067 7261  le without upgra
-00000980: 6469 6e67 2064 6570 656e 6465 6e63 6965  ding dependencie
-00000990: 735c 6e2d 204c 696d 6974 2064 6570 656e  s\n- Limit depen
-000009a0: 6465 6e63 7920 7265 6c61 7861 7469 6f6e  dency relaxation
-000009b0: 2074 6f20 7370 6563 6966 6963 2064 6570   to specific dep
-000009c0: 656e 6465 6e63 7920 6772 6f75 7073 5c6e  endency groups\n
-000009d0: 2d20 5265 7465 6e74 696f 6e20 6f66 2069  - Retention of i
-000009e0: 6e74 656e 7469 6f6e 616c 2075 7070 6572  ntentional upper
-000009f0: 2062 6f75 6e64 7320 696e 6469 6361 7469   bounds indicati
-00000a00: 6e67 2074 7275 6520 696e 636f 6d70 6174  ng true incompat
-00000a10: 6962 696c 6974 6965 735c 6e2d 2043 4c49  ibilities\n- CLI
-00000a20: 206d 6573 7361 6765 7320 6465 7369 676e   messages design
-00000a30: 6564 2074 6f20 6d61 7463 6820 506f 6574  ed to match Poet
-00000a40: 7279 2773 206f 7574 7075 745c 6e5c 6e23  ry's output\n\n#
-00000a50: 2320 496e 7374 616c 6c61 7469 6f6e 5c6e  # Installation\n
-00000a60: 5c6e 5468 6520 706c 7567 696e 206d 7573  \nThe plugin mus
-00000a70: 7420 6265 2069 6e73 7461 6c6c 6564 2069  t be installed i
-00000a80: 6e20 506f 6574 7279 2773 2065 6e76 6972  n Poetry's envir
-00000a90: 6f6e 6d65 6e74 2e20 5468 6973 2072 6571  onment. This req
-00000aa0: 7569 7265 7320 7573 6520 6f66 2074 6865  uires use of the
-00000ab0: 2020 6073 656c 6660 2073 7562 636f 6d6d    `self` subcomm
-00000ac0: 616e 642e 5c6e 5c6e 6060 6062 6173 685c  and.\n\n```bash\
-00000ad0: 6e24 2070 6f65 7472 7920 7365 6c66 2061  n$ poetry self a
-00000ae0: 6464 2070 6f65 7472 792d 7265 6c61 785c  dd poetry-relax\
-00000af0: 6e60 6060 5c6e 5c6e 2323 2055 7361 6765  n```\n\n## Usage
-00000b00: 5c6e 5c6e 5265 6c61 7820 636f 6e73 7472  \n\nRelax constr
-00000b10: 6169 6e74 7320 666f 7220 7768 6963 6820  aints for which 
-00000b20: 506f 6574 7279 2073 6574 2061 6e20 7570  Poetry set an up
-00000b30: 7065 7220 7665 7273 696f 6e3a 5c6e 5c6e  per version:\n\n
-00000b40: 6060 6062 6173 685c 6e24 2070 6f65 7472  ```bash\n$ poetr
-00000b50: 7920 7265 6c61 785c 6e60 6060 5c6e 5c6e  y relax\n```\n\n
-00000b60: 5265 6c61 7820 636f 6e73 7472 6169 6e74  Relax constraint
-00000b70: 7320 616e 6420 6368 6563 6b20 7468 6174  s and check that
-00000b80: 2074 6865 7920 6172 6520 7265 736f 6c76   they are resolv
-00000b90: 6162 6c65 2077 6974 686f 7574 2070 6572  able without per
-00000ba0: 666f 726d 696e 6720 7570 6772 6164 6573  forming upgrades
-00000bb0: 3a5c 6e5c 6e60 6060 6261 7368 5c6e 2420  :\n\n```bash\n$ 
-00000bc0: 706f 6574 7279 2072 656c 6178 202d 2d63  poetry relax --c
-00000bd0: 6865 636b 5c6e 6060 605c 6e5c 6e52 656c  heck\n```\n\nRel
-00000be0: 6178 2063 6f6e 7374 7261 696e 7473 2061  ax constraints a
-00000bf0: 6e64 2075 7067 7261 6465 2070 6163 6b61  nd upgrade packa
-00000c00: 6765 733a 5c6e 5c6e 6060 6062 6173 685c  ges:\n\n```bash\
-00000c10: 6e24 2070 6f65 7472 7920 7265 6c61 7820  n$ poetry relax 
-00000c20: 2d2d 7570 6461 7465 5c6e 6060 605c 6e5c  --update\n```\n\
-00000c30: 6e52 656c 6178 2063 6f6e 7374 7261 696e  nRelax constrain
-00000c40: 7473 2061 6e64 2075 7064 6174 6520 7468  ts and update th
-00000c50: 6520 6c6f 636b 2066 696c 6520 7769 7468  e lock file with
-00000c60: 6f75 7420 7570 6772 6164 696e 6720 7061  out upgrading pa
-00000c70: 636b 6167 6573 3a5c 6e5c 6e60 6060 6261  ckages:\n\n```ba
-00000c80: 7368 5c6e 2420 706f 6574 7279 2072 656c  sh\n$ poetry rel
-00000c90: 6178 202d 2d6c 6f63 6b5c 6e60 6060 5c6e  ax --lock\n```\n
-00000ca0: 5c6e 5072 6576 6965 7720 7468 6520 6368  \nPreview the ch
-00000cb0: 616e 6765 7320 6070 6f65 7472 7920 7265  anges `poetry re
-00000cc0: 6c61 7860 2077 6f75 6c64 206d 616b 6520  lax` would make 
-00000cd0: 7769 7468 6f75 7420 6d6f 6469 6679 696e  without modifyin
-00000ce0: 6720 7468 6520 7072 6f6a 6563 743a 5c6e  g the project:\n
-00000cf0: 5c6e 6060 6062 6173 685c 6e24 2070 6f65  \n```bash\n$ poe
-00000d00: 7472 7920 7265 6c61 7820 2d2d 6472 792d  try relax --dry-
-00000d10: 7275 6e5c 6e60 6060 5c6e 5c6e 2323 2045  run\n```\n\n## E
-00000d20: 7861 6d70 6c65 735c 6e5c 6e54 6865 2062  xamples\n\nThe b
-00000d30: 6568 6176 696f 7220 6f66 2050 6f65 7472  ehavior of Poetr
-00000d40: 7920 6973 2071 7569 7465 2072 6561 736f  y is quite reaso
-00000d50: 6e61 626c 6520 666f 7220 6c6f 6361 6c20  nable for local 
-00000d60: 6465 7665 6c6f 706d 656e 7421 2060 706f  development! `po
-00000d70: 6574 7279 2072 656c 6178 6020 6973 206d  etry relax` is m
-00000d80: 6f73 7420 7573 6566 756c 2077 6865 6e20  ost useful when 
-00000d90: 7573 6564 2069 6e20 4349 2f43 4420 7069  used in CI/CD pi
-00000da0: 7065 6c69 6e65 732e 5c6e 5c6e 2323 2320  pelines.\n\n### 
-00000db0: 5265 6c61 7869 6e67 2072 6571 7569 7265  Relaxing require
-00000dc0: 6d65 6e74 7320 6265 666f 7265 2070 7562  ments before pub
-00000dd0: 6c69 7368 696e 675c 6e5c 6e52 756e 2060  lishing\n\nRun `
-00000de0: 706f 6574 7279 2072 656c 6178 6020 6265  poetry relax` be
-00000df0: 666f 7265 2062 7569 6c64 696e 6720 616e  fore building an
-00000e00: 6420 7075 626c 6973 6869 6e67 2061 2070  d publishing a p
-00000e10: 6163 6b61 6765 2e5c 6e5c 6e53 6565 2069  ackage.\n\nSee i
-00000e20: 7420 6174 2077 6f72 6b20 696e 205b 7468  t at work in [th
-00000e30: 6520 7265 6c65 6173 6520 776f 726b 666c  e release workfl
-00000e40: 6f77 2066 6f72 2074 6869 7320 7072 6f6a  ow for this proj
-00000e50: 6563 745d 2868 7474 7073 3a2f 2f67 6974  ect](https://git
-00000e60: 6875 622e 636f 6d2f 6d61 646b 696e 737a  hub.com/madkinsz
-00000e70: 2f70 6f65 7472 792d 7265 6c61 782f 626c  /poetry-relax/bl
-00000e80: 6f62 2f6d 6169 6e2f 2e67 6974 6875 622f  ob/main/.github/
-00000e90: 776f 726b 666c 6f77 732f 7265 6c65 6173  workflows/releas
-00000ea0: 652e 7961 6d6c 292e 5c6e 5c6e 5c6e 2323  e.yaml).\n\n\n##
-00000eb0: 2320 5265 6c61 7869 6e67 2072 6571 7569  # Relaxing requi
-00000ec0: 7265 6d65 6e74 7320 666f 7220 7465 7374  rements for test
-00000ed0: 696e 675c 6e5c 6e52 756e 2060 706f 6574  ing\n\nRun `poet
-00000ee0: 7279 2072 656c 6178 202d 2d75 7064 6174  ry relax --updat
-00000ef0: 6560 2062 6566 6f72 6520 7465 7374 7320  e` before tests 
-00000f00: 746f 2074 6573 7420 6167 6169 6e73 7420  to test against 
-00000f10: 7468 6520 6e65 7765 7374 2070 6f73 7369  the newest possi
-00000f20: 626c 6520 7665 7273 696f 6e73 206f 6620  ble versions of 
-00000f30: 7061 636b 6167 6573 2e5c 6e5c 6e53 6565  packages.\n\nSee
-00000f40: 2069 7420 6174 2077 6f72 6b20 696e 205b   it at work in [
-00000f50: 7468 6520 7465 7374 2077 6f72 6b66 6c6f  the test workflo
-00000f60: 7720 666f 7220 7468 6973 2070 726f 6a65  w for this proje
-00000f70: 6374 5d28 6874 7470 733a 2f2f 6769 7468  ct](https://gith
-00000f80: 7562 2e63 6f6d 2f6d 6164 6b69 6e73 7a2f  ub.com/madkinsz/
-00000f90: 706f 6574 7279 2d72 656c 6178 2f62 6c6f  poetry-relax/blo
-00000fa0: 622f 6d61 696e 2f2e 6769 7468 7562 2f77  b/main/.github/w
-00000fb0: 6f72 6b66 6c6f 7773 2f74 6573 742e 7961  orkflows/test.ya
-00000fc0: 6d6c 292e 5c6e 5c6e 2323 2046 7265 7175  ml).\n\n## Frequ
-00000fd0: 656e 746c 7920 6173 6b65 6420 7175 6573  ently asked ques
-00000fe0: 7469 6f6e 735c 6e5c 6e3e 2043 616e 2074  tions\n\n> Can t
-00000ff0: 6869 7320 706c 7567 696e 2063 6861 6e67  his plugin chang
-00001000: 6520 7468 6520 6265 6861 7669 6f72 206f  e the behavior o
-00001010: 6620 6070 6f65 7472 7920 6164 6460 2074  f `poetry add` t
-00001020: 6f20 7265 6c61 7820 636f 6e73 7472 6169  o relax constrai
-00001030: 6e74 733f 5c6e 5c6e 4e6f 7420 6174 2074  nts?\n\nNot at t
-00001040: 6869 7320 7469 6d65 2e20 5468 6520 506f  his time. The Po
-00001050: 6574 7279 2070 726f 6a65 6374 2073 7461  etry project sta
-00001060: 7465 7320 7468 6174 2070 6c75 6769 6e73  tes that plugins
-00001070: 206d 7573 7420 6e6f 7420 616c 7465 7220   must not alter 
-00001080: 7468 6520 6265 6861 7669 6f72 206f 6620  the behavior of 
-00001090: 636f 7265 2050 6f65 7472 7920 636f 6d6d  core Poetry comm
-000010a0: 616e 6473 2e20 4966 2074 6869 7320 6265  ands. If this be
-000010b0: 6861 7669 6f72 2077 6f75 6c64 2062 6520  havior would be 
-000010c0: 7573 6566 756c 2066 6f72 2079 6f75 2c20  useful for you, 
-000010d0: 706c 6561 7365 2063 6869 6d65 2069 6e20  please chime in 
-000010e0: 5b6f 6e20 7468 6520 7472 6163 6b69 6e67  [on the tracking
-000010f0: 2069 7373 7565 5d28 6874 7470 733a 2f2f   issue](https://
-00001100: 6769 7468 7562 2e63 6f6d 2f6d 6164 6b69  github.com/madki
-00001110: 6e73 7a2f 706f 6574 7279 2d72 656c 6178  nsz/poetry-relax
-00001120: 2f69 7373 7565 732f 3529 2e5c 6e5c 6e3e  /issues/5).\n\n>
-00001130: 2044 6f65 7320 7468 6973 2070 6c75 6769   Does this plugi
-00001140: 6e20 7265 6d6f 7665 2075 7070 6572 2063  n remove upper c
-00001150: 6f6e 7374 7261 696e 7473 2049 2776 6520  onstraints I've 
-00001160: 6164 6465 643f 5c6e 5c6e 5468 6973 2070  added?\n\nThis p
-00001170: 6c75 6769 6e20 7769 6c6c 206f 6e6c 7920  lugin will only 
-00001180: 7265 6c61 7820 636f 6e73 7472 6169 6e74  relax constraint
-00001190: 7320 7370 6563 6966 6965 6420 7769 7468  s specified with
-000011a0: 2061 2063 6172 6574 2028 605e 6029 2e20   a caret (`^`). 
-000011b0: 5570 7065 7220 636f 6e73 7472 6169 6e74  Upper constraint
-000011c0: 7320 6164 6465 6420 7769 7468 2060 3c60  s added with `<`
-000011d0: 2061 6e64 2060 3c3d 6020 7769 6c6c 206e   and `<=` will n
-000011e0: 6f74 2062 6520 6368 616e 6765 642e 5c6e  ot be changed.\n
-000011f0: 5c6e 3e20 4973 2074 6869 7320 706c 7567  \n> Is this plug
-00001200: 696e 2073 7461 626c 653f 5c6e 5c6e 5468  in stable?\n\nTh
-00001210: 6973 2070 6c75 6769 6e20 6973 2074 6573  is plugin is tes
-00001220: 7465 6420 6167 6169 6e73 7420 6d75 6c74  ted against mult
-00001230: 6970 6c65 2076 6572 7369 6f6e 7320 6f66  iple versions of
-00001240: 2050 6f65 7472 7920 616e 6420 6861 7320   Poetry and has 
-00001250: 616e 2069 6e74 6567 7261 7469 6f6e 2066  an integration f
-00001260: 6f63 7573 6564 2074 6573 7420 7375 6974  ocused test suit
-00001270: 652e 2049 7420 6973 2073 6166 6520 746f  e. It is safe to
-00001280: 2075 7365 2074 6869 7320 696e 2070 726f   use this in pro
-00001290: 6475 6374 696f 6e2c 2074 686f 7567 6820  duction, though 
-000012a0: 6974 2069 7320 7265 636f 6d6d 656e 6420  it is recommend 
-000012b0: 746f 2070 696e 2076 6572 7369 6f6e 732e  to pin versions.
-000012c0: 2042 7265 616b 696e 6720 6368 616e 6765   Breaking change
-000012d0: 7320 7769 6c6c 2062 6520 6176 6f69 6465  s will be avoide
-000012e0: 6420 756e 6c65 7373 2069 6e66 6561 7369  d unless infeasi
-000012f0: 626c 6520 6475 6520 746f 2075 7073 7472  ble due to upstr
-00001300: 6561 6d20 6368 616e 6765 7320 696e 2050  eam changes in P
-00001310: 6f65 7472 792e 5c6e 5c6e 3e20 5769 6c6c  oetry.\n\n> Will
-00001320: 2074 6869 7320 706c 7567 696e 2064 726f   this plugin dro
-00001330: 7020 7468 6520 7570 7065 7220 626f 756e  p the upper boun
-00001340: 6420 6f6e 2050 7974 686f 6e20 6974 7365  d on Python itse
-00001350: 6c66 3f5c 6e5c 6e42 656c 6965 7665 2069  lf?\n\nBelieve i
-00001360: 7420 6f72 206e 6f74 2c20 7468 6973 2069  t or not, this i
-00001370: 7320 616e 2065 7665 6e20 6d6f 7265 2063  s an even more c
-00001380: 6f6e 7465 6e74 696f 7573 2073 7562 7365  ontentious subse
-00001390: 7420 6f66 2074 6869 7320 6973 7375 6520  t of this issue 
-000013a0: 6173 2050 6f65 7472 7920 7769 6c6c 206e  as Poetry will n
-000013b0: 6f74 2061 6c6c 6f77 2070 6163 6b61 6765  ot allow package
-000013c0: 7320 7769 7468 206e 6f20 7570 7065 7220  s with no upper 
-000013d0: 626f 756e 6420 6f6e 2050 7974 686f 6e20  bound on Python 
-000013e0: 746f 2065 7869 7374 2061 6c6f 6e67 7369  to exist alongsi
-000013f0: 6465 2074 686f 7365 2074 6861 7420 696e  de those that in
-00001400: 636c 7564 6520 6f6e 652e 2054 6869 7320  clude one. This 
-00001410: 6261 7369 6361 6c6c 7920 6d65 616e 7320  basically means 
-00001420: 7468 6174 2077 6520 6361 6e6e 6f74 2072  that we cannot r
-00001430: 656c 6178 2074 6869 7320 7265 7175 6972  elax this requir
-00001440: 656d 656e 7420 7769 7468 6f75 7420 6272  ement without br
-00001450: 6561 6b69 6e67 2074 6865 2076 6173 7420  eaking the vast 
-00001460: 6d61 6a6f 7269 7479 206f 6620 7573 652d  majority of use-
-00001470: 6361 7365 732e 2046 6f72 2074 6869 7320  cases. For this 
-00001480: 7265 6173 6f6e 2c20 7765 2063 616e 6e6f  reason, we canno
-00001490: 7420 7265 6c61 7820 6070 7974 686f 6e5e  t relax `python^
-000014a0: 3360 2061 7420 7468 6973 2074 696d 652e  3` at this time.
-000014b0: 2053 6565 205b 7468 6520 706f 7374 206f   See [the post o
-000014c0: 6e20 7468 6520 506f 6574 7279 2064 6973  n the Poetry dis
-000014d0: 6375 7373 696f 6e20 626f 6172 645d 2868  cussion board](h
-000014e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000014f0: 6d2f 7079 7468 6f6e 2d70 6f65 7472 792f  m/python-poetry/
-00001500: 706f 6574 7279 2f64 6973 6375 7373 696f  poetry/discussio
-00001510: 6e73 2f33 3735 3723 6469 7363 7573 7369  ns/3757#discussi
-00001520: 6f6e 636f 6d6d 656e 742d 3433 3533 3435  oncomment-435345
-00001530: 2920 666f 7220 6d6f 7265 2064 6574 6169  ) for more detai
-00001540: 6c73 2e5c 6e5c 6e23 2320 436f 6e74 7269  ls.\n\n## Contri
-00001550: 6275 7469 6e67 5c6e 5c6e 5468 6973 2070  buting\n\nThis p
-00001560: 726f 6a65 6374 2069 7320 6d61 6e61 6765  roject is manage
-00001570: 6420 7769 7468 2050 6f65 7472 792e 2048  d with Poetry. H
-00001580: 6572 6520 6172 6520 7468 6520 6261 7369  ere are the basi
-00001590: 6373 2066 6f72 2067 6574 7469 6e67 2073  cs for getting s
-000015a0: 7461 7274 6564 2e5c 6e5c 6e43 6c6f 6e65  tarted.\n\nClone
-000015b0: 2074 6865 2072 6570 6f73 6974 6f72 793a   the repository:
-000015c0: 5c6e 6060 6062 6173 685c 6e24 2067 6974  \n```bash\n$ git
-000015d0: 2063 6c6f 6e65 2068 7474 7073 3a2f 2f67   clone https://g
-000015e0: 6974 6875 622e 636f 6d2f 6d61 646b 696e  ithub.com/madkin
-000015f0: 737a 2f70 6f65 7472 792d 7265 6c61 782e  sz/poetry-relax.
-00001600: 6769 745c 6e24 2063 6420 706f 6574 7279  git\n$ cd poetry
-00001610: 2d72 656c 6178 5c6e 6060 605c 6e5c 6e49  -relax\n```\n\nI
-00001620: 6e73 7461 6c6c 2070 6163 6b61 6765 733a  nstall packages:
-00001630: 5c6e 6060 6062 6173 685c 6e24 2070 6f65  \n```bash\n$ poe
-00001640: 7472 7920 696e 7374 616c 6c5c 6e60 6060  try install\n```
-00001650: 5c6e 5c6e 5275 6e20 7468 6520 7465 7374  \n\nRun the test
-00001660: 2073 7569 7465 3a5c 6e60 6060 6261 7368   suite:\n```bash
-00001670: 5c6e 2420 7079 7465 7374 2074 6573 7473  \n$ pytest tests
-00001680: 5c6e 6060 605c 6e5c 6e52 756e 206c 696e  \n```\n\nRun lin
-00001690: 7465 7273 2062 6566 6f72 6520 6f70 656e  ters before open
-000016a0: 696e 6720 7075 6c6c 2072 6571 7565 7374  ing pull request
-000016b0: 733a 5c6e 6060 6062 6173 685c 6e24 202e  s:\n```bash\n$ .
-000016c0: 2f62 696e 2f6c 696e 7420 6368 6563 6b20  /bin/lint check 
-000016d0: 2e5c 6e24 202e 2f62 696e 2f6c 696e 7420  .\n$ ./bin/lint 
-000016e0: 6669 7820 2e5c 6e60 6060 5c6e 5c6e 2323  fix .\n```\n\n##
-000016f0: 2052 6566 6572 656e 6365 735c 6e5c 6e54   References\n\nT
-00001700: 6865 7265 2773 2061 206c 6f74 2074 6f20  here's a lot to 
-00001710: 7265 6164 206f 6e20 7468 6973 2074 6f70  read on this top
-00001720: 6963 2120 4974 2773 2063 6f6e 7465 6e74  ic! It's content
-00001730: 696f 7573 2061 6e64 2063 6175 7369 6e67  ious and causing
-00001740: 2061 206c 6f74 206f 6620 7072 6f62 6c65   a lot of proble
-00001750: 6d73 2066 6f72 206d 6169 6e74 6169 6e65  ms for maintaine
-00001760: 7273 2061 6e64 2075 7365 7273 2e5c 6e5c  rs and users.\n\
-00001770: 6e54 6865 2066 6f6c 6c6f 7769 6e67 2062  nThe following b
-00001780: 6c6f 6720 706f 7374 7320 6279 2048 656e  log posts by Hen
-00001790: 7279 2053 6368 7265 696e 6572 2061 7265  ry Schreiner are
-000017a0: 2071 7569 7465 2063 6f6d 7072 6568 656e   quite comprehen
-000017b0: 7369 7665 3a5c 6e2d 205b 5368 6f75 6c64  sive:\n- [Should
-000017c0: 2059 6f75 2055 7365 2055 7070 6572 2042   You Use Upper B
-000017d0: 6f75 6e64 2056 6572 7369 6f6e 2043 6f6e  ound Version Con
-000017e0: 7374 7261 696e 7473 3f5d 2868 7474 7073  straints?](https
-000017f0: 3a2f 2f69 7363 696e 756d 7079 2e64 6576  ://iscinumpy.dev
-00001800: 2f70 6f73 742f 626f 756e 642d 7665 7273  /post/bound-vers
-00001810: 696f 6e2d 636f 6e73 7472 6169 6e74 732f  ion-constraints/
-00001820: 295c 6e2d 205b 506f 6574 7279 2056 6572  )\n- [Poetry Ver
-00001830: 7369 6f6e 735d 2868 7474 7073 3a2f 2f69  sions](https://i
-00001840: 7363 696e 756d 7079 2e64 6576 2f70 6f73  scinumpy.dev/pos
-00001850: 742f 706f 6574 7279 2d76 6572 7369 6f6e  t/poetry-version
-00001860: 732f 295c 6e5c 6e43 6f6e 7465 6e74 2066  s/)\n\nContent f
-00001870: 726f 6d20 736f 6d65 206d 656d 6265 7273  rom some members
-00001880: 206f 6620 7468 6520 5079 7468 6f6e 2063   of the Python c
-00001890: 6f72 6520 6465 7665 6c6f 7065 7220 7465  ore developer te
-000018a0: 616d 3a5c 6e2d 205b 5365 6d61 6e74 6963  am:\n- [Semantic
-000018b0: 2056 6572 7369 6f6e 696e 6720 5769 6c6c   Versioning Will
-000018c0: 204e 6f74 2053 6176 6520 596f 755d 2868   Not Save You](h
-000018d0: 7474 7073 3a2f 2f68 796e 656b 2e6d 652f  ttps://hynek.me/
-000018e0: 6172 7469 636c 6573 2f73 656d 7665 722d  articles/semver-
-000018f0: 7769 6c6c 2d6e 6f74 2d73 6176 652d 796f  will-not-save-yo
-00001900: 752f 295c 6e2d 205b 5768 7920 4920 646f  u/)\n- [Why I do
-00001910: 6e27 7420 6c69 6b65 2053 656d 5665 7220  n't like SemVer 
-00001920: 616e 796d 6f72 655d 2868 7474 7073 3a2f  anymore](https:/
-00001930: 2f73 6e61 726b 792e 6361 2f77 6879 2d69  /snarky.ca/why-i
-00001940: 2d64 6f6e 742d 6c69 6b65 2d73 656d 7665  -dont-like-semve
-00001950: 722f 295c 6e2d 205b 5665 7273 696f 6e20  r/)\n- [Version 
-00001960: 6e75 6d62 6572 733a 2068 6f77 2074 6f20  numbers: how to 
-00001970: 7573 6520 7468 656d 3f5d 2868 7474 7073  use them?](https
-00001980: 3a2f 2f62 6572 6e61 742e 7465 6368 2f70  ://bernat.tech/p
-00001990: 6f73 7473 2f76 6572 7369 6f6e 2d6e 756d  osts/version-num
-000019a0: 6265 7273 2f29 5c6e 2d20 5b56 6572 7369  bers/)\n- [Versi
-000019b0: 6f6e 696e 6720 536f 6674 7761 7265 5d28  oning Software](
-000019c0: 6874 7470 733a 2f2f 6361 7265 6d61 642e  https://caremad.
-000019d0: 696f 2f70 6f73 7473 2f32 3031 362f 3032  io/posts/2016/02
-000019e0: 2f76 6572 7369 6f6e 696e 672d 736f 6674  /versioning-soft
-000019f0: 7761 7265 2f29 5c6e 5c6e 4469 7363 7573  ware/)\n\nDiscus
-00001a00: 7369 6f6e 2061 6e64 2069 7373 7565 7320  sion and issues 
-00001a10: 696e 2074 6865 2050 6f65 7472 7920 7072  in the Poetry pr
-00001a20: 6f6a 6563 743a 5c6e 2d20 5b50 6c65 6173  oject:\n- [Pleas
-00001a30: 6520 7374 6f70 2070 696e 6e69 6e67 2074  e stop pinning t
-00001a40: 6f20 6d61 6a6f 7220 7665 7273 696f 6e73  o major versions
-00001a50: 2062 7920 6465 6661 756c 742c 2065 7370   by default, esp
-00001a60: 6563 6961 6c6c 7920 666f 7220 5079 7468  ecially for Pyth
-00001a70: 6f6e 2069 7473 656c 665d 2868 7474 7073  on itself](https
-00001a80: 3a2f 2f67 6974 6875 622e 636f 6d2f 7079  ://github.com/py
-00001a90: 7468 6f6e 2d70 6f65 7472 792f 706f 6574  thon-poetry/poet
-00001aa0: 7279 2f69 7373 7565 732f 3337 3437 295c  ry/issues/3747)\
-00001ab0: 6e2d 205b 4368 616e 6765 2064 6566 6175  n- [Change defau
-00001ac0: 6c74 2064 6570 656e 6465 6e63 7920 636f  lt dependency co
-00001ad0: 6e73 7472 6169 6e74 2066 726f 6d20 5e20  nstraint from ^ 
-00001ae0: 746f 203e 3d5d 2868 7474 7073 3a2f 2f67  to >=](https://g
-00001af0: 6974 6875 622e 636f 6d2f 7079 7468 6f6e  ithub.com/python
-00001b00: 2d70 6f65 7472 792f 706f 6574 7279 2f69  -poetry/poetry/i
-00001b10: 7373 7565 732f 3334 3237 295c 6e2d 205b  ssues/3427)\n- [
-00001b20: 4465 7665 6c6f 7065 7273 2073 686f 756c  Developers shoul
-00001b30: 6420 6265 2061 626c 6520 746f 2074 7572  d be able to tur
-00001b40: 6e20 6f66 6620 6465 7065 6e64 656e 6379  n off dependency
-00001b50: 2075 7070 6572 2d62 6f75 6e64 2063 616c   upper-bound cal
-00001b60: 6375 6c61 7469 6f6e 735d 2868 7474 7073  culations](https
-00001b70: 3a2f 2f67 6974 6875 622e 636f 6d2f 7079  ://github.com/py
-00001b80: 7468 6f6e 2d70 6f65 7472 792f 706f 6574  thon-poetry/poet
-00001b90: 7279 2f69 7373 7565 732f 3237 3331 295c  ry/issues/2731)\
-00001ba0: 6e22 2c0a 2020 2020 2761 7574 686f 7227  n",.    'author'
-00001bb0: 3a20 275a 616e 6965 272c 0a20 2020 2027  : 'Zanie',.    '
-00001bc0: 6175 7468 6f72 5f65 6d61 696c 273a 2027  author_email': '
-00001bd0: 636f 6e74 6163 7440 7a61 6e69 652e 6465  contact@zanie.de
-00001be0: 7627 2c0a 2020 2020 276d 6169 6e74 6169  v',.    'maintai
-00001bf0: 6e65 7227 3a20 274e 6f6e 6527 2c0a 2020  ner': 'None',.  
-00001c00: 2020 276d 6169 6e74 6169 6e65 725f 656d    'maintainer_em
-00001c10: 6169 6c27 3a20 274e 6f6e 6527 2c0a 2020  ail': 'None',.  
-00001c20: 2020 2775 726c 273a 2027 6874 7470 733a    'url': 'https:
-00001c30: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 6164  //github.com/mad
-00001c40: 6b69 6e73 7a2f 706f 6574 7279 2d72 656c  kinsz/poetry-rel
-00001c50: 6178 272c 0a20 2020 2027 7061 636b 6167  ax',.    'packag
-00001c60: 655f 6469 7227 3a20 7061 636b 6167 655f  e_dir': package_
-00001c70: 6469 722c 0a20 2020 2027 7061 636b 6167  dir,.    'packag
-00001c80: 6573 273a 2070 6163 6b61 6765 732c 0a20  es': packages,. 
-00001c90: 2020 2027 7061 636b 6167 655f 6461 7461     'package_data
-00001ca0: 273a 2070 6163 6b61 6765 5f64 6174 612c  ': package_data,
-00001cb0: 0a20 2020 2027 696e 7374 616c 6c5f 7265  .    'install_re
-00001cc0: 7175 6972 6573 273a 2069 6e73 7461 6c6c  quires': install
-00001cd0: 5f72 6571 7569 7265 732c 0a20 2020 2027  _requires,.    '
-00001ce0: 656e 7472 795f 706f 696e 7473 273a 2065  entry_points': e
-00001cf0: 6e74 7279 5f70 6f69 6e74 732c 0a20 2020  ntry_points,.   
-00001d00: 2027 7079 7468 6f6e 5f72 6571 7569 7265   'python_require
-00001d10: 7327 3a20 273e 3d33 2e37 2c3c 342e 3027  s': '>=3.7,<4.0'
-00001d20: 2c0a 7d0a 0a0a 7365 7475 7028 2a2a 7365  ,.}...setup(**se
-00001d30: 7475 705f 6b77 6172 6773 290a            tup_kwargs).
+00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000010: 223e 0a20 2020 203c 6120 6872 6566 3d22  ">.    <a href="
+00000020: 6874 7470 733a 2f2f 7079 7069 2e70 7974  https://pypi.pyt
+00000030: 686f 6e2e 6f72 672f 7079 7069 2f70 6f65  hon.org/pypi/poe
+00000040: 7472 792d 7265 6c61 782f 2220 616c 743d  try-relax/" alt=
+00000050: 224c 6174 6573 7420 7665 7273 696f 6e22  "Latest version"
+00000060: 3e0a 2020 2020 2020 2020 3c69 6d67 2061  >.        <img a
+00000070: 6c74 3d22 4c61 7465 7374 2076 6572 7369  lt="Latest versi
+00000080: 6f6e 2220 7372 633d 2268 7474 7073 3a2f  on" src="https:/
+00000090: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000000a0: 7079 7069 2f76 2f70 6f65 7472 792d 7265  pypi/v/poetry-re
+000000b0: 6c61 783f 7374 796c 653d 666c 6174 2d73  lax?style=flat-s
+000000c0: 7175 6172 6522 3e0a 2020 2020 3c2f 613e  quare">.    </a>
+000000d0: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+000000e0: 7470 733a 2f2f 6465 7667 7569 6465 2e70  tps://devguide.p
+000000f0: 7974 686f 6e2e 6f72 672f 7665 7273 696f  ython.org/versio
+00000100: 6e73 2f22 2061 6c74 3d22 5375 7070 6f72  ns/" alt="Suppor
+00000110: 7465 6420 5079 7468 6f6e 2076 6572 7369  ted Python versi
+00000120: 6f6e 7322 3e0a 2020 2020 2020 2020 3c69  ons">.        <i
+00000130: 6d67 2061 6c74 3d22 5375 7070 6f72 7465  mg alt="Supporte
+00000140: 6420 5079 7468 6f6e 2076 6572 7369 6f6e  d Python version
+00000150: 7322 2073 7263 3d22 6874 7470 733a 2f2f  s" src="https://
+00000160: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000170: 7970 692f 7079 7665 7273 696f 6e73 2f70  ypi/pyversions/p
+00000180: 6f65 7472 792d 7265 6c61 783f 7374 796c  oetry-relax?styl
+00000190: 653d 666c 6174 2d73 7175 6172 6522 3e0a  e=flat-square">.
+000001a0: 2020 2020 3c2f 613e 0a20 2020 203c 6120      </a>.    <a 
+000001b0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+000001c0: 7468 7562 2e63 6f6d 2f6d 6164 6b69 6e73  thub.com/madkins
+000001d0: 7a2f 706f 6574 7279 2d72 656c 6178 2f61  z/poetry-relax/a
+000001e0: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+000001f0: 2f74 6573 742e 7961 6d6c 3f71 7565 7279  /test.yaml?query
+00000200: 3d62 7261 6e63 6825 3341 6d61 696e 2220  =branch%3Amain" 
+00000210: 616c 743d 2254 6573 7420 7374 6174 7573  alt="Test status
+00000220: 223e 0a20 2020 2020 2020 203c 696d 6720  ">.        <img 
+00000230: 616c 743d 2254 6573 7420 7374 6174 7573  alt="Test status
+00000240: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
+00000250: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
+00000260: 7468 7562 2f61 6374 696f 6e73 2f77 6f72  thub/actions/wor
+00000270: 6b66 6c6f 772f 7374 6174 7573 2f6d 6164  kflow/status/mad
+00000280: 6b69 6e73 7a2f 706f 6574 7279 2d72 656c  kinsz/poetry-rel
+00000290: 6178 2f74 6573 742e 7961 6d6c 3f6c 6162  ax/test.yaml?lab
+000002a0: 656c 3d74 6573 7426 7374 796c 653d 666c  el=test&style=fl
+000002b0: 6174 2d73 7175 6172 6522 3e0a 2020 2020  at-square">.    
+000002c0: 3c2f 613e 0a20 2020 203c 6120 6872 6566  </a>.    <a href
+000002d0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+000002e0: 2e63 6f6d 2f6d 6164 6b69 6e73 7a2f 706f  .com/madkinsz/po
+000002f0: 6574 7279 2d72 656c 6178 2f61 6374 696f  etry-relax/actio
+00000300: 6e73 2f77 6f72 6b66 6c6f 7773 2f62 7569  ns/workflows/bui
+00000310: 6c64 2e79 616d 6c3f 7175 6572 793d 6272  ld.yaml?query=br
+00000320: 616e 6368 2533 416d 6169 6e22 2061 6c74  anch%3Amain" alt
+00000330: 3d22 4275 696c 6420 7374 6174 7573 223e  ="Build status">
+00000340: 0a20 2020 2020 2020 203c 696d 6720 616c  .        <img al
+00000350: 743d 2242 7569 6c64 2073 7461 7475 7322  t="Build status"
+00000360: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00000370: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+00000380: 6875 622f 6163 7469 6f6e 732f 776f 726b  hub/actions/work
+00000390: 666c 6f77 2f73 7461 7475 732f 6d61 646b  flow/status/madk
+000003a0: 696e 737a 2f70 6f65 7472 792d 7265 6c61  insz/poetry-rela
+000003b0: 782f 6275 696c 642e 7961 6d6c 3f6c 6162  x/build.yaml?lab
+000003c0: 656c 3d62 7569 6c64 2673 7479 6c65 3d66  el=build&style=f
+000003d0: 6c61 742d 7371 7561 7265 223e 0a20 2020  lat-square">.   
+000003e0: 203c 2f61 3e0a 3c2f 703e 0a0a 2320 706f   </a>.</p>..# po
+000003f0: 6574 7279 2d72 656c 6178 0a0a 4120 5b50  etry-relax..A [P
+00000400: 6f65 7472 795d 2868 7474 7073 3a2f 2f67  oetry](https://g
+00000410: 6974 6875 622e 636f 6d2f 7079 7468 6f6e  ithub.com/python
+00000420: 2d70 6f65 7472 792f 706f 6574 7279 2920  -poetry/poetry) 
+00000430: 706c 7567 696e 2074 6f20 7265 6c61 7820  plugin to relax 
+00000440: 6465 7065 6e64 656e 6379 2076 6572 7369  dependency versi
+00000450: 6f6e 7320 7768 656e 2070 7562 6c69 7368  ons when publish
+00000460: 696e 6720 6c69 6272 6172 6965 732e 2052  ing libraries. R
+00000470: 656c 6178 2079 6f75 7220 7072 6f6a 6563  elax your projec
+00000480: 7427 7320 6465 7065 6e64 656e 6369 6573  t's dependencies
+00000490: 2066 726f 6d20 6066 6f6f 6261 725e 322e   from `foobar^2.
+000004a0: 302e 3060 2074 6f20 6066 6f6f 6261 723e  0.0` to `foobar>
+000004b0: 3d32 2e30 2e30 602e 0a0a 4279 2064 6566  =2.0.0`...By def
+000004c0: 6175 6c74 2c20 506f 6574 7279 2075 7365  ault, Poetry use
+000004d0: 7320 6361 7265 7420 636f 6e73 7472 6169  s caret constrai
+000004e0: 6e74 7320 7768 6963 6820 776f 756c 6420  nts which would 
+000004f0: 6c69 6d69 7420 6066 6f6f 6261 7260 2076  limit `foobar` v
+00000500: 6572 7369 6f6e 7320 746f 2060 3c33 2e30  ersions to `<3.0
+00000510: 602e 0a2a 2a70 6f65 7472 792d 7265 6c61  `..**poetry-rela
+00000520: 782a 2a20 2072 656d 6f76 6573 2074 6865  x**  removes the
+00000530: 7365 2075 7070 6572 2076 6572 7369 6f6e  se upper version
+00000540: 2062 6f75 6e64 732c 2061 6c6c 6f77 696e   bounds, allowin
+00000550: 6720 6465 7065 6e64 656e 6369 6573 2074  g dependencies t
+00000560: 6f20 6265 2075 7067 7261 6465 642e 0a0a  o be upgraded...
+00000570: 5265 6d6f 7669 6e67 2075 7070 6572 2076  Removing upper v
+00000580: 6572 7369 6f6e 2062 6f75 6e64 7320 6973  ersion bounds is
+00000590: 2069 6d70 6f72 7461 6e74 2077 6865 6e20   important when 
+000005a0: 7075 626c 6973 6869 6e67 206c 6962 7261  publishing libra
+000005b0: 7269 6573 2e0a 5768 656e 2073 6561 7263  ries..When searc
+000005c0: 6869 6e67 2066 6f72 2076 6572 7369 6f6e  hing for version
+000005d0: 7320 6f66 2064 6570 656e 6465 6e63 6965  s of dependencie
+000005e0: 7320 746f 2069 6e73 7461 6c6c 2c20 7468  s to install, th
+000005f0: 6520 7265 736f 6c76 6572 2028 652e 672e  e resolver (e.g.
+00000600: 2060 7069 7060 2920 6d75 7374 2072 6573   `pip`) must res
+00000610: 7065 6374 2074 6865 2062 6f75 6e64 7320  pect the bounds 
+00000620: 796f 7572 206c 6962 7261 7279 2073 7065  your library spe
+00000630: 6369 6669 6573 2e0a 5768 656e 2061 206e  cifies..When a n
+00000640: 6577 2076 6572 7369 6f6e 206f 6620 7468  ew version of th
+00000650: 6520 6465 7065 6e64 656e 6379 2069 7320  e dependency is 
+00000660: 7265 6c65 6173 6564 2c20 636f 6e73 756d  released, consum
+00000670: 6572 7320 6f66 2079 6f75 7220 6c69 6272  ers of your libr
+00000680: 6172 7920 5f63 616e 6e6f 745f 2069 6e73  ary _cannot_ ins
+00000690: 7461 6c6c 2069 7420 756e 6c65 7373 2061  tall it unless a
+000006a0: 206e 6577 2076 6572 7369 6f6e 206f 6620   new version of 
+000006b0: 796f 7572 206c 6962 7261 7279 2069 7320  your library is 
+000006c0: 616c 736f 2072 656c 6561 7365 642e 0a0a  also released...
+000006d0: 4974 2069 7320 6e6f 7420 6665 6173 6962  It is not feasib
+000006e0: 6c65 2074 6f20 7265 6c65 6173 6520 7061  le to release pa
+000006f0: 7463 6865 7320 666f 7220 6576 6572 7920  tches for every 
+00000700: 7072 6576 696f 7573 2076 6572 7369 6f6e  previous version
+00000710: 206f 6620 6d6f 7374 206c 6962 7261 7269   of most librari
+00000720: 6573 2c20 7768 6963 6820 666f 7263 6573  es, which forces
+00000730: 2075 7365 7273 2074 6f20 7573 6520 7468   users to use th
+00000740: 6520 6d6f 7374 2072 6563 656e 7420 7665  e most recent ve
+00000750: 7273 696f 6e20 6f66 2074 6865 206c 6962  rsion of the lib
+00000760: 7261 7279 206f 7220 6265 2073 7475 636b  rary or be stuck
+00000770: 2077 6974 686f 7574 2074 6865 206e 6577   without the new
+00000780: 2076 6572 7369 6f6e 206f 6620 7468 6520   version of the 
+00000790: 6465 7065 6e64 656e 6379 2e0a 5768 656e  dependency..When
+000007a0: 206d 616e 7920 6c69 6272 6172 6965 7320   many libraries 
+000007b0: 636f 6e74 6169 6e20 7570 7065 7220 7665  contain upper ve
+000007c0: 7273 696f 6e20 626f 756e 6473 2c20 7468  rsion bounds, th
+000007d0: 6520 6465 7065 6e64 656e 6369 6573 2063  e dependencies c
+000007e0: 616e 2065 6173 696c 7920 6265 636f 6d65  an easily become
+000007f0: 205f 756e 736f 6c76 6162 6c65 5f20 e280   _unsolvable_ ..
+00000800: 9420 7768 6572 6520 6c69 6272 6172 6965  . where librarie
+00000810: 7320 6861 7665 2069 6e63 6f6d 7061 7469  s have incompati
+00000820: 626c 6520 6465 7065 6e64 656e 6379 2076  ble dependency v
+00000830: 6572 7369 6f6e 2072 6571 7569 7265 6d65  ersion requireme
+00000840: 6e74 732e 0a42 7920 7265 6d6f 7669 6e67  nts..By removing
+00000850: 2075 7070 6572 2076 6572 7369 6f6e 2062   upper version b
+00000860: 6f75 6e64 7320 6672 6f6d 2079 6f75 7220  ounds from your 
+00000870: 6c69 6272 6172 792c 2063 6f6e 7472 6f6c  library, control
+00000880: 2069 7320 7265 7475 726e 6564 2074 6f20   is returned to 
+00000890: 7468 6520 7573 6572 2e0a 0a50 6f65 7472  the user...Poetr
+000008a0: 7927 7320 6465 6661 756c 7420 6265 6861  y's default beha
+000008b0: 7669 6f72 2069 7320 746f 2069 6e63 6c75  vior is to inclu
+000008c0: 6465 2075 7070 6572 2076 6572 7369 6f6e  de upper version
+000008d0: 2062 6f75 6e64 732e 204d 616e 7920 7065   bounds. Many pe
+000008e0: 6f70 6c65 2068 6176 6520 7370 6f6b 656e  ople have spoken
+000008f0: 2075 7020 6167 6169 6e73 7420 7468 6973   up against this
+00000900: 2073 7479 6c65 206f 6620 6465 7065 6e64   style of depend
+00000910: 656e 6379 206d 616e 6167 656d 656e 7420  ency management 
+00000920: 696e 2074 6865 2050 7974 686f 6e20 6563  in the Python ec
+00000930: 6f73 7973 7465 6d2c 2069 6e63 6c75 6469  osystem, includi
+00000940: 6e67 206d 656d 6265 7273 206f 6620 7468  ng members of th
+00000950: 6520 5079 7468 6f6e 2063 6f72 6520 6465  e Python core de
+00000960: 7665 6c6f 706d 656e 7420 7465 616d 2e20  velopment team. 
+00000970: 5365 6520 5b74 6865 2062 6f74 746f 6d20  See [the bottom 
+00000980: 6f66 2074 6865 2072 6561 646d 655d 2823  of the readme](#
+00000990: 7265 6665 7265 6e63 6573 2920 666f 7220  references) for 
+000009a0: 6c69 6e6b 7320 616e 6420 6164 6469 7469  links and additi
+000009b0: 6f6e 616c 2063 6f6e 7465 7874 2e0a 0a53  onal context...S
+000009c0: 696e 6365 2074 6865 2050 6f65 7472 7920  ince the Poetry 
+000009d0: 7072 6f6a 6563 7420 7769 6c6c 206e 6f74  project will not
+000009e0: 2061 6c6c 6f77 2074 6869 7320 6265 6861   allow this beha
+000009f0: 7669 6f72 2074 6f20 6265 2063 6f6e 6669  vior to be confi
+00000a00: 6775 7265 642c 206d 6169 6e74 6169 6e65  gured, maintaine
+00000a10: 7273 2068 6176 6520 7265 736f 7274 6564  rs have resorted
+00000a20: 2074 6f20 6d61 6e75 616c 2065 6469 7469   to manual editi
+00000a30: 6e67 206f 6620 6465 7065 6e64 656e 6379  ng of dependency
+00000a40: 2063 6f6e 7374 7261 696e 7473 2061 6674   constraints aft
+00000a50: 6572 2061 6464 696e 672e 202a 2a70 6f65  er adding. **poe
+00000a60: 7472 792d 7265 6c61 782a 2a20 6169 6d73  try-relax** aims
+00000a70: 2074 6f20 6175 746f 6d61 7465 2061 6e64   to automate and
+00000a80: 2073 696d 706c 6966 7920 7468 6973 2070   simplify this p
+00000a90: 726f 6365 7373 2e0a 0a2a 2a70 6f65 7472  rocess...**poetr
+00000aa0: 792d 7265 6c61 782a 2a20 7072 6f76 6964  y-relax** provid
+00000ab0: 6573 3a0a 2d20 4175 746f 6d61 7465 6420  es:.- Automated 
+00000ac0: 7265 6d6f 7661 6c20 6f66 2075 7070 6572  removal of upper
+00000ad0: 2062 6f75 6e64 2063 6f6e 7374 7261 696e   bound constrain
+00000ae0: 7473 2073 7065 6369 6669 6564 2077 6974  ts specified wit
+00000af0: 6820 605e 600a 2d20 5361 6665 7479 2063  h `^`.- Safety c
+00000b00: 6865 636b 2069 6620 7061 636b 6167 6520  heck if package 
+00000b10: 7265 7175 6972 656d 656e 7473 2061 7265  requirements are
+00000b20: 2073 7469 6c6c 2073 6f6c 7661 626c 6520   still solvable 
+00000b30: 6166 7465 7220 7265 6c61 7869 6e67 2063  after relaxing c
+00000b40: 6f6e 7374 7261 696e 7473 0a2d 2055 7067  onstraints.- Upg
+00000b50: 7261 6465 206f 6620 6465 7065 6e64 656e  rade of dependen
+00000b60: 6369 6573 2061 6674 6572 2072 656c 6178  cies after relax
+00000b70: 696e 6720 636f 6e73 7472 6169 6e74 730a  ing constraints.
+00000b80: 2d20 5570 6461 7465 206f 6620 7468 6520  - Update of the 
+00000b90: 6c6f 636b 2066 696c 6520 7769 7468 6f75  lock file withou
+00000ba0: 7420 7570 6772 6164 696e 6720 6465 7065  t upgrading depe
+00000bb0: 6e64 656e 6369 6573 0a2d 204c 696d 6974  ndencies.- Limit
+00000bc0: 2064 6570 656e 6465 6e63 7920 7265 6c61   dependency rela
+00000bd0: 7861 7469 6f6e 2074 6f20 7370 6563 6966  xation to specif
+00000be0: 6963 2064 6570 656e 6465 6e63 7920 6772  ic dependency gr
+00000bf0: 6f75 7073 0a2d 2052 6574 656e 7469 6f6e  oups.- Retention
+00000c00: 206f 6620 696e 7465 6e74 696f 6e61 6c20   of intentional 
+00000c10: 7570 7065 7220 626f 756e 6473 2069 6e64  upper bounds ind
+00000c20: 6963 6174 696e 6720 7472 7565 2069 6e63  icating true inc
+00000c30: 6f6d 7061 7469 6269 6c69 7469 6573 0a2d  ompatibilities.-
+00000c40: 2043 4c49 206d 6573 7361 6765 7320 6465   CLI messages de
+00000c50: 7369 676e 6564 2074 6f20 6d61 7463 6820  signed to match 
+00000c60: 506f 6574 7279 2773 206f 7574 7075 740a  Poetry's output.
+00000c70: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
+00000c80: 0a0a 5468 6520 706c 7567 696e 206d 7573  ..The plugin mus
+00000c90: 7420 6265 2069 6e73 7461 6c6c 6564 2069  t be installed i
+00000ca0: 6e20 506f 6574 7279 2773 2065 6e76 6972  n Poetry's envir
+00000cb0: 6f6e 6d65 6e74 2e20 5468 6973 2072 6571  onment. This req
+00000cc0: 7569 7265 7320 7573 6520 6f66 2074 6865  uires use of the
+00000cd0: 2020 6073 656c 6660 2073 7562 636f 6d6d    `self` subcomm
+00000ce0: 616e 642e 0a0a 6060 6062 6173 680a 2420  and...```bash.$ 
+00000cf0: 706f 6574 7279 2073 656c 6620 6164 6420  poetry self add 
+00000d00: 706f 6574 7279 2d72 656c 6178 0a60 6060  poetry-relax.```
+00000d10: 0a0a 2323 2055 7361 6765 0a0a 5265 6c61  ..## Usage..Rela
+00000d20: 7820 636f 6e73 7472 6169 6e74 7320 666f  x constraints fo
+00000d30: 7220 7768 6963 6820 506f 6574 7279 2073  r which Poetry s
+00000d40: 6574 2061 6e20 7570 7065 7220 7665 7273  et an upper vers
+00000d50: 696f 6e3a 0a0a 6060 6062 6173 680a 2420  ion:..```bash.$ 
+00000d60: 706f 6574 7279 2072 656c 6178 0a60 6060  poetry relax.```
+00000d70: 0a0a 5265 6c61 7820 636f 6e73 7472 6169  ..Relax constrai
+00000d80: 6e74 7320 616e 6420 6368 6563 6b20 7468  nts and check th
+00000d90: 6174 2074 6865 7920 6172 6520 7265 736f  at they are reso
+00000da0: 6c76 6162 6c65 2077 6974 686f 7574 2070  lvable without p
+00000db0: 6572 666f 726d 696e 6720 7570 6772 6164  erforming upgrad
+00000dc0: 6573 3a0a 0a60 6060 6261 7368 0a24 2070  es:..```bash.$ p
+00000dd0: 6f65 7472 7920 7265 6c61 7820 2d2d 6368  oetry relax --ch
+00000de0: 6563 6b0a 6060 600a 0a52 656c 6178 2063  eck.```..Relax c
+00000df0: 6f6e 7374 7261 696e 7473 2061 6e64 2075  onstraints and u
+00000e00: 7067 7261 6465 2070 6163 6b61 6765 733a  pgrade packages:
+00000e10: 0a0a 6060 6062 6173 680a 2420 706f 6574  ..```bash.$ poet
+00000e20: 7279 2072 656c 6178 202d 2d75 7064 6174  ry relax --updat
+00000e30: 650a 6060 600a 0a52 656c 6178 2063 6f6e  e.```..Relax con
+00000e40: 7374 7261 696e 7473 2061 6e64 2075 7064  straints and upd
+00000e50: 6174 6520 7468 6520 6c6f 636b 2066 696c  ate the lock fil
+00000e60: 6520 7769 7468 6f75 7420 7570 6772 6164  e without upgrad
+00000e70: 696e 6720 7061 636b 6167 6573 3a0a 0a60  ing packages:..`
+00000e80: 6060 6261 7368 0a24 2070 6f65 7472 7920  ``bash.$ poetry 
+00000e90: 7265 6c61 7820 2d2d 6c6f 636b 0a60 6060  relax --lock.```
+00000ea0: 0a0a 5072 6576 6965 7720 7468 6520 6368  ..Preview the ch
+00000eb0: 616e 6765 7320 6070 6f65 7472 7920 7265  anges `poetry re
+00000ec0: 6c61 7860 2077 6f75 6c64 206d 616b 6520  lax` would make 
+00000ed0: 7769 7468 6f75 7420 6d6f 6469 6679 696e  without modifyin
+00000ee0: 6720 7468 6520 7072 6f6a 6563 743a 0a0a  g the project:..
+00000ef0: 6060 6062 6173 680a 2420 706f 6574 7279  ```bash.$ poetry
+00000f00: 2072 656c 6178 202d 2d64 7279 2d72 756e   relax --dry-run
+00000f10: 0a60 6060 0a0a 5265 6c61 7820 636f 6e73  .```..Relax cons
+00000f20: 7472 6169 6e74 7320 666f 7220 7370 6563  traints for spec
+00000f30: 6966 6963 2064 6570 656e 6465 6e63 7920  ific dependency 
+00000f40: 6772 6f75 7073 3a0a 0a60 6060 6261 7368  groups:..```bash
+00000f50: 0a24 2070 6f65 7472 7920 7265 6c61 7820  .$ poetry relax 
+00000f60: 2d2d 6f6e 6c79 2066 6f6f 202d 2d6f 6e6c  --only foo --onl
+00000f70: 7920 6261 720a 6060 600a 0a52 656c 6178  y bar.```..Relax
+00000f80: 2063 6f6e 7374 7261 696e 7473 2065 7863   constraints exc
+00000f90: 6c75 6469 6e67 2073 7065 6369 6669 6320  luding specific 
+00000fa0: 6465 7065 6e64 656e 6379 2067 726f 7570  dependency group
+00000fb0: 733a 0a0a 6060 6062 6173 680a 2420 706f  s:..```bash.$ po
+00000fc0: 6574 7279 2072 656c 6178 202d 2d77 6974  etry relax --wit
+00000fd0: 686f 7574 2066 6f6f 202d 2d77 6974 686f  hout foo --witho
+00000fe0: 7574 2062 6172 0a60 6060 0a0a 0a23 2320  ut bar.```...## 
+00000ff0: 4578 616d 706c 6573 0a0a 5468 6520 6265  Examples..The be
+00001000: 6861 7669 6f72 206f 6620 506f 6574 7279  havior of Poetry
+00001010: 2069 7320 7175 6974 6520 7265 6173 6f6e   is quite reason
+00001020: 6162 6c65 2066 6f72 206c 6f63 616c 2064  able for local d
+00001030: 6576 656c 6f70 6d65 6e74 2120 6070 6f65  evelopment! `poe
+00001040: 7472 7920 7265 6c61 7860 2069 7320 6d6f  try relax` is mo
+00001050: 7374 2075 7365 6675 6c20 7768 656e 2075  st useful when u
+00001060: 7365 6420 696e 2043 492f 4344 2070 6970  sed in CI/CD pip
+00001070: 656c 696e 6573 2e0a 0a23 2323 2052 656c  elines...### Rel
+00001080: 6178 696e 6720 7265 7175 6972 656d 656e  axing requiremen
+00001090: 7473 2062 6566 6f72 6520 7075 626c 6973  ts before publis
+000010a0: 6869 6e67 0a0a 5275 6e20 6070 6f65 7472  hing..Run `poetr
+000010b0: 7920 7265 6c61 7860 2062 6566 6f72 6520  y relax` before 
+000010c0: 6275 696c 6469 6e67 2061 6e64 2070 7562  building and pub
+000010d0: 6c69 7368 696e 6720 6120 7061 636b 6167  lishing a packag
+000010e0: 652e 0a0a 5365 6520 6974 2061 7420 776f  e...See it at wo
+000010f0: 726b 2069 6e20 5b74 6865 2072 656c 6561  rk in [the relea
+00001100: 7365 2077 6f72 6b66 6c6f 7720 666f 7220  se workflow for 
+00001110: 7468 6973 2070 726f 6a65 6374 5d28 6874  this project](ht
+00001120: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001130: 2f6d 6164 6b69 6e73 7a2f 706f 6574 7279  /madkinsz/poetry
+00001140: 2d72 656c 6178 2f62 6c6f 622f 6d61 696e  -relax/blob/main
+00001150: 2f2e 6769 7468 7562 2f77 6f72 6b66 6c6f  /.github/workflo
+00001160: 7773 2f72 656c 6561 7365 2e79 616d 6c29  ws/release.yaml)
+00001170: 2e0a 0a0a 2323 2320 5265 6c61 7869 6e67  ....### Relaxing
+00001180: 2072 6571 7569 7265 6d65 6e74 7320 666f   requirements fo
+00001190: 7220 7465 7374 696e 670a 0a52 756e 2060  r testing..Run `
+000011a0: 706f 6574 7279 2072 656c 6178 202d 2d75  poetry relax --u
+000011b0: 7064 6174 6560 2062 6566 6f72 6520 7465  pdate` before te
+000011c0: 7374 7320 746f 2074 6573 7420 6167 6169  sts to test agai
+000011d0: 6e73 7420 7468 6520 6e65 7765 7374 2070  nst the newest p
+000011e0: 6f73 7369 626c 6520 7665 7273 696f 6e73  ossible versions
+000011f0: 206f 6620 7061 636b 6167 6573 2e0a 0a53   of packages...S
+00001200: 6565 2069 7420 6174 2077 6f72 6b20 696e  ee it at work in
+00001210: 205b 7468 6520 7465 7374 2077 6f72 6b66   [the test workf
+00001220: 6c6f 7720 666f 7220 7468 6973 2070 726f  low for this pro
+00001230: 6a65 6374 5d28 6874 7470 733a 2f2f 6769  ject](https://gi
+00001240: 7468 7562 2e63 6f6d 2f6d 6164 6b69 6e73  thub.com/madkins
+00001250: 7a2f 706f 6574 7279 2d72 656c 6178 2f62  z/poetry-relax/b
+00001260: 6c6f 622f 6d61 696e 2f2e 6769 7468 7562  lob/main/.github
+00001270: 2f77 6f72 6b66 6c6f 7773 2f74 6573 742e  /workflows/test.
+00001280: 7961 6d6c 292e 0a0a 2323 2046 7265 7175  yaml)...## Frequ
+00001290: 656e 746c 7920 6173 6b65 6420 7175 6573  ently asked ques
+000012a0: 7469 6f6e 730a 0a3e 2043 616e 2074 6869  tions..> Can thi
+000012b0: 7320 706c 7567 696e 2063 6861 6e67 6520  s plugin change 
+000012c0: 7468 6520 6265 6861 7669 6f72 206f 6620  the behavior of 
+000012d0: 6070 6f65 7472 7920 6164 6460 2074 6f20  `poetry add` to 
+000012e0: 7265 6c61 7820 636f 6e73 7472 6169 6e74  relax constraint
+000012f0: 733f 0a0a 4e6f 7420 6174 2074 6869 7320  s?..Not at this 
+00001300: 7469 6d65 2e20 5468 6520 506f 6574 7279  time. The Poetry
+00001310: 2070 726f 6a65 6374 2073 7461 7465 7320   project states 
+00001320: 7468 6174 2070 6c75 6769 6e73 206d 7573  that plugins mus
+00001330: 7420 6e6f 7420 616c 7465 7220 7468 6520  t not alter the 
+00001340: 6265 6861 7669 6f72 206f 6620 636f 7265  behavior of core
+00001350: 2050 6f65 7472 7920 636f 6d6d 616e 6473   Poetry commands
+00001360: 2e20 4966 2074 6869 7320 6265 6861 7669  . If this behavi
+00001370: 6f72 2077 6f75 6c64 2062 6520 7573 6566  or would be usef
+00001380: 756c 2066 6f72 2079 6f75 2c20 706c 6561  ul for you, plea
+00001390: 7365 2063 6869 6d65 2069 6e20 5b6f 6e20  se chime in [on 
+000013a0: 7468 6520 7472 6163 6b69 6e67 2069 7373  the tracking iss
+000013b0: 7565 5d28 6874 7470 733a 2f2f 6769 7468  ue](https://gith
+000013c0: 7562 2e63 6f6d 2f6d 6164 6b69 6e73 7a2f  ub.com/madkinsz/
+000013d0: 706f 6574 7279 2d72 656c 6178 2f69 7373  poetry-relax/iss
+000013e0: 7565 732f 3529 2e0a 0a3e 2044 6f65 7320  ues/5)...> Does 
+000013f0: 7468 6973 2070 6c75 6769 6e20 7265 6d6f  this plugin remo
+00001400: 7665 2075 7070 6572 2063 6f6e 7374 7261  ve upper constra
+00001410: 696e 7473 2049 2776 6520 6164 6465 643f  ints I've added?
+00001420: 0a0a 5468 6973 2070 6c75 6769 6e20 7769  ..This plugin wi
+00001430: 6c6c 206f 6e6c 7920 7265 6c61 7820 636f  ll only relax co
+00001440: 6e73 7472 6169 6e74 7320 7370 6563 6966  nstraints specif
+00001450: 6965 6420 7769 7468 2061 2063 6172 6574  ied with a caret
+00001460: 2028 605e 6029 2e20 5570 7065 7220 636f   (`^`). Upper co
+00001470: 6e73 7472 6169 6e74 7320 6164 6465 6420  nstraints added 
+00001480: 7769 7468 2060 3c60 2061 6e64 2060 3c3d  with `<` and `<=
+00001490: 6020 7769 6c6c 206e 6f74 2062 6520 6368  ` will not be ch
+000014a0: 616e 6765 642e 0a0a 3e20 4973 2074 6869  anged...> Is thi
+000014b0: 7320 706c 7567 696e 2073 7461 626c 653f  s plugin stable?
+000014c0: 0a0a 5468 6973 2070 6c75 6769 6e20 6973  ..This plugin is
+000014d0: 2074 6573 7465 6420 6167 6169 6e73 7420   tested against 
+000014e0: 6d75 6c74 6970 6c65 2076 6572 7369 6f6e  multiple version
+000014f0: 7320 6f66 2050 6f65 7472 7920 616e 6420  s of Poetry and 
+00001500: 6861 7320 616e 2069 6e74 6567 7261 7469  has an integrati
+00001510: 6f6e 2066 6f63 7573 6564 2074 6573 7420  on focused test 
+00001520: 7375 6974 652e 2049 7420 6973 2073 6166  suite. It is saf
+00001530: 6520 746f 2075 7365 2074 6869 7320 696e  e to use this in
+00001540: 2070 726f 6475 6374 696f 6e2c 2074 686f   production, tho
+00001550: 7567 6820 6974 2069 7320 7265 636f 6d6d  ugh it is recomm
+00001560: 656e 6420 746f 2070 696e 2076 6572 7369  end to pin versi
+00001570: 6f6e 732e 2042 7265 616b 696e 6720 6368  ons. Breaking ch
+00001580: 616e 6765 7320 7769 6c6c 2062 6520 6176  anges will be av
+00001590: 6f69 6465 6420 756e 6c65 7373 2069 6e66  oided unless inf
+000015a0: 6561 7369 626c 6520 6475 6520 746f 2075  easible due to u
+000015b0: 7073 7472 6561 6d20 6368 616e 6765 7320  pstream changes 
+000015c0: 696e 2050 6f65 7472 792e 0a0a 3e20 5769  in Poetry...> Wi
+000015d0: 6c6c 2074 6869 7320 706c 7567 696e 2064  ll this plugin d
+000015e0: 726f 7020 7468 6520 7570 7065 7220 626f  rop the upper bo
+000015f0: 756e 6420 6f6e 2050 7974 686f 6e20 6974  und on Python it
+00001600: 7365 6c66 3f0a 0a42 656c 6965 7665 2069  self?..Believe i
+00001610: 7420 6f72 206e 6f74 2c20 7468 6973 2069  t or not, this i
+00001620: 7320 616e 2065 7665 6e20 6d6f 7265 2063  s an even more c
+00001630: 6f6e 7465 6e74 696f 7573 2073 7562 7365  ontentious subse
+00001640: 7420 6f66 2074 6869 7320 6973 7375 6520  t of this issue 
+00001650: 6173 2050 6f65 7472 7920 7769 6c6c 206e  as Poetry will n
+00001660: 6f74 2061 6c6c 6f77 2070 6163 6b61 6765  ot allow package
+00001670: 7320 7769 7468 206e 6f20 7570 7065 7220  s with no upper 
+00001680: 626f 756e 6420 6f6e 2050 7974 686f 6e20  bound on Python 
+00001690: 746f 2065 7869 7374 2061 6c6f 6e67 7369  to exist alongsi
+000016a0: 6465 2074 686f 7365 2074 6861 7420 696e  de those that in
+000016b0: 636c 7564 6520 6f6e 652e 2054 6869 7320  clude one. This 
+000016c0: 6261 7369 6361 6c6c 7920 6d65 616e 7320  basically means 
+000016d0: 7468 6174 2077 6520 6361 6e6e 6f74 2072  that we cannot r
+000016e0: 656c 6178 2074 6869 7320 7265 7175 6972  elax this requir
+000016f0: 656d 656e 7420 7769 7468 6f75 7420 6272  ement without br
+00001700: 6561 6b69 6e67 2074 6865 2076 6173 7420  eaking the vast 
+00001710: 6d61 6a6f 7269 7479 206f 6620 7573 652d  majority of use-
+00001720: 6361 7365 732e 2046 6f72 2074 6869 7320  cases. For this 
+00001730: 7265 6173 6f6e 2c20 7765 2063 616e 6e6f  reason, we canno
+00001740: 7420 7265 6c61 7820 6070 7974 686f 6e5e  t relax `python^
+00001750: 3360 2061 7420 7468 6973 2074 696d 652e  3` at this time.
+00001760: 2053 6565 205b 7468 6520 706f 7374 206f   See [the post o
+00001770: 6e20 7468 6520 506f 6574 7279 2064 6973  n the Poetry dis
+00001780: 6375 7373 696f 6e20 626f 6172 645d 2868  cussion board](h
+00001790: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000017a0: 6d2f 7079 7468 6f6e 2d70 6f65 7472 792f  m/python-poetry/
+000017b0: 706f 6574 7279 2f64 6973 6375 7373 696f  poetry/discussio
+000017c0: 6e73 2f33 3735 3723 6469 7363 7573 7369  ns/3757#discussi
+000017d0: 6f6e 636f 6d6d 656e 742d 3433 3533 3435  oncomment-435345
+000017e0: 2920 666f 7220 6d6f 7265 2064 6574 6169  ) for more detai
+000017f0: 6c73 2e0a 0a23 2320 436f 6e74 7269 6275  ls...## Contribu
+00001800: 7469 6e67 0a0a 5468 6973 2070 726f 6a65  ting..This proje
+00001810: 6374 2069 7320 6d61 6e61 6765 6420 7769  ct is managed wi
+00001820: 7468 2050 6f65 7472 792e 2048 6572 6520  th Poetry. Here 
+00001830: 6172 6520 7468 6520 6261 7369 6373 2066  are the basics f
+00001840: 6f72 2067 6574 7469 6e67 2073 7461 7274  or getting start
+00001850: 6564 2e0a 0a43 6c6f 6e65 2074 6865 2072  ed...Clone the r
+00001860: 6570 6f73 6974 6f72 793a 0a60 6060 6261  epository:.```ba
+00001870: 7368 0a24 2067 6974 2063 6c6f 6e65 2068  sh.$ git clone h
+00001880: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001890: 6d2f 6d61 646b 696e 737a 2f70 6f65 7472  m/madkinsz/poetr
+000018a0: 792d 7265 6c61 782e 6769 740a 2420 6364  y-relax.git.$ cd
+000018b0: 2070 6f65 7472 792d 7265 6c61 780a 6060   poetry-relax.``
+000018c0: 600a 0a49 6e73 7461 6c6c 2070 6163 6b61  `..Install packa
+000018d0: 6765 733a 0a60 6060 6261 7368 0a24 2070  ges:.```bash.$ p
+000018e0: 6f65 7472 7920 696e 7374 616c 6c0a 6060  oetry install.``
+000018f0: 600a 0a52 756e 2074 6865 2074 6573 7420  `..Run the test 
+00001900: 7375 6974 653a 0a60 6060 6261 7368 0a24  suite:.```bash.$
+00001910: 2070 7974 6573 7420 7465 7374 730a 6060   pytest tests.``
+00001920: 600a 0a52 756e 206c 696e 7465 7273 2062  `..Run linters b
+00001930: 6566 6f72 6520 6f70 656e 696e 6720 7075  efore opening pu
+00001940: 6c6c 2072 6571 7565 7374 733a 0a60 6060  ll requests:.```
+00001950: 6261 7368 0a24 202e 2f62 696e 2f6c 696e  bash.$ ./bin/lin
+00001960: 7420 6368 6563 6b20 2e0a 2420 2e2f 6269  t check ..$ ./bi
+00001970: 6e2f 6c69 6e74 2066 6978 202e 0a60 6060  n/lint fix ..```
+00001980: 0a0a 2323 2052 6566 6572 656e 6365 730a  ..## References.
+00001990: 0a54 6865 7265 2773 2061 206c 6f74 2074  .There's a lot t
+000019a0: 6f20 7265 6164 206f 6e20 7468 6973 2074  o read on this t
+000019b0: 6f70 6963 2120 4974 2773 2063 6f6e 7465  opic! It's conte
+000019c0: 6e74 696f 7573 2061 6e64 2063 6175 7369  ntious and causi
+000019d0: 6e67 2061 206c 6f74 206f 6620 7072 6f62  ng a lot of prob
+000019e0: 6c65 6d73 2066 6f72 206d 6169 6e74 6169  lems for maintai
+000019f0: 6e65 7273 2061 6e64 2075 7365 7273 2e0a  ners and users..
+00001a00: 0a54 6865 2066 6f6c 6c6f 7769 6e67 2062  .The following b
+00001a10: 6c6f 6720 706f 7374 7320 6279 2048 656e  log posts by Hen
+00001a20: 7279 2053 6368 7265 696e 6572 2061 7265  ry Schreiner are
+00001a30: 2071 7569 7465 2063 6f6d 7072 6568 656e   quite comprehen
+00001a40: 7369 7665 3a0a 2d20 5b53 686f 756c 6420  sive:.- [Should 
+00001a50: 596f 7520 5573 6520 5570 7065 7220 426f  You Use Upper Bo
+00001a60: 756e 6420 5665 7273 696f 6e20 436f 6e73  und Version Cons
+00001a70: 7472 6169 6e74 733f 5d28 6874 7470 733a  traints?](https:
+00001a80: 2f2f 6973 6369 6e75 6d70 792e 6465 762f  //iscinumpy.dev/
+00001a90: 706f 7374 2f62 6f75 6e64 2d76 6572 7369  post/bound-versi
+00001aa0: 6f6e 2d63 6f6e 7374 7261 696e 7473 2f29  on-constraints/)
+00001ab0: 0a2d 205b 506f 6574 7279 2056 6572 7369  .- [Poetry Versi
+00001ac0: 6f6e 735d 2868 7474 7073 3a2f 2f69 7363  ons](https://isc
+00001ad0: 696e 756d 7079 2e64 6576 2f70 6f73 742f  inumpy.dev/post/
+00001ae0: 706f 6574 7279 2d76 6572 7369 6f6e 732f  poetry-versions/
+00001af0: 290a 0a43 6f6e 7465 6e74 2066 726f 6d20  )..Content from 
+00001b00: 736f 6d65 206d 656d 6265 7273 206f 6620  some members of 
+00001b10: 7468 6520 5079 7468 6f6e 2063 6f72 6520  the Python core 
+00001b20: 6465 7665 6c6f 7065 7220 7465 616d 3a0a  developer team:.
+00001b30: 2d20 5b53 656d 616e 7469 6320 5665 7273  - [Semantic Vers
+00001b40: 696f 6e69 6e67 2057 696c 6c20 4e6f 7420  ioning Will Not 
+00001b50: 5361 7665 2059 6f75 5d28 6874 7470 733a  Save You](https:
+00001b60: 2f2f 6879 6e65 6b2e 6d65 2f61 7274 6963  //hynek.me/artic
+00001b70: 6c65 732f 7365 6d76 6572 2d77 696c 6c2d  les/semver-will-
+00001b80: 6e6f 742d 7361 7665 2d79 6f75 2f29 0a2d  not-save-you/).-
+00001b90: 205b 5768 7920 4920 646f 6e27 7420 6c69   [Why I don't li
+00001ba0: 6b65 2053 656d 5665 7220 616e 796d 6f72  ke SemVer anymor
+00001bb0: 655d 2868 7474 7073 3a2f 2f73 6e61 726b  e](https://snark
+00001bc0: 792e 6361 2f77 6879 2d69 2d64 6f6e 742d  y.ca/why-i-dont-
+00001bd0: 6c69 6b65 2d73 656d 7665 722f 290a 2d20  like-semver/).- 
+00001be0: 5b56 6572 7369 6f6e 206e 756d 6265 7273  [Version numbers
+00001bf0: 3a20 686f 7720 746f 2075 7365 2074 6865  : how to use the
+00001c00: 6d3f 5d28 6874 7470 733a 2f2f 6265 726e  m?](https://bern
+00001c10: 6174 2e74 6563 682f 706f 7374 732f 7665  at.tech/posts/ve
+00001c20: 7273 696f 6e2d 6e75 6d62 6572 732f 290a  rsion-numbers/).
+00001c30: 2d20 5b56 6572 7369 6f6e 696e 6720 536f  - [Versioning So
+00001c40: 6674 7761 7265 5d28 6874 7470 733a 2f2f  ftware](https://
+00001c50: 6361 7265 6d61 642e 696f 2f70 6f73 7473  caremad.io/posts
+00001c60: 2f32 3031 362f 3032 2f76 6572 7369 6f6e  /2016/02/version
+00001c70: 696e 672d 736f 6674 7761 7265 2f29 0a0a  ing-software/)..
+00001c80: 4469 7363 7573 7369 6f6e 2061 6e64 2069  Discussion and i
+00001c90: 7373 7565 7320 696e 2074 6865 2050 6f65  ssues in the Poe
+00001ca0: 7472 7920 7072 6f6a 6563 743a 0a2d 205b  try project:.- [
+00001cb0: 506c 6561 7365 2073 746f 7020 7069 6e6e  Please stop pinn
+00001cc0: 696e 6720 746f 206d 616a 6f72 2076 6572  ing to major ver
+00001cd0: 7369 6f6e 7320 6279 2064 6566 6175 6c74  sions by default
+00001ce0: 2c20 6573 7065 6369 616c 6c79 2066 6f72  , especially for
+00001cf0: 2050 7974 686f 6e20 6974 7365 6c66 5d28   Python itself](
+00001d00: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001d10: 6f6d 2f70 7974 686f 6e2d 706f 6574 7279  om/python-poetry
+00001d20: 2f70 6f65 7472 792f 6973 7375 6573 2f33  /poetry/issues/3
+00001d30: 3734 3729 0a2d 205b 4368 616e 6765 2064  747).- [Change d
+00001d40: 6566 6175 6c74 2064 6570 656e 6465 6e63  efault dependenc
+00001d50: 7920 636f 6e73 7472 6169 6e74 2066 726f  y constraint fro
+00001d60: 6d20 5e20 746f 203e 3d5d 2868 7474 7073  m ^ to >=](https
+00001d70: 3a2f 2f67 6974 6875 622e 636f 6d2f 7079  ://github.com/py
+00001d80: 7468 6f6e 2d70 6f65 7472 792f 706f 6574  thon-poetry/poet
+00001d90: 7279 2f69 7373 7565 732f 3334 3237 290a  ry/issues/3427).
+00001da0: 2d20 5b44 6576 656c 6f70 6572 7320 7368  - [Developers sh
+00001db0: 6f75 6c64 2062 6520 6162 6c65 2074 6f20  ould be able to 
+00001dc0: 7475 726e 206f 6666 2064 6570 656e 6465  turn off depende
+00001dd0: 6e63 7920 7570 7065 722d 626f 756e 6420  ncy upper-bound 
+00001de0: 6361 6c63 756c 6174 696f 6e73 5d28 6874  calculations](ht
+00001df0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001e00: 2f70 7974 686f 6e2d 706f 6574 7279 2f70  /python-poetry/p
+00001e10: 6f65 7472 792f 6973 7375 6573 2f32 3733  oetry/issues/273
+00001e20: 3129 0a                                  1).
```

### Comparing `poetry-relax-0.1.2/PKG-INFO` & `poetry_relax-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 706f 6574  : 2.1.Name: poet
 00000020: 7279 2d72 656c 6178 0a56 6572 7369 6f6e  ry-relax.Version
-00000030: 3a20 302e 312e 320a 5375 6d6d 6172 793a  : 0.1.2.Summary:
+00000030: 3a20 312e 302e 300a 5375 6d6d 6172 793a  : 1.0.0.Summary:
 00000040: 2050 6c75 6769 6e20 666f 7220 506f 6574   Plugin for Poet
 00000050: 7279 2074 6f20 7265 6c61 7820 7570 7065  ry to relax uppe
 00000060: 7220 7665 7273 696f 6e20 7069 6e73 0a48  r version pins.H
 00000070: 6f6d 652d 7061 6765 3a20 6874 7470 733a  ome-page: https:
 00000080: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 6164  //github.com/mad
 00000090: 6b69 6e73 7a2f 706f 6574 7279 2d72 656c  kinsz/poetry-rel
 000000a0: 6178 0a4b 6579 776f 7264 733a 2070 6f65  ax.Keywords: poe
@@ -49,446 +49,506 @@
 00000300: 5079 7468 6f6e 203a 3a20 332e 390a 436c  Python :: 3.9.Cl
 00000310: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
 00000320: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
 00000330: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
 00000340: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
 00000350: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
 00000360: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000370: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000380: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000390: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000003a0: 2e31 300a 436c 6173 7369 6669 6572 3a20  .10.Classifier: 
-000003b0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000003c0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000003d0: 3a20 332e 3131 0a43 6c61 7373 6966 6965  : 3.11.Classifie
-000003e0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-000003f0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000400: 6e20 3a3a 2033 2e37 0a43 6c61 7373 6966  n :: 3.7.Classif
-00000410: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000420: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000430: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
-00000440: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000450: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000460: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
-00000470: 7373 6966 6965 723a 2054 6f70 6963 203a  ssifier: Topic :
-00000480: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
-00000490: 6f70 6d65 6e74 0a43 6c61 7373 6966 6965  opment.Classifie
-000004a0: 723a 2054 6f70 6963 203a 3a20 536f 6674  r: Topic :: Soft
-000004b0: 7761 7265 2044 6576 656c 6f70 6d65 6e74  ware Development
-000004c0: 203a 3a20 4c69 6272 6172 6965 730a 436c   :: Libraries.Cl
-000004d0: 6173 7369 6669 6572 3a20 5479 7069 6e67  assifier: Typing
-000004e0: 203a 3a20 5479 7065 640a 5265 7175 6972   :: Typed.Requir
-000004f0: 6573 2d44 6973 743a 2070 6f65 7472 7920  es-Dist: poetry 
-00000500: 283e 3d31 2e32 290a 5072 6f6a 6563 742d  (>=1.2).Project-
-00000510: 5552 4c3a 2052 6570 6f73 6974 6f72 792c  URL: Repository,
-00000520: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000530: 636f 6d2f 6d61 646b 696e 737a 2f70 6f65  com/madkinsz/poe
-00000540: 7472 792d 7265 6c61 780a 4465 7363 7269  try-relax.Descri
-00000550: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
-00000560: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
-00000570: 6e0a 0a23 2070 6f65 7472 792d 7265 6c61  n..# poetry-rela
-00000580: 780a 0a41 205b 506f 6574 7279 5d28 6874  x..A [Poetry](ht
-00000590: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000005a0: 2f70 7974 686f 6e2d 706f 6574 7279 2f70  /python-poetry/p
-000005b0: 6f65 7472 7929 2070 6c75 6769 6e20 746f  oetry) plugin to
-000005c0: 2072 656c 6178 2064 6570 656e 6465 6e63   relax dependenc
-000005d0: 7920 7665 7273 696f 6e73 2077 6865 6e20  y versions when 
-000005e0: 7075 626c 6973 6869 6e67 206c 6962 7261  publishing libra
-000005f0: 7269 6573 2e20 5265 6c61 7820 796f 7572  ries. Relax your
-00000600: 2070 726f 6a65 6374 2773 2064 6570 656e   project's depen
-00000610: 6465 6e63 6965 7320 6672 6f6d 2060 666f  dencies from `fo
-00000620: 6f62 6172 5e32 2e30 2e30 6020 746f 2060  obar^2.0.0` to `
-00000630: 666f 6f62 6172 3e3d 322e 302e 3060 2e0a  foobar>=2.0.0`..
-00000640: 0a42 7920 6465 6661 756c 742c 2050 6f65  .By default, Poe
-00000650: 7472 7920 7573 6573 2063 6172 6574 2063  try uses caret c
-00000660: 6f6e 7374 7261 696e 7473 2077 6869 6368  onstraints which
-00000670: 2077 6f75 6c64 206c 696d 6974 2060 666f   would limit `fo
-00000680: 6f62 6172 6020 7665 7273 696f 6e73 2074  obar` versions t
-00000690: 6f20 603c 332e 3060 2e0a 2a2a 706f 6574  o `<3.0`..**poet
-000006a0: 7279 2d72 656c 6178 2a2a 2020 7265 6d6f  ry-relax**  remo
-000006b0: 7665 7320 7468 6573 6520 7570 7065 7220  ves these upper 
-000006c0: 7665 7273 696f 6e20 626f 756e 6473 2c20  version bounds, 
-000006d0: 616c 6c6f 7769 6e67 2064 6570 656e 6465  allowing depende
-000006e0: 6e63 6965 7320 746f 2062 6520 7570 6772  ncies to be upgr
-000006f0: 6164 6564 2e0a 0a52 656d 6f76 696e 6720  aded...Removing 
-00000700: 7570 7065 7220 7665 7273 696f 6e20 626f  upper version bo
-00000710: 756e 6473 2069 7320 696d 706f 7274 616e  unds is importan
-00000720: 7420 7768 656e 2070 7562 6c69 7368 696e  t when publishin
-00000730: 6720 6c69 6272 6172 6965 732e 0a57 6865  g libraries..Whe
-00000740: 6e20 7365 6172 6368 696e 6720 666f 7220  n searching for 
-00000750: 7665 7273 696f 6e73 206f 6620 6465 7065  versions of depe
-00000760: 6e64 656e 6369 6573 2074 6f20 696e 7374  ndencies to inst
-00000770: 616c 6c2c 2074 6865 2072 6573 6f6c 7665  all, the resolve
-00000780: 7220 2865 2e67 2e20 6070 6970 6029 206d  r (e.g. `pip`) m
-00000790: 7573 7420 7265 7370 6563 7420 7468 6520  ust respect the 
-000007a0: 626f 756e 6473 2079 6f75 7220 6c69 6272  bounds your libr
-000007b0: 6172 7920 7370 6563 6966 6965 732e 0a57  ary specifies..W
-000007c0: 6865 6e20 6120 6e65 7720 7665 7273 696f  hen a new versio
-000007d0: 6e20 6f66 2074 6865 2064 6570 656e 6465  n of the depende
-000007e0: 6e63 7920 6973 2072 656c 6561 7365 642c  ncy is released,
-000007f0: 2063 6f6e 7375 6d65 7273 206f 6620 796f   consumers of yo
-00000800: 7572 206c 6962 7261 7279 205f 6361 6e6e  ur library _cann
-00000810: 6f74 5f20 696e 7374 616c 6c20 6974 2075  ot_ install it u
-00000820: 6e6c 6573 7320 6120 6e65 7720 7665 7273  nless a new vers
-00000830: 696f 6e20 6f66 2079 6f75 7220 6c69 6272  ion of your libr
-00000840: 6172 7920 6973 2061 6c73 6f20 7265 6c65  ary is also rele
-00000850: 6173 6564 2e0a 0a49 7420 6973 206e 6f74  ased...It is not
-00000860: 2066 6561 7369 626c 6520 746f 2072 656c   feasible to rel
-00000870: 6561 7365 2070 6174 6368 6573 2066 6f72  ease patches for
-00000880: 2065 7665 7279 2070 7265 7669 6f75 7320   every previous 
-00000890: 7665 7273 696f 6e20 6f66 206d 6f73 7420  version of most 
-000008a0: 6c69 6272 6172 6965 732c 2077 6869 6368  libraries, which
-000008b0: 2066 6f72 6365 7320 7573 6572 7320 746f   forces users to
-000008c0: 2075 7365 2074 6865 206d 6f73 7420 7265   use the most re
-000008d0: 6365 6e74 2076 6572 7369 6f6e 206f 6620  cent version of 
-000008e0: 7468 6520 6c69 6272 6172 7920 6f72 2062  the library or b
-000008f0: 6520 7374 7563 6b20 7769 7468 6f75 7420  e stuck without 
-00000900: 7468 6520 6e65 7720 7665 7273 696f 6e20  the new version 
-00000910: 6f66 2074 6865 2064 6570 656e 6465 6e63  of the dependenc
-00000920: 792e 0a57 6865 6e20 6d61 6e79 206c 6962  y..When many lib
-00000930: 7261 7269 6573 2063 6f6e 7461 696e 2075  raries contain u
-00000940: 7070 6572 2076 6572 7369 6f6e 2062 6f75  pper version bou
-00000950: 6e64 732c 2074 6865 2064 6570 656e 6465  nds, the depende
-00000960: 6e63 6965 7320 6361 6e20 6561 7369 6c79  ncies can easily
-00000970: 2062 6563 6f6d 6520 5f75 6e73 6f6c 7661   become _unsolva
-00000980: 626c 655f 20e2 8094 2077 6865 7265 206c  ble_ ... where l
-00000990: 6962 7261 7269 6573 2068 6176 6520 696e  ibraries have in
-000009a0: 636f 6d70 6174 6962 6c65 2064 6570 656e  compatible depen
-000009b0: 6465 6e63 7920 7665 7273 696f 6e20 7265  dency version re
-000009c0: 7175 6972 656d 656e 7473 2e0a 4279 2072  quirements..By r
-000009d0: 656d 6f76 696e 6720 7570 7065 7220 7665  emoving upper ve
-000009e0: 7273 696f 6e20 626f 756e 6473 2066 726f  rsion bounds fro
-000009f0: 6d20 796f 7572 206c 6962 7261 7279 2c20  m your library, 
-00000a00: 636f 6e74 726f 6c20 6973 2072 6574 7572  control is retur
-00000a10: 6e65 6420 746f 2074 6865 2075 7365 722e  ned to the user.
-00000a20: 0a0a 506f 6574 7279 2773 2064 6566 6175  ..Poetry's defau
-00000a30: 6c74 2062 6568 6176 696f 7220 6973 2074  lt behavior is t
-00000a40: 6f20 696e 636c 7564 6520 7570 7065 7220  o include upper 
-00000a50: 7665 7273 696f 6e20 626f 756e 6473 2e20  version bounds. 
-00000a60: 4d61 6e79 2070 656f 706c 6520 6861 7665  Many people have
-00000a70: 2073 706f 6b65 6e20 7570 2061 6761 696e   spoken up again
-00000a80: 7374 2074 6869 7320 7374 796c 6520 6f66  st this style of
-00000a90: 2064 6570 656e 6465 6e63 7920 6d61 6e61   dependency mana
-00000aa0: 6765 6d65 6e74 2069 6e20 7468 6520 5079  gement in the Py
-00000ab0: 7468 6f6e 2065 636f 7379 7374 656d 2c20  thon ecosystem, 
-00000ac0: 696e 636c 7564 696e 6720 6d65 6d62 6572  including member
-00000ad0: 7320 6f66 2074 6865 2050 7974 686f 6e20  s of the Python 
-00000ae0: 636f 7265 2064 6576 656c 6f70 6d65 6e74  core development
-00000af0: 2074 6561 6d2e 2053 6565 205b 7468 6520   team. See [the 
-00000b00: 626f 7474 6f6d 206f 6620 7468 6520 7265  bottom of the re
-00000b10: 6164 6d65 5d28 2372 6566 6572 656e 6365  adme](#reference
-00000b20: 7329 2066 6f72 206c 696e 6b73 2061 6e64  s) for links and
-00000b30: 2061 6464 6974 696f 6e61 6c20 636f 6e74   additional cont
-00000b40: 6578 742e 0a0a 5369 6e63 6520 7468 6520  ext...Since the 
-00000b50: 506f 6574 7279 2070 726f 6a65 6374 2077  Poetry project w
-00000b60: 696c 6c20 6e6f 7420 616c 6c6f 7720 7468  ill not allow th
-00000b70: 6973 2062 6568 6176 696f 7220 746f 2062  is behavior to b
-00000b80: 6520 636f 6e66 6967 7572 6564 2c20 6d61  e configured, ma
-00000b90: 696e 7461 696e 6572 7320 6861 7665 2072  intainers have r
-00000ba0: 6573 6f72 7465 6420 746f 206d 616e 7561  esorted to manua
-00000bb0: 6c20 6564 6974 696e 6720 6f66 2064 6570  l editing of dep
-00000bc0: 656e 6465 6e63 7920 636f 6e73 7472 6169  endency constrai
-00000bd0: 6e74 7320 6166 7465 7220 6164 6469 6e67  nts after adding
-00000be0: 2e20 2a2a 706f 6574 7279 2d72 656c 6178  . **poetry-relax
-00000bf0: 2a2a 2061 696d 7320 746f 2061 7574 6f6d  ** aims to autom
-00000c00: 6174 6520 616e 6420 7369 6d70 6c69 6679  ate and simplify
-00000c10: 2074 6869 7320 7072 6f63 6573 732e 0a0a   this process...
-00000c20: 2a2a 706f 6574 7279 2d72 656c 6178 2a2a  **poetry-relax**
-00000c30: 2070 726f 7669 6465 733a 0a2d 2041 7574   provides:.- Aut
-00000c40: 6f6d 6174 6564 2072 656d 6f76 616c 206f  omated removal o
-00000c50: 6620 7570 7065 7220 626f 756e 6420 636f  f upper bound co
-00000c60: 6e73 7472 6169 6e74 7320 7370 6563 6966  nstraints specif
-00000c70: 6965 6420 7769 7468 2060 5e60 0a2d 2053  ied with `^`.- S
-00000c80: 6166 6574 7920 6368 6563 6b20 6966 2070  afety check if p
-00000c90: 6163 6b61 6765 2072 6571 7569 7265 6d65  ackage requireme
-00000ca0: 6e74 7320 6172 6520 7374 696c 6c20 736f  nts are still so
-00000cb0: 6c76 6162 6c65 2061 6674 6572 2072 656c  lvable after rel
-00000cc0: 6178 696e 6720 636f 6e73 7472 6169 6e74  axing constraint
-00000cd0: 730a 2d20 5570 6772 6164 6520 6f66 2064  s.- Upgrade of d
-00000ce0: 6570 656e 6465 6e63 6965 7320 6166 7465  ependencies afte
-00000cf0: 7220 7265 6c61 7869 6e67 2063 6f6e 7374  r relaxing const
-00000d00: 7261 696e 7473 0a2d 2055 7064 6174 6520  raints.- Update 
-00000d10: 6f66 2074 6865 206c 6f63 6b20 6669 6c65  of the lock file
-00000d20: 2077 6974 686f 7574 2075 7067 7261 6469   without upgradi
-00000d30: 6e67 2064 6570 656e 6465 6e63 6965 730a  ng dependencies.
-00000d40: 2d20 4c69 6d69 7420 6465 7065 6e64 656e  - Limit dependen
-00000d50: 6379 2072 656c 6178 6174 696f 6e20 746f  cy relaxation to
-00000d60: 2073 7065 6369 6669 6320 6465 7065 6e64   specific depend
-00000d70: 656e 6379 2067 726f 7570 730a 2d20 5265  ency groups.- Re
-00000d80: 7465 6e74 696f 6e20 6f66 2069 6e74 656e  tention of inten
-00000d90: 7469 6f6e 616c 2075 7070 6572 2062 6f75  tional upper bou
-00000da0: 6e64 7320 696e 6469 6361 7469 6e67 2074  nds indicating t
-00000db0: 7275 6520 696e 636f 6d70 6174 6962 696c  rue incompatibil
-00000dc0: 6974 6965 730a 2d20 434c 4920 6d65 7373  ities.- CLI mess
-00000dd0: 6167 6573 2064 6573 6967 6e65 6420 746f  ages designed to
-00000de0: 206d 6174 6368 2050 6f65 7472 7927 7320   match Poetry's 
-00000df0: 6f75 7470 7574 0a0a 2323 2049 6e73 7461  output..## Insta
-00000e00: 6c6c 6174 696f 6e0a 0a54 6865 2070 6c75  llation..The plu
-00000e10: 6769 6e20 6d75 7374 2062 6520 696e 7374  gin must be inst
-00000e20: 616c 6c65 6420 696e 2050 6f65 7472 7927  alled in Poetry'
-00000e30: 7320 656e 7669 726f 6e6d 656e 742e 2054  s environment. T
-00000e40: 6869 7320 7265 7175 6972 6573 2075 7365  his requires use
-00000e50: 206f 6620 7468 6520 2060 7365 6c66 6020   of the  `self` 
-00000e60: 7375 6263 6f6d 6d61 6e64 2e0a 0a60 6060  subcommand...```
-00000e70: 6261 7368 0a24 2070 6f65 7472 7920 7365  bash.$ poetry se
-00000e80: 6c66 2061 6464 2070 6f65 7472 792d 7265  lf add poetry-re
-00000e90: 6c61 780a 6060 600a 0a23 2320 5573 6167  lax.```..## Usag
-00000ea0: 650a 0a52 656c 6178 2063 6f6e 7374 7261  e..Relax constra
-00000eb0: 696e 7473 2066 6f72 2077 6869 6368 2050  ints for which P
-00000ec0: 6f65 7472 7920 7365 7420 616e 2075 7070  oetry set an upp
-00000ed0: 6572 2076 6572 7369 6f6e 3a0a 0a60 6060  er version:..```
-00000ee0: 6261 7368 0a24 2070 6f65 7472 7920 7265  bash.$ poetry re
-00000ef0: 6c61 780a 6060 600a 0a52 656c 6178 2063  lax.```..Relax c
-00000f00: 6f6e 7374 7261 696e 7473 2061 6e64 2063  onstraints and c
-00000f10: 6865 636b 2074 6861 7420 7468 6579 2061  heck that they a
-00000f20: 7265 2072 6573 6f6c 7661 626c 6520 7769  re resolvable wi
-00000f30: 7468 6f75 7420 7065 7266 6f72 6d69 6e67  thout performing
-00000f40: 2075 7067 7261 6465 733a 0a0a 6060 6062   upgrades:..```b
-00000f50: 6173 680a 2420 706f 6574 7279 2072 656c  ash.$ poetry rel
-00000f60: 6178 202d 2d63 6865 636b 0a60 6060 0a0a  ax --check.```..
-00000f70: 5265 6c61 7820 636f 6e73 7472 6169 6e74  Relax constraint
-00000f80: 7320 616e 6420 7570 6772 6164 6520 7061  s and upgrade pa
-00000f90: 636b 6167 6573 3a0a 0a60 6060 6261 7368  ckages:..```bash
-00000fa0: 0a24 2070 6f65 7472 7920 7265 6c61 7820  .$ poetry relax 
-00000fb0: 2d2d 7570 6461 7465 0a60 6060 0a0a 5265  --update.```..Re
-00000fc0: 6c61 7820 636f 6e73 7472 6169 6e74 7320  lax constraints 
-00000fd0: 616e 6420 7570 6461 7465 2074 6865 206c  and update the l
-00000fe0: 6f63 6b20 6669 6c65 2077 6974 686f 7574  ock file without
-00000ff0: 2075 7067 7261 6469 6e67 2070 6163 6b61   upgrading packa
-00001000: 6765 733a 0a0a 6060 6062 6173 680a 2420  ges:..```bash.$ 
-00001010: 706f 6574 7279 2072 656c 6178 202d 2d6c  poetry relax --l
-00001020: 6f63 6b0a 6060 600a 0a50 7265 7669 6577  ock.```..Preview
-00001030: 2074 6865 2063 6861 6e67 6573 2060 706f   the changes `po
-00001040: 6574 7279 2072 656c 6178 6020 776f 756c  etry relax` woul
-00001050: 6420 6d61 6b65 2077 6974 686f 7574 206d  d make without m
-00001060: 6f64 6966 7969 6e67 2074 6865 2070 726f  odifying the pro
-00001070: 6a65 6374 3a0a 0a60 6060 6261 7368 0a24  ject:..```bash.$
-00001080: 2070 6f65 7472 7920 7265 6c61 7820 2d2d   poetry relax --
-00001090: 6472 792d 7275 6e0a 6060 600a 0a23 2320  dry-run.```..## 
-000010a0: 4578 616d 706c 6573 0a0a 5468 6520 6265  Examples..The be
-000010b0: 6861 7669 6f72 206f 6620 506f 6574 7279  havior of Poetry
-000010c0: 2069 7320 7175 6974 6520 7265 6173 6f6e   is quite reason
-000010d0: 6162 6c65 2066 6f72 206c 6f63 616c 2064  able for local d
-000010e0: 6576 656c 6f70 6d65 6e74 2120 6070 6f65  evelopment! `poe
-000010f0: 7472 7920 7265 6c61 7860 2069 7320 6d6f  try relax` is mo
-00001100: 7374 2075 7365 6675 6c20 7768 656e 2075  st useful when u
-00001110: 7365 6420 696e 2043 492f 4344 2070 6970  sed in CI/CD pip
-00001120: 656c 696e 6573 2e0a 0a23 2323 2052 656c  elines...### Rel
-00001130: 6178 696e 6720 7265 7175 6972 656d 656e  axing requiremen
-00001140: 7473 2062 6566 6f72 6520 7075 626c 6973  ts before publis
-00001150: 6869 6e67 0a0a 5275 6e20 6070 6f65 7472  hing..Run `poetr
-00001160: 7920 7265 6c61 7860 2062 6566 6f72 6520  y relax` before 
-00001170: 6275 696c 6469 6e67 2061 6e64 2070 7562  building and pub
-00001180: 6c69 7368 696e 6720 6120 7061 636b 6167  lishing a packag
-00001190: 652e 0a0a 5365 6520 6974 2061 7420 776f  e...See it at wo
-000011a0: 726b 2069 6e20 5b74 6865 2072 656c 6561  rk in [the relea
-000011b0: 7365 2077 6f72 6b66 6c6f 7720 666f 7220  se workflow for 
-000011c0: 7468 6973 2070 726f 6a65 6374 5d28 6874  this project](ht
-000011d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000011e0: 2f6d 6164 6b69 6e73 7a2f 706f 6574 7279  /madkinsz/poetry
-000011f0: 2d72 656c 6178 2f62 6c6f 622f 6d61 696e  -relax/blob/main
-00001200: 2f2e 6769 7468 7562 2f77 6f72 6b66 6c6f  /.github/workflo
-00001210: 7773 2f72 656c 6561 7365 2e79 616d 6c29  ws/release.yaml)
-00001220: 2e0a 0a0a 2323 2320 5265 6c61 7869 6e67  ....### Relaxing
-00001230: 2072 6571 7569 7265 6d65 6e74 7320 666f   requirements fo
-00001240: 7220 7465 7374 696e 670a 0a52 756e 2060  r testing..Run `
-00001250: 706f 6574 7279 2072 656c 6178 202d 2d75  poetry relax --u
-00001260: 7064 6174 6560 2062 6566 6f72 6520 7465  pdate` before te
-00001270: 7374 7320 746f 2074 6573 7420 6167 6169  sts to test agai
-00001280: 6e73 7420 7468 6520 6e65 7765 7374 2070  nst the newest p
-00001290: 6f73 7369 626c 6520 7665 7273 696f 6e73  ossible versions
-000012a0: 206f 6620 7061 636b 6167 6573 2e0a 0a53   of packages...S
-000012b0: 6565 2069 7420 6174 2077 6f72 6b20 696e  ee it at work in
-000012c0: 205b 7468 6520 7465 7374 2077 6f72 6b66   [the test workf
-000012d0: 6c6f 7720 666f 7220 7468 6973 2070 726f  low for this pro
-000012e0: 6a65 6374 5d28 6874 7470 733a 2f2f 6769  ject](https://gi
-000012f0: 7468 7562 2e63 6f6d 2f6d 6164 6b69 6e73  thub.com/madkins
-00001300: 7a2f 706f 6574 7279 2d72 656c 6178 2f62  z/poetry-relax/b
-00001310: 6c6f 622f 6d61 696e 2f2e 6769 7468 7562  lob/main/.github
-00001320: 2f77 6f72 6b66 6c6f 7773 2f74 6573 742e  /workflows/test.
-00001330: 7961 6d6c 292e 0a0a 2323 2046 7265 7175  yaml)...## Frequ
-00001340: 656e 746c 7920 6173 6b65 6420 7175 6573  ently asked ques
-00001350: 7469 6f6e 730a 0a3e 2043 616e 2074 6869  tions..> Can thi
-00001360: 7320 706c 7567 696e 2063 6861 6e67 6520  s plugin change 
-00001370: 7468 6520 6265 6861 7669 6f72 206f 6620  the behavior of 
-00001380: 6070 6f65 7472 7920 6164 6460 2074 6f20  `poetry add` to 
-00001390: 7265 6c61 7820 636f 6e73 7472 6169 6e74  relax constraint
-000013a0: 733f 0a0a 4e6f 7420 6174 2074 6869 7320  s?..Not at this 
-000013b0: 7469 6d65 2e20 5468 6520 506f 6574 7279  time. The Poetry
-000013c0: 2070 726f 6a65 6374 2073 7461 7465 7320   project states 
-000013d0: 7468 6174 2070 6c75 6769 6e73 206d 7573  that plugins mus
-000013e0: 7420 6e6f 7420 616c 7465 7220 7468 6520  t not alter the 
-000013f0: 6265 6861 7669 6f72 206f 6620 636f 7265  behavior of core
-00001400: 2050 6f65 7472 7920 636f 6d6d 616e 6473   Poetry commands
-00001410: 2e20 4966 2074 6869 7320 6265 6861 7669  . If this behavi
-00001420: 6f72 2077 6f75 6c64 2062 6520 7573 6566  or would be usef
-00001430: 756c 2066 6f72 2079 6f75 2c20 706c 6561  ul for you, plea
-00001440: 7365 2063 6869 6d65 2069 6e20 5b6f 6e20  se chime in [on 
-00001450: 7468 6520 7472 6163 6b69 6e67 2069 7373  the tracking iss
-00001460: 7565 5d28 6874 7470 733a 2f2f 6769 7468  ue](https://gith
-00001470: 7562 2e63 6f6d 2f6d 6164 6b69 6e73 7a2f  ub.com/madkinsz/
-00001480: 706f 6574 7279 2d72 656c 6178 2f69 7373  poetry-relax/iss
-00001490: 7565 732f 3529 2e0a 0a3e 2044 6f65 7320  ues/5)...> Does 
-000014a0: 7468 6973 2070 6c75 6769 6e20 7265 6d6f  this plugin remo
-000014b0: 7665 2075 7070 6572 2063 6f6e 7374 7261  ve upper constra
-000014c0: 696e 7473 2049 2776 6520 6164 6465 643f  ints I've added?
-000014d0: 0a0a 5468 6973 2070 6c75 6769 6e20 7769  ..This plugin wi
-000014e0: 6c6c 206f 6e6c 7920 7265 6c61 7820 636f  ll only relax co
-000014f0: 6e73 7472 6169 6e74 7320 7370 6563 6966  nstraints specif
-00001500: 6965 6420 7769 7468 2061 2063 6172 6574  ied with a caret
-00001510: 2028 605e 6029 2e20 5570 7065 7220 636f   (`^`). Upper co
-00001520: 6e73 7472 6169 6e74 7320 6164 6465 6420  nstraints added 
-00001530: 7769 7468 2060 3c60 2061 6e64 2060 3c3d  with `<` and `<=
-00001540: 6020 7769 6c6c 206e 6f74 2062 6520 6368  ` will not be ch
-00001550: 616e 6765 642e 0a0a 3e20 4973 2074 6869  anged...> Is thi
-00001560: 7320 706c 7567 696e 2073 7461 626c 653f  s plugin stable?
-00001570: 0a0a 5468 6973 2070 6c75 6769 6e20 6973  ..This plugin is
-00001580: 2074 6573 7465 6420 6167 6169 6e73 7420   tested against 
-00001590: 6d75 6c74 6970 6c65 2076 6572 7369 6f6e  multiple version
-000015a0: 7320 6f66 2050 6f65 7472 7920 616e 6420  s of Poetry and 
-000015b0: 6861 7320 616e 2069 6e74 6567 7261 7469  has an integrati
-000015c0: 6f6e 2066 6f63 7573 6564 2074 6573 7420  on focused test 
-000015d0: 7375 6974 652e 2049 7420 6973 2073 6166  suite. It is saf
-000015e0: 6520 746f 2075 7365 2074 6869 7320 696e  e to use this in
-000015f0: 2070 726f 6475 6374 696f 6e2c 2074 686f   production, tho
-00001600: 7567 6820 6974 2069 7320 7265 636f 6d6d  ugh it is recomm
-00001610: 656e 6420 746f 2070 696e 2076 6572 7369  end to pin versi
-00001620: 6f6e 732e 2042 7265 616b 696e 6720 6368  ons. Breaking ch
-00001630: 616e 6765 7320 7769 6c6c 2062 6520 6176  anges will be av
-00001640: 6f69 6465 6420 756e 6c65 7373 2069 6e66  oided unless inf
-00001650: 6561 7369 626c 6520 6475 6520 746f 2075  easible due to u
-00001660: 7073 7472 6561 6d20 6368 616e 6765 7320  pstream changes 
-00001670: 696e 2050 6f65 7472 792e 0a0a 3e20 5769  in Poetry...> Wi
-00001680: 6c6c 2074 6869 7320 706c 7567 696e 2064  ll this plugin d
-00001690: 726f 7020 7468 6520 7570 7065 7220 626f  rop the upper bo
-000016a0: 756e 6420 6f6e 2050 7974 686f 6e20 6974  und on Python it
-000016b0: 7365 6c66 3f0a 0a42 656c 6965 7665 2069  self?..Believe i
-000016c0: 7420 6f72 206e 6f74 2c20 7468 6973 2069  t or not, this i
-000016d0: 7320 616e 2065 7665 6e20 6d6f 7265 2063  s an even more c
-000016e0: 6f6e 7465 6e74 696f 7573 2073 7562 7365  ontentious subse
-000016f0: 7420 6f66 2074 6869 7320 6973 7375 6520  t of this issue 
-00001700: 6173 2050 6f65 7472 7920 7769 6c6c 206e  as Poetry will n
-00001710: 6f74 2061 6c6c 6f77 2070 6163 6b61 6765  ot allow package
-00001720: 7320 7769 7468 206e 6f20 7570 7065 7220  s with no upper 
-00001730: 626f 756e 6420 6f6e 2050 7974 686f 6e20  bound on Python 
-00001740: 746f 2065 7869 7374 2061 6c6f 6e67 7369  to exist alongsi
-00001750: 6465 2074 686f 7365 2074 6861 7420 696e  de those that in
-00001760: 636c 7564 6520 6f6e 652e 2054 6869 7320  clude one. This 
-00001770: 6261 7369 6361 6c6c 7920 6d65 616e 7320  basically means 
-00001780: 7468 6174 2077 6520 6361 6e6e 6f74 2072  that we cannot r
-00001790: 656c 6178 2074 6869 7320 7265 7175 6972  elax this requir
-000017a0: 656d 656e 7420 7769 7468 6f75 7420 6272  ement without br
-000017b0: 6561 6b69 6e67 2074 6865 2076 6173 7420  eaking the vast 
-000017c0: 6d61 6a6f 7269 7479 206f 6620 7573 652d  majority of use-
-000017d0: 6361 7365 732e 2046 6f72 2074 6869 7320  cases. For this 
-000017e0: 7265 6173 6f6e 2c20 7765 2063 616e 6e6f  reason, we canno
-000017f0: 7420 7265 6c61 7820 6070 7974 686f 6e5e  t relax `python^
-00001800: 3360 2061 7420 7468 6973 2074 696d 652e  3` at this time.
-00001810: 2053 6565 205b 7468 6520 706f 7374 206f   See [the post o
-00001820: 6e20 7468 6520 506f 6574 7279 2064 6973  n the Poetry dis
-00001830: 6375 7373 696f 6e20 626f 6172 645d 2868  cussion board](h
-00001840: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001850: 6d2f 7079 7468 6f6e 2d70 6f65 7472 792f  m/python-poetry/
-00001860: 706f 6574 7279 2f64 6973 6375 7373 696f  poetry/discussio
-00001870: 6e73 2f33 3735 3723 6469 7363 7573 7369  ns/3757#discussi
-00001880: 6f6e 636f 6d6d 656e 742d 3433 3533 3435  oncomment-435345
-00001890: 2920 666f 7220 6d6f 7265 2064 6574 6169  ) for more detai
-000018a0: 6c73 2e0a 0a23 2320 436f 6e74 7269 6275  ls...## Contribu
-000018b0: 7469 6e67 0a0a 5468 6973 2070 726f 6a65  ting..This proje
-000018c0: 6374 2069 7320 6d61 6e61 6765 6420 7769  ct is managed wi
-000018d0: 7468 2050 6f65 7472 792e 2048 6572 6520  th Poetry. Here 
-000018e0: 6172 6520 7468 6520 6261 7369 6373 2066  are the basics f
-000018f0: 6f72 2067 6574 7469 6e67 2073 7461 7274  or getting start
-00001900: 6564 2e0a 0a43 6c6f 6e65 2074 6865 2072  ed...Clone the r
-00001910: 6570 6f73 6974 6f72 793a 0a60 6060 6261  epository:.```ba
-00001920: 7368 0a24 2067 6974 2063 6c6f 6e65 2068  sh.$ git clone h
-00001930: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001940: 6d2f 6d61 646b 696e 737a 2f70 6f65 7472  m/madkinsz/poetr
-00001950: 792d 7265 6c61 782e 6769 740a 2420 6364  y-relax.git.$ cd
-00001960: 2070 6f65 7472 792d 7265 6c61 780a 6060   poetry-relax.``
-00001970: 600a 0a49 6e73 7461 6c6c 2070 6163 6b61  `..Install packa
-00001980: 6765 733a 0a60 6060 6261 7368 0a24 2070  ges:.```bash.$ p
-00001990: 6f65 7472 7920 696e 7374 616c 6c0a 6060  oetry install.``
-000019a0: 600a 0a52 756e 2074 6865 2074 6573 7420  `..Run the test 
-000019b0: 7375 6974 653a 0a60 6060 6261 7368 0a24  suite:.```bash.$
-000019c0: 2070 7974 6573 7420 7465 7374 730a 6060   pytest tests.``
-000019d0: 600a 0a52 756e 206c 696e 7465 7273 2062  `..Run linters b
-000019e0: 6566 6f72 6520 6f70 656e 696e 6720 7075  efore opening pu
-000019f0: 6c6c 2072 6571 7565 7374 733a 0a60 6060  ll requests:.```
-00001a00: 6261 7368 0a24 202e 2f62 696e 2f6c 696e  bash.$ ./bin/lin
-00001a10: 7420 6368 6563 6b20 2e0a 2420 2e2f 6269  t check ..$ ./bi
-00001a20: 6e2f 6c69 6e74 2066 6978 202e 0a60 6060  n/lint fix ..```
-00001a30: 0a0a 2323 2052 6566 6572 656e 6365 730a  ..## References.
-00001a40: 0a54 6865 7265 2773 2061 206c 6f74 2074  .There's a lot t
-00001a50: 6f20 7265 6164 206f 6e20 7468 6973 2074  o read on this t
-00001a60: 6f70 6963 2120 4974 2773 2063 6f6e 7465  opic! It's conte
-00001a70: 6e74 696f 7573 2061 6e64 2063 6175 7369  ntious and causi
-00001a80: 6e67 2061 206c 6f74 206f 6620 7072 6f62  ng a lot of prob
-00001a90: 6c65 6d73 2066 6f72 206d 6169 6e74 6169  lems for maintai
-00001aa0: 6e65 7273 2061 6e64 2075 7365 7273 2e0a  ners and users..
-00001ab0: 0a54 6865 2066 6f6c 6c6f 7769 6e67 2062  .The following b
-00001ac0: 6c6f 6720 706f 7374 7320 6279 2048 656e  log posts by Hen
-00001ad0: 7279 2053 6368 7265 696e 6572 2061 7265  ry Schreiner are
-00001ae0: 2071 7569 7465 2063 6f6d 7072 6568 656e   quite comprehen
-00001af0: 7369 7665 3a0a 2d20 5b53 686f 756c 6420  sive:.- [Should 
-00001b00: 596f 7520 5573 6520 5570 7065 7220 426f  You Use Upper Bo
-00001b10: 756e 6420 5665 7273 696f 6e20 436f 6e73  und Version Cons
-00001b20: 7472 6169 6e74 733f 5d28 6874 7470 733a  traints?](https:
-00001b30: 2f2f 6973 6369 6e75 6d70 792e 6465 762f  //iscinumpy.dev/
-00001b40: 706f 7374 2f62 6f75 6e64 2d76 6572 7369  post/bound-versi
-00001b50: 6f6e 2d63 6f6e 7374 7261 696e 7473 2f29  on-constraints/)
-00001b60: 0a2d 205b 506f 6574 7279 2056 6572 7369  .- [Poetry Versi
-00001b70: 6f6e 735d 2868 7474 7073 3a2f 2f69 7363  ons](https://isc
-00001b80: 696e 756d 7079 2e64 6576 2f70 6f73 742f  inumpy.dev/post/
-00001b90: 706f 6574 7279 2d76 6572 7369 6f6e 732f  poetry-versions/
-00001ba0: 290a 0a43 6f6e 7465 6e74 2066 726f 6d20  )..Content from 
-00001bb0: 736f 6d65 206d 656d 6265 7273 206f 6620  some members of 
-00001bc0: 7468 6520 5079 7468 6f6e 2063 6f72 6520  the Python core 
-00001bd0: 6465 7665 6c6f 7065 7220 7465 616d 3a0a  developer team:.
-00001be0: 2d20 5b53 656d 616e 7469 6320 5665 7273  - [Semantic Vers
-00001bf0: 696f 6e69 6e67 2057 696c 6c20 4e6f 7420  ioning Will Not 
-00001c00: 5361 7665 2059 6f75 5d28 6874 7470 733a  Save You](https:
-00001c10: 2f2f 6879 6e65 6b2e 6d65 2f61 7274 6963  //hynek.me/artic
-00001c20: 6c65 732f 7365 6d76 6572 2d77 696c 6c2d  les/semver-will-
-00001c30: 6e6f 742d 7361 7665 2d79 6f75 2f29 0a2d  not-save-you/).-
-00001c40: 205b 5768 7920 4920 646f 6e27 7420 6c69   [Why I don't li
-00001c50: 6b65 2053 656d 5665 7220 616e 796d 6f72  ke SemVer anymor
-00001c60: 655d 2868 7474 7073 3a2f 2f73 6e61 726b  e](https://snark
-00001c70: 792e 6361 2f77 6879 2d69 2d64 6f6e 742d  y.ca/why-i-dont-
-00001c80: 6c69 6b65 2d73 656d 7665 722f 290a 2d20  like-semver/).- 
-00001c90: 5b56 6572 7369 6f6e 206e 756d 6265 7273  [Version numbers
-00001ca0: 3a20 686f 7720 746f 2075 7365 2074 6865  : how to use the
-00001cb0: 6d3f 5d28 6874 7470 733a 2f2f 6265 726e  m?](https://bern
-00001cc0: 6174 2e74 6563 682f 706f 7374 732f 7665  at.tech/posts/ve
-00001cd0: 7273 696f 6e2d 6e75 6d62 6572 732f 290a  rsion-numbers/).
-00001ce0: 2d20 5b56 6572 7369 6f6e 696e 6720 536f  - [Versioning So
-00001cf0: 6674 7761 7265 5d28 6874 7470 733a 2f2f  ftware](https://
-00001d00: 6361 7265 6d61 642e 696f 2f70 6f73 7473  caremad.io/posts
-00001d10: 2f32 3031 362f 3032 2f76 6572 7369 6f6e  /2016/02/version
-00001d20: 696e 672d 736f 6674 7761 7265 2f29 0a0a  ing-software/)..
-00001d30: 4469 7363 7573 7369 6f6e 2061 6e64 2069  Discussion and i
-00001d40: 7373 7565 7320 696e 2074 6865 2050 6f65  ssues in the Poe
-00001d50: 7472 7920 7072 6f6a 6563 743a 0a2d 205b  try project:.- [
-00001d60: 506c 6561 7365 2073 746f 7020 7069 6e6e  Please stop pinn
-00001d70: 696e 6720 746f 206d 616a 6f72 2076 6572  ing to major ver
-00001d80: 7369 6f6e 7320 6279 2064 6566 6175 6c74  sions by default
-00001d90: 2c20 6573 7065 6369 616c 6c79 2066 6f72  , especially for
-00001da0: 2050 7974 686f 6e20 6974 7365 6c66 5d28   Python itself](
-00001db0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001dc0: 6f6d 2f70 7974 686f 6e2d 706f 6574 7279  om/python-poetry
-00001dd0: 2f70 6f65 7472 792f 6973 7375 6573 2f33  /poetry/issues/3
-00001de0: 3734 3729 0a2d 205b 4368 616e 6765 2064  747).- [Change d
-00001df0: 6566 6175 6c74 2064 6570 656e 6465 6e63  efault dependenc
-00001e00: 7920 636f 6e73 7472 6169 6e74 2066 726f  y constraint fro
-00001e10: 6d20 5e20 746f 203e 3d5d 2868 7474 7073  m ^ to >=](https
-00001e20: 3a2f 2f67 6974 6875 622e 636f 6d2f 7079  ://github.com/py
-00001e30: 7468 6f6e 2d70 6f65 7472 792f 706f 6574  thon-poetry/poet
-00001e40: 7279 2f69 7373 7565 732f 3334 3237 290a  ry/issues/3427).
-00001e50: 2d20 5b44 6576 656c 6f70 6572 7320 7368  - [Developers sh
-00001e60: 6f75 6c64 2062 6520 6162 6c65 2074 6f20  ould be able to 
-00001e70: 7475 726e 206f 6666 2064 6570 656e 6465  turn off depende
-00001e80: 6e63 7920 7570 7065 722d 626f 756e 6420  ncy upper-bound 
-00001e90: 6361 6c63 756c 6174 696f 6e73 5d28 6874  calculations](ht
-00001ea0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001eb0: 2f70 7974 686f 6e2d 706f 6574 7279 2f70  /python-poetry/p
-00001ec0: 6f65 7472 792f 6973 7375 6573 2f32 3733  oetry/issues/273
-00001ed0: 3129 0a0a                                1)..
+00000370: 2e31 310a 436c 6173 7369 6669 6572 3a20  .11.Classifier: 
+00000380: 546f 7069 6320 3a3a 2053 6f66 7477 6172  Topic :: Softwar
+00000390: 6520 4465 7665 6c6f 706d 656e 740a 436c  e Development.Cl
+000003a0: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
+000003b0: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
+000003c0: 6c6f 706d 656e 7420 3a3a 204c 6962 7261  lopment :: Libra
+000003d0: 7269 6573 0a43 6c61 7373 6966 6965 723a  ries.Classifier:
+000003e0: 2054 7970 696e 6720 3a3a 2054 7970 6564   Typing :: Typed
+000003f0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000400: 706f 6574 7279 2028 3e3d 312e 3229 0a50  poetry (>=1.2).P
+00000410: 726f 6a65 6374 2d55 524c 3a20 5265 706f  roject-URL: Repo
+00000420: 7369 746f 7279 2c20 6874 7470 733a 2f2f  sitory, https://
+00000430: 6769 7468 7562 2e63 6f6d 2f6d 6164 6b69  github.com/madki
+00000440: 6e73 7a2f 706f 6574 7279 2d72 656c 6178  nsz/poetry-relax
+00000450: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
+00000460: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
+00000470: 6d61 726b 646f 776e 0a0a 3c70 2061 6c69  markdown..<p ali
+00000480: 676e 3d22 6365 6e74 6572 223e 0a20 2020  gn="center">.   
+00000490: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000004a0: 2f2f 7079 7069 2e70 7974 686f 6e2e 6f72  //pypi.python.or
+000004b0: 672f 7079 7069 2f70 6f65 7472 792d 7265  g/pypi/poetry-re
+000004c0: 6c61 782f 2220 616c 743d 224c 6174 6573  lax/" alt="Lates
+000004d0: 7420 7665 7273 696f 6e22 3e0a 2020 2020  t version">.    
+000004e0: 2020 2020 3c69 6d67 2061 6c74 3d22 4c61      <img alt="La
+000004f0: 7465 7374 2076 6572 7369 6f6e 2220 7372  test version" sr
+00000500: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000510: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
+00000520: 2f70 6f65 7472 792d 7265 6c61 783f 7374  /poetry-relax?st
+00000530: 796c 653d 666c 6174 2d73 7175 6172 6522  yle=flat-square"
+00000540: 3e0a 2020 2020 3c2f 613e 0a20 2020 203c  >.    </a>.    <
+00000550: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000560: 6465 7667 7569 6465 2e70 7974 686f 6e2e  devguide.python.
+00000570: 6f72 672f 7665 7273 696f 6e73 2f22 2061  org/versions/" a
+00000580: 6c74 3d22 5375 7070 6f72 7465 6420 5079  lt="Supported Py
+00000590: 7468 6f6e 2076 6572 7369 6f6e 7322 3e0a  thon versions">.
+000005a0: 2020 2020 2020 2020 3c69 6d67 2061 6c74          <img alt
+000005b0: 3d22 5375 7070 6f72 7465 6420 5079 7468  ="Supported Pyth
+000005c0: 6f6e 2076 6572 7369 6f6e 7322 2073 7263  on versions" src
+000005d0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+000005e0: 6965 6c64 732e 696f 2f70 7970 692f 7079  ields.io/pypi/py
+000005f0: 7665 7273 696f 6e73 2f70 6f65 7472 792d  versions/poetry-
+00000600: 7265 6c61 783f 7374 796c 653d 666c 6174  relax?style=flat
+00000610: 2d73 7175 6172 6522 3e0a 2020 2020 3c2f  -square">.    </
+00000620: 613e 0a20 2020 203c 6120 6872 6566 3d22  a>.    <a href="
+00000630: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000640: 6f6d 2f6d 6164 6b69 6e73 7a2f 706f 6574  om/madkinsz/poet
+00000650: 7279 2d72 656c 6178 2f61 6374 696f 6e73  ry-relax/actions
+00000660: 2f77 6f72 6b66 6c6f 7773 2f74 6573 742e  /workflows/test.
+00000670: 7961 6d6c 3f71 7565 7279 3d62 7261 6e63  yaml?query=branc
+00000680: 6825 3341 6d61 696e 2220 616c 743d 2254  h%3Amain" alt="T
+00000690: 6573 7420 7374 6174 7573 223e 0a20 2020  est status">.   
+000006a0: 2020 2020 203c 696d 6720 616c 743d 2254       <img alt="T
+000006b0: 6573 7420 7374 6174 7573 2220 7372 633d  est status" src=
+000006c0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+000006d0: 656c 6473 2e69 6f2f 6769 7468 7562 2f61  elds.io/github/a
+000006e0: 6374 696f 6e73 2f77 6f72 6b66 6c6f 772f  ctions/workflow/
+000006f0: 7374 6174 7573 2f6d 6164 6b69 6e73 7a2f  status/madkinsz/
+00000700: 706f 6574 7279 2d72 656c 6178 2f74 6573  poetry-relax/tes
+00000710: 742e 7961 6d6c 3f6c 6162 656c 3d74 6573  t.yaml?label=tes
+00000720: 7426 7374 796c 653d 666c 6174 2d73 7175  t&style=flat-squ
+00000730: 6172 6522 3e0a 2020 2020 3c2f 613e 0a20  are">.    </a>. 
+00000740: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
+00000750: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
+00000760: 6164 6b69 6e73 7a2f 706f 6574 7279 2d72  adkinsz/poetry-r
+00000770: 656c 6178 2f61 6374 696f 6e73 2f77 6f72  elax/actions/wor
+00000780: 6b66 6c6f 7773 2f62 7569 6c64 2e79 616d  kflows/build.yam
+00000790: 6c3f 7175 6572 793d 6272 616e 6368 2533  l?query=branch%3
+000007a0: 416d 6169 6e22 2061 6c74 3d22 4275 696c  Amain" alt="Buil
+000007b0: 6420 7374 6174 7573 223e 0a20 2020 2020  d status">.     
+000007c0: 2020 203c 696d 6720 616c 743d 2242 7569     <img alt="Bui
+000007d0: 6c64 2073 7461 7475 7322 2073 7263 3d22  ld status" src="
+000007e0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000007f0: 6c64 732e 696f 2f67 6974 6875 622f 6163  lds.io/github/ac
+00000800: 7469 6f6e 732f 776f 726b 666c 6f77 2f73  tions/workflow/s
+00000810: 7461 7475 732f 6d61 646b 696e 737a 2f70  tatus/madkinsz/p
+00000820: 6f65 7472 792d 7265 6c61 782f 6275 696c  oetry-relax/buil
+00000830: 642e 7961 6d6c 3f6c 6162 656c 3d62 7569  d.yaml?label=bui
+00000840: 6c64 2673 7479 6c65 3d66 6c61 742d 7371  ld&style=flat-sq
+00000850: 7561 7265 223e 0a20 2020 203c 2f61 3e0a  uare">.    </a>.
+00000860: 3c2f 703e 0a0a 2320 706f 6574 7279 2d72  </p>..# poetry-r
+00000870: 656c 6178 0a0a 4120 5b50 6f65 7472 795d  elax..A [Poetry]
+00000880: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000890: 636f 6d2f 7079 7468 6f6e 2d70 6f65 7472  com/python-poetr
+000008a0: 792f 706f 6574 7279 2920 706c 7567 696e  y/poetry) plugin
+000008b0: 2074 6f20 7265 6c61 7820 6465 7065 6e64   to relax depend
+000008c0: 656e 6379 2076 6572 7369 6f6e 7320 7768  ency versions wh
+000008d0: 656e 2070 7562 6c69 7368 696e 6720 6c69  en publishing li
+000008e0: 6272 6172 6965 732e 2052 656c 6178 2079  braries. Relax y
+000008f0: 6f75 7220 7072 6f6a 6563 7427 7320 6465  our project's de
+00000900: 7065 6e64 656e 6369 6573 2066 726f 6d20  pendencies from 
+00000910: 6066 6f6f 6261 725e 322e 302e 3060 2074  `foobar^2.0.0` t
+00000920: 6f20 6066 6f6f 6261 723e 3d32 2e30 2e30  o `foobar>=2.0.0
+00000930: 602e 0a0a 4279 2064 6566 6175 6c74 2c20  `...By default, 
+00000940: 506f 6574 7279 2075 7365 7320 6361 7265  Poetry uses care
+00000950: 7420 636f 6e73 7472 6169 6e74 7320 7768  t constraints wh
+00000960: 6963 6820 776f 756c 6420 6c69 6d69 7420  ich would limit 
+00000970: 6066 6f6f 6261 7260 2076 6572 7369 6f6e  `foobar` version
+00000980: 7320 746f 2060 3c33 2e30 602e 0a2a 2a70  s to `<3.0`..**p
+00000990: 6f65 7472 792d 7265 6c61 782a 2a20 2072  oetry-relax**  r
+000009a0: 656d 6f76 6573 2074 6865 7365 2075 7070  emoves these upp
+000009b0: 6572 2076 6572 7369 6f6e 2062 6f75 6e64  er version bound
+000009c0: 732c 2061 6c6c 6f77 696e 6720 6465 7065  s, allowing depe
+000009d0: 6e64 656e 6369 6573 2074 6f20 6265 2075  ndencies to be u
+000009e0: 7067 7261 6465 642e 0a0a 5265 6d6f 7669  pgraded...Removi
+000009f0: 6e67 2075 7070 6572 2076 6572 7369 6f6e  ng upper version
+00000a00: 2062 6f75 6e64 7320 6973 2069 6d70 6f72   bounds is impor
+00000a10: 7461 6e74 2077 6865 6e20 7075 626c 6973  tant when publis
+00000a20: 6869 6e67 206c 6962 7261 7269 6573 2e0a  hing libraries..
+00000a30: 5768 656e 2073 6561 7263 6869 6e67 2066  When searching f
+00000a40: 6f72 2076 6572 7369 6f6e 7320 6f66 2064  or versions of d
+00000a50: 6570 656e 6465 6e63 6965 7320 746f 2069  ependencies to i
+00000a60: 6e73 7461 6c6c 2c20 7468 6520 7265 736f  nstall, the reso
+00000a70: 6c76 6572 2028 652e 672e 2060 7069 7060  lver (e.g. `pip`
+00000a80: 2920 6d75 7374 2072 6573 7065 6374 2074  ) must respect t
+00000a90: 6865 2062 6f75 6e64 7320 796f 7572 206c  he bounds your l
+00000aa0: 6962 7261 7279 2073 7065 6369 6669 6573  ibrary specifies
+00000ab0: 2e0a 5768 656e 2061 206e 6577 2076 6572  ..When a new ver
+00000ac0: 7369 6f6e 206f 6620 7468 6520 6465 7065  sion of the depe
+00000ad0: 6e64 656e 6379 2069 7320 7265 6c65 6173  ndency is releas
+00000ae0: 6564 2c20 636f 6e73 756d 6572 7320 6f66  ed, consumers of
+00000af0: 2079 6f75 7220 6c69 6272 6172 7920 5f63   your library _c
+00000b00: 616e 6e6f 745f 2069 6e73 7461 6c6c 2069  annot_ install i
+00000b10: 7420 756e 6c65 7373 2061 206e 6577 2076  t unless a new v
+00000b20: 6572 7369 6f6e 206f 6620 796f 7572 206c  ersion of your l
+00000b30: 6962 7261 7279 2069 7320 616c 736f 2072  ibrary is also r
+00000b40: 656c 6561 7365 642e 0a0a 4974 2069 7320  eleased...It is 
+00000b50: 6e6f 7420 6665 6173 6962 6c65 2074 6f20  not feasible to 
+00000b60: 7265 6c65 6173 6520 7061 7463 6865 7320  release patches 
+00000b70: 666f 7220 6576 6572 7920 7072 6576 696f  for every previo
+00000b80: 7573 2076 6572 7369 6f6e 206f 6620 6d6f  us version of mo
+00000b90: 7374 206c 6962 7261 7269 6573 2c20 7768  st libraries, wh
+00000ba0: 6963 6820 666f 7263 6573 2075 7365 7273  ich forces users
+00000bb0: 2074 6f20 7573 6520 7468 6520 6d6f 7374   to use the most
+00000bc0: 2072 6563 656e 7420 7665 7273 696f 6e20   recent version 
+00000bd0: 6f66 2074 6865 206c 6962 7261 7279 206f  of the library o
+00000be0: 7220 6265 2073 7475 636b 2077 6974 686f  r be stuck witho
+00000bf0: 7574 2074 6865 206e 6577 2076 6572 7369  ut the new versi
+00000c00: 6f6e 206f 6620 7468 6520 6465 7065 6e64  on of the depend
+00000c10: 656e 6379 2e0a 5768 656e 206d 616e 7920  ency..When many 
+00000c20: 6c69 6272 6172 6965 7320 636f 6e74 6169  libraries contai
+00000c30: 6e20 7570 7065 7220 7665 7273 696f 6e20  n upper version 
+00000c40: 626f 756e 6473 2c20 7468 6520 6465 7065  bounds, the depe
+00000c50: 6e64 656e 6369 6573 2063 616e 2065 6173  ndencies can eas
+00000c60: 696c 7920 6265 636f 6d65 205f 756e 736f  ily become _unso
+00000c70: 6c76 6162 6c65 5f20 e280 9420 7768 6572  lvable_ ... wher
+00000c80: 6520 6c69 6272 6172 6965 7320 6861 7665  e libraries have
+00000c90: 2069 6e63 6f6d 7061 7469 626c 6520 6465   incompatible de
+00000ca0: 7065 6e64 656e 6379 2076 6572 7369 6f6e  pendency version
+00000cb0: 2072 6571 7569 7265 6d65 6e74 732e 0a42   requirements..B
+00000cc0: 7920 7265 6d6f 7669 6e67 2075 7070 6572  y removing upper
+00000cd0: 2076 6572 7369 6f6e 2062 6f75 6e64 7320   version bounds 
+00000ce0: 6672 6f6d 2079 6f75 7220 6c69 6272 6172  from your librar
+00000cf0: 792c 2063 6f6e 7472 6f6c 2069 7320 7265  y, control is re
+00000d00: 7475 726e 6564 2074 6f20 7468 6520 7573  turned to the us
+00000d10: 6572 2e0a 0a50 6f65 7472 7927 7320 6465  er...Poetry's de
+00000d20: 6661 756c 7420 6265 6861 7669 6f72 2069  fault behavior i
+00000d30: 7320 746f 2069 6e63 6c75 6465 2075 7070  s to include upp
+00000d40: 6572 2076 6572 7369 6f6e 2062 6f75 6e64  er version bound
+00000d50: 732e 204d 616e 7920 7065 6f70 6c65 2068  s. Many people h
+00000d60: 6176 6520 7370 6f6b 656e 2075 7020 6167  ave spoken up ag
+00000d70: 6169 6e73 7420 7468 6973 2073 7479 6c65  ainst this style
+00000d80: 206f 6620 6465 7065 6e64 656e 6379 206d   of dependency m
+00000d90: 616e 6167 656d 656e 7420 696e 2074 6865  anagement in the
+00000da0: 2050 7974 686f 6e20 6563 6f73 7973 7465   Python ecosyste
+00000db0: 6d2c 2069 6e63 6c75 6469 6e67 206d 656d  m, including mem
+00000dc0: 6265 7273 206f 6620 7468 6520 5079 7468  bers of the Pyth
+00000dd0: 6f6e 2063 6f72 6520 6465 7665 6c6f 706d  on core developm
+00000de0: 656e 7420 7465 616d 2e20 5365 6520 5b74  ent team. See [t
+00000df0: 6865 2062 6f74 746f 6d20 6f66 2074 6865  he bottom of the
+00000e00: 2072 6561 646d 655d 2823 7265 6665 7265   readme](#refere
+00000e10: 6e63 6573 2920 666f 7220 6c69 6e6b 7320  nces) for links 
+00000e20: 616e 6420 6164 6469 7469 6f6e 616c 2063  and additional c
+00000e30: 6f6e 7465 7874 2e0a 0a53 696e 6365 2074  ontext...Since t
+00000e40: 6865 2050 6f65 7472 7920 7072 6f6a 6563  he Poetry projec
+00000e50: 7420 7769 6c6c 206e 6f74 2061 6c6c 6f77  t will not allow
+00000e60: 2074 6869 7320 6265 6861 7669 6f72 2074   this behavior t
+00000e70: 6f20 6265 2063 6f6e 6669 6775 7265 642c  o be configured,
+00000e80: 206d 6169 6e74 6169 6e65 7273 2068 6176   maintainers hav
+00000e90: 6520 7265 736f 7274 6564 2074 6f20 6d61  e resorted to ma
+00000ea0: 6e75 616c 2065 6469 7469 6e67 206f 6620  nual editing of 
+00000eb0: 6465 7065 6e64 656e 6379 2063 6f6e 7374  dependency const
+00000ec0: 7261 696e 7473 2061 6674 6572 2061 6464  raints after add
+00000ed0: 696e 672e 202a 2a70 6f65 7472 792d 7265  ing. **poetry-re
+00000ee0: 6c61 782a 2a20 6169 6d73 2074 6f20 6175  lax** aims to au
+00000ef0: 746f 6d61 7465 2061 6e64 2073 696d 706c  tomate and simpl
+00000f00: 6966 7920 7468 6973 2070 726f 6365 7373  ify this process
+00000f10: 2e0a 0a2a 2a70 6f65 7472 792d 7265 6c61  ...**poetry-rela
+00000f20: 782a 2a20 7072 6f76 6964 6573 3a0a 2d20  x** provides:.- 
+00000f30: 4175 746f 6d61 7465 6420 7265 6d6f 7661  Automated remova
+00000f40: 6c20 6f66 2075 7070 6572 2062 6f75 6e64  l of upper bound
+00000f50: 2063 6f6e 7374 7261 696e 7473 2073 7065   constraints spe
+00000f60: 6369 6669 6564 2077 6974 6820 605e 600a  cified with `^`.
+00000f70: 2d20 5361 6665 7479 2063 6865 636b 2069  - Safety check i
+00000f80: 6620 7061 636b 6167 6520 7265 7175 6972  f package requir
+00000f90: 656d 656e 7473 2061 7265 2073 7469 6c6c  ements are still
+00000fa0: 2073 6f6c 7661 626c 6520 6166 7465 7220   solvable after 
+00000fb0: 7265 6c61 7869 6e67 2063 6f6e 7374 7261  relaxing constra
+00000fc0: 696e 7473 0a2d 2055 7067 7261 6465 206f  ints.- Upgrade o
+00000fd0: 6620 6465 7065 6e64 656e 6369 6573 2061  f dependencies a
+00000fe0: 6674 6572 2072 656c 6178 696e 6720 636f  fter relaxing co
+00000ff0: 6e73 7472 6169 6e74 730a 2d20 5570 6461  nstraints.- Upda
+00001000: 7465 206f 6620 7468 6520 6c6f 636b 2066  te of the lock f
+00001010: 696c 6520 7769 7468 6f75 7420 7570 6772  ile without upgr
+00001020: 6164 696e 6720 6465 7065 6e64 656e 6369  ading dependenci
+00001030: 6573 0a2d 204c 696d 6974 2064 6570 656e  es.- Limit depen
+00001040: 6465 6e63 7920 7265 6c61 7861 7469 6f6e  dency relaxation
+00001050: 2074 6f20 7370 6563 6966 6963 2064 6570   to specific dep
+00001060: 656e 6465 6e63 7920 6772 6f75 7073 0a2d  endency groups.-
+00001070: 2052 6574 656e 7469 6f6e 206f 6620 696e   Retention of in
+00001080: 7465 6e74 696f 6e61 6c20 7570 7065 7220  tentional upper 
+00001090: 626f 756e 6473 2069 6e64 6963 6174 696e  bounds indicatin
+000010a0: 6720 7472 7565 2069 6e63 6f6d 7061 7469  g true incompati
+000010b0: 6269 6c69 7469 6573 0a2d 2043 4c49 206d  bilities.- CLI m
+000010c0: 6573 7361 6765 7320 6465 7369 676e 6564  essages designed
+000010d0: 2074 6f20 6d61 7463 6820 506f 6574 7279   to match Poetry
+000010e0: 2773 206f 7574 7075 740a 0a23 2320 496e  's output..## In
+000010f0: 7374 616c 6c61 7469 6f6e 0a0a 5468 6520  stallation..The 
+00001100: 706c 7567 696e 206d 7573 7420 6265 2069  plugin must be i
+00001110: 6e73 7461 6c6c 6564 2069 6e20 506f 6574  nstalled in Poet
+00001120: 7279 2773 2065 6e76 6972 6f6e 6d65 6e74  ry's environment
+00001130: 2e20 5468 6973 2072 6571 7569 7265 7320  . This requires 
+00001140: 7573 6520 6f66 2074 6865 2020 6073 656c  use of the  `sel
+00001150: 6660 2073 7562 636f 6d6d 616e 642e 0a0a  f` subcommand...
+00001160: 6060 6062 6173 680a 2420 706f 6574 7279  ```bash.$ poetry
+00001170: 2073 656c 6620 6164 6420 706f 6574 7279   self add poetry
+00001180: 2d72 656c 6178 0a60 6060 0a0a 2323 2055  -relax.```..## U
+00001190: 7361 6765 0a0a 5265 6c61 7820 636f 6e73  sage..Relax cons
+000011a0: 7472 6169 6e74 7320 666f 7220 7768 6963  traints for whic
+000011b0: 6820 506f 6574 7279 2073 6574 2061 6e20  h Poetry set an 
+000011c0: 7570 7065 7220 7665 7273 696f 6e3a 0a0a  upper version:..
+000011d0: 6060 6062 6173 680a 2420 706f 6574 7279  ```bash.$ poetry
+000011e0: 2072 656c 6178 0a60 6060 0a0a 5265 6c61   relax.```..Rela
+000011f0: 7820 636f 6e73 7472 6169 6e74 7320 616e  x constraints an
+00001200: 6420 6368 6563 6b20 7468 6174 2074 6865  d check that the
+00001210: 7920 6172 6520 7265 736f 6c76 6162 6c65  y are resolvable
+00001220: 2077 6974 686f 7574 2070 6572 666f 726d   without perform
+00001230: 696e 6720 7570 6772 6164 6573 3a0a 0a60  ing upgrades:..`
+00001240: 6060 6261 7368 0a24 2070 6f65 7472 7920  ``bash.$ poetry 
+00001250: 7265 6c61 7820 2d2d 6368 6563 6b0a 6060  relax --check.``
+00001260: 600a 0a52 656c 6178 2063 6f6e 7374 7261  `..Relax constra
+00001270: 696e 7473 2061 6e64 2075 7067 7261 6465  ints and upgrade
+00001280: 2070 6163 6b61 6765 733a 0a0a 6060 6062   packages:..```b
+00001290: 6173 680a 2420 706f 6574 7279 2072 656c  ash.$ poetry rel
+000012a0: 6178 202d 2d75 7064 6174 650a 6060 600a  ax --update.```.
+000012b0: 0a52 656c 6178 2063 6f6e 7374 7261 696e  .Relax constrain
+000012c0: 7473 2061 6e64 2075 7064 6174 6520 7468  ts and update th
+000012d0: 6520 6c6f 636b 2066 696c 6520 7769 7468  e lock file with
+000012e0: 6f75 7420 7570 6772 6164 696e 6720 7061  out upgrading pa
+000012f0: 636b 6167 6573 3a0a 0a60 6060 6261 7368  ckages:..```bash
+00001300: 0a24 2070 6f65 7472 7920 7265 6c61 7820  .$ poetry relax 
+00001310: 2d2d 6c6f 636b 0a60 6060 0a0a 5072 6576  --lock.```..Prev
+00001320: 6965 7720 7468 6520 6368 616e 6765 7320  iew the changes 
+00001330: 6070 6f65 7472 7920 7265 6c61 7860 2077  `poetry relax` w
+00001340: 6f75 6c64 206d 616b 6520 7769 7468 6f75  ould make withou
+00001350: 7420 6d6f 6469 6679 696e 6720 7468 6520  t modifying the 
+00001360: 7072 6f6a 6563 743a 0a0a 6060 6062 6173  project:..```bas
+00001370: 680a 2420 706f 6574 7279 2072 656c 6178  h.$ poetry relax
+00001380: 202d 2d64 7279 2d72 756e 0a60 6060 0a0a   --dry-run.```..
+00001390: 5265 6c61 7820 636f 6e73 7472 6169 6e74  Relax constraint
+000013a0: 7320 666f 7220 7370 6563 6966 6963 2064  s for specific d
+000013b0: 6570 656e 6465 6e63 7920 6772 6f75 7073  ependency groups
+000013c0: 3a0a 0a60 6060 6261 7368 0a24 2070 6f65  :..```bash.$ poe
+000013d0: 7472 7920 7265 6c61 7820 2d2d 6f6e 6c79  try relax --only
+000013e0: 2066 6f6f 202d 2d6f 6e6c 7920 6261 720a   foo --only bar.
+000013f0: 6060 600a 0a52 656c 6178 2063 6f6e 7374  ```..Relax const
+00001400: 7261 696e 7473 2065 7863 6c75 6469 6e67  raints excluding
+00001410: 2073 7065 6369 6669 6320 6465 7065 6e64   specific depend
+00001420: 656e 6379 2067 726f 7570 733a 0a0a 6060  ency groups:..``
+00001430: 6062 6173 680a 2420 706f 6574 7279 2072  `bash.$ poetry r
+00001440: 656c 6178 202d 2d77 6974 686f 7574 2066  elax --without f
+00001450: 6f6f 202d 2d77 6974 686f 7574 2062 6172  oo --without bar
+00001460: 0a60 6060 0a0a 0a23 2320 4578 616d 706c  .```...## Exampl
+00001470: 6573 0a0a 5468 6520 6265 6861 7669 6f72  es..The behavior
+00001480: 206f 6620 506f 6574 7279 2069 7320 7175   of Poetry is qu
+00001490: 6974 6520 7265 6173 6f6e 6162 6c65 2066  ite reasonable f
+000014a0: 6f72 206c 6f63 616c 2064 6576 656c 6f70  or local develop
+000014b0: 6d65 6e74 2120 6070 6f65 7472 7920 7265  ment! `poetry re
+000014c0: 6c61 7860 2069 7320 6d6f 7374 2075 7365  lax` is most use
+000014d0: 6675 6c20 7768 656e 2075 7365 6420 696e  ful when used in
+000014e0: 2043 492f 4344 2070 6970 656c 696e 6573   CI/CD pipelines
+000014f0: 2e0a 0a23 2323 2052 656c 6178 696e 6720  ...### Relaxing 
+00001500: 7265 7175 6972 656d 656e 7473 2062 6566  requirements bef
+00001510: 6f72 6520 7075 626c 6973 6869 6e67 0a0a  ore publishing..
+00001520: 5275 6e20 6070 6f65 7472 7920 7265 6c61  Run `poetry rela
+00001530: 7860 2062 6566 6f72 6520 6275 696c 6469  x` before buildi
+00001540: 6e67 2061 6e64 2070 7562 6c69 7368 696e  ng and publishin
+00001550: 6720 6120 7061 636b 6167 652e 0a0a 5365  g a package...Se
+00001560: 6520 6974 2061 7420 776f 726b 2069 6e20  e it at work in 
+00001570: 5b74 6865 2072 656c 6561 7365 2077 6f72  [the release wor
+00001580: 6b66 6c6f 7720 666f 7220 7468 6973 2070  kflow for this p
+00001590: 726f 6a65 6374 5d28 6874 7470 733a 2f2f  roject](https://
+000015a0: 6769 7468 7562 2e63 6f6d 2f6d 6164 6b69  github.com/madki
+000015b0: 6e73 7a2f 706f 6574 7279 2d72 656c 6178  nsz/poetry-relax
+000015c0: 2f62 6c6f 622f 6d61 696e 2f2e 6769 7468  /blob/main/.gith
+000015d0: 7562 2f77 6f72 6b66 6c6f 7773 2f72 656c  ub/workflows/rel
+000015e0: 6561 7365 2e79 616d 6c29 2e0a 0a0a 2323  ease.yaml)....##
+000015f0: 2320 5265 6c61 7869 6e67 2072 6571 7569  # Relaxing requi
+00001600: 7265 6d65 6e74 7320 666f 7220 7465 7374  rements for test
+00001610: 696e 670a 0a52 756e 2060 706f 6574 7279  ing..Run `poetry
+00001620: 2072 656c 6178 202d 2d75 7064 6174 6560   relax --update`
+00001630: 2062 6566 6f72 6520 7465 7374 7320 746f   before tests to
+00001640: 2074 6573 7420 6167 6169 6e73 7420 7468   test against th
+00001650: 6520 6e65 7765 7374 2070 6f73 7369 626c  e newest possibl
+00001660: 6520 7665 7273 696f 6e73 206f 6620 7061  e versions of pa
+00001670: 636b 6167 6573 2e0a 0a53 6565 2069 7420  ckages...See it 
+00001680: 6174 2077 6f72 6b20 696e 205b 7468 6520  at work in [the 
+00001690: 7465 7374 2077 6f72 6b66 6c6f 7720 666f  test workflow fo
+000016a0: 7220 7468 6973 2070 726f 6a65 6374 5d28  r this project](
+000016b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000016c0: 6f6d 2f6d 6164 6b69 6e73 7a2f 706f 6574  om/madkinsz/poet
+000016d0: 7279 2d72 656c 6178 2f62 6c6f 622f 6d61  ry-relax/blob/ma
+000016e0: 696e 2f2e 6769 7468 7562 2f77 6f72 6b66  in/.github/workf
+000016f0: 6c6f 7773 2f74 6573 742e 7961 6d6c 292e  lows/test.yaml).
+00001700: 0a0a 2323 2046 7265 7175 656e 746c 7920  ..## Frequently 
+00001710: 6173 6b65 6420 7175 6573 7469 6f6e 730a  asked questions.
+00001720: 0a3e 2043 616e 2074 6869 7320 706c 7567  .> Can this plug
+00001730: 696e 2063 6861 6e67 6520 7468 6520 6265  in change the be
+00001740: 6861 7669 6f72 206f 6620 6070 6f65 7472  havior of `poetr
+00001750: 7920 6164 6460 2074 6f20 7265 6c61 7820  y add` to relax 
+00001760: 636f 6e73 7472 6169 6e74 733f 0a0a 4e6f  constraints?..No
+00001770: 7420 6174 2074 6869 7320 7469 6d65 2e20  t at this time. 
+00001780: 5468 6520 506f 6574 7279 2070 726f 6a65  The Poetry proje
+00001790: 6374 2073 7461 7465 7320 7468 6174 2070  ct states that p
+000017a0: 6c75 6769 6e73 206d 7573 7420 6e6f 7420  lugins must not 
+000017b0: 616c 7465 7220 7468 6520 6265 6861 7669  alter the behavi
+000017c0: 6f72 206f 6620 636f 7265 2050 6f65 7472  or of core Poetr
+000017d0: 7920 636f 6d6d 616e 6473 2e20 4966 2074  y commands. If t
+000017e0: 6869 7320 6265 6861 7669 6f72 2077 6f75  his behavior wou
+000017f0: 6c64 2062 6520 7573 6566 756c 2066 6f72  ld be useful for
+00001800: 2079 6f75 2c20 706c 6561 7365 2063 6869   you, please chi
+00001810: 6d65 2069 6e20 5b6f 6e20 7468 6520 7472  me in [on the tr
+00001820: 6163 6b69 6e67 2069 7373 7565 5d28 6874  acking issue](ht
+00001830: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001840: 2f6d 6164 6b69 6e73 7a2f 706f 6574 7279  /madkinsz/poetry
+00001850: 2d72 656c 6178 2f69 7373 7565 732f 3529  -relax/issues/5)
+00001860: 2e0a 0a3e 2044 6f65 7320 7468 6973 2070  ...> Does this p
+00001870: 6c75 6769 6e20 7265 6d6f 7665 2075 7070  lugin remove upp
+00001880: 6572 2063 6f6e 7374 7261 696e 7473 2049  er constraints I
+00001890: 2776 6520 6164 6465 643f 0a0a 5468 6973  've added?..This
+000018a0: 2070 6c75 6769 6e20 7769 6c6c 206f 6e6c   plugin will onl
+000018b0: 7920 7265 6c61 7820 636f 6e73 7472 6169  y relax constrai
+000018c0: 6e74 7320 7370 6563 6966 6965 6420 7769  nts specified wi
+000018d0: 7468 2061 2063 6172 6574 2028 605e 6029  th a caret (`^`)
+000018e0: 2e20 5570 7065 7220 636f 6e73 7472 6169  . Upper constrai
+000018f0: 6e74 7320 6164 6465 6420 7769 7468 2060  nts added with `
+00001900: 3c60 2061 6e64 2060 3c3d 6020 7769 6c6c  <` and `<=` will
+00001910: 206e 6f74 2062 6520 6368 616e 6765 642e   not be changed.
+00001920: 0a0a 3e20 4973 2074 6869 7320 706c 7567  ..> Is this plug
+00001930: 696e 2073 7461 626c 653f 0a0a 5468 6973  in stable?..This
+00001940: 2070 6c75 6769 6e20 6973 2074 6573 7465   plugin is teste
+00001950: 6420 6167 6169 6e73 7420 6d75 6c74 6970  d against multip
+00001960: 6c65 2076 6572 7369 6f6e 7320 6f66 2050  le versions of P
+00001970: 6f65 7472 7920 616e 6420 6861 7320 616e  oetry and has an
+00001980: 2069 6e74 6567 7261 7469 6f6e 2066 6f63   integration foc
+00001990: 7573 6564 2074 6573 7420 7375 6974 652e  used test suite.
+000019a0: 2049 7420 6973 2073 6166 6520 746f 2075   It is safe to u
+000019b0: 7365 2074 6869 7320 696e 2070 726f 6475  se this in produ
+000019c0: 6374 696f 6e2c 2074 686f 7567 6820 6974  ction, though it
+000019d0: 2069 7320 7265 636f 6d6d 656e 6420 746f   is recommend to
+000019e0: 2070 696e 2076 6572 7369 6f6e 732e 2042   pin versions. B
+000019f0: 7265 616b 696e 6720 6368 616e 6765 7320  reaking changes 
+00001a00: 7769 6c6c 2062 6520 6176 6f69 6465 6420  will be avoided 
+00001a10: 756e 6c65 7373 2069 6e66 6561 7369 626c  unless infeasibl
+00001a20: 6520 6475 6520 746f 2075 7073 7472 6561  e due to upstrea
+00001a30: 6d20 6368 616e 6765 7320 696e 2050 6f65  m changes in Poe
+00001a40: 7472 792e 0a0a 3e20 5769 6c6c 2074 6869  try...> Will thi
+00001a50: 7320 706c 7567 696e 2064 726f 7020 7468  s plugin drop th
+00001a60: 6520 7570 7065 7220 626f 756e 6420 6f6e  e upper bound on
+00001a70: 2050 7974 686f 6e20 6974 7365 6c66 3f0a   Python itself?.
+00001a80: 0a42 656c 6965 7665 2069 7420 6f72 206e  .Believe it or n
+00001a90: 6f74 2c20 7468 6973 2069 7320 616e 2065  ot, this is an e
+00001aa0: 7665 6e20 6d6f 7265 2063 6f6e 7465 6e74  ven more content
+00001ab0: 696f 7573 2073 7562 7365 7420 6f66 2074  ious subset of t
+00001ac0: 6869 7320 6973 7375 6520 6173 2050 6f65  his issue as Poe
+00001ad0: 7472 7920 7769 6c6c 206e 6f74 2061 6c6c  try will not all
+00001ae0: 6f77 2070 6163 6b61 6765 7320 7769 7468  ow packages with
+00001af0: 206e 6f20 7570 7065 7220 626f 756e 6420   no upper bound 
+00001b00: 6f6e 2050 7974 686f 6e20 746f 2065 7869  on Python to exi
+00001b10: 7374 2061 6c6f 6e67 7369 6465 2074 686f  st alongside tho
+00001b20: 7365 2074 6861 7420 696e 636c 7564 6520  se that include 
+00001b30: 6f6e 652e 2054 6869 7320 6261 7369 6361  one. This basica
+00001b40: 6c6c 7920 6d65 616e 7320 7468 6174 2077  lly means that w
+00001b50: 6520 6361 6e6e 6f74 2072 656c 6178 2074  e cannot relax t
+00001b60: 6869 7320 7265 7175 6972 656d 656e 7420  his requirement 
+00001b70: 7769 7468 6f75 7420 6272 6561 6b69 6e67  without breaking
+00001b80: 2074 6865 2076 6173 7420 6d61 6a6f 7269   the vast majori
+00001b90: 7479 206f 6620 7573 652d 6361 7365 732e  ty of use-cases.
+00001ba0: 2046 6f72 2074 6869 7320 7265 6173 6f6e   For this reason
+00001bb0: 2c20 7765 2063 616e 6e6f 7420 7265 6c61  , we cannot rela
+00001bc0: 7820 6070 7974 686f 6e5e 3360 2061 7420  x `python^3` at 
+00001bd0: 7468 6973 2074 696d 652e 2053 6565 205b  this time. See [
+00001be0: 7468 6520 706f 7374 206f 6e20 7468 6520  the post on the 
+00001bf0: 506f 6574 7279 2064 6973 6375 7373 696f  Poetry discussio
+00001c00: 6e20 626f 6172 645d 2868 7474 7073 3a2f  n board](https:/
+00001c10: 2f67 6974 6875 622e 636f 6d2f 7079 7468  /github.com/pyth
+00001c20: 6f6e 2d70 6f65 7472 792f 706f 6574 7279  on-poetry/poetry
+00001c30: 2f64 6973 6375 7373 696f 6e73 2f33 3735  /discussions/375
+00001c40: 3723 6469 7363 7573 7369 6f6e 636f 6d6d  7#discussioncomm
+00001c50: 656e 742d 3433 3533 3435 2920 666f 7220  ent-435345) for 
+00001c60: 6d6f 7265 2064 6574 6169 6c73 2e0a 0a23  more details...#
+00001c70: 2320 436f 6e74 7269 6275 7469 6e67 0a0a  # Contributing..
+00001c80: 5468 6973 2070 726f 6a65 6374 2069 7320  This project is 
+00001c90: 6d61 6e61 6765 6420 7769 7468 2050 6f65  managed with Poe
+00001ca0: 7472 792e 2048 6572 6520 6172 6520 7468  try. Here are th
+00001cb0: 6520 6261 7369 6373 2066 6f72 2067 6574  e basics for get
+00001cc0: 7469 6e67 2073 7461 7274 6564 2e0a 0a43  ting started...C
+00001cd0: 6c6f 6e65 2074 6865 2072 6570 6f73 6974  lone the reposit
+00001ce0: 6f72 793a 0a60 6060 6261 7368 0a24 2067  ory:.```bash.$ g
+00001cf0: 6974 2063 6c6f 6e65 2068 7474 7073 3a2f  it clone https:/
+00001d00: 2f67 6974 6875 622e 636f 6d2f 6d61 646b  /github.com/madk
+00001d10: 696e 737a 2f70 6f65 7472 792d 7265 6c61  insz/poetry-rela
+00001d20: 782e 6769 740a 2420 6364 2070 6f65 7472  x.git.$ cd poetr
+00001d30: 792d 7265 6c61 780a 6060 600a 0a49 6e73  y-relax.```..Ins
+00001d40: 7461 6c6c 2070 6163 6b61 6765 733a 0a60  tall packages:.`
+00001d50: 6060 6261 7368 0a24 2070 6f65 7472 7920  ``bash.$ poetry 
+00001d60: 696e 7374 616c 6c0a 6060 600a 0a52 756e  install.```..Run
+00001d70: 2074 6865 2074 6573 7420 7375 6974 653a   the test suite:
+00001d80: 0a60 6060 6261 7368 0a24 2070 7974 6573  .```bash.$ pytes
+00001d90: 7420 7465 7374 730a 6060 600a 0a52 756e  t tests.```..Run
+00001da0: 206c 696e 7465 7273 2062 6566 6f72 6520   linters before 
+00001db0: 6f70 656e 696e 6720 7075 6c6c 2072 6571  opening pull req
+00001dc0: 7565 7374 733a 0a60 6060 6261 7368 0a24  uests:.```bash.$
+00001dd0: 202e 2f62 696e 2f6c 696e 7420 6368 6563   ./bin/lint chec
+00001de0: 6b20 2e0a 2420 2e2f 6269 6e2f 6c69 6e74  k ..$ ./bin/lint
+00001df0: 2066 6978 202e 0a60 6060 0a0a 2323 2052   fix ..```..## R
+00001e00: 6566 6572 656e 6365 730a 0a54 6865 7265  eferences..There
+00001e10: 2773 2061 206c 6f74 2074 6f20 7265 6164  's a lot to read
+00001e20: 206f 6e20 7468 6973 2074 6f70 6963 2120   on this topic! 
+00001e30: 4974 2773 2063 6f6e 7465 6e74 696f 7573  It's contentious
+00001e40: 2061 6e64 2063 6175 7369 6e67 2061 206c   and causing a l
+00001e50: 6f74 206f 6620 7072 6f62 6c65 6d73 2066  ot of problems f
+00001e60: 6f72 206d 6169 6e74 6169 6e65 7273 2061  or maintainers a
+00001e70: 6e64 2075 7365 7273 2e0a 0a54 6865 2066  nd users...The f
+00001e80: 6f6c 6c6f 7769 6e67 2062 6c6f 6720 706f  ollowing blog po
+00001e90: 7374 7320 6279 2048 656e 7279 2053 6368  sts by Henry Sch
+00001ea0: 7265 696e 6572 2061 7265 2071 7569 7465  reiner are quite
+00001eb0: 2063 6f6d 7072 6568 656e 7369 7665 3a0a   comprehensive:.
+00001ec0: 2d20 5b53 686f 756c 6420 596f 7520 5573  - [Should You Us
+00001ed0: 6520 5570 7065 7220 426f 756e 6420 5665  e Upper Bound Ve
+00001ee0: 7273 696f 6e20 436f 6e73 7472 6169 6e74  rsion Constraint
+00001ef0: 733f 5d28 6874 7470 733a 2f2f 6973 6369  s?](https://isci
+00001f00: 6e75 6d70 792e 6465 762f 706f 7374 2f62  numpy.dev/post/b
+00001f10: 6f75 6e64 2d76 6572 7369 6f6e 2d63 6f6e  ound-version-con
+00001f20: 7374 7261 696e 7473 2f29 0a2d 205b 506f  straints/).- [Po
+00001f30: 6574 7279 2056 6572 7369 6f6e 735d 2868  etry Versions](h
+00001f40: 7474 7073 3a2f 2f69 7363 696e 756d 7079  ttps://iscinumpy
+00001f50: 2e64 6576 2f70 6f73 742f 706f 6574 7279  .dev/post/poetry
+00001f60: 2d76 6572 7369 6f6e 732f 290a 0a43 6f6e  -versions/)..Con
+00001f70: 7465 6e74 2066 726f 6d20 736f 6d65 206d  tent from some m
+00001f80: 656d 6265 7273 206f 6620 7468 6520 5079  embers of the Py
+00001f90: 7468 6f6e 2063 6f72 6520 6465 7665 6c6f  thon core develo
+00001fa0: 7065 7220 7465 616d 3a0a 2d20 5b53 656d  per team:.- [Sem
+00001fb0: 616e 7469 6320 5665 7273 696f 6e69 6e67  antic Versioning
+00001fc0: 2057 696c 6c20 4e6f 7420 5361 7665 2059   Will Not Save Y
+00001fd0: 6f75 5d28 6874 7470 733a 2f2f 6879 6e65  ou](https://hyne
+00001fe0: 6b2e 6d65 2f61 7274 6963 6c65 732f 7365  k.me/articles/se
+00001ff0: 6d76 6572 2d77 696c 6c2d 6e6f 742d 7361  mver-will-not-sa
+00002000: 7665 2d79 6f75 2f29 0a2d 205b 5768 7920  ve-you/).- [Why 
+00002010: 4920 646f 6e27 7420 6c69 6b65 2053 656d  I don't like Sem
+00002020: 5665 7220 616e 796d 6f72 655d 2868 7474  Ver anymore](htt
+00002030: 7073 3a2f 2f73 6e61 726b 792e 6361 2f77  ps://snarky.ca/w
+00002040: 6879 2d69 2d64 6f6e 742d 6c69 6b65 2d73  hy-i-dont-like-s
+00002050: 656d 7665 722f 290a 2d20 5b56 6572 7369  emver/).- [Versi
+00002060: 6f6e 206e 756d 6265 7273 3a20 686f 7720  on numbers: how 
+00002070: 746f 2075 7365 2074 6865 6d3f 5d28 6874  to use them?](ht
+00002080: 7470 733a 2f2f 6265 726e 6174 2e74 6563  tps://bernat.tec
+00002090: 682f 706f 7374 732f 7665 7273 696f 6e2d  h/posts/version-
+000020a0: 6e75 6d62 6572 732f 290a 2d20 5b56 6572  numbers/).- [Ver
+000020b0: 7369 6f6e 696e 6720 536f 6674 7761 7265  sioning Software
+000020c0: 5d28 6874 7470 733a 2f2f 6361 7265 6d61  ](https://carema
+000020d0: 642e 696f 2f70 6f73 7473 2f32 3031 362f  d.io/posts/2016/
+000020e0: 3032 2f76 6572 7369 6f6e 696e 672d 736f  02/versioning-so
+000020f0: 6674 7761 7265 2f29 0a0a 4469 7363 7573  ftware/)..Discus
+00002100: 7369 6f6e 2061 6e64 2069 7373 7565 7320  sion and issues 
+00002110: 696e 2074 6865 2050 6f65 7472 7920 7072  in the Poetry pr
+00002120: 6f6a 6563 743a 0a2d 205b 506c 6561 7365  oject:.- [Please
+00002130: 2073 746f 7020 7069 6e6e 696e 6720 746f   stop pinning to
+00002140: 206d 616a 6f72 2076 6572 7369 6f6e 7320   major versions 
+00002150: 6279 2064 6566 6175 6c74 2c20 6573 7065  by default, espe
+00002160: 6369 616c 6c79 2066 6f72 2050 7974 686f  cially for Pytho
+00002170: 6e20 6974 7365 6c66 5d28 6874 7470 733a  n itself](https:
+00002180: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7974  //github.com/pyt
+00002190: 686f 6e2d 706f 6574 7279 2f70 6f65 7472  hon-poetry/poetr
+000021a0: 792f 6973 7375 6573 2f33 3734 3729 0a2d  y/issues/3747).-
+000021b0: 205b 4368 616e 6765 2064 6566 6175 6c74   [Change default
+000021c0: 2064 6570 656e 6465 6e63 7920 636f 6e73   dependency cons
+000021d0: 7472 6169 6e74 2066 726f 6d20 5e20 746f  traint from ^ to
+000021e0: 203e 3d5d 2868 7474 7073 3a2f 2f67 6974   >=](https://git
+000021f0: 6875 622e 636f 6d2f 7079 7468 6f6e 2d70  hub.com/python-p
+00002200: 6f65 7472 792f 706f 6574 7279 2f69 7373  oetry/poetry/iss
+00002210: 7565 732f 3334 3237 290a 2d20 5b44 6576  ues/3427).- [Dev
+00002220: 656c 6f70 6572 7320 7368 6f75 6c64 2062  elopers should b
+00002230: 6520 6162 6c65 2074 6f20 7475 726e 206f  e able to turn o
+00002240: 6666 2064 6570 656e 6465 6e63 7920 7570  ff dependency up
+00002250: 7065 722d 626f 756e 6420 6361 6c63 756c  per-bound calcul
+00002260: 6174 696f 6e73 5d28 6874 7470 733a 2f2f  ations](https://
+00002270: 6769 7468 7562 2e63 6f6d 2f70 7974 686f  github.com/pytho
+00002280: 6e2d 706f 6574 7279 2f70 6f65 7472 792f  n-poetry/poetry/
+00002290: 6973 7375 6573 2f32 3733 3129 0a0a       issues/2731)..
```

