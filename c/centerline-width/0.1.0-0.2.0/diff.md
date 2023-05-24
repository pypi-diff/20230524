# Comparing `tmp/centerline-width-0.1.0.tar.gz` & `tmp/centerline-width-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/centerline-width-0.1.0.tar", last modified: Thu May 18 01:12:03 2023, max compression
+gzip compressed data, was "dist/centerline-width-0.2.0.tar", last modified: Wed May 24 02:49:06 2023, max compression
```

## Comparing `centerline-width-0.1.0.tar` & `centerline-width-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-18 01:12:03.219940 centerline-width-0.1.0/
--rw-rw-r--   0 user      (1000) user      (1000)    25284 2023-05-18 01:12:03.219940 centerline-width-0.1.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    21129 2023-05-17 22:01:39.000000 centerline-width-0.1.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-18 01:12:03.211959 centerline-width-0.1.0/centerline_width/
--rw-rw-r--   0 user      (1000) user      (1000)     1379 2023-05-17 02:00:43.000000 centerline-width-0.1.0/centerline_width/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    20385 2023-05-17 21:43:05.000000 centerline-width-0.1.0/centerline_width/centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)    10092 2023-05-17 22:00:01.000000 centerline-width-0.1.0/centerline_width/error_handling.py
--rw-rw-r--   0 user      (1000) user      (1000)     1683 2023-05-17 04:17:41.000000 centerline-width-0.1.0/centerline_width/getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)     8550 2023-05-15 20:31:09.000000 centerline-width-0.1.0/centerline_width/plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     4985 2023-05-15 20:27:53.000000 centerline-width-0.1.0/centerline_width/preprocessing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-18 01:12:03.219940 centerline-width-0.1.0/centerline_width/pytests/
--rw-rw-r--   0 user      (1000) user      (1000)     6697 2023-05-17 22:00:19.000000 centerline-width-0.1.0/centerline_width/pytests/test_centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)     3981 2023-05-17 04:23:14.000000 centerline-width-0.1.0/centerline_width/pytests/test_getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)    11026 2023-05-17 04:31:11.000000 centerline-width-0.1.0/centerline_width/pytests/test_plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-0.1.0/centerline_width/pytests/test_preprocessing.py
--rw-rw-r--   0 user      (1000) user      (1000)     2078 2023-05-17 04:34:35.000000 centerline-width-0.1.0/centerline_width/pytests/test_riverCenterlineClass.py
--rw-rw-r--   0 user      (1000) user      (1000)     3865 2023-05-17 21:19:02.000000 centerline-width-0.1.0/centerline_width/riverCenterlineClass.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-18 01:12:03.215949 centerline-width-0.1.0/centerline_width.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    25284 2023-05-18 01:12:03.000000 centerline-width-0.1.0/centerline_width.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      700 2023-05-18 01:12:03.000000 centerline-width-0.1.0/centerline_width.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-18 01:12:03.000000 centerline-width-0.1.0/centerline_width.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      133 2023-05-18 01:12:03.000000 centerline-width-0.1.0/centerline_width.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       17 2023-05-18 01:12:03.000000 centerline-width-0.1.0/centerline_width.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-18 01:12:03.219940 centerline-width-0.1.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1746 2023-05-18 01:11:03.000000 centerline-width-0.1.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 02:49:06.533476 centerline-width-0.2.0/
+-rw-rw-r--   0 user      (1000) user      (1000)    30825 2023-05-24 02:49:06.533476 centerline-width-0.2.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    26055 2023-05-24 02:34:24.000000 centerline-width-0.2.0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 02:49:06.529477 centerline-width-0.2.0/centerline_width/
+-rw-rw-r--   0 user      (1000) user      (1000)     1382 2023-05-23 20:44:39.000000 centerline-width-0.2.0/centerline_width/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    20854 2023-05-23 21:37:54.000000 centerline-width-0.2.0/centerline_width/centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10712 2023-05-19 19:55:06.000000 centerline-width-0.2.0/centerline_width/error_handling.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1854 2023-05-18 02:15:59.000000 centerline-width-0.2.0/centerline_width/getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8345 2023-05-24 02:25:01.000000 centerline-width-0.2.0/centerline_width/plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6427 2023-05-23 07:06:34.000000 centerline-width-0.2.0/centerline_width/preprocessing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 02:49:06.533476 centerline-width-0.2.0/centerline_width/pytests/
+-rw-rw-r--   0 user      (1000) user      (1000)     6697 2023-05-17 22:00:19.000000 centerline-width-0.2.0/centerline_width/pytests/test_centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3981 2023-05-17 04:23:14.000000 centerline-width-0.2.0/centerline_width/pytests/test_getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11026 2023-05-17 04:31:11.000000 centerline-width-0.2.0/centerline_width/pytests/test_plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-0.2.0/centerline_width/pytests/test_preprocessing.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3397 2023-05-19 19:58:39.000000 centerline-width-0.2.0/centerline_width/pytests/test_riverCenterlineClass.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4569 2023-05-23 21:32:40.000000 centerline-width-0.2.0/centerline_width/riverCenterlineClass.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 02:49:06.533476 centerline-width-0.2.0/centerline_width.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    30825 2023-05-24 02:49:06.000000 centerline-width-0.2.0/centerline_width.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      700 2023-05-24 02:49:06.000000 centerline-width-0.2.0/centerline_width.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-24 02:49:06.000000 centerline-width-0.2.0/centerline_width.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      133 2023-05-24 02:49:06.000000 centerline-width-0.2.0/centerline_width.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2023-05-24 02:49:06.000000 centerline-width-0.2.0/centerline_width.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-24 02:49:06.533476 centerline-width-0.2.0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1813 2023-05-24 02:47:47.000000 centerline-width-0.2.0/setup.py
```

### Comparing `centerline-width-0.1.0/PKG-INFO` & `centerline-width-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 0.1.0
-Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude from a right and left bank
+Version: 0.2.0
+Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
-Author: Una Schneck (unaschneck), C. Y. Schneck (cyschneck)
+Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.1.0.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.2.0.tar.gz
 Description: # Centerline-Width
         ![PyPi](https://img.shields.io/pypi/v/centerline-width)
         ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
         [![NSF-2141064](https://img.shields.io/badge/NSF-2141064-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2141064&HistoricalAwards=false)
         [![pytests](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml/badge.svg)](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml)
         
         Find the centerline and width of rivers based on the latitude and longitude positionss from the right and left bank 
         
         * **Convert raw data from Google Earth Pro to CSV**
         	* extractPointsToTextFile()
         	* convertColumnsToCSV()
         * **Find centerline and width of river**
-        	* centerlineLatitudeLongitude()
         	* plotCenterline()
         	* plotCenterlineWidth()
         	* riverWidthFromCenterline()
+        	* centerlineLatitudeLongtiude
+        	* centerlineLength
+        	* rightBankLength
+        	* leftBankLength
         
         | River Outlined in Google Earth Pro | Generated Centerline for the River Bank |
         | ------------- | ------------- |
         | ![river_google_earth+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example_google_earth.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example.png) |
         
         Python implementation of [R-Code CMGO](https://github.com/AntoniusGolly/cmgo) (with modification)
         
@@ -41,14 +44,42 @@
         
         ## Install
         PyPi pip install at [pypi.org/project/centerline-width/](https://pypi.org/project/centerline-width/)
         
         ```
         pip install centerline-width
         ```
+        ## Quickstart: centerline-width
+        
+        The core of centerline-width works with a .csv file of the left and right bank latitude/longitudes. Starting with Google Earth Pro, two .kml must first be translated to a single .csv file
+        
+        ```python
+        import centerline_width
+        centerline_width.extractPointsToTextFile(left_kml="left_bank.kml",
+        					right_kml="right_bank.kml",
+        					text_output_name="river_coordinates_output.txt")
+        centerline_width.convertColumnsToCSV(text_file="river_coordinates_output.txt")
+        ```
+        Then, to run the centerline-width functions, generate a river object from the `river_coordinates_output.csv`
+        
+        ```python
+        river_object = centerline_width.riverCenterline(csv_data="river_coordinates_output.csv")
+        ```
+        
+        To plot the centerline, run the `plotCenterline()` function from `river_object` created
+        ```python
+        river_object.plotCenterline()
+        ```
+        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/river_coords_centerline.png)
+        
+        To plot the width of the river at intervals along the bank, run `plotCenterlineWidth` (apply_smoothing is optional and defaults to False, but is recommended)
+        ```python
+        river_object.plotCenterlineWidth(apply_smoothing=True)
+        ```
+        ![river_coords_width+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/river_coords_width.png)
         
         ## Preprocessing
         ### Convert KML files to Text File
         
         Convert two .kml files from Google Earth Pro (for the left and right bank) and export the coordinates into a text file
         
         ```
@@ -114,44 +145,55 @@
         30.037648,-92.868546,30.037482,-92.867449
         30.037674,-92.868536,30.037506,-92.867432
         30.037702,-92.868533,30.037525,-92.867430
         ```
         Output: A csv file `data/river_coords.csv` with the headers llat, llon, rlat, rlon
         
         ## Centerline and Width
-        
-        ### Types of Centerlines
-        - Voronoi centerline: centerline generated from where Voronoi vertices intersect within the river
-        - Evenly Spaced Centerline: centerline based on Voronoi centerline but evenly spaced with a fixed number of points
-        - Smoothed Centerline: centerline generated from the evenly spaced centerline but smoothed by a b-spline
-        
         ### River Object
         First, generate a river object to contain river data and available transformations
         ```
-        centerline_width.riverCenterline(csv_data=None, optional_cutoff=None)
+        centerline_width.riverCenterline(csv_data=None,
+        				optional_cutoff=None,
+        				interpolate_data=False,
+        				interpolate_n=5)
         ```
         * **[REQUIRED]** csv_data (string): File location of the text file to convert
         * [OPTIONAL] optional_cutoff (int): Include only the first x amount of the data to chart (useful for debugging)
+        * [OPTIONAL] interpolate_data (bool): Interpolate between existing data by adding additional points
+        * [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
+        
+        Interpolating is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps dues to the combination of sparse data and a narrow river
+        
+        Object (class) useful attributes:
         
-        Object (class) attributes:
+        * centerlineLatitudeLongtiude (list of tuples): List of the latitude and longitude coordinates of the centerline
+        * centerlineLength (float): Length of the centerline of the river (in km)
+        * rightBankLength (float): Length of the right bank of the river (in km)
+        * leftBankLength (float): Length of the left bank of the river (in km)
+        
+        Object (class) additional atttributes:
         
         * river_name (string): name of object, set to the csv_data string
-        * df_len (int): length of the dataframe of the csv data spliced by the optional_cutoff
-        * left_bank_coordinates (list of two element lists): list of coordiantes of the left bank generated from the csv file
-        * right_bank_coordinates (list of two element lists) list of coordinates of the right bank generated from the csv file
-        * river_bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate river bank (used to define an inside and an outside of the river)
-        * top_bank (Shapley Linestring): A linestring that represents the top of the river/polygon
-        * bottom_bank (Shapley Linestring): A linestring that represents the bottom of the river/polygon
-        * starting_node (tuple): Tuple of the starting position of the centerline path
-        * ending_node (tuple): Tuple of the end position of the centerline path
-        * river_bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
-        * centerline_latitude_longtiude (list of two element tuples): Latitude and Longitude coordinates of the centerline
-        * centerline_length (float): Length of the centerline of the river (in km)
+        * left_bank_coordinates (list of tuples): list of coordinates of the left bank generated from the csv file (`[(x, y), (x, y)]`)
+        * right_bank_coordinates (list of tuples) list of coordinates of the right bank generated from the csv file (`[(x, y), (x, y)]`)
+        * df_len (int): Length of the dataframe of the csv data spliced by the optional_cutoff
+        * bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate river bank (used to define an inside and an outside of the river)
+        * top_bank (Shapley Linestring): Linestring that represents the top of the river/polygon
+        * bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon
+        * starting_node (tuple): Tuple of the starting position (latitude and longitude) of the centerline path
+        * ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
+        * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
+        * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
+        * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Longitude position to ending Longitude position)
+        * interpolate_data (bool): if interpolating between existing data, defaults to False
+        * interpolate_n (int): specifies how many additional points will be added when interpolating data, defaults to 5
         
-        ```
+        ```python
+        import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         ```
         
         ### Return Latitude/Longitude Coordinates of Centerline
         Return the latitude/longtiude coordinates of the centerline based on the left and right banks
         ```
         river_object.centerline_latitude_longtiude
@@ -172,15 +214,15 @@
         ```
         Length returned in kilometers
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=550)
         river_centerline_length = river_object.centerline_length
         ```
-        The length of the river object returns `215.34700589636674` km
+        The length of the river centerline returns `215.34700589636674` km
         
         ## Plot Centerline in Matplotlib
         ### Plot the centerline created from a list of right and left banks with Voronoi vertices
         
         ```
         plotCenterline(display_all_possible_paths=False, 
         		plot_title=None, 
@@ -251,20 +293,20 @@
         | ------------- | ------------- |
         | ![river_keep+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_keep_intersections.png) | ![river_remove+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_remove_intersections.png)|
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.plotCenterlineWidth(save_plot_name="data/river_coords_width.png",
-        					display_true_centerline=False,
-        					n_interprolate_centerpoints=None,
-        					transect_span_distance=3,
-        					apply_smoothing=True,
-        					flag_intersections=True,
-        					remove_intersections=True)
+        				display_true_centerline=False,
+        				n_interprolate_centerpoints=None,
+        				transect_span_distance=3,
+        				apply_smoothing=True,
+        				flag_intersections=True,
+        				remove_intersections=True)
         ```
         ![river_coords_width+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/river_coords_width.png)
         
         ### Return Width of River
         
         Return the width of the river at each (evenly spaced) centerline coordinate
         
@@ -306,14 +348,15 @@
         ### Generate a Voronoi based on the points along the river banks
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example3.png)
         
         ### Display Voronoi ridge vertices that lie within the polygon (within the river banks)
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example4.png)
         
         ### Filter out any point pairs that only have one connections to filter out the short dead end paths and find the starting and ending node based on distance from the top and bottom of polygon
+        With the vertices removed, it is possible form multiple unconnected graphs within the polygon. The largest subgraph is assumed to contain the centerline and the other subgraphs are filtered out
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example6.png)
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example7.png)
         
         ### Find the shortest path from the starting node to the ending node ([Dijkstra's Algorithm](https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.shortest_paths.generic.shortest_path.html#networkx.algorithms.shortest_paths.generic.shortest_path))
         | Points on River Bank | NetworkX Graph of Points on River Bank |
         | ------------- | ------------- |
         | ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example10.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example9.png) |
@@ -327,37 +370,64 @@
         
         **All vertices:**
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example4.png)
         
         **Vertices that have at least two connections (that would create gaps):**
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example5.png)
         
+        ### Types of Centerlines
+        - Voronoi centerline: centerline generated from where Voronoi vertices intersect within the river
+        - Evenly Spaced Centerline: centerline based on Voronoi centerline but evenly spaced with a fixed number of points
+        - Smoothed Centerline: centerline generated from the evenly spaced centerline but smoothed by a b-spline
+        
         ## Debugging, Error Handling, and Edge Cases
-        ### Edge Cases
-        If the data starts with a large width, it is possible for the starting node to be invalid
+        ### Wide Start/End of River
+        If the data starts or ends with a large width, it is possible for the starting/ending nodes to end up in the wrong position
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example3.png)
-        Currently, the starting node is determined by the closest node to the top of the bank (in green) and the ending node is determined by the closest node to the bottom of the bank (in red)
+        Currently, the starting node is determined by the closest node to the top of the bank (in green) and the ending node is determined by the closest node to the bottom of the bank (in red) that sits along the longest path
         
         ### Invalid Polygon
+        A polygon is formed to encapsulate the river with the given data (to determine the inside and outside of the river). The top and bottom are connected by a straight line from the start/end of the available data. As a result, it is possible for this straight line to overlap and create an invalid polygon.
+        
         A polygon is invalid if it overlaps within itself:
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example1.png)
         In this example, the polygon is invalid, but with such a small overlap it is still able to find a valid path
         
-        With limited data, the polygon will overlap more dramatically and will no longer be able to find a valid centerline:
+        With limited data, the polygon will overlap more dramatically and will struggle to find a valid centerline:
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example4.png)
         
         ### Invalid Centerline
         If the data is too small, a centerline and its coordinates cannot not be found (since only a single Voronoi vertex exists within the polygon and after deadends are filtered)
         
         `CRITICAL ERROR, Voronoi diagram generated too small to find centerline (no starting node found), unable to plot centerline. Set displayVoronoi=True to view. Can typically be fixed by adding more data to expand range.`
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example2.png)
         Can be fixed by expanding the data until the polygon is large enough to contain at least two different vertex points
         
+        ### Invalid Top and Bottom Bank Postiions (flipDirection = True)
+        If the data for the left and right river banks are generated in reverse order, they will be read in the incorrect order and the graph will find the invalid top and bottom of the bank
+        
+        If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
+        
+        This can be fixed by using the flipDirection optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flipBankDirection=True)`
+        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/flipDirection_example.png)
+        
+        ### Fix Gaps and Jagged Centerlines
+        Gaps formed can cause part of the centerline to be skipped due to sparse data. As a result, the start and end of the centerline can skip parts at the beginning or end of a river
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_short_path.png)
+        Set river object created by `centerline_width.riverCenterline` to `interpolate_data=True` to fix for jagged edges or gaps formed by the interaction of sparse data and narrow banks
+        ```python
+        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", interpolate_data=True)
+        ```
+        | interpolate_data = False | interpolate_data = True |
+        | ------------- | ------------- |
+        | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps.png) |
+        
+        The amount of additional points added by interpolating can be adjusted with `interpolate_n`, but defaults to add 5 additional points between values
+        
         ## Developer Notes: Tech Debt and Bug Fixes
-        * Return the length of the left/right bank in riverCenterline class (right_bank_length, left_bank_length)
         * Verify that smoothing filter option does not produce a line that goes outside of the polygon
         * Return the knickpoints (occurrences of knickpoints)
         
         ## Citations
         Based on work written in R (Golly et al. 2017):
         
         >Golly, A. and Turowski, J. M.: Deriving principal channel metrics from bank and long-profile geometry with the R package cmgo, Earth Surf. Dynam., 5, 557-570, https://doi.org/10.5194/esurf-5-557-2017, 2017.
@@ -372,17 +442,17 @@
         
         This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the atuhors and do not neccessarily reflect the views of the National Science Foundation.
         
         ## Bug and Feature Request
         
         Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/cyschneck/centerline-width/issues) or to ugschneck@gmail.com/cyschneck@gmail.com
         
-Keywords: geophysics,python,voronoi,centerline,centerline-extraction,river-bank,limnology,hydrology
+Keywords: geophysics,python,voronoi,networkx,centerline,centerline-extraction,centerline-detection,rivers,river-bank-length,river-bank,limnology,hydrology
 Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Education
```

### Comparing `centerline-width-0.1.0/README.md` & `centerline-width-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -6,18 +6,21 @@
 
 Find the centerline and width of rivers based on the latitude and longitude positionss from the right and left bank 
 
 * **Convert raw data from Google Earth Pro to CSV**
 	* extractPointsToTextFile()
 	* convertColumnsToCSV()
 * **Find centerline and width of river**
-	* centerlineLatitudeLongitude()
 	* plotCenterline()
 	* plotCenterlineWidth()
 	* riverWidthFromCenterline()
+	* centerlineLatitudeLongtiude
+	* centerlineLength
+	* rightBankLength
+	* leftBankLength
 
 | River Outlined in Google Earth Pro | Generated Centerline for the River Bank |
 | ------------- | ------------- |
 | ![river_google_earth+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example_google_earth.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example.png) |
 
 Python implementation of [R-Code CMGO](https://github.com/AntoniusGolly/cmgo) (with modification)
 
@@ -33,14 +36,42 @@
 
 ## Install
 PyPi pip install at [pypi.org/project/centerline-width/](https://pypi.org/project/centerline-width/)
 
 ```
 pip install centerline-width
 ```
+## Quickstart: centerline-width
+
+The core of centerline-width works with a .csv file of the left and right bank latitude/longitudes. Starting with Google Earth Pro, two .kml must first be translated to a single .csv file
+
+```python
+import centerline_width
+centerline_width.extractPointsToTextFile(left_kml="left_bank.kml",
+					right_kml="right_bank.kml",
+					text_output_name="river_coordinates_output.txt")
+centerline_width.convertColumnsToCSV(text_file="river_coordinates_output.txt")
+```
+Then, to run the centerline-width functions, generate a river object from the `river_coordinates_output.csv`
+
+```python
+river_object = centerline_width.riverCenterline(csv_data="river_coordinates_output.csv")
+```
+
+To plot the centerline, run the `plotCenterline()` function from `river_object` created
+```python
+river_object.plotCenterline()
+```
+![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/river_coords_centerline.png)
+
+To plot the width of the river at intervals along the bank, run `plotCenterlineWidth` (apply_smoothing is optional and defaults to False, but is recommended)
+```python
+river_object.plotCenterlineWidth(apply_smoothing=True)
+```
+![river_coords_width+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/river_coords_width.png)
 
 ## Preprocessing
 ### Convert KML files to Text File
 
 Convert two .kml files from Google Earth Pro (for the left and right bank) and export the coordinates into a text file
 
 ```
@@ -106,44 +137,55 @@
 30.037648,-92.868546,30.037482,-92.867449
 30.037674,-92.868536,30.037506,-92.867432
 30.037702,-92.868533,30.037525,-92.867430
 ```
 Output: A csv file `data/river_coords.csv` with the headers llat, llon, rlat, rlon
 
 ## Centerline and Width
-
-### Types of Centerlines
-- Voronoi centerline: centerline generated from where Voronoi vertices intersect within the river
-- Evenly Spaced Centerline: centerline based on Voronoi centerline but evenly spaced with a fixed number of points
-- Smoothed Centerline: centerline generated from the evenly spaced centerline but smoothed by a b-spline
-
 ### River Object
 First, generate a river object to contain river data and available transformations
 ```
-centerline_width.riverCenterline(csv_data=None, optional_cutoff=None)
+centerline_width.riverCenterline(csv_data=None,
+				optional_cutoff=None,
+				interpolate_data=False,
+				interpolate_n=5)
 ```
 * **[REQUIRED]** csv_data (string): File location of the text file to convert
 * [OPTIONAL] optional_cutoff (int): Include only the first x amount of the data to chart (useful for debugging)
+* [OPTIONAL] interpolate_data (bool): Interpolate between existing data by adding additional points
+* [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
+
+Interpolating is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps dues to the combination of sparse data and a narrow river
+
+Object (class) useful attributes:
 
-Object (class) attributes:
+* centerlineLatitudeLongtiude (list of tuples): List of the latitude and longitude coordinates of the centerline
+* centerlineLength (float): Length of the centerline of the river (in km)
+* rightBankLength (float): Length of the right bank of the river (in km)
+* leftBankLength (float): Length of the left bank of the river (in km)
+
+Object (class) additional atttributes:
 
 * river_name (string): name of object, set to the csv_data string
-* df_len (int): length of the dataframe of the csv data spliced by the optional_cutoff
-* left_bank_coordinates (list of two element lists): list of coordiantes of the left bank generated from the csv file
-* right_bank_coordinates (list of two element lists) list of coordinates of the right bank generated from the csv file
-* river_bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate river bank (used to define an inside and an outside of the river)
-* top_bank (Shapley Linestring): A linestring that represents the top of the river/polygon
-* bottom_bank (Shapley Linestring): A linestring that represents the bottom of the river/polygon
-* starting_node (tuple): Tuple of the starting position of the centerline path
-* ending_node (tuple): Tuple of the end position of the centerline path
-* river_bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
-* centerline_latitude_longtiude (list of two element tuples): Latitude and Longitude coordinates of the centerline
-* centerline_length (float): Length of the centerline of the river (in km)
+* left_bank_coordinates (list of tuples): list of coordinates of the left bank generated from the csv file (`[(x, y), (x, y)]`)
+* right_bank_coordinates (list of tuples) list of coordinates of the right bank generated from the csv file (`[(x, y), (x, y)]`)
+* df_len (int): Length of the dataframe of the csv data spliced by the optional_cutoff
+* bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate river bank (used to define an inside and an outside of the river)
+* top_bank (Shapley Linestring): Linestring that represents the top of the river/polygon
+* bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon
+* starting_node (tuple): Tuple of the starting position (latitude and longitude) of the centerline path
+* ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
+* bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
+* x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
+* y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Longitude position to ending Longitude position)
+* interpolate_data (bool): if interpolating between existing data, defaults to False
+* interpolate_n (int): specifies how many additional points will be added when interpolating data, defaults to 5
 
-```
+```python
+import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 ```
 
 ### Return Latitude/Longitude Coordinates of Centerline
 Return the latitude/longtiude coordinates of the centerline based on the left and right banks
 ```
 river_object.centerline_latitude_longtiude
@@ -164,15 +206,15 @@
 ```
 Length returned in kilometers
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=550)
 river_centerline_length = river_object.centerline_length
 ```
-The length of the river object returns `215.34700589636674` km
+The length of the river centerline returns `215.34700589636674` km
 
 ## Plot Centerline in Matplotlib
 ### Plot the centerline created from a list of right and left banks with Voronoi vertices
 
 ```
 plotCenterline(display_all_possible_paths=False, 
 		plot_title=None, 
@@ -243,20 +285,20 @@
 | ------------- | ------------- |
 | ![river_keep+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_keep_intersections.png) | ![river_remove+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_remove_intersections.png)|
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_object.plotCenterlineWidth(save_plot_name="data/river_coords_width.png",
-					display_true_centerline=False,
-					n_interprolate_centerpoints=None,
-					transect_span_distance=3,
-					apply_smoothing=True,
-					flag_intersections=True,
-					remove_intersections=True)
+				display_true_centerline=False,
+				n_interprolate_centerpoints=None,
+				transect_span_distance=3,
+				apply_smoothing=True,
+				flag_intersections=True,
+				remove_intersections=True)
 ```
 ![river_coords_width+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/river_coords_width.png)
 
 ### Return Width of River
 
 Return the width of the river at each (evenly spaced) centerline coordinate
 
@@ -298,14 +340,15 @@
 ### Generate a Voronoi based on the points along the river banks
 ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example3.png)
 
 ### Display Voronoi ridge vertices that lie within the polygon (within the river banks)
 ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example4.png)
 
 ### Filter out any point pairs that only have one connections to filter out the short dead end paths and find the starting and ending node based on distance from the top and bottom of polygon
+With the vertices removed, it is possible form multiple unconnected graphs within the polygon. The largest subgraph is assumed to contain the centerline and the other subgraphs are filtered out
 ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example6.png)
 ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example7.png)
 
 ### Find the shortest path from the starting node to the ending node ([Dijkstra's Algorithm](https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.shortest_paths.generic.shortest_path.html#networkx.algorithms.shortest_paths.generic.shortest_path))
 | Points on River Bank | NetworkX Graph of Points on River Bank |
 | ------------- | ------------- |
 | ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example10.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example9.png) |
@@ -319,37 +362,64 @@
 
 **All vertices:**
 ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example4.png)
 
 **Vertices that have at least two connections (that would create gaps):**
 ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example5.png)
 
+### Types of Centerlines
+- Voronoi centerline: centerline generated from where Voronoi vertices intersect within the river
+- Evenly Spaced Centerline: centerline based on Voronoi centerline but evenly spaced with a fixed number of points
+- Smoothed Centerline: centerline generated from the evenly spaced centerline but smoothed by a b-spline
+
 ## Debugging, Error Handling, and Edge Cases
-### Edge Cases
-If the data starts with a large width, it is possible for the starting node to be invalid
+### Wide Start/End of River
+If the data starts or ends with a large width, it is possible for the starting/ending nodes to end up in the wrong position
 ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example3.png)
-Currently, the starting node is determined by the closest node to the top of the bank (in green) and the ending node is determined by the closest node to the bottom of the bank (in red)
+Currently, the starting node is determined by the closest node to the top of the bank (in green) and the ending node is determined by the closest node to the bottom of the bank (in red) that sits along the longest path
 
 ### Invalid Polygon
+A polygon is formed to encapsulate the river with the given data (to determine the inside and outside of the river). The top and bottom are connected by a straight line from the start/end of the available data. As a result, it is possible for this straight line to overlap and create an invalid polygon.
+
 A polygon is invalid if it overlaps within itself:
 ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example1.png)
 In this example, the polygon is invalid, but with such a small overlap it is still able to find a valid path
 
-With limited data, the polygon will overlap more dramatically and will no longer be able to find a valid centerline:
+With limited data, the polygon will overlap more dramatically and will struggle to find a valid centerline:
 ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example4.png)
 
 ### Invalid Centerline
 If the data is too small, a centerline and its coordinates cannot not be found (since only a single Voronoi vertex exists within the polygon and after deadends are filtered)
 
 `CRITICAL ERROR, Voronoi diagram generated too small to find centerline (no starting node found), unable to plot centerline. Set displayVoronoi=True to view. Can typically be fixed by adding more data to expand range.`
 ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example2.png)
 Can be fixed by expanding the data until the polygon is large enough to contain at least two different vertex points
 
+### Invalid Top and Bottom Bank Postiions (flipDirection = True)
+If the data for the left and right river banks are generated in reverse order, they will be read in the incorrect order and the graph will find the invalid top and bottom of the bank
+
+If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
+
+This can be fixed by using the flipDirection optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flipBankDirection=True)`
+![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/flipDirection_example.png)
+
+### Fix Gaps and Jagged Centerlines
+Gaps formed can cause part of the centerline to be skipped due to sparse data. As a result, the start and end of the centerline can skip parts at the beginning or end of a river
+![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_short_path.png)
+Set river object created by `centerline_width.riverCenterline` to `interpolate_data=True` to fix for jagged edges or gaps formed by the interaction of sparse data and narrow banks
+```python
+river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", interpolate_data=True)
+```
+| interpolate_data = False | interpolate_data = True |
+| ------------- | ------------- |
+| ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps.png) |
+
+The amount of additional points added by interpolating can be adjusted with `interpolate_n`, but defaults to add 5 additional points between values
+
 ## Developer Notes: Tech Debt and Bug Fixes
-* Return the length of the left/right bank in riverCenterline class (right_bank_length, left_bank_length)
 * Verify that smoothing filter option does not produce a line that goes outside of the polygon
 * Return the knickpoints (occurrences of knickpoints)
 
 ## Citations
 Based on work written in R (Golly et al. 2017):
 
 >Golly, A. and Turowski, J. M.: Deriving principal channel metrics from bank and long-profile geometry with the R package cmgo, Earth Surf. Dynam., 5, 557-570, https://doi.org/10.5194/esurf-5-557-2017, 2017.
```

### Comparing `centerline-width-0.1.0/centerline_width/__init__.py` & `centerline-width-0.2.0/centerline_width/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 
 # preprocessing.py function calls
 from .preprocessing import convertColumnsToCSV
 from .preprocessing import leftRightCoordinates
 from .preprocessing import generatePolygon
 from .preprocessing import generateVoronoi
 from .preprocessing import pointsFromVoronoi
+from .preprocessing import interpolateBetweenPoints
 
 # riverObject.py function calls
 from .riverCenterlineClass import riverCenterline
 
 # centerline.py function calls
 from .centerline import centerlinePath
 from .centerline import networkXGraphShortestPath
 from .centerline import centerlineLength
 from .centerline import evenlySpacedCenterline
 from .centerline import smoothedCoordinates
-from .centerline import returnShortestPathPoints
 from .centerline import riverWidthFromCenterlineCoordinates
 from .centerline import riverWidthFromCenterline
 
 # plotDiagrams.py function calls
 from .plotDiagrams import plotCenterline
 from .plotDiagrams import plotCenterlineWidth
```

### Comparing `centerline-width-0.1.0/centerline_width/centerline.py` & `centerline-width-0.2.0/centerline_width/centerline.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,91 +1,113 @@
 # Built in Python functions
 import math
 import logging
 import csv
 
 # External Python libraries (installed via pip install)
+from haversine import haversine
 import numpy as np
 import networkx as nx
 from scipy import interpolate
 from shapely.geometry import Point, LineString
-from haversine import haversine
 
 # Internal centerline_width reference to access functions, global variables, and error handling
 import centerline_width
 
 ## Logging set up for .INFO
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 stream_handler = logging.StreamHandler()
 logger.addHandler(stream_handler)
 
-def centerlinePath(river_voronoi, river_polygon, top_polygon_line, bottom_polygon_line):
-	# Return the starting node, ending node, all possible paths positions, and all paths starting/end position as a dictionary
-	start_end_points_dict = centerline_width.pointsFromVoronoi(river_voronoi, river_polygon) # All possible path connections from Voronoi
-	x_ridge_point = [] # X position on path
-	y_ridge_point = [] # Y poistion on path
-	starting_node = None # starting position at the top of the river
-	ending_node = None # ending position at the bottom of the river
-	for start_point, end_point_list in start_end_points_dict.items():
-		if len(end_point_list) > 0: # TESTING TESTING: Show only the end points that have multiple connections (set to 0 during production)
-			# Find the starting and ending node based on distance from the top and bottom of the polygon
-			if starting_node is None: starting_node = start_point
-			else:
-				if Point(start_point).distance(top_polygon_line) <= Point(starting_node).distance(top_polygon_line):
-					starting_node = start_point
-			for end_point in end_point_list:
-				if Point(end_point).distance(top_polygon_line) <= Point(starting_node).distance(top_polygon_line):
-					starting_node = end_point
-				if ending_node is None: ending_node = end_point
-				else:
-					if Point(start_point).distance(bottom_polygon_line) <= Point(ending_node).distance(bottom_polygon_line):
-						ending_node = start_point
-					if Point(end_point).distance(bottom_polygon_line) <= Point(ending_node).distance(bottom_polygon_line):
-						ending_node = end_point
-				# Save all starting and end positions for all possible paths
-				x_ridge_point.append([start_point[0], end_point[0]])
-				y_ridge_point.append([start_point[1], end_point[1]])
-
-	if starting_node is None:
-		logger.critical("\nCRITICAL ERROR, Voronoi diagram generated too small to find centerline (no starting node found), unable to plot centerline. Set displayVoronoi=True to view. Can typically be fixed by adding more data to expand range.")
-
-	return starting_node, ending_node, x_ridge_point, y_ridge_point, start_end_points_dict
-
-def networkXGraphShortestPath(all_points_dict, starting_node, ending_node):
+def generateNXGraph(all_points_dict):
+	# Generate a NetworkX graph to find the largest graph
 	def distanceBetween(start, end):
 		lat1 = start[0]
 		lat2 = end[0]
 		lon1 = start[1]
 		lon2 = end[1]
 		p = math.pi/180
 		a = 0.5 - math.cos((lat2-lat1)*p)/2 + math.cos(lat1*p) * math.cos(lat2*p) * (1-math.cos((lon2-lon1)*p))/2
 		return math.asin(math.sqrt(a))
 
+	all_connections_in_graph = nx.Graph()
+	node_as_keys_pos_values = {}
+	for start_point, end_point_list in all_points_dict.items():
+		node_as_keys_pos_values[start_point] = (start_point[0], start_point[1])
+		all_connections_in_graph.add_node(start_point, pos=(start_point[0], start_point[1]))
+		for end_point in end_point_list:
+			all_connections_in_graph.add_node(end_point, pos=(end_point[0], end_point[1]))
+			node_as_keys_pos_values[end_point] = (end_point[0], end_point[1])
+			all_connections_in_graph.add_edge(start_point, end_point, weight=distanceBetween(start_point,end_point))
+
+	components_of_subgraphs = [all_connections_in_graph.subgraph(c).copy() for c in nx.connected_components(all_connections_in_graph)]
+	nodes_of_largest_subgraph = []
+	for idx, g in enumerate(components_of_subgraphs, start=1):
+		if len(g.nodes()) > len(nodes_of_largest_subgraph):
+			nodes_of_largest_subgraph = list(g.nodes())
+		#print("Subgraph {0}: Nodes: {1}, Edges: {2}".format(idx, len(g.nodes()), len(g.edges())))
+
+	return all_connections_in_graph, nodes_of_largest_subgraph
+
+def networkXGraphShortestPath(nx_graph, starting_node, ending_node):
+	# Find the shortest path if it exists
 	if starting_node is not None:
-		graph_connections = nx.Graph()
-		node_as_keys_pos_values = {}
-		for start_point, end_point_list in all_points_dict.items():
-			node_as_keys_pos_values[start_point] = (start_point[0], start_point[1])
-			graph_connections.add_node(start_point, pos=(start_point[0], start_point[1]))
-			for end_point in end_point_list:
-				graph_connections.add_node(end_point, pos=(end_point[0], end_point[1]))
-				node_as_keys_pos_values[end_point] = (end_point[0], end_point[1])
-				graph_connections.add_edge(start_point, end_point, weight=distanceBetween(start_point,end_point))
 		try:
-			shortest_path = nx.shortest_path(graph_connections, source=starting_node, target=ending_node)
+			shortest_path = nx.shortest_path(nx_graph, source=starting_node, target=ending_node)
 			logger.info("[SUCCESS] Valid centerline path found")
 		except nx.NetworkXNoPath: # no direct path found
 			logger.info("[FAILED]  No direct path found from starting node to ending node")
 			return None
 		#nx.draw(graph_connections, with_labels=True, font_size=10)
 		return shortest_path
 	else:
 		return None
 
+def centerlinePath(river_voronoi, river_polygon, top_polygon_line, bottom_polygon_line):
+	# Return the starting node, ending node, all possible paths positions, and all paths starting/end position as a dictionary
+	start_end_points_dict = centerline_width.pointsFromVoronoi(river_voronoi, river_polygon) # All possible path connections from Voronoi
+	nx_graphs, largest_subgraph_nodes = generateNXGraph(start_end_points_dict)
+
+	x_ridge_point = [] # X position on path
+	y_ridge_point = [] # Y poistion on path
+	starting_node = None # starting position at the top of the river
+	ending_node = None # ending position at the bottom of the river
+	for start_point, end_point_list in start_end_points_dict.items():
+			if len(end_point_list) > 0: # TESTING TESTING: Show only the end points that have multiple connections (set to 0 during production)
+				# Find the starting and ending node based on distance from the top and bottom of the polygon
+				if starting_node is None: 
+					starting_node = start_point
+				else:
+					if start_point in largest_subgraph_nodes: # Only include if node is on the largest subgraph (that represents the centerline)
+						if Point(start_point).distance(top_polygon_line) <= Point(starting_node).distance(top_polygon_line):
+							starting_node = start_point
+				for end_point in end_point_list:
+					if start_point in largest_subgraph_nodes: # Only include if node is on the largest subgraph (that represents the centerline)
+						if Point(end_point).distance(top_polygon_line) <= Point(starting_node).distance(top_polygon_line):
+							starting_node = end_point
+						if ending_node is None: 
+							ending_node = end_point
+						else:
+							if Point(start_point).distance(bottom_polygon_line) <= Point(ending_node).distance(bottom_polygon_line):
+								ending_node = start_point
+							if Point(end_point).distance(bottom_polygon_line) <= Point(ending_node).distance(bottom_polygon_line):
+								ending_node = end_point
+					# Save all starting and end positions for all possible paths
+					x_ridge_point.append((start_point[0], end_point[0]))
+					y_ridge_point.append((start_point[1], end_point[1]))
+
+	if starting_node is None:
+		logger.critical("\nCRITICAL ERROR, Voronoi diagram generated too small to find centerline (no starting node found), unable to plot centerline. Set displayVoronoi=True to view. Can typically be fixed by adding more data to expand range.")
+		shortest_path_points = None
+	else:
+		shortest_path_points = networkXGraphShortestPath(nx_graphs, starting_node, ending_node)
+
+	return starting_node, ending_node, x_ridge_point, y_ridge_point, shortest_path_points
+
 def evenlySpacedCenterline(centerline_coordinates=None, number_of_fixed_points=10):
 	# Interpolate to evenly space points along the centerline coordinates (effectively smoothing with fewer points)
 	if centerline_coordinates is None:
 		return None
 
 	centerline_line = LineString(centerline_coordinates)
 
@@ -120,24 +142,14 @@
 	x_smoothed, y_smoothed =  interpolate.splev(u, tck) # interpolated list of points
 
 	x_smoothed, y_smoothed = x_smoothed.tolist(), y_smoothed.tolist() # convert array to list
 	smoothed_coordinates = list(zip(x_smoothed, y_smoothed))
 
 	return smoothed_coordinates
 
-def returnShortestPathPoints(river_voronoi=None, river_polygon=None, top_polygon_line=None, bottom_polygon_line=None):
-	# Find the centerline from NetworkX
-	starting_node, ending_node, x_ridge_point, y_ridge_point, start_end_points_dict = centerline_width.centerlinePath(river_voronoi=river_voronoi,
-																													river_polygon=river_polygon, 
-																													top_polygon_line=top_polygon_line, 
-																													bottom_polygon_line=bottom_polygon_line)
-
-	shortest_path_points = centerline_width.networkXGraphShortestPath(start_end_points_dict, starting_node, ending_node)
-	return shortest_path_points
-
 def riverWidthFromCenterlineCoordinates(river_object=None,
 										centerline_coordinates=None,
 										transect_span_distance=3,
 										remove_intersections=False,
 										save_to_csv=None):
 	# Return the left/right coordinates of width centerlines
 	right_width_coordinates = {}
@@ -309,23 +321,23 @@
 															units=units,
 															save_to_csv=save_to_csv)
 
 	if n_interprolate_centerpoints is None:
 		# if plotting width, but n_interprolate_centerpoints is undefined, set to the size of the dataframe
 		n_interprolate_centerpoints = river_object.df_len
 
-	if river_object.centerline_latitude_longtiude is None:
+	if river_object.centerlineLatitudeLongtiude is None:
 		logger.critical("\nCRITICAL ERROR, unable to find width without a valid centerline")
 		return None
 
 	# recreate the centerline with evenly spaced points
-	defined_centerline_coordinates = centerline_width.evenlySpacedCenterline(centerline_coordinates=river_object.centerline_latitude_longtiude,
+	defined_centerline_coordinates = centerline_width.evenlySpacedCenterline(centerline_coordinates=river_object.centerlineLatitudeLongtiude,
 																			number_of_fixed_points=n_interprolate_centerpoints)
 	if apply_smoothing:
-		defined_centerline_coordinates = centerline_width.smoothedCoordinates(centerline_coordinates=river_object.centerline_latitude_longtiude,
+		defined_centerline_coordinates = centerline_width.smoothedCoordinates(centerline_coordinates=river_object.centerlineLatitudeLongtiude,
 																				interprolate_num=n_interprolate_centerpoints)
 	# if using smoothing, replace left/right coordinates with the smoothed variation
 	right_width_coord, left_width_coord, _ = centerline_width.riverWidthFromCenterlineCoordinates(river_object=river_object, 
 																									centerline_coordinates=defined_centerline_coordinates,
 																									transect_span_distance=transect_span_distance,
 																									remove_intersections=remove_intersections)
 
@@ -348,15 +360,15 @@
 	return width_dict
 
 def centerlineLength(centerline_coordinates=None):
 	# Return the length/distance for all the centerline coordaintes in km
 	total_length = 0
 	previous_pair = None
 	if centerline_coordinates is None:
-		return None
+		return 0
 
 	for xy_pair in centerline_coordinates:
 		if previous_pair is None:
 			previous_pair = xy_pair
 		else:
 			lon1, lon2 = previous_pair[0], xy_pair[0]
 			lat1, lat2 = previous_pair[1], xy_pair[1]
```

### Comparing `centerline-width-0.1.0/centerline_width/error_handling.py` & `centerline-width-0.2.0/centerline_width/error_handling.py`

 * *Files 3% similar despite different names*

```diff
@@ -208,21 +208,32 @@
 		exit()
 	else:
 		if type(text_output_name) != str:
 			logger.critical("\nCRITICAL ERROR, [text_output_name]: Must be a str, current type = '{0}'".format(type(text_output_name)))
 			exit()
 
 ## Error Handling: riverCenterlineClass.py
-def errorHandlingRiverCenterlineClass(csv_data=None, optional_cutoff=None):
+def errorHandlingRiverCenterlineClass(csv_data=None, optional_cutoff=None, interpolate_data=None, interpolate_n=None):
 	# Error Handling for riverCenterlineClass()
 	if csv_data is None:
 		logger.critical("\nCRITICAL ERROR, [csv_data]: Requires csv_data location")
 		exit()
 	else:
-		if type(csv_data) != str and not isinstance(csv_data, StringIO):
+		if type(csv_data) != str and not isinstance(csv_data, StringIO): 
+			# StringIO accounts for testing against a StringIO instead of a CSV (used in pytests)
 			logger.critical("\nCRITICAL ERROR, [csv_data]: Must be a str, current type = '{0}'".format(type(csv_data)))
 			exit()
 
 	if optional_cutoff is not None:
 		if type(optional_cutoff) != int:
 			logger.critical("\nCRITICAL ERROR, [optional_cutoff]: Must be a int, current type = '{0}'".format(type(optional_cutoff)))
 			exit()
+
+	if type(interpolate_data) != bool:
+		logger.critical("\nCRITICAL ERROR, [interpolate_data]: Must be a bool, current type = '{0}'".format(type(interpolate_data)))
+		exit()
+
+	if type(interpolate_n) != int:
+		logger.critical("\nCRITICAL ERROR, [interpolate_n]: Must be a int, current type = '{0}'".format(type(interpolate_n)))
+		exit()
+		if interpolate_n > 15:
+			logger.warn("WARNING, [interpolate_n]: Setting interpolate_n above 15 will cause the code to execute exponentially slower")
```

### Comparing `centerline-width-0.1.0/centerline_width/getCoordinatesKML.py` & `centerline-width-0.2.0/centerline_width/getCoordinatesKML.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,27 +16,33 @@
 														text_output_name=text_output_name)
 
 	# extract points from kml file
 	with open(left_kml) as f:
 		doc = parser.parse(f)
 	root = doc.getroot()
 	coords = root.Document.Placemark.LineString.coordinates.text
-	lon = re.findall(r'(-[0-9]{2}\.[0-9]*)',coords)
-	lat = re.findall(r'[^-]([0-9]{2}\.[0-9]*)',coords)
-	llon = list([float(i) for i in lon])
-	llat = list([float(i) for i in lat])
-	
+	llon = []
+	llat = []
+	coords = coords.replace('\n', '').replace('\t', '')
+	for coord in coords.split(" "): # split coordinates based on commas (excluding preceding 0's)
+		if coord != "":
+			llon.append(coord.split(",")[0])
+			llat.append(coord.split(",")[1])
+
 	with open(right_kml) as f:
 		doc = parser.parse(f)
 	root = doc.getroot()
 	coords = root.Document.Placemark.LineString.coordinates.text
-	lon = re.findall(r'(-[0-9]{2}\.[0-9]*)',coords)
-	lat = re.findall(r'[^-]([0-9]{2}\.[0-9]*)',coords)
-	rlon = list([float(i) for i in lon])
-	rlat = list([float(i) for i in lat])
+	rlon = []
+	rlat = []
+	coords = coords.replace('\n', '').replace('\t', '')
+	for coord in coords.split(" "): # split coordinates based on commas (excluding preceding 0's)
+		if coord != "":
+			rlon.append(coord.split(",")[0])
+			rlat.append(coord.split(",")[1])
 
 	df_lb = pd.DataFrame({'llat':llat,'llon':llon})
 	df_rb = pd.DataFrame({'rlat':rlat,'rlon':rlon})
 	df = pd.concat([df_lb,df_rb],axis=1)
 
 	open(text_output_name, 'w').close() # empty original file to avoid overwriting
```

### Comparing `centerline-width-0.1.0/centerline_width/plotDiagrams.py` & `centerline-width-0.2.0/centerline_width/plotDiagrams.py`

 * *Files 20% similar despite different names*

```diff
@@ -37,28 +37,28 @@
 	for i in river_object.left_bank_coordinates:
 		x.append(i[0])
 		y.append(i[1])
 	plt.scatter(x, y, c="orange", s=scatter_plot_size, label="Left Bank")
 
 	# Plot centerline found from NetworkX
 	valid_path_through = False
-	if river_object.centerline_latitude_longtiude: # shortest path through points
+	if river_object.centerlineLatitudeLongtiude: # shortest path through points
 		valid_path_through = True
 		x = []
 		y = []
-		for k, v in river_object.centerline_latitude_longtiude:
+		for k, v in river_object.centerlineLatitudeLongtiude:
 			x.append(k)
 			y.append(v)
 		#plt.scatter(x, y, c="slategray", label="Centerline Coordinates", s=5)
-		plt.plot(*zip(*river_object.centerline_latitude_longtiude), c="black", label="Centerline")
+		plt.plot(*zip(*river_object.centerlineLatitudeLongtiude), c="black", label="Centerline")
 
 	# Dynamically assign the starting and ending
 	if river_object.starting_node is not None: # error handling for when data is too small to generate centerline coordiantes
-		plt.scatter(river_object.starting_node[0], river_object.starting_node[1], c="green", label="Starting Node", s=45)
-		plt.scatter(river_object.ending_node[0], river_object.ending_node[1], c="red", label="Ending Node", s=45)
+			plt.scatter(river_object.starting_node[0], river_object.starting_node[1], c="green", label="Starting Node", s=45)
+			plt.scatter(river_object.ending_node[0], river_object.ending_node[1], c="red", label="Ending Node", s=45)
 
 	return fig, ax, valid_path_through
 
 def plotCenterline(river_object=None,
 					display_all_possible_paths=False, 
 					plot_title=None, 
 					save_plot_name=None, 
@@ -70,27 +70,24 @@
 												save_plot_name=save_plot_name,
 												display_voronoi=display_voronoi)
 
 	fig, ax, valid_path_through = plotCenterlineBackend(river_object=river_object)
 
 	# Display the Voronoi Diagram
 	if display_voronoi:
-		voronoi_plot_2d(river_bank_voronoi, show_points=True, point_size=1, ax=ax)
+		voronoi_plot_2d(river_object.bank_voronoi, show_points=True, point_size=1, ax=ax)
 
 	# Plot all possible paths with text for positions
-	if display_all_possible_paths or not river_object.bank_polygon.is_valid: # display paths if polygon is not valid (debugging purposes)
-		for i in range(len(x_ridge_point)):
-			plt.plot(x_ridge_point[i], y_ridge_point[i], 'cyan', linewidth=1)
-			# Plot (X, Y) positions as text
-			#ax.text(x=x_ridge_point[i][0], y=y_ridge_point[i][0], s="{0}, {1}".format(x_ridge_point[i][0], y_ridge_point[i][0]))
-			#ax.text(x=x_ridge_point[i][1], y=y_ridge_point[i][1], s="{0}, {1}".format(x_ridge_point[i][1], y_ridge_point[i][1]))
+	if display_all_possible_paths:
+		for i in range(len(river_object.x_voronoi_ridge_point)):
+			plt.plot(river_object.x_voronoi_ridge_point[i], river_object.y_voronoi_ridge_point[i], 'cyan', linewidth=1)
 
 	# Plot Title, Legends, and Axis Labels
 	if not plot_title:
-		plt.title("River Coordinates: Valid Centerline = {0}, Valid Polygon = {1}".format(valid_path_through, river_object.bank_polygon.is_valid))
+		plt.title("River Coordinates: Valid Centerline = {0}, Valid Polygon = {1}, Interpolated = {2}".format(valid_path_through, river_object.bank_polygon.is_valid, river_object.interpolate_data))
 	else:
 		plt.title(plot_title)
 	plt.xlabel("Longitude (°)")
 	plt.ylabel("Latitude (°)")
 	plt.legend(loc="upper right")
 	plt.show()
 	if save_plot_name: fig.savefig(save_plot_name)
@@ -120,22 +117,23 @@
 	# Plot river
 	if n_interprolate_centerpoints is None:
 		# if plotting width, but n_interprolate_centerpoints is undefined, set to the size of the dataframe
 		n_interprolate_centerpoints = river_object.df_len
 
 	# Determine the Width of River
 	number_of_evenly_spaced_points = ""
-	if river_object.centerline_latitude_longtiude:
+
+	if river_object.centerlineLatitudeLongtiude is not None:
 		number_of_evenly_spaced_points = "\nCenterline made of {0} Fixed Points, width lines generated every {1} points".format(n_interprolate_centerpoints, transect_span_distance)
 		if river_object.starting_node is not None: # error handling for when data is too small to generate centerline coordiantes
 			# recreate the centerline with evenly spaced points
-			evenly_spaced_centerline_coordinates = centerline_width.evenlySpacedCenterline(centerline_coordinates=river_object.centerline_latitude_longtiude,
+			evenly_spaced_centerline_coordinates = centerline_width.evenlySpacedCenterline(centerline_coordinates=river_object.centerlineLatitudeLongtiude,
 																						number_of_fixed_points=n_interprolate_centerpoints)
 			if apply_smoothing:
-				smoothed_centerline_coordinates = centerline_width.smoothedCoordinates(centerline_coordinates=river_object.centerline_latitude_longtiude,
+				smoothed_centerline_coordinates = centerline_width.smoothedCoordinates(centerline_coordinates=river_object.centerlineLatitudeLongtiude,
 																						interprolate_num=n_interprolate_centerpoints)
 				# if using smoothing, replace left/right coordinates with the smoothed variation
 				right_width_coordinates, left_width_coordinates, num_intersection_coordinates = centerline_width.riverWidthFromCenterlineCoordinates(river_object=river_object,
 																																					centerline_coordinates=smoothed_centerline_coordinates,
 																																					transect_span_distance=transect_span_distance,
 																																					remove_intersections=remove_intersections)
 				x = []
@@ -177,15 +175,15 @@
 					else:
 						plt.plot(x_points, y_points, 'green', linewidth=1)
 				else:
 					plt.plot(x_points, y_points, 'green', linewidth=1)
 
 	# Plot Title, Legends, and Axis Labels
 	if not plot_title:
-		plt.title("River Width Coordinates: Valid Centerline = {0}, Valid Polygon = {1}{2}".format(valid_path_through, river_object.bank_polygon.is_valid, number_of_evenly_spaced_points))
+		plt.title("River Width Coordinates: Valid Centerline = {0}, Valid Polygon = {1}{2}, Interpolated = {3}".format(valid_path_through, river_object.bank_polygon.is_valid, number_of_evenly_spaced_points, river_object.interpolate_data))
 	else:
 		plt.title(plot_title)
 	plt.xlabel("Longitude (°)")
 	plt.ylabel("Latitude (°)")
 	plt.legend(loc="upper right")
 	plt.show()
 	if save_plot_name: fig.savefig(save_plot_name)
```

### Comparing `centerline-width-0.1.0/centerline_width/pytests/test_centerline.py` & `centerline-width-0.2.0/centerline_width/pytests/test_centerline.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.1.0/centerline_width/pytests/test_getCoordinatesKML.py` & `centerline-width-0.2.0/centerline_width/pytests/test_getCoordinatesKML.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.1.0/centerline_width/pytests/test_plotDiagrams.py` & `centerline-width-0.2.0/centerline_width/pytests/test_plotDiagrams.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.1.0/centerline_width/pytests/test_preprocessing.py` & `centerline-width-0.2.0/centerline_width/pytests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.1.0/centerline_width/pytests/test_riverCenterlineClass.py` & `centerline-width-0.2.0/centerline_width/pytests/test_riverCenterlineClass.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 
 # External Python libraries (installed via pip install)
 import pytest
 
 # Internal centerline-width reference to access functions, global variables, and error handling
 import centerline_width
 
+invalid_non_bool_options = [(1961, "<class 'int'>"),
+						(3.1415, "<class 'float'>"),
+						([], "<class 'list'>"),
+						("testing_string", "<class 'str'>")]
+
 invalid_non_int_options = [("testing_string", "<class 'str'>"),
 						(3.1415, "<class 'float'>"),
 						([], "<class 'list'>"),
 						(False, "<class 'bool'>")]
 
 invalid_non_str_options = [(1961, "<class 'int'>"),
 						(3.1415, "<class 'float'>"),
@@ -38,7 +43,23 @@
 @pytest.mark.parametrize("optional_cutoff_invalid, optional_cutoff_error_output", invalid_non_int_options)
 def test_riverCenterline_optionalCutoffInvalidTypes(caplog, optional_cutoff_invalid, optional_cutoff_error_output):
 	with pytest.raises(SystemExit):
 		centerline_width.riverCenterline(csv_data="csv_example.csv", optional_cutoff=optional_cutoff_invalid)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [optional_cutoff]: Must be a int, current type = '{0}'".format(optional_cutoff_error_output)
+
+@pytest.mark.parametrize("interpolate_data_invalid, interpolate_data_error_output", invalid_non_bool_options)
+def test_riverCenterline_interpolateDataInvalidTypes(caplog, interpolate_data_invalid, interpolate_data_error_output):
+	with pytest.raises(SystemExit):
+		centerline_width.riverCenterline(csv_data="csv_example.csv", interpolate_data=interpolate_data_invalid)
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [interpolate_data]: Must be a bool, current type = '{0}'".format(interpolate_data_error_output)
+
+@pytest.mark.parametrize("interpolate_n_invalid, interpolate_n_error_output", invalid_non_int_options)
+def test_riverCenterline_interpolateNInvalidTypes(caplog, interpolate_n_invalid, interpolate_n_error_output):
+	with pytest.raises(SystemExit):
+		centerline_width.riverCenterline(csv_data="csv_example.csv", interpolate_n=interpolate_n_invalid)
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [interpolate_n]: Must be a int, current type = '{0}'".format(interpolate_n_error_output)
```

### Comparing `centerline-width-0.1.0/centerline_width/riverCenterlineClass.py` & `centerline-width-0.2.0/centerline_width/riverCenterlineClass.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,67 +3,68 @@
 # External Python libraries (installed via pip install)
 import pandas as pd
 
 # Internal centerline_width reference to access functions, global variables, and error handling
 import centerline_width
 
 class riverCenterline:
-	def __init__(self, csv_data=None, optional_cutoff=None):
-		centerline_width.errorHandlingRiverCenterlineClass(csv_data=csv_data, optional_cutoff=optional_cutoff)
+	def __init__(self, csv_data=None, optional_cutoff=None, interpolate_data=False, interpolate_n=5):
+		centerline_width.errorHandlingRiverCenterlineClass(csv_data=csv_data,
+															optional_cutoff=optional_cutoff,
+															interpolate_data=interpolate_data,
+															interpolate_n=interpolate_n)
 
 		# Description and dataframe
 		self.river_name = csv_data
+		self.interpolate_data = interpolate_data
+		self.interpolate_n = interpolate_n
 		df = pd.read_csv(csv_data)
 		if optional_cutoff:
 			df = df.head(optional_cutoff)
 		self.df_len = len(df)
 
 		# Left and Right Coordinates from the given csv data and data cutoff
 		left_bank_coordinates, right_bank_coordinates = centerline_width.leftRightCoordinates(df)
+		if interpolate_data:
+			right_bank_coordinates, left_bank_coordinates = centerline_width.interpolateBetweenPoints(left_bank_coordinates, right_bank_coordinates, interpolate_n)
 		self.left_bank_coordinates = left_bank_coordinates
 		self.right_bank_coordinates = right_bank_coordinates
 
 		# River polygon, position of the top/bottom polygon
-		river_bank_polygon, top_bank, bottom_bank = centerline_width.generatePolygon(left_bank_coordinates, right_bank_coordinates)
+		river_bank_polygon, top_bank, bottom_bank = centerline_width.generatePolygon(self.left_bank_coordinates, self.right_bank_coordinates)
 		self.bank_polygon = river_bank_polygon
 		self.top_bank = top_bank
 		self.bottom_bank = bottom_bank
 
 		# Voronoi generated by left/right bank coordinates
-		river_bank_voronoi = centerline_width.generateVoronoi(left_bank_coordinates, right_bank_coordinates)
-		self.river_bank_voronoi = river_bank_voronoi
+		river_bank_voronoi = centerline_width.generateVoronoi(self.left_bank_coordinates, self.right_bank_coordinates)
+		self.bank_voronoi = river_bank_voronoi
 
 		# All possible paths: starting/ending node, all possible paths (ridges), paths dictionary
-		starting_node, ending_node, x_ridge_point, y_ridge_point, start_end_points_dict = centerline_width.centerlinePath(river_bank_voronoi, river_bank_polygon, top_bank, bottom_bank)
+		starting_node, ending_node, x_ridge_point, y_ridge_point, shortest_path_coordinates = centerline_width.centerlinePath(self.bank_voronoi, self.bank_polygon, self.top_bank, self.bottom_bank)
 		self.starting_node = starting_node # starting position for centerline
 		self.ending_node = ending_node # ending position for centerline
+		self.x_voronoi_ridge_point = x_ridge_point # Voronoi x positions
+		self.y_voronoi_ridge_point = y_ridge_point # Voronoi y postions
 
 		# Centerline coordinates
-		shortest_path_coordinates = centerline_width.networkXGraphShortestPath(start_end_points_dict, starting_node, ending_node)
-		self.centerline_latitude_longtiude = shortest_path_coordinates
+		self.centerlineLatitudeLongtiude = shortest_path_coordinates
 
-		# Centerline length
-		self.centerline_length = centerline_width.centerlineLength(centerline_coordinates=shortest_path_coordinates)
+		# Right/Length Bank Length
+		self.rightBankLength = centerline_width.centerlineLength(centerline_coordinates=right_bank_coordinates)
+		self.leftBankLength = centerline_width.centerlineLength(centerline_coordinates=left_bank_coordinates)
 
-	def riverWidthFromCenterline(self,
-								n_interprolate_centerpoints=None,
-								transect_span_distance=3,
-								apply_smoothing=True,
-								remove_intersections=False,
-								units="km",
-								save_to_csv=None):
-		return centerline_width.riverWidthFromCenterline(river_object=self,
-														n_interprolate_centerpoints=n_interprolate_centerpoints,
-														transect_span_distance=transect_span_distance,
-														apply_smoothing=apply_smoothing,
-														remove_intersections=remove_intersections,
-														units=units,
-														save_to_csv=save_to_csv)
+		# Centerline length
+		self.centerlineLength = centerline_width.centerlineLength(centerline_coordinates=shortest_path_coordinates)
 
-	def plotCenterline(self, display_all_possible_paths=False, plot_title=None, save_plot_name=None, display_voronoi=False):
+	def plotCenterline(self,
+						display_all_possible_paths=False,
+						plot_title=None,
+						save_plot_name=None,
+						display_voronoi=False):
 		centerline_width.plotCenterline(river_object=self,
 										display_all_possible_paths=display_all_possible_paths, 
 										plot_title=plot_title, 
 										save_plot_name=save_plot_name, 
 										display_voronoi=display_voronoi)
 
 	def plotCenterlineWidth(self,
@@ -80,7 +81,22 @@
 											save_plot_name=save_plot_name, 
 											display_true_centerline=display_true_centerline,
 											n_interprolate_centerpoints=n_interprolate_centerpoints,
 											transect_span_distance=transect_span_distance,
 											apply_smoothing=apply_smoothing,
 											flag_intersections=flag_intersections,
 											remove_intersections=remove_intersections)
+
+	def riverWidthFromCenterline(self,
+								n_interprolate_centerpoints=None,
+								transect_span_distance=3,
+								apply_smoothing=True,
+								remove_intersections=False,
+								units="km",
+								save_to_csv=None):
+		return centerline_width.riverWidthFromCenterline(river_object=self,
+														n_interprolate_centerpoints=n_interprolate_centerpoints,
+														transect_span_distance=transect_span_distance,
+														apply_smoothing=apply_smoothing,
+														remove_intersections=remove_intersections,
+														units=units,
+														save_to_csv=save_to_csv)
```

### Comparing `centerline-width-0.1.0/centerline_width.egg-info/PKG-INFO` & `centerline-width-0.2.0/centerline_width.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 0.1.0
-Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude from a right and left bank
+Version: 0.2.0
+Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
-Author: Una Schneck (unaschneck), C. Y. Schneck (cyschneck)
+Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.1.0.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.2.0.tar.gz
 Description: # Centerline-Width
         ![PyPi](https://img.shields.io/pypi/v/centerline-width)
         ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
         [![NSF-2141064](https://img.shields.io/badge/NSF-2141064-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2141064&HistoricalAwards=false)
         [![pytests](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml/badge.svg)](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml)
         
         Find the centerline and width of rivers based on the latitude and longitude positionss from the right and left bank 
         
         * **Convert raw data from Google Earth Pro to CSV**
         	* extractPointsToTextFile()
         	* convertColumnsToCSV()
         * **Find centerline and width of river**
-        	* centerlineLatitudeLongitude()
         	* plotCenterline()
         	* plotCenterlineWidth()
         	* riverWidthFromCenterline()
+        	* centerlineLatitudeLongtiude
+        	* centerlineLength
+        	* rightBankLength
+        	* leftBankLength
         
         | River Outlined in Google Earth Pro | Generated Centerline for the River Bank |
         | ------------- | ------------- |
         | ![river_google_earth+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example_google_earth.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_example.png) |
         
         Python implementation of [R-Code CMGO](https://github.com/AntoniusGolly/cmgo) (with modification)
         
@@ -41,14 +44,42 @@
         
         ## Install
         PyPi pip install at [pypi.org/project/centerline-width/](https://pypi.org/project/centerline-width/)
         
         ```
         pip install centerline-width
         ```
+        ## Quickstart: centerline-width
+        
+        The core of centerline-width works with a .csv file of the left and right bank latitude/longitudes. Starting with Google Earth Pro, two .kml must first be translated to a single .csv file
+        
+        ```python
+        import centerline_width
+        centerline_width.extractPointsToTextFile(left_kml="left_bank.kml",
+        					right_kml="right_bank.kml",
+        					text_output_name="river_coordinates_output.txt")
+        centerline_width.convertColumnsToCSV(text_file="river_coordinates_output.txt")
+        ```
+        Then, to run the centerline-width functions, generate a river object from the `river_coordinates_output.csv`
+        
+        ```python
+        river_object = centerline_width.riverCenterline(csv_data="river_coordinates_output.csv")
+        ```
+        
+        To plot the centerline, run the `plotCenterline()` function from `river_object` created
+        ```python
+        river_object.plotCenterline()
+        ```
+        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/river_coords_centerline.png)
+        
+        To plot the width of the river at intervals along the bank, run `plotCenterlineWidth` (apply_smoothing is optional and defaults to False, but is recommended)
+        ```python
+        river_object.plotCenterlineWidth(apply_smoothing=True)
+        ```
+        ![river_coords_width+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/river_coords_width.png)
         
         ## Preprocessing
         ### Convert KML files to Text File
         
         Convert two .kml files from Google Earth Pro (for the left and right bank) and export the coordinates into a text file
         
         ```
@@ -114,44 +145,55 @@
         30.037648,-92.868546,30.037482,-92.867449
         30.037674,-92.868536,30.037506,-92.867432
         30.037702,-92.868533,30.037525,-92.867430
         ```
         Output: A csv file `data/river_coords.csv` with the headers llat, llon, rlat, rlon
         
         ## Centerline and Width
-        
-        ### Types of Centerlines
-        - Voronoi centerline: centerline generated from where Voronoi vertices intersect within the river
-        - Evenly Spaced Centerline: centerline based on Voronoi centerline but evenly spaced with a fixed number of points
-        - Smoothed Centerline: centerline generated from the evenly spaced centerline but smoothed by a b-spline
-        
         ### River Object
         First, generate a river object to contain river data and available transformations
         ```
-        centerline_width.riverCenterline(csv_data=None, optional_cutoff=None)
+        centerline_width.riverCenterline(csv_data=None,
+        				optional_cutoff=None,
+        				interpolate_data=False,
+        				interpolate_n=5)
         ```
         * **[REQUIRED]** csv_data (string): File location of the text file to convert
         * [OPTIONAL] optional_cutoff (int): Include only the first x amount of the data to chart (useful for debugging)
+        * [OPTIONAL] interpolate_data (bool): Interpolate between existing data by adding additional points
+        * [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
+        
+        Interpolating is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps dues to the combination of sparse data and a narrow river
+        
+        Object (class) useful attributes:
         
-        Object (class) attributes:
+        * centerlineLatitudeLongtiude (list of tuples): List of the latitude and longitude coordinates of the centerline
+        * centerlineLength (float): Length of the centerline of the river (in km)
+        * rightBankLength (float): Length of the right bank of the river (in km)
+        * leftBankLength (float): Length of the left bank of the river (in km)
+        
+        Object (class) additional atttributes:
         
         * river_name (string): name of object, set to the csv_data string
-        * df_len (int): length of the dataframe of the csv data spliced by the optional_cutoff
-        * left_bank_coordinates (list of two element lists): list of coordiantes of the left bank generated from the csv file
-        * right_bank_coordinates (list of two element lists) list of coordinates of the right bank generated from the csv file
-        * river_bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate river bank (used to define an inside and an outside of the river)
-        * top_bank (Shapley Linestring): A linestring that represents the top of the river/polygon
-        * bottom_bank (Shapley Linestring): A linestring that represents the bottom of the river/polygon
-        * starting_node (tuple): Tuple of the starting position of the centerline path
-        * ending_node (tuple): Tuple of the end position of the centerline path
-        * river_bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
-        * centerline_latitude_longtiude (list of two element tuples): Latitude and Longitude coordinates of the centerline
-        * centerline_length (float): Length of the centerline of the river (in km)
+        * left_bank_coordinates (list of tuples): list of coordinates of the left bank generated from the csv file (`[(x, y), (x, y)]`)
+        * right_bank_coordinates (list of tuples) list of coordinates of the right bank generated from the csv file (`[(x, y), (x, y)]`)
+        * df_len (int): Length of the dataframe of the csv data spliced by the optional_cutoff
+        * bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate river bank (used to define an inside and an outside of the river)
+        * top_bank (Shapley Linestring): Linestring that represents the top of the river/polygon
+        * bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon
+        * starting_node (tuple): Tuple of the starting position (latitude and longitude) of the centerline path
+        * ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
+        * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
+        * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
+        * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Longitude position to ending Longitude position)
+        * interpolate_data (bool): if interpolating between existing data, defaults to False
+        * interpolate_n (int): specifies how many additional points will be added when interpolating data, defaults to 5
         
-        ```
+        ```python
+        import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         ```
         
         ### Return Latitude/Longitude Coordinates of Centerline
         Return the latitude/longtiude coordinates of the centerline based on the left and right banks
         ```
         river_object.centerline_latitude_longtiude
@@ -172,15 +214,15 @@
         ```
         Length returned in kilometers
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=550)
         river_centerline_length = river_object.centerline_length
         ```
-        The length of the river object returns `215.34700589636674` km
+        The length of the river centerline returns `215.34700589636674` km
         
         ## Plot Centerline in Matplotlib
         ### Plot the centerline created from a list of right and left banks with Voronoi vertices
         
         ```
         plotCenterline(display_all_possible_paths=False, 
         		plot_title=None, 
@@ -251,20 +293,20 @@
         | ------------- | ------------- |
         | ![river_keep+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_keep_intersections.png) | ![river_remove+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_remove_intersections.png)|
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.plotCenterlineWidth(save_plot_name="data/river_coords_width.png",
-        					display_true_centerline=False,
-        					n_interprolate_centerpoints=None,
-        					transect_span_distance=3,
-        					apply_smoothing=True,
-        					flag_intersections=True,
-        					remove_intersections=True)
+        				display_true_centerline=False,
+        				n_interprolate_centerpoints=None,
+        				transect_span_distance=3,
+        				apply_smoothing=True,
+        				flag_intersections=True,
+        				remove_intersections=True)
         ```
         ![river_coords_width+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/river_coords_width.png)
         
         ### Return Width of River
         
         Return the width of the river at each (evenly spaced) centerline coordinate
         
@@ -306,14 +348,15 @@
         ### Generate a Voronoi based on the points along the river banks
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example3.png)
         
         ### Display Voronoi ridge vertices that lie within the polygon (within the river banks)
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example4.png)
         
         ### Filter out any point pairs that only have one connections to filter out the short dead end paths and find the starting and ending node based on distance from the top and bottom of polygon
+        With the vertices removed, it is possible form multiple unconnected graphs within the polygon. The largest subgraph is assumed to contain the centerline and the other subgraphs are filtered out
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example6.png)
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example7.png)
         
         ### Find the shortest path from the starting node to the ending node ([Dijkstra's Algorithm](https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.shortest_paths.generic.shortest_path.html#networkx.algorithms.shortest_paths.generic.shortest_path))
         | Points on River Bank | NetworkX Graph of Points on River Bank |
         | ------------- | ------------- |
         | ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example10.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example9.png) |
@@ -327,37 +370,64 @@
         
         **All vertices:**
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example4.png)
         
         **Vertices that have at least two connections (that would create gaps):**
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/example5.png)
         
+        ### Types of Centerlines
+        - Voronoi centerline: centerline generated from where Voronoi vertices intersect within the river
+        - Evenly Spaced Centerline: centerline based on Voronoi centerline but evenly spaced with a fixed number of points
+        - Smoothed Centerline: centerline generated from the evenly spaced centerline but smoothed by a b-spline
+        
         ## Debugging, Error Handling, and Edge Cases
-        ### Edge Cases
-        If the data starts with a large width, it is possible for the starting node to be invalid
+        ### Wide Start/End of River
+        If the data starts or ends with a large width, it is possible for the starting/ending nodes to end up in the wrong position
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example3.png)
-        Currently, the starting node is determined by the closest node to the top of the bank (in green) and the ending node is determined by the closest node to the bottom of the bank (in red)
+        Currently, the starting node is determined by the closest node to the top of the bank (in green) and the ending node is determined by the closest node to the bottom of the bank (in red) that sits along the longest path
         
         ### Invalid Polygon
+        A polygon is formed to encapsulate the river with the given data (to determine the inside and outside of the river). The top and bottom are connected by a straight line from the start/end of the available data. As a result, it is possible for this straight line to overlap and create an invalid polygon.
+        
         A polygon is invalid if it overlaps within itself:
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example1.png)
         In this example, the polygon is invalid, but with such a small overlap it is still able to find a valid path
         
-        With limited data, the polygon will overlap more dramatically and will no longer be able to find a valid centerline:
+        With limited data, the polygon will overlap more dramatically and will struggle to find a valid centerline:
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example4.png)
         
         ### Invalid Centerline
         If the data is too small, a centerline and its coordinates cannot not be found (since only a single Voronoi vertex exists within the polygon and after deadends are filtered)
         
         `CRITICAL ERROR, Voronoi diagram generated too small to find centerline (no starting node found), unable to plot centerline. Set displayVoronoi=True to view. Can typically be fixed by adding more data to expand range.`
         ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/invalid_example2.png)
         Can be fixed by expanding the data until the polygon is large enough to contain at least two different vertex points
         
+        ### Invalid Top and Bottom Bank Postiions (flipDirection = True)
+        If the data for the left and right river banks are generated in reverse order, they will be read in the incorrect order and the graph will find the invalid top and bottom of the bank
+        
+        If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
+        
+        This can be fixed by using the flipDirection optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flipBankDirection=True)`
+        ![example+png](https://raw.githubusercontent.com/cyschneck/river-geometry/main/data/doc_examples/flipDirection_example.png)
+        
+        ### Fix Gaps and Jagged Centerlines
+        Gaps formed can cause part of the centerline to be skipped due to sparse data. As a result, the start and end of the centerline can skip parts at the beginning or end of a river
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_short_path.png)
+        Set river object created by `centerline_width.riverCenterline` to `interpolate_data=True` to fix for jagged edges or gaps formed by the interaction of sparse data and narrow banks
+        ```python
+        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", interpolate_data=True)
+        ```
+        | interpolate_data = False | interpolate_data = True |
+        | ------------- | ------------- |
+        | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps.png) |
+        
+        The amount of additional points added by interpolating can be adjusted with `interpolate_n`, but defaults to add 5 additional points between values
+        
         ## Developer Notes: Tech Debt and Bug Fixes
-        * Return the length of the left/right bank in riverCenterline class (right_bank_length, left_bank_length)
         * Verify that smoothing filter option does not produce a line that goes outside of the polygon
         * Return the knickpoints (occurrences of knickpoints)
         
         ## Citations
         Based on work written in R (Golly et al. 2017):
         
         >Golly, A. and Turowski, J. M.: Deriving principal channel metrics from bank and long-profile geometry with the R package cmgo, Earth Surf. Dynam., 5, 557-570, https://doi.org/10.5194/esurf-5-557-2017, 2017.
@@ -372,17 +442,17 @@
         
         This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the atuhors and do not neccessarily reflect the views of the National Science Foundation.
         
         ## Bug and Feature Request
         
         Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/cyschneck/centerline-width/issues) or to ugschneck@gmail.com/cyschneck@gmail.com
         
-Keywords: geophysics,python,voronoi,centerline,centerline-extraction,river-bank,limnology,hydrology
+Keywords: geophysics,python,voronoi,networkx,centerline,centerline-extraction,centerline-detection,rivers,river-bank-length,river-bank,limnology,hydrology
 Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Education
```

### Comparing `centerline-width-0.1.0/centerline_width.egg-info/SOURCES.txt` & `centerline-width-0.2.0/centerline_width.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `centerline-width-0.1.0/setup.py` & `centerline-width-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # -*- coding: utf-8 -*-
 
 # Python Package Setup
 from setuptools import setup, find_namespace_packages
 
-VERSION="0.1.0"
-DESCRIPTION="A Python package to find the centerline and width of rivers based on the latitude and longitude from a right and left bank"
+VERSION="0.2.0"
+DESCRIPTION="A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank"
 
 with open("README.md", "r") as f:
 	long_description_readme = f.read()
 
 setup(
 	name="centerline-width",
 	version=VERSION,
 	description=DESCRIPTION,
 	long_description=long_description_readme,
 	long_description_content_type='text/markdown',
 	url="https://github.com/cyschneck/centerline-width",
 	download_url="https://github.com/cyschneck/centerline-width/archive/refs/tags/v{0}.tar.gz".format(VERSION),
-	author="Una Schneck (unaschneck), C. Y. Schneck (cyschneck)",
-	keywords=["geophysics", "python", "voronoi", "centerline", "centerline-extraction", "river-bank", "limnology", "hydrology"],
+	author="Una Schneck (unaschneck), Cora Schneck (cyschneck)",
+	keywords=["geophysics", "python", "voronoi", "networkx", "centerline", "centerline-extraction", "centerline-detection", "rivers", "river-bank-length", "river-bank", "limnology", "hydrology"],
 	license="MIT",
 	classifiers=[
-		"Development Status :: 1 - Planning",
+		"Development Status :: 2 - Pre-Alpha",
 		"Intended Audience :: Developers",
 		"Intended Audience :: Education",
 		"Intended Audience :: Science/Research",
 		"License :: OSI Approved :: MIT License",
 		"Programming Language :: Python",
 		"Programming Language :: Python :: 3.9",
 		"Intended Audience :: Education",
```

