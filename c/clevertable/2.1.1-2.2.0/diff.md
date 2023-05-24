# Comparing `tmp/clevertable-2.1.1.tar.gz` & `tmp/clevertable-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clevertable-2.1.1.tar", last modified: Wed May 10 15:58:02 2023, max compression
+gzip compressed data, was "clevertable-2.2.0.tar", last modified: Wed May 17 10:59:50 2023, max compression
```

## Comparing `clevertable-2.1.1.tar` & `clevertable-2.2.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 15:58:02.387510 clevertable-2.1.1/
--rw-rw-rw-   0        0        0     1086 2023-04-21 11:55:46.000000 clevertable-2.1.1/LICENSE
--rw-rw-rw-   0        0        0    31025 2023-05-10 15:58:02.386688 clevertable-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    29255 2023-05-10 15:55:34.000000 clevertable-2.1.1/README.md
--rw-rw-rw-   0        0        0     1306 2023-05-10 15:57:08.000000 clevertable-2.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-10 15:58:02.387510 clevertable-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0      230 2023-04-21 12:00:42.000000 clevertable-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 15:58:02.297219 clevertable-2.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 15:58:02.371991 clevertable-2.1.1/src/clevertable/
--rw-rw-rw-   0        0        0     2761 2023-05-03 09:47:00.000000 clevertable-2.1.1/src/clevertable/Binary.py
--rw-rw-rw-   0        0        0      268 2023-05-01 14:12:57.000000 clevertable-2.1.1/src/clevertable/Const.py
--rw-rw-rw-   0        0        0     2948 2023-05-04 17:33:19.000000 clevertable-2.1.1/src/clevertable/ConversionProfile.py
--rw-rw-rw-   0        0        0     3803 2023-05-09 06:20:57.000000 clevertable-2.1.1/src/clevertable/Converter.py
--rw-rw-rw-   0        0        0     3672 2023-05-04 12:32:37.000000 clevertable-2.1.1/src/clevertable/DataFrameProfile.py
--rw-rw-rw-   0        0        0      924 2023-05-03 13:32:15.000000 clevertable-2.1.1/src/clevertable/Enumerate.py
--rw-rw-rw-   0        0        0      258 2023-05-01 13:13:02.000000 clevertable-2.1.1/src/clevertable/Flatten.py
--rw-rw-rw-   0        0        0     3857 2023-05-04 10:30:56.000000 clevertable-2.1.1/src/clevertable/Float.py
--rw-rw-rw-   0        0        0      877 2023-05-01 13:05:29.000000 clevertable-2.1.1/src/clevertable/ForEach.py
--rw-rw-rw-   0        0        0     3864 2023-05-01 18:32:23.000000 clevertable-2.1.1/src/clevertable/Function.py
--rw-rw-rw-   0        0        0      211 2023-05-01 14:33:13.000000 clevertable-2.1.1/src/clevertable/Id.py
--rw-rw-rw-   0        0        0      366 2023-05-01 17:38:30.000000 clevertable-2.1.1/src/clevertable/Ignore.py
--rw-rw-rw-   0        0        0     3018 2023-05-04 06:01:53.000000 clevertable-2.1.1/src/clevertable/Infer.py
--rw-rw-rw-   0        0        0      563 2023-05-03 06:07:00.000000 clevertable-2.1.1/src/clevertable/Label.py
--rw-rw-rw-   0        0        0     3302 2023-05-04 18:08:01.000000 clevertable-2.1.1/src/clevertable/List.py
--rw-rw-rw-   0        0        0     1343 2023-05-03 09:48:28.000000 clevertable-2.1.1/src/clevertable/Map.py
--rw-rw-rw-   0        0        0     1446 2023-05-04 18:08:46.000000 clevertable-2.1.1/src/clevertable/OneHot.py
--rw-rw-rw-   0        0        0     1836 2023-05-03 15:33:14.000000 clevertable-2.1.1/src/clevertable/Parallel.py
--rw-rw-rw-   0        0        0     2872 2023-05-04 05:25:50.000000 clevertable-2.1.1/src/clevertable/Pipeline.py
--rw-rw-rw-   0        0        0     6334 2023-05-04 05:34:03.000000 clevertable-2.1.1/src/clevertable/RecordProfile.py
--rw-rw-rw-   0        0        0      835 2023-05-04 12:11:29.000000 clevertable-2.1.1/src/clevertable/Split.py
--rw-rw-rw-   0        0        0      989 2023-05-04 12:12:21.000000 clevertable-2.1.1/src/clevertable/Strip.py
--rw-rw-rw-   0        0        0      312 2023-05-01 14:33:36.000000 clevertable-2.1.1/src/clevertable/Transpose.py
--rw-rw-rw-   0        0        0     2751 2023-05-10 15:17:59.000000 clevertable-2.1.1/src/clevertable/Try.py
--rw-rw-rw-   0        0        0      672 2023-05-10 15:57:08.000000 clevertable-2.1.1/src/clevertable/__init__.py
--rw-rw-rw-   0        0        0     1271 2023-05-04 11:54:43.000000 clevertable-2.1.1/src/clevertable/__main__.py
--rw-rw-rw-   0        0        0     2664 2023-05-09 10:07:13.000000 clevertable-2.1.1/src/clevertable/_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-10 15:58:02.384986 clevertable-2.1.1/src/clevertable.egg-info/
--rw-rw-rw-   0        0        0    31025 2023-05-10 15:58:02.000000 clevertable-2.1.1/src/clevertable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1010 2023-05-10 15:58:02.000000 clevertable-2.1.1/src/clevertable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 15:58:02.000000 clevertable-2.1.1/src/clevertable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-10 15:58:02.000000 clevertable-2.1.1/src/clevertable.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2023-05-10 15:58:02.000000 clevertable-2.1.1/src/clevertable.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 15:58:02.000000 clevertable-2.1.1/src/clevertable.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 10:59:50.448891 clevertable-2.2.0/
+-rw-rw-rw-   0        0        0     1086 2023-04-21 11:55:46.000000 clevertable-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0    34866 2023-05-17 10:59:50.448891 clevertable-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    33096 2023-05-17 10:51:13.000000 clevertable-2.2.0/README.md
+-rw-rw-rw-   0        0        0     1306 2023-05-17 10:57:33.000000 clevertable-2.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-17 10:59:50.449890 clevertable-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      230 2023-04-21 12:00:42.000000 clevertable-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 10:59:50.372777 clevertable-2.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-17 10:59:50.435373 clevertable-2.2.0/src/clevertable/
+-rw-rw-rw-   0        0        0     2761 2023-05-03 09:47:00.000000 clevertable-2.2.0/src/clevertable/Binary.py
+-rw-rw-rw-   0        0        0      268 2023-05-17 09:40:22.000000 clevertable-2.2.0/src/clevertable/Const.py
+-rw-rw-rw-   0        0        0     2948 2023-05-04 17:33:19.000000 clevertable-2.2.0/src/clevertable/ConversionProfile.py
+-rw-rw-rw-   0        0        0     3803 2023-05-09 06:20:57.000000 clevertable-2.2.0/src/clevertable/Converter.py
+-rw-rw-rw-   0        0        0     3672 2023-05-04 12:32:37.000000 clevertable-2.2.0/src/clevertable/DataFrameProfile.py
+-rw-rw-rw-   0        0        0      924 2023-05-03 13:32:15.000000 clevertable-2.2.0/src/clevertable/Enumerate.py
+-rw-rw-rw-   0        0        0      258 2023-05-01 13:13:02.000000 clevertable-2.2.0/src/clevertable/Flatten.py
+-rw-rw-rw-   0        0        0     3857 2023-05-04 10:30:56.000000 clevertable-2.2.0/src/clevertable/Float.py
+-rw-rw-rw-   0        0        0      877 2023-05-01 13:05:29.000000 clevertable-2.2.0/src/clevertable/ForEach.py
+-rw-rw-rw-   0        0        0     4948 2023-05-17 10:26:00.000000 clevertable-2.2.0/src/clevertable/Function.py
+-rw-rw-rw-   0        0        0      211 2023-05-01 14:33:13.000000 clevertable-2.2.0/src/clevertable/Id.py
+-rw-rw-rw-   0        0        0      366 2023-05-01 17:38:30.000000 clevertable-2.2.0/src/clevertable/Ignore.py
+-rw-rw-rw-   0        0        0     3018 2023-05-04 06:01:53.000000 clevertable-2.2.0/src/clevertable/Infer.py
+-rw-rw-rw-   0        0        0      563 2023-05-03 06:07:00.000000 clevertable-2.2.0/src/clevertable/Label.py
+-rw-rw-rw-   0        0        0     3302 2023-05-04 18:08:01.000000 clevertable-2.2.0/src/clevertable/List.py
+-rw-rw-rw-   0        0        0     1343 2023-05-03 09:48:28.000000 clevertable-2.2.0/src/clevertable/Map.py
+-rw-rw-rw-   0        0        0     1446 2023-05-04 18:08:46.000000 clevertable-2.2.0/src/clevertable/OneHot.py
+-rw-rw-rw-   0        0        0     1836 2023-05-03 15:33:14.000000 clevertable-2.2.0/src/clevertable/Parallel.py
+-rw-rw-rw-   0        0        0     2872 2023-05-04 05:25:50.000000 clevertable-2.2.0/src/clevertable/Pipeline.py
+-rw-rw-rw-   0        0        0     6334 2023-05-04 05:34:03.000000 clevertable-2.2.0/src/clevertable/RecordProfile.py
+-rw-rw-rw-   0        0        0      835 2023-05-04 12:11:29.000000 clevertable-2.2.0/src/clevertable/Split.py
+-rw-rw-rw-   0        0        0     3370 2023-05-17 10:34:53.000000 clevertable-2.2.0/src/clevertable/StrictFunction.py
+-rw-rw-rw-   0        0        0      989 2023-05-04 12:12:21.000000 clevertable-2.2.0/src/clevertable/Strip.py
+-rw-rw-rw-   0        0        0     1159 2023-05-17 09:23:55.000000 clevertable-2.2.0/src/clevertable/Transpose.py
+-rw-rw-rw-   0        0        0     2751 2023-05-10 15:17:59.000000 clevertable-2.2.0/src/clevertable/Try.py
+-rw-rw-rw-   0        0        0      716 2023-05-17 10:57:33.000000 clevertable-2.2.0/src/clevertable/__init__.py
+-rw-rw-rw-   0        0        0     1271 2023-05-04 11:54:43.000000 clevertable-2.2.0/src/clevertable/__main__.py
+-rw-rw-rw-   0        0        0     2664 2023-05-17 09:41:23.000000 clevertable-2.2.0/src/clevertable/_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 10:59:50.447375 clevertable-2.2.0/src/clevertable.egg-info/
+-rw-rw-rw-   0        0        0    34866 2023-05-17 10:59:50.000000 clevertable-2.2.0/src/clevertable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1044 2023-05-17 10:59:50.000000 clevertable-2.2.0/src/clevertable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 10:59:50.000000 clevertable-2.2.0/src/clevertable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-17 10:59:50.000000 clevertable-2.2.0/src/clevertable.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2023-05-17 10:59:50.000000 clevertable-2.2.0/src/clevertable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-17 10:59:50.000000 clevertable-2.2.0/src/clevertable.egg-info/top_level.txt
```

### Comparing `clevertable-2.1.1/LICENSE` & `clevertable-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.1/PKG-INFO` & `clevertable-2.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,7 @@
-Metadata-Version: 2.1
-Name: clevertable
-Version: 2.1.1
-Summary: Low effort conversion of tabular data into numerical values.
-Author: Tom Mohr
-License: MIT License
-        
-        Copyright (c) 2023 Tom Mohr
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/tom-mohr/clevertable
-Keywords: parser,converter,numerical
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # CleverTable
 
 Consistent, intelligent transformation of text-based tabular data into numerical data.<br>
 Minimal configuration required.
 
 Installation:
 
@@ -335,43 +298,44 @@
 - `ConversionProfile`: A collection of converters.
 - `Converter`: Transforms columns of data into columns of data.
 
 ## Converters
 
 Here's a quick overview of all converters:
 
-| Converters                  | Description                                                                       | Shorthand  | Example Usage                                                   |
-|-----------------------------|-----------------------------------------------------------------------------------|------------|-----------------------------------------------------------------|
-| Basic:                      |                                                                                   |            |                                                                 |
-| [`Float()`](#float)         | Converts numbers into floats.                                                     |            |                                                                 |
-| [`Enumerate()`](#enumerate) |                                                                                   |            |                                                                 |
-| [`OneHot()`](#onehot)       |                                                                                   |            |                                                                 |
-| [`Binary()`](#binary)       | Converts a column of text into a column of integers.                              |            |                                                                 |
-| [`List()`](#list)           |                                                                                   |            |                                                                 |
-| [`ListAndOr()`](#listandor) |                                                                                   |            |                                                                 |
-| [`Map()`](#map)             |                                                                                   | dict       | {<br>&nbsp;&nbsp;"foo": 1,<br>&nbsp;&nbsp;"bar": -2,<br>}       |
-| [`Const()`](#const)         | Returns a constant value.                                                         | *any*      | 42<br>"foo"                                                     |
-| Text Processing:            |                                                                                   |            |                                                                 |
-| [`Strip()`](#strip)         |                                                                                   |            |                                                                 |
-| [`Split()`](#split)         |                                                                                   |            |                                                                 |
-| Combining Converters:       |                                                                                   |            |                                                                 |
-| [`Pipeline()`](#pipeline)   | Applies multiple converters in sequence.                                          | list       | [<br>&nbsp;&nbsp;Split(),<br>&nbsp;&nbsp;ForEach(Strip()),<br>] |
-| [`Try()`](#try)             | Try multiple converters and returns the first one that succeeds.                  | tuple      | (Float(), Binary())                                             |
-| [`ForEach()`](#foreach)     | Apply the same converter to all items.                                            |            |                                                                 |
-| [`Parallel()`](#parallel)   | Apply different converters to the respective items.                               |            |                                                                 |
-| Special:                    |                                                                                   |            |                                                                 |
-| [`Id()`](#id)               |                                                                                   |            |                                                                 |
-| [`Ignore()`](#ignore)       | Drops the column.                                                                 | None       | None                                                            |
-| [`Infer()`](#infer)         |                                                                                   |            |                                                                 |
-| [`Label()`](#label)         |                                                                                   |            |                                                                 |
-| Dimensionality:             |                                                                                   |            |                                                                 |
-| [`Flatten()`](#flatten)     | Flattens a list of lists into a single list. This is often needed after ForEach() |            |                                                                 |
-| [`Transpose()`](#transpose) |                                                                                   |            |                                                                 |
-| Arbitrary Functions:        |                                                                                   |            |                                                                 |
-| [`Function()`](#function)   | Applies a user-defined function to the data.                                      | *callable* | lambda x: x**2                                                  |
+| Converters                            | Description                                                                         | Shorthand | Example Usage                                                   |
+|---------------------------------------|-------------------------------------------------------------------------------------|-----------|-----------------------------------------------------------------|
+| Basic:                                |                                                                                     |           |                                                                 |
+| [`Float()`](#float)                   | Convert numbers into floats.                                                        |           |                                                                 |
+| [`Enumerate()`](#enumerate)           |                                                                                     |           |                                                                 |
+| [`OneHot()`](#onehot)                 |                                                                                     |           |                                                                 |
+| [`Binary()`](#binary)                 | Convert a column of text into a column of integers.                                 |           |                                                                 |
+| [`List()`](#list)                     |                                                                                     |           |                                                                 |
+| [`ListAndOr()`](#listandor)           |                                                                                     |           |                                                                 |
+| [`Map()`](#map)                       |                                                                                     | dict      | {<br>&nbsp;&nbsp;"foo": 1,<br>&nbsp;&nbsp;"bar": -2,<br>}       |
+| [`Const()`](#const)                   | Return a constant value.                                                            | *any*     | 42<br>"foo"                                                     |
+| Text Processing:                      |                                                                                     |           |                                                                 |
+| [`Strip()`](#strip)                   |                                                                                     |           |                                                                 |
+| [`Split()`](#split)                   |                                                                                     |           |                                                                 |
+| Combining Converters:                 |                                                                                     |           |                                                                 |
+| [`Pipeline()`](#pipeline)             | Apply multiple converters in sequence.                                              | list      | [<br>&nbsp;&nbsp;Split(),<br>&nbsp;&nbsp;ForEach(Strip()),<br>] |
+| [`Try()`](#try)                       | Try multiple converters and return the first one that succeeds.                     | tuple     | (Float(), Binary())                                             |
+| [`ForEach()`](#foreach)               | Apply the same converter to all items.                                              |           |                                                                 |
+| [`Parallel()`](#parallel)             | Apply different converters to the respective items.                                 |           |                                                                 |
+| Special:                              |                                                                                     |           |                                                                 |
+| [`Id()`](#id)                         |                                                                                     |           |                                                                 |
+| [`Ignore()`](#ignore)                 | Drop the column.                                                                    | None      | None                                                            |
+| [`Infer()`](#infer)                   |                                                                                     |           |                                                                 |
+| [`Label()`](#label)                   |                                                                                     |           |                                                                 |
+| Dimensionality:                       |                                                                                     |           |                                                                 |
+| [`Flatten()`](#flatten)               | Flatten a list of lists into a single list. This is often needed after `ForEach()`. |           |                                                                 |
+| [`Transpose()`](#transpose)           |                                                                                     |           |                                                                 |
+| Arbitrary Functions:                  |                                                                                     |           |                                                                 |
+| [`Function()`](#function)             | Apply a user-defined function to the data.                                          | callable  | lambda x: x**2                                                  |
+| [`StrictFunction()`](#strictfunction) | Apply a user-defined function to the data. Less flexible than `Function()`.         |           |                                                                 |
 
 ---
 
 ### Float
 
 Converts a column of numbers into a column of numbers.
 If invalid values are encountered (`NaN`, `inf`, `None`, etc.),
@@ -699,15 +663,59 @@
 ```
 
 `Transpose()` allows us to apply `max` to each column of the one-hot encodings
 across all list elements.
 
 ### Function
 
-This can be used to specify a custom conversion function.
+```python
+Function(transform, labels=None)
+```
+
+Shorthand: Instead of `Function(transform, None)`, just write `transform`, where `transform` is some callable.
+
+Creates a custom converter from a custom ``transform()`` function
+(and optionally, a custom ``labels()`` function).
+This is a handy way to create a converter that doesn't need ``fit()``.
+
+Unlike ``StrictFunction()``, this class can handle functions that don't accept or return lists,
+which often allows for more concise code.
+
+This is achieved during ``fit()`` as follows:
+
+1. If all incoming items are 1-element lists, it sets a flag ``UNPACK_OUTPUT`` to always
+   unpack the element before passing them to the wrapped function during ``transform()``.
+2. If during ``fit()`` the wrapped function doesn't return lists,
+   it tries to turn that output into a list:
+    - If the output is always a non-string iterable, it will simply set a
+      flag ``CONVERT_ITERABLE`` to always convert the iterable output into a list during ``transform()``.
+    - Otherwise, it sets a flag ``WRAP_OUTPUT`` to always wrap the output in a
+      1-element list during ``transform()``.
+
+A similar logic is applied to the labels.
+If a custom labels function is given, the following procedure is followed during ``labels()``:
+
+1. If the incoming labels are a 1-element list, the single label is unpacked before
+   it is passed to the custom labels function.
+2. If the custom labels function returns something other than a list,
+   this class tries to convert it into a list:
+    - If the output is a non-string iterable, it is converted into a list.
+    - Otherwise, the output is wrapped in a 1-element list.
+
+If no custom labels function is given, the output labels are generated based on the
+output cardinality inferred during ``fit()`` and according to the following logic:
+
+- If the number of incoming labels is identical to the output cardinality,
+  the labels will be returned unchanged.
+- Otherwise, the number of incoming labels must be 1 and the output labels are generated by adding suffixes
+  ``_0``, ``_1``, etc. to the single input label.
+
+A special case are functions returning output of varying cardinality during ``fit()``.
+In this case, a single input label is returned.
+If multiple input labels are given, they are joined with ``_``.
 
 The following example turns a text column into two columns containing the ascii code of the first and last letter.
 
 ```python
 "Name": lambda x: (ord(x[0]), ord(x[-1]))
 ```
 
@@ -722,23 +730,58 @@
 As you can see, the number of columns is inferred directly from the return value of the conversion function.
 If the function returns a list, the resulting column names are indexed.
 
 You can also set the labels explicitly with a lambda function
 that takes the input column name as an argument and returns output column names:
 
 ```python
-"Name": Function(lambda x: (ord(x[0]), ord(x[-1])),
+"Name": Function(lambda x: [ord(x[0]), ord(x[-1])],
                  labels=lambda s: [f"ord(first letter of {s})", f"ord(last letter of {s})"]),
 ```
 
 | Name  | ⇒ | ord(first letter of Name) | ord(last letter of Name) |
 |-------|---|---------------------------|--------------------------|
 | Alice |   | 97                        | 101                      |
 | Bob   |   | 98                        | 98                       |
 
+However, remember that you can always simply use [`Label()`](#label) to rename the columns after the conversion,
+if you don't need the output column names to depend on the input column names.
+
+```python
+"Name": [lambda x: [ord(x[0]), ord(x[-1])],
+         Labels("ord(first letter)", "ord(last letter)")],
+```
+
+### StrictFunction
+
+```python
+StrictFunction(transform, labels=None)
+```
+
+Works mostly like [`Function()`](#function), but simpler:
+``transform`` and ``labels`` must both accept and return lists.
+Instead of something like this:
+
+```python
+"Name": str.lower,
+```
+
+you have to write this:
+
+```python
+"Name": StrictFunction(lambda x: [str.lower(x[0])])
+```
+
+That is, you will still receive 1-element lists as lists to the function,
+even if all input elements during `fit()` are 1-element lists.
+Also, you must now explicitly return a list,
+even if it is just a 1-element list, as otherwise an error will be raised.
+
+See [`Function()`](#function) for a convenient extension of this converter.
+
 ---
 
 ## Understanding Multi-Column Converters
 
 A converter returns two things:
 
 - `transform()`: the items of the transformed data
```

### Comparing `clevertable-2.1.1/README.md` & `clevertable-2.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,44 @@
+Metadata-Version: 2.1
+Name: clevertable
+Version: 2.2.0
+Summary: Low effort conversion of tabular data into numerical values.
+Author: Tom Mohr
+License: MIT License
+        
+        Copyright (c) 2023 Tom Mohr
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/tom-mohr/clevertable
+Keywords: parser,converter,numerical
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # CleverTable
 
 Consistent, intelligent transformation of text-based tabular data into numerical data.<br>
 Minimal configuration required.
 
 Installation:
 
@@ -298,43 +335,44 @@
 - `ConversionProfile`: A collection of converters.
 - `Converter`: Transforms columns of data into columns of data.
 
 ## Converters
 
 Here's a quick overview of all converters:
 
-| Converters                  | Description                                                                       | Shorthand  | Example Usage                                                   |
-|-----------------------------|-----------------------------------------------------------------------------------|------------|-----------------------------------------------------------------|
-| Basic:                      |                                                                                   |            |                                                                 |
-| [`Float()`](#float)         | Converts numbers into floats.                                                     |            |                                                                 |
-| [`Enumerate()`](#enumerate) |                                                                                   |            |                                                                 |
-| [`OneHot()`](#onehot)       |                                                                                   |            |                                                                 |
-| [`Binary()`](#binary)       | Converts a column of text into a column of integers.                              |            |                                                                 |
-| [`List()`](#list)           |                                                                                   |            |                                                                 |
-| [`ListAndOr()`](#listandor) |                                                                                   |            |                                                                 |
-| [`Map()`](#map)             |                                                                                   | dict       | {<br>&nbsp;&nbsp;"foo": 1,<br>&nbsp;&nbsp;"bar": -2,<br>}       |
-| [`Const()`](#const)         | Returns a constant value.                                                         | *any*      | 42<br>"foo"                                                     |
-| Text Processing:            |                                                                                   |            |                                                                 |
-| [`Strip()`](#strip)         |                                                                                   |            |                                                                 |
-| [`Split()`](#split)         |                                                                                   |            |                                                                 |
-| Combining Converters:       |                                                                                   |            |                                                                 |
-| [`Pipeline()`](#pipeline)   | Applies multiple converters in sequence.                                          | list       | [<br>&nbsp;&nbsp;Split(),<br>&nbsp;&nbsp;ForEach(Strip()),<br>] |
-| [`Try()`](#try)             | Try multiple converters and returns the first one that succeeds.                  | tuple      | (Float(), Binary())                                             |
-| [`ForEach()`](#foreach)     | Apply the same converter to all items.                                            |            |                                                                 |
-| [`Parallel()`](#parallel)   | Apply different converters to the respective items.                               |            |                                                                 |
-| Special:                    |                                                                                   |            |                                                                 |
-| [`Id()`](#id)               |                                                                                   |            |                                                                 |
-| [`Ignore()`](#ignore)       | Drops the column.                                                                 | None       | None                                                            |
-| [`Infer()`](#infer)         |                                                                                   |            |                                                                 |
-| [`Label()`](#label)         |                                                                                   |            |                                                                 |
-| Dimensionality:             |                                                                                   |            |                                                                 |
-| [`Flatten()`](#flatten)     | Flattens a list of lists into a single list. This is often needed after ForEach() |            |                                                                 |
-| [`Transpose()`](#transpose) |                                                                                   |            |                                                                 |
-| Arbitrary Functions:        |                                                                                   |            |                                                                 |
-| [`Function()`](#function)   | Applies a user-defined function to the data.                                      | *callable* | lambda x: x**2                                                  |
+| Converters                            | Description                                                                         | Shorthand | Example Usage                                                   |
+|---------------------------------------|-------------------------------------------------------------------------------------|-----------|-----------------------------------------------------------------|
+| Basic:                                |                                                                                     |           |                                                                 |
+| [`Float()`](#float)                   | Convert numbers into floats.                                                        |           |                                                                 |
+| [`Enumerate()`](#enumerate)           |                                                                                     |           |                                                                 |
+| [`OneHot()`](#onehot)                 |                                                                                     |           |                                                                 |
+| [`Binary()`](#binary)                 | Convert a column of text into a column of integers.                                 |           |                                                                 |
+| [`List()`](#list)                     |                                                                                     |           |                                                                 |
+| [`ListAndOr()`](#listandor)           |                                                                                     |           |                                                                 |
+| [`Map()`](#map)                       |                                                                                     | dict      | {<br>&nbsp;&nbsp;"foo": 1,<br>&nbsp;&nbsp;"bar": -2,<br>}       |
+| [`Const()`](#const)                   | Return a constant value.                                                            | *any*     | 42<br>"foo"                                                     |
+| Text Processing:                      |                                                                                     |           |                                                                 |
+| [`Strip()`](#strip)                   |                                                                                     |           |                                                                 |
+| [`Split()`](#split)                   |                                                                                     |           |                                                                 |
+| Combining Converters:                 |                                                                                     |           |                                                                 |
+| [`Pipeline()`](#pipeline)             | Apply multiple converters in sequence.                                              | list      | [<br>&nbsp;&nbsp;Split(),<br>&nbsp;&nbsp;ForEach(Strip()),<br>] |
+| [`Try()`](#try)                       | Try multiple converters and return the first one that succeeds.                     | tuple     | (Float(), Binary())                                             |
+| [`ForEach()`](#foreach)               | Apply the same converter to all items.                                              |           |                                                                 |
+| [`Parallel()`](#parallel)             | Apply different converters to the respective items.                                 |           |                                                                 |
+| Special:                              |                                                                                     |           |                                                                 |
+| [`Id()`](#id)                         |                                                                                     |           |                                                                 |
+| [`Ignore()`](#ignore)                 | Drop the column.                                                                    | None      | None                                                            |
+| [`Infer()`](#infer)                   |                                                                                     |           |                                                                 |
+| [`Label()`](#label)                   |                                                                                     |           |                                                                 |
+| Dimensionality:                       |                                                                                     |           |                                                                 |
+| [`Flatten()`](#flatten)               | Flatten a list of lists into a single list. This is often needed after `ForEach()`. |           |                                                                 |
+| [`Transpose()`](#transpose)           |                                                                                     |           |                                                                 |
+| Arbitrary Functions:                  |                                                                                     |           |                                                                 |
+| [`Function()`](#function)             | Apply a user-defined function to the data.                                          | callable  | lambda x: x**2                                                  |
+| [`StrictFunction()`](#strictfunction) | Apply a user-defined function to the data. Less flexible than `Function()`.         |           |                                                                 |
 
 ---
 
 ### Float
 
 Converts a column of numbers into a column of numbers.
 If invalid values are encountered (`NaN`, `inf`, `None`, etc.),
@@ -662,15 +700,59 @@
 ```
 
 `Transpose()` allows us to apply `max` to each column of the one-hot encodings
 across all list elements.
 
 ### Function
 
-This can be used to specify a custom conversion function.
+```python
+Function(transform, labels=None)
+```
+
+Shorthand: Instead of `Function(transform, None)`, just write `transform`, where `transform` is some callable.
+
+Creates a custom converter from a custom ``transform()`` function
+(and optionally, a custom ``labels()`` function).
+This is a handy way to create a converter that doesn't need ``fit()``.
+
+Unlike ``StrictFunction()``, this class can handle functions that don't accept or return lists,
+which often allows for more concise code.
+
+This is achieved during ``fit()`` as follows:
+
+1. If all incoming items are 1-element lists, it sets a flag ``UNPACK_OUTPUT`` to always
+   unpack the element before passing them to the wrapped function during ``transform()``.
+2. If during ``fit()`` the wrapped function doesn't return lists,
+   it tries to turn that output into a list:
+    - If the output is always a non-string iterable, it will simply set a
+      flag ``CONVERT_ITERABLE`` to always convert the iterable output into a list during ``transform()``.
+    - Otherwise, it sets a flag ``WRAP_OUTPUT`` to always wrap the output in a
+      1-element list during ``transform()``.
+
+A similar logic is applied to the labels.
+If a custom labels function is given, the following procedure is followed during ``labels()``:
+
+1. If the incoming labels are a 1-element list, the single label is unpacked before
+   it is passed to the custom labels function.
+2. If the custom labels function returns something other than a list,
+   this class tries to convert it into a list:
+    - If the output is a non-string iterable, it is converted into a list.
+    - Otherwise, the output is wrapped in a 1-element list.
+
+If no custom labels function is given, the output labels are generated based on the
+output cardinality inferred during ``fit()`` and according to the following logic:
+
+- If the number of incoming labels is identical to the output cardinality,
+  the labels will be returned unchanged.
+- Otherwise, the number of incoming labels must be 1 and the output labels are generated by adding suffixes
+  ``_0``, ``_1``, etc. to the single input label.
+
+A special case are functions returning output of varying cardinality during ``fit()``.
+In this case, a single input label is returned.
+If multiple input labels are given, they are joined with ``_``.
 
 The following example turns a text column into two columns containing the ascii code of the first and last letter.
 
 ```python
 "Name": lambda x: (ord(x[0]), ord(x[-1]))
 ```
 
@@ -685,23 +767,58 @@
 As you can see, the number of columns is inferred directly from the return value of the conversion function.
 If the function returns a list, the resulting column names are indexed.
 
 You can also set the labels explicitly with a lambda function
 that takes the input column name as an argument and returns output column names:
 
 ```python
-"Name": Function(lambda x: (ord(x[0]), ord(x[-1])),
+"Name": Function(lambda x: [ord(x[0]), ord(x[-1])],
                  labels=lambda s: [f"ord(first letter of {s})", f"ord(last letter of {s})"]),
 ```
 
 | Name  | ⇒ | ord(first letter of Name) | ord(last letter of Name) |
 |-------|---|---------------------------|--------------------------|
 | Alice |   | 97                        | 101                      |
 | Bob   |   | 98                        | 98                       |
 
+However, remember that you can always simply use [`Label()`](#label) to rename the columns after the conversion,
+if you don't need the output column names to depend on the input column names.
+
+```python
+"Name": [lambda x: [ord(x[0]), ord(x[-1])],
+         Labels("ord(first letter)", "ord(last letter)")],
+```
+
+### StrictFunction
+
+```python
+StrictFunction(transform, labels=None)
+```
+
+Works mostly like [`Function()`](#function), but simpler:
+``transform`` and ``labels`` must both accept and return lists.
+Instead of something like this:
+
+```python
+"Name": str.lower,
+```
+
+you have to write this:
+
+```python
+"Name": StrictFunction(lambda x: [str.lower(x[0])])
+```
+
+That is, you will still receive 1-element lists as lists to the function,
+even if all input elements during `fit()` are 1-element lists.
+Also, you must now explicitly return a list,
+even if it is just a 1-element list, as otherwise an error will be raised.
+
+See [`Function()`](#function) for a convenient extension of this converter.
+
 ---
 
 ## Understanding Multi-Column Converters
 
 A converter returns two things:
 
 - `transform()`: the items of the transformed data
```

### Comparing `clevertable-2.1.1/pyproject.toml` & `clevertable-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clevertable"
-version = "2.1.1"
+version = "2.2.0"
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
-current_version = "2.1.1"
+current_version = "2.2.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `clevertable-2.1.1/src/clevertable/Binary.py` & `clevertable-2.2.0/src/clevertable/Binary.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.1/src/clevertable/ConversionProfile.py` & `clevertable-2.2.0/src/clevertable/ConversionProfile.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.1/src/clevertable/Converter.py` & `clevertable-2.2.0/src/clevertable/Converter.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.1/src/clevertable/DataFrameProfile.py` & `clevertable-2.2.0/src/clevertable/DataFrameProfile.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.1/src/clevertable/Enumerate.py` & `clevertable-2.2.0/src/clevertable/Enumerate.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.1/src/clevertable/Float.py` & `clevertable-2.2.0/src/clevertable/Float.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.1/src/clevertable/ForEach.py` & `clevertable-2.2.0/src/clevertable/ForEach.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.1/src/clevertable/Infer.py` & `clevertable-2.2.0/src/clevertable/Infer.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.1/src/clevertable/Label.py` & `clevertable-2.2.0/src/clevertable/Label.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.1/src/clevertable/List.py` & `clevertable-2.2.0/src/clevertable/List.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.1/src/clevertable/Map.py` & `clevertable-2.2.0/src/clevertable/Map.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.1/src/clevertable/OneHot.py` & `clevertable-2.2.0/src/clevertable/OneHot.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.1/src/clevertable/Parallel.py` & `clevertable-2.2.0/src/clevertable/Parallel.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.1/src/clevertable/Pipeline.py` & `clevertable-2.2.0/src/clevertable/Pipeline.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.1/src/clevertable/RecordProfile.py` & `clevertable-2.2.0/src/clevertable/RecordProfile.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.1/src/clevertable/Split.py` & `clevertable-2.2.0/src/clevertable/Split.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.1/src/clevertable/Strip.py` & `clevertable-2.2.0/src/clevertable/Strip.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.1/src/clevertable/Try.py` & `clevertable-2.2.0/src/clevertable/Try.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.1/src/clevertable/__init__.py` & `clevertable-2.2.0/src/clevertable/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-__version__ = "2.1.1"
+__version__ = "2.2.0"
 
 from .Binary import Binary
 from .Const import Const
 from .ConversionProfile import ConversionProfile
 from .Converter import Converter
 from .Enumerate import Enumerate
 from .Flatten import Flatten
 from .Float import Float
 from .ForEach import ForEach
+from .StrictFunction import StrictFunction
 from .Function import Function
 from .Id import Id
 from .Ignore import Ignore
 from .Infer import Infer
 from .Label import Label
 from .List import List, ListAndOr
 from .Map import Map
```

### Comparing `clevertable-2.1.1/src/clevertable/__main__.py` & `clevertable-2.2.0/src/clevertable/__main__.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.1/src/clevertable/_utils.py` & `clevertable-2.2.0/src/clevertable/_utils.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.1/src/clevertable.egg-info/PKG-INFO` & `clevertable-2.2.0/src/clevertable.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevertable
-Version: 2.1.1
+Version: 2.2.0
 Summary: Low effort conversion of tabular data into numerical values.
 Author: Tom Mohr
 License: MIT License
         
         Copyright (c) 2023 Tom Mohr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -335,43 +335,44 @@
 - `ConversionProfile`: A collection of converters.
 - `Converter`: Transforms columns of data into columns of data.
 
 ## Converters
 
 Here's a quick overview of all converters:
 
-| Converters                  | Description                                                                       | Shorthand  | Example Usage                                                   |
-|-----------------------------|-----------------------------------------------------------------------------------|------------|-----------------------------------------------------------------|
-| Basic:                      |                                                                                   |            |                                                                 |
-| [`Float()`](#float)         | Converts numbers into floats.                                                     |            |                                                                 |
-| [`Enumerate()`](#enumerate) |                                                                                   |            |                                                                 |
-| [`OneHot()`](#onehot)       |                                                                                   |            |                                                                 |
-| [`Binary()`](#binary)       | Converts a column of text into a column of integers.                              |            |                                                                 |
-| [`List()`](#list)           |                                                                                   |            |                                                                 |
-| [`ListAndOr()`](#listandor) |                                                                                   |            |                                                                 |
-| [`Map()`](#map)             |                                                                                   | dict       | {<br>&nbsp;&nbsp;"foo": 1,<br>&nbsp;&nbsp;"bar": -2,<br>}       |
-| [`Const()`](#const)         | Returns a constant value.                                                         | *any*      | 42<br>"foo"                                                     |
-| Text Processing:            |                                                                                   |            |                                                                 |
-| [`Strip()`](#strip)         |                                                                                   |            |                                                                 |
-| [`Split()`](#split)         |                                                                                   |            |                                                                 |
-| Combining Converters:       |                                                                                   |            |                                                                 |
-| [`Pipeline()`](#pipeline)   | Applies multiple converters in sequence.                                          | list       | [<br>&nbsp;&nbsp;Split(),<br>&nbsp;&nbsp;ForEach(Strip()),<br>] |
-| [`Try()`](#try)             | Try multiple converters and returns the first one that succeeds.                  | tuple      | (Float(), Binary())                                             |
-| [`ForEach()`](#foreach)     | Apply the same converter to all items.                                            |            |                                                                 |
-| [`Parallel()`](#parallel)   | Apply different converters to the respective items.                               |            |                                                                 |
-| Special:                    |                                                                                   |            |                                                                 |
-| [`Id()`](#id)               |                                                                                   |            |                                                                 |
-| [`Ignore()`](#ignore)       | Drops the column.                                                                 | None       | None                                                            |
-| [`Infer()`](#infer)         |                                                                                   |            |                                                                 |
-| [`Label()`](#label)         |                                                                                   |            |                                                                 |
-| Dimensionality:             |                                                                                   |            |                                                                 |
-| [`Flatten()`](#flatten)     | Flattens a list of lists into a single list. This is often needed after ForEach() |            |                                                                 |
-| [`Transpose()`](#transpose) |                                                                                   |            |                                                                 |
-| Arbitrary Functions:        |                                                                                   |            |                                                                 |
-| [`Function()`](#function)   | Applies a user-defined function to the data.                                      | *callable* | lambda x: x**2                                                  |
+| Converters                            | Description                                                                         | Shorthand | Example Usage                                                   |
+|---------------------------------------|-------------------------------------------------------------------------------------|-----------|-----------------------------------------------------------------|
+| Basic:                                |                                                                                     |           |                                                                 |
+| [`Float()`](#float)                   | Convert numbers into floats.                                                        |           |                                                                 |
+| [`Enumerate()`](#enumerate)           |                                                                                     |           |                                                                 |
+| [`OneHot()`](#onehot)                 |                                                                                     |           |                                                                 |
+| [`Binary()`](#binary)                 | Convert a column of text into a column of integers.                                 |           |                                                                 |
+| [`List()`](#list)                     |                                                                                     |           |                                                                 |
+| [`ListAndOr()`](#listandor)           |                                                                                     |           |                                                                 |
+| [`Map()`](#map)                       |                                                                                     | dict      | {<br>&nbsp;&nbsp;"foo": 1,<br>&nbsp;&nbsp;"bar": -2,<br>}       |
+| [`Const()`](#const)                   | Return a constant value.                                                            | *any*     | 42<br>"foo"                                                     |
+| Text Processing:                      |                                                                                     |           |                                                                 |
+| [`Strip()`](#strip)                   |                                                                                     |           |                                                                 |
+| [`Split()`](#split)                   |                                                                                     |           |                                                                 |
+| Combining Converters:                 |                                                                                     |           |                                                                 |
+| [`Pipeline()`](#pipeline)             | Apply multiple converters in sequence.                                              | list      | [<br>&nbsp;&nbsp;Split(),<br>&nbsp;&nbsp;ForEach(Strip()),<br>] |
+| [`Try()`](#try)                       | Try multiple converters and return the first one that succeeds.                     | tuple     | (Float(), Binary())                                             |
+| [`ForEach()`](#foreach)               | Apply the same converter to all items.                                              |           |                                                                 |
+| [`Parallel()`](#parallel)             | Apply different converters to the respective items.                                 |           |                                                                 |
+| Special:                              |                                                                                     |           |                                                                 |
+| [`Id()`](#id)                         |                                                                                     |           |                                                                 |
+| [`Ignore()`](#ignore)                 | Drop the column.                                                                    | None      | None                                                            |
+| [`Infer()`](#infer)                   |                                                                                     |           |                                                                 |
+| [`Label()`](#label)                   |                                                                                     |           |                                                                 |
+| Dimensionality:                       |                                                                                     |           |                                                                 |
+| [`Flatten()`](#flatten)               | Flatten a list of lists into a single list. This is often needed after `ForEach()`. |           |                                                                 |
+| [`Transpose()`](#transpose)           |                                                                                     |           |                                                                 |
+| Arbitrary Functions:                  |                                                                                     |           |                                                                 |
+| [`Function()`](#function)             | Apply a user-defined function to the data.                                          | callable  | lambda x: x**2                                                  |
+| [`StrictFunction()`](#strictfunction) | Apply a user-defined function to the data. Less flexible than `Function()`.         |           |                                                                 |
 
 ---
 
 ### Float
 
 Converts a column of numbers into a column of numbers.
 If invalid values are encountered (`NaN`, `inf`, `None`, etc.),
@@ -699,15 +700,59 @@
 ```
 
 `Transpose()` allows us to apply `max` to each column of the one-hot encodings
 across all list elements.
 
 ### Function
 
-This can be used to specify a custom conversion function.
+```python
+Function(transform, labels=None)
+```
+
+Shorthand: Instead of `Function(transform, None)`, just write `transform`, where `transform` is some callable.
+
+Creates a custom converter from a custom ``transform()`` function
+(and optionally, a custom ``labels()`` function).
+This is a handy way to create a converter that doesn't need ``fit()``.
+
+Unlike ``StrictFunction()``, this class can handle functions that don't accept or return lists,
+which often allows for more concise code.
+
+This is achieved during ``fit()`` as follows:
+
+1. If all incoming items are 1-element lists, it sets a flag ``UNPACK_OUTPUT`` to always
+   unpack the element before passing them to the wrapped function during ``transform()``.
+2. If during ``fit()`` the wrapped function doesn't return lists,
+   it tries to turn that output into a list:
+    - If the output is always a non-string iterable, it will simply set a
+      flag ``CONVERT_ITERABLE`` to always convert the iterable output into a list during ``transform()``.
+    - Otherwise, it sets a flag ``WRAP_OUTPUT`` to always wrap the output in a
+      1-element list during ``transform()``.
+
+A similar logic is applied to the labels.
+If a custom labels function is given, the following procedure is followed during ``labels()``:
+
+1. If the incoming labels are a 1-element list, the single label is unpacked before
+   it is passed to the custom labels function.
+2. If the custom labels function returns something other than a list,
+   this class tries to convert it into a list:
+    - If the output is a non-string iterable, it is converted into a list.
+    - Otherwise, the output is wrapped in a 1-element list.
+
+If no custom labels function is given, the output labels are generated based on the
+output cardinality inferred during ``fit()`` and according to the following logic:
+
+- If the number of incoming labels is identical to the output cardinality,
+  the labels will be returned unchanged.
+- Otherwise, the number of incoming labels must be 1 and the output labels are generated by adding suffixes
+  ``_0``, ``_1``, etc. to the single input label.
+
+A special case are functions returning output of varying cardinality during ``fit()``.
+In this case, a single input label is returned.
+If multiple input labels are given, they are joined with ``_``.
 
 The following example turns a text column into two columns containing the ascii code of the first and last letter.
 
 ```python
 "Name": lambda x: (ord(x[0]), ord(x[-1]))
 ```
 
@@ -722,23 +767,58 @@
 As you can see, the number of columns is inferred directly from the return value of the conversion function.
 If the function returns a list, the resulting column names are indexed.
 
 You can also set the labels explicitly with a lambda function
 that takes the input column name as an argument and returns output column names:
 
 ```python
-"Name": Function(lambda x: (ord(x[0]), ord(x[-1])),
+"Name": Function(lambda x: [ord(x[0]), ord(x[-1])],
                  labels=lambda s: [f"ord(first letter of {s})", f"ord(last letter of {s})"]),
 ```
 
 | Name  | ⇒ | ord(first letter of Name) | ord(last letter of Name) |
 |-------|---|---------------------------|--------------------------|
 | Alice |   | 97                        | 101                      |
 | Bob   |   | 98                        | 98                       |
 
+However, remember that you can always simply use [`Label()`](#label) to rename the columns after the conversion,
+if you don't need the output column names to depend on the input column names.
+
+```python
+"Name": [lambda x: [ord(x[0]), ord(x[-1])],
+         Labels("ord(first letter)", "ord(last letter)")],
+```
+
+### StrictFunction
+
+```python
+StrictFunction(transform, labels=None)
+```
+
+Works mostly like [`Function()`](#function), but simpler:
+``transform`` and ``labels`` must both accept and return lists.
+Instead of something like this:
+
+```python
+"Name": str.lower,
+```
+
+you have to write this:
+
+```python
+"Name": StrictFunction(lambda x: [str.lower(x[0])])
+```
+
+That is, you will still receive 1-element lists as lists to the function,
+even if all input elements during `fit()` are 1-element lists.
+Also, you must now explicitly return a list,
+even if it is just a 1-element list, as otherwise an error will be raised.
+
+See [`Function()`](#function) for a convenient extension of this converter.
+
 ---
 
 ## Understanding Multi-Column Converters
 
 A converter returns two things:
 
 - `transform()`: the items of the transformed data
```

### Comparing `clevertable-2.1.1/src/clevertable.egg-info/SOURCES.txt` & `clevertable-2.2.0/src/clevertable.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 src/clevertable/List.py
 src/clevertable/Map.py
 src/clevertable/OneHot.py
 src/clevertable/Parallel.py
 src/clevertable/Pipeline.py
 src/clevertable/RecordProfile.py
 src/clevertable/Split.py
+src/clevertable/StrictFunction.py
 src/clevertable/Strip.py
 src/clevertable/Transpose.py
 src/clevertable/Try.py
 src/clevertable/__init__.py
 src/clevertable/__main__.py
 src/clevertable/_utils.py
 src/clevertable.egg-info/PKG-INFO
```

