# Comparing `tmp/lazychains-0.2.6.tar.gz` & `tmp/lazychains-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazychains-0.2.6.tar", max compression
+gzip compressed data, was "lazychains-0.2.7.tar", max compression
```

## Comparing `lazychains-0.2.6.tar` & `lazychains-0.2.7.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-01-29 09:47:54.921643 lazychains-0.2.6/LICENSE
--rw-r--r--   0        0        0     2255 2023-02-12 15:08:10.206893 lazychains-0.2.6/README.md
--rw-r--r--   0        0        0     1056 2023-02-12 19:36:56.469274 lazychains-0.2.6/pyproject.toml
--rw-r--r--   0        0        0       50 2023-01-27 18:43:04.214015 lazychains-0.2.6/src/lazychains/__init__.py
--rw-r--r--   0        0        0    12570 2023-02-12 19:22:37.762471 lazychains-0.2.6/src/lazychains/lazychains.py
--rw-r--r--   0        0        0     2997 2023-02-12 19:40:11.473675 lazychains-0.2.6/setup.py
--rw-r--r--   0        0        0     3309 2023-02-12 19:40:11.473966 lazychains-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-01-29 09:47:54.921643 lazychains-0.2.7/LICENSE
+-rw-r--r--   0        0        0     2255 2023-02-12 15:08:10.206893 lazychains-0.2.7/README.md
+-rw-r--r--   0        0        0     1056 2023-05-24 07:44:09.724617 lazychains-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-01-27 18:43:04.214015 lazychains-0.2.7/src/lazychains/__init__.py
+-rw-r--r--   0        0        0    12570 2023-02-12 19:22:37.762471 lazychains-0.2.7/src/lazychains/lazychains.py
+-rw-r--r--   0        0        0     3360 1970-01-01 00:00:00.000000 lazychains-0.2.7/PKG-INFO
```

### Comparing `lazychains-0.2.6/LICENSE` & `lazychains-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lazychains-0.2.6/README.md` & `lazychains-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `lazychains-0.2.6/pyproject.toml` & `lazychains-0.2.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazychains"
-version = "0.2.6"
+version = "0.2.7"
 description = "Singly linked lists with incremental instantiation of iterators"
 authors = ["Stephen Leach <sfkleach@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme="README.md"
 homepage="https://lazychains.readthedocs.io/en/latest/"
 documentation="https://lazychains.readthedocs.io/en/latest/"
 repository = "https://github.com/sfkleach/lazychains"
@@ -20,14 +20,14 @@
     "Typing :: Typed"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.1"
-Sphinx = "^6.1.3"
-mypy = "^1.0.0"
+pytest = "^7.3.1"
+Sphinx = "^7.0.1"
+mypy = "^1.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lazychains-0.2.6/src/lazychains/lazychains.py` & `lazychains-0.2.7/src/lazychains/lazychains.py`

 * *Files identical despite different names*

### Comparing `lazychains-0.2.6/setup.py` & `lazychains-0.2.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,87 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: lazychains
+Version: 0.2.7
+Summary: Singly linked lists with incremental instantiation of iterators
+Home-page: https://lazychains.readthedocs.io/en/latest/
+License: GPL-3.0-or-later
+Keywords: iterators,linked list,single,lazy
+Author: Stephen Leach
+Author-email: sfkleach@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Typing :: Typed
+Project-URL: Documentation, https://lazychains.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/sfkleach/lazychains
+Description-Content-Type: text/markdown
+
+# Package Description
+
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/sfkleach/lazychains/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/sfkleach/lazychains/tree/main) [![Documentation Status](https://readthedocs.org/projects/lazychains/badge/?version=latest)](https://lazychains.readthedocs.io/en/latest/?badge=latest)
+
+A Python library to provide "chains", which are Lisp-like singly linked lists 
+that support the lazy expansion of iterators. For example, we can construct a 
+Chain of three characters from the iterable "abc" and it initially starts as 
+unexpanded, shown by the three dots:
+
+```py
+>>> from lazychains import lazychain
+>>> c = lazychain( "abc")
+>>> c
+chain([...])
+```
+
+We can force the expansion of *c* by performing (say) a lookup or by forcing the whole
+chain of items by calling expand:
+
+```py
+>>> c[1]                   # Force the expansion of the next 2 elements.
+True
+>>> c
+chain(['a','b',...])
+>>> c.expand()             # Force the expansion of the whole chain.
+chain(['a','b','c'])
+```
+
+Chain are typically a lot less efficient than using ordinary arrays. So,
+almost all the time you should carry on using ordinary arrays and/or tuples.
+But Chains have a couple of special features that makes them the 
+perfect choice for some problems.
+
+   * Chains are immutable and hence can safely share their trailing segments.
+   * Chains can make it easy to work with extremely large (or infinite) 
+     sequences.
+
+Expanded or Unexpanded
+----------------------
+
+When you construct a chain from an iterator, you can choose whether or not
+it should be immediately expanded by calling chain rather than lazychain.
+The difference between the two is pictured below. First we can see what happens
+in the example given above where we create the chain using lazychain on 
+"abc".
+
+![chain](https://user-images.githubusercontent.com/1164439/215340284-4b7b44a7-df32-4b90-b925-f0a395694805.png)
+
+By contrast, we would immediately go to a fully expanded chain if we were to
+simply apply chain:
+
+```py
+>>> from lazychains import chain
+>>> c = chain( "abc" )
+>>> c
+chain(['a','b','c'])
+>>> 
+```
 
-package_dir = \
-{'': 'src'}
+![lazychain](https://user-images.githubusercontent.com/1164439/215340294-1667798e-dcad-402e-bccb-e0423f1e8ed9.png)
 
-packages = \
-['lazychains']
 
-package_data = \
-{'': ['*']}
-
-setup_kwargs = {
-    'name': 'lazychains',
-    'version': '0.2.6',
-    'description': 'Singly linked lists with incremental instantiation of iterators',
-    'long_description': '# Package Description\n\n[![CircleCI](https://dl.circleci.com/status-badge/img/gh/sfkleach/lazychains/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/sfkleach/lazychains/tree/main) [![Documentation Status](https://readthedocs.org/projects/lazychains/badge/?version=latest)](https://lazychains.readthedocs.io/en/latest/?badge=latest)\n\nA Python library to provide "chains", which are Lisp-like singly linked lists \nthat support the lazy expansion of iterators. For example, we can construct a \nChain of three characters from the iterable "abc" and it initially starts as \nunexpanded, shown by the three dots:\n\n```py\n>>> from lazychains import lazychain\n>>> c = lazychain( "abc")\n>>> c\nchain([...])\n```\n\nWe can force the expansion of *c* by performing (say) a lookup or by forcing the whole\nchain of items by calling expand:\n\n```py\n>>> c[1]                   # Force the expansion of the next 2 elements.\nTrue\n>>> c\nchain([\'a\',\'b\',...])\n>>> c.expand()             # Force the expansion of the whole chain.\nchain([\'a\',\'b\',\'c\'])\n```\n\nChain are typically a lot less efficient than using ordinary arrays. So,\nalmost all the time you should carry on using ordinary arrays and/or tuples.\nBut Chains have a couple of special features that makes them the \nperfect choice for some problems.\n\n   * Chains are immutable and hence can safely share their trailing segments.\n   * Chains can make it easy to work with extremely large (or infinite) \n     sequences.\n\nExpanded or Unexpanded\n----------------------\n\nWhen you construct a chain from an iterator, you can choose whether or not\nit should be immediately expanded by calling chain rather than lazychain.\nThe difference between the two is pictured below. First we can see what happens\nin the example given above where we create the chain using lazychain on \n"abc".\n\n![chain](https://user-images.githubusercontent.com/1164439/215340284-4b7b44a7-df32-4b90-b925-f0a395694805.png)\n\nBy contrast, we would immediately go to a fully expanded chain if we were to\nsimply apply chain:\n\n```py\n>>> from lazychains import chain\n>>> c = chain( "abc" )\n>>> c\nchain([\'a\',\'b\',\'c\'])\n>>> \n```\n\n![lazychain](https://user-images.githubusercontent.com/1164439/215340294-1667798e-dcad-402e-bccb-e0423f1e8ed9.png)\n\n',
-    'author': 'Stephen Leach',
-    'author_email': 'sfkleach@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://lazychains.readthedocs.io/en/latest/',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

