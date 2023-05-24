# Comparing `tmp/mecoda-minka-1.0.1.tar.gz` & `tmp/mecoda-minka-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecoda-minka-1.0.1.tar", last modified: Thu Mar  2 15:27:10 2023, max compression
+gzip compressed data, was "mecoda-minka-1.1.0.tar", last modified: Wed May 24 11:48:01 2023, max compression
```

## Comparing `mecoda-minka-1.0.1.tar` & `mecoda-minka-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2023-03-02 15:27:10.916145 mecoda-minka-1.0.1/
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    11796 2023-03-02 15:27:10.916145 mecoda-minka-1.0.1/PKG-INFO
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     9006 2023-02-09 13:27:58.000000 mecoda-minka-1.0.1/README.md
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)       38 2023-03-02 15:27:10.916145 mecoda-minka-1.0.1/setup.cfg
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     1433 2023-03-02 15:25:17.000000 mecoda-minka-1.0.1/setup.py
-drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2023-03-02 15:27:10.912145 mecoda-minka-1.0.1/src/
-drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2023-03-02 15:27:10.912145 mecoda-minka-1.0.1/src/mecoda_minka/
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)      566 2022-12-22 16:17:43.000000 mecoda-minka-1.0.1/src/mecoda_minka/__init__.py
-drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2023-03-02 15:27:10.912145 mecoda-minka-1.0.1/src/mecoda_minka/data/
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)  4174945 2022-12-22 16:17:43.000000 mecoda-minka-1.0.1/src/mecoda_minka/data/taxon_tree.csv
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    15474 2023-03-02 14:43:28.000000 mecoda-minka-1.0.1/src/mecoda_minka/mecoda_minka.py
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     2148 2022-12-22 16:17:43.000000 mecoda-minka-1.0.1/src/mecoda_minka/models.py
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)        0 2022-12-22 16:17:43.000000 mecoda-minka-1.0.1/src/mecoda_minka/py.typed
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     1720 2023-03-01 13:46:13.000000 mecoda-minka-1.0.1/src/mecoda_minka/views.py
-drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2023-03-02 15:27:10.912145 mecoda-minka-1.0.1/src/mecoda_minka.egg-info/
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    11796 2023-03-02 15:27:10.000000 mecoda-minka-1.0.1/src/mecoda_minka.egg-info/PKG-INFO
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)      395 2023-03-02 15:27:10.000000 mecoda-minka-1.0.1/src/mecoda_minka.egg-info/SOURCES.txt
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)        1 2023-03-02 15:27:10.000000 mecoda-minka-1.0.1/src/mecoda_minka.egg-info/dependency_links.txt
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)       32 2023-03-02 15:27:10.000000 mecoda-minka-1.0.1/src/mecoda_minka.egg-info/requires.txt
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)       13 2023-03-02 15:27:10.000000 mecoda-minka-1.0.1/src/mecoda_minka.egg-info/top_level.txt
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2023-05-24 11:48:01.154119 mecoda-minka-1.1.0/
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    11796 2023-05-24 11:48:01.154119 mecoda-minka-1.1.0/PKG-INFO
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     9006 2023-02-09 13:27:58.000000 mecoda-minka-1.1.0/README.md
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)       38 2023-05-24 11:48:01.154119 mecoda-minka-1.1.0/setup.cfg
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     1433 2023-05-24 11:47:03.000000 mecoda-minka-1.1.0/setup.py
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2023-05-24 11:48:01.150119 mecoda-minka-1.1.0/src/
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2023-05-24 11:48:01.150119 mecoda-minka-1.1.0/src/mecoda_minka/
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)      566 2022-12-22 16:17:43.000000 mecoda-minka-1.1.0/src/mecoda_minka/__init__.py
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2023-05-24 11:48:01.150119 mecoda-minka-1.1.0/src/mecoda_minka/data/
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)  4174945 2022-12-22 16:17:43.000000 mecoda-minka-1.1.0/src/mecoda_minka/data/taxon_tree.csv
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    15688 2023-05-24 10:41:22.000000 mecoda-minka-1.1.0/src/mecoda_minka/mecoda_minka.py
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     2148 2022-12-22 16:17:43.000000 mecoda-minka-1.1.0/src/mecoda_minka/models.py
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)        0 2022-12-22 16:17:43.000000 mecoda-minka-1.1.0/src/mecoda_minka/py.typed
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     1720 2023-03-01 13:46:13.000000 mecoda-minka-1.1.0/src/mecoda_minka/views.py
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2023-05-24 11:48:01.150119 mecoda-minka-1.1.0/src/mecoda_minka.egg-info/
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    11796 2023-05-24 11:48:01.000000 mecoda-minka-1.1.0/src/mecoda_minka.egg-info/PKG-INFO
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)      395 2023-05-24 11:48:01.000000 mecoda-minka-1.1.0/src/mecoda_minka.egg-info/SOURCES.txt
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)        1 2023-05-24 11:48:01.000000 mecoda-minka-1.1.0/src/mecoda_minka.egg-info/dependency_links.txt
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)       32 2023-05-24 11:48:01.000000 mecoda-minka-1.1.0/src/mecoda_minka.egg-info/requires.txt
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)       13 2023-05-24 11:48:01.000000 mecoda-minka-1.1.0/src/mecoda_minka.egg-info/top_level.txt
```

### Comparing `mecoda-minka-1.0.1/PKG-INFO` & `mecoda-minka-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecoda-minka
-Version: 1.0.1
+Version: 1.1.0
 Summary: Library to download information collected in Minka API.
 Home-page: https://github.com/pynomaly/mecoda-minka
 Author: Ana Alvarez
 Author-email: anomalia@disroot.org
 License: GNU General Public License v3
 Description: <img src="docs/logo-cos4cloud-middle.png" alt="cos4cloud" width="400"/>
```

### Comparing `mecoda-minka-1.0.1/README.md` & `mecoda-minka-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mecoda-minka-1.0.1/setup.py` & `mecoda-minka-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="mecoda-minka",
-    version="1.0.1",
+    version="1.1.0",
     description="Library to download information collected in Minka API.",
     author="Ana Alvarez",
     author_email="anomalia@disroot.org",
     license="GNU General Public License v3",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/pynomaly/mecoda-minka",
```

### Comparing `mecoda-minka-1.0.1/src/mecoda_minka/__init__.py` & `mecoda-minka-1.1.0/src/mecoda_minka/__init__.py`

 * *Files identical despite different names*

### Comparing `mecoda-minka-1.0.1/src/mecoda_minka/data/taxon_tree.csv` & `mecoda-minka-1.1.0/src/mecoda_minka/data/taxon_tree.csv`

 * *Files identical despite different names*

### Comparing `mecoda-minka-1.0.1/src/mecoda_minka/mecoda_minka.py` & `mecoda-minka-1.1.0/src/mecoda_minka/mecoda_minka.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     taxon: Optional[str] = None,
     taxon_id: Optional[int] = None,
     place_id: Optional[int] = None,
     year: Optional[int] = None,
     num_max: Optional[int] = None,
     starts_on: Optional[str] = None,  # Must be observed on or after this date
     ends_on: Optional[str] = None,  # Must be observed on or before this date
+    created_on: Optional[str] = None # Day YYYY-MM-DD
 ) -> List[Observation]:
     """
     Function to extract the observations and that supports different filters
     """
 
     print("Generating list of observations:")
 
@@ -63,14 +64,15 @@
         user,
         taxon,
         taxon_id,
         place_id,
         year,
         starts_on,
         ends_on,
+        created_on,
     )
 
     observations = _request(url, num_max)
 
     return observations
 
 
@@ -81,14 +83,15 @@
     user: Optional[str] = None,
     taxon: Optional[str] = None,
     taxon_id: Optional[int] = None,
     place_id: Optional[int] = None,
     year: Optional[int] = None,
     start_on: Optional[date] = None,
     ends_on: Optional[date] = None,
+    created_on: Optional[date] = None, # day YYYY-MM-DD
 ) -> str:
     """
     Internal function to build the url to which the observation request
     will be made
     """
     # define base url
     if id_project is not None:
@@ -98,14 +101,16 @@
     elif user is not None:
         base_url = f"{API_URL}/observations/{user}.json"
     else:
         base_url = f"{API_URL}/observations.json"
 
     # define the arguments that the API supports
     args = []
+    if created_on is not None:
+        args.append(f"created_on={created_on}")
     if start_on is not None:
         args.append(f"d1={start_on}")
     if ends_on is not None:
         args.append(f"d2={ends_on}")
     if query is not None:
         args.append(f'q="{query}"')
     if taxon is not None:
@@ -359,15 +364,16 @@
         "False",
     )
 
     return df_observations
 
 
 def download_photos(
-    df_photos: pd.DataFrame, directorio: Optional[str] = "minka_photos"
+    df_photos: pd.DataFrame, 
+    directorio: Optional[str] = "minka_photos"
 ):
     """
     Function to download the photos resulting from the query.
     """
     # Create the folder, if it exists overwrite it
     if os.path.exists(directorio):
         shutil.rmtree(directorio)
```

### Comparing `mecoda-minka-1.0.1/src/mecoda_minka/models.py` & `mecoda-minka-1.1.0/src/mecoda_minka/models.py`

 * *Files identical despite different names*

### Comparing `mecoda-minka-1.0.1/src/mecoda_minka/views.py` & `mecoda-minka-1.1.0/src/mecoda_minka/views.py`

 * *Files identical despite different names*

### Comparing `mecoda-minka-1.0.1/src/mecoda_minka.egg-info/PKG-INFO` & `mecoda-minka-1.1.0/src/mecoda_minka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecoda-minka
-Version: 1.0.1
+Version: 1.1.0
 Summary: Library to download information collected in Minka API.
 Home-page: https://github.com/pynomaly/mecoda-minka
 Author: Ana Alvarez
 Author-email: anomalia@disroot.org
 License: GNU General Public License v3
 Description: <img src="docs/logo-cos4cloud-middle.png" alt="cos4cloud" width="400"/>
```

