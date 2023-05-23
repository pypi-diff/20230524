# Comparing `tmp/cqlsh_expansion-0.7.8-py2-none-any.whl.zip` & `tmp/cqlsh_expansion-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,31 +1,40 @@
-Zip file size: 142733 bytes, number of entries: 29
--rw-r--r--  2.0 unx        5 b- defN 21-Nov-12 16:04 config/__init__.py
--rw-r--r--  2.0 unx      334 b- defN 21-Nov-12 16:04 config/cqlshrc_template
--rw-r--r--  2.0 unx     2418 b- defN 21-Nov-12 16:04 config/post_install.py
--rw-r--r--  2.0 unx     1468 b- defN 21-Nov-12 16:04 config/sf-class2-root.crt
--rwxr-xr-x  2.0 unx     1353 b- defN 21-Nov-12 16:04 cqlsh_expansion-0.7.8.data/scripts/cqlsh
--rwxr-xr-x  2.0 unx     1373 b- defN 21-Nov-12 16:04 cqlsh_expansion-0.7.8.data/scripts/cqlsh-expansion
--rwxr-xr-x  2.0 unx   100781 b- defN 21-Nov-17 19:43 cqlsh_expansion-0.7.8.data/scripts/cqlsh-expansion.py
--rwxr-xr-x  2.0 unx    99075 b- defN 21-Nov-12 16:04 cqlsh_expansion-0.7.8.data/scripts/cqlsh.py
--rw-r--r--  2.0 unx      784 b- defN 21-Nov-12 16:04 cqlshlib/__init__.py
--rw-r--r--  2.0 unx   110284 b- defN 21-Nov-12 16:04 cqlshlib/copyutil.py
--rw-r--r--  2.0 unx    55339 b- defN 21-Nov-12 16:04 cqlshlib/cql3handling.py
--rw-r--r--  2.0 unx    13013 b- defN 21-Nov-12 16:04 cqlshlib/cqlhandling.py
--rw-r--r--  2.0 unx    10295 b- defN 21-Nov-12 16:04 cqlshlib/cqlshhandling.py
--rw-r--r--  2.0 unx     3977 b- defN 21-Nov-12 16:04 cqlshlib/displaying.py
--rw-r--r--  2.0 unx    23604 b- defN 21-Nov-12 16:04 cqlshlib/formatting.py
--rw-r--r--  2.0 unx     4532 b- defN 21-Nov-12 16:04 cqlshlib/helptopics.py
--rw-r--r--  2.0 unx    18855 b- defN 21-Nov-12 16:04 cqlshlib/pylexotron.py
--rw-r--r--  2.0 unx     2711 b- defN 21-Nov-12 16:04 cqlshlib/saferscanner.py
--rw-r--r--  2.0 unx     3725 b- defN 21-Nov-12 16:04 cqlshlib/sslhandling.py
--rw-r--r--  2.0 unx     3486 b- defN 21-Nov-12 16:04 cqlshlib/tracing.py
--rw-r--r--  2.0 unx     4525 b- defN 21-Nov-12 16:04 cqlshlib/util.py
--rw-r--r--  2.0 unx    15875 b- defN 21-Nov-12 16:04 cqlshlib/wcwidth.py
--rw-r--r--  2.0 unx      927 b- defN 21-Nov-17 19:45 cqlsh_expansion-0.7.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    10894 b- defN 21-Nov-17 19:45 cqlsh_expansion-0.7.8.dist-info/METADATA
--rw-r--r--  2.0 unx    36491 b- defN 21-Nov-17 19:45 cqlsh_expansion-0.7.8.dist-info/THIRD-PARTY-LICENSES.txt
--rw-r--r--  2.0 unx       92 b- defN 21-Nov-17 19:45 cqlsh_expansion-0.7.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       93 b- defN 21-Nov-17 19:45 cqlsh_expansion-0.7.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 21-Nov-17 19:45 cqlsh_expansion-0.7.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2482 b- defN 21-Nov-17 19:45 cqlsh_expansion-0.7.8.dist-info/RECORD
-29 files, 528807 bytes uncompressed, 138743 bytes compressed:  73.8%
+Zip file size: 270570 bytes, number of entries: 38
+-rw-r--r--  2.0 unx        5 b- defN 21-Nov-22 18:22 config/__init__.py
+-rw-r--r--  2.0 unx     7061 b- defN 23-May-17 17:23 config/cqlshrc_template
+-rw-r--r--  2.0 unx     6991 b- defN 23-Apr-03 09:14 config/cqlshrc_template_4x
+-rw-r--r--  2.0 unx     2418 b- defN 23-Apr-03 11:55 config/post_install.py
+-rw-r--r--  2.0 unx     1468 b- defN 21-Nov-22 18:22 config/sf-class2-root.crt
+-rwxr-xr-x  2.0 unx     3062 b- defN 23-May-17 17:23 cqlsh_expansion-0.9.0.data/scripts/cqlsh
+-rwxr-xr-x  2.0 unx     3072 b- defN 23-May-17 17:23 cqlsh_expansion-0.9.0.data/scripts/cqlsh-expansion
+-rwxr-xr-x  2.0 unx    98927 b- defN 23-May-17 17:33 cqlsh_expansion-0.9.0.data/scripts/cqlsh-expansion.py
+-rwxr-xr-x  2.0 unx    96804 b- defN 23-May-17 17:33 cqlsh_expansion-0.9.0.data/scripts/cqlsh.py
+-rw-r--r--  2.0 unx   113007 b- defN 23-May-15 06:10 cqlshlib/411copyutil.py
+-rw-r--r--  2.0 unx      784 b- defN 23-Apr-03 09:08 cqlshlib/__init__.py
+-rw-r--r--  2.0 unx     7078 b- defN 23-May-17 17:23 cqlshlib/authproviderhandling.py
+-rw-r--r--  2.0 unx   113001 b- defN 23-May-17 17:23 cqlshlib/copyutil.py
+-rw-r--r--  2.0 unx   113007 b- defN 23-May-15 06:10 cqlshlib/copyutil411.py
+-rw-r--r--  2.0 unx    58090 b- defN 23-May-17 17:23 cqlshlib/cql3handling.py
+-rw-r--r--  2.0 unx     1704 b- defN 23-May-09 14:07 cqlshlib/cqlexpansion.py
+-rw-r--r--  2.0 unx    13103 b- defN 23-May-17 17:23 cqlshlib/cqlhandling.py
+-rw-r--r--  2.0 unx    10454 b- defN 23-May-17 17:23 cqlshlib/cqlshhandling.py
+-rw-r--r--  2.0 unx    95680 b- defN 23-Jan-03 12:27 cqlshlib/cqlshmain.py
+-rw-r--r--  2.0 unx     4245 b- defN 23-May-11 20:37 cqlshlib/describecqlexpansion.py
+-rw-r--r--  2.0 unx     3977 b- defN 23-Apr-03 09:08 cqlshlib/displaying.py
+-rw-r--r--  2.0 unx    23470 b- defN 23-May-17 17:23 cqlshlib/formatting.py
+-rw-r--r--  2.0 unx     4524 b- defN 23-May-17 17:23 cqlshlib/helptopics.py
+-rw-r--r--  2.0 unx   112092 b- defN 23-May-15 05:50 cqlshlib/legacycopyutil.py
+-rw-r--r--  2.0 unx     8627 b- defN 23-May-17 17:23 cqlshlib/legacydesc3x.py
+-rw-r--r--  2.0 unx    18528 b- defN 23-May-17 17:23 cqlshlib/pylexotron.py
+-rw-r--r--  2.0 unx     3429 b- defN 23-May-17 17:23 cqlshlib/saferscanner.py
+-rw-r--r--  2.0 unx     3739 b- defN 23-May-17 17:23 cqlshlib/sslhandling.py
+-rw-r--r--  2.0 unx     3403 b- defN 23-May-17 17:23 cqlshlib/tracing.py
+-rw-r--r--  2.0 unx     5057 b- defN 23-May-17 17:23 cqlshlib/util.py
+-rw-r--r--  2.0 unx    15865 b- defN 23-May-17 17:23 cqlshlib/wcwidth.py
+-rw-r--r--  2.0 unx      927 b- defN 23-May-17 17:33 cqlsh_expansion-0.9.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    10461 b- defN 23-May-17 17:33 cqlsh_expansion-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx    36491 b- defN 23-May-17 17:33 cqlsh_expansion-0.9.0.dist-info/THIRD-PARTY-LICENSES.txt
+-rw-r--r--  2.0 unx       92 b- defN 23-May-17 17:33 cqlsh_expansion-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       92 b- defN 23-May-17 17:33 cqlsh_expansion-0.9.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-May-17 17:33 cqlsh_expansion-0.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3233 b- defN 23-May-17 17:33 cqlsh_expansion-0.9.0.dist-info/RECORD
+38 files, 1003984 bytes uncompressed, 265434 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -1,55 +1,82 @@
 Filename: config/__init__.py
 Comment: 
 
 Filename: config/cqlshrc_template
 Comment: 
 
+Filename: config/cqlshrc_template_4x
+Comment: 
+
 Filename: config/post_install.py
 Comment: 
 
 Filename: config/sf-class2-root.crt
 Comment: 
 
-Filename: cqlsh_expansion-0.7.8.data/scripts/cqlsh
+Filename: cqlsh_expansion-0.9.0.data/scripts/cqlsh
 Comment: 
 
-Filename: cqlsh_expansion-0.7.8.data/scripts/cqlsh-expansion
+Filename: cqlsh_expansion-0.9.0.data/scripts/cqlsh-expansion
 Comment: 
 
-Filename: cqlsh_expansion-0.7.8.data/scripts/cqlsh-expansion.py
+Filename: cqlsh_expansion-0.9.0.data/scripts/cqlsh-expansion.py
 Comment: 
 
-Filename: cqlsh_expansion-0.7.8.data/scripts/cqlsh.py
+Filename: cqlsh_expansion-0.9.0.data/scripts/cqlsh.py
+Comment: 
+
+Filename: cqlshlib/411copyutil.py
 Comment: 
 
 Filename: cqlshlib/__init__.py
 Comment: 
 
+Filename: cqlshlib/authproviderhandling.py
+Comment: 
+
 Filename: cqlshlib/copyutil.py
 Comment: 
 
+Filename: cqlshlib/copyutil411.py
+Comment: 
+
 Filename: cqlshlib/cql3handling.py
 Comment: 
 
+Filename: cqlshlib/cqlexpansion.py
+Comment: 
+
 Filename: cqlshlib/cqlhandling.py
 Comment: 
 
 Filename: cqlshlib/cqlshhandling.py
 Comment: 
 
+Filename: cqlshlib/cqlshmain.py
+Comment: 
+
+Filename: cqlshlib/describecqlexpansion.py
+Comment: 
+
 Filename: cqlshlib/displaying.py
 Comment: 
 
 Filename: cqlshlib/formatting.py
 Comment: 
 
 Filename: cqlshlib/helptopics.py
 Comment: 
 
+Filename: cqlshlib/legacycopyutil.py
+Comment: 
+
+Filename: cqlshlib/legacydesc3x.py
+Comment: 
+
 Filename: cqlshlib/pylexotron.py
 Comment: 
 
 Filename: cqlshlib/saferscanner.py
 Comment: 
 
 Filename: cqlshlib/sslhandling.py
@@ -60,29 +87,29 @@
 
 Filename: cqlshlib/util.py
 Comment: 
 
 Filename: cqlshlib/wcwidth.py
 Comment: 
 
-Filename: cqlsh_expansion-0.7.8.dist-info/LICENSE.txt
+Filename: cqlsh_expansion-0.9.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: cqlsh_expansion-0.7.8.dist-info/METADATA
+Filename: cqlsh_expansion-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: cqlsh_expansion-0.7.8.dist-info/THIRD-PARTY-LICENSES.txt
+Filename: cqlsh_expansion-0.9.0.dist-info/THIRD-PARTY-LICENSES.txt
 Comment: 
 
-Filename: cqlsh_expansion-0.7.8.dist-info/WHEEL
+Filename: cqlsh_expansion-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: cqlsh_expansion-0.7.8.dist-info/entry_points.txt
+Filename: cqlsh_expansion-0.9.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: cqlsh_expansion-0.7.8.dist-info/top_level.txt
+Filename: cqlsh_expansion-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: cqlsh_expansion-0.7.8.dist-info/RECORD
+Filename: cqlsh_expansion-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## config/cqlshrc_template

```diff
@@ -1,23 +1,249 @@
+; Licensed to the Apache Software Foundation (ASF) under one
+; or more contributor license agreements.  See the NOTICE file
+; distributed with this work for additional information
+; regarding copyright ownership.  The ASF licenses this file
+; to you under the Apache License, Version 2.0 (the
+; "License"); you may not use this file except in compliance
+; with the License.  You may obtain a copy of the License at
+;
+;   http://www.apache.org/licenses/LICENSE-2.0
+;
+; Unless required by applicable law or agreed to in writing,
+; software distributed under the License is distributed on an
+; "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+; KIND, either express or implied.  See the License for the
+; specific language governing permissions and limitations
+; under the License.
+;
+; Sample ~/.cqlshrc file.
+
+[authentication]
+;; If Cassandra has auth enabled, fill out these options
+;; Path to the credentials file, an initial ~ or ~user is expanded to that user's home directory
+; credentials = ~/.cassandra/credentials
+; keyspace = ks1
+
+[auth_provider]
+;; you can specify any auth provider found in your python environment
+;; module and class will be used to dynamically load the class
+;; all other properties found here and in the credentials file under the class name
+;; will be passed to the constructor
+module = cassandra_sigv4.auth
+classname = SigV4AuthProvider
+;region_name = us-east-1
+; module = cassandra.auth
+; classname = PlainTextAuthProvider
+
+[ui]
+;; Whether or not to display query results with colors
+; color = on
+
+;; Used for displaying timestamps (and reading them with COPY)
+; time_format = %Y-%m-%d %H:%M:%S%z
+
+;; Display timezone
+;timezone = Etc/UTC
+
+;; The number of digits displayed after the decimal point for single and double precision numbers
+;; (note that increasing this to large numbers can result in unusual values)
+;float_precision = 5
+;double_precision = 12
+
+;; Used for automatic completion and suggestions
+; completekey = tab
+
+;; The encoding used for characters
+; encoding = utf8
+
+; To use another than the system default browser for cqlsh HELP to open
+; the CQL doc HTML, use the 'browser' preference.
+; If the field value is empty or not specified, cqlsh will use the
+; default browser (specifying 'browser = default' does not work).
+;
+; Supported browsers are those supported by the Python webbrowser module.
+; (https://docs.python.org/3/library/webbrowser.html).
+;
+; Hint: to use Google Chome, use
+; 'browser = open -a /Applications/Google\ Chrome.app %s' on Mac OS X and
+; 'browser = /usr/bin/google-chrome-stable %s' on Linux and
+; 'browser = C:/Program Files (x86)/Google/Chrome/Application/chrome.exe %s' on Windows.
+;
+; This setting can be overridden with the --browser command line option.
+;
+;browser =
+
+[cql]
+;; A version of CQL to use (this should almost never be set)
+; version = 3.2.1
+
+
+
 [connection]
+
+;; The host to connect to
+hostname = 127.0.0.1
+
+;; The port to connect to (9042 is the native protocol default)
 port = 9142
-factory = cqlshlib.ssl.ssl_transport_factory
+
+;; Always connect using SSL - false by default
+ssl = true
+
+;; A timeout in seconds for opening new connections
+; timeout = 10
+
+;; A timeout in seconds for executing queries
+; request_timeout = 10
+
+
+
+[csv]
+;; The size limit for parsed fields
+field_size_limit = 999999
+
+
+
+[tracing]
+;; The max number of seconds to wait for a trace to complete
+; max_trace_wait = 10.0
+
+
 
 [ssl]
-validate = true
-certfile =  ~/.cassandra/sf-class2-root.crt
-version = TLSv1_2
+certfile = ~/.cassandra/sf-class2-root.crt
 
+;; Optional - true by default.
+;validate = true
+
+;; To be provided when require_client_auth=true
+;userkey = ~/key.pem
+
+;; To be provided when require_client_auth=true
+;usercert = ~/cert.pem
+
+; this is effectively ignored from 4.1 included as TLS protocol is auto-negotiated and will
+; be removed in the next major version of Cassandra, possible values were TLSv1, TLSv1_1 or TLSv1_2
+;version = TLSv1_2
+
+;; Optional section, overrides default certfile in [ssl] section, if present
+; [certfiles]
+; 192.168.1.3 = ~/keys/cassandra01.cert
+; 192.168.1.4 = ~/keys/cassandra02.cert
+
+
+
+;; Options that are common to both COPY TO and COPY FROM
 [copy]
-NUMPROCESSES=16
-MAXATTEMPTS=25
 
+;; The string placeholder for null values
+; nullval = null
+
+;; For COPY TO, controls whether the first line in the CSV output file will
+;; contain the column names.  For COPY FROM, specifies whether the first
+;; line in the CSV file contains column names.
+; header = false
+
+;; The character that is used as the decimal point separator
+; decimalsep = .
+
+;; The character that is used to separate thousands
+;; (defaults to the empty string)
+; thousandssep =
+
+;; The string literal format for boolean values
+; boolstyle = True,False
+
+;; The number of child worker processes to create for
+;; COPY tasks.  Defaults to a max of 4 for COPY FROM and 16
+;; for COPY TO.  However, at most (num_cores - 1) processes
+;; will be created.
+numprocesses = 16
+
+;; The maximum number of failed attempts to fetch a range of data (when using
+;; COPY TO) or insert a chunk of data (when using COPY FROM) before giving up
+maxattempts = 25
+
+;; How often status updates are refreshed, in seconds
+; reportfrequency = 0.25
+
+;; An optional file to output rate statistics to
+; ratefile =
+
+
+
+;; Options specific to COPY TO
+; [copy-to]
+
+;; The maximum number token ranges to fetch simultaneously
+; maxrequests = 6
+
+;; The number of rows to fetch in a single page
+; pagesize = 1000
+
+;; By default the page timeout is 10 seconds per 1000 entries
+;; in the page size or 10 seconds if pagesize is smaller
+; pagetimeout = 10
+
+;; Token range to export.  Defaults to exporting the full ring.
+; begintoken =
+; endtoken =
+
+; The maximum size of the output file measured in number of lines;
+; beyond this maximum the output file will be split into segments.
+; -1 means unlimited.
+; maxoutputsize = -1
+
+;; The encoding used for characters
+; encoding = utf8
+
+
+
+;; Options specific to COPY FROM
 [copy-from]
-CHUNKSIZE=30
-INGESTRATE=1500
-MAXINSERTERRORS=-1
-MAXPARSEERRORS=-1
-MINBATCHSIZE=1
-MAXBATCHSIZE=10
 
-[csv]
-field_size_limit=999999
+;; The maximum number of rows to process per second
+ingestrate = 1500
+
+;; The maximum number of rows to import (-1 means unlimited)
+; maxrows = -1
+
+;; A number of initial rows to skip
+; skiprows = 0
+
+;; A comma-separated list of column names to ignore
+; skipcols =
+
+;; The maximum global number of parsing errors to ignore, -1 means unlimited
+maxparseerrors = -1
+
+;; The maximum global number of insert errors to ignore, -1 means unlimited
+maxinserterrors = -1
+
+;; A file to store all rows that could not be imported, by default this is
+;; import_<ks>_<table>.err where <ks> is your keyspace and <table> is your table name.
+; errfile =
+
+;; The min and max number of rows inserted in a single batch
+maxbatchsize = 10
+minbatchsize = 1
+
+;; The number of rows that are passed to child worker processes from
+;; the main process at a time
+chunksize =  30
+
+
+
+;; The options for COPY can also be specified per-table.  The following
+;; three sections demonstrate this.
+
+;; Optional table-specific options for COPY
+; [copy:mykeyspace.mytable]
+; chunksize = 1000
+
+;; Optional table-specific options for COPY FROM
+; [copy-from:mykeyspace.mytable]
+; ingestrate = 20000
+
+;; Optional table-specific options for COPY TO
+; [copy-to:mykeyspace.mytable]
+; pagetimeout = 30
```

## cqlshlib/copyutil.py

```diff
@@ -12,59 +12,61 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import ConfigParser
 import csv
 import datetime
 import json
 import glob
 import multiprocessing as mp
 import os
 import platform
 import random
 import re
+import signal
 import struct
 import sys
 import threading
 import time
 import traceback
 
 from bisect import bisect_right
 from calendar import timegm
 from collections import defaultdict, namedtuple
 from decimal import Decimal
-from Queue import Queue
 from random import randint
-from StringIO import StringIO
+from io import StringIO
 from select import select
 from uuid import UUID
-from util import profile_on, profile_off
+
+import configparser
+from queue import Queue
 
 from cassandra import OperationTimedOut
 from cassandra.cluster import Cluster, DefaultConnection
-from cassandra.cqltypes import ReversedType, UserType
+from cassandra.cqltypes import ReversedType, UserType, VarcharType
 from cassandra.metadata import protect_name, protect_names, protect_value
 from cassandra.policies import RetryPolicy, WhiteListRoundRobinPolicy, DCAwareRoundRobinPolicy, FallthroughRetryPolicy
 from cassandra.query import BatchStatement, BatchType, SimpleStatement, tuple_factory
 from cassandra.util import Date, Time
+from cqlshlib.util import profile_on, profile_off
 
-from cql3handling import CqlRuleSet
-from displaying import NO_COLOR_MAP
-from formatting import format_value_default, CqlType, DateTimeFormat, EMPTY, get_formatter, BlobType
-from sslhandling import ssl_settings
+from cqlshlib.cql3handling import CqlRuleSet
+from cqlshlib.displaying import NO_COLOR_MAP
+from cqlshlib.formatting import format_value_default, CqlType, DateTimeFormat, EMPTY, get_formatter, BlobType
+from cqlshlib.sslhandling import ssl_settings
 
 PROFILE_ON = False
 STRACE_ON = False
 DEBUG = False  # This may be set to True when initializing the task
+# TODO: review this for MacOS, maybe use in ('Linux', 'Darwin')
 IS_LINUX = platform.system() == 'Linux'
-IS_WINDOWS = platform.system() == 'Windows'
 
 CopyOptions = namedtuple('CopyOptions', 'copy dialect unrecognized')
 
 
 def safe_normpath(fname):
     """
     :return the normalized path but only if there is a filename, we don't want to convert
@@ -74,25 +76,20 @@
 
 
 def printdebugmsg(msg):
     if DEBUG:
         printmsg(msg)
 
 
-def printmsg(msg, eol='\n', encoding='utf8'):
-    sys.stdout.write(msg.encode(encoding))
+def printmsg(msg, eol='\n'):
+    sys.stdout.write(msg)
     sys.stdout.write(eol)
     sys.stdout.flush()
 
 
-# Keep arguments in sync with printmsg
-def swallowmsg(msg, eol='', encoding=''):
-    None
-
-
 class OneWayPipe(object):
     """
     A one way pipe protected by two process level locks, one for reading and one for writing.
     """
     def __init__(self):
         self.reader, self.writer = mp.Pipe(duplex=False)
         self.rlock = mp.Lock()
@@ -134,16 +131,16 @@
         self.pending_messages = Queue()
 
         def feed():
             while True:
                 try:
                     msg = self.pending_messages.get()
                     self.pipe.send(msg)
-                except Exception, e:
-                    printmsg('%s: %s' % (e.__class__.__name__, e.message))
+                except Exception as e:
+                    printmsg('%s: %s' % (e.__class__.__name__, e.message if hasattr(e, 'message') else str(e)))
 
         feeding_thread = threading.Thread(target=feed)
         feeding_thread.setDaemon(True)
         feeding_thread.start()
 
     def send(self, obj):
         self.pending_messages.put(obj)
@@ -156,46 +153,52 @@
 
 
 class SendingChannels(object):
     """
     A group of one way channels for sending messages.
     """
     def __init__(self, num_channels):
-        self.pipes = [OneWayPipe() for _ in xrange(num_channels)]
+        self.pipes = [OneWayPipe() for _ in range(num_channels)]
         self.channels = [SendingChannel(p) for p in self.pipes]
         self.num_channels = num_channels
 
     def close(self):
         for ch in self.channels:
             try:
                 ch.close()
-            except Exception:
+            except ValueError:
                 pass
 
 
 class ReceivingChannels(object):
     """
     A group of one way channels for receiving messages.
     """
     def __init__(self, num_channels):
-        self.pipes = [OneWayPipe() for _ in xrange(num_channels)]
+        self.pipes = [OneWayPipe() for _ in range(num_channels)]
         self.channels = [ReceivingChannel(p) for p in self.pipes]
         self._readers = [p.reader for p in self.pipes]
         self._rlocks = [p.rlock for p in self.pipes]
         self._rlocks_by_readers = dict([(p.reader, p.rlock) for p in self.pipes])
         self.num_channels = num_channels
 
         self.recv = self.recv_select if IS_LINUX else self.recv_polling
 
     def recv_select(self, timeout):
         """
         Implementation of the recv method for Linux, where select is available. Receive an object from
         all pipes that are ready for reading without blocking.
         """
-        readable, _, _ = select(self._readers, [], [], timeout)
+        while True:
+            try:
+                readable, _, _ = select(self._readers, [], [], timeout)
+            except OSError:
+                raise
+            else:
+                break
         for r in readable:
             with self._rlocks_by_readers[r]:
                 try:
                     yield r.recv()
                 except EOFError:
                     continue
 
@@ -218,15 +221,15 @@
             if time.time() - start > timeout:
                 break
 
     def close(self):
         for ch in self.channels:
             try:
                 ch.close()
-            except Exception:
+            except ValueError:
                 pass
 
 
 class CopyTask(object):
     """
     A base class for ImportTask and ExportTask
     """
@@ -242,16 +245,15 @@
 
         # if cqlsh is invoked with --debug then set the global debug flag to True
         if shell.debug:
             global DEBUG
             DEBUG = True
 
         # do not display messages when exporting to STDOUT unless --debug is set
-        self.printmsg = printmsg if self.fname is not None or direction == 'from' or DEBUG \
-            else swallowmsg
+        self.printmsg = printmsg if self.fname is not None or direction == 'from' or DEBUG else None
         self.options = self.parse_options(opts, direction)
 
         self.num_processes = self.options.copy['numprocesses']
         self.encoding = self.options.copy['encoding']
         self.printmsg('Using %d child processes' % (self.num_processes,))
 
         if direction == 'from':
@@ -272,16 +274,16 @@
         config_file = opts.pop('configfile', '')
         if not config_file:
             config_file = self.config_file
 
         if not os.path.isfile(config_file):
             return opts
 
-        configs = ConfigParser.RawConfigParser()
-        configs.readfp(open(config_file))
+        configs = configparser.RawConfigParser()
+        configs.read_file(open(config_file))
 
         ret = dict()
         config_sections = list(['copy', 'copy-%s' % (direction,),
                                 'copy:%s.%s' % (self.ks, self.table),
                                 'copy-%s:%s.%s' % (direction, self.ks, self.table)])
 
         for section in config_sections:
@@ -301,16 +303,16 @@
         return ret
 
     @staticmethod
     def clean_options(opts):
         """
         Convert all option values to valid string literals unless they are path names
         """
-        return dict([(k, v.decode('string_escape') if k not in ['errfile', 'ratefile'] else v)
-                     for k, v, in opts.iteritems()])
+        return dict([(k, v if k not in ['errfile', 'ratefile'] else v)
+                     for k, v, in opts.items()])
 
     def parse_options(self, opts, direction):
         """
         Parse options for import (COPY FROM) and export (COPY TO) operations.
         Extract from opts csv and dialect options.
 
         :return: 3 dictionaries: the csv options, the dialect options, any unrecognized options.
@@ -469,36 +471,35 @@
     def stop_processes(self):
         for process in self.processes:
             process.terminate()
 
     def make_params(self):
         """
         Return a dictionary of parameters to be used by the worker processes.
-        On Windows this dictionary must be pickle-able, therefore we do not pass the
-        parent connection since it may not be pickle-able. Also, on Windows child
-        processes are spawned and not forked, and therefore we don't need to shutdown
-        the parent connection anyway, see CASSANDRA-11749 for more details.
+        On platforms using 'spawn' as the default multiprocessing start method,
+        this dictionary must be picklable.
         """
         shell = self.shell
 
         return dict(ks=self.ks,
                     table=self.table,
                     local_dc=self.host.datacenter,
                     columns=self.columns,
                     options=self.options,
                     connect_timeout=shell.conn.connect_timeout,
                     hostname=self.host.address,
                     port=shell.port,
                     ssl=shell.ssl,
                     auth_provider=shell.auth_provider,
-                    parent_cluster=shell.conn if not IS_WINDOWS else None,
                     cql_version=shell.conn.cql_version,
                     config_file=self.config_file,
                     protocol_version=self.protocol_version,
-                    debug=shell.debug
+                    debug=shell.debug,
+                    coverage=shell.coverage,
+                    coveragerc_path=shell.coveragerc_path
                     )
 
     def validate_columns(self):
         shell = self.shell
 
         if not self.columns:
             shell.printerr("No column specified")
@@ -530,15 +531,15 @@
 
     def __init__(self, fname, shell, columns, options):
         self.fname = fname
         self.shell = shell
         self.columns = columns
         self.options = options
         self.header = options.copy['header']
-        self.max_output_size = long(options.copy['maxoutputsize'])
+        self.max_output_size = int(options.copy['maxoutputsize'])
         self.current_dest = None
         self.num_files = 0
 
         if self.max_output_size > 0:
             if fname is not None:
                 self.write = self._write_with_split
                 self.num_written = 0
@@ -551,15 +552,15 @@
     def open(self):
         self.current_dest = self._get_dest(self.fname)
         if self.current_dest is None:
             return False
 
         if self.header:
             writer = csv.writer(self.current_dest.output, **self.options.dialect)
-            writer.writerow(self.columns)
+            writer.writerow([str(c) for c in self.columns])
 
         return True
 
     def close(self):
         self._close_current_dest()
 
     def _next_dest(self):
@@ -573,18 +574,18 @@
         """
         CsvDest = namedtuple('CsvDest', 'output close')
 
         if self.fname is None:
             return CsvDest(output=sys.stdout, close=False)
         else:
             try:
-                ret = CsvDest(output=open(source_name, 'wb'), close=True)
+                ret = CsvDest(output=open(source_name, 'w'), close=True)
                 self.num_files += 1
                 return ret
-            except IOError, e:
+            except IOError as e:
                 self.shell.printerr("Can't open %r for writing: %s" % (source_name, e))
                 return None
 
     def _close_current_dest(self):
         if self.current_dest and self.current_dest.close:
             self.current_dest.output.close()
             self.current_dest = None
@@ -600,15 +601,15 @@
          Write the data to the current destination output if we still
          haven't reached the maximum number of rows. Otherwise split
          the rows between the current destination and the next.
         """
         if (self.num_written + num) > self.max_output_size:
             num_remaining = self.max_output_size - self.num_written
             last_switch = 0
-            for i, row in enumerate(filter(None, data.split(os.linesep))):
+            for i, row in enumerate([_f for _f in data.split(os.linesep) if _f]):
                 if i == num_remaining:
                     self._next_dest()
                     last_switch = i
                     num_remaining += self.max_output_size
                 self.current_dest.output.write(row + '\n')
 
             self.num_written = num - last_switch
@@ -621,44 +622,44 @@
     """
     A class that exports data to .csv by instantiating one or more processes that work in parallel (ExportProcess).
     """
     def __init__(self, shell, ks, table, columns, fname, opts, protocol_version, config_file):
         CopyTask.__init__(self, shell, ks, table, columns, fname, opts, protocol_version, config_file, 'to')
 
         options = self.options
-        self.begin_token = long(options.copy['begintoken']) if options.copy['begintoken'] else None
-        self.end_token = long(options.copy['endtoken']) if options.copy['endtoken'] else None
+        self.begin_token = int(options.copy['begintoken']) if options.copy['begintoken'] else None
+        self.end_token = int(options.copy['endtoken']) if options.copy['endtoken'] else None
         self.writer = ExportWriter(fname, shell, columns, options)
 
     def run(self):
         """
         Initiates the export by starting the worker processes.
         Then hand over control to export_records.
         """
         shell = self.shell
 
         if self.options.unrecognized:
-            shell.printerr('Unrecognized COPY TO options: %s' % ', '.join(self.options.unrecognized.keys()))
+            shell.printerr('Unrecognized COPY TO options: %s' % ', '.join(list(self.options.unrecognized.keys())))
             return
 
         if not self.validate_columns():
             return 0
 
         ranges = self.get_ranges()
         if not ranges:
             return 0
 
         if not self.writer.open():
             return 0
 
-        columns = u"[" + u", ".join(self.columns) + u"]"
-        self.printmsg(u"\nStarting copy of %s.%s with columns %s." % (self.ks, self.table, columns), encoding=self.encoding)
+        columns = "[" + ", ".join(self.columns) + "]"
+        self.printmsg("\nStarting copy of %s.%s with columns %s." % (self.ks, self.table, columns))
 
         params = self.make_params()
-        for i in xrange(self.num_processes):
+        for i in range(self.num_processes):
             self.processes.append(ExportProcess(self.update_params(params, i)))
 
         self.start_processes()
 
         try:
             self.export_records(ranges)
         finally:
@@ -691,23 +692,23 @@
         def make_range(prev, curr):
             """
             Return the intersection of (prev, curr) and (begin_token, end_token),
             return None if the intersection is empty
             """
             ret = (prev, curr)
             if begin_token:
-                if ret[1] < begin_token:
+                if curr < begin_token:
                     return None
-                elif ret[0] < begin_token:
-                    ret = (begin_token, ret[1])
+                elif (prev is None) or (prev < begin_token):
+                    ret = (begin_token, curr)
 
             if end_token:
-                if ret[0] > end_token:
+                if (ret[0] is not None) and (ret[0] > end_token):
                     return None
-                elif ret[1] > end_token:
+                elif (curr is not None) and (curr > end_token):
                     ret = (ret[0], end_token)
 
             return ret
 
         def make_range_data(replicas=None):
             hosts = []
             if replicas:
@@ -726,15 +727,15 @@
             shell.printerr('Begin token %d must be smaller than end token %d' % (begin_token, end_token))
             return ranges
 
         if shell.conn.metadata.token_map is None or min_token is None:
             ranges[(begin_token, end_token)] = make_range_data()
             return ranges
 
-        ring = shell.get_ring(self.ks).items()
+        ring = list(shell.get_ring(self.ks).items())
         ring.sort()
 
         if not ring:
             #  If the ring is empty we get the entire ring from the host we are currently connected to
             ranges[(begin_token, end_token)] = make_range_data()
         elif len(ring) == 1:
             #  If there is only one token we get the entire ring from the replicas for that token
@@ -756,14 +757,18 @@
 
                 ranges[current_range] = make_range_data(replicas)
                 previous = token.value
 
             #  For the last ring interval we query the same replicas that hold the first token in the ring
             if previous is not None and (not end_token or previous < end_token):
                 ranges[(previous, end_token)] = first_range_data
+            # TODO: fix this logic added in 4.0: if previous is None, then it can't be compared with less than
+            elif previous is None and (not end_token or previous < end_token):
+                previous = begin_token if begin_token else min_token
+                ranges[(previous, end_token)] = first_range_data
 
         if not ranges:
             shell.printerr('Found no ranges to query, check begin and end tokens: %s - %s' % (begin_token, end_token))
 
         return ranges
 
     def get_min_token(self):
@@ -805,15 +810,15 @@
         processes = self.processes
         meter = RateMeter(log_fcn=self.printmsg,
                           update_interval=self.options.copy['reportfrequency'],
                           log_file=self.options.copy['ratefile'])
         total_requests = len(ranges)
         max_attempts = self.options.copy['maxattempts']
 
-        self.send_work(ranges, ranges.keys())
+        self.send_work(ranges, list(ranges.keys()))
 
         num_processes = len(processes)
         succeeded = 0
         failed = 0
         while (failed + succeeded) < total_requests and self.num_live_processes() == num_processes:
             for token_range, result in self.inmsg.recv(timeout=0.1):
                 if token_range is None and result is None:  # a request has finished
@@ -864,42 +869,43 @@
     """
     def __init__(self, fname, options):
         self.chunk_size = options.copy['chunksize']
         self.header = options.copy['header']
         self.max_rows = options.copy['maxrows']
         self.skip_rows = options.copy['skiprows']
         self.fname = fname
-        self.sources = None  # must be created later due to pickle problems on Windows
+        self.sources = None  # might be initialised directly here? (see CASSANDRA-17350)
         self.num_sources = 0
         self.current_source = None
         self.num_read = 0
 
-    def get_source(self, paths):
+    @staticmethod
+    def get_source(paths):
         """
          Return a source generator. Each source is a named tuple
          wrapping the source input, file name and a boolean indicating
          if it requires closing.
         """
         def make_source(fname):
             try:
-                return open(fname, 'rb')
-            except IOError, e:
+                return open(fname, 'r')
+            except IOError as e:
                 raise IOError("Can't open %r for reading: %s" % (fname, e))
 
         for path in paths.split(','):
             path = path.strip()
             if os.path.isfile(path):
                 yield make_source(path)
             else:
                 result = glob.glob(path)
                 if len(result) == 0:
                     raise IOError("Can't open %r for reading: no matching file found" % (path,))
 
                 for f in result:
-                    yield (make_source(f))
+                    yield make_source(f)
 
     def start(self):
         self.sources = self.get_source(self.fname)
         self.next_source()
 
     @property
     def exhausted(self):
@@ -909,22 +915,22 @@
         """
          Close the current source, if any, and open the next one. Return true
          if there is another source, false otherwise.
         """
         self.close_current_source()
         while self.current_source is None:
             try:
-                self.current_source = self.sources.next()
+                self.current_source = next(self.sources)
                 if self.current_source:
                     self.num_sources += 1
             except StopIteration:
                 return False
 
         if self.header:
-            self.current_source.next()
+            next(self.current_source)
 
         return True
 
     def close_current_source(self):
         if not self.current_source:
             return
 
@@ -935,31 +941,31 @@
         self.close_current_source()
 
     def read_rows(self, max_rows):
         if not self.current_source:
             return []
 
         rows = []
-        for i in xrange(min(max_rows, self.chunk_size)):
+        for i in range(min(max_rows, self.chunk_size)):
             try:
-                row = self.current_source.next()
+                row = next(self.current_source)
                 self.num_read += 1
 
                 if 0 <= self.max_rows < self.num_read:
                     self.next_source()
                     break
 
                 if self.num_read > self.skip_rows:
                     rows.append(row)
 
             except StopIteration:
                 self.next_source()
                 break
 
-        return filter(None, rows)
+        return [_f for _f in rows if _f]
 
 
 class PipeReader(object):
     """
     A class for reading rows received on a pipe, this is used for reading input from STDIN
     """
     def __init__(self, inpipe, options):
@@ -973,15 +979,15 @@
         self.num_sources = 1
 
     def start(self):
         pass
 
     def read_rows(self, max_rows):
         rows = []
-        for i in xrange(min(max_rows, self.chunk_size)):
+        for i in range(min(max_rows, self.chunk_size)):
             row = self.inpipe.recv()
             if row is None:
                 self.exhausted = True
                 break
 
             self.num_read += 1
             if 0 <= self.max_rows < self.num_read:
@@ -1139,45 +1145,44 @@
 
         return True
 
     def run(self):
         shell = self.shell
 
         if self.options.unrecognized:
-            shell.printerr('Unrecognized COPY FROM options: %s' % ', '.join(self.options.unrecognized.keys()))
+            shell.printerr('Unrecognized COPY FROM options: %s' % ', '.join(list(self.options.unrecognized.keys())))
             return
 
         if not self.validate_columns():
             return 0
 
-        columns = u"[" + u", ".join(self.valid_columns) + u"]"
-        self.printmsg(u"\nStarting copy of %s.%s with columns %s." % (self.ks, self.table, columns), encoding=self.encoding)
+        columns = "[" + ", ".join(self.valid_columns) + "]"
+        self.printmsg("\nStarting copy of %s.%s with columns %s." % (self.ks, self.table, columns))
 
         try:
             params = self.make_params()
 
             for i in range(self.num_processes - 1):
                 self.processes.append(ImportProcess(self.update_params(params, i)))
 
             feeder = FeedingProcess(self.outmsg.pipes[-1], self.inmsg.pipes[-1],
-                                    self.outmsg.pipes[:-1], self.fname, self.options,
-                                    self.shell.conn if not IS_WINDOWS else None)
+                                    self.outmsg.pipes[:-1], self.fname, self.options)
             self.processes.append(feeder)
 
             self.start_processes()
 
             pr = profile_on() if PROFILE_ON else None
 
             self.import_records()
 
             if pr:
                 profile_off(pr, file_name='parent_profile_%d.txt' % (os.getpid(),))
 
-        except Exception, exc:
-            shell.printerr(unicode(exc))
+        except Exception as exc:
+            shell.printerr(str(exc))
             if shell.debug:
                 traceback.print_exc()
             return 0
         finally:
             self.close()
 
     def send_stdin_rows(self):
@@ -1191,15 +1196,15 @@
 
         self.printmsg("[Use . on a line by itself to end input]")
         for row in shell.use_stdin_reader(prompt='[copy] ', until=r'.'):
             self.outmsg.channels[-1].send(row)
 
         self.outmsg.channels[-1].send(None)
         if shell.tty:
-            print
+            print()
 
     def import_records(self):
         """
         Keep on running until we have stuff to receive or send and until all processes are running.
         Send data (batches or retries) up to the max ingest rate. If we are waiting for stuff to
         receive check the incoming queue.
         """
@@ -1243,15 +1248,15 @@
         # allow time for worker processes to exit cleanly
         attempts = 50  # 100 milliseconds per attempt, so 5 seconds total
         while attempts > 0 and self.num_live_processes() > 0:
             time.sleep(0.1)
             attempts -= 1
 
         self.printmsg("\n%d rows imported from %d files in %s (%d skipped)." %
-                      (self.receive_meter.get_total_records(),
+                      (self.receive_meter.get_total_records() - self.error_handler.num_rows_failed,
                        self.feeding_result.num_sources if self.feeding_result else 0,
                        self.describe_interval(time.time() - self.time_start),
                        self.feeding_result.skip_rows if self.feeding_result else 0))
 
     def all_processes_running(self):
         return self.num_live_processes() == len(self.processes)
 
@@ -1275,43 +1280,38 @@
             self.receive_meter.increment(aggregate_result.imported)
 
 
 class FeedingProcess(mp.Process):
     """
     A process that reads from import sources and sends chunks to worker processes.
     """
-    def __init__(self, inpipe, outpipe, worker_pipes, fname, options, parent_cluster):
-        mp.Process.__init__(self, target=self.run)
+    def __init__(self, inpipe, outpipe, worker_pipes, fname, options):
+        super(FeedingProcess, self).__init__(target=self.run)
         self.inpipe = inpipe
         self.outpipe = outpipe
         self.worker_pipes = worker_pipes
-        self.inmsg = None  # must be created after forking on Windows
-        self.outmsg = None  # must be created after forking on Windows
-        self.worker_channels = None  # must be created after forking on Windows
+        self.inmsg = None  # might be initialised directly here? (see CASSANDRA-17350)
+        self.outmsg = None  # might be initialised directly here? (see CASSANDRA-17350)
+        self.worker_channels = None  # might be initialised directly here? (see CASSANDRA-17350)
         self.reader = FilesReader(fname, options) if fname else PipeReader(inpipe, options)
         self.send_meter = RateMeter(log_fcn=None, update_interval=1)
         self.ingest_rate = options.copy['ingestrate']
         self.num_worker_processes = options.copy['numprocesses']
         self.max_pending_chunks = options.copy['maxpendingchunks']
         self.chunk_id = 0
-        self.parent_cluster = parent_cluster
 
     def on_fork(self):
         """
         Create the channels and release any parent connections after forking,
         see CASSANDRA-11749 for details.
         """
         self.inmsg = ReceivingChannel(self.inpipe)
         self.outmsg = SendingChannel(self.outpipe)
         self.worker_channels = [SendingChannel(p) for p in self.worker_pipes]
 
-        if self.parent_cluster:
-            printdebugmsg("Closing parent cluster sockets")
-            self.parent_cluster.shutdown()
-
     def run(self):
         pr = profile_on() if PROFILE_ON else None
 
         self.inner_run()
 
         if pr:
             profile_off(pr, file_name='feeder_profile_%d.txt' % (os.getpid(),))
@@ -1325,24 +1325,25 @@
         """
 
         self.on_fork()
 
         reader = self.reader
         try:
             reader.start()
-        except IOError, exc:
-            self.outmsg.send(ImportTaskError(exc.__class__.__name__, exc.message))
+        except IOError as exc:
+            self.outmsg.send(
+                ImportTaskError(exc.__class__.__name__, exc.message if hasattr(exc, 'message') else str(exc)))
 
         channels = self.worker_channels
         max_pending_chunks = self.max_pending_chunks
         sent = 0
         failed_attempts = 0
 
         while not reader.exhausted:
-            channels_eligible = filter(lambda c: c.num_pending() < max_pending_chunks, channels)
+            channels_eligible = [c for c in channels if c.num_pending() < max_pending_chunks]
             if not channels_eligible:
                 failed_attempts += 1
                 delay = randint(1, pow(2, failed_attempts))
                 printdebugmsg("All workers busy, sleeping for %d second(s)" % (delay,))
                 time.sleep(delay)
                 continue
             elif failed_attempts > 0:
@@ -1354,16 +1355,17 @@
                     if max_rows <= 0:
                         self.send_meter.maybe_update(sleep=False)
                         continue
 
                     rows = reader.read_rows(max_rows)
                     if rows:
                         sent += self.send_chunk(ch, rows)
-                except Exception, exc:
-                    self.outmsg.send(ImportTaskError(exc.__class__.__name__, exc.message))
+                except Exception as exc:
+                    self.outmsg.send(
+                        ImportTaskError(exc.__class__.__name__, exc.message if hasattr(exc, 'message') else str(exc)))
 
                 if reader.exhausted:
                     break
 
         # send back to the parent process the number of rows sent to the worker processes
         self.outmsg.send(FeedingProcessResult(sent, reader))
 
@@ -1388,30 +1390,29 @@
 
 class ChildProcess(mp.Process):
     """
     An child worker process, this is for common functionality between ImportProcess and ExportProcess.
     """
 
     def __init__(self, params, target):
-        mp.Process.__init__(self, target=target)
+        super(ChildProcess, self).__init__(target=target)
         self.inpipe = params['inpipe']
         self.outpipe = params['outpipe']
-        self.inmsg = None  # must be initialized after fork on Windows
-        self.outmsg = None  # must be initialized after fork on Windows
+        self.inmsg = None  # might be initialised directly here? (see CASSANDRA-17350)
+        self.outmsg = None  # might be initialised directly here? (see CASSANDRA-17350)
         self.ks = params['ks']
         self.table = params['table']
         self.local_dc = params['local_dc']
         self.columns = params['columns']
         self.debug = params['debug']
         self.port = params['port']
         self.hostname = params['hostname']
         self.connect_timeout = params['connect_timeout']
         self.cql_version = params['cql_version']
         self.auth_provider = params['auth_provider']
-        self.parent_cluster = params['parent_cluster']
         self.ssl = params['ssl']
         self.protocol_version = params['protocol_version']
         self.config_file = params['config_file']
 
         options = params['options']
         self.date_time_format = options.copy['dtformats']
         self.consistency_level = options.copy['consistencylevel']
@@ -1421,31 +1422,58 @@
         self.max_attempts = options.copy['maxattempts']
         self.encoding = options.copy['encoding']
         # Here we inject some failures for testing purposes, only if this environment variable is set
         if os.environ.get('CQLSH_COPY_TEST_FAILURES', ''):
             self.test_failures = json.loads(os.environ.get('CQLSH_COPY_TEST_FAILURES', ''))
         else:
             self.test_failures = None
+        # attributes for coverage
+        self.coverage = params['coverage']
+        self.coveragerc_path = params['coveragerc_path']
+        self.coverage_collection = None
+        self.sigterm_handler = None
+        self.sighup_handler = None
 
     def on_fork(self):
         """
         Create the channels and release any parent connections after forking, see CASSANDRA-11749 for details.
         """
         self.inmsg = ReceivingChannel(self.inpipe)
         self.outmsg = SendingChannel(self.outpipe)
 
-        if self.parent_cluster:
-            printdebugmsg("Closing parent cluster sockets")
-            self.parent_cluster.shutdown()
-
     def close(self):
         printdebugmsg("Closing queues...")
         self.inmsg.close()
         self.outmsg.close()
 
+    def start_coverage(self):
+        import coverage
+        self.coverage_collection = coverage.Coverage(config_file=self.coveragerc_path)
+        self.coverage_collection.start()
+
+        # save current handlers for SIGTERM and SIGHUP
+        self.sigterm_handler = signal.getsignal(signal.SIGTERM)
+        self.sighup_handler = signal.getsignal(signal.SIGTERM)
+
+        def handle_sigterm():
+            self.stop_coverage()
+            self.close()
+            self.terminate()
+
+        # set custom handler for SIGHUP and SIGTERM
+        # needed to make sure coverage data is saved
+        signal.signal(signal.SIGTERM, handle_sigterm)
+        signal.signal(signal.SIGHUP, handle_sigterm)
+
+    def stop_coverage(self):
+        self.coverage_collection.stop()
+        self.coverage_collection.save()
+        signal.signal(signal.SIGTERM, self.sigterm_handler)
+        signal.signal(signal.SIGHUP, self.sighup_handler)
+
 
 class ExpBackoffRetryPolicy(RetryPolicy):
     """
     A retry policy with exponential back-off for read timeouts and write timeouts
     """
     def __init__(self, parent_process):
         RetryPolicy.__init__(self)
@@ -1543,17 +1571,21 @@
         self.max_requests = options.copy['maxrequests']
 
         self.hosts_to_sessions = dict()
         self.formatters = dict()
         self.options = options
 
     def run(self):
+        if self.coverage:
+            self.start_coverage()
         try:
             self.inner_run()
         finally:
+            if self.coverage:
+                self.stop_coverage()
             self.close()
 
     def inner_run(self):
         """
         The parent sends us (range, info) on the inbound queue (inmsg)
         in order to request us to process a range, for which we can
         select any of the hosts in info, which also contains other information for this
@@ -1578,15 +1610,15 @@
         if isinstance(err, str):
             msg = err
         elif isinstance(err, BaseException):
             msg = "%s - %s" % (err.__class__.__name__, err)
             if print_traceback and sys.exc_info()[1] == err:
                 traceback.print_exc()
         else:
-            msg = unicode(err)
+            msg = str(err)
         return msg
 
     def report_error(self, err, token_range):
         msg = self.get_error_message(err, print_traceback=self.debug)
         printdebugmsg(msg)
         self.send((token_range, Exception(msg)))
 
@@ -1602,15 +1634,15 @@
         if session:
             metadata = session.cluster.metadata.keyspaces[self.ks].tables[self.table]
             query = self.prepare_query(metadata.partition_key, token_range, info['attempts'])
             future = session.execute_async(query)
             self.attach_callbacks(token_range, future, session)
 
     def num_requests(self):
-        return sum(session.num_requests() for session in self.hosts_to_sessions.values())
+        return sum(session.num_requests() for session in list(self.hosts_to_sessions.values()))
 
     def get_session(self, hosts, token_range):
         """
         We return a session connected to one of the hosts passed in, which are valid replicas for
         the token range. We sort replicas by favouring those without any active requests yet or with the
         smallest number of requests. If we fail to connect we report an error so that the token will
         be retried again later.
@@ -1622,28 +1654,28 @@
                        key=lambda hh: 0 if hh not in self.hosts_to_sessions else self.hosts_to_sessions[hh].requests)
 
         errors = []
         ret = None
         for host in hosts:
             try:
                 ret = self.connect(host)
-            except Exception, e:
+            except Exception as e:
                 errors.append(self.get_error_message(e))
 
             if ret:
                 if errors:
                     printdebugmsg("Warning: failed to connect to some replicas: %s" % (errors,))
                 return ret
 
         self.report_error("Failed to connect to all replicas %s for %s, errors: %s" % (hosts, token_range, errors),
                           token_range)
         return None
 
     def connect(self, host):
-        if host in self.hosts_to_sessions.keys():
+        if host in list(self.hosts_to_sessions.keys()):
             session = self.hosts_to_sessions[host]
             session.add_request()
             return session
 
         new_cluster = Cluster(
             contact_points=(host,),
             port=self.port,
@@ -1687,44 +1719,45 @@
             return  # no rows in this range
 
         try:
             output = StringIO()
             writer = csv.writer(output, **self.options.dialect)
 
             for row in rows:
-                writer.writerow(map(self.format_value, row, cql_types))
+                writer.writerow(list(map(self.format_value, row, cql_types)))
 
             data = (output.getvalue(), len(rows))
             self.send((token_range, data))
             output.close()
 
-        except Exception, e:
+        except Exception as e:
             self.report_error(e, token_range)
 
     def format_value(self, val, cqltype):
         if val is None or val == EMPTY:
             return format_value_default(self.nullval, colormap=NO_COLOR_MAP)
 
         formatter = self.formatters.get(cqltype, None)
         if not formatter:
             formatter = get_formatter(val, cqltype)
             self.formatters[cqltype] = formatter
 
         if not hasattr(cqltype, 'precision'):
             cqltype.precision = self.double_precision if cqltype.type_name == 'double' else self.float_precision
 
-        return formatter(val, cqltype=cqltype,
-                         encoding=self.encoding, colormap=NO_COLOR_MAP, date_time_format=self.date_time_format,
-                         float_precision=cqltype.precision, nullval=self.nullval, quote=False,
-                         decimal_sep=self.decimal_sep, thousands_sep=self.thousands_sep,
-                         boolean_styles=self.boolean_styles)
+        formatted = formatter(val, cqltype=cqltype,
+                              encoding=self.encoding, colormap=NO_COLOR_MAP, date_time_format=self.date_time_format,
+                              float_precision=cqltype.precision, nullval=self.nullval, quote=False,
+                              decimal_sep=self.decimal_sep, thousands_sep=self.thousands_sep,
+                              boolean_styles=self.boolean_styles)
+        return formatted
 
     def close(self):
         ChildProcess.close(self)
-        for session in self.hosts_to_sessions.values():
+        for session in list(self.hosts_to_sessions.values()):
             session.shutdown()
 
     def prepare_query(self, partition_key, token_range, attempts):
         """
         Return the export query or a fake query with some failure injected.
         """
         if self.test_failures:
@@ -1778,14 +1811,30 @@
 
 
 class ParseError(Exception):
     """ We failed to parse an import record """
     pass
 
 
+class ImmutableDict(frozenset):
+    """
+    Immutable dictionary implementation to represent map types.
+    We need to pass BoundStatement.bind() a dict() because it calls iteritems(),
+    except we can't create a dict with another dict as the key, hence we use a class
+    that adds iteritems to a frozen set of tuples (which is how dict are normally made
+    immutable in python).
+    Must be declared in the top level of the module to be available for pickling.
+    """
+    iteritems = frozenset.__iter__
+
+    def items(self):
+        for k, v in self.iteritems():
+            yield k, v
+
+
 class ImportConversion(object):
     """
     A class for converting strings to values when importing from csv, used by ImportProcess,
     the parent.
     """
     def __init__(self, parent, table_meta, statement=None):
         self.ks = parent.ks
@@ -1859,23 +1908,28 @@
             v = unprotect(v)
             if v == self.nullval:
                 return self.get_null_val()
             return converters.get(t.typename, convert_unknown)(v, ct=t)
 
         def convert_mandatory(t, v):
             v = unprotect(v)
-            if v == self.nullval:
+            # we can't distinguish between empty strings and null values in csv. Null values are not supported in
+            # collections, so it must be an empty string.
+            if v == self.nullval and not issubclass(t, VarcharType):
                 raise ParseError('Empty values are not allowed')
             return converters.get(t.typename, convert_unknown)(v, ct=t)
 
         def convert_blob(v, **_):
-            return BlobType(v[2:].decode("hex"))
+            if sys.version_info.major >= 3:
+                return bytes.fromhex(v[2:])
+            else:
+                return BlobType(v[2:].decode("hex"))
 
         def convert_text(v, **_):
-            return v
+            return str(v)
 
         def convert_uuid(v, **_):
             return UUID(v)
 
         def convert_bool(v, **_):
             return True if v.lower() == self.boolean_styles[0].lower() else False
 
@@ -1888,20 +1942,23 @@
             else:
                 return lambda v, ct=cql_type: adapter(v)
 
         def get_convert_decimal_fcn(adapter=float):
             """
             Return a slow and a fast decimal conversion function depending on self.thousands_sep and self.decimal_sep
             """
+            empty_str = ''
+            dot_str = '.'
             if self.thousands_sep and self.decimal_sep:
-                return lambda v, ct=cql_type: adapter(v.replace(self.thousands_sep, '').replace(self.decimal_sep, '.'))
+                return lambda v, ct=cql_type: \
+                    adapter(v.replace(self.thousands_sep, empty_str).replace(self.decimal_sep, dot_str))
             elif self.thousands_sep:
-                return lambda v, ct=cql_type: adapter(v.replace(self.thousands_sep, ''))
+                return lambda v, ct=cql_type: adapter(v.replace(self.thousands_sep, empty_str))
             elif self.decimal_sep:
-                return lambda v, ct=cql_type: adapter(v.replace(self.decimal_sep, '.'))
+                return lambda v, ct=cql_type: adapter(v.replace(self.decimal_sep, dot_str))
             else:
                 return lambda v, ct=cql_type: adapter(v)
 
         def split(val, sep=','):
             """
             Split "val" into a list of values whenever the separator "sep" is found, but
             ignore separators inside parentheses or single quotes, except for the two
@@ -1945,36 +2002,36 @@
             else:
                 if last < len(val) - 1:
                     ret.append(val[last:-1])
 
             return ret
 
         # this should match all possible CQL and CQLSH datetime formats
-        p = re.compile("(\d{4})\-(\d{2})\-(\d{2})\s?(?:'T')?" +  # YYYY-MM-DD[( |'T')]
-                       "(?:(\d{2}):(\d{2})(?::(\d{2})(?:\.(\d{1,6}))?))?" +  # [HH:MM[:SS[.NNNNNN]]]
-                       "(?:([+\-])(\d{2}):?(\d{2}))?")  # [(+|-)HH[:]MM]]
+        p = re.compile(r"(\d{4})-(\d{2})-(\d{2})\s?(?:'T')?"  # YYYY-MM-DD[( |'T')]
+                       + r"(?:(\d{2}):(\d{2})(?::(\d{2})(?:\.(\d{1,6}))?))?"  # [HH:MM[:SS[.NNNNNN]]]
+                       + r"(?:([+\-])(\d{2}):?(\d{2}))?")  # [(+|-)HH[:]MM]]
 
         def convert_datetime(val, **_):
             try:
-                tval = time.strptime(val, self.date_time_format)
-                return timegm(tval) * 1e3  # scale seconds to millis for the raw value
+                dtval = datetime.datetime.strptime(val, self.date_time_format)
+                return dtval.timestamp() * 1000
             except ValueError:
                 pass  # if it's not in the default format we try CQL formats
 
             m = p.match(val)
             if not m:
                 try:
                     # in case of overflow COPY TO prints dates as milliseconds from the epoch, see
                     # deserialize_date_fallback_int in cqlsh.py
                     return int(val)
                 except ValueError:
                     raise ValueError("can't interpret %r as a date with format %s or as int" % (val,
                                                                                                 self.date_time_format))
 
-            # https://docs.python.org/2/library/time.html#time.struct_time
+            # https://docs.python.org/3/library/time.html#time.struct_time
             tval = time.struct_time((int(m.group(1)), int(m.group(2)), int(m.group(3)),  # year, month, day
                                     int(m.group(4)) if m.group(4) else 0,  # hour
                                     int(m.group(5)) if m.group(5) else 0,  # minute
                                     int(m.group(6)) if m.group(6) else 0,  # second
                                     0, 1, -1))  # day of week, day of year, dst-flag
 
             # convert sub-seconds (a number between 1 and 6 digits) to milliseconds
@@ -1982,15 +2039,15 @@
 
             if m.group(8):
                 offset = (int(m.group(9)) * 3600 + int(m.group(10)) * 60) * int(m.group(8) + '1')
             else:
                 offset = -time.timezone
 
             # scale seconds to millis for the raw value
-            return ((timegm(tval) + offset) * 1e3) + milliseconds
+            return ((timegm(tval) + offset) * 1000) + milliseconds
 
         def convert_date(v, **_):
             return Date(v)
 
         def convert_time(v, **_):
             return Time(v)
 
@@ -2001,35 +2058,33 @@
             return tuple(convert_mandatory(ct.subtypes[0], v) for v in split(val))
 
         def convert_set(val, ct=cql_type):
             return frozenset(convert_mandatory(ct.subtypes[0], v) for v in split(val))
 
         def convert_map(val, ct=cql_type):
             """
-            We need to pass to BoundStatement.bind() a dict() because it calls iteritems(),
-            except we can't create a dict with another dict as the key, hence we use a class
-            that adds iteritems to a frozen set of tuples (which is how dict are normally made
-            immutable in python).
+            See ImmutableDict above for a discussion of why a special object is needed here.
             """
-            class ImmutableDict(frozenset):
-                iteritems = frozenset.__iter__
-
+            split_format_str = '{%s}'
+            sep = ':'
             return ImmutableDict(frozenset((convert_mandatory(ct.subtypes[0], v[0]), convert(ct.subtypes[1], v[1]))
-                                 for v in [split('{%s}' % vv, sep=':') for vv in split(val)]))
+                                 for v in [split(split_format_str % vv, sep=sep) for vv in split(val)]))
 
         def convert_user_type(val, ct=cql_type):
             """
             A user type is a dictionary except that we must convert each key into
             an attribute, so we are using named tuples. It must also be hashable,
             so we cannot use dictionaries. Maybe there is a way to instantiate ct
             directly but I could not work it out.
             Also note that it is possible that the subfield names in the csv are in the
             wrong order, so we must sort them according to ct.fieldnames, see CASSANDRA-12959.
             """
-            vals = [v for v in [split('{%s}' % vv, sep=':') for vv in split(val)]]
+            split_format_str = '{%s}'
+            sep = ':'
+            vals = [v for v in [split(split_format_str % vv, sep=sep) for vv in split(val)]]
             dict_vals = dict((unprotect(v[0]), v[1]) for v in vals)
             sorted_converted_vals = [(n, convert(t, dict_vals[n]) if n in dict_vals else self.get_null_val())
                                      for n, t in zip(ct.fieldnames, ct.subtypes)]
             ret_type = namedtuple(ct.typename, [v[0] for v in sorted_converted_vals])
             return ret_type(*tuple(v[1] for v in sorted_converted_vals))
 
         def convert_single_subtype(val, ct=cql_type):
@@ -2049,19 +2104,19 @@
             'decimal': get_convert_decimal_fcn(adapter=Decimal),
             'uuid': convert_uuid,
             'boolean': convert_bool,
             'tinyint': get_convert_integer_fcn(),
             'ascii': convert_text,
             'float': get_convert_decimal_fcn(),
             'double': get_convert_decimal_fcn(),
-            'bigint': get_convert_integer_fcn(adapter=long),
+            'bigint': get_convert_integer_fcn(adapter=int),
             'int': get_convert_integer_fcn(),
             'varint': get_convert_integer_fcn(),
             'inet': convert_text,
-            'counter': get_convert_integer_fcn(adapter=long),
+            'counter': get_convert_integer_fcn(adapter=int),
             'timestamp': convert_datetime,
             'timeuuid': convert_uuid,
             'date': convert_date,
             'smallint': get_convert_integer_fcn(),
             'time': convert_time,
             'text': convert_text,
             'varchar': convert_text,
@@ -2098,25 +2153,25 @@
         for i in self.primary_key_indexes:
             if row[i] == self.nullval:
                 raise ParseError(self.get_null_primary_key_message(i))
 
         def convert(c, v):
             try:
                 return c(v) if v != self.nullval else self.get_null_val()
-            except Exception, e:
+            except Exception as e:
                 # if we could not convert an empty string, then self.nullval has been set to a marker
                 # because the user needs to import empty strings, except that the converters for some types
                 # will fail to convert an empty string, in this case the null value should be inserted
                 # see CASSANDRA-12794
                 if v == '':
                     return self.get_null_val()
 
                 if self.debug:
                     traceback.print_exc()
-                raise ParseError("Failed to parse %s : %s" % (val, e.message))
+                raise ParseError("Failed to parse %s : %s" % (v, e.message if hasattr(e, 'message') else str(e)))
 
         return [convert(conv, val) for conv, val in zip(converters, row)]
 
     def get_null_primary_key_message(self, idx):
         message = "Cannot insert null value for primary key column '%s'." % (self.columns[idx],)
         if self.nullval == '':
             message += " If you want to insert empty strings, consider using" \
@@ -2145,14 +2200,15 @@
 
         def serialize_row_multiple(row):
             pk_values = []
             for i in partition_key_indexes:
                 val = serialize(i, row[i])
                 length = len(val)
                 pk_values.append(struct.pack(">H%dsB" % length, length, val, 0))
+
             return b"".join(pk_values)
 
         if len(partition_key_indexes) == 1:
             return serialize_row_single
         return serialize_row_multiple
 
 
@@ -2200,15 +2256,15 @@
     @staticmethod
     def get_ring_pos(ring, val):
         idx = bisect_right(ring, val)
         return idx if idx < len(ring) else 0
 
     def filter_replicas(self, hosts):
         shuffled = tuple(sorted(hosts, key=lambda k: random.random()))
-        return filter(lambda r: r.is_up is not False and r.datacenter == self.local_dc, shuffled) if hosts else ()
+        return [r for r in shuffled if r.is_up is not False and r.datacenter == self.local_dc] if hosts else ()
 
 
 class FastTokenAwarePolicy(DCAwareRoundRobinPolicy):
     """
     Send to any replicas attached to the query, or else fall back to DCAwareRoundRobinPolicy. Perform
     exponential back-off if too many in flight requests to all replicas are already in progress.
     """
@@ -2233,15 +2289,15 @@
         if replicas:
             def replica_is_not_overloaded(r):
                 if r.address in connections:
                     conn = connections[r.address]
                     return conn.in_flight < min(conn.max_request_id, self.max_inflight_messages)
                 return True
 
-            for i in xrange(self.max_backoff_attempts):
+            for i in range(self.max_backoff_attempts):
                 for r in filter(replica_is_not_overloaded, replicas):
                     yield r
 
                 # the back-off starts at 10 ms (0.01) and it can go up to to 2^max_backoff_attempts,
                 # which is currently 12, so 2^12 = 4096 = ~40 seconds when dividing by 0.01
                 delay = randint(1, pow(2, i + 1)) * 0.01
                 printdebugmsg("All replicas busy, sleeping for %d second(s)..." % (delay,))
@@ -2265,15 +2321,15 @@
 
 class ImportProcess(ChildProcess):
 
     def __init__(self, params):
         ChildProcess.__init__(self, params=params, target=self.run)
 
         self.skip_columns = params['skip_columns']
-        self.valid_columns = [c.encode(self.encoding) for c in params['valid_columns']]
+        self.valid_columns = [c for c in params['valid_columns']]
         self.skip_column_indexes = [i for i, c in enumerate(self.columns) if c in self.skip_columns]
 
         options = params['options']
         self.nullval = options.copy['nullval']
         self.max_attempts = options.copy['maxattempts']
         self.min_batch_size = options.copy['minbatchsize']
         self.max_batch_size = options.copy['maxbatchsize']
@@ -2308,27 +2364,32 @@
                 connection_class=ConnectionWrapper)
 
             self._session = cluster.connect(self.ks)
             self._session.default_timeout = self.request_timeout
         return self._session
 
     def run(self):
+        if self.coverage:
+            self.start_coverage()
+
         try:
             pr = profile_on() if PROFILE_ON else None
 
             self.on_fork()
             self.inner_run(*self.make_params())
 
             if pr:
                 profile_off(pr, file_name='worker_profile_%d.txt' % (os.getpid(),))
 
-        except Exception, exc:
+        except Exception as exc:
             self.report_error(exc)
 
         finally:
+            if self.coverage:
+                self.stop_coverage()
             self.close()
 
     def close(self):
         if self._session:
             self._session.cluster.shutdown()
         ChildProcess.close(self)
 
@@ -2395,23 +2456,23 @@
                         future.add_callbacks(callback=result_callback, callback_args=(batch, chunk),
                                              errback=err_callback, errback_args=(batch, chunk, replicas))
                     # do not handle else case, if a statement could not be created, the exception is handled
                     # in self.wrap_make_statement and the error is reported, if a failure is injected that
                     # causes the statement to be None, then we should not report the error so that we can test
                     # the parent process handling missing batches from child processes
 
-            except Exception, exc:
+            except Exception as exc:
                 self.report_error(exc, chunk, chunk['rows'])
 
     def wrap_make_statement(self, inner_make_statement):
         def make_statement(query, conv, chunk, batch, replicas):
             try:
                 return inner_make_statement(query, conv, batch, replicas)
-            except Exception, exc:
-                print "Failed to make batch statement: {}".format(exc)
+            except Exception as exc:
+                print("Failed to make batch statement: {}".format(exc))
                 self.report_error(exc, chunk, batch['rows'])
                 return None
 
         def make_statement_with_failures(query, conv, chunk, batch, replicas):
             failed_batch, apply_failure = self.maybe_inject_failures(batch)
             if apply_failure:
                 return failed_batch
@@ -2424,17 +2485,17 @@
         statement.replicas = replicas
         statement.keyspace = self.ks
         for row in batch['rows']:
             where_clause = []
             set_clause = []
             for i, value in enumerate(row):
                 if i in conv.primary_key_indexes:
-                    where_clause.append("%s=%s" % (self.valid_columns[i], value))
+                    where_clause.append("{}={}".format(self.valid_columns[i], str(value)))
                 else:
-                    set_clause.append("%s=%s+%s" % (self.valid_columns[i], self.valid_columns[i], value))
+                    set_clause.append("{}={}+{}".format(self.valid_columns[i], self.valid_columns[i], str(value)))
 
             full_query_text = query % (','.join(set_clause), ' AND '.join(where_clause))
             statement.add(full_query_text)
         return statement
 
     def make_prepared_batch_statement(self, query, _, batch, replicas):
         """
@@ -2453,15 +2514,16 @@
         statement._statements_and_parameters = [(True, query.query_id, query.bind(r).values) for r in batch['rows']]
         return statement
 
     def make_non_prepared_batch_statement(self, query, _, batch, replicas):
         statement = BatchStatement(batch_type=BatchType.UNLOGGED, consistency_level=self.consistency_level)
         statement.replicas = replicas
         statement.keyspace = self.ks
-        statement._statements_and_parameters = [(False, query % (','.join(r),), ()) for r in batch['rows']]
+        field_sep = ','
+        statement._statements_and_parameters = [(False, query % (field_sep.join(r),), ()) for r in batch['rows']]
         return statement
 
     def convert_rows(self, conv, chunk):
         """
         Return converted rows and report any errors during conversion.
         """
         def filter_row_values(row):
@@ -2473,22 +2535,22 @@
             rows = list(csv.reader(chunk['rows'], **self.dialect_options))
 
         errors = defaultdict(list)
 
         def convert_row(r):
             try:
                 return conv.convert_row(r)
-            except Exception, err:
-                errors[err.message].append(r)
+            except Exception as err:
+                errors[err.message if hasattr(err, 'message') else str(err)].append(r)
                 return None
 
-        converted_rows = filter(None, [convert_row(r) for r in rows])
+        converted_rows = [_f for _f in [convert_row(r) for r in rows] if _f]
 
         if errors:
-            for msg, rows in errors.iteritems():
+            for msg, rows in errors.items():
                 self.report_error(ParseError(msg), chunk, rows)
         return converted_rows
 
     def maybe_inject_failures(self, batch):
         """
         Examine self.test_failures and see if the batch is a batch
         supposed to cause a failure (failing_batch), or to terminate the worker process
@@ -2545,35 +2607,36 @@
         get_ring_pos = tm.get_ring_pos
         make_batch = self.make_batch
 
         for row in chunk['rows']:
             try:
                 pk = get_row_partition_key_values(row)
                 rows_by_ring_pos[get_ring_pos(ring, pk_to_token_value(pk))].append(row)
-            except Exception, e:
-                errors[e.message].append(row)
+            except Exception as e:
+                errors[e.message if hasattr(e, 'message') else str(e)].append(row)
 
         if errors:
-            for msg, rows in errors.iteritems():
+            for msg, rows in errors.items():
                 self.report_error(ParseError(msg), chunk, rows)
 
         replicas = tm.replicas
         filter_replicas = tm.filter_replicas
         rows_by_replica = defaultdict(list)
-        for ring_pos, rows in rows_by_ring_pos.iteritems():
+        for ring_pos, rows in rows_by_ring_pos.items():
             if len(rows) > min_batch_size:
-                for i in xrange(0, len(rows), max_batch_size):
+                for i in range(0, len(rows), max_batch_size):
                     yield filter_replicas(replicas[ring_pos]), make_batch(chunk['id'], rows[i:i + max_batch_size])
             else:
                 # select only the first valid replica to guarantee more overlap or none at all
-                rows_by_replica[filter_replicas(replicas[ring_pos])[:1]].extend(rows)
+                # TODO: revisit tuple wrapper
+                rows_by_replica[tuple(filter_replicas(replicas[ring_pos])[:1])].extend(rows)
 
         # Now send the batches by replica
-        for replicas, rows in rows_by_replica.iteritems():
-            for i in xrange(0, len(rows), max_batch_size):
+        for replicas, rows in rows_by_replica.items():
+            for i in range(0, len(rows), max_batch_size):
                 yield replicas, make_batch(chunk['id'], rows[i:i + max_batch_size])
 
     def result_callback(self, _, batch, chunk):
         self.update_chunk(batch['rows'], chunk)
 
     def err_callback(self, response, batch, chunk, replicas):
         if isinstance(response, OperationTimedOut) and chunk['imported'] == chunk['num_rows_sent']:
@@ -2583,18 +2646,20 @@
         if not err_is_final:
             batch['attempts'] += 1
             statement = self.make_statement(self.query, self.conv, chunk, batch, replicas)
             future = self.session.execute_async(statement)
             future.add_callbacks(callback=self.result_callback, callback_args=(batch, chunk),
                                  errback=self.err_callback, errback_args=(batch, chunk, replicas))
 
+    # TODO: review why this is defined twice
     def report_error(self, err, chunk=None, rows=None, attempts=1, final=True):
         if self.debug and sys.exc_info()[1] == err:
             traceback.print_exc()
-        self.outmsg.send(ImportTaskError(err.__class__.__name__, err.message, rows, attempts, final))
+        err_msg = err.message if hasattr(err, 'message') else str(err)
+        self.outmsg.send(ImportTaskError(err.__class__.__name__, err_msg, rows, attempts, final))
         if final and chunk is not None:
             self.update_chunk(rows, chunk)
 
     def update_chunk(self, rows, chunk):
         chunk['imported'] += len(rows)
         if chunk['imported'] == chunk['num_rows_sent']:
             self.outmsg.send(ImportProcessResult(chunk['num_rows_sent']))
@@ -2669,8 +2734,8 @@
         if self.log_file:
             with open(self.log_file, "a") as f:
                 f.write(output + '\n')
 
     def get_total_records(self):
         self.update(time.time())
         self.log_message()
-        return self.total_records
+        return self.total_records
```

## cqlshlib/cql3handling.py

```diff
@@ -10,60 +10,62 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .cqlhandling import CqlParsingRuleSet, Hint
 from cassandra.metadata import maybe_escape_name
+from cqlshlib import helptopics
+from cqlshlib.cqlhandling import CqlParsingRuleSet, Hint
 
-
-simple_cql_types = set(('ascii', 'bigint', 'blob', 'boolean', 'counter', 'date', 'decimal', 'double', 'duration', 'float',
-                        'inet', 'int', 'smallint', 'text', 'time', 'timestamp', 'timeuuid', 'tinyint', 'uuid', 'varchar', 'varint'))
+simple_cql_types = {'ascii', 'bigint', 'blob', 'boolean', 'counter', 'date', 'decimal', 'double', 'duration', 'float',
+                    'inet', 'int', 'smallint', 'text', 'time', 'timestamp', 'timeuuid', 'tinyint', 'uuid', 'varchar',
+                    'varint'}
 simple_cql_types.difference_update(('set', 'map', 'list'))
 
-from . import helptopics
 cqldocs = helptopics.CQL3HelpTopics()
 
 
 class UnexpectedTableStructure(UserWarning):
 
     def __init__(self, msg):
         self.msg = msg
 
     def __str__(self):
         return 'Unexpected table structure; may not translate correctly to CQL. ' + self.msg
 
 
-SYSTEM_KEYSPACES = ('system', 'system_schema', 'system_traces', 'system_auth', 'system_distributed')
-NONALTERBALE_KEYSPACES = ('system', 'system_schema')
+SYSTEM_KEYSPACES = ('system', 'system_schema', 'system_traces', 'system_auth', 'system_distributed', 'system_views',
+                    'system_virtual_schema')
+NONALTERBALE_KEYSPACES = ('system', 'system_schema', 'system_views', 'system_virtual_schema')
 
 
 class Cql3ParsingRuleSet(CqlParsingRuleSet):
 
     columnfamily_layout_options = (
         ('bloom_filter_fp_chance', None),
         ('comment', None),
-        ('dclocal_read_repair_chance', 'local_read_repair_chance'),
         ('gc_grace_seconds', None),
         ('min_index_interval', None),
         ('max_index_interval', None),
-        ('read_repair_chance', None),
         ('default_time_to_live', None),
         ('speculative_retry', None),
+        ('additional_write_policy', None),
         ('memtable_flush_period_in_ms', None),
-        ('cdc', None)
+        ('cdc', None),
+        ('read_repair', None),
     )
 
     columnfamily_layout_map_options = (
         # (CQL3 option name, schema_columnfamilies column name (or None if same),
         #  list of known map keys)
         ('compaction', 'compaction_strategy_options',
-            ('class', 'max_threshold', 'tombstone_compaction_interval', 'tombstone_threshold', 'enabled', 'unchecked_tombstone_compaction', 'only_purge_repaired_tombstones')),
+            ('class', 'max_threshold', 'tombstone_compaction_interval', 'tombstone_threshold', 'enabled',
+             'unchecked_tombstone_compaction', 'only_purge_repaired_tombstones', 'provide_overlapping_tombstones')),
         ('compression', 'compression_parameters',
             ('sstable_compression', 'chunk_length_kb', 'crc_check_chance')),
         ('caching', None,
             ('rows_per_partition', 'keys')),
     )
 
     obsolete_cf_options = ()
@@ -76,14 +78,41 @@
         'QUORUM',
         'ALL',
         'LOCAL_QUORUM',
         'EACH_QUORUM',
         'SERIAL'
     )
 
+    size_tiered_compaction_strategy_options = (
+        'min_sstable_size',
+        'min_threshold',
+        'bucket_high',
+        'bucket_low'
+    )
+
+    leveled_compaction_strategy_options = (
+        'sstable_size_in_mb',
+        'fanout_size'
+    )
+
+    date_tiered_compaction_strategy_options = (
+        'base_time_seconds',
+        'max_sstable_age_days',
+        'min_threshold',
+        'max_window_size_seconds',
+        'timestamp_resolution'
+    )
+
+    time_window_compaction_strategy_options = (
+        'compaction_window_unit',
+        'compaction_window_size',
+        'min_threshold',
+        'timestamp_resolution'
+    )
+
     @classmethod
     def escape_value(cls, value):
         if value is None:
             return 'NULL'  # this totally won't work
         if isinstance(value, bool):
             value = str(value).lower()
         elif isinstance(value, float):
@@ -150,15 +179,15 @@
 <uuid> ::=          /[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}/ ;
 <blobLiteral> ::=    /0x[0-9a-f]+/ ;
 <wholenumber> ::=   /[0-9]+/ ;
 <identifier> ::=    /[a-z][a-z0-9_]*/ ;
 <colon> ::=         ":" ;
 <star> ::=          "*" ;
 <endtoken> ::=      ";" ;
-<op> ::=            /[-+=,().]/ ;
+<op> ::=            /[-+=%/,().]/ ;
 <cmp> ::=           /[<>!]=?/ ;
 <brackets> ::=      /[][{}]/ ;
 
 <integer> ::= "-"? <wholenumber> ;
 <boolean> ::= "true"
             | "false"
             ;
@@ -355,14 +384,19 @@
 completer_for('property', 'propeq')(prop_equals_completer)
 
 
 @completer_for('property', 'propname')
 def prop_name_completer(ctxt, cass):
     if working_on_keyspace(ctxt):
         return ks_prop_name_completer(ctxt, cass)
+    elif 'MATERIALIZED' == ctxt.get_binding('wat', '').upper():
+        props = cf_prop_name_completer(ctxt, cass)
+        props.remove('default_time_to_live')
+        props.remove('gc_grace_seconds')
+        return props
     else:
         return cf_prop_name_completer(ctxt, cass)
 
 
 @completer_for('propertyValue', 'propsimpleval')
 def prop_val_completer(ctxt, cass):
     if working_on_keyspace(ctxt):
@@ -411,142 +445,133 @@
     return ()
 
 
 def ks_prop_val_mapkey_completer(ctxt, cass):
     optname = ctxt.get_binding('propname')[-1]
     if optname != 'replication':
         return ()
-    keysseen = map(dequote_value, ctxt.get_binding('propmapkey', ()))
-    valsseen = map(dequote_value, ctxt.get_binding('propmapval', ()))
+    keysseen = list(map(dequote_value, ctxt.get_binding('propmapkey', ())))
+    valsseen = list(map(dequote_value, ctxt.get_binding('propmapval', ())))
     for k, v in zip(keysseen, valsseen):
         if k == 'class':
             repclass = v
             break
     else:
         return ["'class'"]
-    if repclass in CqlRuleSet.replication_factor_strategies:
-        opts = set(('replication_factor',))
+    if repclass == 'SimpleStrategy':
+        opts = {'replication_factor'}
     elif repclass == 'NetworkTopologyStrategy':
         return [Hint('<dc_name>')]
-    return map(escape_value, opts.difference(keysseen))
+    return list(map(escape_value, opts.difference(keysseen)))
 
 
 def ks_prop_val_mapval_completer(ctxt, cass):
     optname = ctxt.get_binding('propname')[-1]
     if optname != 'replication':
         return ()
     currentkey = dequote_value(ctxt.get_binding('propmapkey')[-1])
     if currentkey == 'class':
-        return map(escape_value, CqlRuleSet.replication_strategies)
+        return list(map(escape_value, CqlRuleSet.replication_strategies))
     return [Hint('<term>')]
 
 
 def ks_prop_val_mapender_completer(ctxt, cass):
     optname = ctxt.get_binding('propname')[-1]
     if optname != 'replication':
         return [',']
-    keysseen = map(dequote_value, ctxt.get_binding('propmapkey', ()))
-    valsseen = map(dequote_value, ctxt.get_binding('propmapval', ()))
+    keysseen = list(map(dequote_value, ctxt.get_binding('propmapkey', ())))
+    valsseen = list(map(dequote_value, ctxt.get_binding('propmapval', ())))
     for k, v in zip(keysseen, valsseen):
         if k == 'class':
             repclass = v
             break
     else:
         return [',']
-    if repclass in CqlRuleSet.replication_factor_strategies:
+    if repclass == 'SimpleStrategy':
         if 'replication_factor' not in keysseen:
             return [',']
     if repclass == 'NetworkTopologyStrategy' and len(keysseen) == 1:
         return [',']
     return ['}']
 
 
 def cf_prop_name_completer(ctxt, cass):
-    return [c[0] for c in (CqlRuleSet.columnfamily_layout_options +
-                           CqlRuleSet.columnfamily_layout_map_options)]
+    return [c[0] for c in (CqlRuleSet.columnfamily_layout_options
+                           + CqlRuleSet.columnfamily_layout_map_options)]
 
 
 def cf_prop_val_completer(ctxt, cass):
     exist_opts = ctxt.get_binding('propname')
     this_opt = exist_opts[-1]
     if this_opt == 'compression':
         return ["{'sstable_compression': '"]
     if this_opt == 'compaction':
         return ["{'class': '"]
     if this_opt == 'caching':
         return ["{'keys': '"]
     if any(this_opt == opt[0] for opt in CqlRuleSet.obsolete_cf_options):
         return ["'<obsolete_option>'"]
-    if this_opt in ('read_repair_chance', 'bloom_filter_fp_chance',
-                    'dclocal_read_repair_chance'):
+    if this_opt == 'bloom_filter_fp_chance':
         return [Hint('<float_between_0_and_1>')]
     if this_opt in ('min_compaction_threshold', 'max_compaction_threshold',
                     'gc_grace_seconds', 'min_index_interval', 'max_index_interval'):
         return [Hint('<integer>')]
     if this_opt in ('cdc'):
         return [Hint('<true|false>')]
+    if this_opt in ('read_repair'):
+        return [Hint('<\'none\'|\'blocking\'>')]
     return [Hint('<option_value>')]
 
 
 def cf_prop_val_mapkey_completer(ctxt, cass):
     optname = ctxt.get_binding('propname')[-1]
     for cql3option, _, subopts in CqlRuleSet.columnfamily_layout_map_options:
         if optname == cql3option:
             break
     else:
         return ()
-    keysseen = map(dequote_value, ctxt.get_binding('propmapkey', ()))
-    valsseen = map(dequote_value, ctxt.get_binding('propmapval', ()))
-    pairsseen = dict(zip(keysseen, valsseen))
+    keysseen = list(map(dequote_value, ctxt.get_binding('propmapkey', ())))
+    valsseen = list(map(dequote_value, ctxt.get_binding('propmapval', ())))
+    pairsseen = dict(list(zip(keysseen, valsseen)))
     if optname == 'compression':
-        return map(escape_value, set(subopts).difference(keysseen))
+        return list(map(escape_value, set(subopts).difference(keysseen)))
     if optname == 'caching':
-        return map(escape_value, set(subopts).difference(keysseen))
+        return list(map(escape_value, set(subopts).difference(keysseen)))
     if optname == 'compaction':
         opts = set(subopts)
         try:
             csc = pairsseen['class']
         except KeyError:
             return ["'class'"]
         csc = csc.split('.')[-1]
         if csc == 'SizeTieredCompactionStrategy':
-            opts.add('min_sstable_size')
-            opts.add('min_threshold')
-            opts.add('bucket_high')
-            opts.add('bucket_low')
+            opts = opts.union(set(CqlRuleSet.size_tiered_compaction_strategy_options))
         elif csc == 'LeveledCompactionStrategy':
-            opts.add('sstable_size_in_mb')
-            opts.add('fanout_size')
+            opts = opts.union(set(CqlRuleSet.leveled_compaction_strategy_options))
         elif csc == 'DateTieredCompactionStrategy':
-            opts.add('base_time_seconds')
-            opts.add('max_sstable_age_days')
-            opts.add('min_threshold')
-            opts.add('max_window_size_seconds')
-            opts.add('timestamp_resolution')
+            opts = opts.union(set(CqlRuleSet.date_tiered_compaction_strategy_options))
         elif csc == 'TimeWindowCompactionStrategy':
-            opts.add('compaction_window_unit')
-            opts.add('compaction_window_size')
-            opts.add('min_threshold')
-            opts.add('max_threshold')
-            opts.add('timestamp_resolution')
+            opts = opts.union(set(CqlRuleSet.time_window_compaction_strategy_options))
 
-        return map(escape_value, opts)
+        return list(map(escape_value, opts))
     return ()
 
 
 def cf_prop_val_mapval_completer(ctxt, cass):
     opt = ctxt.get_binding('propname')[-1]
     key = dequote_value(ctxt.get_binding('propmapkey')[-1])
     if opt == 'compaction':
         if key == 'class':
-            return map(escape_value, CqlRuleSet.available_compaction_classes)
+            return list(map(escape_value, CqlRuleSet.available_compaction_classes))
+        if key == 'provide_overlapping_tombstones':
+            return [Hint('<NONE|ROW|CELL>')]
         return [Hint('<option_value>')]
     elif opt == 'compression':
         if key == 'sstable_compression':
-            return map(escape_value, CqlRuleSet.available_compression_classes)
+            return list(map(escape_value, CqlRuleSet.available_compression_classes))
         return [Hint('<option_value>')]
     elif opt == 'caching':
         if key == 'rows_per_partition':
             return ["'ALL'", "'NONE'", Hint('#rows_per_partition')]
         elif key == 'keys':
             return ["'ALL'", "'NONE'"]
     return ()
@@ -564,27 +589,27 @@
 @completer_for('simpleStorageType', 'typename')
 def storagetype_completer(ctxt, cass):
     return simple_cql_types
 
 
 @completer_for('keyspaceName', 'ksname')
 def ks_name_completer(ctxt, cass):
-    return map(maybe_escape_name, cass.get_keyspace_names())
+    return list(map(maybe_escape_name, cass.get_keyspace_names()))
 
 
 @completer_for('nonSystemKeyspaceName', 'ksname')
 def non_system_ks_name_completer(ctxt, cass):
     ksnames = [n for n in cass.get_keyspace_names() if n not in SYSTEM_KEYSPACES]
-    return map(maybe_escape_name, ksnames)
+    return list(map(maybe_escape_name, ksnames))
 
 
 @completer_for('alterableKeyspaceName', 'ksname')
 def alterable_ks_name_completer(ctxt, cass):
     ksnames = [n for n in cass.get_keyspace_names() if n not in NONALTERBALE_KEYSPACES]
-    return map(maybe_escape_name, ksnames)
+    return list(map(maybe_escape_name, ksnames))
 
 
 def cf_ks_name_completer(ctxt, cass):
     return [maybe_escape_name(ks) + '.' for ks in cass.get_keyspace_names()]
 
 
 completer_for('columnFamilyName', 'ksname')(cf_ks_name_completer)
@@ -609,29 +634,29 @@
         ks = dequote_name(ks)
     try:
         cfnames = cass.get_columnfamily_names(ks)
     except Exception:
         if ks is None:
             return ()
         raise
-    return map(maybe_escape_name, cfnames)
+    return list(map(maybe_escape_name, cfnames))
 
 
 @completer_for('materializedViewName', 'mvname')
 def mv_name_completer(ctxt, cass):
     ks = ctxt.get_binding('ksname', None)
     if ks is not None:
         ks = dequote_name(ks)
     try:
         mvnames = cass.get_materialized_view_names(ks)
     except Exception:
         if ks is None:
             return ()
         raise
-    return map(maybe_escape_name, mvnames)
+    return list(map(maybe_escape_name, mvnames))
 
 
 completer_for('userTypeName', 'ksname')(cf_ks_name_completer)
 
 completer_for('userTypeName', 'dot')(cf_ks_dot_completer)
 
 
@@ -641,15 +666,15 @@
         ks = dequote_name(ks)
     try:
         utnames = cass.get_usertype_names(ks)
     except Exception:
         if ks is None:
             return ()
         raise
-    return map(maybe_escape_name, utnames)
+    return list(map(maybe_escape_name, utnames))
 
 
 completer_for('userTypeName', 'utname')(ut_name_completer)
 completer_for('userType', 'utname')(ut_name_completer)
 
 
 @completer_for('unreservedKeyword', 'nocomplete')
@@ -673,15 +698,15 @@
     if ks is not None:
         ks = dequote_name(ks)
     ut = dequote_name(ctxt.get_binding('utname'))
     return cass.get_usertype_layout(ks, ut)
 
 
 def working_on_keyspace(ctxt):
-    wat = ctxt.get_binding('wat').upper()
+    wat = ctxt.get_binding('wat', '').upper()
     if wat in ('KEYSPACE', 'SCHEMA'):
         return True
     return False
 
 
 syntax_rules += r'''
 <useStatement> ::= "USE" <keyspaceName>
@@ -704,77 +729,83 @@
              | [rel_lhs]=<cident> "IN" "(" <term> ( "," <term> )* ")"
              ;
 <selectClause> ::= "DISTINCT"? <selector> ("AS" <cident>)? ("," <selector> ("AS" <cident>)?)*
                  | "*"
                  ;
 <udtSubfieldSelection> ::= <identifier> "." <identifier>
                          ;
-<selector> ::= [colname]=<cident>
+<selector> ::= [colname]=<cident> ( "[" ( <term> ( ".." <term> "]" )? | <term> ".." ) )?
              | <udtSubfieldSelection>
              | "WRITETIME" "(" [colname]=<cident> ")"
              | "TTL" "(" [colname]=<cident> ")"
              | "COUNT" "(" star=( "*" | "1" ) ")"
              | "CAST" "(" <selector> "AS" <storageType> ")"
              | <functionName> <selectionFunctionArguments>
              | <term>
              ;
 <selectionFunctionArguments> ::= "(" ( <selector> ( "," <selector> )* )? ")"
                           ;
 <orderByClause> ::= [ordercol]=<cident> ( "ASC" | "DESC" )?
                   ;
 <groupByClause> ::= [groupcol]=<cident>
+                  | <functionName><groupByFunctionArguments>
                   ;
+<groupByFunctionArguments> ::= "(" ( <groupByFunctionArgument> ( "," <groupByFunctionArgument> )* )? ")"
+                             ;
+<groupByFunctionArgument> ::= [groupcol]=<cident>
+                            | <term>
+                            ;
 '''
 
 
 def udf_name_completer(ctxt, cass):
     ks = ctxt.get_binding('ksname', None)
     if ks is not None:
         ks = dequote_name(ks)
     try:
         udfnames = cass.get_userfunction_names(ks)
     except Exception:
         if ks is None:
             return ()
         raise
-    return map(maybe_escape_name, udfnames)
+    return list(map(maybe_escape_name, udfnames))
 
 
 def uda_name_completer(ctxt, cass):
     ks = ctxt.get_binding('ksname', None)
     if ks is not None:
         ks = dequote_name(ks)
     try:
         udanames = cass.get_useraggregate_names(ks)
     except Exception:
         if ks is None:
             return ()
         raise
-    return map(maybe_escape_name, udanames)
+    return list(map(maybe_escape_name, udanames))
 
 
 def udf_uda_name_completer(ctxt, cass):
     ks = ctxt.get_binding('ksname', None)
     if ks is not None:
         ks = dequote_name(ks)
     try:
         functionnames = cass.get_userfunction_names(ks) + cass.get_useraggregate_names(ks)
     except Exception:
         if ks is None:
             return ()
         raise
-    return map(maybe_escape_name, functionnames)
+    return list(map(maybe_escape_name, functionnames))
 
 
 def ref_udf_name_completer(ctxt, cass):
     try:
         udanames = cass.get_userfunction_names(None)
     except Exception:
         return ()
-    return map(maybe_escape_name, udanames)
+    return list(map(maybe_escape_name, udanames))
 
 
 completer_for('functionAggregateName', 'ksname')(cf_ks_name_completer)
 completer_for('functionAggregateName', 'dot')(cf_ks_dot_completer)
 completer_for('functionAggregateName', 'functionname')(udf_uda_name_completer)
 completer_for('anyFunctionName', 'ksname')(cf_ks_name_completer)
 completer_for('anyFunctionName', 'dot')(cf_ks_dot_completer)
@@ -824,28 +855,28 @@
     return [key.name for key in layout.partition_key]
 
 
 @completer_for('relation', 'rel_lhs')
 def select_relation_lhs_completer(ctxt, cass):
     layout = get_table_meta(ctxt, cass)
     filterable = set()
-    already_filtered_on = map(dequote_name, ctxt.get_binding('rel_lhs', ()))
+    already_filtered_on = list(map(dequote_name, ctxt.get_binding('rel_lhs', ())))
     for num in range(0, len(layout.partition_key)):
         if num == 0 or layout.partition_key[num - 1].name in already_filtered_on:
             filterable.add(layout.partition_key[num].name)
         else:
             break
     for num in range(0, len(layout.clustering_key)):
         if num == 0 or layout.clustering_key[num - 1].name in already_filtered_on:
             filterable.add(layout.clustering_key[num].name)
         else:
             break
-    for idx in layout.indexes.itervalues():
+    for idx in layout.indexes.values():
         filterable.add(idx.index_options["target"])
-    return map(maybe_escape_name, filterable)
+    return list(map(maybe_escape_name, filterable))
 
 
 explain_completion('selector', 'colname')
 
 syntax_rules += r'''
 <insertStatement> ::= "INSERT" "INTO" cf=<columnFamilyName>
                       ( ( "(" [colname]=<cident> ( "," [colname]=<cident> )* ")"
@@ -860,36 +891,36 @@
                 ;
 '''
 
 
 def regular_column_names(table_meta):
     if not table_meta or not table_meta.columns:
         return []
-    regular_columns = list(set(table_meta.columns.keys()) -
-                           set([key.name for key in table_meta.partition_key]) -
-                           set([key.name for key in table_meta.clustering_key]))
+    regular_columns = list(set(table_meta.columns.keys())
+                           - set([key.name for key in table_meta.partition_key])
+                           - set([key.name for key in table_meta.clustering_key]))
     return regular_columns
 
 
 @completer_for('insertStatement', 'colname')
 def insert_colname_completer(ctxt, cass):
     layout = get_table_meta(ctxt, cass)
     colnames = set(map(dequote_name, ctxt.get_binding('colname', ())))
     keycols = layout.primary_key
     for k in keycols:
         if k.name not in colnames:
             return [maybe_escape_name(k.name)]
     normalcols = set(regular_column_names(layout)) - colnames
-    return map(maybe_escape_name, normalcols)
+    return list(map(maybe_escape_name, normalcols))
 
 
 @completer_for('insertStatement', 'newval')
 def insert_newval_completer(ctxt, cass):
     layout = get_table_meta(ctxt, cass)
-    insertcols = map(dequote_name, ctxt.get_binding('colname'))
+    insertcols = list(map(dequote_name, ctxt.get_binding('colname')))
     valuesdone = ctxt.get_binding('newval', ())
     if len(valuesdone) >= len(insertcols):
         return []
     curcol = insertcols[len(valuesdone)]
     coltype = layout.columns[curcol].cql_type
     if coltype in ('map', 'set'):
         return ['{']
@@ -932,15 +963,15 @@
                                 ( counterop=( "+" | "-" ) inc=<wholenumber>
                                 | listadder="+" listcol=<cident> )? )
                     | ( indexbracket="[" <term> "]" "=" <term> )
                     | ( udt_field_dot="." udt_field=<identifier> "=" <term> ))
                ;
 <conditions> ::=  <condition> ( "AND" <condition> )*
                ;
-<condition_op_and_rhs> ::= (("=" | "<" | ">" | "<=" | ">=" | "!=") <term>)
+<condition_op_and_rhs> ::= (("=" | "<" | ">" | "<=" | ">=" | "!=" | "CONTAINS" ( "KEY" )? ) <term>)
                            | ("IN" "(" <term> ( "," <term> )* ")" )
                          ;
 <condition> ::= conditioncol=<cident>
                     ( (( indexbracket="[" <term> "]" )
                       |( udt_field_dot="." udt_field=<identifier> )) )?
                     <condition_op_and_rhs>
               ;
@@ -954,15 +985,15 @@
         opts.discard(opt.split()[0])
     return opts
 
 
 @completer_for('assignment', 'updatecol')
 def update_col_completer(ctxt, cass):
     layout = get_table_meta(ctxt, cass)
-    return map(maybe_escape_name, regular_column_names(layout))
+    return list(map(maybe_escape_name, regular_column_names(layout)))
 
 
 @completer_for('assignment', 'update_rhs')
 def update_countername_completer(ctxt, cass):
     layout = get_table_meta(ctxt, cass)
     curcol = dequote_name(ctxt.get_binding('updatecol', ''))
     coltype = layout.columns[curcol].cql_type
@@ -1096,15 +1127,15 @@
         opts.discard(opt.split()[0])
     return opts
 
 
 @completer_for('deleteSelector', 'delcol')
 def delete_delcol_completer(ctxt, cass):
     layout = get_table_meta(ctxt, cass)
-    return map(maybe_escape_name, regular_column_names(layout))
+    return list(map(maybe_escape_name, regular_column_names(layout)))
 
 
 syntax_rules += r'''
 <batchStatement> ::= "BEGIN" ( "UNLOGGED" | "COUNTER" )? "BATCH"
                         ( "USING" [batchopt]=<usingOption>
                                   ( "AND" [batchopt]=<usingOption> )* )?
                         [batchstmt]=<batchStatementMember> ";"?
@@ -1177,15 +1208,15 @@
                                ( "," [ptkey]=<cident> )* ")"
           ;
 '''
 
 
 @completer_for('cfamOrdering', 'ordercol')
 def create_cf_clustering_order_colname_completer(ctxt, cass):
-    colnames = map(dequote_name, ctxt.get_binding('newcolname', ()))
+    colnames = list(map(dequote_name, ctxt.get_binding('newcolname', ())))
     # Definitely some of these aren't valid for ordering, but I'm not sure
     # precisely which are. This is good enough for now
     return colnames
 
 
 @completer_for('createColumnFamilyStatement', 'wat')
 def create_cf_wat_completer(ctxt, cass):
@@ -1207,27 +1238,27 @@
     return []
 
 
 @completer_for('pkDef', 'ptkey')
 def create_cf_pkdef_declaration_completer(ctxt, cass):
     cols_declared = ctxt.get_binding('newcolname')
     pieces_already = ctxt.get_binding('ptkey', ())
-    pieces_already = map(dequote_name, pieces_already)
+    pieces_already = list(map(dequote_name, pieces_already))
     while cols_declared[0] in pieces_already:
         cols_declared = cols_declared[1:]
         if len(cols_declared) < 2:
             return ()
     return [maybe_escape_name(cols_declared[0])]
 
 
 @completer_for('compositeKeyCfSpec', 'pkey')
 def create_cf_composite_key_declaration_completer(ctxt, cass):
     cols_declared = ctxt.get_binding('newcolname')
     pieces_already = ctxt.get_binding('ptkey', ()) + ctxt.get_binding('pkey', ())
-    pieces_already = map(dequote_name, pieces_already)
+    pieces_already = list(map(dequote_name, pieces_already))
     while cols_declared[0] in pieces_already:
         cols_declared = cols_declared[1:]
         if len(cols_declared) < 2:
             return ()
     return [maybe_escape_name(cols_declared[0])]
 
 
@@ -1261,17 +1292,24 @@
                                    col=<cident> |
                                    "keys(" col=<cident> ")" |
                                    "full(" col=<cident> ")"
                                ) ")"
                                ( "USING" <stringLiteral> ( "WITH" "OPTIONS" "=" <mapLiteral> )? )?
                          ;
 
-<createMaterializedViewStatement> ::= "CREATE" "MATERIALIZED" "VIEW" ("IF" "NOT" "EXISTS")? <materializedViewName>?
-                                      "AS" <selectStatement>
-                                      "PRIMARY" "KEY" <pkDef>
+
+<colList> ::= "(" <cident> ( "," <cident> )* ")"
+          ;
+
+<createMaterializedViewStatement> ::= "CREATE" wat="MATERIALIZED" "VIEW" ("IF" "NOT" "EXISTS")? viewname=<materializedViewName>?
+                                      "AS" "SELECT" <selectClause>
+                                      "FROM" cf=<columnFamilyName>
+                                      "WHERE" <cident> "IS" "NOT" "NULL" ( "AND" <cident> "IS" "NOT" "NULL")*
+                                      "PRIMARY" "KEY" (<colList> | ( "(" <colList> ( "," <cident> )* ")" ))
+                                      ( "WITH" <cfamProperty> ( "AND" <cfamProperty> )* )?
                                     ;
 
 <createUserTypeStatement> ::= "CREATE" "TYPE" ( ks=<nonSystemKeyspaceName> dot="." )? typename=<cfOrKsName> "(" newcol=<cident> <storageType>
                                 ( "," [newcolname]=<cident> <storageType> )*
                             ")"
                          ;
 
@@ -1297,25 +1335,26 @@
                             ( "FINALFUNC" <refUserFunctionName> )?
                             ( "INITCOND" <term> )?
                          ;
 
 '''
 
 explain_completion('createIndexStatement', 'indexname', '<new_index_name>')
+explain_completion('createMaterializedViewStatement', 'viewname', '<new_view_name>')
 explain_completion('createUserTypeStatement', 'typename', '<new_type_name>')
 explain_completion('createUserTypeStatement', 'newcol', '<new_field_name>')
 
 
 @completer_for('createIndexStatement', 'col')
 def create_index_col_completer(ctxt, cass):
     """ Return the columns for which an index doesn't exist yet. """
     layout = get_table_meta(ctxt, cass)
-    idx_targets = [idx.index_options["target"] for idx in layout.indexes.itervalues()]
-    colnames = [cd.name for cd in layout.columns.values() if cd.name not in idx_targets]
-    return map(maybe_escape_name, colnames)
+    idx_targets = [idx.index_options["target"] for idx in layout.indexes.values()]
+    colnames = [cd.name for cd in list(layout.columns.values()) if cd.name not in idx_targets]
+    return list(map(maybe_escape_name, colnames))
 
 
 syntax_rules += r'''
 <dropKeyspaceStatement> ::= "DROP" "KEYSPACE" ("IF" "EXISTS")? ksname=<nonSystemKeyspaceName>
                           ;
 
 <dropColumnFamilyStatement> ::= "DROP" ( "COLUMNFAMILY" | "TABLE" ) ("IF" "EXISTS")? cf=<columnFamilyName>
@@ -1365,72 +1404,72 @@
         ks = dequote_name(ks)
     try:
         idxnames = cass.get_index_names(ks)
     except Exception:
         if ks is None:
             return ()
         raise
-    return map(maybe_escape_name, idxnames)
+    return list(map(maybe_escape_name, idxnames))
 
 
 syntax_rules += r'''
-<alterTableStatement> ::= "ALTER" wat=( "COLUMNFAMILY" | "TABLE" ) cf=<columnFamilyName>
+<alterTableStatement> ::= "ALTER" wat=( "COLUMNFAMILY" | "TABLE" ) ("IF" "EXISTS")? cf=<columnFamilyName>
                                <alterInstructions>
                         ;
-<alterInstructions> ::= "ADD" newcol=<cident> <storageType> ("static")?
-                      | "DROP" existcol=<cident>
+<alterInstructions> ::= "ADD" ("IF" "NOT" "EXISTS")? newcol=<cident> <storageType> ("static")?
+                      | "DROP" ("IF" "EXISTS")? existcol=<cident>
                       | "WITH" <cfamProperty> ( "AND" <cfamProperty> )*
-                      | "RENAME" existcol=<cident> "TO" newcol=<cident>
+                      | "RENAME" ("IF" "EXISTS")? existcol=<cident> "TO" newcol=<cident>
                          ( "AND" existcol=<cident> "TO" newcol=<cident> )*
                       ;
 
-<alterUserTypeStatement> ::= "ALTER" "TYPE" ut=<userTypeName>
+<alterUserTypeStatement> ::= "ALTER" "TYPE" ("IF" "EXISTS")? ut=<userTypeName>
                                <alterTypeInstructions>
                              ;
-<alterTypeInstructions> ::= "ADD" newcol=<cident> <storageType>
-                           | "RENAME" existcol=<cident> "TO" newcol=<cident>
+<alterTypeInstructions> ::= "ADD" ("IF" "NOT" "EXISTS")? newcol=<cident> <storageType>
+                           | "RENAME" ("IF" "EXISTS")? existcol=<cident> "TO" newcol=<cident>
                               ( "AND" existcol=<cident> "TO" newcol=<cident> )*
                            ;
 '''
 
 
 @completer_for('alterInstructions', 'existcol')
 def alter_table_col_completer(ctxt, cass):
     layout = get_table_meta(ctxt, cass)
     cols = [str(md) for md in layout.columns]
-    return map(maybe_escape_name, cols)
+    return list(map(maybe_escape_name, cols))
 
 
 @completer_for('alterTypeInstructions', 'existcol')
 def alter_type_field_completer(ctxt, cass):
     layout = get_ut_layout(ctxt, cass)
-    fields = [tuple[0] for tuple in layout]
-    return map(maybe_escape_name, fields)
+    fields = [atuple[0] for atuple in layout]
+    return list(map(maybe_escape_name, fields))
 
 
 explain_completion('alterInstructions', 'newcol', '<new_column_name>')
 explain_completion('alterTypeInstructions', 'newcol', '<new_field_name>')
 
 
 syntax_rules += r'''
-<alterKeyspaceStatement> ::= "ALTER" wat=( "KEYSPACE" | "SCHEMA" ) ks=<alterableKeyspaceName>
+<alterKeyspaceStatement> ::= "ALTER" wat=( "KEYSPACE" | "SCHEMA" ) ("IF" "EXISTS")? ks=<alterableKeyspaceName>
                                  "WITH" <property> ( "AND" <property> )*
                            ;
 '''
 
 syntax_rules += r'''
 <username> ::= name=( <identifier> | <stringLiteral> )
              ;
 
 <createUserStatement> ::= "CREATE" "USER" ( "IF" "NOT" "EXISTS" )? <username>
-                              ( "WITH" "PASSWORD" <stringLiteral> )?
+                              ( "WITH" ("HASHED")? "PASSWORD" <stringLiteral> )?
                               ( "SUPERUSER" | "NOSUPERUSER" )?
                         ;
 
-<alterUserStatement> ::= "ALTER" "USER" <username>
+<alterUserStatement> ::= "ALTER" "USER" ("IF" "EXISTS")? <username>
                               ( "WITH" "PASSWORD" <stringLiteral> )?
                               ( "SUPERUSER" | "NOSUPERUSER" )?
                        ;
 
 <dropUserStatement> ::= "DROP" "USER" ( "IF" "EXISTS" )? <username>
                       ;
 
@@ -1444,22 +1483,24 @@
              | <unreservedKeyword>
              ;
 
 <createRoleStatement> ::= "CREATE" "ROLE" <rolename>
                               ( "WITH" <roleProperty> ("AND" <roleProperty>)*)?
                         ;
 
-<alterRoleStatement> ::= "ALTER" "ROLE" <rolename>
+<alterRoleStatement> ::= "ALTER" "ROLE" ("IF" "EXISTS")? <rolename>
                               ( "WITH" <roleProperty> ("AND" <roleProperty>)*)?
                        ;
 
-<roleProperty> ::= "PASSWORD" "=" <stringLiteral>
+<roleProperty> ::= (("HASHED")? "PASSWORD") "=" <stringLiteral>
                  | "OPTIONS" "=" <mapLiteral>
                  | "SUPERUSER" "=" <boolean>
                  | "LOGIN" "=" <boolean>
+                 | "ACCESS" "TO" "DATACENTERS" <setLiteral>
+                 | "ACCESS" "TO" "ALL" "DATACENTERS"
                  ;
 
 <dropRoleStatement> ::= "DROP" "ROLE" <rolename>
                       ;
 
 <grantRoleStatement> ::= "GRANT" <rolename> "TO" <rolename>
                        ;
@@ -1489,26 +1530,27 @@
                | "DROP"
                | "SELECT"
                | "MODIFY"
                | "DESCRIBE"
                | "EXECUTE"
                ;
 
-<permissionExpr> ::= ( <permission> "PERMISSION"? )
+<permissionExpr> ::= ( [newpermission]=<permission> "PERMISSION"? ( "," [newpermission]=<permission> "PERMISSION"? )* )
                    | ( "ALL" "PERMISSIONS"? )
                    ;
 
 <resource> ::= <dataResource>
              | <roleResource>
              | <functionResource>
              | <jmxResource>
              ;
 
 <dataResource> ::= ( "ALL" "KEYSPACES" )
                  | ( "KEYSPACE" <keyspaceName> )
+                 | ( "ALL" "TABLES" "IN" "KEYSPACE" <keyspaceName> )
                  | ( "TABLE"? <columnFamilyName> )
                  ;
 
 <roleResource> ::= ("ALL" "ROLES")
                  | ("ROLE" <rolename>)
                  ;
 
@@ -1523,27 +1565,37 @@
 <jmxResource> ::= ( "ALL" "MBEANS")
                 | ( ( "MBEAN" | "MBEANS" ) <stringLiteral> )
                 ;
 
 '''
 
 
+@completer_for('permissionExpr', 'newpermission')
+def permission_completer(ctxt, _):
+    new_permissions = set([permission.upper() for permission in ctxt.get_binding('newpermission')])
+    all_permissions = set([permission.arg for permission in ctxt.ruleset['permission'].arg])
+    suggestions = all_permissions - new_permissions
+    if len(suggestions) == 0:
+        return [Hint('No more permissions here.')]
+    return suggestions
+
+
 @completer_for('username', 'name')
 def username_name_completer(ctxt, cass):
     def maybe_quote(name):
         if CqlRuleSet.is_valid_cql3_name(name):
             return name
         return "'%s'" % name
 
     # disable completion for CREATE USER.
     if ctxt.matched[0][1].upper() == 'CREATE':
         return [Hint('<username>')]
 
     session = cass.session
-    return [maybe_quote(row.values()[0].replace("'", "''")) for row in session.execute("LIST USERS")]
+    return [maybe_quote(list(row.values())[0].replace("'", "''")) for row in session.execute("LIST USERS")]
 
 
 @completer_for('rolename', 'role')
 def rolename_completer(ctxt, cass):
     def maybe_quote(name):
         if CqlRuleSet.is_valid_cql3_name(name):
             return name
@@ -1574,13 +1626,13 @@
         ks = dequote_name(ks)
     return cass.get_trigger_names(ks)
 
 
 @completer_for('dropTriggerStatement', 'triggername')
 def drop_trigger_completer(ctxt, cass):
     names = get_trigger_names(ctxt, cass)
-    return map(maybe_escape_name, names)
+    return list(map(maybe_escape_name, names))
 
 
 # END SYNTAX/COMPLETION RULE DEFINITIONS
 
 CqlRuleSet.append_rules(syntax_rules)
```

## cqlshlib/cqlhandling.py

```diff
@@ -14,71 +14,78 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # code for dealing with CQL's syntax, rules, interpretation
 # i.e., stuff that's not necessarily cqlsh-specific
 
 import traceback
-from cassandra.metadata import cql_keywords_reserved
-from . import pylexotron, util
+
+import cassandra
+from cqlshlib import pylexotron, util
 
 Hint = pylexotron.Hint
 
+cql_keywords_reserved = {'add', 'allow', 'alter', 'and', 'apply', 'asc', 'authorize', 'batch', 'begin', 'by',
+                         'columnfamily', 'create', 'delete', 'desc', 'describe', 'drop', 'entries', 'execute', 'from',
+                         'full', 'grant', 'if', 'in', 'index', 'infinity', 'insert', 'into', 'is', 'keyspace', 'limit',
+                         'materialized', 'modify', 'nan', 'norecursive', 'not', 'null', 'of', 'on', 'or', 'order',
+                         'primary', 'rename', 'revoke', 'schema', 'select', 'set', 'table', 'to', 'token', 'truncate',
+                         'unlogged', 'update', 'use', 'using', 'view', 'where', 'with'}
+"""
+Set of reserved keywords in CQL.
+
+Derived from .../cassandra/src/java/org/apache/cassandra/cql3/ReservedKeywords.java
+"""
+
 
 class CqlParsingRuleSet(pylexotron.ParsingRuleSet):
 
     available_compression_classes = (
         'DeflateCompressor',
         'SnappyCompressor',
         'LZ4Compressor',
+        'ZstdCompressor',
     )
 
     available_compaction_classes = (
         'LeveledCompactionStrategy',
         'SizeTieredCompactionStrategy',
         'DateTieredCompactionStrategy',
         'TimeWindowCompactionStrategy'
     )
 
     replication_strategies = (
         'SimpleStrategy',
-        'OldNetworkTopologyStrategy',
         'NetworkTopologyStrategy'
     )
 
-    replication_factor_strategies = (
-        'SimpleStrategy',
-        'org.apache.cassandra.locator.SimpleStrategy',
-        'OldNetworkTopologyStrategy',
-        'org.apache.cassandra.locator.OldNetworkTopologyStrategy'
-    )
-
     def __init__(self, *args, **kwargs):
-        pylexotron.ParsingRuleSet.__init__(self, *args, **kwargs)
+        pylexotron.ParsingRuleSet.__init__(self)
 
         # note: commands_end_with_newline may be extended by callers.
         self.commands_end_with_newline = set()
-        self.set_reserved_keywords(cql_keywords_reserved)
+        self.set_reserved_keywords()
 
-    def set_reserved_keywords(self, keywords):
+    def set_reserved_keywords(self):
         """
-        We cannot let resreved cql keywords be simple 'identifier' since this caused
+        We cannot let reserved cql keywords be simple 'identifier' since this caused
         problems with completion, see CASSANDRA-10415
         """
-        syntax = '<reserved_identifier> ::= /(' + '|'.join(r'\b{}\b'.format(k) for k in keywords) + ')/ ;'
+        cassandra.metadata.cql_keywords_reserved = cql_keywords_reserved
+        syntax = '<reserved_identifier> ::= /(' + '|'.join(r'\b{}\b'.format(k) for k in cql_keywords_reserved) + ')/ ;'
         self.append_rules(syntax)
 
     def completer_for(self, rulename, symname):
         def registrator(f):
             def completerwrapper(ctxt):
                 cass = ctxt.get_binding('cassandra_conn', None)
                 if cass is None:
                     return ()
                 return f(ctxt, cass)
-            completerwrapper.func_name = 'completerwrapper_on_' + f.func_name
+            completerwrapper.__name__ = 'completerwrapper_on_' + f.__name__
             self.register_completer(completerwrapper, rulename, symname)
             return completerwrapper
         return registrator
 
     def explain_completion(self, rulename, symname, explanation=None):
         if explanation is None:
             explanation = '<%s>' % (symname,)
@@ -99,26 +106,14 @@
             if t[0] == 'endline':
                 if term_on_nl:
                     t = ('endtoken',) + t[1:]
                 else:
                     # don't put any 'endline' tokens in output
                     continue
 
-            # Convert all unicode tokens to ascii, where possible.  This
-            # helps avoid problems with performing unicode-incompatible
-            # operations on tokens (like .lower()).  See CASSANDRA-9083
-            # for one example of this.
-            str_token = t[1]
-            if isinstance(str_token, unicode):
-                try:
-                    str_token = str_token.encode('ascii')
-                    t = (t[0], str_token) + t[2:]
-                except UnicodeEncodeError:
-                    pass
-
             curstmt.append(t)
             if t[0] == 'endtoken':
                 term_on_nl = False
                 output.extend(curstmt)
                 curstmt = []
             else:
                 if len(curstmt) == 1:
@@ -152,18 +147,18 @@
             if len(stmt) > 2:
                 if stmt[-3][1].upper() == 'APPLY':
                     in_batch = False
                 elif stmt[0][1].upper() == 'BEGIN':
                     in_batch = True
         return output, in_batch or in_pg_string
 
-    def cql_complete_single(self, text, partial, init_bindings={}, ignore_case=True,
+    def cql_complete_single(self, text, partial, init_bindings=None, ignore_case=True,
                             startsymbol='Start'):
         tokens = (self.cql_split_statements(text)[0] or [[]])[-1]
-        bindings = init_bindings.copy()
+        bindings = {} if init_bindings is None else init_bindings.copy()
 
         # handle some different completion scenarios- in particular, completing
         # inside a string literal
         prefix = None
         dequoter = util.identity
         lasttype = None
         if tokens:
@@ -200,26 +195,26 @@
 
         # find matches with the partial word under completion
         if ignore_case:
             partial = partial.lower()
             f = lambda s: s and dequoter(s).lower().startswith(partial)
         else:
             f = lambda s: s and dequoter(s).startswith(partial)
-        candidates = filter(f, strcompletes)
+        candidates = list(filter(f, strcompletes))
 
         if prefix is not None:
             # dequote, re-escape, strip quotes: gets us the right quoted text
             # for completion. the opening quote is already there on the command
             # line and not part of the word under completion, and readline
             # fills in the closing quote for us.
             candidates = [requoter(dequoter(c))[len(prefix) + 1:-1] for c in candidates]
 
             # the above process can result in an empty string; this doesn't help for
             # completions
-            candidates = filter(None, candidates)
+            candidates = [_f for _f in candidates if _f]
 
         # prefix a space when desirable for pleasant cql formatting
         if tokens:
             newcandidates = []
             for c in candidates:
                 if self.want_space_between(tokens[-1], c) \
                         and prefix is None \
@@ -253,68 +248,68 @@
         return False
 
     def cql_complete(self, text, partial, cassandra_conn=None, ignore_case=True, debug=False,
                      startsymbol='Start'):
         init_bindings = {'cassandra_conn': cassandra_conn}
         if debug:
             init_bindings['*DEBUG*'] = True
-            print "cql_complete(%r, partial=%r)" % (text, partial)
+            print("cql_complete(%r, partial=%r)" % (text, partial))
 
         completions, hints = self.cql_complete_single(text, partial, init_bindings,
                                                       startsymbol=startsymbol)
 
         if hints:
             hints = [h.text for h in hints]
             hints.append('')
 
         if len(completions) == 1 and len(hints) == 0:
             c = completions[0]
             if debug:
-                print "** Got one completion: %r. Checking for further matches...\n" % (c,)
+                print("** Got one completion: %r. Checking for further matches...\n" % (c,))
             if not c.isspace():
                 new_c = self.cql_complete_multiple(text, c, init_bindings, startsymbol=startsymbol)
                 completions = [new_c]
             if debug:
-                print "** New list of completions: %r" % (completions,)
+                print("** New list of completions: %r" % (completions,))
 
         return hints + completions
 
     def cql_complete_multiple(self, text, first, init_bindings, startsymbol='Start'):
         debug = init_bindings.get('*DEBUG*', False)
         try:
             completions, hints = self.cql_complete_single(text + first, '', init_bindings,
                                                           startsymbol=startsymbol)
         except Exception:
             if debug:
-                print "** completion expansion had a problem:"
+                print("** completion expansion had a problem:")
                 traceback.print_exc()
             return first
         if hints:
             if not first[-1].isspace():
                 first += ' '
             if debug:
-                print "** completion expansion found hints: %r" % (hints,)
+                print("** completion expansion found hints: %r" % (hints,))
             return first
         if len(completions) == 1 and completions[0] != '':
             if debug:
-                print "** Got another completion: %r." % (completions[0],)
+                print("** Got another completion: %r." % (completions[0],))
             if completions[0][0] in (',', ')', ':') and first[-1] == ' ':
                 first = first[:-1]
             first += completions[0]
         else:
             common_prefix = util.find_common_prefix(completions)
             if common_prefix == '':
                 return first
             if common_prefix[0] in (',', ')', ':') and first[-1] == ' ':
                 first = first[:-1]
             if debug:
-                print "** Got a partial completion: %r." % (common_prefix,)
+                print("** Got a partial completion: %r." % (common_prefix,))
             return first + common_prefix
         if debug:
-            print "** New total completion: %r. Checking for further matches...\n" % (first,)
+            print("** New total completion: %r. Checking for further matches...\n" % (first,))
         return self.cql_complete_multiple(text, first, init_bindings, startsymbol=startsymbol)
 
     @staticmethod
     def cql_extract_orig(toklist, srcstr):
         # low end of span for first token, to high end of span for last token
         return srcstr[toklist[0][2][0]:toklist[-1][2][1]]
```

## cqlshlib/cqlshhandling.py

```diff
@@ -11,15 +11,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
-import cqlhandling
+
+from cqlshlib import cqlhandling
 
 # we want the cql parser to understand our cqlsh-specific commands too
 my_commands_ending_with_newline = (
     'help',
     '?',
     'consistency',
     'serial',
@@ -73,29 +74,31 @@
                    | <pagingCommand>
                    | <clearCommand>
                    ;
 '''
 
 cqlsh_describe_cmd_syntax_rules = r'''
 <describeCommand> ::= ( "DESCRIBE" | "DESC" )
-                                  ( "FUNCTIONS"
+                                ( ( "FUNCTIONS"
                                   | "FUNCTION" udf=<anyFunctionName>
                                   | "AGGREGATES"
                                   | "AGGREGATE" uda=<userAggregateName>
                                   | "KEYSPACES"
-                                  | "KEYSPACE" ksname=<keyspaceName>?
+                                  | "ONLY"? "KEYSPACE" ksname=<keyspaceName>?
                                   | ( "COLUMNFAMILY" | "TABLE" ) cf=<columnFamilyName>
                                   | "INDEX" idx=<indexName>
                                   | "MATERIALIZED" "VIEW" mv=<materializedViewName>
                                   | ( "COLUMNFAMILIES" | "TABLES" )
                                   | "FULL"? "SCHEMA"
                                   | "CLUSTER"
                                   | "TYPES"
                                   | "TYPE" ut=<userTypeName>
-                                  | (ksname=<keyspaceName> | cf=<columnFamilyName> | idx=<indexName> | mv=<materializedViewName>))
+                                  | (ksname=<keyspaceName> | cf=<columnFamilyName> | idx=<indexName> | mv=<materializedViewName>)
+                                  ) ("WITH" "INTERNALS")?
+                                )
                     ;
 '''
 
 cqlsh_consistency_cmd_syntax_rules = r'''
 <consistencyCommand> ::= "CONSISTENCY" ( level=<consistencyLevel> )?
                        ;
 '''
@@ -108,14 +111,15 @@
                      | "QUORUM"
                      | "ALL"
                      | "LOCAL_QUORUM"
                      | "EACH_QUORUM"
                      | "SERIAL"
                      | "LOCAL_SERIAL"
                      | "LOCAL_ONE"
+                     | "NODE_LOCAL"
                      ;
 '''
 
 cqlsh_serial_consistency_cmd_syntax_rules = r'''
 <serialConsistencyCommand> ::= "SERIAL" "CONSISTENCY" ( level=<serialConsistencyLevel> )?
                              ;
 '''
@@ -235,15 +239,15 @@
     partial_path = ctxt.get_binding('partial', '')
     head, tail = os.path.split(partial_path)
     exhead = os.path.expanduser(head)
     try:
         contents = os.listdir(exhead or '.')
     except OSError:
         return ()
-    matches = filter(lambda f: f.startswith(tail), contents)
+    matches = [f for f in contents if f.startswith(tail)]
     annotated = []
     for f in matches:
         match = os.path.join(head, f)
         if os.path.isdir(os.path.join(exhead, f)):
             match += '/'
         annotated.append(match)
     return annotated
@@ -262,15 +266,15 @@
     if partial_path == '':
         return ["'"]
     return ()
 
 
 @cqlsh_syntax_completer('copyCommand', 'colnames')
 def complete_copy_column_names(ctxt, cqlsh):
-    existcols = map(cqlsh.cql_unprotect_name, ctxt.get_binding('colnames', ()))
+    existcols = list(map(cqlsh.cql_unprotect_name, ctxt.get_binding('colnames', ())))
     ks = cqlsh.cql_unprotect_name(ctxt.get_binding('ksname', None))
     cf = cqlsh.cql_unprotect_name(ctxt.get_binding('cfname'))
     colnames = cqlsh.get_column_names(ks, cf)
     if len(existcols) == 0:
         return [colnames[0]]
     return set(colnames[1:]) - set(existcols)
 
@@ -283,15 +287,15 @@
                      'TTL']
 COPY_TO_OPTIONS = ['ENCODING', 'PAGESIZE', 'PAGETIMEOUT', 'BEGINTOKEN', 'ENDTOKEN', 'MAXOUTPUTSIZE', 'MAXREQUESTS',
                    'FLOATPRECISION', 'DOUBLEPRECISION']
 
 
 @cqlsh_syntax_completer('copyOption', 'optnames')
 def complete_copy_options(ctxt, cqlsh):
-    optnames = map(str.upper, ctxt.get_binding('optnames', ()))
+    optnames = list(map(str.upper, ctxt.get_binding('optnames', ())))
     direction = ctxt.get_binding('dir').upper()
     if direction == 'FROM':
         opts = set(COPY_COMMON_OPTIONS + COPY_FROM_OPTIONS) - set(optnames)
     elif direction == 'TO':
         opts = set(COPY_COMMON_OPTIONS + COPY_TO_OPTIONS) - set(optnames)
     return opts
```

## cqlshlib/formatting.py

```diff
@@ -10,35 +10,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import binascii
 import calendar
 import datetime
 import math
 import os
 import re
 import sys
-import six
-import platform
-import wcwidth
 
 from collections import defaultdict
-from displaying import colorme, get_str, FormattedValue, DEFAULT_VALUE_COLORS, NO_COLOR_MAP
+
 from cassandra.cqltypes import EMPTY
 from cassandra.util import datetime_from_timestamp
-from util import UTC
-
-is_win = platform.system() == 'Windows'
+from . import wcwidth
+from .displaying import colorme, get_str, FormattedValue, DEFAULT_VALUE_COLORS, NO_COLOR_MAP
+from .util import UTC
 
-unicode_controlchars_re = re.compile(r'[\x00-\x31\x7f-\xa0]')
-controlchars_re = re.compile(r'[\x00-\x31\x7f-\xff]')
+unicode_controlchars_re = re.compile(r'[\x00-\x1f\x7f-\xa0]')
+controlchars_re = re.compile(r'[\x00-\x1f\x7f-\xff]')
 
 
 def _show_control_chars(match):
     txt = repr(match.group(0))
     if txt.startswith('u'):
         txt = txt[2:-1]
     else:
@@ -118,15 +114,15 @@
         self.timestamp_format = timestamp_format
         self.date_format = date_format
         self.nanotime_format = nanotime_format
         self.timezone = timezone
         self.milliseconds_only = milliseconds_only  # the microseconds part, .NNNNNN, wil be rounded to .NNN
 
 
-class CqlType(object):
+class CqlType:
     """
     A class for converting a string into a cql type name that can match a formatter
     and a list of its sub-types, if any.
     """
     pattern = re.compile('^([^<]*)<(.*)>$')  # *<*>
 
     def __init__(self, typestring, ksmeta=None):
@@ -214,15 +210,14 @@
 # making format_value a generic function
 _formatters = {}
 
 
 def format_value(val, cqltype, **kwargs):
     if val == EMPTY:
         return format_value_default('', **kwargs)
-
     formatter = get_formatter(val, cqltype)
     return formatter(val, cqltype=cqltype, **kwargs)
 
 
 def get_formatter(val, cqltype):
     if cqltype and cqltype.formatter:
         return cqltype.formatter
@@ -232,24 +227,26 @@
 
 def formatter_for(typname):
     def registrator(f):
         _formatters[typname.lower()] = f
         return f
     return registrator
 
-class BlobType(object):
+
+class BlobType:
     def __init__(self, val):
         self.val = val
 
     def __str__(self):
         return str(self.val)
 
+
 @formatter_for('BlobType')
 def format_value_blob(val, colormap, **_):
-    bval = '0x' + binascii.hexlify(val)
+    bval = '0x' + val.hex()
     return colorme(bval, colormap, 'blob')
 
 
 formatter_for('bytearray')(format_value_blob)
 formatter_for('buffer')(format_value_blob)
 formatter_for('blob')(format_value_blob)
 
@@ -321,14 +318,15 @@
 formatter_for('float')(format_floating_point_type)
 formatter_for('double')(format_floating_point_type)
 
 
 def format_integer_type(val, colormap, thousands_sep=None, **_):
     # base-10 only for now; support others?
     bval = format_integer_with_thousands_sep(val, thousands_sep) if thousands_sep else str(val)
+    bval = str(bval)
     return colorme(bval, colormap, 'int')
 
 
 # We can get rid of this in cassandra-2.2
 if sys.version_info >= (2, 7):
     def format_integer_with_thousands_sep(val, thousands_sep=','):
         return "{:,.0f}".format(val).replace(',', thousands_sep)
@@ -381,15 +379,15 @@
         # since the epoch. cqlsh does the exact same thing for values below datetime.MINYEAR (1) or above
         # datetime.MAXYEAR (9999). Some versions of strftime() also have problems for dates between MIN_YEAR and 1900.
         # cqlsh COPY assumes milliseconds from the epoch if it fails to parse a datetime string, and so it is
         # able to correctly import timestamps exported as milliseconds since the epoch.
         return '%d' % (seconds * 1000.0)
 
 
-microseconds_regex = re.compile("(.*)(?:\.(\d{1,6}))(.*)")
+microseconds_regex = re.compile(r"(.*)(?:\.(\d{1,6}))(.*)")
 
 
 def round_microseconds(val):
     """
     For COPY TO, we need to round microsecond to milliseconds because server side
     TimestampSerializer.dateStringPatterns only parses milliseconds. If we keep microseconds,
     users may try to import with COPY FROM a file generated with COPY TO and have problems if
@@ -456,22 +454,22 @@
     Cassandra vints are encoded differently than the varints used in protocol buffer.
     The Cassandra vints are encoded with the most significant group first. The most significant byte will contains
     the information about how many extra bytes need to be read as well as the most significant bits of the integer.
     The number extra bytes to read is encoded as 1 bits on the left side.
     For example, if we need to read 3 more bytes the first byte will start with 1110.
     """
 
-    first_byte = buf.next()
+    first_byte = next(buf)
     if (first_byte >> 7) == 0:
         return first_byte
 
     size = number_of_extra_bytes_to_read(first_byte)
     retval = first_byte & (0xff >> size)
     for i in range(size):
-        b = buf.next()
+        b = next(buf)
         retval <<= 8
         retval |= b & 0xff
 
     return retval
 
 
 def number_of_extra_bytes_to_read(b):
@@ -480,23 +478,22 @@
 
 def decode_zig_zag_64(n):
     return (n >> 1) ^ -(n & 1)
 
 
 @formatter_for('str')
 def format_value_text(val, encoding, colormap, quote=False, **_):
-    escapedval = val.replace(u'\\', u'\\\\')
+    escapedval = val.replace('\\', '\\\\')
     if quote:
         escapedval = escapedval.replace("'", "''")
     escapedval = unicode_controlchars_re.sub(_show_control_chars, escapedval)
-    bval = escapedval.encode(encoding, 'backslashreplace')
+    bval = escapedval
     if quote:
-        bval = "'%s'" % bval
-
-    return bval if colormap is NO_COLOR_MAP else color_text(bval, colormap, wcwidth.wcswidth(bval.decode(encoding)))
+        bval = "'{}'".format(bval)
+    return bval if colormap is NO_COLOR_MAP else color_text(bval, colormap, wcwidth.wcswidth(bval))
 
 
 # name alias
 formatter_for('unicode')(format_value_text)
 formatter_for('text')(format_value_text)
 formatter_for('ascii')(format_value_text)
 
@@ -535,15 +532,15 @@
                                     date_time_format, float_precision, nullval,
                                     decimal_sep, thousands_sep, boolean_styles)
 
 
 @formatter_for('set')
 def format_value_set(val, cqltype, encoding, colormap, date_time_format, float_precision, nullval,
                      decimal_sep, thousands_sep, boolean_styles, **_):
-    return format_simple_collection(sorted(val), cqltype, '{', '}', encoding, colormap,
+    return format_simple_collection(val, cqltype, '{', '}', encoding, colormap,
                                     date_time_format, float_precision, nullval,
                                     decimal_sep, thousands_sep, boolean_styles)
 
 
 formatter_for('frozenset')(format_value_set)
 formatter_for('sortedset')(format_value_set)
 formatter_for('SortedSet')(format_value_set)
@@ -587,15 +584,15 @@
                             date_time_format=date_time_format, float_precision=float_precision,
                             nullval=nullval, quote=True, decimal_sep=decimal_sep,
                             thousands_sep=thousands_sep, boolean_styles=boolean_styles)
 
     def format_field_name(name):
         return format_value_text(name, encoding=encoding, colormap=colormap, quote=False)
 
-    subs = [(format_field_name(k), format_field_value(v, t)) for ((k, v), t) in zip(val._asdict().items(),
+    subs = [(format_field_name(k), format_field_value(v, t)) for ((k, v), t) in zip(list(val._asdict().items()),
                                                                                     cqltype.sub_types)]
     bval = '{' + ', '.join(get_str(k) + ': ' + get_str(v) for (k, v) in subs) + '}'
     if colormap is NO_COLOR_MAP:
         return bval
 
     lb, comma, colon, rb = [colormap['collection'] + s + colormap['reset']
                             for s in ('{', ', ', ': ', '}')]
```

## cqlshlib/helptopics.py

```diff
@@ -11,15 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-class CQL3HelpTopics(object):
+class CQL3HelpTopics:
     def get_help_topics(self):
         return [t[5:] for t in dir(self) if t.startswith('help_')]
 
     def get_help_topic(self, topic):
         return getattr(self, 'help_' + topic.lower())()
 
     def help_types(self):
```

## cqlshlib/pylexotron.py

```diff
@@ -11,15 +11,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import re
-from .saferscanner import SaferScanner
+
+from cqlshlib.saferscanner import SaferScanner
 
 
 class LexingError(Exception):
 
     @classmethod
     def from_text(cls, rulestr, unmatched, msg='Lexing error'):
         bad_char = len(rulestr) - len(unmatched)
@@ -103,23 +104,14 @@
             return ''
         orig = self.bindings.get('*SRC*', None)
         if orig is None:
             # pretty much just guess
             return ' '.join([t[1] for t in tokens])
         # low end of span for first token, to high end of span for last token
         orig_text = orig[tokens[0][2][0]:tokens[-1][2][1]]
-
-        # Convert all unicode tokens to ascii, where possible.  This
-        # helps avoid problems with performing unicode-incompatible
-        # operations on tokens (like .lower()).  See CASSANDRA-9083
-        # for one example of this.
-        try:
-            orig_text = orig_text.encode('ascii')
-        except UnicodeEncodeError:
-            pass
         return orig_text
 
     def __repr__(self):
         return '<%s matched=%r remainder=%r prodname=%r bindings=%r>' \
                % (self.__class__.__name__, self.matched, self.remainder, self.productionname, self.bindings)
 
 
@@ -142,24 +134,24 @@
         if ctxt.remainder or completions is None:
             return False
         try:
             completer = ctxt.get_completer(symname)
         except KeyError:
             return False
         if debugging:
-            print "Trying completer %r with %r" % (completer, ctxt)
+            print("Trying completer %r with %r" % (completer, ctxt))
         try:
             new_compls = completer(ctxt)
         except Exception:
             if debugging:
                 import traceback
                 traceback.print_exc()
             return False
         if debugging:
-            print "got %r" % (new_compls,)
+            print("got %r" % (new_compls,))
         completions.update(new_compls)
         return True
 
     def __repr__(self):
         return '%s(%r)' % (self.__class__.__name__, self.arg)
 
 
@@ -280,15 +272,15 @@
 class text_match(terminal_matcher):
     alpha_re = re.compile(r'[a-zA-Z]')
 
     def __init__(self, text):
         try:
             terminal_matcher.__init__(self, eval(text))
         except SyntaxError:
-            print "bad syntax %r" % (text,)
+            print("bad syntax %r" % (text,))
 
     def match(self, ctxt, completions):
         if ctxt.remainder:
             if self.arg.lower() == ctxt.remainder[0][1].lower():
                 return [ctxt.with_match(1)]
         elif completions is not None:
             completions.add(self.arg)
@@ -355,15 +347,15 @@
         (r'/(\[\^?.[^]]*\]|[^/]|\\.)*/', lambda s, t: ('regex', t[1:-1].replace(r'\/', '/'))),
         (r'"([^"]|\\.)*"', lambda s, t: ('litstring', t)),
         (r'<[^>]*>', lambda s, t: ('reference', t[1:-1])),
         (r'\bJUNK\b', lambda s, t: ('junk', t)),
         (r'[@()|?*;]', lambda s, t: t),
         (r'\s+', None),
         (r'#[^\n]*', None),
-    ], re.I | re.S)
+    ], re.I | re.S | re.U)
 
     def __init__(self):
         self.ruleset = {}
         self.scanner = None
         self.terminals = []
 
     @classmethod
@@ -378,15 +370,15 @@
         if unmatched:
             raise LexingError.from_text(rulestr, unmatched, msg="Syntax rules unparseable")
         rules = {}
         terminals = []
         tokeniter = iter(tokens)
         for t in tokeniter:
             if isinstance(t, tuple) and t[0] in ('reference', 'junk'):
-                assign = tokeniter.next()
+                assign = next(tokeniter)
                 if assign != '::=':
                     raise ValueError('Unexpected token %r; expected "::="' % (assign,))
                 name = t[1]
                 production = cls.read_rule_tokens_until(';', tokeniter)
                 if isinstance(production, terminal_matcher):
                     terminals.append((name, production))
                     production = terminal_type_matcher(name, production)
@@ -401,29 +393,29 @@
             if len(pieces) == 1:
                 return pieces[0]
             return rule_series(pieces)
         return pieces
 
     @classmethod
     def read_rule_tokens_until(cls, endtoks, tokeniter):
-        if isinstance(endtoks, basestring):
+        if isinstance(endtoks, str):
             endtoks = (endtoks,)
         counttarget = None
         if isinstance(endtoks, int):
             counttarget = endtoks
             endtoks = ()
         countsofar = 0
         myrules = []
         mybranches = [myrules]
         for t in tokeniter:
             countsofar += 1
             if t in endtoks:
                 if len(mybranches) == 1:
                     return cls.mkrule(mybranches[0])
-                return choice(map(cls.mkrule, mybranches))
+                return choice(list(map(cls.mkrule, mybranches)))
             if isinstance(t, tuple):
                 if t[0] == 'reference':
                     t = rule_reference(t[1])
                 elif t[0] == 'litstring':
                     if t[1][1].isalnum() or t[1][1] == '_':
                         t = word_match(t[1])
                     else:
@@ -437,29 +429,29 @@
             elif t == '(':
                 t = cls.read_rule_tokens_until(')', tokeniter)
             elif t == '?':
                 t = one_or_none(myrules.pop(-1))
             elif t == '*':
                 t = repeat(myrules.pop(-1))
             elif t == '@':
-                x = tokeniter.next()
+                x = next(tokeniter)
                 if not isinstance(x, tuple) or x[0] != 'litstring':
                     raise ValueError("Unexpected token %r following '@'" % (x,))
                 t = case_match(x[1])
             elif t == '|':
                 myrules = []
                 mybranches.append(myrules)
                 continue
             else:
                 raise ValueError('Unparseable rule token %r after %r' % (t, myrules[-1]))
             myrules.append(t)
             if countsofar == counttarget:
                 if len(mybranches) == 1:
                     return cls.mkrule(mybranches[0])
-                return choice(map(cls.mkrule, mybranches))
+                return choice(list(map(cls.mkrule, mybranches)))
         raise ValueError('Unexpected end of rule tokens')
 
     def append_rules(self, rulestr):
         rules, terminals = self.parse_rules(rulestr)
         self.ruleset.update(rules)
         self.terminals.extend(terminals)
         if terminals:
@@ -470,15 +462,15 @@
 
     def make_lexer(self):
         def make_handler(name):
             if name == 'JUNK':
                 return None
             return lambda s, t: (name, t, s.match.span())
         regexes = [(p.pattern(), make_handler(name)) for (name, p) in self.terminals]
-        return SaferScanner(regexes, re.I | re.S).scan
+        return SaferScanner(regexes, re.I | re.S | re.U).scan
 
     def lex(self, text):
         if self.scanner is None:
             self.scanner = self.make_lexer()
         tokens, unmatched = self.scanner(text)
         if unmatched:
             raise LexingError.from_text(text, unmatched, 'text could not be lexed')
```

## cqlshlib/saferscanner.py

```diff
@@ -16,31 +16,18 @@
 
 # SaferScanner is just like re.Scanner, but it neuters any grouping in the lexicon
 # regular expressions and throws an error on group references, named groups, or
 # regex in-pattern flags. Any of those can break correct operation of Scanner.
 
 import re
 from sre_constants import BRANCH, SUBPATTERN, GROUPREF, GROUPREF_IGNORE, GROUPREF_EXISTS
+from sys import version_info
 
 
-class SaferScanner(re.Scanner):
-
-    def __init__(self, lexicon, flags=0):
-        self.lexicon = lexicon
-        p = []
-        s = re.sre_parse.Pattern()
-        s.flags = flags
-        for phrase, action in lexicon:
-            p.append(re.sre_parse.SubPattern(s, [
-                (SUBPATTERN, (len(p) + 1, self.subpat(phrase, flags))),
-            ]))
-        s.groups = len(p) + 1
-        p = re.sre_parse.SubPattern(s, [(BRANCH, (None, p))])
-        self.p = p
-        self.scanner = re.sre_compile.compile(p)
+class SaferScannerBase(re.Scanner):
 
     @classmethod
     def subpat(cls, phrase, flags):
         return cls.scrub_sub(re.sre_parse.parse(phrase, flags), flags)
 
     @classmethod
     def scrub_sub(cls, sub, flags):
@@ -56,7 +43,42 @@
                 raise ValueError("Group references not allowed in SaferScanner lexicon")
             scrubbedsub.append((op, arg))
         if sub.pattern.groupdict:
             raise ValueError("Named captures not allowed in SaferScanner lexicon")
         if sub.pattern.flags ^ flags:
             raise ValueError("RE flag setting not allowed in SaferScanner lexicon (%s)" % (bin(sub.pattern.flags),))
         return re.sre_parse.SubPattern(sub.pattern, scrubbedsub)
+
+
+class Py36SaferScanner(SaferScannerBase):
+
+    def __init__(self, lexicon, flags=0):
+        self.lexicon = lexicon
+        p = []
+        s = re.sre_parse.Pattern()
+        s.flags = flags
+        for phrase, action in lexicon:
+            gid = s.opengroup()
+            p.append(re.sre_parse.SubPattern(s, [(SUBPATTERN, (gid, 0, 0, re.sre_parse.parse(phrase, flags))), ]))
+            s.closegroup(gid, p[-1])
+        p = re.sre_parse.SubPattern(s, [(BRANCH, (None, p))])
+        self.p = p
+        self.scanner = re.sre_compile.compile(p)
+
+
+class Py38SaferScanner(SaferScannerBase):
+
+    def __init__(self, lexicon, flags=0):
+        self.lexicon = lexicon
+        p = []
+        s = re.sre_parse.State()
+        s.flags = flags
+        for phrase, action in lexicon:
+            gid = s.opengroup()
+            p.append(re.sre_parse.SubPattern(s, [(SUBPATTERN, (gid, 0, 0, re.sre_parse.parse(phrase, flags))), ]))
+            s.closegroup(gid, p[-1])
+        p = re.sre_parse.SubPattern(s, [(BRANCH, (None, p))])
+        self.p = p
+        self.scanner = re.sre_compile.compile(p)
+
+
+SaferScanner = Py38SaferScanner if version_info >= (3, 8) else Py36SaferScanner
```

## cqlshlib/sslhandling.py

```diff
@@ -12,17 +12,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import sys
-import ConfigParser
 import ssl
 
+import configparser
+
 
 def ssl_settings(host, config_file, env=os.environ):
     """
     Function which generates SSL setting for cassandra.Cluster
 
     Params:
     * host .........: hostname of Cassandra node.
@@ -34,38 +35,38 @@
                       mapping in [certfiles] section.
 
     [certfiles] section is optional, 'validate' setting in [ssl] section is
     optional too. If validation is enabled then SSL certfile must be provided
     either in the config file or as an environment variable.
     Environment variables override any options set in cqlsh config file.
     """
-    configs = ConfigParser.SafeConfigParser()
+    configs = configparser.ConfigParser()
     configs.read(config_file)
 
     def get_option(section, option):
         try:
             return configs.get(section, option)
-        except ConfigParser.Error:
+        except configparser.Error:
             return None
 
+    def get_best_tls_protocol(ssl_ver_str):
+        if ssl_ver_str:
+            print("Warning: Explicit SSL and TLS versions in the cqlshrc file or in SSL_VERSION environment property are ignored as the protocol is auto-negotiated.\n")
+        return ssl.PROTOCOL_TLS
+
     ssl_validate = env.get('SSL_VALIDATE')
     if ssl_validate is None:
         ssl_validate = get_option('ssl', 'validate')
     ssl_validate = ssl_validate is None or ssl_validate.lower() != 'false'
 
     ssl_version_str = env.get('SSL_VERSION')
     if ssl_version_str is None:
         ssl_version_str = get_option('ssl', 'version')
-    if ssl_version_str is None:
-        ssl_version_str = "TLSv1"
 
-    ssl_version = getattr(ssl, "PROTOCOL_%s" % ssl_version_str, None)
-    if ssl_version is None:
-        sys.exit("%s is not a valid SSL protocol, please use one of SSLv23, "
-                 "TLSv1, TLSv1.1, or TLSv1.2" % (ssl_version_str,))
+    ssl_version = get_best_tls_protocol(ssl_version_str)
 
     ssl_certfile = env.get('SSL_CERTFILE')
     if ssl_certfile is None:
         ssl_certfile = get_option('certfiles', host)
     if ssl_certfile is None:
         ssl_certfile = get_option('ssl', 'certfile')
     if ssl_validate and ssl_certfile is None:
```

## cqlshlib/tracing.py

```diff
@@ -10,19 +10,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from cqlshlib.displaying import MAGENTA
-from datetime import datetime, timedelta
-from formatting import CqlType
+from datetime import datetime
 import time
+
 from cassandra.query import QueryTrace, TraceUnavailable
+from cqlshlib.displaying import MAGENTA
 
 
 def print_trace_session(shell, session, session_id, partial_session=False):
     """
     Lookup a trace by session and trace session ID, then print it.
     """
     trace = QueryTrace(session_id, session)
@@ -41,16 +41,16 @@
     """
     rows = make_trace_rows(trace)
     if not rows:
         shell.printerr("No rows for session %s found." % (trace.trace_id,))
         return
     names = ['activity', 'timestamp', 'source', 'source_elapsed', 'client']
 
-    formatted_names = map(shell.myformat_colname, names)
-    formatted_values = [map(shell.myformat_value, row) for row in rows]
+    formatted_names = list(map(shell.myformat_colname, names))
+    formatted_values = [list(map(shell.myformat_value, row)) for row in rows]
 
     shell.writeresult('')
     shell.writeresult('Tracing session: ', color=MAGENTA, newline=False)
     shell.writeresult(trace.trace_id)
     shell.writeresult('')
     shell.print_formatted_result(formatted_names, formatted_values, with_header=True, tty=shell.tty)
     shell.writeresult('')
@@ -69,16 +69,14 @@
                      event.source,
                      total_micro_seconds(event.source_elapsed),
                      trace.client])
     # append footer row (from sessions table).
     if trace.duration:
         finished_at = (datetime_from_utc_to_local(trace.started_at) + trace.duration)
         rows.append(['Request complete', str(finished_at), trace.coordinator, total_micro_seconds(trace.duration), trace.client])
-    else:
-        finished_at = trace.duration = "--"
 
     return rows
 
 
 def total_micro_seconds(td):
     """
     Convert a timedelta into total microseconds
```

## cqlshlib/util.py

```diff
@@ -14,18 +14,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import cProfile
 import codecs
 import pstats
+import os
+import errno
+import stat
 
-from itertools import izip
 from datetime import timedelta, tzinfo
-from StringIO import StringIO
+from io import StringIO
 
 try:
     from line_profiler import LineProfiler
     HAS_LINE_PROFILER = True
 except ImportError:
     HAS_LINE_PROFILER = False
 
@@ -73,15 +75,15 @@
     >>> find_common_prefix(['abracadabra', 'abracadero', 'abranch'])
     'abra'
     >>> find_common_prefix(['abracadabra', 'abracadero', 'mt. fuji'])
     ''
     """
 
     common = []
-    for cgroup in izip(*strs):
+    for cgroup in zip(*strs):
         if all(x == cgroup[0] for x in cgroup[1:]):
             common.append(cgroup[0])
         else:
             break
     return ''.join(common)
 
 
@@ -108,14 +110,29 @@
 
 def trim_if_present(s, prefix):
     if s.startswith(prefix):
         return s[len(prefix):]
     return s
 
 
+def is_file_secure(filename):
+    try:
+        st = os.stat(filename)
+    except OSError as e:
+        if e.errno != errno.ENOENT:
+            raise
+        # the file doesn't exist, the security of it is irrelevant
+        return True
+    uid = os.getuid()
+
+    # Skip enforcing the file owner and UID matching for the root user (uid == 0).
+    # This is to allow "sudo cqlsh" to work with user owned credentials file.
+    return (uid == 0 or st.st_uid == uid) and stat.S_IMODE(st.st_mode) & (stat.S_IRGRP | stat.S_IROTH) == 0
+
+
 def get_file_encoding_bomsize(filename):
     """
     Checks the beginning of a file for a Unicode BOM.  Based on this check,
     the encoding that should be used to open the file and the number of
     bytes that should be skipped (to skip the BOM) are returned.
     """
     bom_encodings = ((codecs.BOM_UTF8, 'utf-8-sig'),
@@ -157,10 +174,10 @@
     else:
         ps = pstats.Stats(pr, stream=s).sort_stats('cumulative')
         ps.print_stats()
 
     ret = s.getvalue()
     if file_name:
         with open(file_name, 'w') as f:
-            print "Writing to %s\n" % (f.name, )
+            print("Writing to %s\n" % (f.name, ))
             f.write(ret)
     return ret
```

## cqlshlib/wcwidth.py

```diff
@@ -81,15 +81,15 @@
 
 def bisearch(ucs, table):
     min = 0
     max = len(table) - 1
     if ucs < table[0][0] or ucs > table[max][1]:
         return 0
     while max >= min:
-        mid = (min + max) / 2
+        mid = int((min + max) / 2)
         if ucs > table[mid][1]:
             min = mid + 1
         elif ucs < table[mid][0]:
             max = mid - 1
         else:
             return 1
     return 0
@@ -247,28 +247,29 @@
 
     # binary search in table of non-spacing characters
     if bisearch(ucs, combining):
         return 0
 
     # if we arrive here, ucs is not a combining or C0/C1 control character
 
-    return 1 + \
-        int(ucs >= 0x1100 and
-            (ucs <= 0x115f or                     # Hangul Jamo init. consonants
-             ucs == 0x2329 or ucs == 0x232a or
-             (ucs >= 0x2e80 and ucs <= 0xa4cf and
-              ucs != 0x303f) or                   # CJK ... Yi
-                (ucs >= 0xac00 and ucs <= 0xd7a3) or  # Hangul Syllables
-                (ucs >= 0xf900 and ucs <= 0xfaff) or  # CJK Compatibility Ideographs
-                (ucs >= 0xfe10 and ucs <= 0xfe19) or  # Vertical forms
-                (ucs >= 0xfe30 and ucs <= 0xfe6f) or  # CJK Compatibility Forms
-                (ucs >= 0xff00 and ucs <= 0xff60) or  # Fullwidth Forms
-                (ucs >= 0xffe0 and ucs <= 0xffe6) or
-                (ucs >= 0x20000 and ucs <= 0x2fffd) or
-                (ucs >= 0x30000 and ucs <= 0x3fffd)))
+    return 1 + int(
+        ucs >= 0x1100
+        and (ucs <= 0x115f                    # Hangul Jamo init. consonants
+             or ucs == 0x2329 or ucs == 0x232a
+             or (ucs >= 0x2e80 and ucs <= 0xa4cf
+                 and ucs != 0x303f)                # CJK ... Yi
+             or (ucs >= 0xac00 and ucs <= 0xd7a3)  # Hangul Syllables
+             or (ucs >= 0xf900 and ucs <= 0xfaff)  # CJK Compatibility Ideographs
+             or (ucs >= 0xfe10 and ucs <= 0xfe19)  # Vertical forms
+             or (ucs >= 0xfe30 and ucs <= 0xfe6f)  # CJK Compatibility Forms
+             or (ucs >= 0xff00 and ucs <= 0xff60)  # Fullwidth Forms
+             or (ucs >= 0xffe0 and ucs <= 0xffe6)
+             or (ucs >= 0x20000 and ucs <= 0x2fffd)
+             or (ucs >= 0x30000 and ucs <= 0x3fffd))
+    )
 
 
 def mk_wcswidth(pwcs):
     width = 0
     for c in pwcs:
         w = mk_wcwidth(c)
         if w < 0:
@@ -309,23 +310,23 @@
 
 
 def wcwidth(c):
     return mk_wcwidth(ord(c))
 
 
 def wcswidth(s):
-    return mk_wcswidth(map(ord, s))
+    return mk_wcswidth(list(map(ord, s)))
 
 
 def wcwidth_cjk(c):
     return mk_wcwidth_cjk(ord(c))
 
 
 def wcswidth_cjk(s):
-    return mk_wcswidth_cjk(map(ord, s))
+    return mk_wcswidth_cjk(list(map(ord, s)))
 
 
 if __name__ == "__main__":
     samples = (
         ('MUSIC SHARP SIGN', 1),
         ('FULLWIDTH POUND SIGN', 2),
         ('FULLWIDTH LATIN CAPITAL LETTER P', 2),
@@ -337,15 +338,15 @@
         ('CJK COMPATIBILITY IDEOGRAPH-F920', 2),
         ('MALAYALAM VOWEL SIGN UU', 0),
         ('ZERO WIDTH SPACE', 0),
         ('ZERO WIDTH NO-BREAK SPACE', 0),
         ('COMBINING PALATALIZED HOOK BELOW', 0),
         ('COMBINING GRAVE ACCENT', 0),
     )
-    nonprinting = u'\r\n\t\a\b\f\v\x7f'
+    nonprinting = '\r\n\t\a\b\f\v\x7f'
 
     import unicodedata
 
     for name, printwidth in samples:
         uchr = unicodedata.lookup(name)
         calculatedwidth = wcwidth(uchr)
         assert calculatedwidth == printwidth, \
@@ -362,17 +363,17 @@
     # treated as single characters, so ord() won't work. test a few of these
     # manually.
 
     assert mk_wcwidth(0xe01ef) == 0
     assert mk_wcwidth(0x10ffff) == 1
     assert mk_wcwidth(0x3fffd) == 2
 
-    teststr = u'B\0ig br\u00f8wn moose\ub143\u200b'
+    teststr = 'B\0ig br\u00f8wn moose\ub143\u200b'
     calculatedwidth = wcswidth(teststr)
     assert calculatedwidth == 17, 'expected 17, got %d' % calculatedwidth
 
     calculatedwidth = wcswidth_cjk(teststr)
     assert calculatedwidth == 18, 'expected 18, got %d' % calculatedwidth
 
-    assert wcswidth(u'foobar\u200b\a') < 0
+    assert wcswidth('foobar\u200b\a') < 0
 
-    print 'tests pass.'
+    print('tests pass.')
```

## Comparing `cqlsh_expansion-0.7.8.data/scripts/cqlsh-expansion.py` & `cqlsh_expansion-0.9.0.data/scripts/cqlsh-expansion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-#!/bin/sh
-# -*- mode: Python -*-
+#!python
 
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
@@ -13,72 +12,62 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-""":"
-# bash code here; finds a suitable python interpreter and execs this file.
-# prefer unqualified "python" if suitable:
-python -c 'import sys; sys.exit(not (0x020700b0 < sys.hexversion < 0x03000000))' 2>/dev/null \
-    && exec python "$0" "$@"
-for pyver in 2.7; do
-    which python$pyver > /dev/null 2>&1 && exec python$pyver "$0" "$@"
-done
-echo "No appropriate python interpreter found." >&2
-exit 1
-":"""
-
-from __future__ import with_statement
-
 import cmd
 import codecs
-import ConfigParser
+import configparser
 import csv
+import errno
 import getpass
 import optparse
 import os
 import platform
+import re
+import stat
+import subprocess
 import sys
 import traceback
 import warnings
 import webbrowser
-from StringIO import StringIO
 from contextlib import contextmanager
 from glob import glob
+from io import StringIO
 from uuid import UUID
+from ssl import SSLContext, PROTOCOL_TLSv1_2, CERT_REQUIRED
 
-if sys.version_info[0] != 2 or sys.version_info[1] != 7:
-    sys.exit("\nCQL Shell supports only Python 2.7\n")
+if sys.version_info < (3, 6):
+    sys.exit("\ncqlsh requires Python 3.6+\n")
 
 # see CASSANDRA-10428
 if platform.python_implementation().startswith('Jython'):
     sys.exit("\nCQL Shell does not run on Jython\n")
 
 UTF8 = 'utf-8'
-CP65001 = 'cp65001'  # Win utf-8 variant
 
 description = "CQL Shell for Apache Cassandra"
-version = "5.0.1"
+version = "6.1.0"
 
 readline = None
 try:
     # check if tty first, cause readline doesn't check, and only cares
     # about $TERM. we don't want the funky escape code stuff to be
     # output if not a tty.
     if sys.stdin.isatty():
         import readline
 except ImportError:
     pass
 
 CQL_LIB_PREFIX = 'cassandra-driver-internal-only-'
 
 CASSANDRA_PATH = os.path.join(os.path.dirname(os.path.realpath(__file__)), '..')
-CASSANDRA_CQL_HTML_FALLBACK = 'https://cassandra.apache.org/doc/cql3/CQL-3.2.html'
+CASSANDRA_CQL_HTML_FALLBACK = 'https://cassandra.apache.org/doc/latest/cql/index.html'
 
 # default location of local CQL.html
 if os.path.exists(CASSANDRA_PATH + '/doc/cql3/CQL.html'):
     # default location of local CQL.html
     CASSANDRA_CQL_HTML = 'file://' + CASSANDRA_PATH + '/doc/cql3/CQL.html'
 elif os.path.exists('/usr/share/doc/cassandra/CQL.html'):
     # fallback to package file
@@ -88,37 +77,28 @@
     CASSANDRA_CQL_HTML = CASSANDRA_CQL_HTML_FALLBACK
 
 # On Linux, the Python webbrowser module uses the 'xdg-open' executable
 # to open a file/URL. But that only works, if the current session has been
 # opened from _within_ a desktop environment. I.e. 'xdg-open' will fail,
 # if the session's been opened via ssh to a remote box.
 #
-# Use 'python' to get some information about the detected browsers.
-# >>> import webbrowser
-# >>> webbrowser._tryorder
-# >>> webbrowser._browser
-#
-if len(webbrowser._tryorder) == 0:
-    CASSANDRA_CQL_HTML = CASSANDRA_CQL_HTML_FALLBACK
-elif webbrowser._tryorder[0] == 'xdg-open' and os.environ.get('XDG_DATA_DIRS', '') == '':
+try:
+    webbrowser.register_standard_browsers()  # registration is otherwise lazy in Python3
+except AttributeError:
+    pass
+if webbrowser._tryorder and webbrowser._tryorder[0] == 'xdg-open' and os.environ.get('XDG_DATA_DIRS', '') == '':
     # only on Linux (some OS with xdg-open)
     webbrowser._tryorder.remove('xdg-open')
     webbrowser._tryorder.append('xdg-open')
 
-# use bundled libs for python-cql and thrift, if available. if there
+# use bundled lib for python-cql if available. if there
 # is a ../lib dir, use bundled libs there preferentially.
 ZIPLIB_DIRS = [os.path.join(CASSANDRA_PATH, 'lib')]
-myplatform = platform.system()
-is_win = myplatform == 'Windows'
-
-# Workaround for supporting CP65001 encoding on python < 3.3 (https://bugs.python.org/issue13216)
-if is_win and sys.version_info < (3, 3):
-    codecs.register(lambda name: codecs.lookup(UTF8) if name == CP65001 else None)
 
-if myplatform == 'Linux':
+if platform.system() == 'Linux':
     ZIPLIB_DIRS.append('/usr/share/cassandra/lib')
 
 if os.environ.get('CQLSH_NO_BUNDLED', ''):
     ZIPLIB_DIRS = ()
 
 
 def find_zip(libprefix):
@@ -129,69 +109,64 @@
 
 
 cql_zip = find_zip(CQL_LIB_PREFIX)
 if cql_zip:
     ver = os.path.splitext(os.path.basename(cql_zip))[0][len(CQL_LIB_PREFIX):]
     sys.path.insert(0, os.path.join(cql_zip, 'cassandra-driver-' + ver))
 
-third_parties = ('futures-', 'six-', 'cassandra_sigv4-', 'boto3-', 'botocore-', 'python_dateutil-', 'urllib3-', 'jmespath-')
+# the driver needs dependencies
+third_parties = ('six-', 'pure_sasl-', 'futures-', 'cassandra_sigv4-', 'boto3-', 'botocore-', 'python_dateutil-', 'urllib3-', 'jmespath-')
 
 for lib in third_parties:
     lib_zip = find_zip(lib)
     if lib_zip:
         sys.path.insert(0, lib_zip)
 
 warnings.filterwarnings("ignore", r".*blist.*")
 try:
     import cassandra
-except ImportError, e:
+except ImportError as e:
     sys.exit("\nPython Cassandra driver not installed, or not on PYTHONPATH.\n"
              'You might try "pip install cassandra-driver".\n\n'
              'Python: %s\n'
              'Module load path: %r\n\n'
              'Error: %s\n' % (sys.executable, sys.path, e))
 
 from cassandra.auth import PlainTextAuthProvider
-from cassandra.cluster import Cluster
+from cassandra.cluster import Cluster, ExecutionProfile, EXEC_PROFILE_DEFAULT
 from cassandra.cqltypes import cql_typename
 from cassandra.marshal import int64_unpack
-from cassandra.metadata import (ColumnMetadata, KeyspaceMetadata,
-                                TableMetadata, protect_name, protect_names)
+from cassandra.metadata import (ColumnMetadata, KeyspaceMetadata, TableMetadata)
 from cassandra.policies import WhiteListRoundRobinPolicy
 from cassandra.query import SimpleStatement, ordered_dict_factory, TraceUnavailable
 from cassandra.util import datetime_from_timestamp
 
 # cqlsh should run correctly when run out of a Cassandra source tree,
 # out of an unpacked Cassandra tarball, and after a proper package install.
 cqlshlibdir = os.path.join(CASSANDRA_PATH, 'pylib')
 if os.path.isdir(cqlshlibdir):
     sys.path.insert(0, cqlshlibdir)
 
-from cqlshlib import cql3handling, cqlhandling, pylexotron, sslhandling, cqlshhandling
+from cqlshlib import cql3handling, pylexotron, sslhandling, cqlshhandling, authproviderhandling, legacydesc3x
 from cqlshlib.copyutil import ExportTask, ImportTask
 from cqlshlib.displaying import (ANSI_RESET, BLUE, COLUMN_NAME_COLORS, CYAN,
                                  RED, WHITE, FormattedValue, colorme)
 from cqlshlib.formatting import (DEFAULT_DATE_FORMAT, DEFAULT_NANOTIME_FORMAT,
                                  DEFAULT_TIMESTAMP_FORMAT, CqlType, DateTimeFormat,
-                                 format_by_type, formatter_for)
+                                 format_by_type)
 from cqlshlib.tracing import print_trace, print_trace_session
 from cqlshlib.util import get_file_encoding_bomsize, trim_if_present
-
-from cassandra_sigv4.auth import SigV4AuthProvider
-
-import boto3
-import boto3.session
+from cqlshlib.util import is_file_secure
+from cqlshlib.legacydesc3x import *
 
 DEFAULT_HOST = '127.0.0.1'
 DEFAULT_PORT = 9042
 DEFAULT_SSL = False
-DEFAULT_SIGV4 = False
 DEFAULT_CONNECT_TIMEOUT_SECONDS = 5
 DEFAULT_REQUEST_TIMEOUT_SECONDS = 10
-DEFAULT_AUTH_PROVIDER = 'PlainTextAuthProvider'
 
 DEFAULT_FLOAT_PRECISION = 5
 DEFAULT_DOUBLE_PRECISION = 5
 DEFAULT_MAX_TRACE_WAIT = 10
 
 if readline is not None and readline.__doc__ is not None and 'libedit' in readline.__doc__:
     DEFAULT_COMPLETEKEY = '\t'
@@ -210,80 +185,106 @@
                                usage="Usage: %prog [options] [host [port]]",
                                version='cqlsh ' + version)
 parser.add_option("-C", "--color", action='store_true', dest='color',
                   help='Always use color output')
 parser.add_option("--no-color", action='store_false', dest='color',
                   help='Never use color output')
 parser.add_option("--browser", dest='browser', help="""The browser to use to display CQL help, where BROWSER can be:
-                                                    - one of the supported browsers in https://docs.python.org/2/library/webbrowser.html.
+                                                    - one of the supported browsers in https://docs.python.org/3/library/webbrowser.html.
                                                     - browser path followed by %s, example: /usr/bin/google-chrome-stable %s""")
 parser.add_option('--ssl', action='store_true', help='Use SSL', default=False)
-parser.add_option('--no_compact', action='store_true', help='No Compact', default=False)
 parser.add_option("-u", "--username", help="Authenticate as user.")
 parser.add_option("-p", "--password", help="Authenticate using password.")
 parser.add_option('-k', '--keyspace', help='Authenticate to the given keyspace.')
 parser.add_option("-f", "--file", help="Execute commands from FILE, then exit")
 parser.add_option('--debug', action='store_true',
                   help='Show additional debugging information')
-parser.add_option("--encoding", help="Specify a non-default encoding for output." +
-                  " (Default: %s)" % (UTF8,))
+parser.add_option('--coverage', action='store_true',
+                  help='Collect coverage data')
+parser.add_option("--encoding", help="Specify a non-default encoding for output."
+                  + " (Default: %s)" % (UTF8,))
 parser.add_option("--cqlshrc", help="Specify an alternative cqlshrc file location.")
+parser.add_option("--credentials", help="Specify an alternative credentials file location.")
 parser.add_option('--cqlversion', default=None,
                   help='Specify a particular CQL version, '
                        'by default the highest version supported by the server will be used.'
                        ' Examples: "3.0.3", "3.1.0"')
 parser.add_option("--protocol-version", type="int", default=None,
                   help='Specify a specific protcol version otherwise the client will default and downgrade as necessary')
 
 parser.add_option("-e", "--execute", help='Execute the statement and quit.')
 parser.add_option("--connect-timeout", default=DEFAULT_CONNECT_TIMEOUT_SECONDS, dest='connect_timeout',
                   help='Specify the connection timeout in seconds (default: %default seconds).')
 parser.add_option("--request-timeout", default=DEFAULT_REQUEST_TIMEOUT_SECONDS, dest='request_timeout',
                   help='Specify the default request timeout in seconds (default: %default seconds).')
 parser.add_option("-t", "--tty", action='store_true', dest='tty',
                   help='Force tty mode (command prompt).')
-parser.add_option("--sigv4", action='store_true', help='Use SigV4AuthProvider plugin for autentication and authorization', default=DEFAULT_SIGV4)
-parser.add_option("--auth-provider", help="The AuthProvider to use when connecting. Default is PlainTextAuthProvider", dest='auth_provider_name', default=DEFAULT_AUTH_PROVIDER)
+parser.add_option('-v', action="version", help='Print the current version of cqlsh.')
+
+parser.add_option("--sigv4", action='store_true', help='sigv4 flag was deprecated, refer to cqlshrc file for authentication')
+parser.add_option("--auth-provider",action='store_true',  help='AuthProvider flag was deprecated, refer to cqlshrc file', dest='auth_provider_name')
 
-optvalues = optparse.Values()
-(options, arguments) = parser.parse_args(sys.argv[1:], values=optvalues)
+
+# This is a hidden option to suppress the warning when the -p/--password command line option is used.
+# Power users may use this option if they know no other people has access to the system where cqlsh is run or don't care about security.
+# Use of this option in scripting is discouraged. Please use a (temporary) credentials file where possible.
+# The Cassandra distributed tests (dtests) also use this option in some tests when a well-known password is supplied via the command line.
+parser.add_option("--insecure-password-without-warning", action='store_true', dest='insecure_password_without_warning',
+                  help=optparse.SUPPRESS_HELP)
+
+opt_values = optparse.Values()
+(options, arguments) = parser.parse_args(sys.argv[1:], values=opt_values)
+
+# Raise Exception for deprecated options
+if hasattr(options, 'sigv4'):
+    raise Exception('\nWarning: Specified sigv4 flag was deprecated, refer to cqlshrc file for sigv4 authentication'
+          'https://cassandra.apache.org/_/blog/Apache-Cassandra-4.1-Features-Authentication-Plugin-Support-for-CQLSH.html')
+
+if hasattr(options, 'auth_provider_name'):
+    raise Exception('\nWarning: auth-provider flag was deprecated, refer to cqlshrc file for authentication'
+          'https://cassandra.apache.org/_/blog/Apache-Cassandra-4.1-Features-Authentication-Plugin-Support-for-CQLSH.html')
 
 # BEGIN history/config definition
-HISTORY_DIR = os.path.expanduser(os.path.join('~', '.cassandra'))
 
-if hasattr(options, 'cqlshrc'):
-    CONFIG_FILE = options.cqlshrc
-    if not os.path.exists(CONFIG_FILE):
-        print '\nWarning: Specified cqlshrc location `%s` does not exist.  Using `%s` instead.\n' % (CONFIG_FILE, HISTORY_DIR)
-        CONFIG_FILE = os.path.join(HISTORY_DIR, 'cqlshrc')
-else:
-    CONFIG_FILE = os.path.join(HISTORY_DIR, 'cqlshrc')
+def mkdirp(path):
+    """Creates all parent directories up to path parameter or fails when path exists, but it is not a directory."""
 
-HISTORY = os.path.join(HISTORY_DIR, 'cqlsh_history')
-if not os.path.exists(HISTORY_DIR):
     try:
-        os.mkdir(HISTORY_DIR)
+        os.makedirs(path)
     except OSError:
-        print '\nWarning: Cannot create directory at `%s`. Command history will not be saved.\n' % HISTORY_DIR
+        if not os.path.isdir(path):
+            raise
+
 
-OLD_CONFIG_FILE = os.path.expanduser(os.path.join('~', '.cqlshrc'))
-if os.path.exists(OLD_CONFIG_FILE):
-    if os.path.exists(CONFIG_FILE):
-        print '\nWarning: cqlshrc config files were found at both the old location (%s) and \
-                the new location (%s), the old config file will not be migrated to the new \
-                location, and the new location will be used for now.  You should manually \
-                consolidate the config files at the new location and remove the old file.' \
-                % (OLD_CONFIG_FILE, CONFIG_FILE)
+def resolve_cql_history_file():
+    default_cql_history = os.path.expanduser(os.path.join('~', '.cassandra', 'cqlsh_history'))
+    if 'CQL_HISTORY' in os.environ:
+        return os.environ['CQL_HISTORY']
     else:
-        os.rename(OLD_CONFIG_FILE, CONFIG_FILE)
-OLD_HISTORY = os.path.expanduser(os.path.join('~', '.cqlsh_history'))
-if os.path.exists(OLD_HISTORY):
-    os.rename(OLD_HISTORY, HISTORY)
-# END history/config definition
+        return default_cql_history
+
+HISTORY = resolve_cql_history_file()
+HISTORY_DIR = os.path.dirname(HISTORY)
+
+try:
+    mkdirp(HISTORY_DIR)
+except OSError:
+    print('\nWarning: Cannot create directory at `%s`. Command history will not be saved. Please check what was the environment property CQL_HISTORY set to.\n' % HISTORY_DIR)
+
+DEFAULT_CQLSHRC = os.path.expanduser(os.path.join('~', '.cassandra', 'cqlshrc'))
 
+if hasattr(options, 'cqlshrc'):
+    CONFIG_FILE = os.path.expanduser(options.cqlshrc)
+    if not os.path.exists(CONFIG_FILE):
+        print('\nWarning: Specified cqlshrc location `%s` does not exist.  Using `%s` instead.\n' % (CONFIG_FILE, DEFAULT_CQLSHRC))
+        CONFIG_FILE = DEFAULT_CQLSHRC
+else:
+    CONFIG_FILE = DEFAULT_CQLSHRC
+
+CQL_DIR = os.path.dirname(CONFIG_FILE)
 
 CQL_ERRORS = (
     cassandra.AlreadyExists, cassandra.AuthenticationFailed, cassandra.CoordinationFailure,
     cassandra.InvalidRequest, cassandra.Timeout, cassandra.Unauthorized, cassandra.OperationTimedOut,
     cassandra.cluster.NoHostAvailable,
     cassandra.connection.ConnectionBusy, cassandra.connection.ProtocolError, cassandra.connection.ConnectionException,
     cassandra.protocol.ErrorMessage, cassandra.protocol.InternalError, cassandra.query.TraceUnavailable
@@ -350,23 +351,27 @@
         return 'Failed to %s %s : %s' \
                % (self.verb, what, self.err)
 
     def __repr__(self):
         return '<%s %s>' % (self.__class__.__name__, self.message())
 
 
+def maybe_ensure_text(val):
+    return str(val) if val else val
+
+
 class FormatError(DecodeError):
     verb = 'format'
 
 
 def full_cql_version(ver):
     while ver.count('.') < 2:
         ver += '.0'
     ver_parts = ver.split('-', 1) + ['']
-    vertuple = tuple(map(int, ver_parts[0].split('.')) + [ver_parts[1]])
+    vertuple = tuple(list(map(int, ver_parts[0].split('.'))) + [ver_parts[1]])
     return ver, vertuple
 
 
 def format_value(val, cqltype, encoding, addcolor=False, date_time_format=None,
                  float_precision=None, colormap=None, nullval=None):
     if isinstance(val, DecodeError):
         if addcolor:
@@ -411,114 +416,92 @@
     if hasattr(cassandra, 'deserializers'):
         del cassandra.deserializers.DesDateType
 
     # Return cassandra.cqltypes.EMPTY instead of None for empty values
     cassandra.cqltypes.CassandraType.support_empty_values = True
 
 
-class FrozenType(cassandra.cqltypes._ParameterizedType):
-    """
-    Needed until the bundled python driver adds FrozenType.
-    """
-    typename = "frozen"
-    num_subtypes = 1
-
-    @classmethod
-    def deserialize_safe(cls, byts, protocol_version):
-        subtype, = cls.subtypes
-        return subtype.from_binary(byts)
-
-    @classmethod
-    def serialize_safe(cls, val, protocol_version):
-        subtype, = cls.subtypes
-        return subtype.to_binary(val, protocol_version)
-
-
 class Shell(cmd.Cmd):
     custom_prompt = os.getenv('CQLSH_PROMPT', '')
-    if custom_prompt is not '':
+    if custom_prompt != '':
         custom_prompt += "\n"
     default_prompt = custom_prompt + "cqlsh> "
     continue_prompt = "   ... "
-    keyspace_prompt = custom_prompt + "cqlsh:%s> "
-    keyspace_continue_prompt = "%s    ... "
+    keyspace_prompt = custom_prompt + "cqlsh:{}> "
+    keyspace_continue_prompt = "{}    ... "
     show_line_nums = False
     debug = False
+    coverage = False
+    coveragerc_path = None
     stop = False
     last_hist = None
     shunted_query_out = None
     use_paging = True
 
     default_page_size = 100
 
     def __init__(self, hostname, port, color=False,
-                 username=None, password=None, encoding=None, stdin=None, tty=True,
+                 username=None, encoding=None, stdin=None, tty=True,
                  completekey=DEFAULT_COMPLETEKEY, browser=None, use_conn=None,
                  cqlver=None, keyspace=None,
                  tracing_enabled=False, expand_enabled=False,
-                 no_compact=False,
                  display_nanotime_format=DEFAULT_NANOTIME_FORMAT,
                  display_timestamp_format=DEFAULT_TIMESTAMP_FORMAT,
                  display_date_format=DEFAULT_DATE_FORMAT,
                  display_float_precision=DEFAULT_FLOAT_PRECISION,
                  display_double_precision=DEFAULT_DOUBLE_PRECISION,
                  display_timezone=None,
                  max_trace_wait=DEFAULT_MAX_TRACE_WAIT,
                  ssl=False,
                  single_statement=None,
                  request_timeout=DEFAULT_REQUEST_TIMEOUT_SECONDS,
                  protocol_version=None,
-                 connect_timeout=DEFAULT_CONNECT_TIMEOUT_SECONDS):
+                 connect_timeout=DEFAULT_CONNECT_TIMEOUT_SECONDS,
+                 is_subshell=False,
+                 auth_provider=None):
         cmd.Cmd.__init__(self, completekey=completekey)
         self.hostname = hostname
         self.port = port
-        self.auth_provider = None
+        self.auth_provider = auth_provider
+        self.username = username
 
-        if hasattr(options, 'sigv4'):
-          my_session = boto3.session.Session()
-          self.auth_provider = SigV4AuthProvider(my_session)
-        elif hasattr(options, 'auth_provider_name'):
-          if options.auth_provider_name == 'SigV4AuthProvider':
-            my_session = boto3.session.Session()
-            self.auth_provider = SigV4AuthProvider(my_session)
-          elif options.auth_provider_name == DEFAULT_AUTH_PROVIDER:
-            if username:
-              if not password:
+        if isinstance(auth_provider, PlainTextAuthProvider):
+            self.username = auth_provider.username
+            if not auth_provider.password:
+                # if no password is provided, we need to query the user to get one.
                 password = getpass.getpass()
-              self.auth_provider = PlainTextAuthProvider(username=username, password=password)
-          else:
-              raise SyntaxError('cqlsh-expansion.py Invalid parameter for auth-provider. "%s" is not a valid AuthProvider' % (auth_provider,))
-        else:
-          if username:
-            if not password:
-               password = getpass.getpass()
-            self.auth_provider = PlainTextAuthProvider(username=username, password=password)
+                self.auth_provider = PlainTextAuthProvider(username=auth_provider.username, password=password)
 
-        self.username = username
         self.keyspace = keyspace
         self.ssl = ssl
         self.tracing_enabled = tracing_enabled
         self.page_size = self.default_page_size
         self.expand_enabled = expand_enabled
+        Keypsaces_profile = ExecutionProfile(
+            consistency_level=cassandra.ConsistencyLevel.LOCAL_QUORUM,
+            request_timeout=request_timeout,   
+            row_factory = ordered_dict_factory,
+            load_balancing_policy=WhiteListRoundRobinPolicy([self.hostname]))
+
         if use_conn:
             self.conn = use_conn
         else:
             kwargs = {}
             if protocol_version is not None:
                 kwargs['protocol_version'] = protocol_version
             self.conn = Cluster(contact_points=(self.hostname,), port=self.port, cql_version=cqlver,
                                 auth_provider=self.auth_provider,
-                                no_compact=no_compact,
                                 ssl_options=sslhandling.ssl_settings(hostname, CONFIG_FILE) if ssl else None,
-                                load_balancing_policy=WhiteListRoundRobinPolicy([self.hostname]),
                                 control_connection_timeout=connect_timeout,
-                                connect_timeout=connect_timeout,
+                                connect_timeout=connect_timeout, 
+                                execution_profiles={EXEC_PROFILE_DEFAULT: Keypsaces_profile},
                                 **kwargs)
         self.owns_connection = not use_conn
 
+
         if keyspace:
             self.session = self.conn.connect(keyspace)
         else:
             self.session = self.conn.connect()
 
         if browser == "":
             browser = None
@@ -530,70 +513,61 @@
         self.display_date_format = display_date_format
 
         self.display_float_precision = display_float_precision
         self.display_double_precision = display_double_precision
 
         self.display_timezone = display_timezone
 
-        self.session.default_timeout = request_timeout
-        self.session.row_factory = ordered_dict_factory
-        self.session.default_consistency_level = cassandra.ConsistencyLevel.ONE
+        ##### These configurations are moved to EXEC_PROFILE_DEFAULT
+        # self.session.default_timeout = request_timeout
+        # self.session.row_factory = ordered_dict_factory
+        # self.session.default_consistency_level = cassandra.ConsistencyLevel.ONE
+
         self.get_connection_versions()
         self.set_expanded_cql_version(self.connection_versions['cql'])
 
         self.current_keyspace = keyspace
 
         self.max_trace_wait = max_trace_wait
         self.session.max_trace_wait = max_trace_wait
 
         self.tty = tty
         self.encoding = encoding
-        self.check_windows_encoding()
 
         self.output_codec = codecs.lookup(encoding)
 
         self.statement = StringIO()
         self.lineno = 1
         self.in_comment = False
 
         self.prompt = ''
-
         if stdin is None:
             stdin = sys.stdin
 
         self.consistency_level = cassandra.ConsistencyLevel.ONE
         self.serial_consistency_level = cassandra.ConsistencyLevel.SERIAL
 
         if tty:
             self.reset_prompt()
             self.report_connection()
-            print 'Use HELP for help.'
+            print('Use HELP for help.')
             self.show_consistencylevel()
         else:
             self.show_line_nums = True
         self.stdin = stdin
         self.query_out = sys.stdout
 
         self.empty_lines = 0
         self.statement_error = False
         self.single_statement = single_statement
-
+        self.is_subshell = is_subshell
 
     @property
-    def is_using_utf8(self):
-        # utf8 encodings from https://docs.python.org/{2,3}/library/codecs.html
-        return self.encoding.replace('-', '_').lower() in ['utf', 'utf_8', 'u8', 'utf8', CP65001]
-
-    def check_windows_encoding(self):
-        if is_win and os.name == 'nt' and self.tty and \
-           self.is_using_utf8 and sys.stdout.encoding != CP65001:
-            self.printerr("\nWARNING: console codepage must be set to cp65001 "
-                          "to support {} encoding on Windows platforms.\n"
-                          "If you experience encoding problems, change your console"
-                          " codepage with 'chcp 65001' before starting cqlsh.\n".format(self.encoding))
+    def batch_mode(self):
+        return not self.tty
 
     def set_expanded_cql_version(self, ver):
         ver, vertuple = full_cql_version(ver)
         self.cql_version = ver
         self.cql_ver_tuple = vertuple
 
     def cqlver_atleast(self, major, minor=0, patch=0):
@@ -607,15 +581,15 @@
                                        date_format=self.display_date_format, nanotime_format=self.display_nanotime_format,
                                        timezone=self.display_timezone)
             precision = self.display_double_precision if cqltype is not None and cqltype.type_name == 'double' \
                 else self.display_float_precision
             return format_value(val, cqltype=cqltype, encoding=self.output_codec.name,
                                 addcolor=self.color, date_time_format=dtformats,
                                 float_precision=precision, **kwargs)
-        except Exception, e:
+        except Exception as e:
             err = FormatError(val, e)
             self.decoding_errors.append(err)
             return format_value(err, cqltype=cqltype, encoding=self.output_codec.name, addcolor=self.color)
 
     def myformat_colname(self, name, table_meta=None):
         column_colors = COLUMN_NAME_COLORS.copy()
         # check column role and color appropriately
@@ -629,130 +603,121 @@
         return self.myformat_value(name, colormap=column_colors)
 
     def report_connection(self):
         self.show_host()
         self.show_version()
 
     def show_host(self):
-        print "Connected to %s at %s:%d." % \
-            (self.applycolor(self.get_cluster_name(), BLUE),
-              self.hostname,
-              self.port)
-
+        print("Connected to {0} at {1}:{2}"
+              .format(self.applycolor(self.get_cluster_name(), BLUE),
+                      self.hostname,
+                      self.port))
+        
     def show_consistencylevel(self):
-        print 'cqlsh current consistency level is %s.' % \
-         (self.applycolor(cassandra.ConsistencyLevel.value_to_name[self.consistency_level], BLUE))
+        print ('cqlsh current consistency level is %s.' % \
+        self.applycolor(cassandra.ConsistencyLevel.value_to_name[self.consistency_level], BLUE))
 
 
     def show_version(self):
         vers = self.connection_versions.copy()
         vers['shver'] = version
         # system.Versions['cql'] apparently does not reflect changes with
         # set_cql_version.
         vers['cql'] = self.cql_version
-        print "[cqlsh %(shver)s | Cassandra %(build)s | CQL spec %(cql)s | Native protocol v%(protocol)s]" % vers
+        print("[cqlsh %(shver)s | Cassandra %(build)s | CQL spec %(cql)s | Native protocol v%(protocol)s]" % vers)
 
     def show_session(self, sessionid, partial_session=False):
         print_trace_session(self, self.session, sessionid, partial_session)
 
     def get_connection_versions(self):
         result, = self.session.execute("select * from system.local where key = 'local'")
         vers = {
             'build': result['release_version'],
+            'protocol': self.conn.protocol_version,
             'cql': result['cql_version'],
         }
-        vers['protocol'] = self.conn.protocol_version
         self.connection_versions = vers
 
-    def get_keyspace_names(self):
-        return map(str, self.conn.metadata.keyspaces.keys())
-
-    def get_columnfamily_names(self, ksname=None):
-        if ksname is None:
-            ksname = self.current_keyspace
-
-        return map(str, self.get_keyspace_meta(ksname).tables.keys())
-
     def get_materialized_view_names(self, ksname=None):
         if ksname is None:
             ksname = self.current_keyspace
 
-        return map(str, self.get_keyspace_meta(ksname).views.keys())
+        return list(self.get_keyspace_meta(ksname).views)
 
     def get_index_names(self, ksname=None):
         if ksname is None:
             ksname = self.current_keyspace
 
-        return map(str, self.get_keyspace_meta(ksname).indexes.keys())
+        return list(self.get_keyspace_meta(ksname).indexes)
 
     def get_column_names(self, ksname, cfname):
         if ksname is None:
             ksname = self.current_keyspace
         layout = self.get_table_meta(ksname, cfname)
-        return [unicode(col) for col in layout.columns]
+        return list(layout.columns)
 
     def get_usertype_names(self, ksname=None):
         if ksname is None:
             ksname = self.current_keyspace
 
-        return self.get_keyspace_meta(ksname).user_types.keys()
+        return list(self.get_keyspace_meta(ksname).user_types)
 
     def get_usertype_layout(self, ksname, typename):
         if ksname is None:
             ksname = self.current_keyspace
 
         ks_meta = self.get_keyspace_meta(ksname)
 
         try:
             user_type = ks_meta.user_types[typename]
         except KeyError:
-            raise UserTypeNotFound("User type %r not found" % typename)
+            raise UserTypeNotFound("User type {!r} not found".format(typename))
 
-        return zip(user_type.field_names, user_type.field_types)
+        return list(zip(user_type.field_names, user_type.field_types))
 
     def get_userfunction_names(self, ksname=None):
         if ksname is None:
             ksname = self.current_keyspace
 
-        return map(lambda f: f.name, self.get_keyspace_meta(ksname).functions.values())
+        return [f.name for f in list(self.get_keyspace_meta(ksname).functions.values())]
 
     def get_useraggregate_names(self, ksname=None):
         if ksname is None:
             ksname = self.current_keyspace
 
-        return map(lambda f: f.name, self.get_keyspace_meta(ksname).aggregates.values())
+        return [f.name for f in list(self.get_keyspace_meta(ksname).aggregates.values())]
 
     def get_cluster_name(self):
         return self.conn.metadata.cluster_name
 
     def get_partitioner(self):
         return self.conn.metadata.partitioner
 
     def get_keyspace_meta(self, ksname):
-        if ksname not in self.conn.metadata.keyspaces:
-            raise KeyspaceNotFound('Keyspace %r not found.' % ksname)
-        return self.conn.metadata.keyspaces[ksname]
+        if ksname in self.conn.metadata.keyspaces:
+            return self.conn.metadata.keyspaces[ksname]
+
+        raise KeyspaceNotFound('Keyspace %r not found.' % ksname)
 
     def get_keyspaces(self):
-        return self.conn.metadata.keyspaces.values()
+        return list(self.conn.metadata.keyspaces.values())
 
     def get_ring(self, ks):
         self.conn.metadata.token_map.rebuild_keyspace(ks, build_if_absent=True)
         return self.conn.metadata.token_map.tokens_to_hosts_by_ks[ks]
 
     def get_table_meta(self, ksname, tablename):
         if ksname is None:
             ksname = self.current_keyspace
         ksmeta = self.get_keyspace_meta(ksname)
-
         if tablename not in ksmeta.tables:
             if ksname == 'system_auth' and tablename in ['roles', 'role_permissions']:
                 self.get_fake_auth_table_meta(ksname, tablename)
             else:
-                raise ColumnFamilyNotFound("Column family %r not found" % tablename)
+                raise ColumnFamilyNotFound("Column family {} not found".format(tablename))
         else:
             return ksmeta.tables[tablename]
 
     def get_fake_auth_table_meta(self, ksname, tablename):
         # may be using external auth implementation so internal tables
         # aren't actually defined in schema. In this case, we'll fake
         # them up
@@ -765,41 +730,41 @@
         elif tablename == 'role_permissions':
             ks_meta = KeyspaceMetadata(ksname, True, None, None)
             table_meta = TableMetadata(ks_meta, 'role_permissions')
             table_meta.columns['role'] = ColumnMetadata(table_meta, 'role', cassandra.cqltypes.UTF8Type)
             table_meta.columns['resource'] = ColumnMetadata(table_meta, 'resource', cassandra.cqltypes.UTF8Type)
             table_meta.columns['permission'] = ColumnMetadata(table_meta, 'permission', cassandra.cqltypes.UTF8Type)
         else:
-            raise ColumnFamilyNotFound("Column family %r not found" % tablename)
+            raise ColumnFamilyNotFound("Column family {} not found".format(tablename))
 
     def get_index_meta(self, ksname, idxname):
         if ksname is None:
             ksname = self.current_keyspace
         ksmeta = self.get_keyspace_meta(ksname)
 
         if idxname not in ksmeta.indexes:
-            raise IndexNotFound("Index %r not found" % idxname)
+            raise IndexNotFound("Index {} not found".format(idxname))
 
         return ksmeta.indexes[idxname]
 
     def get_view_meta(self, ksname, viewname):
         if ksname is None:
             ksname = self.current_keyspace
         ksmeta = self.get_keyspace_meta(ksname)
 
         if viewname not in ksmeta.views:
-            raise MaterializedViewNotFound("Materialized view %r not found" % viewname)
+            raise MaterializedViewNotFound("Materialized view '{}' not found".format(viewname))
         return ksmeta.views[viewname]
 
     def get_object_meta(self, ks, name):
         if name is None:
             if ks and ks in self.conn.metadata.keyspaces:
                 return self.conn.metadata.keyspaces[ks]
             elif self.current_keyspace is None:
-                raise ObjectNotFound("%r not found in keyspaces" % (ks))
+                raise ObjectNotFound("'{}' not found in keyspaces".format(ks))
             else:
                 name = ks
                 ks = self.current_keyspace
 
         if ks is None:
             ks = self.current_keyspace
 
@@ -808,87 +773,93 @@
         if name in ksmeta.tables:
             return ksmeta.tables[name]
         elif name in ksmeta.indexes:
             return ksmeta.indexes[name]
         elif name in ksmeta.views:
             return ksmeta.views[name]
 
-        raise ObjectNotFound("%r not found in keyspace %r" % (name, ks))
-
-    def get_usertypes_meta(self):
-        data = self.session.execute("select * from system.schema_usertypes")
-        if not data:
-            return cql3handling.UserTypesMeta({})
-
-        return cql3handling.UserTypesMeta.from_layout(data)
+        raise ObjectNotFound("'{}' not found in keyspace '{}'".format(name, ks))
 
     def get_trigger_names(self, ksname=None):
         if ksname is None:
             ksname = self.current_keyspace
 
         return [trigger.name
-                for table in self.get_keyspace_meta(ksname).tables.values()
-                for trigger in table.triggers.values()]
+                for table in list(self.get_keyspace_meta(ksname).tables.values())
+                for trigger in list(table.triggers.values())]
 
     def reset_statement(self):
         self.reset_prompt()
         self.statement.truncate(0)
+        self.statement.seek(0)
         self.empty_lines = 0
 
     def reset_prompt(self):
         if self.current_keyspace is None:
             self.set_prompt(self.default_prompt, True)
         else:
-            self.set_prompt(self.keyspace_prompt % self.current_keyspace, True)
+            self.set_prompt(self.keyspace_prompt.format(self.current_keyspace), True)
 
     def set_continue_prompt(self):
         if self.empty_lines >= 3:
             self.set_prompt("Statements are terminated with a ';'.  You can press CTRL-C to cancel an incomplete statement.")
             self.empty_lines = 0
             return
         if self.current_keyspace is None:
             self.set_prompt(self.continue_prompt)
         else:
             spaces = ' ' * len(str(self.current_keyspace))
-            self.set_prompt(self.keyspace_continue_prompt % spaces)
+            self.set_prompt(self.keyspace_continue_prompt.format(spaces))
         self.empty_lines = self.empty_lines + 1 if not self.lastcmd else 0
 
     @contextmanager
     def prepare_loop(self):
         readline = None
         if self.tty and self.completekey:
             try:
                 import readline
             except ImportError:
-                if is_win:
-                    print "WARNING: pyreadline dependency missing.  Install to enable tab completion."
                 pass
             else:
                 old_completer = readline.get_completer()
                 readline.set_completer(self.complete)
                 if readline.__doc__ is not None and 'libedit' in readline.__doc__:
                     readline.parse_and_bind("bind -e")
                     readline.parse_and_bind("bind '" + self.completekey + "' rl_complete")
                     readline.parse_and_bind("bind ^R em-inc-search-prev")
                 else:
                     readline.parse_and_bind(self.completekey + ": complete")
+        # start coverage collection if requested, unless in subshell
+        if self.coverage and not self.is_subshell:
+            # check for coveragerc file, write it if missing
+            if os.path.exists(CQL_DIR):
+                self.coveragerc_path = os.path.join(CQL_DIR, '.coveragerc')
+                covdata_path = os.path.join(CQL_DIR, '.coverage')
+                if not os.path.isfile(self.coveragerc_path):
+                    with open(self.coveragerc_path, 'w') as f:
+                        f.writelines(["[run]\n",
+                                      "concurrency = multiprocessing\n",
+                                      "data_file = {}\n".format(covdata_path),
+                                      "parallel = true\n"]
+                                     )
+                # start coverage
+                import coverage
+                self.cov = coverage.Coverage(config_file=self.coveragerc_path)
+                self.cov.start()
         try:
             yield
         finally:
             if readline is not None:
                 readline.set_completer(old_completer)
+            if self.coverage and not self.is_subshell:
+                self.stop_coverage()
 
     def get_input_line(self, prompt=''):
         if self.tty:
-            try:
-                self.lastcmd = raw_input(prompt).decode(self.encoding)
-            except UnicodeDecodeError:
-                self.lastcmd = ''
-                traceback.print_exc()
-                self.check_windows_encoding()
+            self.lastcmd = input(str(prompt))
             line = self.lastcmd + '\n'
         else:
             self.lastcmd = self.stdin.readline()
             line = self.lastcmd
             if not len(line):
                 raise EOFError
         self.lineno += 1
@@ -901,15 +872,15 @@
                 newline = self.get_input_line(prompt=prompt)
             except EOFError:
                 return
             if newline == until:
                 return
             yield newline
 
-    def cmdloop(self):
+    def cmdloop(self, intro=None):
         """
         Adapted from cmd.Cmd's version, because there is literally no way with
         cmd.Cmd.cmdloop() to tell the difference between "EOF" showing up in
         input and an actual EOF.
         """
         with self.prepare_loop():
             while not self.stop:
@@ -920,74 +891,91 @@
                     else:
                         line = self.get_input_line(self.prompt)
                     self.statement.write(line)
                     if self.onecmd(self.statement.getvalue()):
                         self.reset_statement()
                 except EOFError:
                     self.handle_eof()
-                except CQL_ERRORS, cqlerr:
-                    self.printerr(cqlerr.message.decode(encoding='utf-8'))
+                except CQL_ERRORS as cqlerr:
+                    self.printerr(cqlerr.message)
                 except KeyboardInterrupt:
                     self.reset_statement()
-                    print
+                    print('')
+
+    def strip_comment_blocks(self, statementtext):
+        comment_block_in_literal_string = re.search('["].*[/][*].*[*][/].*["]', statementtext)
+        if not comment_block_in_literal_string:
+            result = re.sub('[/][*].*[*][/]', "", statementtext)
+            if '*/' in result and '/*' not in result and not self.in_comment:
+                raise SyntaxError("Encountered comment block terminator without being in comment block")
+            if '/*' in result:
+                result = re.sub('[/][*].*', "", result)
+                self.in_comment = True
+            if '*/' in result:
+                result = re.sub('.*[*][/]', "", result)
+                self.in_comment = False
+            if self.in_comment and not re.findall('[/][*]|[*][/]', statementtext):
+                result = ''
+            return result
+        return statementtext
 
     def onecmd(self, statementtext):
         """
         Returns true if the statement is complete and was handled (meaning it
         can be reset).
         """
-
+        statementtext = self.strip_comment_blocks(statementtext)
         try:
             statements, endtoken_escaped = cqlruleset.cql_split_statements(statementtext)
-        except pylexotron.LexingError, e:
+        except pylexotron.LexingError as e:
             if self.show_line_nums:
-                self.printerr('Invalid syntax at char %d' % (e.charnum,))
+                self.printerr('Invalid syntax at line {0}, char {1}'
+                              .format(e.linenum, e.charnum))
             else:
-                self.printerr('Invalid syntax at line %d, char %d'
-                              % (e.linenum, e.charnum))
+                self.printerr('Invalid syntax at char {0}'.format(e.charnum))
             statementline = statementtext.split('\n')[e.linenum - 1]
-            self.printerr('  %s' % statementline)
-            self.printerr(' %s^' % (' ' * e.charnum))
+            self.printerr('  {0}'.format(statementline))
+            self.printerr(' {0}^'.format(' ' * e.charnum))
             return True
 
         while statements and not statements[-1]:
             statements = statements[:-1]
         if not statements:
             return True
         if endtoken_escaped or statements[-1][-1][0] != 'endtoken':
             self.set_continue_prompt()
             return
         for st in statements:
             try:
                 self.handle_statement(st, statementtext)
-            except Exception, e:
+            except Exception as e:
                 if self.debug:
                     traceback.print_exc()
                 else:
                     self.printerr(e)
         return True
 
     def handle_eof(self):
         if self.tty:
-            print
+            print('')
         statement = self.statement.getvalue()
         if statement.strip():
             if not self.onecmd(statement):
                 self.printerr('Incomplete statement at end of file')
         self.do_exit()
 
     def handle_statement(self, tokens, srcstr):
         # Concat multi-line statements and insert into history
         if readline is not None:
             nl_count = srcstr.count("\n")
 
             new_hist = srcstr.replace("\n", " ").rstrip()
 
             if nl_count > 1 and self.last_hist != new_hist:
-                readline.add_history(new_hist.encode(self.encoding))
+                readline.add_history(new_hist)
 
             self.last_hist = new_hist
         cmdword = tokens[0][1]
         if cmdword == '?':
             cmdword = 'help'
         custom_handler = getattr(self, 'do_' + cmdword.lower(), None)
         if custom_handler:
@@ -1043,15 +1031,15 @@
                     for trace in future.get_all_query_traces(max_wait_per=self.max_trace_wait, query_cl=self.consistency_level):
                         print_trace(self, trace)
                 except TraceUnavailable:
                     msg = "Statement trace did not complete within %d seconds; trace data may be incomplete." % (self.session.max_trace_wait,)
                     self.writeresult(msg, color=RED)
                     for trace_id in future.get_query_trace_ids():
                         self.show_session(trace_id, partial_session=True)
-                except Exception, err:
+                except Exception as err:
                     self.printerr("Unable to fetch query trace: %s" % (str(err),))
 
         return success
 
     def parse_for_select_meta(self, query_string):
         try:
             parsed = cqlruleset.cql_parse(query_string)[1]
@@ -1061,15 +1049,15 @@
         name = self.cql_unprotect_name(parsed.get_binding('cfname', None))
         try:
             return self.get_table_meta(ks, name)
         except ColumnFamilyNotFound:
             try:
                 return self.get_view_meta(ks, name)
             except MaterializedViewNotFound:
-                raise ObjectNotFound("%r not found in keyspace %r" % (name, ks))
+                raise ObjectNotFound("'{}' not found in keyspace '{}'".format(name, ks))
 
     def parse_for_update_meta(self, query_string):
         try:
             parsed = cqlruleset.cql_parse(query_string)[1]
         except IndexError:
             return None
         ks = self.cql_unprotect_name(parsed.get_binding('ksname', None))
@@ -1080,16 +1068,17 @@
         if not statement:
             return False, None
 
         future = self.session.execute_async(statement, trace=self.tracing_enabled)
         result = None
         try:
             result = future.result()
-        except CQL_ERRORS, err:
-            self.printerr(unicode(err.__class__.__name__) + u": " + err.message.decode(encoding='utf-8'))
+        except CQL_ERRORS as err:
+            err_msg = err.message if hasattr(err, 'message') else str(err)
+            self.printerr(str(err.__class__.__name__) + ": " + err_msg)
         except Exception:
             import traceback
             self.printerr(traceback.format_exc())
 
         # Even if statement failed we try to refresh schema if not agreed (see CASSANDRA-9689)
         if not future.is_schema_agreed:
             try:
@@ -1107,101 +1096,113 @@
         elif statement.query_string.lower().startswith("list users") or statement.query_string.lower().startswith("list roles"):
             self.print_result(result, self.get_table_meta('system_auth', 'roles'))
         elif statement.query_string.lower().startswith("list"):
             self.print_result(result, self.get_table_meta('system_auth', 'role_permissions'))
         elif result:
             # CAS INSERT/UPDATE
             self.writeresult("")
-            self.print_static_result(result, self.parse_for_update_meta(statement.query_string))
+            self.print_static_result(result, self.parse_for_update_meta(statement.query_string), with_header=True, tty=self.tty)
         self.flush_output()
         return True, future
 
     def print_result(self, result, table_meta):
         self.decoding_errors = []
 
         self.writeresult("")
-        if result.has_more_pages and self.tty:
+
+        def print_all(result, table_meta, tty):
+            # Return the number of rows in total
             num_rows = 0
+            is_first = True
             while True:
-                if result.current_rows:
+                # Always print for the first page even it is empty
+                if result.current_rows or is_first:
+                    with_header = is_first or tty
+                    self.print_static_result(result, table_meta, with_header, tty, num_rows)
                     num_rows += len(result.current_rows)
-                    self.print_static_result(result, table_meta)
                 if result.has_more_pages:
-                    raw_input("---MORE---")
+                    if self.shunted_query_out is None and tty:
+                        # Only pause when not capturing.
+                        input("---MORE---")
                     result.fetch_next_page()
                 else:
+                    if not tty:
+                        self.writeresult("")
                     break
-        else:
-            num_rows = len(result.current_rows)
-            self.print_static_result(result, table_meta)
+                is_first = False
+            return num_rows
+
+        num_rows = print_all(result, table_meta, self.tty)
         self.writeresult("(%d rows)" % num_rows)
 
         if self.decoding_errors:
             for err in self.decoding_errors[:2]:
                 self.writeresult(err.message(), color=RED)
             if len(self.decoding_errors) > 2:
                 self.writeresult('%d more decoding errors suppressed.'
                                  % (len(self.decoding_errors) - 2), color=RED)
 
-    def print_static_result(self, result, table_meta):
+    def print_static_result(self, result, table_meta, with_header, tty, row_count_offset=0):
         if not result.column_names and not table_meta:
             return
 
-        column_names = result.column_names or table_meta.columns.keys()
+        column_names = result.column_names or list(table_meta.columns.keys())
         formatted_names = [self.myformat_colname(name, table_meta) for name in column_names]
         if not result.current_rows:
             # print header only
-            self.print_formatted_result(formatted_names, None)
+            self.print_formatted_result(formatted_names, None, with_header=True, tty=tty)
             return
 
         cql_types = []
         if result.column_types:
             ks_name = table_meta.keyspace_name if table_meta else self.current_keyspace
             ks_meta = self.conn.metadata.keyspaces.get(ks_name, None)
             cql_types = [CqlType(cql_typename(t), ks_meta) for t in result.column_types]
 
-        formatted_values = [map(self.myformat_value, [row[column] for column in column_names], cql_types) for row in result.current_rows]
+        formatted_values = [list(map(self.myformat_value, [row[c] for c in column_names], cql_types)) for row in result.current_rows]
 
         if self.expand_enabled:
-            self.print_formatted_result_vertically(formatted_names, formatted_values)
+            self.print_formatted_result_vertically(formatted_names, formatted_values, row_count_offset)
         else:
-            self.print_formatted_result(formatted_names, formatted_values)
+            self.print_formatted_result(formatted_names, formatted_values, with_header, tty)
 
-    def print_formatted_result(self, formatted_names, formatted_values):
+    def print_formatted_result(self, formatted_names, formatted_values, with_header, tty):
         # determine column widths
         widths = [n.displaywidth for n in formatted_names]
         if formatted_values is not None:
             for fmtrow in formatted_values:
                 for num, col in enumerate(fmtrow):
                     widths[num] = max(widths[num], col.displaywidth)
 
         # print header
-        header = ' | '.join(hdr.ljust(w, color=self.color) for (hdr, w) in zip(formatted_names, widths))
-        self.writeresult(' ' + header.rstrip())
-        self.writeresult('-%s-' % '-+-'.join('-' * w for w in widths))
+        if with_header:
+            header = ' | '.join(hdr.ljust(w, color=self.color) for (hdr, w) in zip(formatted_names, widths))
+            self.writeresult(' ' + header.rstrip())
+            self.writeresult('-%s-' % '-+-'.join('-' * w for w in widths))
 
         # stop if there are no rows
         if formatted_values is None:
             self.writeresult("")
             return
 
         # print row data
         for row in formatted_values:
             line = ' | '.join(col.rjust(w, color=self.color) for (col, w) in zip(row, widths))
             self.writeresult(' ' + line)
 
-        self.writeresult("")
+        if tty:
+            self.writeresult("")
 
-    def print_formatted_result_vertically(self, formatted_names, formatted_values):
+    def print_formatted_result_vertically(self, formatted_names, formatted_values, row_count_offset):
         max_col_width = max([n.displaywidth for n in formatted_names])
         max_val_width = max([n.displaywidth for row in formatted_values for n in row])
 
         # for each row returned, list all the column-value pairs
-        for row_id, row in enumerate(formatted_values):
-            self.writeresult("@ Row %d" % (row_id + 1))
+        for i, row in enumerate(formatted_values):
+            self.writeresult("@ Row %d" % (row_count_offset + i + 1))
             self.writeresult('-%s-' % '-+-'.join(['-' * max_col_width, '-' * max_val_width]))
             for field_id, field in enumerate(row):
                 column = formatted_names[field_id].ljust(max_col_width, color=self.color)
                 value = field.ljust(field.displaywidth, color=self.color)
                 self.writeresult(' ' + " | ".join([column, value]))
             self.writeresult('')
 
@@ -1246,229 +1247,37 @@
         begidx = readline.get_begidx() + len(prevlines)
         stuff_to_complete = wholestmt[:begidx]
         return cqlruleset.cql_complete(stuff_to_complete, text, cassandra_conn=self,
                                        debug=debug_completion, startsymbol='cqlshCommand')
 
     def set_prompt(self, prompt, prepend_user=False):
         if prepend_user and self.username:
-            self.prompt = "%s@%s" % (self.username, prompt)
+            self.prompt = "{0}@{1}".format(self.username, prompt)
             return
         self.prompt = prompt
 
     def cql_unprotect_name(self, namestr):
         if namestr is None:
             return
         return cqlruleset.dequote_name(namestr)
 
     def cql_unprotect_value(self, valstr):
         if valstr is not None:
             return cqlruleset.dequote_value(valstr)
 
-    def print_recreate_keyspace(self, ksdef, out):
-        out.write(ksdef.export_as_string())
-        out.write("\n")
-
-    def print_recreate_columnfamily(self, ksname, cfname, out):
-        """
-        Output CQL commands which should be pasteable back into a CQL session
-        to recreate the given table.
-
-        Writes output to the given out stream.
-        """
-        out.write(self.get_table_meta(ksname, cfname).export_as_string())
-        out.write("\n")
-
-    def print_recreate_index(self, ksname, idxname, out):
-        """
-        Output CQL commands which should be pasteable back into a CQL session
-        to recreate the given index.
-
-        Writes output to the given out stream.
-        """
-        out.write(self.get_index_meta(ksname, idxname).export_as_string())
-        out.write("\n")
-
-    def print_recreate_materialized_view(self, ksname, viewname, out):
-        """
-        Output CQL commands which should be pasteable back into a CQL session
-        to recreate the given materialized view.
-
-        Writes output to the given out stream.
-        """
-        out.write(self.get_view_meta(ksname, viewname).export_as_string())
-        out.write("\n")
-
-    def print_recreate_object(self, ks, name, out):
-        """
-        Output CQL commands which should be pasteable back into a CQL session
-        to recreate the given object (ks, table or index).
-
-        Writes output to the given out stream.
-        """
-        out.write(self.get_object_meta(ks, name).export_as_string())
-        out.write("\n")
-
-    def describe_keyspaces(self):
-        print
-        cmd.Cmd.columnize(self, protect_names(self.get_keyspace_names()))
-        print
-
-    def describe_keyspace(self, ksname):
-        print
-        self.print_recreate_keyspace(self.get_keyspace_meta(ksname), sys.stdout)
-        print
-
-    def describe_columnfamily(self, ksname, cfname):
-        if ksname is None:
-            ksname = self.current_keyspace
-        if ksname is None:
-            raise NoKeyspaceError("No keyspace specified and no current keyspace")
-        print
-        self.print_recreate_columnfamily(ksname, cfname, sys.stdout)
-        print
-
-    def describe_index(self, ksname, idxname):
-        print
-        self.print_recreate_index(ksname, idxname, sys.stdout)
-        print
-
-    def describe_materialized_view(self, ksname, viewname):
-        if ksname is None:
-            ksname = self.current_keyspace
-        if ksname is None:
-            raise NoKeyspaceError("No keyspace specified and no current keyspace")
-        print
-        self.print_recreate_materialized_view(ksname, viewname, sys.stdout)
-        print
-
-    def describe_object(self, ks, name):
-        print
-        self.print_recreate_object(ks, name, sys.stdout)
-        print
-
-    def describe_columnfamilies(self, ksname):
-        print
-        if ksname is None:
-            for k in self.get_keyspaces():
-                name = protect_name(k.name)
-                print 'Keyspace %s' % (name,)
-                print '---------%s' % ('-' * len(name))
-                cmd.Cmd.columnize(self, protect_names(self.get_columnfamily_names(k.name)))
-                print
-        else:
-            cmd.Cmd.columnize(self, protect_names(self.get_columnfamily_names(ksname)))
-            print
-
-    def describe_functions(self, ksname):
-        print
-        if ksname is None:
-            for ksmeta in self.get_keyspaces():
-                name = protect_name(ksmeta.name)
-                print 'Keyspace %s' % (name,)
-                print '---------%s' % ('-' * len(name))
-                self._columnize_unicode(ksmeta.functions.keys())
-        else:
-            ksmeta = self.get_keyspace_meta(ksname)
-            self._columnize_unicode(ksmeta.functions.keys())
-
-    def describe_function(self, ksname, functionname):
-        if ksname is None:
-            ksname = self.current_keyspace
-        if ksname is None:
-            raise NoKeyspaceError("No keyspace specified and no current keyspace")
-        print
-        ksmeta = self.get_keyspace_meta(ksname)
-        functions = filter(lambda f: f.name == functionname, ksmeta.functions.values())
-        if len(functions) == 0:
-            raise FunctionNotFound("User defined function %r not found" % functionname)
-        print "\n\n".join(func.export_as_string() for func in functions)
-        print
-
-    def describe_aggregates(self, ksname):
-        print
-        if ksname is None:
-            for ksmeta in self.get_keyspaces():
-                name = protect_name(ksmeta.name)
-                print 'Keyspace %s' % (name,)
-                print '---------%s' % ('-' * len(name))
-                self._columnize_unicode(ksmeta.aggregates.keys())
-        else:
-            ksmeta = self.get_keyspace_meta(ksname)
-            self._columnize_unicode(ksmeta.aggregates.keys())
-
-    def describe_aggregate(self, ksname, aggregatename):
-        if ksname is None:
-            ksname = self.current_keyspace
-        if ksname is None:
-            raise NoKeyspaceError("No keyspace specified and no current keyspace")
-        print
-        ksmeta = self.get_keyspace_meta(ksname)
-        aggregates = filter(lambda f: f.name == aggregatename, ksmeta.aggregates.values())
-        if len(aggregates) == 0:
-            raise FunctionNotFound("User defined aggregate %r not found" % aggregatename)
-        print "\n\n".join(aggr.export_as_string() for aggr in aggregates)
-        print
-
-    def describe_usertypes(self, ksname):
-        print
-        if ksname is None:
-            for ksmeta in self.get_keyspaces():
-                name = protect_name(ksmeta.name)
-                print 'Keyspace %s' % (name,)
-                print '---------%s' % ('-' * len(name))
-                self._columnize_unicode(ksmeta.user_types.keys(), quote=True)
-        else:
-            ksmeta = self.get_keyspace_meta(ksname)
-            self._columnize_unicode(ksmeta.user_types.keys(), quote=True)
-
-    def describe_usertype(self, ksname, typename):
-        if ksname is None:
-            ksname = self.current_keyspace
-        if ksname is None:
-            raise NoKeyspaceError("No keyspace specified and no current keyspace")
-        print
-        ksmeta = self.get_keyspace_meta(ksname)
-        try:
-            usertype = ksmeta.user_types[typename]
-        except KeyError:
-            raise UserTypeNotFound("User type %r not found" % typename)
-        print usertype.export_as_string()
-
-    def _columnize_unicode(self, name_list, quote=False):
+    def _columnize_unicode(self, name_list):
         """
         Used when columnizing identifiers that may contain unicode
         """
-        names = [n.encode('utf-8') for n in name_list]
-        if quote:
-            names = protect_names(names)
+        names = [n for n in name_list]
         cmd.Cmd.columnize(self, names)
-        print
-
-    def describe_cluster(self):
-        print '\nCluster: %s' % self.get_cluster_name()
-        p = trim_if_present(self.get_partitioner(), 'org.apache.cassandra.dht.')
-        print 'Partitioner: %s\n' % p
-        # TODO: snitch?
-        # snitch = trim_if_present(self.get_snitch(), 'org.apache.cassandra.locator.')
-        # print 'Snitch: %s\n' % snitch
-        if self.current_keyspace is not None and self.current_keyspace != 'system':
-            print "Range ownership:"
-            ring = self.get_ring(self.current_keyspace)
-            for entry in ring.items():
-                print ' %39s  [%s]' % (str(entry[0].value), ', '.join([host.address for host in entry[1]]))
-            print
-
-    def describe_schema(self, include_system=False):
-        print
-        for k in self.get_keyspaces():
-            if include_system or k.name not in cql3handling.SYSTEM_KEYSPACES:
-                self.print_recreate_keyspace(k, sys.stdout)
-                print
+        print('')
 
     def do_describe(self, parsed):
+
         """
         DESCRIBE [cqlsh only]
 
         (DESC may be used as a shorthand.)
 
           Outputs information about the connected Cassandra cluster, or about
           the data objects stored in the cluster. Use in one of the following ways:
@@ -1479,15 +1288,14 @@
 
         DESCRIBE KEYSPACE [<keyspacename>]
 
           Output CQL commands that could be used to recreate the given keyspace,
           and the objects in it (such as tables, types, functions, etc.).
           In some cases, as the CQL interface matures, there will be some metadata
           about a keyspace that is not representable with CQL. That metadata will not be shown.
-
           The '<keyspacename>' argument may be omitted, in which case the current
           keyspace will be described.
 
         DESCRIBE TABLES
 
           Output the names of all tables in the current keyspace, or in all
           keyspaces if there is no current keyspace.
@@ -1551,74 +1359,116 @@
           Output the CQL command that could be used to recreate the given user-defined-aggregate.
 
         DESCRIBE <objname>
 
           Output CQL commands that could be used to recreate the entire object schema,
           where object can be either a keyspace or a table or an index or a materialized
           view (in this order).
-  """
-        what = parsed.matched[1][1].lower()
-        if what == 'functions':
-            self.describe_functions(self.current_keyspace)
-        elif what == 'function':
-            ksname = self.cql_unprotect_name(parsed.get_binding('ksname', None))
-            functionname = self.cql_unprotect_name(parsed.get_binding('udfname'))
-            self.describe_function(ksname, functionname)
-        elif what == 'aggregates':
-            self.describe_aggregates(self.current_keyspace)
-        elif what == 'aggregate':
-            ksname = self.cql_unprotect_name(parsed.get_binding('ksname', None))
-            aggregatename = self.cql_unprotect_name(parsed.get_binding('udaname'))
-            self.describe_aggregate(ksname, aggregatename)
-        elif what == 'keyspaces':
-            self.describe_keyspaces()
-        elif what == 'keyspace':
-            ksname = self.cql_unprotect_name(parsed.get_binding('ksname', ''))
-            if not ksname:
-                ksname = self.current_keyspace
-                if ksname is None:
-                    self.printerr('Not in any keyspace.')
-                    return
-            self.describe_keyspace(ksname)
-        elif what in ('columnfamily', 'table'):
-            ks = self.cql_unprotect_name(parsed.get_binding('ksname', None))
-            cf = self.cql_unprotect_name(parsed.get_binding('cfname'))
-            self.describe_columnfamily(ks, cf)
-        elif what == 'index':
-            ks = self.cql_unprotect_name(parsed.get_binding('ksname', None))
-            idx = self.cql_unprotect_name(parsed.get_binding('idxname', None))
-            self.describe_index(ks, idx)
-        elif what == 'materialized' and parsed.matched[2][1].lower() == 'view':
-            ks = self.cql_unprotect_name(parsed.get_binding('ksname', None))
-            mv = self.cql_unprotect_name(parsed.get_binding('mvname'))
-            self.describe_materialized_view(ks, mv)
-        elif what in ('columnfamilies', 'tables'):
-            self.describe_columnfamilies(self.current_keyspace)
-        elif what == 'types':
-            self.describe_usertypes(self.current_keyspace)
-        elif what == 'type':
-            ks = self.cql_unprotect_name(parsed.get_binding('ksname', None))
-            ut = self.cql_unprotect_name(parsed.get_binding('utname'))
-            self.describe_usertype(ks, ut)
-        elif what == 'cluster':
-            self.describe_cluster()
-        elif what == 'schema':
-            self.describe_schema(False)
-        elif what == 'full' and parsed.matched[2][1].lower() == 'schema':
-            self.describe_schema(True)
-        elif what:
-            ks = self.cql_unprotect_name(parsed.get_binding('ksname', None))
-            name = self.cql_unprotect_name(parsed.get_binding('cfname'))
-            if not name:
-                name = self.cql_unprotect_name(parsed.get_binding('idxname', None))
-            if not name:
-                name = self.cql_unprotect_name(parsed.get_binding('mvname', None))
-            self.describe_object(ks, name)
+        """
+        """ 
+            For cqlsh > 6.0 DESCRIBE|DESC was moved to server side in Cassandra 4.0. As a consequence DESRIBE|DESC
+            will not work in cqlsh connected to Cassandra < 4.0.In cqlsh-expansion we have modified code to support describe statements for 
+            Cassandra 3.11  
+        """
+        stmt = SimpleStatement(parsed.extract_orig(), consistency_level=cassandra.ConsistencyLevel.LOCAL_ONE, fetch_size=self.page_size if self.use_paging else None)
+        future = self.session.execute_async(stmt)
+
+        if self.connection_versions['build'][0] < '4':
+            do_describe_3x(self, parsed)
+        else:
+            try:
+                result = future.result()
+                what = parsed.matched[1][1].lower()
+
+                if what in ('columnfamilies', 'tables', 'types', 'functions', 'aggregates'):
+                    self.describe_list(result)
+                elif what == 'keyspaces':
+                    self.describe_keyspaces(result)
+                elif what == 'cluster':
+                    self.describe_cluster(result)
+                elif what:
+                    self.describe_element(result)
+
+            except CQL_ERRORS as err:
+                err_msg = err.message if hasattr(err, 'message') else str(err)
+                self.printerr(err_msg.partition("message=")[2].strip('"'))
+            except Exception:
+                import traceback
+                self.printerr(traceback.format_exc())
+
+            if future:
+                if future.warnings:
+                    self.print_warnings(future.warnings)
+
+
     do_desc = do_describe
 
+    def describe_keyspaces(self, rows):
+        """
+        Print the output for a DESCRIBE KEYSPACES query
+        """
+        names = [r['name'] for r in rows]
+
+        print('')
+        cmd.Cmd.columnize(self, names)
+        print('')  
+    
+    def describe_list(self, rows):
+        """
+        Print the output for all the DESCRIBE queries for element names (e.g DESCRIBE TABLES, DESCRIBE FUNCTIONS ...)
+        """
+        keyspace = None
+        names = list()
+        for row in rows:
+            if row['keyspace_name'] != keyspace:
+                if keyspace is not None:
+                    self.print_keyspace_element_names(keyspace, names)
+
+                keyspace = row['keyspace_name']
+                names = list()
+
+            names.append(str(row['name']))
+
+        if keyspace is not None:
+            self.print_keyspace_element_names(keyspace, names)
+            print('')
+
+    def print_keyspace_element_names(self, keyspace, names):
+        print('')
+        if self.current_keyspace is None:
+            print('Keyspace %s' % (keyspace))
+            print('---------%s' % ('-' * len(keyspace)))
+        cmd.Cmd.columnize(self, names)
+
+    def describe_element(self, rows):
+        """
+        Print the output for all the DESCRIBE queries where an element name as been specified (e.g DESCRIBE TABLE, DESCRIBE INDEX ...)
+        """
+        for row in rows:
+            print('')
+            self.query_out.write(row['create_statement'])
+            print('')
+
+    def describe_cluster(self, rows):
+        """
+        Print the output for a DESCRIBE CLUSTER query.
+
+        If a specified keyspace was in use the returned ResultSet will contains a 'range_ownership' column,
+        otherwise not.
+        """
+        for row in rows:
+            print('\nCluster: %s' % row['cluster'])
+            print('Partitioner: %s' % row['partitioner'])
+            print('Snitch: %s\n' % row['snitch'])
+            if 'range_ownership' in row:
+                print("Range ownership:")
+                for entry in list(row['range_ownership'].items()):
+                    print(' %39s  [%s]' % (entry[0], ', '.join([host for host in entry[1]])))
+                print('')
+    
     def do_copy(self, parsed):
         r"""
         COPY [cqlsh only]
 
           COPY x FROM: Imports CSV data into a Cassandra table
           COPY x TO: Exports data from a Cassandra table in CSV format.
 
@@ -1692,48 +1542,47 @@
                                      -1 means unlimited.
           FLOATPRECISION=5         - the number of digits displayed after the decimal point for cql float values
           DOUBLEPRECISION=12       - the number of digits displayed after the decimal point for cql double values
 
         When entering CSV data on STDIN, you can use the sequence "\."
         on a line by itself to end the data input.
         """
-
         ks = self.cql_unprotect_name(parsed.get_binding('ksname', None))
         if ks is None:
             ks = self.current_keyspace
             if ks is None:
                 raise NoKeyspaceError("Not in any keyspace.")
         table = self.cql_unprotect_name(parsed.get_binding('cfname'))
         columns = parsed.get_binding('colnames', None)
         if columns is not None:
-            columns = map(self.cql_unprotect_name, columns)
+            columns = list(map(self.cql_unprotect_name, columns))
         else:
             # default to all known columns
             columns = self.get_column_names(ks, table)
 
         fname = parsed.get_binding('fname', None)
         if fname is not None:
             fname = self.cql_unprotect_value(fname)
 
-        copyoptnames = map(str.lower, parsed.get_binding('optnames', ()))
-        copyoptvals = map(self.cql_unprotect_value, parsed.get_binding('optvals', ()))
-        opts = dict(zip(copyoptnames, copyoptvals))
+        copyoptnames = list(map(str.lower, parsed.get_binding('optnames', ())))
+        copyoptvals = list(map(self.cql_unprotect_value, parsed.get_binding('optvals', ())))
+        opts = dict(list(zip(copyoptnames, copyoptvals)))
 
         direction = parsed.get_binding('dir').upper()
         if direction == 'FROM':
             self.show_consistencylevel()
             if self.consistency_level != cassandra.ConsistencyLevel.LOCAL_QUORUM:
-               raise SyntaxError("cqlsh-expansion.py 'COPY FROM' requires LOCAL_QUORUM consistency for writes")
+               raise SyntaxError("cqlsh-expansion.py 'COPY FROM' requires LOCAL_QUORUM consistency for writes")      
             task = ImportTask(self, ks, table, columns, fname, opts, self.conn.protocol_version, CONFIG_FILE)
         elif direction == 'TO':
             self.show_consistencylevel()
             if self.consistency_level != cassandra.ConsistencyLevel.LOCAL_QUORUM and \
             self.consistency_level != cassandra.ConsistencyLevel.LOCAL_ONE and \
             self.consistency_level != cassandra.ConsistencyLevel.ONE:
-               raise SyntaxError("cqlsh-expansion.py 'COPY TO' requires ONE, LOCAL_ONE, or LOCAL_QUORUM consistency for reads")
+               raise SyntaxError("cqlsh-expansion.py 'COPY TO' requires ONE, LOCAL_ONE, or LOCAL_QUORUM consistency for reads")            
             task = ExportTask(self, ks, table, columns, fname, opts, self.conn.protocol_version, CONFIG_FILE)
         else:
             raise SyntaxError("Unknown direction %s" % direction)
 
         task.run()
 
     def do_show(self, parsed):
@@ -1742,16 +1591,16 @@
 
           Displays information about the current cqlsh session. Can be called in
           the following ways:
 
         SHOW VERSION
 
           Shows the version and build of the connected Cassandra instance, as
-          well as the versions of the CQL spec and the Thrift protocol that
-          the connected Cassandra instance understands.
+          well as the version of the CQL spec that the connected Cassandra
+          instance understands.
 
         SHOW HOST
 
           Shows where cqlsh is currently connected.
 
         SHOW SESSION <sessionid>
 
@@ -1791,34 +1640,37 @@
         """
         fname = parsed.get_binding('fname')
         fname = os.path.expanduser(self.cql_unprotect_value(fname))
         try:
             encoding, bom_size = get_file_encoding_bomsize(fname)
             f = codecs.open(fname, 'r', encoding)
             f.seek(bom_size)
-        except IOError, e:
+        except IOError as e:
             self.printerr('Could not open %r: %s' % (fname, e))
             return
-        username = self.auth_provider.username if self.auth_provider else None
-        password = self.auth_provider.password if self.auth_provider else None
         subshell = Shell(self.hostname, self.port, color=self.color,
-                         username=username, password=password,
+                         username=self.username,
                          encoding=self.encoding, stdin=f, tty=False, use_conn=self.conn,
                          cqlver=self.cql_version, keyspace=self.current_keyspace,
                          tracing_enabled=self.tracing_enabled,
                          display_nanotime_format=self.display_nanotime_format,
                          display_timestamp_format=self.display_timestamp_format,
                          display_date_format=self.display_date_format,
                          display_float_precision=self.display_float_precision,
                          display_double_precision=self.display_double_precision,
                          display_timezone=self.display_timezone,
                          max_trace_wait=self.max_trace_wait, ssl=self.ssl,
                          request_timeout=self.session.default_timeout,
                          connect_timeout=self.conn.connect_timeout,
+                         is_subshell=True,
                          auth_provider=self.auth_provider)
+        # duplicate coverage related settings in subshell
+        if self.coverage:
+            subshell.coverage = True
+            subshell.coveragerc_path = self.coveragerc_path
         subshell.cmdloop()
         f.close()
 
     def do_capture(self, parsed):
         """
         CAPTURE [cqlsh only]
 
@@ -1844,17 +1696,17 @@
 
         To inspect the current capture configuration, use CAPTURE with no
         arguments.
         """
         fname = parsed.get_binding('fname')
         if fname is None:
             if self.shunted_query_out is not None:
-                print "Currently capturing query output to %r." % (self.query_out.name,)
+                print("Currently capturing query output to %r." % (self.query_out.name,))
             else:
-                print "Currently not capturing query output."
+                print("Currently not capturing query output.")
             return
 
         if fname.upper() == 'OFF':
             if self.shunted_query_out is None:
                 self.printerr('Not currently capturing output.')
                 return
             self.query_out.close()
@@ -1868,22 +1720,22 @@
             self.printerr('Already capturing output to %s. Use CAPTURE OFF'
                           ' to disable.' % (self.query_out.name,))
             return
 
         fname = os.path.expanduser(self.cql_unprotect_value(fname))
         try:
             f = open(fname, 'a')
-        except IOError, e:
+        except IOError as e:
             self.printerr('Could not open %r for append: %s' % (fname, e))
             return
         self.shunted_query_out = self.query_out
         self.shunted_color = self.color
         self.query_out = f
         self.color = False
-        print 'Now capturing query output to %r.' % (fname,)
+        print('Now capturing query output to %r.' % (fname,))
 
     def do_tracing(self, parsed):
         """
         TRACING [cqlsh]
 
           Enables or disables request tracing.
 
@@ -1939,19 +1791,19 @@
 
         CONSISTENCY
 
            CONSISTENCY with no arguments shows the current consistency level.
         """
         level = parsed.get_binding('level')
         if level is None:
-            print 'Current consistency level is %s.' % (cassandra.ConsistencyLevel.value_to_name[self.consistency_level])
+            print('Current consistency level is %s.' % (cassandra.ConsistencyLevel.value_to_name[self.consistency_level]))
             return
 
         self.consistency_level = cassandra.ConsistencyLevel.name_to_value[level.upper()]
-        print 'Consistency level set to %s.' % (level.upper(),)
+        print('Consistency level set to %s.' % (level.upper(),))
 
     def do_serial(self, parsed):
         """
         SERIAL CONSISTENCY [cqlsh only]
 
            Overrides serial consistency level (default level is SERIAL).
 
@@ -1965,19 +1817,19 @@
 
         SERIAL CONSISTENCY
 
            SERIAL CONSISTENCY with no arguments shows the current consistency level.
         """
         level = parsed.get_binding('level')
         if level is None:
-            print 'Current serial consistency level is %s.' % (cassandra.ConsistencyLevel.value_to_name[self.serial_consistency_level])
+            print('Current serial consistency level is %s.' % (cassandra.ConsistencyLevel.value_to_name[self.serial_consistency_level]))
             return
 
         self.serial_consistency_level = cassandra.ConsistencyLevel.name_to_value[level.upper()]
-        print 'Serial consistency level set to %s.' % (level.upper(),)
+        print('Serial consistency level set to %s.' % (level.upper(),))
 
     def do_login(self, parsed):
         """
         LOGIN [cqlsh only]
 
            Changes login information without requiring restart.
 
@@ -2033,16 +1885,15 @@
 
     def do_clear(self, parsed):
         """
         CLEAR/CLS [cqlsh only]
 
         Clears the console.
         """
-        import subprocess
-        subprocess.call(['clear', 'cls'][is_win], shell=True)
+        subprocess.call('clear', shell=True)
     do_cls = do_clear
 
     def do_debug(self, parsed):
         import pdb
         pdb.set_trace()
 
     def get_help_topics(self):
@@ -2073,20 +1924,20 @@
             if t.lower() in self.get_help_topics():
                 doc = getattr(self, 'do_' + t.lower()).__doc__
                 self.stdout.write(doc + "\n")
             elif t.lower() in cqldocs.get_help_topics():
                 urlpart = cqldocs.get_help_topic(t)
                 if urlpart is not None:
                     url = "%s#%s" % (CASSANDRA_CQL_HTML, urlpart)
-                    if len(webbrowser._tryorder) == 0:
-                        self.printerr("*** No browser to display CQL help. URL for help topic %s : %s" % (t, url))
-                    elif self.browser is not None:
-                        webbrowser.get(self.browser).open_new_tab(url)
+                    if self.browser is not None:
+                        opened = webbrowser.get(self.browser).open_new_tab(url)
                     else:
-                        webbrowser.open_new_tab(url)
+                        opened = webbrowser.open_new_tab(url)
+                    if not opened:
+                        self.printerr("*** No browser to display CQL help. URL for help topic %s : %s" % (t, url))
             else:
                 self.printerr("*** No help on %s" % (t,))
 
     def do_unicode(self, parsed):
         """
         Textual input/output
 
@@ -2122,33 +1973,30 @@
           PAGING with no arguments shows the current query paging status.
         """
         (self.use_paging, requested_page_size) = SwitchCommandWithValue(
             "PAGING", "Query paging", value_type=int).execute(self.use_paging, parsed, self.printerr)
         if self.use_paging and requested_page_size is not None:
             self.page_size = requested_page_size
         if self.use_paging:
-            print("Page size: {}".format(self.page_size))
+            print(("Page size: {}".format(self.page_size)))
         else:
             self.page_size = self.default_page_size
 
     def applycolor(self, text, color=None):
         if not color or not self.color:
             return text
         return color + text + ANSI_RESET
 
     def writeresult(self, text, color=None, newline=True, out=None):
         if out is None:
             out = self.query_out
 
         # convert Exceptions, etc to text
-        if not isinstance(text, (unicode, str)):
-            text = unicode(text)
-
-        if isinstance(text, unicode):
-            text = text.encode(self.encoding)
+        if not isinstance(text, str):
+            text = str(text)
 
         to_write = self.applycolor(text, color) + ('\n' if newline else '')
         out.write(to_write)
 
     def flush_output(self):
         self.query_out.flush()
 
@@ -2156,47 +2004,53 @@
         self.statement_error = True
         if shownum is None:
             shownum = self.show_line_nums
         if shownum:
             text = '%s:%d:%s' % (self.stdin.name, self.lineno, text)
         self.writeresult(text, color, newline=newline, out=sys.stderr)
 
+    def stop_coverage(self):
+        if self.coverage and self.cov is not None:
+            self.cov.stop()
+            self.cov.save()
+            self.cov = None
+
 
 class SwitchCommand(object):
     command = None
     description = None
 
     def __init__(self, command, desc):
         self.command = command
         self.description = desc
 
     def execute(self, state, parsed, printerr):
         switch = parsed.get_binding('switch')
         if switch is None:
             if state:
-                print "%s is currently enabled. Use %s OFF to disable" \
-                      % (self.description, self.command)
+                print("%s is currently enabled. Use %s OFF to disable"
+                      % (self.description, self.command))
             else:
-                print "%s is currently disabled. Use %s ON to enable." \
-                      % (self.description, self.command)
+                print("%s is currently disabled. Use %s ON to enable."
+                      % (self.description, self.command))
             return state
 
         if switch.upper() == 'ON':
             if state:
                 printerr('%s is already enabled. Use %s OFF to disable.'
                          % (self.description, self.command))
                 return state
-            print 'Now %s is enabled' % (self.description,)
+            print('Now %s is enabled' % (self.description,))
             return True
 
         if switch.upper() == 'OFF':
             if not state:
                 printerr('%s is not enabled.' % (self.description,))
                 return state
-            print 'Disabled %s.' % (self.description,)
+            print('Disabled %s.' % (self.description,))
             return False
 
 
 class SwitchCommandWithValue(SwitchCommand):
     """The same as SwitchCommand except it also accepts a value in place of ON.
 
     This returns a tuple of the form: (SWITCH_VALUE, PASSED_VALUE)
@@ -2214,63 +2068,74 @@
         binary_switch_value = SwitchCommand.execute(self, state, parsed, printerr)
         switch = parsed.get_binding('switch')
         try:
             value = self.value_type(switch)
             binary_switch_value = True
         except (ValueError, TypeError):
             value = None
-        return (binary_switch_value, value)
+        return binary_switch_value, value
 
 
 def option_with_default(cparser_getter, section, option, default=None):
     try:
         return cparser_getter(section, option)
-    except ConfigParser.Error:
+    except configparser.Error:
         return default
 
 
 def raw_option_with_default(configs, section, option, default=None):
     """
     Same (almost) as option_with_default() but won't do any string interpolation.
     Useful for config values that include '%' symbol, e.g. time format string.
     """
     try:
         return configs.get(section, option, raw=True)
-    except ConfigParser.Error:
+    except configparser.Error:
         return default
 
 
 def should_use_color():
     if not sys.stdout.isatty():
         return False
     if os.environ.get('TERM', '') in ('dumb', ''):
         return False
     try:
-        import subprocess
         p = subprocess.Popen(['tput', 'colors'], stdout=subprocess.PIPE)
         stdout, _ = p.communicate()
         if int(stdout.strip()) < 8:
             return False
     except (OSError, ImportError, ValueError):
         # oh well, we tried. at least we know there's a $TERM and it's
         # not "dumb".
         pass
     return True
 
 
 def read_options(cmdlineargs, environment):
-    configs = ConfigParser.SafeConfigParser()
+    configs = configparser.ConfigParser()
     configs.read(CONFIG_FILE)
 
-    rawconfigs = ConfigParser.RawConfigParser()
+    rawconfigs = configparser.RawConfigParser()
     rawconfigs.read(CONFIG_FILE)
 
+    username_from_cqlshrc = option_with_default(configs.get, 'authentication', 'username')
+    password_from_cqlshrc = option_with_default(rawconfigs.get, 'authentication', 'password')
+    if username_from_cqlshrc or password_from_cqlshrc:
+        if password_from_cqlshrc and not is_file_secure(os.path.expanduser(CONFIG_FILE)):
+            print("\nWarning: Password is found in an insecure cqlshrc file. The file is owned or readable by other users on the system.",
+                  end='', file=sys.stderr)
+        print("\nNotice: Credentials in the cqlshrc file is deprecated and will be ignored in the future."
+              "\nPlease use a credentials file to specify the username and password.\n", file=sys.stderr)
+
     optvalues = optparse.Values()
-    optvalues.username = option_with_default(configs.get, 'authentication', 'username')
-    optvalues.password = option_with_default(rawconfigs.get, 'authentication', 'password')
+
+    optvalues.username = None
+    optvalues.password = None
+    optvalues.credentials = os.path.expanduser(option_with_default(configs.get, 'authentication', 'credentials',
+                                                                   os.path.join(CQL_DIR, 'credentials')))
     optvalues.keyspace = option_with_default(configs.get, 'authentication', 'keyspace')
     optvalues.browser = option_with_default(configs.get, 'ui', 'browser', None)
     optvalues.completekey = option_with_default(configs.get, 'ui', 'completekey',
                                                 DEFAULT_COMPLETEKEY)
     optvalues.color = option_with_default(configs.getboolean, 'ui', 'color')
     optvalues.time_format = raw_option_with_default(configs, 'ui', 'time_format',
                                                     DEFAULT_TIMESTAMP_FORMAT)
@@ -2284,39 +2149,84 @@
                                                      DEFAULT_DOUBLE_PRECISION)
     optvalues.field_size_limit = option_with_default(configs.getint, 'csv', 'field_size_limit', csv.field_size_limit())
     optvalues.max_trace_wait = option_with_default(configs.getfloat, 'tracing', 'max_trace_wait',
                                                    DEFAULT_MAX_TRACE_WAIT)
     optvalues.timezone = option_with_default(configs.get, 'ui', 'timezone', None)
 
     optvalues.debug = False
+
+    optvalues.coverage = False
+    if 'CQLSH_COVERAGE' in environment.keys():
+        optvalues.coverage = True
+
     optvalues.file = None
     optvalues.ssl = option_with_default(configs.getboolean, 'connection', 'ssl', DEFAULT_SSL)
-
-    optvalues.no_compact = False
     optvalues.encoding = option_with_default(configs.get, 'ui', 'encoding', UTF8)
 
     optvalues.tty = option_with_default(configs.getboolean, 'ui', 'tty', sys.stdin.isatty())
     optvalues.protocol_version = option_with_default(configs.getint, 'protocol', 'version', None)
     optvalues.cqlversion = option_with_default(configs.get, 'cql', 'version', None)
     optvalues.connect_timeout = option_with_default(configs.getint, 'connection', 'timeout', DEFAULT_CONNECT_TIMEOUT_SECONDS)
     optvalues.request_timeout = option_with_default(configs.getint, 'connection', 'request_timeout', DEFAULT_REQUEST_TIMEOUT_SECONDS)
     optvalues.execute = None
+    optvalues.insecure_password_without_warning = False
 
     (options, arguments) = parser.parse_args(cmdlineargs, values=optvalues)
 
+    # Credentials from cqlshrc will be expanded,
+    # credentials from the command line are also expanded if there is a space...
+    # we need the following so that these two scenarios will work
+    #   cqlsh --credentials=~/.cassandra/creds
+    #   cqlsh --credentials ~/.cassandra/creds
+    options.credentials = os.path.expanduser(options.credentials)
+
+    if not is_file_secure(options.credentials):
+        print("\nWarning: Credentials file '{0}' exists but is not used, because:"
+              "\n  a. the file owner is not the current user; or"
+              "\n  b. the file is readable by group or other."
+              "\nPlease ensure the file is owned by the current user and is not readable by group or other."
+              "\nOn a Linux or UNIX-like system, you often can do this by using the `chown` and `chmod` commands:"
+              "\n  chown YOUR_USERNAME credentials"
+              "\n  chmod 600 credentials\n".format(options.credentials),
+              file=sys.stderr)
+        options.credentials = ''  # ConfigParser.read() will ignore unreadable files
+
+    if not options.username:
+        credentials = configparser.ConfigParser()
+        credentials.read(options.credentials)
+
+        # use the username from credentials file but fallback to cqlshrc if username is absent from the command line parameters
+        options.username = username_from_cqlshrc
+
+    if not options.password:
+        rawcredentials = configparser.RawConfigParser()
+        rawcredentials.read(options.credentials)
+
+        # handling password in the same way as username, priority cli > credentials > cqlshrc
+        options.password = option_with_default(rawcredentials.get, 'plain_text_auth', 'password', password_from_cqlshrc)
+        options.password = password_from_cqlshrc
+    elif not options.insecure_password_without_warning:
+        print("\nWarning: Using a password on the command line interface can be insecure."
+              "\nRecommendation: use the credentials file to securely provide the password.\n", file=sys.stderr)
+
+    # Make sure some user values read from the command line are in unicode
+    options.execute = maybe_ensure_text(options.execute)
+    options.username = maybe_ensure_text(options.username)
+    options.password = maybe_ensure_text(options.password)
+    options.keyspace = maybe_ensure_text(options.keyspace)
+
     hostname = option_with_default(configs.get, 'connection', 'hostname', DEFAULT_HOST)
     port = option_with_default(configs.get, 'connection', 'port', DEFAULT_PORT)
 
     try:
         options.connect_timeout = int(options.connect_timeout)
     except ValueError:
         parser.error('"%s" is not a valid connect timeout.' % (options.connect_timeout,))
         options.connect_timeout = DEFAULT_CONNECT_TIMEOUT_SECONDS
 
-
     try:
         options.request_timeout = int(options.request_timeout)
     except ValueError:
         parser.error('"%s" is not a valid request timeout.' % (options.request_timeout,))
         options.request_timeout = DEFAULT_REQUEST_TIMEOUT_SECONDS
 
     hostname = environment.get('CQLSH_HOST', hostname)
@@ -2397,15 +2307,15 @@
     if options.file is None:
         stdin = None
     else:
         try:
             encoding, bom_size = get_file_encoding_bomsize(options.file)
             stdin = codecs.open(options.file, 'r', encoding)
             stdin.seek(bom_size)
-        except IOError, e:
+        except IOError as e:
             sys.exit("Can't open %r: %s" % (options.file, e))
 
     if options.debug:
         sys.stderr.write("Using CQL driver: %s\n" % (cassandra,))
         sys.stderr.write("Using connect timeout: %s seconds\n" % (options.connect_timeout,))
         sys.stderr.write("Using '%s' encoding\n" % (options.encoding,))
         sys.stderr.write("Using ssl: %s\n" % (options.ssl,))
@@ -2433,60 +2343,74 @@
         try:
             from tzlocal import get_localzone
             timezone = get_localzone()
         except ImportError:
             # we silently ignore and fallback to UTC unless a custom timestamp format (which likely
             # does contain a TZ part) was specified
             if options.time_format != DEFAULT_TIMESTAMP_FORMAT:
-                sys.stderr.write("Warning: custom timestamp format specified in cqlshrc, but local timezone could not be detected.\n" +
-                                 "Either install Python 'tzlocal' module for auto-detection or specify client timezone in your cqlshrc.\n\n")
+                sys.stderr.write("Warning: custom timestamp format specified in cqlshrc, "
+                                 + "but local timezone could not be detected.\n"
+                                 + "Either install Python 'tzlocal' module for auto-detection "
+                                 + "or specify client timezone in your cqlshrc.\n\n")
 
     try:
         shell = Shell(hostname,
                       port,
                       color=options.color,
                       username=options.username,
-                      password=options.password,
                       stdin=stdin,
                       tty=options.tty,
                       completekey=options.completekey,
                       browser=options.browser,
                       protocol_version=options.protocol_version,
                       cqlver=options.cqlversion,
                       keyspace=options.keyspace,
-                      no_compact=options.no_compact,
                       display_timestamp_format=options.time_format,
                       display_nanotime_format=options.nanotime_format,
                       display_date_format=options.date_format,
                       display_float_precision=options.float_precision,
                       display_double_precision=options.double_precision,
                       display_timezone=timezone,
                       max_trace_wait=options.max_trace_wait,
                       ssl=options.ssl,
                       single_statement=options.execute,
                       request_timeout=options.request_timeout,
                       connect_timeout=options.connect_timeout,
-                      encoding=options.encoding)
+                      encoding=options.encoding,
+                      auth_provider=authproviderhandling.load_auth_provider(
+                          config_file=CONFIG_FILE,
+                          cred_file=options.credentials,
+                          username=options.username,
+                          password=options.password))
     except KeyboardInterrupt:
         sys.exit('Connection aborted.')
-    except CQL_ERRORS, e:
+    except CQL_ERRORS as e:
         sys.exit('Connection error: %s' % (e,))
-    except VersionNotSupported, e:
+    except VersionNotSupported as e:
         sys.exit('Unsupported CQL version: %s' % (e,))
     if options.debug:
         shell.debug = True
+    if options.coverage:
+        shell.coverage = True
+        import signal
+
+        def handle_sighup():
+            shell.stop_coverage()
+            shell.do_exit()
+
+        signal.signal(signal.SIGHUP, handle_sighup)
 
     shell.cmdloop()
     save_history()
-    batch_mode = options.file or options.execute
-    if batch_mode and shell.statement_error:
+
+    if shell.batch_mode and shell.statement_error:
         sys.exit(2)
 
 
 # always call this regardless of module name: when a sub-process is spawned
-# on Windows then the module name is not __main__, see CASSANDRA-9304
+# on Windows then the module name is not __main__, see CASSANDRA-9304 (Windows support was dropped in CASSANDRA-16956)
 insert_driver_hooks()
 
 if __name__ == '__main__':
     main(*read_options(sys.argv[1:], os.environ))
 
-# vim: set ft=python et ts=4 sw=4 :
+# vim: set ft=python et ts=4 sw=4 :
```

## Comparing `cqlsh_expansion-0.7.8.data/scripts/cqlsh.py` & `cqlshlib/cqlshmain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#!/bin/sh
-# -*- mode: Python -*-
-
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
@@ -13,172 +10,83 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-""":"
-# bash code here; finds a suitable python interpreter and execs this file.
-# prefer unqualified "python" if suitable:
-python -c 'import sys; sys.exit(not (0x020700b0 < sys.hexversion < 0x03000000))' 2>/dev/null \
-    && exec python "$0" "$@"
-for pyver in 2.7; do
-    which python$pyver > /dev/null 2>&1 && exec python$pyver "$0" "$@"
-done
-echo "No appropriate python interpreter found." >&2
-exit 1
-":"""
-
-from __future__ import with_statement
-
 import cmd
 import codecs
-import ConfigParser
+import configparser
 import csv
 import getpass
 import optparse
 import os
-import platform
+import re
+import subprocess
 import sys
 import traceback
 import warnings
 import webbrowser
-from StringIO import StringIO
 from contextlib import contextmanager
-from glob import glob
+from io import StringIO
 from uuid import UUID
 
-if sys.version_info[0] != 2 or sys.version_info[1] != 7:
-    sys.exit("\nCQL Shell supports only Python 2.7\n")
-
-# see CASSANDRA-10428
-if platform.python_implementation().startswith('Jython'):
-    sys.exit("\nCQL Shell does not run on Jython\n")
-
 UTF8 = 'utf-8'
-CP65001 = 'cp65001'  # Win utf-8 variant
 
 description = "CQL Shell for Apache Cassandra"
-version = "5.0.1"
+version = "6.2.0"
 
 readline = None
 try:
     # check if tty first, cause readline doesn't check, and only cares
     # about $TERM. we don't want the funky escape code stuff to be
     # output if not a tty.
     if sys.stdin.isatty():
         import readline
 except ImportError:
     pass
 
-CQL_LIB_PREFIX = 'cassandra-driver-internal-only-'
-
-CASSANDRA_PATH = os.path.join(os.path.dirname(os.path.realpath(__file__)), '..')
-CASSANDRA_CQL_HTML_FALLBACK = 'https://cassandra.apache.org/doc/cql3/CQL-3.2.html'
-
-# default location of local CQL.html
-if os.path.exists(CASSANDRA_PATH + '/doc/cql3/CQL.html'):
-    # default location of local CQL.html
-    CASSANDRA_CQL_HTML = 'file://' + CASSANDRA_PATH + '/doc/cql3/CQL.html'
-elif os.path.exists('/usr/share/doc/cassandra/CQL.html'):
-    # fallback to package file
-    CASSANDRA_CQL_HTML = 'file:///usr/share/doc/cassandra/CQL.html'
-else:
-    # fallback to online version
-    CASSANDRA_CQL_HTML = CASSANDRA_CQL_HTML_FALLBACK
-
 # On Linux, the Python webbrowser module uses the 'xdg-open' executable
 # to open a file/URL. But that only works, if the current session has been
 # opened from _within_ a desktop environment. I.e. 'xdg-open' will fail,
 # if the session's been opened via ssh to a remote box.
 #
-# Use 'python' to get some information about the detected browsers.
-# >>> import webbrowser
-# >>> webbrowser._tryorder
-# >>> webbrowser._browser
-#
-if len(webbrowser._tryorder) == 0:
-    CASSANDRA_CQL_HTML = CASSANDRA_CQL_HTML_FALLBACK
-elif webbrowser._tryorder[0] == 'xdg-open' and os.environ.get('XDG_DATA_DIRS', '') == '':
+try:
+    webbrowser.register_standard_browsers()  # registration is otherwise lazy in Python3
+except AttributeError:
+    pass
+if webbrowser._tryorder and webbrowser._tryorder[0] == 'xdg-open' and os.environ.get('XDG_DATA_DIRS', '') == '':
     # only on Linux (some OS with xdg-open)
     webbrowser._tryorder.remove('xdg-open')
     webbrowser._tryorder.append('xdg-open')
 
-# use bundled libs for python-cql and thrift, if available. if there
-# is a ../lib dir, use bundled libs there preferentially.
-ZIPLIB_DIRS = [os.path.join(CASSANDRA_PATH, 'lib')]
-myplatform = platform.system()
-is_win = myplatform == 'Windows'
-
-# Workaround for supporting CP65001 encoding on python < 3.3 (https://bugs.python.org/issue13216)
-if is_win and sys.version_info < (3, 3):
-    codecs.register(lambda name: codecs.lookup(UTF8) if name == CP65001 else None)
-
-if myplatform == 'Linux':
-    ZIPLIB_DIRS.append('/usr/share/cassandra/lib')
-
-if os.environ.get('CQLSH_NO_BUNDLED', ''):
-    ZIPLIB_DIRS = ()
-
-
-def find_zip(libprefix):
-    for ziplibdir in ZIPLIB_DIRS:
-        zips = glob(os.path.join(ziplibdir, libprefix + '*.zip'))
-        if zips:
-            return max(zips)   # probably the highest version, if multiple
-
-
-cql_zip = find_zip(CQL_LIB_PREFIX)
-if cql_zip:
-    ver = os.path.splitext(os.path.basename(cql_zip))[0][len(CQL_LIB_PREFIX):]
-    sys.path.insert(0, os.path.join(cql_zip, 'cassandra-driver-' + ver))
-
-third_parties = ('futures-', 'six-')
-
-for lib in third_parties:
-    lib_zip = find_zip(lib)
-    if lib_zip:
-        sys.path.insert(0, lib_zip)
-
 warnings.filterwarnings("ignore", r".*blist.*")
-try:
-    import cassandra
-except ImportError, e:
-    sys.exit("\nPython Cassandra driver not installed, or not on PYTHONPATH.\n"
-             'You might try "pip install cassandra-driver".\n\n'
-             'Python: %s\n'
-             'Module load path: %r\n\n'
-             'Error: %s\n' % (sys.executable, sys.path, e))
 
+import cassandra
 from cassandra.auth import PlainTextAuthProvider
 from cassandra.cluster import Cluster
 from cassandra.cqltypes import cql_typename
 from cassandra.marshal import int64_unpack
-from cassandra.metadata import (ColumnMetadata, KeyspaceMetadata,
-                                TableMetadata, protect_name, protect_names)
+from cassandra.metadata import (ColumnMetadata, KeyspaceMetadata, TableMetadata)
 from cassandra.policies import WhiteListRoundRobinPolicy
 from cassandra.query import SimpleStatement, ordered_dict_factory, TraceUnavailable
 from cassandra.util import datetime_from_timestamp
 
-# cqlsh should run correctly when run out of a Cassandra source tree,
-# out of an unpacked Cassandra tarball, and after a proper package install.
-cqlshlibdir = os.path.join(CASSANDRA_PATH, 'pylib')
-if os.path.isdir(cqlshlibdir):
-    sys.path.insert(0, cqlshlibdir)
-
-from cqlshlib import cql3handling, cqlhandling, pylexotron, sslhandling, cqlshhandling
+from cqlshlib import cql3handling, pylexotron, sslhandling, cqlshhandling, authproviderhandling
 from cqlshlib.copyutil import ExportTask, ImportTask
 from cqlshlib.displaying import (ANSI_RESET, BLUE, COLUMN_NAME_COLORS, CYAN,
                                  RED, WHITE, FormattedValue, colorme)
 from cqlshlib.formatting import (DEFAULT_DATE_FORMAT, DEFAULT_NANOTIME_FORMAT,
                                  DEFAULT_TIMESTAMP_FORMAT, CqlType, DateTimeFormat,
-                                 format_by_type, formatter_for)
+                                 format_by_type)
 from cqlshlib.tracing import print_trace, print_trace_session
-from cqlshlib.util import get_file_encoding_bomsize, trim_if_present
+from cqlshlib.util import get_file_encoding_bomsize
+from cqlshlib.util import is_file_secure
+
 
 DEFAULT_HOST = '127.0.0.1'
 DEFAULT_PORT = 9042
 DEFAULT_SSL = False
 DEFAULT_CONNECT_TIMEOUT_SECONDS = 5
 DEFAULT_REQUEST_TIMEOUT_SECONDS = 10
 
@@ -189,91 +97,116 @@
 if readline is not None and readline.__doc__ is not None and 'libedit' in readline.__doc__:
     DEFAULT_COMPLETEKEY = '\t'
 else:
     DEFAULT_COMPLETEKEY = 'tab'
 
 cqldocs = None
 cqlruleset = None
+CASSANDRA_CQL_HTML = None
 
 epilog = """Connects to %(DEFAULT_HOST)s:%(DEFAULT_PORT)d by default. These
 defaults can be changed by setting $CQLSH_HOST and/or $CQLSH_PORT. When a
 host (and optional port number) are given on the command line, they take
 precedence over any defaults.""" % globals()
 
 parser = optparse.OptionParser(description=description, epilog=epilog,
                                usage="Usage: %prog [options] [host [port]]",
                                version='cqlsh ' + version)
 parser.add_option("-C", "--color", action='store_true', dest='color',
                   help='Always use color output')
 parser.add_option("--no-color", action='store_false', dest='color',
                   help='Never use color output')
 parser.add_option("--browser", dest='browser', help="""The browser to use to display CQL help, where BROWSER can be:
-                                                    - one of the supported browsers in https://docs.python.org/2/library/webbrowser.html.
+                                                    - one of the supported browsers in https://docs.python.org/3/library/webbrowser.html.
                                                     - browser path followed by %s, example: /usr/bin/google-chrome-stable %s""")
 parser.add_option('--ssl', action='store_true', help='Use SSL', default=False)
-parser.add_option('--no_compact', action='store_true', help='No Compact', default=False)
 parser.add_option("-u", "--username", help="Authenticate as user.")
 parser.add_option("-p", "--password", help="Authenticate using password.")
 parser.add_option('-k', '--keyspace', help='Authenticate to the given keyspace.')
 parser.add_option("-f", "--file", help="Execute commands from FILE, then exit")
 parser.add_option('--debug', action='store_true',
                   help='Show additional debugging information')
-parser.add_option("--encoding", help="Specify a non-default encoding for output." +
-                  " (Default: %s)" % (UTF8,))
+parser.add_option('--coverage', action='store_true',
+                  help='Collect coverage data')
+parser.add_option("--encoding", help="Specify a non-default encoding for output."
+                  + " (Default: %s)" % (UTF8,))
 parser.add_option("--cqlshrc", help="Specify an alternative cqlshrc file location.")
+parser.add_option("--credentials", help="Specify an alternative credentials file location.")
 parser.add_option('--cqlversion', default=None,
                   help='Specify a particular CQL version, '
                        'by default the highest version supported by the server will be used.'
                        ' Examples: "3.0.3", "3.1.0"')
 parser.add_option("--protocol-version", type="int", default=None,
                   help='Specify a specific protcol version otherwise the client will default and downgrade as necessary')
 
 parser.add_option("-e", "--execute", help='Execute the statement and quit.')
 parser.add_option("--connect-timeout", default=DEFAULT_CONNECT_TIMEOUT_SECONDS, dest='connect_timeout',
                   help='Specify the connection timeout in seconds (default: %default seconds).')
 parser.add_option("--request-timeout", default=DEFAULT_REQUEST_TIMEOUT_SECONDS, dest='request_timeout',
                   help='Specify the default request timeout in seconds (default: %default seconds).')
 parser.add_option("-t", "--tty", action='store_true', dest='tty',
                   help='Force tty mode (command prompt).')
+parser.add_option('-v', action="version", help='Print the current version of cqlsh.')
 
-optvalues = optparse.Values()
-(options, arguments) = parser.parse_args(sys.argv[1:], values=optvalues)
+# This is a hidden option to suppress the warning when the -p/--password command line option is used.
+# Power users may use this option if they know no other people has access to the system where cqlsh is run or don't care about security.
+# Use of this option in scripting is discouraged. Please use a (temporary) credentials file where possible.
+# The Cassandra distributed tests (dtests) also use this option in some tests when a well-known password is supplied via the command line.
+parser.add_option("--insecure-password-without-warning", action='store_true', dest='insecure_password_without_warning',
+                  help=optparse.SUPPRESS_HELP)
 
-# BEGIN history/config definition
-HISTORY_DIR = os.path.expanduser(os.path.join('~', '.cassandra'))
+# use cfoptions for config file
 
-if hasattr(options, 'cqlshrc'):
-    CONFIG_FILE = options.cqlshrc
-    if not os.path.exists(CONFIG_FILE):
-        print '\nWarning: Specified cqlshrc location `%s` does not exist.  Using `%s` instead.\n' % (CONFIG_FILE, HISTORY_DIR)
-        CONFIG_FILE = os.path.join(HISTORY_DIR, 'cqlshrc')
-else:
-    CONFIG_FILE = os.path.join(HISTORY_DIR, 'cqlshrc')
+opt_values = optparse.Values()
+(cfoptions, arguments) = parser.parse_args(sys.argv[1:], values=opt_values)
+
+# BEGIN history config
+
+
+def mkdirp(path):
+    """Creates all parent directories up to path parameter or fails when path exists, but it is not a directory."""
 
-HISTORY = os.path.join(HISTORY_DIR, 'cqlsh_history')
-if not os.path.exists(HISTORY_DIR):
     try:
-        os.mkdir(HISTORY_DIR)
+        os.makedirs(path)
     except OSError:
-        print '\nWarning: Cannot create directory at `%s`. Command history will not be saved.\n' % HISTORY_DIR
+        if not os.path.isdir(path):
+            raise
+
 
-OLD_CONFIG_FILE = os.path.expanduser(os.path.join('~', '.cqlshrc'))
-if os.path.exists(OLD_CONFIG_FILE):
-    if os.path.exists(CONFIG_FILE):
-        print '\nWarning: cqlshrc config files were found at both the old location (%s) and \
-                the new location (%s), the old config file will not be migrated to the new \
-                location, and the new location will be used for now.  You should manually \
-                consolidate the config files at the new location and remove the old file.' \
-                % (OLD_CONFIG_FILE, CONFIG_FILE)
+def resolve_cql_history_file():
+    default_cql_history = os.path.expanduser(os.path.join('~', '.cassandra', 'cqlsh_history'))
+    if 'CQL_HISTORY' in os.environ:
+        return os.environ['CQL_HISTORY']
     else:
-        os.rename(OLD_CONFIG_FILE, CONFIG_FILE)
-OLD_HISTORY = os.path.expanduser(os.path.join('~', '.cqlsh_history'))
-if os.path.exists(OLD_HISTORY):
-    os.rename(OLD_HISTORY, HISTORY)
-# END history/config definition
+        return default_cql_history
+
+
+HISTORY = resolve_cql_history_file()
+HISTORY_DIR = os.path.dirname(HISTORY)
+
+try:
+    mkdirp(HISTORY_DIR)
+except OSError:
+    print('\nWarning: Cannot create directory at `%s`. Command history will not be saved. Please check what was the environment property CQL_HISTORY set to.\n' % HISTORY_DIR)
+
+
+# END history config
+
+
+DEFAULT_CQLSHRC = os.path.expanduser(os.path.join('~', '.cassandra', 'cqlshrc'))
+
+if hasattr(cfoptions, 'cqlshrc'):
+    CONFIG_FILE = os.path.expanduser(cfoptions.cqlshrc)
+    if not os.path.exists(CONFIG_FILE):
+        print('\nWarning: Specified cqlshrc location `%s` does not exist.  Using `%s` instead.\n' % (CONFIG_FILE, DEFAULT_CQLSHRC))
+        CONFIG_FILE = DEFAULT_CQLSHRC
+else:
+    CONFIG_FILE = DEFAULT_CQLSHRC
+
+CQL_DIR = os.path.dirname(CONFIG_FILE)
 
 CQL_ERRORS = (
     cassandra.AlreadyExists, cassandra.AuthenticationFailed, cassandra.CoordinationFailure,
     cassandra.InvalidRequest, cassandra.Timeout, cassandra.Unauthorized, cassandra.OperationTimedOut,
     cassandra.cluster.NoHostAvailable,
     cassandra.connection.ConnectionBusy, cassandra.connection.ProtocolError, cassandra.connection.ConnectionException,
     cassandra.protocol.ErrorMessage, cassandra.protocol.InternalError, cassandra.query.TraceUnavailable
@@ -340,23 +273,27 @@
         return 'Failed to %s %s : %s' \
                % (self.verb, what, self.err)
 
     def __repr__(self):
         return '<%s %s>' % (self.__class__.__name__, self.message())
 
 
+def maybe_ensure_text(val):
+    return str(val) if val else val
+
+
 class FormatError(DecodeError):
     verb = 'format'
 
 
 def full_cql_version(ver):
     while ver.count('.') < 2:
         ver += '.0'
     ver_parts = ver.split('-', 1) + ['']
-    vertuple = tuple(map(int, ver_parts[0].split('.')) + [ver_parts[1]])
+    vertuple = tuple(list(map(int, ver_parts[0].split('.'))) + [ver_parts[1]])
     return ver, vertuple
 
 
 def format_value(val, cqltype, encoding, addcolor=False, date_time_format=None,
                  float_precision=None, colormap=None, nullval=None):
     if isinstance(val, DecodeError):
         if addcolor:
@@ -377,114 +314,78 @@
         pass
 
 
 warnings.showwarning = show_warning_without_quoting_line
 warnings.filterwarnings('always', category=cql3handling.UnexpectedTableStructure)
 
 
-def insert_driver_hooks():
-
-    class DateOverFlowWarning(RuntimeWarning):
-        pass
-
-    # Native datetime types blow up outside of datetime.[MIN|MAX]_YEAR. We will fall back to an int timestamp
-    def deserialize_date_fallback_int(byts, protocol_version):
-        timestamp_ms = int64_unpack(byts)
-        try:
-            return datetime_from_timestamp(timestamp_ms / 1000.0)
-        except OverflowError:
-            warnings.warn(DateOverFlowWarning("Some timestamps are larger than Python datetime can represent. "
-                                              "Timestamps are displayed in milliseconds from epoch."))
-            return timestamp_ms
-
-    cassandra.cqltypes.DateType.deserialize = staticmethod(deserialize_date_fallback_int)
-
-    if hasattr(cassandra, 'deserializers'):
-        del cassandra.deserializers.DesDateType
-
-    # Return cassandra.cqltypes.EMPTY instead of None for empty values
-    cassandra.cqltypes.CassandraType.support_empty_values = True
-
-
-class FrozenType(cassandra.cqltypes._ParameterizedType):
-    """
-    Needed until the bundled python driver adds FrozenType.
-    """
-    typename = "frozen"
-    num_subtypes = 1
-
-    @classmethod
-    def deserialize_safe(cls, byts, protocol_version):
-        subtype, = cls.subtypes
-        return subtype.from_binary(byts)
-
-    @classmethod
-    def serialize_safe(cls, val, protocol_version):
-        subtype, = cls.subtypes
-        return subtype.to_binary(val, protocol_version)
-
-
 class Shell(cmd.Cmd):
     custom_prompt = os.getenv('CQLSH_PROMPT', '')
-    if custom_prompt is not '':
+    if custom_prompt != '':
         custom_prompt += "\n"
     default_prompt = custom_prompt + "cqlsh> "
     continue_prompt = "   ... "
-    keyspace_prompt = custom_prompt + "cqlsh:%s> "
-    keyspace_continue_prompt = "%s    ... "
+    keyspace_prompt = custom_prompt + "cqlsh:{}> "
+    keyspace_continue_prompt = "{}    ... "
     show_line_nums = False
     debug = False
+    coverage = False
+    coveragerc_path = None
     stop = False
     last_hist = None
     shunted_query_out = None
     use_paging = True
 
     default_page_size = 100
 
     def __init__(self, hostname, port, color=False,
-                 username=None, password=None, encoding=None, stdin=None, tty=True,
+                 username=None, encoding=None, stdin=None, tty=True,
                  completekey=DEFAULT_COMPLETEKEY, browser=None, use_conn=None,
                  cqlver=None, keyspace=None,
                  tracing_enabled=False, expand_enabled=False,
-                 no_compact=False,
                  display_nanotime_format=DEFAULT_NANOTIME_FORMAT,
                  display_timestamp_format=DEFAULT_TIMESTAMP_FORMAT,
                  display_date_format=DEFAULT_DATE_FORMAT,
                  display_float_precision=DEFAULT_FLOAT_PRECISION,
                  display_double_precision=DEFAULT_DOUBLE_PRECISION,
                  display_timezone=None,
                  max_trace_wait=DEFAULT_MAX_TRACE_WAIT,
                  ssl=False,
                  single_statement=None,
                  request_timeout=DEFAULT_REQUEST_TIMEOUT_SECONDS,
                  protocol_version=None,
-                 connect_timeout=DEFAULT_CONNECT_TIMEOUT_SECONDS):
+                 connect_timeout=DEFAULT_CONNECT_TIMEOUT_SECONDS,
+                 is_subshell=False,
+                 auth_provider=None):
         cmd.Cmd.__init__(self, completekey=completekey)
         self.hostname = hostname
         self.port = port
-        self.auth_provider = None
-        if username:
-            if not password:
-                password = getpass.getpass()
-            self.auth_provider = PlainTextAuthProvider(username=username, password=password)
+        self.auth_provider = auth_provider
         self.username = username
+
+        if isinstance(auth_provider, PlainTextAuthProvider):
+            self.username = auth_provider.username
+            if not auth_provider.password:
+                # if no password is provided, we need to query the user to get one.
+                password = getpass.getpass()
+                self.auth_provider = PlainTextAuthProvider(username=auth_provider.username, password=password)
+
         self.keyspace = keyspace
         self.ssl = ssl
         self.tracing_enabled = tracing_enabled
         self.page_size = self.default_page_size
         self.expand_enabled = expand_enabled
         if use_conn:
             self.conn = use_conn
         else:
             kwargs = {}
             if protocol_version is not None:
                 kwargs['protocol_version'] = protocol_version
             self.conn = Cluster(contact_points=(self.hostname,), port=self.port, cql_version=cqlver,
                                 auth_provider=self.auth_provider,
-                                no_compact=no_compact,
                                 ssl_options=sslhandling.ssl_settings(hostname, CONFIG_FILE) if ssl else None,
                                 load_balancing_policy=WhiteListRoundRobinPolicy([self.hostname]),
                                 control_connection_timeout=connect_timeout,
                                 connect_timeout=connect_timeout,
                                 **kwargs)
         self.owns_connection = not use_conn
 
@@ -516,58 +417,45 @@
         self.current_keyspace = keyspace
 
         self.max_trace_wait = max_trace_wait
         self.session.max_trace_wait = max_trace_wait
 
         self.tty = tty
         self.encoding = encoding
-        self.check_windows_encoding()
 
         self.output_codec = codecs.lookup(encoding)
 
         self.statement = StringIO()
         self.lineno = 1
         self.in_comment = False
 
         self.prompt = ''
         if stdin is None:
             stdin = sys.stdin
 
         if tty:
             self.reset_prompt()
             self.report_connection()
-            print 'Use HELP for help.'
+            print('Use HELP for help.')
         else:
             self.show_line_nums = True
         self.stdin = stdin
         self.query_out = sys.stdout
         self.consistency_level = cassandra.ConsistencyLevel.ONE
         self.serial_consistency_level = cassandra.ConsistencyLevel.SERIAL
 
         self.empty_lines = 0
         self.statement_error = False
         self.single_statement = single_statement
+        self.is_subshell = is_subshell
 
     @property
     def batch_mode(self):
         return not self.tty
 
-    @property
-    def is_using_utf8(self):
-        # utf8 encodings from https://docs.python.org/{2,3}/library/codecs.html
-        return self.encoding.replace('-', '_').lower() in ['utf', 'utf_8', 'u8', 'utf8', CP65001]
-
-    def check_windows_encoding(self):
-        if is_win and os.name == 'nt' and self.tty and \
-           self.is_using_utf8 and sys.stdout.encoding != CP65001:
-            self.printerr("\nWARNING: console codepage must be set to cp65001 "
-                          "to support {} encoding on Windows platforms.\n"
-                          "If you experience encoding problems, change your console"
-                          " codepage with 'chcp 65001' before starting cqlsh.\n".format(self.encoding))
-
     def set_expanded_cql_version(self, ver):
         ver, vertuple = full_cql_version(ver)
         self.cql_version = ver
         self.cql_ver_tuple = vertuple
 
     def cqlver_atleast(self, major, minor=0, patch=0):
         return self.cql_ver_tuple[:3] >= (major, minor, patch)
@@ -580,15 +468,15 @@
                                        date_format=self.display_date_format, nanotime_format=self.display_nanotime_format,
                                        timezone=self.display_timezone)
             precision = self.display_double_precision if cqltype is not None and cqltype.type_name == 'double' \
                 else self.display_float_precision
             return format_value(val, cqltype=cqltype, encoding=self.output_codec.name,
                                 addcolor=self.color, date_time_format=dtformats,
                                 float_precision=precision, **kwargs)
-        except Exception, e:
+        except Exception as e:
             err = FormatError(val, e)
             self.decoding_errors.append(err)
             return format_value(err, cqltype=cqltype, encoding=self.output_codec.name, addcolor=self.color)
 
     def myformat_colname(self, name, table_meta=None):
         column_colors = COLUMN_NAME_COLORS.copy()
         # check column role and color appropriately
@@ -602,125 +490,132 @@
         return self.myformat_value(name, colormap=column_colors)
 
     def report_connection(self):
         self.show_host()
         self.show_version()
 
     def show_host(self):
-        print "Connected to %s at %s:%d." % \
-            (self.applycolor(self.get_cluster_name(), BLUE),
-              self.hostname,
-              self.port)
+        print("Connected to {0} at {1}:{2}"
+              .format(self.applycolor(self.get_cluster_name(), BLUE),
+                      self.hostname,
+                      self.port))
 
     def show_version(self):
         vers = self.connection_versions.copy()
         vers['shver'] = version
         # system.Versions['cql'] apparently does not reflect changes with
         # set_cql_version.
         vers['cql'] = self.cql_version
-        print "[cqlsh %(shver)s | Cassandra %(build)s | CQL spec %(cql)s | Native protocol v%(protocol)s]" % vers
+        print("[cqlsh %(shver)s | Cassandra %(build)s | CQL spec %(cql)s | Native protocol v%(protocol)s]" % vers)
 
     def show_session(self, sessionid, partial_session=False):
         print_trace_session(self, self.session, sessionid, partial_session)
 
+    def show_replicas(self, token_value, keyspace=None):
+        ks = self.current_keyspace if keyspace is None else keyspace
+        token_map = self.conn.metadata.token_map
+        nodes = token_map.get_replicas(ks, token_map.token_class(token_value))
+        addresses = [x.address for x in nodes]
+        print(f"{addresses}")
+
     def get_connection_versions(self):
         result, = self.session.execute("select * from system.local where key = 'local'")
         vers = {
             'build': result['release_version'],
+            'protocol': self.conn.protocol_version,
             'cql': result['cql_version'],
         }
-        vers['protocol'] = self.conn.protocol_version
         self.connection_versions = vers
 
     def get_keyspace_names(self):
-        return map(str, self.conn.metadata.keyspaces.keys())
+        return list(self.conn.metadata.keyspaces)
 
     def get_columnfamily_names(self, ksname=None):
         if ksname is None:
             ksname = self.current_keyspace
 
-        return map(str, self.get_keyspace_meta(ksname).tables.keys())
+        return list(self.get_keyspace_meta(ksname).tables)
 
     def get_materialized_view_names(self, ksname=None):
         if ksname is None:
             ksname = self.current_keyspace
 
-        return map(str, self.get_keyspace_meta(ksname).views.keys())
+        return list(self.get_keyspace_meta(ksname).views)
 
     def get_index_names(self, ksname=None):
         if ksname is None:
             ksname = self.current_keyspace
 
-        return map(str, self.get_keyspace_meta(ksname).indexes.keys())
+        return list(self.get_keyspace_meta(ksname).indexes)
 
     def get_column_names(self, ksname, cfname):
         if ksname is None:
             ksname = self.current_keyspace
         layout = self.get_table_meta(ksname, cfname)
-        return [unicode(col) for col in layout.columns]
+        return list(layout.columns)
 
     def get_usertype_names(self, ksname=None):
         if ksname is None:
             ksname = self.current_keyspace
 
-        return self.get_keyspace_meta(ksname).user_types.keys()
+        return list(self.get_keyspace_meta(ksname).user_types)
 
     def get_usertype_layout(self, ksname, typename):
         if ksname is None:
             ksname = self.current_keyspace
 
         ks_meta = self.get_keyspace_meta(ksname)
 
         try:
             user_type = ks_meta.user_types[typename]
         except KeyError:
-            raise UserTypeNotFound("User type %r not found" % typename)
+            raise UserTypeNotFound("User type {!r} not found".format(typename))
 
-        return zip(user_type.field_names, user_type.field_types)
+        return list(zip(user_type.field_names, user_type.field_types))
 
     def get_userfunction_names(self, ksname=None):
         if ksname is None:
             ksname = self.current_keyspace
 
-        return map(lambda f: f.name, self.get_keyspace_meta(ksname).functions.values())
+        return [f.name for f in list(self.get_keyspace_meta(ksname).functions.values())]
 
     def get_useraggregate_names(self, ksname=None):
         if ksname is None:
             ksname = self.current_keyspace
 
-        return map(lambda f: f.name, self.get_keyspace_meta(ksname).aggregates.values())
+        return [f.name for f in list(self.get_keyspace_meta(ksname).aggregates.values())]
 
     def get_cluster_name(self):
         return self.conn.metadata.cluster_name
 
     def get_partitioner(self):
         return self.conn.metadata.partitioner
 
     def get_keyspace_meta(self, ksname):
-        if ksname not in self.conn.metadata.keyspaces:
-            raise KeyspaceNotFound('Keyspace %r not found.' % ksname)
-        return self.conn.metadata.keyspaces[ksname]
+        if ksname in self.conn.metadata.keyspaces:
+            return self.conn.metadata.keyspaces[ksname]
+
+        raise KeyspaceNotFound('Keyspace %r not found.' % ksname)
 
     def get_keyspaces(self):
-        return self.conn.metadata.keyspaces.values()
+        return list(self.conn.metadata.keyspaces.values())
 
     def get_ring(self, ks):
         self.conn.metadata.token_map.rebuild_keyspace(ks, build_if_absent=True)
         return self.conn.metadata.token_map.tokens_to_hosts_by_ks[ks]
 
     def get_table_meta(self, ksname, tablename):
         if ksname is None:
             ksname = self.current_keyspace
         ksmeta = self.get_keyspace_meta(ksname)
-
         if tablename not in ksmeta.tables:
             if ksname == 'system_auth' and tablename in ['roles', 'role_permissions']:
                 self.get_fake_auth_table_meta(ksname, tablename)
             else:
-                raise ColumnFamilyNotFound("Column family %r not found" % tablename)
+                raise ColumnFamilyNotFound("Column family {} not found".format(tablename))
         else:
             return ksmeta.tables[tablename]
 
     def get_fake_auth_table_meta(self, ksname, tablename):
         # may be using external auth implementation so internal tables
         # aren't actually defined in schema. In this case, we'll fake
         # them up
@@ -733,41 +628,41 @@
         elif tablename == 'role_permissions':
             ks_meta = KeyspaceMetadata(ksname, True, None, None)
             table_meta = TableMetadata(ks_meta, 'role_permissions')
             table_meta.columns['role'] = ColumnMetadata(table_meta, 'role', cassandra.cqltypes.UTF8Type)
             table_meta.columns['resource'] = ColumnMetadata(table_meta, 'resource', cassandra.cqltypes.UTF8Type)
             table_meta.columns['permission'] = ColumnMetadata(table_meta, 'permission', cassandra.cqltypes.UTF8Type)
         else:
-            raise ColumnFamilyNotFound("Column family %r not found" % tablename)
+            raise ColumnFamilyNotFound("Column family {} not found".format(tablename))
 
     def get_index_meta(self, ksname, idxname):
         if ksname is None:
             ksname = self.current_keyspace
         ksmeta = self.get_keyspace_meta(ksname)
 
         if idxname not in ksmeta.indexes:
-            raise IndexNotFound("Index %r not found" % idxname)
+            raise IndexNotFound("Index {} not found".format(idxname))
 
         return ksmeta.indexes[idxname]
 
     def get_view_meta(self, ksname, viewname):
         if ksname is None:
             ksname = self.current_keyspace
         ksmeta = self.get_keyspace_meta(ksname)
 
         if viewname not in ksmeta.views:
-            raise MaterializedViewNotFound("Materialized view %r not found" % viewname)
+            raise MaterializedViewNotFound("Materialized view '{}' not found".format(viewname))
         return ksmeta.views[viewname]
 
     def get_object_meta(self, ks, name):
         if name is None:
             if ks and ks in self.conn.metadata.keyspaces:
                 return self.conn.metadata.keyspaces[ks]
             elif self.current_keyspace is None:
-                raise ObjectNotFound("%r not found in keyspaces" % (ks))
+                raise ObjectNotFound("'{}' not found in keyspaces".format(ks))
             else:
                 name = ks
                 ks = self.current_keyspace
 
         if ks is None:
             ks = self.current_keyspace
 
@@ -776,87 +671,93 @@
         if name in ksmeta.tables:
             return ksmeta.tables[name]
         elif name in ksmeta.indexes:
             return ksmeta.indexes[name]
         elif name in ksmeta.views:
             return ksmeta.views[name]
 
-        raise ObjectNotFound("%r not found in keyspace %r" % (name, ks))
-
-    def get_usertypes_meta(self):
-        data = self.session.execute("select * from system.schema_usertypes")
-        if not data:
-            return cql3handling.UserTypesMeta({})
-
-        return cql3handling.UserTypesMeta.from_layout(data)
+        raise ObjectNotFound("'{}' not found in keyspace '{}'".format(name, ks))
 
     def get_trigger_names(self, ksname=None):
         if ksname is None:
             ksname = self.current_keyspace
 
         return [trigger.name
-                for table in self.get_keyspace_meta(ksname).tables.values()
-                for trigger in table.triggers.values()]
+                for table in list(self.get_keyspace_meta(ksname).tables.values())
+                for trigger in list(table.triggers.values())]
 
     def reset_statement(self):
         self.reset_prompt()
         self.statement.truncate(0)
+        self.statement.seek(0)
         self.empty_lines = 0
 
     def reset_prompt(self):
         if self.current_keyspace is None:
             self.set_prompt(self.default_prompt, True)
         else:
-            self.set_prompt(self.keyspace_prompt % self.current_keyspace, True)
+            self.set_prompt(self.keyspace_prompt.format(self.current_keyspace), True)
 
     def set_continue_prompt(self):
         if self.empty_lines >= 3:
             self.set_prompt("Statements are terminated with a ';'.  You can press CTRL-C to cancel an incomplete statement.")
             self.empty_lines = 0
             return
         if self.current_keyspace is None:
             self.set_prompt(self.continue_prompt)
         else:
             spaces = ' ' * len(str(self.current_keyspace))
-            self.set_prompt(self.keyspace_continue_prompt % spaces)
+            self.set_prompt(self.keyspace_continue_prompt.format(spaces))
         self.empty_lines = self.empty_lines + 1 if not self.lastcmd else 0
 
     @contextmanager
     def prepare_loop(self):
         readline = None
         if self.tty and self.completekey:
             try:
                 import readline
             except ImportError:
-                if is_win:
-                    print "WARNING: pyreadline dependency missing.  Install to enable tab completion."
                 pass
             else:
                 old_completer = readline.get_completer()
                 readline.set_completer(self.complete)
                 if readline.__doc__ is not None and 'libedit' in readline.__doc__:
                     readline.parse_and_bind("bind -e")
                     readline.parse_and_bind("bind '" + self.completekey + "' rl_complete")
                     readline.parse_and_bind("bind ^R em-inc-search-prev")
                 else:
                     readline.parse_and_bind(self.completekey + ": complete")
+        # start coverage collection if requested, unless in subshell
+        if self.coverage and not self.is_subshell:
+            # check for coveragerc file, write it if missing
+            if os.path.exists(CQL_DIR):
+                self.coveragerc_path = os.path.join(CQL_DIR, '.coveragerc')
+                covdata_path = os.path.join(CQL_DIR, '.coverage')
+                if not os.path.isfile(self.coveragerc_path):
+                    with open(self.coveragerc_path, 'w') as f:
+                        f.writelines(["[run]\n",
+                                      "concurrency = multiprocessing\n",
+                                      "data_file = {}\n".format(covdata_path),
+                                      "parallel = true\n"]
+                                     )
+                # start coverage
+                import coverage
+                self.cov = coverage.Coverage(config_file=self.coveragerc_path)
+                self.cov.start()
         try:
             yield
         finally:
             if readline is not None:
                 readline.set_completer(old_completer)
+            if self.coverage and not self.is_subshell:
+                self.stop_coverage()
 
     def get_input_line(self, prompt=''):
         if self.tty:
-            try:
-                self.lastcmd = raw_input(prompt).decode(self.encoding)
-            except UnicodeDecodeError:
-                self.lastcmd = ''
-                traceback.print_exc()
-                self.check_windows_encoding()
+            self.lastcmd = input(str(prompt))
             line = self.lastcmd + '\n'
         else:
             self.lastcmd = self.stdin.readline()
             line = self.lastcmd
             if not len(line):
                 raise EOFError
         self.lineno += 1
@@ -869,15 +770,15 @@
                 newline = self.get_input_line(prompt=prompt)
             except EOFError:
                 return
             if newline == until:
                 return
             yield newline
 
-    def cmdloop(self):
+    def cmdloop(self, intro=None):
         """
         Adapted from cmd.Cmd's version, because there is literally no way with
         cmd.Cmd.cmdloop() to tell the difference between "EOF" showing up in
         input and an actual EOF.
         """
         with self.prepare_loop():
             while not self.stop:
@@ -888,74 +789,91 @@
                     else:
                         line = self.get_input_line(self.prompt)
                     self.statement.write(line)
                     if self.onecmd(self.statement.getvalue()):
                         self.reset_statement()
                 except EOFError:
                     self.handle_eof()
-                except CQL_ERRORS, cqlerr:
-                    self.printerr(cqlerr.message.decode(encoding='utf-8'))
+                except CQL_ERRORS as cqlerr:
+                    self.printerr(cqlerr.message)
                 except KeyboardInterrupt:
                     self.reset_statement()
-                    print
+                    print('')
+
+    def strip_comment_blocks(self, statementtext):
+        comment_block_in_literal_string = re.search('["].*[/][*].*[*][/].*["]', statementtext)
+        if not comment_block_in_literal_string:
+            result = re.sub('[/][*].*[*][/]', "", statementtext)
+            if '*/' in result and '/*' not in result and not self.in_comment:
+                raise SyntaxError("Encountered comment block terminator without being in comment block")
+            if '/*' in result:
+                result = re.sub('[/][*].*', "", result)
+                self.in_comment = True
+            if '*/' in result:
+                result = re.sub('.*[*][/]', "", result)
+                self.in_comment = False
+            if self.in_comment and not re.findall('[/][*]|[*][/]', statementtext):
+                result = ''
+            return result
+        return statementtext
 
     def onecmd(self, statementtext):
         """
         Returns true if the statement is complete and was handled (meaning it
         can be reset).
         """
-
+        statementtext = self.strip_comment_blocks(statementtext)
         try:
             statements, endtoken_escaped = cqlruleset.cql_split_statements(statementtext)
-        except pylexotron.LexingError, e:
+        except pylexotron.LexingError as e:
             if self.show_line_nums:
-                self.printerr('Invalid syntax at char %d' % (e.charnum,))
+                self.printerr('Invalid syntax at line {0}, char {1}'
+                              .format(e.linenum, e.charnum))
             else:
-                self.printerr('Invalid syntax at line %d, char %d'
-                              % (e.linenum, e.charnum))
+                self.printerr('Invalid syntax at char {0}'.format(e.charnum))
             statementline = statementtext.split('\n')[e.linenum - 1]
-            self.printerr('  %s' % statementline)
-            self.printerr(' %s^' % (' ' * e.charnum))
+            self.printerr('  {0}'.format(statementline))
+            self.printerr(' {0}^'.format(' ' * e.charnum))
             return True
 
         while statements and not statements[-1]:
             statements = statements[:-1]
         if not statements:
             return True
         if endtoken_escaped or statements[-1][-1][0] != 'endtoken':
             self.set_continue_prompt()
             return
         for st in statements:
             try:
                 self.handle_statement(st, statementtext)
-            except Exception, e:
+            except Exception as e:
                 if self.debug:
                     traceback.print_exc()
                 else:
                     self.printerr(e)
         return True
 
     def handle_eof(self):
         if self.tty:
-            print
+            print('')
         statement = self.statement.getvalue()
         if statement.strip():
             if not self.onecmd(statement):
                 self.printerr('Incomplete statement at end of file')
         self.do_exit()
 
     def handle_statement(self, tokens, srcstr):
         # Concat multi-line statements and insert into history
         if readline is not None:
             nl_count = srcstr.count("\n")
 
             new_hist = srcstr.replace("\n", " ").rstrip()
 
             if nl_count > 1 and self.last_hist != new_hist:
-                readline.add_history(new_hist.encode(self.encoding))
+                readline.add_history(new_hist)
 
             self.last_hist = new_hist
         cmdword = tokens[0][1]
         if cmdword == '?':
             cmdword = 'help'
         custom_handler = getattr(self, 'do_' + cmdword.lower(), None)
         if custom_handler:
@@ -974,15 +892,15 @@
                                'batch', 'list'):
             # hey, maybe they know about some new syntax we don't. type
             # assumptions won't work, but maybe the query will.
             return self.perform_statement(cqlruleset.cql_extract_orig(tokens, srcstr))
         if parsed:
             self.printerr('Improper %s command (problem at %r).' % (cmdword, parsed.remainder[0]))
         else:
-            self.printerr('Improper %s command.' % cmdword)
+            self.printerr(f'Improper {cmdword} command.')
 
     def do_use(self, parsed):
         ksname = parsed.get_binding('ksname')
         success, _ = self.perform_simple_statement(SimpleStatement(parsed.extract_orig()))
         if success:
             if ksname[0] == '"' and ksname[-1] == '"':
                 self.current_keyspace = self.cql_unprotect_name(ksname)
@@ -995,14 +913,15 @@
         stop_tracing = ksname == 'system_traces' or (ksname is None and self.current_keyspace == 'system_traces')
         self.tracing_enabled = self.tracing_enabled and not stop_tracing
         statement = parsed.extract_orig()
         self.perform_statement(statement)
         self.tracing_enabled = tracing_was_enabled
 
     def perform_statement(self, statement):
+
         stmt = SimpleStatement(statement, consistency_level=self.consistency_level, serial_consistency_level=self.serial_consistency_level, fetch_size=self.page_size if self.use_paging else None)
         success, future = self.perform_simple_statement(stmt)
 
         if future:
             if future.warnings:
                 self.print_warnings(future.warnings)
 
@@ -1011,15 +930,15 @@
                     for trace in future.get_all_query_traces(max_wait_per=self.max_trace_wait, query_cl=self.consistency_level):
                         print_trace(self, trace)
                 except TraceUnavailable:
                     msg = "Statement trace did not complete within %d seconds; trace data may be incomplete." % (self.session.max_trace_wait,)
                     self.writeresult(msg, color=RED)
                     for trace_id in future.get_query_trace_ids():
                         self.show_session(trace_id, partial_session=True)
-                except Exception, err:
+                except Exception as err:
                     self.printerr("Unable to fetch query trace: %s" % (str(err),))
 
         return success
 
     def parse_for_select_meta(self, query_string):
         try:
             parsed = cqlruleset.cql_parse(query_string)[1]
@@ -1029,15 +948,15 @@
         name = self.cql_unprotect_name(parsed.get_binding('cfname', None))
         try:
             return self.get_table_meta(ks, name)
         except ColumnFamilyNotFound:
             try:
                 return self.get_view_meta(ks, name)
             except MaterializedViewNotFound:
-                raise ObjectNotFound("%r not found in keyspace %r" % (name, ks))
+                raise ObjectNotFound("'{}' not found in keyspace '{}'".format(name, ks))
 
     def parse_for_update_meta(self, query_string):
         try:
             parsed = cqlruleset.cql_parse(query_string)[1]
         except IndexError:
             return None
         ks = self.cql_unprotect_name(parsed.get_binding('ksname', None))
@@ -1048,16 +967,17 @@
         if not statement:
             return False, None
 
         future = self.session.execute_async(statement, trace=self.tracing_enabled)
         result = None
         try:
             result = future.result()
-        except CQL_ERRORS, err:
-            self.printerr(unicode(err.__class__.__name__) + u": " + err.message.decode(encoding='utf-8'))
+        except CQL_ERRORS as err:
+            err_msg = err.message if hasattr(err, 'message') else str(err)
+            self.printerr(str(err.__class__.__name__) + ": " + err_msg)
         except Exception:
             import traceback
             self.printerr(traceback.format_exc())
 
         # Even if statement failed we try to refresh schema if not agreed (see CASSANDRA-9689)
         if not future.is_schema_agreed:
             try:
@@ -1087,64 +1007,64 @@
         self.decoding_errors = []
 
         self.writeresult("")
 
         def print_all(result, table_meta, tty):
             # Return the number of rows in total
             num_rows = 0
-            isFirst = True
+            is_first = True
             while True:
                 # Always print for the first page even it is empty
-                if result.current_rows or isFirst:
+                if result.current_rows or is_first:
+                    with_header = is_first or tty
+                    self.print_static_result(result, table_meta, with_header, tty, num_rows)
                     num_rows += len(result.current_rows)
-                    with_header = isFirst or tty
-                    self.print_static_result(result, table_meta, with_header, tty)
                 if result.has_more_pages:
                     if self.shunted_query_out is None and tty:
                         # Only pause when not capturing.
-                        raw_input("---MORE---")
+                        input("---MORE---")
                     result.fetch_next_page()
                 else:
                     if not tty:
                         self.writeresult("")
                     break
-                isFirst = False
+                is_first = False
             return num_rows
 
         num_rows = print_all(result, table_meta, self.tty)
         self.writeresult("(%d rows)" % num_rows)
 
         if self.decoding_errors:
             for err in self.decoding_errors[:2]:
                 self.writeresult(err.message(), color=RED)
             if len(self.decoding_errors) > 2:
                 self.writeresult('%d more decoding errors suppressed.'
                                  % (len(self.decoding_errors) - 2), color=RED)
 
-    def print_static_result(self, result, table_meta, with_header, tty):
+    def print_static_result(self, result, table_meta, with_header, tty, row_count_offset=0):
         if not result.column_names and not table_meta:
             return
 
-        column_names = result.column_names or table_meta.columns.keys()
+        column_names = result.column_names or list(table_meta.columns.keys())
         formatted_names = [self.myformat_colname(name, table_meta) for name in column_names]
         if not result.current_rows:
             # print header only
             self.print_formatted_result(formatted_names, None, with_header=True, tty=tty)
             return
 
         cql_types = []
         if result.column_types:
             ks_name = table_meta.keyspace_name if table_meta else self.current_keyspace
             ks_meta = self.conn.metadata.keyspaces.get(ks_name, None)
             cql_types = [CqlType(cql_typename(t), ks_meta) for t in result.column_types]
 
-        formatted_values = [map(self.myformat_value, [row[column] for column in column_names], cql_types) for row in result.current_rows]
+        formatted_values = [list(map(self.myformat_value, [row[c] for c in column_names], cql_types)) for row in result.current_rows]
 
         if self.expand_enabled:
-            self.print_formatted_result_vertically(formatted_names, formatted_values)
+            self.print_formatted_result_vertically(formatted_names, formatted_values, row_count_offset)
         else:
             self.print_formatted_result(formatted_names, formatted_values, with_header, tty)
 
     def print_formatted_result(self, formatted_names, formatted_values, with_header, tty):
         # determine column widths
         widths = [n.displaywidth for n in formatted_names]
         if formatted_values is not None:
@@ -1167,21 +1087,21 @@
         for row in formatted_values:
             line = ' | '.join(col.rjust(w, color=self.color) for (col, w) in zip(row, widths))
             self.writeresult(' ' + line)
 
         if tty:
             self.writeresult("")
 
-    def print_formatted_result_vertically(self, formatted_names, formatted_values):
+    def print_formatted_result_vertically(self, formatted_names, formatted_values, row_count_offset):
         max_col_width = max([n.displaywidth for n in formatted_names])
         max_val_width = max([n.displaywidth for row in formatted_values for n in row])
 
         # for each row returned, list all the column-value pairs
-        for row_id, row in enumerate(formatted_values):
-            self.writeresult("@ Row %d" % (row_id + 1))
+        for i, row in enumerate(formatted_values):
+            self.writeresult("@ Row %d" % (row_count_offset + i + 1))
             self.writeresult('-%s-' % '-+-'.join(['-' * max_col_width, '-' * max_val_width]))
             for field_id, field in enumerate(row):
                 column = formatted_names[field_id].ljust(max_col_width, color=self.color)
                 value = field.ljust(field.displaywidth, color=self.color)
                 self.writeresult(' ' + " | ".join([column, value]))
             self.writeresult('')
 
@@ -1226,229 +1146,37 @@
         begidx = readline.get_begidx() + len(prevlines)
         stuff_to_complete = wholestmt[:begidx]
         return cqlruleset.cql_complete(stuff_to_complete, text, cassandra_conn=self,
                                        debug=debug_completion, startsymbol='cqlshCommand')
 
     def set_prompt(self, prompt, prepend_user=False):
         if prepend_user and self.username:
-            self.prompt = "%s@%s" % (self.username, prompt)
+            self.prompt = "{0}@{1}".format(self.username, prompt)
             return
         self.prompt = prompt
 
     def cql_unprotect_name(self, namestr):
         if namestr is None:
             return
         return cqlruleset.dequote_name(namestr)
 
     def cql_unprotect_value(self, valstr):
         if valstr is not None:
             return cqlruleset.dequote_value(valstr)
 
-    def print_recreate_keyspace(self, ksdef, out):
-        out.write(ksdef.export_as_string())
-        out.write("\n")
-
-    def print_recreate_columnfamily(self, ksname, cfname, out):
-        """
-        Output CQL commands which should be pasteable back into a CQL session
-        to recreate the given table.
-
-        Writes output to the given out stream.
-        """
-        out.write(self.get_table_meta(ksname, cfname).export_as_string())
-        out.write("\n")
-
-    def print_recreate_index(self, ksname, idxname, out):
-        """
-        Output CQL commands which should be pasteable back into a CQL session
-        to recreate the given index.
-
-        Writes output to the given out stream.
-        """
-        out.write(self.get_index_meta(ksname, idxname).export_as_string())
-        out.write("\n")
-
-    def print_recreate_materialized_view(self, ksname, viewname, out):
-        """
-        Output CQL commands which should be pasteable back into a CQL session
-        to recreate the given materialized view.
-
-        Writes output to the given out stream.
-        """
-        out.write(self.get_view_meta(ksname, viewname).export_as_string())
-        out.write("\n")
-
-    def print_recreate_object(self, ks, name, out):
-        """
-        Output CQL commands which should be pasteable back into a CQL session
-        to recreate the given object (ks, table or index).
-
-        Writes output to the given out stream.
-        """
-        out.write(self.get_object_meta(ks, name).export_as_string())
-        out.write("\n")
-
-    def describe_keyspaces(self):
-        print
-        cmd.Cmd.columnize(self, protect_names(self.get_keyspace_names()))
-        print
-
-    def describe_keyspace(self, ksname):
-        print
-        self.print_recreate_keyspace(self.get_keyspace_meta(ksname), sys.stdout)
-        print
-
-    def describe_columnfamily(self, ksname, cfname):
-        if ksname is None:
-            ksname = self.current_keyspace
-        if ksname is None:
-            raise NoKeyspaceError("No keyspace specified and no current keyspace")
-        print
-        self.print_recreate_columnfamily(ksname, cfname, sys.stdout)
-        print
-
-    def describe_index(self, ksname, idxname):
-        print
-        self.print_recreate_index(ksname, idxname, sys.stdout)
-        print
-
-    def describe_materialized_view(self, ksname, viewname):
-        if ksname is None:
-            ksname = self.current_keyspace
-        if ksname is None:
-            raise NoKeyspaceError("No keyspace specified and no current keyspace")
-        print
-        self.print_recreate_materialized_view(ksname, viewname, sys.stdout)
-        print
-
-    def describe_object(self, ks, name):
-        print
-        self.print_recreate_object(ks, name, sys.stdout)
-        print
-
-    def describe_columnfamilies(self, ksname):
-        print
-        if ksname is None:
-            for k in self.get_keyspaces():
-                name = protect_name(k.name)
-                print 'Keyspace %s' % (name,)
-                print '---------%s' % ('-' * len(name))
-                cmd.Cmd.columnize(self, protect_names(self.get_columnfamily_names(k.name)))
-                print
-        else:
-            cmd.Cmd.columnize(self, protect_names(self.get_columnfamily_names(ksname)))
-            print
-
-    def describe_functions(self, ksname):
-        print
-        if ksname is None:
-            for ksmeta in self.get_keyspaces():
-                name = protect_name(ksmeta.name)
-                print 'Keyspace %s' % (name,)
-                print '---------%s' % ('-' * len(name))
-                self._columnize_unicode(ksmeta.functions.keys())
-        else:
-            ksmeta = self.get_keyspace_meta(ksname)
-            self._columnize_unicode(ksmeta.functions.keys())
-
-    def describe_function(self, ksname, functionname):
-        if ksname is None:
-            ksname = self.current_keyspace
-        if ksname is None:
-            raise NoKeyspaceError("No keyspace specified and no current keyspace")
-        print
-        ksmeta = self.get_keyspace_meta(ksname)
-        functions = filter(lambda f: f.name == functionname, ksmeta.functions.values())
-        if len(functions) == 0:
-            raise FunctionNotFound("User defined function %r not found" % functionname)
-        print "\n\n".join(func.export_as_string() for func in functions)
-        print
-
-    def describe_aggregates(self, ksname):
-        print
-        if ksname is None:
-            for ksmeta in self.get_keyspaces():
-                name = protect_name(ksmeta.name)
-                print 'Keyspace %s' % (name,)
-                print '---------%s' % ('-' * len(name))
-                self._columnize_unicode(ksmeta.aggregates.keys())
-        else:
-            ksmeta = self.get_keyspace_meta(ksname)
-            self._columnize_unicode(ksmeta.aggregates.keys())
-
-    def describe_aggregate(self, ksname, aggregatename):
-        if ksname is None:
-            ksname = self.current_keyspace
-        if ksname is None:
-            raise NoKeyspaceError("No keyspace specified and no current keyspace")
-        print
-        ksmeta = self.get_keyspace_meta(ksname)
-        aggregates = filter(lambda f: f.name == aggregatename, ksmeta.aggregates.values())
-        if len(aggregates) == 0:
-            raise FunctionNotFound("User defined aggregate %r not found" % aggregatename)
-        print "\n\n".join(aggr.export_as_string() for aggr in aggregates)
-        print
-
-    def describe_usertypes(self, ksname):
-        print
-        if ksname is None:
-            for ksmeta in self.get_keyspaces():
-                name = protect_name(ksmeta.name)
-                print 'Keyspace %s' % (name,)
-                print '---------%s' % ('-' * len(name))
-                self._columnize_unicode(ksmeta.user_types.keys(), quote=True)
-        else:
-            ksmeta = self.get_keyspace_meta(ksname)
-            self._columnize_unicode(ksmeta.user_types.keys(), quote=True)
-
-    def describe_usertype(self, ksname, typename):
-        if ksname is None:
-            ksname = self.current_keyspace
-        if ksname is None:
-            raise NoKeyspaceError("No keyspace specified and no current keyspace")
-        print
-        ksmeta = self.get_keyspace_meta(ksname)
-        try:
-            usertype = ksmeta.user_types[typename]
-        except KeyError:
-            raise UserTypeNotFound("User type %r not found" % typename)
-        print usertype.export_as_string()
-
-    def _columnize_unicode(self, name_list, quote=False):
+    def _columnize_unicode(self, name_list):
         """
         Used when columnizing identifiers that may contain unicode
         """
-        names = [n.encode('utf-8') for n in name_list]
-        if quote:
-            names = protect_names(names)
+        names = [n for n in name_list]
         cmd.Cmd.columnize(self, names)
-        print
-
-    def describe_cluster(self):
-        print '\nCluster: %s' % self.get_cluster_name()
-        p = trim_if_present(self.get_partitioner(), 'org.apache.cassandra.dht.')
-        print 'Partitioner: %s\n' % p
-        # TODO: snitch?
-        # snitch = trim_if_present(self.get_snitch(), 'org.apache.cassandra.locator.')
-        # print 'Snitch: %s\n' % snitch
-        if self.current_keyspace is not None and self.current_keyspace != 'system':
-            print "Range ownership:"
-            ring = self.get_ring(self.current_keyspace)
-            for entry in ring.items():
-                print ' %39s  [%s]' % (str(entry[0].value), ', '.join([host.address for host in entry[1]]))
-            print
-
-    def describe_schema(self, include_system=False):
-        print
-        for k in self.get_keyspaces():
-            if include_system or k.name not in cql3handling.SYSTEM_KEYSPACES:
-                self.print_recreate_keyspace(k, sys.stdout)
-                print
+        print('')
 
     def do_describe(self, parsed):
+
         """
         DESCRIBE [cqlsh only]
 
         (DESC may be used as a shorthand.)
 
           Outputs information about the connected Cassandra cluster, or about
           the data objects stored in the cluster. Use in one of the following ways:
@@ -1459,15 +1187,14 @@
 
         DESCRIBE KEYSPACE [<keyspacename>]
 
           Output CQL commands that could be used to recreate the given keyspace,
           and the objects in it (such as tables, types, functions, etc.).
           In some cases, as the CQL interface matures, there will be some metadata
           about a keyspace that is not representable with CQL. That metadata will not be shown.
-
           The '<keyspacename>' argument may be omitted, in which case the current
           keyspace will be described.
 
         DESCRIBE TABLES
 
           Output the names of all tables in the current keyspace, or in all
           keyspaces if there is no current keyspace.
@@ -1531,74 +1258,114 @@
           Output the CQL command that could be used to recreate the given user-defined-aggregate.
 
         DESCRIBE <objname>
 
           Output CQL commands that could be used to recreate the entire object schema,
           where object can be either a keyspace or a table or an index or a materialized
           view (in this order).
-  """
-        what = parsed.matched[1][1].lower()
-        if what == 'functions':
-            self.describe_functions(self.current_keyspace)
-        elif what == 'function':
-            ksname = self.cql_unprotect_name(parsed.get_binding('ksname', None))
-            functionname = self.cql_unprotect_name(parsed.get_binding('udfname'))
-            self.describe_function(ksname, functionname)
-        elif what == 'aggregates':
-            self.describe_aggregates(self.current_keyspace)
-        elif what == 'aggregate':
-            ksname = self.cql_unprotect_name(parsed.get_binding('ksname', None))
-            aggregatename = self.cql_unprotect_name(parsed.get_binding('udaname'))
-            self.describe_aggregate(ksname, aggregatename)
-        elif what == 'keyspaces':
-            self.describe_keyspaces()
-        elif what == 'keyspace':
-            ksname = self.cql_unprotect_name(parsed.get_binding('ksname', ''))
-            if not ksname:
-                ksname = self.current_keyspace
-                if ksname is None:
-                    self.printerr('Not in any keyspace.')
-                    return
-            self.describe_keyspace(ksname)
-        elif what in ('columnfamily', 'table'):
-            ks = self.cql_unprotect_name(parsed.get_binding('ksname', None))
-            cf = self.cql_unprotect_name(parsed.get_binding('cfname'))
-            self.describe_columnfamily(ks, cf)
-        elif what == 'index':
-            ks = self.cql_unprotect_name(parsed.get_binding('ksname', None))
-            idx = self.cql_unprotect_name(parsed.get_binding('idxname', None))
-            self.describe_index(ks, idx)
-        elif what == 'materialized' and parsed.matched[2][1].lower() == 'view':
-            ks = self.cql_unprotect_name(parsed.get_binding('ksname', None))
-            mv = self.cql_unprotect_name(parsed.get_binding('mvname'))
-            self.describe_materialized_view(ks, mv)
-        elif what in ('columnfamilies', 'tables'):
-            self.describe_columnfamilies(self.current_keyspace)
-        elif what == 'types':
-            self.describe_usertypes(self.current_keyspace)
-        elif what == 'type':
-            ks = self.cql_unprotect_name(parsed.get_binding('ksname', None))
-            ut = self.cql_unprotect_name(parsed.get_binding('utname'))
-            self.describe_usertype(ks, ut)
-        elif what == 'cluster':
-            self.describe_cluster()
-        elif what == 'schema':
-            self.describe_schema(False)
-        elif what == 'full' and parsed.matched[2][1].lower() == 'schema':
-            self.describe_schema(True)
-        elif what:
-            ks = self.cql_unprotect_name(parsed.get_binding('ksname', None))
-            name = self.cql_unprotect_name(parsed.get_binding('cfname'))
-            if not name:
-                name = self.cql_unprotect_name(parsed.get_binding('idxname', None))
-            if not name:
-                name = self.cql_unprotect_name(parsed.get_binding('mvname', None))
-            self.describe_object(ks, name)
+        """
+        stmt = SimpleStatement(parsed.extract_orig(), consistency_level=cassandra.ConsistencyLevel.LOCAL_ONE, fetch_size=self.page_size if self.use_paging else None)
+        future = self.session.execute_async(stmt)
+
+        if self.connection_versions['build'][0] < '4':
+            print('\nWARN: DESCRIBE|DESC was moved to server side in Cassandra 4.0. As a consequence DESRIBE|DESC '
+                  'will not work in cqlsh %r connected to Cassandra %r, the version that you are connected to. '
+                  'DESCRIBE does not exist server side prior Cassandra 4.0.'
+                  % (version, self.connection_versions['build']))
+        else:
+            try:
+                result = future.result()
+
+                what = parsed.matched[1][1].lower()
+
+                if what in ('columnfamilies', 'tables', 'types', 'functions', 'aggregates'):
+                    self.describe_list(result)
+                elif what == 'keyspaces':
+                    self.describe_keyspaces(result)
+                elif what == 'cluster':
+                    self.describe_cluster(result)
+                elif what:
+                    self.describe_element(result)
+
+            except CQL_ERRORS as err:
+                err_msg = err.message if hasattr(err, 'message') else str(err)
+                self.printerr(err_msg.partition("message=")[2].strip('"'))
+            except Exception:
+                import traceback
+                self.printerr(traceback.format_exc())
+
+            if future:
+                if future.warnings:
+                    self.print_warnings(future.warnings)
+
     do_desc = do_describe
 
+    def describe_keyspaces(self, rows):
+        """
+        Print the output for a DESCRIBE KEYSPACES query
+        """
+        names = [r['name'] for r in rows]
+
+        print('')
+        cmd.Cmd.columnize(self, names)
+        print('')
+
+    def describe_list(self, rows):
+        """
+        Print the output for all the DESCRIBE queries for element names (e.g DESCRIBE TABLES, DESCRIBE FUNCTIONS ...)
+        """
+        keyspace = None
+        names = list()
+        for row in rows:
+            if row['keyspace_name'] != keyspace:
+                if keyspace is not None:
+                    self.print_keyspace_element_names(keyspace, names)
+
+                keyspace = row['keyspace_name']
+                names = list()
+
+            names.append(str(row['name']))
+
+        if keyspace is not None:
+            self.print_keyspace_element_names(keyspace, names)
+            print('')
+
+    def print_keyspace_element_names(self, keyspace, names):
+        print('')
+        if self.current_keyspace is None:
+            print('Keyspace %s' % (keyspace))
+            print('---------%s' % ('-' * len(keyspace)))
+        cmd.Cmd.columnize(self, names)
+
+    def describe_element(self, rows):
+        """
+        Print the output for all the DESCRIBE queries where an element name as been specified (e.g DESCRIBE TABLE, DESCRIBE INDEX ...)
+        """
+        for row in rows:
+            print('')
+            self.query_out.write(row['create_statement'])
+            print('')
+
+    def describe_cluster(self, rows):
+        """
+        Print the output for a DESCRIBE CLUSTER query.
+
+        If a specified keyspace was in use the returned ResultSet will contains a 'range_ownership' column,
+        otherwise not.
+        """
+        for row in rows:
+            print('\nCluster: %s' % row['cluster'])
+            print('Partitioner: %s' % row['partitioner'])
+            print('Snitch: %s\n' % row['snitch'])
+            if 'range_ownership' in row:
+                print("Range ownership:")
+                for entry in list(row['range_ownership'].items()):
+                    print(' %39s  [%s]' % (entry[0], ', '.join([host for host in entry[1]])))
+                print('')
+
     def do_copy(self, parsed):
         r"""
         COPY [cqlsh only]
 
           COPY x FROM: Imports CSV data into a Cassandra table
           COPY x TO: Exports data from a Cassandra table in CSV format.
 
@@ -1681,26 +1448,26 @@
         if ks is None:
             ks = self.current_keyspace
             if ks is None:
                 raise NoKeyspaceError("Not in any keyspace.")
         table = self.cql_unprotect_name(parsed.get_binding('cfname'))
         columns = parsed.get_binding('colnames', None)
         if columns is not None:
-            columns = map(self.cql_unprotect_name, columns)
+            columns = list(map(self.cql_unprotect_name, columns))
         else:
             # default to all known columns
             columns = self.get_column_names(ks, table)
 
         fname = parsed.get_binding('fname', None)
         if fname is not None:
             fname = self.cql_unprotect_value(fname)
 
-        copyoptnames = map(str.lower, parsed.get_binding('optnames', ()))
-        copyoptvals = map(self.cql_unprotect_value, parsed.get_binding('optvals', ()))
-        opts = dict(zip(copyoptnames, copyoptvals))
+        copyoptnames = list(map(str.lower, parsed.get_binding('optnames', ())))
+        copyoptvals = list(map(self.cql_unprotect_value, parsed.get_binding('optvals', ())))
+        opts = dict(list(zip(copyoptnames, copyoptvals)))
 
         direction = parsed.get_binding('dir').upper()
         if direction == 'FROM':
             task = ImportTask(self, ks, table, columns, fname, opts, self.conn.protocol_version, CONFIG_FILE)
         elif direction == 'TO':
             task = ExportTask(self, ks, table, columns, fname, opts, self.conn.protocol_version, CONFIG_FILE)
         else:
@@ -1714,34 +1481,43 @@
 
           Displays information about the current cqlsh session. Can be called in
           the following ways:
 
         SHOW VERSION
 
           Shows the version and build of the connected Cassandra instance, as
-          well as the versions of the CQL spec and the Thrift protocol that
-          the connected Cassandra instance understands.
+          well as the version of the CQL spec that the connected Cassandra
+          instance understands.
 
         SHOW HOST
 
           Shows where cqlsh is currently connected.
 
         SHOW SESSION <sessionid>
 
           Pretty-prints the requested tracing session.
+
+        SHOW REPLICAS <token> (<keyspace>)
+
+          Lists the replica nodes by IP address for the given token. The current
+          keyspace is used if one is not specified.
         """
         showwhat = parsed.get_binding('what').lower()
         if showwhat == 'version':
             self.get_connection_versions()
             self.show_version()
         elif showwhat == 'host':
             self.show_host()
         elif showwhat.startswith('session'):
             session_id = parsed.get_binding('sessionid').lower()
             self.show_session(UUID(session_id))
+        elif showwhat.startswith('replicas'):
+            token_id = parsed.get_binding('token')
+            keyspace = parsed.get_binding('keyspace')
+            self.show_replicas(token_id, keyspace)
         else:
             self.printerr('Wait, how do I show %r?' % (showwhat,))
 
     def do_source(self, parsed):
         """
         SOURCE [cqlsh only]
 
@@ -1763,33 +1539,37 @@
         """
         fname = parsed.get_binding('fname')
         fname = os.path.expanduser(self.cql_unprotect_value(fname))
         try:
             encoding, bom_size = get_file_encoding_bomsize(fname)
             f = codecs.open(fname, 'r', encoding)
             f.seek(bom_size)
-        except IOError, e:
+        except IOError as e:
             self.printerr('Could not open %r: %s' % (fname, e))
             return
-        username = self.auth_provider.username if self.auth_provider else None
-        password = self.auth_provider.password if self.auth_provider else None
         subshell = Shell(self.hostname, self.port, color=self.color,
-                         username=username, password=password,
+                         username=self.username,
                          encoding=self.encoding, stdin=f, tty=False, use_conn=self.conn,
                          cqlver=self.cql_version, keyspace=self.current_keyspace,
                          tracing_enabled=self.tracing_enabled,
                          display_nanotime_format=self.display_nanotime_format,
                          display_timestamp_format=self.display_timestamp_format,
                          display_date_format=self.display_date_format,
                          display_float_precision=self.display_float_precision,
                          display_double_precision=self.display_double_precision,
                          display_timezone=self.display_timezone,
                          max_trace_wait=self.max_trace_wait, ssl=self.ssl,
                          request_timeout=self.session.default_timeout,
-                         connect_timeout=self.conn.connect_timeout)
+                         connect_timeout=self.conn.connect_timeout,
+                         is_subshell=True,
+                         auth_provider=self.auth_provider)
+        # duplicate coverage related settings in subshell
+        if self.coverage:
+            subshell.coverage = True
+            subshell.coveragerc_path = self.coveragerc_path
         subshell.cmdloop()
         f.close()
 
     def do_capture(self, parsed):
         """
         CAPTURE [cqlsh only]
 
@@ -1815,17 +1595,17 @@
 
         To inspect the current capture configuration, use CAPTURE with no
         arguments.
         """
         fname = parsed.get_binding('fname')
         if fname is None:
             if self.shunted_query_out is not None:
-                print "Currently capturing query output to %r." % (self.query_out.name,)
+                print("Currently capturing query output to %r." % (self.query_out.name,))
             else:
-                print "Currently not capturing query output."
+                print("Currently not capturing query output.")
             return
 
         if fname.upper() == 'OFF':
             if self.shunted_query_out is None:
                 self.printerr('Not currently capturing output.')
                 return
             self.query_out.close()
@@ -1839,22 +1619,22 @@
             self.printerr('Already capturing output to %s. Use CAPTURE OFF'
                           ' to disable.' % (self.query_out.name,))
             return
 
         fname = os.path.expanduser(self.cql_unprotect_value(fname))
         try:
             f = open(fname, 'a')
-        except IOError, e:
+        except IOError as e:
             self.printerr('Could not open %r for append: %s' % (fname, e))
             return
         self.shunted_query_out = self.query_out
         self.shunted_color = self.color
         self.query_out = f
         self.color = False
-        print 'Now capturing query output to %r.' % (fname,)
+        print('Now capturing query output to %r.' % (fname,))
 
     def do_tracing(self, parsed):
         """
         TRACING [cqlsh]
 
           Enables or disables request tracing.
 
@@ -1910,19 +1690,19 @@
 
         CONSISTENCY
 
            CONSISTENCY with no arguments shows the current consistency level.
         """
         level = parsed.get_binding('level')
         if level is None:
-            print 'Current consistency level is %s.' % (cassandra.ConsistencyLevel.value_to_name[self.consistency_level])
+            print('Current consistency level is %s.' % (cassandra.ConsistencyLevel.value_to_name[self.consistency_level]))
             return
 
         self.consistency_level = cassandra.ConsistencyLevel.name_to_value[level.upper()]
-        print 'Consistency level set to %s.' % (level.upper(),)
+        print('Consistency level set to %s.' % (level.upper(),))
 
     def do_serial(self, parsed):
         """
         SERIAL CONSISTENCY [cqlsh only]
 
            Overrides serial consistency level (default level is SERIAL).
 
@@ -1936,19 +1716,19 @@
 
         SERIAL CONSISTENCY
 
            SERIAL CONSISTENCY with no arguments shows the current consistency level.
         """
         level = parsed.get_binding('level')
         if level is None:
-            print 'Current serial consistency level is %s.' % (cassandra.ConsistencyLevel.value_to_name[self.serial_consistency_level])
+            print('Current serial consistency level is %s.' % (cassandra.ConsistencyLevel.value_to_name[self.serial_consistency_level]))
             return
 
         self.serial_consistency_level = cassandra.ConsistencyLevel.name_to_value[level.upper()]
-        print 'Serial consistency level set to %s.' % (level.upper(),)
+        print('Serial consistency level set to %s.' % (level.upper(),))
 
     def do_login(self, parsed):
         """
         LOGIN [cqlsh only]
 
            Changes login information without requiring restart.
 
@@ -2004,16 +1784,15 @@
 
     def do_clear(self, parsed):
         """
         CLEAR/CLS [cqlsh only]
 
         Clears the console.
         """
-        import subprocess
-        subprocess.call(['clear', 'cls'][is_win], shell=True)
+        subprocess.call('clear', shell=True)
     do_cls = do_clear
 
     def do_debug(self, parsed):
         import pdb
         pdb.set_trace()
 
     def get_help_topics(self):
@@ -2044,20 +1823,20 @@
             if t.lower() in self.get_help_topics():
                 doc = getattr(self, 'do_' + t.lower()).__doc__
                 self.stdout.write(doc + "\n")
             elif t.lower() in cqldocs.get_help_topics():
                 urlpart = cqldocs.get_help_topic(t)
                 if urlpart is not None:
                     url = "%s#%s" % (CASSANDRA_CQL_HTML, urlpart)
-                    if len(webbrowser._tryorder) == 0:
-                        self.printerr("*** No browser to display CQL help. URL for help topic %s : %s" % (t, url))
-                    elif self.browser is not None:
-                        webbrowser.get(self.browser).open_new_tab(url)
+                    if self.browser is not None:
+                        opened = webbrowser.get(self.browser).open_new_tab(url)
                     else:
-                        webbrowser.open_new_tab(url)
+                        opened = webbrowser.open_new_tab(url)
+                    if not opened:
+                        self.printerr("*** No browser to display CQL help. URL for help topic %s : %s" % (t, url))
             else:
                 self.printerr("*** No help on %s" % (t,))
 
     def do_unicode(self, parsed):
         """
         Textual input/output
 
@@ -2093,33 +1872,30 @@
           PAGING with no arguments shows the current query paging status.
         """
         (self.use_paging, requested_page_size) = SwitchCommandWithValue(
             "PAGING", "Query paging", value_type=int).execute(self.use_paging, parsed, self.printerr)
         if self.use_paging and requested_page_size is not None:
             self.page_size = requested_page_size
         if self.use_paging:
-            print("Page size: {}".format(self.page_size))
+            print(("Page size: {}".format(self.page_size)))
         else:
             self.page_size = self.default_page_size
 
     def applycolor(self, text, color=None):
         if not color or not self.color:
             return text
         return color + text + ANSI_RESET
 
     def writeresult(self, text, color=None, newline=True, out=None):
         if out is None:
             out = self.query_out
 
         # convert Exceptions, etc to text
-        if not isinstance(text, (unicode, str)):
-            text = unicode(text)
-
-        if isinstance(text, unicode):
-            text = text.encode(self.encoding)
+        if not isinstance(text, str):
+            text = str(text)
 
         to_write = self.applycolor(text, color) + ('\n' if newline else '')
         out.write(to_write)
 
     def flush_output(self):
         self.query_out.flush()
 
@@ -2127,47 +1903,53 @@
         self.statement_error = True
         if shownum is None:
             shownum = self.show_line_nums
         if shownum:
             text = '%s:%d:%s' % (self.stdin.name, self.lineno, text)
         self.writeresult(text, color, newline=newline, out=sys.stderr)
 
+    def stop_coverage(self):
+        if self.coverage and self.cov is not None:
+            self.cov.stop()
+            self.cov.save()
+            self.cov = None
+
 
 class SwitchCommand(object):
     command = None
     description = None
 
     def __init__(self, command, desc):
         self.command = command
         self.description = desc
 
     def execute(self, state, parsed, printerr):
         switch = parsed.get_binding('switch')
         if switch is None:
             if state:
-                print "%s is currently enabled. Use %s OFF to disable" \
-                      % (self.description, self.command)
+                print("%s is currently enabled. Use %s OFF to disable"
+                      % (self.description, self.command))
             else:
-                print "%s is currently disabled. Use %s ON to enable." \
-                      % (self.description, self.command)
+                print("%s is currently disabled. Use %s ON to enable."
+                      % (self.description, self.command))
             return state
 
         if switch.upper() == 'ON':
             if state:
                 printerr('%s is already enabled. Use %s OFF to disable.'
                          % (self.description, self.command))
                 return state
-            print 'Now %s is enabled' % (self.description,)
+            print('Now %s is enabled' % (self.description,))
             return True
 
         if switch.upper() == 'OFF':
             if not state:
                 printerr('%s is not enabled.' % (self.description,))
                 return state
-            print 'Disabled %s.' % (self.description,)
+            print('Disabled %s.' % (self.description,))
             return False
 
 
 class SwitchCommandWithValue(SwitchCommand):
     """The same as SwitchCommand except it also accepts a value in place of ON.
 
     This returns a tuple of the form: (SWITCH_VALUE, PASSED_VALUE)
@@ -2185,63 +1967,74 @@
         binary_switch_value = SwitchCommand.execute(self, state, parsed, printerr)
         switch = parsed.get_binding('switch')
         try:
             value = self.value_type(switch)
             binary_switch_value = True
         except (ValueError, TypeError):
             value = None
-        return (binary_switch_value, value)
+        return binary_switch_value, value
 
 
 def option_with_default(cparser_getter, section, option, default=None):
     try:
         return cparser_getter(section, option)
-    except ConfigParser.Error:
+    except configparser.Error:
         return default
 
 
 def raw_option_with_default(configs, section, option, default=None):
     """
     Same (almost) as option_with_default() but won't do any string interpolation.
     Useful for config values that include '%' symbol, e.g. time format string.
     """
     try:
         return configs.get(section, option, raw=True)
-    except ConfigParser.Error:
+    except configparser.Error:
         return default
 
 
 def should_use_color():
     if not sys.stdout.isatty():
         return False
     if os.environ.get('TERM', '') in ('dumb', ''):
         return False
     try:
-        import subprocess
         p = subprocess.Popen(['tput', 'colors'], stdout=subprocess.PIPE)
         stdout, _ = p.communicate()
         if int(stdout.strip()) < 8:
             return False
     except (OSError, ImportError, ValueError):
         # oh well, we tried. at least we know there's a $TERM and it's
         # not "dumb".
         pass
     return True
 
 
-def read_options(cmdlineargs, environment):
-    configs = ConfigParser.SafeConfigParser()
+def read_options(cmdlineargs, environment=os.environ):
+    configs = configparser.ConfigParser()
     configs.read(CONFIG_FILE)
 
-    rawconfigs = ConfigParser.RawConfigParser()
+    rawconfigs = configparser.RawConfigParser()
     rawconfigs.read(CONFIG_FILE)
 
+    username_from_cqlshrc = option_with_default(configs.get, 'authentication', 'username')
+    password_from_cqlshrc = option_with_default(rawconfigs.get, 'authentication', 'password')
+    if username_from_cqlshrc or password_from_cqlshrc:
+        if password_from_cqlshrc and not is_file_secure(os.path.expanduser(CONFIG_FILE)):
+            print("\nWarning: Password is found in an insecure cqlshrc file. The file is owned or readable by other users on the system.",
+                  end='', file=sys.stderr)
+        print("\nNotice: Credentials in the cqlshrc file is deprecated and will be ignored in the future."
+              "\nPlease use a credentials file to specify the username and password.\n", file=sys.stderr)
+
     optvalues = optparse.Values()
-    optvalues.username = option_with_default(configs.get, 'authentication', 'username')
-    optvalues.password = option_with_default(rawconfigs.get, 'authentication', 'password')
+
+    optvalues.username = None
+    optvalues.password = None
+    optvalues.credentials = os.path.expanduser(option_with_default(configs.get, 'authentication', 'credentials',
+                                                                   os.path.join(CQL_DIR, 'credentials')))
     optvalues.keyspace = option_with_default(configs.get, 'authentication', 'keyspace')
     optvalues.browser = option_with_default(configs.get, 'ui', 'browser', None)
     optvalues.completekey = option_with_default(configs.get, 'ui', 'completekey',
                                                 DEFAULT_COMPLETEKEY)
     optvalues.color = option_with_default(configs.getboolean, 'ui', 'color')
     optvalues.time_format = raw_option_with_default(configs, 'ui', 'time_format',
                                                     DEFAULT_TIMESTAMP_FORMAT)
@@ -2255,28 +2048,75 @@
                                                      DEFAULT_DOUBLE_PRECISION)
     optvalues.field_size_limit = option_with_default(configs.getint, 'csv', 'field_size_limit', csv.field_size_limit())
     optvalues.max_trace_wait = option_with_default(configs.getfloat, 'tracing', 'max_trace_wait',
                                                    DEFAULT_MAX_TRACE_WAIT)
     optvalues.timezone = option_with_default(configs.get, 'ui', 'timezone', None)
 
     optvalues.debug = False
+
+    optvalues.coverage = False
+    if 'CQLSH_COVERAGE' in environment.keys():
+        optvalues.coverage = True
+
     optvalues.file = None
     optvalues.ssl = option_with_default(configs.getboolean, 'connection', 'ssl', DEFAULT_SSL)
-    optvalues.no_compact = False
     optvalues.encoding = option_with_default(configs.get, 'ui', 'encoding', UTF8)
 
     optvalues.tty = option_with_default(configs.getboolean, 'ui', 'tty', sys.stdin.isatty())
     optvalues.protocol_version = option_with_default(configs.getint, 'protocol', 'version', None)
     optvalues.cqlversion = option_with_default(configs.get, 'cql', 'version', None)
     optvalues.connect_timeout = option_with_default(configs.getint, 'connection', 'timeout', DEFAULT_CONNECT_TIMEOUT_SECONDS)
     optvalues.request_timeout = option_with_default(configs.getint, 'connection', 'request_timeout', DEFAULT_REQUEST_TIMEOUT_SECONDS)
     optvalues.execute = None
+    optvalues.insecure_password_without_warning = False
 
     (options, arguments) = parser.parse_args(cmdlineargs, values=optvalues)
 
+    # Credentials from cqlshrc will be expanded,
+    # credentials from the command line are also expanded if there is a space...
+    # we need the following so that these two scenarios will work
+    #   cqlsh --credentials=~/.cassandra/creds
+    #   cqlsh --credentials ~/.cassandra/creds
+    options.credentials = os.path.expanduser(options.credentials)
+
+    if not is_file_secure(options.credentials):
+        print("\nWarning: Credentials file '{0}' exists but is not used, because:"
+              "\n  a. the file owner is not the current user; or"
+              "\n  b. the file is readable by group or other."
+              "\nPlease ensure the file is owned by the current user and is not readable by group or other."
+              "\nOn a Linux or UNIX-like system, you often can do this by using the `chown` and `chmod` commands:"
+              "\n  chown YOUR_USERNAME credentials"
+              "\n  chmod 600 credentials\n".format(options.credentials),
+              file=sys.stderr)
+        options.credentials = ''  # ConfigParser.read() will ignore unreadable files
+
+    if not options.username:
+        credentials = configparser.ConfigParser()
+        credentials.read(options.credentials)
+
+        # use the username from credentials file but fallback to cqlshrc if username is absent from the command line parameters
+        options.username = username_from_cqlshrc
+
+    if not options.password:
+        rawcredentials = configparser.RawConfigParser()
+        rawcredentials.read(options.credentials)
+
+        # handling password in the same way as username, priority cli > credentials > cqlshrc
+        options.password = option_with_default(rawcredentials.get, 'plain_text_auth', 'password', password_from_cqlshrc)
+        options.password = password_from_cqlshrc
+    elif not options.insecure_password_without_warning:
+        print("\nWarning: Using a password on the command line interface can be insecure."
+              "\nRecommendation: use the credentials file to securely provide the password.\n", file=sys.stderr)
+
+    # Make sure some user values read from the command line are in unicode
+    options.execute = maybe_ensure_text(options.execute)
+    options.username = maybe_ensure_text(options.username)
+    options.password = maybe_ensure_text(options.password)
+    options.keyspace = maybe_ensure_text(options.keyspace)
+
     hostname = option_with_default(configs.get, 'connection', 'hostname', DEFAULT_HOST)
     port = option_with_default(configs.get, 'connection', 'port', DEFAULT_PORT)
 
     try:
         options.connect_timeout = int(options.connect_timeout)
     except ValueError:
         parser.error('"%s" is not a valid connect timeout.' % (options.connect_timeout,))
@@ -2333,14 +2173,30 @@
 
 
 def setup_cqldocs(cqlmodule):
     global cqldocs
     cqldocs = cqlmodule.cqldocs
 
 
+def setup_docspath(path):
+    global CASSANDRA_CQL_HTML
+    CASSANDRA_CQL_HTML_FALLBACK = 'https://cassandra.apache.org/doc/latest/cql/index.html'
+    #
+    # default location of local CQL.html
+    if os.path.exists(path + '/doc/cql3/CQL.html'):
+        # default location of local CQL.html
+        CASSANDRA_CQL_HTML = 'file://' + path + '/doc/cql3/CQL.html'
+    elif os.path.exists('/usr/share/doc/cassandra/CQL.html'):
+        # fallback to package file
+        CASSANDRA_CQL_HTML = 'file:///usr/share/doc/cassandra/CQL.html'
+    else:
+        # fallback to online version
+        CASSANDRA_CQL_HTML = CASSANDRA_CQL_HTML_FALLBACK
+
+
 def init_history():
     if readline is not None:
         try:
             readline.read_history_file(HISTORY)
         except IOError:
             pass
         delims = readline.get_completer_delims()
@@ -2353,28 +2209,57 @@
     if readline is not None:
         try:
             readline.write_history_file(HISTORY)
         except IOError:
             pass
 
 
-def main(options, hostname, port):
+def insert_driver_hooks():
+
+    class DateOverFlowWarning(RuntimeWarning):
+        pass
+
+    # Display milliseconds when datetime overflows (CASSANDRA-10625), E.g., the year 10000.
+    # Native datetime types blow up outside of datetime.[MIN|MAX]_YEAR. We will fall back to an int timestamp
+    def deserialize_date_fallback_int(byts, protocol_version):
+        timestamp_ms = int64_unpack(byts)
+        try:
+            return datetime_from_timestamp(timestamp_ms / 1000.0)
+        except OverflowError:
+            warnings.warn(DateOverFlowWarning("Some timestamps are larger than Python datetime can represent. "
+                                              "Timestamps are displayed in milliseconds from epoch."))
+            return timestamp_ms
+
+    cassandra.cqltypes.DateType.deserialize = staticmethod(deserialize_date_fallback_int)
+
+    if hasattr(cassandra, 'deserializers'):
+        del cassandra.deserializers.DesDateType
+
+    # Return cassandra.cqltypes.EMPTY instead of None for empty values
+    cassandra.cqltypes.CassandraType.support_empty_values = True
+
+
+def main(cmdline, pkgpath):
+    insert_driver_hooks()
+    (options, hostname, port) = read_options(cmdline)
+
+    setup_docspath(pkgpath)
     setup_cqlruleset(options.cqlmodule)
     setup_cqldocs(options.cqlmodule)
     init_history()
     csv.field_size_limit(options.field_size_limit)
 
     if options.file is None:
         stdin = None
     else:
         try:
             encoding, bom_size = get_file_encoding_bomsize(options.file)
             stdin = codecs.open(options.file, 'r', encoding)
             stdin.seek(bom_size)
-        except IOError, e:
+        except IOError as e:
             sys.exit("Can't open %r: %s" % (options.file, e))
 
     if options.debug:
         sys.stderr.write("Using CQL driver: %s\n" % (cassandra,))
         sys.stderr.write("Using connect timeout: %s seconds\n" % (options.connect_timeout,))
         sys.stderr.write("Using '%s' encoding\n" % (options.encoding,))
         sys.stderr.write("Using ssl: %s\n" % (options.ssl,))
@@ -2402,60 +2287,67 @@
         try:
             from tzlocal import get_localzone
             timezone = get_localzone()
         except ImportError:
             # we silently ignore and fallback to UTC unless a custom timestamp format (which likely
             # does contain a TZ part) was specified
             if options.time_format != DEFAULT_TIMESTAMP_FORMAT:
-                sys.stderr.write("Warning: custom timestamp format specified in cqlshrc, but local timezone could not be detected.\n" +
-                                 "Either install Python 'tzlocal' module for auto-detection or specify client timezone in your cqlshrc.\n\n")
+                sys.stderr.write("Warning: custom timestamp format specified in cqlshrc, "
+                                 + "but local timezone could not be detected.\n"
+                                 + "Either install Python 'tzlocal' module for auto-detection "
+                                 + "or specify client timezone in your cqlshrc.\n\n")
 
     try:
         shell = Shell(hostname,
                       port,
                       color=options.color,
                       username=options.username,
-                      password=options.password,
                       stdin=stdin,
                       tty=options.tty,
                       completekey=options.completekey,
                       browser=options.browser,
                       protocol_version=options.protocol_version,
                       cqlver=options.cqlversion,
                       keyspace=options.keyspace,
-                      no_compact=options.no_compact,
                       display_timestamp_format=options.time_format,
                       display_nanotime_format=options.nanotime_format,
                       display_date_format=options.date_format,
                       display_float_precision=options.float_precision,
                       display_double_precision=options.double_precision,
                       display_timezone=timezone,
                       max_trace_wait=options.max_trace_wait,
                       ssl=options.ssl,
                       single_statement=options.execute,
                       request_timeout=options.request_timeout,
                       connect_timeout=options.connect_timeout,
-                      encoding=options.encoding)
+                      encoding=options.encoding,
+                      auth_provider=authproviderhandling.load_auth_provider(
+                          config_file=CONFIG_FILE,
+                          cred_file=options.credentials,
+                          username=options.username,
+                          password=options.password))
     except KeyboardInterrupt:
         sys.exit('Connection aborted.')
-    except CQL_ERRORS, e:
+    except CQL_ERRORS as e:
         sys.exit('Connection error: %s' % (e,))
-    except VersionNotSupported, e:
+    except VersionNotSupported as e:
         sys.exit('Unsupported CQL version: %s' % (e,))
     if options.debug:
         shell.debug = True
+    if options.coverage:
+        shell.coverage = True
+        import signal
+
+        def handle_sighup():
+            shell.stop_coverage()
+            shell.do_exit()
+
+        signal.signal(signal.SIGHUP, handle_sighup)
 
     shell.cmdloop()
     save_history()
 
     if shell.batch_mode and shell.statement_error:
         sys.exit(2)
 
 
-# always call this regardless of module name: when a sub-process is spawned
-# on Windows then the module name is not __main__, see CASSANDRA-9304
-insert_driver_hooks()
-
-if __name__ == '__main__':
-    main(*read_options(sys.argv[1:], os.environ))
-
 # vim: set ft=python et ts=4 sw=4 :
```

## Comparing `cqlsh_expansion-0.7.8.dist-info/LICENSE.txt` & `cqlsh_expansion-0.9.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `cqlsh_expansion-0.7.8.dist-info/METADATA` & `cqlsh_expansion-0.9.0.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,53 @@
 Metadata-Version: 2.1
 Name: cqlsh-expansion
-Version: 0.7.8
+Version: 0.9.0
 Summary: The cqlsh-expansion utility extends native cqlsh functionality to include parameters and capabilities specific to Amazon Keyspaces such as support for Sigv4 Authentication.
 Home-page: https://github.com/aws-samples/amazon-keyspaces-toolkit/tree/master/cqlsh-expansion
-License: UNKNOWN
 Keywords: cql,cqlsh,cqlsh-expansion,amazon-keyspaces,ApacheCassandra
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Requires-Python: ~=2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: <3.8
 Description-Content-Type: text/markdown
+License-File: THIRD-PARTY-LICENSES.txt
+License-File: LICENSE.txt
 Requires-Dist: futures (>=2.1.6)
 Requires-Dist: six (>=1.15.0)
-Requires-Dist: urllib3 (>=1.26.2)
-Requires-Dist: python-dateutil (>=2.8.1)
-Requires-Dist: cassandra-driver (<3.18.0,>=3.12.0)
+Requires-Dist: urllib3
+Requires-Dist: python-dateutil
+Requires-Dist: cassandra-driver (>=3.25.0)
 Requires-Dist: botocore
 Requires-Dist: boto3
 Requires-Dist: cassandra-sigv4 (>=4.0.2)
 
+
 # The Amazon Keyspaces (for Apache Cassandra) developer toolkit cqlsh-expansion script
 
 The Amazon Keyspaces toolkit contains common Cassandra tooling and helpers preconfigured for Amazon Keyspaces. The cqlsh-expansion utility extends native cqlsh functionality to include parameters and capabilities specific to Amazon Keyspaces without breaking compatibility with Apache Cassandra. This includes support for the Sigv4 Authentication plugin. Normally, cqlsh is packaged with the full distribution of Apache Cassandra, but since Amazon Keyspaces is a serverless database service, we only require the cqlsh scripts and not the full distribution. This repository provides a lightweight distribution of cqlsh that can be installed on platforms that support python. 
 
 
 ## Installing cqlsh-expansion
 
 To install the cqlsh-expansion python package you can run the following pip command. The command below executes a “pip install” that will install the cqlsh-expansion scripts. It will also install a requirements file containing a list of dependencies. The --`user` flag tells pip to use the Python *user install directory* for your platform. Typically ~/.local/ on unix based systems. 
 
 ```
-
 pip install --user cqlsh-expansion 
-
 ```
 
 Alternatively, if you are using python3 as default you may have to use the following command to install the cqlsh-expansion package. 
 
 ```
-
-python2 -m pip install --user cqlsh-expansion
-
+python3 -m pip install --user cqlsh-expansion
 ```
 
-
-
 ## Setup cqlsh-expansion to connect to Amazon Keyspaces
 
 To use the cqlsh-expansion with Amazon Keyspaces you can use the following post install script or by following the instructions found in the official [Amazon Keyspaces documentation.](https://docs.aws.amazon.com/keyspaces/latest/devguide/programmatic.cqlsh.html) 
 
 By default the cqlsh-expansion is not configured with ssl enabled, but the package includes a [post install script](https://github.com/aws-samples/amazon-keyspaces-toolkit/blob/master/cqlsh-expansion/config/post_install.py) helper to quickly setup your environment after installation. The script will place the necessary configuration and SSL certificate in the user’s *.cassandra* directory. Amazon Keyspaces only accepts secure connections using Transport Layer Security (TLS). Encryption in transit provides an additional layer of data protection by encrypting your data as it travels to and from Amazon Keyspaces. The post install script first will create the .cassandra directory if it does not exist already. Then it will copy a [preconfigure a cqlshrc file](https://github.com/aws-samples/amazon-keyspaces-toolkit/blob/master/cqlsh-expansion/config/cqlshrc_template) and the Starfield digital certificate into the .cassandra directory. The .cassandra directory will be created in the user home directory as it is the default location. As best practice, please review the [post install script](https://github.com/aws-samples/amazon-keyspaces-toolkit/blob/master/cqlsh-expansion/config/post_install.py)before executing. Modifications made by this post install script will not be undone if uninstalling the cqlsh-expansion with pip. 
 
 ```
@@ -65,62 +61,72 @@
 Now that you have you cqlsh-expansion installed and have setup up the configuration for SSL communication with Amazon Keyspaces, you can now connect to the Amazon Keyspaces services using your IAM access keys or Service Specific Credentials. 
 
 ### Choose a region and endpoint
 
 To connect to Amazon Keyspaces you will need to choose one of the [service endpoints](https://docs.aws.amazon.com/keyspaces/latest/devguide/programmatic.endpoints.html). You can also connect to Amazon Keyspaces using [Interface VPC endpoints](https://docs.aws.amazon.com/keyspaces/latest/devguide/vpc-endpoints.html) to enable private communication between your virtual private cloud (VPC) running in Amazon VPC and Amazon Keyspaces. For example, to connect to the Keyspaces service in US East (N. Virginia) (us-east-1) you will want to use the [cassandra.us-east-1.amazonaws.com](http://cassandra.us-east-1.amazonaws.com/) service endpoint.  All communication with Amazon Keyspaces will be over port 9142. 
 
 ### Choose authentication method and connect
-
- To provide users and applications with credentials for programmatic access to Amazon Keyspaces resources, you can do either of the following:
+To provide users and applications with credentials for programmatic access to Amazon Keyspaces resources, you can do either of the following:
 
 #### Connect with IAM access keys (users,roles, and federated identities)
 
-For enhanced security, we recommend to create IAM access keys for IAM users and roles that are used across all AWS services. To use IAM access keys to connect to Amazon Keyspaces, customers can use the Signature Version 4 Process (SigV4) authentication plugin for Cassandra client drivers. To learn more about how the Amazon Keyspaces SigV4 plugin enables [IAM users, roles, and federated identities](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles.html) to authenticate in Amazon Keyspaces API requests, see [AWS Signature Version 4 process (SigV4)](https://docs.aws.amazon.com/general/latest/gr/signature-version-4.html). You can use the Sigv4 plugin with the cqlsh-expansion script by providing the following flag. . `--auth-provider "SigV4AuthProvider"` . The Sigv4 plugin depends on the AWS SDK for Python (Boto3) which is included in the requirements file.  You will also need to set the the proper credentials to make service calls. You can use the following tutorial to [setup credentials using the AWS CLI.](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) 
+For enhanced security, we recommend to create IAM access keys for IAM users and roles that are used across all AWS services. To use IAM access keys to connect to Amazon Keyspaces, customers can use the Signature Version 4 Process (SigV4) authentication plugin for Cassandra client drivers. To learn more about how the Amazon Keyspaces SigV4 plugin enables [IAM users, roles, and federated identities](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles.html) to authenticate in Amazon Keyspaces API requests, see [AWS Signature Version 4 process (SigV4)](https://docs.aws.amazon.com/general/latest/gr/signature-version-4.html). 
 
 After you have the credentials setup with [privileges](https://docs.aws.amazon.com/keyspaces/latest/devguide/security_iam_service-with-iam.html) to access Amazon Keyspaces system tables, you can execute the following command to connect to Amazon Keyspaces with CQLSH using the Sigv4 process.  
 
-```
+Validate the module name and classname, region_name based on keyspaces endpoint in cqlshrc file. 
 
-cqlsh-expansion cassandra.us-east-1.amazonaws.com 9142 --ssl --auth-provider "SigV4AuthProvider"
+```
+[auth_provider]
+;; you can specify any auth provider found in your python environment
+;; module and class will be used to dynamically load the class
+;; all other properties found here and in the credentials file under the class name
+;; will be passed to the constructor
+module = cassandra_sigv4.auth
+classname = SigV4AuthProvider
+region_name = us-east-1
+```
+you can also set region as Environment variable
 
 ```
+ export AWS_DEFAULT_REGION = us-east-1
+```
 
+To connect to Amazon Keyspaces with cqlsh-expansion using Sigv4 authenticator.  
+```
+cqlsh-expansion cassandra.us-east-1.amazonaws.com 
+```
 
 #### Connect with service-specific credentials
 
-You can create service-specific credentials that are similar to the traditional username and password that Cassandra uses for authentication and access management. AWS service-specific credentials are associated with a specific AWS Identity and Access Management (IAM) user and can only be used for the service they were created for. For more information, see [Using IAM with Amazon Keyspaces (for Apache Cassandra)](http://using%20iam%20with%20amazon%20keyspaces%20%28for%20apache%20cassandra%29/) in the IAM User Guide. To connect to Amazon Keyspaces using the cqlsh-expansion and IAM service-specific credentials you can use the command below. In this command we are connecting to us-east-1 region with service specific user *‘mike-user-99’ *and service specific user password* ‘user-pass-01’. *You will need to replace these credentials with your own user name and password that were given to you when creating the service specific credentials. 
+You can create service-specific credentials that are similar to the traditional username and password that Cassandra uses for authentication and access management. AWS service-specific credentials are associated with a specific AWS Identity and Access Management (IAM) user and can only be used for the service they were created for. For more information, see [Using IAM with Amazon Keyspaces (for Apache Cassandra)](http://using%20iam%20with%20amazon%20keyspaces%20%28for%20apache%20cassandra%29/) in the IAM User Guide. To connect to Amazon Keyspaces using the cqlsh-expansion and IAM service-specific credentials you can use the command below. In this command we are connecting to us-east-1 region with service specific user *‘Sri-user-99’ *and service specific user password* ‘user-pass-01’. *You will need to replace these credentials with your own user name and password that were given to you when creating the service specific credentials. 
 
-```
-
-cqlsh-expansion cassandra.us-east-1.amazonaws.com 9142 --ssl -u mike-user-99 -p user-pass-01
 
 ```
-
-Alternatively, if you want to use the cqlsh without the additional functionality included in the cqlsh-expansion package you can execute the following. 
-
+[auth_provider]
+;; you can specify any auth provider found in your python environment
+;; module and class will be used to dynamically load the class
+;; all other properties found here and in the credentials file under the class name
+;; will be passed to the constructor
+module = cassandra.auth
+classname = PlainTextAuthProvider
 ```
 
-cqlsh cassandra.us-east-1.amazonaws.com 9142 --ssl -u mike-user-99 -p user-pass-01
-
 ```
+cqlsh-expansion cassandra.us-east-1.amazonaws.com -u Sri-user-99 -p user-pass-01
+```
+
 
 ## Cleanup
 To remove the cqlsh-expansion package you can use the pip uninstall api. Additionally, if you executed the post install script ```cqlsh-expansion.init```, you may want to delete the .cassandra directory which contains the cqlshrc file and the ssl certificate. Using pip uninstall will not remove changes made by the post install script. 
 
 ```
 pip uninstall cqlsh-expansion
-
 ```
 
-## Functional differences from CQLSH
-
-### Sigv4 authentication
-
-Instead of using the service specific credentials for an IAM user, you can use the `--auth-provider "SigV4AuthProvider"` parameter to leverage the Sigv4 authentication plugin for temporary credentials. This plugin enables IAM users, roles, and federated identities to add authentication information to Amazon Keyspaces (for Apache Cassandra) API requests using the AWS Signature Version 4 Process (SigV4). The plugin depends on the AWS SDK for Python (Boto3) and the [Amazon Keyspaces Sigv4 plugin for the DataStax python driver](https://github.com/aws/aws-sigv4-auth-cassandra-python-driver-plugin).
-
 ### New output for TTY
 
 When creating a new cqlsh session with the cqlsh-expansion utility, it will show the default consistency level after establishing a new connection. We find customers using cqlsh may not be aware of the default consistency level of `ONE`, and additional transparency will lead to better operational excellence.
 
 ### COPY FROM/TO required Consistency Levels
 
 When executing the `COPY FROM` import operation from the cqlsh-expansion utility, `LOCAL_QUORUM` will be strictly enforced. Executing `COPY FROM` with consistency level other than LOCAL_QUORUM will result in an SyntaxError. This restriction is to provide better experience when using `COPY FROM` with Amazon Keyspaces. Amazon Keyspaces replicates all write operations three times across multiple Availability Zones for durability and high availability. Writes are durably stored before they are acknowledged using the `LOCAL_QUORUM` consistency level.
@@ -135,9 +141,7 @@
 See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.
 
 # License
 
 This library is licensed under the MIT-0 License. See the LICENSE file.
 ```
 
-
-
```

## Comparing `cqlsh_expansion-0.7.8.dist-info/THIRD-PARTY-LICENSES.txt` & `cqlsh_expansion-0.9.0.dist-info/THIRD-PARTY-LICENSES.txt`

 * *Files identical despite different names*

