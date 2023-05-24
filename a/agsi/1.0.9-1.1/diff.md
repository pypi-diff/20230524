# Comparing `tmp/agsi-1.0.9.tar.gz` & `tmp/agsi-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agsi-1.0.9.tar", last modified: Fri May 19 09:54:09 2023, max compression
+gzip compressed data, was "agsi-1.1.tar", last modified: Wed May 24 10:24:00 2023, max compression
```

## Comparing `agsi-1.0.9.tar` & `agsi-1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-19 09:54:09.587170 agsi-1.0.9/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       56 2023-05-17 09:39:46.000000 agsi-1.0.9/.gitignore
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      214 2023-05-19 09:54:09.587170 agsi-1.0.9/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     2077 2023-05-17 09:13:44.000000 agsi-1.0.9/README.md
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-19 09:54:09.587170 agsi-1.0.9/agsi/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-17 09:19:23.000000 agsi-1.0.9/agsi/__init__.py
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-19 09:54:09.587170 agsi-1.0.9/agsi/data/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)    14206 2023-05-19 09:52:33.000000 agsi-1.0.9/agsi/data/FarmData.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:16:41.000000 agsi-1.0.9/agsi/data/__init__.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     5980 2023-05-17 09:13:44.000000 agsi-1.0.9/agsi/data/utils.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)   931124 2023-05-19 09:52:59.000000 agsi-1.0.9/agsi/demo_V2.ipynb
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-17 09:13:44.000000 agsi-1.0.9/agsi/main.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-17 09:13:44.000000 agsi-1.0.9/agsi/requirements.txt
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-19 09:54:09.587170 agsi-1.0.9/agsi.egg-info/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      214 2023-05-19 09:54:09.000000 agsi-1.0.9/agsi.egg-info/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-05-19 09:54:09.000000 agsi-1.0.9/agsi.egg-info/SOURCES.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-19 09:54:09.000000 agsi-1.0.9/agsi.egg-info/dependency_links.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-19 09:54:09.000000 agsi-1.0.9/agsi.egg-info/requires.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-05-19 09:54:09.000000 agsi-1.0.9/agsi.egg-info/top_level.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-19 09:54:09.587170 agsi-1.0.9/setup.cfg
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      369 2023-05-19 09:54:05.000000 agsi-1.0.9/setup.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-24 10:24:00.176120 agsi-1.1/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       71 2023-05-24 10:23:11.000000 agsi-1.1/.gitignore
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-05-24 10:24:00.176120 agsi-1.1/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     2077 2023-05-17 09:13:44.000000 agsi-1.1/README.md
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-24 10:24:00.176120 agsi-1.1/agsi/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-17 09:19:23.000000 agsi-1.1/agsi/__init__.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-24 10:24:00.176120 agsi-1.1/agsi/data/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)    14628 2023-05-24 10:22:28.000000 agsi-1.1/agsi/data/FarmData.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:16:41.000000 agsi-1.1/agsi/data/__init__.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     5980 2023-05-17 09:13:44.000000 agsi-1.1/agsi/data/utils.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)   931124 2023-05-19 09:52:59.000000 agsi-1.1/agsi/demo_V2.ipynb
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-17 09:13:44.000000 agsi-1.1/agsi/main.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-17 09:13:44.000000 agsi-1.1/agsi/requirements.txt
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-24 10:24:00.176120 agsi-1.1/agsi.egg-info/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-05-24 10:24:00.000000 agsi-1.1/agsi.egg-info/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-05-24 10:24:00.000000 agsi-1.1/agsi.egg-info/SOURCES.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-24 10:24:00.000000 agsi-1.1/agsi.egg-info/dependency_links.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-24 10:24:00.000000 agsi-1.1/agsi.egg-info/requires.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-05-24 10:24:00.000000 agsi-1.1/agsi.egg-info/top_level.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-24 10:24:00.176120 agsi-1.1/setup.cfg
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      367 2023-05-24 10:22:52.000000 agsi-1.1/setup.py
```

### Comparing `agsi-1.0.9/README.md` & `agsi-1.1/README.md`

 * *Files identical despite different names*

### Comparing `agsi-1.0.9/agsi/data/FarmData.py` & `agsi-1.1/agsi/data/FarmData.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,15 @@
                 block_id = row['block_id']
                 farm_id = row['farm_id']
                 block_name = row['block_name']
                 vegetation_type = row['vegetation_type']
                 crop_name = row['crop_name']
                 yield_val = row['yield']
                 shp_val = row['shp']
+                time=row['timestamp']
 
                 # Extract drone image paths or shp files
                 data_path = {}
                 for key in row.keys():
                     if key.startswith('drone_'):
                         if row[key]:
                             data_path[key] = row[key]
@@ -152,28 +153,39 @@
                     data_path['sat_planet'] = ""
 
                 if row['sat_sentinel2']:
                     data_path['sentinel_2'] =row['sat_sentinel2']
                 else:
                     data_path['sentinel_2'] =""
 
+
+
                 # Create output dictionary for block
                 block_dict = {
                     'block_id':block_id,
                     'farm_id' : farm_id,
                     'block_name': block_name,
                     'vegetation_type': vegetation_type,
                     'crop_name': crop_name,
                     'yield': yield_val,
                     'shp': shp_val,
-                    'data_path': data_path # Use dynamically generated drone data dictionary
+                    'data_path': data_path, # Use dynamically generated drone data dictionary
+                    'timestamps':[]
                 }
-                # Add block dictionary to output dictionary
-                output_dict[block_id] = block_dict
 
+
+                if block_id in output_dict:
+                   timestamp_list=output_dict[block_id]['timestamps']
+                   timestamp_list.append(time)
+                   timestamp_list=list(set(timestamp_list))
+                   output_dict[block_id]['timestamps']=timestamp_list
+                else:
+                   output_dict[block_id] = block_dict   
+                   output_dict[block_id]['timestamps'].append(time)
+                
             # Return output dictionary
         return output_dict
 
 class Farm():
 
   """
     A subclass of FarmData that represents farm-specific data.
```

### Comparing `agsi-1.0.9/agsi/data/utils.py` & `agsi-1.1/agsi/data/utils.py`

 * *Files identical despite different names*

### Comparing `agsi-1.0.9/agsi/demo_V2.ipynb` & `agsi-1.1/agsi/demo_V2.ipynb`

 * *Files identical despite different names*

