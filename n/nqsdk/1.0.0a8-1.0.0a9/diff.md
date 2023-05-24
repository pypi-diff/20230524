# Comparing `tmp/nqsdk-1.0.0a8.tar.gz` & `tmp/nqsdk-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nqsdk-1.0.0a8.tar", last modified: Sun Nov 13 14:38:48 2022, max compression
+gzip compressed data, was "nqsdk-1.0.0a9.tar", last modified: Tue Nov 22 10:10:12 2022, max compression
```

## Comparing `nqsdk-1.0.0a8.tar` & `nqsdk-1.0.0a9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 14:38:48.515699 nqsdk-1.0.0a8/
--rw-rw-rw-   0 root         (0) root         (0)      556 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       89 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2070 2022-11-13 14:38:48.515699 nqsdk-1.0.0a8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1621 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 14:38:48.515699 nqsdk-1.0.0a8/nqsdk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/nqsdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 14:38:48.515699 nqsdk-1.0.0a8/nqsdk/abstract/
--rw-rw-rw-   0 root         (0) root         (0)      620 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/nqsdk/abstract/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1434 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/nqsdk/abstract/channel.py
--rw-rw-rw-   0 root         (0) root         (0)     2478 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/nqsdk/abstract/message.py
--rw-rw-rw-   0 root         (0) root         (0)     7168 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/nqsdk/abstract/provider.py
--rw-rw-rw-   0 root         (0) root         (0)     2868 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/nqsdk/abstract/quotas.py
--rw-rw-rw-   0 root         (0) root         (0)     1728 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/nqsdk/callback.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 14:38:48.515699 nqsdk-1.0.0a8/nqsdk/dummy/
--rw-rw-rw-   0 root         (0) root         (0)      609 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/nqsdk/dummy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1720 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/nqsdk/dummy/message.py
--rw-rw-rw-   0 root         (0) root         (0)     6012 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/nqsdk/dummy/provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/nqsdk/dummy/quotas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 14:38:48.515699 nqsdk-1.0.0a8/nqsdk/dummy/resources/
--rw-rw-rw-   0 root         (0) root         (0)     1054 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/nqsdk/dummy/resources/config_schema.json
--rw-rw-rw-   0 root         (0) root         (0)     1071 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/nqsdk/enums.py
--rw-rw-rw-   0 root         (0) root         (0)     1731 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/nqsdk/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/nqsdk/mixins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 14:38:48.515699 nqsdk-1.0.0a8/nqsdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2070 2022-11-13 14:38:48.000000 nqsdk-1.0.0a8/nqsdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      675 2022-11-13 14:38:48.000000 nqsdk-1.0.0a8/nqsdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-13 14:38:48.000000 nqsdk-1.0.0a8/nqsdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2022-11-13 14:38:48.000000 nqsdk-1.0.0a8/nqsdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-11-13 14:38:48.000000 nqsdk-1.0.0a8/nqsdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-13 14:38:48.000000 nqsdk-1.0.0a8/nqsdk.egg-info/zip-safe
--rw-rw-rw-   0 root         (0) root         (0)     1425 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-13 14:38:48.515699 nqsdk-1.0.0a8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 14:38:48.515699 nqsdk-1.0.0a8/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      824 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     1960 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/tests/factories.py
--rw-rw-rw-   0 root         (0) root         (0)     3066 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/tests/test_dummy_config.py
--rw-rw-rw-   0 root         (0) root         (0)     6607 2022-11-13 14:38:31.000000 nqsdk-1.0.0a8/tests/test_dummy_requests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 10:10:12.630125 nqsdk-1.0.0a9/
+-rw-rw-rw-   0 root         (0) root         (0)      556 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       89 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2070 2022-11-22 10:10:12.630125 nqsdk-1.0.0a9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1621 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 10:10:12.626125 nqsdk-1.0.0a9/nqsdk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/nqsdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 10:10:12.626125 nqsdk-1.0.0a9/nqsdk/abstract/
+-rw-rw-rw-   0 root         (0) root         (0)      620 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/nqsdk/abstract/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1434 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/nqsdk/abstract/channel.py
+-rw-rw-rw-   0 root         (0) root         (0)     2478 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/nqsdk/abstract/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     7168 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/nqsdk/abstract/provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     2868 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/nqsdk/abstract/quotas.py
+-rw-rw-rw-   0 root         (0) root         (0)     1728 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/nqsdk/callback.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 10:10:12.626125 nqsdk-1.0.0a9/nqsdk/dummy/
+-rw-rw-rw-   0 root         (0) root         (0)      609 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/nqsdk/dummy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1720 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/nqsdk/dummy/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     6008 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/nqsdk/dummy/provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/nqsdk/dummy/quotas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 10:10:12.626125 nqsdk-1.0.0a9/nqsdk/dummy/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     1054 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/nqsdk/dummy/resources/config_schema.json
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/nqsdk/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/nqsdk/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/nqsdk/mixins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 10:10:12.626125 nqsdk-1.0.0a9/nqsdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2070 2022-11-22 10:10:12.000000 nqsdk-1.0.0a9/nqsdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      675 2022-11-22 10:10:12.000000 nqsdk-1.0.0a9/nqsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 10:10:12.000000 nqsdk-1.0.0a9/nqsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2022-11-22 10:10:12.000000 nqsdk-1.0.0a9/nqsdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-11-22 10:10:12.000000 nqsdk-1.0.0a9/nqsdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 10:10:12.000000 nqsdk-1.0.0a9/nqsdk.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)     1425 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-11-22 10:10:12.630125 nqsdk-1.0.0a9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 10:10:12.630125 nqsdk-1.0.0a9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      824 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1960 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/tests/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)     3066 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/tests/test_dummy_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     6607 2022-11-22 10:09:53.000000 nqsdk-1.0.0a9/tests/test_dummy_requests.py
```

### Comparing `nqsdk-1.0.0a8/LICENSE` & `nqsdk-1.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `nqsdk-1.0.0a8/PKG-INFO` & `nqsdk-1.0.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nqsdk
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: NQ SDK
 Author-email: "Inqana Ltd." <develop@inqana.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `nqsdk-1.0.0a8/README.md` & `nqsdk-1.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `nqsdk-1.0.0a8/nqsdk/abstract/__init__.py` & `nqsdk-1.0.0a9/nqsdk/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `nqsdk-1.0.0a8/nqsdk/abstract/channel.py` & `nqsdk-1.0.0a9/nqsdk/abstract/channel.py`

 * *Files identical despite different names*

### Comparing `nqsdk-1.0.0a8/nqsdk/abstract/message.py` & `nqsdk-1.0.0a9/nqsdk/abstract/message.py`

 * *Files identical despite different names*

### Comparing `nqsdk-1.0.0a8/nqsdk/abstract/provider.py` & `nqsdk-1.0.0a9/nqsdk/abstract/provider.py`

 * *Files identical despite different names*

### Comparing `nqsdk-1.0.0a8/nqsdk/abstract/quotas.py` & `nqsdk-1.0.0a9/nqsdk/abstract/quotas.py`

 * *Files identical despite different names*

### Comparing `nqsdk-1.0.0a8/nqsdk/callback.py` & `nqsdk-1.0.0a9/nqsdk/callback.py`

 * *Files identical despite different names*

### Comparing `nqsdk-1.0.0a8/nqsdk/dummy/__init__.py` & `nqsdk-1.0.0a9/nqsdk/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `nqsdk-1.0.0a8/nqsdk/dummy/message.py` & `nqsdk-1.0.0a9/nqsdk/dummy/message.py`

 * *Files identical despite different names*

### Comparing `nqsdk-1.0.0a8/nqsdk/dummy/provider.py` & `nqsdk-1.0.0a9/nqsdk/dummy/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,24 +34,24 @@
     AckHandleMixin,
     BalanceCheckMixin,
     DeliveryCheckMixin,
     DeliveryHandleMixin,
     HealthCheckMixin,
     Provider,
 )
+from nqsdk.callback import CallbackResponse
 from nqsdk.enums import CallbackStatus, CallbackUrl
 from .message import DummyAckMeta, DummyDeliveredMeta, DummySentMeta
 from .quotas import PerHourQuota, PerSecondQuota
 
 if TYPE_CHECKING:  # pragma: no cover
     from rest_framework.request import Request
 
     from nqsdk.abstract.message import AckMeta, DeliveredMeta, Message, SentMeta
     from nqsdk.abstract.quotas import ProviderQuota
-    from nqsdk.callback import CallbackResponse
 
 
 class DummyProvider(
     BalanceCheckMixin,
     HealthCheckMixin,
     DeliveryCheckMixin,
     AckCheckMixin,
```

### Comparing `nqsdk-1.0.0a8/nqsdk/dummy/quotas.py` & `nqsdk-1.0.0a9/nqsdk/dummy/quotas.py`

 * *Files identical despite different names*

### Comparing `nqsdk-1.0.0a8/nqsdk/dummy/resources/config_schema.json` & `nqsdk-1.0.0a9/nqsdk/dummy/resources/config_schema.json`

 * *Files identical despite different names*

### Comparing `nqsdk-1.0.0a8/nqsdk/enums.py` & `nqsdk-1.0.0a9/nqsdk/enums.py`

 * *Files identical despite different names*

### Comparing `nqsdk-1.0.0a8/nqsdk/exceptions.py` & `nqsdk-1.0.0a9/nqsdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `nqsdk-1.0.0a8/nqsdk/mixins.py` & `nqsdk-1.0.0a9/nqsdk/mixins.py`

 * *Files identical despite different names*

### Comparing `nqsdk-1.0.0a8/nqsdk.egg-info/PKG-INFO` & `nqsdk-1.0.0a9/nqsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nqsdk
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: NQ SDK
 Author-email: "Inqana Ltd." <develop@inqana.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `nqsdk-1.0.0a8/nqsdk.egg-info/SOURCES.txt` & `nqsdk-1.0.0a9/nqsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nqsdk-1.0.0a8/pyproject.toml` & `nqsdk-1.0.0a9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nqsdk"
-version = "1.0.0-alpha-8"
+version = "1.0.0-alpha-9"
 authors = [
   {name="Inqana Ltd.", email="develop@inqana.com"},
 ]
 description = "NQ SDK"
 readme = "README.md"
 requires-python = ">= 3.10"
 dependencies = [
```

### Comparing `nqsdk-1.0.0a8/tests/conftest.py` & `nqsdk-1.0.0a9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nqsdk-1.0.0a8/tests/factories.py` & `nqsdk-1.0.0a9/tests/factories.py`

 * *Files identical despite different names*

### Comparing `nqsdk-1.0.0a8/tests/test_dummy_config.py` & `nqsdk-1.0.0a9/tests/test_dummy_config.py`

 * *Files identical despite different names*

### Comparing `nqsdk-1.0.0a8/tests/test_dummy_requests.py` & `nqsdk-1.0.0a9/tests/test_dummy_requests.py`

 * *Files identical despite different names*

