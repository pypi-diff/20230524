# Comparing `tmp/quickboard-0.3.2.tar.gz` & `tmp/quickboard-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickboard-0.3.2.tar", last modified: Thu Jul 28 05:14:41 2022, max compression
+gzip compressed data, was "quickboard-0.3.3.tar", last modified: Wed May 24 18:28:36 2023, max compression
```

## Comparing `quickboard-0.3.2.tar` & `quickboard-0.3.3.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 05:14:41.119388 quickboard-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (116)     1523 2022-07-28 05:14:31.000000 quickboard-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     3088 2022-07-28 05:14:41.119388 quickboard-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2547 2022-07-28 05:14:31.000000 quickboard-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 05:14:41.119388 quickboard-0.3.2/quickboard/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1260 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/app.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 05:14:41.119388 quickboard-0.3.2/quickboard/base/
--rw-r--r--   0 runner    (1001) docker     (116)      177 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4650 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/base/_dynamicpanel.py
--rw-r--r--   0 runner    (1001) docker     (116)     1461 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/base/basetab.py
--rw-r--r--   0 runner    (1001) docker     (116)     1449 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/base/contentgrid.py
--rw-r--r--   0 runner    (1001) docker     (116)     2753 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/base/datapanel.py
--rw-r--r--   0 runner    (1001) docker     (116)     2837 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/base/plotpanel.py
--rw-r--r--   0 runner    (1001) docker     (116)     6008 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/base/quickboard.py
--rw-r--r--   0 runner    (1001) docker     (116)      725 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/base/sidebar.py
--rw-r--r--   0 runner    (1001) docker     (116)      510 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/dashsetup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 05:14:41.119388 quickboard-0.3.2/quickboard/plugins/
--rw-r--r--   0 runner    (1001) docker     (116)      356 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2319 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/plugins/datadisplay.py
--rw-r--r--   0 runner    (1001) docker     (116)     1387 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/plugins/datafilterchecklist.py
--rw-r--r--   0 runner    (1001) docker     (116)     1397 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/plugins/datafilterradiobuttons.py
--rw-r--r--   0 runner    (1001) docker     (116)     2971 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/plugins/datafilterrangeslider.py
--rw-r--r--   0 runner    (1001) docker     (116)     2279 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/plugins/datafilterslider.py
--rw-r--r--   0 runner    (1001) docker     (116)      576 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/plugins/datasumchecklist.py
--rw-r--r--   0 runner    (1001) docker     (116)     1478 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/plugins/plotinputradiobuttons.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 05:14:41.119388 quickboard-0.3.2/quickboard/primitives/
--rw-r--r--   0 runner    (1001) docker     (116)      104 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2483 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/primitives/_datamanager.py
--rw-r--r--   0 runner    (1001) docker     (116)      836 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/primitives/_panel.py
--rw-r--r--   0 runner    (1001) docker     (116)     1566 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/primitives/controlplugin.py
--rw-r--r--   0 runner    (1001) docker     (116)     2402 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/styles.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 05:14:41.119388 quickboard-0.3.2/quickboard/textboxes/
--rw-r--r--   0 runner    (1001) docker     (116)       29 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/textboxes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1782 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/textboxes/getupdatedtext.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 05:14:41.119388 quickboard-0.3.2/quickboard/utils/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       60 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (116)      395 2022-07-28 05:14:32.000000 quickboard-0.3.2/quickboard/utils/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 05:14:41.119388 quickboard-0.3.2/quickboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3088 2022-07-28 05:14:41.000000 quickboard-0.3.2/quickboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1150 2022-07-28 05:14:41.000000 quickboard-0.3.2/quickboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-07-28 05:14:41.000000 quickboard-0.3.2/quickboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       93 2022-07-28 05:14:41.000000 quickboard-0.3.2/quickboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       11 2022-07-28 05:14:41.000000 quickboard-0.3.2/quickboard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      779 2022-07-28 05:14:41.123389 quickboard-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       53 2022-07-28 05:14:32.000000 quickboard-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:28:36.843448 quickboard-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-24 18:28:27.000000 quickboard-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-24 18:28:36.843448 quickboard-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-24 18:28:27.000000 quickboard-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:28:36.839448 quickboard-0.3.3/quickboard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:28:36.839448 quickboard-0.3.3/quickboard/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/base/_dynamicpanel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/base/basetab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/base/contentgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/base/datapanel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/base/plotpanel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/base/quickboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/base/sidebar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/dashsetup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:28:36.843448 quickboard-0.3.3/quickboard/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/plugins/datadisplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/plugins/datafilterchecklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/plugins/datafilterradiobuttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/plugins/datafilterrangeslider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/plugins/datafilterslider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/plugins/datasumchecklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/plugins/plotinputradiobuttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/plugins/plotinputrangeslider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/plugins/plotinputslider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:28:36.843448 quickboard-0.3.3/quickboard/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/primitives/_datamanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/primitives/_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/primitives/controlplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/styles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:28:36.843448 quickboard-0.3.3/quickboard/textboxes/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/textboxes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/textboxes/getupdatedtext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:28:36.843448 quickboard-0.3.3/quickboard/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-24 18:28:28.000000 quickboard-0.3.3/quickboard/utils/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:28:36.839448 quickboard-0.3.3/quickboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-24 18:28:36.000000 quickboard-0.3.3/quickboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-24 18:28:36.000000 quickboard-0.3.3/quickboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:28:36.000000 quickboard-0.3.3/quickboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-24 18:28:36.000000 quickboard-0.3.3/quickboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-24 18:28:36.000000 quickboard-0.3.3/quickboard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-24 18:28:36.843448 quickboard-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-24 18:28:28.000000 quickboard-0.3.3/setup.py
```

### Comparing `quickboard-0.3.2/LICENSE` & `quickboard-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quickboard-0.3.2/PKG-INFO` & `quickboard-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickboard
-Version: 0.3.2
+Version: 0.3.3
 Summary: "A simple Python package for creating quick, modular dashboards."
 Home-page: https://github.com/broadinstitute/quickboard
 Download-URL: https://github.com/broadinstitute/quickboard
 Author: Ricky Magner
 Author-email: rmagner@broadinstitute.org
 Keywords: dash,dashboard,interactive,plot,graph
 Classifier: Framework :: Dash
```

### Comparing `quickboard-0.3.2/README.md` & `quickboard-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `quickboard-0.3.2/quickboard/app.py` & `quickboard-0.3.3/quickboard/app.py`

 * *Files identical despite different names*

### Comparing `quickboard-0.3.2/quickboard/base/_dynamicpanel.py` & `quickboard-0.3.3/quickboard/base/_dynamicpanel.py`

 * *Files identical despite different names*

### Comparing `quickboard-0.3.2/quickboard/base/basetab.py` & `quickboard-0.3.3/quickboard/base/basetab.py`

 * *Files identical despite different names*

### Comparing `quickboard-0.3.2/quickboard/base/contentgrid.py` & `quickboard-0.3.3/quickboard/base/contentgrid.py`

 * *Files identical despite different names*

### Comparing `quickboard-0.3.2/quickboard/base/datapanel.py` & `quickboard-0.3.3/quickboard/base/datapanel.py`

 * *Files identical despite different names*

### Comparing `quickboard-0.3.2/quickboard/base/plotpanel.py` & `quickboard-0.3.3/quickboard/base/plotpanel.py`

 * *Files identical despite different names*

### Comparing `quickboard-0.3.2/quickboard/base/quickboard.py` & `quickboard-0.3.3/quickboard/base/quickboard.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         sidebar_header = header text/object to use if no tabs
         sidebar_plugins = list of plugins to use in sidebar if no tabs
         tab_list = list of tab objects from which the board is comprised
         content_list = objects to display in the absence of tabs
     """
     def __init__(self, sidebar_header="Data Controls", sidebar_plugins=[], tab_list=[], content_list=[]):
         self.style = styles.CONTENT_STYLE
+        self.tab_list = tab_list
         self.tabs_container = self.initialize_tabs(tab_list)
         self.sidebar_container = self.initialize_sidebar(sidebar_header, sidebar_plugins)
 
         # Used in case user doesn't want to have tabs, but one page with some contents
         self.content_list = html.Div([x.container for x in content_list])
 
         self.container = html.Div(
@@ -56,15 +57,14 @@
             Output('data_store', 'data'),
             State('data_store', 'data'),
             update_data_inputs,
         )(self.update_data)
 
     def initialize_tabs(self, tab_list):
         # Collect tabs together unless user inputs none
-        self.tab_list = tab_list
         if len(tab_list) != 0:
             self.tabs = dcc.Tabs(
                     value=self.tab_list[0].tab_label,
                     children=[x.tab for x in self.tab_list]
             )
 
             self.current_tab_content = html.Div(children=html.P('If this message persists, then there was an ERROR '
```

### Comparing `quickboard-0.3.2/quickboard/base/sidebar.py` & `quickboard-0.3.3/quickboard/base/sidebar.py`

 * *Files identical despite different names*

### Comparing `quickboard-0.3.2/quickboard/plugins/datadisplay.py` & `quickboard-0.3.3/quickboard/plugins/datadisplay.py`

 * *Files identical despite different names*

### Comparing `quickboard-0.3.2/quickboard/plugins/datafilterchecklist.py` & `quickboard-0.3.3/quickboard/plugins/datafilterchecklist.py`

 * *Files identical despite different names*

### Comparing `quickboard-0.3.2/quickboard/plugins/datafilterradiobuttons.py` & `quickboard-0.3.3/quickboard/plugins/datafilterradiobuttons.py`

 * *Files identical despite different names*

### Comparing `quickboard-0.3.2/quickboard/plugins/datafilterrangeslider.py` & `quickboard-0.3.3/quickboard/plugins/datafilterrangeslider.py`

 * *Files identical despite different names*

### Comparing `quickboard-0.3.2/quickboard/plugins/datafilterslider.py` & `quickboard-0.3.3/quickboard/plugins/datafilterslider.py`

 * *Files identical despite different names*

### Comparing `quickboard-0.3.2/quickboard/plugins/datasumchecklist.py` & `quickboard-0.3.3/quickboard/plugins/datasumchecklist.py`

 * *Files identical despite different names*

### Comparing `quickboard-0.3.2/quickboard/plugins/plotinputradiobuttons.py` & `quickboard-0.3.3/quickboard/plugins/plotinputradiobuttons.py`

 * *Files identical despite different names*

### Comparing `quickboard-0.3.2/quickboard/primitives/_datamanager.py` & `quickboard-0.3.3/quickboard/primitives/_datamanager.py`

 * *Files identical despite different names*

### Comparing `quickboard-0.3.2/quickboard/primitives/_panel.py` & `quickboard-0.3.3/quickboard/primitives/_panel.py`

 * *Files identical despite different names*

### Comparing `quickboard-0.3.2/quickboard/primitives/controlplugin.py` & `quickboard-0.3.3/quickboard/primitives/controlplugin.py`

 * *Files identical despite different names*

### Comparing `quickboard-0.3.2/quickboard/styles.py` & `quickboard-0.3.3/quickboard/styles.py`

 * *Files identical despite different names*

### Comparing `quickboard-0.3.2/quickboard/textboxes/getupdatedtext.py` & `quickboard-0.3.3/quickboard/textboxes/getupdatedtext.py`

 * *Files identical despite different names*

### Comparing `quickboard-0.3.2/quickboard.egg-info/PKG-INFO` & `quickboard-0.3.3/quickboard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickboard
-Version: 0.3.2
+Version: 0.3.3
 Summary: "A simple Python package for creating quick, modular dashboards."
 Home-page: https://github.com/broadinstitute/quickboard
 Download-URL: https://github.com/broadinstitute/quickboard
 Author: Ricky Magner
 Author-email: rmagner@broadinstitute.org
 Keywords: dash,dashboard,interactive,plot,graph
 Classifier: Framework :: Dash
```

### Comparing `quickboard-0.3.2/quickboard.egg-info/SOURCES.txt` & `quickboard-0.3.3/quickboard.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 quickboard/plugins/datadisplay.py
 quickboard/plugins/datafilterchecklist.py
 quickboard/plugins/datafilterradiobuttons.py
 quickboard/plugins/datafilterrangeslider.py
 quickboard/plugins/datafilterslider.py
 quickboard/plugins/datasumchecklist.py
 quickboard/plugins/plotinputradiobuttons.py
+quickboard/plugins/plotinputrangeslider.py
+quickboard/plugins/plotinputslider.py
 quickboard/primitives/__init__.py
 quickboard/primitives/_datamanager.py
 quickboard/primitives/_panel.py
 quickboard/primitives/controlplugin.py
 quickboard/textboxes/__init__.py
 quickboard/textboxes/getupdatedtext.py
 quickboard/utils/__init__.py
```

### Comparing `quickboard-0.3.2/setup.cfg` & `quickboard-0.3.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = quickboard
-version = 0.3.2
+version = 0.3.3
 url = https://github.com/broadinstitute/quickboard
 download_url = https://github.com/broadinstitute/quickboard
 author = Ricky Magner
 author_email = rmagner@broadinstitute.org
 description = "A simple Python package for creating quick, modular dashboards."
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -13,19 +13,19 @@
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python
 keywords = dash, dashboard, interactive, plot, graph
 
 [options]
 packages = find:
 install_requires = 
-	dash==2.6.0
-	dash_bootstrap_components==1.2.0
-	jupyter_dash==0.4.2
+	dash>=2.9.3
+	dash_bootstrap_components>=1.4.1
+	jupyter_dash>=0.4.2
 	numpy>=1.21.0
-	pandas>=1.3.0
+	pandas>=2.0.1
 
 [options.packages.find]
 exclude = 
 	examples*
 	docs*
 
 [egg_info]
```

