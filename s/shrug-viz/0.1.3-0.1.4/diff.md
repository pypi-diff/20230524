# Comparing `tmp/shrug_viz-0.1.3.tar.gz` & `tmp/shrug_viz-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shrug_viz-0.1.3.tar", last modified: Wed May 24 11:07:28 2023, max compression
+gzip compressed data, was "shrug_viz-0.1.4.tar", last modified: Wed May 24 11:23:59 2023, max compression
```

## Comparing `shrug_viz-0.1.3.tar` & `shrug_viz-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 11:07:28.908110 shrug_viz-0.1.3/
--rw-rw-rw-   0        0        0       36 2023-05-24 10:51:15.000000 shrug_viz-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      418 2023-05-24 11:07:28.908110 shrug_viz-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-24 11:07:28.908110 shrug_viz-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      718 2023-05-24 11:06:33.000000 shrug_viz-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 11:07:28.686424 shrug_viz-0.1.3/shrug_viz/
--rw-rw-rw-   0        0        0      508 2023-05-24 11:06:16.000000 shrug_viz-0.1.3/shrug_viz/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 11:07:28.686424 shrug_viz-0.1.3/shrug_viz/data/
-drwxrwxrwx   0        0        0        0 2023-05-24 11:07:28.717858 shrug_viz-0.1.3/shrug_viz/data/keys/
--rw-rw-rw-   0        0        0 41016362 2022-11-09 10:04:36.000000 shrug_viz-0.1.3/shrug_viz/data/keys/shrug_names.csv
-drwxrwxrwx   0        0        0        0 2023-05-24 11:07:28.828544 shrug_viz-0.1.3/shrug_viz/data/shrug-v1.5.samosa-keys-csv/
--rw-rw-rw-   0        0        0 32111026 2022-11-07 11:49:14.000000 shrug_viz-0.1.3/shrug_viz/data/shrug-v1.5.samosa-keys-csv/shrug_pc11_district_key.csv
--rw-rw-rw-   0        0        0    12426 2023-05-24 10:36:43.000000 shrug_viz-0.1.3/shrug_viz/shrug_viz.py
-drwxrwxrwx   0        0        0        0 2023-05-24 11:07:28.717858 shrug_viz-0.1.3/shrug_viz.egg-info/
--rw-rw-rw-   0        0        0      418 2023-05-24 11:07:28.000000 shrug_viz-0.1.3/shrug_viz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-05-24 11:07:28.000000 shrug_viz-0.1.3/shrug_viz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 11:07:28.000000 shrug_viz-0.1.3/shrug_viz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-24 11:07:28.000000 shrug_viz-0.1.3/shrug_viz.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-24 11:07:28.000000 shrug_viz-0.1.3/shrug_viz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 11:23:59.277375 shrug_viz-0.1.4/
+-rw-rw-rw-   0        0        0       36 2023-05-24 10:51:15.000000 shrug_viz-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      418 2023-05-24 11:23:59.277375 shrug_viz-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-24 11:23:59.277375 shrug_viz-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      742 2023-05-24 11:22:46.000000 shrug_viz-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 11:23:59.012280 shrug_viz-0.1.4/shrug_viz/
+-rw-rw-rw-   0        0        0      508 2023-05-24 11:06:16.000000 shrug_viz-0.1.4/shrug_viz/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 11:23:59.012280 shrug_viz-0.1.4/shrug_viz/data/
+drwxrwxrwx   0        0        0        0 2023-05-24 11:23:59.058563 shrug_viz-0.1.4/shrug_viz/data/keys/
+-rw-rw-rw-   0        0        0 41016362 2022-11-09 10:04:36.000000 shrug_viz-0.1.4/shrug_viz/data/keys/shrug_names.csv
+drwxrwxrwx   0        0        0        0 2023-05-24 11:23:59.183600 shrug_viz-0.1.4/shrug_viz/data/shrug-v1.5.samosa-keys-csv/
+-rw-rw-rw-   0        0        0 32111026 2022-11-07 11:49:14.000000 shrug_viz-0.1.4/shrug_viz/data/shrug-v1.5.samosa-keys-csv/shrug_pc11_district_key.csv
+-rw-rw-rw-   0        0        0    12762 2023-05-24 11:20:35.000000 shrug_viz-0.1.4/shrug_viz/shrug_viz.py
+drwxrwxrwx   0        0        0        0 2023-05-24 11:23:59.058563 shrug_viz-0.1.4/shrug_viz.egg-info/
+-rw-rw-rw-   0        0        0      418 2023-05-24 11:23:58.000000 shrug_viz-0.1.4/shrug_viz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-05-24 11:23:58.000000 shrug_viz-0.1.4/shrug_viz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 11:23:58.000000 shrug_viz-0.1.4/shrug_viz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-05-24 11:23:58.000000 shrug_viz-0.1.4/shrug_viz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-24 11:23:58.000000 shrug_viz-0.1.4/shrug_viz.egg-info/top_level.txt
```

### Comparing `shrug_viz-0.1.3/setup.py` & `shrug_viz-0.1.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 
 
 # In[1]:
 
 
 setup(
     name='shrug_viz',
-    version='0.1.3',
+    version='0.1.4',
     author='Kashmira L, Maithili K, Vibhuti D, Pradnya K',
     author_email='kashmira.lodha@cumminscollege.in, pradnya.kanale@cumminscollege.in, vibhuti.dhande@cumminscollege.in, maithili.karlekar@cumminscollege.in',
     description='Choropleth visualization for SHRUG data platform (SAMOSA version)',
     packages=find_packages(),
     install_requires=[
         'pandas',
         'plotly',
         'numpy',
         'jellyfish',
         'matplotlib',
         'geopandas',
+        'pkg_resources'
     ],
     include_package_data=True,
     package_data={'': ['data/*']},
 )
 
 
 # In[ ]:
```

### Comparing `shrug_viz-0.1.3/shrug_viz/data/keys/shrug_names.csv` & `shrug_viz-0.1.4/shrug_viz/data/keys/shrug_names.csv`

 * *Files identical despite different names*

### Comparing `shrug_viz-0.1.3/shrug_viz/data/shrug-v1.5.samosa-keys-csv/shrug_pc11_district_key.csv` & `shrug_viz-0.1.4/shrug_viz/data/shrug-v1.5.samosa-keys-csv/shrug_pc11_district_key.csv`

 * *Files identical despite different names*

### Comparing `shrug_viz-0.1.3/shrug_viz/shrug_viz.py` & `shrug_viz-0.1.4/shrug_viz/shrug_viz.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-# In[1]:
+# In[2]:
 
 
 import pandas as pd
 import plotly.express as px
 import numpy as np
 import os
 import jellyfish
 import matplotlib.pyplot as plt
 import geopandas as gpd
 import plotly.express as px
 import plotly.io as pio
 
 
-# In[2]:
+# In[3]:
 
 
 def csv_to_df(file_path):
     """
     Read in a CSV file and return a pandas DataFrame.
     
     Args:
@@ -35,15 +35,15 @@
         print("File not found: {}".format(file_path))
         return None
     except:
         print("Error reading file: {}".format(file_path))
         return None
 
 
-# In[3]:
+# In[4]:
 
 
 def get_column_names(df):
     """
     Returns a list of column names in the given dataframe.
 
     Parameters:
@@ -55,15 +55,15 @@
     --------
     list
         A list of column names in the given dataframe.
     """
     print(list(df.columns))
 
 
-# In[4]:
+# In[5]:
 
 
 def read_shp(file_path):
     """
     Read in a shapefile and return a GeoDataFrame.
     
     Args:
@@ -79,15 +79,15 @@
         print("File not found: {}".format(file_path))
         return None
     except:
         print("Error reading file: {}".format(file_path))
         return None
 
 
-# In[5]:
+# In[6]:
 
 
 def get_key_from_value(my_dict, value):
     """
     Return the key in a dictionary that corresponds to a given value.
 
     Args:
@@ -99,15 +99,15 @@
     """
     for k, v in my_dict.items():
         if v == value:
             return k
         
 
 
-# In[6]:
+# In[7]:
 
 
 def get_state_map():
     
     
     """
     Retrieves a dictionary mapping state IDs to state names.
@@ -115,55 +115,61 @@
     Returns:
         state_map (dict): Dictionary mapping state IDs to state names.
     """
         
     id_name = 'shrid'
     state_variable ='state_name'
     latest_year='11-'
-    
-    keys = pd.read_csv("data/keys/shrug_names.csv")
+    import pkg_resources
+
+    filepath = pkg_resources.resource_filename('shrug_viz', 'data/keys/shrug_names.csv')
+
+    keys = pd.read_csv(filepath)
     keys=keys[[id_name,state_variable]]
     keys[id_name] = keys.shrid.str[0:5]
     keys=keys[keys[id_name].str.contains(latest_year)]
     keys[id_name] = keys.shrid.str[3:5]
     keys = keys.drop_duplicates()
     keys.dropna(inplace=True)
     keys[id_name]=keys[id_name].astype(str)
     state_map = keys.set_index(id_name)[state_variable].to_dict()
     return state_map
 
 
-# In[7]:
+# In[8]:
 
 
 def get_district_map():
     """
     Retrieves a dictionary mapping district IDs to district names.
 
     Returns:
         district_map (dict): Dictionary mapping district IDs to district names.
     """
     district_id = 'pc11_district_id'
     district_name = 'pc11_district_name'
-    
-    keys = pd.read_csv("data/shrug-v1.5.samosa-keys-csv/shrug_pc11_district_key.csv")
+    import pkg_resources
+
+    filepath = pkg_resources.resource_filename('shrug_viz',"data/shrug-v1.5.samosa-keys-csv/shrug_pc11_district_key.csv")
+
+    keys = pd.read_csv(filepath)
     keys=keys[[ district_id,district_name]]
     keys = keys.drop_duplicates()
     keys.dropna(inplace=True)
     keys[district_id]=keys[district_id].astype(int)
     keys[district_id]=keys[district_id].astype(str)
     district_map = keys.set_index(district_id)[district_name].to_dict()
     for k,v in district_map.items():
         k = str(k)
         district_map[k]=v
     return district_map
 
 
 
-# In[8]:
+# In[9]:
 
 
 def get_agg_map():
     """
     Retrieves a dictionary mapping variable names to aggregation functions.
 
     Returns:
@@ -181,15 +187,15 @@
     df=df[[column_name_variable,column_name_function]]
     agg_map = df.set_index(column_name_variable)[column_name_function].to_dict()
     for (k,v) in agg_map.items():
         agg_map[k] = agg_map[k].lower()
     return agg_map
 
 
-# In[9]:
+# In[10]:
 
 
 def get_state_names():
     """
     Gets a list of state names from the state_map dictionary.
 
     Returns:
@@ -198,41 +204,44 @@
     state_map=get_state_map()
     state_list=[]
     for k,v in state_map.items():
         state_list.append(v)
     return state_list
 
 
-# In[16]:
+# In[11]:
 
 
 def get_district_names(state_name='Maharashtra'):
     """
     Given a state name, returns a list of all district names within that state. 
     
     Args:
     state_name (str): Name of the state for which district names are to be returned.
     
     Returns:
     list: A list of strings, where each string represents a district name within the specified state.
     """
     state_variable ='state_name'
     district_variable = 'district_name'
-    
-    keys = csv_to_df("data/keys/shrug_names.csv")
+    import pkg_resources
+
+    filepath = pkg_resources.resource_filename('shrug_viz', 'data/keys/shrug_names.csv')
+
+    keys = pd.read_csv(filepath)
     keys =keys[keys[state_variable]==state_name]
     keys = keys[[district_variable]]
     district_names = keys[district_variable].unique()
     print(district_names)
 
     
     
 
 
-# In[11]:
+# In[12]:
 
 
 def shp_corrections(shapefile, dataframe, granularity):
     """
     This function corrects the mismatch between the names of the locations in the shapefile and the data frame.
     
     Parameters:
@@ -269,15 +278,15 @@
         matches.append(best_location)
         
     shapefile[new_str] = matches
     shapefile = shapefile[['geometry',new_str]]
     return shapefile
 
 
-# In[12]:
+# In[13]:
 
 
 def c_plot(merged_df, column_name, gb_str):
     """
     Plots a choropleth map based on a given column in a GeoDataFrame.
 
     Parameters:
@@ -310,15 +319,15 @@
     coloraxis_colorbar={
         'title':column_name})
 
     fig.show()
     return
 
 
-# In[13]:
+# In[14]:
 
 
 def choropleth(df=None, column_name=None, granularity='state', state_name='Maharashtra', district_name='aurangabad',shapefile_path=None):
     """
     Creates a choropleth map using the provided dataframe, column name, and granularity.
 
     Args:
@@ -344,15 +353,19 @@
     shapefile_col_name_district = 'pc11_d_id'
     granularity = granularity
     
     #shapefile
     #shapefile_path = os.path.join('data/shapefiles', granularity+'.shp')
     shapefile = read_shp(shapefile_path)
     #keys dataframe
-    keys_path = os.path.join('data/keys','shrug_names.csv')
+    import pkg_resources
+
+    keys_path = pkg_resources.resource_filename('shrug_viz', 'data/keys/shrug_names.csv')
+
+
     keys = csv_to_df(keys_path)
     
     #aggregation_function
     aggregation_map =get_agg_map()
     agg_func = aggregation_map[column_name]
     
     gb_str = granularity+"_name"
```

