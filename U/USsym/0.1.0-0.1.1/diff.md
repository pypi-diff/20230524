# Comparing `tmp/USsym-0.1.0.tar.gz` & `tmp/USsym-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "USsym-0.1.0.tar", last modified: Wed May 24 08:24:36 2023, max compression
+gzip compressed data, was "USsym-0.1.1.tar", last modified: Wed May 24 08:31:48 2023, max compression
```

## Comparing `USsym-0.1.0.tar` & `USsym-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,20 @@
-drwxr-x---   0 vscode    (1010) vscode    (1013)        0 2023-05-24 08:24:34.985227 USsym-0.1.0/
-drwxr-x---   0 vscode    (1010) vscode    (1013)        0 2023-05-24 08:24:34.965227 USsym-0.1.0/.devcontainer/
--rwxrwxrwx   0 vscode    (1010) vscode    (1013)     1181 2023-05-10 15:58:06.000000 USsym-0.1.0/.devcontainer/devcontainer.json
--rwxrwxrwx   0 vscode    (1010) vscode    (1013)       73 2023-05-05 15:13:29.000000 USsym-0.1.0/.gitignore
-drwxr-x---   0 vscode    (1010) vscode    (1013)        0 2023-05-24 08:24:34.975227 USsym-0.1.0/BeamPatternCompute/
--rwxrwxrwx   0 vscode    (1010) vscode    (1013)     6794 2023-05-23 12:14:35.000000 USsym-0.1.0/BeamPatternCompute/BpCompute.py
--rwxrwxrwx   0 vscode    (1010) vscode    (1013)     8763 2023-05-23 10:11:08.000000 USsym-0.1.0/BeamPatternCompute/MapGeneration.py
--rw-r-----   0 vscode    (1010) vscode    (1013)        0 2023-05-24 07:59:29.000000 USsym-0.1.0/BeamPatternCompute/__init__.py
--rwxrwxrwx   0 vscode    (1010) vscode    (1013)     9963 2023-05-23 14:01:03.000000 USsym-0.1.0/BeamPatternCompute/classBP.py
--rwxrwxrwx   0 vscode    (1010) vscode    (1013)     5668 2023-05-23 12:09:25.000000 USsym-0.1.0/BeamPatternCompute/f_initialization.py
--rw-r-----   0 vscode    (1010) vscode    (1013)       31 2023-05-24 08:18:51.000000 USsym-0.1.0/BeamPatternCompute/modules.py
--rw-r-----   0 vscode    (1010) vscode    (1013)    35149 2023-05-24 06:29:16.000000 USsym-0.1.0/LICENSE
--rw-r-----   0 vscode    (1010) vscode    (1013)      178 2023-05-24 08:24:34.985227 USsym-0.1.0/PKG-INFO
--rw-r-----   0 vscode    (1010) vscode    (1013)     2032 2023-05-24 06:29:16.000000 USsym-0.1.0/README.md
-drwxr-x---   0 vscode    (1010) vscode    (1013)        0 2023-05-24 08:24:34.985227 USsym-0.1.0/USsym.egg-info/
--rw-r-----   0 vscode    (1010) vscode    (1013)      178 2023-05-24 08:24:34.000000 USsym-0.1.0/USsym.egg-info/PKG-INFO
--rw-r-----   0 vscode    (1010) vscode    (1013)      436 2023-05-24 08:24:34.000000 USsym-0.1.0/USsym.egg-info/SOURCES.txt
--rw-r-----   0 vscode    (1010) vscode    (1013)        1 2023-05-24 08:24:34.000000 USsym-0.1.0/USsym.egg-info/dependency_links.txt
--rw-r-----   0 vscode    (1010) vscode    (1013)       36 2023-05-24 08:24:34.000000 USsym-0.1.0/USsym.egg-info/requires.txt
--rw-r-----   0 vscode    (1010) vscode    (1013)       19 2023-05-24 08:24:34.000000 USsym-0.1.0/USsym.egg-info/top_level.txt
--rwxrwxrwx   0 vscode    (1010) vscode    (1013)     1143 2023-05-24 07:52:06.000000 USsym-0.1.0/main.py
--rwxrwxrwx   0 vscode    (1010) vscode    (1013)       47 2023-05-24 06:49:52.000000 USsym-0.1.0/requirements.txt
--rw-r-----   0 vscode    (1010) vscode    (1013)       38 2023-05-24 08:24:34.985227 USsym-0.1.0/setup.cfg
--rw-r-----   0 vscode    (1010) vscode    (1013)      459 2023-05-24 08:23:08.000000 USsym-0.1.0/setup.py
+drwxr-x---   0 vscode    (1010) vscode    (1013)        0 2023-05-24 08:31:46.935137 USsym-0.1.1/
+drwxr-x---   0 vscode    (1010) vscode    (1013)        0 2023-05-24 08:31:46.915137 USsym-0.1.1/.devcontainer/
+-rwxrwxrwx   0 vscode    (1010) vscode    (1013)     1181 2023-05-10 15:58:06.000000 USsym-0.1.1/.devcontainer/devcontainer.json
+-rwxrwxrwx   0 vscode    (1010) vscode    (1013)       73 2023-05-05 15:13:29.000000 USsym-0.1.1/.gitignore
+-rw-r-----   0 vscode    (1010) vscode    (1013)    35149 2023-05-24 06:29:16.000000 USsym-0.1.1/LICENSE
+-rw-r-----   0 vscode    (1010) vscode    (1013)      178 2023-05-24 08:31:46.935137 USsym-0.1.1/PKG-INFO
+-rw-r-----   0 vscode    (1010) vscode    (1013)     2032 2023-05-24 06:29:16.000000 USsym-0.1.1/README.md
+drwxr-x---   0 vscode    (1010) vscode    (1013)        0 2023-05-24 08:31:46.925137 USsym-0.1.1/USsym/
+-rw-r-----   0 vscode    (1010) vscode    (1013)        0 2023-05-24 07:59:29.000000 USsym-0.1.1/USsym/__init__.py
+-rw-r-----   0 vscode    (1010) vscode    (1013)       31 2023-05-24 08:18:51.000000 USsym-0.1.1/USsym/modules.py
+drwxr-x---   0 vscode    (1010) vscode    (1013)        0 2023-05-24 08:31:46.935137 USsym-0.1.1/USsym.egg-info/
+-rw-r-----   0 vscode    (1010) vscode    (1013)      178 2023-05-24 08:31:46.000000 USsym-0.1.1/USsym.egg-info/PKG-INFO
+-rw-r-----   0 vscode    (1010) vscode    (1013)      273 2023-05-24 08:31:46.000000 USsym-0.1.1/USsym.egg-info/SOURCES.txt
+-rw-r-----   0 vscode    (1010) vscode    (1013)        1 2023-05-24 08:31:46.000000 USsym-0.1.1/USsym.egg-info/dependency_links.txt
+-rw-r-----   0 vscode    (1010) vscode    (1013)       36 2023-05-24 08:31:46.000000 USsym-0.1.1/USsym.egg-info/requires.txt
+-rw-r-----   0 vscode    (1010) vscode    (1013)       25 2023-05-24 08:31:46.000000 USsym-0.1.1/USsym.egg-info/top_level.txt
+-rwxrwxrwx   0 vscode    (1010) vscode    (1013)     1153 2023-05-24 08:27:41.000000 USsym-0.1.1/main.py
+-rwxrwxrwx   0 vscode    (1010) vscode    (1013)       47 2023-05-24 06:49:52.000000 USsym-0.1.1/requirements.txt
+-rw-r-----   0 vscode    (1010) vscode    (1013)       38 2023-05-24 08:31:46.935137 USsym-0.1.1/setup.cfg
+-rw-r-----   0 vscode    (1010) vscode    (1013)      459 2023-05-24 08:31:43.000000 USsym-0.1.1/setup.py
```

### Comparing `USsym-0.1.0/.devcontainer/devcontainer.json` & `USsym-0.1.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `USsym-0.1.0/LICENSE` & `USsym-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `USsym-0.1.0/README.md` & `USsym-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `USsym-0.1.0/main.py` & `USsym-0.1.1/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # %%
-from medus import BeamPattern
-
+from BeamPatternCompute import BpCompute
 # %%
 ####### Generate a test Narrow Beam Pattern with default values #######
 
 NB = BeamPattern(device = "gpu")
 
 # Compute and saving of maps
 NB.MapsCompute()
```

