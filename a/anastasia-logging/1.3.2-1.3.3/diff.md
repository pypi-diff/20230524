# Comparing `tmp/anastasia_logging-1.3.2.tar.gz` & `tmp/anastasia_logging-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anastasia_logging-1.3.2.tar", max compression
+gzip compressed data, was "anastasia_logging-1.3.3.tar", max compression
```

## Comparing `anastasia_logging-1.3.2.tar` & `anastasia_logging-1.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     6447 2023-05-17 19:42:51.898783 anastasia_logging-1.3.2/README.md
--rw-r--r--   0        0        0    12541 2023-05-17 15:16:00.243593 anastasia_logging-1.3.2/anastasia_logging/__init__.py
--rw-r--r--   0        0        0       35 2023-05-09 14:56:24.294304 anastasia_logging-1.3.2/anastasia_logging/codes/__init__.py
--rw-r--r--   0        0        0     1200 2023-05-17 15:16:00.243593 anastasia_logging-1.3.2/anastasia_logging/codes/standard.py
--rw-r--r--   0        0        0       62 2023-05-17 15:40:56.723080 anastasia_logging-1.3.2/anastasia_logging/codes/standard_critical.py
--rw-r--r--   0        0        0       57 2023-05-17 15:40:56.723080 anastasia_logging-1.3.2/anastasia_logging/codes/standard_debug.py
--rw-r--r--   0        0        0       92 2023-05-08 16:28:55.501019 anastasia_logging-1.3.2/anastasia_logging/codes/standard_errors.py
--rw-r--r--   0        0        0       55 2023-05-08 16:28:55.505019 anastasia_logging-1.3.2/anastasia_logging/codes/standard_info.py
--rw-r--r--   0        0        0      118 2023-05-08 16:28:55.505019 anastasia_logging-1.3.2/anastasia_logging/codes/standard_warning.py
--rw-r--r--   0        0        0       47 2023-05-09 20:12:08.106577 anastasia_logging-1.3.2/anastasia_logging/env/__init__.py
--rw-r--r--   0        0        0      555 2023-05-17 19:49:11.232077 anastasia_logging-1.3.2/anastasia_logging/env/env_variables.py
--rw-r--r--   0        0        0    17527 2023-05-17 15:16:00.247593 anastasia_logging-1.3.2/anastasia_logging/logger.py
--rw-r--r--   0        0        0      285 2023-05-17 19:41:18.600499 anastasia_logging-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     6890 1970-01-01 00:00:00.000000 anastasia_logging-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     6590 2023-05-24 14:19:15.579312 anastasia_logging-1.3.3/README.md
+-rw-r--r--   0        0        0    12541 2023-05-17 15:16:00.243593 anastasia_logging-1.3.3/anastasia_logging/__init__.py
+-rw-r--r--   0        0        0       35 2023-05-09 14:56:24.294304 anastasia_logging-1.3.3/anastasia_logging/codes/__init__.py
+-rw-r--r--   0        0        0     1200 2023-05-17 15:16:00.243593 anastasia_logging-1.3.3/anastasia_logging/codes/standard.py
+-rw-r--r--   0        0        0       62 2023-05-17 15:40:56.723080 anastasia_logging-1.3.3/anastasia_logging/codes/standard_critical.py
+-rw-r--r--   0        0        0       57 2023-05-17 15:40:56.723080 anastasia_logging-1.3.3/anastasia_logging/codes/standard_debug.py
+-rw-r--r--   0        0        0       92 2023-05-08 16:28:55.501019 anastasia_logging-1.3.3/anastasia_logging/codes/standard_errors.py
+-rw-r--r--   0        0        0       55 2023-05-08 16:28:55.505019 anastasia_logging-1.3.3/anastasia_logging/codes/standard_info.py
+-rw-r--r--   0        0        0      118 2023-05-08 16:28:55.505019 anastasia_logging-1.3.3/anastasia_logging/codes/standard_warning.py
+-rw-r--r--   0        0        0       47 2023-05-09 20:12:08.106577 anastasia_logging-1.3.3/anastasia_logging/env/__init__.py
+-rw-r--r--   0        0        0      615 2023-05-24 14:13:42.445599 anastasia_logging-1.3.3/anastasia_logging/env/env_variables.py
+-rw-r--r--   0        0        0    17527 2023-05-17 15:16:00.247593 anastasia_logging-1.3.3/anastasia_logging/logger.py
+-rw-r--r--   0        0        0      285 2023-05-24 14:19:19.467336 anastasia_logging-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     7033 1970-01-01 00:00:00.000000 anastasia_logging-1.3.3/PKG-INFO
```

### Comparing `anastasia_logging-1.3.2/README.md` & `anastasia_logging-1.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,20 @@
 logging.print("Some prints to show")
 
 OUTPUT => 2023-05-08 11:55:27 UTC/GMT-0400 | [ANASTASIA-JOB] PRINT: Some prints to show
 ```
 
 ## **3. Versioning** ##
 
+### v1.3.3 ###
+
+* Fixes:
+
+    * Fixed edge case of ```ANASTASIA_LOG_SAVELOG``` environment variable detection if value entered is not a digit
+
 ### v1.3.2 ###
 
 * Fixes:
 
     * Fixed parameter assignation for ```ANASTASIA_LOG_SAVELOG``` environment variable
 
 ### v1.3.1 ###
```

### Comparing `anastasia_logging-1.3.2/anastasia_logging/__init__.py` & `anastasia_logging-1.3.3/anastasia_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `anastasia_logging-1.3.2/anastasia_logging/codes/standard.py` & `anastasia_logging-1.3.3/anastasia_logging/codes/standard.py`

 * *Files identical despite different names*

### Comparing `anastasia_logging-1.3.2/anastasia_logging/env/env_variables.py` & `anastasia_logging-1.3.3/anastasia_logging/env/env_variables.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,9 +8,9 @@
     Holds environment variables that AnastasiaLogger can recieve
 
     """
 
     ANASTASIA_LOG_NAME: str = os.getenv("ANASTASIA_LOG_NAME", "anastasia-log")
     ANASTASIA_LOG_TAG: str = os.getenv("ANASTASIA_LOG_TAG", "ANASTASIA-JOB")
     ANASTASIA_LOG_LEVEL: str = os.getenv("ANASTASIA_LOG_LEVEL", "INFO")
-    ANASTASIA_LOG_SAVELOG: int = int(os.getenv("ANASTASIA_LOG_SAVELOG", "0"))
+    ANASTASIA_LOG_SAVELOG: int = int(os.getenv("ANASTASIA_LOG_SAVELOG", "0")) if os.getenv("ANASTASIA_LOG_SAVELOG", "0").isdigit() else 0
     ANASTASIA_LOG_PATH: str = os.getenv("ANASTASIA_LOG_TAG", "anastasia-log.log")
```

### Comparing `anastasia_logging-1.3.2/anastasia_logging/logger.py` & `anastasia_logging-1.3.3/anastasia_logging/logger.py`

 * *Files identical despite different names*

### Comparing `anastasia_logging-1.3.2/PKG-INFO` & `anastasia_logging-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anastasia-logging
-Version: 1.3.2
+Version: 1.3.3
 Summary: Anastasia Logging Standarization
 Author: anastasiaai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -136,14 +136,20 @@
 logging.print("Some prints to show")
 
 OUTPUT => 2023-05-08 11:55:27 UTC/GMT-0400 | [ANASTASIA-JOB] PRINT: Some prints to show
 ```
 
 ## **3. Versioning** ##
 
+### v1.3.3 ###
+
+* Fixes:
+
+    * Fixed edge case of ```ANASTASIA_LOG_SAVELOG``` environment variable detection if value entered is not a digit
+
 ### v1.3.2 ###
 
 * Fixes:
 
     * Fixed parameter assignation for ```ANASTASIA_LOG_SAVELOG``` environment variable
 
 ### v1.3.1 ###
```

