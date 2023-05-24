# Comparing `tmp/kyoslib_py-4.1.0.tar.gz` & `tmp/kyoslib_py-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kyoslib_py-4.1.0.tar", max compression
+gzip compressed data, was "kyoslib_py-4.1.1.tar", max compression
```

## Comparing `kyoslib_py-4.1.0.tar` & `kyoslib_py-4.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1078 2023-04-25 07:30:03.825109 kyoslib_py-4.1.0/LICENSE.txt
--rw-r--r--   0        0        0      944 2023-04-25 07:30:03.825109 kyoslib_py-4.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-25 07:30:03.829109 kyoslib_py-4.1.0/kyoslib_py/__init__.py
--rw-r--r--   0        0        0     8805 2023-04-25 07:30:03.829109 kyoslib_py-4.1.0/kyoslib_py/forward_curve.py
--rw-r--r--   0        0        0    15638 2023-04-25 07:30:03.829109 kyoslib_py-4.1.0/kyoslib_py/front_end.py
--rw-r--r--   0        0        0    24395 2023-04-25 07:30:03.833109 kyoslib_py-4.1.0/kyoslib_py/historical_price.py
--rw-r--r--   0        0        0     3459 2023-04-25 07:30:03.833109 kyoslib_py-4.1.0/kyoslib_py/kyos_api.py
--rw-r--r--   0        0        0     4233 2023-04-25 07:30:03.833109 kyoslib_py-4.1.0/kyoslib_py/kyos_utils.py
--rw-r--r--   0        0        0    45293 2023-04-25 07:30:03.833109 kyoslib_py-4.1.0/kyoslib_py/settings.py
--rw-r--r--   0        0        0    92410 2023-04-25 07:30:03.833109 kyoslib_py-4.1.0/kyoslib_py/simulation.py
--rw-r--r--   0        0        0    21363 2023-04-25 07:30:03.833109 kyoslib_py-4.1.0/kyoslib_py/tradable_product.py
--rw-r--r--   0        0        0    36060 2023-04-25 07:30:03.833109 kyoslib_py-4.1.0/kyoslib_py/valuation_interface.py
--rw-r--r--   0        0        0     1061 2023-04-25 07:30:03.833109 kyoslib_py-4.1.0/pyproject.toml
--rw-r--r--   0        0        0     1901 1970-01-01 00:00:00.000000 kyoslib_py-4.1.0/setup.py
--rw-r--r--   0        0        0     1872 1970-01-01 00:00:00.000000 kyoslib_py-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-24 10:04:53.877723 kyoslib_py-4.1.1/LICENSE.txt
+-rw-r--r--   0        0        0      944 2023-05-24 10:04:53.877723 kyoslib_py-4.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-24 10:04:53.881723 kyoslib_py-4.1.1/kyoslib_py/__init__.py
+-rw-r--r--   0        0        0     8805 2023-05-24 10:04:53.881723 kyoslib_py-4.1.1/kyoslib_py/forward_curve.py
+-rw-r--r--   0        0        0    15638 2023-05-24 10:04:53.881723 kyoslib_py-4.1.1/kyoslib_py/front_end.py
+-rw-r--r--   0        0        0    24395 2023-05-24 10:04:53.881723 kyoslib_py-4.1.1/kyoslib_py/historical_price.py
+-rw-r--r--   0        0        0     3459 2023-05-24 10:04:53.881723 kyoslib_py-4.1.1/kyoslib_py/kyos_api.py
+-rw-r--r--   0        0        0     4233 2023-05-24 10:04:53.881723 kyoslib_py-4.1.1/kyoslib_py/kyos_utils.py
+-rw-r--r--   0        0        0    45293 2023-05-24 10:04:53.881723 kyoslib_py-4.1.1/kyoslib_py/settings.py
+-rw-r--r--   0        0        0    92420 2023-05-24 10:04:53.881723 kyoslib_py-4.1.1/kyoslib_py/simulation.py
+-rw-r--r--   0        0        0    21363 2023-05-24 10:04:53.881723 kyoslib_py-4.1.1/kyoslib_py/tradable_product.py
+-rw-r--r--   0        0        0    36060 2023-05-24 10:04:53.881723 kyoslib_py-4.1.1/kyoslib_py/valuation_interface.py
+-rw-r--r--   0        0        0     1061 2023-05-24 10:04:53.881723 kyoslib_py-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1901 1970-01-01 00:00:00.000000 kyoslib_py-4.1.1/setup.py
+-rw-r--r--   0        0        0     1872 1970-01-01 00:00:00.000000 kyoslib_py-4.1.1/PKG-INFO
```

### Comparing `kyoslib_py-4.1.0/LICENSE.txt` & `kyoslib_py-4.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kyoslib_py-4.1.0/README.md` & `kyoslib_py-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `kyoslib_py-4.1.0/kyoslib_py/forward_curve.py` & `kyoslib_py-4.1.1/kyoslib_py/forward_curve.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-4.1.0/kyoslib_py/front_end.py` & `kyoslib_py-4.1.1/kyoslib_py/front_end.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-4.1.0/kyoslib_py/historical_price.py` & `kyoslib_py-4.1.1/kyoslib_py/historical_price.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-4.1.0/kyoslib_py/kyos_api.py` & `kyoslib_py-4.1.1/kyoslib_py/kyos_api.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-4.1.0/kyoslib_py/kyos_utils.py` & `kyoslib_py-4.1.1/kyoslib_py/kyos_utils.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-4.1.0/kyoslib_py/settings.py` & `kyoslib_py-4.1.1/kyoslib_py/settings.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-4.1.0/kyoslib_py/simulation.py` & `kyoslib_py-4.1.1/kyoslib_py/simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1615,27 +1615,27 @@
                 start_date = self.get_trading_date()
             # End Date
             if end_date is None:
                 end_date = self.get_end_date()
 
             sim_other_dir = Path(self.get_other_sim_folder_path())
             if not sim_other_dir.exists():
-                SimulationError(message=sim_other_dir + ' does not not exist!')
+                SimulationError(message=sim_other_dir.name + ' does not not exist!')
 
             if series_type.lower() == 'volume' or series_type.lower() == "renewable":
                 suffix = ""
                 if series_type.lower() == "renewable":
                     suffix = "RenewableAsset_"
                 # Declare input file name and the path
                 inputFilePath = sim_other_dir.joinpath(
                     'VolumeSims_' + suffix + str(series_identifier) + '.mat'
                 )
 
                 if not inputFilePath.exists():
-                    SimulationError(message=inputFilePath + 'does not exist!')
+                    SimulationError(message=inputFilePath.name + 'does not exist!')
 
                 # Import Volume Simulations
                 try:
                     f = h5py.File(inputFilePath, 'r')
                     raw_data = f['VolumeSim'][()].T
                     raw_data = pd.DataFrame(raw_data)
                 except:
```

### Comparing `kyoslib_py-4.1.0/kyoslib_py/tradable_product.py` & `kyoslib_py-4.1.1/kyoslib_py/tradable_product.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-4.1.0/kyoslib_py/valuation_interface.py` & `kyoslib_py-4.1.1/kyoslib_py/valuation_interface.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-4.1.0/pyproject.toml` & `kyoslib_py-4.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kyoslib_py"
-version = "4.1.0"
+version = "4.1.1"
 description = "KYOS shared lib code as python package"
 authors = ["KYOS <support@kyos.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "http://github.com/kyosenergy/kyoslib_py"
 documentation = "https://kyosenergy.github.io/kyoslib_py/"
 
@@ -15,22 +15,22 @@
 requests = "^2.28.1"
 h5py = "^3.6.0"
 numba = "0.56.4"
 plotly = "^5.7.0"
 mkdocstrings-python = "^0.8.2"
 
 [tool.poetry.dev-dependencies]
-invoke = "^2.0.0"
+invoke = "^2.1.0"
 pytest = "^7.3"
 pytest-cov = "^4.0.0"
 black = "^23.3.0"
 isort = "^5.8.0"
 safety = "^2.0.0"
-mkdocs-material = "^9.1.6"
-mkdocstrings = "^0.19.1"
+mkdocs-material = "^9.1.9"
+mkdocstrings = "^0.21.2"
 darglint = "^1.8.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
```

### Comparing `kyoslib_py-4.1.0/setup.py` & `kyoslib_py-4.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'requests>=2.28.1,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['run_model = src.entry:main']}
 
 setup_kwargs = {
     'name': 'kyoslib-py',
-    'version': '4.1.0',
+    'version': '4.1.1',
     'description': 'KYOS shared lib code as python package',
     'long_description': "# kyoslib_py\n\n## Usage\n\nExample code:\n\n```python\nfrom kyoslib_py.simulation import Simulation\nsimulation_set = Simulation()\n```\n\n## Installation\n\n```pip install kyoslib_py```\n\n## Dependencies\n\nPython 3.7+\n\n## Development\n\nThis project is executing CI checks using **GitHub actions**.\n\nIt will run `pytest` and `black`.\n\n### Invoking development tasks\n\n[Invoke](https://www.pyinvoke.org/) is used for development tasks.\n\nTasks are stored in `tasks.py` and are executable using the `inv[oke]` command line tool.\n\nTo see the list of tasks, you can type:\n\n```bash\ninv --list\n```\n\nFor example, before your commits, you should run\n```bash\ninv format\n```\nto format your code.\n\n## Documentation\n\nThe package documentation is generated by MkDocs. The correct version can be installed in the project's virtual environment by:\n\n```bash\npoetry install\n```\n\nThen the documentation can be built, and a server to view it started by:\n\n```bash\nmkdocs serve\n```\n",
     'author': 'KYOS',
     'author_email': 'support@kyos.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'http://github.com/kyosenergy/kyoslib_py',
```

### Comparing `kyoslib_py-4.1.0/PKG-INFO` & `kyoslib_py-4.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kyoslib-py
-Version: 4.1.0
+Version: 4.1.1
 Summary: KYOS shared lib code as python package
 Home-page: http://github.com/kyosenergy/kyoslib_py
 License: MIT
 Author: KYOS
 Author-email: support@kyos.com
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
```

