# Comparing `tmp/ansys_dpf_composites-0.2b1.tar.gz` & `tmp/ansys_dpf_composites-0.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_dpf_composites-0.2b1.tar", max compression
+gzip compressed data, was "ansys_dpf_composites-0.2b2.tar", max compression
```

## Comparing `ansys_dpf_composites-0.2b1.tar` & `ansys_dpf_composites-0.2b2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1089 2023-03-30 14:59:01.473503 ansys_dpf_composites-0.2b1/LICENSE
--rw-r--r--   0        0        0     6073 2023-03-30 14:59:01.473503 ansys_dpf_composites-0.2b1/README.rst
--rw-r--r--   0        0        0     3709 2023-03-30 14:59:01.477503 ansys_dpf_composites-0.2b1/pyproject.toml
--rw-r--r--   0        0        0      666 2023-03-30 14:59:01.477503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/__init__.py
--rw-r--r--   0        0        0     7464 2023-03-30 14:59:01.477503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/_indexer.py
--rw-r--r--   0        0        0      132 2023-03-30 14:59:01.477503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/_typing_helper.py
--rw-r--r--   0        0        0    25401 2023-03-30 14:59:01.477503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/composite_model.py
--rw-r--r--   0        0        0      726 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/constants.py
--rw-r--r--   0        0        0    11041 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/data_sources.py
--rw-r--r--   0        0        0     8001 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/example_helper/__init__.py
--rw-r--r--   0        0        0     1030 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/__init__.py
--rw-r--r--   0        0        0     4276 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_combined_failure_criterion.py
--rw-r--r--   0        0        0     1355 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_core_failure.py
--rw-r--r--   0        0        0     6866 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_cuntze.py
--rw-r--r--   0        0        0     2461 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_face_sheet_wrinkling.py
--rw-r--r--   0        0        0     2094 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_failure_criterion_base.py
--rw-r--r--   0        0        0     3247 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_hashin.py
--rw-r--r--   0        0        0      630 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_hoffman.py
--rw-r--r--   0        0        0     4053 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_larc.py
--rw-r--r--   0        0        0     8874 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_max_strain.py
--rw-r--r--   0        0        0     4705 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_max_stress.py
--rw-r--r--   0        0        0     9183 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_puck.py
--rw-r--r--   0        0        0     1192 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_quadratic_failure_criterion.py
--rw-r--r--   0        0        0     1901 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_shear_crimping.py
--rw-r--r--   0        0        0      641 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_tsai_hill.py
--rw-r--r--   0        0        0      629 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_tsai_wu.py
--rw-r--r--   0        0        0     2324 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_von_mises.py
--rw-r--r--   0        0        0      912 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/layup_info/__init__.py
--rw-r--r--   0        0        0     2879 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/layup_info/_add_layup_info_to_mesh.py
--rw-r--r--   0        0        0      398 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/layup_info/_enums.py
--rw-r--r--   0        0        0    19828 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/layup_info/_layup_info.py
--rw-r--r--   0        0        0     4071 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/layup_info/material_operators.py
--rw-r--r--   0        0        0     8676 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/layup_info/material_properties.py
--rw-r--r--   0        0        0        0 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/py.typed
--rw-r--r--   0        0        0    10613 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/result_definition.py
--rw-r--r--   0        0        0    29595 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/sampling_point.py
--rw-r--r--   0        0        0     6039 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/select_indices.py
--rw-r--r--   0        0        0      332 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/server_helpers/__init__.py
--rw-r--r--   0        0        0     3586 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/server_helpers/_connect_to_or_start_server.py
--rw-r--r--   0        0        0     2801 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/server_helpers/_load_plugin.py
--rw-r--r--   0        0        0     1944 2023-03-30 14:59:01.481503 ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/unit_system.py
--rw-r--r--   0        0        0     8835 1970-01-01 00:00:00.000000 ansys_dpf_composites-0.2b1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-04 09:31:11.035109 ansys_dpf_composites-0.2b2/LICENSE
+-rw-r--r--   0        0        0     5800 2023-04-04 09:31:11.035109 ansys_dpf_composites-0.2b2/README.rst
+-rw-r--r--   0        0        0     3711 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/pyproject.toml
+-rw-r--r--   0        0        0      666 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/__init__.py
+-rw-r--r--   0        0        0     7464 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/_indexer.py
+-rw-r--r--   0        0        0      132 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/_typing_helper.py
+-rw-r--r--   0        0        0    25401 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/composite_model.py
+-rw-r--r--   0        0        0      726 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/constants.py
+-rw-r--r--   0        0        0    11041 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/data_sources.py
+-rw-r--r--   0        0        0     8001 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/example_helper/__init__.py
+-rw-r--r--   0        0        0     1030 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/__init__.py
+-rw-r--r--   0        0        0     4276 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_combined_failure_criterion.py
+-rw-r--r--   0        0        0     1355 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_core_failure.py
+-rw-r--r--   0        0        0     6866 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_cuntze.py
+-rw-r--r--   0        0        0     2461 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_face_sheet_wrinkling.py
+-rw-r--r--   0        0        0     2094 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_failure_criterion_base.py
+-rw-r--r--   0        0        0     3247 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_hashin.py
+-rw-r--r--   0        0        0      630 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_hoffman.py
+-rw-r--r--   0        0        0     4053 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_larc.py
+-rw-r--r--   0        0        0     8874 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_max_strain.py
+-rw-r--r--   0        0        0     4705 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_max_stress.py
+-rw-r--r--   0        0        0     9183 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_puck.py
+-rw-r--r--   0        0        0     1192 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_quadratic_failure_criterion.py
+-rw-r--r--   0        0        0     1901 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_shear_crimping.py
+-rw-r--r--   0        0        0      641 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_tsai_hill.py
+-rw-r--r--   0        0        0      629 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_tsai_wu.py
+-rw-r--r--   0        0        0     2324 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_von_mises.py
+-rw-r--r--   0        0        0      912 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/layup_info/__init__.py
+-rw-r--r--   0        0        0     2879 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/layup_info/_add_layup_info_to_mesh.py
+-rw-r--r--   0        0        0      398 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/layup_info/_enums.py
+-rw-r--r--   0        0        0    19828 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/layup_info/_layup_info.py
+-rw-r--r--   0        0        0     4071 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/layup_info/material_operators.py
+-rw-r--r--   0        0        0     8676 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/layup_info/material_properties.py
+-rw-r--r--   0        0        0        0 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/py.typed
+-rw-r--r--   0        0        0    10613 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/result_definition.py
+-rw-r--r--   0        0        0    29595 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/sampling_point.py
+-rw-r--r--   0        0        0     6039 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/select_indices.py
+-rw-r--r--   0        0        0      332 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/server_helpers/__init__.py
+-rw-r--r--   0        0        0     3586 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/server_helpers/_connect_to_or_start_server.py
+-rw-r--r--   0        0        0     2801 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/server_helpers/_load_plugin.py
+-rw-r--r--   0        0        0     1944 2023-04-04 09:31:11.039109 ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/unit_system.py
+-rw-r--r--   0        0        0     8556 1970-01-01 00:00:00.000000 ansys_dpf_composites-0.2b2/PKG-INFO
```

### Comparing `ansys_dpf_composites-0.2b1/LICENSE` & `ansys_dpf_composites-0.2b2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/README.rst` & `ansys_dpf_composites-0.2b2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -77,21 +77,16 @@
 
 #.  Create a virtual environment and install the package with development
     dependencies. PyDPF Composites uses `Poetry <https://python-poetry.org>`_
     to manage the development environment.
 
     .. code:: bash
 
-        poetry config installer.modern-installation false
         poetry install --all-extras
 
-    Setting ``installer.modern-installation`` to ``false`` is a temporary workaround.
-    See `this pydata-sphinx-theme issue <https://github.com/pydata/pydata-sphinx-theme/issues/1253>`_
-    for more information.
-
 
 #.  Activate the virtual environment:
 
     .. code:: bash
 
         poetry shell
```

### Comparing `ansys_dpf_composites-0.2b1/pyproject.toml` & `ansys_dpf_composites-0.2b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 # Check https://python-poetry.org/docs/pyproject/ for all available sections
 name = "ansys-dpf-composites"
-version = "0.2b1"
+version = "0.2b2"
 description = "A python wrapper for ansys dpf composites"
 license = "MIT"
 authors = ["ANSYS, Inc. <ansys.support@ansys.com>"]
 maintainers = ["PyAnsys developers <pyansys.maintainers@ansys.com>"]
 readme = "README.rst"
 repository = "https://github.com/pyansys/pydpf-composites"
 documentation = "https://composites.dpf.docs.pyansys.com"
@@ -40,15 +40,15 @@
 sphinx-design = {version = "^0.3.0", optional = true}
 pypandoc = {version = "^1.8.1", optional = true}
 pytest = {version = "^7.1.2", optional = true}
 pytest-cov = {version = "^3.0.0", optional = true}
 mypy = {version = "^0.931", optional = true}
 mypy-extensions = {version = "^0.4.3", optional = true}
 # If this version changes also the link in doc/src/conf.py intersphinx-mapping has to change
-ansys-dpf-core = "^0.7.3"
+ansys-dpf-core = ">=0.8,<1"
 vtk = {version = "*"}
 matplotlib = {version = "^3.5.0"}
 pyvista = {version = "^0.36.1"}
 pre-commit = {version = "*", optional = true}
 # Upper bound because there is a problem with examples in versions > 1.20.1
 sphinx-autodoc-typehints = {version = "^1.19,<1.20.2", optional = true}
 pylint = {version = "^2.13", optional = true}
```

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/__init__.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/_indexer.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/_indexer.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/composite_model.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/composite_model.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/constants.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/constants.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/data_sources.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/data_sources.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/example_helper/__init__.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/example_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/__init__.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_combined_failure_criterion.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_combined_failure_criterion.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_core_failure.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_core_failure.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_cuntze.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_cuntze.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_face_sheet_wrinkling.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_face_sheet_wrinkling.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_failure_criterion_base.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_failure_criterion_base.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_hashin.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_hashin.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_hoffman.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_hoffman.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_larc.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_larc.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_max_strain.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_max_strain.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_max_stress.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_max_stress.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_puck.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_puck.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_quadratic_failure_criterion.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_quadratic_failure_criterion.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_shear_crimping.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_shear_crimping.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_tsai_hill.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_tsai_hill.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_tsai_wu.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_tsai_wu.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/failure_criteria/_von_mises.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/failure_criteria/_von_mises.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/layup_info/__init__.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/layup_info/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/layup_info/_add_layup_info_to_mesh.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/layup_info/_add_layup_info_to_mesh.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/layup_info/_layup_info.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/layup_info/_layup_info.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/layup_info/material_operators.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/layup_info/material_operators.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/layup_info/material_properties.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/layup_info/material_properties.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/result_definition.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/result_definition.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/sampling_point.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/sampling_point.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/select_indices.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/select_indices.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/server_helpers/_connect_to_or_start_server.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/server_helpers/_connect_to_or_start_server.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/server_helpers/_load_plugin.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/server_helpers/_load_plugin.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/src/ansys/dpf/composites/unit_system.py` & `ansys_dpf_composites-0.2b2/src/ansys/dpf/composites/unit_system.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.2b1/PKG-INFO` & `ansys_dpf_composites-0.2b2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-dpf-composites
-Version: 0.2b1
+Version: 0.2b2
 Summary: A python wrapper for ansys dpf composites
 Home-page: https://github.com/pyansys/pydpf-composites
 License: MIT
 Author: ANSYS, Inc.
 Author-email: ansys.support@ansys.com
 Maintainer: PyAnsys developers
 Maintainer-email: pyansys.maintainers@ansys.com
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: all
 Provides-Extra: build
 Provides-Extra: docs
 Provides-Extra: pre-commit
 Provides-Extra: test
 Requires-Dist: Sphinx (>=5.0.1,<6.0.0) ; extra == "all" or extra == "docs"
-Requires-Dist: ansys-dpf-core (>=0.7.3,<0.8.0)
+Requires-Dist: ansys-dpf-core (>=0.8,<1)
 Requires-Dist: ansys-sphinx-theme (>=0,<1) ; extra == "all" or extra == "docs"
 Requires-Dist: build (>=0.8.0,<0.9.0) ; extra == "all" or extra == "build"
 Requires-Dist: importlib-metadata (>=4.0,<5.0) ; python_version < "3.8"
 Requires-Dist: matplotlib (>=3.5.0,<4.0.0)
 Requires-Dist: mypy (>=0.931,<0.932) ; extra == "all" or extra == "pre-commit"
 Requires-Dist: mypy-extensions (>=0.4.3,<0.5.0) ; extra == "all" or extra == "pre-commit"
 Requires-Dist: numpy (>=1.19,<1.22) ; python_version >= "3.7" and python_version < "3.8"
@@ -130,21 +130,16 @@
 
 #.  Create a virtual environment and install the package with development
     dependencies. PyDPF Composites uses `Poetry <https://python-poetry.org>`_
     to manage the development environment.
 
     .. code:: bash
 
-        poetry config installer.modern-installation false
         poetry install --all-extras
 
-    Setting ``installer.modern-installation`` to ``false`` is a temporary workaround.
-    See `this pydata-sphinx-theme issue <https://github.com/pydata/pydata-sphinx-theme/issues/1253>`_
-    for more information.
-
 
 #.  Activate the virtual environment:
 
     .. code:: bash
 
         poetry shell
```

