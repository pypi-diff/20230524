# Comparing `tmp/copul-0.0.3.tar.gz` & `tmp/copul-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copul-0.0.3.tar", last modified: Mon May 22 16:19:16 2023, max compression
+gzip compressed data, was "copul-0.0.4.tar", last modified: Wed May 24 13:24:38 2023, max compression
```

## Comparing `copul-0.0.3.tar` & `copul-0.0.4.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 16:19:16.482399 copul-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-05-21 18:41:35.000000 copul-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       30 2023-05-17 14:16:18.000000 copul-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1986 2023-05-22 16:19:16.482399 copul-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1449 2023-05-22 16:18:24.000000 copul-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 16:19:16.460007 copul-0.0.3/copul/
--rw-rw-rw-   0        0        0      357 2023-05-21 18:51:19.000000 copul-0.0.3/copul/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:19:16.462011 copul-0.0.3/copul/docs/
--rw-rw-rw-   0        0        0        0 2023-05-17 14:16:18.000000 copul-0.0.3/copul/docs/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-05-22 16:19:16.463515 copul-0.0.3/copul/families/
--rw-rw-rw-   0        0        0      293 2023-05-22 15:10:27.000000 copul-0.0.3/copul/families/__init__.py
--rw-rw-rw-   0        0        0     2380 2023-05-22 16:16:20.000000 copul-0.0.3/copul/families/abstract_copula.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:19:16.475027 copul-0.0.3/copul/families/archimedean/
--rw-rw-rw-   0        0        0     5839 2023-05-21 18:51:44.000000 copul-0.0.3/copul/families/archimedean/__init__.py
--rw-rw-rw-   0        0        0     5386 2023-05-22 15:34:05.000000 copul-0.0.3/copul/families/archimedean/archimedean_copula.py
--rw-rw-rw-   0        0        0     5160 2023-05-21 18:41:35.000000 copul-0.0.3/copul/families/archimedean/derivatives_overview_constructor.py
--rw-rw-rw-   0        0        0      828 2023-05-21 18:52:04.000000 copul-0.0.3/copul/families/archimedean/nelsen1.py
--rw-rw-rw-   0        0        0      299 2023-05-21 18:54:30.000000 copul-0.0.3/copul/families/archimedean/nelsen10.py
--rw-rw-rw-   0        0        0      294 2023-05-21 18:54:30.000000 copul-0.0.3/copul/families/archimedean/nelsen11.py
--rw-rw-rw-   0        0        0      503 2023-05-22 15:14:02.000000 copul-0.0.3/copul/families/archimedean/nelsen12.py
--rw-rw-rw-   0        0        0      322 2023-05-21 18:54:30.000000 copul-0.0.3/copul/families/archimedean/nelsen13.py
--rw-rw-rw-   0        0        0      531 2023-05-22 15:34:05.000000 copul-0.0.3/copul/families/archimedean/nelsen14.py
--rw-rw-rw-   0        0        0      357 2023-05-21 18:54:30.000000 copul-0.0.3/copul/families/archimedean/nelsen15.py
--rw-rw-rw-   0        0        0      892 2023-05-22 15:36:21.000000 copul-0.0.3/copul/families/archimedean/nelsen16.py
--rw-rw-rw-   0        0        0     2156 2023-05-22 15:43:32.000000 copul-0.0.3/copul/families/archimedean/nelsen17.py
--rw-rw-rw-   0        0        0      318 2023-05-21 18:54:30.000000 copul-0.0.3/copul/families/archimedean/nelsen18.py
--rw-rw-rw-   0        0        0      333 2023-05-21 18:54:30.000000 copul-0.0.3/copul/families/archimedean/nelsen19.py
--rw-rw-rw-   0        0        0      506 2023-05-22 14:44:54.000000 copul-0.0.3/copul/families/archimedean/nelsen2.py
--rw-rw-rw-   0        0        0      330 2023-05-21 18:54:30.000000 copul-0.0.3/copul/families/archimedean/nelsen20.py
--rw-rw-rw-   0        0        0      658 2023-05-22 15:49:15.000000 copul-0.0.3/copul/families/archimedean/nelsen21.py
--rw-rw-rw-   0        0        0      686 2023-05-22 15:52:14.000000 copul-0.0.3/copul/families/archimedean/nelsen22.py
--rw-rw-rw-   0        0        0      596 2023-05-21 18:54:44.000000 copul-0.0.3/copul/families/archimedean/nelsen3.py
--rw-rw-rw-   0        0        0      354 2023-05-21 18:54:30.000000 copul-0.0.3/copul/families/archimedean/nelsen4.py
--rw-rw-rw-   0        0        0      376 2023-05-21 18:54:30.000000 copul-0.0.3/copul/families/archimedean/nelsen5.py
--rw-rw-rw-   0        0        0      336 2023-05-21 18:54:30.000000 copul-0.0.3/copul/families/archimedean/nelsen6.py
--rw-rw-rw-   0        0        0      524 2023-05-22 15:12:30.000000 copul-0.0.3/copul/families/archimedean/nelsen7.py
--rw-rw-rw-   0        0        0      616 2023-05-22 15:12:30.000000 copul-0.0.3/copul/families/archimedean/nelsen8.py
--rw-rw-rw-   0        0        0      557 2023-05-21 18:54:44.000000 copul-0.0.3/copul/families/archimedean/nelsen9.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:19:16.479402 copul-0.0.3/copul/families/extreme_value/
--rw-rw-rw-   0        0        0      386 2023-05-21 18:54:30.000000 copul-0.0.3/copul/families/extreme_value/__init__.py
--rw-rw-rw-   0        0        0      650 2023-05-21 18:54:30.000000 copul-0.0.3/copul/families/extreme_value/bb5.py
--rw-rw-rw-   0        0        0     6222 2023-05-21 18:41:35.000000 copul-0.0.3/copul/families/extreme_value/extreme_value_copula.py
--rw-rw-rw-   0        0        0      619 2023-05-21 18:54:30.000000 copul-0.0.3/copul/families/extreme_value/galambos.py
--rw-rw-rw-   0        0        0      441 2023-05-21 18:54:30.000000 copul-0.0.3/copul/families/extreme_value/gumbel.py
--rw-rw-rw-   0        0        0      771 2023-05-21 18:54:30.000000 copul-0.0.3/copul/families/extreme_value/huesler_reiss.py
--rw-rw-rw-   0        0        0      867 2023-05-21 18:54:30.000000 copul-0.0.3/copul/families/extreme_value/joe.py
--rw-rw-rw-   0        0        0      527 2023-05-21 18:54:30.000000 copul-0.0.3/copul/families/extreme_value/marshall_olkin.py
--rw-rw-rw-   0        0        0      820 2023-05-21 18:54:30.000000 copul-0.0.3/copul/families/extreme_value/t_ev.py
--rw-rw-rw-   0        0        0      770 2023-05-21 18:54:30.000000 copul-0.0.3/copul/families/extreme_value/tawn.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:19:16.481399 copul-0.0.3/copul/families/other/
--rw-rw-rw-   0        0        0        0 2023-05-21 18:41:35.000000 copul-0.0.3/copul/families/other/__init__.py
--rw-rw-rw-   0        0        0      886 2023-05-21 18:54:30.000000 copul-0.0.3/copul/families/other/farlie_gumbell_morgenstern.py
--rw-rw-rw-   0        0        0      976 2023-05-22 15:32:08.000000 copul-0.0.3/copul/families/other/frechet.py
--rw-rw-rw-   0        0        0     9165 2023-05-22 16:12:09.000000 copul-0.0.3/copul/families/other/plackett.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:19:16.481399 copul-0.0.3/copul/simulations/
--rw-rw-rw-   0        0        0        0 2023-05-17 14:16:18.000000 copul-0.0.3/copul/simulations/__init__.py
--rw-rw-rw-   0        0        0     1102 2023-05-22 16:10:23.000000 copul-0.0.3/copul/sympy_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:19:16.462011 copul-0.0.3/copul.egg-info/
--rw-rw-rw-   0        0        0     1986 2023-05-22 16:19:16.000000 copul-0.0.3/copul.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1912 2023-05-22 16:19:16.000000 copul-0.0.3/copul.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 16:19:16.000000 copul-0.0.3/copul.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-05-22 16:19:16.000000 copul-0.0.3/copul.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-22 16:19:16.000000 copul-0.0.3/copul.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      985 2023-05-22 16:18:24.000000 copul-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-05-22 16:19:16.482399 copul-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 13:24:38.373880 copul-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-05-21 18:41:35.000000 copul-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-05-17 14:16:18.000000 copul-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1986 2023-05-24 13:24:38.373880 copul-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1449 2023-05-22 16:18:24.000000 copul-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 13:24:38.337684 copul-0.0.4/copul/
+-rw-rw-rw-   0        0        0      357 2023-05-21 18:51:19.000000 copul-0.0.4/copul/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 13:24:38.346170 copul-0.0.4/copul/docs/
+-rw-rw-rw-   0        0        0        0 2023-05-17 14:16:18.000000 copul-0.0.4/copul/docs/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-05-24 13:24:38.351512 copul-0.0.4/copul/families/
+-rw-rw-rw-   0        0        0      293 2023-05-22 15:10:27.000000 copul-0.0.4/copul/families/__init__.py
+-rw-rw-rw-   0        0        0     2380 2023-05-22 16:16:20.000000 copul-0.0.4/copul/families/abstract_copula.py
+drwxrwxrwx   0        0        0        0 2023-05-24 13:24:38.367035 copul-0.0.4/copul/families/archimedean/
+-rw-rw-rw-   0        0        0     5839 2023-05-21 18:51:44.000000 copul-0.0.4/copul/families/archimedean/__init__.py
+-rw-rw-rw-   0        0        0     5386 2023-05-22 15:34:05.000000 copul-0.0.4/copul/families/archimedean/archimedean_copula.py
+-rw-rw-rw-   0        0        0     5160 2023-05-21 18:41:35.000000 copul-0.0.4/copul/families/archimedean/derivatives_overview_constructor.py
+-rw-rw-rw-   0        0        0     1141 2023-05-24 13:23:47.000000 copul-0.0.4/copul/families/archimedean/nelsen1.py
+-rw-rw-rw-   0        0        0      299 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/archimedean/nelsen10.py
+-rw-rw-rw-   0        0        0      294 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/archimedean/nelsen11.py
+-rw-rw-rw-   0        0        0      503 2023-05-22 15:14:02.000000 copul-0.0.4/copul/families/archimedean/nelsen12.py
+-rw-rw-rw-   0        0        0      322 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/archimedean/nelsen13.py
+-rw-rw-rw-   0        0        0      531 2023-05-22 15:34:05.000000 copul-0.0.4/copul/families/archimedean/nelsen14.py
+-rw-rw-rw-   0        0        0      357 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/archimedean/nelsen15.py
+-rw-rw-rw-   0        0        0     1079 2023-05-24 13:13:50.000000 copul-0.0.4/copul/families/archimedean/nelsen16.py
+-rw-rw-rw-   0        0        0     2454 2023-05-24 13:13:50.000000 copul-0.0.4/copul/families/archimedean/nelsen17.py
+-rw-rw-rw-   0        0        0      318 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/archimedean/nelsen18.py
+-rw-rw-rw-   0        0        0      333 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/archimedean/nelsen19.py
+-rw-rw-rw-   0        0        0      506 2023-05-22 14:44:54.000000 copul-0.0.4/copul/families/archimedean/nelsen2.py
+-rw-rw-rw-   0        0        0      330 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/archimedean/nelsen20.py
+-rw-rw-rw-   0        0        0      658 2023-05-22 15:49:15.000000 copul-0.0.4/copul/families/archimedean/nelsen21.py
+-rw-rw-rw-   0        0        0      686 2023-05-22 15:52:14.000000 copul-0.0.4/copul/families/archimedean/nelsen22.py
+-rw-rw-rw-   0        0        0      615 2023-05-24 13:11:22.000000 copul-0.0.4/copul/families/archimedean/nelsen3.py
+-rw-rw-rw-   0        0        0      354 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/archimedean/nelsen4.py
+-rw-rw-rw-   0        0        0      378 2023-05-24 13:13:50.000000 copul-0.0.4/copul/families/archimedean/nelsen5.py
+-rw-rw-rw-   0        0        0      336 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/archimedean/nelsen6.py
+-rw-rw-rw-   0        0        0      524 2023-05-22 15:12:30.000000 copul-0.0.4/copul/families/archimedean/nelsen7.py
+-rw-rw-rw-   0        0        0      616 2023-05-22 15:12:30.000000 copul-0.0.4/copul/families/archimedean/nelsen8.py
+-rw-rw-rw-   0        0        0      557 2023-05-21 18:54:44.000000 copul-0.0.4/copul/families/archimedean/nelsen9.py
+drwxrwxrwx   0        0        0        0 2023-05-24 13:24:38.371437 copul-0.0.4/copul/families/extreme_value/
+-rw-rw-rw-   0        0        0      386 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/extreme_value/__init__.py
+-rw-rw-rw-   0        0        0      650 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/extreme_value/bb5.py
+-rw-rw-rw-   0        0        0     6222 2023-05-21 18:41:35.000000 copul-0.0.4/copul/families/extreme_value/extreme_value_copula.py
+-rw-rw-rw-   0        0        0      619 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/extreme_value/galambos.py
+-rw-rw-rw-   0        0        0      441 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/extreme_value/gumbel.py
+-rw-rw-rw-   0        0        0      771 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/extreme_value/huesler_reiss.py
+-rw-rw-rw-   0        0        0      867 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/extreme_value/joe.py
+-rw-rw-rw-   0        0        0      527 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/extreme_value/marshall_olkin.py
+-rw-rw-rw-   0        0        0      820 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/extreme_value/t_ev.py
+-rw-rw-rw-   0        0        0      770 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/extreme_value/tawn.py
+drwxrwxrwx   0        0        0        0 2023-05-24 13:24:38.372440 copul-0.0.4/copul/families/other/
+-rw-rw-rw-   0        0        0        0 2023-05-21 18:41:35.000000 copul-0.0.4/copul/families/other/__init__.py
+-rw-rw-rw-   0        0        0      886 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/other/farlie_gumbell_morgenstern.py
+-rw-rw-rw-   0        0        0      976 2023-05-22 15:32:08.000000 copul-0.0.4/copul/families/other/frechet.py
+-rw-rw-rw-   0        0        0     9165 2023-05-22 16:12:09.000000 copul-0.0.4/copul/families/other/plackett.py
+drwxrwxrwx   0        0        0        0 2023-05-24 13:24:38.372440 copul-0.0.4/copul/simulations/
+-rw-rw-rw-   0        0        0        0 2023-05-17 14:16:18.000000 copul-0.0.4/copul/simulations/__init__.py
+-rw-rw-rw-   0        0        0     1276 2023-05-24 13:19:17.000000 copul-0.0.4/copul/sympy_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-05-24 13:24:38.346170 copul-0.0.4/copul.egg-info/
+-rw-rw-rw-   0        0        0     1986 2023-05-24 13:24:38.000000 copul-0.0.4/copul.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1912 2023-05-24 13:24:38.000000 copul-0.0.4/copul.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 13:24:38.000000 copul-0.0.4/copul.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-05-24 13:24:38.000000 copul-0.0.4/copul.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-24 13:24:38.000000 copul-0.0.4/copul.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1030 2023-05-24 13:24:19.000000 copul-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-05-24 13:24:38.373880 copul-0.0.4/setup.cfg
```

### Comparing `copul-0.0.3/LICENSE` & `copul-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `copul-0.0.3/PKG-INFO` & `copul-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copul
-Version: 0.0.3
+Version: 0.0.4
 Summary: Risk analysis with copulas.
 Author-email: Marcus Rockel <marcus.rockel@finance.uni-freiburg.de>, Eva Lütkebohmert-Holtz <eva.luetkebohmert@finance.uni-freiburg.de>, Jonathan Ansari <jonathan.ansari@plus.ac.at>
 Project-URL: Homepage, https://github.com/Corrram/copulas_in_systemic_risk
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `copul-0.0.3/README.md` & `copul-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `copul-0.0.3/copul/families/abstract_copula.py` & `copul-0.0.4/copul/families/abstract_copula.py`

 * *Files identical despite different names*

### Comparing `copul-0.0.3/copul/families/archimedean/__init__.py` & `copul-0.0.4/copul/families/archimedean/__init__.py`

 * *Files identical despite different names*

### Comparing `copul-0.0.3/copul/families/archimedean/archimedean_copula.py` & `copul-0.0.4/copul/families/archimedean/archimedean_copula.py`

 * *Files identical despite different names*

### Comparing `copul-0.0.3/copul/families/archimedean/derivatives_overview_constructor.py` & `copul-0.0.4/copul/families/archimedean/derivatives_overview_constructor.py`

 * *Files identical despite different names*

### Comparing `copul-0.0.3/copul/families/archimedean/nelsen1.py` & `copul-0.0.4/copul/families/archimedean/nelsen8.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,17 @@
 import numpy as np
 import sympy
 
 from copul.families.archimedean.archimedean_copula import ArchimedeanCopula
 from copul.sympy_wrapper import SymPyFunctionWrapper
 
 
-class Clayton(ArchimedeanCopula):
+class Nelsen8(ArchimedeanCopula):
     ac = ArchimedeanCopula
-    _inv_generator = ((1 / ac.t) ** ac.theta - 1) / ac.theta
-    theta_interval = sympy.Interval(0, np.inf, left_open=False, right_open=True)
+    _inv_generator = (1 - ac.t) / (1 + (ac.theta - 1) * ac.t)
+    theta_interval = sympy.Interval(1, np.inf, left_open=False, right_open=True)
 
     @property
     def cdf(self):
-        cdf = sympy.Max((self.u**(-self.theta) + self.v**(-self.theta) - 1)**(-1/self.theta), 0)
-        return SymPyFunctionWrapper(cdf)
-
-    @property
-    def pdf(self):  # ToDo: check this
-        pdf = (self.u**(-self.theta) + self.v**(-self.theta) - 1)**(-1-2/self.theta) \
-            * self.u**(-self.theta-1) * self.v**(-self.theta-1)
-        return SymPyFunctionWrapper(pdf)
-
-
-Nelsen1 = Clayton
+        num = self.theta**2*self.u*self.v - (1-self.u)*(1-self.v)
+        den = self.theta**2 - (self.theta - 1)**2*(1-self.u)*(1-self.v)
+        return SymPyFunctionWrapper(sympy.Max(num/den, 0))
```

### Comparing `copul-0.0.3/copul/families/archimedean/nelsen14.py` & `copul-0.0.4/copul/families/archimedean/nelsen14.py`

 * *Files identical despite different names*

### Comparing `copul-0.0.3/copul/families/archimedean/nelsen16.py` & `copul-0.0.4/copul/families/archimedean/nelsen16.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,16 +8,28 @@
 class Nelsen16(ArchimedeanCopula):
     ac = ArchimedeanCopula
     _inv_generator = (ac.theta / ac.t + 1) * (1 - ac.t)
     theta_interval = sympy.Interval(0, np.inf, left_open=True, right_open=True)
 
     @property
     def generator(self):
-        gen = - self.theta / 2 - self.y / 2 + 1 / 2 + 1 / 2 * \
-              sympy.sqrt((self.theta + self.y - 1) ** 2 + 4 * self.theta)
+        gen = (
+            -self.theta / 2
+            - self.y / 2
+            + 1 / 2
+            + 1 / 2 * sympy.sqrt((self.theta + self.y - 1) ** 2 + 4 * self.theta)
+        )
         return SymPyFunctionWrapper(gen)
 
+    @property
     def first_deriv_of_generator(self):
-        return (self.theta + self.y - 1) / (2 * ((self.theta + self.y - 1) ** 2 + 4 * self.theta)) - 1 / 2
+        return (self.theta + self.y - 1) / (
+            2 * ((self.theta + self.y - 1) ** 2 + 4 * self.theta)
+        ) - 1 / 2
 
+    @property
     def ci_char(self):
-        return sympy.log(1 / 2 - (self.theta + self.y - 1) / (8 * self.theta + 2 * (self.theta + self.y - 1) ** 2))
+        ci_char = sympy.log(
+            1 / 2
+            - (self.theta + self.y - 1) / (8 * self.theta + 2 * (self.theta + self.y - 1) ** 2)
+        )
+        return SymPyFunctionWrapper(ci_char)
```

### Comparing `copul-0.0.3/copul/families/archimedean/nelsen21.py` & `copul-0.0.4/copul/families/archimedean/nelsen21.py`

 * *Files identical despite different names*

### Comparing `copul-0.0.3/copul/families/archimedean/nelsen22.py` & `copul-0.0.4/copul/families/archimedean/nelsen22.py`

 * *Files identical despite different names*

### Comparing `copul-0.0.3/copul/families/archimedean/nelsen3.py` & `copul-0.0.4/copul/families/archimedean/nelsen3.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,11 +10,12 @@
     """
     ac = ArchimedeanCopula
     _inv_generator = sympy.log((1 - ac.theta * (1 - ac.t)) / ac.t)
     theta_interval = sympy.Interval(-1, 1, left_open=False, right_open=True)
 
     @property
     def cdf(self):
-        return SymPyFunctionWrapper((self.u * self.v) / (1 - self.theta * (1 - self.u) * (1 - self.v)))
+        cdf = (self.u * self.v) / (1 - self.theta * (1 - self.u) * (1 - self.v))
+        return SymPyFunctionWrapper(cdf)
 
 
 Nelsen3 = AliMikhailHak
```

### Comparing `copul-0.0.3/copul/families/archimedean/nelsen7.py` & `copul-0.0.4/copul/families/archimedean/nelsen7.py`

 * *Files identical despite different names*

### Comparing `copul-0.0.3/copul/families/archimedean/nelsen8.py` & `copul-0.0.4/copul/families/archimedean/nelsen9.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-import numpy as np
 import sympy
 
 from copul.families.archimedean.archimedean_copula import ArchimedeanCopula
 from copul.sympy_wrapper import SymPyFunctionWrapper
 
 
-class Nelsen8(ArchimedeanCopula):
+class GumbellBarnett(ArchimedeanCopula):
     ac = ArchimedeanCopula
-    _inv_generator = (1 - ac.t) / (1 + (ac.theta - 1) * ac.t)
-    theta_interval = sympy.Interval(1, np.inf, left_open=False, right_open=True)
+    _inv_generator = sympy.log(1 - ac.theta * sympy.log(ac.t))
+    theta_interval = sympy.Interval(0, 1, left_open=True, right_open=False)
 
     @property
     def cdf(self):
-        num = self.theta**2*self.u*self.v - (1-self.u)*(1-self.v)
-        den = self.theta**2 - (self.theta - 1)**2*(1-self.u)*(1-self.v)
-        return SymPyFunctionWrapper(sympy.Max(num/den, 0))
+        cdf = self.u*self.v*sympy.exp(-self.theta*sympy.log(self.u)*sympy.log(self.v))
+        return SymPyFunctionWrapper(cdf)
+
+
+Nelsen9 = GumbellBarnett
```

### Comparing `copul-0.0.3/copul/families/extreme_value/bb5.py` & `copul-0.0.4/copul/families/extreme_value/bb5.py`

 * *Files identical despite different names*

### Comparing `copul-0.0.3/copul/families/extreme_value/extreme_value_copula.py` & `copul-0.0.4/copul/families/extreme_value/extreme_value_copula.py`

 * *Files identical despite different names*

### Comparing `copul-0.0.3/copul/families/extreme_value/galambos.py` & `copul-0.0.4/copul/families/extreme_value/galambos.py`

 * *Files identical despite different names*

### Comparing `copul-0.0.3/copul/families/extreme_value/huesler_reiss.py` & `copul-0.0.4/copul/families/extreme_value/huesler_reiss.py`

 * *Files identical despite different names*

### Comparing `copul-0.0.3/copul/families/extreme_value/joe.py` & `copul-0.0.4/copul/families/extreme_value/joe.py`

 * *Files identical despite different names*

### Comparing `copul-0.0.3/copul/families/extreme_value/marshall_olkin.py` & `copul-0.0.4/copul/families/extreme_value/marshall_olkin.py`

 * *Files identical despite different names*

### Comparing `copul-0.0.3/copul/families/extreme_value/t_ev.py` & `copul-0.0.4/copul/families/extreme_value/t_ev.py`

 * *Files identical despite different names*

### Comparing `copul-0.0.3/copul/families/extreme_value/tawn.py` & `copul-0.0.4/copul/families/extreme_value/tawn.py`

 * *Files identical despite different names*

### Comparing `copul-0.0.3/copul/families/other/farlie_gumbell_morgenstern.py` & `copul-0.0.4/copul/families/other/farlie_gumbell_morgenstern.py`

 * *Files identical despite different names*

### Comparing `copul-0.0.3/copul/families/other/frechet.py` & `copul-0.0.4/copul/families/other/frechet.py`

 * *Files identical despite different names*

### Comparing `copul-0.0.3/copul/families/other/plackett.py` & `copul-0.0.4/copul/families/other/plackett.py`

 * *Files identical despite different names*

### Comparing `copul-0.0.3/copul/sympy_wrapper.py` & `copul-0.0.4/copul/sympy_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 import sympy
 
 
 class SymPyFunctionWrapper:
-
     def __init__(self, sympy_func):
-        allowed = (sympy.Pow, sympy.Mul, sympy.Add, sympy.Max, sympy.log, sympy.exp)
-        assert isinstance(sympy_func, allowed), f"Function must be from sympy, but is {type(sympy_func)}"
+        allowed = (
+            sympy.Pow,
+            sympy.Mul,
+            sympy.Add,
+            sympy.Max,
+            sympy.log,
+            sympy.exp,
+            sympy.core.numbers.Zero,
+        )
+        assert isinstance(
+            sympy_func, allowed
+        ), f"Function must be from sympy, but is {type(sympy_func)}"
         self._func = sympy_func
 
     def __str__(self):
         return str(self._func)
 
     def __repr__(self):
         return repr(self._func)
 
     def __call__(self, **kwargs):
         free_symbols = {str(f) for f in self._func.free_symbols}
-        assert set(kwargs).issubset(free_symbols), f"keys: {set(kwargs)}, free symbols: {self._func.free_symbols}"
+        assert set(kwargs).issubset(
+            free_symbols
+        ), f"keys: {set(kwargs)}, free symbols: {self._func.free_symbols}"
         vars_ = {f: kwargs[str(f)] for f in self._func.free_symbols if str(f) in kwargs}
         self._func = self._func.subs(vars_)
         return self
 
     @property
     def func(self):
         return self._func
```

### Comparing `copul-0.0.3/copul.egg-info/PKG-INFO` & `copul-0.0.4/copul.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copul
-Version: 0.0.3
+Version: 0.0.4
 Summary: Risk analysis with copulas.
 Author-email: Marcus Rockel <marcus.rockel@finance.uni-freiburg.de>, Eva Lütkebohmert-Holtz <eva.luetkebohmert@finance.uni-freiburg.de>, Jonathan Ansari <jonathan.ansari@plus.ac.at>
 Project-URL: Homepage, https://github.com/Corrram/copulas_in_systemic_risk
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `copul-0.0.3/copul.egg-info/SOURCES.txt` & `copul-0.0.4/copul.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `copul-0.0.3/pyproject.toml` & `copul-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "twine",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "copul"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Marcus Rockel", email="marcus.rockel@finance.uni-freiburg.de" },
   { name="Eva Lütkebohmert-Holtz", email="eva.luetkebohmert@finance.uni-freiburg.de" },
   { name="Jonathan Ansari", email="jonathan.ansari@plus.ac.at" },
 ]
 description = "Risk analysis with copulas."
 readme = "README.md"
@@ -32,9 +32,14 @@
     "sympy",
     "sympy_plot_backends>=1.6.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Corrram/copulas_in_systemic_risk"
 
+[tool]
+
+[tool.black]
+line-length = 100
+
 [tool.setuptools.package-data]
 copul = ["docs/*"]
```

