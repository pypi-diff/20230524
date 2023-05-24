# Comparing `tmp/mypy-boto3-cur-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-cur-1.26.140.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cur-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:18 2022, max compression
+gzip compressed data, was "mypy-boto3-cur-1.26.140.tar", last modified: Wed May 24 20:47:52 2023, max compression
```

## Comparing `mypy-boto3-cur-1.26.0.post1.tar` & `mypy-boto3-cur-1.26.140.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:18.244821 mypy-boto3-cur-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:32:30.000000 mypy-boto3-cur-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    13146 2022-11-01 21:43:18.244821 mypy-boto3-cur-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11699 2022-11-01 21:32:30.000000 mypy-boto3-cur-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:18.244821 mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-11-01 21:32:30.000000 mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      723 2022-11-01 21:32:30.000000 mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      945 2022-11-01 21:32:30.000000 mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6061 2022-11-01 21:32:30.000000 mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     6049 2022-11-01 21:32:30.000000 mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8118 2022-11-01 21:32:31.000000 mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8116 2022-11-01 21:32:30.000000 mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1984 2022-11-01 21:32:30.000000 mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1981 2022-11-01 21:32:30.000000 mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:32:30.000000 mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     3912 2022-11-01 21:32:31.000000 mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3909 2022-11-01 21:32:31.000000 mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:32:30.000000 mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:18.244821 mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13146 2022-11-01 21:43:18.000000 mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-11-01 21:43:18.000000 mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:18.000000 mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:18.000000 mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:18.000000 mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-01 21:43:18.000000 mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:18.244821 mypy-boto3-cur-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-11-01 21:32:30.000000 mypy-boto3-cur-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:52.290331 mypy-boto3-cur-1.26.140/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-24 20:47:12.000000 mypy-boto3-cur-1.26.140/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13170 2023-05-24 20:47:52.290331 mypy-boto3-cur-1.26.140/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-05-24 20:47:12.000000 mypy-boto3-cur-1.26.140/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:52.290331 mypy-boto3-cur-1.26.140/mypy_boto3_cur/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-24 20:47:12.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-24 20:47:12.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-24 20:47:12.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-24 20:47:13.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-24 20:47:12.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-05-24 20:47:13.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-05-24 20:47:13.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-24 20:47:13.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-24 20:47:13.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:12.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-24 20:47:13.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-24 20:47:13.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-24 20:47:12.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:52.290331 mypy-boto3-cur-1.26.140/mypy_boto3_cur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13170 2023-05-24 20:47:52.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-24 20:47:52.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:47:52.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:47:52.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-24 20:47:52.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 20:47:52.000000 mypy-boto3-cur-1.26.140/mypy_boto3_cur.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 20:47:52.290331 mypy-boto3-cur-1.26.140/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-24 20:47:12.000000 mypy-boto3-cur-1.26.140/setup.py
```

### Comparing `mypy-boto3-cur-1.26.0.post1/LICENSE` & `mypy-boto3-cur-1.26.140/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-cur-1.26.0.post1/PKG-INFO` & `mypy-boto3-cur-1.26.140/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,60 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-cur
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CostandUsageReportService 1.26.0 service generated with mypy-boto3-builder 7.11.10
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 cur type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-cur"></a>
 
 # mypy-boto3-cur
 
 [![PyPI - mypy-boto3-cur](https://img.shields.io/pypi/v/mypy-boto3-cur.svg?color=blue)](https://pypi.org/project/mypy-boto3-cur)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cur.svg?color=blue)](https://pypi.org/project/mypy-boto3-cur)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cur?color=blue)](https://pypistats.org/packages/mypy-boto3-cur)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostandUsageReportService 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
+[boto3.CostandUsageReportService 1.26.140](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cur docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/).
 
 See how it helps to find and fix potential bugs:
 
@@ -327,20 +296,20 @@
 
 `mypy_boto3_cur.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cur.type_defs import (
     DeleteReportDefinitionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeReportDefinitionsRequestRequestTypeDef,
-    ReportDefinitionTypeDef,
     DeleteReportDefinitionResponseTypeDef,
     DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef,
+    DescribeReportDefinitionsRequestRequestTypeDef,
+    ReportDefinitionTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     DescribeReportDefinitionsResponseTypeDef,
     ModifyReportDefinitionRequestRequestTypeDef,
     PutReportDefinitionRequestRequestTypeDef,
 )
 
 
 def get_structure() -> DeleteReportDefinitionRequestRequestTypeDef:
@@ -350,42 +319,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-cur-1.26.0.post1/README.md` & `mypy-boto3-cur-1.26.140/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-cur
+Version: 1.26.140
+Summary: Type annotations for boto3.CostandUsageReportService 1.26.140 service generated with mypy-boto3-builder 7.14.5
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 cur type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-cur"></a>
 
 # mypy-boto3-cur
 
 [![PyPI - mypy-boto3-cur](https://img.shields.io/pypi/v/mypy-boto3-cur.svg?color=blue)](https://pypi.org/project/mypy-boto3-cur)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cur.svg?color=blue)](https://pypi.org/project/mypy-boto3-cur)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cur?color=blue)](https://pypistats.org/packages/mypy-boto3-cur)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostandUsageReportService 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
+[boto3.CostandUsageReportService 1.26.140](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cur docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/).
 
 See how it helps to find and fix potential bugs:
 
@@ -296,20 +328,20 @@
 
 `mypy_boto3_cur.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cur.type_defs import (
     DeleteReportDefinitionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeReportDefinitionsRequestRequestTypeDef,
-    ReportDefinitionTypeDef,
     DeleteReportDefinitionResponseTypeDef,
     DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef,
+    DescribeReportDefinitionsRequestRequestTypeDef,
+    ReportDefinitionTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     DescribeReportDefinitionsResponseTypeDef,
     ModifyReportDefinitionRequestRequestTypeDef,
     PutReportDefinitionRequestRequestTypeDef,
 )
 
 
 def get_structure() -> DeleteReportDefinitionRequestRequestTypeDef:
@@ -319,42 +351,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/__init__.py` & `mypy-boto3-cur-1.26.140/mypy_boto3_cur/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/__init__.pyi` & `mypy-boto3-cur-1.26.140/mypy_boto3_cur/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/__main__.py` & `mypy-boto3-cur-1.26.140/mypy_boto3_cur/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CostandUsageReportService 1.26.0\nVersion:        "
-        " 1.26.0.post1\nBuilder version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.CostandUsageReportService 1.26.140\nVersion:        "
+        " 1.26.140\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.0.post1")
+    print("1.26.140")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/client.py` & `mypy-boto3-cur-1.26.140/mypy_boto3_cur/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/client.pyi` & `mypy-boto3-cur-1.26.140/mypy_boto3_cur/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/literals.py` & `mypy-boto3-cur-1.26.140/mypy_boto3_cur/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AWSRegionType",
     "AdditionalArtifactType",
     "CompressionFormatType",
     "DescribeReportDefinitionsPaginatorName",
     "ReportFormatType",
     "ReportVersioningType",
@@ -31,29 +30,30 @@
     "CostandUsageReportServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AWSRegionType = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ca-central-1",
     "cn-north-1",
     "cn-northwest-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
@@ -65,15 +65,15 @@
     "us-west-2",
 ]
 AdditionalArtifactType = Literal["ATHENA", "QUICKSIGHT", "REDSHIFT"]
 CompressionFormatType = Literal["GZIP", "Parquet", "ZIP"]
 DescribeReportDefinitionsPaginatorName = Literal["describe_report_definitions"]
 ReportFormatType = Literal["Parquet", "textORcsv"]
 ReportVersioningType = Literal["CREATE_NEW_REPORT", "OVERWRITE_REPORT"]
-SchemaElementType = Literal["RESOURCES"]
+SchemaElementType = Literal["RESOURCES", "SPLIT_COST_ALLOCATION_DATA"]
 TimeUnitType = Literal["DAILY", "HOURLY", "MONTHLY"]
 CostandUsageReportServiceServiceName = Literal["cur"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -92,14 +92,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -109,27 +110,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -158,14 +163,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -210,51 +216,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -267,14 +279,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -286,28 +299,33 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -316,14 +334,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -334,55 +353,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/literals.pyi` & `mypy-boto3-cur-1.26.140/mypy_boto3_cur/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AWSRegionType",
     "AdditionalArtifactType",
     "CompressionFormatType",
     "DescribeReportDefinitionsPaginatorName",
     "ReportFormatType",
     "ReportVersioningType",
@@ -30,28 +31,31 @@
     "CostandUsageReportServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AWSRegionType = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ca-central-1",
     "cn-north-1",
     "cn-northwest-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
@@ -63,15 +67,15 @@
     "us-west-2",
 ]
 AdditionalArtifactType = Literal["ATHENA", "QUICKSIGHT", "REDSHIFT"]
 CompressionFormatType = Literal["GZIP", "Parquet", "ZIP"]
 DescribeReportDefinitionsPaginatorName = Literal["describe_report_definitions"]
 ReportFormatType = Literal["Parquet", "textORcsv"]
 ReportVersioningType = Literal["CREATE_NEW_REPORT", "OVERWRITE_REPORT"]
-SchemaElementType = Literal["RESOURCES"]
+SchemaElementType = Literal["RESOURCES", "SPLIT_COST_ALLOCATION_DATA"]
 TimeUnitType = Literal["DAILY", "HOURLY", "MONTHLY"]
 CostandUsageReportServiceServiceName = Literal["cur"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -90,14 +94,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -107,27 +112,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -156,14 +165,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -208,51 +218,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -265,14 +281,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -284,28 +301,33 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -314,14 +336,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -332,55 +355,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/paginator.py` & `mypy-boto3-cur-1.26.140/mypy_boto3_cur/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -23,31 +23,28 @@
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import DescribeReportDefinitionsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("DescribeReportDefinitionsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeReportDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Paginator.DescribeReportDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/paginators/#describereportdefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReportDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Paginator.DescribeReportDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/paginators/#describereportdefinitionspaginator)
         """
```

### Comparing `mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/paginator.pyi` & `mypy-boto3-cur-1.26.140/mypy_boto3_cur/paginator.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,28 +23,31 @@
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import DescribeReportDefinitionsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("DescribeReportDefinitionsPaginator",)
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeReportDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Paginator.DescribeReportDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/paginators/#describereportdefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReportDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Paginator.DescribeReportDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/paginators/#describereportdefinitionspaginator)
         """
```

### Comparing `mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/type_defs.py` & `mypy-boto3-cur-1.26.140/mypy_boto3_cur/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,65 +16,57 @@
 
 from .literals import (
     AdditionalArtifactType,
     AWSRegionType,
     CompressionFormatType,
     ReportFormatType,
     ReportVersioningType,
+    SchemaElementType,
     TimeUnitType,
 )
 
 if sys.version_info >= (3, 9):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
-if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "DeleteReportDefinitionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "PaginatorConfigTypeDef",
-    "DescribeReportDefinitionsRequestRequestTypeDef",
-    "ReportDefinitionTypeDef",
     "DeleteReportDefinitionResponseTypeDef",
     "DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef",
+    "DescribeReportDefinitionsRequestRequestTypeDef",
+    "ReportDefinitionTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeReportDefinitionsResponseTypeDef",
     "ModifyReportDefinitionRequestRequestTypeDef",
     "PutReportDefinitionRequestRequestTypeDef",
 )
 
 DeleteReportDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteReportDefinitionRequestRequestTypeDef",
     {
         "ReportName": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+DeleteReportDefinitionResponseTypeDef = TypedDict(
+    "DeleteReportDefinitionResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResponseMessage": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef = TypedDict(
+    "DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeReportDefinitionsRequestRequestTypeDef = TypedDict(
     "DescribeReportDefinitionsRequestRequestTypeDef",
     {
@@ -87,15 +79,15 @@
 _RequiredReportDefinitionTypeDef = TypedDict(
     "_RequiredReportDefinitionTypeDef",
     {
         "ReportName": str,
         "TimeUnit": TimeUnitType,
         "Format": ReportFormatType,
         "Compression": CompressionFormatType,
-        "AdditionalSchemaElements": List[Literal["RESOURCES"]],
+        "AdditionalSchemaElements": List[SchemaElementType],
         "S3Bucket": str,
         "S3Prefix": str,
         "S3Region": AWSRegionType,
     },
 )
 _OptionalReportDefinitionTypeDef = TypedDict(
     "_OptionalReportDefinitionTypeDef",
@@ -109,36 +101,41 @@
 )
 
 
 class ReportDefinitionTypeDef(_RequiredReportDefinitionTypeDef, _OptionalReportDefinitionTypeDef):
     pass
 
 
-DeleteReportDefinitionResponseTypeDef = TypedDict(
-    "DeleteReportDefinitionResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ResponseMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef = TypedDict(
-    "DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 DescribeReportDefinitionsResponseTypeDef = TypedDict(
     "DescribeReportDefinitionsResponseTypeDef",
     {
         "ReportDefinitions": List[ReportDefinitionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyReportDefinitionRequestRequestTypeDef = TypedDict(
     "ModifyReportDefinitionRequestRequestTypeDef",
     {
         "ReportName": str,
```

### Comparing `mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur/type_defs.pyi` & `mypy-boto3-cur-1.26.140/mypy_boto3_cur/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -16,64 +16,56 @@
 
 from .literals import (
     AdditionalArtifactType,
     AWSRegionType,
     CompressionFormatType,
     ReportFormatType,
     ReportVersioningType,
+    SchemaElementType,
     TimeUnitType,
 )
 
 if sys.version_info >= (3, 9):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
-if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "DeleteReportDefinitionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "PaginatorConfigTypeDef",
-    "DescribeReportDefinitionsRequestRequestTypeDef",
-    "ReportDefinitionTypeDef",
     "DeleteReportDefinitionResponseTypeDef",
     "DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef",
+    "DescribeReportDefinitionsRequestRequestTypeDef",
+    "ReportDefinitionTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeReportDefinitionsResponseTypeDef",
     "ModifyReportDefinitionRequestRequestTypeDef",
     "PutReportDefinitionRequestRequestTypeDef",
 )
 
 DeleteReportDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteReportDefinitionRequestRequestTypeDef",
     {
         "ReportName": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+DeleteReportDefinitionResponseTypeDef = TypedDict(
+    "DeleteReportDefinitionResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResponseMessage": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef = TypedDict(
+    "DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeReportDefinitionsRequestRequestTypeDef = TypedDict(
     "DescribeReportDefinitionsRequestRequestTypeDef",
     {
@@ -86,15 +78,15 @@
 _RequiredReportDefinitionTypeDef = TypedDict(
     "_RequiredReportDefinitionTypeDef",
     {
         "ReportName": str,
         "TimeUnit": TimeUnitType,
         "Format": ReportFormatType,
         "Compression": CompressionFormatType,
-        "AdditionalSchemaElements": List[Literal["RESOURCES"]],
+        "AdditionalSchemaElements": List[SchemaElementType],
         "S3Bucket": str,
         "S3Prefix": str,
         "S3Region": AWSRegionType,
     },
 )
 _OptionalReportDefinitionTypeDef = TypedDict(
     "_OptionalReportDefinitionTypeDef",
@@ -106,36 +98,41 @@
     },
     total=False,
 )
 
 class ReportDefinitionTypeDef(_RequiredReportDefinitionTypeDef, _OptionalReportDefinitionTypeDef):
     pass
 
-DeleteReportDefinitionResponseTypeDef = TypedDict(
-    "DeleteReportDefinitionResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ResponseMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef = TypedDict(
-    "DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 DescribeReportDefinitionsResponseTypeDef = TypedDict(
     "DescribeReportDefinitionsResponseTypeDef",
     {
         "ReportDefinitions": List[ReportDefinitionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyReportDefinitionRequestRequestTypeDef = TypedDict(
     "ModifyReportDefinitionRequestRequestTypeDef",
     {
         "ReportName": str,
```

### Comparing `mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur.egg-info/PKG-INFO` & `mypy-boto3-cur-1.26.140/mypy_boto3_cur.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cur
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CostandUsageReportService 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.140
+Summary: Type annotations for boto3.CostandUsageReportService 1.26.140 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-cur"></a>
 
 # mypy-boto3-cur
 
 [![PyPI - mypy-boto3-cur](https://img.shields.io/pypi/v/mypy-boto3-cur.svg?color=blue)](https://pypi.org/project/mypy-boto3-cur)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cur.svg?color=blue)](https://pypi.org/project/mypy-boto3-cur)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cur?color=blue)](https://pypistats.org/packages/mypy-boto3-cur)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostandUsageReportService 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
+[boto3.CostandUsageReportService 1.26.140](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cur docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/).
 
 See how it helps to find and fix potential bugs:
 
@@ -327,20 +328,20 @@
 
 `mypy_boto3_cur.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cur.type_defs import (
     DeleteReportDefinitionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeReportDefinitionsRequestRequestTypeDef,
-    ReportDefinitionTypeDef,
     DeleteReportDefinitionResponseTypeDef,
     DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef,
+    DescribeReportDefinitionsRequestRequestTypeDef,
+    ReportDefinitionTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     DescribeReportDefinitionsResponseTypeDef,
     ModifyReportDefinitionRequestRequestTypeDef,
     PutReportDefinitionRequestRequestTypeDef,
 )
 
 
 def get_structure() -> DeleteReportDefinitionRequestRequestTypeDef:
@@ -350,42 +351,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-cur-1.26.0.post1/mypy_boto3_cur.egg-info/SOURCES.txt` & `mypy-boto3-cur-1.26.140/mypy_boto3_cur.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.26.0.post1/setup.py` & `mypy-boto3-cur-1.26.140/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-cur.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cur",
-    version="1.26.0.post1",
+    version="1.26.140",
     packages=["mypy_boto3_cur"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CostandUsageReportService 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.CostandUsageReportService 1.26.140 service generated with"
+        " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 cur type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_cur": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_cur": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```

