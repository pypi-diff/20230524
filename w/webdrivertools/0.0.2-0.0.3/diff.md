# Comparing `tmp/webdrivertools-0.0.2.tar.gz` & `tmp/webdrivertools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webdrivertools-0.0.2.tar", last modified: Thu May 11 02:03:31 2023, max compression
+gzip compressed data, was "webdrivertools-0.0.3.tar", last modified: Wed May 24 00:49:04 2023, max compression
```

## Comparing `webdrivertools-0.0.2.tar` & `webdrivertools-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-11 02:03:31.945246 webdrivertools-0.0.2/
--rw-r--r--   0 leandro    (501) staff       (20)     1127 2023-04-24 02:15:44.000000 webdrivertools-0.0.2/LICENSE
--rw-r--r--   0 leandro    (501) staff       (20)     3340 2023-05-11 02:03:31.945132 webdrivertools-0.0.2/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)     2480 2023-05-11 02:02:57.000000 webdrivertools-0.0.2/README.md
--rw-r--r--   0 leandro    (501) staff       (20)     1012 2023-05-11 02:03:03.000000 webdrivertools-0.0.2/pyproject.toml
--rw-r--r--   0 leandro    (501) staff       (20)       38 2023-05-11 02:03:31.945277 webdrivertools-0.0.2/setup.cfg
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-11 02:03:31.944234 webdrivertools-0.0.2/webdrivertools/
--rw-r--r--   0 leandro    (501) staff       (20)      163 2023-05-11 01:56:46.000000 webdrivertools-0.0.2/webdrivertools/__init__.py
--rw-r--r--   0 leandro    (501) staff       (20)     4294 2023-05-11 01:42:53.000000 webdrivertools-0.0.2/webdrivertools/webdrivertools.py
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-11 02:03:31.944981 webdrivertools-0.0.2/webdrivertools.egg-info/
--rw-r--r--   0 leandro    (501) staff       (20)     3340 2023-05-11 02:03:31.000000 webdrivertools-0.0.2/webdrivertools.egg-info/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)      281 2023-05-11 02:03:31.000000 webdrivertools-0.0.2/webdrivertools.egg-info/SOURCES.txt
--rw-r--r--   0 leandro    (501) staff       (20)        1 2023-05-11 02:03:31.000000 webdrivertools-0.0.2/webdrivertools.egg-info/dependency_links.txt
--rw-r--r--   0 leandro    (501) staff       (20)       16 2023-05-11 02:03:31.000000 webdrivertools-0.0.2/webdrivertools.egg-info/requires.txt
--rw-r--r--   0 leandro    (501) staff       (20)       15 2023-05-11 02:03:31.000000 webdrivertools-0.0.2/webdrivertools.egg-info/top_level.txt
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-24 00:49:04.961232 webdrivertools-0.0.3/
+-rw-r--r--   0 leandro    (501) staff       (20)     1127 2023-04-24 02:15:44.000000 webdrivertools-0.0.3/LICENSE
+-rw-r--r--   0 leandro    (501) staff       (20)     3340 2023-05-24 00:49:04.961094 webdrivertools-0.0.3/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)     2480 2023-05-11 02:02:57.000000 webdrivertools-0.0.3/README.md
+-rw-r--r--   0 leandro    (501) staff       (20)     1012 2023-05-24 00:48:26.000000 webdrivertools-0.0.3/pyproject.toml
+-rw-r--r--   0 leandro    (501) staff       (20)       38 2023-05-24 00:49:04.961263 webdrivertools-0.0.3/setup.cfg
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-24 00:49:04.958874 webdrivertools-0.0.3/webdrivertools/
+-rw-r--r--   0 leandro    (501) staff       (20)      163 2023-05-11 01:56:46.000000 webdrivertools-0.0.3/webdrivertools/__init__.py
+-rw-r--r--   0 leandro    (501) staff       (20)     4663 2023-05-23 21:48:05.000000 webdrivertools-0.0.3/webdrivertools/webdrivertools.py
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-24 00:49:04.960880 webdrivertools-0.0.3/webdrivertools.egg-info/
+-rw-r--r--   0 leandro    (501) staff       (20)     3340 2023-05-24 00:49:04.000000 webdrivertools-0.0.3/webdrivertools.egg-info/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)      281 2023-05-24 00:49:04.000000 webdrivertools-0.0.3/webdrivertools.egg-info/SOURCES.txt
+-rw-r--r--   0 leandro    (501) staff       (20)        1 2023-05-24 00:49:04.000000 webdrivertools-0.0.3/webdrivertools.egg-info/dependency_links.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       16 2023-05-24 00:49:04.000000 webdrivertools-0.0.3/webdrivertools.egg-info/requires.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       15 2023-05-24 00:49:04.000000 webdrivertools-0.0.3/webdrivertools.egg-info/top_level.txt
```

### Comparing `webdrivertools-0.0.2/LICENSE` & `webdrivertools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `webdrivertools-0.0.2/PKG-INFO` & `webdrivertools-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdrivertools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Functions to make life with Selenium easier.
 Author-email: Leandro Pereira de Lima e Silva <leandro@lls-software.com>
 Project-URL: Homepage, https://github.com/leandropls/webdrivertools
 Project-URL: Bug Tracker, https://github.com/leandropls/webdrivertools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `webdrivertools-0.0.2/README.md` & `webdrivertools-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `webdrivertools-0.0.2/pyproject.toml` & `webdrivertools-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "webdrivertools"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Leandro Pereira de Lima e Silva", email="leandro@lls-software.com" },
 ]
 description = "Functions to make life with Selenium easier."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `webdrivertools-0.0.2/webdrivertools/webdrivertools.py` & `webdrivertools-0.0.3/webdrivertools/webdrivertools.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from time import sleep
 
+from selenium.common import ElementNotInteractableException
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
 
 
 def click(
     driver: WebDriver,
@@ -75,30 +76,39 @@
         # Raise error if no matching element found
         raise ValueError(f"Element not found: {value} (innerText: {innerText})")
     return element
 
 
 def click_element_area(driver: WebDriver, element: WebElement) -> None:
     """
-    Click on the element area, even if it is covered by an overlay. This function is useful when dealing
-    with elements obstructed by modal overlays or other overlapping elements, which may cause issues when
-    attempting to interact with the intended element using Selenium.
+    Click on the element area, even if it is covered by an overlay. This function
+    is useful when dealing with elements obstructed by modal overlays or other
+    overlapping elements, which may cause issues when attempting to interact
+    with the intended element using Selenium.
 
     :param driver: A WebDriver instance used to interact with the webpage.
     :param element: A WebElement instance representing the element to be clicked.
     """
     # Get the Rect object of the element, containing its position and dimensions
     rect = element.rect
 
     # Use JavaScript to find the topmost element at the center of the given element
     overlayElement = driver.execute_script(
         "return document.elementFromPoint(arguments[0], arguments[1]);",
         rect["x"] + rect["width"] // 2,
         rect["y"] + rect["height"] // 2,
     )
 
-    # If an overlay element is found, replace the original element with it
+    # If an overlay element is found
     if overlayElement is not None:
-        element = overlayElement
+        try:
+            # If the overlay element is clickable, click on it
+            overlayElement.click()
+        except ElementNotInteractableException:
+            # Ignore exceptions related to unclickable overlay elements
+            pass
+        else:
+            # If the click on the overlay element succeeds, stop execution
+            return
 
-    # Click the determined element, either the original one or the overlay element
+    # If there's no overlay element, or the overlayElemet is not clickable, click on the given element
     element.click()
```

### Comparing `webdrivertools-0.0.2/webdrivertools.egg-info/PKG-INFO` & `webdrivertools-0.0.3/webdrivertools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdrivertools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Functions to make life with Selenium easier.
 Author-email: Leandro Pereira de Lima e Silva <leandro@lls-software.com>
 Project-URL: Homepage, https://github.com/leandropls/webdrivertools
 Project-URL: Bug Tracker, https://github.com/leandropls/webdrivertools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

