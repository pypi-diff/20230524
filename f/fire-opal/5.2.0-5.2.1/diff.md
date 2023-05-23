# Comparing `tmp/fire_opal-5.2.0.tar.gz` & `tmp/fire_opal-5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fire_opal-5.2.0.tar", max compression
+gzip compressed data, was "fire_opal-5.2.1.tar", max compression
```

## Comparing `fire_opal-5.2.0.tar` & `fire_opal-5.2.1.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0    36653 2023-05-02 03:26:14.965359 fire_opal-5.2.0/LICENSE
--rw-r--r--   0        0        0      524 2023-05-02 03:26:14.965359 fire_opal-5.2.0/README.md
--rw-r--r--   0        0        0      743 2023-05-02 03:26:39.862620 fire_opal-5.2.0/fireopal/__init__.py
--rw-r--r--   0        0        0      697 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/admin.py
--rw-r--r--   0        0        0     3120 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/config.py
--rw-r--r--   0        0        0      869 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/constants.py
--rw-r--r--   0        0        0      891 2023-05-02 03:26:39.862620 fire_opal-5.2.0/fireopal/functions/__init__.py
--rw-r--r--   0        0        0      818 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/functions/base.py
--rw-r--r--   0        0        0     1087 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/functions/benchmark.py
--rw-r--r--   0        0        0     1772 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/functions/create_calibration_data.py
--rw-r--r--   0        0        0      979 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/functions/create_mitigation_data.py
--rw-r--r--   0        0        0     1711 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/functions/execute.py
--rw-r--r--   0        0        0      838 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/functions/read_data.py
--rw-r--r--   0        0        0      845 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/functions/show_supported_devices.py
--rw-r--r--   0        0        0     2145 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/functions/solve_qaoa.py
--rw-r--r--   0        0        0     1556 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/functions/validate.py
--rw-r--r--   0        0        0     2724 2023-05-02 03:26:39.854620 fire_opal-5.2.0/pyproject.toml
--rw-r--r--   0        0        0     1247 1970-01-01 00:00:00.000000 fire_opal-5.2.0/setup.py
--rw-r--r--   0        0        0     2717 1970-01-01 00:00:00.000000 fire_opal-5.2.0/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-05-23 22:28:06.351850 fire_opal-5.2.1/LICENSE
+-rw-r--r--   0        0        0      524 2023-05-23 22:28:06.351850 fire_opal-5.2.1/README.md
+-rw-r--r--   0        0        0      743 2023-05-23 22:28:25.419901 fire_opal-5.2.1/fireopal/__init__.py
+-rw-r--r--   0        0        0      697 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/admin.py
+-rw-r--r--   0        0        0     3298 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/config.py
+-rw-r--r--   0        0        0      869 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/constants.py
+-rw-r--r--   0        0        0      891 2023-05-23 22:28:25.419901 fire_opal-5.2.1/fireopal/functions/__init__.py
+-rw-r--r--   0        0        0      818 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/functions/base.py
+-rw-r--r--   0        0        0     1478 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/functions/benchmark.py
+-rw-r--r--   0        0        0     2711 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/functions/create_calibration_data.py
+-rw-r--r--   0        0        0     1435 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/functions/create_mitigation_data.py
+-rw-r--r--   0        0        0     1826 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/functions/execute.py
+-rw-r--r--   0        0        0     1140 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/functions/read_data.py
+-rw-r--r--   0        0        0     1063 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/functions/show_supported_devices.py
+-rw-r--r--   0        0        0     2247 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/functions/solve_qaoa.py
+-rw-r--r--   0        0        0     1643 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/functions/validate.py
+-rw-r--r--   0        0        0     2740 2023-05-23 22:28:25.411901 fire_opal-5.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2717 1970-01-01 00:00:00.000000 fire_opal-5.2.1/PKG-INFO
```

### Comparing `fire_opal-5.2.0/LICENSE` & `fire_opal-5.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.0/README.md` & `fire_opal-5.2.1/README.md`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.0/fireopal/__init__.py` & `fire_opal-5.2.1/fireopal/__init__.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.0/fireopal/admin.py` & `fire_opal-5.2.1/fireopal/admin.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.0/fireopal/config.py` & `fire_opal-5.2.1/fireopal/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,23 +55,29 @@
 
 @global_value("FIRE_OPAL_CONFIG")
 def get_config() -> CoreClientSettings:
     """Returns the global Fire Opal settings."""
     return CoreClientSettings(router=get_default_router, product=Product.FIRE_OPAL)
 
 
-def configure(**kwargs):
-    """Updates the global Fire Opal settings. See `CoreClientSettings`
+def configure(**kwargs) -> None:  # type: ignore
+    """
+    Updates the global Fire Opal settings. See `CoreClientSettings`
     for details on which fields can be updated.
+
+    Parameters
+    ----------
+    **kwargs
+        Arbitrary keyword arguments to update the configuration.
     """
     config = get_config()
     config.update(**kwargs)
 
 
-def configure_api(api_url: str, oidc_url: str):
+def configure_api(api_url: str, oidc_url: str) -> None:
     """Convenience function to configure Fire Opal for API
     routing.
 
     Parameters
     ----------
     api_url : str
         URL of the GraphQL schema
@@ -80,29 +86,29 @@
     """
     client = _get_graphql_client(api_url, CliAuth(oidc_url))
     settings = get_config()
 
     configure(router=ApiRouter(client, settings))
 
 
-def configure_local(resolver: "BaseResolver"):
+def configure_local(resolver: "BaseResolver") -> None:  # type: ignore
     """Convenience function to configure Fire Opal for local
     routing.
 
     Parameters
     ----------
     resolver : BaseResolver
         A local implementation of a workflow resolver which uses
         a registry that implements all of the available Fire Opal
         workflows
     """
     configure(router=LocalRouter(resolver))
 
 
-def configure_organization(organization_slug: str):
+def configure_organization(organization_slug: str) -> None:
     """Convenience function to configure the organization.
 
     Parameters
     ----------
     organization_slug : str
         Unique slug for the organization.
     """
```

### Comparing `fire_opal-5.2.0/fireopal/constants.py` & `fire_opal-5.2.1/fireopal/constants.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.0/fireopal/functions/__init__.py` & `fire_opal-5.2.1/fireopal/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.0/fireopal/functions/base.py` & `fire_opal-5.2.1/fireopal/functions/base.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.0/fireopal/functions/create_mitigation_data.py` & `fire_opal-5.2.1/fireopal/functions/create_mitigation_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,27 +7,48 @@
 #
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
+from typing import Dict
 
 from .base import fire_opal_workflow
 
 
-@fire_opal_workflow("mitigation_workflow")
+@fire_opal_workflow("ibm_mitigation_workflow")
 def create_mitigation_data(
     ibm_device_name: str,
     ibmq_token: str,
     hub: str,
     group: str,
     project: str,
-):
-    """Creates mitigation data for Fire Opal."""
+) -> Dict:
+    """
+    Creates mitigation data for Fire Opal.
+
+    Parameters
+    ----------
+    ibm_device_name : str
+        The device to run mitigation on.
+    ibmq_token : str
+        The IBM token for authentication.
+    hub : str
+        The IBM hub for authentication.
+    group : str
+        The IBM group for authentication.
+    project : str
+        The IBM project for authentication.
+
+    Returns
+    -------
+    Dict
+        Dictionary with workflow output.
+    """
 
     return {
         "ibm_device_name": ibm_device_name,
         "ibmq_token": ibmq_token,
         "hub": hub,
         "group": group,
         "project": project,
```

### Comparing `fire_opal-5.2.0/fireopal/functions/execute.py` & `fire_opal-5.2.1/fireopal/functions/execute.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 @fire_opal_workflow("compile_and_run_workflow", formatter=print_warnings)
 def execute(
     circuits: List[str],
     shot_count: int,
     credentials: Dict[str, Any],
     backend_name: str,
-):
+) -> Dict:
     """
     Execute a batch of `circuits` where `shot_count` measurements are taken per circuit.
 
     Parameters
     ----------
     circuits : List[str]
         A list of quantum circuits in the form of a QASM strings. You may use Qiskit to
@@ -40,14 +40,19 @@
     shot_count : int
         Number of bitstrings that are sampled from the final quantum state.
     credentials : Dict[str, Any]
         The credentials for running circuits on an IBM backend. This dictionary should
         contain key-value entries with keys `token`, `project`, `hub`, and `group`.
     backend_name : str
         The backend device name that should be used to run circuits.
+
+    Returns
+    -------
+    Dict
+        A dictionary containing probability mass functions and warnings.
     """
     return {
         "circuits": circuits,
         "shot_count": shot_count,
         "credentials": credentials,
         "backend_name": backend_name,
     }
```

### Comparing `fire_opal-5.2.0/fireopal/functions/show_supported_devices.py` & `fire_opal-5.2.1/fireopal/functions/show_supported_devices.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,13 +14,25 @@
 
 from typing import Dict
 
 from .base import fire_opal_workflow
 
 
 @fire_opal_workflow("show_supported_devices_workflow")
-def show_supported_devices(credentials: Dict[str, str]):
-    """Shows the current supported devices for Fire Opal."""
+def show_supported_devices(credentials: Dict[str, str]) -> Dict:
+    """
+    Shows the current supported devices for Fire Opal.
+
+    Parameters
+    ----------
+    credentials : Dict[str, str]
+        The hardware provider credentials.
+
+    Returns
+    -------
+    Dict
+        The output of the show supported devices workflow.
+    """
 
     return {
         "credentials": credentials,
     }
```

### Comparing `fire_opal-5.2.0/fireopal/functions/solve_qaoa.py` & `fire_opal-5.2.1/fireopal/functions/validate.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,55 +8,47 @@
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
 from typing import (
+    Any,
     Dict,
-    Optional,
-    Union,
+    List,
 )
 
-import networkx as nx
 from qctrlclient.core import print_warnings
-from sympy import Expr
 
 from .base import fire_opal_workflow
 
 
-@fire_opal_workflow("solve_qaoa_workflow", formatter=print_warnings)
-def solve_qaoa(
-    problem: Union[Expr, nx.Graph],
-    problem_type: str,
-    credentials: Dict[str, str],
-    backend_name: Optional[str] = None,
-):
+@fire_opal_workflow("validate_input_circuits_workflow", formatter=print_warnings)
+def validate(
+    circuits: List[str],
+    credentials: Dict[str, Any],
+    backend_name: str,
+) -> Dict:
     """
-    Solve a QAOA problem.
+    Validate the compatibility of a batch of circuits for Fire Opal.
 
     Parameters
     ----------
-    problem : Union[Expr, nx.Graph]
-        The QAOA problem definition, represented as either an
-        `nx.Graph` or `sympy.Expr`.
-    problem_type : str
-        The class of QAOA problem to solve.
-    credentials : Dict[str, str]
+    circuits : List[str]
+        A list of quantum circuit in the form QASM string. You can use Qiskit to
+        generate these strings.
+    credentials : Dict[str, Any]
         The credentials for running circuits on an IBM backend. This dictionary should
         contain key-value entries with keys `token`, `project`, `hub`, and `group`.
-    backend_name : str, optional
-        The backend device that should be used to run circuits. Defaults to None.
+    backend_name : str
+        The backend device name that will be used to run circuits after validation.
+
+    Returns
+    -------
+    Dict
+        The output of the validate workflow.
     """
-    print(
-        "This function performs multiple circuit executions. "
-        "The total execution time is expected to take a few minutes but will take "
-        "much longer if waiting in the public queue. It is highly recommended to visit "
-        "https://quantum-computing.ibm.com/reservations and make a dedicated reservation.\n"
-    )
-    print("Visit https://quantum-computing.ibm.com/jobs to check your queue position.")
     return {
-        "problem": problem,
-        "problem_type": problem_type,
+        "circuits": circuits,
         "credentials": credentials,
         "backend_name": backend_name,
     }
```

### Comparing `fire_opal-5.2.0/fireopal/functions/validate.py` & `fire_opal-5.2.1/fireopal/functions/solve_qaoa.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,44 +6,62 @@
 # with the License. You may obtain a copy of the License at
 #
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
+from __future__ import annotations
 
 from typing import (
-    Any,
     Dict,
-    List,
+    Optional,
 )
 
+import networkx as nx
 from qctrlclient.core import print_warnings
+from sympy import Expr
 
 from .base import fire_opal_workflow
 
 
-@fire_opal_workflow("validate_input_circuits_workflow", formatter=print_warnings)
-def validate(
-    circuits: List[str],
-    credentials: Dict[str, Any],
-    backend_name: str,
-):
+@fire_opal_workflow("solve_qaoa_workflow", formatter=print_warnings)
+def solve_qaoa(
+    problem: Expr | nx.Graph,
+    problem_type: str,
+    credentials: Dict[str, str],
+    backend_name: Optional[str] = None,
+) -> Dict:
     """
-    Validate the compatibility of a batch of circuits for Fire Opal.
+    Solve a QAOA problem.
 
     Parameters
     ----------
-    circuits : List[str]
-        A list of quantum circuit in the form QASM string. You can use Qiskit to
-        generate these strings.
-    credentials : Dict[str, Any]
+    problem : Expr or nx.Graph
+        The QAOA problem definition, represented as either an
+        `nx.Graph` or `sympy.Expr`.
+    problem_type : str
+        The class of QAOA problem to solve.
+    credentials : Dict[str, str]
         The credentials for running circuits on an IBM backend. This dictionary should
         contain key-value entries with keys `token`, `project`, `hub`, and `group`.
-    backend_name : str
-        The backend device name that will be used to run circuits after validation.
+    backend_name : str, optional
+        The backend device that should be used to run circuits. Defaults to None.
+
+    Returns
+    -------
+    Dict
+        The output of the solve qaoa workflow.
     """
+    print(
+        "This function performs multiple circuit executions. "
+        "The total execution time is expected to take a few minutes but will take "
+        "much longer if waiting in the public queue. It is highly recommended to visit "
+        "https://quantum-computing.ibm.com/reservations and make a dedicated reservation.\n"
+    )
+    print("Visit https://quantum-computing.ibm.com/jobs to check your queue position.")
     return {
-        "circuits": circuits,
+        "problem": problem,
+        "problem_type": problem_type,
         "credentials": credentials,
         "backend_name": backend_name,
     }
```

### Comparing `fire_opal-5.2.0/pyproject.toml` & `fire_opal-5.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fire-opal"
-version = "5.2.0"
+version = "5.2.1"
 description = "Fire Opal Client"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
@@ -74,23 +74,24 @@
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 qctrl-client = "^7.0.0"
 click = "^8.1.0"
 qctrl-commons = "^18.0.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.2"
+pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 pytest-xdist = "^3.2.1"
-pylint = "^2.17.1"
+pylint = "^2.17.4"
 pylint_runner = "^0.6.0"
-black = "^23.1.0"
+black = "^23.3.0"
 isort = "^5.12.0"
-pre-commit = "^3.2.0"
+mypy = "^1.3.0"
+pre-commit = "^3.3.1"
 qctrl-core-workflow-manager = "^2.0.0"
 sphinx = "^5.3.0"
 tomli = "^2.0.1"
 qctrl-sphinx-theme = "~0.1.3"
 
 [tool.black]
 exclude = '''
```

### Comparing `fire_opal-5.2.0/PKG-INFO` & `fire_opal-5.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fire-opal
-Version: 5.2.0
+Version: 5.2.1
 Summary: Fire Opal Client
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
```

