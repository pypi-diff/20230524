# Comparing `tmp/bose-1.5.1.tar.gz` & `tmp/bose-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bose-1.5.1.tar", last modified: Mon May 22 11:20:43 2023, max compression
+gzip compressed data, was "bose-1.5.3.tar", last modified: Wed May 24 16:21:10 2023, max compression
```

## Comparing `bose-1.5.1.tar` & `bose-1.5.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 11:20:43.373329 bose-1.5.1/
--rw-rw-rw-   0        0        0     1460 2023-05-22 11:20:43.373329 bose-1.5.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-22 11:20:43.373329 bose-1.5.1/bose/
--rw-rw-rw-   0        0        0      340 2023-05-13 11:28:45.126433 bose-1.5.1/bose/__init__.py
--rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-1.5.1/bose/base_data.py
--rw-rw-rw-   0        0        0     4990 2023-05-18 07:22:46.924306 bose-1.5.1/bose/base_task.py
--rw-rw-rw-   0        0        0     9037 2023-05-13 23:12:33.521981 bose-1.5.1/bose/boss_driver.py
--rw-rw-rw-   0        0        0     9049 2023-05-22 11:19:35.255308 bose-1.5.1/bose/boss_undetected_driver.py
--rw-rw-rw-   0        0        0     7295 2023-05-13 11:28:17.686088 bose-1.5.1/bose/create_driver.py
--rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-1.5.1/bose/download_driver.py
--rw-rw-rw-   0        0        0     3185 2023-05-18 07:50:25.651854 bose-1.5.1/bose/local_storage.py
--rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-1.5.1/bose/local_storage_driver.py
--rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-1.5.1/bose/opponent.py
--rw-rw-rw-   0        0        0     3187 2023-05-15 09:11:34.318135 bose-1.5.1/bose/output.py
--rw-rw-rw-   0        0        0     1650 2023-05-13 11:28:17.687091 bose-1.5.1/bose/task_info.py
--rw-rw-rw-   0        0        0     3977 2023-05-13 13:31:08.141431 bose-1.5.1/bose/temp_mail.py
--rw-rw-rw-   0        0        0     7361 2023-05-10 09:24:37.900794 bose-1.5.1/bose/user_agent.py
--rw-rw-rw-   0        0        0     6050 2023-05-10 10:34:20.625623 bose-1.5.1/bose/utils.py
--rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-1.5.1/bose/wait.py
--rw-rw-rw-   0        0        0     1203 2023-05-09 07:09:28.075948 bose-1.5.1/bose/window_size.py
--rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     2328 2023-05-22 11:19:06.029461 bose-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 16:21:10.757282 bose-1.5.3/
+-rw-rw-rw-   0        0        0     1346 2023-05-24 16:21:10.757282 bose-1.5.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-24 16:21:10.756284 bose-1.5.3/bose/
+-rw-rw-rw-   0        0        0      340 2023-05-13 11:28:45.126433 bose-1.5.3/bose/__init__.py
+-rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-1.5.3/bose/base_data.py
+-rw-rw-rw-   0        0        0     4990 2023-05-18 07:22:46.924306 bose-1.5.3/bose/base_task.py
+-rw-rw-rw-   0        0        0     9039 2023-05-22 11:25:15.734584 bose-1.5.3/bose/boss_driver.py
+-rw-rw-rw-   0        0        0     9051 2023-05-22 11:25:15.732590 bose-1.5.3/bose/boss_undetected_driver.py
+-rw-rw-rw-   0        0        0     7295 2023-05-13 11:28:17.686088 bose-1.5.3/bose/create_driver.py
+-rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-1.5.3/bose/download_driver.py
+-rw-rw-rw-   0        0        0     3185 2023-05-18 07:50:25.651854 bose-1.5.3/bose/local_storage.py
+-rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-1.5.3/bose/local_storage_driver.py
+-rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-1.5.3/bose/opponent.py
+-rw-rw-rw-   0        0        0     3187 2023-05-15 09:11:34.318135 bose-1.5.3/bose/output.py
+-rw-rw-rw-   0        0        0     1650 2023-05-13 11:28:17.687091 bose-1.5.3/bose/task_info.py
+-rw-rw-rw-   0        0        0     3977 2023-05-13 13:31:08.141431 bose-1.5.3/bose/temp_mail.py
+-rw-rw-rw-   0        0        0     7361 2023-05-10 09:24:37.900794 bose-1.5.3/bose/user_agent.py
+-rw-rw-rw-   0        0        0     6050 2023-05-10 10:34:20.625623 bose-1.5.3/bose/utils.py
+-rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-1.5.3/bose/wait.py
+-rw-rw-rw-   0        0        0     1203 2023-05-09 07:09:28.075948 bose-1.5.3/bose/window_size.py
+-rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     2452 2023-05-24 16:20:28.885271 bose-1.5.3/setup.py
```

### Comparing `bose-1.5.1/PKG-INFO` & `bose-1.5.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 1.1
 Name: bose
-Version: 1.5.1
+Version: 1.5.3
 Summary: The Ultimate Web Scraping Framework
 Home-page: UNKNOWN
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
-Description: # Bose - The Ultimate Web Scraping Framework!
-        
-        Read Bose Documentation at https://www.omkar.cloud/bose/
+Description: UNKNOWN
 Keywords: crawler,framework,scraping,crawling,web-scraping,web-scraping-python,cloudflare-bypass,anti-detection,bot-detection,automation,webdriver,browser
 Platform: UNKNOWN
 Classifier: Framework :: Scrapy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bose-1.5.1/bose/base_data.py` & `bose-1.5.3/bose/base_data.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.1/bose/base_task.py` & `bose-1.5.3/bose/base_task.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.1/bose/boss_driver.py` & `bose-1.5.3/bose/boss_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,15 @@
         def is_starts_with(link):
             if search == None:
                 return True
             return search in link
 
         return list(filter(is_starts_with, filter(is_not_none, links)))
 
-    def is_in_page(self, target, wait=None, raiseException=False):
+    def is_in_page(self, target, wait=None, raise_exception=False):
 
         def check_page(driver, target):
             if isinstance(target, str):
                 return target in driver.current_url
             else:
                 for x in target:
                     if x in driver.current_url:
@@ -257,15 +257,15 @@
                 if check_page(self, target):
                     return True
 
                 sleep_time = 0.2
                 time += sleep_time
                 sleep(sleep_time)
 
-        if raiseException:
+        if raise_exception:
             raise Exception(f"Page {target} not found")
         return False
 
     def save_screenshot(self, filename=datetime.now().strftime('%Y-%m-%d_%H-%M-%S') + ".png"):
         try:
             saving_screenshot_at = relative_path(
                 f'{self.task_path}/{filename}', 0)
```

### Comparing `bose-1.5.1/bose/boss_undetected_driver.py` & `bose-1.5.3/bose/boss_undetected_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,15 @@
         def is_starts_with(link):
             if search == None:
                 return True
             return search in link
 
         return list(filter(is_starts_with, filter(is_not_none, links)))
 
-    def is_in_page(self, target, wait=None, raiseException=False):
+    def is_in_page(self, target, wait=None, raise_exception=False):
 
         def check_page(driver, target):
             if isinstance(target, str):
                 return target in driver.current_url
             else:
                 for x in target:
                     if x in driver.current_url:
@@ -257,15 +257,15 @@
                 if check_page(self, target):
                     return True
 
                 sleep_time = 0.2
                 time += sleep_time
                 sleep(sleep_time)
 
-        if raiseException:
+        if raise_exception:
             raise Exception(f"Page {target} not found")
         return False
 
     def save_screenshot(self, filename=datetime.now().strftime('%Y-%m-%d_%H-%M-%S') + ".png"):
         try:
             saving_screenshot_at = relative_path(
                 f'{self.task_path}/{filename}', 0)
```

### Comparing `bose-1.5.1/bose/create_driver.py` & `bose-1.5.3/bose/create_driver.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.1/bose/download_driver.py` & `bose-1.5.3/bose/download_driver.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.1/bose/local_storage.py` & `bose-1.5.3/bose/local_storage.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.1/bose/local_storage_driver.py` & `bose-1.5.3/bose/local_storage_driver.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.1/bose/output.py` & `bose-1.5.3/bose/output.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.1/bose/task_info.py` & `bose-1.5.3/bose/task_info.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.1/bose/temp_mail.py` & `bose-1.5.3/bose/temp_mail.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.1/bose/user_agent.py` & `bose-1.5.3/bose/user_agent.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.1/bose/utils.py` & `bose-1.5.3/bose/utils.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.1/bose/window_size.py` & `bose-1.5.3/bose/window_size.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.1/setup.py` & `bose-1.5.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,23 +13,27 @@
 extras_require = {}
 cpython_dependencies = [
     "PyDispatcher>=2.0.5",
 ]
 
 def get_description():
     try:
+      import pypandoc
+      long_description = pypandoc.convert_file('README.md', 'rst')
+      return long_description
+
       return open("README.md", encoding="utf-8").read()
     except:
       return None
     
 
 setup(
     name='bose',
     packages=['bose'],
-    version='1.5.1',
+    version='1.5.3',
     license='MIT',
     project_urls={
         "Documentation": "https://omkar.cloud/bose/docs/",
         "Source": "https://github.com/omkarcloud/boss",
         "Tracker": "https://github.com/omkarcloud/boss/issues",
     },
```

