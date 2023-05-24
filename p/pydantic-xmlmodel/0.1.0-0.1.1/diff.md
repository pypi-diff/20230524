# Comparing `tmp/pydantic_xmlmodel-0.1.0.tar.gz` & `tmp/pydantic_xmlmodel-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_xmlmodel-0.1.0.tar", max compression
+gzip compressed data, was "pydantic_xmlmodel-0.1.1.tar", max compression
```

## Comparing `pydantic_xmlmodel-0.1.0.tar` & `pydantic_xmlmodel-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-05-17 13:32:22.273043 pydantic_xmlmodel-0.1.0/LICENSE
--rw-r--r--   0        0        0     2328 2023-05-17 14:52:06.359687 pydantic_xmlmodel-0.1.0/README.md
--rw-r--r--   0        0        0       55 2023-05-17 13:44:08.514440 pydantic_xmlmodel-0.1.0/pydantic_xmlmodel/__init__.py
--rw-r--r--   0        0        0     9357 2023-05-17 14:11:17.819658 pydantic_xmlmodel-0.1.0/pydantic_xmlmodel/xmlmodel.py
--rw-r--r--   0        0        0      613 2023-05-17 14:52:44.039172 pydantic_xmlmodel-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3072 1970-01-01 00:00:00.000000 pydantic_xmlmodel-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-17 13:32:22.273043 pydantic_xmlmodel-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2327 2023-05-17 14:55:31.763327 pydantic_xmlmodel-0.1.1/README.md
+-rw-r--r--   0        0        0       55 2023-05-17 13:44:08.514440 pydantic_xmlmodel-0.1.1/pydantic_xmlmodel/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:52:39.775359 pydantic_xmlmodel-0.1.1/pydantic_xmlmodel/py.typed
+-rw-r--r--   0        0        0     9357 2023-05-20 18:36:21.749673 pydantic_xmlmodel-0.1.1/pydantic_xmlmodel/xmlmodel.py
+-rw-r--r--   0        0        0      613 2023-05-24 08:52:59.623623 pydantic_xmlmodel-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3071 1970-01-01 00:00:00.000000 pydantic_xmlmodel-0.1.1/PKG-INFO
```

### Comparing `pydantic_xmlmodel-0.1.0/LICENSE` & `pydantic_xmlmodel-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_xmlmodel-0.1.0/README.md` & `pydantic_xmlmodel-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 ```python
 from pydantic_xmlmodel import XMLModel
 ```
 
 Here is the class diagram of the library:
 
-![Graph](https://mermaid.ink/img/pako:eNp9UstqwzAQ_BWhUxqcHzAh0NetpodeCnERG2ntiugRpHXTkObfu3ZCGpNQgSxpZnYGr7SXOhqUpdQOcn6y0CbwdRA8BkS8Vy8VK1yFBGJ_ZPoxn3tGBs1i8QcLpQJulZpolwsRwGMhVpCRD0CUeJlO11tIbb4rxX3YHSsPtxLHaQ9sMsCXaTOlvr1TfYxSpXjdkI0B3DJT-ritarqge9FI_gjOwcrhcigsRP-9rtcxEAb6J0ioFumcNeE_ZP6CNlYTReYnNhi2ujCygTjYBu06g4PFF6bMXClWMborqyZF3xvxHCgWnDs06uno_uY_s9kZkYX0mDxYw9c_9LqW9Ikea1ny1kAS61rW4cBC6Ci-7YKWJaUOC9ltDBCenssYfDaWYpJlAy4ziMOxOj2yGBrbysMv1qTMwg?type=png)]
+![Graph](https://mermaid.ink/img/pako:eNp9UstqwzAQ_BWhUxqcHzAh0NetpodeCnERG2ntiugRpHXTkObfu3ZCGpNQgSxpZnYGr7SXOhqUpdQOcn6y0CbwdRA8BkS8Vy8VK1yFBGJ_ZPoxn3tGBs1i8QcLpQJulZpolwsRwGMhVpCRD0CUeJlO11tIbb4rxX3YHSsPtxLHaQ9sMsCXaTOlvr1TfYxSpXjdkI0B3DJT-ritarqge9FI_gjOwcrhcigsRP-9rtcxEAb6J0ioFumcNeE_ZP6CNlYTReYnNhi2ujCygTjYBu06g4PFF6bMXClWMborqyZF3xvxHCgWnDs06uno_uY_s9kZkYX0mDxYw9c_9LqW9Ikea1ny1kAS61rW4cBC6Ci-7YKWJaUOC9ltDBCenssYfDaWYpJlAy4ziMOxOj2yGBrbysMv1qTMwg?type=png)
 
 ## Examples
 
 ### Defining a Model
 
 You can define a model by subclassing `XMLModel` and defining attributes with type annotations:
```

### Comparing `pydantic_xmlmodel-0.1.0/pydantic_xmlmodel/xmlmodel.py` & `pydantic_xmlmodel-0.1.1/pydantic_xmlmodel/xmlmodel.py`

 * *Files identical despite different names*

### Comparing `pydantic_xmlmodel-0.1.0/pyproject.toml` & `pydantic_xmlmodel-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-xmlmodel"
-version = "0.1.0"
+version = "0.1.1"
 description = "PydanticXML is a Python library that provides a way to convert Pydantic models to XML and vice versa."
 authors = ["cofob <cofob@riseup.net>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/cofob/pydanticxml"
 homepage = "https://github.com/cofob/pydanticxml"
```

### Comparing `pydantic_xmlmodel-0.1.0/PKG-INFO` & `pydantic_xmlmodel-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-xmlmodel
-Version: 0.1.0
+Version: 0.1.1
 Summary: PydanticXML is a Python library that provides a way to convert Pydantic models to XML and vice versa.
 Home-page: https://github.com/cofob/pydanticxml
 License: MIT
 Author: cofob
 Author-email: cofob@riseup.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -35,15 +35,15 @@
 
 ```python
 from pydantic_xmlmodel import XMLModel
 ```
 
 Here is the class diagram of the library:
 
-![Graph](https://mermaid.ink/img/pako:eNp9UstqwzAQ_BWhUxqcHzAh0NetpodeCnERG2ntiugRpHXTkObfu3ZCGpNQgSxpZnYGr7SXOhqUpdQOcn6y0CbwdRA8BkS8Vy8VK1yFBGJ_ZPoxn3tGBs1i8QcLpQJulZpolwsRwGMhVpCRD0CUeJlO11tIbb4rxX3YHSsPtxLHaQ9sMsCXaTOlvr1TfYxSpXjdkI0B3DJT-ritarqge9FI_gjOwcrhcigsRP-9rtcxEAb6J0ioFumcNeE_ZP6CNlYTReYnNhi2ujCygTjYBu06g4PFF6bMXClWMborqyZF3xvxHCgWnDs06uno_uY_s9kZkYX0mDxYw9c_9LqW9Ikea1ny1kAS61rW4cBC6Ci-7YKWJaUOC9ltDBCenssYfDaWYpJlAy4ziMOxOj2yGBrbysMv1qTMwg?type=png)]
+![Graph](https://mermaid.ink/img/pako:eNp9UstqwzAQ_BWhUxqcHzAh0NetpodeCnERG2ntiugRpHXTkObfu3ZCGpNQgSxpZnYGr7SXOhqUpdQOcn6y0CbwdRA8BkS8Vy8VK1yFBGJ_ZPoxn3tGBs1i8QcLpQJulZpolwsRwGMhVpCRD0CUeJlO11tIbb4rxX3YHSsPtxLHaQ9sMsCXaTOlvr1TfYxSpXjdkI0B3DJT-ritarqge9FI_gjOwcrhcigsRP-9rtcxEAb6J0ioFumcNeE_ZP6CNlYTReYnNhi2ujCygTjYBu06g4PFF6bMXClWMborqyZF3xvxHCgWnDs06uno_uY_s9kZkYX0mDxYw9c_9LqW9Ikea1ny1kAS61rW4cBC6Ci-7YKWJaUOC9ltDBCenssYfDaWYpJlAy4ziMOxOj2yGBrbysMv1qTMwg?type=png)
 
 ## Examples
 
 ### Defining a Model
 
 You can define a model by subclassing `XMLModel` and defining attributes with type annotations:
```

