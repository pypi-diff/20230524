# Comparing `tmp/CUQIpy-FEniCS-0.3.0.post0.dev36.tar.gz` & `tmp/CUQIpy-FEniCS-0.3.0.post0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CUQIpy-FEniCS-0.3.0.post0.dev36.tar", last modified: Wed May 24 08:58:05 2023, max compression
+gzip compressed data, was "CUQIpy-FEniCS-0.3.0.post0.dev5.tar", last modified: Thu Apr 27 13:30:34 2023, max compression
```

## Comparing `CUQIpy-FEniCS-0.3.0.post0.dev36.tar` & `CUQIpy-FEniCS-0.3.0.post0.dev5.tar`

### file list

```diff
@@ -1,25 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:58:05.047409 CUQIpy-FEniCS-0.3.0.post0.dev36/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:58:05.043409 CUQIpy-FEniCS-0.3.0.post0.dev36/CUQIpy_FEniCS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42479 2023-05-24 08:58:05.000000 CUQIpy-FEniCS-0.3.0.post0.dev36/CUQIpy_FEniCS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-24 08:58:05.000000 CUQIpy-FEniCS-0.3.0.post0.dev36/CUQIpy_FEniCS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 08:58:05.000000 CUQIpy-FEniCS-0.3.0.post0.dev36/CUQIpy_FEniCS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 08:58:05.000000 CUQIpy-FEniCS-0.3.0.post0.dev36/CUQIpy_FEniCS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-24 08:58:05.000000 CUQIpy-FEniCS-0.3.0.post0.dev36/CUQIpy_FEniCS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 08:57:56.000000 CUQIpy-FEniCS-0.3.0.post0.dev36/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42479 2023-05-24 08:58:05.047409 CUQIpy-FEniCS-0.3.0.post0.dev36/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-24 08:57:56.000000 CUQIpy-FEniCS-0.3.0.post0.dev36/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:58:05.047409 CUQIpy-FEniCS-0.3.0.post0.dev36/cuqipy_fenics/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-24 08:57:56.000000 CUQIpy-FEniCS-0.3.0.post0.dev36/cuqipy_fenics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-24 08:58:05.047409 CUQIpy-FEniCS-0.3.0.post0.dev36/cuqipy_fenics/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-05-24 08:57:56.000000 CUQIpy-FEniCS-0.3.0.post0.dev36/cuqipy_fenics/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    18510 2023-05-24 08:57:56.000000 CUQIpy-FEniCS-0.3.0.post0.dev36/cuqipy_fenics/pde.py
--rw-r--r--   0 runner    (1001) docker     (123)    18458 2023-05-24 08:57:56.000000 CUQIpy-FEniCS-0.3.0.post0.dev36/cuqipy_fenics/testproblem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-24 08:57:56.000000 CUQIpy-FEniCS-0.3.0.post0.dev36/cuqipy_fenics/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-24 08:57:56.000000 CUQIpy-FEniCS-0.3.0.post0.dev36/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-24 08:57:56.000000 CUQIpy-FEniCS-0.3.0.post0.dev36/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 08:58:05.047409 CUQIpy-FEniCS-0.3.0.post0.dev36/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-24 08:57:56.000000 CUQIpy-FEniCS-0.3.0.post0.dev36/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:58:05.043409 CUQIpy-FEniCS-0.3.0.post0.dev36/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13573 2023-05-24 08:57:56.000000 CUQIpy-FEniCS-0.3.0.post0.dev36/tests/test_PDEModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-24 08:57:56.000000 CUQIpy-FEniCS-0.3.0.post0.dev36/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-05-24 08:57:56.000000 CUQIpy-FEniCS-0.3.0.post0.dev36/tests/test_testproblem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:34.167682 CUQIpy-FEniCS-0.3.0.post0.dev5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:34.167682 CUQIpy-FEniCS-0.3.0.post0.dev5/CUQIpy_FEniCS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42478 2023-04-27 13:30:34.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/CUQIpy_FEniCS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-27 13:30:34.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/CUQIpy_FEniCS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:30:34.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/CUQIpy_FEniCS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 13:30:34.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/CUQIpy_FEniCS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 13:30:34.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/CUQIpy_FEniCS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 13:30:24.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42478 2023-04-27 13:30:34.167682 CUQIpy-FEniCS-0.3.0.post0.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-27 13:30:24.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:34.167682 CUQIpy-FEniCS-0.3.0.post0.dev5/cuqipy_fenics/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-27 13:30:24.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/cuqipy_fenics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-27 13:30:34.167682 CUQIpy-FEniCS-0.3.0.post0.dev5/cuqipy_fenics/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-04-27 13:30:24.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/cuqipy_fenics/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18227 2023-04-27 13:30:24.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/cuqipy_fenics/pde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-04-27 13:30:24.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/cuqipy_fenics/testproblem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-27 13:30:24.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-27 13:30:24.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 13:30:34.167682 CUQIpy-FEniCS-0.3.0.post0.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-27 13:30:24.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:34.167682 CUQIpy-FEniCS-0.3.0.post0.dev5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13498 2023-04-27 13:30:24.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/tests/test_PDEModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-27 13:30:24.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/tests/test_geometry.py
```

### Comparing `CUQIpy-FEniCS-0.3.0.post0.dev36/CUQIpy_FEniCS.egg-info/PKG-INFO` & `CUQIpy-FEniCS-0.3.0.post0.dev5/CUQIpy_FEniCS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUQIpy-FEniCS
-Version: 0.3.0.post0.dev36
+Version: 0.3.0.post0.dev5
 Summary: CUQIpy plugin for FEniCS
 Maintainer-email: "Nicolai A. B. Riis" <nabr@dtu.dk>, "Jakob S. Jørgensen" <jakj@dtu.dk>, "Amal M. Alghamdi" <amaal@dtu.dk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `CUQIpy-FEniCS-0.3.0.post0.dev36/LICENSE` & `CUQIpy-FEniCS-0.3.0.post0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `CUQIpy-FEniCS-0.3.0.post0.dev36/PKG-INFO` & `CUQIpy-FEniCS-0.3.0.post0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUQIpy-FEniCS
-Version: 0.3.0.post0.dev36
+Version: 0.3.0.post0.dev5
 Summary: CUQIpy plugin for FEniCS
 Maintainer-email: "Nicolai A. B. Riis" <nabr@dtu.dk>, "Jakob S. Jørgensen" <jakj@dtu.dk>, "Amal M. Alghamdi" <amaal@dtu.dk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `CUQIpy-FEniCS-0.3.0.post0.dev36/README.md` & `CUQIpy-FEniCS-0.3.0.post0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `CUQIpy-FEniCS-0.3.0.post0.dev36/cuqipy_fenics/geometry.py` & `CUQIpy-FEniCS-0.3.0.post0.dev5/cuqipy_fenics/geometry.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-FEniCS-0.3.0.post0.dev36/cuqipy_fenics/pde.py` & `CUQIpy-FEniCS-0.3.0.post0.dev5/cuqipy_fenics/pde.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,19 +39,19 @@
 
     solution_function_space : FEniCS function space
         FEniCS function space object that defines the function space of the state variable (solution variable).
 
     parameter_function_space : FEniCS function space
         FEniCS function space object that defines the function space of the Bayesian parameter (input of the forward model).
 
-    dirichlet_bcs: FEniCS Dirichlet boundary condition object or a list of them
-        FEniCS Dirichlet boundary condition object(s) that define the Dirichlet boundary conditions of the PDE.
+    dirichlet_bc : FEniCS Dirichlet boundary condition object
+        FEniCS Dirichlet boundary condition object that defines the Dirichlet boundary conditions of the PDE.
 
-    adjoint_dirichlet_bcs : FEniCS Dirichlet boundary condition object or a list of them, required if the gradient is to be computed
-        FEniCS Dirichlet boundary condition object(s) that define the Dirichlet boundary conditions of the adjoint PDE.
+    adjoint_dirichlet_bc : FEniCS Dirichlet boundary condition object, required if the gradient is to be computed
+        FEniCS Dirichlet boundary condition object that defines the Dirichlet boundary conditions of the adjoint PDE.
 
     observation_operator : python function handle, optional
         Function handle of a python function that returns the observed quantity from the PDE solution. If not provided, the identity operator is assumed (i.e. the entire solution is observed).
         This python function takes as input the Bayesian parameter (input of the forward model) and the state variable (solution variable) as first and second inputs, respectively.
 
         The returned observed quantity can be a ufl.algebra.Operator, FEniCS Function, np.ndarray, int, or float.
 
@@ -82,15 +82,15 @@
         parameter_function_space = dl.FunctionSpace(mesh, 'Lagrange', 1)
         
         # Set up Dirichlet boundaries
         def u_boundary(x, on_boundary):
             return on_boundary
         
         dirichlet_bc_expr = dl.Expression("0", degree=1) 
-        dirichlet_bcs = dl.DirichletBC(solution_function_space,
+        dirichlet_bc = dl.DirichletBC(solution_function_space,
                                       dirichlet_bc_expr,
                                       u_boundary)
         
         # Set up PDE variational form
         def lhs_form(m,u,p):
             return ufl.exp(m)*ufl.inner(ufl.grad(u), ufl.grad(p))*ufl.dx 
         
@@ -99,36 +99,34 @@
         
         # Create the PDE object 
         PDE = cuqipy_fenics.pde.SteadyStateLinearFEniCSPDE( 
                 (lhs_form, rhs_form),
                 mesh, 
                 parameter_function_space=parameter_function_space,
                 solution_function_space=solution_function_space,
-                dirichlet_bcs=dirichlet_bcs)
+                dirichlet_bc=dirichlet_bc)
             
 
     """
 
     def __init__(self, PDE_form, mesh, solution_function_space,
-                 parameter_function_space, dirichlet_bcs, adjoint_dirichlet_bcs=None,
+                 parameter_function_space, dirichlet_bc, adjoint_dirichlet_bc=None,
                  observation_operator=None, reuse_assembled=False, linalg_solve=None,
                  linalg_solve_kwargs=None):
 
         if PDE_form is None:
             raise ValueError('PDE_form should be provided and cannot be None.')
 
         self._form = PDE_form
 
         self.mesh = mesh
         self.solution_function_space = solution_function_space
         self.parameter_function_space = parameter_function_space
-        self._dirichlet_bcs = dirichlet_bcs if isinstance(
-            dirichlet_bcs, list) else [dirichlet_bcs]
-        self._adjoint_dirichlet_bcs = adjoint_dirichlet_bcs if isinstance(
-            adjoint_dirichlet_bcs, list) else [adjoint_dirichlet_bcs]
+        self.dirichlet_bc = dirichlet_bc
+        self.adjoint_dirichlet_bc = adjoint_dirichlet_bc
         self.observation_operator = observation_operator
         self.reuse_assembled = reuse_assembled
 
         if linalg_solve is None:
             linalg_solve = dl.LUSolver()
         if linalg_solve_kwargs is None:
             linalg_solve_kwargs = {}
@@ -336,43 +334,43 @@
                                         self._solution_test_function))
 
         if self.rhs.empty():
             self.rhs = dl.Constant(0)*self._solution_test_function*dl.dx
 
         diff_op = dl.assemble(diff_op)
         self.rhs = dl.assemble(self.rhs)
-        for bc in self._dirichlet_bcs: 
-            bc.apply(diff_op)
-            bc.apply(self.rhs)
+
+        self.dirichlet_bc.apply(diff_op)
+        self.dirichlet_bc.apply(self.rhs)
         self._solver.set_operator(diff_op)
         self._flags["is_operator_valid"] = True
 
     def _assemble_lhs(self):
         """ Assemble the lhs form """
         if self.reuse_assembled\
                 and self._flags["is_operator_valid"]:
             return
 
         diff_op = dl.assemble(self.lhs_form(self.parameter,
                                             self._solution_trial_function,
                                             self._solution_test_function))
 
-        for bc in self._dirichlet_bcs: bc.apply(diff_op)
+        self.dirichlet_bc.apply(diff_op)
         self._solver.set_operator(diff_op)
         self._flags["is_operator_valid"] = True
 
     def _assemble_rhs(self):
         """ Assemble the rhs form """
         if self.reuse_assembled\
                 and self.rhs is not None:
             return
 
         self.rhs = dl.assemble(self.rhs_form(self.parameter,
                                              self._solution_test_function))
-        for bc in self._dirichlet_bcs: bc.apply(self.rhs)
+        self.dirichlet_bc.apply(self.rhs)
 
 
     def solve(self):
         self.forward_solution = dl.Function(self.solution_function_space)       
         self._solver.solve(self.forward_solution.vector(), self.rhs)
         return self.forward_solution, None
 
@@ -387,41 +385,40 @@
 
         Note: This implementation is largely based on the code:
         https://github.com/hippylib/hippylib/blob/master/hippylib/modeling/PDEProblem.py
 
         See also: Gunzburger, M. D. (2002). Perspectives in flow control and optimization. Society for Industrial and Applied Mathematics, for adjoint based derivative derivation. 
         """
         # Raise an error if the adjoint boundary conditions are not provided
-        if self._adjoint_dirichlet_bcs is None:
+        if self.adjoint_dirichlet_bc is None:
             raise ValueError(
                 "The adjoint Dirichlet boundary conditions are not defined.")
 
         # Create needed functions
         trial_adjoint = dl.TrialFunction(self.solution_function_space)
         adjoint = dl.Function(self.solution_function_space)
 
         # Compute forward solution
         # TODO: Use stored forward solution if available and wrt == self.parameter
         self.parameter = wrt
-        self.assemble()
         self.forward_solution, _ = self.solve()
 
         # Compute adjoint solution
         test_parameter = dl.TestFunction(self.parameter_function_space)
         test_solution = dl.TestFunction(self.solution_function_space)
 
         # note: temp_form is a weak form used for building the adjoint operator
         temp_form = self.PDE_form(wrt, self.forward_solution, trial_adjoint)
         adjoint_form = dl.derivative(
             temp_form, self.forward_solution, test_solution)
 
         adjoint_matrix, _ = dl.assemble_system(
             adjoint_form,
             ufl.inner(self.forward_solution, test_solution) * ufl.dx,
-            self._adjoint_dirichlet_bcs,
+            self.adjoint_dirichlet_bc,
         )
 
         #TODO: account for observation operator
         if self.observation_operator is not None:
             raise NotImplementedError(
                 "Gradient wrt parameter for PDE with observation operator not implemented")
```

### Comparing `CUQIpy-FEniCS-0.3.0.post0.dev36/pyproject.toml` & `CUQIpy-FEniCS-0.3.0.post0.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `CUQIpy-FEniCS-0.3.0.post0.dev36/tests/test_PDEModel.py` & `CUQIpy-FEniCS-0.3.0.post0.dev5/tests/test_PDEModel.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,28 +50,28 @@
 
     # Create a PDE object with Krylov solver
     PDE_with_solver1 = cuqipy_fenics.pde.SteadyStateLinearFEniCSPDE(
         poisson.form,
         poisson.mesh,
         poisson.solution_function_space,
         poisson.parameter_function_space,
-        poisson.bcs,
+        poisson.bc,
         linalg_solve=dl.KrylovSolver())
 
     # Solve the PDE
     PDE_with_solver1.assemble(m)
     u1, info = PDE_with_solver1.solve()
 
     # Create a PDE object with direct LU solver
     PDE_with_solver2 = cuqipy_fenics.pde.SteadyStateLinearFEniCSPDE(
         poisson.form,
         poisson.mesh,
         poisson.solution_function_space,
         poisson.parameter_function_space,
-        poisson.bcs,
+        poisson.bc,
         linalg_solve=dl.LUSolver())
 
     # Solve the PDE
     PDE_with_solver2.assemble(m)
     u2, info = PDE_with_solver2.solve()
 
     # Check that the solutions are the same
@@ -93,24 +93,24 @@
     # but reuse_assembled is True
     with pytest.raises(ValueError):
         PDE = cuqipy_fenics.pde.SteadyStateLinearFEniCSPDE(
             poisson.form,
             poisson.mesh,
             poisson.solution_function_space,
             poisson.parameter_function_space,
-            poisson.bcs,
+            poisson.bc,
             reuse_assembled=True)
 
     # Create a PDE object
     PDE = cuqipy_fenics.pde.SteadyStateLinearFEniCSPDE(
         (poisson.lhs_form, poisson.rhs_form),
         poisson.mesh,
         poisson.solution_function_space,
         poisson.parameter_function_space,
-        poisson.bcs,
+        poisson.bc,
         reuse_assembled=True)
 
     # Solve the PDE
     PDE.assemble(m)
     u1, info = PDE.solve()
 
     # update the parameter and solve again
@@ -147,27 +147,27 @@
 
     # Create a PDE object with full form
     PDE_with_full_form = cuqipy_fenics.pde.SteadyStateLinearFEniCSPDE(
         poisson.form,
         poisson.mesh,
         poisson.solution_function_space,
         poisson.parameter_function_space,
-        poisson.bcs)
+        poisson.bc)
 
     # Solve the PDE
     PDE_with_full_form.assemble(m)
     u1, info = PDE_with_full_form.solve()
 
     # Create a PDE object with lhs and rhs forms
     PDE_with_lhs_rhs_forms = cuqipy_fenics.pde.SteadyStateLinearFEniCSPDE(
         (poisson.lhs_form, poisson.rhs_form),
         poisson.mesh,
         poisson.solution_function_space,
         poisson.parameter_function_space,
-        poisson.bcs)
+        poisson.bc)
 
     # Solve the PDE
     PDE_with_lhs_rhs_forms.assemble(m)
     u2, info = PDE_with_lhs_rhs_forms.solve()
 
     # Check that the solutions are the same
     assert np.allclose(u1.vector().get_local(), u2.vector().get_local())
@@ -182,46 +182,46 @@
     # Skip case 2 test if the operating system is not Mac OS X
     if  case == 2 and not sys.platform.startswith('darwin'):
         pytest.skip("Test on MAC OS only")
 
     # Set up first poisson problem
     poisson1 = Poisson()
     poisson1.mesh = dl.UnitSquareMesh(40, 40)
-    poisson1.source_term = dl.Constant(1.0)
+    poisson1.f = dl.Constant(1.0)
 
     # Set up second poisson problem
     poisson2 = Poisson()
     poisson2.mesh = poisson1.mesh
-    poisson2.source_term = dl.Expression("sin(2*x[0]*pi)*sin(2*x[1]*pi)", degree=1)
+    poisson2.f = dl.Expression("sin(2*x[0]*pi)*sin(2*x[1]*pi)", degree=1)
 
     # Set up boundary function (where the Dirichlet boundary conditions are applied)
     def u_boundary(x, on_boundary):
         return on_boundary and\
             (x[0] < dl.DOLFIN_EPS or x[0] > 1.0 - dl.DOLFIN_EPS)
 
-    poisson1.bcs = dl.DirichletBC(poisson1.solution_function_space,
+    poisson1.bc = dl.DirichletBC(poisson1.solution_function_space,
                                  dl.Constant(0.0), u_boundary)
-    poisson2.bcs = poisson1.bcs
+    poisson2.bc = poisson1.bc
 
     # Create two PDE objects with different rhs terms
     PDE1 = cuqipy_fenics.pde.SteadyStateLinearFEniCSPDE(
         (poisson1.lhs_form, poisson1.rhs_form),
         poisson1.mesh,
         parameter_function_space=poisson1.parameter_function_space,
         solution_function_space=poisson1.solution_function_space,
-        dirichlet_bcs=poisson1.bcs,
+        dirichlet_bc=poisson1.bc,
         observation_operator=None,
         reuse_assembled=False)
 
     PDE2 = cuqipy_fenics.pde.SteadyStateLinearFEniCSPDE(
         (poisson2.lhs_form, poisson2.rhs_form),
         poisson2.mesh,
         parameter_function_space=poisson2.parameter_function_space,
         solution_function_space=poisson2.solution_function_space,
-        dirichlet_bcs=poisson2.bcs,
+        dirichlet_bc=poisson2.bc,
         observation_operator=None,
         reuse_assembled=False)
 
     # Create domain geometry
     fenics_continuous_geo = cuqipy_fenics.geometry.FEniCSContinuous(
         poisson1.parameter_function_space)
     domain_geometry = cuqipy_fenics.geometry.MaternKLExpansion(
@@ -315,49 +315,49 @@
         # parameter
         self.mesh = dl.UnitIntervalMesh(10)
 
         # Define the boundary condition
         self.bc_value = dl.Constant(0.0)
 
         # the source term
-        self.source_term = dl.Expression('x[0]', degree=1)
+        self.f = dl.Expression('x[0]', degree=1)
 
     @property
     def form(self):
         return lambda m, u, v:\
             ufl.exp(m)*ufl.inner(ufl.grad(u), ufl.grad(v))*ufl.dx\
-            + self.source_term*v*ufl.dx
+            + self.f*v*ufl.dx
 
     @property
     def lhs_form(self):
         return lambda m, u, v:\
             ufl.exp(m)*ufl.inner(ufl.grad(u), ufl.grad(v))*ufl.dx
 
     @property
     def rhs_form(self):
-        return lambda m, v: -self.source_term*v*ufl.dx
+        return lambda m, v: -self.f*v*ufl.dx
 
     @property
     def solution_function_space(self):
         return dl.FunctionSpace(self.mesh, "Lagrange", 2)
 
     @property
     def parameter_function_space(self):
         return dl.FunctionSpace(self.mesh, "Lagrange", 1)
 
     @property
-    def bcs(self):
-        if not hasattr(self, "_bcs") or self._bcs is None:
-            self._bcs = dl.DirichletBC(self.solution_function_space,
+    def bc(self):
+        if not hasattr(self, "_bc") or self._bc is None:
+            self._bc = dl.DirichletBC(self.solution_function_space,
                                       self.bc_value, "on_boundary")
-        return self._bcs
+        return self._bc
 
-    @bcs.setter
-    def bcs(self, bcs):
-        self._bcs = bcs
+    @bc.setter
+    def bc(self, bc):
+        self._bc = bc
 
 
 def test_observation_operator_setter():
     """Test that the observation setter works as expected"""
     # Create the variational problem
     poisson = Poisson()
     poisson.mesh = dl.UnitSquareMesh(50, 50)
@@ -371,25 +371,25 @@
 
     # Create a PDE object (set observation_operator through setter)
     PDE1 = cuqipy_fenics.pde.SteadyStateLinearFEniCSPDE(
         (poisson.lhs_form, poisson.rhs_form),
         poisson.mesh,
         poisson.solution_function_space,
         poisson.parameter_function_space,
-        poisson.bcs,
+        poisson.bc,
         observation_operator=None)
     PDE1.observation_operator = observation_operator
 
     # Create a PDE object (pass observation_operator as argument)  
     PDE2 = cuqipy_fenics.pde.SteadyStateLinearFEniCSPDE(
         (poisson.lhs_form, poisson.rhs_form),
         poisson.mesh,
         poisson.solution_function_space,
         poisson.parameter_function_space,
-        poisson.bcs,
+        poisson.bc,
         observation_operator=observation_operator)
 
     # Solve the first PDE
     PDE1.assemble(m)
     u1, info = PDE1.solve()
     u1_obs = PDE1.observe(u1)
```

### Comparing `CUQIpy-FEniCS-0.3.0.post0.dev36/tests/test_geometry.py` & `CUQIpy-FEniCS-0.3.0.post0.dev5/tests/test_geometry.py`

 * *Files identical despite different names*

