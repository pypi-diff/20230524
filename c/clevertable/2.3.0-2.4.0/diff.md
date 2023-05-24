# Comparing `tmp/clevertable-2.3.0.tar.gz` & `tmp/clevertable-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clevertable-2.3.0.tar", last modified: Wed May 24 04:39:08 2023, max compression
+gzip compressed data, was "clevertable-2.4.0.tar", last modified: Wed May 24 09:03:34 2023, max compression
```

## Comparing `clevertable-2.3.0.tar` & `clevertable-2.4.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 04:39:08.151047 clevertable-2.3.0/
--rw-rw-rw-   0        0        0     1086 2023-04-21 11:55:46.000000 clevertable-2.3.0/LICENSE
--rw-rw-rw-   0        0        0    34868 2023-05-24 04:39:08.151047 clevertable-2.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    33098 2023-05-24 04:34:02.000000 clevertable-2.3.0/README.md
--rw-rw-rw-   0        0        0     1306 2023-05-24 04:37:45.000000 clevertable-2.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 04:39:08.151047 clevertable-2.3.0/setup.cfg
--rw-rw-rw-   0        0        0      230 2023-04-21 12:00:42.000000 clevertable-2.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:39:08.088130 clevertable-2.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 04:39:08.151047 clevertable-2.3.0/src/clevertable/
--rw-rw-rw-   0        0        0     2761 2023-05-03 09:47:00.000000 clevertable-2.3.0/src/clevertable/Binary.py
--rw-rw-rw-   0        0        0      268 2023-05-17 09:40:22.000000 clevertable-2.3.0/src/clevertable/Const.py
--rw-rw-rw-   0        0        0     3016 2023-05-24 04:34:02.000000 clevertable-2.3.0/src/clevertable/ConversionProfile.py
--rw-rw-rw-   0        0        0     3803 2023-05-09 06:20:57.000000 clevertable-2.3.0/src/clevertable/Converter.py
--rw-rw-rw-   0        0        0     4074 2023-05-24 04:34:02.000000 clevertable-2.3.0/src/clevertable/DataFrameProfile.py
--rw-rw-rw-   0        0        0      924 2023-05-03 13:32:15.000000 clevertable-2.3.0/src/clevertable/Enumerate.py
--rw-rw-rw-   0        0        0      258 2023-05-01 13:13:02.000000 clevertable-2.3.0/src/clevertable/Flatten.py
--rw-rw-rw-   0        0        0     3857 2023-05-04 10:30:56.000000 clevertable-2.3.0/src/clevertable/Float.py
--rw-rw-rw-   0        0        0      877 2023-05-01 13:05:29.000000 clevertable-2.3.0/src/clevertable/ForEach.py
--rw-rw-rw-   0        0        0     4948 2023-05-17 10:26:00.000000 clevertable-2.3.0/src/clevertable/Function.py
--rw-rw-rw-   0        0        0      211 2023-05-01 14:33:13.000000 clevertable-2.3.0/src/clevertable/Id.py
--rw-rw-rw-   0        0        0      366 2023-05-01 17:38:30.000000 clevertable-2.3.0/src/clevertable/Ignore.py
--rw-rw-rw-   0        0        0     3018 2023-05-04 06:01:53.000000 clevertable-2.3.0/src/clevertable/Infer.py
--rw-rw-rw-   0        0        0      563 2023-05-03 06:07:00.000000 clevertable-2.3.0/src/clevertable/Label.py
--rw-rw-rw-   0        0        0     3302 2023-05-04 18:08:01.000000 clevertable-2.3.0/src/clevertable/List.py
--rw-rw-rw-   0        0        0     1343 2023-05-03 09:48:28.000000 clevertable-2.3.0/src/clevertable/Map.py
--rw-rw-rw-   0        0        0     1446 2023-05-04 18:08:46.000000 clevertable-2.3.0/src/clevertable/OneHot.py
--rw-rw-rw-   0        0        0     1836 2023-05-03 15:33:14.000000 clevertable-2.3.0/src/clevertable/Parallel.py
--rw-rw-rw-   0        0        0     2872 2023-05-04 05:25:50.000000 clevertable-2.3.0/src/clevertable/Pipeline.py
--rw-rw-rw-   0        0        0     6829 2023-05-24 04:34:02.000000 clevertable-2.3.0/src/clevertable/RecordProfile.py
--rw-rw-rw-   0        0        0      835 2023-05-04 12:11:29.000000 clevertable-2.3.0/src/clevertable/Split.py
--rw-rw-rw-   0        0        0     3370 2023-05-17 10:34:53.000000 clevertable-2.3.0/src/clevertable/StrictFunction.py
--rw-rw-rw-   0        0        0      989 2023-05-04 12:12:21.000000 clevertable-2.3.0/src/clevertable/Strip.py
--rw-rw-rw-   0        0        0     1159 2023-05-17 09:23:55.000000 clevertable-2.3.0/src/clevertable/Transpose.py
--rw-rw-rw-   0        0        0     2751 2023-05-10 15:17:59.000000 clevertable-2.3.0/src/clevertable/Try.py
--rw-rw-rw-   0        0        0      716 2023-05-24 04:37:45.000000 clevertable-2.3.0/src/clevertable/__init__.py
--rw-rw-rw-   0        0        0     1271 2023-05-04 11:54:43.000000 clevertable-2.3.0/src/clevertable/__main__.py
--rw-rw-rw-   0        0        0     2664 2023-05-17 09:41:23.000000 clevertable-2.3.0/src/clevertable/_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:39:08.151047 clevertable-2.3.0/src/clevertable.egg-info/
--rw-rw-rw-   0        0        0    34868 2023-05-24 04:39:08.000000 clevertable-2.3.0/src/clevertable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1044 2023-05-24 04:39:08.000000 clevertable-2.3.0/src/clevertable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 04:39:08.000000 clevertable-2.3.0/src/clevertable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-24 04:39:08.000000 clevertable-2.3.0/src/clevertable.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2023-05-24 04:39:08.000000 clevertable-2.3.0/src/clevertable.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-24 04:39:08.000000 clevertable-2.3.0/src/clevertable.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 09:03:34.661159 clevertable-2.4.0/
+-rw-rw-rw-   0        0        0     1086 2023-04-21 11:55:46.000000 clevertable-2.4.0/LICENSE
+-rw-rw-rw-   0        0        0    34992 2023-05-24 09:03:34.661159 clevertable-2.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    33222 2023-05-24 08:31:40.000000 clevertable-2.4.0/README.md
+-rw-rw-rw-   0        0        0     1306 2023-05-24 09:02:54.000000 clevertable-2.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 09:03:34.661159 clevertable-2.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      230 2023-04-21 12:00:42.000000 clevertable-2.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:03:34.598636 clevertable-2.4.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 09:03:34.661159 clevertable-2.4.0/src/clevertable/
+-rw-rw-rw-   0        0        0     3512 2023-05-24 08:33:41.000000 clevertable-2.4.0/src/clevertable/Binary.py
+-rw-rw-rw-   0        0        0      268 2023-05-17 09:40:22.000000 clevertable-2.4.0/src/clevertable/Const.py
+-rw-rw-rw-   0        0        0     3016 2023-05-24 04:34:02.000000 clevertable-2.4.0/src/clevertable/ConversionProfile.py
+-rw-rw-rw-   0        0        0     3803 2023-05-09 06:20:57.000000 clevertable-2.4.0/src/clevertable/Converter.py
+-rw-rw-rw-   0        0        0     4074 2023-05-24 04:34:02.000000 clevertable-2.4.0/src/clevertable/DataFrameProfile.py
+-rw-rw-rw-   0        0        0      924 2023-05-03 13:32:15.000000 clevertable-2.4.0/src/clevertable/Enumerate.py
+-rw-rw-rw-   0        0        0      258 2023-05-01 13:13:02.000000 clevertable-2.4.0/src/clevertable/Flatten.py
+-rw-rw-rw-   0        0        0     3857 2023-05-04 10:30:56.000000 clevertable-2.4.0/src/clevertable/Float.py
+-rw-rw-rw-   0        0        0      877 2023-05-01 13:05:29.000000 clevertable-2.4.0/src/clevertable/ForEach.py
+-rw-rw-rw-   0        0        0     4948 2023-05-17 10:26:00.000000 clevertable-2.4.0/src/clevertable/Function.py
+-rw-rw-rw-   0        0        0      211 2023-05-01 14:33:13.000000 clevertable-2.4.0/src/clevertable/Id.py
+-rw-rw-rw-   0        0        0      366 2023-05-01 17:38:30.000000 clevertable-2.4.0/src/clevertable/Ignore.py
+-rw-rw-rw-   0        0        0     3018 2023-05-04 06:01:53.000000 clevertable-2.4.0/src/clevertable/Infer.py
+-rw-rw-rw-   0        0        0      402 2023-05-24 08:56:57.000000 clevertable-2.4.0/src/clevertable/Label.py
+-rw-rw-rw-   0        0        0     3302 2023-05-04 18:08:01.000000 clevertable-2.4.0/src/clevertable/List.py
+-rw-rw-rw-   0        0        0     1343 2023-05-03 09:48:28.000000 clevertable-2.4.0/src/clevertable/Map.py
+-rw-rw-rw-   0        0        0     1446 2023-05-04 18:08:46.000000 clevertable-2.4.0/src/clevertable/OneHot.py
+-rw-rw-rw-   0        0        0     1836 2023-05-03 15:33:14.000000 clevertable-2.4.0/src/clevertable/Parallel.py
+-rw-rw-rw-   0        0        0     2872 2023-05-04 05:25:50.000000 clevertable-2.4.0/src/clevertable/Pipeline.py
+-rw-rw-rw-   0        0        0     6829 2023-05-24 04:34:02.000000 clevertable-2.4.0/src/clevertable/RecordProfile.py
+-rw-rw-rw-   0        0        0      835 2023-05-04 12:11:29.000000 clevertable-2.4.0/src/clevertable/Split.py
+-rw-rw-rw-   0        0        0     3370 2023-05-17 10:34:53.000000 clevertable-2.4.0/src/clevertable/StrictFunction.py
+-rw-rw-rw-   0        0        0      989 2023-05-04 12:12:21.000000 clevertable-2.4.0/src/clevertable/Strip.py
+-rw-rw-rw-   0        0        0     1159 2023-05-17 09:23:55.000000 clevertable-2.4.0/src/clevertable/Transpose.py
+-rw-rw-rw-   0        0        0     2751 2023-05-10 15:17:59.000000 clevertable-2.4.0/src/clevertable/Try.py
+-rw-rw-rw-   0        0        0      716 2023-05-24 09:02:54.000000 clevertable-2.4.0/src/clevertable/__init__.py
+-rw-rw-rw-   0        0        0     1271 2023-05-04 11:54:43.000000 clevertable-2.4.0/src/clevertable/__main__.py
+-rw-rw-rw-   0        0        0     2664 2023-05-17 09:41:23.000000 clevertable-2.4.0/src/clevertable/_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:03:34.661159 clevertable-2.4.0/src/clevertable.egg-info/
+-rw-rw-rw-   0        0        0    34992 2023-05-24 09:03:34.000000 clevertable-2.4.0/src/clevertable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1044 2023-05-24 09:03:34.000000 clevertable-2.4.0/src/clevertable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 09:03:34.000000 clevertable-2.4.0/src/clevertable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-24 09:03:34.000000 clevertable-2.4.0/src/clevertable.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2023-05-24 09:03:34.000000 clevertable-2.4.0/src/clevertable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-24 09:03:34.000000 clevertable-2.4.0/src/clevertable.egg-info/top_level.txt
```

### Comparing `clevertable-2.3.0/LICENSE` & `clevertable-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clevertable-2.3.0/PKG-INFO` & `clevertable-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevertable
-Version: 2.3.0
+Version: 2.4.0
 Summary: Low effort conversion of tabular data into numerical values.
 Author: Tom Mohr
 License: MIT License
         
         Copyright (c) 2023 Tom Mohr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -60,21 +60,21 @@
 
 df = profile.fit_transform("datasets/survey.xlsx")  # transformed pandas.DataFrame
 ```
 
 # Why this Library?
 
 - CleverTable makes it really easy to convert text-based tabular data
-  (optionally mixed with numbers), e.g. a medical survey,
-  into numerical data, e.g. a Pandas DataFrame or a NumPy array.
+  (optionally mixed with numbers) into numerical data, e.g. a medical survey
+  into a Pandas DataFrame or a NumPy array.
 - If something is obvious, you should not need to specify it.
   CleverTable will try to make choices for you if you don't make them.
 - You stay in control: All choices made by CleverTable can be modified and overridden.
 
-This is how CleverTable works:
+This is how CleverTable works: (see below for a full [tutorial](#tutorial))
 
 1. You create a new `profile = ConversionProfile()`.
    Here, you can optionally specify certain converters.
 2. You call `profile.fit(data)` on a sample data set, which creates a fixed conversion profile.
     - CleverTable chooses the best converter for each column if you don't specify it.
     - The converter (chosen by you or by CleverTable) adapts its internal state to fit the data.
 3. You call `profile.transform(data)` on the actual data set (which may be the same as for `fit()`),
@@ -252,27 +252,26 @@
     "Country": OneHot(),
     "Diagnosis": Binary(positive="cancer", negative="benign"),
 }).fit(table)  # fit() returns self
 ```
 
 Two final notes:
 
-- You can ignore columns by setting their converter to `Ignore()"`.
-- You can use `fit_transform()` to perform `fit()` and `transform()`
-  in one step on the same data.
+- You can ignore columns by setting their converter to `None` (which is shorthand for the `Ignore()` converter).
+- You can use `fit_transform()` to perform `fit()` and `transform()` with the same data in one call.
 
 This leaves us with this very concise code:
 
 ```python
 from clevertable import *
 
 df = ConversionProfile({
     "Country": OneHot(),
     "Diagnosis": Binary(positive="cancer", negative="benign"),
-    "Hospitalized": Ignore(),
+    "Hospitalized": None,
 }, pre_processing=None).fit_transform("datasets/survey.xlsx")
 ```
 
 Which produces the following transformed table:
 
 | Country=China | Country=France | ... | Country=Zimbabwe | Age | Diagnosis | Education level=High School | Education level=PhD | Education level=University | Symptoms=cough | Symptoms=fever |
 |---------------|----------------|-----|------------------|-----|-----------|-----------------------------|---------------------|----------------------------|----------------|----------------|
@@ -341,15 +340,15 @@
 
 | Converters                            | Description                                                                         | Shorthand | Example Usage                                                   |
 |---------------------------------------|-------------------------------------------------------------------------------------|-----------|-----------------------------------------------------------------|
 | Basic:                                |                                                                                     |           |                                                                 |
 | [`Float()`](#float)                   | Convert numbers into floats.                                                        |           |                                                                 |
 | [`Enumerate()`](#enumerate)           |                                                                                     |           |                                                                 |
 | [`OneHot()`](#onehot)                 |                                                                                     |           |                                                                 |
-| [`Binary()`](#binary)                 | Convert a column of text into a column of integers.                                 |           |                                                                 |
+| [`Binary()`](#binary)                 | Convert to 0 and 1. Detects common "positive" and "negative" terms in strings.      |           |                                                                 |
 | [`List()`](#list)                     |                                                                                     |           |                                                                 |
 | [`ListAndOr()`](#listandor)           |                                                                                     |           |                                                                 |
 | [`Map()`](#map)                       |                                                                                     | dict      | {<br>&nbsp;&nbsp;"foo": 1,<br>&nbsp;&nbsp;"bar": -2,<br>}       |
 | [`Const()`](#const)                   | Return a constant value.                                                            | *any*     | 42<br>"foo"                                                     |
 | Text Processing:                      |                                                                                     |           |                                                                 |
 | [`Strip()`](#strip)                   |                                                                                     |           |                                                                 |
 | [`Split()`](#split)                   |                                                                                     |           |                                                                 |
@@ -448,15 +447,15 @@
 
 If no values are specified, the possible values are inferred from the data.
 
 ---
 
 ### Binary
 
-Similar to [`Enumerate()`](#enumerate), but only for columns with two possible values,
+Similar to [`Enumerate()`](#enumerate), but with just two possible values,
 and with some extra intelligence for this purpose.
 For example, it can detect words commonly used for positive and negative values:
 
 - Positive: `yes`, `true`, `positive`, `1`, `female`
 - Negative: `no`, `false`, `negative`, `0`, `male`, `none`
 
 Example:
@@ -476,59 +475,59 @@
 Results in:
 
 ```python
 "Hospitalized": Binary(positive={"yes", "true"},
                        negative={"no", "false", "none"})
 ```
 
-You can also specify the positive and negative values via the `positive` and `negative` arguments:
+You can explicitly specify the values of the `positive` class and the `negative` class via the constructor:
 
 ```python
 "Hospitalized": Binary(positive="yes", negative="no")
 ```
 
 | Hospitalized | ⇒ | Hospitalized |
 |--------------|---|--------------|
 | yes          |   | 1            |
 | no           |   | 0            |
 | no           |   | 0            |
 | yes          |   | 1            |
 
-If only one value is specified, all other values present in the data
-are treated as instances of the other class:
+If only one argument is specified (either `positive` or `negative`),
+all other values present in the data are treated as instances of the other class:
 
 ```python
 "Time served": Binary(negative="none")
 ```
 
 | Time served | ⇒ | Time served |
 |-------------|---|-------------|
 | none        |   | 0           |
 | 1 year      |   | 1           |
 | 4 years     |   | 1           |
 | none        |   | 0           |
 
-It is also possible to specify more than one values for the positive and negative values.
+It's also possible to specify more than one value for the ``positive`` and ``negative`` classes.
 Example:
 
 ```python
 "Hospitalized": Binary(positive={"yes", "true"}, negative={"no", "false"})
 ```
 
 | Hospitalized | ⇒ | Hospitalized |
 |--------------|---|--------------|
 | yes          |   | 1            |
 | no           |   | 0            |
 | false        |   | 0            |
 | true         |   | 1            |
 
-If no positive or negative value is specified, a set of strings commonly used
+If no positive or negative values are specified, a set of strings commonly used
 to indicate positive / negative values is tested against the available data.
 For instance, in the example above, the specified arguments would have been
-identified automatically as positive and negative.
+inferred automatically as positive and negative.
 
 If this approach is not successful, the lexically smallest value is chosen as the `negative` argument and
 the `positive` argument is left empty, causing all other values to be treated as positive:
 
 ```python
 "Fruits": Binary()
 ```
```

### Comparing `clevertable-2.3.0/README.md` & `clevertable-2.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 
 df = profile.fit_transform("datasets/survey.xlsx")  # transformed pandas.DataFrame
 ```
 
 # Why this Library?
 
 - CleverTable makes it really easy to convert text-based tabular data
-  (optionally mixed with numbers), e.g. a medical survey,
-  into numerical data, e.g. a Pandas DataFrame or a NumPy array.
+  (optionally mixed with numbers) into numerical data, e.g. a medical survey
+  into a Pandas DataFrame or a NumPy array.
 - If something is obvious, you should not need to specify it.
   CleverTable will try to make choices for you if you don't make them.
 - You stay in control: All choices made by CleverTable can be modified and overridden.
 
-This is how CleverTable works:
+This is how CleverTable works: (see below for a full [tutorial](#tutorial))
 
 1. You create a new `profile = ConversionProfile()`.
    Here, you can optionally specify certain converters.
 2. You call `profile.fit(data)` on a sample data set, which creates a fixed conversion profile.
     - CleverTable chooses the best converter for each column if you don't specify it.
     - The converter (chosen by you or by CleverTable) adapts its internal state to fit the data.
 3. You call `profile.transform(data)` on the actual data set (which may be the same as for `fit()`),
@@ -215,27 +215,26 @@
     "Country": OneHot(),
     "Diagnosis": Binary(positive="cancer", negative="benign"),
 }).fit(table)  # fit() returns self
 ```
 
 Two final notes:
 
-- You can ignore columns by setting their converter to `Ignore()"`.
-- You can use `fit_transform()` to perform `fit()` and `transform()`
-  in one step on the same data.
+- You can ignore columns by setting their converter to `None` (which is shorthand for the `Ignore()` converter).
+- You can use `fit_transform()` to perform `fit()` and `transform()` with the same data in one call.
 
 This leaves us with this very concise code:
 
 ```python
 from clevertable import *
 
 df = ConversionProfile({
     "Country": OneHot(),
     "Diagnosis": Binary(positive="cancer", negative="benign"),
-    "Hospitalized": Ignore(),
+    "Hospitalized": None,
 }, pre_processing=None).fit_transform("datasets/survey.xlsx")
 ```
 
 Which produces the following transformed table:
 
 | Country=China | Country=France | ... | Country=Zimbabwe | Age | Diagnosis | Education level=High School | Education level=PhD | Education level=University | Symptoms=cough | Symptoms=fever |
 |---------------|----------------|-----|------------------|-----|-----------|-----------------------------|---------------------|----------------------------|----------------|----------------|
@@ -304,15 +303,15 @@
 
 | Converters                            | Description                                                                         | Shorthand | Example Usage                                                   |
 |---------------------------------------|-------------------------------------------------------------------------------------|-----------|-----------------------------------------------------------------|
 | Basic:                                |                                                                                     |           |                                                                 |
 | [`Float()`](#float)                   | Convert numbers into floats.                                                        |           |                                                                 |
 | [`Enumerate()`](#enumerate)           |                                                                                     |           |                                                                 |
 | [`OneHot()`](#onehot)                 |                                                                                     |           |                                                                 |
-| [`Binary()`](#binary)                 | Convert a column of text into a column of integers.                                 |           |                                                                 |
+| [`Binary()`](#binary)                 | Convert to 0 and 1. Detects common "positive" and "negative" terms in strings.      |           |                                                                 |
 | [`List()`](#list)                     |                                                                                     |           |                                                                 |
 | [`ListAndOr()`](#listandor)           |                                                                                     |           |                                                                 |
 | [`Map()`](#map)                       |                                                                                     | dict      | {<br>&nbsp;&nbsp;"foo": 1,<br>&nbsp;&nbsp;"bar": -2,<br>}       |
 | [`Const()`](#const)                   | Return a constant value.                                                            | *any*     | 42<br>"foo"                                                     |
 | Text Processing:                      |                                                                                     |           |                                                                 |
 | [`Strip()`](#strip)                   |                                                                                     |           |                                                                 |
 | [`Split()`](#split)                   |                                                                                     |           |                                                                 |
@@ -411,15 +410,15 @@
 
 If no values are specified, the possible values are inferred from the data.
 
 ---
 
 ### Binary
 
-Similar to [`Enumerate()`](#enumerate), but only for columns with two possible values,
+Similar to [`Enumerate()`](#enumerate), but with just two possible values,
 and with some extra intelligence for this purpose.
 For example, it can detect words commonly used for positive and negative values:
 
 - Positive: `yes`, `true`, `positive`, `1`, `female`
 - Negative: `no`, `false`, `negative`, `0`, `male`, `none`
 
 Example:
@@ -439,59 +438,59 @@
 Results in:
 
 ```python
 "Hospitalized": Binary(positive={"yes", "true"},
                        negative={"no", "false", "none"})
 ```
 
-You can also specify the positive and negative values via the `positive` and `negative` arguments:
+You can explicitly specify the values of the `positive` class and the `negative` class via the constructor:
 
 ```python
 "Hospitalized": Binary(positive="yes", negative="no")
 ```
 
 | Hospitalized | ⇒ | Hospitalized |
 |--------------|---|--------------|
 | yes          |   | 1            |
 | no           |   | 0            |
 | no           |   | 0            |
 | yes          |   | 1            |
 
-If only one value is specified, all other values present in the data
-are treated as instances of the other class:
+If only one argument is specified (either `positive` or `negative`),
+all other values present in the data are treated as instances of the other class:
 
 ```python
 "Time served": Binary(negative="none")
 ```
 
 | Time served | ⇒ | Time served |
 |-------------|---|-------------|
 | none        |   | 0           |
 | 1 year      |   | 1           |
 | 4 years     |   | 1           |
 | none        |   | 0           |
 
-It is also possible to specify more than one values for the positive and negative values.
+It's also possible to specify more than one value for the ``positive`` and ``negative`` classes.
 Example:
 
 ```python
 "Hospitalized": Binary(positive={"yes", "true"}, negative={"no", "false"})
 ```
 
 | Hospitalized | ⇒ | Hospitalized |
 |--------------|---|--------------|
 | yes          |   | 1            |
 | no           |   | 0            |
 | false        |   | 0            |
 | true         |   | 1            |
 
-If no positive or negative value is specified, a set of strings commonly used
+If no positive or negative values are specified, a set of strings commonly used
 to indicate positive / negative values is tested against the available data.
 For instance, in the example above, the specified arguments would have been
-identified automatically as positive and negative.
+inferred automatically as positive and negative.
 
 If this approach is not successful, the lexically smallest value is chosen as the `negative` argument and
 the `positive` argument is left empty, causing all other values to be treated as positive:
 
 ```python
 "Fruits": Binary()
 ```
```

### Comparing `clevertable-2.3.0/pyproject.toml` & `clevertable-2.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clevertable"
-version = "2.3.0"
+version = "2.4.0"
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
-current_version = "2.3.0"
+current_version = "2.4.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `clevertable-2.3.0/src/clevertable/Binary.py` & `clevertable-2.4.0/src/clevertable/Binary.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,49 @@
 from __future__ import annotations
 
+from typing import Iterable
+
 from .Converter import Converter
 
 _COMMON_POSITIVE_STRINGS = {"yes", "true", "positive", "1", "female"}
 _COMMON_NEGATIVE_STRINGS = {"no", "false", "negative", "0", "male", "none"}
 
 
 class Binary(Converter):
 
     def __init__(self,
-                 positive: set | str = None,
-                 negative: set | str = None):
+                 positive: any = None,
+                 negative: any = None):
         """
         Converts values to 0 or 1.
+        :param positive: A value or an iterable of values that should be considered positive.
+        ``None`` is equivalent to passing an empty iterable.
+        :param negative: A value or an iterable of values that should be considered negative.
+        ``None`` is equivalent to passing an empty iterable.
         """
         # save args for __repr__
         self.__args_positive = positive
         self.__args_negative = negative
 
-        # wrap single values in sets
-        if type(positive) is str:
-            positive = {positive}
-        if type(negative) is str:
-            negative = {negative}
+        if positive is None:
+            positive = set()  # empty set
+        elif isinstance(positive, Iterable) and not isinstance(positive, str):  # non-string iterable
+            positive = set(positive)  # ensure set
+        else:
+            positive = {positive}  # wrap single value in set
+
+        if negative is None:
+            negative = set()  # empty set
+        elif isinstance(negative, Iterable) and not isinstance(negative, str):  # non-string iterable
+            negative = set(negative)  # ensure set
+        else:
+            negative = {negative}  # wrap single value in set
 
-        self.positive: set = positive or set()
-        self.negative: set = negative or set()
+        self.positive: set = positive
+        self.negative: set = negative
 
     def fit(self, rows: list[list]):
         if self.positive or self.negative:
             # at least either one positive or negative value was passed to the constructor,
             # -> no need to infer them from the data
             return
```

### Comparing `clevertable-2.3.0/src/clevertable/ConversionProfile.py` & `clevertable-2.4.0/src/clevertable/ConversionProfile.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.3.0/src/clevertable/Converter.py` & `clevertable-2.4.0/src/clevertable/Converter.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.3.0/src/clevertable/DataFrameProfile.py` & `clevertable-2.4.0/src/clevertable/DataFrameProfile.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.3.0/src/clevertable/Enumerate.py` & `clevertable-2.4.0/src/clevertable/Enumerate.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.3.0/src/clevertable/Float.py` & `clevertable-2.4.0/src/clevertable/Float.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.3.0/src/clevertable/ForEach.py` & `clevertable-2.4.0/src/clevertable/ForEach.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.3.0/src/clevertable/Function.py` & `clevertable-2.4.0/src/clevertable/Function.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.3.0/src/clevertable/Infer.py` & `clevertable-2.4.0/src/clevertable/Infer.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.3.0/src/clevertable/List.py` & `clevertable-2.4.0/src/clevertable/List.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.3.0/src/clevertable/Map.py` & `clevertable-2.4.0/src/clevertable/Map.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.3.0/src/clevertable/OneHot.py` & `clevertable-2.4.0/src/clevertable/OneHot.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.3.0/src/clevertable/Parallel.py` & `clevertable-2.4.0/src/clevertable/Parallel.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.3.0/src/clevertable/Pipeline.py` & `clevertable-2.4.0/src/clevertable/Pipeline.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.3.0/src/clevertable/RecordProfile.py` & `clevertable-2.4.0/src/clevertable/RecordProfile.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.3.0/src/clevertable/Split.py` & `clevertable-2.4.0/src/clevertable/Split.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.3.0/src/clevertable/StrictFunction.py` & `clevertable-2.4.0/src/clevertable/StrictFunction.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.3.0/src/clevertable/Strip.py` & `clevertable-2.4.0/src/clevertable/Strip.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.3.0/src/clevertable/Transpose.py` & `clevertable-2.4.0/src/clevertable/Transpose.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.3.0/src/clevertable/Try.py` & `clevertable-2.4.0/src/clevertable/Try.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.3.0/src/clevertable/__init__.py` & `clevertable-2.4.0/src/clevertable/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.3.0"
+__version__ = "2.4.0"
 
 from .Binary import Binary
 from .Const import Const
 from .ConversionProfile import ConversionProfile
 from .Converter import Converter
 from .Enumerate import Enumerate
 from .Flatten import Flatten
```

### Comparing `clevertable-2.3.0/src/clevertable/__main__.py` & `clevertable-2.4.0/src/clevertable/__main__.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.3.0/src/clevertable/_utils.py` & `clevertable-2.4.0/src/clevertable/_utils.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.3.0/src/clevertable.egg-info/PKG-INFO` & `clevertable-2.4.0/src/clevertable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevertable
-Version: 2.3.0
+Version: 2.4.0
 Summary: Low effort conversion of tabular data into numerical values.
 Author: Tom Mohr
 License: MIT License
         
         Copyright (c) 2023 Tom Mohr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -60,21 +60,21 @@
 
 df = profile.fit_transform("datasets/survey.xlsx")  # transformed pandas.DataFrame
 ```
 
 # Why this Library?
 
 - CleverTable makes it really easy to convert text-based tabular data
-  (optionally mixed with numbers), e.g. a medical survey,
-  into numerical data, e.g. a Pandas DataFrame or a NumPy array.
+  (optionally mixed with numbers) into numerical data, e.g. a medical survey
+  into a Pandas DataFrame or a NumPy array.
 - If something is obvious, you should not need to specify it.
   CleverTable will try to make choices for you if you don't make them.
 - You stay in control: All choices made by CleverTable can be modified and overridden.
 
-This is how CleverTable works:
+This is how CleverTable works: (see below for a full [tutorial](#tutorial))
 
 1. You create a new `profile = ConversionProfile()`.
    Here, you can optionally specify certain converters.
 2. You call `profile.fit(data)` on a sample data set, which creates a fixed conversion profile.
     - CleverTable chooses the best converter for each column if you don't specify it.
     - The converter (chosen by you or by CleverTable) adapts its internal state to fit the data.
 3. You call `profile.transform(data)` on the actual data set (which may be the same as for `fit()`),
@@ -252,27 +252,26 @@
     "Country": OneHot(),
     "Diagnosis": Binary(positive="cancer", negative="benign"),
 }).fit(table)  # fit() returns self
 ```
 
 Two final notes:
 
-- You can ignore columns by setting their converter to `Ignore()"`.
-- You can use `fit_transform()` to perform `fit()` and `transform()`
-  in one step on the same data.
+- You can ignore columns by setting their converter to `None` (which is shorthand for the `Ignore()` converter).
+- You can use `fit_transform()` to perform `fit()` and `transform()` with the same data in one call.
 
 This leaves us with this very concise code:
 
 ```python
 from clevertable import *
 
 df = ConversionProfile({
     "Country": OneHot(),
     "Diagnosis": Binary(positive="cancer", negative="benign"),
-    "Hospitalized": Ignore(),
+    "Hospitalized": None,
 }, pre_processing=None).fit_transform("datasets/survey.xlsx")
 ```
 
 Which produces the following transformed table:
 
 | Country=China | Country=France | ... | Country=Zimbabwe | Age | Diagnosis | Education level=High School | Education level=PhD | Education level=University | Symptoms=cough | Symptoms=fever |
 |---------------|----------------|-----|------------------|-----|-----------|-----------------------------|---------------------|----------------------------|----------------|----------------|
@@ -341,15 +340,15 @@
 
 | Converters                            | Description                                                                         | Shorthand | Example Usage                                                   |
 |---------------------------------------|-------------------------------------------------------------------------------------|-----------|-----------------------------------------------------------------|
 | Basic:                                |                                                                                     |           |                                                                 |
 | [`Float()`](#float)                   | Convert numbers into floats.                                                        |           |                                                                 |
 | [`Enumerate()`](#enumerate)           |                                                                                     |           |                                                                 |
 | [`OneHot()`](#onehot)                 |                                                                                     |           |                                                                 |
-| [`Binary()`](#binary)                 | Convert a column of text into a column of integers.                                 |           |                                                                 |
+| [`Binary()`](#binary)                 | Convert to 0 and 1. Detects common "positive" and "negative" terms in strings.      |           |                                                                 |
 | [`List()`](#list)                     |                                                                                     |           |                                                                 |
 | [`ListAndOr()`](#listandor)           |                                                                                     |           |                                                                 |
 | [`Map()`](#map)                       |                                                                                     | dict      | {<br>&nbsp;&nbsp;"foo": 1,<br>&nbsp;&nbsp;"bar": -2,<br>}       |
 | [`Const()`](#const)                   | Return a constant value.                                                            | *any*     | 42<br>"foo"                                                     |
 | Text Processing:                      |                                                                                     |           |                                                                 |
 | [`Strip()`](#strip)                   |                                                                                     |           |                                                                 |
 | [`Split()`](#split)                   |                                                                                     |           |                                                                 |
@@ -448,15 +447,15 @@
 
 If no values are specified, the possible values are inferred from the data.
 
 ---
 
 ### Binary
 
-Similar to [`Enumerate()`](#enumerate), but only for columns with two possible values,
+Similar to [`Enumerate()`](#enumerate), but with just two possible values,
 and with some extra intelligence for this purpose.
 For example, it can detect words commonly used for positive and negative values:
 
 - Positive: `yes`, `true`, `positive`, `1`, `female`
 - Negative: `no`, `false`, `negative`, `0`, `male`, `none`
 
 Example:
@@ -476,59 +475,59 @@
 Results in:
 
 ```python
 "Hospitalized": Binary(positive={"yes", "true"},
                        negative={"no", "false", "none"})
 ```
 
-You can also specify the positive and negative values via the `positive` and `negative` arguments:
+You can explicitly specify the values of the `positive` class and the `negative` class via the constructor:
 
 ```python
 "Hospitalized": Binary(positive="yes", negative="no")
 ```
 
 | Hospitalized | ⇒ | Hospitalized |
 |--------------|---|--------------|
 | yes          |   | 1            |
 | no           |   | 0            |
 | no           |   | 0            |
 | yes          |   | 1            |
 
-If only one value is specified, all other values present in the data
-are treated as instances of the other class:
+If only one argument is specified (either `positive` or `negative`),
+all other values present in the data are treated as instances of the other class:
 
 ```python
 "Time served": Binary(negative="none")
 ```
 
 | Time served | ⇒ | Time served |
 |-------------|---|-------------|
 | none        |   | 0           |
 | 1 year      |   | 1           |
 | 4 years     |   | 1           |
 | none        |   | 0           |
 
-It is also possible to specify more than one values for the positive and negative values.
+It's also possible to specify more than one value for the ``positive`` and ``negative`` classes.
 Example:
 
 ```python
 "Hospitalized": Binary(positive={"yes", "true"}, negative={"no", "false"})
 ```
 
 | Hospitalized | ⇒ | Hospitalized |
 |--------------|---|--------------|
 | yes          |   | 1            |
 | no           |   | 0            |
 | false        |   | 0            |
 | true         |   | 1            |
 
-If no positive or negative value is specified, a set of strings commonly used
+If no positive or negative values are specified, a set of strings commonly used
 to indicate positive / negative values is tested against the available data.
 For instance, in the example above, the specified arguments would have been
-identified automatically as positive and negative.
+inferred automatically as positive and negative.
 
 If this approach is not successful, the lexically smallest value is chosen as the `negative` argument and
 the `positive` argument is left empty, causing all other values to be treated as positive:
 
 ```python
 "Fruits": Binary()
 ```
```

### Comparing `clevertable-2.3.0/src/clevertable.egg-info/SOURCES.txt` & `clevertable-2.4.0/src/clevertable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

