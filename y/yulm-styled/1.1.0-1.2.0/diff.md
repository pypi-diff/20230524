# Comparing `tmp/yulm-styled-1.1.0.tar.gz` & `tmp/yulm-styled-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yulm-styled-1.1.0.tar", last modified: Wed May 24 06:44:10 2023, max compression
+gzip compressed data, was "yulm-styled-1.2.0.tar", last modified: Wed May 24 07:33:55 2023, max compression
```

## Comparing `yulm-styled-1.1.0.tar` & `yulm-styled-1.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-24 06:44:10.031018 yulm-styled-1.1.0/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3325 2023-05-24 06:44:10.031018 yulm-styled-1.1.0/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2778 2023-05-24 06:37:39.000000 yulm-styled-1.1.0/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-24 06:44:10.031018 yulm-styled-1.1.0/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      719 2023-05-24 06:41:22.000000 yulm-styled-1.1.0/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-24 06:44:10.031018 yulm-styled-1.1.0/yulm_styled.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3325 2023-05-24 06:44:09.000000 yulm-styled-1.1.0/yulm_styled.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      158 2023-05-24 06:44:09.000000 yulm-styled-1.1.0/yulm_styled.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-24 06:44:09.000000 yulm-styled-1.1.0/yulm_styled.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-24 06:44:09.000000 yulm-styled-1.1.0/yulm_styled.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-24 07:33:55.340101 yulm-styled-1.2.0/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2542 2023-05-24 07:33:55.340101 yulm-styled-1.2.0/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1995 2023-05-24 07:32:06.000000 yulm-styled-1.2.0/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-24 07:33:55.340101 yulm-styled-1.2.0/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      719 2023-05-24 07:33:43.000000 yulm-styled-1.2.0/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-24 07:33:55.340101 yulm-styled-1.2.0/yulm_styled.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2542 2023-05-24 07:33:55.000000 yulm-styled-1.2.0/yulm_styled.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      158 2023-05-24 07:33:55.000000 yulm-styled-1.2.0/yulm_styled.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-24 07:33:55.000000 yulm-styled-1.2.0/yulm_styled.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-24 07:33:55.000000 yulm-styled-1.2.0/yulm_styled.egg-info/top_level.txt
```

### Comparing `yulm-styled-1.1.0/setup.py` & `yulm-styled-1.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='yulm-styled',
-    version='1.1.0',
+    version='1.2.0',
     author='LopeKinz',
     author_email='pinkyhax@gmail.com',
     description='A package for colorizing and styling text',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/lopekinz/yulm-styled',
     packages=find_packages(),
```

