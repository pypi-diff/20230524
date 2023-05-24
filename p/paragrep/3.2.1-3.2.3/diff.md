# Comparing `tmp/paragrep-3.2.1.zip` & `tmp/paragrep-3.2.3.zip`

## zipinfo {}

```diff
@@ -1,20 +1,19 @@
-Zip file size: 11429 bytes, number of entries: 18
-drwxr-xr-x  2.0 unx        0 b- stor 19-Aug-28 13:29 paragrep-3.2.1/
-drwxr-xr-x  2.0 unx        0 b- stor 19-Aug-28 13:29 paragrep-3.2.1/man/
-drwxr-xr-x  2.0 unx        0 b- stor 19-Aug-28 13:29 paragrep-3.2.1/paragrep.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 19-Aug-28 13:29 paragrep-3.2.1/paragrep/
--rw-r--r--  2.0 unx     1651 b- defN 19-Aug-28 13:29 paragrep-3.2.1/PKG-INFO
--rw-r--r--  2.0 unx     1611 b- defN 12-Mar-24 10:00 paragrep-3.2.1/LICENSE
--rw-r--r--  2.0 unx       47 b- defN 09-Jul-13 10:49 paragrep-3.2.1/MANIFEST.in
--rw-r--r--  2.0 unx      698 b- defN 19-Feb-12 14:52 paragrep-3.2.1/README.md
--rw-r--r--  2.0 unx     1906 b- defN 19-Aug-28 13:26 paragrep-3.2.1/setup.py
--rw-r--r--  2.0 unx       61 b- defN 19-Aug-28 13:29 paragrep-3.2.1/setup.cfg
--rw-r--r--  2.0 unx     6313 b- defN 09-Jul-13 10:49 paragrep-3.2.1/man/paragrep.1
--rw-r--r--  2.0 unx     1651 b- defN 19-Aug-28 13:29 paragrep-3.2.1/paragrep.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      278 b- defN 19-Aug-28 13:29 paragrep-3.2.1/paragrep.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       42 b- defN 19-Aug-28 13:29 paragrep-3.2.1/paragrep.egg-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 19-Aug-28 13:29 paragrep-3.2.1/paragrep.egg-info/requires.txt
--rw-r--r--  2.0 unx        9 b- defN 19-Aug-28 13:29 paragrep-3.2.1/paragrep.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 19-Aug-28 13:29 paragrep-3.2.1/paragrep.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx    10343 b- defN 19-Aug-28 13:28 paragrep-3.2.1/paragrep/__init__.py
-18 files, 24622 bytes uncompressed, 8889 bytes compressed:  63.9%
+Zip file size: 11151 bytes, number of entries: 17
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 00:42 paragrep-3.2.3/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 00:42 paragrep-3.2.3/man/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 00:42 paragrep-3.2.3/paragrep.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 00:42 paragrep-3.2.3/paragrep/
+-rw-r--r--  2.0 unx     1450 b- defN 23-May-24 00:42 paragrep-3.2.3/PKG-INFO
+-rw-r--r--  2.0 unx     1611 b- defN 12-Mar-24 10:00 paragrep-3.2.3/LICENSE
+-rw-r--r--  2.0 unx       47 b- defN 09-Jul-13 10:49 paragrep-3.2.3/MANIFEST.in
+-rw-r--r--  2.0 unx      698 b- defN 19-Feb-12 14:52 paragrep-3.2.3/README.md
+-rw-r--r--  2.0 unx     1874 b- defN 23-May-24 00:39 paragrep-3.2.3/setup.py
+-rw-r--r--  2.0 unx       61 b- defN 23-May-24 00:42 paragrep-3.2.3/setup.cfg
+-rw-r--r--  2.0 unx     6313 b- defN 09-Jul-13 10:49 paragrep-3.2.3/man/paragrep.1
+-rw-r--r--  2.0 unx     1450 b- defN 23-May-24 00:42 paragrep-3.2.3/paragrep.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx      247 b- defN 23-May-24 00:42 paragrep-3.2.3/paragrep.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       43 b- defN 23-May-24 00:42 paragrep-3.2.3/paragrep.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-May-24 00:42 paragrep-3.2.3/paragrep.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-24 00:42 paragrep-3.2.3/paragrep.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx    10286 b- defN 23-May-24 00:40 paragrep-3.2.3/paragrep/__init__.py
+17 files, 24090 bytes uncompressed, 8777 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -1,55 +1,52 @@
-Filename: paragrep-3.2.1/
+Filename: paragrep-3.2.3/
 Comment: 
 
-Filename: paragrep-3.2.1/man/
+Filename: paragrep-3.2.3/man/
 Comment: 
 
-Filename: paragrep-3.2.1/paragrep.egg-info/
+Filename: paragrep-3.2.3/paragrep.egg-info/
 Comment: 
 
-Filename: paragrep-3.2.1/paragrep/
+Filename: paragrep-3.2.3/paragrep/
 Comment: 
 
-Filename: paragrep-3.2.1/PKG-INFO
+Filename: paragrep-3.2.3/PKG-INFO
 Comment: 
 
-Filename: paragrep-3.2.1/LICENSE
+Filename: paragrep-3.2.3/LICENSE
 Comment: 
 
-Filename: paragrep-3.2.1/MANIFEST.in
+Filename: paragrep-3.2.3/MANIFEST.in
 Comment: 
 
-Filename: paragrep-3.2.1/README.md
+Filename: paragrep-3.2.3/README.md
 Comment: 
 
-Filename: paragrep-3.2.1/setup.py
+Filename: paragrep-3.2.3/setup.py
 Comment: 
 
-Filename: paragrep-3.2.1/setup.cfg
+Filename: paragrep-3.2.3/setup.cfg
 Comment: 
 
-Filename: paragrep-3.2.1/man/paragrep.1
+Filename: paragrep-3.2.3/man/paragrep.1
 Comment: 
 
-Filename: paragrep-3.2.1/paragrep.egg-info/PKG-INFO
+Filename: paragrep-3.2.3/paragrep.egg-info/PKG-INFO
 Comment: 
 
-Filename: paragrep-3.2.1/paragrep.egg-info/SOURCES.txt
+Filename: paragrep-3.2.3/paragrep.egg-info/SOURCES.txt
 Comment: 
 
-Filename: paragrep-3.2.1/paragrep.egg-info/entry_points.txt
+Filename: paragrep-3.2.3/paragrep.egg-info/entry_points.txt
 Comment: 
 
-Filename: paragrep-3.2.1/paragrep.egg-info/requires.txt
+Filename: paragrep-3.2.3/paragrep.egg-info/top_level.txt
 Comment: 
 
-Filename: paragrep-3.2.1/paragrep.egg-info/top_level.txt
+Filename: paragrep-3.2.3/paragrep.egg-info/dependency_links.txt
 Comment: 
 
-Filename: paragrep-3.2.1/paragrep.egg-info/dependency_links.txt
-Comment: 
-
-Filename: paragrep-3.2.1/paragrep/__init__.py
+Filename: paragrep-3.2.3/paragrep/__init__.py
 Comment: 
 
 Zip file comment:
```

## Comparing `paragrep-3.2.1/PKG-INFO` & `paragrep-3.2.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: paragrep
-Version: 3.2.1
+Version: 3.2.3
 Summary: Print paragraphs matching regular expressions
 Home-page: http://software.clapper.org/paragrep/
 Author: Brian M. Clapper
 Author-email: bmc@clapper.org
 License: BSD-style license
-Description: 
-        paragrep - Paragraph Grep utility
-        
-        **paragrep** is a paragraph grep utility. It searches for a series of regular
-        expressions in a text file (or several text files) and prints out the
-        paragraphs containing those expressions. Normally **paragrep** displays a
-        paragraph if it contains any of the expressions; this behavior can be modified
-        by using the `-a` option.
-        
-        By default, a paragraph is defined as a block of text delimited by an empty or
-        blank line; this behavior can be altered with the `-p` option.
-        
-        If no files are specified on the command line, **paragrep** searches
-        standard input.
-        
-        This is the third implementation of **paragrep**. The first implementation,
-        in 1989, was in C. The second implementation, in 2003, was in perl. This is
-        the latest and greatest.
-        
-        For help, run with `-h`.
-        
-        For detailed documentation, see <http://software.clapper.org/paragrep/>
-        
-        This software is released under a BSD license.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Utilities
+License-File: LICENSE
+
+
+paragrep - Paragraph Grep utility
+
+**paragrep** is a paragraph grep utility. It searches for a series of regular
+expressions in a text file (or several text files) and prints out the
+paragraphs containing those expressions. Normally **paragrep** displays a
+paragraph if it contains any of the expressions; this behavior can be modified
+by using the `-a` option.
+
+By default, a paragraph is defined as a block of text delimited by an empty or
+blank line; this behavior can be altered with the `-p` option.
+
+If no files are specified on the command line, **paragrep** searches
+standard input.
+
+This is the third implementation of **paragrep**. The first implementation,
+in 1989, was in C. The second implementation, in 2003, was in perl. This is
+the latest and greatest.
+
+For help, run with `-h`.
+
+For detailed documentation, see <http://software.clapper.org/paragrep/>
+
+This software is released under a BSD license.
```

## Comparing `paragrep-3.2.1/LICENSE` & `paragrep-3.2.3/LICENSE`

 * *Files identical despite different names*

## Comparing `paragrep-3.2.1/README.md` & `paragrep-3.2.3/README.md`

 * *Files identical despite different names*

## Comparing `paragrep-3.2.1/setup.py` & `paragrep-3.2.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,17 +40,15 @@
        long_description = paragrep.__doc__,
        packages         = find_packages(),
        url              = paragrep.__url__,
        license          = paragrep.__license__,
        author           = paragrep.__author__,
        author_email     = paragrep.__email__,
        entry_points     = {'console_scripts' : 'paragrep=paragrep:main'},
-       install_requires = [
-           "Click==7.0"
-       ],
+       install_requires = [],
        data_files       = [('man', ['man/paragrep.1'])],
        classifiers = [
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python',
         'Topic :: Text Processing :: Filters',
```

## Comparing `paragrep-3.2.1/man/paragrep.1` & `paragrep-3.2.3/man/paragrep.1`

 * *Files identical despite different names*

## Comparing `paragrep-3.2.1/paragrep.egg-info/PKG-INFO` & `paragrep-3.2.3/paragrep.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: paragrep
-Version: 3.2.1
+Version: 3.2.3
 Summary: Print paragraphs matching regular expressions
 Home-page: http://software.clapper.org/paragrep/
 Author: Brian M. Clapper
 Author-email: bmc@clapper.org
 License: BSD-style license
-Description: 
-        paragrep - Paragraph Grep utility
-        
-        **paragrep** is a paragraph grep utility. It searches for a series of regular
-        expressions in a text file (or several text files) and prints out the
-        paragraphs containing those expressions. Normally **paragrep** displays a
-        paragraph if it contains any of the expressions; this behavior can be modified
-        by using the `-a` option.
-        
-        By default, a paragraph is defined as a block of text delimited by an empty or
-        blank line; this behavior can be altered with the `-p` option.
-        
-        If no files are specified on the command line, **paragrep** searches
-        standard input.
-        
-        This is the third implementation of **paragrep**. The first implementation,
-        in 1989, was in C. The second implementation, in 2003, was in perl. This is
-        the latest and greatest.
-        
-        For help, run with `-h`.
-        
-        For detailed documentation, see <http://software.clapper.org/paragrep/>
-        
-        This software is released under a BSD license.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Utilities
+License-File: LICENSE
+
+
+paragrep - Paragraph Grep utility
+
+**paragrep** is a paragraph grep utility. It searches for a series of regular
+expressions in a text file (or several text files) and prints out the
+paragraphs containing those expressions. Normally **paragrep** displays a
+paragraph if it contains any of the expressions; this behavior can be modified
+by using the `-a` option.
+
+By default, a paragraph is defined as a block of text delimited by an empty or
+blank line; this behavior can be altered with the `-p` option.
+
+If no files are specified on the command line, **paragrep** searches
+standard input.
+
+This is the third implementation of **paragrep**. The first implementation,
+in 1989, was in C. The second implementation, in 2003, was in perl. This is
+the latest and greatest.
+
+For help, run with `-h`.
+
+For detailed documentation, see <http://software.clapper.org/paragrep/>
+
+This software is released under a BSD license.
```

## Comparing `paragrep-3.2.1/paragrep/__init__.py` & `paragrep-3.2.3/paragrep/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,50 +21,49 @@
 
 For detailed documentation, see <http://software.clapper.org/paragrep/>
 
 This software is released under a BSD license.
 """
 
 # Info about the module
-__version__   = '3.2.1'
+__version__   = '3.2.3'
 __author__    = 'Brian M. Clapper'
 __email__     = 'bmc@clapper.org'
 __url__       = 'http://software.clapper.org/paragrep/'
-__copyright__ = '1989-2012 Brian M. Clapper'
+__copyright__ = '1989-2023 Brian M. Clapper'
 __license__   = 'BSD-style license'
 
 # Package stuff
 
 __all__     = ['Paragrepper', 'main']
 
 # ---------------------------------------------------------------------------
 # Imports
 # ---------------------------------------------------------------------------
 
 import sys
 import os
 import re
 from typing import Sequence, Optional, TextIO, NoReturn
-import click
 
 # ---------------------------------------------------------------------------
 # Constants
 # ---------------------------------------------------------------------------
 
-FULL_VERSION_STRING = 'paragrep, Version %s. Copyright %s' %\
-                    (__version__, __copyright__)
+FULL_VERSION_STRING = (f'paragrep, Version {__version__}. '
+                       f'Copyright {__copyright__}')
 
 # ---------------------------------------------------------------------------
 # Classes
 # ---------------------------------------------------------------------------
 
 class ParagrepError(Exception):
     pass
 
-class Paragrepper(object):
+class Paragrepper:
     """
     Grep through a file, printing paragraphs that match one or more regular
     expressions.
     """
     def __init__(self):
         self.regexps = []
         self.files = None
@@ -186,15 +185,15 @@
                 for l in f.readlines():
                     result += [l.strip()]
         except IOError as e:
             raise ParagrepError(f'''Can't open file "{file}": {e}''')
 
     return result
 
-def _parse_params(paragrepper: Paragrepper, argv: Sequence[str]) -> NoReturn:
+def _parse_params(paragrepper: Paragrepper, argv: Sequence[str]) -> None:
     # Parse the command-line parameters
 
     prog = os.path.basename(argv[0])
     USAGE = (
 f'''
 {prog} [-iv] [-p EOP_REGEXP] regexp [file] ...
 {prog} [-aiov] [-p EOP_REGEXP] [-e REGEXP] ... [-f EXP_FILE] ... [file] ...
@@ -251,16 +250,15 @@
             parser.error(e.message)
 
     # Try to compile the end-of-paragraph regular expression.
 
     try:
         paragrepper.eop_regexp = re.compile(options.eop_regexp)
     except Exception as e:
-        parser.error('Bad regular expression "%s" to -p option' % \
-                     options.eop_regexp)
+        parser.error(f'Bad regular expression "{options.eop_regexp}" to -p')
 
     args = args[1:]
     if len(uncompiled_regexps) == 0:
         # No -e or -f seen. Use first non-option parameter.
 
         try:
             uncompiled_regexps += [args[0]]
@@ -275,15 +273,15 @@
         try:
             if flags:
                 re_args = (expr, flags)
             else:
                 re_args = (expr,)
             paragrepper.regexps += [re.compile(*re_args)]
         except Exception as e:
-            parser.error('Bad regular expression: "%s"' % expr)
+            parser.error(f'Bad regular expression: "{expr}"')
 
     # Are there any files, or are we searching standard input?
 
     if len(args) > 0:
         paragrepper.files = args
 
 def main() -> NoReturn:
```

