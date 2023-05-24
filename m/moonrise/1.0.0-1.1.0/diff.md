# Comparing `tmp/moonrise-1.0.0.tar.gz` & `tmp/moonrise-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonrise-1.0.0.tar", last modified: Mon May  1 03:03:43 2023, max compression
+gzip compressed data, was "moonrise-1.1.0.tar", last modified: Wed May 24 17:42:04 2023, max compression
```

## Comparing `moonrise-1.0.0.tar` & `moonrise-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 03:03:43.484101 moonrise-1.0.0/
--rw-rw-rw-   0        0        0     1103 2023-04-30 17:28:27.000000 moonrise-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     6448 2023-05-01 03:03:43.485101 moonrise-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5878 2023-05-01 03:00:14.000000 moonrise-1.0.0/README.md
--rw-rw-rw-   0        0        0      104 2023-04-30 20:29:54.000000 moonrise-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      830 2023-05-01 03:03:43.488102 moonrise-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-01 03:03:43.417102 moonrise-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 03:03:43.447108 moonrise-1.0.0/src/moonrise/
--rw-rw-rw-   0        0        0     6231 2023-05-01 02:57:08.000000 moonrise-1.0.0/src/moonrise/Base_Test.py
--rw-rw-rw-   0        0        0     4989 2023-04-30 17:26:48.000000 moonrise-1.0.0/src/moonrise/Moon_Browser.py
--rw-rw-rw-   0        0        0     6562 2023-04-20 14:11:28.000000 moonrise-1.0.0/src/moonrise/Moon_Methods.py
--rw-rw-rw-   0        0        0     1876 2023-05-01 02:55:41.000000 moonrise-1.0.0/src/moonrise/__init__.py
--rw-rw-rw-   0        0        0     2364 2023-05-01 02:47:47.000000 moonrise-1.0.0/src/moonrise/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 03:03:43.483101 moonrise-1.0.0/src/moonrise.egg-info/
--rw-rw-rw-   0        0        0     6448 2023-05-01 03:03:43.000000 moonrise-1.0.0/src/moonrise.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-05-01 03:03:43.000000 moonrise-1.0.0/src/moonrise.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 03:03:43.000000 moonrise-1.0.0/src/moonrise.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-01 03:03:43.000000 moonrise-1.0.0/src/moonrise.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2023-05-01 03:03:43.000000 moonrise-1.0.0/src/moonrise.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-01 03:03:43.000000 moonrise-1.0.0/src/moonrise.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 17:42:04.544958 moonrise-1.1.0/
+-rw-rw-rw-   0        0        0     1103 2023-05-01 03:19:38.000000 moonrise-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     6448 2023-05-24 17:42:04.544958 moonrise-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5878 2023-05-15 20:49:18.000000 moonrise-1.1.0/README.md
+-rw-rw-rw-   0        0        0      104 2023-05-01 03:19:38.000000 moonrise-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      846 2023-05-24 17:42:04.547958 moonrise-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 17:42:04.480956 moonrise-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 17:42:04.511958 moonrise-1.1.0/src/moonrise/
+-rw-rw-rw-   0        0        0     6864 2023-05-23 21:39:47.000000 moonrise-1.1.0/src/moonrise/Base_Test.py
+-rw-rw-rw-   0        0        0     5711 2023-05-22 01:31:15.000000 moonrise-1.1.0/src/moonrise/Moon_Browser.py
+-rw-rw-rw-   0        0        0     6562 2023-05-15 15:31:11.000000 moonrise-1.1.0/src/moonrise/Moon_Methods.py
+-rw-rw-rw-   0        0        0     2053 2023-05-22 01:31:15.000000 moonrise-1.1.0/src/moonrise/Moon_Movie.py
+-rw-rw-rw-   0        0        0     1876 2023-05-15 20:38:47.000000 moonrise-1.1.0/src/moonrise/__init__.py
+-rw-rw-rw-   0        0        0     2363 2023-05-11 19:30:47.000000 moonrise-1.1.0/src/moonrise/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 17:42:04.542960 moonrise-1.1.0/src/moonrise.egg-info/
+-rw-rw-rw-   0        0        0     6448 2023-05-24 17:42:04.000000 moonrise-1.1.0/src/moonrise.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2023-05-24 17:42:04.000000 moonrise-1.1.0/src/moonrise.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 17:42:04.000000 moonrise-1.1.0/src/moonrise.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-24 17:42:04.000000 moonrise-1.1.0/src/moonrise.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-05-24 17:42:04.000000 moonrise-1.1.0/src/moonrise.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-24 17:42:04.000000 moonrise-1.1.0/src/moonrise.egg-info/top_level.txt
```

### Comparing `moonrise-1.0.0/LICENSE` & `moonrise-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moonrise-1.0.0/PKG-INFO` & `moonrise-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonrise
-Version: 1.0.0
+Version: 1.1.0
 Summary: Test suite creation toolset with additional quality of life upgrades for using the selenium test framework.
 Home-page: https://github.com/Worakow1138/Moonrise
 Author: Christopher Diamond-Jones
 Author-email: christopher.jones1138@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `moonrise-1.0.0/README.md` & `moonrise-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `moonrise-1.0.0/setup.cfg` & `moonrise-1.1.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6f6f 6e72 6973 650d 0a76 6572   = moonrise..ver
-00000020: 7369 6f6e 203d 2031 2e30 2e30 0d0a 6175  sion = 1.0.0..au
+00000020: 7369 6f6e 203d 2031 2e31 2e30 0d0a 6175  sion = 1.1.0..au
 00000030: 7468 6f72 203d 2043 6872 6973 746f 7068  thor = Christoph
 00000040: 6572 2044 6961 6d6f 6e64 2d4a 6f6e 6573  er Diamond-Jones
 00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000060: 2063 6872 6973 746f 7068 6572 2e6a 6f6e   christopher.jon
 00000070: 6573 3131 3338 4067 6d61 696c 2e63 6f6d  es1138@gmail.com
 00000080: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000090: 5465 7374 2073 7569 7465 2063 7265 6174  Test suite creat
@@ -35,18 +35,19 @@
 00000220: 696f 6e73 5d0d 0a70 6163 6b61 6765 5f64  ions]..package_d
 00000230: 6972 203d 200d 0a09 3d20 7372 630d 0a70  ir = ...= src..p
 00000240: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
 00000250: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
 00000260: 203d 203e 3d33 2e37 0d0a 696e 7374 616c   = >=3.7..instal
 00000270: 6c5f 7265 7175 6972 6573 203d 200d 0a09  l_requires = ...
 00000280: 7365 6c65 6e69 756d 0d0a 0963 6f6c 6f72  selenium...color
-00000290: 616d 610d 0a0d 0a5b 6f70 7469 6f6e 732e  ama....[options.
-000002a0: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
-000002b0: 7768 6572 6520 3d20 7372 630d 0a0d 0a5b  where = src....[
-000002c0: 6f70 7469 6f6e 732e 656e 7472 795f 706f  options.entry_po
-000002d0: 696e 7473 5d0d 0a63 6f6e 736f 6c65 5f73  ints]..console_s
-000002e0: 6372 6970 7473 203d 200d 0a09 6d6f 6f6e  cripts = ...moon
-000002f0: 7269 7365 203d 206d 6f6f 6e72 6973 652e  rise = moonrise.
-00000300: 5f5f 6d61 696e 5f5f 3a72 756e 5f63 6c69  __main__:run_cli
-00000310: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-00000320: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-00000330: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+00000290: 616d 610d 0a09 6666 6d70 6567 2d70 7974  ama...ffmpeg-pyt
+000002a0: 686f 6e0d 0a0d 0a5b 6f70 7469 6f6e 732e  hon....[options.
+000002b0: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
+000002c0: 7768 6572 6520 3d20 7372 630d 0a0d 0a5b  where = src....[
+000002d0: 6f70 7469 6f6e 732e 656e 7472 795f 706f  options.entry_po
+000002e0: 696e 7473 5d0d 0a63 6f6e 736f 6c65 5f73  ints]..console_s
+000002f0: 6372 6970 7473 203d 200d 0a09 6d6f 6f6e  cripts = ...moon
+00000300: 7269 7365 203d 206d 6f6f 6e72 6973 652e  rise = moonrise.
+00000310: 5f5f 6d61 696e 5f5f 3a72 756e 5f63 6c69  __main__:run_cli
+00000320: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+00000330: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000340: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

### Comparing `moonrise-1.0.0/src/moonrise/Base_Test.py` & `moonrise-1.1.0/src/moonrise/Base_Test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import traceback
 from colorama import Fore, Style, init
 import datetime
+import shutil
 init(convert=True)
 
 class BaseTest:
     """Creates the structure for test suites written using the Moonrise framework
     """
 
     # The dictionary to be referenced when evaluating what tests to run
@@ -16,14 +17,15 @@
         """Evaluates whether to run tests within the current test suite based on user input and creates report folder and file structures.
 
            Arguments:
            - `test_cases`: Test Case names to be executed. If none specified, will execute all test cases under the current test suite.
         """
 
         self.suite_tests = self.tests.get(f"{self.__module__}.{self.__class__.__name__}")
+        self.video_folder = None
 
         # If the condition is present where there are no tests in a suite or the user-requested tests cases do not match the current suite,
         # do not proceed.
         if self.suite_tests is None or (test_cases != () and len(set(test_cases).intersection(self.suite_tests)) == 0):
             # Add an extra note if test cases were specified but do not exist in the current suite.
             if test_cases and self.suite_tests:
                 print(f'Skipping test suite "{self.__class__.__name__}" in module "{self.__module__}" because no tests matching {test_cases} were found.')
@@ -41,33 +43,41 @@
         self.colors = {
         "pass": Fore.LIGHTGREEN_EX,
         "fail": Fore.LIGHTRED_EX,
         "header": Fore.LIGHTCYAN_EX,
         "info": ""
         }
 
-        if not os.path.exists(str(f"{os.getcwd()}\\reports\\{self.__module__}\\{self.__class__.__name__}")):
-            os.makedirs(str(f"{os.getcwd()}\\reports\\{self.__module__}\\{self.__class__.__name__}"))
-        self.reports_folder = str(f"{os.getcwd()}\\reports\\{self.__module__}\\{self.__class__.__name__}")
-        self.report_file = open(f"{self.reports_folder}\\{self.__class__.__name__}.log", "w")
+        if not os.path.exists(str(f"{os.getcwd()}/reports/{self.__module__}/{self.__class__.__name__}")):
+            os.makedirs(str(f"{os.getcwd()}/reports/{self.__module__}/{self.__class__.__name__}"))
+        self.reports_folder = str(f"{os.getcwd()}/reports/{self.__module__}/{self.__class__.__name__}")
+
+        if not os.path.exists(str(f"{self.reports_folder}/video")):
+            os.makedirs(str(f"{self.reports_folder}/video"))
+        self.video_folder = self.reports_folder + "/video"
+
+        self.report_file = open(f"{self.reports_folder}/{self.__class__.__name__}.log", "w")
 
         self.run_tests(test_cases)
 
+        shutil.rmtree(self.video_folder)
 
     def run_tests(self, test_cases):
         """Method to call the requested tests.
 
            Arguments:
            - `test_cases`: Test Case names to be executed.
         """
+        if self.video_thread:
+            self.video_thread.video_folder = self.video_folder
         
         self.log_to_report(f"----------------- Beginning Suite: {self.__class__.__name__} -----------------", log_type="header")
         # Perform suite setup actions before any tests are executed.
         self.suite_setup()
-
+        
         self.totals += len(test_cases)
         
         for tc in test_cases:
             self.log_to_report(f"--- Starting test: {tc} ---", log_type="header")
             self.suite_tests.get(tc)(self)
 
         self.log_to_report(f"----------------- Ending Suite: {self.__class__.__name__} -----------------", log_type="header")
@@ -77,14 +87,19 @@
         if self.failures > 0:
             end_string = f"{self.colors.get('pass')}{self.passes} tests passing, {self.colors.get('fail')}{self.failures} tests failing, {self.colors.get('header')}{self.totals} tests total"
         else:
             end_string = f"{self.colors.get('pass')}{self.passes} tests passing, {self.colors.get('header')}{self.totals} tests total"
 
         self.log_to_report(end_string, log_type="header")
 
+        # Create video from screenshots if video_thread was created.
+        if self.video_thread:
+            self.video_thread.create_video_from_pngs(f"{self.reports_folder}/{self.__class__.__name__}.mp4")
+            self.video_thread.stop()
+
     def log_to_report(cls, message, log_type = "info"):
         """Log information with a timestamp to the console and to the report file.
 
            Arguments:
            - message: The text to log.
            - log_type: The color of the text as it will appear in the console. Consult the colors variable in this class for specifics.
         """
@@ -123,23 +138,23 @@
            Arguments:
            - test_case: The name of the method to add as a test case.
         """
 
         def test_executor(self):
             """Executes the current test case, performing test setup actions, handling failures, and finally calling test teardown actions.
             """
-            self.test_setup()
             try:
+                self.test_setup()
                 test_case(self)
                 self.log_to_report(f"{test_case.__name__} PASS", log_type = "pass")
                 self.passes += 1
             except Exception:
                 self.log_to_report(f"{traceback.format_exc()}")
                 if self.moon_driver:
-                    self.moon_driver.save_screenshot(f"{self.reports_folder}\\{test_case.__name__}.png")
+                    self.moon_driver.save_screenshot(f"{self.reports_folder}/{test_case.__name__}.png")
                 self.log_to_report(f"{test_case.__name__} FAIL", log_type = "fail")
                 self.failures += 1
             finally:
                 self.test_teardown()
 
         mod_and_suite = f"{test_case.__module__}.{test_case.__qualname__.split('.')[0]}"
         cls.tests.setdefault(mod_and_suite, {})
```

### Comparing `moonrise-1.0.0/src/moonrise/Moon_Browser.py` & `moonrise-1.1.0/src/moonrise/Moon_Browser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import os
 import subprocess
 from selenium import webdriver
 from selenium.webdriver.remote.webdriver import WebDriver as RemoteWebDriver
 from selenium.webdriver.common.service import Service
+from moonrise.Moon_Movie import VideoThread
 
 
 
 class MoonBrowser:
 
     moon_driver = None
+    video_thread = None
 
-    def open_browser(self, browser_type, *browser_args, persist=False):
+    def open_browser(self, browser_type, *browser_args, persist=False, record_test=True):
         """Opens a selenium browser of a specified browser type
            Arguments:
            - browser_type: The desired browser (Chrome, Firefox, Edge, or IE).
            - browser_args: Selenium browser arguments, e.g. --headless.
            - persist: If set to True, will keep the browser open for later use.
+           - record_test: If set to True, will create a video recording during the time that the browser is open.
 
            Creates class variable moon_driver for access to selenium webdriver methods.
         """ 
 
         browser_options = {
             'edge': {
                 'options': webdriver.EdgeOptions(),
@@ -50,17 +53,26 @@
         # Prevent the default browser cleanup 
         if persist == True:
             Service.__del__ = lambda new_del: None
 
         # moon_driver not only creates a browser session, but also can be used in higher-order methods to access selenium methods, e.g. refresh(), maximize_window(), etc.
         self.moon_driver = browser_options[browser_type]['webdriver_create'](options=options)
 
+        # Creates VideoThread object.
+        if persist != True and record_test == True:
+            # Stops any previously running screenshot threads
+            if self.video_thread:
+                self.video_thread.stop()
+            self.video_thread = VideoThread(self.moon_driver)
+            if self.video_folder:
+                self.video_thread.video_folder = self.video_folder
+
         # write executor_url and session_id to a file named session_info.py for future use
         try:
-            session_info_file = open(os.path.dirname(os.path.realpath(__file__))+'\\session_info.py', 'w')
+            session_info_file = open(os.path.dirname(os.path.realpath(__file__))+'/session_info.py', 'w')
             session_info_file.write(f'executor_url="{self.moon_driver.command_executor._url}"\nsession_id="{self.moon_driver.session_id}"')
             session_info_file.close()
         except FileNotFoundError:
             pass
 
     def use_current_browser(self):
         """Allows for test executions to begin on the last opened browser
@@ -92,24 +104,35 @@
         RemoteWebDriver.execute = org_command_execute
 
 
     def cleanup_browser(self):
         """Attempts to tear down most recent browser.
            Kills all geckodriver.exe, chromedriver.exe, and msedgedriver.exe processes.
         """
+        if self.video_thread:
+            self.video_thread.stop()
+
         try:
             self.moon_driver.quit()
             self.moon_driver = None
-            os.remove(os.path.dirname(os.path.realpath(__file__))+'\\session_info.py')
-        except:
+        except AttributeError:
             pass
-        subprocess.call('taskkill /f /im geckodriver.exe', stdout=open(os.devnull, "wb"), stderr=open(os.devnull, "wb"))
-        subprocess.call('taskkill /f /im chromedriver.exe', stdout=open(os.devnull, "wb"), stderr=open(os.devnull, "wb"))
-        subprocess.call('taskkill /f /im msedgedriver.exe', stdout=open(os.devnull, "wb"), stderr=open(os.devnull, "wb"))
 
+        try:
+            os.remove(os.path.dirname(os.path.realpath(__file__))+'/session_info.py')
+        except FileNotFoundError:
+            pass
+        
+        processes = ["geckodriver.exe", "chromedriver.exe", "msedgedriver.exe"]
+        try:
+            for process in processes:
+                subprocess.call(f'taskkill /f /im {process}', stdout=open(os.devnull, "wb"), stderr=open(os.devnull, "wb"))
+        except FileNotFoundError:
+            pass
+            
     def navigate_to_page(self, url):
         """Attempts to navigate to a web page without first needing https or http prefix
            Arguments:
            - url: The desired url
         """
         
         if not url.startswith("https") and not url.startswith("http"):
```

### Comparing `moonrise-1.0.0/src/moonrise/Moon_Methods.py` & `moonrise-1.1.0/src/moonrise/Moon_Methods.py`

 * *Files identical despite different names*

### Comparing `moonrise-1.0.0/src/moonrise/__init__.py` & `moonrise-1.1.0/src/moonrise/__init__.py`

 * *Files identical despite different names*

### Comparing `moonrise-1.0.0/src/moonrise/__main__.py` & `moonrise-1.1.0/src/moonrise/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def import_modules(filepath):
         """Add relevant modules to path and to modules to examine for Moonrise tests and suites.
         """
 
         if ":" in filepath:
             dir_name = filepath
         else:
-            dir_name = os.getcwd() + "\\" + filepath
+            dir_name = os.getcwd() + "/" + filepath
 
         if os.path.isfile(dir_name):
             sys.path.append(os.path.abspath(os.path.join(dir_name, os.pardir)))
             module = os.path.basename(dir_name[:-3])
             modules.append(__import__(module))
         elif os.path.isdir(dir_name):
             sys.path.append(dir_name)
```

### Comparing `moonrise-1.0.0/src/moonrise.egg-info/PKG-INFO` & `moonrise-1.1.0/src/moonrise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonrise
-Version: 1.0.0
+Version: 1.1.0
 Summary: Test suite creation toolset with additional quality of life upgrades for using the selenium test framework.
 Home-page: https://github.com/Worakow1138/Moonrise
 Author: Christopher Diamond-Jones
 Author-email: christopher.jones1138@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

