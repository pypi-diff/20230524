# Comparing `tmp/cdo-1.5.7.tar.gz` & `tmp/cdo-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdo-1.5.7.tar", last modified: Fri Oct 14 07:56:19 2022, max compression
+gzip compressed data, was "cdo-1.6.0.tar", last modified: Wed May 24 13:30:05 2023, max compression
```

## Comparing `cdo-1.5.7.tar` & `cdo-1.6.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxr-x   0 ram       (1000) ram       (1000)        0 2022-10-14 07:56:19.311410 cdo-1.5.7/
--rw-rw-r--   0 ram       (1000) ram       (1000)    13711 2022-10-14 07:56:19.308077 cdo-1.5.7/PKG-INFO
-drwxrwxr-x   0 ram       (1000) ram       (1000)        0 2022-10-14 07:56:19.308077 cdo-1.5.7/cdo.egg-info/
--rw-rw-r--   0 ram       (1000) ram       (1000)    13711 2022-10-14 07:56:18.000000 cdo-1.5.7/cdo.egg-info/PKG-INFO
--rw-rw-r--   0 ram       (1000) ram       (1000)      166 2022-10-14 07:56:19.000000 cdo-1.5.7/cdo.egg-info/SOURCES.txt
--rw-rw-r--   0 ram       (1000) ram       (1000)        1 2022-10-14 07:56:18.000000 cdo-1.5.7/cdo.egg-info/dependency_links.txt
--rw-rw-r--   0 ram       (1000) ram       (1000)       52 2022-10-14 07:56:19.000000 cdo-1.5.7/cdo.egg-info/requires.txt
--rw-rw-r--   0 ram       (1000) ram       (1000)        4 2022-10-14 07:56:19.000000 cdo-1.5.7/cdo.egg-info/top_level.txt
--rw-rw-r--   0 ram       (1000) ram       (1000)    29404 2022-10-13 09:02:37.000000 cdo-1.5.7/cdo.py
--rw-rw-r--   0 ram       (1000) ram       (1000)       38 2022-10-14 07:56:19.311410 cdo-1.5.7/setup.cfg
--rw-rw-r--   0 ram       (1000) ram       (1000)     3685 2022-10-13 09:02:06.000000 cdo-1.5.7/setup.py
-drwxrwxr-x   0 ram       (1000) ram       (1000)        0 2022-10-14 07:56:19.308077 cdo-1.5.7/test/
--rw-rw-r--   0 ram       (1000) ram       (1000)    40710 2022-10-14 07:48:29.000000 cdo-1.5.7/test/test_cdo.py
+drwxrwxr-x   0 ram       (1000) ram       (1000)        0 2023-05-24 13:30:05.635396 cdo-1.6.0/
+-rw-rw-r--   0 ram       (1000) ram       (1000)    14332 2023-05-24 13:30:05.635396 cdo-1.6.0/PKG-INFO
+-rw-rw-r--   0 ram       (1000) ram       (1000)       89 2020-12-22 09:00:50.000000 cdo-1.6.0/buildAndUpload
+drwxrwxr-x   0 ram       (1000) ram       (1000)        0 2023-05-24 13:30:05.635396 cdo-1.6.0/cdo/
+-rw-rw-r--   0 ram       (1000) ram       (1000)      123 2023-05-24 13:23:13.000000 cdo-1.6.0/cdo/__init__.py
+-rw-rw-r--   0 ram       (1000) ram       (1000)    32544 2023-05-24 12:57:03.000000 cdo-1.6.0/cdo/cdo.py
+drwxrwxr-x   0 ram       (1000) ram       (1000)        0 2023-05-24 13:30:05.635396 cdo-1.6.0/cdo.egg-info/
+-rw-rw-r--   0 ram       (1000) ram       (1000)    14332 2023-05-24 13:30:05.000000 cdo-1.6.0/cdo.egg-info/PKG-INFO
+-rw-rw-r--   0 ram       (1000) ram       (1000)      201 2023-05-24 13:30:05.000000 cdo-1.6.0/cdo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ram       (1000) ram       (1000)        1 2023-05-24 13:30:05.000000 cdo-1.6.0/cdo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ram       (1000) ram       (1000)       52 2023-05-24 13:30:05.000000 cdo-1.6.0/cdo.egg-info/requires.txt
+-rw-rw-r--   0 ram       (1000) ram       (1000)        4 2023-05-24 13:30:05.000000 cdo-1.6.0/cdo.egg-info/top_level.txt
+-rw-rw-r--   0 ram       (1000) ram       (1000)       38 2023-05-24 13:30:05.635396 cdo-1.6.0/setup.cfg
+-rw-rw-r--   0 ram       (1000) ram       (1000)     3634 2023-05-24 13:23:08.000000 cdo-1.6.0/setup.py
+drwxrwxr-x   0 ram       (1000) ram       (1000)        0 2023-05-24 13:30:05.635396 cdo-1.6.0/test/
+-rw-rw-r--   0 ram       (1000) ram       (1000)    44226 2023-05-24 13:09:23.000000 cdo-1.6.0/test/test_cdo.py
```

### Comparing `cdo-1.5.7/PKG-INFO` & `cdo-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 Metadata-Version: 2.1
 Name: cdo
-Version: 1.5.7
+Version: 1.6.0
 Summary: python bindings to CDO
 Home-page: https://code.mpimet.mpg.de/projects/cdo/wiki/Cdo%7Brbpy%7D
 Author: Ralf Mueller
 Author-email: stark.dreamdetective@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=2.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: Numpy output
 Provides-Extra: XArray output
 
 
 # Cdo.{rb,py} - Use Ruby/Python to access the power of CDO
 
 [![Tests](https://circleci.com/gh/Try2Code/cdo-bindings/tree/master.svg?style=shield)](https://circleci.com/gh/Try2Code/cdo-bindings)
 
-Welcome to the scripting interfaces of [CDO](https://code.zmaw.de/projects/cdo/wiki)!
+Welcome to the scripting interfaces of [CDO](https://code.mpimet.mpg.de/projects/cdo/wiki)!
 This repository contains interfaces for [Ruby](http://www.ruby-lang.org) and [Python](https://www.python.org). If you are not sure, wether this is useful or not, please have a look at:
-[Why the .... should I use this???](https://code.zmaw.de/projects/cdo/wiki/Cdo%7Brbpy%7D#Why-the-)
+[Why the .... should I use this???](https://code.mpimet.mpg.de/projects/cdo/wiki/Cdo%7Brbpy%7D#Why-the-)
 
 ## What's going on
 
 Currently this package is in a re-design phase. The target is a 2.0 release that will **not be compatible** with the exising release 1.5.x:
 * Write operator chains like methods chains with ```.``` as much as possible
 * hopefully reduce the number of ```kwargs``` keys
 * keep the Ruby and Python interface similar
@@ -43,14 +40,15 @@
 *  Ruby
 ```
     gem install cdo (--user-install)
 ```
 *  Python
 ```
     pip install cdo (--user)
+    conda -c conda-forge install python-cdo
 ```
 
 ### Requirements
 
 Cdo.{rb,py} requires a working CDO binary and Ruby 2.x or Python 2.7/3.x
 
 **PLEASE NOTE: python-2.7 is unmaintained since January 2021**
@@ -200,15 +198,15 @@
 *) If you use scipy >= 0.14 as netcdf backend, you have to use following code
 instead to avoid possible segmentation faults:
 ```python
     cdf = cdo.fldmin(input = ifile,returnCdf = True)
     temperatures = cdf.variables['T'][:]
 ```
 More examples can be found in test/cdo-examples.rb and [on the
-homepage](https://code.zmaw.de/projects/cdo/wiki/Cdo%7Brbpy%7D)
+homepage](https://code.mpimet.mpg.de/projects/cdo/wiki/Cdo%7Brbpy%7D)
 
 ### Avoid re-processing
 
 If you do not want to re-compute files, you can set
 
 *  the instance attribute 'forceOutput' to false: this will effect all later
    call of that instance **or**
@@ -216,22 +214,34 @@
    operator call of this instance
 
 For more information, please have a look at the unit tests.
 
 ## Support, Issues, Bugs, ...
 
 Please use the forum or ticket system of CDOs official web page:
-http://code.zmaw.de/projects/cdo
+http://code.mpimet.mpg.de/projects/cdo
 
 ## Changelog
+* **next 2.0**:
+  - reduced usage of keywords:
+    - many of them just set return type, so they will go to the _run()_ method
+    - options only has effect during run of the tool, so this can also go into _run()_
+    - the different input types can be handled in something like _input()_ or
+* **1.6.0**:
+  - merged pull requests regarding threading, signal and tempfile handling
+  - added support for xarray/xdataset input AND output at the same time (request by Pauline Millet)
 * **1.5.6**:
   - slight adoptions for CDO-2.0.0
   - limitted support for python-2.7: many other libs dropped support for it so I can only do limitted testing
   - new API: `cdo.config` holds a dictionary/hash with built-in CDO features (availble sind CDO-1.9.x), empty otherwise
   - removed cdo.hasLib() and cdo.libsVersion(): relied on unstable output of `cdo -V`. use cdo.config instead
+      _infiles()_. This should clean up the lengthy code, which does this
+      currently
+* **1.5.4(python-only)**:
+  - bugfix release for @pgierz regarding #30
 * **1.5.1(ruby-only)**:
   - fix some warnings with latest ruby release 2.7.x
 * **1.5.0(ruby)/1.5.3(python)** API change :
   - simplify the interface:
     - remove returnCdf from constructor, only use it with operator calls
     - remove methods setReturnArray/unsetReturnArray: I fear it's not used anyway, but 'returnArray' in each call
     - remove the optional dependency to scipy since it offers less functionality than netCDF4 and just blows up the code
@@ -314,9 +324,7 @@
 ---
 
 ## [Thanks to all contributors!](https://github.com/Try2Code/cdo-bindings/graphs/contributors)
 
 ## License
 
 Cdo.{rb,py} makes use of the BSD-3-clause license
-
-
```

### Comparing `cdo-1.5.7/cdo.egg-info/PKG-INFO` & `cdo-1.6.0/cdo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 Metadata-Version: 2.1
 Name: cdo
-Version: 1.5.7
+Version: 1.6.0
 Summary: python bindings to CDO
 Home-page: https://code.mpimet.mpg.de/projects/cdo/wiki/Cdo%7Brbpy%7D
 Author: Ralf Mueller
 Author-email: stark.dreamdetective@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=2.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: Numpy output
 Provides-Extra: XArray output
 
 
 # Cdo.{rb,py} - Use Ruby/Python to access the power of CDO
 
 [![Tests](https://circleci.com/gh/Try2Code/cdo-bindings/tree/master.svg?style=shield)](https://circleci.com/gh/Try2Code/cdo-bindings)
 
-Welcome to the scripting interfaces of [CDO](https://code.zmaw.de/projects/cdo/wiki)!
+Welcome to the scripting interfaces of [CDO](https://code.mpimet.mpg.de/projects/cdo/wiki)!
 This repository contains interfaces for [Ruby](http://www.ruby-lang.org) and [Python](https://www.python.org). If you are not sure, wether this is useful or not, please have a look at:
-[Why the .... should I use this???](https://code.zmaw.de/projects/cdo/wiki/Cdo%7Brbpy%7D#Why-the-)
+[Why the .... should I use this???](https://code.mpimet.mpg.de/projects/cdo/wiki/Cdo%7Brbpy%7D#Why-the-)
 
 ## What's going on
 
 Currently this package is in a re-design phase. The target is a 2.0 release that will **not be compatible** with the exising release 1.5.x:
 * Write operator chains like methods chains with ```.``` as much as possible
 * hopefully reduce the number of ```kwargs``` keys
 * keep the Ruby and Python interface similar
@@ -43,14 +40,15 @@
 *  Ruby
 ```
     gem install cdo (--user-install)
 ```
 *  Python
 ```
     pip install cdo (--user)
+    conda -c conda-forge install python-cdo
 ```
 
 ### Requirements
 
 Cdo.{rb,py} requires a working CDO binary and Ruby 2.x or Python 2.7/3.x
 
 **PLEASE NOTE: python-2.7 is unmaintained since January 2021**
@@ -200,15 +198,15 @@
 *) If you use scipy >= 0.14 as netcdf backend, you have to use following code
 instead to avoid possible segmentation faults:
 ```python
     cdf = cdo.fldmin(input = ifile,returnCdf = True)
     temperatures = cdf.variables['T'][:]
 ```
 More examples can be found in test/cdo-examples.rb and [on the
-homepage](https://code.zmaw.de/projects/cdo/wiki/Cdo%7Brbpy%7D)
+homepage](https://code.mpimet.mpg.de/projects/cdo/wiki/Cdo%7Brbpy%7D)
 
 ### Avoid re-processing
 
 If you do not want to re-compute files, you can set
 
 *  the instance attribute 'forceOutput' to false: this will effect all later
    call of that instance **or**
@@ -216,22 +214,34 @@
    operator call of this instance
 
 For more information, please have a look at the unit tests.
 
 ## Support, Issues, Bugs, ...
 
 Please use the forum or ticket system of CDOs official web page:
-http://code.zmaw.de/projects/cdo
+http://code.mpimet.mpg.de/projects/cdo
 
 ## Changelog
+* **next 2.0**:
+  - reduced usage of keywords:
+    - many of them just set return type, so they will go to the _run()_ method
+    - options only has effect during run of the tool, so this can also go into _run()_
+    - the different input types can be handled in something like _input()_ or
+* **1.6.0**:
+  - merged pull requests regarding threading, signal and tempfile handling
+  - added support for xarray/xdataset input AND output at the same time (request by Pauline Millet)
 * **1.5.6**:
   - slight adoptions for CDO-2.0.0
   - limitted support for python-2.7: many other libs dropped support for it so I can only do limitted testing
   - new API: `cdo.config` holds a dictionary/hash with built-in CDO features (availble sind CDO-1.9.x), empty otherwise
   - removed cdo.hasLib() and cdo.libsVersion(): relied on unstable output of `cdo -V`. use cdo.config instead
+      _infiles()_. This should clean up the lengthy code, which does this
+      currently
+* **1.5.4(python-only)**:
+  - bugfix release for @pgierz regarding #30
 * **1.5.1(ruby-only)**:
   - fix some warnings with latest ruby release 2.7.x
 * **1.5.0(ruby)/1.5.3(python)** API change :
   - simplify the interface:
     - remove returnCdf from constructor, only use it with operator calls
     - remove methods setReturnArray/unsetReturnArray: I fear it's not used anyway, but 'returnArray' in each call
     - remove the optional dependency to scipy since it offers less functionality than netCDF4 and just blows up the code
@@ -314,9 +324,7 @@
 ---
 
 ## [Thanks to all contributors!](https://github.com/Try2Code/cdo-bindings/graphs/contributors)
 
 ## License
 
 Cdo.{rb,py} makes use of the BSD-3-clause license
-
-
```

### Comparing `cdo-1.5.7/cdo.py` & `cdo-1.6.0/cdo/cdo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import os
 import re
 import subprocess
 import tempfile
 import random
 import glob
 import signal
+import threading
+import functools
 from pkg_resources import parse_version
 from io import StringIO
 import logging as pyLog
 import six
 import sys
 import threading
 import json
 try:
-    from shutil import which
+    from shutil import which, get_terminal_size
 except ImportError:
     from backports.shutil_which import which
 
 # workaround for python2/3 string handling {{{
 try:
-  from string import strip
+    from string import strip
 except ImportError:
-  strip = str.strip
-#}}}
+    strip = str.strip
+# }}}
 
-# Copyright 2011-2019 Ralf Mueller, ralf.mueller@dkrz.de {{{
+# Copyright 2011-2023 Ralf Mueller, ralf.mueller@dkrz.de {{{
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
 # 2. Redistributions in binary form must reproduce the above copyright notice,
@@ -47,806 +49,819 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 # }}}
 
-CDO_PY_VERSION = "1.5.7"
-
 # build interactive documentation: help(cdo.sinfo) {{{
-def auto_doc(tool, path2cdo):
-  """Generate the __doc__ string of the decorated function by calling the cdo help command
-  use like this:
-    c = cdo.Cdo()
-    help(c.sinfov)"""
-  def desc(func):
-    func.__doc__ = operator_doc(tool, path2cdo)
-    return func
-  return desc
-#}}}
 
 def operator_doc(tool, path2cdo):
     proc = subprocess.Popen('%s -h %s ' % (path2cdo, tool),
                             shell=True,
                             stderr=subprocess.PIPE,
                             stdout=subprocess.PIPE)
     retvals = proc.communicate()
     return retvals[0].decode("utf-8")
+# }}}
+
+# return the cdo version {{{
 
-# some helper functions without side effects {{{
 def getCdoVersion(path2cdo, verbose=False):
-  proc = subprocess.Popen([path2cdo, '-V'], stderr=subprocess.PIPE, stdout=subprocess.PIPE)
-  ret = proc.communicate()
+    proc = subprocess.Popen(
+        [path2cdo, '-V'], stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+    retvals = proc.communicate()
+    cdo_help = retvals[0].decode("utf-8")
+    if verbose:
+        return cdo_help
+    match = re.search(r"Climate Data Operators version (\d.*) .*", cdo_help)
+    return match.group(1)
+
+# helper function without side effects {{{
 
-  cdo_help_stdout = ret[0].decode("utf-8")
-  cdo_help_stderr = ret[1].decode("utf-8")
+def setupLogging(logFile):
+    logger = pyLog.getLogger(__name__)
+    logger.setLevel(pyLog.INFO)
 
-  # there was a change in cdo-2.0.0 to print out more to stdout instead of stderr
-  # so both have to be checked
-  match_stdout = re.search("Climate Data Operators version (\d.*) .*", cdo_help_stdout)
-  match_stderr = re.search("Climate Data Operators version (\d.*) .*", cdo_help_stderr)
-
-  if (None == match_stderr):
-    if (None == match_stdout):
-      raise CDOException(*ret)
+    if isinstance(logFile, six.string_types):
+        handler = pyLog.FileHandler(logFile)
     else:
-      return match_stdout.group(1)
-  else:
-    return match_stderr.group(1)
-  if verbose:
-    return cdo_help
-  match = re.search("Climate Data Operators version (\d.*) .*", cdo_help)
-  return match.group(1)
+        handler = pyLog.StreamHandler(stream=logFile)
 
-def setupLogging(logFile):
-  logger = pyLog.getLogger(__name__)
-  logger.setLevel(pyLog.INFO)
+    formatter = pyLog.Formatter('%(asctime)s - %(levelname)s - %(message)s')
+    handler.setFormatter(formatter)
+    logger.addHandler(handler)
 
-  if isinstance(logFile, six.string_types):
-    handler = pyLog.FileHandler(logFile)
-  else:
-    handler = pyLog.StreamHandler(stream=logFile)
-
-  formatter = pyLog.Formatter('%(asctime)s - %(levelname)s - %(message)s')
-  handler.setFormatter(formatter)
-  logger.addHandler(handler)
+    return logger
+# }}}
 
-  return logger
-#}}}
+# extra exceptions for CDO {{{
 
-# extra execptions for CDO {{{
 class CDOException(Exception):
 
-  def __init__(self, stdout, stderr, returncode, msg=''):
-    super(CDOException, self).__init__()
-    self.stdout = stdout
-    self.stderr = stderr
-    self.returncode = returncode
-    self.msg = '(returncode:%s) %s :: %s' % (returncode, stderr,msg)
+    def __init__(self, stdout, stderr, returncode):
+        super(CDOException, self).__init__()
+        self.stdout = stdout
+        self.stderr = stderr
+        self.returncode = returncode
+        self.msg = '(returncode:%s) %s' % (returncode, stderr)
 
-  def __str__(self):
-    return self.msg
+    def __str__(self):
+        return self.msg
 # }}}
 
 # MAIN Cdo class {{{
+
 class Cdo(object):
 
-  # fallback operator lists {{{
-  NoOutputOperators = 'cdiread cmor codetab conv_cmor_table diff diffc diffn \
-  diffp diffv dump_cmor_table dumpmap filedes gmtcells gmtxyz gradsdes griddes \
-  griddes2 gridverify info infoc infon infop infos infov map ncode ndate \
-  ngridpoints ngrids nlevel nmon npar ntime nvar nyear output outputarr \
-  outputbounds outputboundscpt outputcenter outputcenter2 outputcentercpt \
-  outputext outputf outputfld outputint outputkey outputsrv outputtab outputtri \
-  outputts outputvector outputvrml outputxyz pardes partab partab2 seinfo \
-  seinfoc seinfon seinfop showattribute showatts showattsglob showattsvar \
-  showcode showdate showformat showgrid showlevel showltype showmon showname \
-  showparam showstdname showtime showtimestamp showunit showvar showyear sinfo \
-  sinfoc sinfon sinfop sinfov spartab specinfo tinfo vardes vct vct2 verifygrid \
-  vlist xinfon zaxisdes'.split()
-  TwoOutputOperators = 'trend samplegridicon mrotuv eoftime \
-  eofspatial eof3dtime eof3dspatial eof3d eof complextorect complextopol'.split()
-  MoreOutputOperators = 'distgrid eofcoeff eofcoeff3d intyear scatter splitcode \
-  splitday splitgrid splithour splitlevel splitmon splitname splitparam splitrec \
-  splitseas splitsel splittabnum splitvar splityear splityearmon splitzaxis'.split()
-  AliasOperators = {'seq':'for'}
-
-  # the following operators introduce additional new lines in cdo-2.0.0 for
-  # increased readability in the therminal. This leads to inconsistens parsing
-  # behaviour here because before new lines indicated meta data for a new
-  # variable for all show* operators.
-  ShowTimeOperators = 'showdate showtime showtimestamp showyear showmon'.split()
-  # operators are now called with '-s' to ease the parsing process. diff* does
-  # not print the errors when '-s' is given, so these operators need special
-  # treatment
-  # avoiding '-s' can lead to errors when working with operators which write to
-  # stdout, but it can done with cdo.silent = False
-  DiffOperators = 'diff diffc diffn diffv diffp'.split()
-  #}}}
-
-  name = ''
-
-  def __init__(self,
-               cdo='cdo',
-               returnNoneOnError=False,
-               forceOutput=True,
-               env=os.environ,
-               debug=False,
-               tempdir=tempfile.gettempdir(),
-               logging=False,
-               logFile=StringIO(),
-               cmd=[],
-               options=[],
-               silent=True):
+    # fallback operator lists {{{
+    NoOutputOperators = 'cdiread cmor codetab conv_cmor_table diff diffc diffn \
+    diffp diffv dump_cmor_table dumpmap filedes gmtcells gmtxyz gradsdes griddes \
+    griddes2 gridverify info infoc infon infop infos infov map ncode ndate \
+    ngridpoints ngrids nlevel nmon npar ntime nvar nyear output outputarr \
+    outputbounds outputboundscpt outputcenter outputcenter2 outputcentercpt \
+    outputext outputf outputfld outputint outputkey outputsrv outputtab outputtri \
+    outputts outputvector outputvrml outputxyz pardes partab partab2 seinfo \
+    seinfoc seinfon seinfop showattribute showatts showattsglob showattsvar \
+    showcode showdate showformat showgrid showlevel showltype showmon showname \
+    showparam showstdname showtime showtimestamp showunit showvar showyear sinfo \
+    sinfoc sinfon sinfop sinfov spartab specinfo tinfo vardes vct vct2 verifygrid \
+    vlist xinfon zaxisdes'.split()
+    TwoOutputOperators = 'trend samplegridicon mrotuv eoftime \
+    eofspatial eof3dtime eof3dspatial eof3d eof complextorect complextopol'.split()
+    MoreOutputOperators = 'distgrid eofcoeff eofcoeff3d intyear scatter splitcode \
+    splitday splitgrid splithour splitlevel splitmon splitname splitparam splitrec \
+    splitseas splitsel splittabnum splitvar splityear splityearmon splitzaxis'.split()
+    AliasOperators = {'seq': 'for'}
+
+    # the following operators introduce additional new lines in cdo-2.0.0 for
+    # increased readability in the therminal. This leads to inconsistens parsing
+    # behaviour here because before new lines indicated meta data for a new
+    # variable for all show* operators.
+    ShowTimeOperators = 'showdate showtime showtimestamp showyear showmon'.split()
+    # operators are now called with '-s' to ease the parsing process. diff* does
+    # not print the errors when '-s' is given, so these operators need special
+    # treatment
+    # avoiding '-s' can lead to errors when working with operators which write to
+    # stdout, but it can done with cdo.silent = False
+    DiffOperators = 'diff diffc diffn diffv diffp'.split()
+    # }}}
+
+    name = ''
+
+    def __init__(self,
+                 cdo='cdo',
+                 returnNoneOnError=False,
+                 forceOutput=True,
+                 env=os.environ,
+                 debug=False,
+                 tempdir=tempfile.gettempdir(),
+                 tempStore=None,
+                 logging=False,
+                 logFile=StringIO(),
+                 cmd=[],
+                 options=[],
+                 silent=True):
 
-    if 'CDO' in os.environ and os.path.isfile(os.environ['CDO']):
-      self.CDO = which(os.environ['CDO'])
-    else:
-      self.CDO = which(cdo)
+        if 'CDO' in os.environ and os.path.isfile(os.environ['CDO']):
+            self.CDO = os.environ['CDO']
+        else:
+            self.CDO = cdo
 
-    self._cmd = cmd
-    self._options = options
+        self._cmd = cmd
+        self._options = options
 
-    self.operators         = self.__getOperators()
-    self.noOutputOperators = [op for op in self.operators.keys() if 0 == self.operators[op]]
-    self.returnNoneOnError = returnNoneOnError
-    self.tempStore         = CdoTempfileStore(dir = tempdir)
-    self.forceOutput       = forceOutput
-    self.env               = env
-    self.debug             = True if 'DEBUG' in os.environ else debug
-    self.silent            = silent
-
-    # optional IO libraries for additional return types {{{
-    self.hasNetcdf         = False
-    self.hasXarray         = False
-    self.cdf               = None
-    self.xa_open           = None
-    self.__loadOptionalLibs()
-
-    self.logging = logging  # internal logging {{{
-    self.logFile = logFile
-    if (self.logging):
-        self.logger = setupLogging(self.logFile)  # }}}
-
-    # CDO build configuration available since cdo-1.9x
-    self.config = self.__getConfig()
-
-    # handling different exits from interactive sessions {{{
-    # python3 has threading.main_thread(), but python2 doesn't
-    if (2 == sys.version_info[0]): # check python major version
-      signal.signal(signal.SIGINT,  self.__catch__)
-      signal.signal(signal.SIGTERM, self.__catch__)
-      signal.signal(signal.SIGSEGV, self.__catch__)
-      signal.siginterrupt(signal.SIGINT,  False)
-      signal.siginterrupt(signal.SIGTERM, False)
-      signal.siginterrupt(signal.SIGSEGV, False)
-    else:
-      #   remove tempfiles from those sessions
-      if threading.current_thread() is threading.main_thread():
-        signal.signal(signal.SIGINT,  self.__catch__)
-        signal.signal(signal.SIGTERM, self.__catch__)
-        signal.signal(signal.SIGSEGV, self.__catch__)
-        signal.siginterrupt(signal.SIGINT,  False)
-        signal.siginterrupt(signal.SIGTERM, False)
-        signal.siginterrupt(signal.SIGSEGV, False)
-    # other left-overs can only be handled afterwards
-    # might be good to use the tempdir keyword to ease this, but deletion can
-    # be triggered using cleanTempDir() }}}
-
-  def __get__(self, instance, owner):
-    if instance is None:
-      return self
-    name = self.name
-    # CDO (version 1.9.6 and older) has an operator called 'for', which cannot
-    # called with 'cdo.for()' because 'for' is a keyword in python. 'for' is
-    # renamed to 'seq' in 1.9.7.
-    # This workaround translates all calls of 'seq' into for in case of
-    # versions prior tp 1.9.7
-    if name in self.AliasOperators.keys() and \
-      ( parse_version(getCdoVersion(self.CDO)) < parse_version('1.9.7') ):
-      name = self.AliasOperators[name]
-    return self.__class__(
-        instance.CDO,
-        instance.returnNoneOnError,
-        instance.forceOutput,
-        instance.env,
-        instance.debug,
-        instance.tempStore.dir,
-        instance.logging,
-        instance.logFile,
-        instance._cmd + ['-' + name],
-        instance._options,
-        instance.silent)
-
-  # from 1.9.6 onwards CDO returns 1 of diff* finds a difference
-  def __exit_success(self,operatorName):
-    if ( parse_version(getCdoVersion(self.CDO)) < parse_version('1.9.6') ):
-      return 0
-    if ( 'diff' != operatorName[0:4] ):
-      return 0
-    return 1
-
-  # read json formatted output of 'cdo --config all'
-  def __getConfig(self):
-    proc = subprocess.Popen([self.CDO, '--config','all'], stderr=subprocess.PIPE, stdout=subprocess.PIPE)
-    ret  = proc.communicate()
-    try:
-      return json.loads(ret[0].decode('utf-8'))
-    except:
-      return {}
-
-  # retrieve the list of operators from the CDO binary plus info out number of
-  # output streams
-  def __getOperators(self):  # {{{
-    operators = {}
-
-    version = parse_version(getCdoVersion(self.CDO))
-    if (version < parse_version('1.7.2')):
-      proc = subprocess.Popen([self.CDO, '-h'], stderr=subprocess.PIPE, stdout=subprocess.PIPE)
+        self.operators = self.__getOperators()
+        self.noOutputOperators = [op for op, num in self.operators.items() if 0 == num]
+        self.returnNoneOnError = returnNoneOnError
+        self.tempStore = tempStore or CdoTempfileStore(dir=tempdir)
+        self.forceOutput = forceOutput
+        self.env = env
+        self.debug = True if 'DEBUG' in os.environ else debug
+        self.silent = silent
+        self.libs = self.getSupportedLibs()
+
+        # optional IO libraries for additional return types {{{
+        self.hasNetcdf = False
+        self.hasXarray = False
+        self.cdf = None
+        self.xa_open = None
+        self.__loadOptionalLibs()
+
+        self.logging = logging  # internal logging {{{
+        self.logFile = logFile
+        if self.logging:
+            self.logger = setupLogging(self.logFile)  # }}}
+
+        # CDO build configuration available since cdo-1.9x
+        self.config = self.__getConfig()
+
+    def __get__(self, instance, owner):
+        if instance is None:
+            return self
+        name = self.name
+        # CDO (version 1.9.6 and older) has an operator called 'for', which cannot
+        # called with 'cdo.for()' because 'for' is a keyword in python. 'for' is
+        # renamed to 'seq' in 1.9.7.
+        # This workaround translates all calls of 'seq' into for in case of
+        # versions prior to 1.9.7
+        if name in self.AliasOperators and (
+                parse_version(getCdoVersion(self.CDO)) < parse_version('1.9.7')):
+            name = self.AliasOperators[name]
+        return self.__class__(
+            instance.CDO,
+            instance.returnNoneOnError,
+            instance.forceOutput,
+            instance.env,
+            instance.debug,
+            instance.tempStore.dir,
+            instance.tempStore,
+            instance.logging,
+            instance.logFile,
+            instance._cmd + ['-' + name],
+            instance._options,
+            instance.silent)
+
+    # from 1.9.6 onwards CDO returns 1 of diff* finds a difference
+    def __exit_success(self, operatorName):
+        if parse_version(getCdoVersion(self.CDO)) < parse_version('1.9.6'):
+            return 0
+        if 'diff' != operatorName[0:4]:
+            return 0
+        return 1
+
+    # read json formatted output of 'cdo --config all'
+    def __getConfig(self):
+      proc = subprocess.Popen([self.CDO, '--config','all'], stderr=subprocess.PIPE, stdout=subprocess.PIPE)
       ret  = proc.communicate()
-      l    = ret[1].decode("utf-8").find("Operators:")
-      ops  = ret[1].decode("utf-8")[l:-1].split(os.linesep)[1:-1]
-      endI = ops.index('')
-      s    = ' '.join(ops[:endI]).strip()
-      s    = re.sub("\s+", " ", s)
-
-      for op in list(set(s.split(" "))):
-        operators[op] = 1
-        if op in self.NoOutputOperators:
-          operators[op] = 0
-        if op in self.TwoOutputOperators:
-          operators[op] = 2
-        if op in self.MoreOutputOperators:
-          operators[op] = -1
-
-    elif (version < parse_version('1.8.0') or parse_version('1.9.0') == version):
-      proc = subprocess.Popen([self.CDO, '--operators'], stderr=subprocess.PIPE, stdout=subprocess.PIPE)
-      ret = proc.communicate()
-      ops = list(map(lambda x: x.split(' ')[0], ret[0].decode("utf-8")[0:-1].split(os.linesep)))
-
-      for op in ops:
-        operators[op] = 1
-        if op in self.NoOutputOperators:
-          operators[op] = 0
-        if op in self.TwoOutputOperators:
-          operators[op] = 2
-        if op in self.MoreOutputOperators:
-          operators[op] = -1
-
-    elif (version < parse_version('1.9.3')):
-      proc = subprocess.Popen([self.CDO, '--operators'], stderr=subprocess.PIPE, stdout=subprocess.PIPE)
-      ret = proc.communicate()
-      ops = list(map(lambda x: x.split(' ')[0], ret[0].decode("utf-8")[0:-1].split(os.linesep)))
-
-      proc = subprocess.Popen([self.CDO, '--operators_no_output'], stderr=subprocess.PIPE, stdout=subprocess.PIPE)
-      ret = proc.communicate()
-      opsNoOutput = list(map(lambda x: x.split(' ')[0], ret[0].decode("utf-8")[0:-1].split(os.linesep)))
-
-      for op in ops:
-        operators[op] = 1
-        if op in opsNoOutput:
-          operators[op] = 0
-        if op in self.TwoOutputOperators:
-          operators[op] = 2
-        if op in self.MoreOutputOperators:
-          operators[op] = -1
-
-    else:
-      proc = subprocess.Popen([self.CDO, '--operators'], stderr=subprocess.PIPE, stdout=subprocess.PIPE)
-      ret = proc.communicate()
-      ops = list(map(lambda x: x.split(' ')[0], ret[0].decode("utf-8")[0:-1].split(os.linesep)))
-      ios = list(map(lambda x: x.split(' ')[-1], ret[0].decode("utf-8")[0:-1].split(os.linesep)))
-
-      for i, op in enumerate(ops):
-        operators[op] = int(ios[i][1:len(ios[i]) - 1].split('|')[1])
-
-    return operators  # }}}
-
-  # execute a single CDO command line {{{
-  def __call(self, cmd, envOfCall={}):
-    if self.logging and '-h' != cmd[1]:
-      self.logger.info(u' '.join(cmd))
-
-    env = dict(self.env)
-    env.update(envOfCall)
-
-    proc = subprocess.Popen(' '.join(cmd),
-                            shell=True,
-                            stderr=subprocess.PIPE,
-                            stdout=subprocess.PIPE,
-                            env=env)
-
-    retvals = proc.communicate()
-    stdout = retvals[0].decode("utf-8")
-    stderr = retvals[1].decode("utf-8")
-
-    if self.debug:  # debug printing {{{
-      print('# DEBUG - start =============================================================')
-#     if {} != env:
-#       for k,v in list(env.items()):
-#         print("ENV: " + k + " = " + v)
-      print('CALL  :' + ' '.join(cmd))
-      print('STDOUT:')
-      if (0 != len(stdout.strip())):
-        print(stdout)
-      print('STDERR:')
-      if (0 != len(stderr.strip())):
-        print(stderr)
-      print('# DEBUG - end ===============================================================')  # }}}
-
-    return {"stdout": stdout, "stderr": stderr, "returncode": proc.returncode}  # }}}
-
-  # error handling for CDO calls
-  def __hasError(self, method_name, cmd, retvals):  # {{{
-    if (self.debug):
-      print("RETURNCODE:" + retvals["returncode"].__str__())
-    if ( self.__exit_success(method_name) < retvals["returncode"] ):
-      print("Error in calling operator " + method_name + " with:")
-      print(">>> " + ' '.join(cmd) + "<<<")
-      print('STDOUT:' + retvals["stdout"])
-      print('STDERR:' + retvals["stderr"])
-
-      if self.logging:
-          self.logger.error(cmd + " with:" + retvals["stderr"])
-      return True
-    else:
-      return False  # }}}
+      try:
+        return json.loads(ret[0].decode('utf-8'))
+      except:
+        return {}
+
+    # retrieve the list of operators from the CDO binary plus info out number of
+    # output streams
+    def __getOperators(self):  # {{{
+        operators = {}
+
+        version = parse_version(getCdoVersion(self.CDO))
+        if version < parse_version('1.7.2'):
+            proc = subprocess.Popen(
+                [self.CDO, '-h'], stderr=subprocess.PIPE, stdout=subprocess.PIPE)
+            ret = proc.communicate()
+            l = ret[1].decode("utf-8").find("Operators:")
+            ops = ret[1].decode("utf-8")[l:-1].split(os.linesep)[1:-1]
+            endI = ops.index('')
+            s = ' '.join(ops[:endI]).strip()
+            s = re.sub(r"\s+", " ", s)
+
+            for op in list(set(s.split(" "))):
+                operators[op] = 1
+                if op in self.NoOutputOperators:
+                    operators[op] = 0
+                if op in self.TwoOutputOperators:
+                    operators[op] = 2
+                if op in self.MoreOutputOperators:
+                    operators[op] = -1
+
+        elif version < parse_version('1.8.0') or parse_version('1.9.0') == version:
+            proc = subprocess.Popen([self.CDO, '--operators'],
+                                    stderr=subprocess.PIPE, stdout=subprocess.PIPE)
+            ret = proc.communicate()
+            ops = list(map(lambda x: x.split(' ')[0], ret[0].decode(
+                "utf-8")[0:-1].split(os.linesep)))
+
+            for op in ops:
+                operators[op] = 1
+                if op in self.NoOutputOperators:
+                    operators[op] = 0
+                if op in self.TwoOutputOperators:
+                    operators[op] = 2
+                if op in self.MoreOutputOperators:
+                    operators[op] = -1
+
+        elif version < parse_version('1.9.3'):
+            proc = subprocess.Popen([self.CDO, '--operators'],
+                                    stderr=subprocess.PIPE, stdout=subprocess.PIPE)
+            ret = proc.communicate()
+            ops = list(map(lambda x: x.split(' ')[0], ret[0].decode(
+                "utf-8")[0:-1].split(os.linesep)))
+
+            proc = subprocess.Popen(
+                [self.CDO, '--operators_no_output'],
+                stderr=subprocess.PIPE,
+                stdout=subprocess.PIPE)
+            ret = proc.communicate()
+            opsNoOutput = list(map(lambda x: x.split(
+                ' ')[0], ret[0].decode("utf-8")[0:-1].split(os.linesep)))
+
+            for op in ops:
+                operators[op] = 1
+                if op in opsNoOutput:
+                    operators[op] = 0
+                if op in self.TwoOutputOperators:
+                    operators[op] = 2
+                if op in self.MoreOutputOperators:
+                    operators[op] = -1
 
-  # {{{ attempt to load optional libraries: netcdf-IO + XArray
-  # numpy is a dependency of both, so no need to check that
-  def __loadOptionalLibs(self):
-    try:
-      import xarray
-      self.hasXarray = True
-      self.xa_open = xarray.open_dataset
-    except:
-      print("-->> Could not load xarray!! <<--")
-
-    try:
-      from netCDF4 import Dataset as cdf
-      self.cdf       = cdf
-      self.hasNetcdf = True
-      import numpy as np
-      self.np        = np
-    except:
-      print("-->> Could not load netCDF4! <<--") #}}}
-
-  def infile(self, *infiles):
-    for infile in infiles:
-      if isinstance(infile, six.string_types):
-        self._cmd.append(infile)
-      elif self.hasXarray:
-        import xarray #<<-- python2 workaround
-        if (type(infile) == xarray.core.dataset.Dataset):
-          # create a temp nc file from input data
-          tmpfile = self.tempStore.newFile()
-          infile.to_netcdf(tmpfile)
-          self._cmd.append(tmpfile)
-    return self
-
-  def add_option(self, *options):
-    self._options = self._options + list(options)
-    return self
-
-  def __call__(self, *args, **kwargs):
-    user_kwargs = kwargs.copy()
-    try:
-      method_name = self._cmd[0][1:].split(',')[0]
-    except IndexError:
-      method_name = ''
-    operatorPrintsOut = method_name in self.noOutputOperators
-
-    self.envByCall = {}
-
-    # Build the cdo command
-    # 0. the cdo command itself
-    cmd = [self.CDO]
-
-    # 1. OVERWRITE EXISTING FILES
-    cmd.append('-O')
-
-    # 2. set the options
-    # show full output in case of diff-like operators
-    # or user requested the non-silent mode directly
-    if (not method_name in self.DiffOperators) and self.silent:
-      cmd.append('-s')
-    cmd.extend(self._options)
-    # switch to netcdf output in case of numpy/xarray usage
-    if (   None != kwargs.get('returnArray')
-        or None != kwargs.get('returnMaArray')
-        or None != kwargs.get('returnXArray')
-        or None != kwargs.get('returnXDataset')
-        or None != kwargs.get('returnCdf')):
-      cmd.append('-f nc')
-    if 'options' in kwargs:
-      cmd += kwargs['options'].split()
-
-
-    # 3. add operators
-    #   collect operator parameters and pad them to the operator name
-    if len(args) != 0:
-      self._cmd[-1] += ',' + ','.join(map(str, args))
-    if self._cmd:
-      cmd.extend(self._cmd)
-
-    # 4. input files or other operators
-    if 'input' in kwargs:
-      if isinstance(kwargs["input"], six.string_types):
-        cmd.append(kwargs["input"])
-      elif type(kwargs["input"]) == list:
-        cmd.append(' '.join(kwargs["input"]))
-      elif self.hasXarray:
-        import xarray #<<-- python2 workaround
-        if (type(kwargs["input"]) == xarray.core.dataset.Dataset):
-          # create a temp nc file from input data
-          tmpfile = self.tempStore.newFile()
-          kwargs["input"].to_netcdf(tmpfile)
-          kwargs["input"] = tmpfile
-
-          cmd.append(kwargs["input"])
-      else:
-        # we assume it's either a list, a tuple or any iterable.
-        cmd.append(kwargs["input"])
-
-    # 5. handle rewrite of existing output files
-    if not kwargs.__contains__("force"):
-      kwargs["force"] = self.forceOutput
-
-    # 6. handle environment setup per call
-    envOfCall = {}
-    if kwargs.__contains__("env"):
-      for k, v in kwargs["env"].items():
-        envOfCall[k] = v
-
-    # 7. output handling: use given outputs or create temporary files
-    outputs = []
-
-    # collect the given output
-    if None != kwargs.get("output"):
-      outputs.append(kwargs["output"])
-
-    if not user_kwargs or not kwargs.get('compute', True):
-      return self
-    elif not kwargs.get('keep', True):
-      self._cmd.clear()
-
-    if operatorPrintsOut:
-      retvals = self.__call(cmd, envOfCall)
-      if (not self.__hasError(method_name, cmd, retvals)):
-        r = list(map(strip, retvals["stdout"].split(os.linesep)))
-        # skip the last newline
-        r = r[:len(r) - 1]
-        # join the list into a single one in case we deal with time
-        # axis-related output. This output must me on a single line since CDO
-        # can handle only one time axis. cdo-2.0.0 introduced newlines for
-        # readability
-        if method_name in self.ShowTimeOperators:
-          r = ['  '.join(r)]
-        # starting with cdo-2.0.0 diff* operators print more warnings. those
-        # lines start with 'cdo' and must be removed
-        if method_name in self.DiffOperators:
-          r = [item for item in r if 'cdo' != item[0:3]]
-
-        if "autoSplit" in kwargs:
-          splitString = kwargs["autoSplit"]
-          _output = [x.split(splitString) for x in r]
-          if (1 == len(_output)):
-              return _output[0]
-          else:
-              return _output
-        else:
-         return r
-      else:
-        if self.returnNoneOnError:
-          return None
         else:
-          raise CDOException(**retvals)
-    else:
-      if kwargs["force"] or \
-         (kwargs.__contains__("output") and not os.path.isfile(kwargs["output"])):
-        if not kwargs.__contains__("output") or None == kwargs["output"]:
-          for i in range(0, self.operators[method_name]):
-            outputs.append(self.tempStore.newFile())
-
-        cmd.append(' '.join(outputs))
-
-        retvals = self.__call(cmd, envOfCall)
-        if self.__hasError(method_name, cmd, retvals):
-          if self.returnNoneOnError:
-            return None
-          else:
-            raise CDOException(**retvals)
-      else:
-        if self.debug:
-          print(("Use existing file'" + kwargs["output"] + "'"))
+            proc = subprocess.Popen([self.CDO, '--operators'],
+                                    stderr=subprocess.PIPE, stdout=subprocess.PIPE)
+            ret = proc.communicate()
+            ops = list(map(lambda x: x.split(' ')[0], ret[0].decode(
+                "utf-8")[0:-1].split(os.linesep)))
+            ios = list(map(lambda x: x.split(' ')[-1], ret[0].decode(
+                "utf-8")[0:-1].split(os.linesep)))
+
+            for i, op in enumerate(ops):
+                operators[op] = int(ios[i][1:len(ios[i]) - 1].split('|')[1])
+
+        return operators  # }}}
+
+    # execute a single CDO command line {{{
+    def __call(self, cmd, envOfCall={}):
+        if self.logging and '-h' != cmd[1]:
+            self.logger.info(u' '.join(cmd))
+
+        env = dict(self.env)
+        env.update(envOfCall)
+
+        proc = subprocess.Popen(' '.join(cmd),
+                                shell=True,
+                                stderr=subprocess.PIPE,
+                                stdout=subprocess.PIPE,
+                                env=env)
+
+        retvals = proc.communicate()
+        stdout = retvals[0].decode("utf-8")
+        stderr = retvals[1].decode("utf-8")
+
+        if self.debug:  # debug printing {{{
+            print('# DEBUG - start =============================================================')
+            # if {} != env:
+            #     for k,v in list(env.items()):
+            #         print("ENV: " + k + " = " + v)
+            print('CALL  :' + ' '.join(cmd))
+            print('STDOUT:')
+            if 0 != len(stdout.strip()):
+                print(stdout)
+            print('STDERR:')
+            if 0 != len(stderr.strip()):
+                print(stderr)
+            # }}}
+            print('# DEBUG - end ===============================================================')
 
-    # defaults for file handles as return values
-    if not kwargs.__contains__("returnCdf"):
-      kwargs["returnCdf"] = False
-    if not kwargs.__contains__("returnXDataset"):
-      kwargs["returnXDataset"] = False
-
-    # return data arrays
-    if None != kwargs.get("returnArray"):
-      return self.readArray(outputs[0], kwargs["returnArray"])
-    elif None != kwargs.get("returnMaArray"):
-      return self.readMaArray(outputs[0], kwargs["returnMaArray"])
-    elif None != kwargs.get("returnXArray"):
-      return self.readXArray(outputs[0], kwargs.get("returnXArray"))
-
-    # return files handles (or lists of them)
-    elif kwargs["returnCdf"]:
-      if 1 == len(outputs):
-        return self.readCdf(outputs[0])
-      else:
-        return [self.readCdf(file) for file in outputs]
-    elif kwargs["returnXDataset"]:
-      if 1 == len(outputs):
-        return self.readXDataset(outputs[0])
-      else:
-        return [self.readXDataset(file) for file in outputs]
-
-    # handle split-operator outputs
-    elif ('split' == method_name[0:5]):
-      return glob.glob(kwargs["output"] + '*')
-
-    # default: return filename (given or tempfile)
-    else:
-      if (1 == len(outputs)):
-        return outputs[0]
-      else:
-        return outputs
+        return {"stdout": stdout, "stderr": stderr, "returncode": proc.returncode}  # }}}
 
-  def __getattr__(self, method_name):  # main method-call handling for Cdo-objects {{{
-
-    if ((method_name in self.__dict__) or (method_name in list(self.operators.keys()))
-        or (method_name in self.AliasOperators)):
-      if self.debug:
-        print(("Found method:" + method_name))
+    # error handling for CDO calls
+    def __hasError(self, method_name, cmd, retvals):  # {{{
+        if self.debug:
+            print("RETURNCODE:" + retvals["returncode"].__str__())
+        if self.__exit_success(method_name) < retvals["returncode"]:
+            print("Error in calling operator " + method_name + " with:")
+            print(">>> " + ' '.join(cmd) + "<<<")
+            print('STDOUT:' + retvals["stdout"])
+            print('STDERR:' + retvals["stderr"])
+
+            if self.logging:
+                self.logger.error(cmd + " with:" + retvals["stderr"])
+            return True
+        else:
+            return False  # }}}
 
-      # cache the method for later
-      class Operator(self.__class__):
+    # {{{ attempt to load optional libraries: netcdf-IO + XArray
+    # numpy is a dependency of both, so no need to check that
+    def __loadOptionalLibs(self):
+        try:
+            import xarray
+            self.hasXarray = True
+            self.xa_open = xarray.open_dataset
+        except Exception:
+            print("-->> Could not load xarray!! <<--")
+
+        try:
+            from netCDF4 import Dataset as cdf
+            import numpy as np
+            self.hasNetcdf = True
+            self.cdf = cdf
+            self.np = np
+        except Exception:
+            print("-->> Could not load netCDF4! <<--")  # }}}
+
+    def infile(self, *infiles):
+        for infile in infiles:
+            if isinstance(infile, six.string_types):
+                self._cmd.append(infile)
+            elif self.hasXarray:
+                import xarray  # <<-- python2 workaround
+                if type(infile) == xarray.core.dataset.Dataset:
+                    # create a temp nc file from input data
+                    tmpfile = self.tempStore.newFile()
+                    infile.to_netcdf(tmpfile)
+                    self._cmd.append(tmpfile)
+        return self
+
+    def add_option(self, *options):
+        self._options = self._options + list(options)
+        return self
+
+    def __call__(self, *args, **kwargs):
+        user_kwargs = kwargs.copy()
+        try:
+            method_name = self._cmd[0][1:].split(',')[0]
+        except IndexError:
+            method_name = ''
+        operatorPrintsOut = method_name in self.noOutputOperators
+
+        self.envByCall = {}
+
+        # Build the cdo command
+        # 0. the cdo command itself
+        cmd = [self.CDO]
+
+        # 1. OVERWRITE EXISTING FILES
+        cmd.append('-O')
+
+        # 2. set the options
+        # show full output in case of diff-like operators
+        # or user requested the non-silent mode directly
+        if (not method_name in self.DiffOperators) and self.silent:
+            cmd.append('-s')
+        cmd.extend(self._options)
+        # switch to netcdf output in case of numpy/xarray usage
+        if kwargs.get('returnArray') is not None \
+           or kwargs.get('returnMaArray') is not None \
+           or kwargs.get('returnXArray') is not None \
+           or kwargs.get('returnXDataset') is not None \
+           or kwargs.get('returnCdf') is not None:
+            cmd.append('-f nc')
+        if 'options' in kwargs:
+            cmd += kwargs['options'].split()
+
+        # 3. add operators
+        # collect operator parameters and pad them to the operator name
+        if len(args) != 0:
+            self._cmd[-1] += ',' + ','.join(map(str, args))
+        if self._cmd:
+            cmd.extend(self._cmd)
+
+        # 4. input files or other operators
+        if 'input' in kwargs:
+            if isinstance(kwargs["input"], six.string_types):
+                cmd.append(kwargs["input"])
+            elif type(kwargs["input"]) == list:
+                cmd.append(' '.join(kwargs["input"]))
+            elif self.hasXarray:
+                import xarray  # <<-- python2 workaround
+                if type(kwargs["input"]) in [xarray.core.dataset.Dataset,xarray.core.dataarray.DataArray]:
+                    # create a temp nc file from input data
+                    tmpfile = self.tempStore.newFile()
+                    kwargs["input"].to_netcdf(tmpfile)
+                    kwargs["input"] = tmpfile
+
+                    cmd.append(kwargs["input"])
+            else:
+                # we assume it's either a list, a tuple or any iterable.
+                cmd.append(kwargs["input"])
+
+        # 5. handle rewrite of existing output files
+        if not kwargs.__contains__("force"):
+            kwargs["force"] = self.forceOutput
+
+        # 6. handle environment setup per call
+        envOfCall = {}
+        if kwargs.__contains__("env"):
+            for k, v in kwargs["env"].items():
+                envOfCall[k] = v
+
+        # 7. output handling: use given outputs or create temporary files
+        outputs = []
+
+        # collect the given output
+        if kwargs.get("output") is not None:
+            outputs.append(kwargs["output"])
+
+        if not user_kwargs or not kwargs.get('compute', True):
+            return self
+        elif not kwargs.get('keep', True):
+            self._cmd.clear()
+
+        if operatorPrintsOut:
+            retvals = self.__call(cmd, envOfCall)
+            if not self.__hasError(method_name, cmd, retvals):
+                r = list(map(strip, retvals["stdout"].split(os.linesep)))
+                if "autoSplit" in kwargs:
+                    splitString = kwargs["autoSplit"]
+                    _output = [x.split(splitString) for x in r[:len(r) - 1]]
+                    if 1 == len(_output):
+                        return _output[0]
+                    else:
+                        return _output
+                else:
+                    return r[:len(r) - 1]
+            else:
+                if self.returnNoneOnError:
+                    return None
+                else:
+                    raise CDOException(**retvals)
+        else:
+            if kwargs["force"] or \
+               (kwargs.__contains__("output") and not os.path.isfile(kwargs["output"])):
+                if not kwargs.__contains__("output") or kwargs["output"] is None:
+                    for i in range(0, self.operators[method_name]):
+                        outputs.append(self.tempStore.newFile())
+
+                cmd.append(' '.join(outputs))
+
+                retvals = self.__call(cmd, envOfCall)
+                if self.__hasError(method_name, cmd, retvals):
+                    if self.returnNoneOnError:
+                        return None
+                    else:
+                        raise CDOException(**retvals)
+            else:
+                if self.debug:
+                    print(("Use existing file'" + kwargs["output"] + "'"))
+
+        # defaults for file handles as return values
+        if not kwargs.__contains__("returnCdf"):
+            kwargs["returnCdf"] = False
+        if not kwargs.__contains__("returnXDataset"):
+            kwargs["returnXDataset"] = False
+
+        # return data arrays
+        if kwargs.get("returnArray") is not None:
+            return self.readArray(outputs[0], kwargs["returnArray"])
+        elif kwargs.get("returnMaArray") is not None:
+            return self.readMaArray(outputs[0], kwargs["returnMaArray"])
+        elif kwargs.get("returnXArray") is not None:
+            return self.readXArray(outputs[0], kwargs.get("returnXArray"))
+
+        # return files handles (or lists of them)
+        elif kwargs["returnCdf"]:
+            if 1 == len(outputs):
+                return self.readCdf(outputs[0])
+            else:
+                return [self.readCdf(file) for file in outputs]
+        elif kwargs["returnXDataset"]:
+            if 1 == len(outputs):
+                return self.readXDataset(outputs[0])
+            else:
+                return [self.readXDataset(file) for file in outputs]
+
+        # handle split-operator outputs
+        elif 'split' == method_name[0:5]:
+            return glob.glob(kwargs["output"] + '*')
 
-        __doc__ = operator_doc(method_name, self.CDO)
+        # default: return filename (given or tempfile)
+        else:
+            if 1 == len(outputs):
+                return outputs[0]
+            else:
+                return outputs
+
+    def __getattr__(self, method_name):  # main method-call handling for Cdo-objects {{{
+        if any(method_name in opts for opts in (
+               self.__dict__, self.operators, self.AliasOperators)):
+            if self.debug:
+                print(("Found operator:" + method_name))
+
+            # cache the method for later
+            class Operator(self.__class__):
+                name = method_name
+                __name__ = method_name
+                __qualname__ = getattr(  # __qualname__ is available in python 3.3+
+                    self.__class__, '__qualname__', self.__class__.__name__
+                ) + '.' + method_name
+
+                def __init__(self, *args, **kwargs):
+                    super().__init__(*args, **kwargs)
+                    self.__doc__ = operator_doc(method_name, self.CDO)
 
-        name = method_name
+            setattr(self.__class__, method_name, Operator())
+            return getattr(self, method_name)
+        else:
+            # given method might match part of know operators: autocompletion
+            func = lambda x: re.search(method_name, x)
+            options = list(filter(func, self.operators))
+            message = "Unknown operator '" + method_name + "'!"
+            if 0 != len(options):
+                message += " Did you mean: " + ", ".join(options) + "?"
+            raise AttributeError(message)
+    # }}}
+
+    def getSupportedLibs(self):
+        proc = subprocess.Popen(self.CDO + ' -V',
+                                shell=True,
+                                stdout=subprocess.PIPE,
+                                stderr=subprocess.STDOUT)
+        retvals = proc.communicate()
+        withs = list(re.findall('(with|Features): (.*)',
+                                retvals[0].decode("utf-8"))[0])[1].split(' ')
+
+        # do an additional split if the entry has a /
+        # and collect everything into a flatt list
+        withs = list(map(lambda x: x.split('/') if re.search(r'\/', x) else x, withs))
+        allWiths = []
+        for _withs in withs:
+            if isinstance(_withs, list):
+                for __withs in _withs:
+                    allWiths.append(__withs)
+            else:
+                allWiths.append(_withs)
+        withs = allWiths
+
+        libs = re.findall(r'(\w+) library version : (\d+\.\S+) ',
+                          retvals[0].decode("utf-8"))
+        libraries = dict({})
+        for w in withs:
+            libraries[w.lower()] = True
+
+        for lib in libs:
+            l, v = lib
+            libraries[l.lower()] = v
+
+        return libraries
+
+    def collectLogs(self):
+        if isinstance(self.logFile, six.string_types):
+            content = []
+            with open(self.logFile, 'r') as f:
+                content.append(f.read())
+            return ''.join(content)
+        else:
+            self.logFile.flush()
+            return self.logFile.getvalue()
 
-      setattr(self.__class__, method_name, Operator())
-      return getattr(self, method_name)
-    else:
-      # given method might match part of know operators: autocompletion
-      if (len(list(filter(lambda x: re.search(method_name, x), list(self.operators.keys())))) == 0):
-        # If the method isn't in our dictionary, act normal.
-        raise AttributeError("Unknown method '" + method_name + "'!")
-  # }}}
-
-  def collectLogs(self):
-    if isinstance(self.logFile, six.string_types):
-      content = []
-      with open(self.logFile, 'r') as f:
-        content.append(f.read())
-      return ''.join(content)
-    else:
-      self.logFile.flush()
-      return self.logFile.getvalue()
+    def showLog(self):
+        print(self.collectLogs())
 
-  def showLog(self):
-    print(self.collectLogs())
+    # check if the current (or given) CDO binary works
+    def hasCdo(self, path=None):
+        if path is None:
+            path = self.CDO
+        cmd = [path, ' -V', '>/dev/null 2>&1']
+        executable = (0 == self.__call(cmd)["returncode"])
+        fullpath = (os.path.isfile(path) and os.access(path, os.X_OK))
+        return (executable or fullpath)
+
+    # selfcheck for the current CDO binary
+    def check(self):
+        if not self.hasCdo():
+            return False
+        if self.debug:
+            print(self.__call([self.CDO, ' -V']))
+        return True
 
-  # check if the current (or given) CDO binary works
-  def hasCdo(self, path=None):
-    if path is None:
-      path = self.CDO
-
-    cmd = [path, " -V", '>/dev/null 2>&1']
-
-    executable = (0 == self.__call(cmd)["returncode"])
-    fullpath = (os.path.isfile(path) and os.access(path, os.X_OK))
-
-    return (executable or fullpath)
-
-  # selfcheck for the current CDO binary
-  def check(self):
-    if not self.hasCdo():
-      return False
-    if self.debug:
-      print(self.__call([self.CDO, ' -V']))
-    return True
-
-  # change the CDO binary for the current object
-  def setCdo(self, value):
-    self.CDO = value
-    self.operators = self.__getOperators()
-
-  # return the path to the CDO binary currently used
-  def getCdo(self):
-    return self.CDO
-
-  def cleanTempDir(self):
-    self.tempStore.cleanTempDir()
-
-  # if a termination signal could be caught, remove tempfile
-  def __catch__(self, signum, frame):
-    self.tempStore.__del__()
-    print("caught signal", self, signum, frame)
-
-  # make use of internal documentation structure of python
-  def __dir__(self):
-    res = dir(type(self)) + list(self.__dict__.keys())
-    res.extend(list(self.operators.keys()))
-    return res
-  # ==================================================================
-  # Addional operators:
-  # ------------------------------------------------------------------
-
-  def version(self, verbose=False):
-    # return CDO's version
-    return getCdoVersion(self.CDO, verbose)
-
-  def boundaryLevels(self, **kwargs):
-    ilevels = list(map(float, self.showlevel(input=kwargs['input'])[0].split()))
-    bound_levels = []
-    bound_levels.insert(0, 0)
-    for i in range(1, len(ilevels) + 1):
-      bound_levels.insert(i, bound_levels[i - 1] + 2 * (ilevels[i - 1] - bound_levels[i - 1]))
-
-    return bound_levels
-
-  def thicknessOfLevels(self, **kwargs):
-    bound_levels = self.boundaryLevels(**kwargs)
-    delta_levels = []
-    for i in range(0, len(bound_levels)):
-      v = bound_levels[i]
-      if 0 == i:
-        continue
-
-      delta_levels.append(v - bound_levels[i - 1])
-
-    return delta_levels
-
-  def run(self, output=None):
-    if output:
-      return self(output=output, compute=True)
-    else:
-      return self(compute=True)
+    # change the CDO binary for the current object
+    def setCdo(self, value):
+        self.CDO = value
+        self.operators = self.__getOperators()
+
+    # return the path to the CDO binary currently used
+    def getCdo(self):
+        return self.CDO
+
+    def hasLib(self, lib):
+        return lib in self.libs
+
+    def libsVersion(self, lib):
+        if not self.hasLib(lib):
+            raise AttributeError("Cdo does NOT have support for '#{lib}'")
+        else:
+            if self.libs[lib] is not True:
+                return self.libs[lib]
+            else:
+                print("No version information available about '" + lib + "'")
+                return False
+
+    def cleanTempDir(self):
+        self.tempStore.cleanTempDir()
+
+    # make use of internal documentation structure of python
+    def __dir__(self):
+        res = dir(type(self)) + list(self.__dict__)
+        res.extend(list(self.operators))
+        return res
+
+    # ==================================================================
+    # Addional operators:
+    # ------------------------------------------------------------------
+
+    def version(self, verbose=False):
+        # return CDO's version
+        return getCdoVersion(self.CDO, verbose)
+
+    def boundaryLevels(self, **kwargs):
+        ilevels = list(map(float, self.showlevel(input=kwargs['input'])[0].split()))
+        bound_levels = []
+        bound_levels.insert(0, 0)
+        for i in range(1, len(ilevels) + 1):
+            bound_levels.insert(
+                i, bound_levels[i - 1] + 2 * (ilevels[i - 1] - bound_levels[i - 1]))
+
+        return bound_levels
+
+    def thicknessOfLevels(self, **kwargs):
+        bound_levels = self.boundaryLevels(**kwargs)
+        delta_levels = []
+        for i in range(0, len(bound_levels)):
+            v = bound_levels[i]
+            if 0 == i:
+                continue
+
+            delta_levels.append(v - bound_levels[i - 1])
+
+        return delta_levels
+
+    def run(self, output=None):
+        if output:
+            return self(output=output, compute=True)
+        else:
+            return self(compute=True)
 
-  def readCdf(self, iFile=None):
-    """Return a cdf handle created by the available cdf library"""
-    if iFile is None:
-      iFile = self.run()
-    if self.hasNetcdf:
-      fileObj = self.cdf(iFile, mode='r')
-      return fileObj
-    else:
-      print("Could not import data from file '%s' (python-netCDF4)" % iFile)
-      six.raise_from(ImportError,None)
+    def readCdf(self, iFile=None):
+        """Return a cdf handle created by the available cdf library"""
+        if iFile is None:
+            iFile = self.run()
+        if self.hasNetcdf:
+            fileObj = self.cdf(iFile, mode='r')
+            return fileObj
+        else:
+            print("Could not import data from file '%s' (python-netCDF4)" % iFile)
+            six.raise_from(ImportError, None)
 
-  def readArray(self, iFile=None, varname=None):
-    """Direcly return a numpy array for a given variable name"""
-    if iFile is None:
-      iFile = self.run()
-    if varname is None:
-      raise ValueError("A varname needs to be specified!")
-    filehandle = self.readCdf(iFile)
-    try:
-      # return the data array for given variable name
-      return filehandle.variables[varname][:].copy()
-    except:
-      print("Cannot find variable '%s'" % varname)
-      six.raise_from(LookupError,None)
-
-
-  def readMaArray(self, iFile=None, varname=None):# {{{
-    """Create a masked array based on cdf's FillValue"""
-    if iFile is None:
-      iFile = self.run()
-    if varname is None:
-      raise ValueError("A varname needs to be specified!")
-    fileObj = self.readCdf(iFile)
-
-    if not varname in fileObj.variables:
-      print("Cannot find variables '%s'" % varname)
-      six.raise_from(LookupError,None)
-    else:
-      data = fileObj.variables[varname][:].copy()
+    def readArray(self, iFile=None, varname=None):
+        """Direcly return a numpy array for a given variable name"""
+        if iFile is None:
+            iFile = self.run()
+        if varname is None:
+            raise ValueError("A varname needs to be specified!")
+        filehandle = self.readCdf(iFile)
+        try:
+            # return the data array for given variable name
+            return filehandle.variables[varname][:].copy()
+        except Exception:
+            print("Cannot find variable '%s'" % varname)
+            six.raise_from(LookupError, None)
+
+    def readMaArray(self, iFile=None, varname=None):  # {{{
+        """Create a masked array based on cdf's FillValue"""
+        if iFile is None:
+            iFile = self.run()
+        if varname is None:
+            raise ValueError("A varname needs to be specified!")
+        fileObj = self.readCdf(iFile)
+
+        if varname not in fileObj.variables:
+            print("Cannot find variables '%s'" % varname)
+            six.raise_from(LookupError, None)
+        else:
+            data = fileObj.variables[varname][:].copy()
 
-    if hasattr(fileObj.variables[varname], '_FillValue'):
-      # return masked array
-      retval = self.np.ma.array(data, mask=data == fileObj.variables[varname]._FillValue)
-    else:
-      # generate dummy mask which is always valid
-      retval = self.np.ma.array(data, mask=data != data)
+        if hasattr(fileObj.variables[varname], '_FillValue'):
+            # return masked array
+            retval = self.np.ma.array(
+                data, mask=data == fileObj.variables[varname]._FillValue)
+        else:
+            # generate dummy mask which is always valid
+            retval = self.np.ma.array(data, mask=data != data)
 
-    return retval# }}}
+        return retval  # }}}
 
-  def readXArray(self, ifile=None, varname=None):
-    if ifile is None:
-      ifile = self.run()
-    if varname is None:
-      raise ValueError("A varname needs to be specified!")
-    if not self.hasXarray:
-      print("Could not load XArray")
-      six.raise_from(ImportError,None)
-
-    dataSet = self.xa_open(ifile)
-    try:
-      return dataSet[varname]
-    except:
-      print("Cannot find variable '%s'" % varname)
-      six.raise_from(LookupError,None)
-
-  def readXDataset(self, ifile=None):
-    if ifile is None:
-      ifile = self.run()
-    if not self.hasXarray:
-      print("Could not load XArray")
-      six.raise_from(ImportError,None)
-
-    return self.xa_open(ifile)
-
-  # internal helper methods:
-  # return internal cdo.py version
-  def __version__(self):
-    return CDO_PY_VERSION
-
-  def __print__(self, context=''):
-    if '' != context:
-      print('CDO:CONTEXT ' + context)
-    print("CDO:ID  = " + str(id(self)))
-    print("CDO:ENV = " + str(self.env))
+    def readXArray(self, ifile=None, varname=None):
+        if ifile is None:
+            ifile = self.run()
+        if varname is None:
+            raise ValueError("A varname needs to be specified!")
+        if not self.hasXarray:
+            print("Could not load XArray")
+            six.raise_from(ImportError, None)
+
+        dataSet = self.xa_open(ifile)
+        try:
+            return dataSet[varname]
+        except Exception:
+            print("Cannot find variable '%s'" % varname)
+            six.raise_from(LookupError, None)
+
+    def readXDataset(self, ifile=None):
+        if ifile is None:
+            ifile = self.run()
+        if not self.hasXarray:
+            print("Could not load XArray")
+            six.raise_from(ImportError, None)
+
+        return self.xa_open(ifile)
+
+    def __print__(self, context=''):
+        if '' != context:
+            print('CDO:CONTEXT ' + context)
+        print("CDO:ID  = " + str(id(self)))
+        print("CDO:ENV = " + str(self.env))
 # }}}
 
 # Helper module for easy temp file handling {{{
+
 class CdoTempfileStore(object):
 
-  __tempfiles = []
+    __tempfiles = []
 
-  __tempdirs = []
+    def __init__(self, dir):
+        self.persistent_tempfile = False
+        self.fileTag = 'cdoPy'
+        self.dir = dir
+        if not os.path.isdir(dir):
+            os.makedirs(dir)
+        # handling different exits from interactive sessions
+        # python3 has threading.main_thread(), but python2 doesn't
+        if sys.version_info[0] == 2 \
+                or threading.current_thread() is threading.main_thread():
+            for sig in (signal.SIGINT, signal.SIGTERM, signal.SIGSEGV):
+                sig_default = signal.getsignal(sig)
+                sig_wrapped = functools.partial(self.__catch__, throw=sig_default)
+                signal.signal(sig, sig_wrapped)
+                signal.siginterrupt(sig, False)
+
+    def __del__(self):
+        # remove temporary files
+        for filename in self.__class__.__tempfiles:
+            if os.path.isfile(filename):
+                os.remove(filename)
+
+    def __catch__(self, signum, frame, throw=None, **kwargs):
+        # if a termination signal could be caught, remove tempfile
+        self.__del__()
+        if callable(throw):
+            throw(signum, frame, **kwargs)
+        else:
+            print("caught signal", signum, frame)
 
-  def __init__(self, dir):
-    self.persistent_tempfile = False
-    self.fileTag = 'cdoPy'
-    self.dir = dir
-    if not os.path.isdir(dir):
-      os.makedirs(dir)
-    self.__tempdirs.append(dir)
-
-  def __del__(self):
-    # remove temporary files
-    try:
-      self.__tempdirs.remove(self.dir)
-    except ValueError:
-      pass
-    if self.dir not in self.__tempdirs:
-      for filename in self.__class__.__tempfiles:
-        if os.path.isfile(filename):
-          os.remove(filename)
-
-  def cleanTempDir(self):
-    leftOvers = [os.path.join(self.dir, f) for f in os.listdir(self.dir)]
-    # filter for cdo.py's tempfiles owned by you
-    leftOvers = [f for f in leftOvers if
-                 self.fileTag in f and
-                 os.path.isfile(f) and
-                 os.stat(f).st_uid == os.getuid()]
-    # this might lead to trouble if it is used by server side computing like
-    # jupyter notebooks, filtering by userid might no be enough
-    for f in leftOvers:
-      os.remove(f)
-
-  def setPersist(self, value):
-    self.persistent_tempfiles = value
-
-  def newFile(self):
-    if not self.persistent_tempfile:
-      t = tempfile.NamedTemporaryFile(delete=True, prefix=self.fileTag, dir=self.dir)
-      self.__class__.__tempfiles.append(t.name)
-      t.close()
+    def cleanTempDir(self):
+        leftOvers = [os.path.join(self.dir, f) for f in os.listdir(self.dir)]
+        # filter for cdo.py's tempfiles owned by you
+        leftOvers = [f for f in leftOvers if
+                     self.fileTag in f
+                     and os.path.isfile(f)
+                     and os.stat(f).st_uid == os.getuid()]
+        # this might lead to trouble if it is used by server side computing like
+        # jupyter notebooks, filtering by userid might no be enough
+        for f in leftOvers:
+            os.remove(f)
+
+    def setPersist(self, value):
+        self.persistent_tempfiles = value
+
+    def newFile(self):
+        if not self.persistent_tempfile:
+            t = tempfile.NamedTemporaryFile(
+                delete=True, prefix=self.fileTag, dir=self.dir)
+            self.__class__.__tempfiles.append(t.name)
+            t.close()
 
-      return t.name
-    else:
-      N = 10000000
-      return "_" + random.randint(0, N).__str__()
+            return t.name
+        else:
+            N = 10000000
+            return "_" + random.randint(0, N).__str__()
 # }}}
 
-# vim: tabstop=2 expandtab shiftwidth=2 softtabstop=2 fdm=marker
+# vim: expandtab tabstop=4 shiftwidth=4 softtabstop=4 fdm=marker
```

### Comparing `cdo-1.5.7/setup.py` & `cdo-1.6.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # Package meta-data.
 NAME = 'cdo'
 DESCRIPTION = 'python bindings to CDO'
 URL = 'https://code.mpimet.mpg.de/projects/cdo/wiki/Cdo%7Brbpy%7D'
 EMAIL = 'stark.dreamdetective@gmail.com'
 AUTHOR = 'Ralf Mueller'
 REQUIRES_PYTHON = '>=2.7.0'
-VERSION = '1.5.7'
+VERSION = '1.6.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'six'
 ]
 
 # What packages are optional?
@@ -102,26 +102,25 @@
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
-    py_modules  = ["cdo"],
+    packages  = ["cdo"],
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
 
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy'
     ],
     # $ setup.py publish support.
     cmdclass={
         'upload': UploadCommand,
```

### Comparing `cdo-1.5.7/test/test_cdo.py` & `cdo-1.6.0/test/test_cdo.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,16 +18,16 @@
   import unittest
   testModule=unittest
   testClass=unittest.TestCase
   testLoader=unittest.TestLoader()
 
 # add local dir to search path
 sys.path.insert(0,os.path.dirname(sys.path[0]))
-from cdo import Cdo,CDOException,CdoTempfileStore
-
+from cdo import Cdo, CDOException
+import cdo as cdoPkg
 
 if 'CDF_MOD' in os.environ:
   CDF_MOD = os.environ['CDF_MOD']
 else:
   CDF_MOD = 'netcdf4'
 
 HOSTNAME       = 'luthien'
@@ -36,14 +36,15 @@
 SHOW           = 'SHOW' in os.environ
 DEBUG          = 'DEBUG' in os.environ
 
 MAINTAINERMODE = 'MAINTAINERMODE' in os.environ
 
 if SHOW:
   from matplotlib import pylab as pl
+  from matplotlib import pyplot as plt
 
 def plot(ary,ofile=False,title=None):
   if not SHOW:
     return
 
   pl.grid(True)
 
@@ -80,17 +81,17 @@
     def test_ju(self):
         cdo = Cdo()
         cdo.debug = True
         print(cdo.version())
         print(cdo.sinfov(input='-topo'))
 
     def testCDO(self):
+        self.assertTrue(parse_version(cdoPkg.__version__) >= parse_version('1.6.0'))
         cdo = Cdo()
         print('this is CDO version %s'%(cdo.version()))
-        print('cdo-bindings version: %s'%(cdo.__version__()))
         newCDO="/home/ram/src/tools/spack/opt/spack/linux-antergos-skylake/gcc-11.1.0/cdo-1.9.9-switof25xqmlys765t7aonnc564wl3jl/bin/cdo"
         if os.path.isfile(newCDO):
             cdo.setCdo(newCDO)
             self.assertEqual(newCDO,cdo.getCdo())
             cdo.setCdo('cdo')
             self.assertEqual('cdo',cdo.getCdo())
             # now constructor option
@@ -181,16 +182,22 @@
           '2001-01-01T15:00:00',
           '2001-01-01T16:00:00',
           '2001-01-01T17:00:00',
           '2001-01-01T18:00:00',
           '2001-01-01T19:00:00',
           '2001-01-01T20:00:00',
           '2001-01-01T21:00:00']
-        self.assertEqual(timesExpected,
-                         cdo.showtimestamp(input="-settaxis,2001-01-01,12:00,1hour -for,1,10", autoSplit='  '))
+        if (parse_version(cdo.version()) == parse_version('2.0.0')):
+          # cdo-2.0.0 does not put output on a single line with '-s' like previous and later versions'
+          timesExpected = [['2001-01-01T12:00:00', '2001-01-01T13:00:00', '2001-01-01T14:00:00', '2001-01-01T15:00:00'],
+                           ['2001-01-01T16:00:00', '2001-01-01T17:00:00', '2001-01-01T18:00:00', '2001-01-01T19:00:00'],
+                           ['2001-01-01T20:00:00', '2001-01-01T21:00:00']]
+
+        actualOutput = cdo.showtimestamp(input="-settaxis,2001-01-01,12:00,1hour -for,1,10", autoSplit='  ')
+        self.assertEqual(timesExpected, actualOutput)
 
         self.assertEqual(['P T'],cdo.showname(input="-stdatm,0"))
         self.assertEqual(['P','T'],cdo.showname(input="-stdatm,0",autoSplit=' '))
 
     def test_bndLevels(self):
         cdo = Cdo()
         ofile = cdo.stdatm(25,100,250,500,875,1400,2100,3000,4000,5000,options = "-f nc")
@@ -203,37 +210,41 @@
         cdo = Cdo()
         cdo.debug = DEBUG
         names = cdo.showname(input = "-stdatm,0",options = "-f nc")
         self.assertEqual(["P T"],names)
 
     def test_chain(self):
         cdo = Cdo()
-        ofile = cdo.setname("veloc", input=" -copy -random,r1x1",options = "-f nc")
-        self.assertEqual(["veloc"],cdo.showname(input = ofile))
+        self.assertEqual(["veloc"],cdo.showname(input = cdo.setname("veloc", input=" -copy -random,r1x1",options = "-f nc")))
 
     def test_pychain(self):
         cdo = Cdo()
         ofile = cdo.setname("veloc").copy.random("r1x1").add_option("-f nc").run()
         self.assertEqual(["veloc"],cdo.showname(input = ofile))
 
     def test_pychain2(self):
         # compare the two different ways
         cdo = Cdo()
         ofile1 = cdo.setname("veloc").copy.random("r1x1").add_option("-f nc").run()
         cdo = Cdo()
         ofile2 = cdo.setname("veloc", input=" -copy -random,r1x1",options = "-f nc")
-        diff = cdo.diff(input=[ofile1, ofile2])
+        diff = cdo.diff(input=[ofile1, ofile2], options='-s')
         self.assertFalse(diff, msg=diff)
 
     def test_diff(self):
         cdo = Cdo()
         cdo.debug = DEBUG
         diffv = cdo.diffn(input = "-random,global_0.5 -random,global_0.5")
-        self.assertEqual('random', diffv[-2].split(' ')[-1],"random")
-        self.assertEqual('1 of 1 records differ',diffv[-1])
+        thisVersion = parse_version(cdo.version())
+        if (thisVersion >= parse_version('2.0.0') and thisVersion <= parse_version('2.0.5')):
+          self.assertEqual('random', diffv[-5].split(' ')[-1],"random")
+          self.assertEqual('1 of 1 records differ',diffv[-4])
+        else:
+          self.assertEqual('random', diffv[-2].split(' ')[-1],"random")
+          self.assertEqual('1 of 1 records differ',diffv[-1])
 
     def test_returnCdf(self):
         cdo = Cdo()
         ofile = tempfile.NamedTemporaryFile(delete=True,prefix='cdoPy').name
         press = cdo.stdatm("0",output=ofile,options="-f nc")
         self.assertEqual(ofile,press)
         if cdo.hasNetcdf:
@@ -445,14 +456,23 @@
       self.assertEqual(1.0,minByCdo)
 
       #do the same without explicit tempfile
       self.assertEqual(1.0,cdo.fldmin(input=dataSet,returnArray='topo').min())
 
       xarrayFile.close()
 
+    def test_xarray_input_and_output(self):
+      cdo = Cdo()
+      ifile = cdo.setcalendar('360_day', input=' -settaxis,1800-01-01,12:00:00,1months -seq,1,10000',options='-f nc -r')
+      (var,) = cdo.showname(input=ifile)
+      self.assertEqual('seq',var)
+      x = cdo.selyear('1985/2100', input=ifile, returnXArray=var)
+      y = cdo.yearsum(input=x, returnXArray=var)
+      self.assertEqual(4059768.0,float(y[:,0,0].sum()))
+
     def test_xarray_output(self):
       cdo = Cdo()
       try:
         import xarray
       except:
         print("no xarray installation available!")
         return
@@ -487,24 +507,25 @@
             self.assertTrue(e.returncode != 0)
             self.assertTrue(len(e.stderr) > 1)
             self.assertTrue(hasattr(e, 'stdout'))
 
     def test_inputArray(self):
         cdo = Cdo()
         cdo.debug = DEBUG
+        cdo.silent = True
         # check for file input
         fileA = cdo.stdatm(0,output='A_{0}'.format( random.randrange(1,100000)))
         fileB = cdo.stdatm(0,output='B_{0}'.format( random.randrange(1,100000)))
         files = [fileA,fileB]
-        self.assertEqual(cdo.diffv(input = ' '.join(files)), cdo.diffv(input = files))
-        self.assertEqual([],cdo.diffv(input = files))
+        self.assertEqual(cdo.diffv(input = ' '.join(files), options='-s'), cdo.diffv(input = files, options='-s'))
+        self.assertEqual([],cdo.diffv(input = files, options='-s'))
         # check for operator input
-        self.assertEqual([],cdo.diffv(input = ["-stdatm,0","-stdatm,0"]))
+        self.assertEqual([],cdo.diffv(input = ["-stdatm,0","-stdatm,0"], options='-s'))
         # check for operator input and files
-        self.assertEqual([],cdo.diffv(input = ["-stdatm,0",fileB]))
+        self.assertEqual([],cdo.diffv(input = ["-stdatm,0",fileB], options='-s'))
         rm([fileA, fileB])
 
     def test_splitOps(self):
         cdo = Cdo()
         cdo.debug = DEBUG
         pattern = 'stdAtm_{0}'.format( random.randrange(1,100000))
         cdo.__print__('test_splitOps')
@@ -792,14 +813,16 @@
       self.assertEqual(0,len(os.listdir(tempPath)))
 
     def testVerifyGrid(self):
       cdo = Cdo()
       output = cdo.verifygrid(input='-topo,global_10')
       self.assertEqual([],output)
 
+      self.assertEqual(True,cdo.silent)
+
       cdo.silent = False
       output = cdo.verifygrid(input='-topo,global_10')
       if parse_version('2.0.6') <= parse_version(cdo.version()):
         expectedOutput = ['cdo    verifygrid: Grid consists of 648 (36x18) cells (type: lonlat), of which',
                           'cdo    verifygrid:       648 cells have 4 vertices',
                           'cdo    verifygrid:        72 cells have duplicate vertices',
                           'cdo    verifygrid:        lon : -175 to 175 degrees',
@@ -809,36 +832,48 @@
                           'cdo    verifygrid: Grid consists of 648 (36x18) cells (type: lonlat), of which',
                           'cdo    verifygrid:       648 cells have 4 vertices',
                           'cdo    verifygrid:        72 cells have duplicate vertices',
                           'cdo    verifygrid:        lon : -175 to 175 degrees',
                           'cdo    verifygrid:        lat : -85 to 85 degrees',
                           'cdo(1) topo:',
                           'cdo    verifygrid: Processed 1 variable [0.00s 94MB].']
+        expectedOutput = expectedOutput[0:-2]
+        output = output[0:-2]
       elif parse_version('2.0.0') > parse_version(cdo.version()):
         # versions 1.9.x and earlier write to stderr and will not be tested
         expectedOutput = []
       else:
         expectedOutput = []
 
       self.assertEqual(expectedOutput,output)
       cdo.silent = True
 
 
     if MAINTAINERMODE:
 
       def test_config(self):
         cdo = Cdo()
-        if (parse_version(cdo.version()) > parse_version('1.9.8')):
+        if (parse_version(cdo.version()) > parse_version('1.9.8') and
+            parse_version(cdo.version()) <= parse_version('2.0.0')):
           self.assertEqual({'has-cgribex': 'yes', 'has-cmor': 'no', 'has-ext': 'yes', 'has-grb': 'yes', 'has-grb1': 'yes', 'has-grb2': 'yes', 'has-hdf5': 'yes', 'has-ieg': 'yes', 'has-nc': 'yes', 'has-nc2': 'yes', 'has-nc4': 'yes', 'has-nc4c': 'yes', 'has-nc5': 'yes', 'has-openmp': 'yes', 'has-proj': 'yes', 'has-srv': 'yes', 'has-threads': 'yes', 'has-wordexp': 'yes'},
               cdo.config)
+        else:
+          self.assertEqual({'has-cgribex': 'yes', 'has-cmor': 'no', 'has-ext': 'yes', 'has-grb': 'yes', 'has-grb1': 'yes', 'has-grb2': 'yes', 'has-hdf5': 'yes', 'has-ieg': 'yes', 'has-nc': 'yes', 'has-nc2': 'yes', 'has-nc4': 'yes', 'has-nc4c': 'yes', 'has-nc5': 'yes', 'has-openmp': 'yes', 'has-proj': 'yes', 'has-srv': 'yes', 'has-threads': 'yes', 'has-wordexp': 'yes', 'has-nczarr': 'yes', 'has-magics': 'yes', 'has-hirlam_extensions': 'no'},
+              cdo.config)
 
       def test_system_tempdir(self):
-        # automatic path
-        tempPath = tempfile.gettempdir()
-        cdo = Cdo()
+        # system tempdir migh be cluttered with other stuff, so lets use a
+        # private directory
+        import tempfile
+        tempfile.tempdir = os.path.abspath('.')
+
+        # create and use local tempdir
+        tempPath = tempfile.mkdtemp()
+        cdo = Cdo(tempdir=tempPath)
+
         cdo.topo('r10x10',options = '-f nc')
         self.assertEqual(1,len([ f for f in os.listdir(tempPath) if 'cdoPy' in f]))
         cdo.topo('r10x10',options = '-f nc')
         cdo.topo('r10x10',options = '-f nc')
         self.assertEqual(3,len([ f for f in os.listdir(tempPath) if 'cdoPy' in f]))
         cdo.topo('r10x10',options = '-f nc')
         cdo.topo('r10x10',options = '-f nc')
@@ -897,71 +932,101 @@
           cdf     = cdo.readCdf(cdfFile)
           if (parse_version(cdo.version()) < parse_version('1.9.8')):
             self.assertEqual(sorted(['lat','lon','for','time']),sorted(list(cdf.variables.keys())))
           else:
             self.assertEqual(sorted(['lat','lon','seq','time']),sorted(list(cdf.variables.keys())))
 
       def test_phc(self):
-        if os.path.isfile(DATA_DIR + '/icon/phc.nc'):
-          ifile = "-select,level=0 " + DATA_DIR + '/icon/phc.nc'
+        ifile = DATA_DIR + '/icon/phc.nc'
+        if os.path.isfile(ifile):
+          ifile = "-setctomiss,nan -select,level=0,timestep=1 " + DATA_DIR + '/icon/phc.nc'
           cdo = Cdo()
           cdo.debug = DEBUG
           if not cdo.hasNetcdf:
             return
+          saltVarname, tempVarname = 'salt', 'temp'
           #cdo.merge(input='/home/ram/data/icon/input/phc3.0/PHC__3.0__TempO__1x1__annual.nc /home/ram/data/icon/input/phc3.0/PHC__3.0__SO__1x1__annual.nc',
           #          output=ifile,
           #          options='-O')
-          s = cdo.sellonlatbox(0,30,0,90, input="-chname,SO,s,TempO,t " + ifile,output='test_my_phc.nc',returnMaArray='s',options='-f nc')
-          plot(np.flipud(s[0,:,:]),ofile='org',title='original')
-          sfmo = cdo.sellonlatbox(0,30,0,90, input="-fillmiss -chname,SO,s,TempO,t " + ifile,returnMaArray='s',options='-f nc')
-          plot(np.flipud(sfmo[0,:,:]),ofile='fm',title='fillmiss')
-          sfm = cdo.sellonlatbox(0,30,0,90, input="-fillmiss2 -chname,SO,s,TempO,t " + ifile,returnMaArray='s',options='-f nc')
-          plot(np.flipud(sfm[0,:,:]),ofile='fm2',title='fillmiss2')
-          ssetmisstonn = cdo.sellonlatbox(0,30,0,90, input="-setmisstonn -chname,SO,s,TempO,t " + ifile,returnMaArray='s',options='-f nc')
-          plot(np.flipud(ssetmisstonn[0,:,:]),ofile='setmisstonn',title='setmisstonn')
+          s = cdo.sellonlatbox(0,30,0,90, input=ifile,output='test_my_phc.nc',returnMaArray=saltVarname,options='-f nc')[0,0,:,:]
+          plot(s,ofile='org',title='original')
+
+          sfmo = cdo.sellonlatbox(0,30,0,90, input="-fillmiss " + ifile,returnMaArray=saltVarname,options='-f nc')[0,0,:,:]
+          plot(sfmo,ofile='fm',title='fillmiss')
+
+          sfm = cdo.sellonlatbox(0,30,0,90, input="-fillmiss2 " + ifile,returnMaArray=saltVarname,options='-f nc')[0,0,:,:]
+          plot(sfm,ofile='fm2',title='fillmiss2')
+
+          ssetmisstonn = cdo.sellonlatbox(0,30,0,90, input="-setmisstonn " + ifile,returnMaArray=saltVarname,options='-f nc')[0,0,:,:]
+          plot(ssetmisstonn,ofile='setmisstonn',title='setmisstonn')
+
           if (parse_version(cdo.version()) >= parse_version('1.7.2')):
-            smooth = cdo.sellonlatbox(0,30,0,90, input="-smooth -chname,SO,s,TempO,t " + ifile,returnMaArray='s',options='-f nc')
-            plot(np.flipud(ssetmisstonn[0,:,:]),ofile='smooth',title='smooth')
+            smooth = cdo.sellonlatbox(0,30,0,90, input="-smooth " + ifile,returnMaArray=saltVarname,options='-f nc')[0,0,:,:]
+            plot(ssetmisstonn,ofile='smooth',title='smooth')
           #global plot
           #s_global = cdo.chname('SO,s,TempO,t',input=ifile,output='my_phc.nc',returnMaArray='s',options='-f nc')
           #plot(s_global[0,:,:],ofile='org_global',title='org_global')
           #sfmo_global = cdo.fillmiss(input=" -chname,SO,s,TempO,t " + ifile,returnMaArray='s',options='-f nc')
           #plot(sfmo_global[0,:,:],ofile='fm_global',title='fm_global')
           #sfm_global = cdo.fillmiss2(input=" -chname,SO,s,TempO,t " + ifile,returnMaArray='s',options='-f nc')
           #plot(sfm_global[0,:,:],ofile='fm2_global',title='fm2_global')
           #ssetmisstonn_global = cdo.setmisstonn(input=" -chname,SO,s,TempO,t " + ifile,returnMaArray='s',options='-f nc')
           #plot(ssetmisstonn_global[0,:,:],ofile='setmisstonn_global',title='setmisstonn_global')
+        else:
+          print(f"Could not find data '{ifile}'")
 
       def test_smooth(self):
         if os.path.isfile(DATA_DIR + '/icon/phc.nc'):
+          saltVarname, tempVarname = 'salt', 'temp'
+          selectionOperator = 'sellonlatbox'
+          region = "0,30,30,90"
+          regionSelection = f"-{selectionOperator},{region}"
           cdo = Cdo()
           if (parse_version(cdo.version()) >= parse_version('1.7.2') and cdo.hasNetcdf):
-            ifile = "-select,level=0 " + DATA_DIR + '/icon/phc.nc'
+            ifile = "-setctomiss,nan -select,level=0,timestep=1 " + DATA_DIR + '/icon/phc.nc'
             cdo = Cdo()
             cdo.debug = DEBUG
             #cdo.merge(input='/home/ram/data/icon/input/phc3.0/PHC__3.0__TempO__1x1__annual.nc /home/ram/data/icon/input/phc3.0/PHC__3.0__SO__1x1__annual.nc',
             #          output=ifile,
             #          options='-O')
-            smooth = cdo.smooth(input=" -sellonlatbox,0,30,0,90 -chname,SO,s,TempO,t " + ifile, returnMaArray='s',options='-f nc')
-            plot(np.flipud(smooth[0,:,:]),ofile='smooth',title='smooth')
-
-            smooth2 = cdo.smooth('nsmooth=2',input="-sellonlatbox,0,30,0,90 -chname,SO,s,TempO,t " + ifile, returnMaArray='s',options='-f nc')
-            plot(np.flipud(smooth2[0,:,:]),ofile='smooth2',title='smooth,nsmooth=2')
-
-            smooth4 = cdo.smooth('nsmooth=4',input="-sellonlatbox,0,30,0,90 -chname,SO,s,TempO,t " + ifile, returnMaArray='s',options='-f nc')
-            plot(np.flipud(smooth4[0,:,:]),ofile='smooth4',title='smooth,nsmooth=4')
-
-            smooth9 = cdo.smooth9(input="-sellonlatbox,0,30,0,90 -chname,SO,s,TempO,t " + ifile, returnMaArray='s',options='-f nc')
-            plot(np.flipud(smooth9[0,:,:]),ofile='smooth9',title='smooth9')
-
-            smooth3deg = cdo.smooth('radius=6deg',input="-sellonlatbox,0,30,0,90 -chname,SO,s,TempO,t " + ifile, returnMaArray='s',options='-f nc')
-            plot(np.flipud(smooth3deg[0,:,:]),ofile='smooth3deg',title='smooth,radius=6deg')
-
-            smooth20 = cdo.smooth('nsmooth=20',input="-sellonlatbox,0,30,0,90 -chname,SO,s,TempO,t " + ifile, returnMaArray='s',options='-f nc')
-            plot(np.flipud(smooth20[0,:,:]),ofile='smooth20',title='smooth,nsmooth=20')
+            org, tag = cdo.sellonlatbox(region,input=ifile, returnMaArray=saltVarname)[0,0,:,:], 'org'
+            plot(org,ofile=tag,title=tag)
+            smooth, tag = cdo.smooth(input=f" {regionSelection} {ifile}",
+                                options='-L',
+                                returnMaArray=saltVarname)[0,0,:,:], 'smooth'
+            plot(smooth,ofile=tag,title=tag)
+
+            smooth2, tag = cdo.smooth('nsmooth=2',
+                                 input=f" {regionSelection} {ifile}",
+                                 options='-L',
+                                 returnMaArray=saltVarname)[0,0,:,:], 'smooth2'
+            plot(np.flipud(smooth2),ofile=tag,title='smooth,nsmooth=2')
+            print(smooth - org)
+
+            smooth4 = cdo.smooth('nsmooth=4',
+                                 input=f" {regionSelection} {ifile}",
+                                 options='-L',
+                                 returnMaArray=saltVarname)[0,0,:,:]
+            plot(np.flipud(smooth4),ofile='smooth4',title='smooth,nsmooth=4')
+
+            smooth9 = cdo.smooth9(input=f" {regionSelection} {ifile}",
+                                  options='-L',
+                                  returnMaArray=saltVarname)[0,0,:,:]
+            plot(np.flipud(smooth9),ofile='smooth9',title='smooth9')
+
+            smooth3deg = cdo.smooth('radius=6deg',
+                                    input=f" {regionSelection} {ifile}",options='-L',
+                                    returnMaArray=saltVarname)[0,0,:,:]
+            plot(np.flipud(smooth3deg),ofile='smooth3deg',title='smooth,radius=6deg')
+
+            smooth20 = cdo.smooth('nsmooth=20',
+                                  input=f" {regionSelection} {ifile}",
+                                  options='-L',
+                                  returnMaArray=saltVarname)[0,0,:,:]
+            plot(np.flipud(smooth20),ofile='smooth20',title='smooth,nsmooth=20')
 
       def test_ydiv(self):
         cdo = Cdo()
         cdo.debug = True
         if ('yeardiv' in cdo.operators):
           input = "-expr,'seq=seq*cyear()/seq;' -settaxis,2001-01-01,12:00:00,12hours -for,1,10000 -yearmean -expr,'seq=seq*cyear()/seq;' -settaxis,2001-01-01,12:00:00,12hours -for,1,10000"
           values = cdo.yeardiv(input=input,returnArray='seq')
@@ -977,14 +1042,27 @@
         cdo.debug = True
         gridfile  = '/home/ram/Downloads/gridfile.txt'
         inputfile = '/home/ram/Downloads/tmax.txt'
         cdo.settaxis('1979-01-01,00:12:00,1days',
             options = ' -r -f nc',
             input = "-setname,tmax -setctomiss,-999.99 -input,{} tmax.nc < ".format(gridfile),
             output = inputfile)
+
+      def test_pauline(self):
+        ifile='/home/ram/local/data/cdo/pauline.nc'
+        cdo = Cdo()
+        (var,) = cdo.showname(input=ifile)
+        x = cdo.selyear('1985/2100', input=ifile, returnXArray=var)
+        print(x)
+        self.assertEqual((4018, 7, 5),x[:,:,:].shape)
+        y = cdo.yearsum(input=x, returnXArray=var)
+        print(y)
+        self.assertEqual((11, 7, 5),y[:,:,:].shape)
+
+
 #===============================================================================
 if __name__ == '__main__':
     suite = testLoader.loadTestsFromTestCase(CdoTest)
 #   print(suite)
     testModule.main()
 #   unittest.TextTestRunner(verbosity=2).run(suite)
```

