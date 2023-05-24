# Comparing `tmp/swspy-1.0.1.tar.gz` & `tmp/swspy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swspy-1.0.1.tar", last modified: Mon May 22 09:25:19 2023, max compression
+gzip compressed data, was "dist/swspy-1.0.2.tar", last modified: Wed May 24 14:33:43 2023, max compression
```

## Comparing `swspy-1.0.1.tar` & `swspy-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-22 09:25:19.000000 swspy-1.0.1/
--rw-r--r--   0 eart0504   (502) staff       (20)     1053 2021-08-25 10:24:55.000000 swspy-1.0.1/LICENSE
--rw-r--r--   0 eart0504   (502) staff       (20)     1447 2023-05-22 09:25:19.000000 swspy-1.0.1/PKG-INFO
--rw-r--r--   0 eart0504   (502) staff       (20)      896 2023-05-19 14:16:55.000000 swspy-1.0.1/README.md
--rw-r--r--   0 eart0504   (502) staff       (20)       38 2023-05-22 09:25:19.000000 swspy-1.0.1/setup.cfg
--rw-r--r--   0 eart0504   (502) staff       (20)      723 2023-05-22 09:23:25.000000 swspy-1.0.1/setup.py
-drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-22 09:25:19.000000 swspy-1.0.1/swspy/
--rw-r--r--   0 eart0504   (502) staff       (20)      436 2021-09-23 09:04:50.000000 swspy-1.0.1/swspy/__init__.py
-drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-22 09:25:19.000000 swspy-1.0.1/swspy/automate/
--rw-r--r--   0 eart0504   (502) staff       (20)      127 2021-09-23 09:03:55.000000 swspy-1.0.1/swspy/automate/__init__.py
--rw-r--r--   0 eart0504   (502) staff       (20)    15043 2023-05-19 14:05:48.000000 swspy-1.0.1/swspy/automate/automation_manager.py
-drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-22 09:25:19.000000 swspy-1.0.1/swspy/io/
--rw-r--r--   0 eart0504   (502) staff       (20)      168 2023-05-19 14:02:00.000000 swspy-1.0.1/swspy/io/__init__.py
--rw-r--r--   0 eart0504   (502) staff       (20)     8958 2023-05-19 14:06:58.000000 swspy-1.0.1/swspy/io/load.py
--rw-r--r--   0 eart0504   (502) staff       (20)     5115 2023-05-19 14:00:58.000000 swspy-1.0.1/swspy/io/read_nonlinloc.py
-drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-22 09:25:19.000000 swspy-1.0.1/swspy/splitting/
--rw-r--r--   0 eart0504   (502) staff       (20)      133 2023-04-04 15:14:25.000000 swspy-1.0.1/swspy/splitting/__init__.py
--rw-r--r--   0 eart0504   (502) staff       (20)     7008 2023-04-17 13:05:11.000000 swspy-1.0.1/swspy/splitting/forward_model.py
--rw-r--r--   0 eart0504   (502) staff       (20)   120925 2023-05-22 09:15:48.000000 swspy-1.0.1/swspy/splitting/split.py
-drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-22 09:25:19.000000 swspy-1.0.1/swspy.egg-info/
--rw-r--r--   0 eart0504   (502) staff       (20)     1447 2023-05-22 09:25:19.000000 swspy-1.0.1/swspy.egg-info/PKG-INFO
--rw-r--r--   0 eart0504   (502) staff       (20)      419 2023-05-22 09:25:19.000000 swspy-1.0.1/swspy.egg-info/SOURCES.txt
--rw-r--r--   0 eart0504   (502) staff       (20)        1 2023-05-22 09:25:19.000000 swspy-1.0.1/swspy.egg-info/dependency_links.txt
--rw-r--r--   0 eart0504   (502) staff       (20)        6 2023-05-22 09:25:19.000000 swspy-1.0.1/swspy.egg-info/top_level.txt
-drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-22 09:25:19.000000 swspy-1.0.1/tests/
--rw-r--r--   0 eart0504   (502) staff       (20)     1725 2023-05-15 11:18:33.000000 swspy-1.0.1/tests/test_notebooks.py
--rw-r--r--   0 eart0504   (502) staff       (20)     3208 2023-05-02 08:15:38.000000 swspy-1.0.1/tests/test_synth.py
+drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-24 14:33:43.000000 swspy-1.0.2/
+-rw-r--r--   0 eart0504   (502) staff       (20)     1053 2021-08-25 10:24:55.000000 swspy-1.0.2/LICENSE
+-rw-r--r--   0 eart0504   (502) staff       (20)     1447 2023-05-24 14:33:43.000000 swspy-1.0.2/PKG-INFO
+-rw-r--r--   0 eart0504   (502) staff       (20)      896 2023-05-19 14:16:55.000000 swspy-1.0.2/README.md
+-rw-r--r--   0 eart0504   (502) staff       (20)       38 2023-05-24 14:33:43.000000 swspy-1.0.2/setup.cfg
+-rw-r--r--   0 eart0504   (502) staff       (20)      948 2023-05-24 14:30:32.000000 swspy-1.0.2/setup.py
+drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-24 14:33:43.000000 swspy-1.0.2/swspy/
+-rw-r--r--   0 eart0504   (502) staff       (20)      458 2023-05-24 14:31:07.000000 swspy-1.0.2/swspy/__init__.py
+drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-24 14:33:43.000000 swspy-1.0.2/swspy/automate/
+-rw-r--r--   0 eart0504   (502) staff       (20)      127 2021-09-23 09:03:55.000000 swspy-1.0.2/swspy/automate/__init__.py
+-rw-r--r--   0 eart0504   (502) staff       (20)    15043 2023-05-19 14:05:48.000000 swspy-1.0.2/swspy/automate/automation_manager.py
+drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-24 14:33:43.000000 swspy-1.0.2/swspy/io/
+-rw-r--r--   0 eart0504   (502) staff       (20)      168 2023-05-19 14:02:00.000000 swspy-1.0.2/swspy/io/__init__.py
+-rw-r--r--   0 eart0504   (502) staff       (20)     8958 2023-05-19 14:06:58.000000 swspy-1.0.2/swspy/io/load.py
+-rw-r--r--   0 eart0504   (502) staff       (20)     5115 2023-05-19 14:00:58.000000 swspy-1.0.2/swspy/io/read_nonlinloc.py
+drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-24 14:33:43.000000 swspy-1.0.2/swspy/splitting/
+-rw-r--r--   0 eart0504   (502) staff       (20)      133 2023-04-04 15:14:25.000000 swspy-1.0.2/swspy/splitting/__init__.py
+-rw-r--r--   0 eart0504   (502) staff       (20)     7008 2023-04-17 13:05:11.000000 swspy-1.0.2/swspy/splitting/forward_model.py
+-rw-r--r--   0 eart0504   (502) staff       (20)   121191 2023-05-24 10:12:19.000000 swspy-1.0.2/swspy/splitting/split.py
+-rw-r--r--   0 eart0504   (502) staff       (20)     1322 2023-05-24 10:11:51.000000 swspy-1.0.2/swspy/testing.py
+drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-24 14:33:43.000000 swspy-1.0.2/swspy.egg-info/
+-rw-r--r--   0 eart0504   (502) staff       (20)     1447 2023-05-24 14:33:43.000000 swspy-1.0.2/swspy.egg-info/PKG-INFO
+-rw-r--r--   0 eart0504   (502) staff       (20)      464 2023-05-24 14:33:43.000000 swspy-1.0.2/swspy.egg-info/SOURCES.txt
+-rw-r--r--   0 eart0504   (502) staff       (20)        1 2023-05-24 14:33:43.000000 swspy-1.0.2/swspy.egg-info/dependency_links.txt
+-rw-r--r--   0 eart0504   (502) staff       (20)       91 2023-05-24 14:33:43.000000 swspy-1.0.2/swspy.egg-info/requires.txt
+-rw-r--r--   0 eart0504   (502) staff       (20)        6 2023-05-24 14:33:43.000000 swspy-1.0.2/swspy.egg-info/top_level.txt
+drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-24 14:33:43.000000 swspy-1.0.2/tests/
+-rw-r--r--   0 eart0504   (502) staff       (20)     1725 2023-05-15 11:18:33.000000 swspy-1.0.2/tests/test_notebooks.py
+-rw-r--r--   0 eart0504   (502) staff       (20)     3167 2023-05-24 10:11:51.000000 swspy-1.0.2/tests/test_synth.py
```

### Comparing `swspy-1.0.1/LICENSE` & `swspy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swspy-1.0.1/PKG-INFO` & `swspy-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swspy
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for automatically calculating shear wave splitting for large earthquake catalogues.
 Home-page: https://github.com/TomSHudson/swspy/
 Author: Tom Hudson
 Author-email: thomas.hudson@earth.ox.ac.uk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swspy-1.0.1/README.md` & `swspy-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `swspy-1.0.1/setup.py` & `swspy-1.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
+install_requires_list = []
+with open("requirements.txt") as file:
+    for line in file:
+        if not line.startswith("#"):
+            install_requires_list.append(line.rstrip())
 
 setuptools.setup(
     name="swspy",
-    version="1.0.1",
+    version="1.0.2",
     author="Tom Hudson",
     author_email="thomas.hudson@earth.ox.ac.uk",
     description="A package for automatically calculating shear wave splitting for large earthquake catalogues.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TomSHudson/swspy/",
     packages=setuptools.find_packages(),
     classifiers=[
         "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
+    install_requires=install_requires_list,
 )
```

### Comparing `swspy-1.0.1/swspy/automate/automation_manager.py` & `swspy-1.0.2/swspy/automate/automation_manager.py`

 * *Files identical despite different names*

### Comparing `swspy-1.0.1/swspy/io/load.py` & `swspy-1.0.2/swspy/io/load.py`

 * *Files identical despite different names*

### Comparing `swspy-1.0.1/swspy/io/read_nonlinloc.py` & `swspy-1.0.2/swspy/io/read_nonlinloc.py`

 * *Files identical despite different names*

### Comparing `swspy-1.0.1/swspy/splitting/forward_model.py` & `swspy-1.0.2/swspy/splitting/forward_model.py`

 * *Files identical despite different names*

### Comparing `swspy-1.0.1/swspy/splitting/split.py` & `swspy-1.0.2/swspy/splitting/split.py`

 * *Files 1% similar despite different names*

```diff
@@ -983,21 +983,21 @@
         else:
             arrival_time_curr = self.S_phase_arrival_times[station_idx_tmp]
         st_ZNE_curr.trim(starttime=arrival_time_curr - self.overall_win_start_pre_fast_S_pick,
                             endtime=arrival_time_curr + self.overall_win_start_post_fast_S_pick + self.max_t_shift_s)
 
         # 2. And remove splitting to get corrected waveforms:
         try:
-            phi_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['phi_from_Q'])
-            dt_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['dt'])
-            phi_err_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['phi_err'])
-            dt_err_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['dt_err'])
-            src_pol_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['src_pol_from_N'])
-            src_pol_err_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['src_pol_from_N_err'])
-            Q_w_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['Q_w'])
+            phi_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['phi_from_Q'].iloc[0])
+            dt_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['dt'].iloc[0])
+            phi_err_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['phi_err'].iloc[0])
+            dt_err_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['dt_err'].iloc[0])
+            src_pol_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['src_pol_from_N'].iloc[0])
+            src_pol_err_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['src_pol_from_N_err'].iloc[0])
+            Q_w_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['Q_w'].iloc[0])
         except TypeError:
             # If cannot get parameters becuase splitting clustering failed, skip station:
             raise CustomError("Cannot get splitting parameters because splitting clustering failed.")
         st_ZNE_curr_sws_corrected = remove_splitting(st_ZNE_curr, phi_curr, dt_curr, back_azi, event_inclin_angle_at_station,
                                                     return_BPA=True, src_pol=src_pol_curr) # (Note: Uses src_pol in horizontal direction, as calc. P and A from horizontal dir at the moment)
 
         return st_ZNE_curr, st_ZNE_curr_sws_corrected
@@ -1033,28 +1033,28 @@
         else:
             arrival_time_curr = self.S_phase_arrival_times[station_idx_tmp]
         st_ZNE_curr.trim(starttime=arrival_time_curr - self.overall_win_start_pre_fast_S_pick,
                             endtime=arrival_time_curr + self.overall_win_start_post_fast_S_pick + self.max_t_shift_s)
 
         # 2. And remove splitting to get corrected waveforms, post layer 2 correction:
         try:
-            phi_curr = float(self.sws_multi_layer_result_df.loc[self.sws_multi_layer_result_df['station'] == station]['phi2_from_Q'])
-            dt_curr = float(self.sws_multi_layer_result_df.loc[self.sws_multi_layer_result_df['station'] == station]['dt2'])
-            src_pol_curr = float(self.sws_multi_layer_result_df.loc[self.sws_multi_layer_result_df['station'] == station]['src_pol_from_N'])
+            phi_curr = float(self.sws_multi_layer_result_df.loc[self.sws_multi_layer_result_df['station'] == station]['phi2_from_Q'].iloc[0])
+            dt_curr = float(self.sws_multi_layer_result_df.loc[self.sws_multi_layer_result_df['station'] == station]['dt2'].iloc[0])
+            src_pol_curr = float(self.sws_multi_layer_result_df.loc[self.sws_multi_layer_result_df['station'] == station]['src_pol_from_N'].iloc[0])
         except TypeError:
             # If cannot get parameters becuase splitting clustering failed, skip station:
             raise CustomError("Cannot get splitting parameters because splitting clustering failed.")
         st_ZNE_curr_sws_corrected_layer_2 = remove_splitting(st_ZNE_curr, phi_curr, dt_curr, back_azi, event_inclin_angle_at_station,
                                                     return_BPA=True, src_pol=src_pol_curr) # (Note: Uses src_pol in horizontal direction, as calc. P and A from horizontal dir at the moment)
         
         # 3. And remove splitting to get corrected waveforms, post layer 1 correction:
         try:
-            phi_curr = float(self.sws_multi_layer_result_df.loc[self.sws_multi_layer_result_df['station'] == station]['phi1_from_Q'])
-            dt_curr = float(self.sws_multi_layer_result_df.loc[self.sws_multi_layer_result_df['station'] == station]['dt1'])
-            src_pol_curr = float(self.sws_multi_layer_result_df.loc[self.sws_multi_layer_result_df['station'] == station]['src_pol_from_N'])
+            phi_curr = float(self.sws_multi_layer_result_df.loc[self.sws_multi_layer_result_df['station'] == station]['phi1_from_Q'].iloc[0])
+            dt_curr = float(self.sws_multi_layer_result_df.loc[self.sws_multi_layer_result_df['station'] == station]['dt1'].iloc[0])
+            src_pol_curr = float(self.sws_multi_layer_result_df.loc[self.sws_multi_layer_result_df['station'] == station]['src_pol_from_N'].iloc[0])
         except TypeError:
             # If cannot get parameters becuase splitting clustering failed, skip station:
             raise CustomError("Cannot get splitting parameters because splitting clustering failed.")
         st_ZNE_curr_sws_corrected_layer_2_ZNE_only = obspy.Stream() # (Note: So that don't duplicate B,P,A,F,S components)
         st_ZNE_curr_sws_corrected_layer_2_ZNE_only.append(st_ZNE_curr_sws_corrected_layer_2.select(channel="??Z")[0])
         st_ZNE_curr_sws_corrected_layer_2_ZNE_only.append(st_ZNE_curr_sws_corrected_layer_2.select(channel="??N")[0])
         st_ZNE_curr_sws_corrected_layer_2_ZNE_only.append(st_ZNE_curr_sws_corrected_layer_2.select(channel="??E")[0])
@@ -1559,34 +1559,31 @@
                 ray_back_azi = np.nan
                 ray_inc_at_station = np.nan
             # And append data to result dfs:
             df_tmp = pd.DataFrame(data={'station': [station], 'phi1_from_Q': [opt_phi_layer1], 'phi1_from_N': [opt_phi_vec_layer1[0]], 'phi1_from_U': [opt_phi_vec_layer1[1]], 'phi1_err': [opt_phi_err_layer1], 'dt1': [opt_lag_layer1], 'dt1_err': [opt_lag_err_layer1], 
                                     'phi2_from_Q': [opt_phi_layer2], 'phi2_from_N': [opt_phi_vec_layer2[0]], 'phi2_from_U': [opt_phi_vec_layer2[1]], 'phi2_err': [opt_phi_err_layer2], 'dt2': [opt_lag_layer2], 'dt2_err': [opt_lag_err_layer2], 
                                         'src_pol_from_N': [src_pol_deg[0]], 'src_pol_from_U': [src_pol_deg[1]], 'src_pol_from_N_err': [src_pol_deg_err[0]], 'src_pol_from_U_err': [src_pol_deg_err[1]], 'Q_w' : [np.nan],  'lambda2/lambda1 ratio': [opt_eig_ratio],
                                          'lambda2/lambda1 ratio1': [opt_eig_ratio_layer1], 'lambda2/lambda1 ratio2': [opt_eig_ratio_layer2], 'ray_back_azi': [ray_back_azi], 'ray_inc': [ray_inc_at_station]})
-            self.sws_multi_layer_result_df = self.sws_multi_layer_result_df.append(df_tmp)
+            self.sws_multi_layer_result_df = pd.concat([self.sws_multi_layer_result_df, df_tmp])
             df_tmp = pd.DataFrame(data={'station': [station], 'phi_from_Q': [opt_phi_layer1], 'phi_from_N': [opt_phi_vec_layer1[0]], 'phi_from_U': [opt_phi_vec_layer1[1]], 'phi_err': [opt_phi_err_layer1], 'dt': [opt_lag_layer1], 'dt_err': [opt_lag_err_layer1], 
                                         'src_pol_from_N': [src_pol_deg[0]], 'src_pol_from_U': [src_pol_deg[1]], 'src_pol_from_N_err': [src_pol_deg_err[0]], 'src_pol_from_U_err': [src_pol_deg_err[1]], 'Q_w' : [np.nan],  'lambda2/lambda1 ratio': [opt_eig_ratio],
                                         'ray_back_azi': [ray_back_azi], 'ray_inc': [ray_inc_at_station]})
-            sws_result_df_out = sws_result_df_out.append(df_tmp)
+            self.sws_result_df = pd.concat([self.sws_result_df, df_tmp])
             try:
                 opt_phi_idx = np.where(self.phis_labels == opt_phi_layer1)[0][0]
                 opt_lag_idx = np.where(self.lags_labels == opt_lag_layer1)[0][0]
             except IndexError:
                 raise CustomError("Cannot find optimal phi or lag.")
             self.phi_dt_grid_average[station] = np.average(grid_search_results_all_win_EV_layer1, axis=0) # (lambda2 divided by lambda1 as in Wuestefeld2010 (most stable))
             self.phi_dt_grid_average_layer1[station] = np.average(grid_search_results_all_win_EV_layer1, axis=0) # (lambda2 divided by lambda1 as in Wuestefeld2010 (most stable))
             self.phi_dt_grid_average_layer2[station] = np.average(grid_search_results_all_win_EV_layer2, axis=0) # (lambda2 divided by lambda1 as in Wuestefeld2010 (most stable))
             self.event_station_win_idxs[station] = {}
             self.event_station_win_idxs[station]['win_start_idxs'] = win_start_idxs
             self.event_station_win_idxs[station]['win_end_idxs'] = win_end_idxs
 
-        # And update one output df:
-        self.sws_result_df = sws_result_df_out
-
         return self.sws_result_df, self.sws_multi_layer_result_df
 
 
     def plot(self, outdir=None, suppress_direct_plotting=False):
         """Function to perform plotting...
         """
         # Loop over stations, plotting:
@@ -1602,32 +1599,32 @@
             if self.sws_multi_layer_result_df is not None:
                 print("Passed multi-layer result, therefore plotting this result.")
                 # (Note: Get layer 2 correction, as intermediate stage correction, and layer 1+2 correction is full correction)
                 del st_ZNE_curr_sws_corrected
                 st_ZNE_curr, st_ZNE_curr_sws_corrected_layer_2, st_ZNE_curr_sws_corrected = self._get_uncorr_and_corr_waveforms_multi_layer(station)
             # Splitting parameters:
             try:
-                phi_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['phi_from_Q'])
-                phi_from_N_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['phi_from_N'])
-                dt_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['dt'])
-                phi_err_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['phi_err'])
-                dt_err_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['dt_err'])
-                src_pol_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['src_pol_from_N'])
-                src_pol_err_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['src_pol_from_N_err'])
-                Q_w_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['Q_w'])
-                opt_eig_ratio_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['lambda2/lambda1 ratio'])
+                phi_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['phi_from_Q'].iloc[0])
+                phi_from_N_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['phi_from_N'].iloc[0])
+                dt_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['dt'].iloc[0])
+                phi_err_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['phi_err'].iloc[0])
+                dt_err_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['dt_err'].iloc[0])
+                src_pol_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['src_pol_from_N'].iloc[0])
+                src_pol_err_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['src_pol_from_N_err'].iloc[0])
+                Q_w_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['Q_w'].iloc[0])
+                opt_eig_ratio_curr = float(self.sws_result_df.loc[self.sws_result_df['station'] == station]['lambda2/lambda1 ratio'].iloc[0])
                 if self.sws_multi_layer_result_df is not None:
-                    dt_layer1 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['dt1'])
-                    dt_err_layer1 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['dt1_err'])
-                    dt_layer2 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['dt2'])
-                    dt_err_layer2 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['dt2_err'])
-                    phi_layer1 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['phi1_from_N'])
-                    phi_err_layer1 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['phi1_err'])
-                    phi_layer2 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['phi2_from_N'])
-                    phi_err_layer2 = float(self.sws_multi_layer_result_df.loc[self.sws_result_df['station'] == station]['phi2_err'])
+                    dt_layer1 = float(self.sws_multi_layer_result_df.loc[self.sws_multi_layer_result_df['station'] == station]['dt1'].iloc[0])
+                    dt_err_layer1 = float(self.sws_multi_layer_result_df.loc[self.sws_multi_layer_result_df['station'] == station]['dt1_err'].iloc[0])
+                    dt_layer2 = float(self.sws_multi_layer_result_df.loc[self.sws_multi_layer_result_df['station'] == station]['dt2'].iloc[0])
+                    dt_err_layer2 = float(self.sws_multi_layer_result_df.loc[self.sws_multi_layer_result_df['station'] == station]['dt2_err'].iloc[0])
+                    phi_layer1 = float(self.sws_multi_layer_result_df.loc[self.sws_multi_layer_result_df['station'] == station]['phi1_from_N'].iloc[0])
+                    phi_err_layer1 = float(self.sws_multi_layer_result_df.loc[self.sws_multi_layer_result_df['station'] == station]['phi1_err'].iloc[0])
+                    phi_layer2 = float(self.sws_multi_layer_result_df.loc[self.sws_multi_layer_result_df['station'] == station]['phi2_from_N'].iloc[0])
+                    phi_err_layer2 = float(self.sws_multi_layer_result_df.loc[self.sws_multi_layer_result_df['station'] == station]['phi2_err'].iloc[0])
             except TypeError:
                 # If cannot get parameters becuase splitting clustering failed, skip station:
                 print("Cannot get splitting parameters because splitting clustering failed. Skipping station:", 
                         station)
                 continue
             # And get unncorrected P and A waveforms:
             tr_tmp_P = st_ZNE_curr.select(channel="??N")[0].copy()
```

### Comparing `swspy-1.0.1/swspy.egg-info/PKG-INFO` & `swspy-1.0.2/swspy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swspy
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for automatically calculating shear wave splitting for large earthquake catalogues.
 Home-page: https://github.com/TomSHudson/swspy/
 Author: Tom Hudson
 Author-email: thomas.hudson@earth.ox.ac.uk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swspy-1.0.1/tests/test_notebooks.py` & `swspy-1.0.2/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `swspy-1.0.1/tests/test_synth.py` & `swspy-1.0.2/tests/test_synth.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,13 +62,12 @@
     phi_N_res = splitting_event.sws_result_df['phi_from_N'].values[0]
     phi_err_res = splitting_event.sws_result_df['phi_err'].values[0]
     dt_res = splitting_event.sws_result_df['dt'].values[0]
     dt_err_res = splitting_event.sws_result_df['dt_err'].values[0]
     lam2_lam1 = splitting_event.sws_result_df['lambda2/lambda1 ratio'].values[0]
 
     assert(lam2_lam1 >= 0.0)
-    # What about 180 degree errors or around 0
-    numpy.testing.assert_allclose(phi_N, phi_N_res, rtol=0.0, atol=phi_err_res)
+    swspy.testing.assert_angle_allclose(phi_N, phi_N_res, rtol=0.0, atol=phi_err_res)
     numpy.testing.assert_allclose(dt, dt_res, rtol=0.0, atol=dt_err_res)
```

