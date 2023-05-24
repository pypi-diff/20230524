# Comparing `tmp/qctrl_sphinx_theme-0.1.3.tar.gz` & `tmp/qctrl_sphinx_theme-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_sphinx_theme-0.1.3.tar", max compression
+gzip compressed data, was "qctrl_sphinx_theme-0.2.0.tar", max compression
```

## Comparing `qctrl_sphinx_theme-0.1.3.tar` & `qctrl_sphinx_theme-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0    36653 2023-03-29 22:39:45.340875 qctrl_sphinx_theme-0.1.3/LICENSE
--rw-r--r--   0        0        0      710 2023-03-29 22:39:45.340875 qctrl_sphinx_theme-0.1.3/README.md
--rw-r--r--   0        0        0     2220 2023-03-29 22:40:00.025005 qctrl_sphinx_theme-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      887 2023-03-29 22:40:00.033005 qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/__init__.py
--rw-r--r--   0        0        0      467 2023-03-29 22:39:45.340875 qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/breadcrumbs.html
--rw-r--r--   0        0        0        0 2023-03-29 22:39:45.340875 qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/footer.html
--rw-r--r--   0        0        0     3084 2023-03-29 22:39:45.340875 qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/layout.html
--rw-r--r--   0        0        0     1749 2023-03-29 22:39:45.340875 qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/search.html
--rw-r--r--   0        0        0      359 2023-03-29 22:39:45.340875 qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/searchbox.html
--rw-r--r--   0        0        0     8557 2023-03-29 22:39:45.340875 qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/static/css/qctrlsphinxtheme.css
--rw-r--r--   0        0        0     5430 2023-03-29 22:39:45.340875 qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/static/favicon.ico
--rw-r--r--   0        0        0    26880 2023-03-29 22:39:45.340875 qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/static/img/q-ctrl-icon-180.png
--rw-r--r--   0        0        0    29759 2023-03-29 22:39:45.340875 qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/static/img/q-ctrl-icon-192.png
--rw-r--r--   0        0        0   122791 2023-03-29 22:39:45.344875 qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/static/img/q-ctrl-icon-512.png
--rw-r--r--   0        0        0     9545 2023-03-29 22:39:45.344875 qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/static/img/q-ctrl-icon.svg
--rw-r--r--   0        0        0    10694 2023-03-29 22:39:45.344875 qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/static/img/q-ctrl-logo.svg
--rw-r--r--   0        0        0   317604 2023-03-29 22:39:45.344875 qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/static/img/social/image.jpg
--rw-r--r--   0        0        0     1194 2023-03-29 22:39:45.344875 qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/static/js/qctrlsphinxtheme.js_t
--rw-r--r--   0        0        0      609 2023-03-29 22:39:45.344875 qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/static/manifest.webmanifest
--rw-r--r--   0        0        0     1985 2023-03-29 22:39:45.344875 qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/static/pygments.css
--rw-r--r--   0        0        0      118 2023-03-29 22:39:45.344875 qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/theme.conf
--rw-r--r--   0        0        0     1728 1970-01-01 00:00:00.000000 qctrl_sphinx_theme-0.1.3/setup.py
--rw-r--r--   0        0        0     2971 1970-01-01 00:00:00.000000 qctrl_sphinx_theme-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-05-24 04:56:53.808957 qctrl_sphinx_theme-0.2.0/LICENSE
+-rw-r--r--   0        0        0      710 2023-05-24 04:56:53.808957 qctrl_sphinx_theme-0.2.0/README.md
+-rw-r--r--   0        0        0     2175 2023-05-24 04:57:13.025274 qctrl_sphinx_theme-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      887 2023-05-24 04:57:13.033274 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/__init__.py
+-rw-r--r--   0        0        0      467 2023-05-24 04:56:53.808957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/breadcrumbs.html
+-rw-r--r--   0        0        0        0 2023-05-24 04:56:53.808957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/footer.html
+-rw-r--r--   0        0        0     3084 2023-05-24 04:56:53.808957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/layout.html
+-rw-r--r--   0        0        0     1749 2023-05-24 04:56:53.808957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/search.html
+-rw-r--r--   0        0        0      359 2023-05-24 04:56:53.808957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/searchbox.html
+-rw-r--r--   0        0        0     8557 2023-05-24 04:56:53.808957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/css/qctrlsphinxtheme.css
+-rw-r--r--   0        0        0     5430 2023-05-24 04:56:53.808957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/favicon.ico
+-rw-r--r--   0        0        0    26880 2023-05-24 04:56:53.812957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/q-ctrl-icon-180.png
+-rw-r--r--   0        0        0    29759 2023-05-24 04:56:53.812957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/q-ctrl-icon-192.png
+-rw-r--r--   0        0        0   122791 2023-05-24 04:56:53.812957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/q-ctrl-icon-512.png
+-rw-r--r--   0        0        0     9545 2023-05-24 04:56:53.812957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/q-ctrl-icon.svg
+-rw-r--r--   0        0        0    10694 2023-05-24 04:56:53.812957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/q-ctrl-logo.svg
+-rw-r--r--   0        0        0   317604 2023-05-24 04:56:53.812957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/social/image.jpg
+-rw-r--r--   0        0        0     1194 2023-05-24 04:56:53.812957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/js/qctrlsphinxtheme.js_t
+-rw-r--r--   0        0        0      609 2023-05-24 04:56:53.812957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/manifest.webmanifest
+-rw-r--r--   0        0        0     1985 2023-05-24 04:56:53.812957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/pygments.css
+-rw-r--r--   0        0        0      118 2023-05-24 04:56:53.812957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/theme.conf
+-rw-r--r--   0        0        0     2871 1970-01-01 00:00:00.000000 qctrl_sphinx_theme-0.2.0/PKG-INFO
```

### Comparing `qctrl_sphinx_theme-0.1.3/LICENSE` & `qctrl_sphinx_theme-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.1.3/README.md` & `qctrl_sphinx_theme-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.1.3/pyproject.toml` & `qctrl_sphinx_theme-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qctrl-sphinx-theme"
-version = "0.1.3"
+version = "0.2.0"
 description = "Q-CTRL Sphinx Theme"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
@@ -42,15 +42,14 @@
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
     "Natural Language :: English",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Scientific/Engineering :: Visualization",
@@ -58,17 +57,17 @@
     "Topic :: System :: Distributed Computing"
 ]
 packages = [
     { include = "qctrlsphinxtheme" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7, <3.12"
+python = ">=3.8, <3.12"
 sphinx = "^5.0.0"
-sphinx_rtd_theme = "~1.1.1"
+sphinx_rtd_theme = "~1.2.0"
 
 [tool.poetry.plugins."sphinx.html_themes"]
 "qctrl_sphinx_theme" = "qctrlsphinxtheme"
 
 [tool.poetry.urls]
 LinkedIn = "https://www.linkedin.com/company/q-ctrl/"
 Facebook = "https://www.facebook.com/qctrl"
```

### Comparing `qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/__init__.py` & `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
 """Q-CTRL Sphinx Theme"""
 from os import path
 
-__version__ = "0.1.3"
+__version__ = "0.2.0"
 __author__ = "Q-CTRL <support@q-ctrl.com>"
 
 # See https://www.sphinx-doc.org/en/master/development/theming.html#distribute-your-theme-as-a-python-package
 def setup(app):
     app.add_html_theme(
         "qctrl_sphinx_theme", path.abspath(path.dirname(__file__))
     )
```

### Comparing `qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/layout.html` & `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/layout.html`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/search.html` & `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/search.html`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/static/css/qctrlsphinxtheme.css` & `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/css/qctrlsphinxtheme.css`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/static/favicon.ico` & `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/static/img/q-ctrl-icon-180.png` & `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/q-ctrl-icon-180.png`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/static/img/q-ctrl-icon-192.png` & `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/q-ctrl-icon-192.png`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/static/img/q-ctrl-icon-512.png` & `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/q-ctrl-icon-512.png`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/static/img/q-ctrl-icon.svg` & `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/q-ctrl-icon.svg`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/static/img/q-ctrl-logo.svg` & `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/q-ctrl-logo.svg`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/static/img/social/image.jpg` & `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/social/image.jpg`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/static/js/qctrlsphinxtheme.js_t` & `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/js/qctrlsphinxtheme.js_t`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/static/manifest.webmanifest` & `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/manifest.webmanifest`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.1.3/qctrlsphinxtheme/static/pygments.css` & `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/pygments.css`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.1.3/PKG-INFO` & `qctrl_sphinx_theme-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 Metadata-Version: 2.1
 Name: qctrl-sphinx-theme
-Version: 0.1.3
+Version: 0.2.0
 Summary: Q-CTRL Sphinx Theme
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
 Maintainer-email: support@q-ctrl.com
-Requires-Python: >=3.7,<3.12
+Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: sphinx (>=5.0.0,<6.0.0)
-Requires-Dist: sphinx_rtd_theme (>=1.1.1,<1.2.0)
+Requires-Dist: sphinx_rtd_theme (>=1.2.0,<1.3.0)
 Project-URL: Facebook, https://www.facebook.com/qctrl
 Project-URL: GitHub, https://github.com/qctrl
 Project-URL: LinkedIn, https://www.linkedin.com/company/q-ctrl/
 Project-URL: Twitter, https://twitter.com/qctrlHQ
 Project-URL: YouTube, https://www.youtube.com/qctrl
 Description-Content-Type: text/markdown
```

