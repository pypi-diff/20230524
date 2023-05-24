# Comparing `tmp/centerline-width-0.0.2.tar.gz` & `tmp/centerline-width-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/centerline-width-0.0.2.tar", last modified: Wed Mar 15 08:57:31 2023, max compression
+gzip compressed data, was "dist/centerline-width-0.1.0.tar", last modified: Thu May 18 01:12:03 2023, max compression
```

## Comparing `centerline-width-0.0.2.tar` & `centerline-width-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,25 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-15 08:57:31.542870 centerline-width-0.0.2/
--rw-rw-r--   0 user      (1000) user      (1000)    13137 2023-03-15 08:57:31.542870 centerline-width-0.0.2/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    10398 2023-03-15 08:46:38.000000 centerline-width-0.0.2/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-15 08:57:31.538870 centerline-width-0.0.2/centerline_width/
--rw-rw-r--   0 user      (1000) user      (1000)      846 2023-03-14 21:55:29.000000 centerline-width-0.0.2/centerline_width/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     5715 2023-03-15 08:54:56.000000 centerline-width-0.0.2/centerline_width/centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)     5108 2023-03-15 08:05:21.000000 centerline-width-0.0.2/centerline_width/error_handling.py
--rw-rw-r--   0 user      (1000) user      (1000)     3921 2023-03-14 21:54:08.000000 centerline-width-0.0.2/centerline_width/plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     4793 2023-03-15 08:53:00.000000 centerline-width-0.0.2/centerline_width/preprocessing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-15 08:57:31.542870 centerline-width-0.0.2/centerline_width.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    13137 2023-03-15 08:57:31.000000 centerline-width-0.0.2/centerline_width.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      379 2023-03-15 08:57:31.000000 centerline-width-0.0.2/centerline_width.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-03-15 08:57:31.000000 centerline-width-0.0.2/centerline_width.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       89 2023-03-15 08:57:31.000000 centerline-width-0.0.2/centerline_width.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       17 2023-03-15 08:57:31.000000 centerline-width-0.0.2/centerline_width.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-03-15 08:57:31.542870 centerline-width-0.0.2/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1687 2023-03-15 08:56:33.000000 centerline-width-0.0.2/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-18 01:12:03.219940 centerline-width-0.1.0/
+-rw-rw-r--   0 user      (1000) user      (1000)    25284 2023-05-18 01:12:03.219940 centerline-width-0.1.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    21129 2023-05-17 22:01:39.000000 centerline-width-0.1.0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-18 01:12:03.211959 centerline-width-0.1.0/centerline_width/
+-rw-rw-r--   0 user      (1000) user      (1000)     1379 2023-05-17 02:00:43.000000 centerline-width-0.1.0/centerline_width/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    20385 2023-05-17 21:43:05.000000 centerline-width-0.1.0/centerline_width/centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10092 2023-05-17 22:00:01.000000 centerline-width-0.1.0/centerline_width/error_handling.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1683 2023-05-17 04:17:41.000000 centerline-width-0.1.0/centerline_width/getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8550 2023-05-15 20:31:09.000000 centerline-width-0.1.0/centerline_width/plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4985 2023-05-15 20:27:53.000000 centerline-width-0.1.0/centerline_width/preprocessing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-18 01:12:03.219940 centerline-width-0.1.0/centerline_width/pytests/
+-rw-rw-r--   0 user      (1000) user      (1000)     6697 2023-05-17 22:00:19.000000 centerline-width-0.1.0/centerline_width/pytests/test_centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3981 2023-05-17 04:23:14.000000 centerline-width-0.1.0/centerline_width/pytests/test_getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11026 2023-05-17 04:31:11.000000 centerline-width-0.1.0/centerline_width/pytests/test_plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-0.1.0/centerline_width/pytests/test_preprocessing.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2078 2023-05-17 04:34:35.000000 centerline-width-0.1.0/centerline_width/pytests/test_riverCenterlineClass.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3865 2023-05-17 21:19:02.000000 centerline-width-0.1.0/centerline_width/riverCenterlineClass.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-18 01:12:03.215949 centerline-width-0.1.0/centerline_width.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    25284 2023-05-18 01:12:03.000000 centerline-width-0.1.0/centerline_width.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      700 2023-05-18 01:12:03.000000 centerline-width-0.1.0/centerline_width.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-18 01:12:03.000000 centerline-width-0.1.0/centerline_width.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      133 2023-05-18 01:12:03.000000 centerline-width-0.1.0/centerline_width.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2023-05-18 01:12:03.000000 centerline-width-0.1.0/centerline_width.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-18 01:12:03.219940 centerline-width-0.1.0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1746 2023-05-18 01:11:03.000000 centerline-width-0.1.0/setup.py
```

### Comparing `centerline-width-0.0.2/centerline_width/__init__.py` & `centerline-width-0.1.0/centerline_width/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,34 @@
+# get_coordinates_kml.py function calls
+from .getCoordinatesKML import extractPointsToTextFile
+
 # preprocessing.py function calls
 from .preprocessing import convertColumnsToCSV
 from .preprocessing import leftRightCoordinates
 from .preprocessing import generatePolygon
 from .preprocessing import generateVoronoi
 from .preprocessing import pointsFromVoronoi
 
+# riverObject.py function calls
+from .riverCenterlineClass import riverCenterline
+
 # centerline.py function calls
 from .centerline import centerlinePath
 from .centerline import networkXGraphShortestPath
-from .centerline import centerlineLatitudeLongitude
+from .centerline import centerlineLength
+from .centerline import evenlySpacedCenterline
+from .centerline import smoothedCoordinates
+from .centerline import returnShortestPathPoints
+from .centerline import riverWidthFromCenterlineCoordinates
 from .centerline import riverWidthFromCenterline
 
 # plotDiagrams.py function calls
 from .plotDiagrams import plotCenterline
+from .plotDiagrams import plotCenterlineWidth
 
 # error_handling.py function calls
 from .error_handling import errrorHandlingConvertColumnsToCSV
 from .error_handling import errorHandlingPlotCenterline
-from .error_handling import errorHandlingCenterlineLatitudeLongitude
+from .error_handling import errorHandlingPlotCenterlineWidth
 from .error_handling import errorHandlingRiverWidthFromCenterline
+from .error_handling import errorHandlingExtractPointsToTextFile
+from .error_handling import errorHandlingRiverCenterlineClass
```

### Comparing `centerline-width-0.0.2/centerline_width/preprocessing.py` & `centerline-width-0.1.0/centerline_width/preprocessing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# Convert a text file to a csv
-# Option to flip bank directions
+# Built in Python functions
 import csv
 import logging
 import math
 
+# External Python libraries (installed via pip install)
 from collections import Counter
 import numpy as np
 from shapely.geometry import Point, Polygon, LineString
 from scipy.spatial import Voronoi
 
 # Internal centerline_width reference to access functions, global variables, and error handling
 import centerline_width
@@ -69,33 +69,34 @@
 		bank_points_swapped.append([bank_point[0], bank_point[1]]) # Swap the x and y to graph with longitude on the y-axis
 
 	river_polygon = Polygon(bank_points_swapped)
 	top_river = LineString([Point(left_bank_lst[::-1][0][0],left_bank_lst[::-1][0][1]), Point(right_bank_lst[::-1][0][0], right_bank_lst[::-1][0][1])])
 	bottom_river = LineString([Point(right_bank_lst[0][0], right_bank_lst[0][1]), Point(left_bank_lst[0][0], left_bank_lst[0][1])])
 
 	if not river_polygon.is_valid:
-		logger.critical("Invalid Polygon needs to be corrected")
+		logger.critical("[FAILED]  Invalid Polygon needs to be corrected")
 	else:
-		logger.info("Valid polygon generated")
+		logger.info("[SUCCESS] Valid polygon generated")
 
 	return river_polygon, top_river, bottom_river
 
 def generateVoronoi(left_bank_lst, right_bank_lst):
 	# Generate a Voronoi shape based on the left/right bank points
 	all_banks_points = left_bank_lst + right_bank_lst
 	all_banks_points = np.array(all_banks_points)
 
 	river_voronoi = Voronoi(all_banks_points)
-	logger.info("Voronoi diagram generated")
+	logger.info("[SUCCESS] Voronoi diagram generated")
 	return river_voronoi
 
 def pointsFromVoronoi(river_voronoi, river_polygon):
 	# Returns a dictionary list of all the voronoi points: {start point : [list of end points]}
 	points_dict = {}
 	all_connections_start_to_end = []
+	logger.info("[PROCESSING] Attempting to determine a valid centerline from Voronoi points, may take a few minutes...") # longest step, O(n^n)
 	for ridge_vertex_point in river_voronoi.ridge_vertices:
 		if ridge_vertex_point[0] >= 0 and ridge_vertex_point[1] >= 0: # Only include non-infinity vertex edges
 			v0 = river_voronoi.vertices[ridge_vertex_point[0]]
 			v1 = river_voronoi.vertices[ridge_vertex_point[1]]
 			# Check if start and end points are within the polygon, otherwise remove the connection pair
 			if river_polygon.contains(Point([v0[0], v0[1]])) and river_polygon.contains(Point([v1[0], v1[1]])):
 				start_point = tuple([v0[0], v0[1]])
```

### Comparing `centerline-width-0.0.2/setup.py` & `centerline-width-0.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 # Python Package Setup
 from setuptools import setup, find_namespace_packages
 
-VERSION="0.0.2"
+VERSION="0.1.0"
 DESCRIPTION="A Python package to find the centerline and width of rivers based on the latitude and longitude from a right and left bank"
 
 with open("README.md", "r") as f:
 	long_description_readme = f.read()
 
 setup(
 	name="centerline-width",
@@ -34,16 +34,19 @@
 		"Topic :: Scientific/Engineering :: Hydrology",
 		"Topic :: Scientific/Engineering :: Visualization"
 	],
 	packages=find_namespace_packages(include=['centerline_width',
 											'centerline_width.*']),
 	include_package_data=True,
 	install_requires=[
+		"haversine>=2.8.0",
 		"matplotlib>=3.1.0",
 		"networkx>=3.0",
 		"numpy>=1.24.1",
 		"pandas>=1.3.5",
+		"pykml>=0.2.0",
+		"pytest>=7.2.2",
 		"scipy>=1.10.1",
 		"shapely>=2.0.1"
 	],
 	python_requires='>=3.9'
 )
```

