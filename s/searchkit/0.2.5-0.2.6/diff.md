# Comparing `tmp/searchkit-0.2.5.tar.gz` & `tmp/searchkit-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchkit-0.2.5.tar", last modified: Mon May 15 14:27:28 2023, max compression
+gzip compressed data, was "searchkit-0.2.6.tar", last modified: Wed May 24 11:46:36 2023, max compression
```

## Comparing `searchkit-0.2.5.tar` & `searchkit-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-15 14:27:28.015197 searchkit-0.2.5/
--rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.2.5/LICENSE
--rw-rw-r--   0 user1     (1000) user1     (1000)     3105 2023-05-15 14:27:28.015197 searchkit-0.2.5/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)     2897 2023-04-12 11:04:01.000000 searchkit-0.2.5/README.md
--rw-rw-r--   0 user1     (1000) user1     (1000)      734 2023-05-11 09:19:48.000000 searchkit-0.2.5/pyproject.toml
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-15 14:27:28.015197 searchkit-0.2.5/searchkit/
--rw-rw-r--   0 user1     (1000) user1     (1000)      121 2023-05-11 09:19:48.000000 searchkit-0.2.5/searchkit/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    26546 2023-05-15 14:26:31.000000 searchkit-0.2.5/searchkit/constraints.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-29 21:35:16.000000 searchkit-0.2.5/searchkit/log.py
--rwxrwxr-x   0 user1     (1000) user1     (1000)    49277 2023-05-11 09:19:48.000000 searchkit-0.2.5/searchkit/search.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5726 2023-05-15 14:26:31.000000 searchkit-0.2.5/searchkit/utils.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-15 14:27:28.015197 searchkit-0.2.5/searchkit.egg-info/
--rw-rw-r--   0 user1     (1000) user1     (1000)     3105 2023-05-15 14:27:28.000000 searchkit-0.2.5/searchkit.egg-info/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)      308 2023-05-15 14:27:28.000000 searchkit-0.2.5/searchkit.egg-info/SOURCES.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-05-15 14:27:28.000000 searchkit-0.2.5/searchkit.egg-info/dependency_links.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-05-15 14:27:28.000000 searchkit-0.2.5/searchkit.egg-info/requires.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       10 2023-05-15 14:27:28.000000 searchkit-0.2.5/searchkit.egg-info/top_level.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       38 2023-05-15 14:27:28.015197 searchkit-0.2.5/setup.cfg
--rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.2.5/setup.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-24 11:46:36.675693 searchkit-0.2.6/
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.2.6/LICENSE
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4352 2023-05-24 11:46:36.675693 searchkit-0.2.6/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4144 2023-05-24 11:46:12.000000 searchkit-0.2.6/README.md
+-rw-rw-r--   0 user1     (1000) user1     (1000)      734 2023-05-18 09:56:58.000000 searchkit-0.2.6/pyproject.toml
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-24 11:46:36.675693 searchkit-0.2.6/searchkit/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      121 2023-05-22 10:26:50.000000 searchkit-0.2.6/searchkit/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    29452 2023-05-24 11:46:12.000000 searchkit-0.2.6/searchkit/constraints.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-29 21:35:16.000000 searchkit-0.2.6/searchkit/log.py
+-rwxrwxr-x   0 user1     (1000) user1     (1000)    49277 2023-05-22 09:42:32.000000 searchkit-0.2.6/searchkit/search.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5726 2023-05-16 10:48:26.000000 searchkit-0.2.6/searchkit/utils.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-24 11:46:36.675693 searchkit-0.2.6/searchkit.egg-info/
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4352 2023-05-24 11:46:36.000000 searchkit-0.2.6/searchkit.egg-info/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)      308 2023-05-24 11:46:36.000000 searchkit-0.2.6/searchkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-05-24 11:46:36.000000 searchkit-0.2.6/searchkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-05-24 11:46:36.000000 searchkit-0.2.6/searchkit.egg-info/requires.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       10 2023-05-24 11:46:36.000000 searchkit-0.2.6/searchkit.egg-info/top_level.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       38 2023-05-24 11:46:36.675693 searchkit-0.2.6/setup.cfg
+-rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.2.6/setup.py
```

### Comparing `searchkit-0.2.5/LICENSE` & `searchkit-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.5/PKG-INFO` & `searchkit-0.2.6/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: searchkit
-Version: 0.2.5
-Summary: Python library providing tools to search files in parallel.
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Searchkit
 
 Python library providing tools to search files in parallel.
 
 ## Search Types
 
 Different types of search are supported. Add one or more search definition to a `FileSearcher` object, registering them against a file, directory or glob path. Results are collected and returned as a `SearchResultsCollection` which provides different ways to retrieve results.
@@ -66,14 +58,18 @@
     cmd = r.CMD
 ```
 
 ### Sequence Search
 
 The `SequenceSearchDef` class supports matching string sequences ("sections") over multiple lines by matching a start, end and optional body in between. These section components are each defined with their own `SearchDef` object.
 
+### Search Constraints
+
+If searching e.g. a log file where each line starts with a timestamp and you only want results that match after a specific time then you can use ```search.constraints.SearchConstraintSearchSince``` and apply to either the whole file or each line in turn. The latter allows constraints to be associated with a SearchDef and therefore only apply within the context of that search.
+
 ## Installation
 
 searchkit is packaged in [pypi](https://pypi.org/project/searchkit) and can be installed as follows:
 
 ```console
 sudo apt install python3-pip
 pip install searchkit
@@ -116,7 +112,33 @@
 fs.add(SequenceSearchDef(start, tag='myseq', body=body), fname)
 results = fs.run()
 for seq, results in results.find_sequence_by_tag('myseq').items():
     for r in results:
         if 'body' in r.tag:
             print(r.get(0))
 ```
+
+An example search with constraints is as follows:
+
+```python
+from searchkit import FileSearcher, SearchDef
+from searchkit.constraints import SearchConstraintSearchSince, DateTimeMatcherBase
+
+class MyDateTimeMatcher(DateTimeMatcherBase):
+    EXPRS = [r'^(?P<year>\d{4})-(?P<month>\d{2})-(?P<day>\d{2}) '
+             r'(?P<hours>\d{2}):(?P<minutes>\d{2}):(?P<seconds>\d{2})']
+
+fname = 'foo.txt'
+with open(fname, 'w') as fd:
+  fd.write('2023-01-01 12:34:24 feeling cold\n')
+  fd.write('2023-06-01 12:34:24 feeling hot')
+
+today = '2023-06-02 12:34:24'
+constraint = SearchConstraintSearchSince(today, None,
+                                         MyDateTimeMatcher)
+fs = FileSearcher(constraint=constraint)
+fs.add(SearchDef(r'\S+ \S+ \S+ (\S+)'), fname)
+results = fs.run()
+for r in results.find_by_path(fname):
+    print(r.get(1) == 'hot')
+```
+
```

### Comparing `searchkit-0.2.5/pyproject.toml` & `searchkit-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.5/searchkit/constraints.py` & `searchkit-0.2.6/searchkit/constraints.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,79 @@
 from datetime import datetime, timedelta
 from functools import cached_property
 
 from searchkit.utils import MPCacheSharded
 from searchkit.log import log
 
 
+class TimestampMatcherBase(object):
+    """
+    Match start of line timestamps in a standard way.
+
+    Files containing lines starting with timestamps allow us to find a line
+    that is before/after a specific time. This class is implemented to provides
+    a common way to identify timestamps of varying format.
+    """
+
+    # used when converting a string to datetime.datetime
+    DEFAULT_DATETIME_FORMAT = '%Y-%m-%d %H:%M:%S'
+
+    def __init__(self, line):
+        self.result = None
+        for expr in self.patterns:
+            ret = re.match(expr, line)
+            if ret:
+                self.result = ret
+                break
+        else:
+            log.debug("failed to identify constraint datetime")
+
+    @property
+    @abc.abstractmethod
+    def patterns(self):
+        """
+        List of regex patterns used to match a timestamp at the start of lines.
+
+        Patterns *must* use named groups according to types i.e. year,
+        month etc. See https://docs.python.org/3/library/re.html for format
+        options.
+
+        If the format of the timestamp is non-standard and the result needs
+        post-processing before being used, a property with the group name
+        can be added to implementations of this class and that will be used
+        rather than extracting the value directly from the result.
+        """
+
+    @property
+    def matched(self):
+        """ Return True if a timestamp has been matched. """
+        return self.result is not None
+
+    @property
+    def strptime(self):
+        """
+        Converts the extracted timestamp into a datetime.datetime object.
+
+        Group names are extracted directly from the result unless an override
+        property has been defined.
+
+        @return: datetime.datetime object
+        """
+        vals = {}
+        for key in ['day', 'month', 'year', 'hours', 'minutes', 'seconds']:
+            if hasattr(self, key):
+                vals[key] = getattr(self, key)
+            else:
+                vals[key] = self.result.group(key)
+
+        _date = ("{year}-{month}-{day} {hours}:{minutes}:{seconds}".
+                 format(**vals))
+        return datetime.strptime(_date, self.DEFAULT_DATETIME_FORMAT)
+
+
 class ConstraintBase(abc.ABC):
 
     @cached_property
     def id(self):
         """
         A unique identifier for this constraint.
         """
@@ -401,18 +466,18 @@
     def __init__(self, allow_constraints_for_unverifiable_logs=True):
         self.fd_info = None
         self.allow_unverifiable_logs = allow_constraints_for_unverifiable_logs
 
     @abc.abstractmethod
     def extracted_datetime(self, line):
         """
-        Extract datetime from line. Returns a datetime object or None if unable
-        to extract one from the line.
+        Extract timestamp from start of line.
 
         @param line: text line to extract a datetime from.
+        @return: datetime.datetime object or None
         """
 
     @abc.abstractproperty
     def _since_date(self):
         """ A datetime.datetime object representing the "since" date/time """
 
     def _line_date_is_valid(self, extracted_datetime):
@@ -618,58 +683,72 @@
                   self.fd_info.fd.tell(), offset, self.fd_info.iterations)
 
         return offset
 
 
 class SearchConstraintSearchSince(BinarySeekSearchBase):
 
-    def __init__(self, current_date, cache_path, exprs=None, days=0, hours=24,
-                 **kwargs):
+    def __init__(self, current_date, cache_path, exprs=None,
+                 ts_matcher_cls=None, days=0, hours=24, **kwargs):
         """
         A search expression is provided that allows us to identify a datetime
         on each line and check whether it is within a given time period. The
         time period used defaults to 24 hours if use_all_logs is false, 7 days
         if it is true and max_logrotate_depth is default otherwise whatever
         value provided. This can be overridden by providing a specific number
         of hours.
 
         @param current_date: cli.date(format="+{}".format(self.date_format))
-        @param exprs: a list of search/regex expressions used to identify a
-                      date/time in.
-        each line in the file we are applying this constraint to.
+        @param cache_path: path to location where we can create an MPCache
+        @param exprs: [DEPRECATED] a list of search/regex expressions used to
+                      identify a date/time in. This is deprecated, use
+                      ts_matcher_cls.
+        @param ts_matcher_cls: TimestampMatcherBase implementation used to
+                               match timestamps at start if lines.
         @param days: override default period with number of days
         @param hours: override default period with number of hours
         """
         super().__init__(**kwargs)
         self.cache_path = cache_path
-        self.date_format = '%Y-%m-%d %H:%M:%S'
+        self.ts_matcher_cls = ts_matcher_cls
+        if ts_matcher_cls:
+            self.date_format = ts_matcher_cls.DEFAULT_DATETIME_FORMAT
+        else:
+            log.warning("using patterns to identify timestamp is deprecated - "
+                        "use ts_matcher_cls instead")
+            self.date_format = TimestampMatcherBase.DEFAULT_DATETIME_FORMAT
+
         self.current_date = datetime.strptime(current_date, self.date_format)
         self._line_pass = 0
         self._line_fail = 0
         self.exprs = exprs
         self.days = days
         if days:
             self.hours = 0
         else:
             self.hours = hours
 
         self._results = {}
 
     def extracted_datetime(self, line):
-        """
-        Validate if the given line falls within the provided constraint. In
-        this case that's whether it has a datetime that is >= to the "since"
-        date.
-
-        @param line: text line to extract a datetime from.
-        """
         if type(line) == bytes:
             # need this for e.g. gzipped files
             line = line.decode("utf-8")
 
+        if self.ts_matcher_cls:
+            timestamp = self.ts_matcher_cls(line)
+            if timestamp.matched:
+                return timestamp.strptime
+
+            return
+
+        # NOTE: the following code can be removed once we remove the deprecated
+        # exprs arg from this class.
+        log.debug("using patterns to identify timestamp is deprecated - "
+                  "use ts_matcher_cls instead")
         for expr in self.exprs:
             # log.debug("attempting to extract from line using expr '%s'",
             #           expr)
             ret = re.search(expr, line)
             if ret:
                 # log.debug("expr '%s' successful", expr)
                 break
```

### Comparing `searchkit-0.2.5/searchkit/search.py` & `searchkit-0.2.6/searchkit/search.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.5/searchkit/utils.py` & `searchkit-0.2.6/searchkit/utils.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.5/searchkit.egg-info/PKG-INFO` & `searchkit-0.2.6/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Searchkit
 
@@ -66,14 +66,18 @@
     cmd = r.CMD
 ```
 
 ### Sequence Search
 
 The `SequenceSearchDef` class supports matching string sequences ("sections") over multiple lines by matching a start, end and optional body in between. These section components are each defined with their own `SearchDef` object.
 
+### Search Constraints
+
+If searching e.g. a log file where each line starts with a timestamp and you only want results that match after a specific time then you can use ```search.constraints.SearchConstraintSearchSince``` and apply to either the whole file or each line in turn. The latter allows constraints to be associated with a SearchDef and therefore only apply within the context of that search.
+
 ## Installation
 
 searchkit is packaged in [pypi](https://pypi.org/project/searchkit) and can be installed as follows:
 
 ```console
 sudo apt install python3-pip
 pip install searchkit
@@ -116,7 +120,33 @@
 fs.add(SequenceSearchDef(start, tag='myseq', body=body), fname)
 results = fs.run()
 for seq, results in results.find_sequence_by_tag('myseq').items():
     for r in results:
         if 'body' in r.tag:
             print(r.get(0))
 ```
+
+An example search with constraints is as follows:
+
+```python
+from searchkit import FileSearcher, SearchDef
+from searchkit.constraints import SearchConstraintSearchSince, DateTimeMatcherBase
+
+class MyDateTimeMatcher(DateTimeMatcherBase):
+    EXPRS = [r'^(?P<year>\d{4})-(?P<month>\d{2})-(?P<day>\d{2}) '
+             r'(?P<hours>\d{2}):(?P<minutes>\d{2}):(?P<seconds>\d{2})']
+
+fname = 'foo.txt'
+with open(fname, 'w') as fd:
+  fd.write('2023-01-01 12:34:24 feeling cold\n')
+  fd.write('2023-06-01 12:34:24 feeling hot')
+
+today = '2023-06-02 12:34:24'
+constraint = SearchConstraintSearchSince(today, None,
+                                         MyDateTimeMatcher)
+fs = FileSearcher(constraint=constraint)
+fs.add(SearchDef(r'\S+ \S+ \S+ (\S+)'), fname)
+results = fs.run()
+for r in results.find_by_path(fname):
+    print(r.get(1) == 'hot')
+```
+
```

