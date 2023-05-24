# Comparing `tmp/salure_helpers_profit-1.3.0.tar.gz` & `tmp/salure_helpers_profit-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_profit-1.3.0.tar", last modified: Fri May 12 07:18:59 2023, max compression
+gzip compressed data, was "dist/salure_helpers_profit-1.3.1.tar", last modified: Wed May 24 12:07:11 2023, max compression
```

## Comparing `salure_helpers_profit-1.3.0.tar` & `salure_helpers_profit-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:18:59.000000 salure_helpers_profit-1.3.0/
--rw-r--r--   0 root         (0) root         (0)      262 2023-05-12 07:18:59.000000 salure_helpers_profit-1.3.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:18:59.000000 salure_helpers_profit-1.3.0/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:18:59.000000 salure_helpers_profit-1.3.0/salure_helpers/profit/
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-05-12 07:18:44.000000 salure_helpers_profit-1.3.0/salure_helpers/profit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3855 2023-05-12 07:18:44.000000 salure_helpers_profit-1.3.0/salure_helpers/profit/profit_data_cleaner.py
--rw-rw-rw-   0 root         (0) root         (0)    14489 2023-05-12 07:18:44.000000 salure_helpers_profit-1.3.0/salure_helpers/profit/profit_get.py
--rw-rw-rw-   0 root         (0) root         (0)    17549 2023-05-12 07:18:44.000000 salure_helpers_profit-1.3.0/salure_helpers/profit/profit_get_async.py
--rw-rw-rw-   0 root         (0) root         (0)   130048 2023-05-12 07:18:44.000000 salure_helpers_profit-1.3.0/salure_helpers/profit/profit_update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:18:59.000000 salure_helpers_profit-1.3.0/salure_helpers_profit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      262 2023-05-12 07:18:58.000000 salure_helpers_profit-1.3.0/salure_helpers_profit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2023-05-12 07:18:58.000000 salure_helpers_profit-1.3.0/salure_helpers_profit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 07:18:58.000000 salure_helpers_profit-1.3.0/salure_helpers_profit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 07:18:58.000000 salure_helpers_profit-1.3.0/salure_helpers_profit.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      130 2023-05-12 07:18:58.000000 salure_helpers_profit-1.3.0/salure_helpers_profit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-12 07:18:58.000000 salure_helpers_profit-1.3.0/salure_helpers_profit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 07:18:59.000000 salure_helpers_profit-1.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-05-12 07:18:44.000000 salure_helpers_profit-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:07:11.000000 salure_helpers_profit-1.3.1/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-05-24 12:07:11.000000 salure_helpers_profit-1.3.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:07:11.000000 salure_helpers_profit-1.3.1/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:07:11.000000 salure_helpers_profit-1.3.1/salure_helpers/profit/
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-05-24 12:06:56.000000 salure_helpers_profit-1.3.1/salure_helpers/profit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3855 2023-05-24 12:06:56.000000 salure_helpers_profit-1.3.1/salure_helpers/profit/profit_data_cleaner.py
+-rw-rw-rw-   0 root         (0) root         (0)    14489 2023-05-24 12:06:56.000000 salure_helpers_profit-1.3.1/salure_helpers/profit/profit_get.py
+-rw-rw-rw-   0 root         (0) root         (0)    17456 2023-05-24 12:06:56.000000 salure_helpers_profit-1.3.1/salure_helpers/profit/profit_get_async.py
+-rw-rw-rw-   0 root         (0) root         (0)   130048 2023-05-24 12:06:56.000000 salure_helpers_profit-1.3.1/salure_helpers/profit/profit_update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:07:11.000000 salure_helpers_profit-1.3.1/salure_helpers_profit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-05-24 12:07:11.000000 salure_helpers_profit-1.3.1/salure_helpers_profit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2023-05-24 12:07:11.000000 salure_helpers_profit-1.3.1/salure_helpers_profit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 12:07:11.000000 salure_helpers_profit-1.3.1/salure_helpers_profit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 12:07:11.000000 salure_helpers_profit-1.3.1/salure_helpers_profit.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      130 2023-05-24 12:07:11.000000 salure_helpers_profit-1.3.1/salure_helpers_profit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-24 12:07:11.000000 salure_helpers_profit-1.3.1/salure_helpers_profit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 12:07:11.000000 salure_helpers_profit-1.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-05-24 12:06:56.000000 salure_helpers_profit-1.3.1/setup.py
```

### Comparing `salure_helpers_profit-1.3.0/salure_helpers/profit/profit_data_cleaner.py` & `salure_helpers_profit-1.3.1/salure_helpers/profit/profit_data_cleaner.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-1.3.0/salure_helpers/profit/profit_get.py` & `salure_helpers_profit-1.3.1/salure_helpers/profit/profit_get.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-1.3.0/salure_helpers/profit/profit_get_async.py` & `salure_helpers_profit-1.3.1/salure_helpers/profit/profit_get_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             self.profit_async.get_data(connectors=connectors,
                                        parameters=parameters,
                                        batch_size=batch_size,
                                        take=take))
 
         return total_response
 
-    def get_complex_filtered_data(self, connector: Union[str, List], fields: list, values: list, operators: list, orderbyfields: str = None, batch_size: int = 8, take: int = 40000) -> json:
+    def get_complex_filtered_data(self, connector: str, fields: list, values: list, operators: list, orderbyfields: str = None, batch_size: int = 8, take: int = 40000) -> json:
         """
         This method is meant for complex combined filters like (a and b) or (a and c)
 
         Possible filter operators are:
         1: is gelijk aan
         2: is groter of gelijk aan
         3: is kleiner of gelijk aan
@@ -131,24 +131,23 @@
             values_values = values[filter_no].split(',')
             for number in range(0, len(fields_values)):
                 filter["Field"].append({"@FieldId": fields_values[number],
                                         "@OperatorType": operators_values[number],
                                         "#text": values_values[number]})
             parameters['Filters']['Filter'].append(filter)
 
-        # Dit stukje hieronder heeft JJ een paar uur van zn leven gekost. Do not touch
-        # querystring = parse.quote(json.dumps(parameters, separators=(',', ':')))
+        # eliminate whitespaces and escape special characters
         querystring = json.dumps(parameters, separators=(',', ':'))
         if orderbyfields is not None:
-            querystring = {"filterjson": querystring, "orderbyfieldids": f"{orderbyfields}"}
+            querystring = {connector: {"filterjson": querystring, "orderbyfieldids": f"{orderbyfields}"}}
         else:
-            querystring = {"filterjson": querystring}
+            querystring = {connector: {"filterjson": querystring}}
 
         total_response_raw = asyncio.run(
-            self.profit_async.get_data(connectors=connector,
+            self.profit_async.get_data(connectors=[connector],
                                        parameters=querystring,
                                        batch_size=batch_size,
                                        take=take))
         total_response = [item for sublist in total_response_raw for item in sublist]
 
         return total_response
```

### Comparing `salure_helpers_profit-1.3.0/salure_helpers/profit/profit_update.py` & `salure_helpers_profit-1.3.1/salure_helpers/profit/profit_update.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-1.3.0/setup.py` & `salure_helpers_profit-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='salure_helpers_profit',
-    version='1.3.0',
+    version='1.3.1',
     description='Profit wrapper from Salure',
     long_description='Profit wrapper from Salure',
     author='D&A Salure',
     author_email='support@salureconnnect.com',
     packages=["salure_helpers.profit"],
     license='Salure License',
     install_requires=[
```

