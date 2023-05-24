# Comparing `tmp/gmlutil-0.7.9.tar.gz` & `tmp/gmlutil-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gmlutil-0.7.9.tar", last modified: Wed Apr  5 00:16:23 2023, max compression
+gzip compressed data, was "dist/gmlutil-0.8.1.tar", last modified: Wed May 24 00:53:51 2023, max compression
```

## Comparing `gmlutil-0.7.9.tar` & `gmlutil-0.8.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 phillip.kimejgallo.com   (502) staff       (20)        0 2023-04-05 00:16:23.305602 gmlutil-0.7.9/
--rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)      854 2023-04-05 00:16:23.300077 gmlutil-0.7.9/PKG-INFO
--rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)      199 2022-07-26 00:57:31.000000 gmlutil-0.7.9/README.md
-drwxr-xr-x   0 phillip.kimejgallo.com   (502) staff       (20)        0 2023-04-05 00:16:23.288806 gmlutil-0.7.9/gmlutil/
--rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)       77 2022-07-25 19:26:55.000000 gmlutil-0.7.9/gmlutil/__init__.py
--rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)    43804 2023-01-25 19:55:11.000000 gmlutil-0.7.9/gmlutil/gmlutil.py
-drwxr-xr-x   0 phillip.kimejgallo.com   (502) staff       (20)        0 2023-04-05 00:16:23.298263 gmlutil-0.7.9/gmlutil.egg-info/
--rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)      854 2023-04-05 00:16:22.000000 gmlutil-0.7.9/gmlutil.egg-info/PKG-INFO
--rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)      211 2023-04-05 00:16:23.000000 gmlutil-0.7.9/gmlutil.egg-info/SOURCES.txt
--rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)        1 2023-04-05 00:16:22.000000 gmlutil-0.7.9/gmlutil.egg-info/dependency_links.txt
--rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)      535 2023-04-05 00:16:22.000000 gmlutil-0.7.9/gmlutil.egg-info/requires.txt
--rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)        8 2023-04-05 00:16:22.000000 gmlutil-0.7.9/gmlutil.egg-info/top_level.txt
--rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)       38 2023-04-05 00:16:23.305913 gmlutil-0.7.9/setup.cfg
--rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)     1670 2023-04-05 00:16:19.000000 gmlutil-0.7.9/setup.py
+drwxr-xr-x   0 phillip.kimejgallo.com   (502) staff       (20)        0 2023-05-24 00:53:51.099423 gmlutil-0.8.1/
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)      905 2023-05-24 00:53:51.098928 gmlutil-0.8.1/PKG-INFO
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)      199 2022-07-26 00:57:31.000000 gmlutil-0.8.1/README.md
+drwxr-xr-x   0 phillip.kimejgallo.com   (502) staff       (20)        0 2023-05-24 00:53:51.089037 gmlutil-0.8.1/gmlutil/
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)       77 2022-07-25 19:26:55.000000 gmlutil-0.8.1/gmlutil/__init__.py
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)    43871 2023-04-06 23:52:50.000000 gmlutil-0.8.1/gmlutil/gmlutil.py
+drwxr-xr-x   0 phillip.kimejgallo.com   (502) staff       (20)        0 2023-05-24 00:53:51.098031 gmlutil-0.8.1/gmlutil.egg-info/
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)      905 2023-05-24 00:53:50.000000 gmlutil-0.8.1/gmlutil.egg-info/PKG-INFO
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)      211 2023-05-24 00:53:50.000000 gmlutil-0.8.1/gmlutil.egg-info/SOURCES.txt
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)        1 2023-05-24 00:53:50.000000 gmlutil-0.8.1/gmlutil.egg-info/dependency_links.txt
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)      585 2023-05-24 00:53:50.000000 gmlutil-0.8.1/gmlutil.egg-info/requires.txt
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)        8 2023-05-24 00:53:50.000000 gmlutil-0.8.1/gmlutil.egg-info/top_level.txt
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)       38 2023-05-24 00:53:51.099598 gmlutil-0.8.1/setup.cfg
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)     1825 2023-05-24 00:52:23.000000 gmlutil-0.8.1/setup.py
```

### Comparing `gmlutil-0.7.9/PKG-INFO` & `gmlutil-0.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: gmlutil
-Version: 0.7.9
+Version: 0.8.1
 Summary: General Machine Learning Utility Package
 Home-page: https://github.com/Phillip1982/gmlutil
 Author: Phillip Kim
 Author-email: phillip.kim@ejgallo.com
 License: BSD 2-clause
 Description: UNKNOWN
 Platform: UNKNOWN
@@ -16,7 +16,8 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows XP
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gmlutil-0.7.9/gmlutil/gmlutil.py` & `gmlutil-0.8.1/gmlutil/gmlutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import pickle
 import plotly.graph_objects as go
 import plotly.express as px
 import seaborn as sns
 import sqlalchemy as sa
 import sys
 import time
-import umap.umap_ as umap
+# import umap.umap_ as umap
 from fuzzywuzzy import fuzz
 from geopandas import GeoDataFrame
 from geopandas import points_from_xy
 from imblearn.over_sampling import SMOTE
 from imblearn.under_sampling import RandomUnderSampler
 from imblearn.pipeline import Pipeline
 from io import BufferedReader, TextIOWrapper
@@ -36,15 +36,15 @@
 from sklearn.model_selection import train_test_split, cross_val_score, RepeatedStratifiedKFold
 from sklearn.linear_model import LinearRegression, LogisticRegression
 from sklearn.naive_bayes import GaussianNB
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.svm import SVC
 from sklearn.tree import DecisionTreeClassifier
 from sklearn.ensemble import BaggingClassifier, RandomForestClassifier, StackingClassifier
-from sklearn.metrics import classification_report, confusion_matrix, plot_confusion_matrix
+from sklearn.metrics import classification_report, confusion_matrix, ConfusionMatrixDisplay
 from sklearn.decomposition import PCA
 from sklearn.cluster import KMeans, SpectralClustering, AgglomerativeClustering, DBSCAN, Birch
 from sklearn.manifold import TSNE
 from sklearn.mixture import GaussianMixture
 from sqlalchemy import Table, MetaData, select, delete
 from statsmodels.tsa.stattools import adfuller
 from types import SimpleNamespace
@@ -592,26 +592,26 @@
         return X_train, X_test, y_train, y_test
 
 ########################### Data Visualization ###########################
 class data_visualization:
     def __init__(self):
         pass
 
-    def plot_confusion(self, model, X, y, class_names, normalized='true'):
-        titles_options = [("Confusion matrix, without normalization", None),
-                          ("Normalized confusion matrix", normalized)]
-        for title, normalize in titles_options:
-            display = plot_confusion_matrix(model, X, y,
-                                         display_labels=class_names,
-                                         cmap=plt.cm.Blues,
-                                         normalize=normalize)
-            display.ax_.set_title(title)
-            print(title)
-            print(display.confusion_matrix)
-        plt.show()
+#     def plot_confusion(self, model, X, y, class_names, normalized='true'):
+#         titles_options = [("Confusion matrix, without normalization", None),
+#                           ("Normalized confusion matrix", normalized)]
+#         for title, normalize in titles_options:
+#             display = plot_confusion_matrix(model, X, y,
+#                                          display_labels=class_names,
+#                                          cmap=plt.cm.Blues,
+#                                          normalize=normalize)
+#             display.ax_.set_title(title)
+#             print(title)
+#             print(display.confusion_matrix)
+#         plt.show()
 
     def data_visualization(self, df, column_list, removal_list, title, x_axis):
         try:
             df = df.drop(removal_list, axis=1)
         except:
             pass
         sqrt_num = int(math.sqrt(len(column_list)))
@@ -680,34 +680,34 @@
         transformed = model_tsne.fit_transform(df)
         x_axis = transformed[:, 0]
         y_axis = transformed[:, 1]
         plt.scatter(x_axis, y_axis)
         print(model_name)
         plt.show()
 
-    def umap_graph(self, df):
-        numerical_df = df.select_dtypes(exclude='object')
-        for c in numerical_df.columns:
-            pt = PowerTransformer()
-            numerical_df.loc[:, c] = pt.fit_transform(np.array(numerical_df[c]).reshape(-1, 1))
-        categorical_df = df.select_dtypes(include='object')
-        categorical_df = pd.get_dummies(categorical_df)
-        categorical_weight = len(df.select_dtypes(include='object').columns) / len(df.columns)
-        fit1 = umap.UMAP(metric='l2').fit(numerical_df)
-        fit2 = umap.UMAP(metric='dice').fit(categorical_df)
-        intersection = umap.general_simplicial_set_intersection(fit1.graph_, fit2.graph_, weight=categorical_weight)
-        intersection = umap.reset_local_connectivity(intersection)
-        embedding = umap.simplicial_set_embedding(fit1._raw_data, intersection, fit1.n_components, 
-                                                        fit1._initial_alpha, fit1._a, fit1._b, 
-                                                        fit1.repulsion_strength, fit1.negative_sample_rate, 
-                                                        200, 'random', np.random, fit1.metric, 
-                                                        fit1._metric_kwds, False)
-        plt.figure(figsize=(20, 10))
-        plt.scatter(*embedding.T, s=2, cmap='Spectral', alpha=1.0)
-        plt.show()
+#     def umap_graph(self, df):
+#         numerical_df = df.select_dtypes(exclude='object')
+#         for c in numerical_df.columns:
+#             pt = PowerTransformer()
+#             numerical_df.loc[:, c] = pt.fit_transform(np.array(numerical_df[c]).reshape(-1, 1))
+#         categorical_df = df.select_dtypes(include='object')
+#         categorical_df = pd.get_dummies(categorical_df)
+#         categorical_weight = len(df.select_dtypes(include='object').columns) / len(df.columns)
+#         fit1 = umap.UMAP(metric='l2').fit(numerical_df)
+#         fit2 = umap.UMAP(metric='dice').fit(categorical_df)
+#         intersection = umap.general_simplicial_set_intersection(fit1.graph_, fit2.graph_, weight=categorical_weight)
+#         intersection = umap.reset_local_connectivity(intersection)
+#         embedding = umap.simplicial_set_embedding(fit1._raw_data, intersection, fit1.n_components, 
+#                                                         fit1._initial_alpha, fit1._a, fit1._b, 
+#                                                         fit1.repulsion_strength, fit1.negative_sample_rate, 
+#                                                         200, 'random', np.random, fit1.metric, 
+#                                                         fit1._metric_kwds, False)
+#         plt.figure(figsize=(20, 10))
+#         plt.scatter(*embedding.T, s=2, cmap='Spectral', alpha=1.0)
+#         plt.show()
 
 
 ########################### Model Training ###########################
 class model_training:
     def __init__(self):
         pass
```

### Comparing `gmlutil-0.7.9/gmlutil.egg-info/PKG-INFO` & `gmlutil-0.8.1/gmlutil.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: gmlutil
-Version: 0.7.9
+Version: 0.8.1
 Summary: General Machine Learning Utility Package
 Home-page: https://github.com/Phillip1982/gmlutil
 Author: Phillip Kim
 Author-email: phillip.kim@ejgallo.com
 License: BSD 2-clause
 Description: UNKNOWN
 Platform: UNKNOWN
@@ -16,7 +16,8 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows XP
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gmlutil-0.7.9/gmlutil.egg-info/requires.txt` & `gmlutil-0.8.1/gmlutil.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 aiobotocore==2.5.0
+awscli==1.27.76
 boto3==1.26.76
 botocore==1.29.76
 cx-Oracle==8.3.0
 dash==2.0.0
 datetime==4.3
 folium==0.14.0
 fuzzywuzzy==0.18.0
 geopandas==0.10.2
 hana-ml
 imbalanced-learn==0.8.0
 jupyter_dash==0.4.0
 kmodes==0.11.0
 minio==4.0.6
 numpy==1.21.6
-pandas==1.1.5
+pandas==1.3.0
+packaging==21.3
 plotly==5.4.0
 psycopg2-binary==2.9.1
 pyhdb==0.3.4
 pymssql==2.2.1
 pytest-astropy
 pytrends==4.7.3
 rsa<4.8,>=3.1.2
 sagemaker==2.0.0
 sagemaker-data-insights==0.3.0
+seaborn==0.11.2
 sparkmagic==0.20.4
 sqlalchemy-redshift==0.8.6
+statsmodels==0.13.2
 s3transfer==0.6.0
 typing_extensions>=4.0
-umap-learn==0.5.1
 xgboost==1.3.3
```

### Comparing `gmlutil-0.7.9/setup.py` & `gmlutil-0.8.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,63 @@
 from setuptools import setup
 
 setup(
     name='gmlutil',
-    version='0.7.9',    
+    version='0.8.1',    
     description='General Machine Learning Utility Package',
     url='https://github.com/Phillip1982/gmlutil',
     author='Phillip Kim',
     author_email='phillip.kim@ejgallo.com',
     license='BSD 2-clause', ## Change this
     packages=['gmlutil'],
     install_requires=[
     	'aiobotocore==2.5.0',
+    	'awscli==1.27.76',
 		'boto3==1.26.76', # 1.20.24', 
 		'botocore==1.29.76', # 1.23.24', 
 		'cx-Oracle==8.3.0',
 		'dash==2.0.0',
 		'datetime==4.3',
 		'folium==0.14.0',
 		'fuzzywuzzy==0.18.0',
 		'geopandas==0.10.2',
 		'hana-ml',
 		'imbalanced-learn==0.8.0',
 		'jupyter_dash==0.4.0',
 		'kmodes==0.11.0',
 		'minio==4.0.6',
 		'numpy==1.21.6',
-		'pandas==1.1.5',
+		'pandas==1.3.0',
+        'packaging==21.3',
 		'plotly==5.4.0',
 		'psycopg2-binary==2.9.1',
 		'pyhdb==0.3.4',
 		'pymssql==2.2.1',
 		'pytest-astropy',
 		'pytrends==4.7.3',
 		'rsa<4.8,>=3.1.2',
 		'sagemaker==2.0.0',
 		'sagemaker-data-insights==0.3.0',
+        'seaborn==0.11.2',
 		'sparkmagic==0.20.4',
 		'sqlalchemy-redshift==0.8.6',
+		'statsmodels==0.13.2',
 		's3transfer==0.6.0', # 0.5.0',
 		'typing_extensions>=4.0',
-		'umap-learn==0.5.1',
+# 		'umap-learn==0.5.1',
 		'xgboost==1.3.3'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Framework :: IPython',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
 		'Operating System :: MacOS',
 		'Operating System :: Microsoft :: Windows :: Windows XP',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9'
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10'
     ],
 )
```

