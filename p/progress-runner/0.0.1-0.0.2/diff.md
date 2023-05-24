# Comparing `tmp/progress_runner-0.0.1.tar.gz` & `tmp/progress_runner-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progress_runner-0.0.1.tar", last modified: Wed May 24 00:33:46 2023, max compression
+gzip compressed data, was "progress_runner-0.0.2.tar", last modified: Wed May 24 00:42:31 2023, max compression
```

## Comparing `progress_runner-0.0.1.tar` & `progress_runner-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-24 00:33:46.715789 progress_runner-0.0.1/
--rwxrwxrwx   0 root         (0) root         (0)      729 2023-05-24 00:33:46.713196 progress_runner-0.0.1/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-24 00:33:46.621315 progress_runner-0.0.1/progress_runner/
--rwxrwxrwx   0 root         (0) root         (0)       13 2023-05-24 00:30:47.000000 progress_runner-0.0.1/progress_runner/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4592 2023-05-24 00:29:50.000000 progress_runner-0.0.1/progress_runner/progress_runner.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-24 00:33:46.696744 progress_runner-0.0.1/progress_runner.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      729 2023-05-24 00:33:46.000000 progress_runner-0.0.1/progress_runner.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      269 2023-05-24 00:33:46.000000 progress_runner-0.0.1/progress_runner.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-24 00:33:46.000000 progress_runner-0.0.1/progress_runner.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       74 2023-05-24 00:33:46.000000 progress_runner-0.0.1/progress_runner.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       16 2023-05-24 00:33:46.000000 progress_runner-0.0.1/progress_runner.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-24 00:33:46.716333 progress_runner-0.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3817 2023-05-24 00:33:14.000000 progress_runner-0.0.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-24 00:42:31.392889 progress_runner-0.0.2/
+-rwxrwxrwx   0 root         (0) root         (0)     1970 2023-05-24 00:42:31.389883 progress_runner-0.0.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      855 2023-05-24 00:41:41.000000 progress_runner-0.0.2/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-24 00:42:31.291149 progress_runner-0.0.2/progress_runner/
+-rwxrwxrwx   0 root         (0) root         (0)       13 2023-05-24 00:30:47.000000 progress_runner-0.0.2/progress_runner/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4592 2023-05-24 00:29:50.000000 progress_runner-0.0.2/progress_runner/progress_runner.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-24 00:42:31.373497 progress_runner-0.0.2/progress_runner.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1970 2023-05-24 00:42:31.000000 progress_runner-0.0.2/progress_runner.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      279 2023-05-24 00:42:31.000000 progress_runner-0.0.2/progress_runner.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-24 00:42:31.000000 progress_runner-0.0.2/progress_runner.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       74 2023-05-24 00:42:31.000000 progress_runner-0.0.2/progress_runner.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       16 2023-05-24 00:42:31.000000 progress_runner-0.0.2/progress_runner.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-24 00:42:31.393053 progress_runner-0.0.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3817 2023-05-24 00:42:07.000000 progress_runner-0.0.2/setup.py
```

### Comparing `progress_runner-0.0.1/progress_runner/progress_runner.py` & `progress_runner-0.0.2/progress_runner/progress_runner.py`

 * *Files identical despite different names*

### Comparing `progress_runner-0.0.1/setup.py` & `progress_runner-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'progress_runner'
 DESCRIPTION = 'an ncurses process runner with progress display'
 URL = 'https://github.com/danroblewis/progress_runner'
 EMAIL = 'daniel.robert.lewis@gmail.com'
 AUTHOR = 'Daniel Lewis'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
 ]
 
 # What packages are optional?
 EXTRAS = {
```

