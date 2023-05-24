# Comparing `tmp/USsym-0.1.2.tar.gz` & `tmp/USsym-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "USsym-0.1.2.tar", last modified: Wed May 24 08:35:18 2023, max compression
+gzip compressed data, was "USsym-0.1.3.tar", last modified: Wed May 24 08:37:16 2023, max compression
```

## Comparing `USsym-0.1.2.tar` & `USsym-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-x---   0 vscode    (1010) vscode    (1013)        0 2023-05-24 08:35:17.295094 USsym-0.1.2/
-drwxr-x---   0 vscode    (1010) vscode    (1013)        0 2023-05-24 08:35:17.265094 USsym-0.1.2/.devcontainer/
--rwxrwxrwx   0 vscode    (1010) vscode    (1013)     1181 2023-05-10 15:58:06.000000 USsym-0.1.2/.devcontainer/devcontainer.json
--rwxrwxrwx   0 vscode    (1010) vscode    (1013)       73 2023-05-05 15:13:29.000000 USsym-0.1.2/.gitignore
--rw-r-----   0 vscode    (1010) vscode    (1013)    35149 2023-05-24 06:29:16.000000 USsym-0.1.2/LICENSE
--rw-r-----   0 vscode    (1010) vscode    (1013)      178 2023-05-24 08:35:17.285094 USsym-0.1.2/PKG-INFO
--rw-r-----   0 vscode    (1010) vscode    (1013)     2032 2023-05-24 06:29:16.000000 USsym-0.1.2/README.md
-drwxr-x---   0 vscode    (1010) vscode    (1013)        0 2023-05-24 08:35:17.275094 USsym-0.1.2/USsym/
--rw-r-----   0 vscode    (1010) vscode    (1013)        0 2023-05-24 07:59:29.000000 USsym-0.1.2/USsym/__init__.py
--rw-r-----   0 vscode    (1010) vscode    (1013)       31 2023-05-24 08:18:51.000000 USsym-0.1.2/USsym/modules.py
-drwxr-x---   0 vscode    (1010) vscode    (1013)        0 2023-05-24 08:35:17.285094 USsym-0.1.2/USsym.egg-info/
--rw-r-----   0 vscode    (1010) vscode    (1013)      178 2023-05-24 08:35:17.000000 USsym-0.1.2/USsym.egg-info/PKG-INFO
--rw-r-----   0 vscode    (1010) vscode    (1013)      273 2023-05-24 08:35:17.000000 USsym-0.1.2/USsym.egg-info/SOURCES.txt
--rw-r-----   0 vscode    (1010) vscode    (1013)        1 2023-05-24 08:35:17.000000 USsym-0.1.2/USsym.egg-info/dependency_links.txt
--rw-r-----   0 vscode    (1010) vscode    (1013)       36 2023-05-24 08:35:17.000000 USsym-0.1.2/USsym.egg-info/requires.txt
--rw-r-----   0 vscode    (1010) vscode    (1013)       25 2023-05-24 08:35:17.000000 USsym-0.1.2/USsym.egg-info/top_level.txt
--rwxrwxrwx   0 vscode    (1010) vscode    (1013)     1153 2023-05-24 08:27:41.000000 USsym-0.1.2/main.py
--rwxrwxrwx   0 vscode    (1010) vscode    (1013)       47 2023-05-24 06:49:52.000000 USsym-0.1.2/requirements.txt
--rw-r-----   0 vscode    (1010) vscode    (1013)       38 2023-05-24 08:35:17.295094 USsym-0.1.2/setup.cfg
--rw-r-----   0 vscode    (1010) vscode    (1013)      459 2023-05-24 08:35:02.000000 USsym-0.1.2/setup.py
+drwxr-x---   0 vscode    (1010) vscode    (1013)        0 2023-05-24 08:37:15.715069 USsym-0.1.3/
+drwxr-x---   0 vscode    (1010) vscode    (1013)        0 2023-05-24 08:37:15.695069 USsym-0.1.3/.devcontainer/
+-rwxrwxrwx   0 vscode    (1010) vscode    (1013)     1181 2023-05-10 15:58:06.000000 USsym-0.1.3/.devcontainer/devcontainer.json
+-rwxrwxrwx   0 vscode    (1010) vscode    (1013)       73 2023-05-05 15:13:29.000000 USsym-0.1.3/.gitignore
+-rw-r-----   0 vscode    (1010) vscode    (1013)    35149 2023-05-24 06:29:16.000000 USsym-0.1.3/LICENSE
+-rw-r-----   0 vscode    (1010) vscode    (1013)      178 2023-05-24 08:37:15.715069 USsym-0.1.3/PKG-INFO
+-rw-r-----   0 vscode    (1010) vscode    (1013)     2032 2023-05-24 06:29:16.000000 USsym-0.1.3/README.md
+drwxr-x---   0 vscode    (1010) vscode    (1013)        0 2023-05-24 08:37:15.695069 USsym-0.1.3/USsym/
+-rw-r-----   0 vscode    (1010) vscode    (1013)        0 2023-05-24 07:59:29.000000 USsym-0.1.3/USsym/__init__.py
+-rw-r-----   0 vscode    (1010) vscode    (1013)       51 2023-05-24 08:37:01.000000 USsym-0.1.3/USsym/modules.py
+drwxr-x---   0 vscode    (1010) vscode    (1013)        0 2023-05-24 08:37:15.705069 USsym-0.1.3/USsym.egg-info/
+-rw-r-----   0 vscode    (1010) vscode    (1013)      178 2023-05-24 08:37:15.000000 USsym-0.1.3/USsym.egg-info/PKG-INFO
+-rw-r-----   0 vscode    (1010) vscode    (1013)      273 2023-05-24 08:37:15.000000 USsym-0.1.3/USsym.egg-info/SOURCES.txt
+-rw-r-----   0 vscode    (1010) vscode    (1013)        1 2023-05-24 08:37:15.000000 USsym-0.1.3/USsym.egg-info/dependency_links.txt
+-rw-r-----   0 vscode    (1010) vscode    (1013)       36 2023-05-24 08:37:15.000000 USsym-0.1.3/USsym.egg-info/requires.txt
+-rw-r-----   0 vscode    (1010) vscode    (1013)       25 2023-05-24 08:37:15.000000 USsym-0.1.3/USsym.egg-info/top_level.txt
+-rwxrwxrwx   0 vscode    (1010) vscode    (1013)     1153 2023-05-24 08:27:41.000000 USsym-0.1.3/main.py
+-rwxrwxrwx   0 vscode    (1010) vscode    (1013)       47 2023-05-24 06:49:52.000000 USsym-0.1.3/requirements.txt
+-rw-r-----   0 vscode    (1010) vscode    (1013)       38 2023-05-24 08:37:15.715069 USsym-0.1.3/setup.cfg
+-rw-r-----   0 vscode    (1010) vscode    (1013)      459 2023-05-24 08:37:12.000000 USsym-0.1.3/setup.py
```

### Comparing `USsym-0.1.2/.devcontainer/devcontainer.json` & `USsym-0.1.3/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `USsym-0.1.2/LICENSE` & `USsym-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `USsym-0.1.2/README.md` & `USsym-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `USsym-0.1.2/main.py` & `USsym-0.1.3/main.py`

 * *Files identical despite different names*

