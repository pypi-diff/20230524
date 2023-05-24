# Comparing `tmp/predictable-0.0.1.tar.gz` & `tmp/predictable-0.0.2.tar.gz`

## Comparing `predictable-0.0.1.tar` & `predictable-0.0.2.tar`

### file list

```diff
@@ -1,34 +1,37 @@
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 predictable-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 predictable-0.0.1/.readthedocs.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 predictable-0.0.1/examples/__init__.py
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 predictable-0.0.1/examples/model.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 predictable-0.0.1/examples/rpt.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 predictable-0.0.1/examples/run.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 predictable-0.0.1/examples/input/modelpoints.csv
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 predictable-0.0.1/examples/input/modelpoints.rpt
--rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 predictable-0.0.1/examples/tables/economic.csv
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 predictable-0.0.1/examples/tables/lapses.csv
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 predictable-0.0.1/examples/tables/sa8990.csv
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 predictable-0.0.1/predictable/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 predictable-0.0.1/predictable/core/__init__.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 predictable-0.0.1/predictable/core/discounting.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 predictable-0.0.1/predictable/core/flows.py
--rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 predictable-0.0.1/predictable/core/io.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 predictable-0.0.1/predictable/core/lookup.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 predictable-0.0.1/predictable/core/model.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 predictable-0.0.1/predictable/core/precision.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 predictable-0.0.1/predictable/core/rating_factors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 predictable-0.0.1/predictable/engine/__init__.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 predictable-0.0.1/predictable/engine/run.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 predictable-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 predictable-0.0.1/tests/test_discounting.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 predictable-0.0.1/tests/test_flows.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 predictable-0.0.1/tests/test_lookup.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 predictable-0.0.1/tests/test_model.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 predictable-0.0.1/tests/test_precision.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 predictable-0.0.1/tests/test_run.py
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 predictable-0.0.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 predictable-0.0.1/LICENSE
--rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 predictable-0.0.1/README.md
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 predictable-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 predictable-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 predictable-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 predictable-0.0.2/.readthedocs.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 predictable-0.0.2/examples/__init__.py
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 predictable-0.0.2/examples/model.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 predictable-0.0.2/examples/rpt.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 predictable-0.0.2/examples/run.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 predictable-0.0.2/examples/input/modelpoints.csv
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 predictable-0.0.2/examples/input/modelpoints.rpt
+-rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 predictable-0.0.2/examples/tables/economic.csv
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 predictable-0.0.2/examples/tables/lapses.csv
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 predictable-0.0.2/examples/tables/sa8990.csv
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 predictable-0.0.2/predictable/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 predictable-0.0.2/predictable/__main__.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 predictable-0.0.2/predictable/cli/__init__.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 predictable-0.0.2/predictable/cli/scaffold.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 predictable-0.0.2/predictable/core/__init__.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 predictable-0.0.2/predictable/core/discounting.py
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 predictable-0.0.2/predictable/core/flows.py
+-rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 predictable-0.0.2/predictable/core/io.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 predictable-0.0.2/predictable/core/lookup.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 predictable-0.0.2/predictable/core/model.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 predictable-0.0.2/predictable/core/precision.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 predictable-0.0.2/predictable/core/rating_factors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 predictable-0.0.2/predictable/engine/__init__.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 predictable-0.0.2/predictable/engine/run.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 predictable-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 predictable-0.0.2/tests/test_discounting.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 predictable-0.0.2/tests/test_flows.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 predictable-0.0.2/tests/test_lookup.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 predictable-0.0.2/tests/test_model.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 predictable-0.0.2/tests/test_precision.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 predictable-0.0.2/tests/test_run.py
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 predictable-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 predictable-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 predictable-0.0.2/README.md
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 predictable-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 predictable-0.0.2/PKG-INFO
```

### Comparing `predictable-0.0.1/examples/model.py` & `predictable-0.0.2/examples/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     # Add components that have a projected value
     prem = pr.CashFlow(
         input_array=[modelpoint.premium],
         formula=lambda prev: prev * 1.05,
         label="premium",
     )
     cover = pr.CashFlow(input_array=[modelpoint.cover], label="cover")
-    exp = pr.StaticFlow(
+    exp = pr.StaticCashFlow(
         input_array=[modelpoint.expenses for _ in range(5)],
         label="expense",
     )
 
     # Add actuarial components
     qx = pr.TableLookup(
         table_name=kwargs["table_location"] / "sa8990.csv",
```

### Comparing `predictable-0.0.1/examples/run.py` & `predictable-0.0.2/examples/run.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from predictable import RunConfig, dataclass
 
 from model import handler
 
 
-# This is just the pydantic dataclass
+# You define what a modelpoint looks like
 @dataclass
 class ModelPoint:
     policy_number: str
     age: int
     gender: str
     smoker_status: str
     premium: float
```

### Comparing `predictable-0.0.1/examples/tables/economic.csv` & `predictable-0.0.2/examples/tables/economic.csv`

 * *Files identical despite different names*

### Comparing `predictable-0.0.1/examples/tables/sa8990.csv` & `predictable-0.0.2/examples/tables/sa8990.csv`

 * *Files identical despite different names*

### Comparing `predictable-0.0.1/predictable/core/discounting.py` & `predictable-0.0.2/predictable/core/discounting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from numpy.typing import ArrayLike
 from pandas import DataFrame
 
-from .flows import StaticFlow
+from .flows import StaticCashFlow
 
 
 def i_to_v(i: float) -> float:
     """Convert interest rate i to discount factor
     where discount factor = 1 / (1 + interest rate)
 
     :param i: Interest rate
@@ -38,22 +38,22 @@
     def __array_finalize__(self, obj):
         if obj is None:
             return
         self.interest_rate = getattr(obj, "interest_rate", None)
         self.formula = getattr(obj, "formula", lambda i: i)
         self.label = getattr(obj, "label", None)
 
-    def project(self, term: int, results: DataFrame) -> StaticFlow:
+    def project(self, term: int, results: DataFrame) -> StaticCashFlow:
         """This method is used to handle the projection logic for the component.
 
         :param term: Term over which to project
         :type term: int
         :return: StaticDiscountFactors object containing projected values
         :rtype: StaticDiscountFactors
         """
         results = self
         for n in range(1, term + 1):
             results = np.append(results, i_to_v(self.formula(self.interest_rate)) ** n)
-        return StaticFlow(
+        return StaticCashFlow(
             input_array=results,
             label=self.label,
         )
```

### Comparing `predictable-0.0.1/predictable/core/flows.py` & `predictable-0.0.2/predictable/core/flows.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 from numpy.typing import ArrayLike
 from pandas import DataFrame
 
 from .precision import get_precision
 
 
-class StaticFlow(np.ndarray):
+class StaticCashFlow(np.ndarray):
     """
     Static cashflow object created from an Array-Like object.
     Subclasses numpy.ndarray
     """
 
     def __new__(cls, input_array: ArrayLike, label: str = None):
         # We first cast to be our class type
@@ -25,25 +25,25 @@
         self.label = getattr(obj, "label", None)
 
     def project(self, term: int, results: DataFrame):
         """This method is used to handle the projection logic for the component.
 
         :param term: Term over which to project
         :type term: int
-        :return: StaticFlow object containing projected values
-        :rtype: StaticFlow
+        :return: StaticCashFlow object containing projected values
+        :rtype: StaticCashFlow
         """
         if len(self) == term:
             return self
         elif len(self) < term:
             results = np.append(self, (term - len(self) + 1) * [0])
-            return StaticFlow(input_array=results, label=self.label)
+            return StaticCashFlow(input_array=results, label=self.label)
         elif len(self) > term:
             results = self[: term + 1]
-            return StaticFlow(input_array=results, label=self.label)
+            return StaticCashFlow(input_array=results, label=self.label)
 
 
 class CashFlow(np.ndarray):
     """CashFlow object created from an Array-Like object. Subclasses numpy.ndarray"""
 
     def __new__(
         cls,
@@ -55,36 +55,36 @@
         obj = np.asarray(input_array).view(cls)
         # add new attributes to the created instance
         obj.label = label
         obj.formula = formula
         # Finally, we must return the newly created object:
         if len(input_array) > 1:
             raise ValueError(
-                "Use StaticFlow instead if you wish to pre-populate cashflows.",
+                "Use StaticCashFlow instead if you wish to pre-populate cashflows.",
                 input_array,
             )
         return obj
 
     def __array_finalize__(self, obj):
         if obj is None:
             return
         self.label = getattr(obj, "label", None)
         self.formula = getattr(obj, "formula", lambda x: x)
 
-    def project(self, term: int, results: DataFrame) -> StaticFlow:
+    def project(self, term: int, results: DataFrame) -> StaticCashFlow:
         """This method is used to handle the projection logic for the component.
 
         :param term: Term over which to project
         :type term: int
-        :return: StaticFlow object containing projected values
-        :rtype: StaticFlow
+        :return: StaticCashFlow object containing projected values
+        :rtype: StaticCashFlow
         """
         results = self
         for _ in range(0, term):
             results = np.append(
                 results,
                 round(
                     self.formula(results[-1]),
                     get_precision(),
                 ),
             )
-        return StaticFlow(input_array=results, label=self.label)
+        return StaticCashFlow(input_array=results, label=self.label)
```

### Comparing `predictable-0.0.1/predictable/core/io.py` & `predictable-0.0.2/predictable/core/io.py`

 * *Files identical despite different names*

### Comparing `predictable-0.0.1/predictable/core/lookup.py` & `predictable-0.0.2/predictable/core/lookup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 from typing import Any, List
 
 import numpy as np
 from pandas import DataFrame, read_csv
 
-from .flows import StaticFlow
+from .flows import StaticCashFlow
 
 
 class TableLookup(np.ndarray):
     """RiskRates object created from an Array-Like object. Subclasses numpy.ndarray"""
 
     def __new__(
         cls,
@@ -42,27 +42,27 @@
             return
         self.table_name = getattr(obj, "table_name", None)
         self.label = getattr(obj, "label", None)
         self.lookup_on = getattr(obj, "lookup_on", [])
         self.keep_column = getattr(obj, "keep_column", [])
         self.default_value = getattr(obj, "default_value", [])
 
-    def project(self, term: int, results: DataFrame) -> StaticFlow:
+    def project(self, term: int, results: DataFrame) -> StaticCashFlow:
         """This method is used to handle the projection logic for the component.
 
         :param term: Term over which to project
         :type term: int
-        :return: StaticFlow object containing projected values
-        :rtype: StaticFlow
+        :return: StaticCashFlow object containing projected values
+        :rtype: StaticCashFlow
         """
         table = read_csv(Path(self.table_name))
 
         # join the table and the results
         results = results.join(table, on=self.lookup_on, how="left", rsuffix="_table")[
             self.keep_column
         ]
 
         # Optionally handle nulls
         if self.default_value is not None:
             results = results.replace(np.NaN, self.default_value)
 
-        return StaticFlow(input_array=results, label=self.label)
+        return StaticCashFlow(input_array=results, label=self.label)
```

### Comparing `predictable-0.0.1/predictable/core/model.py` & `predictable-0.0.2/predictable/core/model.py`

 * *Files identical despite different names*

### Comparing `predictable-0.0.1/predictable/core/precision.py` & `predictable-0.0.2/predictable/core/precision.py`

 * *Files identical despite different names*

### Comparing `predictable-0.0.1/predictable/core/rating_factors.py` & `predictable-0.0.2/predictable/core/rating_factors.py`

 * *Files identical despite different names*

### Comparing `predictable-0.0.1/predictable/engine/run.py` & `predictable-0.0.2/predictable/engine/run.py`

 * *Files identical despite different names*

### Comparing `predictable-0.0.1/tests/test_discounting.py` & `predictable-0.0.2/tests/test_discounting.py`

 * *Files identical despite different names*

### Comparing `predictable-0.0.1/tests/test_flows.py` & `predictable-0.0.2/tests/test_flows.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 from pandas import DataFrame
-from predictable import CashFlow, StaticFlow
+from predictable import CashFlow, StaticCashFlow
 
 
 def test_cashflow_setup():
     c = CashFlow(input_array=[100], label="test")
     assert c.label == "test"
     assert len(c) == 1
     assert c.sum() == 100
@@ -25,21 +25,21 @@
 )
 def test_cashflow_formula_projection(input_value, formula, output_value):
     c = CashFlow(label="test", input_array=[input_value], formula=formula)
     results = c.project(term=1, results=DataFrame())
     assert results[-1] == output_value
 
 
-def test_staticflow_setup():
-    s = StaticFlow(label="test", input_array=[1, 2, 3])
+def test_StaticCashFlow_setup():
+    s = StaticCashFlow(label="test", input_array=[1, 2, 3])
     assert s.label == "test"
     assert len(s) == 3
     assert s.sum() == 6
 
 
 @pytest.mark.parametrize(
     "projected_period, projected_sum", [(10, 1.5), (1, 1.0), (3, 1.5)]
 )
 def test_static_discounting_projections(projected_period, projected_sum):
-    d = StaticFlow([0.5, 0.5, 0.5], label="test")
+    d = StaticCashFlow([0.5, 0.5, 0.5], label="test")
     results = d.project(projected_period, results=DataFrame())
     assert results.sum() == projected_sum
```

### Comparing `predictable-0.0.1/tests/test_lookup.py` & `predictable-0.0.2/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `predictable-0.0.1/tests/test_precision.py` & `predictable-0.0.2/tests/test_precision.py`

 * *Files identical despite different names*

### Comparing `predictable-0.0.1/tests/test_run.py` & `predictable-0.0.2/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `predictable-0.0.1/.gitignore` & `predictable-0.0.2/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 test.py
 .vscode/
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 output/
+tmp/
+predictable_project/
 
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
```

### Comparing `predictable-0.0.1/LICENSE` & `predictable-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `predictable-0.0.1/README.md` & `predictable-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 ## Quick start example
 
 A `model.py` file will be used to house the modelling logic which will be applied to each modelpoint.
 
 ```python
 # import the library
-from predictable import CashFlow, DiscountFactors, Model, StaticFlow
+from predictable import CashFlow, DiscountFactors, Model, StaticCashFlow
 
 # Create new model instance
 model = Model()
 
 # Add a premium component
 model.add_component(
     CashFlow(
@@ -37,15 +37,15 @@
 )
 
 # Add a sum assured component
 model.add_component(CashFlow(label="cover", input_array=[1_000_000]))
 
 # Add an expense component
 model.add_component(
-    StaticFlow(
+    StaticCashFlow(
         input_array=[10, 10, 10, 10, 10],
         label="expense",
     )
 )
 
 # Add discounting component
 model.add_component(DiscountFactors(interest_rate=0.05, label="V"))
```

### Comparing `predictable-0.0.1/pyproject.toml` & `predictable-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,79 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.sdist]
-exclude = [
-  "/.github",
-  "/docs",
-]
+exclude = ["/.github", "/docs"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["predictable"]
 
 [project]
 name = "predictable"
 description = "A framework for actuarial modelling."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.11"
 authors = [{ name = "Ratul Maharaj", email = "ratulmaharaj@gmail.com" }]
 classifiers = [
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
+  "Programming Language :: Python :: 3",
 ]
-dependencies = ["numpy==1.24.3", "pandas==2.0.1", "pydantic==1.10.7", "pre-commit==3.3.1", "ruff==0.0.264", "black==23.3.0"]
+dependencies = ["numpy==1.24.3", "pandas==2.0.1", "pydantic==1.10.7"]
 dynamic = ["version"]
-keywords = ["actuarial", "modelling", "financial services", "python", "predictable"]
+keywords = [
+  "actuarial",
+  "modelling",
+  "financial services",
+  "python",
+  "predictable",
+]
 
 [project.urls]
 "Bug Tracker" = "https://github.com/RatulMaharaj/predictable/issues"
 homepage = "https://github.com/RatulMaharaj/predictable"
 documentation = "https://predictable.readthedocs.io"
 
+[project.scripts]
+predictable = "predictable.cli:cli"
+
 [tool.hatch.version]
 path = "predictable/__init__.py"
 
-[tool.hatch.envs.default]
-post-install-commands = ["pre-commit install"]
-
 [tool.hatch.envs.default.scripts]
 test = "hatch run test:test"
+lint = "hatch run dev:lint"
+format = "hatch run dev:format"
+example = "python examples/rpt.py"
+
+[tool.hatch.envs.dev]
+post-install-commands = ["pre-commit install"]
+
+[tool.hatch.envs.dev.scripts]
 lint = "ruff check ."
 format = "black ."
-example = "python examples/rpt.py"
 
 # Test environment
 [tool.hatch.envs.test]
 dependencies = ["pytest"]
 
 [tool.hatch.envs.test.scripts]
 test = "pytest"
 
 # Docs environment
 [tool.hatch.envs.docs]
-dependencies = ["sphinx", "sphinx-copybutton", "sphinxext-opengraph", "myst-parser", "furo"]
+dependencies = [
+  "sphinx",
+  "sphinx-copybutton",
+  "sphinxext-opengraph",
+  "myst-parser",
+  "furo",
+]
 
 [tool.hatch.envs.docs.scripts]
 build = "sphinx-build -b html docs docs/_build"
 serve = ["cd docs/_build/html && python -m http.server"]
 
 # Formatter settings
 [tool.black]
```

### Comparing `predictable-0.0.1/PKG-INFO` & `predictable-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: predictable
-Version: 0.0.1
+Version: 0.0.2
 Summary: A framework for actuarial modelling.
 Project-URL: Bug Tracker, https://github.com/RatulMaharaj/predictable/issues
 Project-URL: homepage, https://github.com/RatulMaharaj/predictable
 Project-URL: documentation, https://predictable.readthedocs.io
 Author-email: Ratul Maharaj <ratulmaharaj@gmail.com>
 License: MIT License
         
@@ -17,20 +17,17 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 License-File: LICENSE
 Keywords: actuarial,financial services,modelling,predictable,python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
-Requires-Dist: black==23.3.0
 Requires-Dist: numpy==1.24.3
 Requires-Dist: pandas==2.0.1
-Requires-Dist: pre-commit==3.3.1
 Requires-Dist: pydantic==1.10.7
-Requires-Dist: ruff==0.0.264
 Description-Content-Type: text/markdown
 
 # Predictable
 
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 ![PyPI](https://img.shields.io/pypi/v/predictable)
@@ -51,15 +48,15 @@
 
 ## Quick start example
 
 A `model.py` file will be used to house the modelling logic which will be applied to each modelpoint.
 
 ```python
 # import the library
-from predictable import CashFlow, DiscountFactors, Model, StaticFlow
+from predictable import CashFlow, DiscountFactors, Model, StaticCashFlow
 
 # Create new model instance
 model = Model()
 
 # Add a premium component
 model.add_component(
     CashFlow(
@@ -68,15 +65,15 @@
 )
 
 # Add a sum assured component
 model.add_component(CashFlow(label="cover", input_array=[1_000_000]))
 
 # Add an expense component
 model.add_component(
-    StaticFlow(
+    StaticCashFlow(
         input_array=[10, 10, 10, 10, 10],
         label="expense",
     )
 )
 
 # Add discounting component
 model.add_component(DiscountFactors(interest_rate=0.05, label="V"))
```

