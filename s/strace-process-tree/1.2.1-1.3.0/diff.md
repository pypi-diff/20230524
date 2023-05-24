# Comparing `tmp/strace-process-tree-1.2.1.tar.gz` & `tmp/strace-process-tree-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strace-process-tree-1.2.1.tar", last modified: Fri Oct 28 06:36:59 2022, max compression
+gzip compressed data, was "strace-process-tree-1.3.0.tar", last modified: Wed May 24 07:38:20 2023, max compression
```

## Comparing `strace-process-tree-1.2.1.tar` & `strace-process-tree-1.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2022-10-28 06:36:59.958187 strace-process-tree-1.2.1/
--rw-r--r--   0 mg        (1000) mg        (1000)      126 2019-08-22 13:46:49.000000 strace-process-tree-1.2.1/.coveragerc
--rw-r--r--   0 mg        (1000) mg        (1000)       71 2019-08-21 13:01:00.000000 strace-process-tree-1.2.1/.gitignore
--rw-rw-r--   0 mg        (1000) mg        (1000)     3031 2022-10-28 06:35:50.000000 strace-process-tree-1.2.1/CHANGES.rst
--rw-r--r--   0 mg        (1000) mg        (1000)    18092 2019-08-21 13:59:11.000000 strace-process-tree-1.2.1/LICENSE
--rw-r--r--   0 mg        (1000) mg        (1000)      175 2019-08-21 14:00:54.000000 strace-process-tree-1.2.1/MANIFEST.in
--rw-rw-r--   0 mg        (1000) mg        (1000)      366 2020-10-24 10:07:13.000000 strace-process-tree-1.2.1/Makefile
--rw-rw-r--   0 mg        (1000) mg        (1000)     3594 2022-10-28 06:36:59.958187 strace-process-tree-1.2.1/PKG-INFO
--rw-rw-r--   0 mg        (1000) mg        (1000)     2404 2020-11-30 19:57:48.000000 strace-process-tree-1.2.1/README.rst
--rw-rw-r--   0 mg        (1000) mg        (1000)      870 2022-10-28 06:33:45.000000 strace-process-tree-1.2.1/appveyor.yml
--rw-r--r--   0 mg        (1000) mg        (1000)       44 2019-08-21 13:47:16.000000 strace-process-tree-1.2.1/pytest.ini
--rw-rw-r--   0 mg        (1000) mg        (1000)     5599 2021-04-19 14:36:29.000000 strace-process-tree-1.2.1/release.mk
--rw-r--r--   0 mg        (1000) mg        (1000)      397 2022-10-28 06:36:59.958187 strace-process-tree-1.2.1/setup.cfg
--rwxrwxr-x   0 mg        (1000) mg        (1000)     1936 2022-10-28 06:33:45.000000 strace-process-tree-1.2.1/setup.py
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2022-10-28 06:36:59.958187 strace-process-tree-1.2.1/strace_process_tree.egg-info/
--rw-r--r--   0 mg        (1000) mg        (1000)     3594 2022-10-28 06:36:59.000000 strace-process-tree-1.2.1/strace_process_tree.egg-info/PKG-INFO
--rw-r--r--   0 mg        (1000) mg        (1000)      514 2022-10-28 06:36:59.000000 strace-process-tree-1.2.1/strace_process_tree.egg-info/SOURCES.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2022-10-28 06:36:59.000000 strace-process-tree-1.2.1/strace_process_tree.egg-info/dependency_links.txt
--rw-r--r--   0 mg        (1000) mg        (1000)       66 2022-10-28 06:36:59.000000 strace-process-tree-1.2.1/strace_process_tree.egg-info/entry_points.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2019-08-21 12:43:27.000000 strace-process-tree-1.2.1/strace_process_tree.egg-info/not-zip-safe
--rw-r--r--   0 mg        (1000) mg        (1000)       20 2022-10-28 06:36:59.000000 strace-process-tree-1.2.1/strace_process_tree.egg-info/top_level.txt
--rwxrwxr-x   0 mg        (1000) mg        (1000)    15085 2022-10-28 06:35:50.000000 strace-process-tree-1.2.1/strace_process_tree.py
--rw-r--r--   0 mg        (1000) mg        (1000)     1126 2019-08-21 11:55:33.000000 strace-process-tree-1.2.1/strace_process_tree_example_output.txt
--rw-r--r--   0 mg        (1000) mg        (1000)     7072 2019-08-21 11:55:33.000000 strace-process-tree-1.2.1/strace_process_tree_example_verbose_output.txt
--rw-r--r--   0 mg        (1000) mg        (1000)    16970 2021-04-14 12:46:51.000000 strace-process-tree-1.2.1/tests.py
--rw-rw-r--   0 mg        (1000) mg        (1000)      710 2022-10-28 06:33:45.000000 strace-process-tree-1.2.1/tox.ini
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 07:38:20.517836 strace-process-tree-1.3.0/
+-rw-r--r--   0 mg        (1000) mg        (1000)      126 2019-08-22 13:46:49.000000 strace-process-tree-1.3.0/.coveragerc
+-rw-r--r--   0 mg        (1000) mg        (1000)       71 2019-08-21 13:01:00.000000 strace-process-tree-1.3.0/.gitignore
+-rw-rw-r--   0 mg        (1000) mg        (1000)     3354 2023-05-24 07:37:21.000000 strace-process-tree-1.3.0/CHANGES.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)    18092 2019-08-21 13:59:11.000000 strace-process-tree-1.3.0/LICENSE
+-rw-r--r--   0 mg        (1000) mg        (1000)      175 2019-08-21 14:00:54.000000 strace-process-tree-1.3.0/MANIFEST.in
+-rw-rw-r--   0 mg        (1000) mg        (1000)      366 2020-10-24 10:07:13.000000 strace-process-tree-1.3.0/Makefile
+-rw-rw-r--   0 mg        (1000) mg        (1000)     3611 2023-05-24 07:38:20.517836 strace-process-tree-1.3.0/PKG-INFO
+-rw-rw-r--   0 mg        (1000) mg        (1000)     2404 2020-11-30 19:57:48.000000 strace-process-tree-1.3.0/README.rst
+-rw-rw-r--   0 mg        (1000) mg        (1000)      870 2022-10-28 06:33:45.000000 strace-process-tree-1.3.0/appveyor.yml
+-rw-r--r--   0 mg        (1000) mg        (1000)       44 2019-08-21 13:47:16.000000 strace-process-tree-1.3.0/pytest.ini
+-rw-rw-r--   0 mg        (1000) mg        (1000)     5599 2021-04-19 14:36:29.000000 strace-process-tree-1.3.0/release.mk
+-rw-r--r--   0 mg        (1000) mg        (1000)      397 2023-05-24 07:38:20.517836 strace-process-tree-1.3.0/setup.cfg
+-rwxrwxr-x   0 mg        (1000) mg        (1000)     1984 2022-10-28 06:37:52.000000 strace-process-tree-1.3.0/setup.py
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 07:38:20.517836 strace-process-tree-1.3.0/strace_process_tree.egg-info/
+-rw-r--r--   0 mg        (1000) mg        (1000)     3611 2023-05-24 07:38:20.000000 strace-process-tree-1.3.0/strace_process_tree.egg-info/PKG-INFO
+-rw-r--r--   0 mg        (1000) mg        (1000)      514 2023-05-24 07:38:20.000000 strace-process-tree-1.3.0/strace_process_tree.egg-info/SOURCES.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        1 2023-05-24 07:38:20.000000 strace-process-tree-1.3.0/strace_process_tree.egg-info/dependency_links.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)       65 2023-05-24 07:38:20.000000 strace-process-tree-1.3.0/strace_process_tree.egg-info/entry_points.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        1 2019-08-21 12:43:27.000000 strace-process-tree-1.3.0/strace_process_tree.egg-info/not-zip-safe
+-rw-r--r--   0 mg        (1000) mg        (1000)       20 2023-05-24 07:38:20.000000 strace-process-tree-1.3.0/strace_process_tree.egg-info/top_level.txt
+-rwxrwxr-x   0 mg        (1000) mg        (1000)    15300 2023-05-24 07:37:21.000000 strace-process-tree-1.3.0/strace_process_tree.py
+-rw-r--r--   0 mg        (1000) mg        (1000)     1126 2019-08-21 11:55:33.000000 strace-process-tree-1.3.0/strace_process_tree_example_output.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)     7072 2019-08-21 11:55:33.000000 strace-process-tree-1.3.0/strace_process_tree_example_verbose_output.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)    19802 2023-05-24 07:32:02.000000 strace-process-tree-1.3.0/tests.py
+-rw-rw-r--   0 mg        (1000) mg        (1000)      710 2022-10-28 06:33:45.000000 strace-process-tree-1.3.0/tox.ini
```

### Comparing `strace-process-tree-1.2.1/CHANGES.rst` & `strace-process-tree-1.3.0/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 Changes
 =======
 
 
+1.3.0 (2023-05-24)
+------------------
+
+* Support the NO_COLOR environment variable for disabling color autodetection
+  (see https://no-color.org/).
+* Fix parsing '<... syscall resumed>)' lines without a space in front of
+  the closing parenthesis (`issue 5
+  <https://github.com/mgedmin/strace-process-tree/issues/5>`_).
+
+
 1.2.1 (2022-10-28)
 ------------------
 
 * Add support for Python 3.8, 3.9, 3.10, and 3.11.
 * Drop support for Python 3.5 and 3.6.
 * Show line numbers when complaining about malformed input lines.
 * Handle "[pid  NNN]" prefixes with more than one space.
```

### Comparing `strace-process-tree-1.2.1/LICENSE` & `strace-process-tree-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strace-process-tree-1.2.1/PKG-INFO` & `strace-process-tree-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: strace-process-tree
-Version: 1.2.1
+Version: 1.3.0
 Summary: Produce a process tree from an strace log
 Home-page: https://github.com/mgedmin/strace-process-tree
 Author: Marius Gedminas
 Author-email: marius@gedmin.as
 License: GPL v2 or v3
 Keywords: strace log process tree
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
@@ -19,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 strace-process-tree
 ===================
 
 .. image:: https://github.com/mgedmin/strace-process-tree/workflows/build/badge.svg?branch=master
     :target: https://github.com/mgedmin/strace-process-tree/actions
@@ -86,9 +86,7 @@
   --version       show program's version number and exit
   -c, --color     force color output
   -C, --no-color  disable color output
   -U, --unicode   force Unicode output
   -A, --ascii     force ASCII output
   -v, --verbose   more verbose output
 
-
-
```

### Comparing `strace-process-tree-1.2.1/README.rst` & `strace-process-tree-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `strace-process-tree-1.2.1/appveyor.yml` & `strace-process-tree-1.3.0/appveyor.yml`

 * *Files identical despite different names*

### Comparing `strace-process-tree-1.2.1/release.mk` & `strace-process-tree-1.3.0/release.mk`

 * *Files identical despite different names*

### Comparing `strace-process-tree-1.2.1/setup.py` & `strace-process-tree-1.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     name="strace-process-tree",
     version=version,
     author="Marius Gedminas",
     author_email="marius@gedmin.as",
     url="https://github.com/mgedmin/strace-process-tree",
     description="Produce a process tree from an strace log",
     long_description=long_description,
+    long_description_content_type='text/x-rst',
     keywords="strace log process tree",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
```

### Comparing `strace-process-tree-1.2.1/strace_process_tree.egg-info/PKG-INFO` & `strace-process-tree-1.3.0/strace_process_tree.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: strace-process-tree
-Version: 1.2.1
+Version: 1.3.0
 Summary: Produce a process tree from an strace log
 Home-page: https://github.com/mgedmin/strace-process-tree
 Author: Marius Gedminas
 Author-email: marius@gedmin.as
 License: GPL v2 or v3
 Keywords: strace log process tree
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
@@ -19,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 strace-process-tree
 ===================
 
 .. image:: https://github.com/mgedmin/strace-process-tree/workflows/build/badge.svg?branch=master
     :target: https://github.com/mgedmin/strace-process-tree/actions
@@ -86,9 +86,7 @@
   --version       show program's version number and exit
   -c, --color     force color output
   -C, --no-color  disable color output
   -U, --unicode   force Unicode output
   -A, --ascii     force ASCII output
   -v, --verbose   more verbose output
 
-
-
```

### Comparing `strace-process-tree-1.2.1/strace_process_tree.egg-info/SOURCES.txt` & `strace-process-tree-1.3.0/strace_process_tree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `strace-process-tree-1.2.1/strace_process_tree.py` & `strace-process-tree-1.3.0/strace_process_tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import re
 import string
 import sys
 from collections import defaultdict, namedtuple
 from functools import partial
 
 
-__version__ = '1.2.1'
+__version__ = '1.3.0'
 __author__ = 'Marius Gedminas <marius@gedmin.as>'
 __url__ = "https://github.com/mgedmin/strace-process-tree"
 __licence__ = 'GPL v2 or v3'  # or ask me for MIT
 
 
 Tree = namedtuple('Tree', 'trunk, fork, end, space')
 
@@ -67,25 +67,34 @@
         if unicode is None:
             unicode = self.can_unicode()
         self.tree = self.unicode_tree if unicode else self.ascii_tree
         self.styles = dict(self.default_styles)
 
     @classmethod
     def should_use_color(cls):
-        return cls.is_terminal() and cls.terminal_supports_color()
+        return (
+            cls.is_terminal()
+            and cls.terminal_supports_color()
+            and not cls.user_dislikes_color()
+        )
 
     @classmethod
     def is_terminal(cls):
         return hasattr(sys.stdout, 'isatty') and sys.stdout.isatty()
 
     @classmethod
     def terminal_supports_color(cls):
         return (os.environ.get('TERM') or 'dumb') != 'dumb'
 
     @classmethod
+    def user_dislikes_color(cls):
+        # https://no-color.org/
+        return bool(os.environ.get('NO_COLOR'))
+
+    @classmethod
     def can_unicode(cls):
         return getattr(sys.stdout, 'encoding', None) == 'UTF-8'
 
     def _format(self, prefix, suffix, text):
         if not text:
             return ''
         return '{}{}{}'.format(prefix, text, suffix)
@@ -134,15 +143,15 @@
     if ':' in timestamp:
         h, m, s = timestamp.split(':')
         return (float(h) * 60 + float(m)) * 60 + float(s)
     else:
         return float(timestamp)
 
 
-RESUMED_PREFIX = re.compile(r'<... \w+ resumed> ')
+RESUMED_PREFIX = re.compile(r'<... \w+ resumed> ?')
 UNFINISHED_SUFFIX = ' <unfinished ...>'
 DURATION_SUFFIX = re.compile(r' <\d+(?:\.\d+)?>$')
 PID = re.compile(r'^\[pid +(\d+)\]')
 TIMESTAMP = re.compile(r'^\d+(?::\d+:\d+)?(?:\.\d+)?\s+')
 IGNORE = re.compile(r'^$|^strace: Process \d+ attached$')
```

### Comparing `strace-process-tree-1.2.1/strace_process_tree_example_output.txt` & `strace-process-tree-1.3.0/strace_process_tree_example_output.txt`

 * *Files identical despite different names*

### Comparing `strace-process-tree-1.2.1/strace_process_tree_example_verbose_output.txt` & `strace-process-tree-1.3.0/strace_process_tree_example_verbose_output.txt`

 * *Files identical despite different names*

### Comparing `strace-process-tree-1.2.1/tests.py` & `strace-process-tree-1.3.0/tests.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf-8 -*-
-import os
 import sys
 
 import pytest
 
 import strace_process_tree as stp
 
 
@@ -18,32 +17,55 @@
 
 def test_Theme_is_terminal_yes_it_is(monkeypatch):
     monkeypatch.setattr(sys, 'stdout', FakeStdout())
     assert stp.Theme.is_terminal()
 
 
 def test_Theme_terminal_supports_color_no(monkeypatch):
-    monkeypatch.setitem(os.environ, 'TERM', 'dumb')
+    monkeypatch.setenv('TERM', 'dumb')
     assert not stp.Theme.terminal_supports_color()
 
 
 def test_Theme_terminal_supports_color_yes(monkeypatch):
-    monkeypatch.setitem(os.environ, 'TERM', 'xterm')
+    monkeypatch.setenv('TERM', 'xterm')
     assert stp.Theme.terminal_supports_color()
 
 
+def test_Theme_no_color_unset(monkeypatch):
+    monkeypatch.delenv('NO_COLOR', raising=False)
+    assert not stp.Theme.user_dislikes_color()
+
+
+def test_Theme_no_color_blank(monkeypatch):
+    monkeypatch.setenv('NO_COLOR', '')
+    assert not stp.Theme.user_dislikes_color()
+
+
+def test_Theme_no_color_nonblank(monkeypatch):
+    monkeypatch.setenv('NO_COLOR', 'please')
+    assert stp.Theme.user_dislikes_color()
+
+
 def test_Theme_autodetection_color_yes(monkeypatch):
     monkeypatch.setattr(sys, 'stdout', FakeStdout())
-    monkeypatch.setitem(os.environ, 'TERM', 'xterm')
+    monkeypatch.setenv('TERM', 'xterm')
+    monkeypatch.delenv('NO_COLOR', raising=False)
     assert isinstance(stp.Theme(), stp.AnsiTheme)
 
 
 def test_Theme_autodetection_color_no(monkeypatch):
     monkeypatch.setattr(sys, 'stdout', FakeStdout())
-    monkeypatch.setitem(os.environ, 'TERM', 'dumb')
+    monkeypatch.setenv('TERM', 'dumb')
+    assert isinstance(stp.Theme(), stp.PlainTheme)
+
+
+def test_Theme_autodetection_color_disabled(monkeypatch):
+    monkeypatch.setattr(sys, 'stdout', FakeStdout())
+    monkeypatch.setenv('TERM', 'xterm')
+    monkeypatch.setenv('NO_COLOR', '1')
     assert isinstance(stp.Theme(), stp.PlainTheme)
 
 
 def test_PlainTheme_bad_style():
     with pytest.raises(AttributeError):
         stp.PlainTheme().waterfall("oOoOoO")
 
@@ -100,14 +122,29 @@
         (27370, 50007.214709, 'execve("/bin/sh", ["sh", "-c", "uname -p 2> /dev/null"], 0x55842eb789e0 /* 72 vars */) = 0'),
         (27370, 50007.216357, '--- SIGCHLD {si_signo=SIGCHLD, si_code=CLD_EXITED, si_pid=27371, si_uid=1000, si_status=0, si_utime=0, si_stime=0} ---'),
         (27370, 50007.216395, 'exit_group(0)     = ?'),
         (27370, 50007.216441, '+++ exited with 0 +++'),
     ]
 
 
+def test_events_split_vfork():
+    # Regression test for https://github.com/mgedmin/strace-process-tree/issues/5
+    log_lines = [
+        '230473 02:47:49 vfork( <unfinished ...>',
+        '230474 02:47:49 execve("/home/jtojnar/Projects/tartan/scripts/tartan-build", ["tartan-build", "gcc", "-Isrc/commands/rpm2cpio.p", "-Isrc/commands", "-I../src/commands", "-I.", "-I..", "-I/nix/store/kfizydssj99lf8f6dbmrfa5hap1162m5-glib-2.76.2-dev/include/glib-2.0", "-I/nix/store/763gsnl7y7nj6v98fp1l380ddvyr6zqv-glib-2.76.2/lib/glib-2.0/include", "-fdiagnostics-color=always", "-D_FILE_OFFSET_BITS=64", "-Wall", "-Winvalid-pch", "-O0", "-g", "-DGLIB_VERSION_MIN_REQUIRED=GLIB_VERSION_2_38", "-Wall", "-Wextra", "-Wcast-align", "-Wmissing-prototypes", "-Wnested-externs", "-Wpointer-arith", "-Wformat-security", "-Wno-unused-parameter", "-MD", "-MQ", "src/commands/rpm2cpio.p/rpm2cpio.c.o", "-MF", "src/commands/rpm2cpio.p/rpm2cpio.c.o.d", "-o", "src/commands/rpm2cpio.p/rpm2cpio.c.o", "-c", "../src/commands/rpm2cpio.c"], 0x2507640 /* 163 vars */ <unfinished ...>',
+        '230473 02:47:49 <... vfork resumed>)    = 230474',
+        '230474 02:47:49 <... execve resumed>)   = 0',
+    ]
+    result = list(stp.events(log_lines))
+    assert result == [
+        stp.Event(230473, 10069.0, 'vfork()    = 230474'),
+        stp.Event(230474, 10069.0, 'execve("/home/jtojnar/Projects/tartan/scripts/tartan-build", ["tartan-build", "gcc", "-Isrc/commands/rpm2cpio.p", "-Isrc/commands", "-I../src/commands", "-I.", "-I..", "-I/nix/store/kfizydssj99lf8f6dbmrfa5hap1162m5-glib-2.76.2-dev/include/glib-2.0", "-I/nix/store/763gsnl7y7nj6v98fp1l380ddvyr6zqv-glib-2.76.2/lib/glib-2.0/include", "-fdiagnostics-color=always", "-D_FILE_OFFSET_BITS=64", "-Wall", "-Winvalid-pch", "-O0", "-g", "-DGLIB_VERSION_MIN_REQUIRED=GLIB_VERSION_2_38", "-Wall", "-Wextra", "-Wcast-align", "-Wmissing-prototypes", "-Wnested-externs", "-Wpointer-arith", "-Wformat-security", "-Wno-unused-parameter", "-MD", "-MQ", "src/commands/rpm2cpio.p/rpm2cpio.c.o", "-MF", "src/commands/rpm2cpio.p/rpm2cpio.c.o.d", "-o", "src/commands/rpm2cpio.p/rpm2cpio.c.o", "-c", "../src/commands/rpm2cpio.c"], 0x2507640 /* 163 vars */)   = 0'),
+    ]
+
+
 def test_events_special_pid_format():
     log_lines = [
         '[pid 27369] execve("bin/test", ["bin/test", "-pvc", "-t", "allowhosts.txt"], 0x7fffa04e8ba0 /* 71 vars */) = 0',
         '[pid   123] execve("bin/test", ["bin/test", "-pvc", "-t", "allowhosts.txt"], 0x7fffa04e8ba0 /* 71 vars */) = 0',
     ]
     result = list(stp.events(log_lines))
     assert result == [
```

### Comparing `strace-process-tree-1.2.1/tox.ini` & `strace-process-tree-1.3.0/tox.ini`

 * *Files identical despite different names*

