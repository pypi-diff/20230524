# Comparing `tmp/acrod-1.1.3.tar.gz` & `tmp/acrod-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acrod-1.1.3.tar", last modified: Sat May 20 12:04:49 2023, max compression
+gzip compressed data, was "acrod-1.1.4.tar", last modified: Wed May 24 14:50:22 2023, max compression
```

## Comparing `acrod-1.1.3.tar` & `acrod-1.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 12:04:49.694766 acrod-1.1.3/
--rw-r--r--   0 apple      (501) staff       (20)    35149 2023-04-12 12:17:39.000000 acrod-1.1.3/LICENSE
--rw-r--r--   0 apple      (501) staff       (20)    44795 2023-05-20 12:04:49.693597 acrod-1.1.3/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)     3529 2023-05-20 12:04:14.000000 acrod-1.1.3/README.md
--rw-r--r--   0 apple      (501) staff       (20)      873 2023-05-20 12:04:21.000000 acrod-1.1.3/pyproject.toml
--rw-r--r--   0 apple      (501) staff       (20)       38 2023-05-20 12:04:49.695074 acrod-1.1.3/setup.cfg
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 12:04:49.674618 acrod-1.1.3/src/
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 12:04:49.680992 acrod-1.1.3/src/acrod/
--rw-r--r--   0 apple      (501) staff       (20)        0 2023-05-20 11:54:40.000000 acrod-1.1.3/src/acrod/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    42322 2023-05-20 11:54:40.000000 acrod-1.1.3/src/acrod/functions.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 12:04:49.688570 acrod-1.1.3/src/acrod.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)    44795 2023-05-20 12:04:49.000000 acrod-1.1.3/src/acrod.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      264 2023-05-20 12:04:49.000000 acrod-1.1.3/src/acrod.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2023-05-20 12:04:49.000000 acrod-1.1.3/src/acrod.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)       12 2023-05-20 12:04:49.000000 acrod-1.1.3/src/acrod.egg-info/requires.txt
--rw-r--r--   0 apple      (501) staff       (20)        6 2023-05-20 12:04:49.000000 acrod-1.1.3/src/acrod.egg-info/top_level.txt
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 12:04:49.689833 acrod-1.1.3/tests/
--rw-r--r--   0 apple      (501) staff       (20)   236428 2023-05-20 11:54:40.000000 acrod-1.1.3/tests/test_jacobian.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-24 14:50:22.946897 acrod-1.1.4/
+-rw-r--r--   0 apple      (501) staff       (20)    35149 2023-04-12 12:17:39.000000 acrod-1.1.4/LICENSE
+-rw-r--r--   0 apple      (501) staff       (20)    45222 2023-05-24 14:50:22.945755 acrod-1.1.4/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)     3956 2023-05-20 16:44:06.000000 acrod-1.1.4/README.md
+-rw-r--r--   0 apple      (501) staff       (20)      873 2023-05-24 14:47:53.000000 acrod-1.1.4/pyproject.toml
+-rw-r--r--   0 apple      (501) staff       (20)       38 2023-05-24 14:50:22.947327 acrod-1.1.4/setup.cfg
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-24 14:50:22.916937 acrod-1.1.4/src/
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-24 14:50:22.924657 acrod-1.1.4/src/acrod/
+-rw-r--r--   0 apple      (501) staff       (20)        0 2023-05-20 11:54:40.000000 acrod-1.1.4/src/acrod/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    42544 2023-05-23 14:24:19.000000 acrod-1.1.4/src/acrod/functions.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-24 14:50:22.935763 acrod-1.1.4/src/acrod.egg-info/
+-rw-r--r--   0 apple      (501) staff       (20)    45222 2023-05-24 14:50:22.000000 acrod-1.1.4/src/acrod.egg-info/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)      264 2023-05-24 14:50:22.000000 acrod-1.1.4/src/acrod.egg-info/SOURCES.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2023-05-24 14:50:22.000000 acrod-1.1.4/src/acrod.egg-info/dependency_links.txt
+-rw-r--r--   0 apple      (501) staff       (20)       12 2023-05-24 14:50:22.000000 acrod-1.1.4/src/acrod.egg-info/requires.txt
+-rw-r--r--   0 apple      (501) staff       (20)        6 2023-05-24 14:50:22.000000 acrod-1.1.4/src/acrod.egg-info/top_level.txt
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-24 14:50:22.937556 acrod-1.1.4/tests/
+-rw-r--r--   0 apple      (501) staff       (20)   236428 2023-05-20 11:54:40.000000 acrod-1.1.4/tests/test_jacobian.py
```

### Comparing `acrod-1.1.3/LICENSE` & `acrod-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `acrod-1.1.3/PKG-INFO` & `acrod-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acrod
-Version: 1.1.3
+Version: 1.1.4
 Summary: Automatic Computation for Robot Design (ACRoD)
 Author-email: Suneesh Jacob Akkarapakam <suneeshjacob@gmail.com>, Rituparna Datta <rituparndatta@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -695,14 +695,21 @@
 
 This repository is dedicated to develop functions for automatic computations for designing robotic manipulators.
 
 ## Currently available functions
 
 - Jacobian formulation for planar and spatial manipulators around a given end-effector point. (This is useful in performing optimisation of Jacobian-based performance parameters of any non-redundant robot directly from its robot-topology matrix)
 
+## Installation
+
+The package can be installed from PyPI by using the following command via terminal.
+```shell
+pip install acrod
+```
+
 ## Usage
 
 ### Jacobian for planar manipulators
 
 The topological information of a robot is to be specified by using its robot-topology matrix, as defined [here](Robot_Topology_Matrix.md). For a planar 2R serial manipulator, the robot topology matrix is given by
 
 $$\left[\begin{matrix}
@@ -711,15 +718,15 @@
 0 & 1 & 9
 \end{matrix}\right]$$
 
 The corresponding Jacobian function can be formulated as follows.
 
 Firstly, the required functions are imported as shown below.
 ```py
-from src.acrod.functions import jacobian
+from acrod.functions import jacobian
 from numpy import matrix
 ```
 
 
 The robot-topology matrix for 3R planar serial manipulator is defined and jacobian information is processed via the imported jacobian class as follows.
 ```py
 M = matrix('9 1 0;1 9 1;0 1 9')
@@ -729,15 +736,15 @@
 
 Jacobian function is generated as shown below.
 ```py
 jacobian_function = jac.get_jacobian_function()
 ```
 
 
-Symbolic Jacobian is extracted from `jacobian_information` as follows.
+In the process of generating the above jacobian function, other attributes of the jacobian object also are updated. Symbolic Jacobian matrices can be extracted from the attributes. Since this is a serial robot, the matrix $J_a$ itself would be the Jacobian matrix of the manipulator. The matrix $J_a$ is extracted from `Ja` attribute of the jacobian object as follows.
 ```py
 symbolic_jacobian = jac.Ja
 symbolic_jacobian
 ```
 
 In an ipynb file of JupyterLab, the above code would produce the following output.
```

### Comparing `acrod-1.1.3/README.md` & `acrod-1.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 
 This repository is dedicated to develop functions for automatic computations for designing robotic manipulators.
 
 ## Currently available functions
 
 - Jacobian formulation for planar and spatial manipulators around a given end-effector point. (This is useful in performing optimisation of Jacobian-based performance parameters of any non-redundant robot directly from its robot-topology matrix)
 
+## Installation
+
+The package can be installed from PyPI by using the following command via terminal.
+```shell
+pip install acrod
+```
+
 ## Usage
 
 ### Jacobian for planar manipulators
 
 The topological information of a robot is to be specified by using its robot-topology matrix, as defined [here](Robot_Topology_Matrix.md). For a planar 2R serial manipulator, the robot topology matrix is given by
 
 $$\left[\begin{matrix}
@@ -20,15 +27,15 @@
 0 & 1 & 9
 \end{matrix}\right]$$
 
 The corresponding Jacobian function can be formulated as follows.
 
 Firstly, the required functions are imported as shown below.
 ```py
-from src.acrod.functions import jacobian
+from acrod.functions import jacobian
 from numpy import matrix
 ```
 
 
 The robot-topology matrix for 3R planar serial manipulator is defined and jacobian information is processed via the imported jacobian class as follows.
 ```py
 M = matrix('9 1 0;1 9 1;0 1 9')
@@ -38,15 +45,15 @@
 
 Jacobian function is generated as shown below.
 ```py
 jacobian_function = jac.get_jacobian_function()
 ```
 
 
-Symbolic Jacobian is extracted from `jacobian_information` as follows.
+In the process of generating the above jacobian function, other attributes of the jacobian object also are updated. Symbolic Jacobian matrices can be extracted from the attributes. Since this is a serial robot, the matrix $J_a$ itself would be the Jacobian matrix of the manipulator. The matrix $J_a$ is extracted from `Ja` attribute of the jacobian object as follows.
 ```py
 symbolic_jacobian = jac.Ja
 symbolic_jacobian
 ```
 
 In an ipynb file of JupyterLab, the above code would produce the following output.
```

### Comparing `acrod-1.1.3/pyproject.toml` & `acrod-1.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "acrod"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="Suneesh Jacob Akkarapakam", email="suneeshjacob@gmail.com" },
   { name="Rituparna Datta", email="rituparndatta@gmail.com" }
 ]
 description = "Automatic Computation for Robot Design (ACRoD)"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `acrod-1.1.3/src/acrod/functions.py` & `acrod-1.1.4/src/acrod/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,22 +365,25 @@
         return Ja_func, Jp_func, Aa_func, Ap_func, active_jointvelocities, passive_jointvelocities, decision_variables_str
 
     def process_functions(self):
         self.get_all_paths()
         self.get_independent_paths()
         self.execute_equations()
 
-    def get_jacobian_function(self):
+    def get_jacobian_function(self, MoorePenrose = False):
         self.process_functions()
         Ja = self.Ja_func
         if self.is_serial == False:
             Jp = self.Jp_func
             Aa = self.Aa_func
             Ap = self.Ap_func
-            J = lambda a,x: numpy.matrix(Ja(a,x)) - numpy.matrix(Jp(a,x))*numpy.linalg.inv(numpy.matrix(Ap(a,x)))*numpy.matrix(Aa(a,x))
+            if MoorePenrose == True:
+                J = lambda a,x: numpy.matrix(Ja(a,x)) - numpy.matrix(Jp(a,x))*numpy.linalg.pinv(numpy.matrix(Ap(a,x)))*numpy.matrix(Aa(a,x))
+            else:
+                J = lambda a,x: numpy.matrix(Ja(a,x)) - numpy.matrix(Jp(a,x))*numpy.linalg.inv(numpy.matrix(Ap(a,x)))*numpy.matrix(Aa(a,x))
         else:
             J = lambda a,x: numpy.matrix(Ja(a,x))
         return J
 
 def vel_path_planar(M, path, available_variables):
     """
     vel_path_planar function processes the strings to be executed for symbolic variabes and velocity expressions of a given path by using the robot-topology matrix, and it also updates the available_variables (so that only those variables that are unavailable are added, thereby avoiding redundancy). this is for planar manipulators.
```

### Comparing `acrod-1.1.3/src/acrod.egg-info/PKG-INFO` & `acrod-1.1.4/src/acrod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acrod
-Version: 1.1.3
+Version: 1.1.4
 Summary: Automatic Computation for Robot Design (ACRoD)
 Author-email: Suneesh Jacob Akkarapakam <suneeshjacob@gmail.com>, Rituparna Datta <rituparndatta@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -695,14 +695,21 @@
 
 This repository is dedicated to develop functions for automatic computations for designing robotic manipulators.
 
 ## Currently available functions
 
 - Jacobian formulation for planar and spatial manipulators around a given end-effector point. (This is useful in performing optimisation of Jacobian-based performance parameters of any non-redundant robot directly from its robot-topology matrix)
 
+## Installation
+
+The package can be installed from PyPI by using the following command via terminal.
+```shell
+pip install acrod
+```
+
 ## Usage
 
 ### Jacobian for planar manipulators
 
 The topological information of a robot is to be specified by using its robot-topology matrix, as defined [here](Robot_Topology_Matrix.md). For a planar 2R serial manipulator, the robot topology matrix is given by
 
 $$\left[\begin{matrix}
@@ -711,15 +718,15 @@
 0 & 1 & 9
 \end{matrix}\right]$$
 
 The corresponding Jacobian function can be formulated as follows.
 
 Firstly, the required functions are imported as shown below.
 ```py
-from src.acrod.functions import jacobian
+from acrod.functions import jacobian
 from numpy import matrix
 ```
 
 
 The robot-topology matrix for 3R planar serial manipulator is defined and jacobian information is processed via the imported jacobian class as follows.
 ```py
 M = matrix('9 1 0;1 9 1;0 1 9')
@@ -729,15 +736,15 @@
 
 Jacobian function is generated as shown below.
 ```py
 jacobian_function = jac.get_jacobian_function()
 ```
 
 
-Symbolic Jacobian is extracted from `jacobian_information` as follows.
+In the process of generating the above jacobian function, other attributes of the jacobian object also are updated. Symbolic Jacobian matrices can be extracted from the attributes. Since this is a serial robot, the matrix $J_a$ itself would be the Jacobian matrix of the manipulator. The matrix $J_a$ is extracted from `Ja` attribute of the jacobian object as follows.
 ```py
 symbolic_jacobian = jac.Ja
 symbolic_jacobian
 ```
 
 In an ipynb file of JupyterLab, the above code would produce the following output.
```

### Comparing `acrod-1.1.3/tests/test_jacobian.py` & `acrod-1.1.4/tests/test_jacobian.py`

 * *Files identical despite different names*

