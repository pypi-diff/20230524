# Comparing `tmp/poetry_plugin_bump-0.0.9.tar.gz` & `tmp/poetry_plugin_bump-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_bump-0.0.9.tar", max compression
+gzip compressed data, was "poetry_plugin_bump-0.1.0.tar", max compression
```

## Comparing `poetry_plugin_bump-0.0.9.tar` & `poetry_plugin_bump-0.1.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2443 2023-03-02 14:07:41.947508 poetry_plugin_bump-0.0.9/poetry_plugin_bump/plugin.py
--rw-r--r--   0        0        0      733 2023-03-02 14:07:41.947508 poetry_plugin_bump-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      773 2023-03-02 14:07:41.947508 poetry_plugin_bump-0.0.9/readme.md
--rw-r--r--   0        0        0     1528 1970-01-01 00:00:00.000000 poetry_plugin_bump-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     2442 2023-05-24 01:04:27.409655 poetry_plugin_bump-0.1.0/poetry_plugin_bump/plugin.py
+-rw-r--r--   0        0        0      740 2023-05-24 01:04:27.409655 poetry_plugin_bump-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      942 2023-05-24 01:04:27.409655 poetry_plugin_bump-0.1.0/readme.md
+-rw-r--r--   0        0        0     1696 1970-01-01 00:00:00.000000 poetry_plugin_bump-0.1.0/PKG-INFO
```

### Comparing `poetry_plugin_bump-0.0.9/poetry_plugin_bump/plugin.py` & `poetry_plugin_bump-0.1.0/poetry_plugin_bump/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def exec(self, bin: str, *args: str) -> int:
         ret = self.env.execute(bin, *args)
         if ret:
             exit(ret)
 
     def handle(self) -> Any:
-        pyproject_folder_path = self.poetry.pyproject._file.path.parent
+        pyproject_folder_path = self.poetry.pyproject.file.path.parent
         pyproject_data = self.poetry.pyproject.data
 
         target: str = self.argument("target_version")
         current_version = pyproject_data["tool"]["poetry"]["version"]
 
         if target == "major":
             target_version = semver.bump_major(current_version)
```

### Comparing `poetry_plugin_bump-0.0.9/pyproject.toml` & `poetry_plugin_bump-0.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "poetry-plugin-bump"
-version = "0.0.9"
+version = "0.1.0"
 description = "poetry plugin to bump version"
 authors = ["trim21"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/trim21/poetry-plugin-bump"
 repository = "https://github.com/trim21/poetry-plugin-bump"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 #
-poetry = "^1.2.0"
-semver = "^2.13.0"
+poetry = ">=1.5.0,<1.6.0"
+semver = "^3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = {version = "^3.0.4", python = "^3.9"}
 
 [tool.poetry.plugins."poetry.application.plugin"]
 bump = "poetry_plugin_bump.plugin:ExecPlugin"
```

### Comparing `poetry_plugin_bump-0.0.9/readme.md` & `poetry_plugin_bump-0.1.0/readme.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 # poetry-plugin-bump
 
 A plugin for poetry to bump version, just like you can in npm.
 
 ## Installation
 
+supported version:
+
+| poetry version  | plugin version |
+|:---------------:|:--------------:|
+| \>=1.2.0,<1.5.0 |     <0.1.0     |
+|    \>=1.5.0     |    >=0.1.0     |
+
 Installation requires poetry 1.2.0+. To install this plugin run:
 
 `poetry self add poetry-plugin-bump`
 
 If your poetry is installed with `pipx`:
 
 ```
```

### Comparing `poetry_plugin_bump-0.0.9/PKG-INFO` & `poetry_plugin_bump-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-bump
-Version: 0.0.9
+Version: 0.1.0
 Summary: poetry plugin to bump version
 Home-page: https://github.com/trim21/poetry-plugin-bump
 License: MIT
 Author: trim21
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: poetry (>=1.2.0,<2.0.0)
-Requires-Dist: semver (>=2.13.0,<3.0.0)
+Requires-Dist: poetry (>=1.5.0,<1.6.0)
+Requires-Dist: semver (>=3.0.0,<4.0.0)
 Project-URL: Repository, https://github.com/trim21/poetry-plugin-bump
 Description-Content-Type: text/markdown
 
 # poetry-plugin-bump
 
 A plugin for poetry to bump version, just like you can in npm.
 
 ## Installation
 
+supported version:
+
+| poetry version  | plugin version |
+|:---------------:|:--------------:|
+| \>=1.2.0,<1.5.0 |     <0.1.0     |
+|    \>=1.5.0     |    >=0.1.0     |
+
 Installation requires poetry 1.2.0+. To install this plugin run:
 
 `poetry self add poetry-plugin-bump`
 
 If your poetry is installed with `pipx`:
 
 ```
```

