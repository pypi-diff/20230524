# Comparing `tmp/treeordination-1.3.0.tar.gz` & `tmp/treeordination-1.3.1.tar.gz`

## Comparing `treeordination-1.3.0.tar` & `treeordination-1.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 treeordination-1.3.0/environment.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 treeordination-1.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 treeordination-1.3.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 treeordination-1.3.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 treeordination-1.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 treeordination-1.3.0/TreeOrdination/TreeOrdination.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 treeordination-1.3.0/TreeOrdination/__init__.py
--rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 treeordination-1.3.0/TreeOrdination/feature_importance_treeord.py
--rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 treeordination-1.3.0/TreeOrdination/transformers_treeord.py
--rw-r--r--   0        0        0     9119 2020-02-02 00:00:00.000000 treeordination-1.3.0/docs/API.md
--rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 treeordination-1.3.0/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treeordination-1.3.0/notebooks/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treeordination-1.3.0/tests/__init__.py
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 treeordination-1.3.0/tests/test_treeord.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 treeordination-1.3.0/.gitignore
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 treeordination-1.3.0/LICENSE
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 treeordination-1.3.0/README.md
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 treeordination-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 treeordination-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 treeordination-1.3.1/environment.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 treeordination-1.3.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 treeordination-1.3.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 treeordination-1.3.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 treeordination-1.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     8766 2020-02-02 00:00:00.000000 treeordination-1.3.1/TreeOrdination/TreeOrdination.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 treeordination-1.3.1/TreeOrdination/__init__.py
+-rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 treeordination-1.3.1/TreeOrdination/feature_importance_treeord.py
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 treeordination-1.3.1/TreeOrdination/transformers_treeord.py
+-rw-r--r--   0        0        0     9119 2020-02-02 00:00:00.000000 treeordination-1.3.1/docs/API.md
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 treeordination-1.3.1/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treeordination-1.3.1/notebooks/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treeordination-1.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 treeordination-1.3.1/tests/test_treeord.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 treeordination-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 treeordination-1.3.1/LICENSE
+-rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 treeordination-1.3.1/README.md
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 treeordination-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5821 2020-02-02 00:00:00.000000 treeordination-1.3.1/PKG-INFO
```

### Comparing `treeordination-1.3.0/.github/ISSUE_TEMPLATE/bug_report.md` & `treeordination-1.3.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.0/.github/ISSUE_TEMPLATE/feature_request.md` & `treeordination-1.3.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.0/.github/workflows/ci.yml` & `treeordination-1.3.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.0/.github/workflows/python-publish.yml` & `treeordination-1.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.0/TreeOrdination/TreeOrdination.py` & `treeordination-1.3.1/TreeOrdination/TreeOrdination.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,28 +27,28 @@
 
     # Transform data
     if exclude_col[0]:
         excl_range = np.asarray(exclude_col[1])
 
         X_transformed = np.delete(X_in, excl_range, axis=1)
 
-        if isinstance(self.transformer, type(None)) == False:
+        if isinstance(transformer, type(None)) == False:
             X_transformed = transformer.transform(X_transformed)
 
         X_no_transform = X_in[:, excl_range]
 
         if X_transformed.ndim == 1:
             X_transformed = [X_transformed]
 
         X_transformed = np.hstack((X_transformed, X_no_transform))
 
     else:
         X_transformed = X_in
 
-        if isinstance(self.transformer, type(None)) == False:
+        if isinstance(transformer, type(None)) == False:
             X_transformed = transformer.transform(X_in)
 
     if X.ndim == 2:
         return X_transformed
 
     else:
         return X_transformed[0]
@@ -165,26 +165,32 @@
             X_transformed = np.delete(X, excl_range, axis=1)
 
             if isinstance(self.transformer, type(None)) == False:
                 self.proj_transformer = clone(self.transformer)
 
                 X_transformed = self.proj_transformer.fit_transform(X_transformed)
 
+            else:
+                self.proj_transformer = None
+
             X_no_transform = X[:, excl_range]
 
             X_transformed = np.hstack((X_transformed, X_no_transform))
 
         else:
             X_transformed = np.copy(X, "C")
 
             if isinstance(self.transformer, type(None)) == False:
                 self.proj_transformer = clone(self.transformer)
 
                 X_transformed = self.proj_transformer.fit_transform(X)
 
+            else:
+                self.proj_transformer = None
+
         self.l_model = clone(self.proxy_model).fit(
             X_transformed, self.PCA_emb
         )
 
         return self
 
     def get_importance(self):
@@ -226,16 +232,16 @@
         # Plot data
         projection = self.emb_transform(X, trf_type)
 
         fig, ax = plt.subplots(figsize=(10, 5))
 
         sns.scatterplot(x=projection[:, ax_1], y=projection[:, ax_2], hue=y, ax=ax)
 
-        pc_ax_1 = self.R_PCA.explained_variance_ratio_[ax_1] * 100
-        pc_ax_2 = self.R_PCA.explained_variance_ratio_[ax_2] * 100
+        pc_ax_1 = self.PCA_trf.explained_variance_ratio_[ax_1] * 100
+        pc_ax_2 = self.PCA_trf.explained_variance_ratio_[ax_2] * 100
 
         ax.set_xlabel("PCA %s (%.3f Percent)" % (str(ax_1 + 1), pc_ax_1))
         ax.set_ylabel("PCA %s (%.3f Percent)" % (str(ax_2 + 1), pc_ax_2))
 
         ax.legend(loc="center left", bbox_to_anchor=(1, 0.5))
 
         return fig, ax
```

### Comparing `treeordination-1.3.0/TreeOrdination/feature_importance_treeord.py` & `treeordination-1.3.1/TreeOrdination/feature_importance_treeord.py`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.0/TreeOrdination/transformers_treeord.py` & `treeordination-1.3.1/TreeOrdination/transformers_treeord.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 
         self.do_clr = do_clr
         self.delta = delta
 
     def fit_transform(self, X, y=None, **kwargs):
 
         if self.do_clr:
-            return clr(multiplicative_replacement(closure(X[rows_to_keep]), delta=self.delta))
+            return clr(multiplicative_replacement(closure(X), delta=self.delta))
 
         else:
             return closure(X)
 
     def transform(self, X, y=None, **kwargs):
 
         if self.do_clr:
-            return clr(multiplicative_replacement(closure(X[rows_to_keep]), delta=self.delta))
+            return clr(multiplicative_replacement(closure(X), delta=self.delta))
 
         else:
             return closure(X)
 
 
 class ResampleRandomizeTransform(BaseEstimator, TransformerMixin):
     def __init__(self, resampler, transformer, exclude_cols):
```

### Comparing `treeordination-1.3.0/docs/API.md` & `treeordination-1.3.1/docs/API.md`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.0/docs/CONTRIBUTING.md` & `treeordination-1.3.1/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.0/tests/test_treeord.py` & `treeordination-1.3.1/tests/test_treeord.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from TreeOrdination import (
     TreeOrdination,
     CLRClosureTransformer,
+    ResampleRandomizeTransform
 )
 
 from sklearn.datasets import make_classification
 from sklearn.preprocessing import StandardScaler
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import balanced_accuracy_score, median_absolute_error
 
@@ -43,21 +44,21 @@
     pd.testing.assert_frame_equal(X_clr, R, check_dtype=False)
 
     # Ensures that CLRTransformer returns the Closure of X
     R = pd.DataFrame(CLRClosureTransformer(do_clr=False).fit_transform(X_non_neg))
     X_closure = pd.DataFrame(closure(X_non_neg))
     pd.testing.assert_frame_equal(X_closure, R, check_dtype=False)
 
-    R = pd.DataFrame(R)
-    pd.testing.assert_frame_equal(X, R, check_dtype=False)
-
-    R_y = pd.Series(R_y)
-    y = pd.Series(y)
-    pd.testing.assert_series_equal(y, R_y, check_dtype=False)
-
+    # Ensure sampler, transformer objected works
+    R_trf = ResampleRandomizeTransform(None, StandardScaler(), [False, -1])
+    R, y_random = R_trf.fit_resample(X, y)
+    
+    assert R.shape[0] == int(X.shape[0] * 2)
+    assert R.shape[1] == X.shape[1]
+    assert y_random.shape[0] == int(X.shape[0] * 2)
 
 # Tests the overall TreeOrdination pipeline
 def test_treeord_basic():
 
     # Create the dataset
     X, y = make_classification(
         n_samples=200,
@@ -76,25 +77,24 @@
     )
 
     # Set up TreeOrdinaton
     model = TreeOrdination(
         feature_names=[i for i in range(0, X.shape[1])],
         transformer=StandardScaler(),
         n_iter_unsup=2,
-        n_jobs=10,
     )
 
     # Identify predictive features
     model.fit(X_train, y_train)
 
-    X_emb_train = model.emb_transform(X_train)
-    X_approx_train = model.approx_emb(X_train)
+    X_emb_train = model.emb_transform(X_train, "PCA")
+    X_approx_train = model.emb_transform(X_train, "approx")
 
-    X_emb_test = model.emb_transform(X_test)
-    X_approx_test = model.approx_emb(X_test)
+    X_emb_test = model.emb_transform(X_test, "PCA")
+    X_approx_test = model.emb_transform(X_test, "approx")
 
     error_train = median_absolute_error(X_emb_train, X_approx_train)
     assert error_train <= 0.75
 
     error_test = median_absolute_error(X_emb_test, X_approx_test)
     assert error_test <= 0.75
```

### Comparing `treeordination-1.3.0/.gitignore` & `treeordination-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.0/LICENSE` & `treeordination-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.0/README.md` & `treeordination-1.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -34,21 +34,21 @@
         
         #Give features a name
         f_names = ["Feature %s" %str(i) for i in range(X.shape[0])]
         
         tree_ord = TreeOrdination(feature_names = f_names).fit(X, y)
 
         #This is the LANDMark embedding of the dataset. This dataset is used to train the supervised model ('supervised_clf' parameter)
-        landmark_embedding = tree_ord.R_final
+        landmark_embedding = tree_ord.LM_emb
         
         #This is the UMAP projection of the LANDMark embedding
-        umap_projection = tree_ord.tree_emb
+        umap_projection = tree_ord.UMAP_emb
         
         #This is the PCA projetion of the UMAP embedding
-        pca_projection = tree_ord.R_PCA_emb      
+        pca_projection = tree_ord.PCA_emb     
 
 ### Notebooks and Other Examples
 Comming Soon.
 When available, examples of how to use `TreeOrdination` will be found [here](notebooks/README.md).
 
 ### Interface
 An overview of the API can be found [here](docs/API.md).
```

### Comparing `treeordination-1.3.0/pyproject.toml` & `treeordination-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "TreeOrdination"
-version = "1.3.0"
+version = "1.3.1"
 authors = [
     {name = "Josip Rudar", email = "rudarj@uoguelph.ca"},
     {name = "G. Brian Golding"},
     {name = "Stefan C. Kremer"},
     {name = "Mehrdad Hajibabaei", email = "mhajibab@uoguelph.ca"}
 ]
 description = "Projection of High-Dimensional Data Using Multivariate Decision Trees and UMAP"
```

### Comparing `treeordination-1.3.0/PKG-INFO` & `treeordination-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TreeOrdination
-Version: 1.3.0
+Version: 1.3.1
 Summary: Projection of High-Dimensional Data Using Multivariate Decision Trees and UMAP
 Project-URL: Homepage, https://github.com/jrudar/TreeOrdination
 Project-URL: Repository, https://github.com/jrudar/TreeOrdination.git
 Project-URL: Bug Tracker, https://github.com/jrudar/TreeOrdination/issues
 Author: G. Brian Golding, Stefan C. Kremer
 Author-email: Josip Rudar <rudarj@uoguelph.ca>, Mehrdad Hajibabaei <mhajibab@uoguelph.ca>
 License: MIT License
@@ -95,21 +95,21 @@
         
         #Give features a name
         f_names = ["Feature %s" %str(i) for i in range(X.shape[0])]
         
         tree_ord = TreeOrdination(feature_names = f_names).fit(X, y)
 
         #This is the LANDMark embedding of the dataset. This dataset is used to train the supervised model ('supervised_clf' parameter)
-        landmark_embedding = tree_ord.R_final
+        landmark_embedding = tree_ord.LM_emb
         
         #This is the UMAP projection of the LANDMark embedding
-        umap_projection = tree_ord.tree_emb
+        umap_projection = tree_ord.UMAP_emb
         
         #This is the PCA projetion of the UMAP embedding
-        pca_projection = tree_ord.R_PCA_emb      
+        pca_projection = tree_ord.PCA_emb     
 
 ### Notebooks and Other Examples
 Comming Soon.
 When available, examples of how to use `TreeOrdination` will be found [here](notebooks/README.md).
 
 ### Interface
 An overview of the API can be found [here](docs/API.md).
```

