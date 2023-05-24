# Comparing `tmp/importer-local-0.0.5.tar.gz` & `tmp/importer-local-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "importer-local-0.0.5.tar", last modified: Sat May 20 08:02:03 2023, max compression
+gzip compressed data, was "importer-local-0.0.6.tar", last modified: Wed May 24 02:09:08 2023, max compression
```

## Comparing `importer-local-0.0.5.tar` & `importer-local-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:02:03.427306 importer-local-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:02:03.423306 importer-local-0.0.5/CirclesImporter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 08:01:45.000000 importer-local-0.0.5/CirclesImporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-20 08:01:45.000000 importer-local-0.0.5/CirclesImporter/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-20 08:02:03.427306 importer-local-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-20 08:01:45.000000 importer-local-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:02:03.427306 importer-local-0.0.5/importer_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-20 08:02:03.000000 importer-local-0.0.5/importer_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-20 08:02:03.000000 importer-local-0.0.5/importer_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 08:02:03.000000 importer-local-0.0.5/importer_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 08:02:03.000000 importer-local-0.0.5/importer_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 08:02:03.427306 importer-local-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-20 08:01:45.000000 importer-local-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:02:03.427306 importer-local-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-20 08:01:45.000000 importer-local-0.0.5/tests/test_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:09:08.513712 importer-local-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:09:08.513712 importer-local-0.0.6/CirclesImporter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 02:08:57.000000 importer-local-0.0.6/CirclesImporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-24 02:08:57.000000 importer-local-0.0.6/CirclesImporter/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-24 02:09:08.513712 importer-local-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-24 02:08:57.000000 importer-local-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:09:08.513712 importer-local-0.0.6/importer_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-24 02:09:08.000000 importer-local-0.0.6/importer_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-24 02:09:08.000000 importer-local-0.0.6/importer_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 02:09:08.000000 importer-local-0.0.6/importer_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-24 02:09:08.000000 importer-local-0.0.6/importer_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 02:09:08.513712 importer-local-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-24 02:08:57.000000 importer-local-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:09:08.513712 importer-local-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-24 02:08:57.000000 importer-local-0.0.6/tests/test_importer.py
```

### Comparing `importer-local-0.0.5/CirclesImporter/importer.py` & `importer-local-0.0.6/CirclesImporter/importer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from circles_local_database_python.database import database
-from opencage.geocoder import OpenCageGeocode
-import os
+from opencage_get_country_name import Country
 from dotenv import load_dotenv
 from CirclesLocalLoggerPython.LoggerServiceSingleton import locallgr
 from functools import wraps
 load_dotenv()
 
 
 def log_function_execution(func):
@@ -22,39 +21,14 @@
 
 
 class Importer:
     def __init__(self, source):
         self.source_name = source
 
     @log_function_execution
-    def get_country_name(self, location):
-        # Create a geocoder instance
-        api_key = os.getenv("RDS_OPENCAGE_KEY")
-
-        # Define the city or state
-        geocoder = OpenCageGeocode(api_key)
-
-        # Use geocoding to get the location details
-        results = geocoder.geocode(location)
-
-        if results and len(results) > 0:
-            first_result = results[0]
-            components = first_result['components']
-
-            # Extract the country from components
-            country = components.get('country', '')
-            if not country:
-                # If country is not found, check for country_code as an alternative
-                country = components.get('country_code', '')
-            return country
-
-        else:
-            return None
-
-    @log_function_execution
     def insert_new_entity(self, entity_type_name):
         database_conn = database()
         db = database_conn.connect_to_database()
         cursor = db.cursor()
 
         cursor.execute("SELECT entity_type_id FROM {} WHERE entity_type_name = '{}'".format('entity_type.entity_type_ml_table', entity_type_name))
         entity_type_id = cursor.fetchone()
@@ -68,15 +42,16 @@
             last_inserted_id = cursor.lastrowid
             query_entity_ml = "INSERT INTO {}(`entity_type_name`,`entity_type_id`,`lang_code`,`created_user_id`,`updated_user_id`)" \
                               " VALUES (%s, %s, %s, 1, 1)".format('entity_type.entity_type_ml_table')
             cursor.execute(query_entity_ml, (entity_type_name, last_inserted_id, 'en'))
 
             db.commit()
         else:
-            locallgr.log("Entity already exist")
+            source_message = "Entity %s already exist." % entity_type_name
+            locallgr.log(source_message)
         db.close()
 
     @log_function_execution
     def insert_new_source(self):
         database_conn = database()
         db = database_conn.connect_to_database()
         cursor = db.cursor()
@@ -93,27 +68,29 @@
             last_inserted_id = cursor.lastrowid
             query_importer_source_ml = "INSERT INTO {}(`source_name`,`source_id`,`created_user_id`,`updated_user_id`)" \
                               " VALUES (%s, %s, 1, 1)".format('source.source_ml_table')
             cursor.execute(query_importer_source_ml, (self.source_name, last_inserted_id))
 
             db.commit()
         else:
-            locallgr.log("Source already exist")
+            source_message = "Source %s already exist." % self.source_name
+            locallgr.log(source_message)
         db.close()
 
     @log_function_execution
     def insert_record_source(self, location, entity_type_name, entity_id, url):
         database_conn = database()
         db = database_conn.connect_to_database()
         cursor = db.cursor()
 
         cursor.execute("SELECT source_id FROM {} WHERE source_name = '{}'".format('source.source_ml_table', self.source_name))
         source_id = cursor.fetchone()
 
-        country_name = self.get_country_name(location)
+        find_country = Country()
+        country_name = find_country.get_country_name(location)
         cursor.execute(
             "SELECT id FROM {} WHERE name = '{}'".format('location.country_table', country_name))
         country_id = cursor.fetchone()
 
         cursor.execute("SELECT entity_type_id FROM {} WHERE entity_type_name = '{}'".format('entity_type.entity_type_ml_table', entity_type_name))
         entity_type_id = cursor.fetchone()
```

### Comparing `importer-local-0.0.5/setup.py` & `importer-local-0.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
-     # TODO: Please update the name
-     name='importer-local',
-     version='0.0.5',
+     # TODO: Please update the name and delete this line i.e. XXX-local or XXX-remote (without the -python-package suffix)
+     name='importer-local',  
+     version='0.0.6',
      author="Circles",
      author_email="info@circles.life",
-     description="PyPI Package for Circles Local importer Python",
-     long_description="This is a package for sharing common importer function used in different repositories",
+     # TODO: Please update the description and delete this line
+     description="PyPI Package for Circles <project-name> Local/Remote Python",
+     # TODO: Please update the long description and delete this line    
+     long_description="This is a package for sharing common XXX function used in different repositories",
      long_description_content_type="text/markdown",
-     url="https://github.com/javatechy/dokr",
+     url="https://github.com/circles",
      packages=setuptools.find_packages(),
      classifiers=[
          "Programming Language :: Python :: 3",
          "License :: Other/Proprietary License",
          "Operating System :: OS Independent",
      ],
  )
```

### Comparing `importer-local-0.0.5/tests/test_importer.py` & `importer-local-0.0.6/tests/test_importer.py`

 * *Files identical despite different names*

