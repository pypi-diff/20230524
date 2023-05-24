# Comparing `tmp/data-spec-validator-3.0.1.tar.gz` & `tmp/data-spec-validator-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/data-spec-validator-3.0.1.tar", last modified: Wed Mar  1 08:33:17 2023, max compression
+gzip compressed data, was "dist/data-spec-validator-3.1.0.tar", last modified: Wed May 24 06:13:10 2023, max compression
```

## Comparing `data-spec-validator-3.0.1.tar` & `data-spec-validator-3.1.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-03-01 08:33:17.000000 data-spec-validator-3.0.1/
--rw-r--r--   0 kilikkuo   (501) staff       (20)    13902 2023-03-01 08:33:17.000000 data-spec-validator-3.0.1/PKG-INFO
-drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-03-01 08:33:17.000000 data-spec-validator-3.0.1/test/
--rw-r--r--   0 kilikkuo   (501) staff       (20)     1813 2023-02-23 07:51:32.000000 data-spec-validator-3.0.1/test/test_nested_spec.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     4764 2023-03-01 07:50:37.000000 data-spec-validator-3.0.1/test/test_class_type_spec.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)    58443 2023-03-01 07:50:37.000000 data-spec-validator-3.0.1/test/test_spec.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)        0 2022-05-22 06:41:36.000000 data-spec-validator-3.0.1/test/__init__.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)      270 2023-02-23 07:50:57.000000 data-spec-validator-3.0.1/test/utils.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     6848 2023-03-01 08:29:12.000000 data-spec-validator-3.0.1/test/test_decorator.py
-drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-03-01 08:33:17.000000 data-spec-validator-3.0.1/data_spec_validator/
-drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-03-01 08:33:17.000000 data-spec-validator-3.0.1/data_spec_validator/decorator/
--rw-r--r--   0 kilikkuo   (501) staff       (20)       46 2022-05-22 06:41:36.000000 data-spec-validator-3.0.1/data_spec_validator/decorator/__init__.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     5037 2023-03-01 08:29:12.000000 data-spec-validator-3.0.1/data_spec_validator/decorator/decorators.py
-drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-03-01 08:33:17.000000 data-spec-validator-3.0.1/data_spec_validator/spec/
-drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-03-01 08:33:17.000000 data-spec-validator-3.0.1/data_spec_validator/spec/custom_spec/
--rw-r--r--   0 kilikkuo   (501) staff       (20)       30 2022-05-22 06:41:36.000000 data-spec-validator-3.0.1/data_spec_validator/spec/custom_spec/__init__.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)      917 2022-05-22 06:41:36.000000 data-spec-validator-3.0.1/data_spec_validator/spec/custom_spec/defines.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)    18501 2023-03-01 07:50:37.000000 data-spec-validator-3.0.1/data_spec_validator/spec/validators.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     7490 2023-03-01 07:50:37.000000 data-spec-validator-3.0.1/data_spec_validator/spec/checks.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     3408 2023-03-01 07:50:37.000000 data-spec-validator-3.0.1/data_spec_validator/spec/actions.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)      629 2023-03-01 07:50:37.000000 data-spec-validator-3.0.1/data_spec_validator/spec/__init__.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     2101 2023-03-01 07:50:37.000000 data-spec-validator-3.0.1/data_spec_validator/spec/features.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)      168 2022-05-22 06:41:36.000000 data-spec-validator-3.0.1/data_spec_validator/spec/utils.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)      404 2022-05-22 06:41:36.000000 data-spec-validator-3.0.1/data_spec_validator/spec/wrappers.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     2664 2023-03-01 07:50:37.000000 data-spec-validator-3.0.1/data_spec_validator/spec/defines.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)        0 2022-05-22 06:41:36.000000 data-spec-validator-3.0.1/data_spec_validator/__init__.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)       22 2023-03-01 08:29:31.000000 data-spec-validator-3.0.1/data_spec_validator/__version__.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)    10524 2023-03-01 08:14:05.000000 data-spec-validator-3.0.1/README.md
--rw-r--r--   0 kilikkuo   (501) staff       (20)     1217 2022-09-08 00:14:57.000000 data-spec-validator-3.0.1/setup.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)      458 2023-03-01 08:33:17.000000 data-spec-validator-3.0.1/setup.cfg
-drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-03-01 08:33:17.000000 data-spec-validator-3.0.1/data_spec_validator.egg-info/
--rw-r--r--   0 kilikkuo   (501) staff       (20)    13902 2023-03-01 08:33:17.000000 data-spec-validator-3.0.1/data_spec_validator.egg-info/PKG-INFO
--rw-r--r--   0 kilikkuo   (501) staff       (20)      909 2023-03-01 08:33:17.000000 data-spec-validator-3.0.1/data_spec_validator.egg-info/SOURCES.txt
--rw-r--r--   0 kilikkuo   (501) staff       (20)       56 2023-03-01 08:33:17.000000 data-spec-validator-3.0.1/data_spec_validator.egg-info/requires.txt
--rw-r--r--   0 kilikkuo   (501) staff       (20)       25 2023-03-01 08:33:17.000000 data-spec-validator-3.0.1/data_spec_validator.egg-info/top_level.txt
--rw-r--r--   0 kilikkuo   (501) staff       (20)        1 2023-03-01 08:33:17.000000 data-spec-validator-3.0.1/data_spec_validator.egg-info/dependency_links.txt
+drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/
+-rw-r--r--   0 kilikkuo   (501) staff       (20)    14029 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/PKG-INFO
+drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/test/
+-rw-r--r--   0 kilikkuo   (501) staff       (20)     1813 2023-02-23 07:51:32.000000 data-spec-validator-3.1.0/test/test_nested_spec.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)     4764 2023-03-01 07:50:37.000000 data-spec-validator-3.1.0/test/test_class_type_spec.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)     5664 2023-05-24 06:12:07.000000 data-spec-validator-3.1.0/test/test_decorator_drf.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)    58443 2023-03-01 07:50:37.000000 data-spec-validator-3.1.0/test/test_spec.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)        0 2022-05-22 06:41:36.000000 data-spec-validator-3.1.0/test/__init__.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)     1633 2023-05-24 06:12:07.000000 data-spec-validator-3.1.0/test/utils.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)     6290 2023-05-24 06:12:07.000000 data-spec-validator-3.1.0/test/test_decorator_dj.py
+drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/data_spec_validator/
+drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/data_spec_validator/decorator/
+-rw-r--r--   0 kilikkuo   (501) staff       (20)       46 2023-05-24 04:08:19.000000 data-spec-validator-3.1.0/data_spec_validator/decorator/__init__.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)     6567 2023-05-24 06:12:07.000000 data-spec-validator-3.1.0/data_spec_validator/decorator/decorators.py
+drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/data_spec_validator/spec/
+drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/data_spec_validator/spec/custom_spec/
+-rw-r--r--   0 kilikkuo   (501) staff       (20)       30 2022-05-22 06:41:36.000000 data-spec-validator-3.1.0/data_spec_validator/spec/custom_spec/__init__.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)      917 2022-05-22 06:41:36.000000 data-spec-validator-3.1.0/data_spec_validator/spec/custom_spec/defines.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)    18501 2023-03-01 07:50:37.000000 data-spec-validator-3.1.0/data_spec_validator/spec/validators.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)     7490 2023-03-01 07:50:37.000000 data-spec-validator-3.1.0/data_spec_validator/spec/checks.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)     3408 2023-03-01 07:50:37.000000 data-spec-validator-3.1.0/data_spec_validator/spec/actions.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)      629 2023-03-01 07:50:37.000000 data-spec-validator-3.1.0/data_spec_validator/spec/__init__.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)     2101 2023-03-01 07:50:37.000000 data-spec-validator-3.1.0/data_spec_validator/spec/features.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)      168 2022-05-22 06:41:36.000000 data-spec-validator-3.1.0/data_spec_validator/spec/utils.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)      404 2022-05-22 06:41:36.000000 data-spec-validator-3.1.0/data_spec_validator/spec/wrappers.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)     2664 2023-03-01 07:50:37.000000 data-spec-validator-3.1.0/data_spec_validator/spec/defines.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)        0 2022-05-22 06:41:36.000000 data-spec-validator-3.1.0/data_spec_validator/__init__.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)       22 2023-05-24 06:12:07.000000 data-spec-validator-3.1.0/data_spec_validator/__version__.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)    10614 2023-05-24 06:12:07.000000 data-spec-validator-3.1.0/README.md
+-rw-r--r--   0 kilikkuo   (501) staff       (20)     1253 2023-05-24 06:12:07.000000 data-spec-validator-3.1.0/setup.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)      458 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/setup.cfg
+drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/data_spec_validator.egg-info/
+-rw-r--r--   0 kilikkuo   (501) staff       (20)    14029 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/data_spec_validator.egg-info/PKG-INFO
+-rw-r--r--   0 kilikkuo   (501) staff       (20)      939 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/data_spec_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 kilikkuo   (501) staff       (20)       79 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/data_spec_validator.egg-info/requires.txt
+-rw-r--r--   0 kilikkuo   (501) staff       (20)       25 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/data_spec_validator.egg-info/top_level.txt
+-rw-r--r--   0 kilikkuo   (501) staff       (20)        1 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/data_spec_validator.egg-info/dependency_links.txt
```

### Comparing `data-spec-validator-3.0.1/PKG-INFO` & `data-spec-validator-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-spec-validator
-Version: 3.0.1
+Version: 3.1.0
 Summary: Validation tool for API/Function parameters
 Home-page: https://github.com/hardcoretech/data-spec-validator
 Author: GoFreight
 Author-email: pypi@hardcoretech.co
 License: UNKNOWN
 Project-URL: Changelog, https://github.com/hardcoretech/data-spec-validator/blob/develop/CHANGELOG.md
 Description: # data-spec-validator
@@ -39,17 +39,18 @@
         
         ## Installation
         - Basic usage:
         ```shell
         pip install data-spec-validator
         ```
         - Advance usage (decorator)
-          1. The decorator function `dsv` depends on `Django` & `djangorestframework`.
+          1. The decorator function `dsv` may depend on `Django` or `djangorestframework`.
         ```shell
-        pip install data-spec-validator[decorator]
+        pip install data-spec-validator[decorator-dj]  # Django Only
+        pip install data-spec-validator[decorator]  # Django Rest Framework
         ```
         
         ## Quick Example
         * Do `validate_data_spec` directly wherever you like
         ```python
         from data_spec_validator.spec import INT, DIGIT_STR, ONE_OF, Checker, CheckerOP, validate_data_spec
         
@@ -356,7 +357,8 @@
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: decorator
+Provides-Extra: decorator-dj
```

### Comparing `data-spec-validator-3.0.1/test/test_nested_spec.py` & `data-spec-validator-3.1.0/test/test_nested_spec.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.0.1/test/test_class_type_spec.py` & `data-spec-validator-3.1.0/test/test_class_type_spec.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.0.1/test/test_spec.py` & `data-spec-validator-3.1.0/test/test_spec.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.0.1/test/test_decorator.py` & `data-spec-validator-3.1.0/test/test_decorator_drf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,84 +1,45 @@
 import itertools
 import unittest
-from io import StringIO
 from unittest.mock import patch
 
-from django.conf import settings
 from parameterized import parameterized
-from rest_framework.request import clone_request, override_method
 
 from data_spec_validator.decorator import dsv, dsv_request_meta
 from data_spec_validator.spec import DIGIT_STR, LIST_OF, ONE_OF, STR, Checker, dsv_feature
 
-settings.configure()
+from .utils import is_drf_installed, make_request
 
 try:
-    from django.core.handlers.wsgi import WSGIRequest
+    from django.conf import settings
     from django.test import RequestFactory
     from django.views import View
     from rest_framework.exceptions import ParseError
-    from rest_framework.parsers import FormParser
-    from rest_framework.request import Request
+    from rest_framework.request import Request, override_method
+
+    settings.configure()
 except Exception:
     # To skip E402 module level import not at top of file
     pass
 
 
-def _make_request(cls, path='/', method='GET', user=None, headers=None, data=None, qs=None):
-    assert cls in [WSGIRequest, Request]
-    kwargs = {'REQUEST_METHOD': method, 'PATH_INFO': path, 'wsgi.input': StringIO()}
-    if qs:
-        kwargs.update({'QUERY_STRING': qs})
-    req = WSGIRequest(kwargs)
-
-    req.user = user
-
-    if headers:
-        req.META.update(headers)
-
-    if data:
-        if method == 'GET':
-            setattr(req, 'GET', data)
-        elif method == 'POST':
-            req.read()  # trigger RawPostDataException and force DRF to load data from req.POST
-            req.META.update(
-                {
-                    'CONTENT_TYPE': 'application/x-www-form-urlencoded',
-                    'CONTENT_LENGTH': len(str(data)),
-                }
-            )
-            req.POST = data
-
-    if cls == Request:
-        return clone_request(cls(req, parsers=[FormParser]), method)
-    return req
-
-
-def _make_django_view_params(req, kwargs=None):
-    class DjangoView(View):
-        request = req
-
-    return (DjangoView(),), kwargs or {}
-
-
-class TestDSV(unittest.TestCase):
+@unittest.skipUnless(is_drf_installed(), 'DRF is not installed')
+class TestDSVDRF(unittest.TestCase):
     def test_should_check_name_url_params(self):
         # arrange
         class _ViewSpec:
             named_arg = Checker([DIGIT_STR])
 
         class _View(View):
             @dsv(_ViewSpec)
             def decorated_func(self, request, named_arg):
                 pass
 
         factory = RequestFactory()
-        req = factory.request()
-        req = Request(req)
+        req = Request(factory.request())
         view = _View()
 
         # action & assert
         view.decorated_func(req, named_arg='1')  # should pass validation
 
         with self.assertRaises(ParseError):
             view.decorated_func(req, named_arg='')
@@ -99,67 +60,69 @@
         req = Request(wsgi_req)
         view = _View()
 
         # action & assert
         with self.assertRaises(RuntimeError):
             view.decorated_func(req, named_arg='')
 
-    @parameterized.expand(itertools.product([dsv, dsv_request_meta], [Request, WSGIRequest], ['GET', 'POST']))
-    def test_data_and_path_named_param_should_combine_together(self, dsv_deco, cls, method):
+    @parameterized.expand(itertools.product([dsv, dsv_request_meta], ['GET', 'POST']))
+    def test_data_and_path_named_param_should_combine_together(self, dsv_deco, method):
         # arrange
         payload = {'test_a': 'TEST A'}
         if dsv_deco == dsv:
-            fake_request = _make_request(cls, method=method, data=payload)
+            fake_request = make_request(Request, method=method, data=payload)
         elif dsv_deco == dsv_request_meta:
-            fake_request = _make_request(cls, method=method, headers=payload)
+            fake_request = make_request(Request, method=method, headers=payload)
+        else:
+            assert False
 
         kwargs = {'test_b': 'TEST_B'}
 
         class _ViewSpec:
             test_a = Checker([ONE_OF], ONE_OF='TEST A')
             test_b = Checker([ONE_OF], ONE_OF='TEST_B')
 
         class _View(View):
             @dsv_deco(_ViewSpec)
-            def decorated_func(self, request, *_args, **_kwargs):
+            def decorated_func(self, req, *_args, **_kwargs):
                 pass
 
         view = _View(request=fake_request)
         view.decorated_func(fake_request, **kwargs)
 
-    @parameterized.expand(itertools.product([Request], ['PUT', 'PATCH', 'DELETE']))
-    def test_query_params_with_data(self, cls, method):
+    @parameterized.expand(['PUT', 'PATCH', 'DELETE'])
+    def test_query_params_with_data(self, method):
         # arrange
         qs = 'q_a=3&q_b=true'
         payload = {'test_a': 'TEST A'}
 
-        fake_request = _make_request(cls, method='POST', data=payload, qs=qs)
+        fake_request = make_request(Request, method='POST', data=payload, qs=qs)
 
         kwargs = {'test_b': 'TEST_B'}
 
         @dsv_feature(strict=True)
         class _ViewSpec:
             q_a = Checker([LIST_OF], LIST_OF=STR)
             q_b = Checker([LIST_OF], LIST_OF=STR)
             test_a = Checker([ONE_OF], ONE_OF='TEST A')
             test_b = Checker([ONE_OF], ONE_OF='TEST_B')
 
         class _View(View):
             @dsv(_ViewSpec)
-            def decorated_func(self, request, *_args, **_kwargs):
+            def decorated_func(self, req, *_args, **_kwargs):
                 pass
 
         view = _View(request=fake_request)
         with override_method(view, fake_request, method) as request:
             view.decorated_func(request, **kwargs)
 
     def test_req_list_data_with_no_multirow_set(self):
         # arrange
         payload = [{'test_a': 'TEST A1'}, {'test_a': 'TEST A2'}, {'test_a': 'TEST A3'}]
-        fake_request = _make_request(Request, method='POST', data=payload)
+        fake_request = make_request(Request, method='POST', data=payload)
         kwargs = {'test_b': 'TEST_B'}
 
         class _ViewSingleRowSpec:
             test_a = Checker([STR])
 
         class _View(View):
             @dsv(_ViewSingleRowSpec)
@@ -168,15 +131,15 @@
 
         view = _View(request=fake_request)
         view.decorated_func(fake_request, **kwargs)
 
     def test_req_list_data_with_multirow_true(self):
         # arrange
         payload = [{'test_a': 'TEST A1'}, {'test_a': 'TEST A2'}, {'test_a': 'TEST A3'}]
-        fake_request = _make_request(WSGIRequest, method='POST', data=payload)
+        fake_request = make_request(Request, method='POST', data=payload)
         kwargs = {'test_b': 'TEST_B'}
 
         class _ViewSingleRowSpec:
             test_a = Checker([STR])
 
         class _View(View):
             @dsv(_ViewSingleRowSpec, multirow=True)
@@ -195,16 +158,15 @@
 
         class _NonView:
             @dsv(_NonViewSpec)
             def decorated_func(self, request, field_a):
                 pass
 
         factory = RequestFactory()
-        req = factory.request()
-        req = Request(req)
+        req = Request(factory.request())
         non_view = _NonView()
 
         # action & assert
         non_view.decorated_func(req, field_a='1')  # should pass validation
 
         fake_args = ['1', '2', 3]
         with self.assertRaises(Exception):
```

### Comparing `data-spec-validator-3.0.1/data_spec_validator/spec/custom_spec/defines.py` & `data-spec-validator-3.1.0/data_spec_validator/spec/custom_spec/defines.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.0.1/data_spec_validator/spec/validators.py` & `data-spec-validator-3.1.0/data_spec_validator/spec/validators.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.0.1/data_spec_validator/spec/checks.py` & `data-spec-validator-3.1.0/data_spec_validator/spec/checks.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.0.1/data_spec_validator/spec/actions.py` & `data-spec-validator-3.1.0/data_spec_validator/spec/actions.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.0.1/data_spec_validator/spec/__init__.py` & `data-spec-validator-3.1.0/data_spec_validator/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.0.1/data_spec_validator/spec/features.py` & `data-spec-validator-3.1.0/data_spec_validator/spec/features.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.0.1/data_spec_validator/spec/defines.py` & `data-spec-validator-3.1.0/data_spec_validator/spec/defines.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.0.1/README.md` & `data-spec-validator-3.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,18 @@
 
 ## Installation
 - Basic usage:
 ```shell
 pip install data-spec-validator
 ```
 - Advance usage (decorator)
-  1. The decorator function `dsv` depends on `Django` & `djangorestframework`.
+  1. The decorator function `dsv` may depend on `Django` or `djangorestframework`.
 ```shell
-pip install data-spec-validator[decorator]
+pip install data-spec-validator[decorator-dj]  # Django Only
+pip install data-spec-validator[decorator]  # Django Rest Framework
 ```
 
 ## Quick Example
 * Do `validate_data_spec` directly wherever you like
 ```python
 from data_spec_validator.spec import INT, DIGIT_STR, ONE_OF, Checker, CheckerOP, validate_data_spec
```

### Comparing `data-spec-validator-3.0.1/setup.py` & `data-spec-validator-3.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,11 +28,12 @@
     package_dir={"data_spec_validator": "data_spec_validator"},
     packages=setuptools.find_packages(),
     install_requires=[
         "python-dateutil",
     ],
     extras_require={
         'decorator': ['Django', 'djangorestframework'],
+        'decorator-dj': ['Django'],
     },
     python_requires=">=3.6",
     project_urls={"Changelog": "https://github.com/hardcoretech/data-spec-validator/blob/develop/CHANGELOG.md"},
 )
```

### Comparing `data-spec-validator-3.0.1/data_spec_validator.egg-info/PKG-INFO` & `data-spec-validator-3.1.0/data_spec_validator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-spec-validator
-Version: 3.0.1
+Version: 3.1.0
 Summary: Validation tool for API/Function parameters
 Home-page: https://github.com/hardcoretech/data-spec-validator
 Author: GoFreight
 Author-email: pypi@hardcoretech.co
 License: UNKNOWN
 Project-URL: Changelog, https://github.com/hardcoretech/data-spec-validator/blob/develop/CHANGELOG.md
 Description: # data-spec-validator
@@ -39,17 +39,18 @@
         
         ## Installation
         - Basic usage:
         ```shell
         pip install data-spec-validator
         ```
         - Advance usage (decorator)
-          1. The decorator function `dsv` depends on `Django` & `djangorestframework`.
+          1. The decorator function `dsv` may depend on `Django` or `djangorestframework`.
         ```shell
-        pip install data-spec-validator[decorator]
+        pip install data-spec-validator[decorator-dj]  # Django Only
+        pip install data-spec-validator[decorator]  # Django Rest Framework
         ```
         
         ## Quick Example
         * Do `validate_data_spec` directly wherever you like
         ```python
         from data_spec_validator.spec import INT, DIGIT_STR, ONE_OF, Checker, CheckerOP, validate_data_spec
         
@@ -356,7 +357,8 @@
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: decorator
+Provides-Extra: decorator-dj
```

### Comparing `data-spec-validator-3.0.1/data_spec_validator.egg-info/SOURCES.txt` & `data-spec-validator-3.1.0/data_spec_validator.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,11 +18,12 @@
 data_spec_validator/spec/utils.py
 data_spec_validator/spec/validators.py
 data_spec_validator/spec/wrappers.py
 data_spec_validator/spec/custom_spec/__init__.py
 data_spec_validator/spec/custom_spec/defines.py
 test/__init__.py
 test/test_class_type_spec.py
-test/test_decorator.py
+test/test_decorator_dj.py
+test/test_decorator_drf.py
 test/test_nested_spec.py
 test/test_spec.py
 test/utils.py
```

