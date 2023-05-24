# Comparing `tmp/nonebot-plugin-herocard-1.0.0.tar.gz` & `tmp/nonebot_plugin_herocard-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-herocard-1.0.0.tar", last modified: Wed May 24 05:41:09 2023, max compression
+gzip compressed data, was "nonebot_plugin_herocard-1.0.1.tar", last modified: Wed May 24 07:12:09 2023, max compression
```

## Comparing `nonebot-plugin-herocard-1.0.0.tar` & `nonebot_plugin_herocard-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 05:41:09.364409 nonebot-plugin-herocard-1.0.0/
--rw-rw-rw-   0        0        0      504 2023-05-24 05:41:09.347725 nonebot-plugin-herocard-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       94 2023-05-24 05:39:04.000000 nonebot-plugin-herocard-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 05:41:09.188723 nonebot-plugin-herocard-1.0.0/nonebot_plugin_herocard/
--rw-rw-rw-   0        0        0     2704 2023-05-24 05:34:54.000000 nonebot-plugin-herocard-1.0.0/nonebot_plugin_herocard/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 05:41:09.310705 nonebot-plugin-herocard-1.0.0/nonebot_plugin_herocard.egg-info/
--rw-rw-rw-   0        0        0      504 2023-05-24 05:41:08.000000 nonebot-plugin-herocard-1.0.0/nonebot_plugin_herocard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-05-24 05:41:09.000000 nonebot-plugin-herocard-1.0.0/nonebot_plugin_herocard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 05:41:09.000000 nonebot-plugin-herocard-1.0.0/nonebot_plugin_herocard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-24 05:41:09.000000 nonebot-plugin-herocard-1.0.0/nonebot_plugin_herocard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 05:41:09.365409 nonebot-plugin-herocard-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1131 2023-05-24 05:30:02.000000 nonebot-plugin-herocard-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:12:09.902664 nonebot_plugin_herocard-1.0.1/
+-rw-rw-rw-   0        0        0     2131 2023-05-24 07:12:09.899677 nonebot_plugin_herocard-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1683 2023-05-24 07:02:47.000000 nonebot_plugin_herocard-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 07:12:09.778216 nonebot_plugin_herocard-1.0.1/nonebot_plugin_herocard/
+-rw-rw-rw-   0        0        0     2704 2023-05-24 05:34:54.000000 nonebot_plugin_herocard-1.0.1/nonebot_plugin_herocard/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:12:09.858780 nonebot_plugin_herocard-1.0.1/nonebot_plugin_herocard.egg-info/
+-rw-rw-rw-   0        0        0     2131 2023-05-24 07:12:09.000000 nonebot_plugin_herocard-1.0.1/nonebot_plugin_herocard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-05-24 07:12:09.000000 nonebot_plugin_herocard-1.0.1/nonebot_plugin_herocard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 07:12:09.000000 nonebot_plugin_herocard-1.0.1/nonebot_plugin_herocard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-24 07:12:09.000000 nonebot_plugin_herocard-1.0.1/nonebot_plugin_herocard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 07:12:09.902664 nonebot_plugin_herocard-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1137 2023-05-24 07:07:07.000000 nonebot_plugin_herocard-1.0.1/setup.py
```

### Comparing `nonebot-plugin-herocard-1.0.0/nonebot_plugin_herocard/__init__.py` & `nonebot_plugin_herocard-1.0.1/nonebot_plugin_herocard/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-herocard-1.0.0/setup.py` & `nonebot_plugin_herocard-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 # these things are needed for the README.md show on pypi (if you dont need delete it)
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 # you need to change all these
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'nonebot小插件，提供简单的文本提取功能'
-LONG_DESCRIPTION = 'nonebot插件【herocard】，用于提取含“平假名/片假名”文本中的关键文本，用途详见README.md'
+LONG_DESCRIPTION = 'nonebot插件【herocard】，用于提取含“平假名/片假名”文本中的关键文本，使用方法详见README.md'
 
 setup(
-    name="nonebot-plugin-herocard",
+    name="nonebot_plugin_herocard",
     version=VERSION,
     author="Xie-Tiao",
     author_email="1183004468@qq.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

