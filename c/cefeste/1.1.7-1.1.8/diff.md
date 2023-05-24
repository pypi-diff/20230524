# Comparing `tmp/cefeste-1.1.7.tar.gz` & `tmp/cefeste-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cefeste-1.1.7.tar", last modified: Mon May 22 21:11:03 2023, max compression
+gzip compressed data, was "cefeste-1.1.8.tar", last modified: Wed May 24 10:07:49 2023, max compression
```

## Comparing `cefeste-1.1.7.tar` & `cefeste-1.1.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 21:11:03.780634 cefeste-1.1.7/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1073 2023-05-05 08:25:33.000000 cefeste-1.1.7/LICENCE
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2821 2023-05-22 21:11:03.780634 cefeste-1.1.7/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2321 2023-05-22 20:53:27.000000 cefeste-1.1.7/README.md
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      754 2023-05-22 21:09:34.000000 cefeste-1.1.7/pyproject.toml
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2023-05-22 21:11:03.780634 cefeste-1.1.7/setup.cfg
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      999 2023-05-22 21:09:36.000000 cefeste-1.1.7/setup.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 21:11:03.760632 cefeste-1.1.7/src/
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 21:11:03.768633 cefeste-1.1.7/src/cefeste/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3364 2023-05-05 08:25:33.000000 cefeste-1.1.7/src/cefeste/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      444 2023-05-05 08:25:33.000000 cefeste-1.1.7/src/cefeste/config.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 21:11:03.776633 cefeste-1.1.7/src/cefeste/elimination/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    15386 2023-05-22 20:53:27.000000 cefeste-1.1.7/src/cefeste/elimination/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    25817 2023-05-10 10:23:33.000000 cefeste-1.1.7/src/cefeste/elimination/shap_rfe.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 21:11:03.776633 cefeste-1.1.7/src/cefeste/selection/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    27726 2023-05-05 08:25:33.000000 cefeste-1.1.7/src/cefeste/selection/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10558 2023-05-05 08:25:33.000000 cefeste-1.1.7/src/cefeste/selection/explanatory.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    21561 2023-05-05 08:25:33.000000 cefeste-1.1.7/src/cefeste/selection/multivariate.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10122 2023-05-05 08:25:33.000000 cefeste-1.1.7/src/cefeste/selection/univariate.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 21:11:03.776633 cefeste-1.1.7/src/cefeste/transform/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2801 2023-05-22 21:09:54.000000 cefeste-1.1.7/src/cefeste/transform/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2434 2023-05-10 10:23:33.000000 cefeste-1.1.7/src/cefeste/utils.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 21:11:03.772633 cefeste-1.1.7/src/cefeste.egg-info/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2821 2023-05-22 21:11:03.000000 cefeste-1.1.7/src/cefeste.egg-info/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      533 2023-05-22 21:11:03.000000 cefeste-1.1.7/src/cefeste.egg-info/SOURCES.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2023-05-22 21:11:03.000000 cefeste-1.1.7/src/cefeste.egg-info/dependency_links.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      131 2023-05-22 21:11:03.000000 cefeste-1.1.7/src/cefeste.egg-info/requires.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        8 2023-05-22 21:11:03.000000 cefeste-1.1.7/src/cefeste.egg-info/top_level.txt
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-24 10:07:49.203394 cefeste-1.1.8/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1073 2023-05-05 08:25:33.000000 cefeste-1.1.8/LICENCE
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2683 2023-05-24 10:07:49.203394 cefeste-1.1.8/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2321 2023-05-22 20:53:27.000000 cefeste-1.1.8/README.md
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      758 2023-05-24 10:06:35.000000 cefeste-1.1.8/pyproject.toml
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2023-05-24 10:07:49.203394 cefeste-1.1.8/setup.cfg
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1001 2023-05-24 10:06:45.000000 cefeste-1.1.8/setup.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-24 10:07:49.187393 cefeste-1.1.8/src/
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-24 10:07:49.195394 cefeste-1.1.8/src/cefeste/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3364 2023-05-05 08:25:33.000000 cefeste-1.1.8/src/cefeste/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      444 2023-05-05 08:25:33.000000 cefeste-1.1.8/src/cefeste/config.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-24 10:07:49.199394 cefeste-1.1.8/src/cefeste/elimination/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    15613 2023-05-24 10:03:32.000000 cefeste-1.1.8/src/cefeste/elimination/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    27438 2023-05-24 10:05:17.000000 cefeste-1.1.8/src/cefeste/elimination/shap_rfe.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-24 10:07:49.203394 cefeste-1.1.8/src/cefeste/selection/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    27726 2023-05-05 08:25:33.000000 cefeste-1.1.8/src/cefeste/selection/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10558 2023-05-05 08:25:33.000000 cefeste-1.1.8/src/cefeste/selection/explanatory.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    21561 2023-05-05 08:25:33.000000 cefeste-1.1.8/src/cefeste/selection/multivariate.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10122 2023-05-05 08:25:33.000000 cefeste-1.1.8/src/cefeste/selection/univariate.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-24 10:07:49.203394 cefeste-1.1.8/src/cefeste/transform/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2801 2023-05-24 08:21:06.000000 cefeste-1.1.8/src/cefeste/transform/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2434 2023-05-10 10:23:33.000000 cefeste-1.1.8/src/cefeste/utils.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-24 10:07:49.199394 cefeste-1.1.8/src/cefeste.egg-info/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2683 2023-05-24 10:07:49.000000 cefeste-1.1.8/src/cefeste.egg-info/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      533 2023-05-24 10:07:49.000000 cefeste-1.1.8/src/cefeste.egg-info/SOURCES.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2023-05-24 10:07:49.000000 cefeste-1.1.8/src/cefeste.egg-info/dependency_links.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      131 2023-05-24 10:07:49.000000 cefeste-1.1.8/src/cefeste.egg-info/requires.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        8 2023-05-24 10:07:49.000000 cefeste-1.1.8/src/cefeste.egg-info/top_level.txt
```

### Comparing `cefeste-1.1.7/LICENCE` & `cefeste-1.1.8/LICENCE`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.7/PKG-INFO` & `cefeste-1.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: cefeste
-Version: 1.1.7
+Version: 1.1.8
 Summary: Feature Selection and Elimination
-Home-page: https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Author: DAT/Mattia Centurelli
 Author-email: DAT - Mattia Centurelli <mcenturelli@credem.it>
-Project-URL: Homepage, https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `cefeste-1.1.7/README.md` & `cefeste-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.7/pyproject.toml` & `cefeste-1.1.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cefeste"
-version = "1.1.7"
+version = "1.1.8"
 authors = [
   { name="DAT - Mattia Centurelli", email="mcenturelli@credem.it" },
 ]
 description = "Feature Selection and Elimination"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -23,9 +23,9 @@
     "scikit-learn==1.1.1",
     "scipy==1.8.1",
     "statsmodels==0.13.2",
     "PyYAML==6.0",
     "shap==0.38.1",
     "ipython",
 ]
-[project.urls]
-"Homepage" = "https://dev.azure.com/credem-data/DAT/_git/ce-feste"
+# [project.urls]
+# "Homepage" = "https://dev.azure.com/credem-data/DAT/_git/ce-feste"
```

### Comparing `cefeste-1.1.7/setup.py` & `cefeste-1.1.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ce-feste",
-    version="1.1.7",
+    version="1.1.8",
     description="Package for Feature Selection, Transformation, Elimination",
     author="DAT/Mattia Centurelli",
     author_email="mcenturelli@credem.it",
-    url="https://dev.azure.com/credem-data/DAT/_git/ce-feste",
+    # url="https://dev.azure.com/credem-data/DAT/_git/ce-feste",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3 :: Only",
     ],
```

### Comparing `cefeste-1.1.7/src/cefeste/__init__.py` & `cefeste-1.1.8/src/cefeste/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.7/src/cefeste/elimination/__init__.py` & `cefeste-1.1.8/src/cefeste/elimination/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,22 +24,23 @@
         cv_funct=RandomizedSearchCV,
         cv_scoring="auto",
         n_iter=20,
         manage_groups=False,
         groups=None,
         cv_type=StratifiedKFold(5, random_state=42, shuffle=True),
         use_ohe=False,
+        dim_cat_threshold=10,
+        use_shap=True,
         # Reporting
         step_size=0.1,
         min_n_feat_step=5,
         final_n_feature=1,
         verbose=True,
         write_final=False,
         write_substep=False,
-        dim_cat_threshold=10,
     ):
         """Feature Elimination Class.
 
         Args:
             db (pd.DataFrame): DataFrame to analyze.
             target_col (str): Name of the target column.
             model : classifier or regressor in sklearn API class.
@@ -53,23 +54,25 @@
             cv_scoring: scoring argument of the cv_functs. Defaults to "auto" selects "roc_auc" fo classification, "r2" for regression
                 and "balanced accuracy" for multiclass.
             n_iter (int, optional): number of iteration, i.e. set of hyperparams tested in Cross Validation. Defaults to 20.
             manage_groups (bool, optional): determines if there is a feature whose groups have to be kept joined in CV. Defaults to False.
             groups (pd.Series, optional): feature whose groups have to be kept joined in CV. Defaults to None.
             cv_type : function or class for defining the CV sets. Defaults to StratifiedKFold(5, random_state=42, shuffle=True).
             use_ohe (bool, optional): determines whether to use One Hot Encoding on categorical features or not. Defaults to False.
+            dim_cat_threshold (int, optional): cardinality threshold for categorical variables to apply or not 'simplified' OHE.
+                Defaults to 10.
+            use_shap (bool, optional): If True it uses shap feature importance. Otherwise it uses the default attribute of the model.
             step_size (int or float, optional): determines how many features to remove at each step.
                 Fixed int or percentage of total features. Defaults to 0.1.
             min_n_feat_step (int, optional): min number of feature to remove at each step. Defaults to 5.
             final_n_feature (int, optional): number of features of the last model. Defaults to 1.
             verbose (bool, optional): If True print a log of information. Defaults to True.
             write_final (bool, optional): If True it saves in the current directory the final report that can be used for quick start. Defaults to False.
             write_substep (bool, optional): If True it saves in the current directory the report after SHAP_RFE that can be used for quick start. Defaults to False.
-            dim_cat_threshold (int, optional): cardinality threshold for categorical variables to apply or not 'simplified' OHE.
-                Defaults to 10.
+
 
         """
         super().__init__(db, feat_to_check)
         self.feat_to_check = list(set(self.feat_to_check) - set([target_col, sample_col]))
         # Target check
         if (target_col in db.columns) | (target_col is None):
             self.target_col = target_col
@@ -123,14 +126,15 @@
         self.cv_funct = cv_funct
         self.cv_scoring = cv_scoring
         self.n_iter = n_iter
         self.manage_groups = manage_groups
         self.groups = groups
         self.cv_type = cv_type
         self.use_ohe = use_ohe
+        self.use_shap = use_shap
         self.step_size = step_size
         self.min_n_feat_step = min_n_feat_step
         self.final_n_feature = final_n_feature
         self.verbose = verbose
         self.write_final = write_final
         self.write_substep = write_substep
         self.dim_cat_threshold = dim_cat_threshold
@@ -206,14 +210,15 @@
             final_n_feature=self.final_n_feature,
             verbose=self.verbose,
             write_final=self.write_final,
             write_substep=self.write_substep,
             use_ohe=self.use_ohe,
             categorical_features_list_ohe=self.categorical_features_list_ohe,
             dim_cat_threshold=self.dim_cat_threshold,
+            use_shap=self.use_shap,
         )
 
         self.report = shap_report
 
         return self.report
 
     def plot_report(self):
```

### Comparing `cefeste-1.1.7/src/cefeste/elimination/shap_rfe.py` & `cefeste-1.1.8/src/cefeste/elimination/shap_rfe.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pandas as pd
 import numpy as np
 import shap
 from sklearn.metrics import roc_auc_score, r2_score, balanced_accuracy_score
 from sklearn.model_selection import RandomizedSearchCV, StratifiedKFold, GroupKFold
-from sklearn.preprocessing import OneHotEncoder, OrdinalEncoder
+from sklearn.preprocessing import OneHotEncoder
 from sklearn.compose import ColumnTransformer
 import re
-from cefeste.utils import remove_features, time_step, get_categorical_features
+from cefeste.utils import remove_features, time_step
 from functools import reduce
 import warnings
 
 
 @time_step
 def Shap_RFE_full(
     X_train,
@@ -29,14 +29,15 @@
     final_n_feature=1,
     verbose=True,
     write_final=False,
     write_substep=False,
     use_ohe=True,
     categorical_features_list_ohe=None,
     dim_cat_threshold=10,
+    use_shap=True,
 ):
     """Recursive Feature Elimination Process with Hyperparameters grid search.
 
     Args:
         X_train (pd.DataFrame): Feature dataset.
         y_train (pd.Series): target set.
         model: classifier or regressor in sklearn API class.
@@ -55,34 +56,35 @@
         verbose (bool, optional): If True print a log of information. Defaults to True.
         write_final (bool, optional): If True it saves in the current directory the final report that can be used for quick start. Defaults to False.
         write_substep (bool, optional): If True it saves in the current directory the report after SHAP_RFE that can be used for quick start. Defaults to False.
         use_ohe (bool, optional): determines whether to use One Hot Encoding on categorical features or not. Defaults to True.
         categorical_features_list_ohe (list, optional): list of categorical features for One Hot Encoding. Defaults to None.
         dim_cat_threshold (int, optional): cardinality threshold for categorical variables to apply or not 'simplified' OHE.
             Defaults to 10.
+        use_shap (bool, optional): If True it uses shap feature importance. Otherwise it uses the default attribute of the model.
 
     Return:
     pd.DataFrame: Report of the detail and result of each step of FE and Grid Search.
     """
     if groups is None:
         groups = pd.Series()
-        
+
     if algo_type not in ["classification", "regression", "multiclass"]:
-        raise ValueError("algo_type argument must be one of ['classification', 'regression', 'multiclass']")  
-        
+        raise ValueError("algo_type argument must be one of ['classification', 'regression', 'multiclass']")
+
     if (algo_type == "regression") and (str(cv_type.__class__()).startswith("StratifiedKFold")):
-            raise ValueError("Fold Cross Validation uncorrect for regression algorithm, use KFold() or GroupKFold()")
-            
+        raise ValueError("Fold Cross Validation uncorrect for regression algorithm, use KFold() or GroupKFold()")
+
     if cv_scoring == "auto":
         if algo_type == "classification":
-            cv_scoring="roc_auc"
+            cv_scoring = "roc_auc"
         elif algo_type == "regression":
-            cv_scoring="r2"
+            cv_scoring = "r2"
         elif algo_type == "multiclass":
-            cv_scoring="balanced_accuracy"
+            cv_scoring = "balanced_accuracy"
 
     # Define the algo
     try:
         CVSel_algo = cv_funct(model, grid, n_iter=n_iter, cv=cv_type, scoring=cv_scoring)
     except Exception:
         CVSel_algo = cv_funct(model, grid, cv=cv_type, scoring=cv_scoring)  # for GridSearchCV
 
@@ -110,28 +112,29 @@
         final_n_feature=final_n_feature,
         verbose=verbose,
         write=write_substep,
         use_ohe=use_ohe,
         categorical_features_list_ohe=categorical_features_list_ohe,
         number_splits=number_splits,
         dim_cat_threshold=dim_cat_threshold,
+        use_shap=use_shap,
     )
     # Train the final model
     X_train = X_train[report["feat_select"].iloc[-1]]
     initial_feat_n = X_train.shape[1]
     if manage_groups:
         CVSel_algo.cv = GroupKFold(number_splits).split(X_train, y_train, groups)
     X_train_tsf = X_train.copy()
     if use_ohe:
-        cats_feat = list(set(categorical_features_list_ohe) & set(X_train.columns))   
+        cats_feat = list(set(categorical_features_list_ohe) & set(X_train.columns))
         for col in cats_feat:
             if X_train_tsf[col].nunique() > dim_cat_threshold:
-                values_cat = list(
-                    X_train_tsf.groupby(col, sort=False)[col].count().sort_values(ascending=False).index
-                )[:dim_cat_threshold]
+                values_cat = list(X_train_tsf.groupby(col, sort=False)[col].count().sort_values(ascending=False).index)[
+                    :dim_cat_threshold
+                ]
                 for val in values_cat:
                     X_train_tsf[col + "_" + str(val)] = (X_train_tsf[col] == val).astype("int")
                 X_train_tsf = X_train_tsf.drop(columns=col)
                 cats_feat.remove(col)
         preprocessor = ColumnTransformer(
             transformers=[
                 ("cat", OneHotEncoder(handle_unknown="ignore", sparse=False), cats_feat),
@@ -139,15 +142,17 @@
             remainder="passthrough",
         )
         preprocessor.fit(X_train_tsf)
         feat_names = preprocessor.get_feature_names_out()
         feat_names = [re.sub(r"((remainder)|(cat))__", "", x) for x in feat_names]
         X_train_tsf = pd.DataFrame(preprocessor.transform(X_train_tsf), columns=feat_names)
     else:
-        X_train_tsf[X_train_tsf.select_dtypes(['object']).columns] = X_train_tsf.select_dtypes(['object']).apply(lambda x: x.astype('category'))
+        X_train_tsf[X_train_tsf.select_dtypes(["object"]).columns] = X_train_tsf.select_dtypes(["object"]).apply(
+            lambda x: x.astype("category")
+        )
     CVSel_algo.fit(X_train_tsf, y_train)
 
     model = CVSel_algo.best_estimator_
     # Get measure
     if algo_type == "classification":
         train_model_score = roc_auc_score(y_train, CVSel_algo.predict_proba(X_train_tsf)[:, 1])
     elif algo_type == "regression":
@@ -189,14 +194,15 @@
     write=True,
     use_ohe=False,
     categorical_features_list_ohe=None,
     manage_groups=False,
     groups=None,
     number_splits=5,
     dim_cat_threshold=10,
+    use_shap=True,
 ):
     """Recursive Feature Elimination Process with Hyperparameters grid search.
 
     Args:
         X_train (pd.DataFrame): Feature dataset.
         y_train (pd.Series): target set.
         CVSel_algo: class that include the classifier/regresor, grid search and detail of CV selection.
@@ -210,53 +216,63 @@
         use_ohe (bool, optional): determines whether to use One Hot Encoding on categorical features or not. Defaults to False.
         categorical_features_list_ohe (list, optional): list of categorical features for One Hot Encoding. Defaults to None.
         manage_groups (bool, optional): determines if there is a feature whose groups have to be kept joined in CV. Defaults to False.
         groups (pd.Series, optional): feature whose groups have to be kept joined in CV. Defaults to None.
         number_splits (int, optional): number of splits in CV for GroupFold. Defaults to 5.
         dim_cat_threshold (int, optional): cardinality threshold for categorical variables to apply or not 'simplified' OHE.
             Defaults to 10.
+        use_shap (bool, optional): If True it uses shap feature importance. Otherwise it uses the default attribute of the model.
 
 
     Return:
     pd.DataFrame: Report of the detail and result of each step of FE and Grid Search.
     """
     initial_feat_n = X_train.shape[1]
     if use_ohe:
         cats_feat = list(set(X_train.columns) & set(categorical_features_list_ohe))
 
         if algo_type == "classification":
             shap_importance, model, train_model_score, valid_model_score = get_Shap_AUC(
-                X_train, y_train, CVSel_algo, categorical_feature=cats_feat, dim_cat_threshold=dim_cat_threshold
+                X_train,
+                y_train,
+                CVSel_algo,
+                categorical_feature=cats_feat,
+                dim_cat_threshold=dim_cat_threshold,
+                use_shap=use_shap,
             )
         elif algo_type == "regression":
             shap_importance, model, train_model_score, valid_model_score = get_Shap_R2(
-                X_train, y_train, CVSel_algo, categorical_feature=cats_feat, dim_cat_threshold=dim_cat_threshold
+                X_train,
+                y_train,
+                CVSel_algo,
+                categorical_feature=cats_feat,
+                dim_cat_threshold=dim_cat_threshold,
+                use_shap=use_shap,
             )
         elif algo_type == "multiclass":
             shap_importance, model, train_model_score, valid_model_score = get_Shap_BalAcc(
-                X_train, y_train, CVSel_algo, categorical_feature=cats_feat, dim_cat_threshold=dim_cat_threshold
+                X_train,
+                y_train,
+                CVSel_algo,
+                categorical_feature=cats_feat,
+                dim_cat_threshold=dim_cat_threshold,
+                use_shap=use_shap,
             )
     else:
         if algo_type == "classification":
             shap_importance, model, train_model_score, valid_model_score = get_Shap_AUC(
-                X_train,
-                y_train,
-                CVSel_algo,
+                X_train, y_train, CVSel_algo, use_shap=use_shap
             )
         elif algo_type == "regression":
             shap_importance, model, train_model_score, valid_model_score = get_Shap_R2(
-                X_train,
-                y_train,
-                CVSel_algo,
+                X_train, y_train, CVSel_algo, use_shap=use_shap
             )
         elif algo_type == "multiclass":
             shap_importance, model, train_model_score, valid_model_score = get_Shap_BalAcc(
-                X_train,
-                y_train,
-                CVSel_algo,
+                X_train, y_train, CVSel_algo, use_shap=use_shap
             )
 
     X_train, feat_to_remove = get_new_X(X_train, shap_importance, step_size, min_n_feat_step, final_n_feature)
     report = pd.DataFrame(
         {
             "n_feat": [initial_feat_n],
             "train_score": [train_model_score],
@@ -287,55 +303,66 @@
             write,
             use_ohe,
             categorical_features_list_ohe,
             manage_groups,
             groups,
             number_splits=number_splits,
             dim_cat_threshold=dim_cat_threshold,
+            use_shap=use_shap,
         )
         report = pd.concat([report, report_step])
 
     if write:
         report.to_csv(f"rsfe_report_until{X_train.shape[1]}", index=False)
 
     return report
 
 
-def get_Shap(X_train, model, categorical_shap_ohe=False, categorical_feature=None, y_train=None):
+def get_Shap(X_train, model, categorical_shap_ohe=False, categorical_feature=None, y_train=None, use_shap=True):
     """Get Features' Shapley Value.
 
     Args:
         X_train (pd.DataFrame): Feature dataset.
         model: the fitted best estimator of the CV Selection.
         categorical_shap_ohe (bool, optional): determines if there are columns coming from OHE. Defaults to False.
         categorical_feature (list, optional): list of categorical features before OHE. Defaults to [].
         y_train (pd.Series, optional): target set. Defaults to None.
+        use_shap (bool, optional): If True it uses shap feature importance. Otherwise it uses the default attribute of the model.
     Returns:
         pd.DataFrame: Shap DataFrame.
     """
     if categorical_feature is None:
         categorical_feature = []
 
     # Get Shap
     feature_names = X_train.columns
+    tree_explainer = True
     using_features_importance = False
-    try:
-        shap_values = shap.TreeExplainer(model).shap_values(X_train)
-    except Exception:
+
+    if use_shap:
         try:
-            # For Support Vector Machine and other no-Tree Algorithms
-            n_clusters = max(10, min(1000, int(X_train.shape[0] / 100)))
-            model.fit(X_train.values, y_train.values)
-            shap_values = shap.KernelExplainer(model.predict, shap.kmeans(X_train, n_clusters)).shap_values(X_train)
+            shap_values = shap.TreeExplainer(model).shap_values(X_train)
         except Exception:
-            warnings.warn('shap inconsistent with this numpy version. Using feature_importance_ attribute')
-            # For computing features importance due to numpy version issues
-            feature_importances = model.feature_importances_
-            using_features_importance = True
-    
+            tree_explainer = False
+
+        if not tree_explainer:
+            try:
+                # For Support Vector Machine and other no-Tree Algorithms
+                n_clusters = max(10, min(1000, int(X_train.shape[0] / 100)))
+                model.fit(X_train.values, y_train.values)
+                shap_values = shap.KernelExplainer(model.predict, shap.kmeans(X_train, n_clusters)).shap_values(X_train)
+            except Exception:
+                warnings.warn("shap inconsistent with this numpy version. Using feature_importance_ attribute")
+                # For computing features importance due to numpy version issues
+                feature_importances = model.feature_importances_
+                using_features_importance = True
+    else:
+        using_features_importance = True
+        feature_importances = model.feature_importances_
+
     if using_features_importance:
         shap_importance = pd.DataFrame({"feature": feature_names, "shap_importance": feature_importances})
     else:
         # For (multi) classification
         if isinstance(shap_values, list):
             db_list = list()
             for i in range(len(shap_values)):
@@ -349,15 +376,17 @@
                 .set_index("feature")
                 .assign(shap_importance=lambda x: x.sum(axis=1))
                 .loc[:, "shap_importance"]
                 .reset_index()
             )
         # For regression and (some - depending on the classifier) binary classification
         elif isinstance(shap_values, np.ndarray):
-            shap_importance = pd.DataFrame({"feature": feature_names, "shap_importance": np.abs(shap_values).mean(axis=0)})
+            shap_importance = pd.DataFrame(
+                {"feature": feature_names, "shap_importance": np.abs(shap_values).mean(axis=0)}
+            )
 
     # For categorical features one-hot-encoded sum the shap values referring the same pivot feature
     if categorical_shap_ohe:
         for i in categorical_feature:
             shap_importance.loc[shap_importance.feature.str.startswith(i)] = shap_importance.loc[
                 shap_importance.feature.str.startswith(i)
             ].assign(
@@ -365,41 +394,42 @@
                 shap_importance=shap_importance.loc[shap_importance.feature.str.startswith(i), "shap_importance"].sum(),
             )
         shap_importance = shap_importance.drop_duplicates().dropna().reset_index(drop=True)
     shap_importance.sort_values(by=["shap_importance"], ascending=True, inplace=True)
     return shap_importance
 
 
-def get_Shap_AUC(X_train, y_train, CVSel_algo, categorical_feature=None, dim_cat_threshold=10):
+def get_Shap_AUC(X_train, y_train, CVSel_algo, categorical_feature=None, dim_cat_threshold=10, use_shap=True):
     """Get the AUC of the model and Features' Shapley Value.
 
-    Args:
-        X_train (pd.DataFrame): Feature dataset.
-        y_train (pd.Series): target set.
-        CVSel_algo: class that include the classifier, grid search and detail of CV selection.
-        categorical_feature (list, optional): list of categorical feature to be preprocessed. Defaults to None.
-        dim_cat_threshold (int, optional): cardinality threshold for categorical variables to apply or not 'simplified' OHE.
-            Defaults to 10.
+     Args:
+         X_train (pd.DataFrame): Feature dataset.
+         y_train (pd.Series): target set.
+         CVSel_algo: class that include the classifier, grid search and detail of CV selection.
+         categorical_feature (list, optional): list of categorical feature to be preprocessed. Defaults to None.
+         dim_cat_threshold (int, optional): cardinality threshold for categorical variables to apply or not 'simplified' OHE.
+             Defaults to 10.
+          use_shap (bool, optional): If True it uses shap feature importance. Otherwise it uses the default attribute of the model.
     Returns:
-        (pd.DataFrame, classifier, float, float): Shap DataFrame, Best Classifier, Train and Valid AUC.
+         (pd.DataFrame, classifier, float, float): Shap DataFrame, Best Classifier, Train and Valid AUC.
     """
     if categorical_feature is None:
         categorical_feature = []
 
     # Estimate
     categorical_shap_ohe = False
     X_train_tsf = X_train.copy()
     if len(categorical_feature) > 0:
         # Categorical Preprocessing Hot-One-Encoder
         cats_feat = categorical_feature.copy()
         for col in cats_feat:
             if X_train_tsf[col].nunique() > dim_cat_threshold:
-                values_cat = list(
-                    X_train_tsf.groupby(col, sort=False)[col].count().sort_values(ascending=False).index
-                )[:dim_cat_threshold]
+                values_cat = list(X_train_tsf.groupby(col, sort=False)[col].count().sort_values(ascending=False).index)[
+                    :dim_cat_threshold
+                ]
                 for val in values_cat:
                     X_train_tsf[col + "_" + str(val)] = (X_train_tsf[col] == val).astype("int")
                 X_train_tsf = X_train_tsf.drop(columns=col)
                 cats_feat.remove(col)
         preprocessor = ColumnTransformer(
             transformers=[
                 ("cat", OneHotEncoder(handle_unknown="ignore", sparse=False), cats_feat),
@@ -409,58 +439,63 @@
         preprocessor.fit(X_train_tsf)
         feat_names = preprocessor.get_feature_names_out()
         feat_names = [re.sub(r"((remainder)|(cat))__", "", x) for x in feat_names]
         X_train_tsf = pd.DataFrame(preprocessor.transform(X_train_tsf), columns=feat_names)
         categorical_shap_ohe = True
 
     else:
-        X_train_tsf[X_train_tsf.select_dtypes(['object']).columns] = X_train_tsf.select_dtypes(['object']).apply(lambda x: x.astype('category'))
-    
+        X_train_tsf[X_train_tsf.select_dtypes(["object"]).columns] = X_train_tsf.select_dtypes(["object"]).apply(
+            lambda x: x.astype("category")
+        )
+
     CVSel_algo.fit(X_train_tsf, y_train)
 
     model = CVSel_algo.best_estimator_
 
     # Get AUC
     train_model_score = roc_auc_score(y_train, CVSel_algo.predict_proba(X_train_tsf)[:, 1])
     valid_model_score = CVSel_algo.best_score_
 
     # Get Shap
-    shap_importance = get_Shap(X_train_tsf, model, categorical_shap_ohe, categorical_feature, y_train=y_train)
+    shap_importance = get_Shap(
+        X_train_tsf, model, categorical_shap_ohe, categorical_feature, y_train=y_train, use_shap=use_shap
+    )
 
     return shap_importance, model, train_model_score, valid_model_score
 
 
-def get_Shap_R2(X_train, y_train, CVSel_algo, categorical_feature=None, dim_cat_threshold=10):
+def get_Shap_R2(X_train, y_train, CVSel_algo, categorical_feature=None, dim_cat_threshold=10, use_shap=True):
     """Get the R squared of the model and Features' Shapley Value.
 
-    Args:
-        X_train (pd.DataFrame): Feature dataset.
-        y_train (pd.Series): target set.
-        CVSel_algo: class that include the regressor, grid search and detail of CV selection.
-        categorical_feature (list, optional): list of categorical feature to be preprocessed. Defaults to None.
-        dim_cat_threshold (int, optional): cardinality threshold for categorical variables to apply or not 'simplified' OHE.
-            Defaults to 10.
+     Args:
+         X_train (pd.DataFrame): Feature dataset.
+         y_train (pd.Series): target set.
+         CVSel_algo: class that include the regressor, grid search and detail of CV selection.
+         categorical_feature (list, optional): list of categorical feature to be preprocessed. Defaults to None.
+         dim_cat_threshold (int, optional): cardinality threshold for categorical variables to apply or not 'simplified' OHE.
+             Defaults to 10.
+          use_shap (bool, optional): If True it uses shap feature importance. Otherwise it uses the default attribute of the model.
     Returns:
-        (pd.DataFrame, classifier, float, float): Shap DataFrame, Best Classifier, Train and Valid R2.
+         (pd.DataFrame, classifier, float, float): Shap DataFrame, Best Classifier, Train and Valid R2.
 
     """
     if categorical_feature is None:
         categorical_feature = []
 
     # Estimate
     categorical_shap_ohe = False
     X_train_tsf = X_train.copy()
     if len(categorical_feature) > 0:
         # Categorical Preprocessing Hot-One-Encoder
         cats_feat = categorical_feature.copy()
         for col in cats_feat:
             if X_train_tsf[col].nunique() > dim_cat_threshold:
-                values_cat = list(
-                    X_train_tsf.groupby(col, sort=False)[col].count().sort_values(ascending=False).index
-                )[:dim_cat_threshold]
+                values_cat = list(X_train_tsf.groupby(col, sort=False)[col].count().sort_values(ascending=False).index)[
+                    :dim_cat_threshold
+                ]
                 for val in values_cat:
                     X_train_tsf[col + "_" + str(val)] = (X_train_tsf[col] == val).astype("int")
                 X_train_tsf = X_train_tsf.drop(columns=col)
                 cats_feat.remove(col)
         preprocessor = ColumnTransformer(
             transformers=[
                 ("cat", OneHotEncoder(handle_unknown="ignore", sparse=False), cats_feat),
@@ -470,40 +505,45 @@
         preprocessor.fit(X_train_tsf)
         feat_names = preprocessor.get_feature_names_out()
         feat_names = [re.sub(r"((remainder)|(cat))__", "", x) for x in feat_names]
         X_train_tsf = pd.DataFrame(preprocessor.transform(X_train_tsf), columns=feat_names)
         categorical_shap_ohe = True
 
     else:
-        X_train_tsf[X_train_tsf.select_dtypes(['object']).columns] = X_train_tsf.select_dtypes(['object']).apply(lambda x: x.astype('category'))
+        X_train_tsf[X_train_tsf.select_dtypes(["object"]).columns] = X_train_tsf.select_dtypes(["object"]).apply(
+            lambda x: x.astype("category")
+        )
 
     CVSel_algo.fit(X_train_tsf, y_train)
 
     model = CVSel_algo.best_estimator_
 
     # Get R2
     train_model_score = r2_score(y_train, CVSel_algo.predict(X_train_tsf))
     valid_model_score = CVSel_algo.best_score_
 
     # Get Shap
-    shap_importance = get_Shap(X_train_tsf, model, categorical_shap_ohe, categorical_feature, y_train=y_train)
+    shap_importance = get_Shap(
+        X_train_tsf, model, categorical_shap_ohe, categorical_feature, y_train=y_train, use_shap=use_shap
+    )
 
     return shap_importance, model, train_model_score, valid_model_score
 
 
-def get_Shap_BalAcc(X_train, y_train, CVSel_algo, categorical_feature=None, dim_cat_threshold=10):
+def get_Shap_BalAcc(X_train, y_train, CVSel_algo, categorical_feature=None, dim_cat_threshold=10, use_shap=True):
     """Get the Balanced Accuracy of the model and Features' Shapley Value.
 
     Args:
         X_train (pd.DataFrame): Feature dataset.
         y_train (pd.Series): target set.
         CVSel_algo: class that include the regressor, grid search and detail of CV selection.
         categorical_feature (list, optional): list of categorical feature to be preprocessed. Defaults to [].
         dim_cat_threshold (int, optional): cardinality threshold for categorical variables to apply or not 'simplified' OHE.
             Defaults to 10.
+        use_shap (bool, optional): If True it uses shap feature importance. Otherwise it uses the default attribute of the model.
     Returns:
         (pd.DataFrame, classifier, float, float): Shap DataFrame, Best Classifier, Train and Valid Balanced accuracy.
 
     """
     if categorical_feature is None:
         categorical_feature = []
 
@@ -511,17 +551,17 @@
     categorical_shap_ohe = False
     X_train_tsf = X_train.copy()
     if len(categorical_feature) > 0:
         # Categorical Preprocessing Hot-One-Encoder
         cats_feat = categorical_feature.copy()
         for col in cats_feat:
             if X_train_tsf[col].nunique() > dim_cat_threshold:
-                values_cat = list(
-                    X_train_tsf.groupby(col, sort=False)[col].count().sort_values(ascending=False).index
-                )[:dim_cat_threshold]
+                values_cat = list(X_train_tsf.groupby(col, sort=False)[col].count().sort_values(ascending=False).index)[
+                    :dim_cat_threshold
+                ]
                 for val in values_cat:
                     X_train_tsf[col + "_" + str(val)] = (X_train_tsf[col] == val).astype("int")
                 X_train_tsf = X_train_tsf.drop(columns=col)
                 cats_feat.remove(col)
         preprocessor = ColumnTransformer(
             transformers=[
                 ("cat", OneHotEncoder(handle_unknown="ignore", sparse=False), cats_feat),
@@ -531,25 +571,29 @@
         preprocessor.fit(X_train_tsf)
         feat_names = preprocessor.get_feature_names_out()
         feat_names = [re.sub(r"((remainder)|(cat))__", "", x) for x in feat_names]
         X_train_tsf = pd.DataFrame(preprocessor.transform(X_train_tsf), columns=feat_names)
         categorical_shap_ohe = True
 
     else:
-        X_train_tsf[X_train_tsf.select_dtypes(['object']).columns] = X_train_tsf.select_dtypes(['object']).apply(lambda x: x.astype('category'))
+        X_train_tsf[X_train_tsf.select_dtypes(["object"]).columns] = X_train_tsf.select_dtypes(["object"]).apply(
+            lambda x: x.astype("category")
+        )
 
     CVSel_algo.fit(X_train_tsf, y_train)
 
     model = CVSel_algo.best_estimator_
     # Get Balanced Accuracy
     train_model_score = balanced_accuracy_score(y_train, CVSel_algo.predict(X_train_tsf))
     valid_model_score = CVSel_algo.best_score_
 
     # Get Shap
-    shap_importance = get_Shap(X_train_tsf, model, categorical_shap_ohe, categorical_feature, y_train=y_train)
+    shap_importance = get_Shap(
+        X_train_tsf, model, categorical_shap_ohe, categorical_feature, y_train=y_train, use_shap=use_shap
+    )
 
     return shap_importance, model, train_model_score, valid_model_score
 
 
 def get_new_X(X_train, shap_importance, step_size=0.1, min_n_feat_step=5, final_n_feature=1):
     """Determines the reduced DataFrame excluding the shap-useless features.
```

### Comparing `cefeste-1.1.7/src/cefeste/selection/__init__.py` & `cefeste-1.1.8/src/cefeste/selection/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.7/src/cefeste/selection/explanatory.py` & `cefeste-1.1.8/src/cefeste/selection/explanatory.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.7/src/cefeste/selection/multivariate.py` & `cefeste-1.1.8/src/cefeste/selection/multivariate.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.7/src/cefeste/selection/univariate.py` & `cefeste-1.1.8/src/cefeste/selection/univariate.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.7/src/cefeste/transform/__init__.py` & `cefeste-1.1.8/src/cefeste/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.7/src/cefeste/utils.py` & `cefeste-1.1.8/src/cefeste/utils.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.7/src/cefeste.egg-info/PKG-INFO` & `cefeste-1.1.8/src/cefeste.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: cefeste
-Version: 1.1.7
+Version: 1.1.8
 Summary: Feature Selection and Elimination
-Home-page: https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Author: DAT/Mattia Centurelli
 Author-email: DAT - Mattia Centurelli <mcenturelli@credem.it>
-Project-URL: Homepage, https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `cefeste-1.1.7/src/cefeste.egg-info/SOURCES.txt` & `cefeste-1.1.8/src/cefeste.egg-info/SOURCES.txt`

 * *Files identical despite different names*

