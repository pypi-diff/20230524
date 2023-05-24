# Comparing `tmp/m3-core-3.1.8.tar.gz` & `tmp/m3-core-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/m3-core-3.1.8.tar", last modified: Tue Feb  2 07:22:11 2021, max compression
+gzip compressed data, was "dist/m3-core-3.1.9.tar", last modified: Fri Feb 26 10:23:29 2021, max compression
```

## Comparing `m3-core-3.1.8.tar` & `m3-core-3.1.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 babay     (1000) babay     (1000)        0 2021-02-02 07:22:11.546356 m3-core-3.1.8/
--rw-rw-r--   0 babay     (1000) babay     (1000)       48 2021-02-02 07:17:22.000000 m3-core-3.1.8/DESCRIPTION.md
--rw-rw-r--   0 babay     (1000) babay     (1000)       77 2021-02-02 07:19:57.000000 m3-core-3.1.8/MANIFEST.in
--rw-rw-r--   0 babay     (1000) babay     (1000)     3390 2021-02-02 07:22:11.542356 m3-core-3.1.8/PKG-INFO
--rw-rw-r--   0 babay     (1000) babay     (1000)     2621 2021-02-02 07:19:57.000000 m3-core-3.1.8/README.md
--rw-rw-r--   0 babay     (1000) babay     (1000)        2 2021-02-02 07:19:57.000000 m3-core-3.1.8/REQUIREMENTS
--rw-rw-r--   0 babay     (1000) babay     (1000)       38 2021-02-02 07:22:11.546356 m3-core-3.1.8/setup.cfg
--rw-rw-r--   0 babay     (1000) babay     (1000)     1276 2021-02-02 07:19:57.000000 m3-core-3.1.8/setup.py
-drwxrwxr-x   0 babay     (1000) babay     (1000)        0 2021-02-02 07:22:11.542356 m3-core-3.1.8/src/
-drwxrwxr-x   0 babay     (1000) babay     (1000)        0 2021-02-02 07:22:11.542356 m3-core-3.1.8/src/m3/
--rw-rw-r--   0 babay     (1000) babay     (1000)    13920 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/__init__.py
-drwxrwxr-x   0 babay     (1000) babay     (1000)        0 2021-02-02 07:22:11.542356 m3-core-3.1.8/src/m3/actions/
--rw-rw-r--   0 babay     (1000) babay     (1000)    71675 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/actions/__init__.py
--rw-rw-r--   0 babay     (1000) babay     (1000)    12523 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/actions/async.py
--rw-rw-r--   0 babay     (1000) babay     (1000)    23587 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/actions/context.py
-drwxrwxr-x   0 babay     (1000) babay     (1000)        0 2021-02-02 07:22:11.542356 m3-core-3.1.8/src/m3/actions/dicts/
--rw-rw-r--   0 babay     (1000) babay     (1000)      355 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/actions/dicts/__init__.py
--rw-rw-r--   0 babay     (1000) babay     (1000)    34872 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/actions/dicts/simple.py
--rw-rw-r--   0 babay     (1000) babay     (1000)    46149 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/actions/dicts/tree.py
--rw-rw-r--   0 babay     (1000) babay     (1000)     2388 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/actions/exceptions.py
--rw-rw-r--   0 babay     (1000) babay     (1000)     1933 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/actions/interfaces.py
--rw-rw-r--   0 babay     (1000) babay     (1000)     2228 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/actions/metrics.py
--rw-rw-r--   0 babay     (1000) babay     (1000)    32992 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/actions/packs.py
--rw-rw-r--   0 babay     (1000) babay     (1000)    10089 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/actions/results.py
--rw-rw-r--   0 babay     (1000) babay     (1000)    46032 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/actions/tree_packs.py
--rw-rw-r--   0 babay     (1000) babay     (1000)    11088 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/actions/urls.py
--rw-rw-r--   0 babay     (1000) babay     (1000)    17567 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/actions/utils.py
--rw-rw-r--   0 babay     (1000) babay     (1000)    15951 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/caching.py
-drwxrwxr-x   0 babay     (1000) babay     (1000)        0 2021-02-02 07:22:11.542356 m3-core-3.1.8/src/m3/db/
--rw-rw-r--   0 babay     (1000) babay     (1000)    14804 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/db/__init__.py
--rw-rw-r--   0 babay     (1000) babay     (1000)     3371 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/db/mptt_util.py
--rw-rw-r--   0 babay     (1000) babay     (1000)     4909 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/db/tools.py
--rw-rw-r--   0 babay     (1000) babay     (1000)     4611 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/db/transaction_context.py
--rw-rw-r--   0 babay     (1000) babay     (1000)     2191 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/finders.py
-drwxrwxr-x   0 babay     (1000) babay     (1000)        0 2021-02-02 07:22:11.542356 m3-core-3.1.8/src/m3/management/
--rw-rw-r--   0 babay     (1000) babay     (1000)        0 2021-02-02 07:17:22.000000 m3-core-3.1.8/src/m3/management/__init__.py
-drwxrwxr-x   0 babay     (1000) babay     (1000)        0 2021-02-02 07:22:11.542356 m3-core-3.1.8/src/m3/management/commands/
--rw-rw-r--   0 babay     (1000) babay     (1000)       24 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/management/commands/__init__.py
--rw-rw-r--   0 babay     (1000) babay     (1000)      514 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/management/commands/selftest.py
--rw-rw-r--   0 babay     (1000) babay     (1000)     3448 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/metrics.py
--rw-rw-r--   0 babay     (1000) babay     (1000)    10637 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/plugins.py
-drwxrwxr-x   0 babay     (1000) babay     (1000)        0 2021-02-02 07:22:11.542356 m3-core-3.1.8/src/m3/templatetags/
--rw-rw-r--   0 babay     (1000) babay     (1000)        0 2021-02-02 07:17:22.000000 m3-core-3.1.8/src/m3/templatetags/__init__.py
--rw-rw-r--   0 babay     (1000) babay     (1000)      381 2021-02-02 07:19:57.000000 m3-core-3.1.8/src/m3/templatetags/m3_tags.py
-drwxrwxr-x   0 babay     (1000) babay     (1000)        0 2021-02-02 07:22:11.542356 m3-core-3.1.8/src/m3_core.egg-info/
--rw-rw-r--   0 babay     (1000) babay     (1000)     3390 2021-02-02 07:22:11.000000 m3-core-3.1.8/src/m3_core.egg-info/PKG-INFO
--rw-rw-r--   0 babay     (1000) babay     (1000)      984 2021-02-02 07:22:11.000000 m3-core-3.1.8/src/m3_core.egg-info/SOURCES.txt
--rw-rw-r--   0 babay     (1000) babay     (1000)        1 2021-02-02 07:22:11.000000 m3-core-3.1.8/src/m3_core.egg-info/dependency_links.txt
--rw-rw-r--   0 babay     (1000) babay     (1000)       42 2021-02-02 07:22:11.000000 m3-core-3.1.8/src/m3_core.egg-info/requires.txt
--rw-rw-r--   0 babay     (1000) babay     (1000)        3 2021-02-02 07:22:11.000000 m3-core-3.1.8/src/m3_core.egg-info/top_level.txt
--rw-rw-r--   0 babay     (1000) babay     (1000)      450 2021-02-02 07:22:11.000000 m3-core-3.1.8/version.conf
+drwxrwxr-x   0 babay     (1000) babay     (1000)        0 2021-02-26 10:23:29.055792 m3-core-3.1.9/
+-rw-rw-r--   0 babay     (1000) babay     (1000)       48 2021-02-02 07:17:22.000000 m3-core-3.1.9/DESCRIPTION.md
+-rw-rw-r--   0 babay     (1000) babay     (1000)       77 2021-02-02 07:19:57.000000 m3-core-3.1.9/MANIFEST.in
+-rw-rw-r--   0 babay     (1000) babay     (1000)     3390 2021-02-26 10:23:29.055792 m3-core-3.1.9/PKG-INFO
+-rw-rw-r--   0 babay     (1000) babay     (1000)     2621 2021-02-02 07:19:57.000000 m3-core-3.1.9/README.md
+-rw-rw-r--   0 babay     (1000) babay     (1000)        2 2021-02-02 07:19:57.000000 m3-core-3.1.9/REQUIREMENTS
+-rw-rw-r--   0 babay     (1000) babay     (1000)       38 2021-02-26 10:23:29.055792 m3-core-3.1.9/setup.cfg
+-rw-rw-r--   0 babay     (1000) babay     (1000)     1276 2021-02-02 07:19:57.000000 m3-core-3.1.9/setup.py
+drwxrwxr-x   0 babay     (1000) babay     (1000)        0 2021-02-26 10:23:29.051792 m3-core-3.1.9/src/
+drwxrwxr-x   0 babay     (1000) babay     (1000)        0 2021-02-26 10:23:29.051792 m3-core-3.1.9/src/m3/
+-rw-rw-r--   0 babay     (1000) babay     (1000)    13920 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/__init__.py
+drwxrwxr-x   0 babay     (1000) babay     (1000)        0 2021-02-26 10:23:29.055792 m3-core-3.1.9/src/m3/actions/
+-rw-rw-r--   0 babay     (1000) babay     (1000)    72538 2021-02-26 10:22:05.000000 m3-core-3.1.9/src/m3/actions/__init__.py
+-rw-rw-r--   0 babay     (1000) babay     (1000)    12523 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/actions/async.py
+-rw-rw-r--   0 babay     (1000) babay     (1000)    24559 2021-02-26 10:22:05.000000 m3-core-3.1.9/src/m3/actions/context.py
+drwxrwxr-x   0 babay     (1000) babay     (1000)        0 2021-02-26 10:23:29.055792 m3-core-3.1.9/src/m3/actions/dicts/
+-rw-rw-r--   0 babay     (1000) babay     (1000)      355 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/actions/dicts/__init__.py
+-rw-rw-r--   0 babay     (1000) babay     (1000)    34872 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/actions/dicts/simple.py
+-rw-rw-r--   0 babay     (1000) babay     (1000)    46149 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/actions/dicts/tree.py
+-rw-rw-r--   0 babay     (1000) babay     (1000)     2388 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/actions/exceptions.py
+-rw-rw-r--   0 babay     (1000) babay     (1000)     1933 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/actions/interfaces.py
+-rw-rw-r--   0 babay     (1000) babay     (1000)     2228 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/actions/metrics.py
+-rw-rw-r--   0 babay     (1000) babay     (1000)    32992 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/actions/packs.py
+-rw-rw-r--   0 babay     (1000) babay     (1000)    10089 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/actions/results.py
+-rw-rw-r--   0 babay     (1000) babay     (1000)    46032 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/actions/tree_packs.py
+-rw-rw-r--   0 babay     (1000) babay     (1000)    11088 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/actions/urls.py
+-rw-rw-r--   0 babay     (1000) babay     (1000)    17567 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/actions/utils.py
+-rw-rw-r--   0 babay     (1000) babay     (1000)    15951 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/caching.py
+drwxrwxr-x   0 babay     (1000) babay     (1000)        0 2021-02-26 10:23:29.055792 m3-core-3.1.9/src/m3/db/
+-rw-rw-r--   0 babay     (1000) babay     (1000)    14804 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/db/__init__.py
+-rw-rw-r--   0 babay     (1000) babay     (1000)     3371 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/db/mptt_util.py
+-rw-rw-r--   0 babay     (1000) babay     (1000)     4909 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/db/tools.py
+-rw-rw-r--   0 babay     (1000) babay     (1000)     4611 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/db/transaction_context.py
+-rw-rw-r--   0 babay     (1000) babay     (1000)     2191 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/finders.py
+drwxrwxr-x   0 babay     (1000) babay     (1000)        0 2021-02-26 10:23:29.055792 m3-core-3.1.9/src/m3/management/
+-rw-rw-r--   0 babay     (1000) babay     (1000)        0 2021-02-02 07:17:22.000000 m3-core-3.1.9/src/m3/management/__init__.py
+drwxrwxr-x   0 babay     (1000) babay     (1000)        0 2021-02-26 10:23:29.055792 m3-core-3.1.9/src/m3/management/commands/
+-rw-rw-r--   0 babay     (1000) babay     (1000)       24 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/management/commands/__init__.py
+-rw-rw-r--   0 babay     (1000) babay     (1000)      514 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/management/commands/selftest.py
+-rw-rw-r--   0 babay     (1000) babay     (1000)     3448 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/metrics.py
+-rw-rw-r--   0 babay     (1000) babay     (1000)    10637 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/plugins.py
+drwxrwxr-x   0 babay     (1000) babay     (1000)        0 2021-02-26 10:23:29.055792 m3-core-3.1.9/src/m3/templatetags/
+-rw-rw-r--   0 babay     (1000) babay     (1000)        0 2021-02-02 07:17:22.000000 m3-core-3.1.9/src/m3/templatetags/__init__.py
+-rw-rw-r--   0 babay     (1000) babay     (1000)      381 2021-02-02 07:19:57.000000 m3-core-3.1.9/src/m3/templatetags/m3_tags.py
+drwxrwxr-x   0 babay     (1000) babay     (1000)        0 2021-02-26 10:23:29.055792 m3-core-3.1.9/src/m3_core.egg-info/
+-rw-rw-r--   0 babay     (1000) babay     (1000)     3390 2021-02-26 10:23:28.000000 m3-core-3.1.9/src/m3_core.egg-info/PKG-INFO
+-rw-rw-r--   0 babay     (1000) babay     (1000)      984 2021-02-26 10:23:28.000000 m3-core-3.1.9/src/m3_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 babay     (1000) babay     (1000)        1 2021-02-26 10:23:28.000000 m3-core-3.1.9/src/m3_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 babay     (1000) babay     (1000)       42 2021-02-26 10:23:28.000000 m3-core-3.1.9/src/m3_core.egg-info/requires.txt
+-rw-rw-r--   0 babay     (1000) babay     (1000)        3 2021-02-26 10:23:28.000000 m3-core-3.1.9/src/m3_core.egg-info/top_level.txt
+-rw-rw-r--   0 babay     (1000) babay     (1000)      450 2021-02-26 10:23:28.000000 m3-core-3.1.9/version.conf
```

### Comparing `m3-core-3.1.8/PKG-INFO` & `m3-core-3.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m3-core
-Version: 3.1.8
+Version: 3.1.9
 Summary: ## M3-Core  Ядро платформы **M3**  
 Home-page: https://github.com/barsgroup/m3-core
 Author: BARS Group
 Author-email: bars@bars-open.ru
 License: MIT
 Description: [![Build Status](https://travis-ci.org/barsgroup/m3-core.svg?branch=3.x)](https://travis-ci.org/barsgroup/m3-core)
         ## M3-Core
```

### Comparing `m3-core-3.1.8/README.md` & `m3-core-3.1.9/README.md`

 * *Files identical despite different names*

### Comparing `m3-core-3.1.8/setup.py` & `m3-core-3.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `m3-core-3.1.8/src/m3/__init__.py` & `m3-core-3.1.9/src/m3/__init__.py`

 * *Files identical despite different names*

### Comparing `m3-core-3.1.8/src/m3/actions/__init__.py` & `m3-core-3.1.9/src/m3/actions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 from .context import (
     ActionContext,
     ActionContextDeclaration,
     DeclarativeActionContext,
     RequiredFailed,
     ContextBuildingError,
     CriticalContextBuildingError,
+    convert_dac_to_acd,
 )
 from .metrics import create_statsd_client
 from . import utils
 import six
 from six.moves import map
 
 _STATSD_CLIENT = create_statsd_client(settings)
@@ -547,14 +548,36 @@
         :return: описание необходимости наличия определенных параметров
             в запросе
         :rtype: list of m3_core.actions.context.ActionContextDeclaration либо
             m3_core.actions.context.DeclarativeActionContext
         """
         pass
 
+    def get_acd_with_ccd(self):
+        """
+        Возвращает набор правил ACD или декларативное описание
+        вместе с контекстом контроллера
+        :return: [ACD] или DAC
+        """
+        acd = self.context_declaration()
+        ccd = self.controller.get_ccd()
+        if acd and ccd:
+            if DeclarativeActionContext.matches(acd):
+                acd = convert_dac_to_acd(acd)
+
+            if DeclarativeActionContext.matches(ccd):
+                ccd = convert_dac_to_acd(ccd)
+
+            if isinstance(acd, tuple):
+                acd = list(acd)
+
+            acd.extend(ccd)
+
+        return acd or ccd
+
     def run(self, request, context):
         """
         Обеспечивает непосредственное исполнение запроса
         (аналог views в Django).
         Обязательно должен быть перекрыт в наследнике.
 
         :param request: запрос
@@ -1443,14 +1466,20 @@
         url = self.url
         if url.startswith('/'):
             url = url[1:]
         if url.endswith('/'):
             url = url[:-2]
         return (r'^%s/' % url, self.process_request)
 
+    def get_ccd(self):
+        """
+        Контекст контроллера
+        """
+        pass
+
 
 class ControllerCache(object):
     '''
     Внутренний класс платформы,
     который отвечает за хранение кеша контроллеров
     и связанных с ним экшенов и паков.
     '''
```

### Comparing `m3-core-3.1.8/src/m3/actions/async.py` & `m3-core-3.1.9/src/m3/actions/async.py`

 * *Files identical despite different names*

### Comparing `m3-core-3.1.8/src/m3/actions/context.py` & `m3-core-3.1.9/src/m3/actions/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from __future__ import (
     absolute_import,
 )
 
 import ast
 import datetime
 import json
+import re
+
 import six
 
 from abc import (
     ABCMeta,
     abstractmethod,
 )
 from decimal import (
@@ -328,16 +330,32 @@
         self,
         raw_value,
     ):
         """
         Пасинг сырой строки для выделения первичного ключа и приведения его к
         указанному в моделе типу
         """
+        raw_value = self._parse_obj_id(raw_value)
+
         return self._model._meta.pk.to_python(raw_value)
 
+    def _parse_obj_id(self, raw_value):
+        """
+        Преобразовывает raw_value если в конекст значение ид модели пришло
+        в виде '{1}'.
+
+        TODO: BOBUH-17847
+              Метод нужно удалить в рамках задачи по исправлению рендера контекста
+        """
+        found_id = re.findall(r'^{(\d+)}$', raw_value)
+        if found_id:
+            raw_value = found_id[0]
+
+        return raw_value
+
 
 class ModelMultiplePKType(AbstractModelPKType):
     """
     Парсер списка первичных ключей с приведением к типу, указанному в моделе
     """
 
     def _parse(
@@ -674,7 +692,19 @@
         :rtype: boolean
         """
         return isinstance(data, dict) or (
             isinstance(data, tuple) and
             len(data) == 2 and
             isinstance(data[0], six.string_types)
         )
+
+
+def convert_dac_to_acd(dac):
+    """
+    Преобразовывает декларативное описание контекста в набор ACD
+    :param dac: словарь описания DeclarativeActionContext
+    :return: Набор правил ACD
+    """
+    return [
+        ActionContextDeclaration(name=name, **rules)
+        for name, rules in dac.items()
+    ]
```

### Comparing `m3-core-3.1.8/src/m3/actions/dicts/simple.py` & `m3-core-3.1.9/src/m3/actions/dicts/simple.py`

 * *Files identical despite different names*

### Comparing `m3-core-3.1.8/src/m3/actions/dicts/tree.py` & `m3-core-3.1.9/src/m3/actions/dicts/tree.py`

 * *Files identical despite different names*

### Comparing `m3-core-3.1.8/src/m3/actions/exceptions.py` & `m3-core-3.1.9/src/m3/actions/exceptions.py`

 * *Files identical despite different names*

### Comparing `m3-core-3.1.8/src/m3/actions/interfaces.py` & `m3-core-3.1.9/src/m3/actions/interfaces.py`

 * *Files identical despite different names*

### Comparing `m3-core-3.1.8/src/m3/actions/metrics.py` & `m3-core-3.1.9/src/m3/actions/metrics.py`

 * *Files identical despite different names*

### Comparing `m3-core-3.1.8/src/m3/actions/packs.py` & `m3-core-3.1.9/src/m3/actions/packs.py`

 * *Files identical despite different names*

### Comparing `m3-core-3.1.8/src/m3/actions/results.py` & `m3-core-3.1.9/src/m3/actions/results.py`

 * *Files identical despite different names*

### Comparing `m3-core-3.1.8/src/m3/actions/tree_packs.py` & `m3-core-3.1.9/src/m3/actions/tree_packs.py`

 * *Files identical despite different names*

### Comparing `m3-core-3.1.8/src/m3/actions/urls.py` & `m3-core-3.1.9/src/m3/actions/urls.py`

 * *Files identical despite different names*

### Comparing `m3-core-3.1.8/src/m3/actions/utils.py` & `m3-core-3.1.9/src/m3/actions/utils.py`

 * *Files identical despite different names*

### Comparing `m3-core-3.1.8/src/m3/caching.py` & `m3-core-3.1.9/src/m3/caching.py`

 * *Files identical despite different names*

### Comparing `m3-core-3.1.8/src/m3/db/__init__.py` & `m3-core-3.1.9/src/m3/db/__init__.py`

 * *Files identical despite different names*

### Comparing `m3-core-3.1.8/src/m3/db/mptt_util.py` & `m3-core-3.1.9/src/m3/db/mptt_util.py`

 * *Files identical despite different names*

### Comparing `m3-core-3.1.8/src/m3/db/tools.py` & `m3-core-3.1.9/src/m3/db/tools.py`

 * *Files identical despite different names*

### Comparing `m3-core-3.1.8/src/m3/db/transaction_context.py` & `m3-core-3.1.9/src/m3/db/transaction_context.py`

 * *Files identical despite different names*

### Comparing `m3-core-3.1.8/src/m3/finders.py` & `m3-core-3.1.9/src/m3/finders.py`

 * *Files identical despite different names*

### Comparing `m3-core-3.1.8/src/m3/management/commands/selftest.py` & `m3-core-3.1.9/src/m3/management/commands/selftest.py`

 * *Files identical despite different names*

### Comparing `m3-core-3.1.8/src/m3/metrics.py` & `m3-core-3.1.9/src/m3/metrics.py`

 * *Files identical despite different names*

### Comparing `m3-core-3.1.8/src/m3/plugins.py` & `m3-core-3.1.9/src/m3/plugins.py`

 * *Files identical despite different names*

### Comparing `m3-core-3.1.8/src/m3_core.egg-info/PKG-INFO` & `m3-core-3.1.9/src/m3_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m3-core
-Version: 3.1.8
+Version: 3.1.9
 Summary: ## M3-Core  Ядро платформы **M3**  
 Home-page: https://github.com/barsgroup/m3-core
 Author: BARS Group
 Author-email: bars@bars-open.ru
 License: MIT
 Description: [![Build Status](https://travis-ci.org/barsgroup/m3-core.svg?branch=3.x)](https://travis-ci.org/barsgroup/m3-core)
         ## M3-Core
```

### Comparing `m3-core-3.1.8/src/m3_core.egg-info/SOURCES.txt` & `m3-core-3.1.9/src/m3_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

