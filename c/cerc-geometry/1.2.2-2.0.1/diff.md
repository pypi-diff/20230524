# Comparing `tmp/cerc-geometry-1.2.2.tar.gz` & `tmp/cerc-geometry-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/peteryefi/Desktop/dompark/geometry/dist/.tmp-py5a9jq4/cerc-geometry-1.2.2.tar", last modified: Mon May 22 23:23:31 2023, max compression
+gzip compressed data, was "/Users/peteryefi/Desktop/dompark/geometry/dist/.tmp-an5izcij/cerc-geometry-2.0.1.tar", last modified: Wed May 24 01:31:08 2023, max compression
```

## Comparing `cerc-geometry-1.2.2.tar` & `cerc-geometry-2.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-22 23:23:31.718396 cerc-geometry-1.2.2/
--rw-rw-rw-   0 peteryefi   (501) staff       (20)     7431 2023-05-11 00:53:33.000000 cerc-geometry-1.2.2/LICENSE.md
--rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-22 23:23:31.718065 cerc-geometry-1.2.2/PKG-INFO
--rw-r--r--   0 peteryefi   (501) staff       (20)      522 2023-05-12 17:30:08.000000 cerc-geometry-1.2.2/README.md
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-22 23:23:31.707310 cerc-geometry-1.2.2/cerc_geometry.egg-info/
--rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-22 23:23:31.000000 cerc-geometry-1.2.2/cerc_geometry.egg-info/PKG-INFO
--rw-r--r--   0 peteryefi   (501) staff       (20)      535 2023-05-22 23:23:31.000000 cerc-geometry-1.2.2/cerc_geometry.egg-info/SOURCES.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)        1 2023-05-22 23:23:31.000000 cerc-geometry-1.2.2/cerc_geometry.egg-info/dependency_links.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)       48 2023-05-22 23:23:31.000000 cerc-geometry-1.2.2/cerc_geometry.egg-info/requires.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)        9 2023-05-22 23:23:31.000000 cerc-geometry-1.2.2/cerc_geometry.egg-info/top_level.txt
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-22 23:23:31.713589 cerc-geometry-1.2.2/geometry/
--rw-r--r--   0 peteryefi   (501) staff       (20)      200 2023-05-19 00:02:34.000000 cerc-geometry-1.2.2/geometry/__init__.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     5398 2023-05-16 00:05:51.000000 cerc-geometry-1.2.2/geometry/helper.py
--rw-r--r--   0 peteryefi   (501) staff       (20)    11135 2023-05-22 23:18:20.000000 cerc-geometry-1.2.2/geometry/library.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      574 2023-05-18 23:39:06.000000 cerc-geometry-1.2.2/geometry/location.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      707 2023-05-18 23:38:20.000000 cerc-geometry-1.2.2/geometry/map_point.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     2168 2023-05-15 23:21:05.000000 cerc-geometry-1.2.2/geometry/plane.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1002 2023-05-15 23:21:05.000000 cerc-geometry-1.2.2/geometry/point.py
--rw-r--r--   0 peteryefi   (501) staff       (20)    14604 2023-05-16 00:05:51.000000 cerc-geometry-1.2.2/geometry/polygon.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     6590 2023-05-15 23:21:05.000000 cerc-geometry-1.2.2/geometry/polyhedron.py
--rw-r--r--   0 peteryefi   (501) staff       (20)       99 2023-05-15 23:40:38.000000 cerc-geometry-1.2.2/pyproject.toml
--rw-r--r--   0 peteryefi   (501) staff       (20)       37 2023-05-18 23:51:47.000000 cerc-geometry-1.2.2/requirements.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)       38 2023-05-22 23:23:31.718519 cerc-geometry-1.2.2/setup.cfg
--rw-r--r--   0 peteryefi   (501) staff       (20)     1320 2023-05-22 23:18:57.000000 cerc-geometry-1.2.2/setup.py
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-22 23:23:31.717393 cerc-geometry-1.2.2/tests/
--rw-r--r--   0 peteryefi   (501) staff       (20)     1961 2023-05-16 00:05:50.000000 cerc-geometry-1.2.2/tests/test_helper.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      736 2023-05-16 00:05:50.000000 cerc-geometry-1.2.2/tests/test_plane.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      842 2023-05-16 00:05:50.000000 cerc-geometry-1.2.2/tests/test_point.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1513 2023-05-16 00:05:50.000000 cerc-geometry-1.2.2/tests/test_polygon.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1076 2023-05-16 00:05:50.000000 cerc-geometry-1.2.2/tests/test_polyhedron.py
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-24 01:31:08.407451 cerc-geometry-2.0.1/
+-rw-rw-rw-   0 peteryefi   (501) staff       (20)     7431 2023-05-11 00:53:33.000000 cerc-geometry-2.0.1/LICENSE.md
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-24 01:31:08.407138 cerc-geometry-2.0.1/PKG-INFO
+-rw-r--r--   0 peteryefi   (501) staff       (20)      522 2023-05-12 17:30:08.000000 cerc-geometry-2.0.1/README.md
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-24 01:31:08.397112 cerc-geometry-2.0.1/cerc_geometry.egg-info/
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-24 01:31:08.000000 cerc-geometry-2.0.1/cerc_geometry.egg-info/PKG-INFO
+-rw-r--r--   0 peteryefi   (501) staff       (20)      535 2023-05-24 01:31:08.000000 cerc-geometry-2.0.1/cerc_geometry.egg-info/SOURCES.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)        1 2023-05-24 01:31:08.000000 cerc-geometry-2.0.1/cerc_geometry.egg-info/dependency_links.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)       48 2023-05-24 01:31:08.000000 cerc-geometry-2.0.1/cerc_geometry.egg-info/requires.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)        9 2023-05-24 01:31:08.000000 cerc-geometry-2.0.1/cerc_geometry.egg-info/top_level.txt
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-24 01:31:08.403111 cerc-geometry-2.0.1/geometry/
+-rw-r--r--   0 peteryefi   (501) staff       (20)      200 2023-05-19 00:02:34.000000 cerc-geometry-2.0.1/geometry/__init__.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     5690 2023-05-23 00:07:56.000000 cerc-geometry-2.0.1/geometry/helper.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)    11135 2023-05-22 23:18:20.000000 cerc-geometry-2.0.1/geometry/library.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      574 2023-05-18 23:39:06.000000 cerc-geometry-2.0.1/geometry/location.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      707 2023-05-18 23:38:20.000000 cerc-geometry-2.0.1/geometry/map_point.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     2168 2023-05-15 23:21:05.000000 cerc-geometry-2.0.1/geometry/plane.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1002 2023-05-15 23:21:05.000000 cerc-geometry-2.0.1/geometry/point.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)    14604 2023-05-16 00:05:51.000000 cerc-geometry-2.0.1/geometry/polygon.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     6590 2023-05-15 23:21:05.000000 cerc-geometry-2.0.1/geometry/polyhedron.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)       99 2023-05-15 23:40:38.000000 cerc-geometry-2.0.1/pyproject.toml
+-rw-r--r--   0 peteryefi   (501) staff       (20)       37 2023-05-18 23:51:47.000000 cerc-geometry-2.0.1/requirements.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)       38 2023-05-24 01:31:08.407563 cerc-geometry-2.0.1/setup.cfg
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1320 2023-05-24 01:30:33.000000 cerc-geometry-2.0.1/setup.py
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-24 01:31:08.406514 cerc-geometry-2.0.1/tests/
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1961 2023-05-16 00:05:50.000000 cerc-geometry-2.0.1/tests/test_helper.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      736 2023-05-16 00:05:50.000000 cerc-geometry-2.0.1/tests/test_plane.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      842 2023-05-16 00:05:50.000000 cerc-geometry-2.0.1/tests/test_point.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1513 2023-05-16 00:05:50.000000 cerc-geometry-2.0.1/tests/test_polygon.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1076 2023-05-16 00:05:50.000000 cerc-geometry-2.0.1/tests/test_polyhedron.py
```

### Comparing `cerc-geometry-1.2.2/LICENSE.md` & `cerc-geometry-2.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.2.2/PKG-INFO` & `cerc-geometry-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-geometry
-Version: 1.2.2
+Version: 2.0.1
 Summary: CERC Geometry Library with different modules to manipulate geometric objects
 Home-page: https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Author: CERC
 Author-email:  cerc@concordia.ca
 Project-URL: Repository, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Project-URL: Bug Tracker, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cerc-geometry-1.2.2/README.md` & `cerc-geometry-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.2.2/cerc_geometry.egg-info/PKG-INFO` & `cerc-geometry-2.0.1/cerc_geometry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-geometry
-Version: 1.2.2
+Version: 2.0.1
 Summary: CERC Geometry Library with different modules to manipulate geometric objects
 Home-page: https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Author: CERC
 Author-email:  cerc@concordia.ca
 Project-URL: Repository, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Project-URL: Bug Tracker, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cerc-geometry-1.2.2/cerc_geometry.egg-info/SOURCES.txt` & `cerc-geometry-2.0.1/cerc_geometry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.2.2/geometry/helper.py` & `cerc-geometry-2.0.1/geometry/helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,14 +50,25 @@
             points = np.fromstring(coordinates, dtype=float, sep=' ')
             points = cls.to_points_matrix(points)
             return points
         except TypeError:
             sys.stderr.write('Expect coordinates to be a string of floats separated by spaces')
         except Exception as error:
             sys.stderr.write(f'An error occurred: {error}')
+
+    @classmethod
+    def gml_surface_to_libs(cls, surface):
+        """
+        Transform citygml surface names into hub names
+        """
+        if surface == 'WallSurface':
+            return 'Wall'
+        if surface == 'GroundSurface':
+            return 'Ground'
+        return 'Roof'
         
     @classmethod
     def remove_last_point_from_string(cls, points: str) -> str:
         """
         Ignore last point in a string of points
         :param points:
         :return:
```

### Comparing `cerc-geometry-1.2.2/geometry/library.py` & `cerc-geometry-2.0.1/geometry/library.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.2.2/geometry/location.py` & `cerc-geometry-2.0.1/geometry/location.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.2.2/geometry/map_point.py` & `cerc-geometry-2.0.1/geometry/map_point.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.2.2/geometry/plane.py` & `cerc-geometry-2.0.1/geometry/plane.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.2.2/geometry/point.py` & `cerc-geometry-2.0.1/geometry/point.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.2.2/geometry/polygon.py` & `cerc-geometry-2.0.1/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.2.2/geometry/polyhedron.py` & `cerc-geometry-2.0.1/geometry/polyhedron.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.2.2/setup.py` & `cerc-geometry-2.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     for requirement
     in pkg_resources.parse_requirements(r)
   ]
 install_requires.append('setuptools')
 
 setuptools.setup(
   name="cerc-geometry",
-  version="1.2.2",
+  version="2.0.1",
   author="CERC",
   author_email=" cerc@concordia.ca",
   description="CERC Geometry Library with different modules to manipulate geometric objects",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry",
   project_urls={
```

### Comparing `cerc-geometry-1.2.2/tests/test_helper.py` & `cerc-geometry-2.0.1/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.2.2/tests/test_plane.py` & `cerc-geometry-2.0.1/tests/test_plane.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.2.2/tests/test_point.py` & `cerc-geometry-2.0.1/tests/test_point.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.2.2/tests/test_polygon.py` & `cerc-geometry-2.0.1/tests/test_polygon.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.2.2/tests/test_polyhedron.py` & `cerc-geometry-2.0.1/tests/test_polyhedron.py`

 * *Files identical despite different names*

