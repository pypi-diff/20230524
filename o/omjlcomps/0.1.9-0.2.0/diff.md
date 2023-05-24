# Comparing `tmp/omjlcomps-0.1.9.tar.gz` & `tmp/omjlcomps-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omjlcomps-0.1.9.tar", last modified: Fri Mar 17 16:38:22 2023, max compression
+gzip compressed data, was "omjlcomps-0.2.0.tar", last modified: Wed May 24 02:33:16 2023, max compression
```

## Comparing `omjlcomps-0.1.9.tar` & `omjlcomps-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 dingraha  (1002) dingraha  (1002)        0 2023-03-17 16:38:22.651309 omjlcomps-0.1.9/
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)      106 2023-01-19 11:27:29.000000 omjlcomps-0.1.9/MANIFEST.in
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)      168 2023-03-17 16:38:22.651309 omjlcomps-0.1.9/PKG-INFO
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)       38 2023-01-19 11:27:29.000000 omjlcomps-0.1.9/README.md
-drwxr-xr-x   0 dingraha  (1002) dingraha  (1002)        0 2023-03-17 16:38:22.649309 omjlcomps-0.1.9/omjlcomps/
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)    12024 2023-03-17 13:52:15.000000 omjlcomps-0.1.9/omjlcomps/__init__.py
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)      253 2023-03-17 15:36:29.000000 omjlcomps-0.1.9/omjlcomps/juliapkg.json
-drwxr-xr-x   0 dingraha  (1002) dingraha  (1002)        0 2023-03-17 16:38:22.651309 omjlcomps-0.1.9/omjlcomps/test/
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)        0 2023-01-19 11:27:29.000000 omjlcomps-0.1.9/omjlcomps/test/__init__.py
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)     7788 2023-03-17 13:52:15.000000 omjlcomps-0.1.9/omjlcomps/test/test_ecomp.jl
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)    15688 2023-03-17 13:52:15.000000 omjlcomps-0.1.9/omjlcomps/test/test_icomp.jl
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)    15615 2023-03-17 13:52:15.000000 omjlcomps-0.1.9/omjlcomps/test/test_julia_explicit_comp.py
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)    23809 2023-03-17 13:52:15.000000 omjlcomps-0.1.9/omjlcomps/test/test_julia_implicit_comp.py
-drwxr-xr-x   0 dingraha  (1002) dingraha  (1002)        0 2023-03-17 16:38:22.650309 omjlcomps-0.1.9/omjlcomps.egg-info/
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)      168 2023-03-17 16:38:22.000000 omjlcomps-0.1.9/omjlcomps.egg-info/PKG-INFO
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)      447 2023-03-17 16:38:22.000000 omjlcomps-0.1.9/omjlcomps.egg-info/SOURCES.txt
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)        1 2023-03-17 16:38:22.000000 omjlcomps-0.1.9/omjlcomps.egg-info/dependency_links.txt
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)      117 2023-03-17 16:38:22.000000 omjlcomps-0.1.9/omjlcomps.egg-info/entry_points.txt
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)       28 2023-03-17 16:38:22.000000 omjlcomps-0.1.9/omjlcomps.egg-info/requires.txt
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)       10 2023-03-17 16:38:22.000000 omjlcomps-0.1.9/omjlcomps.egg-info/top_level.txt
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)       38 2023-03-17 16:38:22.651309 omjlcomps-0.1.9/setup.cfg
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)      585 2023-03-17 15:35:37.000000 omjlcomps-0.1.9/setup.py
+drwxr-xr-x   0 dingraha  (1002) dingraha  (1002)        0 2023-05-24 02:33:16.290444 omjlcomps-0.2.0/
+-rw-r--r--   0 dingraha  (1002) dingraha  (1002)      106 2023-01-19 11:27:29.000000 omjlcomps-0.2.0/MANIFEST.in
+-rw-r--r--   0 dingraha  (1002) dingraha  (1002)      168 2023-05-24 02:33:16.290444 omjlcomps-0.2.0/PKG-INFO
+-rw-r--r--   0 dingraha  (1002) dingraha  (1002)       38 2023-01-19 11:27:29.000000 omjlcomps-0.2.0/README.md
+drwxr-xr-x   0 dingraha  (1002) dingraha  (1002)        0 2023-05-24 02:33:16.285444 omjlcomps-0.2.0/omjlcomps/
+-rw-r--r--   0 dingraha  (1002) dingraha  (1002)    12319 2023-05-20 11:38:03.000000 omjlcomps-0.2.0/omjlcomps/__init__.py
+-rw-r--r--   0 dingraha  (1002) dingraha  (1002)      300 2023-05-24 01:37:31.000000 omjlcomps-0.2.0/omjlcomps/juliapkg.json
+drwxr-xr-x   0 dingraha  (1002) dingraha  (1002)        0 2023-05-24 02:33:16.289444 omjlcomps-0.2.0/omjlcomps/test/
+-rw-r--r--   0 dingraha  (1002) dingraha  (1002)        0 2023-01-19 11:27:29.000000 omjlcomps-0.2.0/omjlcomps/test/__init__.py
+-rw-r--r--   0 dingraha  (1002) dingraha  (1002)     8146 2023-03-17 19:37:43.000000 omjlcomps-0.2.0/omjlcomps/test/test_ecomp.jl
+-rw-r--r--   0 dingraha  (1002) dingraha  (1002)    15739 2023-03-17 19:37:43.000000 omjlcomps-0.2.0/omjlcomps/test/test_icomp.jl
+-rw-r--r--   0 dingraha  (1002) dingraha  (1002)    15620 2023-03-17 19:37:43.000000 omjlcomps-0.2.0/omjlcomps/test/test_julia_explicit_comp.py
+-rw-r--r--   0 dingraha  (1002) dingraha  (1002)    23809 2023-03-17 13:52:15.000000 omjlcomps-0.2.0/omjlcomps/test/test_julia_implicit_comp.py
+drwxr-xr-x   0 dingraha  (1002) dingraha  (1002)        0 2023-05-24 02:33:16.287444 omjlcomps-0.2.0/omjlcomps.egg-info/
+-rw-r--r--   0 dingraha  (1002) dingraha  (1002)      168 2023-05-24 02:33:16.000000 omjlcomps-0.2.0/omjlcomps.egg-info/PKG-INFO
+-rw-r--r--   0 dingraha  (1002) dingraha  (1002)      447 2023-05-24 02:33:16.000000 omjlcomps-0.2.0/omjlcomps.egg-info/SOURCES.txt
+-rw-r--r--   0 dingraha  (1002) dingraha  (1002)        1 2023-05-24 02:33:16.000000 omjlcomps-0.2.0/omjlcomps.egg-info/dependency_links.txt
+-rw-r--r--   0 dingraha  (1002) dingraha  (1002)      117 2023-05-24 02:33:16.000000 omjlcomps-0.2.0/omjlcomps.egg-info/entry_points.txt
+-rw-r--r--   0 dingraha  (1002) dingraha  (1002)       36 2023-05-24 02:33:16.000000 omjlcomps-0.2.0/omjlcomps.egg-info/requires.txt
+-rw-r--r--   0 dingraha  (1002) dingraha  (1002)       10 2023-05-24 02:33:16.000000 omjlcomps-0.2.0/omjlcomps.egg-info/top_level.txt
+-rw-r--r--   0 dingraha  (1002) dingraha  (1002)       38 2023-05-24 02:33:16.290444 omjlcomps-0.2.0/setup.cfg
+-rw-r--r--   0 dingraha  (1002) dingraha  (1002)      593 2023-05-24 01:43:58.000000 omjlcomps-0.2.0/setup.py
```

### Comparing `omjlcomps-0.1.9/omjlcomps/__init__.py` & `omjlcomps-0.2.0/omjlcomps/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,17 +52,17 @@
 
 def _setup_partials_common(self):
     if jl.OpenMDAOCore.has_setup_partials(self._jlcomp):
         # Ignore the partials data from `setup`, since we've already passed that to `declare_partials` in `_setup_common`.
         input_data, output_data, _ = jl.OpenMDAOCore.setup(self._jlcomp)
 
         # Build up a dict mapping the input names to their size.
-        input_sizes = juliacall.convert(jl.Dict, {vd.name: self._get_var_meta(vd.name, "size") for vd in input_data})
+        input_sizes = juliacall.convert(jl.Dict, {vd.name: self._get_var_meta(vd.name, "shape") for vd in input_data})
         # Build up a dict mapping the output names to their size.
-        output_sizes = juliacall.convert(jl.Dict, {vd.name: self._get_var_meta(vd.name, "size") for vd in output_data})
+        output_sizes = juliacall.convert(jl.Dict, {vd.name: self._get_var_meta(vd.name, "shape") for vd in output_data})
 
         partials_data = jl.OpenMDAOCore.setup_partials(self._jlcomp, input_sizes, output_sizes)
         for data in partials_data:
             self.declare_partials(data.of, data.wrt,
                                   rows=data.rows, cols=data.cols,
                                   val=data.val, method=data.method)
 
@@ -118,14 +118,16 @@
                 except JuliaError as e:
                     if jl.isa(e.exception, jl.DomainError):
                         raise AnalysisError(f"caught Julia DomainError in {self}.compute_jacvec_product:\n{e}")
                     else:
                         raise e from None
 
             self.compute_jacvec_product = MethodType(compute_jacvec_product, self)
+            # https://github.com/OpenMDAO/OpenMDAO/pull/2802
+            self.matrix_free = True
 
     def setup_partials(self):
         _setup_partials_common(self)
 
 
     def compute(self, inputs, outputs):
         inputs_dict = juliacall.convert(jl.Dict, dict(inputs))
@@ -183,14 +185,16 @@
                 except JuliaError as e:
                     if jl.isa(e.exception, jl.DomainError):
                         raise AnalysisError(f"caught Julia DomainError in {self}.solve_nonlinear:\n{e}")
                     else:
                         raise e from None
 
             self.solve_nonlinear = MethodType(solve_nonlinear, self)
+            # https://github.com/OpenMDAO/OpenMDAO/pull/2802
+            self._has_solve_nl = True
 
         if jl.OpenMDAOCore.has_linearize(self._jlcomp):
             def linearize(self, inputs, outputs, partials):
                 inputs_dict = juliacall.convert(jl.Dict, dict(inputs))
                 outputs_dict = juliacall.convert(jl.Dict, dict(outputs))
 
                 partials_dict = {}
@@ -224,14 +228,16 @@
                 except JuliaError as e:
                     if jl.isa(e.exception, jl.DomainError):
                         raise AnalysisError(f"caught Julia DomainError in {self}.apply_linear:\n{e}")
                     else:
                         raise e from None
 
             self.apply_linear = MethodType(apply_linear, self)
+            # https://github.com/OpenMDAO/OpenMDAO/pull/2802
+            self.matrix_free = True
 
         if jl.OpenMDAOCore.has_solve_linear(self._jlcomp):
             def solve_linear(self, d_outputs, d_residuals, mode):
                 d_outputs_dict = juliacall.convert(jl.Dict, dict(d_outputs))
                 d_residuals_dict = juliacall.convert(jl.Dict, dict(d_residuals))
 
                 try:
```

### Comparing `omjlcomps-0.1.9/omjlcomps/test/test_ecomp.jl` & `omjlcomps-0.2.0/omjlcomps/test/test_ecomp.jl`

 * *Files 3% similar despite different names*

```diff
@@ -227,28 +227,33 @@
     partials_data = []
 
     return input_data, output_data, partials_data
 end
 
 function OpenMDAOCore.setup_partials(self::ECompShapeByConn, input_sizes, output_sizes)
     @assert input_sizes["x"] == output_sizes["y"]
-    n = only(input_sizes["x"])
-    partials_data = [PartialsData("y", "x"; rows=0:n-1, cols=0:n-1)]
+    m, n = input_sizes["x"]
+    rows, cols = OpenMDAOCore.get_rows_cols(ss_sizes=Dict(:i=>m, :j=>n), of_ss=[:i, :j], wrt_ss=[:i, :j])
+    partials_data = [PartialsData("y", "x"; rows=rows, cols=cols)]
 
     return partials_data
 end
 
 function OpenMDAOCore.compute!(self::ECompShapeByConn, inputs, outputs)
     x = inputs["x"]
     y = outputs["y"]
     y .= 2 .* x.^2 .+ 1
     return nothing
 end
 
 function OpenMDAOCore.compute_partials!(self::ECompShapeByConn, inputs, partials)
     x = inputs["x"]
-    dydx = partials["y", "x"]
+    m, n = size(x)
+    # So, with the way I've declared the partials above, OpenMDAO will have
+    # created a Numpy array of shape (m, n) and then flattened it. So, to get
+    # that to work, I'll need to do this:
+    dydx = PermutedDimsArray(reshape(partials["y", "x"], n, m), (2, 1))
     dydx .= 4 .* x
     return nothing
 end
 
 end # module
```

### Comparing `omjlcomps-0.1.9/omjlcomps/test/test_icomp.jl` & `omjlcomps-0.2.0/omjlcomps/test/test_icomp.jl`

 * *Files 2% similar despite different names*

```diff
@@ -514,18 +514,18 @@
         VarData("z2"; val=3.0, shape_by_conn=true, copy_shape="x")]
 
     partials = []
     return inputs, outputs, partials
 end
 
 function OpenMDAOCore.setup_partials(self::ImplicitShapeByConn, input_sizes, output_sizes)
-    n = input_sizes["x"]
-    @assert input_sizes["y"] == n
-    @assert output_sizes["z1"] == n
-    @assert output_sizes["z2"] == n
+    @assert input_sizes["y"] == input_sizes["x"]
+    @assert output_sizes["z1"] == input_sizes["x"]
+    @assert output_sizes["z2"] == input_sizes["x"]
+    n = only(input_sizes["x"])
     rows = 0:n-1
     cols = 0:n-1
     partials = [
         PartialsData("z1", "x"; rows=rows, cols=cols),
         PartialsData("z1", "y"; rows, cols),
         PartialsData("z1", "z1"; rows, cols),
         PartialsData("z2", "x"; rows, cols),
```

### Comparing `omjlcomps-0.1.9/omjlcomps/test/test_julia_explicit_comp.py` & `omjlcomps-0.2.0/omjlcomps/test/test_julia_explicit_comp.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,15 +340,15 @@
 
 
 class TestShapeByConn(unittest.TestCase):
     def setUp(self):
         p = self.p = om.Problem()
         n = 8
         comp = om.IndepVarComp()
-        comp.add_output("x", shape=n)
+        comp.add_output("x", shape=(n, n))
         p.model.add_subsystem("inputs_comp", comp, promotes_outputs=["x"])
 
         comp = JuliaExplicitComp(jlcomp=jl.ECompTest.ECompShapeByConn())
         p.model.add_subsystem("ecomp", comp, promotes_inputs=["x"], promotes_outputs=["y"])
 
         p.setup(force_alloc_complex=True)
         p.set_val("x", np.arange(n))
```

### Comparing `omjlcomps-0.1.9/omjlcomps/test/test_julia_implicit_comp.py` & `omjlcomps-0.2.0/omjlcomps/test/test_julia_implicit_comp.py`

 * *Files identical despite different names*

### Comparing `omjlcomps-0.1.9/setup.py` & `omjlcomps-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 setup_args = {'description': 'Create OpenMDAO Components using the Julia programming language',
    'entry_points': {
        'openmdao_component': [
            'juliaexplicitcomp=omjlcomps:JuliaExplicitComp',
            'juliaimplicitcomp=omjlcomps:JuliaImplicitComp'
        ]
     },
-   'install_requires': ['openmdao', 'juliapkg', 'juliacall'],
+   'install_requires': ['openmdao~=3.26.0', 'juliapkg', 'juliacall'],
    'keywords': ['openmdao_component'],
    'license': 'MIT',
    'name': 'omjlcomps',
    'packages': ['omjlcomps', 'omjlcomps.test'],
-   'version': '0.1.9',
+   'version': '0.2.0',
    'include_package_data': True}
 
 setup(**setup_args)
```

