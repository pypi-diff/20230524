# Comparing `tmp/gmltools-0.0.65.tar.gz` & `tmp/gmltools-0.0.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.65.tar", last modified: Mon May 22 08:03:14 2023, max compression
+gzip compressed data, was "gmltools-0.0.66.tar", last modified: Wed May 24 08:39:02 2023, max compression
```

## Comparing `gmltools-0.0.65.tar` & `gmltools-0.0.66.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 08:03:14.952368 gmltools-0.0.65/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.65/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.65/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-05-22 08:03:14.951354 gmltools-0.0.65/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.65/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 08:03:14.632418 gmltools-0.0.65/dist/
--rw-rw-rw-   0        0        0    74791 2023-04-14 10:52:54.000000 gmltools-0.0.65/dist/gmltools-0.0.59.tar.gz
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.65/gmltools.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.65/mltools.yml
--rw-rw-rw-   0        0        0      546 2023-05-22 08:02:30.000000 gmltools-0.0.65/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-22 08:03:14.952368 gmltools-0.0.65/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-05-22 08:02:08.000000 gmltools-0.0.65/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 08:03:14.551759 gmltools-0.0.65/src/
-drwxrwxrwx   0        0        0        0 2023-05-22 08:03:14.667636 gmltools-0.0.65/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.65/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.65/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 08:03:14.763395 gmltools-0.0.65/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.65/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    40126 2023-04-17 07:50:02.000000 gmltools-0.0.65/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-05-22 08:03:14.830436 gmltools-0.0.65/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.65/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.65/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.65/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0     5143 2023-04-14 11:04:34.000000 gmltools-0.0.65/src/gmltools/models/dummy_model.py
--rw-rw-rw-   0        0        0   126791 2023-05-22 08:00:36.000000 gmltools-0.0.65/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     6170 2023-05-22 07:56:38.000000 gmltools-0.0.65/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0    13212 2023-05-12 09:20:42.000000 gmltools-0.0.65/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-05-22 08:03:14.875102 gmltools-0.0.65/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.65/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.65/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.65/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-05-22 08:03:14.945263 gmltools-0.0.65/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.65/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.65/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.65/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.65/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-05-22 08:03:14.738041 gmltools-0.0.65/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-05-22 08:03:13.000000 gmltools-0.0.65/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-05-22 08:03:14.000000 gmltools-0.0.65/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 08:03:13.000000 gmltools-0.0.65/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-05-22 08:03:13.000000 gmltools-0.0.65/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 08:03:13.000000 gmltools-0.0.65/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 08:39:02.839106 gmltools-0.0.66/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.66/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.66/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-05-24 08:39:02.838039 gmltools-0.0.66/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.66/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 08:39:02.573719 gmltools-0.0.66/dist/
+-rw-rw-rw-   0        0        0    74791 2023-04-14 10:52:54.000000 gmltools-0.0.66/dist/gmltools-0.0.59.tar.gz
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.66/gmltools.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.66/mltools.yml
+-rw-rw-rw-   0        0        0      546 2023-05-24 08:38:09.000000 gmltools-0.0.66/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 08:39:02.840032 gmltools-0.0.66/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-05-24 08:37:54.000000 gmltools-0.0.66/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 08:39:02.478191 gmltools-0.0.66/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 08:39:02.605636 gmltools-0.0.66/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.66/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.66/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 08:39:02.675423 gmltools-0.0.66/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.66/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    40126 2023-04-17 07:50:02.000000 gmltools-0.0.66/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-05-24 08:39:02.743200 gmltools-0.0.66/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.66/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.66/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.66/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0     5518 2023-05-24 08:37:38.000000 gmltools-0.0.66/src/gmltools/models/dummy_model.py
+-rw-rw-rw-   0        0        0   126801 2023-05-24 08:27:59.000000 gmltools-0.0.66/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     6170 2023-05-22 07:56:38.000000 gmltools-0.0.66/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0    13212 2023-05-12 09:20:42.000000 gmltools-0.0.66/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-05-24 08:39:02.779204 gmltools-0.0.66/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.66/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.66/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.66/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-05-24 08:39:02.833084 gmltools-0.0.66/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.66/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.66/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.66/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.66/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-05-24 08:39:02.653516 gmltools-0.0.66/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-05-24 08:39:01.000000 gmltools-0.0.66/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-05-24 08:39:02.000000 gmltools-0.0.66/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 08:39:01.000000 gmltools-0.0.66/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-05-24 08:39:01.000000 gmltools-0.0.66/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-24 08:39:01.000000 gmltools-0.0.66/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.65/LICENSE` & `gmltools-0.0.66/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.65/Models.ipynb` & `gmltools-0.0.66/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.65/PKG-INFO` & `gmltools-0.0.66/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.65
+Version: 0.0.66
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.65/README.md` & `gmltools-0.0.66/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.65/dist/gmltools-0.0.59.tar.gz` & `gmltools-0.0.66/dist/gmltools-0.0.59.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.65/gmltools.yml` & `gmltools-0.0.66/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.65/mltools.yml` & `gmltools-0.0.66/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.65/pyproject.toml` & `gmltools-0.0.66/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.65"
+version = "0.0.66"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.65/setup.py` & `gmltools-0.0.66/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.65',
+    'version': '0.0.66',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.65/src/gmltools/To_Do.txt` & `gmltools-0.0.66/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.65/src/gmltools/eda/eda.py` & `gmltools-0.0.66/src/gmltools/eda/eda.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.65/src/gmltools/models/bayes.py` & `gmltools-0.0.66/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.65/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.66/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.65/src/gmltools/models/dummy_model.py` & `gmltools-0.0.66/src/gmltools/models/dummy_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         mse=np.mean(mse_list)
         std_mse=np.std(mse_list)
         index.extend(["mean","std"])
         mse_list.extend([mse,std_mse])
 
         self.df_scores=pd.DataFrame(mse_list,columns=[f"Naive Model shifts {self.shifts}"],index=index)
         return self.df_scores
-    def get_plot(self,figsize:tuple=(5000,2800), continious:bool=False):
+    def get_plot(self,figsize:tuple=(5000,2800), title_font=25, ytitle="y", xtitle="x",xtickfont=16, ytickfont=16, ytitlefont=16, xtitlefont=16, continious:bool=False):
         """
         This function returns a plotly figure with the predictions of the model for each test split.
         Making continious=True will plot all the predictions in one plot. Otherwise each test split will be plotted in a subplot.
 
         Parameters
         ----------
         figsize : tuple, optional
@@ -105,19 +105,23 @@
         if continious:
             continious_preds=pd.concat(pred_list)
             #plot the true and pred col of the dataframe in one plotly
             fig = go.Figure()
             fig.add_trace(go.Scatter(x=continious_preds.index, y=continious_preds["true"], mode="lines", name="True"))
             fig.add_trace(go.Scatter(x=continious_preds.index, y=continious_preds["pred"], mode="lines", name="Predicted"))
 
-            fig.update_layout(title="Naive True vs Predicted Values", xaxis_title="Date", yaxis_title="Value")
+            fig.update_layout(title="Naive, True vs Predicted Values",height=figsize[0], width=figsize[1],title_font=dict(size=title_font))
+            fig.update_layout(xaxis=dict(title=xtitle, tickfont=dict(size=xtickfont), title_font=dict(size=xtitlefont)),
+                              yaxis=dict(title=ytitle, tickfont=dict(size=ytickfont), title_font=dict(size=ytitlefont)))
             fig.show()
 
 
         else:
             fig=make_subplots(rows=len(pred_list),cols=1,subplot_titles=self.tscv.get_test_days(self.X),)
             for i,df in enumerate(pred_list):
                 fig.add_trace(go.Scatter(x=df.index, y=df["true"], mode="lines", name="True"), row=i+1, col=1)
                 fig.add_trace(go.Scatter(x=df.index, y=df["pred"], mode="lines", name="Predicted"), row=i+1, col=1)
 
             fig.update_layout(height=figsize[0], width=figsize[1], title=f"Naive Model Predictions with {self.shifts} hour shifts")
-            fig.show()
+            fig.show()
+
+
```

### Comparing `gmltools-0.0.65/src/gmltools/models/model.py` & `gmltools-0.0.66/src/gmltools/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1774,15 +1774,15 @@
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
                                         'scoring':str(scoring), 'cv':str(self.cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
         
             print(self.model.best_params_)
 
 
-    def SVR(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
+    def SVR_Regressor(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'SVR__kernel':['linear','poly','rbf'],
                                 'SVR__C': [0.00001,0.0001,0.001,0.01,0.1,1,10,100,1000],
                                 'SVR__gamma':[0.0001,0.001,0.01,0.1,1,10]}, 
                             random_params=None, random_n_iter=10, bayes_pbounds=None,
                             bayes_int_params=None, bayes_n_iter=30, sample_weight=None, n_jobs=-1,
                             columns_lags=None, column_rolled_lags=None,lags=None,rolled_lags=None, rolled_metrics=None, column_rolled_lags_initial=None):
```

### Comparing `gmltools-0.0.65/src/gmltools/models/models_info.py` & `gmltools-0.0.66/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.65/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.66/src/gmltools/models/timeseriesplit.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.65/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.66/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.65/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.66/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.65/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.66/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.65/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.66/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.65/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.66/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.65/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.66/src/gmltools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.65
+Version: 0.0.66
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.65/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.66/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

