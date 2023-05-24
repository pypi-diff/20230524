# Comparing `tmp/neptune-tensorboard-0.5.1.tar.gz` & `tmp/neptune_tensorboard-1.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/neptune-tensorboard-0.5.1.tar", last modified: Wed Nov  4 10:13:42 2020, max compression
+gzip compressed data, was "neptune_tensorboard-1.0.0rc0.tar", max compression
```

## Comparing `neptune-tensorboard-0.5.1.tar` & `neptune_tensorboard-1.0.0rc0.tar`

### file list

```diff
@@ -1,43 +1,9 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-04 10:13:42.000000 neptune-tensorboard-0.5.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2020-11-04 10:13:42.000000 neptune-tensorboard-0.5.1/VERSION
--rw-rw-r--   0 travis    (2000) travis    (2000)       63 2020-11-04 10:09:08.000000 neptune-tensorboard-0.5.1/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      203 2020-11-04 10:09:08.000000 neptune-tensorboard-0.5.1/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      831 2020-11-04 10:13:42.000000 neptune-tensorboard-0.5.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4140 2020-11-04 10:09:08.000000 neptune-tensorboard-0.5.1/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1543 2020-11-04 10:09:08.000000 neptune-tensorboard-0.5.1/git_version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-04 10:13:42.000000 neptune-tensorboard-0.5.1/neptune_tensorboard/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-04 10:13:42.000000 neptune-tensorboard-0.5.1/neptune_tensorboard/integration/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10432 2020-11-04 10:09:08.000000 neptune-tensorboard-0.5.1/neptune_tensorboard/integration/tensorflow_integration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      596 2020-11-04 10:09:08.000000 neptune-tensorboard-0.5.1/neptune_tensorboard/integration/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-04 10:13:42.000000 neptune-tensorboard-0.5.1/neptune_tensorboard/internal/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1435 2020-11-04 10:09:08.000000 neptune-tensorboard-0.5.1/neptune_tensorboard/internal/deprecations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      596 2020-11-04 10:09:08.000000 neptune-tensorboard-0.5.1/neptune_tensorboard/internal/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-04 10:13:42.000000 neptune-tensorboard-0.5.1/neptune_tensorboard/sync/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-04 10:13:42.000000 neptune-tensorboard-0.5.1/neptune_tensorboard/sync/internal/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1832 2020-11-04 10:09:08.000000 neptune-tensorboard-0.5.1/neptune_tensorboard/sync/internal/path_parser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1016 2020-11-04 10:09:08.000000 neptune-tensorboard-0.5.1/neptune_tensorboard/sync/internal/events_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      596 2020-11-04 10:09:08.000000 neptune-tensorboard-0.5.1/neptune_tensorboard/sync/internal/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      979 2020-11-04 10:09:08.000000 neptune-tensorboard-0.5.1/neptune_tensorboard/sync/sync.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      716 2020-11-04 10:09:08.000000 neptune-tensorboard-0.5.1/neptune_tensorboard/sync/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6030 2020-11-04 10:09:08.000000 neptune-tensorboard-0.5.1/neptune_tensorboard/sync/tensorflow_data_sync.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1119 2020-11-04 10:09:08.000000 neptune-tensorboard-0.5.1/neptune_tensorboard/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       61 2020-11-04 10:13:42.000000 neptune-tensorboard-0.5.1/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-04 10:13:42.000000 neptune-tensorboard-0.5.1/neptune_tensorboard_plugin/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1541 2020-11-04 10:09:08.000000 neptune-tensorboard-0.5.1/neptune_tensorboard_plugin/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-04 10:13:42.000000 neptune-tensorboard-0.5.1/neptune_tensorboard.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      831 2020-11-04 10:13:42.000000 neptune-tensorboard-0.5.1/neptune_tensorboard.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-11-04 10:13:42.000000 neptune-tensorboard-0.5.1/neptune_tensorboard.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       53 2020-11-04 10:13:42.000000 neptune-tensorboard-0.5.1/neptune_tensorboard.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1075 2020-11-04 10:13:42.000000 neptune-tensorboard-0.5.1/neptune_tensorboard.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      203 2020-11-04 10:13:42.000000 neptune-tensorboard-0.5.1/neptune_tensorboard.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       65 2020-11-04 10:13:42.000000 neptune-tensorboard-0.5.1/neptune_tensorboard.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2831 2020-11-04 10:09:08.000000 neptune-tensorboard-0.5.1/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-04 10:13:42.000000 neptune-tensorboard-0.5.1/tests/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-04 10:13:42.000000 neptune-tensorboard-0.5.1/tests/neptune_tensorboard/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-04 10:13:42.000000 neptune-tensorboard-0.5.1/tests/neptune_tensorboard/sync/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-04 10:13:42.000000 neptune-tensorboard-0.5.1/tests/neptune_tensorboard/sync/internal/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4270 2020-11-04 10:09:08.000000 neptune-tensorboard-0.5.1/tests/neptune_tensorboard/sync/internal/test_path_parser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      596 2020-11-04 10:09:08.000000 neptune-tensorboard-0.5.1/tests/neptune_tensorboard/sync/internal/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      596 2020-11-04 10:09:08.000000 neptune-tensorboard-0.5.1/tests/neptune_tensorboard/sync/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      596 2020-11-04 10:09:08.000000 neptune-tensorboard-0.5.1/tests/neptune_tensorboard/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      596 2020-11-04 10:09:08.000000 neptune-tensorboard-0.5.1/tests/__init__.py
+-rw-r--r--   0        0        0      416 2023-05-24 14:17:24.834326 neptune_tensorboard-1.0.0rc0/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-05-24 14:17:24.834326 neptune_tensorboard-1.0.0rc0/LICENSE
+-rw-r--r--   0        0        0     3420 2023-05-24 14:17:24.834326 neptune_tensorboard-1.0.0rc0/README.md
+-rw-r--r--   0        0        0     2639 2023-05-24 14:17:38.422524 neptune_tensorboard-1.0.0rc0/pyproject.toml
+-rw-r--r--   0        0        0      750 2023-05-24 14:17:24.834326 neptune_tensorboard-1.0.0rc0/src/neptune_tensorboard/__init__.py
+-rw-r--r--   0        0        0     1960 2023-05-24 14:17:24.834326 neptune_tensorboard-1.0.0rc0/src/neptune_tensorboard/integration/__init__.py
+-rw-r--r--   0        0        0     3232 2023-05-24 14:17:24.834326 neptune_tensorboard-1.0.0rc0/src/neptune_tensorboard/integration/tensorflow_integration.py
+-rw-r--r--   0        0        0      742 2023-05-24 14:17:24.834326 neptune_tensorboard-1.0.0rc0/src/neptune_tensorboard/integration/version.py
+-rw-r--r--   0        0        0     5399 1970-01-01 00:00:00.000000 neptune_tensorboard-1.0.0rc0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `neptune-tensorboard-0.5.1/neptune_tensorboard/integration/__init__.py` & `neptune_tensorboard-1.0.0rc0/src/neptune_tensorboard/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,7 +9,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+__all__ = ["enable_tensorboard_logging", "__version__"]
+
+from neptune_tensorboard.integration import (
+    __version__,
+    enable_tensorboard_logging,
+)
```

