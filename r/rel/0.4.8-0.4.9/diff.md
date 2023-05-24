# Comparing `tmp/rel-0.4.8-py2.py3-none-any.whl.zip` & `tmp/rel-0.4.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 11377 bytes, number of entries: 13
--rw-r--r--  2.0 unx      284 b- defN 21-Dec-14 01:33 rel/__init__.py
+Zip file size: 12679 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      296 b- defN 23-May-24 01:42 rel/__init__.py
 -rw-r--r--  2.0 unx       35 b- defN 20-Nov-15 23:15 rel/errors.py
--rw-r--r--  2.0 unx     5526 b- defN 21-Oct-07 03:45 rel/listener.py
--rw-r--r--  2.0 unx     8061 b- defN 23-Jan-28 03:39 rel/registrar.py
--rw-r--r--  2.0 unx     6445 b- defN 21-Nov-30 22:18 rel/rel.py
--rw-r--r--  2.0 unx     6276 b- defN 20-Nov-15 23:15 rel/test.py
--rw-r--r--  2.0 unx     3695 b- defN 20-Nov-15 23:15 rel/tools.py
--rw-r--r--  2.0 unx       22 b- defN 23-Jan-28 03:42 rel/version.py
--rw-r--r--  2.0 unx      829 b- defN 23-Jan-28 03:44 rel-0.4.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jan-28 03:44 rel-0.4.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 23-Jan-28 03:44 rel-0.4.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 23-Jan-28 03:44 rel-0.4.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      929 b- defN 23-Jan-28 03:44 rel-0.4.8.dist-info/RECORD
-13 files, 32283 bytes uncompressed, 9859 bytes compressed:  69.5%
+-rw-r--r--  2.0 unx     5986 b- defN 23-Feb-10 07:02 rel/listener.py
+-rw-r--r--  2.0 unx    10028 b- defN 23-Feb-10 07:02 rel/registrar.py
+-rw-r--r--  2.0 unx     7412 b- defN 23-May-24 01:41 rel/rel.py
+-rw-r--r--  2.0 unx     6175 b- defN 23-Feb-10 07:02 rel/test.py
+-rw-r--r--  2.0 unx     4802 b- defN 23-May-24 01:41 rel/tools.py
+-rw-r--r--  2.0 unx       22 b- defN 23-May-24 01:47 rel/version.py
+-rw-r--r--  2.0 unx      803 b- defN 23-May-24 01:49 rel-0.4.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-24 01:49 rel-0.4.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-May-24 01:49 rel-0.4.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-May-24 01:49 rel-0.4.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      930 b- defN 23-May-24 01:49 rel-0.4.9.dist-info/RECORD
+13 files, 36649 bytes uncompressed, 11161 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: rel/tools.py
 Comment: 
 
 Filename: rel/version.py
 Comment: 
 
-Filename: rel-0.4.8.dist-info/METADATA
+Filename: rel-0.4.9.dist-info/METADATA
 Comment: 
 
-Filename: rel-0.4.8.dist-info/WHEEL
+Filename: rel-0.4.9.dist-info/WHEEL
 Comment: 
 
-Filename: rel-0.4.8.dist-info/entry_points.txt
+Filename: rel-0.4.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: rel-0.4.8.dist-info/top_level.txt
+Filename: rel-0.4.9.dist-info/top_level.txt
 Comment: 
 
-Filename: rel-0.4.8.dist-info/RECORD
+Filename: rel-0.4.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rel/__init__.py

```diff
@@ -1,2 +1,2 @@
 from .version import __version__
-from .rel import override, supported_methods, initialize, set_sleep, set_turbo, safe_read, read, write, timeout, signal, event, dispatch, loop, report, abort, abort_branch, thread, tick, init, sys, EV_PERSIST, EV_READ, EV_SIGNAL, EV_TIMEOUT, EV_WRITE
+from .rel import override, supported_methods, initialize, set_sleep, set_turbo, safe_read, read, write, timeout, signal, event, dispatch, loop, report, is_running, abort, abort_branch, thread, tick, init, sys, EV_PERSIST, EV_READ, EV_SIGNAL, EV_TIMEOUT, EV_WRITE
```

## rel/listener.py

```diff
@@ -1,7 +1,26 @@
+"""
+This module includes four classes: Event, SocketIO, Signal, and Timer.
+
+### Event
+This class uses a Registrar subclass instance to manage read, write,
+signal, and timeout events.
+
+### SocketIO
+This class uses a Registrar subclass instance to manage read, and
+write events.
+
+### Signal
+This class uses the signal library and a Registrar subclass instance
+to manage signal events.
+
+### Timer
+This class uses a Registrar subclass to manage timer events.
+"""
+
 import time
 import signal
 
 EV_PERSIST = 16
 EV_READ = 2
 EV_SIGNAL = 8
 EV_TIMEOUT = 1
```

## rel/registrar.py

```diff
@@ -1,7 +1,60 @@
+"""
+This module includes the Registrar class and four subclasses,
+KqueueRegistrar, SelectRegistrar, PollRegistrar, and EpollRegistrar,
+each of which utilizes a different subsystem (kqueue, select, poll,
+or epoll) to manage read and write events. Registrar and its subclasses
+also manage signals and timers.
+
+### Reads and Writes
+Reads and writes are handled by the SocketIO class defined in the
+listener module, which is instantiated by a couple Registrar functions:
+
+    def read(self,sock,cb,*args):
+        return SocketIO(self,'read',sock,cb,*args)
+
+    def write(self,sock,cb,*args):
+        return SocketIO(self,'write',sock,cb,*args)
+
+### Signals and Timers
+Signals and timers are handled by the Signal and Timer classes
+defined in the listener module, which can be instantiated through
+a couple Registrar functions:
+
+    def signal(self,sig,cb,*args):
+        return Signal(self,sig,cb,*args)
+
+    def timeout(self,delay,cb,*args):
+        return Timer(self,delay,cb,*args)
+
+The Registrar API is taken from [pyevent](https://github.com/jaraco/pyevent),
+which is a wrapper around [libevent](http://monkey.org/~provos/libevent/).
+
+Note that while rel can be configured to use pyevent under the hood
+(instead of one of the Registrar subclasses), such usage forfeits
+various benefits of the pure-Python Registrar subclasses, including
+GIL integration / thread compatibility.
+
+### Event Engine Rates
+Another benefit of the pure-Python Registrar subclasses (wrapping epoll,
+poll, kqueue, and select - by default, rel uses the fastest available) is
+that they run at configurable rates. By default, rel's CPU footprint is
+unnoticeably tiny unless it's currently managing active writes, in which
+case it ramps up to push the bytes through faster. These rates (normal
+and turbo) can be adjusted with a couple functions:
+
+    def set_sleep(s):
+        global SLEEP_SEC
+        SLEEP_SEC = s
+
+    def set_turbo(s):
+        global SLEEP_TURBO
+        SLEEP_TURBO = s
+"""
+
 from datetime import datetime
 from .listener import Event, SocketIO, Timer, Signal, contains
 from .errors import AbortBranch
 import select, signal, time, operator
 try:
     import epoll
 except ImportError:
```

## rel/rel.py

```diff
@@ -1,22 +1,45 @@
 """
 R.E.L.
-Registed Event Listener
-module that uses various methods to emulate event-like behavior
-functions:
+Registed Event Listener is a pure-python implementation of [pyevent](https://github.com/jaraco/pyevent),
+which is a wrapper around [libevent](http://monkey.org/~provos/libevent/), providing an identical interface
+without the need to compile C code, and without breaking the GIL / threading.
+
+### basic functions:
     read(socket, callback, *args)
     write(socket, callback, *args)
     timeout(delay, callback, *args)
     signal(sig, callback, *args)
     event(callback,arg=None,evtype=0,handle=None)
     dispatch()
     loop()
     abort()
+    abort_branch() (non-pyevent only)
+    thread()
     init()
+
+### registrars
+rel will use the fastest registrar available on your system:
+
+    supported_methods = ['epoll','poll','kqueue','select','pyevent']
+
+The supported_methods[] registrar priority list, as well as other
+settings, can be altered using the (optional) initialize() function:
+
+### initialize(methods=supported_methods,options=()) - possible options:
+    'verbose' - prints out certain events
+    'report' - prints status of non-pyevent registrar every 5 seconds
+    'strict' - ONLY try specified methods
+    'threaded' - enable GIL hack -- pyevent only!
+
+### override()
+This override function can be used to seamlessly swap rel into
+a pyevent application.
 """
+
 import sys, threading, time, pprint
 from .registrar import set_sleep, set_turbo, SelectRegistrar, PollRegistrar, EpollRegistrar, KqueueRegistrar
 from .listener import EV_PERSIST, EV_READ, EV_SIGNAL, EV_TIMEOUT, EV_WRITE
 try:
     import event as pyevent
 except ImportError:
     pyevent = None
@@ -208,14 +231,17 @@
     check_init()
     registrar.loop()
 
 def report():
     check_init()
     return registrar.report()
 
+def is_running():
+    return running
+
 def abort():
     global running
     running = False
     check_init()
     registrar.abort()
 
 def abort_branch():
```

## rel/test.py

```diff
@@ -1,25 +1,20 @@
-#!/usr/bin/env python
-# -*- coding: us-ascii -*-
-# vim:ts=4:sw=4:softtabstop=4:smarttab:expandtab
-#
 """
 REL Test Suite - regular unittest compatible suite
 Submitted by Chris Clark on 10/12/2011. Thanks, Chris!
 
 Original code here:
 http://code.google.com/r/clach04-pyeventtestfixes/source/browse/test.py
 
 Sample usage:
 
     rel\test.py
     rel\test.py -v
     rel\test.py -v EventTest.test_exception EventTest.test_timeout
     ... etc.
-
 """
 
 from . import rel
 rel.override()
 
 import glob
 import os
```

## rel/tools.py

```diff
@@ -1,9 +1,52 @@
-### rel tools module.
-### (mostly rel example code)
+"""
+This module contains a single tool (Timer) and a
+CLI wrapper (timerCLI()).
+
+### Timer
+Timer's start() function contains basic usage examples
+of the timeout(), signal(), and dispatch() functions:
+
+    def start(self):
+        self.count = 0
+        notice("starting countdown to %s"%(self.goal,))
+        rel.timeout(1, self.update)
+        rel.signal(2, self.stop)
+        rel.dispatch()
+
+Similarly, Timer.stop() triggers rel.abort().
+
+### timerCLI
+This function contains an example of rel initialization,
+which is optional, but may be used to specify particular
+settings:
+
+    if options.verbose:
+        rel.initialize(options=["verbose"])
+
+### usage
+
+    rtimer [seconds] [minutes] [hours] [update_increment]
+
+All arguments default to zero. So:
+
+    rtimer 15 30 2 60
+
+means run for 15 seconds, 30 minutes, and 2 hours, printing
+a notice every 60 seconds.
+
+    rtimer 0 5
+
+means run for 5 minutes, printing no incremental updates.
+
+When the time runs out, a sound will play on two conditions:
+there is a readable file at the specified path (configurable
+via the -m flag, with default: /var/local/rtimer_elapsed.mp3),
+and mplayer is installed.
+"""
 
 import rel
 try:
     from subprocess import getoutput # py3
 except:
     from commands import getoutput # py2
 
@@ -11,15 +54,15 @@
 
 def notice(*lines):
     print("")
     print("\n".join(lines))
 
 def exit():
     notice("goodbye")
-    if rel.running:
+    if rel.is_running():
         rel.abort()
     else:
         import sys
         sys.exit()
 
 def error(msg, *lines):
     notice("fatal exception!", "error: %s"%(msg,), *lines)
```

## rel/version.py

```diff
@@ -1 +1 @@
-__version__ = "0.4.8"
+__version__ = "0.4.9"
```

## Comparing `rel-0.4.8.dist-info/METADATA` & `rel-0.4.9.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: rel
-Version: 0.4.8
+Version: 0.4.9
 Summary: Registered Event Listener. Provides standard (pyevent) interface and functionality without external dependencies
-Home-page: UNKNOWN
 Author: Mario Balibrera
 Author-email: mario.balibrera@gmail.com
 License: MIT License
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 
 Select preferred event notification methods with initialize([methods in order of preference]). If initialize(...) is not called, methods are tried in default order: pyevent,epoll,poll,kqueue,select.
-
```

