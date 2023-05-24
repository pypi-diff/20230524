# Comparing `tmp/clevertable-2.2.0.tar.gz` & `tmp/clevertable-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clevertable-2.2.0.tar", last modified: Wed May 17 10:59:50 2023, max compression
+gzip compressed data, was "clevertable-2.3.0.tar", last modified: Wed May 24 04:39:08 2023, max compression
```

## Comparing `clevertable-2.2.0.tar` & `clevertable-2.3.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 10:59:50.448891 clevertable-2.2.0/
--rw-rw-rw-   0        0        0     1086 2023-04-21 11:55:46.000000 clevertable-2.2.0/LICENSE
--rw-rw-rw-   0        0        0    34866 2023-05-17 10:59:50.448891 clevertable-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    33096 2023-05-17 10:51:13.000000 clevertable-2.2.0/README.md
--rw-rw-rw-   0        0        0     1306 2023-05-17 10:57:33.000000 clevertable-2.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-17 10:59:50.449890 clevertable-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0      230 2023-04-21 12:00:42.000000 clevertable-2.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 10:59:50.372777 clevertable-2.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-17 10:59:50.435373 clevertable-2.2.0/src/clevertable/
--rw-rw-rw-   0        0        0     2761 2023-05-03 09:47:00.000000 clevertable-2.2.0/src/clevertable/Binary.py
--rw-rw-rw-   0        0        0      268 2023-05-17 09:40:22.000000 clevertable-2.2.0/src/clevertable/Const.py
--rw-rw-rw-   0        0        0     2948 2023-05-04 17:33:19.000000 clevertable-2.2.0/src/clevertable/ConversionProfile.py
--rw-rw-rw-   0        0        0     3803 2023-05-09 06:20:57.000000 clevertable-2.2.0/src/clevertable/Converter.py
--rw-rw-rw-   0        0        0     3672 2023-05-04 12:32:37.000000 clevertable-2.2.0/src/clevertable/DataFrameProfile.py
--rw-rw-rw-   0        0        0      924 2023-05-03 13:32:15.000000 clevertable-2.2.0/src/clevertable/Enumerate.py
--rw-rw-rw-   0        0        0      258 2023-05-01 13:13:02.000000 clevertable-2.2.0/src/clevertable/Flatten.py
--rw-rw-rw-   0        0        0     3857 2023-05-04 10:30:56.000000 clevertable-2.2.0/src/clevertable/Float.py
--rw-rw-rw-   0        0        0      877 2023-05-01 13:05:29.000000 clevertable-2.2.0/src/clevertable/ForEach.py
--rw-rw-rw-   0        0        0     4948 2023-05-17 10:26:00.000000 clevertable-2.2.0/src/clevertable/Function.py
--rw-rw-rw-   0        0        0      211 2023-05-01 14:33:13.000000 clevertable-2.2.0/src/clevertable/Id.py
--rw-rw-rw-   0        0        0      366 2023-05-01 17:38:30.000000 clevertable-2.2.0/src/clevertable/Ignore.py
--rw-rw-rw-   0        0        0     3018 2023-05-04 06:01:53.000000 clevertable-2.2.0/src/clevertable/Infer.py
--rw-rw-rw-   0        0        0      563 2023-05-03 06:07:00.000000 clevertable-2.2.0/src/clevertable/Label.py
--rw-rw-rw-   0        0        0     3302 2023-05-04 18:08:01.000000 clevertable-2.2.0/src/clevertable/List.py
--rw-rw-rw-   0        0        0     1343 2023-05-03 09:48:28.000000 clevertable-2.2.0/src/clevertable/Map.py
--rw-rw-rw-   0        0        0     1446 2023-05-04 18:08:46.000000 clevertable-2.2.0/src/clevertable/OneHot.py
--rw-rw-rw-   0        0        0     1836 2023-05-03 15:33:14.000000 clevertable-2.2.0/src/clevertable/Parallel.py
--rw-rw-rw-   0        0        0     2872 2023-05-04 05:25:50.000000 clevertable-2.2.0/src/clevertable/Pipeline.py
--rw-rw-rw-   0        0        0     6334 2023-05-04 05:34:03.000000 clevertable-2.2.0/src/clevertable/RecordProfile.py
--rw-rw-rw-   0        0        0      835 2023-05-04 12:11:29.000000 clevertable-2.2.0/src/clevertable/Split.py
--rw-rw-rw-   0        0        0     3370 2023-05-17 10:34:53.000000 clevertable-2.2.0/src/clevertable/StrictFunction.py
--rw-rw-rw-   0        0        0      989 2023-05-04 12:12:21.000000 clevertable-2.2.0/src/clevertable/Strip.py
--rw-rw-rw-   0        0        0     1159 2023-05-17 09:23:55.000000 clevertable-2.2.0/src/clevertable/Transpose.py
--rw-rw-rw-   0        0        0     2751 2023-05-10 15:17:59.000000 clevertable-2.2.0/src/clevertable/Try.py
--rw-rw-rw-   0        0        0      716 2023-05-17 10:57:33.000000 clevertable-2.2.0/src/clevertable/__init__.py
--rw-rw-rw-   0        0        0     1271 2023-05-04 11:54:43.000000 clevertable-2.2.0/src/clevertable/__main__.py
--rw-rw-rw-   0        0        0     2664 2023-05-17 09:41:23.000000 clevertable-2.2.0/src/clevertable/_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-17 10:59:50.447375 clevertable-2.2.0/src/clevertable.egg-info/
--rw-rw-rw-   0        0        0    34866 2023-05-17 10:59:50.000000 clevertable-2.2.0/src/clevertable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1044 2023-05-17 10:59:50.000000 clevertable-2.2.0/src/clevertable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 10:59:50.000000 clevertable-2.2.0/src/clevertable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-17 10:59:50.000000 clevertable-2.2.0/src/clevertable.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2023-05-17 10:59:50.000000 clevertable-2.2.0/src/clevertable.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-17 10:59:50.000000 clevertable-2.2.0/src/clevertable.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 04:39:08.151047 clevertable-2.3.0/
+-rw-rw-rw-   0        0        0     1086 2023-04-21 11:55:46.000000 clevertable-2.3.0/LICENSE
+-rw-rw-rw-   0        0        0    34868 2023-05-24 04:39:08.151047 clevertable-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    33098 2023-05-24 04:34:02.000000 clevertable-2.3.0/README.md
+-rw-rw-rw-   0        0        0     1306 2023-05-24 04:37:45.000000 clevertable-2.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 04:39:08.151047 clevertable-2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      230 2023-04-21 12:00:42.000000 clevertable-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:39:08.088130 clevertable-2.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 04:39:08.151047 clevertable-2.3.0/src/clevertable/
+-rw-rw-rw-   0        0        0     2761 2023-05-03 09:47:00.000000 clevertable-2.3.0/src/clevertable/Binary.py
+-rw-rw-rw-   0        0        0      268 2023-05-17 09:40:22.000000 clevertable-2.3.0/src/clevertable/Const.py
+-rw-rw-rw-   0        0        0     3016 2023-05-24 04:34:02.000000 clevertable-2.3.0/src/clevertable/ConversionProfile.py
+-rw-rw-rw-   0        0        0     3803 2023-05-09 06:20:57.000000 clevertable-2.3.0/src/clevertable/Converter.py
+-rw-rw-rw-   0        0        0     4074 2023-05-24 04:34:02.000000 clevertable-2.3.0/src/clevertable/DataFrameProfile.py
+-rw-rw-rw-   0        0        0      924 2023-05-03 13:32:15.000000 clevertable-2.3.0/src/clevertable/Enumerate.py
+-rw-rw-rw-   0        0        0      258 2023-05-01 13:13:02.000000 clevertable-2.3.0/src/clevertable/Flatten.py
+-rw-rw-rw-   0        0        0     3857 2023-05-04 10:30:56.000000 clevertable-2.3.0/src/clevertable/Float.py
+-rw-rw-rw-   0        0        0      877 2023-05-01 13:05:29.000000 clevertable-2.3.0/src/clevertable/ForEach.py
+-rw-rw-rw-   0        0        0     4948 2023-05-17 10:26:00.000000 clevertable-2.3.0/src/clevertable/Function.py
+-rw-rw-rw-   0        0        0      211 2023-05-01 14:33:13.000000 clevertable-2.3.0/src/clevertable/Id.py
+-rw-rw-rw-   0        0        0      366 2023-05-01 17:38:30.000000 clevertable-2.3.0/src/clevertable/Ignore.py
+-rw-rw-rw-   0        0        0     3018 2023-05-04 06:01:53.000000 clevertable-2.3.0/src/clevertable/Infer.py
+-rw-rw-rw-   0        0        0      563 2023-05-03 06:07:00.000000 clevertable-2.3.0/src/clevertable/Label.py
+-rw-rw-rw-   0        0        0     3302 2023-05-04 18:08:01.000000 clevertable-2.3.0/src/clevertable/List.py
+-rw-rw-rw-   0        0        0     1343 2023-05-03 09:48:28.000000 clevertable-2.3.0/src/clevertable/Map.py
+-rw-rw-rw-   0        0        0     1446 2023-05-04 18:08:46.000000 clevertable-2.3.0/src/clevertable/OneHot.py
+-rw-rw-rw-   0        0        0     1836 2023-05-03 15:33:14.000000 clevertable-2.3.0/src/clevertable/Parallel.py
+-rw-rw-rw-   0        0        0     2872 2023-05-04 05:25:50.000000 clevertable-2.3.0/src/clevertable/Pipeline.py
+-rw-rw-rw-   0        0        0     6829 2023-05-24 04:34:02.000000 clevertable-2.3.0/src/clevertable/RecordProfile.py
+-rw-rw-rw-   0        0        0      835 2023-05-04 12:11:29.000000 clevertable-2.3.0/src/clevertable/Split.py
+-rw-rw-rw-   0        0        0     3370 2023-05-17 10:34:53.000000 clevertable-2.3.0/src/clevertable/StrictFunction.py
+-rw-rw-rw-   0        0        0      989 2023-05-04 12:12:21.000000 clevertable-2.3.0/src/clevertable/Strip.py
+-rw-rw-rw-   0        0        0     1159 2023-05-17 09:23:55.000000 clevertable-2.3.0/src/clevertable/Transpose.py
+-rw-rw-rw-   0        0        0     2751 2023-05-10 15:17:59.000000 clevertable-2.3.0/src/clevertable/Try.py
+-rw-rw-rw-   0        0        0      716 2023-05-24 04:37:45.000000 clevertable-2.3.0/src/clevertable/__init__.py
+-rw-rw-rw-   0        0        0     1271 2023-05-04 11:54:43.000000 clevertable-2.3.0/src/clevertable/__main__.py
+-rw-rw-rw-   0        0        0     2664 2023-05-17 09:41:23.000000 clevertable-2.3.0/src/clevertable/_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:39:08.151047 clevertable-2.3.0/src/clevertable.egg-info/
+-rw-rw-rw-   0        0        0    34868 2023-05-24 04:39:08.000000 clevertable-2.3.0/src/clevertable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1044 2023-05-24 04:39:08.000000 clevertable-2.3.0/src/clevertable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 04:39:08.000000 clevertable-2.3.0/src/clevertable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-24 04:39:08.000000 clevertable-2.3.0/src/clevertable.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2023-05-24 04:39:08.000000 clevertable-2.3.0/src/clevertable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-24 04:39:08.000000 clevertable-2.3.0/src/clevertable.egg-info/top_level.txt
```

### Comparing `clevertable-2.2.0/LICENSE` & `clevertable-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clevertable-2.2.0/PKG-INFO` & `clevertable-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevertable
-Version: 2.2.0
+Version: 2.3.0
 Summary: Low effort conversion of tabular data into numerical values.
 Author: Tom Mohr
 License: MIT License
         
         Copyright (c) 2023 Tom Mohr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -69,17 +69,17 @@
 - If something is obvious, you should not need to specify it.
   CleverTable will try to make choices for you if you don't make them.
 - You stay in control: All choices made by CleverTable can be modified and overridden.
 
 This is how CleverTable works:
 
 1. You create a new `profile = ConversionProfile()`.
-   Here, you can specify certain converters, but you don't have to.
+   Here, you can optionally specify certain converters.
 2. You call `profile.fit(data)` on a sample data set, which creates a fixed conversion profile.
-    - CleverTable chooses the best converter if you don't specify it.
+    - CleverTable chooses the best converter for each column if you don't specify it.
     - The converter (chosen by you or by CleverTable) adapts its internal state to fit the data.
 3. You call `profile.transform(data)` on the actual data set (which may be the same as for `fit()`),
    which converts the data according to the fixed profile.
 
 Here are some examples on what you can do with CleverTable:
 
 - Chain multiple converters to achieve complex conversions:
@@ -111,15 +111,15 @@
   ```python
   my_weather_conv = profile["Weather"]            # e.g. OneHot()
   my_weather_categories = my_weather_conv.values  # e.g. ["sunny", "cloudy", "rainy"]
   ```
 
 # Tutorial
 
-Suppose you want to convert the following table of survey results into a 2D numpy array of numbers:
+Suppose you want to convert the following table of survey results in a 2D numpy array of numbers:
 
 | Country | Age | Diagnosis | Hospitalized | Education level | Symptoms        |
 |---------|-----|-----------|--------------|-----------------|-----------------|
 | China   | 32  | benign    | no           | University      | cough, fever    |
 | France  | 45  | cancer    | yes          | PhD             | fever           |
 | Italy   | 19  | benign    | yes          | High School     | cough           |
 | Germany | 56  | cancer    | yes          | High School     | fever and cough |
```

### Comparing `clevertable-2.2.0/README.md` & `clevertable-2.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 - If something is obvious, you should not need to specify it.
   CleverTable will try to make choices for you if you don't make them.
 - You stay in control: All choices made by CleverTable can be modified and overridden.
 
 This is how CleverTable works:
 
 1. You create a new `profile = ConversionProfile()`.
-   Here, you can specify certain converters, but you don't have to.
+   Here, you can optionally specify certain converters.
 2. You call `profile.fit(data)` on a sample data set, which creates a fixed conversion profile.
-    - CleverTable chooses the best converter if you don't specify it.
+    - CleverTable chooses the best converter for each column if you don't specify it.
     - The converter (chosen by you or by CleverTable) adapts its internal state to fit the data.
 3. You call `profile.transform(data)` on the actual data set (which may be the same as for `fit()`),
    which converts the data according to the fixed profile.
 
 Here are some examples on what you can do with CleverTable:
 
 - Chain multiple converters to achieve complex conversions:
@@ -74,15 +74,15 @@
   ```python
   my_weather_conv = profile["Weather"]            # e.g. OneHot()
   my_weather_categories = my_weather_conv.values  # e.g. ["sunny", "cloudy", "rainy"]
   ```
 
 # Tutorial
 
-Suppose you want to convert the following table of survey results into a 2D numpy array of numbers:
+Suppose you want to convert the following table of survey results in a 2D numpy array of numbers:
 
 | Country | Age | Diagnosis | Hospitalized | Education level | Symptoms        |
 |---------|-----|-----------|--------------|-----------------|-----------------|
 | China   | 32  | benign    | no           | University      | cough, fever    |
 | France  | 45  | cancer    | yes          | PhD             | fever           |
 | Italy   | 19  | benign    | yes          | High School     | cough           |
 | Germany | 56  | cancer    | yes          | High School     | fever and cough |
```

### Comparing `clevertable-2.2.0/pyproject.toml` & `clevertable-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clevertable"
-version = "2.2.0"
+version = "2.3.0"
 description = "Low effort conversion of tabular data into numerical values."
 readme = "README.md"
 authors = [{ name = "Tom Mohr" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -29,15 +29,15 @@
 [project.urls]
 Homepage = "https://github.com/tom-mohr/clevertable"
 
 [project.scripts]
 clevertable = "clevertable.__main__:main"
 
 [tool.bumpver]
-current_version = "2.2.0"
+current_version = "2.3.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `clevertable-2.2.0/src/clevertable/Binary.py` & `clevertable-2.3.0/src/clevertable/Binary.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.2.0/src/clevertable/ConversionProfile.py` & `clevertable-2.3.0/src/clevertable/ConversionProfile.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,17 +35,18 @@
     if type(val) == str:
         return val.strip().lower()
     return val
 
 
 class ConversionProfile(DataFrameProfile):
     def __init__(self, profile: dict[str, any] = None,
+                 ignore_undefined: bool = False,
                  ignore_uninferrable: bool = False,
                  pre_processing: Optional[Callable[[any], any]] = default_preprocessing):
-        super().__init__(profile, ignore_uninferrable, pre_processing)
+        super().__init__(profile, ignore_undefined, ignore_uninferrable, pre_processing)
 
     def fit(self, obj: pd.DataFrame | str) -> 'ConversionProfile':
         """
         Fit the conversion profile to the given DataFrame.
         If a filename is given, the DataFrame is loaded from the file first.
         :param obj: DataFrame or filename
         :return: self
```

### Comparing `clevertable-2.2.0/src/clevertable/Converter.py` & `clevertable-2.3.0/src/clevertable/Converter.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.2.0/src/clevertable/DataFrameProfile.py` & `clevertable-2.3.0/src/clevertable/DataFrameProfile.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,32 +5,35 @@
 import pandas as pd
 
 from .RecordProfile import RecordProfile
 
 
 class DataFrameProfile:
     def __init__(self, profile: dict[str, any] = None,
+                 ignore_undefined: bool = False,
                  ignore_uninferrable: bool = False,
                  pre_processing: Optional[Callable[[any], any]] = str.lower):
         """
         Wraps a RecordProfile and provides a DataFrame interface.
         Behind the scenes, this class simply takes the individual
         entries of a DataFrame and feeds them as records to the
         wrapped RecordProfile.
 
         :param profile: A dictionary that maps column names to converters.
-        :param ignore_uninferrable:
-        If True, there is no error when a column cannot be inferred, and it will be processed by an Ignore() converter,
-        leading to no output column.
-        :param pre_processing:
-        A function that is applied to each value before it is fed to the converters.
-        Every time the function fails (i.e. raises an exception), the original value is used.
+        :param ignore_undefined: If ``False``, all columns without a converter will be assigned a converter
+               automatically. If ``True``, these columns will be ignored instead, i.e. not produce any output columns.
+        :param ignore_uninferrable: If True, there is no error when a column cannot be inferred, and it will be
+               processed by an Ignore() converter, leading to no output column.
+        :param pre_processing: A function that is applied to each value before it is fed to the converters.
+               Every time the function fails (i.e. raises an exception), the original value is used.
         """
         self.pre_processing = pre_processing
-        self._record_profile = RecordProfile(profile, ignore_uninferrable=ignore_uninferrable)
+        self._record_profile = RecordProfile(profile,
+                                             ignore_undefined=ignore_undefined,
+                                             ignore_uninferrable=ignore_uninferrable)
 
     def fit(self, df: pd.DataFrame) -> 'DataFrameProfile':
         """
         Fit the profile to the given DataFrame.
         :param df: The DataFrame to fit to.
         :return: self
         """
```

### Comparing `clevertable-2.2.0/src/clevertable/Enumerate.py` & `clevertable-2.3.0/src/clevertable/Enumerate.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.2.0/src/clevertable/Float.py` & `clevertable-2.3.0/src/clevertable/Float.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.2.0/src/clevertable/ForEach.py` & `clevertable-2.3.0/src/clevertable/ForEach.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.2.0/src/clevertable/Function.py` & `clevertable-2.3.0/src/clevertable/Function.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.2.0/src/clevertable/Infer.py` & `clevertable-2.3.0/src/clevertable/Infer.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.2.0/src/clevertable/Label.py` & `clevertable-2.3.0/src/clevertable/Label.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.2.0/src/clevertable/List.py` & `clevertable-2.3.0/src/clevertable/List.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.2.0/src/clevertable/Map.py` & `clevertable-2.3.0/src/clevertable/Map.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.2.0/src/clevertable/OneHot.py` & `clevertable-2.3.0/src/clevertable/OneHot.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.2.0/src/clevertable/Parallel.py` & `clevertable-2.3.0/src/clevertable/Parallel.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.2.0/src/clevertable/Pipeline.py` & `clevertable-2.3.0/src/clevertable/Pipeline.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.2.0/src/clevertable/RecordProfile.py` & `clevertable-2.3.0/src/clevertable/RecordProfile.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,64 @@
 from .Converter import Converter
+from .Ignore import Ignore
 from .Infer import Infer
 from ._utils import _parse_converter, _flatten, _index_duplicates
 
 
 def _check_and_unpack(row: list) -> dict:
     # unpack a 1-element list with a dict
     assert len(row) == 1, "Expects a 1-element list with a dict"
     val = row[0]  # unpack 1-element list
     assert isinstance(val, dict), "Expects a 1-element list with a dict"
     return val
 
 
 class RecordProfile(Converter):
     def __init__(self, profile: dict[any, any] = None,
+                 ignore_undefined: bool = False,
                  ignore_uninferrable: bool = False):
         """
         Works on records (dicts).
         Takes a record, applies a different converter for each key (according to the given profile)
         and outputs a record with transformed keys and values.
         The new keys are computed using the label() function of the respective converter.
         Their cardinality must match the cardinality of the output of the converter.
 
         For keys that are not present in the profile but appear during fit(), the Infer() converter is used.
 
         Keys that are not present in the profile and weren't present during fit() are simply ignored.
 
         :param profile: Maps keys to converters.
-        :param ignore_uninferrable:
-        If True, keys which are not present in the profile and for which the converter
-        cannot be inferred during fit() are ignored during transform().
+        :param ignore_undefined: If ``False``, all columns without a converter will be assigned a converter
+               automatically. If ``True``, these columns will be ignored instead, i.e. not produce any output columns.
+        :param ignore_uninferrable: If ``True``, keys which are not present in the profile and for which the converter
+               cannot be inferred during ``fit()`` are ignored during transform().
         """
         self.profile: dict[any, Converter] = {}
         if profile:
             self.update(profile)  # parses converters
 
         self.keys: dict[any, list[any]] = {}  # cache for the output keys computed during fit()
 
-        self.ingore_uninferrable = ignore_uninferrable
+        self.ignore_undefined = ignore_undefined
+        self.ignore_uninferrable = ignore_uninferrable
 
     def fit(self, rows: list[list]):
         # unpack each row and check the type
         dicts = [_check_and_unpack(row) for row in rows]
 
         all_keys = {key for d in dicts for key in d.keys()}  # collect all possible keys present in the dicts
 
-        # replace missing converters with Infer()
+        # replace missing converters with Infer() or Ignore()
         for key in all_keys:
             if key not in self.profile:
-                self.profile[key] = Infer(ignore_uninferrable=self.ingore_uninferrable)
+                if self.ignore_undefined:
+                    self.profile[key] = Ignore()
+                else:
+                    self.profile[key] = Infer(ignore_uninferrable=self.ignore_uninferrable)
 
         # now actual fit
         for key, conv in self.profile.items():
             rows = [[d[key]] for d in dicts if key in d]
             if not rows:
                 raise ValueError(f"Not a single value for key '{key}' present int fit()!"
                                  f" You must at least provide one value to fit() for this key.")
```

### Comparing `clevertable-2.2.0/src/clevertable/Split.py` & `clevertable-2.3.0/src/clevertable/Split.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.2.0/src/clevertable/StrictFunction.py` & `clevertable-2.3.0/src/clevertable/StrictFunction.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.2.0/src/clevertable/Strip.py` & `clevertable-2.3.0/src/clevertable/Strip.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.2.0/src/clevertable/Transpose.py` & `clevertable-2.3.0/src/clevertable/Transpose.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.2.0/src/clevertable/Try.py` & `clevertable-2.3.0/src/clevertable/Try.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.2.0/src/clevertable/__init__.py` & `clevertable-2.3.0/src/clevertable/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.2.0"
+__version__ = "2.3.0"
 
 from .Binary import Binary
 from .Const import Const
 from .ConversionProfile import ConversionProfile
 from .Converter import Converter
 from .Enumerate import Enumerate
 from .Flatten import Flatten
```

### Comparing `clevertable-2.2.0/src/clevertable/__main__.py` & `clevertable-2.3.0/src/clevertable/__main__.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.2.0/src/clevertable/_utils.py` & `clevertable-2.3.0/src/clevertable/_utils.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.2.0/src/clevertable.egg-info/PKG-INFO` & `clevertable-2.3.0/src/clevertable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevertable
-Version: 2.2.0
+Version: 2.3.0
 Summary: Low effort conversion of tabular data into numerical values.
 Author: Tom Mohr
 License: MIT License
         
         Copyright (c) 2023 Tom Mohr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -69,17 +69,17 @@
 - If something is obvious, you should not need to specify it.
   CleverTable will try to make choices for you if you don't make them.
 - You stay in control: All choices made by CleverTable can be modified and overridden.
 
 This is how CleverTable works:
 
 1. You create a new `profile = ConversionProfile()`.
-   Here, you can specify certain converters, but you don't have to.
+   Here, you can optionally specify certain converters.
 2. You call `profile.fit(data)` on a sample data set, which creates a fixed conversion profile.
-    - CleverTable chooses the best converter if you don't specify it.
+    - CleverTable chooses the best converter for each column if you don't specify it.
     - The converter (chosen by you or by CleverTable) adapts its internal state to fit the data.
 3. You call `profile.transform(data)` on the actual data set (which may be the same as for `fit()`),
    which converts the data according to the fixed profile.
 
 Here are some examples on what you can do with CleverTable:
 
 - Chain multiple converters to achieve complex conversions:
@@ -111,15 +111,15 @@
   ```python
   my_weather_conv = profile["Weather"]            # e.g. OneHot()
   my_weather_categories = my_weather_conv.values  # e.g. ["sunny", "cloudy", "rainy"]
   ```
 
 # Tutorial
 
-Suppose you want to convert the following table of survey results into a 2D numpy array of numbers:
+Suppose you want to convert the following table of survey results in a 2D numpy array of numbers:
 
 | Country | Age | Diagnosis | Hospitalized | Education level | Symptoms        |
 |---------|-----|-----------|--------------|-----------------|-----------------|
 | China   | 32  | benign    | no           | University      | cough, fever    |
 | France  | 45  | cancer    | yes          | PhD             | fever           |
 | Italy   | 19  | benign    | yes          | High School     | cough           |
 | Germany | 56  | cancer    | yes          | High School     | fever and cough |
```

### Comparing `clevertable-2.2.0/src/clevertable.egg-info/SOURCES.txt` & `clevertable-2.3.0/src/clevertable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

