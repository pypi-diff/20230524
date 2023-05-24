# Comparing `tmp/pynamer-1.3.4.tar.gz` & `tmp/pynamer-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamer-1.3.4.tar", last modified: Mon May 22 12:56:36 2023, max compression
+gzip compressed data, was "pynamer-2.0.0.tar", last modified: Wed May 24 16:02:12 2023, max compression
```

## Comparing `pynamer-1.3.4.tar` & `pynamer-2.0.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 12:56:36.378340 pynamer-1.3.4/
--rw-rw-rw-   0        0        0      172 2023-05-21 12:10:39.000000 pynamer-1.3.4/AUTHORS.md
--rw-rw-rw-   0        0        0     9429 2023-05-22 12:56:20.000000 pynamer-1.3.4/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2023-05-21 12:10:39.000000 pynamer-1.3.4/LICENSE
--rw-rw-rw-   0        0        0      237 2023-05-21 12:10:39.000000 pynamer-1.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0    18662 2023-05-22 12:56:36.379341 pynamer-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0    17081 2023-05-22 08:49:55.000000 pynamer-1.3.4/README.md
--rw-rw-rw-   0        0        0     2071 2023-05-21 12:45:00.000000 pynamer-1.3.4/pyproject.toml
--rw-rw-rw-   0        0        0     1893 2023-05-22 12:56:36.382348 pynamer-1.3.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-22 12:56:35.900674 pynamer-1.3.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-22 12:56:36.043405 pynamer-1.3.4/src/pynamer/
--rw-rw-rw-   0        0        0       11 2023-05-21 12:10:39.000000 pynamer-1.3.4/src/pynamer/README.md
--rw-rw-rw-   0        0        0     1807 2023-05-22 12:56:20.000000 pynamer-1.3.4/src/pynamer/__init__.py
--rw-rw-rw-   0        0        0      754 2023-05-21 12:10:39.000000 pynamer-1.3.4/src/pynamer/config.py
-drwxrwxrwx   0        0        0        0 2023-05-22 12:56:36.056393 pynamer-1.3.4/src/pynamer/project_name/
--rw-rw-rw-   0        0        0        0 2023-05-21 12:10:39.000000 pynamer-1.3.4/src/pynamer/project_name/__init__.py
--rw-rw-rw-   0        0        0    35223 2023-05-21 12:10:39.000000 pynamer-1.3.4/src/pynamer/pynamer.py
--rw-rw-rw-   0        0        0      401 2023-05-22 08:56:28.000000 pynamer-1.3.4/src/pynamer/setup.txt
--rw-rw-rw-   0        0        0      401 2023-05-21 12:10:39.000000 pynamer-1.3.4/src/pynamer/setup_base.txt
--rw-rw-rw-   0        0        0     1641 2023-05-21 12:10:39.000000 pynamer-1.3.4/src/pynamer/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-22 12:56:36.054392 pynamer-1.3.4/src/pynamer.egg-info/
--rw-rw-rw-   0        0        0    18662 2023-05-22 12:56:35.000000 pynamer-1.3.4/src/pynamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1053 2023-05-22 12:56:35.000000 pynamer-1.3.4/src/pynamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 12:56:35.000000 pynamer-1.3.4/src/pynamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-22 12:56:35.000000 pynamer-1.3.4/src/pynamer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       74 2023-05-22 12:56:35.000000 pynamer-1.3.4/src/pynamer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-22 12:56:35.000000 pynamer-1.3.4/src/pynamer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-22 12:56:36.376345 pynamer-1.3.4/tests/
--rw-rw-rw-   0        0        0     1869 2023-05-21 12:10:39.000000 pynamer-1.3.4/tests/test_args.py
--rw-rw-rw-   0        0        0     1923 2023-05-21 12:10:39.000000 pynamer-1.3.4/tests/test_build_dist.py
--rw-rw-rw-   0        0        0     1080 2023-05-21 12:10:39.000000 pynamer-1.3.4/tests/test_cleanup.py
--rw-rw-rw-   0        0        0      978 2023-05-21 12:10:39.000000 pynamer-1.3.4/tests/test_create_setup_file.py
--rw-rw-rw-   0        0        0     1587 2023-05-21 12:10:39.000000 pynamer-1.3.4/tests/test_defaults.py
--rw-rw-rw-   0        0        0      538 2023-05-21 12:10:39.000000 pynamer-1.3.4/tests/test_delete_director.py
--rw-rw-rw-   0        0        0     1289 2023-05-21 12:10:39.000000 pynamer-1.3.4/tests/test_feedback.py
--rw-rw-rw-   0        0        0     2698 2023-05-21 12:10:39.000000 pynamer-1.3.4/tests/test_final_analysis.py
--rw-rw-rw-   0        0        0      738 2023-05-21 12:10:39.000000 pynamer-1.3.4/tests/test_find_pypirc_file.py
--rw-rw-rw-   0        0        0     1450 2023-05-21 12:10:39.000000 pynamer-1.3.4/tests/test_generate_pypi_index.py
--rw-rw-rw-   0        0        0      295 2023-05-21 12:10:39.000000 pynamer-1.3.4/tests/test_is_valid_package_name.py
--rw-rw-rw-   0        0        0     1721 2023-05-21 12:10:39.000000 pynamer-1.3.4/tests/test_ping_json.py
--rw-rw-rw-   0        0        0     1547 2023-05-21 12:10:39.000000 pynamer-1.3.4/tests/test_ping_project.py
--rw-rw-rw-   0        0        0      522 2023-05-21 12:10:39.000000 pynamer-1.3.4/tests/test_process_input_file.py
--rw-rw-rw-   0        0        0     1129 2023-05-21 12:10:39.000000 pynamer-1.3.4/tests/test_pypi_search.py
--rw-rw-rw-   0        0        0      517 2023-05-21 12:10:39.000000 pynamer-1.3.4/tests/test_pypi_search_index.py
--rw-rw-rw-   0        0        0      764 2023-05-21 12:10:39.000000 pynamer-1.3.4/tests/test_rename_project_dir.py
--rw-rw-rw-   0        0        0      882 2023-05-21 12:10:39.000000 pynamer-1.3.4/tests/test_upload_dist.py
--rw-rw-rw-   0        0        0     1671 2023-05-21 12:10:39.000000 pynamer-1.3.4/tests/test_utils_version.py
--rw-rw-rw-   0        0        0      647 2023-05-21 12:10:39.000000 pynamer-1.3.4/tests/test_write_output_file.py
+drwxrwxrwx   0        0        0        0 2023-05-24 16:02:12.504706 pynamer-2.0.0/
+-rw-rw-rw-   0        0        0      172 2023-05-21 12:10:39.000000 pynamer-2.0.0/AUTHORS.md
+-rw-rw-rw-   0        0        0     9599 2023-05-24 16:01:59.000000 pynamer-2.0.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2023-05-21 12:10:39.000000 pynamer-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0      237 2023-05-21 12:10:39.000000 pynamer-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    18662 2023-05-24 16:02:12.504706 pynamer-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    17081 2023-05-22 08:49:55.000000 pynamer-2.0.0/README.md
+-rw-rw-rw-   0        0        0     2071 2023-05-21 12:45:00.000000 pynamer-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1893 2023-05-24 16:02:12.505710 pynamer-2.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 16:02:12.407715 pynamer-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 16:02:12.437711 pynamer-2.0.0/src/pynamer/
+-rw-rw-rw-   0        0        0       11 2023-05-21 12:10:39.000000 pynamer-2.0.0/src/pynamer/README.md
+-rw-rw-rw-   0        0        0     1853 2023-05-24 16:02:00.000000 pynamer-2.0.0/src/pynamer/__init__.py
+-rw-rw-rw-   0        0        0     9660 2023-05-24 15:55:39.000000 pynamer-2.0.0/src/pynamer/builder.py
+-rw-rw-rw-   0        0        0      754 2023-05-21 12:10:39.000000 pynamer-2.0.0/src/pynamer/config.py
+drwxrwxrwx   0        0        0        0 2023-05-24 16:02:12.447708 pynamer-2.0.0/src/pynamer/project_name/
+-rw-rw-rw-   0        0        0        0 2023-05-21 12:10:39.000000 pynamer-2.0.0/src/pynamer/project_name/__init__.py
+-rw-rw-rw-   0        0        0    15174 2023-05-24 09:27:39.000000 pynamer-2.0.0/src/pynamer/pynamer.py
+-rw-rw-rw-   0        0        0      386 2023-05-24 15:24:28.000000 pynamer-2.0.0/src/pynamer/setup.txt
+-rw-rw-rw-   0        0        0      401 2023-05-21 12:10:39.000000 pynamer-2.0.0/src/pynamer/setup_base.txt
+-rw-rw-rw-   0        0        0     5781 2023-05-24 09:37:42.000000 pynamer-2.0.0/src/pynamer/utils.py
+-rw-rw-rw-   0        0        0     6128 2023-05-24 15:55:39.000000 pynamer-2.0.0/src/pynamer/validators.py
+drwxrwxrwx   0        0        0        0 2023-05-24 16:02:12.445710 pynamer-2.0.0/src/pynamer.egg-info/
+-rw-rw-rw-   0        0        0    18662 2023-05-24 16:02:12.000000 pynamer-2.0.0/src/pynamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1102 2023-05-24 16:02:12.000000 pynamer-2.0.0/src/pynamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 16:02:12.000000 pynamer-2.0.0/src/pynamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-24 16:02:12.000000 pynamer-2.0.0/src/pynamer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       74 2023-05-24 16:02:12.000000 pynamer-2.0.0/src/pynamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-24 16:02:12.000000 pynamer-2.0.0/src/pynamer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 16:02:12.502708 pynamer-2.0.0/tests/
+-rw-rw-rw-   0        0        0     1869 2023-05-21 12:10:39.000000 pynamer-2.0.0/tests/test_args.py
+-rw-rw-rw-   0        0        0     2000 2023-05-24 15:55:39.000000 pynamer-2.0.0/tests/test_build_dist.py
+-rw-rw-rw-   0        0        0     1102 2023-05-24 15:55:39.000000 pynamer-2.0.0/tests/test_cleanup.py
+-rw-rw-rw-   0        0        0     1222 2023-05-24 15:55:39.000000 pynamer-2.0.0/tests/test_create_setup_file.py
+-rw-rw-rw-   0        0        0     1541 2023-05-24 15:55:39.000000 pynamer-2.0.0/tests/test_defaults.py
+-rw-rw-rw-   0        0        0      529 2023-05-24 15:55:39.000000 pynamer-2.0.0/tests/test_delete_director.py
+-rw-rw-rw-   0        0        0     1289 2023-05-21 12:10:39.000000 pynamer-2.0.0/tests/test_feedback.py
+-rw-rw-rw-   0        0        0     2698 2023-05-21 12:10:39.000000 pynamer-2.0.0/tests/test_final_analysis.py
+-rw-rw-rw-   0        0        0      738 2023-05-21 12:10:39.000000 pynamer-2.0.0/tests/test_find_pypirc_file.py
+-rw-rw-rw-   0        0        0     1407 2023-05-24 15:55:39.000000 pynamer-2.0.0/tests/test_generate_pypi_index.py
+-rw-rw-rw-   0        0        0      295 2023-05-21 12:10:39.000000 pynamer-2.0.0/tests/test_is_valid_package_name.py
+-rw-rw-rw-   0        0        0     1721 2023-05-21 12:10:39.000000 pynamer-2.0.0/tests/test_ping_json.py
+-rw-rw-rw-   0        0        0     1547 2023-05-21 12:10:39.000000 pynamer-2.0.0/tests/test_ping_project.py
+-rw-rw-rw-   0        0        0      522 2023-05-21 12:10:39.000000 pynamer-2.0.0/tests/test_process_input_file.py
+-rw-rw-rw-   0        0        0     1129 2023-05-21 12:10:39.000000 pynamer-2.0.0/tests/test_pypi_search.py
+-rw-rw-rw-   0        0        0      515 2023-05-24 15:55:39.000000 pynamer-2.0.0/tests/test_pypi_search_index.py
+-rw-rw-rw-   0        0        0      746 2023-05-24 15:55:39.000000 pynamer-2.0.0/tests/test_rename_project_dir.py
+-rw-rw-rw-   0        0        0      914 2023-05-24 15:55:39.000000 pynamer-2.0.0/tests/test_upload_dist.py
+-rw-rw-rw-   0        0        0     1671 2023-05-21 12:10:39.000000 pynamer-2.0.0/tests/test_utils_version.py
+-rw-rw-rw-   0        0        0      647 2023-05-21 12:10:39.000000 pynamer-2.0.0/tests/test_write_output_file.py
```

### Comparing `pynamer-1.3.4/CHANGELOG.md` & `pynamer-2.0.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.0.0 (2023-05-24)
+### Documentation
+* Update citation ([`6cd655b`](https://github.com/Stephen-RA-King/pynamer/commit/6cd655bc1c9672fd5f64cbf63a78fc739a141328))
+
 ## v1.3.4 (2023-05-22)
 ### Documentation
 * Fix type ([`a0cc3e1`](https://github.com/Stephen-RA-King/pynamer/commit/a0cc3e1b63cc3d147dea05085f7c9ecc80944815))
 * Add documentation assets ([`eb45590`](https://github.com/Stephen-RA-King/pynamer/commit/eb455904f0c2dc73410e318e3bbe50b7d03a7273))
 
 ## v1.3.3 (2023-05-21)
```

### Comparing `pynamer-1.3.4/LICENSE` & `pynamer-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.4/PKG-INFO` & `pynamer-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 1.3.4
+Version: 2.0.0
 Summary: Utility to find an available package name on the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
```

### Comparing `pynamer-1.3.4/README.md` & `pynamer-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.4/pyproject.toml` & `pynamer-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.4/setup.cfg` & `pynamer-2.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.4/src/pynamer/__init__.py` & `pynamer-2.0.0/src/pynamer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 """Top-level package for pynamer."""
 # Core Library modules
 import logging.config
 import pickle
-from importlib.resources import as_file, files
+from importlib.resources import files
 
 # Third party modules
 import yaml
 
 __title__ = "pynamer"
-__version__ = "1.3.4"
+__version__ = "2.0.0"
 __author__ = "Stephen R A King"
 __description__ = (
     "Utility to find an available package name in the PyPI repository and register it "
 )
 __email__ = "sking.github@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Stephen R A King"
@@ -46,14 +46,15 @@
 """
 
 logging.config.dictConfig(yaml.safe_load(LOGGING_CONFIG))
 logger = logging.getLogger("init")
 
 project_path = files("pynamer")
 setup_file_trv = project_path.joinpath("setup.txt")
+setup_file_py_trv = project_path.joinpath("setup.py")
 setup_base_file_trv = project_path.joinpath("setup_base.txt")
 project_count_file_trv = project_path.joinpath("project_count.pickle")
 pypi_index_file_trv = project_path.joinpath("pypi_index")
 meta_file_trv = project_path.joinpath("meta.pickle")
 
 
 if setup_file_trv.is_file():
```

### Comparing `pynamer-1.3.4/src/pynamer/config.py` & `pynamer-2.0.0/src/pynamer/config.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.4/src/pynamer.egg-info/PKG-INFO` & `pynamer-2.0.0/src/pynamer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 1.3.4
+Version: 2.0.0
 Summary: Utility to find an available package name on the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
```

### Comparing `pynamer-1.3.4/src/pynamer.egg-info/SOURCES.txt` & `pynamer-2.0.0/src/pynamer.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 src/pynamer/README.md
 src/pynamer/__init__.py
+src/pynamer/builder.py
 src/pynamer/config.py
 src/pynamer/pynamer.py
 src/pynamer/setup.txt
 src/pynamer/setup_base.txt
 src/pynamer/utils.py
+src/pynamer/validators.py
 src/pynamer.egg-info/PKG-INFO
 src/pynamer.egg-info/SOURCES.txt
 src/pynamer.egg-info/dependency_links.txt
 src/pynamer.egg-info/entry_points.txt
 src/pynamer.egg-info/requires.txt
 src/pynamer.egg-info/top_level.txt
 src/pynamer/project_name/__init__.py
```

### Comparing `pynamer-1.3.4/tests/test_args.py` & `pynamer-2.0.0/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.4/tests/test_build_dist.py` & `pynamer-2.0.0/tests/test_build_dist.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,74 +1,77 @@
-#!/usr/bin/env python3
-# Core Library modules
-import shutil
-from pathlib import Path
-
-# Third party modules
-import pytest
-
-# First party modules
-from pynamer import pynamer
-
-BASE_DIR = Path(__file__).parents[0]
-
-setup_text = """#!/usr/bin/env python3
-
-# Third party modules
-from setuptools import setup
-
-setup(name='pynamer',
-      version='0.0.0',
-      description='place holder',
-      url='http://github.com/SK/pynamer',
-      author='sking',
-      author_email='flyingcircus@example.com',
-      license='MIT',
-      packages=['pynamer'],
-      zip_safe=False)"""
-
-
-@pytest.fixture()
-def pre_build_dist(monkeypatch):
-    project_dir = BASE_DIR / "pynamer"
-    project_dir.mkdir()
-    project_init_file = BASE_DIR / "pynamer" / "__init__.py"
-    project_init_file.touch()
-    pypirc_file = BASE_DIR / ".pypirc"
-    pypirc_file.touch()
-    setup_py = BASE_DIR / "setup.py"
-    setup_py.touch()
-    setup_py.write_text(setup_text)
-    readme_file = BASE_DIR / "README.md"
-    readme_file.touch()
-    readme_file.write_text("pynamer")
-    build = BASE_DIR / "build"
-    dist = BASE_DIR / "dist"
-    egg = BASE_DIR / "pynamer.egg-info"
-
-    yield
-
-    manifest = [
-        project_dir,
-        pypirc_file,
-        setup_py,
-        readme_file,
-        build,
-        dist,
-        egg,
-    ]
-    for item in manifest:
-        if item.exists():
-            if item.is_dir():
-                shutil.rmtree(item)
-            elif item.is_file():
-                item.unlink()
-
-
-@pytest.mark.slow
-def test_build_dist(pre_build_dist, project_path_mock):
-    pynamer._build_dist()
-    assert (BASE_DIR / "build").exists()
-    assert (BASE_DIR / "dist").exists()
-    assert (BASE_DIR / "dist" / "pynamer-0.0.0.tar.gz").exists()
-    assert (BASE_DIR / "dist" / "pynamer-0.0.0-py3-none-any.whl").exists()
-    assert (BASE_DIR / "pynamer.egg-info").exists()
+#!/usr/bin/env python3
+# Core Library modules
+import shutil
+from pathlib import Path
+
+# Third party modules
+import pytest
+
+# First party modules
+from pynamer import builder, pynamer
+
+BASE_DIR = Path(__file__).parents[0]
+
+setup_text = """#!/usr/bin/env python3
+
+# Third party modules
+from setuptools import setup
+
+setup(name='pynamer',
+      version='0.0.0',
+      description='place holder',
+      url='http://github.com/SK/pynamer',
+      author='sking',
+      author_email='flyingcircus@example.com',
+      license='MIT',
+      packages=['pynamer'],
+      zip_safe=False)"""
+
+
+@pytest.fixture()
+def pre_build_dist(monkeypatch):
+    project_dir = BASE_DIR / "pynamer"
+    project_dir.mkdir()
+    project_init_file = BASE_DIR / "pynamer" / "__init__.py"
+    project_init_file.touch()
+    pypirc_file = BASE_DIR / ".pypirc"
+    pypirc_file.touch()
+    setup_py = BASE_DIR / "setup.py"
+    setup_py.touch()
+    setup_py.write_text(setup_text)
+    readme_file = BASE_DIR / "README.md"
+    readme_file.touch()
+    readme_file.write_text("pynamer")
+    build = BASE_DIR / "build"
+    dist = BASE_DIR / "dist"
+    egg = BASE_DIR / "pynamer.egg-info"
+
+    yield
+
+    manifest = [
+        project_dir,
+        pypirc_file,
+        setup_py,
+        readme_file,
+        build,
+        dist,
+        egg,
+    ]
+    for item in manifest:
+        if item.exists():
+            if item.is_dir():
+                shutil.rmtree(item)
+            elif item.is_file():
+                item.unlink()
+
+
+@pytest.mark.slow
+def test_build_dist(pre_build_dist, monkeypatch):
+    # monkeypatch.setattr(pynamer, "project_path", BASE_DIR)
+    monkeypatch.setattr(builder, "project_path", BASE_DIR)
+    pynamer._build_dist()
+    # builder._build_dist()
+    assert (BASE_DIR / "build").exists()
+    assert (BASE_DIR / "dist").exists()
+    assert (BASE_DIR / "dist" / "pynamer-0.0.0.tar.gz").exists()
+    assert (BASE_DIR / "dist" / "pynamer-0.0.0-py3-none-any.whl").exists()
+    assert (BASE_DIR / "pynamer.egg-info").exists()
```

### Comparing `pynamer-1.3.4/tests/test_cleanup.py` & `pynamer-2.0.0/tests/test_cleanup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-#!/usr/bin/env python3
-# Core Library modules
-import shutil
-from pathlib import Path
-
-# Third party modules
-import pytest
-
-# First party modules
-from pynamer import pynamer
-
-BASE_DIR = Path(__file__).parents[0]
-
-
-@pytest.fixture()
-def pre_cleanup(monkeypatch):
-    project_dir = BASE_DIR / "pynamer"
-    project_dir.mkdir()
-    build_dir = BASE_DIR / "build"
-    build_dir.mkdir()
-    dist_dir = BASE_DIR / "dist"
-    dist_dir.mkdir()
-    egg_dir = BASE_DIR / "pynamer.egg-info"
-    egg_dir.mkdir()
-    setup_py = BASE_DIR / "setup.py"
-    setup_py.touch()
-
-    yield
-
-    if (BASE_DIR / "project_name").exists():
-        shutil.rmtree(BASE_DIR / "project_name")
-
-
-def test_cleanup(pre_cleanup, project_path_mock):
-    pynamer._cleanup("pynamer")
-    assert not (BASE_DIR / "build").exists()
-    assert not (BASE_DIR / "dist").exists()
-    assert not (BASE_DIR / "dist" / "pynamer-0.0.0.tar.gz").exists()
-    assert not (BASE_DIR / "dist" / "pynamer-0.0.0-py3-none-any.whl").exists()
-    assert not (BASE_DIR / "pynamer.egg-info").exists()
+#!/usr/bin/env python3
+# Core Library modules
+import shutil
+from pathlib import Path
+
+# Third party modules
+import pytest
+
+# First party modules
+from pynamer import builder, pynamer
+
+BASE_DIR = Path(__file__).parents[0]
+
+
+@pytest.fixture()
+def pre_cleanup(monkeypatch):
+    project_dir = BASE_DIR / "pynamer"
+    project_dir.mkdir()
+    build_dir = BASE_DIR / "build"
+    build_dir.mkdir()
+    dist_dir = BASE_DIR / "dist"
+    dist_dir.mkdir()
+    egg_dir = BASE_DIR / "pynamer.egg-info"
+    egg_dir.mkdir()
+    setup_py = BASE_DIR / "setup.py"
+    setup_py.touch()
+
+    yield
+
+    if (BASE_DIR / "project_name").exists():
+        shutil.rmtree(BASE_DIR / "project_name")
+
+
+def test_cleanup(pre_cleanup, monkeypatch):
+    monkeypatch.setattr(builder, "project_path", BASE_DIR)
+    pynamer._cleanup("pynamer")
+    assert not (BASE_DIR / "build").exists()
+    assert not (BASE_DIR / "dist").exists()
+    assert not (BASE_DIR / "dist" / "pynamer-0.0.0.tar.gz").exists()
+    assert not (BASE_DIR / "dist" / "pynamer-0.0.0-py3-none-any.whl").exists()
+    assert not (BASE_DIR / "pynamer.egg-info").exists()
```

### Comparing `pynamer-1.3.4/tests/test_create_setup_file.py` & `pynamer-2.0.0/tests/test_create_setup_file.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,41 @@
-#!/usr/bin/env python3
-# Core Library modules
-from pathlib import Path
-
-# First party modules
-from pynamer import pynamer
-
-BASE_DIR = Path(__file__).parents[0]
-expected_content = """#!/usr/bin/env python3
-
-
-# Third party modules
-from setuptools import setup
-
-setup(name='pynball',
-      version='0.0.1',
-      description='a new project',
-      url='http://github.com/SK/pynball',
-      author='sking',
-      author_email='sking@gmail.com',
-      license='MIT',
-      packages=['pynball'],
-      zip_safe=False)"""
-
-
-def test_create_setup(create_env, project_path_mock, monkeypatch):
-    inputs = iter(["sking", "sking@gmail.com", "0.0.1", "a new project"])
-    monkeypatch.setattr("builtins.input", lambda _: next(inputs))
-    pynamer._create_setup("pynball")
-    setup_file = BASE_DIR / "setup.py"
-    with open(setup_file, encoding="utf-8") as f:
-        contents = f.read()
-    assert contents == expected_content
-
-    setup_file.unlink()
+#!/usr/bin/env python3
+# Core Library modules
+from pathlib import Path
+
+# First party modules
+from pynamer import builder, pynamer
+
+BASE_DIR = Path(__file__).parents[0]
+expected_content = """#!/usr/bin/env python3
+
+
+# Third party modules
+from setuptools import setup
+
+setup(name='pynball',
+      version='0.0.1',
+      description='a new project',
+      url='http://github.com/SK/pynball',
+      author='sking',
+      author_email='sking@gmail.com',
+      license='MIT',
+      packages=['pynball'],
+      zip_safe=False)"""
+
+
+def test_create_setup(create_env, monkeypatch):
+    inputs = iter(["sking", "sking@gmail.com", "0.0.1", "a new project"])
+    monkeypatch.setattr("builtins.input", lambda _: next(inputs))
+    monkeypatch.setattr(builder, "project_path", BASE_DIR)
+    monkeypatch.setattr(builder, "setup_file_trv", BASE_DIR / "setup.txt")
+    monkeypatch.setattr(builder, "setup_file_py_trv", BASE_DIR / "setup.py")
+    monkeypatch.setattr(builder, "meta_file_trv", BASE_DIR / "meta.pickle")
+
+    builder._create_setup("pynball")
+
+    setup_file = BASE_DIR / "setup.py"
+    with open(setup_file, encoding="utf-8") as f:
+        contents = f.read()
+    assert contents == expected_content
+
+    setup_file.unlink()
```

### Comparing `pynamer-1.3.4/tests/test_defaults.py` & `pynamer-2.0.0/tests/test_defaults.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-#!/usr/bin/env python3
-# Core Library modules
-import platform
-from pathlib import Path
-
-# First party modules
-from pynamer import pynamer
-
-OS = platform.system()
-BASE_DIR = Path(__file__).parents[0]
-
-
-def test_project_path():
-    if OS == "Windows":
-        assert str(pynamer.project_path).endswith("pynamer\\src\\pynamer")
-    else:
-        assert str(pynamer.project_path).endswith("pynamer/src/pynamer")
-
-
-def test_project_count(project_path_mock):
-    assert pynamer.project_count >= 452490
-
-
-def test_setup_text():
-    assert (
-        pynamer.setup_text
-        == """#!/usr/bin/env python3
-
-
-# Third party modules
-from setuptools import setup
-
-setup(name='{{ PROJECT_NAME }}',
-      version='{{ PACKAGE_VERSION }}',
-      description='{{ DESCRIPTION }}',
-      url='http://github.com/SK/{{ PROJECT_NAME }}',
-      author='{{ AUTHOR }}',
-      author_email='{{ EMAIL }}',
-      license='MIT',
-      packages=['{{ PROJECT_NAME }}'],
-      zip_safe=False)
-"""
-    )
-
-
-def test_defaults():
-    assert pynamer.config.pypirc is None
-    assert pynamer.config.original_project_name == "project_name"
-    assert pynamer.config.no_cleanup is False
-    assert pynamer.config.package_version == "0.0.0"
-    assert pynamer.config.pypi_search_url == "https://pypi.org/search/"
-    assert pynamer.config.pypi_project_url == "https://pypi.org/project/"
-    assert pynamer.config.pypi_json_url == "https://pypi.org/pypi/"
-    assert pynamer.config.pypi_simple_index_url == "https://pypi.org/simple/"
-    assert pynamer.config.idlemode == 0
+#!/usr/bin/env python3
+# Core Library modules
+import platform
+from pathlib import Path
+
+# First party modules
+from pynamer import builder, pynamer
+
+OS = platform.system()
+BASE_DIR = Path(__file__).parents[0]
+
+
+def test_project_path():
+    if OS == "Windows":
+        assert str(pynamer.project_path).endswith("pynamer\\src\\pynamer")
+    else:
+        assert str(pynamer.project_path).endswith("pynamer/src/pynamer")
+
+
+def test_project_count(project_path_mock):
+    assert pynamer.project_count >= 452490
+
+
+def test_setup_text():
+    assert (
+        builder.setup_text
+        == """#!/usr/bin/env python3
+
+
+# Third party modules
+from setuptools import setup
+
+setup(name='{{ PROJECT_NAME }}',
+      version='{{ PACKAGE_VERSION }}',
+      description='{{ DESCRIPTION }}',
+      url='http://github.com/SK/{{ PROJECT_NAME }}',
+      author='{{ AUTHOR }}',
+      author_email='{{ EMAIL }}',
+      license='MIT',
+      packages=['{{ PROJECT_NAME }}'],
+      zip_safe=False)
+"""
+    )
+
+
+def test_defaults():
+    assert pynamer.config.pypirc is None
+    assert pynamer.config.original_project_name == "project_name"
+    assert pynamer.config.no_cleanup is False
+    assert pynamer.config.package_version == "0.0.0"
+    assert pynamer.config.pypi_search_url == "https://pypi.org/search/"
+    assert pynamer.config.pypi_project_url == "https://pypi.org/project/"
+    assert pynamer.config.pypi_json_url == "https://pypi.org/pypi/"
+    assert pynamer.config.pypi_simple_index_url == "https://pypi.org/simple/"
+    assert pynamer.config.idlemode == 0
```

### Comparing `pynamer-1.3.4/tests/test_feedback.py` & `pynamer-2.0.0/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.4/tests/test_final_analysis.py` & `pynamer-2.0.0/tests/test_final_analysis.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.4/tests/test_find_pypirc_file.py` & `pynamer-2.0.0/tests/test_find_pypirc_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.4/tests/test_generate_pypi_index.py` & `pynamer-2.0.0/tests/test_generate_pypi_index.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-#!/usr/bin/env python3
-# Core Library modules
-import pickle
-from pathlib import Path
-
-# Third party modules
-import pytest
-import requests
-from requests.exceptions import ConnectTimeout
-
-# First party modules
-from pynamer import pynamer
-
-BASE_DIR = Path(__file__).parents[0]
-
-
-def my_custom_get(url, **kwargs):
-    _pickle_file = BASE_DIR / "resources" / "simple_index.pickle"
-    _pickle_bytes = _pickle_file.read_bytes()
-    pickle_content = pickle.loads(_pickle_bytes)
-    return pickle_content
-
-
-def test_generate_pypi_index(monkeypatch):
-    monkeypatch.setattr(requests, "get", my_custom_get)
-    monkeypatch.setattr(pynamer, "pypi_index_file_trv", BASE_DIR / "pypi_index")
-    monkeypatch.setattr(
-        pynamer, "project_count_file_trv", BASE_DIR / "project_count.pickle"
-    )
-    pynamer._generate_pypi_index()
-    assert (BASE_DIR / "pypi_index").exists()
-    assert (BASE_DIR / "project_count.pickle").exists()
-    (BASE_DIR / "pypi_index").unlink()
-    (BASE_DIR / "project_count.pickle").unlink()
-
-
-def test_generate_pypi_index_error(monkeypatch, project_path_mock):
-    def mock_requests_error(*args, **kwargs):
-        raise ConnectTimeout("Connection timed out")
-
-    monkeypatch.setattr(requests, "get", mock_requests_error)
-
-    with pytest.raises(SystemExit) as excinfo:
-        pynamer._generate_pypi_index()
-    assert str(excinfo.value) == "An error occurred with an HTTP request"
+#!/usr/bin/env python3
+# Core Library modules
+import pickle
+from pathlib import Path
+
+# Third party modules
+import pytest
+import requests
+from requests.exceptions import ConnectTimeout
+
+# First party modules
+from pynamer import pynamer, utils
+
+BASE_DIR = Path(__file__).parents[0]
+
+
+def my_custom_get(url, **kwargs):
+    _pickle_file = BASE_DIR / "resources" / "simple_index.pickle"
+    _pickle_bytes = _pickle_file.read_bytes()
+    pickle_content = pickle.loads(_pickle_bytes)
+    return pickle_content
+
+
+def test_generate_pypi_index(monkeypatch):
+    monkeypatch.setattr(requests, "get", my_custom_get)
+    monkeypatch.setattr(utils, "pypi_index_file_trv", BASE_DIR / "pypi_index")
+    monkeypatch.setattr(
+        utils, "project_count_file_trv", BASE_DIR / "project_count.pickle"
+    )
+    utils._generate_pypi_index()
+
+    assert (BASE_DIR / "pypi_index").exists()
+    assert (BASE_DIR / "project_count.pickle").exists()
+    (BASE_DIR / "pypi_index").unlink()
+    (BASE_DIR / "project_count.pickle").unlink()
+
+
+def test_generate_pypi_index_error(monkeypatch, project_path_mock):
+    def mock_requests_error(*args, **kwargs):
+        raise ConnectTimeout("Connection timed out")
+
+    monkeypatch.setattr(requests, "get", mock_requests_error)
+
+    with pytest.raises(SystemExit) as excinfo:
+        pynamer._generate_pypi_index()
+    assert str(excinfo.value) == "An error occurred with an HTTP request"
```

### Comparing `pynamer-1.3.4/tests/test_ping_json.py` & `pynamer-2.0.0/tests/test_ping_json.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.4/tests/test_ping_project.py` & `pynamer-2.0.0/tests/test_ping_project.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.4/tests/test_process_input_file.py` & `pynamer-2.0.0/tests/test_process_input_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.4/tests/test_pypi_search.py` & `pynamer-2.0.0/tests/test_pypi_search.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.4/tests/test_pypi_search_index.py` & `pynamer-2.0.0/tests/test_pypi_search_index.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-#!/usr/bin/env python3
-# Core Library modules
-from pathlib import Path
-
-# First party modules
-from pynamer import pynamer
-
-BASE_DIR = Path(__file__).parents[0]
-
-
-def test_pypi_search_index(monkeypatch):
-    monkeypatch.setattr(pynamer, "project_path", BASE_DIR / "resources")
-    monkeypatch.setattr(
-        pynamer, "pypi_index_file_trv", BASE_DIR / "resources" / "pypi_index"
-    )
-    assert pynamer._pypi_search_index("pynball") is True
-    assert pynamer._pypi_search_index("zeedonk") is False
+#!/usr/bin/env python3
+# Core Library modules
+from pathlib import Path
+
+# First party modules
+from pynamer import pynamer, validators
+
+BASE_DIR = Path(__file__).parents[0]
+
+
+def test_pypi_search_index(monkeypatch):
+    monkeypatch.setattr(pynamer, "project_path", BASE_DIR / "resources")
+    monkeypatch.setattr(
+        validators, "pypi_index_file_trv", BASE_DIR / "resources" / "pypi_index"
+    )
+    assert pynamer._pypi_search_index("pynball") is True
+    assert pynamer._pypi_search_index("zeedonk") is False
```

### Comparing `pynamer-1.3.4/tests/test_rename_project_dir.py` & `pynamer-2.0.0/tests/test_rename_project_dir.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-#!/usr/bin/env python3
-# Core Library modules
-from pathlib import Path
-
-# Third party modules
-import pytest
-
-# First party modules
-from pynamer import pynamer
-
-BASE_DIR = Path(__file__).parents[0]
-
-
-def test_rename_directory(create_env):
-    old_name = BASE_DIR / "project_name"
-    new_name = BASE_DIR / "pynamer"
-    assert old_name.exists()
-    pynamer._rename_project_dir(str(old_name), str(new_name))
-    assert new_name.exists()
-    pynamer._rename_project_dir(str(new_name), str(old_name))
-
-
-def test_rename_directory_dir_missing(create_env):
-    old_name = BASE_DIR / "project_name1"
-    new_name = BASE_DIR / "pynamer"
-    with pytest.raises(FileNotFoundError):
-        pynamer._rename_project_dir(str(old_name), str(new_name))
+#!/usr/bin/env python3
+# Core Library modules
+from pathlib import Path
+
+# Third party modules
+import pytest
+
+# First party modules
+from pynamer import builder, pynamer
+
+BASE_DIR = Path(__file__).parents[0]
+
+
+def test_rename_directory(create_env):
+    old_name = BASE_DIR / "project_name"
+    new_name = BASE_DIR / "pynamer"
+    assert old_name.exists()
+    pynamer._rename_project_dir(str(old_name), str(new_name))
+    assert new_name.exists()
+    pynamer._rename_project_dir(str(new_name), str(old_name))
+
+
+def test_rename_directory_dir_missing(create_env):
+    old_name = BASE_DIR / "project_name1"
+    new_name = BASE_DIR / "pynamer"
+    with pytest.raises(FileNotFoundError):
+        pynamer._rename_project_dir(str(old_name), str(new_name))
```

### Comparing `pynamer-1.3.4/tests/test_upload_dist.py` & `pynamer-2.0.0/tests/test_upload_dist.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-#!/usr/bin/env python3
-# Core Library modules
-import os
-import sys
-from pathlib import Path
-
-# First party modules
-from pynamer import pynamer
-
-BASE_DIR = Path(__file__).parents[0]
-
-
-def test_dist_upload(monkeypatch, project_path_mock, capsys):
-    captured_args = []
-    python_path = str(sys.executable)
-    pypirc_path = os.fspath(BASE_DIR / ".pypirc")
-    dist_path = os.fspath(BASE_DIR / "dist" / "*")
-
-    def mock_run_command(*args, **kwargs):
-        captured_args.extend(args)
-        return args
-
-    monkeypatch.setattr(pynamer, "_run_command", mock_run_command)
-    monkeypatch.setattr(pynamer.config, "pypirc", pypirc_path)
-
-    pynamer._upload_dist("pynball")
-
-    assert captured_args == [
-        python_path,
-        "-m",
-        "twine",
-        "upload",
-        "--config-file",
-        pypirc_path,
-        dist_path,
-    ]
+#!/usr/bin/env python3
+# Core Library modules
+import os
+import sys
+from pathlib import Path
+
+# First party modules
+from pynamer import builder, pynamer
+
+BASE_DIR = Path(__file__).parents[0]
+
+
+def test_upload_dist(monkeypatch, project_path_mock, capsys):
+    captured_args = []
+    python_path = str(sys.executable)
+    pypirc_path = os.fspath(BASE_DIR / ".pypirc")
+    dist_path = os.fspath(BASE_DIR / "dist" / "*")
+
+    def mock_run_command(*args, **kwargs):
+        captured_args.extend(args)
+        return args
+
+    monkeypatch.setattr(builder, "_run_command", mock_run_command)
+    monkeypatch.setattr(builder, "project_path", BASE_DIR)
+    monkeypatch.setattr(pynamer.config, "pypirc", pypirc_path)
+
+    pynamer._upload_dist("pynball")
+
+    assert captured_args == [
+        python_path,
+        "-m",
+        "twine",
+        "upload",
+        "--config-file",
+        pypirc_path,
+        dist_path,
+    ]
```

### Comparing `pynamer-1.3.4/tests/test_utils_version.py` & `pynamer-2.0.0/tests/test_utils_version.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.4/tests/test_write_output_file.py` & `pynamer-2.0.0/tests/test_write_output_file.py`

 * *Files identical despite different names*

