# Comparing `tmp/aplr-3.1.0-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/aplr-4.0.0-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 297835 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat   328704 b- defN 23-May-06 16:34 aplr_cpp.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   340992 b- defN 23-May-06 16:38 aplr_cpp.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat       19 b- defN 23-May-06 16:30 aplr/__init__.py
--rw-rw-rw-  2.0 fat     6307 b- defN 23-May-06 16:30 aplr/aplr.py
--rw-rw-rw-  2.0 fat     1134 b- defN 23-May-06 16:38 aplr-3.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      626 b- defN 23-May-06 16:38 aplr-3.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-May-06 16:38 aplr-3.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-May-06 16:38 aplr-3.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      690 b- defN 23-May-06 16:38 aplr-3.1.0.dist-info/RECORD
-9 files, 678593 bytes uncompressed, 296663 bytes compressed:  56.3%
+Zip file size: 345459 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat   388608 b- defN 23-May-24 16:13 aplr_cpp.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   410624 b- defN 23-May-24 16:17 aplr_cpp.pypy39-pp73-win_amd64.pyd
+-rw-rw-rw-  2.0 fat       19 b- defN 23-May-24 16:08 aplr/__init__.py
+-rw-rw-rw-  2.0 fat    10794 b- defN 23-May-24 16:08 aplr/aplr.py
+-rw-rw-rw-  2.0 fat     1134 b- defN 23-May-24 16:17 aplr-4.0.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      655 b- defN 23-May-24 16:17 aplr-4.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 23-May-24 16:17 aplr-4.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-May-24 16:17 aplr-4.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      691 b- defN 23-May-24 16:17 aplr-4.0.0.dist-info/RECORD
+9 files, 812646 bytes uncompressed, 344287 bytes compressed:  57.6%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: aplr/__init__.py
 Comment: 
 
 Filename: aplr/aplr.py
 Comment: 
 
-Filename: aplr-3.1.0.dist-info/LICENSE
+Filename: aplr-4.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: aplr-3.1.0.dist-info/METADATA
+Filename: aplr-4.0.0.dist-info/METADATA
 Comment: 
 
-Filename: aplr-3.1.0.dist-info/WHEEL
+Filename: aplr-4.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: aplr-3.1.0.dist-info/top_level.txt
+Filename: aplr-4.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: aplr-3.1.0.dist-info/RECORD
+Filename: aplr-4.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aplr/aplr.py

```diff
@@ -86,16 +86,16 @@
 
     def get_intercept(self)->float:
         return self.APLRRegressor.get_intercept()
 
     def get_intercept_steps(self)->npt.ArrayLike:
         return self.APLRRegressor.get_intercept_steps()
 
-    def get_m(self)->int:
-        return self.APLRRegressor.get_m()
+    def get_optimal_m(self)->int:
+        return self.APLRRegressor.get_optimal_m()
     
     def get_validation_tuning_metric(self)->str:
         return self.APLRRegressor.get_validation_tuning_metric()
  
     def get_validation_indexes(self)->List[int]:
         return self.APLRRegressor.get_validation_indexes()
 
@@ -123,8 +123,98 @@
         }
 
     #For sklearn
     def set_params(self, **parameters):
         for parameter, value in parameters.items():
             setattr(self, parameter, value)
         self.__set_params_cpp()
+        return self
+    
+
+class APLRClassifier():
+    def __init__(self, m:int=9000, v:float=0.1, random_state:int=0, n_jobs:int=0, validation_ratio:float=0.2, bins:int=300, verbosity:int=0, max_interaction_level:int=1, max_interactions:int=100000, min_observations_in_split:int=20, ineligible_boosting_steps_added:int=10, max_eligible_terms:int=5):
+        self.m=m
+        self.v=v
+        self.random_state=random_state
+        self.n_jobs=n_jobs
+        self.validation_ratio=validation_ratio
+        self.bins=bins
+        self.verbosity=verbosity
+        self.max_interaction_level=max_interaction_level
+        self.max_interactions=max_interactions
+        self.min_observations_in_split=min_observations_in_split
+        self.ineligible_boosting_steps_added=ineligible_boosting_steps_added
+        self.max_eligible_terms=max_eligible_terms
+
+        #Creating aplr_cpp and setting parameters
+        self.APLRClassifier=aplr_cpp.APLRClassifier()
+        self.__set_params_cpp()
+
+    #Sets parameters for aplr_cpp.APLRClassifier cpp object
+    def __set_params_cpp(self):
+        self.APLRClassifier.m=self.m
+        self.APLRClassifier.v=self.v
+        self.APLRClassifier.random_state=self.random_state
+        self.APLRClassifier.n_jobs=self.n_jobs
+        self.APLRClassifier.validation_ratio=self.validation_ratio
+        self.APLRClassifier.bins=self.bins
+        self.APLRClassifier.verbosity=self.verbosity
+        self.APLRClassifier.max_interaction_level=self.max_interaction_level
+        self.APLRClassifier.max_interactions=self.max_interactions
+        self.APLRClassifier.min_observations_in_split=self.min_observations_in_split
+        self.APLRClassifier.ineligible_boosting_steps_added=self.ineligible_boosting_steps_added
+        self.APLRClassifier.max_eligible_terms=self.max_eligible_terms
+
+    def fit(self, X:npt.ArrayLike, y:List[str], sample_weight:npt.ArrayLike = np.empty(0), X_names:List[str]=[], validation_set_indexes:List[int]=[], prioritized_predictors_indexes:List[int]=[], monotonic_constraints:List[int]=[], interaction_constraints:List[int]=[]):
+        self.__set_params_cpp()
+        self.APLRClassifier.fit(X,y,sample_weight,X_names,validation_set_indexes,prioritized_predictors_indexes,monotonic_constraints,interaction_constraints)
+
+    def predict_class_probabilities(self, X:npt.ArrayLike, cap_predictions_to_minmax_in_training:bool=False)->npt.ArrayLike:
+        return self.APLRClassifier.predict_class_probabilities(X, cap_predictions_to_minmax_in_training)
+    
+    def predict(self, X:npt.ArrayLike, cap_predictions_to_minmax_in_training:bool=False)->List[str]:
+        return self.APLRClassifier.predict(X, cap_predictions_to_minmax_in_training)
+
+    def calculate_local_feature_importance(self,X:npt.ArrayLike)->npt.ArrayLike:
+        return self.APLRClassifier.calculate_local_feature_importance(X)
+
+    def get_categories(self)->List[str]:
+        return self.APLRClassifier.get_categories()
+
+    def get_logit_model(self,category:str)->APLRRegressor:
+        return self.APLRClassifier.get_logit_model(category)
+
+    def get_validation_indexes(self)->List[int]:
+        return self.APLRClassifier.get_validation_indexes()
+    
+    def get_validation_error_steps(self)->npt.ArrayLike:
+        return self.APLRClassifier.get_validation_error_steps()
+
+    def get_validation_error(self)->float:
+        return self.APLRClassifier.get_validation_error()
+
+    def get_feature_importance(self)->npt.ArrayLike:
+        return self.APLRClassifier.get_feature_importance() 
+
+    #For sklearn
+    def get_params(self, deep=True):
+        return {
+            "m": self.m,
+            "v": self.v,
+            "random_state":self.random_state,
+            "n_jobs":self.n_jobs,
+            "validation_ratio":self.validation_ratio,
+            "bins":self.bins,
+            "verbosity":self.verbosity,
+            "max_interaction_level":self.max_interaction_level,
+            "max_interactions":self.max_interactions,
+            "min_observations_in_split":self.min_observations_in_split,
+            "ineligible_boosting_steps_added":self.ineligible_boosting_steps_added,
+            "max_eligible_terms":self.max_eligible_terms,
+        }
+
+    #For sklearn
+    def set_params(self, **parameters):
+        for parameter, value in parameters.items():
+            setattr(self, parameter, value)
+        self.__set_params_cpp()
         return self
```

## Comparing `aplr-3.1.0.dist-info/LICENSE` & `aplr-4.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aplr-3.1.0.dist-info/METADATA` & `aplr-4.0.0.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: aplr
-Version: 3.1.0
+Version: 4.0.0
 Summary: Automatic Piecewise Linear Regression
 Home-page: https://github.com/ottenbreit-data-science/aplr
 Author: Mathias von Ottenbreit
 Author-email: ottenbreitdatascience@gmail.com
 License: MIT
 Platform: Windows
 Platform: Linux
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy (>=1.20)
 
-Build predictive and interpretable parametric machine learning models in Python based on the Automatic Piecewise Linear Regression methodology developed by Mathias von Ottenbreit.
+Build predictive and interpretable parametric regression or classification machine learning models in Python based on the Automatic Piecewise Linear Regression methodology developed by Mathias von Ottenbreit.
```

