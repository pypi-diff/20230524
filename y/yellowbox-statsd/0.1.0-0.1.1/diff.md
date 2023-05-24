# Comparing `tmp/yellowbox_statsd-0.1.0.tar.gz` & `tmp/yellowbox_statsd-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowbox_statsd-0.1.0.tar", max compression
+gzip compressed data, was "yellowbox_statsd-0.1.1.tar", max compression
```

## Comparing `yellowbox_statsd-0.1.0.tar` & `yellowbox_statsd-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-05-17 06:36:13.625707 yellowbox_statsd-0.1.0/LICENSE
--rw-r--r--   0        0        0     1512 2023-05-17 06:36:13.625707 yellowbox_statsd-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      144 2023-05-17 06:36:13.625707 yellowbox_statsd-0.1.0/yellowbox_statsd/__init__.py
--rw-r--r--   0        0        0       22 2023-05-17 06:36:13.625707 yellowbox_statsd-0.1.0/yellowbox_statsd/_version.py
--rw-r--r--   0        0        0     7808 2023-05-17 06:36:13.629707 yellowbox_statsd-0.1.0/yellowbox_statsd/metrics.py
--rw-r--r--   0        0        0     2461 2023-05-17 06:36:13.629707 yellowbox_statsd-0.1.0/yellowbox_statsd/statsd.py
--rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 yellowbox_statsd-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-24 15:34:25.891606 yellowbox_statsd-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1597 2023-05-24 15:34:25.891606 yellowbox_statsd-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      144 2023-05-24 15:34:25.891606 yellowbox_statsd-0.1.1/yellowbox_statsd/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-24 15:34:25.891606 yellowbox_statsd-0.1.1/yellowbox_statsd/_version.py
+-rw-r--r--   0        0        0     9956 2023-05-24 15:34:25.891606 yellowbox_statsd-0.1.1/yellowbox_statsd/metrics.py
+-rw-r--r--   0        0        0     4872 2023-05-24 15:34:25.891606 yellowbox_statsd-0.1.1/yellowbox_statsd/statsd.py
+-rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 yellowbox_statsd-0.1.1/PKG-INFO
```

### Comparing `yellowbox_statsd-0.1.0/LICENSE` & `yellowbox_statsd-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowbox_statsd-0.1.0/pyproject.toml` & `yellowbox_statsd-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yellowbox-statsd"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Biocatch LTD <serverteam@biocatch.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 yellowbox = { version = ">=0.7.0" }
@@ -20,14 +20,16 @@
 [tool.ruff]
 # https://beta.ruff.rs/docs/rules/
 select = ["I", "E", "W", "F", "N", "S", "BLE", "COM", "C4", "ISC", "ICN", "G", "PIE", "T20", "PYI", "Q", "SLF", "SIM",
           "ERA", "PGH", "PLC", "PLE", "PLR", "PLW", "RUF", "PT", "UP", "B"]
 ignore = [
     "COM812",  # trailing comma, handled by black
     "UP035",  # deprecated imports
+    "PLR0912", # Too many branches
+    "S104",  # Possible binding to all interfaces
 ]
 line-length = 120
 show-source = true
 
 [tool.ruff.isort]
 combine-as-imports=true
```

### Comparing `yellowbox_statsd-0.1.0/yellowbox_statsd/metrics.py` & `yellowbox_statsd-0.1.1/yellowbox_statsd/metrics.py`

 * *Files 20% similar despite different names*

```diff
@@ -119,14 +119,28 @@
         return cls(metric.values, metric.sample_rate, metric.tags, metric.metric_timestamp, metric.container_id)
 
 
 Self = TypeVar("Self", bound="CapturedMetrics")
 
 
 class CapturedMetrics(List[CapturedMetric]):
+    def tags(self) -> Iterable[str]:
+        s: Set[str] = set()
+        for m in self:
+            if m.tags is not None:
+                s.update(m.tags)
+        return sorted(s)
+
+    def tag_values(self, tag: str) -> Iterable[str]:
+        s: Set[str] = set()
+        for m in self:
+            if m.tags is not None:
+                s.update(m.tags[tag])
+        return sorted(s)
+
     def filter(
         self: Self, *extra_tags, tags: Union[Iterable[str], Mapping[str, str]] = (), **extra_tags_assigned
     ) -> Self:
         return type(self)(m for m in self if m.tags_match(*extra_tags, tags=tags, **extra_tags_assigned))
 
     def filter_not(
         self: Self, *extra_tags, tags: Union[Iterable[str], Mapping[str, str]] = (), **extra_tags_assigned
@@ -218,24 +232,63 @@
         key = metric.name, metric.type
         if key not in self:
             capture_cls = self.METRIC_TYPES_TO_CLASS.get(metric.type, CapturedMetrics)
             self[key] = capture_cls()
         m = CapturedMetric.from_metric(metric)
         self[key].append(m)
 
+    def __getitem__(self, key: Tuple[str, str]) -> CapturedMetrics:
+        try:
+            return super().__getitem__(key)
+        except KeyError:
+            if self:
+                raise KeyError(
+                    f"Metric {key[0]} of type {key[1]} not found, available metrics: {sorted(self.keys())}"
+                ) from None
+            else:
+                raise
+
     def count(self, name: str) -> CountCapturedMetric:
         return self[name, "c"]  # type: ignore[return-value]
 
+    def get_count(self, name: str, tags=(), **tags_kwargs) -> CountCapturedMetric:
+        return self.get((name, "c"), CountCapturedMetric()).filter(
+            tags=tags, **tags_kwargs
+        )  # type: ignore[return-value]
+
     def gauge(self, name: str) -> GaugeCapturedMetric:
         return self[name, "g"]  # type: ignore[return-value]
 
+    def get_gauge(self, name: str, tags=(), **tags_kwargs) -> GaugeCapturedMetric:
+        return self.get((name, "g"), GaugeCapturedMetric()).filter(
+            tags=tags, **tags_kwargs
+        )  # type: ignore[return-value]
+
     def histogram(self, name: str) -> HistogramCapturedMetric:
         return self[name, "h"]  # type: ignore[return-value]
 
+    def get_histogram(self, name: str, tags=(), **tags_kwargs) -> HistogramCapturedMetric:
+        return self.get((name, "h"), HistogramCapturedMetric()).filter(
+            tags=tags, **tags_kwargs
+        )  # type: ignore[return-value]
+
     def set(self, name: str) -> SetCapturedMetric:
         return self[name, "s"]  # type: ignore[return-value]
 
+    def get_set(self, name: str, tags=(), **tags_kwargs) -> SetCapturedMetric:
+        return self.get((name, "s"), SetCapturedMetric()).filter(tags=tags, **tags_kwargs)  # type: ignore[return-value]
+
     def timing(self, name: str) -> HistogramCapturedMetric:
         return self[name, "ms"]  # type: ignore[return-value]
 
+    def get_timing(self, name: str, tags=(), **tags_kwargs) -> HistogramCapturedMetric:
+        return self.get((name, "ms"), HistogramCapturedMetric()).filter(
+            tags=tags, **tags_kwargs
+        )  # type: ignore[return-value]
+
     def distribution(self, name: str) -> HistogramCapturedMetric:
         return self[name, "d"]  # type: ignore[return-value]
+
+    def get_distribution(self, name: str, tags=(), **tags_kwargs) -> HistogramCapturedMetric:
+        return self.get((name, "d"), HistogramCapturedMetric()).filter(
+            tags=tags, **tags_kwargs
+        )  # type: ignore[return-value]
```

### Comparing `yellowbox_statsd-0.1.0/PKG-INFO` & `yellowbox_statsd-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowbox-statsd
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: Biocatch LTD
 Author-email: serverteam@biocatch.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

