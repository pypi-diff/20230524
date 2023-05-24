# Comparing `tmp/easyfrenchtax-0.0.1.tar.gz` & `tmp/easyfrenchtax-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyfrenchtax-0.0.1.tar", last modified: Fri May 20 20:12:43 2022, max compression
+gzip compressed data, was "easyfrenchtax-0.0.2.tar", last modified: Sun Nov 27 06:39:17 2022, max compression
```

## Comparing `easyfrenchtax-0.0.1.tar` & `easyfrenchtax-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2022-05-20 20:12:43.101621 easyfrenchtax-0.0.1/
--rw-r--r--   0 hadrien    (501) staff       (20)     1069 2021-12-17 08:32:37.000000 easyfrenchtax-0.0.1/LICENSE
--rw-r--r--   0 hadrien    (501) staff       (20)     2527 2022-05-20 20:12:43.101677 easyfrenchtax-0.0.1/PKG-INFO
--rw-r--r--   0 hadrien    (501) staff       (20)     1794 2022-04-29 07:59:34.000000 easyfrenchtax-0.0.1/README.md
--rw-r--r--   0 hadrien    (501) staff       (20)      103 2021-12-17 08:19:56.000000 easyfrenchtax-0.0.1/pyproject.toml
--rw-r--r--   0 hadrien    (501) staff       (20)      853 2022-05-20 20:12:43.101929 easyfrenchtax-0.0.1/setup.cfg
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2022-05-20 20:12:43.099351 easyfrenchtax-0.0.1/src/
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2022-05-20 20:12:43.100823 easyfrenchtax-0.0.1/src/easyfrenchtax/
--rw-r--r--   0 hadrien    (501) staff       (20)       90 2021-10-10 19:27:02.000000 easyfrenchtax-0.0.1/src/easyfrenchtax/__init__.py
--rw-r--r--   0 hadrien    (501) staff       (20)    22090 2022-04-26 09:27:15.000000 easyfrenchtax-0.0.1/src/easyfrenchtax/stock_helper.py
--rw-r--r--   0 hadrien    (501) staff       (20)    15265 2022-04-29 08:41:16.000000 easyfrenchtax-0.0.1/src/easyfrenchtax/tax_simulator.py
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2022-05-20 20:12:43.101534 easyfrenchtax-0.0.1/src/easyfrenchtax.egg-info/
--rw-r--r--   0 hadrien    (501) staff       (20)     2527 2022-05-20 20:12:42.000000 easyfrenchtax-0.0.1/src/easyfrenchtax.egg-info/PKG-INFO
--rw-r--r--   0 hadrien    (501) staff       (20)      345 2022-05-20 20:12:43.000000 easyfrenchtax-0.0.1/src/easyfrenchtax.egg-info/SOURCES.txt
--rw-r--r--   0 hadrien    (501) staff       (20)        1 2022-05-20 20:12:42.000000 easyfrenchtax-0.0.1/src/easyfrenchtax.egg-info/dependency_links.txt
--rw-r--r--   0 hadrien    (501) staff       (20)       18 2022-05-20 20:12:43.000000 easyfrenchtax-0.0.1/src/easyfrenchtax.egg-info/requires.txt
--rw-r--r--   0 hadrien    (501) staff       (20)       14 2022-05-20 20:12:43.000000 easyfrenchtax-0.0.1/src/easyfrenchtax.egg-info/top_level.txt
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2022-11-27 06:39:17.305689 easyfrenchtax-0.0.2/
+-rw-r--r--   0 hadrien    (501) staff       (20)     1069 2021-12-17 08:32:37.000000 easyfrenchtax-0.0.2/LICENSE
+-rw-r--r--   0 hadrien    (501) staff       (20)     2557 2022-11-27 06:39:17.305745 easyfrenchtax-0.0.2/PKG-INFO
+-rw-r--r--   0 hadrien    (501) staff       (20)     1824 2022-06-07 08:55:19.000000 easyfrenchtax-0.0.2/README.md
+-rw-r--r--   0 hadrien    (501) staff       (20)      103 2021-12-17 08:19:56.000000 easyfrenchtax-0.0.2/pyproject.toml
+-rw-r--r--   0 hadrien    (501) staff       (20)      853 2022-11-27 06:39:17.305992 easyfrenchtax-0.0.2/setup.cfg
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2022-11-27 06:39:17.303156 easyfrenchtax-0.0.2/src/
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2022-11-27 06:39:17.304712 easyfrenchtax-0.0.2/src/easyfrenchtax/
+-rw-r--r--   0 hadrien    (501) staff       (20)      100 2022-06-09 10:23:03.000000 easyfrenchtax-0.0.2/src/easyfrenchtax/__init__.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    22090 2022-04-26 09:27:15.000000 easyfrenchtax-0.0.2/src/easyfrenchtax/stock_helper.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    26441 2022-09-08 20:38:27.000000 easyfrenchtax-0.0.2/src/easyfrenchtax/tax_simulator.py
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2022-11-27 06:39:17.305593 easyfrenchtax-0.0.2/src/easyfrenchtax.egg-info/
+-rw-r--r--   0 hadrien    (501) staff       (20)     2557 2022-11-27 06:39:17.000000 easyfrenchtax-0.0.2/src/easyfrenchtax.egg-info/PKG-INFO
+-rw-r--r--   0 hadrien    (501) staff       (20)      345 2022-11-27 06:39:17.000000 easyfrenchtax-0.0.2/src/easyfrenchtax.egg-info/SOURCES.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)        1 2022-11-27 06:39:17.000000 easyfrenchtax-0.0.2/src/easyfrenchtax.egg-info/dependency_links.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)       18 2022-11-27 06:39:17.000000 easyfrenchtax-0.0.2/src/easyfrenchtax.egg-info/requires.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)       14 2022-11-27 06:39:17.000000 easyfrenchtax-0.0.2/src/easyfrenchtax.egg-info/top_level.txt
```

### Comparing `easyfrenchtax-0.0.1/LICENSE` & `easyfrenchtax-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.1/PKG-INFO` & `easyfrenchtax-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyfrenchtax
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simulator of French taxes
 Home-page: https://github.com/had/easyfrenchtax
 Author: Hadrien Hamel
 Author-email: hadrien.hamel@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/had/easyfrenchtax/issues
 Classifier: Programming Language :: Python :: 3
@@ -20,14 +20,15 @@
 
 # easyfrenchtax
 This project helps me understanding and projecting French taxes, especially wrt. stock, stock options, RSUs and other systems. It doesn't replace a tax advisor, I am not a lawyer, you should not rely blindly on this software for filling your tax return.
 
 # Tax simulator
 The following are supported:
 - Progressive income tax
+- Rental income (unfurnished)
 - Family quotient (incl. capping, but excl. shared custody situations)
 - Some deductions/reductions (PER, child care, home services, charity donations)
 - Capping of fiscal advantages ("plafonnement des niches fiscales" in French)
 - Exercising stock options, RSU acquisition gain, capital gain (but not capital loss - yet)
 - Fixed interest income, incl. when tax has been partially withheld by a bank
 - Social taxes
```

### Comparing `easyfrenchtax-0.0.1/README.md` & `easyfrenchtax-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # easyfrenchtax
 This project helps me understanding and projecting French taxes, especially wrt. stock, stock options, RSUs and other systems. It doesn't replace a tax advisor, I am not a lawyer, you should not rely blindly on this software for filling your tax return.
 
 # Tax simulator
 The following are supported:
 - Progressive income tax
+- Rental income (unfurnished)
 - Family quotient (incl. capping, but excl. shared custody situations)
 - Some deductions/reductions (PER, child care, home services, charity donations)
 - Capping of fiscal advantages ("plafonnement des niches fiscales" in French)
 - Exercising stock options, RSU acquisition gain, capital gain (but not capital loss - yet)
 - Fixed interest income, incl. when tax has been partially withheld by a bank
 - Social taxes
```

### Comparing `easyfrenchtax-0.0.1/setup.cfg` & `easyfrenchtax-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = easyfrenchtax
-version = 0.0.1
+version = 0.0.2
 author = Hadrien Hamel
 author_email = hadrien.hamel@gmail.com
 license = MIT
 description = A simulator of French taxes
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/had/easyfrenchtax
```

### Comparing `easyfrenchtax-0.0.1/src/easyfrenchtax/stock_helper.py` & `easyfrenchtax-0.0.2/src/easyfrenchtax/stock_helper.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.1/src/easyfrenchtax.egg-info/PKG-INFO` & `easyfrenchtax-0.0.2/src/easyfrenchtax.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyfrenchtax
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simulator of French taxes
 Home-page: https://github.com/had/easyfrenchtax
 Author: Hadrien Hamel
 Author-email: hadrien.hamel@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/had/easyfrenchtax/issues
 Classifier: Programming Language :: Python :: 3
@@ -20,14 +20,15 @@
 
 # easyfrenchtax
 This project helps me understanding and projecting French taxes, especially wrt. stock, stock options, RSUs and other systems. It doesn't replace a tax advisor, I am not a lawyer, you should not rely blindly on this software for filling your tax return.
 
 # Tax simulator
 The following are supported:
 - Progressive income tax
+- Rental income (unfurnished)
 - Family quotient (incl. capping, but excl. shared custody situations)
 - Some deductions/reductions (PER, child care, home services, charity donations)
 - Capping of fiscal advantages ("plafonnement des niches fiscales" in French)
 - Exercising stock options, RSU acquisition gain, capital gain (but not capital loss - yet)
 - Fixed interest income, incl. when tax has been partially withheld by a bank
 - Social taxes
```

