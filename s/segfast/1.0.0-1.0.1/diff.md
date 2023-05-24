# Comparing `tmp/segfast-1.0.0.tar.gz` & `tmp/segfast-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segfast-1.0.0.tar", last modified: Wed Apr  5 11:31:33 2023, max compression
+gzip compressed data, was "segfast-1.0.1.tar", last modified: Wed May 24 13:48:35 2023, max compression
```

## Comparing `segfast-1.0.0.tar` & `segfast-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 11:31:33.876258 segfast-1.0.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-05 11:31:21.000000 segfast-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      795 2023-04-05 11:31:33.876258 segfast-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      204 2023-04-05 11:31:21.000000 segfast-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 11:31:33.876258 segfast-1.0.0/segfast/
--rw-r--r--   0 root         (0) root         (0)      214 2023-04-05 11:31:21.000000 segfast-1.0.0/segfast/__init__.py
--rw-r--r--   0 root         (0) root         (0)      739 2023-04-05 11:31:21.000000 segfast-1.0.0/segfast/loader.py
--rwxr-xr-x   0 root         (0) root         (0)    21887 2023-04-05 11:31:21.000000 segfast-1.0.0/segfast/memmap_loader.py
--rwxr-xr-x   0 root         (0) root         (0)    13980 2023-04-05 11:31:21.000000 segfast-1.0.0/segfast/segyio_loader.py
--rw-r--r--   0 root         (0) root         (0)     1797 2023-04-05 11:31:21.000000 segfast-1.0.0/segfast/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 11:31:33.876258 segfast-1.0.0/segfast.egg-info/
--rw-r--r--   0 root         (0) root         (0)      795 2023-04-05 11:31:33.000000 segfast-1.0.0/segfast.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      315 2023-04-05 11:31:33.000000 segfast-1.0.0/segfast.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 11:31:33.000000 segfast-1.0.0/segfast.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 11:31:33.000000 segfast-1.0.0/segfast.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       70 2023-04-05 11:31:33.000000 segfast-1.0.0/segfast.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-05 11:31:33.000000 segfast-1.0.0/segfast.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-05 11:31:33.876258 segfast-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1223 2023-04-05 11:31:21.000000 segfast-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:48:35.492240 segfast-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-24 13:48:22.000000 segfast-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3786 2023-05-24 13:48:35.492240 segfast-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3196 2023-05-24 13:48:22.000000 segfast-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:48:35.488240 segfast-1.0.1/segfast/
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-24 13:48:22.000000 segfast-1.0.1/segfast/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      739 2023-05-24 13:48:22.000000 segfast-1.0.1/segfast/loader.py
+-rwxr-xr-x   0 root         (0) root         (0)    21599 2023-05-24 13:48:22.000000 segfast-1.0.1/segfast/memmap_loader.py
+-rwxr-xr-x   0 root         (0) root         (0)    13578 2023-05-24 13:48:22.000000 segfast-1.0.1/segfast/segyio_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1797 2023-05-24 13:48:22.000000 segfast-1.0.1/segfast/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:48:35.492240 segfast-1.0.1/segfast.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3786 2023-05-24 13:48:35.000000 segfast-1.0.1/segfast.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      315 2023-05-24 13:48:35.000000 segfast-1.0.1/segfast.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 13:48:35.000000 segfast-1.0.1/segfast.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 13:48:35.000000 segfast-1.0.1/segfast.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       70 2023-05-24 13:48:35.000000 segfast-1.0.1/segfast.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-24 13:48:35.000000 segfast-1.0.1/segfast.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 13:48:35.492240 segfast-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1223 2023-05-24 13:48:22.000000 segfast-1.0.1/setup.py
```

### Comparing `segfast-1.0.0/LICENSE` & `segfast-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `segfast-1.0.0/segfast/loader.py` & `segfast-1.0.1/segfast/loader.py`

 * *Files identical despite different names*

### Comparing `segfast-1.0.0/segfast/memmap_loader.py` & `segfast-1.0.1/segfast/memmap_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -219,47 +219,44 @@
         if void_counter:
             unused_dtype = (f'unused_{unused_counter}', np.void, void_counter)
             dtype_list.append(unused_dtype)
         return dtype_list
 
 
     # Data loading
-    def load_traces(self, indices, limits=None, buffer=None, return_samples=False):
+    def load_traces(self, indices, limits=None, buffer=None):
         """ Load traces by their indices.
         Under the hood, we use a pre-made memory mapping over the file, where trace data is viewed with a special dtype.
         Regardless of the numerical dtype of SEG-Y file, we output IEEE float32:
         for IBM floats, that requires an additional conversion.
 
         Parameters
         ----------
         indices : sequence
             Indices (TRACE_SEQUENCE_FILE) of the traces to read.
         limits : sequence of ints, slice, optional
             Slice of the data along the depth axis.
         buffer : np.ndarray, optional
             Buffer to read the data into. If possible, avoids copies.
-        return_samples : bool
-            Whether to return samples of loaded traces in accordance to `limits`.
         """
         limits = self.process_limits(limits)
 
         if self.file_format != 1:
             traces = self.data_mmap[indices, limits]
         else:
             traces = self.data_mmap[indices, limits.start:limits.stop]
             if limits.step != 1:
                 traces = traces[:, ::limits.step]
             traces = self._ibm_to_ieee(traces)
 
         if buffer is None:
-            buffer = np.require(traces, dtype=self.dtype, requirements='C')
-            return buffer if return_samples is False else (buffer, self.samples[limits])
+            return np.require(traces, dtype=self.dtype, requirements='C')
 
         buffer[:len(indices)] = traces
-        return buffer if return_samples is False else (buffer, self.samples[limits])
+        return buffer
 
     def load_depth_slices(self, indices, buffer=None):
         """ Load horizontal (depth) slices of the data.
         Requires a ~full sweep through SEG-Y, therefore is slow.
 
         Parameters
         ----------
```

### Comparing `segfast-1.0.0/segfast/segyio_loader.py` & `segfast-1.0.1/segfast/segyio_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,38 +60,37 @@
         self.file_handler.mmap()
 
         # Number of traces and depth
         self.n_samples = self.file_handler.trace.shape
         self.n_traces = self.file_handler.trace.length
         self.dtype = self.file_handler.dtype
 
-        # Sample interval, rate and delay
-        self.sample_interval = self._infer_sample_interval() # ms
-        self.sample_rate = 1000 / self.sample_interval       # Hz
-        self.samples = np.arange(self.n_samples) * self.sample_interval
-        self.delay = self.file_handler.header[0].get(segyio.TraceField.DelayRecordingTime)
-
         # Misc
         self.metrics = self.file_handler.xfd.metrics()
         self.text = [self.file_handler.text[i] for i in range(1 + self.file_handler.ext_headers)]
 
-
-    def _infer_sample_interval(self):
-        """ Get sample interval from file headers. """
+    @property
+    def sample_interval(self):
+        """ Sample interval of seismic traces. """
         bin_sample_interval = self.file_handler.bin[segyio.BinField.Interval]
         trace_sample_interval = self.file_handler.header[0][segyio.TraceField.TRACE_SAMPLE_INTERVAL]
         # 0 means undefined sample interval, so it is removed from the set
         union_sample_interval = {bin_sample_interval, trace_sample_interval} - {0}
 
         if len(union_sample_interval) != 1:
             raise ValueError("Cannot infer sample interval from file headers: "
                              "either both `Interval` (bytes 3217-3218 in the binary header) "
                              "and `TRACE_SAMPLE_INTERVAL` (bytes 117-118 in the header of the first trace) "
                              "are undefined or they have different values.")
-        return union_sample_interval.pop() / 1000  # convert from microseconds to milliseconds
+        return union_sample_interval.pop()
+
+    @property
+    def delay(self):
+        """ Delay recording time of seismic traces. """
+        return self.file_handler.header[0].get(segyio.TraceField.DelayRecordingTime)
 
 
     # Headers
     def headers_to_bytes(self, headers):
         """ Compute the byte location of a header. """
         return [getattr(segyio.TraceField, header) for header in headers]
 
@@ -156,39 +155,36 @@
     def make_tsf_header(self):
         """ Reconstruct the `TRACE_SEQUENCE_FILE` header. """
         dtype = np.int32 if self.n_traces < np.iinfo(np.int32).max else np.int64
         return np.arange(1, self.n_traces + 1, dtype=dtype)
 
 
     # Data loading: traces
-    def load_traces(self, indices, limits=None, buffer=None, return_samples=False):
+    def load_traces(self, indices, limits=None, buffer=None):
         """ Load traces by their indices.
         By pre-allocating memory for all of the requested traces, we significantly speed up the process.
 
         Parameters
         ----------
         indices : sequence
             Indices (TRACE_SEQUENCE_FILE) of the traces to read.
         limits : sequence of ints, slice, optional
             Slice of the data along the depth axis.
         buffer : np.ndarray, optional
             Buffer to read the data into. If possible, avoids copies.
-        return_samples : bool
-            Whether to return samples of loaded traces in accordance to `limits`.
         """
         limits = self.process_limits(limits)
-        samples = self.samples[limits]
-        n_samples = len(samples)
+        n_samples = len(range(*limits.indices(self.n_samples)))
 
         if buffer is None:
             buffer = np.empty((len(indices), n_samples), dtype=self.dtype)
 
         for i, index in enumerate(indices):
             self.load_trace(index=index, buffer=buffer[i], limits=limits)
-        return buffer if return_samples is False else (buffer, samples)
+        return buffer
 
     def process_limits(self, limits):
         """ Convert given `limits` to a `slice`. """
         if limits is None:
             return slice(0, self.n_samples, 1)
         if isinstance(limits, int):
             limits = slice(limits)
@@ -205,14 +201,15 @@
 
     def load_trace(self, index, buffer, limits):
         """ Load one trace into buffer. """
         self.file_handler.xfd.gettr(buffer, index, 1, 1,
                                     limits.start, limits.stop, limits.step,
                                     buffer.size)
 
+
     # Data loading: depth slices
     def load_depth_slices(self, indices, buffer=None):
         """ Load horizontal (depth) slices of the data.
         Requires a ~full sweep through SEG-Y, therefore is slow.
 
         Parameters
         ----------
```

### Comparing `segfast-1.0.0/segfast/utils.py` & `segfast-1.0.1/segfast/utils.py`

 * *Files identical despite different names*

### Comparing `segfast-1.0.0/setup.py` & `segfast-1.0.1/setup.py`

 * *Files identical despite different names*

