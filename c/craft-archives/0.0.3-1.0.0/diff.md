# Comparing `tmp/craft-archives-0.0.3.tar.gz` & `tmp/craft-archives-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft-archives-0.0.3.tar", last modified: Thu Mar 23 17:48:46 2023, max compression
+gzip compressed data, was "craft-archives-1.0.0.tar", last modified: Wed May 24 18:13:32 2023, max compression
```

## Comparing `craft-archives-0.0.3.tar` & `craft-archives-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:48:46.826116 craft-archives-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-03-23 17:48:20.000000 craft-archives-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-23 17:48:46.826116 craft-archives-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-23 17:48:20.000000 craft-archives-0.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:48:46.822116 craft-archives-0.0.3/craft_archives/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-23 17:48:20.000000 craft-archives-0.0.3/craft_archives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-23 17:48:20.000000 craft-archives-0.0.3/craft_archives/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-03-23 17:48:20.000000 craft-archives-0.0.3/craft_archives/os_release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:48:46.826116 craft-archives-0.0.3/craft_archives/repo/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-23 17:48:20.000000 craft-archives-0.0.3/craft_archives/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-03-23 17:48:20.000000 craft-archives-0.0.3/craft_archives/repo/apt_key_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-03-23 17:48:20.000000 craft-archives-0.0.3/craft_archives/repo/apt_ppa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-03-23 17:48:20.000000 craft-archives-0.0.3/craft_archives/repo/apt_preferences_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-03-23 17:48:20.000000 craft-archives-0.0.3/craft_archives/repo/apt_sources_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-03-23 17:48:20.000000 craft-archives-0.0.3/craft_archives/repo/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-03-23 17:48:20.000000 craft-archives-0.0.3/craft_archives/repo/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22565 2023-03-23 17:48:20.000000 craft-archives-0.0.3/craft_archives/repo/package_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-03-23 17:48:20.000000 craft-archives-0.0.3/craft_archives/repo/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-03-23 17:48:20.000000 craft-archives-0.0.3/craft_archives/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:48:46.826116 craft-archives-0.0.3/craft_archives.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-23 17:48:46.000000 craft-archives-0.0.3/craft_archives.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-03-23 17:48:46.000000 craft-archives-0.0.3/craft_archives.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 17:48:46.000000 craft-archives-0.0.3/craft_archives.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-23 17:48:46.000000 craft-archives-0.0.3/craft_archives.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-23 17:48:46.000000 craft-archives-0.0.3/craft_archives.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-03-23 17:48:20.000000 craft-archives-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 17:48:46.826116 craft-archives-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.593578 craft-archives-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.codespell_ignore_lines
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.585578 craft-archives-1.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.github/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.github/renovate.json5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.585578 craft-archives-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.github/workflows/cla-check.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.github/workflows/release-drafter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.github/workflows/release-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.yamlignore
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-24 18:13:15.000000 craft-archives-1.0.0/HACKING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-24 18:13:15.000000 craft-archives-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-24 18:13:32.593578 craft-archives-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-24 18:13:15.000000 craft-archives-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.585578 craft-archives-1.0.0/craft_archives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 18:13:32.000000 craft-archives-1.0.0/craft_archives/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.585578 craft-archives-1.0.0/craft_archives/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/repo/apt_key_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/repo/apt_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/repo/apt_preferences_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/repo/apt_sources_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/repo/apt_uca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/repo/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/repo/installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/repo/package_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/repo/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.585578 craft-archives-1.0.0/craft_archives.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-24 18:13:32.000000 craft-archives-1.0.0/craft_archives.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-24 18:13:32.000000 craft-archives-1.0.0/craft_archives.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:13:32.000000 craft-archives-1.0.0/craft_archives.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-24 18:13:32.000000 craft-archives-1.0.0/craft_archives.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 18:13:32.000000 craft-archives-1.0.0/craft_archives.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.589578 craft-archives-1.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.581578 craft-archives-1.0.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.589578 craft-archives-1.0.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-24 18:13:15.000000 craft-archives-1.0.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-24 18:13:15.000000 craft-archives-1.0.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-24 18:13:15.000000 craft-archives-1.0.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.589578 craft-archives-1.0.0/docs/explanation/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-24 18:13:15.000000 craft-archives-1.0.0/docs/explanation/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.589578 craft-archives-1.0.0/docs/howto/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-24 18:13:15.000000 craft-archives-1.0.0/docs/howto/add_repo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-24 18:13:15.000000 craft-archives-1.0.0/docs/howto/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-24 18:13:15.000000 craft-archives-1.0.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.589578 craft-archives-1.0.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-24 18:13:15.000000 craft-archives-1.0.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-24 18:13:15.000000 craft-archives-1.0.0/docs/reference/repo_properties.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.589578 craft-archives-1.0.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-24 18:13:15.000000 craft-archives-1.0.0/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-05-24 18:13:15.000000 craft-archives-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 18:13:32.593578 craft-archives-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.589578 craft-archives-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.589578 craft-archives-1.0.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.589578 craft-archives-1.0.0/tests/integration/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/integration/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/integration/repo/test_apt_key_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/integration/repo/test_installer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.589578 craft-archives-1.0.0/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/test_data/FC42E99D.asc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/test_data/empty.preferences
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/test_data/expected.preferences
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/test_data/many_blank_lines.preferences
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/test_data/no_header.preferences
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/test_data/only_comment.preferences
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/test_data/with_header.preferences
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.589578 craft-archives-1.0.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.593578 craft-archives-1.0.0/tests/unit/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/unit/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/unit/repo/test_apt_key_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/unit/repo/test_apt_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/unit/repo/test_apt_preferences_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/unit/repo/test_apt_sources_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/unit/repo/test_apt_uca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/unit/repo/test_installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16191 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/unit/repo/test_package_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/unit/repo/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tox.ini
```

### Comparing `craft-archives-0.0.3/LICENSE` & `craft-archives-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `craft-archives-0.0.3/craft_archives/errors.py` & `craft-archives-1.0.0/craft_archives/errors.py`

 * *Files identical despite different names*

### Comparing `craft-archives-0.0.3/craft_archives/repo/__init__.py` & `craft-archives-1.0.0/craft_archives/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-archives-0.0.3/craft_archives/repo/apt_key_manager.py` & `craft-archives-1.0.0/craft_archives/repo/apt_key_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 
 # pyright: reportMissingTypeStubs=false
 
 import logging
 import pathlib
 import subprocess
 import tempfile
-from typing import Iterable, List, Optional
+from contextlib import contextmanager
+from typing import Iterable, Iterator, List, Optional
 
 from . import apt_ppa, errors, package_repository
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_APT_KEYSERVER = "keyserver.ubuntu.com"
 
@@ -75,24 +76,33 @@
 
     :returns: A Path object matching the expected filename
     """
     file_base = prefix + key_id[-8:].upper()
     return base_path.joinpath(file_base).with_suffix(".asc" if is_ascii else ".gpg")
 
 
+def _configure_keyring_file(keyring_file: pathlib.Path) -> None:
+    """Configure a newly created keyring file."""
+    # Change the permissions on the file so that APT itself can read it later
+    keyring_file.chmod(0o644)
+    # Also remove the backup file, if gpg created it
+    backup = keyring_file.with_suffix(keyring_file.suffix + "~")
+    backup.unlink(missing_ok=True)
+
+
 class AptKeyManager:
     """Manage APT repository keys."""
 
     def __init__(
         self,
         *,
-        keyrings_path: pathlib.Path = KEYRINGS_PATH,
+        keyrings_path: Optional[pathlib.Path] = None,
         key_assets: pathlib.Path,
     ) -> None:
-        self._keyrings_path = keyrings_path
+        self._keyrings_path = keyrings_path or KEYRINGS_PATH
         self._key_assets = key_assets
 
     def find_asset_with_key_id(self, *, key_id: str) -> Optional[pathlib.Path]:
         """Find snap key asset matching key_id.
 
         The key asset much be named with the last 8 characters of the key
         identifier, in upper case.
@@ -114,35 +124,38 @@
     def get_key_fingerprints(cls, *, key: str) -> List[str]:
         """List fingerprints found in specified key.
 
         :param key: Key data (string) to parse.
 
         :returns: List of key fingerprints/IDs.
         """
-        response = _call_gpg(
-            "--import-options", "show-only", "--import", stdin=key.encode()
-        ).splitlines()
+        with _temporary_home_dir() as tmpdir:
+            response = _call_gpg(
+                "--homedir",
+                str(tmpdir),
+                "--import-options",
+                "show-only",
+                "--import",
+                stdin=key.encode(),
+            ).splitlines()
         fingerprints: List[str] = []
         for line in response:
             if line.startswith(b"fpr:"):
                 fingerprints.append(line[4:].decode().strip(":"))
         return fingerprints
 
-    @classmethod
-    def is_key_installed(
-        cls, *, key_id: str, keyring_path: pathlib.Path = KEYRINGS_PATH
-    ) -> bool:
+    def is_key_installed(self, *, key_id: str) -> bool:
         """Check if specified key_id is installed.
 
-        :param key_id: Key ID to check for.
-        :param keyring_path: An optional override to check for the keyring.
+        :param key_id: Key ID to check for. The key will be looked for in the
+          AptKeyManager's configured keyrings path.
 
         :returns: True if key is installed.
         """
-        keyring_file = get_keyring_path(key_id, base_path=keyring_path)
+        keyring_file = get_keyring_path(key_id, base_path=self._keyrings_path)
         # Check if the keyring file exists first, otherwise the gpg check itself
         # creates it.
         if not keyring_file.is_file():
             logger.debug(f"Keyring file not found: {keyring_file}")
             return False
 
         # Ensure the keyring file contains the correct key
@@ -174,16 +187,15 @@
         self._create_keyrings_path()
         keyring_path = get_keyring_path(fingerprints[0], base_path=self._keyrings_path)
         try:
             _call_gpg("--import", "-", keyring=keyring_path, stdin=key.encode())
         except subprocess.CalledProcessError as error:
             raise errors.AptGPGKeyInstallError(error.output.decode(), key=key)
 
-        # Change the permissions on the file so that APT itself can read it later
-        keyring_path.chmod(0o644)
+        _configure_keyring_file(keyring_path)
         logger.debug(f"Installed apt repository key:\n{key}")
 
     def install_key_from_keyserver(
         self, *, key_id: str, key_server: str = DEFAULT_APT_KEYSERVER
     ) -> None:
         """Install key from specified key server.
 
@@ -191,29 +203,27 @@
         :param key_server: Key server to query.
 
         :raises: AptGPGKeyInstallError if unable to install key.
         """
         self._create_keyrings_path()
         keyring_path = get_keyring_path(key_id, base_path=self._keyrings_path)
         try:
-            with tempfile.TemporaryDirectory() as tmpdir_str:
+            with _temporary_home_dir() as tmpdir:
                 # We use a tmpdir because gpg needs a "homedir" to place temporary
                 # files into during the download process.
-                tmpdir = pathlib.Path(tmpdir_str)
-                tmpdir.chmod(0o700)
                 _call_gpg(
                     "--homedir",
-                    tmpdir_str,
+                    str(tmpdir),
                     "--keyserver",
                     key_server,
                     "--recv-keys",
                     key_id,
                     keyring=keyring_path,
                 )
-            keyring_path.chmod(0o644)
+            _configure_keyring_file(keyring_path)
         except subprocess.CalledProcessError as error:
             raise errors.AptGPGKeyInstallError(
                 error.output.decode(), key_id=key_id, key_server=key_server
             )
 
     def install_package_repository_key(
         self, *, package_repo: package_repository.PackageRepository
@@ -232,38 +242,50 @@
             key already installed.
 
         :raises: AptGPGKeyInstallError if unable to install key.
         """
         key_server = DEFAULT_APT_KEYSERVER
         if isinstance(package_repo, package_repository.PackageRepositoryAptPPA):
             key_id = apt_ppa.get_launchpad_ppa_key_id(ppa=package_repo.ppa)
+        elif isinstance(package_repo, package_repository.PackageRepositoryAptUCA):
+            key_id = package_repository.UCA_KEY_ID
         elif isinstance(package_repo, package_repository.PackageRepositoryApt):
             key_id = package_repo.key_id
             if package_repo.key_server:
                 key_server = package_repo.key_server
         else:
             raise RuntimeError(f"unhandled package repo type: {package_repo!r}")
 
         # Already installed, nothing to do.
         if self.is_key_installed(key_id=key_id):
             return False
 
         # If the keyring exists but does not contain the key, remove it and
         # install a fresh one.
         keyring_path = get_keyring_path(key_id, base_path=self._keyrings_path)
-        keyring_path.unlink(missing_ok=True)
+        if keyring_path.parent.is_dir():
+            keyring_path.unlink(missing_ok=True)
 
         key_path = self.find_asset_with_key_id(key_id=key_id)
         if key_path is not None:
             self.install_key(key=key_path.read_text())
         else:
             self.install_key_from_keyserver(key_id=key_id, key_server=key_server)
 
         return True
 
-    def _create_keyrings_path(self):
+    def _create_keyrings_path(self) -> None:
         """Create the directory that will contain the keys, if necessary."""
         if not self._keyrings_path.exists():
             logger.debug(
                 f"Keyrings location {self._keyrings_path} doesn't exist; Attempting to create it."
             )
             self._keyrings_path.mkdir(mode=0o755, parents=False)
+
+
+@contextmanager
+def _temporary_home_dir() -> Iterator[pathlib.Path]:
+    """Yield a temporary directory with proper permissions for gpg."""
+    with tempfile.TemporaryDirectory() as tmpdir_str:
+        tmpdir = pathlib.Path(tmpdir_str)
+        tmpdir.chmod(0o700)
+        yield tmpdir
```

### Comparing `craft-archives-0.0.3/craft_archives/repo/apt_ppa.py` & `craft-archives-1.0.0/craft_archives/repo/apt_ppa.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """Personal Package Archive helpers."""
 
 # pyright: reportMissingTypeStubs=false
+# Eliminate launchpadlib typing issues:
+# pyright: reportUnknownMemberType=false
 
 import logging
-from typing import Tuple
+from typing import Tuple, cast
 
 import lazr.restfulclient.errors  # type: ignore
 from launchpadlib.launchpad import Launchpad  # type: ignore
 
 from . import errors
 
 logger = logging.getLogger(__name__)
@@ -35,21 +37,20 @@
     if len(ppa_split) != 2:  # noqa: PLR2004
         raise errors.AptPPAInstallError(ppa, "invalid PPA format")
     return ppa_split[0], ppa_split[1]
 
 
 def get_launchpad_ppa_key_id(*, ppa: str) -> str:
     """Query Launchpad for PPA's key ID."""
-    # pyright: reportUnknownMemberType=false, reportUnknownVariableType=false
     owner, name = split_ppa_parts(ppa=ppa)
     launchpad = Launchpad.login_anonymously("snapcraft", "production")
     launchpad_url = f"~{owner}/+archive/{name}"
 
     logger.debug(f"Loading launchpad url: {launchpad_url}")
     try:
-        key_id: str = launchpad.load(launchpad_url).signing_key_fingerprint
+        key_id: str = cast(str, launchpad.load(launchpad_url).signing_key_fingerprint)
     except lazr.restfulclient.errors.NotFound as error:
         raise errors.AptPPAInstallError(ppa, "not found on launchpad") from error
 
     logger.debug(f"Retrieved launchpad PPA key ID: {key_id}")
 
     return key_id
```

### Comparing `craft-archives-0.0.3/craft_archives/repo/apt_preferences_manager.py` & `craft-archives-1.0.0/craft_archives/repo/apt_preferences_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,19 +104,19 @@
     :param path: Path to the preferences file
     :param header: A comment string to act as the file header.
     """
 
     def __init__(
         self,
         *,
-        path: Path = _DEFAULT_PREFERENCES_FILE,
+        path: typing.Optional[Path] = None,
         header: str = _DEFAULT_HEADER,
     ) -> None:
         self._header = header
-        self._path = path
+        self._path = path or _DEFAULT_PREFERENCES_FILE
         self._preferences: typing.List[Preference] = []
 
     def read(self) -> None:
         """Read the preferences file and populate Preferences objects."""
         if not self._path.exists():
             logger.debug("No preferences read.")
             return
```

### Comparing `craft-archives-0.0.3/craft_archives/repo/apt_sources_manager.py` & `craft-archives-1.0.0/craft_archives/repo/apt_sources_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,29 +15,30 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 """Manage the host's apt source repository configuration."""
 
 import io
 import logging
 import pathlib
-import re
 import subprocess
 from pathlib import Path
-from typing import List, Optional
+from typing import List, Optional, cast
 
-from craft_archives import os_release, utils
+import distro
 
-from . import apt_key_manager, apt_ppa, errors, package_repository
+from craft_archives import utils
+
+from . import apt_key_manager, apt_ppa, apt_uca, errors, package_repository
 
 logger = logging.getLogger(__name__)
 
 _DEFAULT_SOURCES_DIRECTORY = Path("/etc/apt/sources.list.d")
 
 
-def _construct_deb822_source(
+def _construct_deb822_source(  # noqa: PLR0913
     *,
     architectures: Optional[List[str]] = None,
     components: Optional[List[str]] = None,
     formats: Optional[List[str]] = None,
     suites: List[str],
     url: str,
     signed_by: pathlib.Path,
@@ -78,35 +79,35 @@
     :param sources_list_d: Path to sources.list.d directory.
     """
 
     # pylint: disable=too-few-public-methods
     def __init__(
         self,
         *,
-        sources_list_d: Path = _DEFAULT_SOURCES_DIRECTORY,
-        keyrings_dir: Path = apt_key_manager.KEYRINGS_PATH,
+        sources_list_d: Optional[Path] = None,
+        keyrings_dir: Optional[Path] = None,
     ) -> None:
-        self._sources_list_d = sources_list_d
-        self._keyrings_dir = keyrings_dir
+        self._sources_list_d = sources_list_d or _DEFAULT_SOURCES_DIRECTORY
+        self._keyrings_dir = keyrings_dir or apt_key_manager.KEYRINGS_PATH
 
-    def _install_sources(
+    def _install_sources(  # noqa: PLR0913
         self,
         *,
         architectures: Optional[List[str]] = None,
         components: Optional[List[str]] = None,
         formats: Optional[List[str]] = None,
         name: str,
         suites: List[str],
         url: str,
         keyring_path: pathlib.Path,
     ) -> bool:
         """Install sources list configuration.
 
         Write config to:
-        /etc/apt/sources.list.d/snapcraft-<name>.sources
+        /etc/apt/sources.list.d/craft-<name>.sources
 
         :returns: True if configuration was changed.
         """
         if keyring_path and not keyring_path.is_file():
             raise errors.AptGPGKeyringError(keyring_path)
 
         config = _construct_deb822_source(
@@ -115,15 +116,15 @@
             formats=formats,
             suites=suites,
             url=url,
             signed_by=keyring_path,
         )
 
         if name not in ["default", "default-security"]:
-            name = "snapcraft-" + name
+            name = "craft-" + name
 
         config_path = self._sources_list_d / f"{name}.sources"
         if config_path.exists() and config_path.read_text() == config:
             # Already installed and matches, nothing to do.
             logger.debug(f"Ignoring unchanged sources: {config_path!s}")
             return False
 
@@ -158,32 +159,27 @@
             # Suites denoting exact path must end with '/'.
             path = package_repo.path
             if not path.endswith("/"):
                 path += "/"
             suites = [path]
         elif package_repo.suites:
             suites = package_repo.suites
-            if not package_repo.components:
-                raise RuntimeError("no components with suite")
-        else:
+        else:  # pragma: no cover
             raise RuntimeError("no suites or path")
 
-        if package_repo.name:
-            name = package_repo.name
-        else:
-            name = re.sub(r"\W+", "_", package_repo.url)
+        name = package_repo.name
 
         keyring_path = apt_key_manager.get_keyring_path(
             package_repo.key_id, base_path=self._keyrings_dir
         )
 
         return self._install_sources(
             architectures=package_repo.architectures,
             components=package_repo.components,
-            formats=package_repo.formats,
+            formats=cast(Optional[List[str]], package_repo.formats),
             name=name,
             suites=suites,
             url=package_repo.url,
             keyring_path=keyring_path,
         )
 
     def _install_sources_ppa(
@@ -196,15 +192,15 @@
           entry.
         - Formulate deb URL to point to PPA.
         - Enable only "deb" formats.
 
         :returns: True if source configuration was changed.
         """
         owner, name = apt_ppa.split_ppa_parts(ppa=package_repo.ppa)
-        codename = os_release.OsRelease().version_codename()
+        codename = distro.codename()
 
         key_id = apt_ppa.get_launchpad_ppa_key_id(ppa=package_repo.ppa)
         keyring_path = apt_key_manager.get_keyring_path(
             key_id, base_path=self._keyrings_dir
         )
 
         return self._install_sources(
@@ -212,14 +208,46 @@
             formats=["deb"],
             name=f"ppa-{owner}_{name}",
             suites=[codename],
             url=f"http://ppa.launchpad.net/{owner}/{name}/ubuntu",
             keyring_path=keyring_path,
         )
 
+    def _install_sources_uca(
+        self, *, package_repo: package_repository.PackageRepositoryAptUCA
+    ) -> bool:
+        """Install UCA formatted repository.
+
+        Create a sources list config by:
+        - Looking up the codename of the host OS and using it as the "suites"
+          entry.
+        - Formulate deb URL to point to UCA.
+        - Enable only "deb" formats.
+
+        :returns: True if source configuration was changed.
+        """
+        cloud = package_repo.cloud
+        pocket = package_repo.pocket
+
+        codename = distro.codename()
+        apt_uca.check_release_compatibility(codename, cloud, pocket)
+
+        key_id = package_repository.UCA_KEY_ID
+        keyring_path = apt_key_manager.get_keyring_path(
+            key_id, base_path=self._keyrings_dir
+        )
+        return self._install_sources(
+            components=["main"],
+            formats=["deb"],
+            name=f"cloud-{cloud}",
+            suites=[f"{codename}-{pocket}/{cloud}"],
+            url=package_repository.UCA_ARCHIVE,
+            keyring_path=keyring_path,
+        )
+
     def install_package_repository_sources(
         self,
         *,
         package_repo: package_repository.PackageRepository,
     ) -> bool:
         """Install configured package repositories.
 
@@ -227,14 +255,17 @@
 
         :returns: True if source configuration was changed.
         """
         logger.debug(f"Processing repo: {package_repo!r}")
         if isinstance(package_repo, package_repository.PackageRepositoryAptPPA):
             return self._install_sources_ppa(package_repo=package_repo)
 
+        if isinstance(package_repo, package_repository.PackageRepositoryAptUCA):
+            return self._install_sources_uca(package_repo=package_repo)
+
         if isinstance(package_repo, package_repository.PackageRepositoryApt):
             changed = self._install_sources_apt(package_repo=package_repo)
             architectures = package_repo.architectures
             if changed and architectures:
                 _add_architecture(architectures)
             return changed
```

### Comparing `craft-archives-0.0.3/craft_archives/repo/errors.py` & `craft-archives-1.0.0/craft_archives/repo/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,14 +65,24 @@
     def __init__(self, ppa: str, reason: str) -> None:
         super().__init__(
             f"Failed to install PPA {ppa!r}: {reason}",
             resolution="Verify PPA is correct and try again",
         )
 
 
+class AptUCAInstallError(PackageRepositoryError):
+    """Installation of an UCA repository failed."""
+
+    def __init__(self, cloud: str, pocket: str, reason: str) -> None:
+        super().__init__(
+            f"Failed to install UCA '{cloud}/{pocket}': {reason}",
+            resolution="Verify UCA is correct and try again",
+        )
+
+
 class AptGPGKeyringError(PackageRepositoryError):
     """GPG keyring for repository does not exist or not valid."""
 
     def __init__(self, keyring_path: pathlib.Path) -> None:
         super().__init__(
             "Could not find keyring file for repository.",
             f"Keyring file does not exist or is invalid: {keyring_path}",
```

### Comparing `craft-archives-0.0.3/craft_archives/repo/installer.py` & `craft-archives-1.0.0/craft_archives/repo/installer.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from .apt_key_manager import AptKeyManager
 from .apt_preferences_manager import AptPreferencesManager
 from .apt_sources_manager import AptSourcesManager
 from .package_repository import (
     PackageRepository,
     PackageRepositoryApt,
     PackageRepositoryAptPPA,
+    PackageRepositoryAptUCA,
 )
 
 
 def install(
     project_repositories: List[Dict[str, Any]], *, key_assets: pathlib.Path
 ) -> bool:
     """Add package repositories to the host system.
@@ -51,19 +52,26 @@
         refresh_required |= key_manager.install_package_repository_key(
             package_repo=package_repo
         )
         refresh_required |= sources_manager.install_package_repository_sources(
             package_repo=package_repo
         )
         if (
-            isinstance(package_repo, (PackageRepositoryApt, PackageRepositoryAptPPA))
+            isinstance(
+                package_repo,
+                (
+                    PackageRepositoryApt,
+                    PackageRepositoryAptPPA,
+                    PackageRepositoryAptUCA,
+                ),
+            )
             and package_repo.priority is not None
         ):
             refresh_required |= preferences_manager.add(
-                pin=package_repo.pin, priority=package_repo.priority
+                pin=package_repo.pin, priority=int(package_repo.priority)
             )
 
     refresh_required |= preferences_manager.write()
 
     _verify_all_key_assets_installed(key_assets=key_assets, key_manager=key_manager)
 
     return refresh_required
@@ -92,13 +100,15 @@
     """Create package repositories objects from project data."""
     repositories: List[PackageRepository] = []
     for data in project_repositories:
         pkg_repo: PackageRepository
 
         if "ppa" in data:
             pkg_repo = PackageRepositoryAptPPA.unmarshal(data)
+        elif "cloud" in data:
+            pkg_repo = PackageRepositoryAptUCA.unmarshal(data)
         else:
             pkg_repo = PackageRepositoryApt.unmarshal(data)
 
         repositories.append(pkg_repo)
 
     return repositories
```

### Comparing `craft-archives-0.0.3/craft_archives/utils.py` & `craft-archives-1.0.0/craft_archives/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     "armv8l": "armv7l",
     "ppc64le": "ppc",
     "x86_64": "i686",
 }
 
 
 def get_os_platform(
-    filepath: Path = Path("/etc/os-release"),  # noqa: B008
+    filepath: Path = Path("/etc/os-release"),
 ) -> OSPlatform:
     """Determine a system/release combo for an OS using /etc/os-release if available."""
     system = platform.system()
     release = platform.release()
     machine = platform.machine()
 
     if system == "Linux":
```

### Comparing `craft-archives-0.0.3/pyproject.toml` & `craft-archives-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,80 +1,92 @@
 [project]
 name = "craft-archives"
-version = "0.0.3"
-readme = "README.rst"
+dynamic = ["version", "readme"]
 dependencies = [
-    "gnupg",
+    "distro>=1.3.0",
     "launchpadlib",
     "lazr.restfulclient",
     "lazr.uri",
     "overrides",
     "pydantic",
 ]
 classifiers = [
-    "Development Status :: 1 - Planning",
-    "License :: OSI Approved :: GNU General Public License (GPL)",
+    "Development Status :: 3 - Alpha",
+    "Operating System :: POSIX :: Linux",
+    "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Topic :: Software Development :: Libraries",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Topic :: System :: Archiving :: Packaging",
 ]
 requires-python = ">=3.8"
 
 [project.scripts]
 
 [project.optional-dependencies]
 dev = [
-    "pytest==7.2.2",
+    "pytest==7.3.1",
     "pytest-cov==4.0.0",
     "pytest-check==2.1.4",
-    "coverage[toml]==7.2.1",
+    "coverage[toml]==7.2.5",
     "pytest-mock==3.10.0",
 ]
-dev-lint = [  # Static linting environment dependencies
-    "black==23.1.0",
-    "codespell[tomli]==2.2.4",
-    "ruff==0.0.254",
-]
-types = [  # Dependencies for typing. Both types packages and mypy itself.
-    "mypy[reports]==1.1.1",
+lint = [
+    "black==23.3.0",
+    "codespell[toml]==2.2.4",
+    "ruff==0.0.269",
+    "yamllint==1.32.0"
+]
+types = [
+    "mypy[reports]==1.3.0",
+    "pyright==1.1.309",
 ]
 docs = [
-    "furo==2022.12.07",
-    "sphinx==5.3.0",
+    "furo==2023.5.20",
+    "sphinx>=6.2.1,<7.0",
     "sphinx-autobuild==2021.3.14",
-    "sphinx-copybutton==0.5.1",
-    "sphinx-design==0.3.0",
+    "sphinx-copybutton==0.5.2",
+    "sphinx-design==0.4.1",
     "sphinx-pydantic==0.1.1",
     "sphinx-toolbox==3.4.0",
     "sphinx-lint==0.6.7",
 ]
 
 [build-system]
 requires = [
-    "setuptools==67.6.0",
+    "setuptools==67.7.2",
+    "setuptools_scm[toml]>=7.1"
 ]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools.dynamic]
+readme = {file = "README.rst"}
+
 [tool.setuptools.packages.find]
 exclude = [
     "dist",
     "docs",
     "results",
-    "test*",
+    "tests",
 ]
 
+[tool.setuptools_scm]
+write_to = "craft_archives/_version.py"
+
 [tool.black]
 target-version = ["py38"]
 
 [tool.codespell]
 ignore-words-list = "buildd,crate,keyserver,comandos,ro,dedent,dedented"
-skip = ".tox,.git,build,.*_cache,__pycache__,*.tar,*.snap,*.png,./node_modules,./docs/_build"
+skip = ".tox,.git,build,.*_cache,__pycache__,*.tar,*.snap,*.png,./node_modules,./docs/_build,.direnv,.venv,venv,.vscode"
 quiet-level = 3
 check-filenames = true
 exclude-file = ".codespell_ignore_lines"
 
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = true
@@ -87,29 +99,24 @@
 minversion = "7.0"
 testpaths = "tests"
 xfail_strict = true
 
 [tool.coverage.run]
 branch = true
 parallel = true
-omit = [
-    "tests/**",
-    "craft_archives/os_release.py",
-]
+omit = ["tests/**"]
 
 [tool.coverage.report]
 skip_empty = true
-#fail_under = 80
+fail_under = 80
 
 [tool.pyright]
 strict = ["craft_archives"]
 pythonVersion = "3.8"
 pythonPlatform = "Linux"
-venvPath = ".tox"
-venv = "py38"
 
 [tool.mypy]
 python_version = "3.8"
 exclude = [
     "build",
     "tests",
     "results",
@@ -137,15 +144,16 @@
 target-version = "py38"
 src = ["craft_archives", "tests"]
 extend-exclude = [
     "docs",
     "__pycache__",
 ]
 pep8-naming.classmethod-decorators = [
-    "pydantic.validator"
+    "pydantic.validator",
+    "pydantic.root_validator"
 ]
 
 # Follow ST063 - Maintaining and updating linting specifications for updating these.
 select = [  # Base linting rule selections.
     # See the internal document for discussion:
     # https://docs.google.com/document/d/1i1n8pDmFmWi4wTDpk-JfnWCVUThPJiggyPi2DYwBBu4/edit
     # All sections here are stable in ruff and shouldn't randomly introduce
@@ -161,39 +169,40 @@
     "FBT",  # Disallow boolean positional arguments (make them keyword-only)
     "A",  # Shadowing built-ins.
     "C4", # Encourage comprehensions, which tend to be faster than alternatives.
     "T10",  # Don't call the debugger in production code
     "ISC",  # Implicit string concatenation that can cause subtle issues
     "ICN",  # Only use common conventions for import aliases.
     "Q",  # Consistent quotations
-    "RET"  # Simpler logic after return, raise, continue or break
+    "RET",  # Simpler logic after return, raise, continue or break
+    "UP018", "C408",  # Convert type calls to literals. The latest pylint enforces this, but ruff has auto-fixes.
 ]
 extend-select = [
     # These sets are still frequently getting new rules.
     # Therefore, they're getting frozen with the current rules so we can
     # upgrade ruff without breaking linting.
     # Pyupgrade: https://github.com/charliermarsh/ruff#pyupgrade-up
     "UP00", "UP01", "UP02", "UP030", "UP032", "UP033",
     # "UP034",  # Very new, not yet enabled in ruff 0.0.227
     # Annotations: https://github.com/charliermarsh/ruff#flake8-annotations-ann
     "ANN0",  # Type annotations for arguments other than `self` and `cls`
     "ANN2",  # Return type annotations
+    "B026",  # Keyword arguments must come after starred arguments
     # flake8-bandit: security testing. https://github.com/charliermarsh/ruff#flake8-bandit-s
     # https://bandit.readthedocs.io/en/latest/plugins/index.html#complete-test-plugin-listing
     "S101", "S102",  # assert or exec
     "S103", "S108",  # File permissions and tempfiles - use #noqa to silence when appropriate.
     "S104",  # Network binds
     "S105", "S106", "S107",  # Hardcoded passwords
     "S113",  # Requests calls without timeouts
     "S506",  # Unsafe YAML load
     "S508", "S509",  # Insecure SNMP
     "S701",  # jinja2 templates without autoescape
     "B0",  # Common mistakes and typos.
     "RUF001", "RUF002", "RUF003",  # Ambiguous unicode characters
-    "RUF004",  # Keyword arguments must come after starred arguments
     "RUF005",  # Encourages unpacking rather than concatenation
     "RUF100",  # #noqa directive that doesn't flag anything.
 ]
 ignore = [
     #"E203",  # Whitespace before ":"  -- Commented because ruff doesn't currently check E203
     "E501",  # Line too long (reason: black will automatically fix this for us)
     "D105",  # Missing docstring in magic method (reason: magic methods already have definitions)
@@ -208,12 +217,11 @@
 [tool.ruff.per-file-ignores]
 "tests/**.py" = [  # Some things we want for the moin project are unnecessary in tests.
     "D",  # Ignore docstring rules in tests
     "ANN", # Ignore type annotations in tests
     "S101",  # Allow assertions in tests
     "S103", # Allow `os.chmod` setting a permissive mask `0o555` on file or directory
     "S108", # Allow Probable insecure usage of temporary file or directory
-    "PLR0913", # Too many arguments to function
-    "PLR2004", # Allow magic values used in comparisons
+    "PLR0913",  # Allow many arguments for test functions
 ]
 # isort leaves init files alone by default, this makes ruff ignore them too.
 "__init__.py" = ["I001"]
```

