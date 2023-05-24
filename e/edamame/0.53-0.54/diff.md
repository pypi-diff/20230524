# Comparing `tmp/edamame-0.53.tar.gz` & `tmp/edamame-0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edamame-0.53.tar", last modified: Mon May 22 22:03:42 2023, max compression
+gzip compressed data, was "edamame-0.54.tar", last modified: Wed May 24 21:35:58 2023, max compression
```

## Comparing `edamame-0.53.tar` & `edamame-0.54.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-22 22:03:42.168505 edamame-0.53/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 edamame-0.53/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11959 2023-05-22 22:03:42.168115 edamame-0.53/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10205 2023-05-22 22:01:40.000000 edamame-0.53/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-22 22:03:42.158633 edamame-0.53/edamame/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       21 2023-05-22 22:01:51.000000 edamame-0.53/edamame/__init__.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-22 22:03:42.162581 edamame-0.53/edamame/classifier/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      194 2023-05-04 19:56:56.000000 edamame-0.53/edamame/classifier/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    22537 2023-05-22 21:51:22.000000 edamame-0.53/edamame/classifier/classification.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8611 2023-05-22 22:01:19.000000 edamame-0.53/edamame/classifier/diagnose.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-22 22:03:42.164985 edamame-0.53/edamame/eda/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      876 2023-05-06 16:04:28.000000 edamame-0.53/edamame/eda/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    32458 2023-03-25 15:28:28.000000 edamame-0.53/edamame/eda/eda.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4460 2023-05-22 20:40:47.000000 edamame-0.53/edamame/eda/tools.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-22 22:03:42.167001 edamame-0.53/edamame/regressor/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      189 2023-04-06 20:53:01.000000 edamame-0.53/edamame/regressor/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8347 2023-05-04 19:55:27.000000 edamame-0.53/edamame/regressor/diagnose.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    22034 2023-05-13 12:08:20.000000 edamame-0.53/edamame/regressor/regression.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-22 22:03:42.160761 edamame-0.53/edamame.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11959 2023-05-22 22:03:42.000000 edamame-0.53/edamame.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      461 2023-05-22 22:03:42.000000 edamame-0.53/edamame.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-05-22 22:03:42.000000 edamame-0.53/edamame.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       83 2023-05-22 22:03:42.000000 edamame-0.53/edamame.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        8 2023-05-22 22:03:42.000000 edamame-0.53/edamame.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      803 2023-05-22 22:01:47.000000 edamame-0.53/pyproject.toml
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-05-22 22:03:42.168618 edamame-0.53/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-24 21:35:58.775701 edamame-0.54/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 edamame-0.54/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11946 2023-05-24 21:35:58.775166 edamame-0.54/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10192 2023-05-23 09:35:51.000000 edamame-0.54/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-24 21:35:58.767033 edamame-0.54/edamame/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       21 2023-05-24 21:28:49.000000 edamame-0.54/edamame/__init__.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-24 21:35:58.770671 edamame-0.54/edamame/classifier/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      194 2023-05-04 19:56:56.000000 edamame-0.54/edamame/classifier/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    22454 2023-05-24 21:28:18.000000 edamame-0.54/edamame/classifier/classification.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8611 2023-05-22 22:01:19.000000 edamame-0.54/edamame/classifier/diagnose.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-24 21:35:58.772617 edamame-0.54/edamame/eda/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      876 2023-05-06 16:04:28.000000 edamame-0.54/edamame/eda/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    32458 2023-05-23 21:20:45.000000 edamame-0.54/edamame/eda/eda.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4460 2023-05-22 20:40:47.000000 edamame-0.54/edamame/eda/tools.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-24 21:35:58.774423 edamame-0.54/edamame/regressor/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      189 2023-04-06 20:53:01.000000 edamame-0.54/edamame/regressor/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8347 2023-05-04 19:55:27.000000 edamame-0.54/edamame/regressor/diagnose.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    22021 2023-05-23 08:36:34.000000 edamame-0.54/edamame/regressor/regression.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-24 21:35:58.768586 edamame-0.54/edamame.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11946 2023-05-24 21:35:58.000000 edamame-0.54/edamame.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      461 2023-05-24 21:35:58.000000 edamame-0.54/edamame.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-05-24 21:35:58.000000 edamame-0.54/edamame.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       83 2023-05-24 21:35:58.000000 edamame-0.54/edamame.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        8 2023-05-24 21:35:58.000000 edamame-0.54/edamame.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      803 2023-05-24 21:28:37.000000 edamame-0.54/pyproject.toml
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-05-24 21:35:58.775839 edamame-0.54/setup.cfg
```

### Comparing `edamame-0.53/LICENSE` & `edamame-0.54/LICENSE`

 * *Files identical despite different names*

### Comparing `edamame-0.53/PKG-INFO` & `edamame-0.54/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edamame
-Version: 0.53
+Version: 0.54
 Summary: Exploratory data analysis tools
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -27,30 +27,30 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Edamame
+## Edamame
 
 <h1 align="center">
 <img src="logo.png" width="200">
 </h1><br>
 
 [![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://edamame-doc.readthedocs.io/en/latest/index.html) [![PyPI version](https://badge.fury.io/py/edamame.svg)](https://badge.fury.io/py/edamame) ![PyPI - Downloads](https://img.shields.io/pypi/dm/edamame) [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 
 - [Edamame](#edamame)
-  - [Functionalities](#functionalities)
-  - [Eda module](#eda-module)
-  - [Regressor module](#regressor-module)
-    - [Example:](#example)
-  - [Classifier module](#classifier-module)
-    - [Example:](#example-1)
-  - [Todos](#todos)
+- [Functionalities](#functionalities)
+- [Eda module](#eda-module)
+- [Regressor module](#regressor-module)
+  - [Example:](#example)
+- [Classifier module](#classifier-module)
+  - [Example:](#example-1)
+- [Todos](#todos)
 
 
 Edamame is inspired by packages such as [pandas-profiling](https://github.com/ydataai/pandas-profiling), [pycaret](https://github.com/pycaret/pycaret>), and [yellowbrick](https://github.com/DistrictDataLabs/yellowbrick>). The goal of Edamame is to provide user-friendly functions for conducting exploratory data analysis (EDA) on datasets, as well as for training and analyzing batteries of models for regression or classification problems.
 
 To install the package,
 
 ```console
```

### Comparing `edamame-0.53/README.md` & `edamame-0.54/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# Edamame
+## Edamame
 
 <h1 align="center">
 <img src="logo.png" width="200">
 </h1><br>
 
 [![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://edamame-doc.readthedocs.io/en/latest/index.html) [![PyPI version](https://badge.fury.io/py/edamame.svg)](https://badge.fury.io/py/edamame) ![PyPI - Downloads](https://img.shields.io/pypi/dm/edamame) [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 
 - [Edamame](#edamame)
-  - [Functionalities](#functionalities)
-  - [Eda module](#eda-module)
-  - [Regressor module](#regressor-module)
-    - [Example:](#example)
-  - [Classifier module](#classifier-module)
-    - [Example:](#example-1)
-  - [Todos](#todos)
+- [Functionalities](#functionalities)
+- [Eda module](#eda-module)
+- [Regressor module](#regressor-module)
+  - [Example:](#example)
+- [Classifier module](#classifier-module)
+  - [Example:](#example-1)
+- [Todos](#todos)
 
 
 Edamame is inspired by packages such as [pandas-profiling](https://github.com/ydataai/pandas-profiling), [pycaret](https://github.com/pycaret/pycaret>), and [yellowbrick](https://github.com/DistrictDataLabs/yellowbrick>). The goal of Edamame is to provide user-friendly functions for conducting exploratory data analysis (EDA) on datasets, as well as for training and analyzing batteries of models for regression or classification problems.
 
 To install the package,
 
 ```console
```

### Comparing `edamame-0.53/edamame/classifier/classification.py` & `edamame-0.54/edamame/classifier/classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,28 +115,23 @@
 
 
     # ------------ #
     # KNN
     # ------------ #
     def knn(self, n_neighbors: Tuple[int, int, int] = (1, 50, 50), n_folds: int = 5, **kwargs) -> KNeighborsClassifier:
         """
-        Train a k-Nearest Neighbors classification model using the training data, and perform a grid search to find the
-    best value of 'n_neighbors' hyperparameter. 
+        Train a k-Nearest Neighbors classification model using the training data, and perform a grid search to find the best value of 'n_neighbors' hyperparameter. 
 
         Args:
-            n_neighbors (Tuple[int, int, int]): A tuple with three integers. The first and second integers are the range of the 
-                'n_neighbors' hyperparameter that will be searched by the grid search, and the third integer is the 
-                number of values to generate in the interval [n_neighbors[0], n_neighbors[1]]. Default is [1, 50, 50].
+            n_neighbors (Tuple[int, int, int]): A tuple with three integers. The first and second integers are the range of the 'n_neighbors' hyperparameter that will be searched by the grid search, and the third integer is the number of values to generate in the interval [n_neighbors[0], n_neighbors[1]]. Default is [1, 50, 50].
             n_folds (int): The number of cross-validation folds to use for the grid search. Default is 5.
             **kwargs: Arbitrary keyword arguments to be passed to the `KNN` constructor.
 
-
         Returns:
-            KNeighborsClassifier: The trained k-Nearest Neighbors classification model with the best 'n_neighbors' 
-                hyperparameter found by the grid search. 
+            KNeighborsClassifier: The trained k-Nearest Neighbors classification model with the best 'n_neighbors' hyperparameter found by the grid search. 
         
         Example:
             >>> from edamame.classifier import TrainClassifier
             >>> classifier = TrainClassifier(X_train=X_train, y_train=y_train, X_test=X_test, y_test=y_test)
             >>> knn = classifier.knn(n_neighbors=(1,50,50), n_folds=3) 
         """
         n_n = np.linspace(n_neighbors[0], n_neighbors[1], n_neighbors[2]).astype(np.int32)
@@ -155,15 +150,14 @@
     
         Args:
             alpha (Tuple[float, float, int]): A tuple containing the minimum and maximum values of ccp_alpha and the number of values to try (default: (0., 0.001, 5)).
             impurity (Tuple[float, float, int]): A tuple containing the minimum and maximum values of min_impurity_decrease and the number of values to try (default: (0., 0.00001, 5)).
             n_folds (int): The number of cross-validation folds to use for grid search (default: 5).
             **kwargs: Arbitrary keyword arguments to be passed to the `tree` constructor.
 
-
         Returns:
             DecisionTreeClassifier: The trained decision tree classifier model.
 
         Example:
             >>> from edamame.classifier import TrainClassifier
             >>> classifier = TrainClassifier(X_train=X_train, y_train=y_train, X_test=X_test, y_test=y_test)
             >>> tree = classifier.tree(alpha=(0., 0.001, 5), impurity=(0., 0.00001, 5), n_folds=3) 
@@ -256,21 +250,21 @@
         grid_svm_c = GridSearchCV(svm_c, tuned_parameters, cv=n_folds, refit=True, verbose=0, scoring='accuracy')
         grid_svm_c.fit(self.X_train, self.y_train.squeeze())
         # save the model in the instance attributes
         self.__svm_fit = grid_svm_c.best_estimator_
         return self.__svm_fit
 
 
-    def model_metrics(self, model_name: Literal["all", "logistic", "guassian_nb", "knn", "tree", "random_forest", "xgboost", "svm"] = 'all', confusion_matrix: bool = True) -> None:
+    def model_metrics(self, model_name: Literal["all", "logistic", "guassian_nb", "knn", "tree", "random_forest", "xgboost", "svm"] = 'all', cm: bool = False) -> None:
         """
         Display classification metrics (confusion matrix and classification report) for specified or all trained models.
 
         Args:
             model_name (Literal["all", "logistic", "guassian_nb", "knn", "tree", "random_forest", "xgboost", "svm"]): The name of the model to display the metrics for. Defaults to 'all'.
-            confusion_matrix (bool): Whether to display the confusion matrix. Defaults to True.
+            cm (bool): Whether to display the confusion matrix. Defaults to False.
 
         Returns:
             None
 
         Example:
             >>> from edamame.classifier import TrainClassifier
             >>> classifier = TrainClassifier(X_train=X_train, y_train=y_train, X_test=X_test, y_test=y_test)
```

### Comparing `edamame-0.53/edamame/classifier/diagnose.py` & `edamame-0.54/edamame/classifier/diagnose.py`

 * *Files identical despite different names*

### Comparing `edamame-0.53/edamame/eda/__init__.py` & `edamame-0.54/edamame/eda/__init__.py`

 * *Files identical despite different names*

### Comparing `edamame-0.53/edamame/eda/eda.py` & `edamame-0.54/edamame/eda/eda.py`

 * *Files identical despite different names*

### Comparing `edamame-0.53/edamame/eda/tools.py` & `edamame-0.54/edamame/eda/tools.py`

 * *Files identical despite different names*

### Comparing `edamame-0.53/edamame/regressor/diagnose.py` & `edamame-0.54/edamame/regressor/diagnose.py`

 * *Files identical despite different names*

### Comparing `edamame-0.53/edamame/regressor/regression.py` & `edamame-0.54/edamame/regressor/regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         Args: 
             **kwargs: Arbitrary keyword arguments to be passed to the `linear` constructor.
 
         Returns:
             LinearRegression: The trained linear regression model.
 
-    Example:
+        Example:
             >>> from edamame.regressor import TrainRegressor
             >>> regressor = TrainRegressor(X_train, np.log(y_train), X_test, np.log(y_test))
             >>> linear = regressor.linear()
         """
         linear = LinearRegression(**kwargs)
         linear.fit(self.X_train, self.y_train.squeeze())
         # save the model in the instance attributes
@@ -378,16 +378,15 @@
 
 
     def save_model(self, model_name: Literal["all", "linear", "lasso", "ridge", "tree", "random_forest", "xgboost"] = 'all') -> None:
         """
         Saves the specified machine learning model or all models in the instance to a pickle file.
 
         Args:
-            model_name (Literal["all", "linear", "lasso", "ridge", "tree", "random_forest", "xgboost"]): 
-                The name of the model to save. Defaults to 'all'.
+            model_name (Literal["all", "linear", "lasso", "ridge", "tree", "random_forest", "xgboost"]): The name of the model to save. Defaults to 'all'.
             
         Returns:
             None
 
         Example:
             >>> from edamame.regressor import TrainRegressor
             >>> regressor = TrainRegressor(X_train, np.log(y_train), X_test, np.log(y_test))
```

### Comparing `edamame-0.53/edamame.egg-info/PKG-INFO` & `edamame-0.54/edamame.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edamame
-Version: 0.53
+Version: 0.54
 Summary: Exploratory data analysis tools
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -27,30 +27,30 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Edamame
+## Edamame
 
 <h1 align="center">
 <img src="logo.png" width="200">
 </h1><br>
 
 [![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://edamame-doc.readthedocs.io/en/latest/index.html) [![PyPI version](https://badge.fury.io/py/edamame.svg)](https://badge.fury.io/py/edamame) ![PyPI - Downloads](https://img.shields.io/pypi/dm/edamame) [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 
 - [Edamame](#edamame)
-  - [Functionalities](#functionalities)
-  - [Eda module](#eda-module)
-  - [Regressor module](#regressor-module)
-    - [Example:](#example)
-  - [Classifier module](#classifier-module)
-    - [Example:](#example-1)
-  - [Todos](#todos)
+- [Functionalities](#functionalities)
+- [Eda module](#eda-module)
+- [Regressor module](#regressor-module)
+  - [Example:](#example)
+- [Classifier module](#classifier-module)
+  - [Example:](#example-1)
+- [Todos](#todos)
 
 
 Edamame is inspired by packages such as [pandas-profiling](https://github.com/ydataai/pandas-profiling), [pycaret](https://github.com/pycaret/pycaret>), and [yellowbrick](https://github.com/DistrictDataLabs/yellowbrick>). The goal of Edamame is to provide user-friendly functions for conducting exploratory data analysis (EDA) on datasets, as well as for training and analyzing batteries of models for regression or classification problems.
 
 To install the package,
 
 ```console
```

### Comparing `edamame-0.53/pyproject.toml` & `edamame-0.54/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "edamame"
-version = "0.53"
+version = "0.54"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Exploratory data analysis tools"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

