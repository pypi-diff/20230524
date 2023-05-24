# Comparing `tmp/centerline-width-0.2.1.tar.gz` & `tmp/centerline-width-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/centerline-width-0.2.1.tar", last modified: Wed May 24 19:43:32 2023, max compression
+gzip compressed data, was "dist/centerline-width-0.2.2.tar", last modified: Wed May 24 21:12:42 2023, max compression
```

## Comparing `centerline-width-0.2.1.tar` & `centerline-width-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 19:43:32.460573 centerline-width-0.2.1/
--rw-rw-r--   0 user      (1000) user      (1000)    30899 2023-05-24 19:43:32.460573 centerline-width-0.2.1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    26121 2023-05-24 19:24:29.000000 centerline-width-0.2.1/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 19:43:32.456573 centerline-width-0.2.1/centerline_width/
--rw-rw-r--   0 user      (1000) user      (1000)     1382 2023-05-23 20:44:39.000000 centerline-width-0.2.1/centerline_width/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    20854 2023-05-23 21:37:54.000000 centerline-width-0.2.1/centerline_width/centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)    10941 2023-05-24 19:30:15.000000 centerline-width-0.2.1/centerline_width/error_handling.py
--rw-rw-r--   0 user      (1000) user      (1000)     1854 2023-05-18 02:15:59.000000 centerline-width-0.2.1/centerline_width/getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)     8345 2023-05-24 02:25:01.000000 centerline-width-0.2.1/centerline_width/plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     6427 2023-05-23 07:06:34.000000 centerline-width-0.2.1/centerline_width/preprocessing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 19:43:32.460573 centerline-width-0.2.1/centerline_width/pytests/
--rw-rw-r--   0 user      (1000) user      (1000)     6697 2023-05-17 22:00:19.000000 centerline-width-0.2.1/centerline_width/pytests/test_centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-05-24 19:31:02.000000 centerline-width-0.2.1/centerline_width/pytests/test_getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)    11026 2023-05-17 04:31:11.000000 centerline-width-0.2.1/centerline_width/pytests/test_plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-0.2.1/centerline_width/pytests/test_preprocessing.py
--rw-rw-r--   0 user      (1000) user      (1000)     3397 2023-05-19 19:58:39.000000 centerline-width-0.2.1/centerline_width/pytests/test_riverCenterlineClass.py
--rw-rw-r--   0 user      (1000) user      (1000)     4569 2023-05-23 21:32:40.000000 centerline-width-0.2.1/centerline_width/riverCenterlineClass.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 19:43:32.460573 centerline-width-0.2.1/centerline_width.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    30899 2023-05-24 19:43:32.000000 centerline-width-0.2.1/centerline_width.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      700 2023-05-24 19:43:32.000000 centerline-width-0.2.1/centerline_width.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-24 19:43:32.000000 centerline-width-0.2.1/centerline_width.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      133 2023-05-24 19:43:32.000000 centerline-width-0.2.1/centerline_width.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       17 2023-05-24 19:43:32.000000 centerline-width-0.2.1/centerline_width.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-24 19:43:32.460573 centerline-width-0.2.1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1813 2023-05-24 19:39:43.000000 centerline-width-0.2.1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 21:12:42.731609 centerline-width-0.2.2/
+-rw-rw-r--   0 user      (1000) user      (1000)    31128 2023-05-24 21:12:42.731609 centerline-width-0.2.2/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    26334 2023-05-24 21:09:28.000000 centerline-width-0.2.2/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 21:12:42.727609 centerline-width-0.2.2/centerline_width/
+-rw-rw-r--   0 user      (1000) user      (1000)     1382 2023-05-23 20:44:39.000000 centerline-width-0.2.2/centerline_width/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    20859 2023-05-24 21:09:07.000000 centerline-width-0.2.2/centerline_width/centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10941 2023-05-24 19:30:15.000000 centerline-width-0.2.2/centerline_width/error_handling.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1854 2023-05-18 02:15:59.000000 centerline-width-0.2.2/centerline_width/getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8345 2023-05-24 20:50:36.000000 centerline-width-0.2.2/centerline_width/plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6750 2023-05-24 20:32:04.000000 centerline-width-0.2.2/centerline_width/preprocessing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 21:12:42.731609 centerline-width-0.2.2/centerline_width/pytests/
+-rw-rw-r--   0 user      (1000) user      (1000)     6697 2023-05-17 22:00:19.000000 centerline-width-0.2.2/centerline_width/pytests/test_centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-05-24 19:31:02.000000 centerline-width-0.2.2/centerline_width/pytests/test_getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11026 2023-05-17 04:31:11.000000 centerline-width-0.2.2/centerline_width/pytests/test_plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-0.2.2/centerline_width/pytests/test_preprocessing.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3397 2023-05-19 19:58:39.000000 centerline-width-0.2.2/centerline_width/pytests/test_riverCenterlineClass.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4569 2023-05-23 21:32:40.000000 centerline-width-0.2.2/centerline_width/riverCenterlineClass.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 21:12:42.727609 centerline-width-0.2.2/centerline_width.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    31128 2023-05-24 21:12:42.000000 centerline-width-0.2.2/centerline_width.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      700 2023-05-24 21:12:42.000000 centerline-width-0.2.2/centerline_width.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-24 21:12:42.000000 centerline-width-0.2.2/centerline_width.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      133 2023-05-24 21:12:42.000000 centerline-width-0.2.2/centerline_width.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2023-05-24 21:12:42.000000 centerline-width-0.2.2/centerline_width.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-24 21:12:42.731609 centerline-width-0.2.2/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1813 2023-05-24 21:04:30.000000 centerline-width-0.2.2/setup.py
```

### Comparing `centerline-width-0.2.1/PKG-INFO` & `centerline-width-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.2.1.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.2.2.tar.gz
 Description: # Centerline-Width
         ![PyPi](https://img.shields.io/pypi/v/centerline-width)
         ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
         [![NSF-2141064](https://img.shields.io/badge/NSF-2141064-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2141064&HistoricalAwards=false)
         [![pytests](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml/badge.svg)](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml)
         
         Find the centerline and width of rivers based on the latitude and longitude positionss from the right and left bank 
@@ -190,15 +190,15 @@
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         ```
         
         ### Return Latitude/Longitude Coordinates of Centerline
-        Return the latitude/longtiude coordinates of the centerline based on the left and right banks
+        Return the latitude/longitude coordinates of the centerline based on the left and right banks
         ```
         river_object.centerlineLatitudeLongtiude
         ```
         Centerline coordinates are formed from Voronoi vertices
         
         ```python
         import centerline_width
@@ -392,26 +392,28 @@
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example1.png)
         In this example, the polygon is invalid, but with such a small overlap it is still able to find a valid path
         
         With limited data, the polygon will overlap more dramatically and will struggle to find a valid centerline:
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example4.png)
         
         ### Invalid Centerline
-        If the data is too small, a centerline and its coordinates cannot not be found (since only a single Voronoi vertex exists within the polygon and after deadends are filtered)
+        If the data is too small, a centerline and its coordinates cannot not be found (since only a single Voronoi vertex exists within the polygon and after dead ends are filtered)
         
-        `CRITICAL ERROR, Voronoi diagram generated too small to find centerline (no starting node found), unable to plot centerline. Set displayVoronoi=True to view. Can typically be fixed by adding more data to expand range.`
+        `CRITICAL ERROR, Polygon too short for the Voronoi diagram generated (no starting node found), unable to plot centerline. Set displayVoronoi=True to view vertices. Can typically be fixed by adding more data to expand range.`
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example2.png)
         Can be fixed by expanding the data until the polygon is large enough to contain at least two different vertex points
         
-        ### Invalid Top and Bottom Bank Postiions (flipDirection = True)
+        ### Invalid Top and Bottom Bank Postions (flipBankDirection = True)
+        Error: `Invalid Polygon Due to Flipped Banks, fix recommendation: rerun convertColumnsToCSV() and set flipBankDirection=True (or reset to default 'False' if currently set to flipBankDirection=True)`
+        
         If the data for the left and right river banks are generated in reverse order, they will be read in the incorrect order and the graph will find the invalid top and bottom of the bank
         
         If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
         
-        This can be fixed by using the flipDirection optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flipBankDirection=True)`
+        This can be fixed by using the flipBankDirection optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flipBankDirection=True)`
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/flipDirection_example.png)
         
         ### Fix Gaps and Jagged Centerlines
         Gaps formed can cause part of the centerline to be skipped due to sparse data. As a result, the start and end of the centerline can skip parts at the beginning or end of a river
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_short_path.png)
         Set river object created by `centerline_width.riverCenterline` to `interpolate_data=True` to fix for jagged edges or gaps formed by the interaction of sparse data and narrow banks
         ```python
@@ -437,15 +439,15 @@
         
          <p align="center">
           <img src="https://user-images.githubusercontent.com/22159116/222872092-e0b579cc-4f84-4f49-aa53-397785fb9bf2.png" />
           <img src="https://user-images.githubusercontent.com/22159116/222872119-7c485ee2-4ffd-413a-9e4f-b043b122d2bb.png" />
           <img src="https://user-images.githubusercontent.com/22159116/222872019-12931138-9e10-4e51-aa1e-552e72d09af0.png" />
         </p>
         
-        This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the atuhors and do not neccessarily reflect the views of the National Science Foundation.
+        This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not necessarily reflect the views of the National Science Foundation.
         
         ## Bug and Feature Request
         
         Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/cyschneck/centerline-width/issues) or to ugschneck@gmail.com/cyschneck@gmail.com
         
 Keywords: geophysics,python,voronoi,networkx,centerline,centerline-extraction,centerline-detection,rivers,river-bank-length,river-bank,limnology,hydrology
 Platform: UNKNOWN
```

### Comparing `centerline-width-0.2.1/README.md` & `centerline-width-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 ```
 
 ### Return Latitude/Longitude Coordinates of Centerline
-Return the latitude/longtiude coordinates of the centerline based on the left and right banks
+Return the latitude/longitude coordinates of the centerline based on the left and right banks
 ```
 river_object.centerlineLatitudeLongtiude
 ```
 Centerline coordinates are formed from Voronoi vertices
 
 ```python
 import centerline_width
@@ -384,26 +384,28 @@
 ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example1.png)
 In this example, the polygon is invalid, but with such a small overlap it is still able to find a valid path
 
 With limited data, the polygon will overlap more dramatically and will struggle to find a valid centerline:
 ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example4.png)
 
 ### Invalid Centerline
-If the data is too small, a centerline and its coordinates cannot not be found (since only a single Voronoi vertex exists within the polygon and after deadends are filtered)
+If the data is too small, a centerline and its coordinates cannot not be found (since only a single Voronoi vertex exists within the polygon and after dead ends are filtered)
 
-`CRITICAL ERROR, Voronoi diagram generated too small to find centerline (no starting node found), unable to plot centerline. Set displayVoronoi=True to view. Can typically be fixed by adding more data to expand range.`
+`CRITICAL ERROR, Polygon too short for the Voronoi diagram generated (no starting node found), unable to plot centerline. Set displayVoronoi=True to view vertices. Can typically be fixed by adding more data to expand range.`
 ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example2.png)
 Can be fixed by expanding the data until the polygon is large enough to contain at least two different vertex points
 
-### Invalid Top and Bottom Bank Postiions (flipDirection = True)
+### Invalid Top and Bottom Bank Postions (flipBankDirection = True)
+Error: `Invalid Polygon Due to Flipped Banks, fix recommendation: rerun convertColumnsToCSV() and set flipBankDirection=True (or reset to default 'False' if currently set to flipBankDirection=True)`
+
 If the data for the left and right river banks are generated in reverse order, they will be read in the incorrect order and the graph will find the invalid top and bottom of the bank
 
 If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
 
-This can be fixed by using the flipDirection optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flipBankDirection=True)`
+This can be fixed by using the flipBankDirection optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flipBankDirection=True)`
 ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/flipDirection_example.png)
 
 ### Fix Gaps and Jagged Centerlines
 Gaps formed can cause part of the centerline to be skipped due to sparse data. As a result, the start and end of the centerline can skip parts at the beginning or end of a river
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_short_path.png)
 Set river object created by `centerline_width.riverCenterline` to `interpolate_data=True` to fix for jagged edges or gaps formed by the interaction of sparse data and narrow banks
 ```python
@@ -429,12 +431,12 @@
 
  <p align="center">
   <img src="https://user-images.githubusercontent.com/22159116/222872092-e0b579cc-4f84-4f49-aa53-397785fb9bf2.png" />
   <img src="https://user-images.githubusercontent.com/22159116/222872119-7c485ee2-4ffd-413a-9e4f-b043b122d2bb.png" />
   <img src="https://user-images.githubusercontent.com/22159116/222872019-12931138-9e10-4e51-aa1e-552e72d09af0.png" />
 </p>
 
-This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the atuhors and do not neccessarily reflect the views of the National Science Foundation.
+This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not necessarily reflect the views of the National Science Foundation.
 
 ## Bug and Feature Request
 
 Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/cyschneck/centerline-width/issues) or to ugschneck@gmail.com/cyschneck@gmail.com
```

### Comparing `centerline-width-0.2.1/centerline_width/__init__.py` & `centerline-width-0.2.2/centerline_width/__init__.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.1/centerline_width/centerline.py` & `centerline-width-0.2.2/centerline_width/centerline.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 							if Point(end_point).distance(bottom_polygon_line) <= Point(ending_node).distance(bottom_polygon_line):
 								ending_node = end_point
 					# Save all starting and end positions for all possible paths
 					x_ridge_point.append((start_point[0], end_point[0]))
 					y_ridge_point.append((start_point[1], end_point[1]))
 
 	if starting_node is None:
-		logger.critical("\nCRITICAL ERROR, Voronoi diagram generated too small to find centerline (no starting node found), unable to plot centerline. Set displayVoronoi=True to view. Can typically be fixed by adding more data to expand range.")
+		logger.critical("\nCRITICAL ERROR, Polygon too short for the Voronoi diagram generated (no starting node found), unable to plot centerline. Set displayVoronoi=True to view vertices. Can typically be fixed by adding more data to expand range.")
 		shortest_path_points = None
 	else:
 		shortest_path_points = networkXGraphShortestPath(nx_graphs, starting_node, ending_node)
 
 	return starting_node, ending_node, x_ridge_point, y_ridge_point, shortest_path_points
 
 def evenlySpacedCenterline(centerline_coordinates=None, number_of_fixed_points=10):
@@ -256,15 +256,15 @@
 						if linestring_to_check not in linestring_with_linestrings_that_intersect.keys():
 							linestring_with_linestrings_that_intersect[linestring_to_check] = []
 						linestring_with_linestrings_that_intersect[linestring_to_check].append(linestring_to_check_against)
 
 	# Remove Intersection Lines
 	centerline_coordinates_to_be_removed = []
 	if remove_intersections:
-		logger.info("[PROCSESING] Recursively removing interesection lines...")
+		logger.info("[PROCESSING] Recursively removing intersection lines...")
 		# iterate from the most intersections to the least intersections
 		for linestring_most_interactions in sorted(linestring_with_linestrings_that_intersect, key=lambda k: len(linestring_with_linestrings_that_intersect[k]), reverse=True):
 
 			# when number of intersections > 1, remove lines with the most interactions to the smallest
 			if num_intersection_coordinates[linestring_with_centerlines[linestring_most_interactions]] > 1: 
 				lst_linestrings_hit_by_linestring = linestring_with_linestrings_that_intersect[linestring_most_interactions]
```

### Comparing `centerline-width-0.2.1/centerline_width/error_handling.py` & `centerline-width-0.2.2/centerline_width/error_handling.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.1/centerline_width/getCoordinatesKML.py` & `centerline-width-0.2.2/centerline_width/getCoordinatesKML.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.1/centerline_width/plotDiagrams.py` & `centerline-width-0.2.2/centerline_width/plotDiagrams.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.1/centerline_width/preprocessing.py` & `centerline-width-0.2.2/centerline_width/preprocessing.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,35 +55,34 @@
 	for index, row in dataframe.iterrows():
 		if not math.isnan(row.rlat) and not math.isnan(row.rlon):
 			right_bank_coordinates.append([row.rlon, row.rlat])
 		if not math.isnan(row.llat) and not math.isnan(row.llon):
 			left_bank_coordinates.append([row.llon, row.llat])
 	return left_bank_coordinates, right_bank_coordinates
 
-def generatePolygon(left_bank_lst, right_bank_lst):
+def generatePolygon(left_bank_lst, right_bank_lst, recursion_check=False):
 	# Return a shapely polygon based on the position of the river bank points
 	if len(right_bank_lst) == 0:
 		logger.critical("\nCRITICAL ERROR, right bank data is empty (or NaN)")
 		exit()
 	if len(left_bank_lst) == 0:
 		logger.critical("\nCRITICAL ERROR, left bank data is empty (or NaN)")
 		exit()
 	circular_list_of_banks = left_bank_lst + right_bank_lst[::-1] + [left_bank_lst[0]]
 
-	bank_points_swapped = []
-	for i, bank_point in enumerate(circular_list_of_banks):
-		bank_points_swapped.append([bank_point[0], bank_point[1]]) # Swap the x and y to graph with longitude on the y-axis
-
-	river_polygon = Polygon(bank_points_swapped)
+	river_polygon = Polygon(circular_list_of_banks)
 	top_river = LineString([Point(left_bank_lst[::-1][0][0],left_bank_lst[::-1][0][1]), Point(right_bank_lst[::-1][0][0], right_bank_lst[::-1][0][1])])
 	bottom_river = LineString([Point(right_bank_lst[0][0], right_bank_lst[0][1]), Point(left_bank_lst[0][0], left_bank_lst[0][1])])
 
-	if not river_polygon.is_valid:
+	if not river_polygon.is_valid and not recursion_check:
 		logger.critical("[FAILED]  Invalid Polygon may need to be corrected")
-	else:
+		polygon_check, _, _ = generatePolygon(left_bank_lst, right_bank_lst[::-1], recursion_check=True) # only run once with recursion_check set (just to check if reverse banks fixes issue)
+		if polygon_check.is_valid:
+			logger.critical("\nInvalid Polygon Due to Flipped Banks, fix recommendation: rerun convertColumnsToCSV() and set flipBankDirection=True (or reset to default 'False' if currently set to flipBankDirection=True)\n")
+	if river_polygon.is_valid and not recursion_check:
 		logger.info("[SUCCESS] Valid polygon generated")
 
 	return river_polygon, top_river, bottom_river
 
 def generateVoronoi(left_bank_lst, right_bank_lst):
 	# Generate a Voronoi shape based on the left/right bank points
 	all_banks_points = left_bank_lst + right_bank_lst
```

### Comparing `centerline-width-0.2.1/centerline_width/pytests/test_centerline.py` & `centerline-width-0.2.2/centerline_width/pytests/test_centerline.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.1/centerline_width/pytests/test_getCoordinatesKML.py` & `centerline-width-0.2.2/centerline_width/pytests/test_getCoordinatesKML.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.1/centerline_width/pytests/test_plotDiagrams.py` & `centerline-width-0.2.2/centerline_width/pytests/test_plotDiagrams.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.1/centerline_width/pytests/test_preprocessing.py` & `centerline-width-0.2.2/centerline_width/pytests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.1/centerline_width/pytests/test_riverCenterlineClass.py` & `centerline-width-0.2.2/centerline_width/pytests/test_riverCenterlineClass.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.1/centerline_width/riverCenterlineClass.py` & `centerline-width-0.2.2/centerline_width/riverCenterlineClass.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.1/centerline_width.egg-info/PKG-INFO` & `centerline-width-0.2.2/centerline_width.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.2.1.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.2.2.tar.gz
 Description: # Centerline-Width
         ![PyPi](https://img.shields.io/pypi/v/centerline-width)
         ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
         [![NSF-2141064](https://img.shields.io/badge/NSF-2141064-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2141064&HistoricalAwards=false)
         [![pytests](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml/badge.svg)](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml)
         
         Find the centerline and width of rivers based on the latitude and longitude positionss from the right and left bank 
@@ -190,15 +190,15 @@
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         ```
         
         ### Return Latitude/Longitude Coordinates of Centerline
-        Return the latitude/longtiude coordinates of the centerline based on the left and right banks
+        Return the latitude/longitude coordinates of the centerline based on the left and right banks
         ```
         river_object.centerlineLatitudeLongtiude
         ```
         Centerline coordinates are formed from Voronoi vertices
         
         ```python
         import centerline_width
@@ -392,26 +392,28 @@
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example1.png)
         In this example, the polygon is invalid, but with such a small overlap it is still able to find a valid path
         
         With limited data, the polygon will overlap more dramatically and will struggle to find a valid centerline:
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example4.png)
         
         ### Invalid Centerline
-        If the data is too small, a centerline and its coordinates cannot not be found (since only a single Voronoi vertex exists within the polygon and after deadends are filtered)
+        If the data is too small, a centerline and its coordinates cannot not be found (since only a single Voronoi vertex exists within the polygon and after dead ends are filtered)
         
-        `CRITICAL ERROR, Voronoi diagram generated too small to find centerline (no starting node found), unable to plot centerline. Set displayVoronoi=True to view. Can typically be fixed by adding more data to expand range.`
+        `CRITICAL ERROR, Polygon too short for the Voronoi diagram generated (no starting node found), unable to plot centerline. Set displayVoronoi=True to view vertices. Can typically be fixed by adding more data to expand range.`
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example2.png)
         Can be fixed by expanding the data until the polygon is large enough to contain at least two different vertex points
         
-        ### Invalid Top and Bottom Bank Postiions (flipDirection = True)
+        ### Invalid Top and Bottom Bank Postions (flipBankDirection = True)
+        Error: `Invalid Polygon Due to Flipped Banks, fix recommendation: rerun convertColumnsToCSV() and set flipBankDirection=True (or reset to default 'False' if currently set to flipBankDirection=True)`
+        
         If the data for the left and right river banks are generated in reverse order, they will be read in the incorrect order and the graph will find the invalid top and bottom of the bank
         
         If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
         
-        This can be fixed by using the flipDirection optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flipBankDirection=True)`
+        This can be fixed by using the flipBankDirection optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flipBankDirection=True)`
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/flipDirection_example.png)
         
         ### Fix Gaps and Jagged Centerlines
         Gaps formed can cause part of the centerline to be skipped due to sparse data. As a result, the start and end of the centerline can skip parts at the beginning or end of a river
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_short_path.png)
         Set river object created by `centerline_width.riverCenterline` to `interpolate_data=True` to fix for jagged edges or gaps formed by the interaction of sparse data and narrow banks
         ```python
@@ -437,15 +439,15 @@
         
          <p align="center">
           <img src="https://user-images.githubusercontent.com/22159116/222872092-e0b579cc-4f84-4f49-aa53-397785fb9bf2.png" />
           <img src="https://user-images.githubusercontent.com/22159116/222872119-7c485ee2-4ffd-413a-9e4f-b043b122d2bb.png" />
           <img src="https://user-images.githubusercontent.com/22159116/222872019-12931138-9e10-4e51-aa1e-552e72d09af0.png" />
         </p>
         
-        This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the atuhors and do not neccessarily reflect the views of the National Science Foundation.
+        This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not necessarily reflect the views of the National Science Foundation.
         
         ## Bug and Feature Request
         
         Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/cyschneck/centerline-width/issues) or to ugschneck@gmail.com/cyschneck@gmail.com
         
 Keywords: geophysics,python,voronoi,networkx,centerline,centerline-extraction,centerline-detection,rivers,river-bank-length,river-bank,limnology,hydrology
 Platform: UNKNOWN
```

### Comparing `centerline-width-0.2.1/centerline_width.egg-info/SOURCES.txt` & `centerline-width-0.2.2/centerline_width.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.1/setup.py` & `centerline-width-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 # Python Package Setup
 from setuptools import setup, find_namespace_packages
 
-VERSION="0.2.1"
+VERSION="0.2.2"
 DESCRIPTION="A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank"
 
 with open("README.md", "r") as f:
 	long_description_readme = f.read()
 
 setup(
 	name="centerline-width",
```

