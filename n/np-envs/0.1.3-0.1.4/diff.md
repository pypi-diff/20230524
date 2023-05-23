# Comparing `tmp/np_envs-0.1.3.tar.gz` & `tmp/np_envs-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_envs-0.1.3.tar", last modified: Fri May 19 05:24:31 2023, max compression
+gzip compressed data, was "np_envs-0.1.4.tar", last modified: Tue May 23 22:18:06 2023, max compression
```

## Comparing `np_envs-0.1.3.tar` & `np_envs-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0       93 2023-05-18 06:03:05.768579 np_envs-0.1.3/README.md
--rw-r--r--   0        0        0      541 2023-05-19 05:24:31.705913 np_envs-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       54 2023-05-18 07:49:42.185517 np_envs-0.1.3/src/np_envs/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 06:08:40.452037 np_envs-0.1.3/src/np_envs/__main__.py
--rw-r--r--   0        0        0     1246 2023-05-19 04:35:25.235779 np_envs-0.1.3/src/np_envs/config.py
--rw-r--r--   0        0        0     6915 2023-05-19 05:15:50.702210 np_envs-0.1.3/src/np_envs/env.py
--rw-r--r--   0        0        0       87 2023-05-18 05:48:25.501423 np_envs-0.1.3/src/np_envs/pip.ini
--rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 np_envs-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       93 2023-05-18 06:03:05.768579 np_envs-0.1.4/README.md
+-rw-r--r--   0        0        0      639 2023-05-23 22:18:06.945971 np_envs-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      116 2023-05-23 19:33:37.789068 np_envs-0.1.4/src/np_envs/__init__.py
+-rw-r--r--   0        0        0      906 2023-05-23 22:03:57.956677 np_envs-0.1.4/src/np_envs/__main__.py
+-rw-r--r--   0        0        0     1169 2023-05-18 06:05:48.985287 np_envs-0.1.4/src/np_envs/assets/activate_this.py
+-rw-r--r--   0        0        0       87 2023-05-18 05:48:25.501423 np_envs-0.1.4/src/np_envs/assets/example-pip.ini
+-rw-r--r--   0        0        0     1500 2023-05-23 19:53:27.225583 np_envs-0.1.4/src/np_envs/config.py
+-rw-r--r--   0        0        0     8264 2023-05-23 22:02:33.723563 np_envs-0.1.4/src/np_envs/env.py
+-rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 np_envs-0.1.4/PKG-INFO
```

### Comparing `np_envs-0.1.3/pyproject.toml` & `np_envs-0.1.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 [project]
 name = "np_envs"
-version = "0.1.3"
+version = "0.1.4"
 description = "Config and scripts for managing virtual envs for Mindscope Neuropixels projects."
 authors = [
     { name = "bjhardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "np-config>=0.4.20",
     "np-logging>=0.5.1",
+    "np-tools>=0.1.14",
+    "importlib-resources>=5.12.0",
+    "typer>=0.9.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
+[project.scripts]
+
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm.scripts.pub]
```

### Comparing `np_envs-0.1.3/src/np_envs/config.py` & `np_envs-0.1.4/src/np_envs/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 from __future__ import annotations
 
 import pathlib
 import sys
 from typing import Any
 
+import importlib_resources
 import np_config
 import np_logging
 
 logger = np_logging.getLogger(__name__)
 
+PKG_ROOT = importlib_resources.files(__package__)
+"""This package's root folder in `site-packages`"""
+
 ZK_CONFIG_NODE = '/projects/np_envs' 
 CONFIG = np_config.fetch(ZK_CONFIG_NODE)
 
-ROOT = pathlib.Path(CONFIG['root'])
+ROOT = np_config.normalize_path(CONFIG['root'])
+"""Root folder for all envs on all platforms."""""
 PLATFORM_ROOT = ROOT / ('win' if sys.platform == 'win32' else 'unix')
+"""OS-specific root folder for all envs on this platform."""
 REQUIREMENTS_TXT_ROOT = PLATFORM_ROOT / CONFIG['requirements_txt_dir_relative_to_root']
 """Where pip requirements are stored. Might not be possible to store in yaml
 for ZooKeeper, so we just use txt files"""
 
 PROJECT_TO_PIP_CONFIG: dict[str, dict] = CONFIG['pip_ini']
 PROJECT_TO_PYTHON_VERSION: dict[str, str] = CONFIG['python_versions']
 DEFAULT_PYTHON_VERSION = PROJECT_TO_PYTHON_VERSION['default']
```

### Comparing `np_envs-0.1.3/src/np_envs/env.py` & `np_envs-0.1.4/src/np_envs/env.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,40 +18,50 @@
 import configparser
 import pathlib
 import subprocess
 import sys
 
 import np_config
 import np_logging
+import np_tools
 
 import np_envs.config as config
 
 logger = np_logging.getLogger(__name__)
 
 ON_WINDOWS: bool = sys.platform == 'win32'
 
 class EnvPython:
     
     project_root: pathlib.Path
     """Root folder for all envs for the specified project, and platform/OS."""
     python: pathlib.Path
     """Path to python interpreter in this env."""
-    version: str = config.DEFAULT_PYTHON_VERSION
+    version: str
     """Python version in this env, e.g. '3.8.5' or '3.8.*'"""
     
-    def __init__(self, project_root: pathlib.Path, python_version: str | None = None, **kwargs):
-        if python_version is not None:
-            self.version = python_version
-        self.project_root = np_config.normalize_path(project_root)
+    def __init__(self, project_name_or_root_path: str | pathlib.Path, python_version: str | None = None, **kwargs):
+        path = pathlib.Path(project_name_or_root_path)
+        if len(tuple(path.parents)) == 1:
+            # not a path, just an env name
+            self.project_root = config.PLATFORM_ROOT / path.name
+        else:
+            self.project_root = np_config.normalize_path(path)
+            
+        if python_version is None:
+            python_version = config.PROJECT_TO_PYTHON_VERSION.get(self.name, config.DEFAULT_PYTHON_VERSION)
+        assert python_version and python_version.split('.')[-1] in '*0123456789'
+        self.version = python_version
+        
         if not self.root.exists():
             logger.warning(f'{self!r} does not exist: build with `env.create({self.version})')
             
     def __repr__(self) -> str:
-        return f'{self.__class__.__name__}({self.root})'
-    
+        return f'{self.__class__.__name__}({self.project_root})'
+
     @property
     def name(self) -> str:
         return self.project_root.name
 
     @property
     def root(self) -> pathlib.Path:
         """Root folder for this specific env (e.g. `.venv/`)."""
@@ -59,20 +69,25 @@
     
     def create(self, *args, **kwargs) -> None:
         raise NotImplementedError
     
     def update(self, *args, **kwargs) -> None:
         raise NotImplementedError
     
+    def remove(self, *args, **kwargs) -> None:
+        raise NotImplementedError
+        
+    def activate_shell(self, *args, **kwargs) -> None:
+        raise NotImplementedError
     
 class PipManaged(EnvPython):
     
     def create(self, *args, **kwargs) -> None:
         if self.python.exists():
-            logger.warning(f'{self} already exists at {self.root}: aborting creation.')
+            logger.warning(f'{self.name} {self.version} already exists at {self.root}: aborting creation.')
             return
         logger.info('Creating %s', self)
         self.run_create_cmd(*args, **kwargs)
         logger.info('Finished creating %s', self)
         self.add_pip_config()
         
     
@@ -88,16 +103,17 @@
         """Shared cache, across versions and across env types (not platforms)."""
         return config.ROOT / '.pip-cache'
     
     @property 
     def pip_ini_config(self) -> configparser.ConfigParser:
         pip_ini_config = configparser.ConfigParser()
         pip_ini_config.read_dict(
-                config.PROJECT_TO_PIP_CONFIG.get(self.name, config.PROJECT_TO_PIP_CONFIG['default'])
-            )
+            config.PROJECT_TO_PIP_CONFIG.get(self.name,
+            config.PROJECT_TO_PIP_CONFIG['default']),
+        )
         pip_ini_config.set('global', 'cache-dir', np_config.normalize_path(self.pip_cache).as_posix())
         return pip_ini_config
     
     def add_pip_config(self):
         if not self.root.exists():
             raise FileNotFoundError(f'Cannot add pip config: {self.root} does not exist')
         if not self.pip_ini.parent.exists():
@@ -108,25 +124,27 @@
 
     @property
     def requirements_txt(self) -> pathlib.Path:
         """Path to requirements.txt file (may not exist)."""
         return config.REQUIREMENTS_TXT_ROOT / f'{self.name}.requirements.txt'
         
     def update(self, requirements: pathlib.Path | None = None, **kwargs) -> None:
+        if not self.python.exists():
+            self.create()
         if requirements is None:
             requirements = self.requirements_txt
         if not requirements.exists():
             raise FileNotFoundError(f'Cannot update {self}: {requirements} does not exist')
         logger.info('Updating %s', self)
         self.add_pip_config()
         self.run_update_cmd(requirements, **kwargs)
         logger.info('Finished updating %s', self)
 
     def run_update_cmd(self, requirements: pathlib.Path) -> None:
-        subprocess.run(f'{self.python} -m pip install -r {requirements}', check=True)
+        subprocess.run(f'{self.python} -m pip install -U -r {requirements}', check=True)
 
     
 class PipManagedConda(PipManaged):
     
     @property
     def root(self) -> pathlib.Path:
         return super().root / 'conda'
@@ -137,14 +155,18 @@
     
     def run_create_cmd(self, *args, **kwargs) -> None:
         subprocess.run(
             f'conda create -p {self.root} python={self.version} -y --copy --no-shortcuts {" ".join(args)}',
             check=True,
             )
     
+    def remove(self) -> None:
+        subprocess.run(f'conda env remove -n {self.name} --all -y', check=True)
+        if self.root.exists():
+            self.root.rmdir()
     
 class PipManagedVenv(PipManaged):    
     
     @property
     def root(self) -> pathlib.Path:
         return super().root / '.venv'
     
@@ -159,18 +181,29 @@
         if not conda_env.python.exists():
             conda_env.create('--no-default-packages')
         subprocess.run(
             f'{conda_env.python} -m venv --copies {self.root} {" ".join(args)}',
             check=True,
             )
 
-    def activate(self):
-        activate_file = self.root / ('Scripts' if ON_WINDOWS else 'bin') / 'activate_this.py'
-        exec(activate_file.read_text(), {'__file__': activate_file})
-    
+    def activate(self) -> None:
+        activation_script = self.root / ('Scripts' if ON_WINDOWS else 'bin') / 'activate_this.py'
+        if not activation_script.exists():
+            np_tools.copy(config.PKG_ROOT / 'assets' / activation_script.name, activation_script)
+        exec(activation_script.read_text(), {'__file__': activation_script})
+
+    @property
+    def activate_path(self) -> pathlib.Path:
+        if ON_WINDOWS:
+            return self.root / "scripts" / "activate"
+        return self.root / "bin" / "activate"
+
+    def activate_shell(self) -> None:
+        subprocess.run(self.activate_path, check=True, shell=True)
+
 class EnvPath(pathlib.WindowsPath if ON_WINDOWS else pathlib.PosixPath): # type: ignore
     """
     >>> env = EnvPath('np_pipeline_qc')
     """
 
     version: str
     """Python version to used for any envs, e.g. '3.8.5' or '3.8.*'."""
@@ -197,9 +230,10 @@
     def venv(self) -> EnvPython:
         if not hasattr(self, '_venv'):
             self._venv = PipManagedVenv(self, self.version)
         return self._venv
     
     
 if __name__ == '__main__':
+    PipManagedVenv('np_pipeline_qc')
     import doctest
     doctest.testmod()
```

