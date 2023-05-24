# Comparing `tmp/invopt-0.0.3.tar.gz` & `tmp/invopt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invopt-0.0.3.tar", last modified: Mon May 22 13:13:58 2023, max compression
+gzip compressed data, was "invopt-0.0.4.tar", last modified: Wed May 24 15:45:54 2023, max compression
```

## Comparing `invopt-0.0.3.tar` & `invopt-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 13:13:58.093986 invopt-0.0.3/
--rw-rw-rw-   0        0        0     1099 2023-05-01 20:52:18.000000 invopt-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     3928 2023-05-22 13:13:58.093986 invopt-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3338 2023-05-16 12:23:45.000000 invopt-0.0.3/README.md
--rw-rw-rw-   0        0        0      712 2023-05-22 13:10:07.000000 invopt-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-22 13:13:58.093986 invopt-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-22 13:13:58.031453 invopt-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-22 13:13:58.062713 invopt-0.0.3/src/invopt/
--rw-rw-rw-   0        0        0      371 2023-05-02 08:10:57.000000 invopt-0.0.3/src/invopt/__init__.py
--rw-rw-rw-   0        0        0    54267 2023-05-18 11:10:46.000000 invopt-0.0.3/src/invopt/main.py
-drwxrwxrwx   0        0        0        0 2023-05-22 13:13:58.093986 invopt-0.0.3/src/invopt.egg-info/
--rw-rw-rw-   0        0        0     3928 2023-05-22 13:13:58.000000 invopt-0.0.3/src/invopt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-22 13:13:58.000000 invopt-0.0.3/src/invopt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 13:13:58.000000 invopt-0.0.3/src/invopt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-22 13:13:58.000000 invopt-0.0.3/src/invopt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-22 13:13:58.000000 invopt-0.0.3/src/invopt.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-22 13:13:58.093986 invopt-0.0.3/tests/
--rw-rw-rw-   0        0        0     1682 2023-05-12 10:16:00.000000 invopt-0.0.3/tests/test_examples.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:45:54.322594 invopt-0.0.4/
+-rw-rw-rw-   0        0        0     1099 2023-05-01 20:52:18.000000 invopt-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     3944 2023-05-24 15:45:54.322594 invopt-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3354 2023-05-24 15:40:37.000000 invopt-0.0.4/README.md
+-rw-rw-rw-   0        0        0      712 2023-05-24 09:24:06.000000 invopt-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 15:45:54.322594 invopt-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 15:45:54.290927 invopt-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 15:45:54.309587 invopt-0.0.4/src/invopt/
+-rw-rw-rw-   0        0        0      388 2023-05-24 15:25:36.000000 invopt-0.0.4/src/invopt/__init__.py
+-rw-rw-rw-   0        0        0    53495 2023-05-24 15:21:47.000000 invopt-0.0.4/src/invopt/main.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:45:54.322594 invopt-0.0.4/src/invopt.egg-info/
+-rw-rw-rw-   0        0        0     3944 2023-05-24 15:45:54.000000 invopt-0.0.4/src/invopt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-24 15:45:54.000000 invopt-0.0.4/src/invopt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 15:45:54.000000 invopt-0.0.4/src/invopt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-24 15:45:54.000000 invopt-0.0.4/src/invopt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-24 15:45:54.000000 invopt-0.0.4/src/invopt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 15:45:54.322594 invopt-0.0.4/tests/
+-rw-rw-rw-   0        0        0     1681 2023-05-24 15:26:39.000000 invopt-0.0.4/tests/test_examples.py
```

### Comparing `invopt-0.0.3/LICENSE.txt` & `invopt-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `invopt-0.0.3/PKG-INFO` & `invopt-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invopt
-Version: 0.0.3
+Version: 0.0.4
 Summary: Inverse Optimization with Python
 Author-email: Pedro Zattoni Scroccaro <pedroszattoni@gmail.com>
 Project-URL: Homepage, https://github.com/pedroszattoni/invopt
 Project-URL: Bug Tracker, https://github.com/pedroszattoni/inverse-optimization/issues
 Keywords: inverse-optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -26,18 +26,18 @@
 ```
 InvOpt depends on NumPy. Moreover, some of its functions also depend on gurobipy or cvxpy. You can get a free academic license for Gurobi [here](https://www.gurobi.com/academia/academic-program-and-licenses/).
 
 ## Usage and examples
 
 The following functions are available in the InvOpt package to solving IO problems:
 
-- [`discrete_model_consistent`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_model_consistent): for FOPs with dicrete decision spaces (e.g., binary), and when the dataset is consistent with some cost vector. Can be used to check if the data is consistent.
-- [`discrete_model`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_model): for FOPs with dicrete decision spaces (e.g., binary).
-- [`MIP_linear`](https://github.com/pedroszattoni/invopt/tree/main/examples/MIP_linear): for FOPs with mixed-integer decision spaces and cost functions linear w.r.t. the continuous part of the decision variable.
-- [`MIP_quadratic`](https://github.com/pedroszattoni/invopt/tree/main/examples/MIP_quadratic): for FOPs with mixed-integer decision spaces and cost functions quadratic w.r.t. the continuous part of the decision variable.
+- [`discrete_consistent`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_consistent): for FOPs with dicrete decision spaces (e.g., binary), and when the dataset is consistent with some cost vector. Can be used to check if the data is consistent.
+- [`discrete`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete): for FOPs with dicrete decision spaces (e.g., binary).
+- [`mixed_integer_linear`](https://github.com/pedroszattoni/invopt/tree/main/examples/mixed_integer_linear): for FOPs with mixed-integer decision spaces and cost functions linear w.r.t. the continuous part of the decision variable.
+- [`mixed_integer_quadratic`](https://github.com/pedroszattoni/invopt/tree/main/examples/mixed_integer_quadratic): for FOPs with mixed-integer decision spaces and cost functions quadratic w.r.t. the continuous part of the decision variable.
 - [`FOM`](https://github.com/pedroszattoni/invopt/tree/main/examples/FOM): for general FOPs. Solves IO problem approximately using first-order methods.
 
 ## Contributing
 
 Contributions, pull requests and suggestions are very much welcome. The  [TODO](https://github.com/pedroszattoni/invopt/blob/main/TODO.txt) file contains a number of ideas to possibly improve the InvOpt package.
 
 ## Citing
```

### Comparing `invopt-0.0.3/README.md` & `invopt-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 ```
 InvOpt depends on NumPy. Moreover, some of its functions also depend on gurobipy or cvxpy. You can get a free academic license for Gurobi [here](https://www.gurobi.com/academia/academic-program-and-licenses/).
 
 ## Usage and examples
 
 The following functions are available in the InvOpt package to solving IO problems:
 
-- [`discrete_model_consistent`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_model_consistent): for FOPs with dicrete decision spaces (e.g., binary), and when the dataset is consistent with some cost vector. Can be used to check if the data is consistent.
-- [`discrete_model`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_model): for FOPs with dicrete decision spaces (e.g., binary).
-- [`MIP_linear`](https://github.com/pedroszattoni/invopt/tree/main/examples/MIP_linear): for FOPs with mixed-integer decision spaces and cost functions linear w.r.t. the continuous part of the decision variable.
-- [`MIP_quadratic`](https://github.com/pedroszattoni/invopt/tree/main/examples/MIP_quadratic): for FOPs with mixed-integer decision spaces and cost functions quadratic w.r.t. the continuous part of the decision variable.
+- [`discrete_consistent`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_consistent): for FOPs with dicrete decision spaces (e.g., binary), and when the dataset is consistent with some cost vector. Can be used to check if the data is consistent.
+- [`discrete`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete): for FOPs with dicrete decision spaces (e.g., binary).
+- [`mixed_integer_linear`](https://github.com/pedroszattoni/invopt/tree/main/examples/mixed_integer_linear): for FOPs with mixed-integer decision spaces and cost functions linear w.r.t. the continuous part of the decision variable.
+- [`mixed_integer_quadratic`](https://github.com/pedroszattoni/invopt/tree/main/examples/mixed_integer_quadratic): for FOPs with mixed-integer decision spaces and cost functions quadratic w.r.t. the continuous part of the decision variable.
 - [`FOM`](https://github.com/pedroszattoni/invopt/tree/main/examples/FOM): for general FOPs. Solves IO problem approximately using first-order methods.
 
 ## Contributing
 
 Contributions, pull requests and suggestions are very much welcome. The  [TODO](https://github.com/pedroszattoni/invopt/blob/main/TODO.txt) file contains a number of ideas to possibly improve the InvOpt package.
 
 ## Citing
```

### Comparing `invopt-0.0.3/pyproject.toml` & `invopt-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "invopt"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Pedro Zattoni Scroccaro", email="pedroszattoni@gmail.com" },
 ]
 description = "Inverse Optimization with Python"
 readme = "README.md"
 keywords = ["inverse-optimization"]
 requires-python = ">=3.7"
```

### Comparing `invopt-0.0.3/src/invopt/main.py` & `invopt-0.0.4/src/invopt/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,22 +47,24 @@
         warnings.warn('Attention! Using this IO method for models with binary '
                       'decision variables requires solving an optimization '
                       'problem with potentially O(N*2^n) constraints, '
                       'where N is the number of training examples and n is '
                       'the dimension of the binary decision vector.')
 
 
-def warning_dist_func_reg_param_sub_loss(dist_func, reg_param, sub_loss):
-    """Warn user dist_func / reg_param are not necessary when sub_loss=True."""
-    if sub_loss:
-        if dist_func is not None:
-            warnings.warn('dist_func not used when sub_loss=True.')
+def warning_dist_func_sub_loss(dist_func, sub_loss):
+    """Warn user dist_func is not used when sub_loss=True."""
+    if sub_loss and (dist_func is not None):
+        warnings.warn('dist_func is not used when sub_loss=True.')
 
-        if reg_param > 0:
-            warnings.warn('reg_param not used when sub_loss=True.')
+
+def warning_theta_hat_reg_param(theta_hat, reg_param):
+    """Warn user theta_hat is not used when reg_param=0."""
+    if (theta_hat is not None) and (reg_param == 0):
+        warnings.warn('theta_hat is not used when reg_param=0.')
 
 
 def normalize(vec, norm):
     """
     Normalize nonzero array according to some norm.
 
     Parameters
@@ -112,30 +114,31 @@
         between them according to some distance metric.
     regularizer : {'L2_squared', 'L1'}, optional
         Type of regularization on cost vector theta. The default is
         'L2_squared'.
     reg_param : float, optional
         Nonnegative regularization parameter. The default is 0.
     theta_hat : {1D ndarray, None}, optional
-        A priory belief or estimate of the true cost vector. The default is
+        A priory belief or estimate of the true cost vector. When
+        theta_hat=None, it is defined as the vector of zeros. The default is
         None.
 
     Raises
     ------
     Exception
         If invalid regularization parameter. If negative regularization
         parameter.
 
     Returns
     -------
     float
         Augmented suboptimality loss value.
 
     """
-    # Check if inputs are valid
+    # Check if the inputs are valid
     check_regularizer(regularizer)
     check_reg_parameter(reg_param)
 
     if theta_hat is None:
         theta_hat = 0
 
     if regularizer == 'L2_squared':
@@ -265,65 +268,64 @@
         results = (x_diff_avg, obj_diff_avg, theta_diff)
     else:
         results = x_diff_avg
 
     return results
 
 
-def discrete_model_consistent(dataset, phi, decision_space,
-                              X=None,
-                              dist_func=None,
-                              Theta=None,
-                              regularizer='L2_squared',
-                              theta_hat=None,
-                              feasibility=False,
-                              verbose=False,
-                              gurobi_params=None):
+def discrete_consistent(dataset, decision_space, phi,
+                        X=None,
+                        dist_func=None,
+                        Theta=None,
+                        regularizer='L2_squared',
+                        theta_hat=None,
+                        feasibility=False,
+                        verbose=False,
+                        gurobi_params=None):
     """
     Inverse optimization for discrete models with consistent data.
 
     Uses incenter (default) or feasibility strategy. For more details, see
-    https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_model_consistent
+    https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_consistent
 
     Parameters
     ----------
     dataset : list of tuples
         List of tuples (s, x), where s is the signal and x is the response.
     phi : callable
         Feature function. Given a signal s and response x, returns a 1D
         ndarray feature vector. Syntax: phi(s, x).
     decision_space : {tuple('binary', n)}
         Tuple containing type and dimension of the decision space.
     X : {callable, None}, optional
         Constraint set. Given a signal s and response x, returns True if x is a
         feasible response, and False otherwise. It does not need to check for
-        the type of the decision space contained in decision_space. For
-        example, if decision_space=('binary', n), X does not need to check if x
-        is a binary vector. Syntax: X(s, x). If None, it will be defined as
+        the type of the decision variables contained in decision_space. For
+        example, if decision_space=('binary', n), X should not check if x is a
+        binary vector. Syntax: X(s, x). If None, it will be defined as
         "def X(s, x): return True". The default is None.
     dist_func : {callable, None}, optional
         Distance function. Given two responses x1 and x2, returns the distance
         between them according to some distance metric. Not required when
         using the feasibility strategy. Syntax: dist_func(x1, x2). The default
         is None.
     Theta : {None, 'nonnegative'}, optional
         Constraints on cost vector theta. The default is None.
     regularizer : {'L2_squared', 'L1'}, optional
         Type of regularization on cost vector theta. The default is
         'L2_squared'.
     theta_hat : {1D ndarray, None}, optional
-        A priory belief or estimate of the true cost vector. When not None, the
-        cost vector returned will be the feasible vector closest to theta_hat.
-        The default is None.
+        A priory belief or estimate of the true cost vector. The default is
+        None.
     feasibility : bool, optional
-        If True, solve problem as a feasibility problem. Namely, searches
-        over the facets of the unit L-infinity sphere until a feasible
-        cost vector is found. If Theta='nonnegative', only searches over the
-        nonnegative facet of the L-1 sphere. If False, solve the problem
-        using the Incenter strategy. The default is False.
+        If True, solve problem using the feasibility strategy. Namely, if
+        theta_hat=None, we search over the facets of the unit L-infinity sphere
+        until a feasible cost vector is found. If Theta='nonnegative', only
+        searches over the nonnegative facet of the L-1 sphere. If False, solve
+        the problem using the Incenter strategy. The default is False.
     verbose : bool, optional
         If True, print Gurobi's solver output. The default is False.
     gurobi_params : {list of tuple(str, value), None}, optional
         List of tuples with Gurobi's parameter name and value. For example,
         [('TimeLimit', 0.5), ('Method', 2)]. The default is None.
 
     Raises
@@ -338,39 +340,29 @@
     theta_opt : 1D ndarray
         An optimal cost vector according to the chosen strategy.
 
     """
     try:
         import gurobipy as gp
     except ImportError:
-        print("gurobipy is required for invopt's discrete_model_consistent " +
+        print("gurobipy is required for invopt's discrete_consistent " +
               "function.")
 
-    # Check if inputs are valid
+    # Check if the inputs are valid
     check_Theta(Theta)
     check_decision_space(decision_space)
     check_regularizer(regularizer)
 
     warning_large_decision_space(decision_space)
 
-    if (theta_hat is not None) and feasibility:
-        raise Exception('Either set feasibility=True or set theta_hat not '
-                        'None. When feasibility=True, returns any feasible '
-                        'solution. When theta_hat is not None, returns the '
-                        'feasible solution closest to theta_hat, that is, '
-                        'regularizer(theta - theta_hat) is minimized.')
-
-    if dist_func is None:
-        if (not feasibility) and (theta_hat is None):
-            raise Exception('dist_func required when feasibility=False and '
-                            'theta_hat is not given.')
-    else:
-        if feasibility or (theta_hat is not None):
-            warnings.warn('dist_func not used when a theta_hat is given or '
-                          'feasibility=True.')
+    if (dist_func is None) and (not feasibility):
+        raise Exception('dist_func required when feasibility=False.')
+
+    if (dist_func is not None) and feasibility:
+        warnings.warn('dist_func not used when feasibility=True.')
 
     if X is None:
         def X(s, x): return True
 
     N = len(dataset)
 
     # Sample signal and response to get dimension of the cost vector
@@ -396,22 +388,22 @@
         if decision_space[0] == 'binary':
             n = decision_space[1]
             for k in range(2**n):
                 x = dec_to_bin(k, n)
                 if X(s_hat, x):
                     phi_1 = phi(s_hat, x)
                     phi_2 = phi(s_hat, x_hat)
-                    if (theta_hat is not None) or feasibility:
+                    if feasibility:
                         dist = 0
                     else:
                         dist = dist_func(x_hat, x)
                     mdl.addConstr(gp.quicksum(theta[j]*(phi_1[j] - phi_2[j])
                                               for j in range(p)) >= dist)
 
-    if feasibility:
+    if feasibility and (theta_hat is None):
         if Theta == 'nonnegative':
             mdl.addConstr(gp.quicksum(theta) == 1)
             mdl.optimize()
         else:
             # Search over facets of unit L-infinity sphere for a feasible
             # solution.
             for i in range(p):
@@ -424,16 +416,16 @@
                 if mdl.status == 2:
                     break
     else:
         if theta_hat is None:
             theta_hat = np.zeros(p)
 
         if regularizer == 'L2_squared':
-            obj = 0.5*gp.quicksum((theta[i] - theta_hat[i])**2
-                                  for i in range(p))
+            obj = 0.5 * gp.quicksum((theta[i] - theta_hat[i])**2
+                                    for i in range(p))
         elif regularizer == 'L1':
             t = mdl.addVars(p, lb=-gp.GRB.INFINITY, vtype=gp.GRB.CONTINUOUS)
             obj = gp.quicksum(t)
             mdl.addConstrs(theta[i] - theta_hat[i] <= t[i] for i in range(p))
             mdl.addConstrs(theta_hat[i] - theta[i] <= t[i] for i in range(p))
 
         mdl.setObjective(obj, gp.GRB.MINIMIZE)
@@ -446,60 +438,61 @@
                         f'= {mdl.status}. Set the flag verbose=True for more '
                         'details. The optimization problem will '
                         'always be infeasible if the data is not consistent.')
 
     return theta_opt
 
 
-def discrete_model(dataset, phi, decision_space,
-                   X=None,
-                   dist_func=None,
-                   Theta=None,
-                   regularizer='L2_squared',
-                   reg_param=0,
-                   theta_hat=None,
-                   sub_loss=False,
-                   verbose=False,
-                   gurobi_params=None):
+def discrete(dataset, decision_space, phi,
+             X=None,
+             dist_func=None,
+             Theta=None,
+             regularizer='L2_squared',
+             reg_param=0,
+             theta_hat=None,
+             sub_loss=False,
+             verbose=False,
+             gurobi_params=None):
     """
     Inverse optimization for discrete models.
 
     For more details, see
-    https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_model
+    https://github.com/pedroszattoni/invopt/tree/main/examples/discrete
 
     Parameters
     ----------
     dataset : list of tuples
         List of tuples (s, x), where s is the signal and x is the response.
     phi : callable
         Feature function. Given a signal s and response x, returns a 1D
         ndarray feature vector. Syntax: phi(s, x).
     decision_space : {tuple('binary', n)}
         Tuple containing type and dimension of the decision space.
     X : {callable, None}, optional
         Constraint set. Given a signal s and response x, returns True if x is a
         feasible response, and False otherwise. It does not need to check for
-        the type of the decision space contained in decision_space. For
-        example, if decision_space=('binary', n), X does not need to check if x
-        is a binary vector. Syntax: X(s, x). If None, it will be defined as
+        the type of the decision variables contained in decision_space. For
+        example, if decision_space=('binary', n), X should not check if x is a
+        binary vector. Syntax: X(s, x). If None, it will be defined as
         "def X(s, x): return True". The default is None.
     dist_func : {callable, None}, optional
         Distance function. Given two responses x1 and x2, returns the distance
         between them according to some distance metric. Not required when
         sub_loss=True. Syntax: dist_func(x1, x2). The default is None.
     Theta : {None, 'nonnegative'}, optional
         Constraints on cost vector theta. The default is None.
     regularizer : {'L2_squared', 'L1'}, optional
         Type of regularization on cost vector theta. The default is
         'L2_squared'.
     reg_param : float, optional
         Nonnegative regularization parameter. The default is 0.
     theta_hat : {1D ndarray, None}, optional
-        A priory belief or estimate of the true cost vector. When not None,
-        theta_hat is defined as the vector of zeros. The default is None.
+        A priory belief or estimate of the true cost vector. When
+        theta_hat=None, it is defined as the vector of zeros. The default is
+        None.
     sub_loss : bool, optional
         If True, solve the problem using the Suboptimality loss. Namely,
         searches over the facts of the unit L-infinity sphere for the cost
         vector with the smallest loss. If Theta='nonnegative', only searches
         over the nonnegative facet of the L-1 sphere. If False, solve the
         problem using the Augmented Suboptimality loss. The default is False.
     verbose : bool, optional
@@ -516,170 +509,103 @@
 
     Returns
     -------
     theta_opt : 1D ndarray
         An optimal cost vector according to the chosen strategy.
 
     """
-    try:
-        import gurobipy as gp
-    except ImportError:
-        print("gurobipy is required for invopt's discrete_model function.")
-
-    # Check if inputs are valid
-    check_Theta(Theta)
-    check_decision_space(decision_space)
-    check_regularizer(regularizer)
-    check_reg_parameter(reg_param)
-    check_dist_func(dist_func, sub_loss)
+    _, n = decision_space
 
-    # Warnings
-    warning_large_decision_space(decision_space)
-    warning_dist_func_reg_param_sub_loss(dist_func, reg_param, sub_loss)
-
-    if X is None:
-        def X(s, x): return True
-
-    N = len(dataset)
-
-    # Sample signal and response to get dimension of the cost vector
-    s_test, x_test = dataset[0]
-    p = len(phi(s_test, x_test))
-
-    # Initialize Gurobi model
-    mdl = gp.Model()
-    if not verbose:
-        mdl.setParam('OutputFlag', 0)
-    if gurobi_params is not None:
-        for param, value in gurobi_params:
-            mdl.setParam(param, value)
-
-    theta = mdl.addVars(p, lb=-gp.GRB.INFINITY, vtype=gp.GRB.CONTINUOUS)
-    beta = mdl.addVars(N, vtype=gp.GRB.CONTINUOUS)
-    sum_beta = (1/N)*gp.quicksum(beta)
-
-    if Theta == 'nonnegative':
-        mdl.addConstrs(theta[i] >= 0 for i in range(p))
-
-    # Add constraints
-    for i in range(N):
-        s_hat, x_hat = dataset[i]
-        if decision_space[0] == 'binary':
-            n = decision_space[1]
-            for k in range(2**n):
-                x = dec_to_bin(k, n)
-                if X(s_hat, x):
-                    phi_1 = phi(s_hat, x)
-                    phi_2 = phi(s_hat, x_hat)
-                    if sub_loss:
-                        dist = 0
-                    else:
-                        dist = dist_func(x_hat, x)
-                    mdl.addConstr(
-                        gp.quicksum(theta[j]*(phi_1[j] - phi_2[j])
-                                    for j in range(p)) >= dist - beta[i])
-
-    if sub_loss:
-        mdl.setObjective(sum_beta, gp.GRB.MINIMIZE)
-
-        if Theta is None:
-            # Search over facets of unit L-infinity sphere for the solution
-            # with the lowest objective value.
-            best_obj = np.inf
-            for i in range(p):
-                for j in [-1, 1]:
-                    cons = mdl.addConstr(theta[i] == j)
-                    mdl.optimize()
-                    obj_val = mdl.objVal
-                    mdl.remove(cons)
-                    if (mdl.status == 2) and (obj_val < best_obj):
-                        best_obj = obj_val
-                        theta_opt = np.array([theta[i].X for i in range(p)])
-        elif Theta == 'nonnegative':
-            mdl.addConstr(gp.quicksum(theta) == 1)
-            mdl.optimize()
-            theta_opt = np.array([theta[i].X for i in range(p)])
+    if theta_hat is None:
+        theta_hat_mod = None
     else:
-        if theta_hat is None:
-            theta_hat = np.zeros(p)
+        theta_hat_mod = (np.zeros((1, 1)), theta_hat)
 
-        if regularizer == 'L2_squared':
-            reg_term = (reg_param/2)*gp.quicksum((theta[i] - theta_hat[i])**2
-                                                 for i in range(p))
-        elif regularizer == 'L1':
-            t = mdl.addVars(p, lb=-gp.GRB.INFINITY, vtype=gp.GRB.CONTINUOUS)
-            reg_term = reg_param*gp.quicksum(t)
-            mdl.addConstrs(theta[i] - theta_hat[i] <= t[i] for i in range(p))
-            mdl.addConstrs(theta_hat[i] - theta[i] <= t[i] for i in range(p))
+    dataset_mod = []
+    for data in dataset:
+        w_hat, z_hat = data
+        s_hat = (np.zeros((1, 1)), np.zeros((1, n)), np.array([0]), w_hat)
+        x_hat = (np.array([0]), z_hat)
+        dataset_mod.append((s_hat, x_hat))
+
+    theta_opt_mod = mixed_integer_linear(dataset_mod, decision_space,
+                                         phi2=phi,
+                                         Z=X,
+                                         dist_func_z=dist_func,
+                                         Theta=Theta,
+                                         regularizer=regularizer,
+                                         reg_param=reg_param,
+                                         theta_hat=theta_hat_mod,
+                                         sub_loss=sub_loss,
+                                         verbose=verbose,
+                                         gurobi_params=gurobi_params)
 
-        mdl.setObjective(reg_term + sum_beta, gp.GRB.MINIMIZE)
-        mdl.optimize()
-        theta_opt = np.array([theta[i].X for i in range(p)])
-
-    if mdl.status != 2:
-        raise Exception('Optimal solution not found. Gurobi status code '
-                        f'= {mdl.status}. Set the flag verbose=True for more '
-                        'details.')
+    theta_opt = theta_opt_mod[1:]
 
     return theta_opt
 
 
-def MIP_linear(dataset, decision_space,
-               Z=None,
-               phi1=None,
-               phi2=None,
-               dist_func=None,
-               Theta=None,
-               regularizer='L2_squared',
-               reg_param=0,
-               sub_loss=False,
-               verbose=False,
-               gurobi_params=None):
+def mixed_integer_linear(dataset, decision_space,
+                         phi1=None,
+                         phi2=None,
+                         Z=None,
+                         dist_func_z=None,
+                         Theta=None,
+                         regularizer='L2_squared',
+                         reg_param=0,
+                         theta_hat=None,
+                         sub_loss=False,
+                         verbose=False,
+                         gurobi_params=None):
     """
     Inverse optimization for linear models with mixed-integer feasible sets.
 
     For more details, see
-    https://github.com/pedroszattoni/invopt/tree/main/examples/MIP_linear
+    https://github.com/pedroszattoni/invopt/tree/main/examples/mixed_integer_linear
 
     Parameters
     ----------
     dataset : list of tuples
         List of tuples (s, x), where s is the signal and x is the response.
     decision_space : {tuple('binary', n)}
         Tuple containing type and dimension of the decision space fo the
         integer part of the decision vector.
     Z : {callable, None}, optional
         Constraint set of the integer part of the decision vector. Given a
         signal s = (A, B, c, w) and response x = (y, z), returns True if z
         (i.e., the integer part of x) is a feasible response, and False
-        otherwise. It does not need to check for the type of the decision space
-        contained in decision_space. For example, if
-        decision_space=('binary', n), Z does not need to check if z
-        is a binary vector. Syntax: Z(w, z). If None, it will be defined as
+        otherwise. It does not need to check for the type of the decision
+        variables contained in decision_space. For example, if
+        decision_space=('binary', n), Z should not check if z is a binary
+        vector. Syntax: Z(w, z). If None, it will be defined as
         "def Z(w, x): return True". The default is None.
     phi1 : {callable, None}, optional
         Feature function. Given w and response z, returns a 1D
         ndarray feature vector. Syntax: phi1(w, z). If None, it will be defined
         as "def phi1(w, z): return np.array([0])". The default is None.
     phi2 : {callable, None}, optional
         Feature function. Given w and response z, returns a 1D
         ndarray feature vector. Syntax: phi1(w, z). If None, it will be defined
         as "def phi2(w, z): return np.array([0])". The default is None.
-    dist_func : {callable, None}, optional
+    dist_func_z : {callable, None}, optional
         Distance function. Given two responses x1=(y1,z1) and x2=(y2,z2),
         returns the distance of their integer parts according to some distance
-        metric. Not required when sub_loss=True. Syntax: dist_func(z1, z2).
+        metric. Not required when sub_loss=True. Syntax: dist_func_z(z1, z2).
         The default is None.
     Theta : {None, 'nonnegative'}, optional
         Constraints on cost vector theta. The default is None.
     regularizer : {'L2_squared', 'L1'}, optional
         Type of regularization on cost vector theta. The default is
         'L2_squared'.
     reg_param : float, optional
         Nonnegative regularization parameter. The default is 0.
+    theta_hat : {tuple(2D ndarray, 1D ndarray), None}, optional
+        A priory belief or estimate of the true cost vector theta=(vec(Q), q).
+        Should be provided as a tuple (Q_hat, q_hat). When None, theta_hat is
+        defined as zeros. The default is None.
     sub_loss : bool, optional
         If True, solve the problem using the Suboptimality loss. Namely,
         searches over the facts of the unit L-infinity sphere for the cost
         vector with the smallest loss. If Theta='nonnegative', only searches
         over the nonnegative facet of the L-1 sphere. If False, solve the
         problem using the Augmented Suboptimality loss. The default is False.
     verbose : bool, optional
@@ -700,26 +626,28 @@
     theta_opt : 1D ndarray
         An optimal cost vector according to the chosen strategy.
 
     """
     try:
         import gurobipy as gp
     except ImportError:
-        print("gurobipy is required for invopt's MIP_linear function.")
+        print("gurobipy is required for invopt's mixed_integer_linear " +
+              'function.')
 
-    # Check if inputs are valid
+    # Check if the inputs are valid
     check_Theta(Theta)
     check_decision_space(decision_space)
     check_regularizer(regularizer)
     check_reg_parameter(reg_param)
-    check_dist_func(dist_func, sub_loss)
+    check_dist_func(dist_func_z, sub_loss)
 
     # Warnings
     warning_large_decision_space(decision_space)
-    warning_dist_func_reg_param_sub_loss(dist_func, reg_param, sub_loss)
+    warning_dist_func_sub_loss(dist_func_z, sub_loss)
+    warning_theta_hat_reg_param(theta_hat, reg_param)
 
     if (phi1 is None) and (phi2 is None):
         raise Exception('Either phi1 or phi2 have to be given.')
 
     N = len(dataset)
 
     if Z is None:
@@ -765,15 +693,15 @@
                 z = dec_to_bin(k, n)
                 if Z(w_hat, z):
                     lamb = mdl.addVars(m1, vtype=gp.GRB.CONTINUOUS)
 
                     if sub_loss:
                         dist = 0
                     else:
-                        dist = dist_func(z_hat, z)
+                        dist = dist_func_z(z_hat, z)
 
                     phi1_hat = phi1(w_hat, z_hat)
                     phi2_hat = phi2(w_hat, z_hat)
                     Qphi1 = [gp.quicksum(Q[i, j]*phi1_hat[j]
                                          for j in range(u1))
                              for i in range(m2)]
                     yQphi1 = gp.quicksum(y_hat[j]*Qphi1[j] for j in range(m2))
@@ -793,22 +721,58 @@
                     ph1 = phi1(w_hat, z)
                     mdl.addConstrs(gp.quicksum(Q[i, j]*ph1[j]
                                                for j in range(u1))
                                    + gp.quicksum(lamb[j]*A[j, i]
                                                  for j in range(m1))
                                    == 0 for i in range(m2))
 
-    if sub_loss:
-        mdl.setObjective(sum_beta, gp.GRB.MINIMIZE)
+    if reg_param > 0:
+        if theta_hat is None:
+            Q_hat = np.zeros((m2, u1))
+            q_hat = np.zeros(u2)
+        else:
+            Q_hat, q_hat = theta_hat
+
+        if regularizer == 'L2_squared':
+            Q_sum = gp.quicksum((Q[i, j] - Q_hat[i, j])**2 for i in range(m2)
+                                for j in range(u1))
+            q_sum = gp.quicksum((q[i] - q_hat[i])**2 for i in range(u2))
+            reg_term = (reg_param/2)*(Q_sum + q_sum)
+        elif regularizer == 'L1':
+            tQ = mdl.addVars(m2, u1, lb=-gp.GRB.INFINITY,
+                             vtype=gp.GRB.CONTINUOUS)
+            tq = mdl.addVars(u2, lb=-gp.GRB.INFINITY, vtype=gp.GRB.CONTINUOUS)
+
+            reg_term = reg_param*(gp.quicksum(tQ) + gp.quicksum(tq))
+
+            mdl.addConstrs(Q[i, j] - Q_hat[i, j] <= tQ[i, j]
+                           for i in range(m2) for j in range(u1))
+            mdl.addConstrs(Q_hat[i, j] - Q[i, j] <= tQ[i, j]
+                           for i in range(m2) for j in range(u1))
+            mdl.addConstrs(q[i] - q_hat[i] <= tq[i] for i in range(u2))
+            mdl.addConstrs(q_hat[i] - q[i] <= tq[i] for i in range(u2))
+    else:
+        reg_term = 0
+
+    mdl.setObjective(reg_term + sum_beta, gp.GRB.MINIMIZE)
 
+    # Check if norm equality constraint needs to be added to avoid the trivial
+    # solution theta=0
+    if sub_loss and ((reg_param == 0) or (theta_hat is None)):
         if Theta == 'nonnegative':
             mdl.addConstr(gp.quicksum(q) + gp.quicksum(Q) == 1)
             mdl.optimize()
+
+            if mdl.status != 2:
+                raise Exception('Optimal solution not found. Gurobi status '
+                                f'code = {mdl.status}. Set the flag '
+                                'verbose=True for more details.')
+
             Q_opt = np.array([[Q[i, j].X for i in range(m2)]
-                              for j in range(u1)])
+                             for j in range(u1)])
             q_opt = np.array([q[i].X for i in range(u2)])
         else:
             # Search over facets of unit L-infinity sphere for the solution
             # with the lowest objective value.
             best_obj = np.inf
             for i in range(u1):
                 for j in [-1, 1]:
@@ -835,98 +799,87 @@
                             if obj_val < best_obj:
                                 best_obj = obj_val
                                 Q_opt = np.array([[Q[i, j].X
                                                    for i in range(m2)]
                                                   for j in range(u1)])
                                 q_opt = np.array([q[i].X for i in range(u2)])
     else:
-        if regularizer == 'L2_squared':
-            Q_sum = gp.quicksum(Q[i, j]**2 for i in range(m2)
-                                for j in range(u1))
-            q_sum = gp.quicksum(q[i]**2 for i in range(u2))
-            reg_term = (reg_param/2)*(Q_sum + q_sum)
-        elif regularizer == 'L1':
-            tQ = mdl.addVars(m2, u1, lb=-gp.GRB.INFINITY,
-                             vtype=gp.GRB.CONTINUOUS)
-            tq = mdl.addVars(u2, lb=-gp.GRB.INFINITY, vtype=gp.GRB.CONTINUOUS)
-            reg_term = reg_param*(gp.quicksum(tQ) + gp.quicksum(tq))
-            mdl.addConstrs(Q[i, j] <= tQ[i, j]
-                           for i in range(m2) for i in range(u1))
-            mdl.addConstrs(-Q[i, j] <= tQ[i, j]
-                           for i in range(m2) for i in range(u1))
-            mdl.addConstrs(q[i] <= tq[i] for i in range(u2))
-            mdl.addConstrs(-q[i] <= tq[i] for i in range(u2))
-
-        mdl.setObjective(reg_term + sum_beta, gp.GRB.MINIMIZE)
         mdl.optimize()
 
         if mdl.status != 2:
             raise Exception('Optimal solution not found. Gurobi status code '
                             f'= {mdl.status}. Set the flag verbose=True for '
                             'more details.')
 
-        Q_opt = np.array([[Q[i, j].X for i in range(m2)] for j in range(u1)])
+        Q_opt = np.array([[Q[i, j].X for i in range(m2)]
+                         for j in range(u1)])
         q_opt = np.array([q[i].X for i in range(u2)])
 
     theta_opt = np.concatenate((Q_opt.flatten('F'), q_opt))
     return theta_opt
 
 
-def MIP_quadratic(dataset, decision_space,
-                  Z=None,
-                  phi1=None,
-                  phi2=None,
-                  dist_func=None,
-                  Theta=None,
-                  regularizer='L2_squared',
-                  reg_param=0,
-                  sub_loss=False,
-                  verbose=False,
-                  solver='mosek'):
+def mixed_integer_quadratic(dataset, decision_space,
+                            phi1=None,
+                            phi2=None,
+                            Z=None,
+                            dist_func_z=None,
+                            Theta=None,
+                            regularizer='L2_squared',
+                            reg_param=0,
+                            theta_hat=None,
+                            sub_loss=False,
+                            verbose=False,
+                            solver='mosek'):
     """
     Inverse optimization for quadratic models with mixed-integer feasible sets.
 
     For more details, see
-    https://github.com/pedroszattoni/invopt/tree/main/examples/MIP_quadratic
+    https://github.com/pedroszattoni/invopt/tree/main/examples/mixed_integer_quadratic
 
     Parameters
     ----------
     dataset : list of tuples
         List of tuples (s, x), where s is the signal and x is the response.
     decision_space : {tuple('binary', n)}
         Tuple containing type and dimension of the decision space.
     Z : {callable, None}, optional
         Constraint set of the integer part of the decision vector. Given a
         signal s = (A, B, c, w) and response x = (y, z), returns True if z
         (i.e., the integer part of x) is a feasible response, and False
-        otherwise. It does not need to check for the type of the decision space
-        contained in decision_space. For example, if
-        decision_space=('binary', n), Z does not need to check if z
-        is a binary vector. Syntax: Z(w, z). If None, it will be defined as
+        otherwise. It does not need to check for the type of the decision
+        variables contained in decision_space. For example, if
+        decision_space=('binary', n), Z should not check if z is a binary
+        vector. Syntax: Z(w, z). If None, it will be defined as
         "def Z(w, x): return True". The default is None.
     phi1 : {callable, None}, optional
         Feature function. Given w and response z, returns a 1D
         ndarray feature vector. Syntax: phi1(w, z). If None, it will be defined
         as "def phi1(w, z): return np.array([0])". The default is None.
     phi2 : {callable, None}, optional
         Feature function. Given w and response z, returns a 1D
         ndarray feature vector. Syntax: phi1(w, z). If None, it will be defined
         as "def phi2(w, z): return np.array([0])". The default is None.
-    dist_func : {callable, None}, optional
+    dist_func_z : {callable, None}, optional
         Distance function. Given two responses x1=(y1,z1) and x2=(y2,z2),
         returns the distance of their integer parts according to some distance
-        metric. Not required when sub_loss=True. Syntax: dist_func(z1, z2).
+        metric. Not required when sub_loss=True. Syntax: dist_func_z(z1, z2).
         The default is None.
     Theta : {None, 'nonnegative'}, optional
         Constraints on cost vector theta. The default is None.
     regularizer : {'L2_squared', 'L1'}, optional
         Type of regularization on cost vector theta. The default is
         'L2_squared'.
     reg_param : float, optional
         Nonnegative regularization parameter. The default is 0.
+    theta_hat : {tuple(2D ndarray, 2D ndarray, 1D ndarray), None}, optional
+        A priory belief or estimate of the true cost vector
+        theta=(vec(Qyy), vec(Q), q). Should be provided as a tuple
+        (Qyy_hat, Q_hat, q_hat). When None, theta_hat is defined as zeros. The
+        default is None.
     sub_loss : bool, optional
         If True, solve the problem using the Suboptimality loss. Namely,
         searches over the facts of the unit L-infinity sphere for the cost
         vector with the smallest loss. If Theta='nonnegative', only searches
         over the nonnegative facet of the L-1 sphere. If False, solve the
         problem using the Augmented Suboptimality loss. The default is False.
     verbose : bool, optional
@@ -943,25 +896,27 @@
     theta_opt : 1D ndarray
         An optimal cost vector according to the chosen strategy.
 
     """
     try:
         import cvxpy as cp
     except ImportError:
-        print("cvxpy is required for invopt's MIP_quadratic function.")
+        print("cvxpy is required for invopt's mixed_integer_quadratic " +
+              "function.")
 
-    # Check if inputs are valid
+    # Check if the inputs are valid
     check_Theta(Theta)
     check_decision_space(decision_space)
     check_regularizer(regularizer)
     check_reg_parameter(reg_param)
 
     # Warnings
     warning_large_decision_space(decision_space)
-    warning_dist_func_reg_param_sub_loss(dist_func, reg_param, sub_loss)
+    warning_dist_func_sub_loss(dist_func_z, sub_loss)
+    warning_theta_hat_reg_param(theta_hat, reg_param)
 
     N = len(dataset)
 
     if Z is None:
         def Z(s, z): return True
 
     if phi1 is None:
@@ -1000,15 +955,15 @@
                 if Z(w_hat, z):
                     alpha = cp.Variable((1, 1))
                     lamb = cp.Variable((m1, 1))
 
                     if sub_loss:
                         dist = 0
                     else:
-                        dist = dist_func(z_hat, z)
+                        dist = dist_func_z(z_hat, z)
 
                     theta_phi_hat = (y_hat.T @ Qyy @ y_hat
                                      + y_hat.T @ Q @ phi1(w_hat, z_hat)
                                      + q.T @ phi2(w_hat, z_hat))
 
                     lambcBz = lamb.T @ (c - B @ z)
 
@@ -1018,33 +973,44 @@
                                     <= beta[i] - dist]
 
                     off_diag = Q @ phi1(w_hat, z).reshape((u1, 1)) + A.T @ lamb
                     constraints += [cp.bmat([[Qyy, off_diag],
                                              [off_diag.T, 4*alpha]]) >> 0]
                     constraints += [lamb >= 0]
 
-    if sub_loss:
-        constraints += [cp.trace(Qyy) == 1]
-        obj = cp.Minimize(sum_beta)
-    else:
+    if reg_param > 0:
+        if theta_hat is None:
+            Qyy_hat = np.zeros((m2, m2))
+            Q_hat = np.zeros((m2, u1))
+            q_hat = np.zeros((u2, 1))
+        else:
+            Qyy_hat, Q_hat, q_hat = theta_hat
+
         if regularizer == 'L2_squared':
-            Qyy_sum = cp.sum_squares(Qyy)
-            Q_sum = cp.sum_squares(Q)
-            q_sum = cp.sum_squares(q)
+            Qyy_sum = cp.sum_squares(Qyy - Qyy_hat)
+            Q_sum = cp.sum_squares(Q - Q_hat)
+            q_sum = cp.sum_squares(q - q_hat)
             reg_term = (reg_param/2)*(Qyy_sum + Q_sum + q_sum)
         elif regularizer == 'L1':
             tQyy = cp.Variable((m2, m2), symmetric=True)
             tQ = cp.Variable((m2, u1))
             tq = cp.Variable((u2, 1))
             reg_term = reg_param*(cp.sum(tQyy) + cp.sum(tQ) + cp.sum(tq))
-            constraints += [Qyy <= tQyy, -Qyy <= tQyy]
-            constraints += [Q <= tQ, -Q <= tQ]
-            constraints += [q <= tq, -q <= tq]
+            constraints += [Qyy - Qyy_hat <= tQyy, Qyy_hat - Qyy <= tQyy]
+            constraints += [Q - Q_hat <= tQ, Q_hat - Q <= tQ]
+            constraints += [q - q_hat <= tq, q_hat - q <= tq]
+    else:
+        reg_term = 0
 
-        obj = cp.Minimize(reg_term + sum_beta)
+    obj = cp.Minimize(reg_term + sum_beta)
+
+    # Check if trace equality constraint needs to be added to avoid the trivial
+    # solution theta=0
+    if sub_loss and ((reg_param == 0) or (theta_hat is None)):
+        constraints += [cp.trace(Qyy) == 1]
 
     prob = cp.Problem(obj, constraints)
     prob.solve(verbose=verbose)
 
     if prob.status != 'optimal':
         raise Exception('Optimal solution not found. CVXPY status code '
                         f'= {prob.status}. Set the flag verbose=True for more '
@@ -1108,16 +1074,17 @@
         'standard'.
     regularizer : {'L2_squared', 'L1'}, optional
         Type of regularization on cost vector theta. The default is
         'L2_squared'.
     reg_param : float, optional
         Nonnegative regularization parameter. The default is 0.
     theta_hat : {1D ndarray, None}, optional
-        A priory belief or estimate of the true cost vector. When not None,
-        theta_hat is defined as the vector of zeros. The default is None.
+        A priory belief or estimate of the true cost vector. When
+        theta_hat=None, it is defined as the vector of zeros. The default is
+        None.
     batch_type : {float, 'reshuffled'}, optional
         If float, it is the fraction of the dataset used to compute stochastic
         subgradients of the loss function, where batch_type=b means use 10*b %
         of the data to compute (stochastic) subgradients. If
         batch_type='reshuffled', T is the number of epochs instead of the
         number of iterations. For each epoch, run the algorithm for N
         iterations, where N is the size of the dataset. That is, perform one
@@ -1145,35 +1112,42 @@
         is used. The default is False.
     verbose : bool, optional
         If True, prints iteration counter. The default is False.
 
     Raises
     ------
     Exception
-        If unsupported Theta or regularizer. If step = 'exponentiated', and
-        the regularizer is not 'L1'.
+        If unsupported Theta or regularizer. If step = 'exponentiated' and
+        the regularizer is not 'L1' or theta_hat is not None.
 
     Returns
     -------
     theta_T : {1D ndarray, list}
         If callback=None, returns the final (averaged) vector found after T
         iterations of the algorithm. Otherwise, returns a list of size T+1
         with elements callback(theta_t) for t=0,...,T, where theta_t is the
         (averaged) vector after t iterations of the algorithm.
 
     """
-    # Check if inputs are valid
+    # Check if the inputs are valid
     check_Theta(Theta)
     check_regularizer(regularizer)
     check_reg_parameter(reg_param)
 
+    # Warnings
+    warning_theta_hat_reg_param(theta_hat, reg_param)
+
     if (step == 'exponentiated') and (regularizer != 'L1'):
         raise Exception('To use step = \'exponentiated\', '
                         'regularizer = \'L1\' is required.')
 
+    if (step == 'exponentiated') and (theta_hat is not None):
+        raise Exception('To use step = \'exponentiated\', '
+                        'theta_hat = None is required.')
+
     # Get the number of examples and dimension of the problem
     N = len(dataset)
     p = len(theta_0)
 
     if theta_hat is None:
         theta_hat = np.zeros(p)
```

### Comparing `invopt-0.0.3/src/invopt.egg-info/PKG-INFO` & `invopt-0.0.4/src/invopt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invopt
-Version: 0.0.3
+Version: 0.0.4
 Summary: Inverse Optimization with Python
 Author-email: Pedro Zattoni Scroccaro <pedroszattoni@gmail.com>
 Project-URL: Homepage, https://github.com/pedroszattoni/invopt
 Project-URL: Bug Tracker, https://github.com/pedroszattoni/inverse-optimization/issues
 Keywords: inverse-optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -26,18 +26,18 @@
 ```
 InvOpt depends on NumPy. Moreover, some of its functions also depend on gurobipy or cvxpy. You can get a free academic license for Gurobi [here](https://www.gurobi.com/academia/academic-program-and-licenses/).
 
 ## Usage and examples
 
 The following functions are available in the InvOpt package to solving IO problems:
 
-- [`discrete_model_consistent`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_model_consistent): for FOPs with dicrete decision spaces (e.g., binary), and when the dataset is consistent with some cost vector. Can be used to check if the data is consistent.
-- [`discrete_model`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_model): for FOPs with dicrete decision spaces (e.g., binary).
-- [`MIP_linear`](https://github.com/pedroszattoni/invopt/tree/main/examples/MIP_linear): for FOPs with mixed-integer decision spaces and cost functions linear w.r.t. the continuous part of the decision variable.
-- [`MIP_quadratic`](https://github.com/pedroszattoni/invopt/tree/main/examples/MIP_quadratic): for FOPs with mixed-integer decision spaces and cost functions quadratic w.r.t. the continuous part of the decision variable.
+- [`discrete_consistent`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_consistent): for FOPs with dicrete decision spaces (e.g., binary), and when the dataset is consistent with some cost vector. Can be used to check if the data is consistent.
+- [`discrete`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete): for FOPs with dicrete decision spaces (e.g., binary).
+- [`mixed_integer_linear`](https://github.com/pedroszattoni/invopt/tree/main/examples/mixed_integer_linear): for FOPs with mixed-integer decision spaces and cost functions linear w.r.t. the continuous part of the decision variable.
+- [`mixed_integer_quadratic`](https://github.com/pedroszattoni/invopt/tree/main/examples/mixed_integer_quadratic): for FOPs with mixed-integer decision spaces and cost functions quadratic w.r.t. the continuous part of the decision variable.
 - [`FOM`](https://github.com/pedroszattoni/invopt/tree/main/examples/FOM): for general FOPs. Solves IO problem approximately using first-order methods.
 
 ## Contributing
 
 Contributions, pull requests and suggestions are very much welcome. The  [TODO](https://github.com/pedroszattoni/invopt/blob/main/TODO.txt) file contains a number of ideas to possibly improve the InvOpt package.
 
 ## Citing
```

### Comparing `invopt-0.0.3/tests/test_examples.py` & `invopt-0.0.4/tests/test_examples.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-This script runs the entire scrips from the examples folder, and check if any
-exception was raised.
+This script runs all scrips in the examples folder, and check if any exception
+was raised.
 
 Author: Pedro Zattoni Scroccaro
 """
 import unittest
 from os.path import dirname, abspath
 import subprocess
 
@@ -22,29 +22,29 @@
     else:
         print(f"Script {script_name} ran successfully.")
         return True
 
 
 class TestScript(unittest.TestCase):
     def test_binary_LP_consistent_data(self):
-        script_name = 'discrete_model_consistent\\binary_LP_consistent_data.py'
+        script_name = 'discrete_consistent\\binary_LP_consistent_data.py'
         self.assertTrue(test_script(path_to_examples, script_name))
 
     def test_binary_LP_inconsistent_data(self):
-        script_name = 'discrete_model\\binary_LP_inconsistent_data.py'
-        self.assertTrue(test_script(path_to_examples, script_name))
-
-    def test_first_order_methods(self):
-        script_name = 'FOM\\first_order_methods.py'
+        script_name = 'discrete\\binary_LP_inconsistent_data.py'
         self.assertTrue(test_script(path_to_examples, script_name))
 
     def test_MILP(self):
-        script_name = 'MIP_linear\\MILP.py'
+        script_name = 'mixed_integer_linear\\MILP.py'
         self.assertTrue(test_script(path_to_examples, script_name))
 
     def test_MIQP(self):
-        script_name = 'MIP_quadratic\\MIQP.py'
+        script_name = 'mixed_integer_quadratic\\MIQP.py'
+        self.assertTrue(test_script(path_to_examples, script_name))
+
+    def test_first_order_methods(self):
+        script_name = 'FOM\\first_order_methods.py'
         self.assertTrue(test_script(path_to_examples, script_name))
 
 
 if __name__ == '__main__':
     unittest.main()
```

