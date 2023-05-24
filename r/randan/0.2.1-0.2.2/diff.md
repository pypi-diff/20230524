# Comparing `tmp/randan-0.2.1.tar.gz` & `tmp/randan-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/lanalob/Yandex.Disk-lana.lob.localized/??????/???????_???????????/?????_??????/randan/dist/tmpp44fuyen/randan-0.2.1.tar", last modified: Sun Feb 28 21:13:35 2021, max compression
+gzip compressed data, was "randan-0.2.2.tar", last modified: Wed May 24 11:24:36 2023, max compression
```

## Comparing `randan-0.2.1.tar` & `randan-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 lanalob    (501) staff       (20)        0 2021-02-28 21:13:35.000000 randan-0.2.1/
--rw-r--r--   0 lanalob    (501) staff       (20)     1436 2021-02-28 21:13:35.000000 randan-0.2.1/PKG-INFO
-drwxr-xr-x   0 lanalob    (501) staff       (20)        0 2021-02-28 21:13:35.000000 randan-0.2.1/randan/
--rw-r--r--   0 lanalob    (501) staff       (20)    78916 2021-02-28 21:05:47.000000 randan-0.2.1/randan/dimension_reduction.py
--rw-r--r--   0 lanalob    (501) staff       (20)    69370 2020-11-15 15:23:31.000000 randan-0.2.1/randan/tree.py
--rw-r--r--   0 lanalob    (501) staff       (20)    50612 2020-11-15 15:23:31.000000 randan-0.2.1/randan/regression.py
--rw-r--r--   0 lanalob    (501) staff       (20)    16076 2020-11-15 15:23:31.000000 randan-0.2.1/randan/clustering.py
--rw-r--r--   0 lanalob    (501) staff       (20)      184 2020-11-15 15:59:50.000000 randan-0.2.1/randan/__init__.py
--rw-r--r--   0 lanalob    (501) staff       (20)     6101 2020-11-15 15:23:31.000000 randan-0.2.1/randan/comparison_of_central_tendency.py
--rw-r--r--   0 lanalob    (501) staff       (20)     4369 2020-11-15 15:24:38.000000 randan-0.2.1/randan/utils.py
--rw-r--r--   0 lanalob    (501) staff       (20)    21378 2020-11-18 07:19:51.000000 randan-0.2.1/randan/descriptive_statistics.py
--rw-r--r--   0 lanalob    (501) staff       (20)    17720 2020-11-15 16:43:25.000000 randan-0.2.1/randan/bivariate_association.py
-drwxr-xr-x   0 lanalob    (501) staff       (20)        0 2021-02-28 21:13:35.000000 randan-0.2.1/randan.egg-info/
--rw-r--r--   0 lanalob    (501) staff       (20)     1436 2021-02-28 21:13:35.000000 randan-0.2.1/randan.egg-info/PKG-INFO
--rw-r--r--   0 lanalob    (501) staff       (20)      395 2021-02-28 21:13:35.000000 randan-0.2.1/randan.egg-info/SOURCES.txt
--rw-r--r--   0 lanalob    (501) staff       (20)      131 2021-02-28 21:13:35.000000 randan-0.2.1/randan.egg-info/requires.txt
--rw-r--r--   0 lanalob    (501) staff       (20)        7 2021-02-28 21:13:35.000000 randan-0.2.1/randan.egg-info/top_level.txt
--rw-r--r--   0 lanalob    (501) staff       (20)        1 2021-02-28 21:13:35.000000 randan-0.2.1/randan.egg-info/dependency_links.txt
--rw-r--r--   0 lanalob    (501) staff       (20)      820 2020-11-15 15:23:30.000000 randan-0.2.1/README.md
--rw-r--r--   0 lanalob    (501) staff       (20)     1023 2021-02-28 21:10:28.000000 randan-0.2.1/setup.py
--rw-r--r--   0 lanalob    (501) staff       (20)       38 2021-02-28 21:13:35.000000 randan-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 11:24:36.506990 randan-0.2.2/
+-rw-rw-rw-   0        0        0     1064 2023-05-23 13:47:22.000000 randan-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0    10726 2023-05-24 11:24:36.480941 randan-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10042 2023-05-23 13:47:22.000000 randan-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 11:24:36.364853 randan-0.2.2/randan/
+-rw-rw-rw-   0        0        0      186 2023-05-23 13:47:22.000000 randan-0.2.2/randan/__init__.py
+-rw-rw-rw-   0        0        0    17604 2023-05-23 13:47:22.000000 randan-0.2.2/randan/bivariate_association.py
+-rw-rw-rw-   0        0        0    15970 2023-05-23 13:47:22.000000 randan-0.2.2/randan/clustering.py
+-rw-rw-rw-   0        0        0     6076 2023-05-23 13:47:22.000000 randan-0.2.2/randan/comparison_of_central_tendency.py
+-rw-rw-rw-   0        0        0    21177 2023-05-23 13:47:22.000000 randan-0.2.2/randan/descriptive_statistics.py
+-rw-rw-rw-   0        0        0    78729 2023-05-23 13:47:22.000000 randan-0.2.2/randan/dimension_reduction.py
+-rw-rw-rw-   0        0        0    50545 2023-05-23 13:47:22.000000 randan-0.2.2/randan/regression.py
+-rw-rw-rw-   0        0        0    69334 2023-05-23 13:47:22.000000 randan-0.2.2/randan/tree.py
+-rw-rw-rw-   0        0        0     4371 2023-05-23 13:47:22.000000 randan-0.2.2/randan/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-24 11:24:36.472974 randan-0.2.2/randan.egg-info/
+-rw-rw-rw-   0        0        0    10726 2023-05-24 11:24:35.000000 randan-0.2.2/randan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-05-24 11:24:35.000000 randan-0.2.2/randan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 11:24:35.000000 randan-0.2.2/randan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2023-05-24 11:24:35.000000 randan-0.2.2/randan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-24 11:24:35.000000 randan-0.2.2/randan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 11:24:36.507988 randan-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2023-05-24 11:16:45.000000 randan-0.2.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `randan-0.2.1/randan/dimension_reduction.py` & `randan-0.2.2/randan/dimension_reduction.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,23 +261,21 @@
         n_decimals : int 
             Number of digits to round results when showing them
         """
         print('\nCA SUMMARY')
         print('------------------\n')
         print('Explained inertia')
         display(self.inertia_by_dimensions.style\
-                    .format(None, na_rep="")\
-                    .set_caption("attribute .inertia_by_dimensions")\
-                    .set_precision(n_decimals))
+                    .format(None, na_rep="", precision=n_decimals)\
+                    .set_caption("attribute .inertia_by_dimensions"))
         print('------------------\n')
         print('Detailed information')
         display(self.summary().style\
-                    .format(None, na_rep="")\
-                    .set_caption("method .summary()")\
-                    .set_precision(n_decimals))        
+                    .format(None, na_rep="", precision=n_decimals)\
+                    .set_caption("method .summary()"))
     
     def summary(self, 
                 display_component_loadings=True, 
                 display_contributions=False,
                 display_coordinates=False):
         """
         Return summary of the fitted model
@@ -1034,36 +1032,33 @@
                 elif self.n_components_criterion=='Inflection point (based on scree plot)':
                     print(f'The number of selected components by an inflection point: {self.n_components}')
                 print('------------------\n')
         
         if self.rotation != 'natural collinearity':
             print('Explained variance')
             display(self.get_explained_variance(scree_plot=True).style\
-                    .format(None, na_rep="")\
-                    .set_caption("methods .get_explained_variance() and .scree_plot()")\
-                    .set_precision(n_decimals))
+                    .format(None, na_rep="", precision=n_decimals)\
+                    .set_caption("methods .get_explained_variance() and .scree_plot()"))
             print(f'The model explains {round(self.explained_variance_total, n_decimals)}% of variance.')
             print('------------------\n')
         if self.rotation is None:
             print('Component loadings')
         elif self.rotation == 'varimax':
             print('Rotated component loadings')
         elif self.rotation in ['natural collinearity', 'promax']:
             print('Structure matrix')
         display(self.communalities_and_loadings.style\
-                .format(None, na_rep="")\
-                .set_caption("attribute .communalities_and_loadings")\
-                .set_precision(n_decimals))
+                .format(None, na_rep="", precision=n_decimals)\
+                .set_caption("attribute .communalities_and_loadings"))
         print(f'The minimum communality is {round(self.communalities["Communality"].min(), n_decimals)}.')
         if self.rotation in ['natural collinearity', 'promax']:
             print("Components' correlation")
             display(self.correlation_matrix_components.style\
-                .format(None, na_rep="")\
-                .set_caption("attribute .correlation_matrix_components")\
-                .set_precision(n_decimals))
+                .format(None, na_rep="", precision=n_decimals)\
+                .set_caption("attribute .correlation_matrix_components"))
         print('------------------\n')
         print('To get component scores, use [model].transform().')
     def transform(self, data, standardize=True, add_to_data=False):
         
         """
         Return component scores for every observation in the given dataset. 
         
@@ -1628,27 +1623,25 @@
 #         print('\nPCA SUMMARY')
 #         print('------------------\n')                                 
 #         if self.n_components_criterion=='Kaiser':
 #             print(f'The number of selected components by Kaiser criterion: {self.n_components}')
 #             print('------------------\n')
 #         print('Explained variance')
 #         display(self.get_explained_variance(scree_plot=True).style\
-#                     .format(None, na_rep="")\
-#                     .set_caption("methods .get_explained_variance() and .scree_plot()")\
-#                     .set_precision(n_decimals))
+#                     .format(None, na_rep="", precision=n_decimals)\
+#                     .set_caption("methods .get_explained_variance() and .scree_plot()"))
 #         print(f'The model explains {round(self.explained_variance_total, 3)}% of variance.')
 #         print('------------------\n')
 #         if self.rotation is None:
 #             print('Component loadings')
 #         elif self.rotation == 'varimax':
 #             print('Rotated component loadings')
 #         display(self.communalities_and_loadings.style\
-#                 .format(None, na_rep="")\
-#                 .set_caption("attribute .communalities_and_loadings")\
-#                 .set_precision(n_decimals))
+#                 .format(None, na_rep="", precision=n_decimals)\
+#                 .set_caption("attribute .communalities_and_loadings"))
 #         print(f'The minimum communality is {round(self.communalities["Communality"].min(), 3)}.')
 #         print('------------------\n')
 #         print('To get component scores, use [model].transform().')
 
 #     def transform(self, data=None, standardize=True, add_to_data=False):
         
 #         """
@@ -1821,8 +1814,8 @@
 #             acc_sum_by_n_components = [explained_variance.iloc[self.n_components-1, 2]] * len(pc_num)
 #             plt.plot(pc_num, acc_sum_by_n_components, linestyle='--', label='Current solution', c='black')
                 
 #         plt.xlabel('Principal components')
 #         plt.ylabel('Variance accounted for, %')
 #         plt.title('Variance accounted by components', fontsize=16)
 #         plt.legend(loc='upper left')
-#         plt.show()
+#         plt.show()
```

### Comparing `randan-0.2.1/randan/tree.py` & `randan-0.2.2/randan/tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,33 +379,32 @@
         print('------------------\n')
         print('Tree information')
         display(self.summary())
         if tree_in_table_format:
             print('------------------\n')
             print('Tree nodes')
             display(self.nodes.style\
-                    .format(None, na_rep="")\
-                    .set_caption(f'Dependent variable: {self._dependent_variable}, independent variables: {", ".join(self._independent_variables)}')\
-                    .set_precision(n_decimals))
+                    .format(None, na_rep="", precision=n_decimals)\
+                    .set_caption(f'Dependent variable: {self._dependent_variable}, independent variables: {", ".join(self._independent_variables)}'))
         print('------------------\n')
         print('Classification table')
         display(self.classification_table.style\
-                .set_precision(1))
+                .format(precision=1))
         if self._use_test_data:
             print('Classification table for test data')
             display(self.classification_table_test.style\
-                .set_precision(1))
+                    .format(precision=1))
         print('------------------\n')
         print('Prediction quality metrics')
         display(self.precision_and_recall.style\
-                .set_precision(n_decimals))
+                .format(precision=n_decimals))
         if self._use_test_data:
             print('Prediction quality metrics for test data')
             display(self.precision_and_recall_test.style\
-                .set_precision(n_decimals))
+                .format(precision=n_decimals))
                              
     
     def get_classification_table(self):
         """
         Get the classification table as it is shown in SPSS.
 
         Returns
@@ -1172,17 +1171,16 @@
         print('------------------\n')
         print('Tree information')
         display(self.summary())
         if tree_in_table_format:
             print('------------------\n')
             print('Tree nodes')
             display(self.nodes.style\
-                    .format(None, na_rep="")\
-                    .set_caption(f'Dependent variable: {self._dependent_variable}, independent variables: {", ".join(self._independent_variables)}')\
-                    .set_precision(n_decimals))
+                    .format(None, na_rep="", precision=n_decimals)\
+                    .set_caption(f'Dependent variable: {self._dependent_variable}, independent variables: {", ".join(self._independent_variables)}'))
                                  
     def _check_if_terminal_node(self, node):
         if node['Node'] in self.nodes['Parent node'].tolist() or pd.isna(node['Parent node']):
             return False
         else:
             return True
     
@@ -1567,8 +1565,8 @@
         results = self.nodes.apply(lambda x: CHAIDRegressor._get_one_node_interaction(x, self.nodes), axis=1)
         results.index = self.nodes['Node']
         if result.lower() == 'dict':
             return dict(results)
         elif result.lower() == 'dataframe':
             return pd.DataFrame(results, columns=['Interaction'])
         else:
-            raise ValueError("Unknown result type. Possible values: 'dict' and 'DataFrame'.")
+            raise ValueError("Unknown result type. Possible values: 'dict' and 'DataFrame'.")
```

### Comparing `randan-0.2.1/randan/regression.py` & `randan-0.2.2/randan/regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,27 +340,25 @@
         phrase = 'method {}'
         
         print('\nLINEAR REGRESSION SUMMARY')
         print('------------------\n')
         print('Model summary')
         display(self.summary_r2().style\
                     .set_caption(phrase.format('.summary_r2()'))\
-                    .set_precision(n_decimals))
+                    .format(precision=n_decimals))
         print('------------------\n')
         print('ANOVA')
         display(self.summary_F().style\
-                    .format(None, na_rep="")\
-                    .set_caption(phrase.format('.summary_F()'))\
-                    .set_precision(n_decimals))
+                    .format(None, na_rep="", precision=n_decimals)\
+                    .set_caption(phrase.format('.summary_F()')))
         print('------------------\n')
         print('Coefficients')
         display(self.summary().style\
-                    .format(None, na_rep="")\
-                    .set_caption(phrase.format('.summary()'))\
-                    .set_precision(n_decimals))
+                    .format(None, na_rep="", precision=n_decimals)\
+                    .set_caption(phrase.format('.summary()')))
     
     def summary(self):
         """
         Summary table with requested information related to regression coefficients.
 
         Returns
         -------
@@ -1012,31 +1010,30 @@
         print('Dependent variable encoding')
         display(self.get_dependent_variable_codes().style\
                     .set_caption(phrase.format('.get_dependent_variable_codes()')))
         print('------------------\n')
         print('Model summary')
         display(self.summary_r2().style\
                     .set_caption(phrase.format('.summary_r2()'))\
-                    .set_precision(n_decimals))
+                    .format(precision=n_decimals))
         print('------------------\n')
         print('Classification table')
         display(self.get_classification_table().style\
                     .set_caption(phrase.format('.get_classification_table()'))\
-                    .set_precision(n_decimals))
+                    .format(precision=n_decimals))
         print('------------------\n')
         print('Precision and recall')
         display(self.get_precision_and_recall().style\
                     .set_caption(phrase.format('.get_precision_and_recall()'))\
-                    .set_precision(n_decimals))
+                    .format(precision=n_decimals))
         print('------------------\n')
         print('Coefficients')
         display(self.summary().style\
-                    .format(None, na_rep="")\
-                    .set_caption(phrase.format('.summary()'))\
-                    .set_precision(n_decimals))
+                    .format(None, na_rep="", precision=n_decimals)\
+                    .set_caption(phrase.format('.summary()')))
         
     def summary_r2(self):
         """
         Summary table with information related to pseudo coefficients of determination.
 
         Returns
         -------
@@ -1352,8 +1349,8 @@
         result = pd.concat(result, axis=1)
         
         result = result[columns_to_show].copy()
             
         if add_to_data:
             result = pd.concat([self._data, result], axis=1)
             
-        return result
+        return result
```

### Comparing `randan-0.2.1/randan/clustering.py` & `randan-0.2.2/randan/clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,38 +154,34 @@
             print(f'Estimation was succesfully converged in {self.n_iters} iterations.')
         else:
             print('Estimation was NOT converged successfully.')
             print('Please enlarge the number of iterations.')
         print('------------------\n')
         print('Final cluster centers')
         display(self.get_cluster_centers(round_discrete=True).style\
-                    .format(None, na_rep="")\
-                    .set_caption(phrase.format('.get_cluster_centers()'))\
-                    .set_precision(n_decimals))
+                    .format(None, na_rep="", precision=n_decimals)\
+                    .set_caption(phrase.format('.get_cluster_centers()')))
         if self._integer_type_vars != []:
             print("""Cluster centers for discrete variables are rounded for better interpretability.
 To see the exact centers, use [model].get_cluster_centers(round_discrete=False)""")
         print('------------------\n')
         print('Distances between centers')
         display(self.get_distances_between_centers().style\
-                    .format(None, na_rep="")\
-                    .set_caption(phrase.format('.get_distances_between_centers()'))\
-                    .set_precision(n_decimals))
+                    .format(None, na_rep="", precision=n_decimals)\
+                    .set_caption(phrase.format('.get_distances_between_centers()')))
         print('------------------\n')
         print('ANOVA')
         display(self.get_ANOVA_table().style\
-                    .format(None, na_rep="")\
-                    .set_caption(phrase.format('.get_ANOVA_table()'))\
-                    .set_precision(n_decimals))
+                    .format(None, na_rep="", precision=n_decimals)\
+                    .set_caption(phrase.format('.get_ANOVA_table()')))
         print('------------------\n')
         print('Cluster membership')
         display(self.get_number_of_cases_by_clusters().style\
-                    .format(None, na_rep="")\
-                    .set_caption(phrase.format('.get_number_of_cases_by_clusters()'))\
-                    .set_precision(n_decimals))
+                    .format(None, na_rep="", precision=n_decimals)\
+                    .set_caption(phrase.format('.get_number_of_cases_by_clusters()')))
 
     
     def get_cluster_centers(self, round_discrete=False):
         """
         Get the dataframe with cluster centers (means of each variable within clusters).
         
         Parameters
@@ -433,8 +429,8 @@
         plt.scatter([silh_score], [0.1], c='black', zorder=2)
         plt.annotate(round(silh_score, 2), (silh_score+0.01, 0.1+0.01))
         plt.annotate('Poor', (0.07, 0.01))
         plt.annotate('Fair', (0.37, 0.01))
         plt.annotate('Good', (0.85, 0.01))
         plt.yticks([])
         plt.title('Solution quality')
-        plt.show();
+        plt.show();
```

### Comparing `randan-0.2.1/randan/comparison_of_central_tendency.py` & `randan-0.2.2/randan/comparison_of_central_tendency.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,25 +151,24 @@
             Number of digits to round results when showing them
         """
 
         
         print('\nANOVA SUMMARY')
         print('------------------')
         display(self.summary().style\
-                    .format(None, na_rep="")\
-                    .set_caption("method .summary()")\
-                    .set_precision(n_decimals))
+                    .format(None, na_rep="", precision=n_decimals)\
+                    .set_caption("method .summary()"))
         
     def _perform_anova_for_several_variables(self):
         summary = pd.DataFrame(
             columns = ['Sum of Squares', 'df', 'Mean Square', 'F', 'p-value']
         )
         
         for var in self._dependent_variables:
             aux_model = ANOVA(self._data, var, self._independent_variable, show_results=False)
             aux_model_summary = aux_model.summary()
             aux_model_summary.index = [f'{var}: {res}' for res in ['Between Groups', 'Within Groups', 'Total']]
 #             aux_model_summary.index = pd.MultiIndex.from_product([[var]*3,
 #                                                     ['Between Groups', 'Within Groups', 'Total']])
             summary = pd.concat([summary, aux_model_summary])
             
-        return summary 
+        return summary
```

### Comparing `randan-0.2.1/randan/utils.py` & `randan-0.2.2/randan/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -111,8 +111,8 @@
         else:
             f1 = 0
         results.append([precision, recall, f1])
     results = pd.DataFrame(results, 
                             index=categories, 
                             columns = ['Precision', 'Recall', 'F score'])
     results.loc['Mean'] = results.mean()
-    return results
+    return results
```

### Comparing `randan-0.2.1/randan/descriptive_statistics.py` & `randan-0.2.2/randan/descriptive_statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,17 +63,16 @@
         ----------
         n_decimals : int
             Number of digits to round results when showing them
         """
         print('\nNOMINAL STATISTICS SUMMARY')
         print('------------------\n')
         display(self.summary().style\
-                    .format(None, na_rep="")\
-                    .set_caption("method .summary()")\
-                    .set_precision(n_decimals))
+                    .format(None, na_rep="", precision=n_decimals)\
+                    .set_caption("method .summary()"))
         if len(self._mult_modes) > 0:
             vars_ = ', '.join(self._mult_modes)
             print(f'Following variables have multiple modes: {vars_}')
     
     def show_frequencies(self, n_decimals=3):
         """
         Show frequency tables.
@@ -84,17 +83,16 @@
             Number of digits to round results when showing them
         """
         print('\nFREQUENCIES')
         for var in self._variables:
             print('------------------\n')
             print(f'variable: {var}')
             display(self.frequencies()[var].style\
-                        .format(None, na_rep="")\
-                        .set_caption(f"method .frequencies()['{var}']")\
-                        .set_precision(n_decimals))
+                        .format(None, na_rep="", precision=n_decimals)\
+                        .set_caption(f"method .frequencies()['{var}']"))
     
     def _get_statistics(self):
         measures = {}
         self._mult_modes = []
         for var in self._variables:
             ser = self._data[var]
             n = len(ser.dropna())
@@ -230,17 +228,16 @@
         ----------
         n_decimals : int
             Number of digits to round results when showing them
         """
         print('\nORDINAL STATISTICS SUMMARY')
         print('------------------\n')
         display(self.summary().style\
-                    .format(None, na_rep="")\
-                    .set_caption("method .summary()")\
-                    .set_precision(n_decimals))
+                    .format(None, na_rep="", precision=n_decimals)\
+                    .set_caption("method .summary()"))
         if len(self._mult_modes) > 0:
             vars_ = ', '.join(self._mult_modes)
             print(f'Following variables have multiple modes: {vars_}')
     
     def show_frequencies(self, n_decimals=3):
         """
         Show frequency tables.
@@ -251,17 +248,16 @@
             Number of digits to round results when showing them
         """
         print('\nFREQUENCIES')
         for var in self._variables:
             print('------------------\n')
             print(f'variable: {var}')
             display(self.frequencies()[var].style\
-                        .format(None, na_rep="")\
-                        .set_caption(f"method .frequencies()['{var}']")\
-                        .set_precision(n_decimals))
+                        .format(None, na_rep="", precision=n_decimals)\
+                        .set_caption(f"method .frequencies()['{var}']"))
     
     def _get_statistics(self):
         measures = {}
         self._mult_modes = []
         for var in self._variables:
             ser = self._data[var]
             n = len(ser.dropna())
@@ -451,17 +447,16 @@
         ----------
         n_decimals : int 
         Number of digits to round results when showing them
         """
         print('\nNORMALITY TESTS')
         print('------------------\n')
         display(self.normality_test(self.normality_test_type).style\
-                    .format(None, na_rep="")\
-                    .set_caption(f"method .normality_test(test_type='{self.normality_test_type}')")\
-                    .set_precision(n_decimals))
+                    .format(None, na_rep="", precision=n_decimals)\
+                    .set_caption(f"method .normality_test(test_type='{self.normality_test_type}')"))
     
     def _get_mappers_for_nonumerical_vars(self):
         nonnum_vars = [var for var in self._variables if not is_numeric_dtype(self._data[var])]
         mappers = {}
         for var in nonnum_vars:
             mappers.update({var: ScaleStatistics._get_mappers_for_one_var(self._data[var])})
         return mappers
@@ -482,17 +477,16 @@
         ----------
         n_decimals : int
             Number of digits to round results when showing them
         """
         print('\nSCALE STATISTICS SUMMARY')
         print('------------------\n')
         display(self.summary().style\
-                    .format(None, na_rep="")\
-                    .set_caption("method .summary()")\
-                    .set_precision(n_decimals))
+                    .format(None, na_rep="", precision=n_decimals)\
+                    .set_caption("method .summary()"))
         if len(self._mult_modes) > 0:
             vars_ = ', '.join(self._mult_modes)
             print(f'Following variables have multiple modes: {vars_}')
     
     def show_frequencies(self, n_decimals=3):
         """
         Show frequency tables.
@@ -503,17 +497,16 @@
             Number of digits to round results when showing them
         """
         print('\nFREQUENCIES')
         for var in self._variables:
             print('------------------\n')
             print(f'variable: {var}')
             display(self.frequencies()[var].style\
-                        .format(None, na_rep="")\
-                        .set_caption(f"method .frequencies()['{var}']")\
-                        .set_precision(n_decimals))
+                        .format(None, na_rep="", precision=n_decimals)\
+                        .set_caption(f"method .frequencies()['{var}']"))
     
     def _get_statistics(self):
         measures = {}
         self._mult_modes = []
         for var in self._variables:
             ser = self._data[var]
             n = len(ser.dropna())
```

### Comparing `randan-0.2.1/randan/bivariate_association.py` & `randan-0.2.2/randan/bivariate_association.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,32 +229,29 @@
         
         sig_level = self.sig_level
         
         print('\nCROSSTAB SUMMARY')
         print('------------------\n')
         print('Observed frequencies')
         display(self.frequencies_observed.style\
-                    .format(None, na_rep="")\
-                    .set_caption("attribute .frequencies_observed")\
-                    .set_precision(n_decimals))
+                    .format(None, na_rep="", precision=n_decimals)\
+                    .set_caption("attribute .frequencies_observed"))
         print('------------------\n')
         print('Expected frequencies')
         display(self.frequencies_expected.style\
-                    .format(None, na_rep="")\
-                    .set_caption("attribute .frequencies_expected")\
-                    .set_precision(n_decimals))        
+                    .format(None, na_rep="", precision=n_decimals)\
+                    .set_caption("attribute .frequencies_expected"))
         self.check_small_counts(n_decimals)
         print('------------------\n')
         print(f'Chi-square statistic is {round(self.chi_square, n_decimals)} (p-value = {round(self.pvalue, n_decimals)}).')
         print('------------------\n')
         print("Pearson's residuals")
         display(self.residuals_pearson.style\
-                    .format(None, na_rep="")\
-                    .set_caption("attribute .residuals_pearson")\
-                    .set_precision(n_decimals))
+                    .format(None, na_rep="", precision=n_decimals)\
+                    .set_caption("attribute .residuals_pearson"))
         self.check_significant_residuals(sig_level, n_decimals)
 
 #todo: flag significant, pairwise deletion
 
 class Correlation:
     """
     
@@ -388,17 +385,16 @@
         if len(self._non_num_vars) > 0:
             phrase = 'The following variables were removed from the analysis since they do not belong to numerical dtypes: {}\n'
             print(phrase.format(', '.join(self._non_num_vars)))
         if len(self._zero_var_vars) > 0:
             phrase = 'The following variables were removed from the analysis since they have zero variance: {}\n'
             print(phrase.format(', '.join(self._zero_var_vars)))
         display(self.correlation_matrix.style\
-                    .format(None, na_rep="")\
-                    .set_caption("attribute .correlation_matrix")\
-                    .set_precision(n_decimals))
+                    .format(None, na_rep="", precision=n_decimals)\
+                    .set_caption("attribute .correlation_matrix"))
         if min_max:
             results = self.sort_correlations()
             self.min_corr = results['Coefficient'].min()
             idxmin = results['Coefficient'].idxmin()
             min_pval = round(results.loc[idxmin, 'p-value'], n_decimals)
             self.max_corr = results['Coefficient'].max()
             idxmax = results['Coefficient'].idxmax()
```

### Comparing `randan-0.2.1/setup.py` & `randan-0.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="randan", # Replace with your own username
-    version="0.2.1",
+    version="0.2.2",
     author="Aleksei Rotmistrov, Svetlana Zhuchkova",
     author_email="alexey.n.rotmistrov@gmail.com, lana_lob@mail.ru",
     description="A python package for the analysis of social data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LanaLob/randan",
     packages=setuptools.find_packages(),
```

