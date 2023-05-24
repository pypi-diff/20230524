# Comparing `tmp/pydisadm-1.3.0.tar.gz` & `tmp/pydisadm-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydisadm-1.3.0.tar", max compression
+gzip compressed data, was "pydisadm-1.3.1.tar", max compression
```

## Comparing `pydisadm-1.3.0.tar` & `pydisadm-1.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     2936 2023-05-21 16:07:32.973435 pydisadm-1.3.0/README.md
--rw-r--r--   0        0        0      111 2023-05-21 16:07:32.977435 pydisadm-1.3.0/pydisadm/__init__.py
--rw-r--r--   0        0        0     1130 2023-05-21 16:07:32.977435 pydisadm-1.3.0/pydisadm/__main__.py
--rw-r--r--   0        0        0     1540 2023-05-21 16:07:32.977435 pydisadm-1.3.0/pydisadm/bot/adm_bot.py
--rw-r--r--   0        0        0     7714 2023-05-21 16:07:32.977435 pydisadm-1.3.0/pydisadm/bot/adm_cog.py
--rw-r--r--   0        0        0     2649 2023-05-21 16:07:32.977435 pydisadm-1.3.0/pydisadm/bot/update_adm_modal.py
--rw-r--r--   0        0        0      702 2023-05-21 16:07:32.977435 pydisadm-1.3.0/pydisadm/bot/utils.py
--rw-r--r--   0        0        0     1535 2023-05-21 16:07:32.977435 pydisadm-1.3.0/pydisadm/configuration.py
--rw-r--r--   0        0        0     8044 2023-05-21 16:07:32.977435 pydisadm-1.3.0/pydisadm/controller/adm_controller.py
--rw-r--r--   0        0        0        0 2023-05-21 16:07:32.977435 pydisadm-1.3.0/pydisadm/data/__init__.py
--rw-r--r--   0        0        0   368313 2023-05-21 16:07:32.977435 pydisadm-1.3.0/pydisadm/data/mapConstellations.csv
--rw-r--r--   0        0        0    34613 2023-05-21 16:07:32.977435 pydisadm-1.3.0/pydisadm/data/mapRegions.csv
--rw-r--r--   0        0        0  3277768 2023-05-21 16:07:32.993436 pydisadm-1.3.0/pydisadm/data/mapSolarSystems.csv
--rw-r--r--   0        0        0      607 2023-05-21 16:07:32.993436 pydisadm-1.3.0/pydisadm/loader/datasets.py
--rw-r--r--   0        0        0     1085 2023-05-21 16:07:32.993436 pydisadm-1.3.0/pydisadm/loader/static_data.py
--rw-r--r--   0        0        0     1294 2023-05-21 16:07:32.993436 pydisadm-1.3.0/pydisadm/runnable/runnable_refresh.py
--rw-r--r--   0        0        0     3814 2023-05-21 16:07:32.993436 pydisadm-1.3.0/pydisadm/services/database.py
--rw-r--r--   0        0        0     1543 2023-05-21 16:07:32.993436 pydisadm-1.3.0/pydisadm/services/esi.py
--rw-r--r--   0        0        0      484 2023-05-21 16:07:32.993436 pydisadm-1.3.0/pydisadm/utils/adm_utils.py
--rw-r--r--   0        0        0      472 2023-05-21 16:07:32.993436 pydisadm-1.3.0/pydisadm/utils/datetime_utils.py
--rw-r--r--   0        0        0      623 2023-05-21 16:07:32.993436 pydisadm-1.3.0/pydisadm/utils/plot_utils.py
--rw-r--r--   0        0        0      193 2023-05-21 16:07:32.993436 pydisadm-1.3.0/pydisadm/utils/thread_utils.py
--rw-r--r--   0        0        0      953 2023-05-21 16:08:05.201922 pydisadm-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     3842 1970-01-01 00:00:00.000000 pydisadm-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2936 2023-05-24 12:39:18.484325 pydisadm-1.3.1/README.md
+-rw-r--r--   0        0        0      111 2023-05-24 12:39:18.488325 pydisadm-1.3.1/pydisadm/__init__.py
+-rw-r--r--   0        0        0     1130 2023-05-24 12:39:18.488325 pydisadm-1.3.1/pydisadm/__main__.py
+-rw-r--r--   0        0        0     1540 2023-05-24 12:39:18.488325 pydisadm-1.3.1/pydisadm/bot/adm_bot.py
+-rw-r--r--   0        0        0     7714 2023-05-24 12:39:18.488325 pydisadm-1.3.1/pydisadm/bot/adm_cog.py
+-rw-r--r--   0        0        0     2649 2023-05-24 12:39:18.488325 pydisadm-1.3.1/pydisadm/bot/update_adm_modal.py
+-rw-r--r--   0        0        0      702 2023-05-24 12:39:18.488325 pydisadm-1.3.1/pydisadm/bot/utils.py
+-rw-r--r--   0        0        0     1535 2023-05-24 12:39:18.488325 pydisadm-1.3.1/pydisadm/configuration.py
+-rw-r--r--   0        0        0     8044 2023-05-24 12:39:18.488325 pydisadm-1.3.1/pydisadm/controller/adm_controller.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:39:18.488325 pydisadm-1.3.1/pydisadm/data/__init__.py
+-rw-r--r--   0        0        0   368313 2023-05-24 12:39:18.488325 pydisadm-1.3.1/pydisadm/data/mapConstellations.csv
+-rw-r--r--   0        0        0    34613 2023-05-24 12:39:18.488325 pydisadm-1.3.1/pydisadm/data/mapRegions.csv
+-rw-r--r--   0        0        0  3277768 2023-05-24 12:39:18.508325 pydisadm-1.3.1/pydisadm/data/mapSolarSystems.csv
+-rw-r--r--   0        0        0      607 2023-05-24 12:39:18.508325 pydisadm-1.3.1/pydisadm/loader/datasets.py
+-rw-r--r--   0        0        0     1085 2023-05-24 12:39:18.508325 pydisadm-1.3.1/pydisadm/loader/static_data.py
+-rw-r--r--   0        0        0     1294 2023-05-24 12:39:18.508325 pydisadm-1.3.1/pydisadm/runnable/runnable_refresh.py
+-rw-r--r--   0        0        0     3814 2023-05-24 12:39:18.508325 pydisadm-1.3.1/pydisadm/services/database.py
+-rw-r--r--   0        0        0     1543 2023-05-24 12:39:18.508325 pydisadm-1.3.1/pydisadm/services/esi.py
+-rw-r--r--   0        0        0      484 2023-05-24 12:39:18.508325 pydisadm-1.3.1/pydisadm/utils/adm_utils.py
+-rw-r--r--   0        0        0      472 2023-05-24 12:39:18.508325 pydisadm-1.3.1/pydisadm/utils/datetime_utils.py
+-rw-r--r--   0        0        0      623 2023-05-24 12:39:18.508325 pydisadm-1.3.1/pydisadm/utils/plot_utils.py
+-rw-r--r--   0        0        0      193 2023-05-24 12:39:18.508325 pydisadm-1.3.1/pydisadm/utils/thread_utils.py
+-rw-r--r--   0        0        0      953 2023-05-24 12:39:58.203914 pydisadm-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3842 1970-01-01 00:00:00.000000 pydisadm-1.3.1/PKG-INFO
```

### Comparing `pydisadm-1.3.0/README.md` & `pydisadm-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.0/pydisadm/__main__.py` & `pydisadm-1.3.1/pydisadm/__main__.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.0/pydisadm/bot/adm_bot.py` & `pydisadm-1.3.1/pydisadm/bot/adm_bot.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.0/pydisadm/bot/adm_cog.py` & `pydisadm-1.3.1/pydisadm/bot/adm_cog.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.0/pydisadm/bot/update_adm_modal.py` & `pydisadm-1.3.1/pydisadm/bot/update_adm_modal.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.0/pydisadm/bot/utils.py` & `pydisadm-1.3.1/pydisadm/bot/utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.0/pydisadm/configuration.py` & `pydisadm-1.3.1/pydisadm/configuration.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.0/pydisadm/controller/adm_controller.py` & `pydisadm-1.3.1/pydisadm/controller/adm_controller.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.0/pydisadm/data/mapConstellations.csv` & `pydisadm-1.3.1/pydisadm/data/mapConstellations.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.0/pydisadm/data/mapRegions.csv` & `pydisadm-1.3.1/pydisadm/data/mapRegions.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.0/pydisadm/data/mapSolarSystems.csv` & `pydisadm-1.3.1/pydisadm/data/mapSolarSystems.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.0/pydisadm/loader/datasets.py` & `pydisadm-1.3.1/pydisadm/loader/datasets.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.0/pydisadm/loader/static_data.py` & `pydisadm-1.3.1/pydisadm/loader/static_data.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.0/pydisadm/runnable/runnable_refresh.py` & `pydisadm-1.3.1/pydisadm/runnable/runnable_refresh.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.0/pydisadm/services/database.py` & `pydisadm-1.3.1/pydisadm/services/database.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.0/pydisadm/services/esi.py` & `pydisadm-1.3.1/pydisadm/services/esi.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.0/pydisadm/utils/plot_utils.py` & `pydisadm-1.3.1/pydisadm/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.0/pyproject.toml` & `pydisadm-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydisadm"
-version = "1.3.0"
+version = "1.3.1"
 description = "A Discord bot providing ADM summaries."
 repository = "https://github.com/agelito/adm-bot"
 authors = ["Axel Wettervik"]
 license = "MIT"
 readme = "README.md"
 include = ["data/*.csv"]
```

### Comparing `pydisadm-1.3.0/PKG-INFO` & `pydisadm-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydisadm
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Discord bot providing ADM summaries.
 Home-page: https://github.com/agelito/adm-bot
 License: MIT
 Author: Axel Wettervik
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

