# Comparing `tmp/lockss_debugpanel-0.7.0.tar.gz` & `tmp/lockss_debugpanel-0.7.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lockss_debugpanel-0.7.0.tar", max compression
+gzip compressed data, was "lockss_debugpanel-0.7.0.post1.tar", max compression
```

## Comparing `lockss_debugpanel-0.7.0.tar` & `lockss_debugpanel-0.7.0.post1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      647 2023-05-02 07:40:55.864231 lockss_debugpanel-0.7.0/CHANGELOG.rst
--rw-r--r--   0        0        0     1506 2023-03-14 16:04:54.653141 lockss_debugpanel-0.7.0/LICENSE
--rw-r--r--   0        0        0    37646 2023-05-02 07:40:55.864231 lockss_debugpanel-0.7.0/README.rst
--rw-r--r--   0        0        0      947 2023-05-02 07:40:55.864231 lockss_debugpanel-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     5673 2023-05-02 07:40:55.864231 lockss_debugpanel-0.7.0/src/lockss/debugpanel/__init__.py
--rw-r--r--   0        0        0     1639 2023-03-14 16:04:54.653141 lockss_debugpanel-0.7.0/src/lockss/debugpanel/__main__.py
--rw-r--r--   0        0        0    20145 2023-05-02 07:40:55.864231 lockss_debugpanel-0.7.0/src/lockss/debugpanel/cli.py
--rw-r--r--   0        0        0    38761 1970-01-01 00:00:00.000000 lockss_debugpanel-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      647 2023-05-23 23:23:39.236200 lockss_debugpanel-0.7.0.post1/CHANGELOG.rst
+-rw-r--r--   0        0        0     1506 2023-03-06 21:34:27.042789 lockss_debugpanel-0.7.0.post1/LICENSE
+-rw-r--r--   0        0        0    37779 2023-05-23 23:26:53.382784 lockss_debugpanel-0.7.0.post1/README.rst
+-rw-r--r--   0        0        0      953 2023-05-23 23:24:36.923832 lockss_debugpanel-0.7.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     5679 2023-05-23 23:24:53.694112 lockss_debugpanel-0.7.0.post1/src/lockss/debugpanel/__init__.py
+-rw-r--r--   0        0        0     1639 2023-03-07 02:50:58.596838 lockss_debugpanel-0.7.0.post1/src/lockss/debugpanel/__main__.py
+-rw-r--r--   0        0        0    20145 2023-05-23 17:33:13.987419 lockss_debugpanel-0.7.0.post1/src/lockss/debugpanel/cli.py
+-rw-r--r--   0        0        0    38900 1970-01-01 00:00:00.000000 lockss_debugpanel-0.7.0.post1/PKG-INFO
```

### Comparing `lockss_debugpanel-0.7.0/CHANGELOG.rst` & `lockss_debugpanel-0.7.0.post1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `lockss_debugpanel-0.7.0/LICENSE` & `lockss_debugpanel-0.7.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `lockss_debugpanel-0.7.0/README.rst` & `lockss_debugpanel-0.7.0.post1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 ==========
 Debugpanel
 ==========
 
-.. |RELEASE| replace:: 0.7.0
+.. |RELEASE| replace:: 0.7.0-post1
 .. |RELEASE_DATE| replace:: 2023-05-02
 
 .. |AUID| replace:: ``--auid/-a``
 .. |AUIDS| replace:: ``--auids/-A``
 .. |HELP| replace:: ``--help/-h``
 .. |NODE| replace:: ``--node/-n``
 .. |NODES| replace:: ``--nodes/-N``
 
+.. image:: https://assets.lockss.org/images/logos/debugpanel/debugpanel_128x128.png
+   :alt: Debugpanel logo
+   :align: right
+
 Debugpanel is a library and command line tool to interact with the LOCKSS 1.x DebugPanel servlet.
 
 **Latest release:** |RELEASE| (|RELEASE_DATE|)
 
 -----------------
 Table of Contents
 -----------------
```

### Comparing `lockss_debugpanel-0.7.0/pyproject.toml` & `lockss_debugpanel-0.7.0.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lockss-debugpanel"
-version = "0.7.0"
+version = "0.7.0-post1"
 description = "Library and command line tool to interact with the LOCKSS 1.x DebugPanel servlet"
 license = "BSD-3-Clause"
 authors = [
     "Thib Guicherd-Callin <thib@cs.stanford.edu>"
 ]
 readme = "README.rst"
 homepage = "https://www.lockss.org/"
```

### Comparing `lockss_debugpanel-0.7.0/src/lockss/debugpanel/__init__.py` & `lockss_debugpanel-0.7.0.post1/src/lockss/debugpanel/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = '0.7.0'
+__version__ = '0.7.0-post1'
 
 __copyright__ = '''
 Copyright (c) 2000-2023, Board of Trustees of Leland Stanford Jr. University
 '''.strip()
 
 __license__ = __copyright__ + '\n\n' + '''
 Redistribution and use in source and binary forms, with or without
```

### Comparing `lockss_debugpanel-0.7.0/src/lockss/debugpanel/__main__.py` & `lockss_debugpanel-0.7.0.post1/src/lockss/debugpanel/__main__.py`

 * *Files identical despite different names*

### Comparing `lockss_debugpanel-0.7.0/src/lockss/debugpanel/cli.py` & `lockss_debugpanel-0.7.0.post1/src/lockss/debugpanel/cli.py`

 * *Files identical despite different names*

### Comparing `lockss_debugpanel-0.7.0/PKG-INFO` & `lockss_debugpanel-0.7.0.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lockss-debugpanel
-Version: 0.7.0
+Version: 0.7.0.post1
 Summary: Library and command line tool to interact with the LOCKSS 1.x DebugPanel servlet
 Home-page: https://www.lockss.org/
 License: BSD-3-Clause
 Author: Thib Guicherd-Callin
 Author-email: thib@cs.stanford.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,23 +25,27 @@
 Project-URL: Repository, https://github.com/lockss/lockss-debugpanel
 Description-Content-Type: text/x-rst
 
 ==========
 Debugpanel
 ==========
 
-.. |RELEASE| replace:: 0.7.0
+.. |RELEASE| replace:: 0.7.0-post1
 .. |RELEASE_DATE| replace:: 2023-05-02
 
 .. |AUID| replace:: ``--auid/-a``
 .. |AUIDS| replace:: ``--auids/-A``
 .. |HELP| replace:: ``--help/-h``
 .. |NODE| replace:: ``--node/-n``
 .. |NODES| replace:: ``--nodes/-N``
 
+.. image:: https://assets.lockss.org/images/logos/debugpanel/debugpanel_128x128.png
+   :alt: Debugpanel logo
+   :align: right
+
 Debugpanel is a library and command line tool to interact with the LOCKSS 1.x DebugPanel servlet.
 
 **Latest release:** |RELEASE| (|RELEASE_DATE|)
 
 -----------------
 Table of Contents
 -----------------
```

