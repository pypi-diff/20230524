# Comparing `tmp/wordlink-1.0.4.tar.gz` & `tmp/wordlink-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordlink-1.0.4.tar", last modified: Tue May 23 01:41:36 2023, max compression
+gzip compressed data, was "wordlink-1.0.5.tar", last modified: Wed May 24 21:16:56 2023, max compression
```

## Comparing `wordlink-1.0.4.tar` & `wordlink-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-23 01:41:36.316065 wordlink-1.0.4/
--rw-r--r--   0 bloom      (501) staff       (20)     4117 2023-05-23 01:41:36.316230 wordlink-1.0.4/PKG-INFO
--rw-r--r--   0 bloom      (501) staff       (20)     3615 2023-05-23 01:40:33.000000 wordlink-1.0.4/readme.md
--rw-r--r--   0 bloom      (501) staff       (20)      746 2023-05-23 01:41:36.316517 wordlink-1.0.4/setup.cfg
--rw-r--r--   0 bloom      (501) staff       (20)      713 2023-05-23 01:41:27.000000 wordlink-1.0.4/setup.py
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-23 01:41:36.315030 wordlink-1.0.4/wordlink/
--rw-r--r--   0 bloom      (501) staff       (20)        0 2023-05-22 21:54:44.000000 wordlink-1.0.4/wordlink/__init__.py
--rw-r--r--   0 bloom      (501) staff       (20)     3582 2023-05-22 21:54:44.000000 wordlink-1.0.4/wordlink/__main__.py
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-23 01:41:36.315969 wordlink-1.0.4/wordlink.egg-info/
--rw-r--r--   0 bloom      (501) staff       (20)     4117 2023-05-23 01:41:36.000000 wordlink-1.0.4/wordlink.egg-info/PKG-INFO
--rw-r--r--   0 bloom      (501) staff       (20)      264 2023-05-23 01:41:36.000000 wordlink-1.0.4/wordlink.egg-info/SOURCES.txt
--rw-r--r--   0 bloom      (501) staff       (20)        1 2023-05-23 01:41:36.000000 wordlink-1.0.4/wordlink.egg-info/dependency_links.txt
--rw-r--r--   0 bloom      (501) staff       (20)       43 2023-05-23 01:41:36.000000 wordlink-1.0.4/wordlink.egg-info/entry_points.txt
--rw-r--r--   0 bloom      (501) staff       (20)       24 2023-05-23 01:41:36.000000 wordlink-1.0.4/wordlink.egg-info/requires.txt
--rw-r--r--   0 bloom      (501) staff       (20)        9 2023-05-23 01:41:36.000000 wordlink-1.0.4/wordlink.egg-info/top_level.txt
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-24 21:16:56.719028 wordlink-1.0.5/
+-rw-r--r--   0 bloom      (501) staff       (20)     1048 2023-05-24 20:43:31.000000 wordlink-1.0.5/LICENSE
+-rw-r--r--   0 bloom      (501) staff       (20)      523 2023-05-24 21:16:56.719096 wordlink-1.0.5/PKG-INFO
+-rw-r--r--   0 bloom      (501) staff       (20)     3641 2023-05-24 21:00:09.000000 wordlink-1.0.5/README
+-rw-r--r--   0 bloom      (501) staff       (20)      746 2023-05-24 21:16:56.719330 wordlink-1.0.5/setup.cfg
+-rw-r--r--   0 bloom      (501) staff       (20)      713 2023-05-24 20:57:22.000000 wordlink-1.0.5/setup.py
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-24 21:16:56.717798 wordlink-1.0.5/tests/
+-rw-r--r--   0 bloom      (501) staff       (20)        0 2023-05-24 20:48:47.000000 wordlink-1.0.5/tests/__init__.py
+-rw-r--r--   0 bloom      (501) staff       (20)     3758 2023-05-24 20:43:31.000000 wordlink-1.0.5/tests/main_test.py
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-24 21:16:56.718147 wordlink-1.0.5/wordlink/
+-rw-r--r--   0 bloom      (501) staff       (20)        0 2023-05-24 20:43:31.000000 wordlink-1.0.5/wordlink/__init__.py
+-rw-r--r--   0 bloom      (501) staff       (20)     3582 2023-05-24 20:43:31.000000 wordlink-1.0.5/wordlink/__main__.py
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-24 21:16:56.718935 wordlink-1.0.5/wordlink.egg-info/
+-rw-r--r--   0 bloom      (501) staff       (20)      523 2023-05-24 21:16:56.000000 wordlink-1.0.5/wordlink.egg-info/PKG-INFO
+-rw-r--r--   0 bloom      (501) staff       (20)      306 2023-05-24 21:16:56.000000 wordlink-1.0.5/wordlink.egg-info/SOURCES.txt
+-rw-r--r--   0 bloom      (501) staff       (20)        1 2023-05-24 21:16:56.000000 wordlink-1.0.5/wordlink.egg-info/dependency_links.txt
+-rw-r--r--   0 bloom      (501) staff       (20)       43 2023-05-24 21:16:56.000000 wordlink-1.0.5/wordlink.egg-info/entry_points.txt
+-rw-r--r--   0 bloom      (501) staff       (20)       24 2023-05-24 21:16:56.000000 wordlink-1.0.5/wordlink.egg-info/requires.txt
+-rw-r--r--   0 bloom      (501) staff       (20)       15 2023-05-24 21:16:56.000000 wordlink-1.0.5/wordlink.egg-info/top_level.txt
```

### Comparing `wordlink-1.0.4/PKG-INFO` & `wordlink-1.0.5/README`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,10 @@
-Metadata-Version: 2.1
-Name: wordlink
-Version: 1.0.4
-Summary: Word Link Generator
-Home-page: https://github.com/psibir/wordlink
-Download-URL: https://github.com/psibir/wordlink/archive/v_01.tar.gz
-Author: Trevor Bloomfield
-Author-email: bloomfieldtm@gmail.com
-Keywords: word,link,html,console
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # wordlink
 
-![wordlink logo](/wordlink_logo.png)
+![wordlink logo](/logo.png)
 
 A Word Link Generator that searches for a given term in multiple text files within a specified directory and generates links to the matched occurrences. It provides two output options: an HTML file with clickable links or a console display using a formatted table.
 The `__main__.py` file is located in the `/wordlink/` directory.
 
 ## Prerequisites
 
 - Python 3.x
@@ -32,14 +17,16 @@
 1. Clone the repository or download the script file.
 2. Install the required libraries by running the following command:
 
    ```bash
    pip install wordlink
    ```
 
+See [INSTALL](INSTALL) for instructions to clone from GitHub.
+
 ## Usage
 
 Run the script using the following command:
 
 ```bash
 python3 wordlink <search_term> <search_directory> [-o OUTPUT_FILE]
 ```
@@ -89,8 +76,8 @@
 ## Limitations
 
 - The tool searches for the specified term within all text files (`.txt`) in the given directory and its subdirectories. It does not support searching within other file formats.
 - The maximum Levenshtein distance for finding near matches is set to 1. This can be adjusted by modifying the `max_l_dist` parameter in the `find_near_matches` function call within the `find_word_locations` method.
 
 ## License
 
-This code is provided under the [MIT License](https://opensource.org/licenses/MIT). Feel free to modify and use it according to your needs.
+This code is provided under the [MIT License](LICENSE). Feel free to modify and use it according to your needs.
```

### Comparing `wordlink-1.0.4/setup.cfg` & `wordlink-1.0.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wordlink
-version = 1.0.0
+version = 1.0.5
 author = Trevor Bloomfield
 author_email = bloomfieldtm@gmail.com
 description = A Word Link Generator that searches for a given term in multiple text files within a specified directory and generates links to the matched occurrences.
 long_description = file: readme.md
 long_description_content_type = text/markdown
 url = https://github.com/psibir/wordlink
 classifiers =
```

### Comparing `wordlink-1.0.4/setup.py` & `wordlink-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wordlink',
-    version='1.0.4',
+    version='1.0.5',
     author='Trevor Bloomfield',
     author_email='bloomfieldtm@gmail.com',
     description='Word Link Generator',
     py_modules=['wordlink'],
     url = 'https://github.com/psibir/wordlink',   # Provide either the link to your github or to your website
     download_url = 'https://github.com/psibir/wordlink/archive/v_01.tar.gz',    # I explain this later on
     keywords = ['word', 'link', 'html', 'console'],   # Keywords that define your package best
```

### Comparing `wordlink-1.0.4/wordlink/__main__.py` & `wordlink-1.0.5/wordlink/__main__.py`

 * *Files identical despite different names*

