# Comparing `tmp/np_envs-0.1.4.tar.gz` & `tmp/np_envs-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_envs-0.1.4.tar", last modified: Tue May 23 22:18:06 2023, max compression
+gzip compressed data, was "np_envs-0.1.5.tar", last modified: Tue May 23 22:53:59 2023, max compression
```

## Comparing `np_envs-0.1.4.tar` & `np_envs-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       93 2023-05-18 06:03:05.768579 np_envs-0.1.4/README.md
--rw-r--r--   0        0        0      639 2023-05-23 22:18:06.945971 np_envs-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      116 2023-05-23 19:33:37.789068 np_envs-0.1.4/src/np_envs/__init__.py
--rw-r--r--   0        0        0      906 2023-05-23 22:03:57.956677 np_envs-0.1.4/src/np_envs/__main__.py
--rw-r--r--   0        0        0     1169 2023-05-18 06:05:48.985287 np_envs-0.1.4/src/np_envs/assets/activate_this.py
--rw-r--r--   0        0        0       87 2023-05-18 05:48:25.501423 np_envs-0.1.4/src/np_envs/assets/example-pip.ini
--rw-r--r--   0        0        0     1500 2023-05-23 19:53:27.225583 np_envs-0.1.4/src/np_envs/config.py
--rw-r--r--   0        0        0     8264 2023-05-23 22:02:33.723563 np_envs-0.1.4/src/np_envs/env.py
--rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 np_envs-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       93 2023-05-18 06:03:05.768579 np_envs-0.1.5/README.md
+-rw-r--r--   0        0        0      639 2023-05-23 22:53:59.463471 np_envs-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      116 2023-05-23 19:33:37.789068 np_envs-0.1.5/src/np_envs/__init__.py
+-rw-r--r--   0        0        0      906 2023-05-23 22:03:57.956677 np_envs-0.1.5/src/np_envs/__main__.py
+-rw-r--r--   0        0        0     1169 2023-05-18 06:05:48.985287 np_envs-0.1.5/src/np_envs/assets/activate_this.py
+-rw-r--r--   0        0        0       87 2023-05-18 05:48:25.501423 np_envs-0.1.5/src/np_envs/assets/example-pip.ini
+-rw-r--r--   0        0        0     1585 2023-05-23 22:27:54.864655 np_envs-0.1.5/src/np_envs/config.py
+-rw-r--r--   0        0        0     8481 2023-05-23 22:30:24.873472 np_envs-0.1.5/src/np_envs/env.py
+-rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 np_envs-0.1.5/PKG-INFO
```

### Comparing `np_envs-0.1.4/pyproject.toml` & `np_envs-0.1.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "np_envs"
-version = "0.1.4"
+version = "0.1.5"
 description = "Config and scripts for managing virtual envs for Mindscope Neuropixels projects."
 authors = [
     { name = "bjhardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "np-config>=0.4.20",
     "np-logging>=0.5.1",
```

### Comparing `np_envs-0.1.4/src/np_envs/__main__.py` & `np_envs-0.1.5/src/np_envs/__main__.py`

 * *Files identical despite different names*

### Comparing `np_envs-0.1.4/src/np_envs/assets/activate_this.py` & `np_envs-0.1.5/src/np_envs/assets/activate_this.py`

 * *Files identical despite different names*

### Comparing `np_envs-0.1.4/src/np_envs/config.py` & `np_envs-0.1.5/src/np_envs/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 ZK_CONFIG_NODE = '/projects/np_envs' 
 CONFIG = np_config.fetch(ZK_CONFIG_NODE)
 
 ROOT = np_config.normalize_path(CONFIG['root'])
 """Root folder for all envs on all platforms."""""
 PLATFORM_ROOT = ROOT / ('win' if sys.platform == 'win32' else 'unix')
 """OS-specific root folder for all envs on this platform."""
-REQUIREMENTS_TXT_ROOT = PLATFORM_ROOT / CONFIG['requirements_txt_dir_relative_to_root']
+REQUIREMENTS_TXT_ROOT: pathlib.Path = PLATFORM_ROOT / CONFIG['requirements_txt_dir_relative_to_root']
 """Where pip requirements are stored. Might not be possible to store in yaml
 for ZooKeeper, so we just use txt files"""
 
+PROJECT_TO_REQUIREMENTS: dict[str, list[str]] = CONFIG['requirements']
 PROJECT_TO_PIP_CONFIG: dict[str, dict] = CONFIG['pip_ini']
 PROJECT_TO_PYTHON_VERSION: dict[str, str] = CONFIG['python_versions']
 DEFAULT_PYTHON_VERSION = PROJECT_TO_PYTHON_VERSION['default']
 """Should be compatible with the most common `np_*` packages in use."""
 
 def add_or_update_config(new_config: dict[str, Any]) -> None:
     logger.debug('Adding or updating %s in ZooKeeper node %s', new_config, ZK_CONFIG_NODE)
```

### Comparing `np_envs-0.1.4/src/np_envs/env.py` & `np_envs-0.1.5/src/np_envs/env.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,28 +121,33 @@
         with open(self.pip_ini, 'w') as f:
             self.pip_ini_config.write(f)
         logger.debug('Pip config written to %s', self.pip_ini)
 
     @property
     def requirements_txt(self) -> pathlib.Path:
         """Path to requirements.txt file (may not exist)."""
-        return config.REQUIREMENTS_TXT_ROOT / f'{self.name}.requirements.txt'
-        
+        path = config.REQUIREMENTS_TXT_ROOT / f'{self.name}.requirements.txt'
+        if not path.exists():
+            requirements = config.PROJECT_TO_REQUIREMENTS.get(self.name)
+            if requirements:
+                path.write_text('\n'.join(requirements))
+        return path
+    
     def update(self, requirements: pathlib.Path | None = None, **kwargs) -> None:
         if not self.python.exists():
             self.create()
         if requirements is None:
             requirements = self.requirements_txt
         if not requirements.exists():
             raise FileNotFoundError(f'Cannot update {self}: {requirements} does not exist')
         logger.info('Updating %s', self)
         self.add_pip_config()
         self.run_update_cmd(requirements, **kwargs)
         logger.info('Finished updating %s', self)
-
+            
     def run_update_cmd(self, requirements: pathlib.Path) -> None:
         subprocess.run(f'{self.python} -m pip install -U -r {requirements}', check=True)
 
     
 class PipManagedConda(PipManaged):
     
     @property
```

### Comparing `np_envs-0.1.4/PKG-INFO` & `np_envs-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-envs
-Version: 0.1.4
+Version: 0.1.5
 Summary: Config and scripts for managing virtual envs for Mindscope Neuropixels projects.
 Author-Email: bjhardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: np-config>=0.4.20
 Requires-Dist: np-logging>=0.5.1
 Requires-Dist: np-tools>=0.1.14
```

