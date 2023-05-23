# Comparing `tmp/animegifs-0.5.3.tar.gz` & `tmp/animegifs-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animegifs-0.5.3.tar", last modified: Sat May 20 23:53:58 2023, max compression
+gzip compressed data, was "animegifs-0.5.4.tar", last modified: Tue May 23 23:33:14 2023, max compression
```

## Comparing `animegifs-0.5.3.tar` & `animegifs-0.5.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 23:53:58.465564 animegifs-0.5.3/
--rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.5.3/LICENSE
--rw-rw-rw-   0        0        0     1214 2023-05-20 23:53:58.464563 animegifs-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0      622 2023-05-20 23:51:48.000000 animegifs-0.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 23:53:58.437562 animegifs-0.5.3/animegifs/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.5.3/animegifs/__init__.py
--rw-rw-rw-   0        0        0     1064 2023-05-20 23:51:21.000000 animegifs-0.5.3/animegifs/animegifs.py
-drwxrwxrwx   0        0        0        0 2023-05-20 23:53:58.462563 animegifs-0.5.3/animegifs/distutils/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.5.3/animegifs/distutils/__init__.py
--rw-rw-rw-   0        0        0     1186 2023-05-10 14:18:41.000000 animegifs-0.5.3/animegifs/distutils/errors.py
--rw-rw-rw-   0        0        0      705 2023-05-20 23:51:21.000000 animegifs-0.5.3/animegifs/distutils/gifs.py
-drwxrwxrwx   0        0        0        0 2023-05-20 23:53:58.453564 animegifs-0.5.3/animegifs.egg-info/
--rw-rw-rw-   0        0        0     1214 2023-05-20 23:53:58.000000 animegifs-0.5.3/animegifs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-05-20 23:53:58.000000 animegifs-0.5.3/animegifs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 23:53:58.000000 animegifs-0.5.3/animegifs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-20 23:53:58.000000 animegifs-0.5.3/animegifs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-20 23:53:58.000000 animegifs-0.5.3/animegifs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 23:53:58.466565 animegifs-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1072 2023-05-20 23:51:21.000000 animegifs-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:33:14.481083 animegifs-0.5.4/
+-rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.5.4/LICENSE
+-rw-rw-rw-   0        0        0     1258 2023-05-23 23:33:14.480082 animegifs-0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0      662 2023-05-23 16:46:53.000000 animegifs-0.5.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 23:33:14.460080 animegifs-0.5.4/animegifs/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.5.4/animegifs/__init__.py
+-rw-rw-rw-   0        0        0     1096 2023-05-23 16:46:53.000000 animegifs-0.5.4/animegifs/animegifs.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:33:14.478085 animegifs-0.5.4/animegifs/distutils/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.5.4/animegifs/distutils/__init__.py
+-rw-rw-rw-   0        0        0     1186 2023-05-10 14:18:41.000000 animegifs-0.5.4/animegifs/distutils/errors.py
+-rw-rw-rw-   0        0        0      779 2023-05-23 16:46:53.000000 animegifs-0.5.4/animegifs/distutils/gifs.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:33:14.469081 animegifs-0.5.4/animegifs.egg-info/
+-rw-rw-rw-   0        0        0     1258 2023-05-23 23:33:14.000000 animegifs-0.5.4/animegifs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-05-23 23:33:14.000000 animegifs-0.5.4/animegifs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 23:33:14.000000 animegifs-0.5.4/animegifs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-23 23:33:14.000000 animegifs-0.5.4/animegifs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-23 23:33:14.000000 animegifs-0.5.4/animegifs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 23:33:14.481083 animegifs-0.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     1072 2023-05-23 16:46:53.000000 animegifs-0.5.4/setup.py
```

### Comparing `animegifs-0.5.3/LICENSE` & `animegifs-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `animegifs-0.5.3/PKG-INFO` & `animegifs-0.5.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.5.3
+Version: 0.5.4
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
 Keywords: anime,gif,python,anime-gif,discord
 Platform: UNKNOWN
@@ -56,11 +56,15 @@
 * Highfive
 * Hug
 * Icecream
 * Insult
 * Kill
 * Kiss
 * Lick
+* Love
+* Marry
+* Nosebleed
+* Nuzzle
 
 WIP.
```

### Comparing `animegifs-0.5.3/README.md` & `animegifs-0.5.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -38,9 +38,13 @@
 * Highfive
 * Hug
 * Icecream
 * Insult
 * Kill
 * Kiss
 * Lick
+* Love
+* Marry
+* Nosebleed
+* Nuzzle
 
 WIP.
```

### Comparing `animegifs-0.5.3/animegifs/animegifs.py` & `animegifs-0.5.4/animegifs/animegifs.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         """
         Insert a valid category and get a gif.
 
         Args:
             category (str): Valid categories: attack, bite, bloodsuck, blush, bonk,
                 brofist, cry, cuddle, dance, disgust, facedesk, facepalm, flick, flirt,
                 handhold, happy, harass, highfive, hug, icecream, insult, kill, kiss,
-                lick.
+                lick, love, marry, nosebleed, nuzzle.
 
         Returns:
             gif: gif (url) -> str
         """
         if type(category) is int:
             raise errors.CategoryIntegral(category)
         elif category.lower() in gifs.gifs_name_list:
```

### Comparing `animegifs-0.5.3/animegifs/distutils/errors.py` & `animegifs-0.5.4/animegifs/distutils/errors.py`

 * *Files identical despite different names*

### Comparing `animegifs-0.5.3/animegifs/distutils/gifs.py` & `animegifs-0.5.4/animegifs/distutils/gifs.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,16 +5,16 @@
                   "bite", 'bloodsuck', 'blush', 'bonk', 'brofist',
                   'cry', 'cuddle',
                   'dance', 'disgust',
                   'facedesk', 'facepalm', 'flick', 'flirt',
                   'handhold', 'happy', 'harass', 'highfive', 'hug',
                   'icecream', 'insult',
                   'kill', 'kiss',
-                  'lick']
+                  'lick', 'love',
+                  'marry',
+                  'nosebleed', 'nuzzle']
 
 def access():
     data = requests.get("https://objectstorage.eu-frankfurt-1.oraclecloud.com/p/zDPowf1lXXMMpXzo_Lnb31IOtUyxrtD-kDS7fpKxLuCYnR5xr-171Tyz0tW0EhKV/n/frqs54dqeajn/b/animegifs_lib/o/gifs.json").content
     data = json.loads(data)
 
     return data
-
-
```

### Comparing `animegifs-0.5.3/animegifs.egg-info/PKG-INFO` & `animegifs-0.5.4/animegifs.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.5.3
+Version: 0.5.4
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
 Keywords: anime,gif,python,anime-gif,discord
 Platform: UNKNOWN
@@ -56,11 +56,15 @@
 * Highfive
 * Hug
 * Icecream
 * Insult
 * Kill
 * Kiss
 * Lick
+* Love
+* Marry
+* Nosebleed
+* Nuzzle
 
 WIP.
```

### Comparing `animegifs-0.5.3/setup.py` & `animegifs-0.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 LONG_DESCRIPTION = long_description
-VERSION = '0.5.3'
+VERSION = '0.5.4'
 
 setup(
     name='animegifs',
     package_dir={"anime_gifs": "animegifs"},
     packages=["animegifs", "animegifs.distutils"],
     version=VERSION,
     description='Get random anime gifs by category.',
```

