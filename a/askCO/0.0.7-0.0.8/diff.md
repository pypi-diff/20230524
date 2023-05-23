# Comparing `tmp/askCO-0.0.7.tar.gz` & `tmp/askCO-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "askCO-0.0.7.tar", last modified: Tue May 23 04:41:32 2023, max compression
+gzip compressed data, was "askCO-0.0.8.tar", last modified: Tue May 23 23:37:07 2023, max compression
```

## Comparing `askCO-0.0.7.tar` & `askCO-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 04:41:32.099534 askCO-0.0.7/
--rw-rw-rw-   0        0        0     3994 2023-05-23 04:41:32.099534 askCO-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3424 2023-05-23 00:07:57.000000 askCO-0.0.7/README.md
--rw-rw-rw-   0        0        0      676 2023-05-23 04:40:23.000000 askCO-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 04:41:32.099534 askCO-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-23 04:41:32.068288 askCO-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 04:41:32.068288 askCO-0.0.7/src/askCO/
--rw-rw-rw-   0        0        0     9732 2023-05-23 04:37:53.000000 askCO-0.0.7/src/askCO/__init__.py
--rw-rw-rw-   0        0        0     2296 2023-05-18 02:08:58.000000 askCO-0.0.7/src/askCO/tryCO.py
-drwxrwxrwx   0        0        0        0 2023-05-23 04:41:32.099534 askCO-0.0.7/src/askCO.egg-info/
--rw-rw-rw-   0        0        0     3994 2023-05-23 04:41:32.000000 askCO-0.0.7/src/askCO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-05-23 04:41:32.000000 askCO-0.0.7/src/askCO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 04:41:32.000000 askCO-0.0.7/src/askCO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-23 04:41:32.000000 askCO-0.0.7/src/askCO.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 23:37:07.493689 askCO-0.0.8/
+-rw-rw-rw-   0        0        0     3994 2023-05-23 23:37:07.493689 askCO-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3424 2023-05-23 00:07:57.000000 askCO-0.0.8/README.md
+-rw-rw-rw-   0        0        0      676 2023-05-23 23:36:25.000000 askCO-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 23:37:07.493689 askCO-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-23 23:37:07.462447 askCO-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 23:37:07.478063 askCO-0.0.8/src/askCO/
+-rw-rw-rw-   0        0        0     9721 2023-05-23 23:30:08.000000 askCO-0.0.8/src/askCO/__init__.py
+-rw-rw-rw-   0        0        0     2387 2023-05-23 23:35:16.000000 askCO-0.0.8/src/askCO/tryCO.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:37:07.493689 askCO-0.0.8/src/askCO.egg-info/
+-rw-rw-rw-   0        0        0     3994 2023-05-23 23:37:07.000000 askCO-0.0.8/src/askCO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-05-23 23:37:07.000000 askCO-0.0.8/src/askCO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 23:37:07.000000 askCO-0.0.8/src/askCO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-23 23:37:07.000000 askCO-0.0.8/src/askCO.egg-info/top_level.txt
```

### Comparing `askCO-0.0.7/PKG-INFO` & `askCO-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: askCO
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python interface for Te Papa's collections API
 Author-email: Lucy Schrader <lucy@schrader.nz>
 License: MIT License
 Project-URL: Homepage, https://github.com/lucyschrader/askCO
 Keywords: python,museum,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `askCO-0.0.7/README.md` & `askCO-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `askCO-0.0.7/pyproject.toml` & `askCO-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "askCO"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
 	{name = "Lucy Schrader", email = "lucy@schrader.nz"},
 ]
 description = "Python interface for Te Papa's collections API"
 readme = "README.md"
 keywords = ["python", "museum", "api"]
 requires-python = ">=3.7"
```

### Comparing `askCO-0.0.7/src/askCO/__init__.py` & `askCO-0.0.8/src/askCO/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,14 @@
 		self.method = None
 		self.allow_redirects = None
 		self.timeout = kwargs.get("timeout")
 		self.attempts = kwargs.get("attempts")
 
 		# Query elements
 		self.endpoint = kwargs.get("endpoint")
-		if not self.endpoint:
-			self.endpoint = "object"
 		self.base_url = "https://data.tepapa.govt.nz/collection"
 		self.request_url = None
 		self.request_body = None
 
 		# Response element
 		self.status_code = None
 		self.response = None
@@ -160,15 +158,15 @@
 		self.start = kwargs.get("start")
 		self.size = kwargs.get("size")
 		self.filters = kwargs.get("filters")
 
 		self.build_query()
 
 	def build_query(self):
-		if self.endpoint == "object":
+		if not self.endpoint:
 			self.request_url = "{}/search".format(self.base_url)
 			self.method = "POST"
 			self.request_body = {}
 
 			if self.query:
 				self.request_body.update(self._singleValueFormatter("query", self.query))
 			if self.fields:
@@ -194,15 +192,15 @@
 
 			url_parts = []
 			query_parts = []
 
 			if self.query:
 				query_parts.append(self.query)
 			if self.filters:
-				for f in filters:
+				for f in self.filters:
 					query_parts.append("{k}:{v}".format(k=f["field"], v=f["keyword"]))
 
 			query_string = " AND ".join(query_parts)
 			url_parts.append(query_string)
 			
 			if self.fields:
 				url_parts.append("fields={}".format(self.fields))
@@ -242,15 +240,15 @@
 
 		if kwargs.get("max_records") != -1:
 			self.record_limit = kwargs.get("max_records")
 
 		self.build_query()
 
 	def build_query(self):
-		if self.endpoint == "object":
+		if not self.endpoint:
 			slug = "search"
 		else:
 			slug = self.endpoint
 
 		scroll_base_url = "{b}/{s}/_scroll/?q=".format(b=self.base_url, s=slug)
 
 		url_parts = []
@@ -287,14 +285,16 @@
 		self.related = False
 		self.size = None
 		self.types = None
 
 		self.build_query()
 
 	def build_query(self):
+		if not self.endpoint:
+			self.endpoint = "object"
 		self.request_url = "{b}/{e}/{i}".format(b=self.base_url, e=self.endpoint, i=self.irn)
 
 		# Build a search for related
 		if self.related == True:
 			self.request_url += "/related"
 			if self.size or self.types:
 				self.request_url += "?"
```

### Comparing `askCO-0.0.7/src/askCO/tryCO.py` & `askCO-0.0.8/src/askCO/tryCO.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 quiet = False
 sleep = 0.1
 timeout = 5
 attempts = 3
 
 def try_search():
 	# Set the search request parameters
-	endpoint = "object"
+	# No endpoint specified - will search all records
 	query = "Myosotis"
 	filters = [{"field": "type", "keyword": "Specimen"}, {"field": "collection", "keyword": "Plants"}]
 	fields = None
 	size = 100
 	start = 0
 
 	# Create the query object
 	request = Search(api_key=api_key,
-		endpoint=endpoint,
 		query=query,
 		filters=filters,
 		fields=fields,
 		size=size,
 		start=start,
 		timeout=timeout,
 		attempts=attempts,
@@ -40,14 +39,15 @@
 	print("Search returned {} results".format(request.record_count))
 	if request.record_count > 0:
 		print("First result:")
 		print(next(iter(request.records)))
 
 def try_scroll():
 	# Set the scroll request parameters
+	# Endpoint specified, will only search the object endpoint
 	endpoint = "object"
 	query = "wellington"
 	filters = [{"field": "type", "keyword": "Object"}, {"field": "hasRepresentation.rights.allowsDownload", "keyword": "True"}]
 	fields = None,
 	size = 1000
 	duration = 1
 	max_records = 5000
@@ -72,14 +72,15 @@
 	# See what you got
 	print("Search returned {} results".format(request.record_count))
 	if request.record_count > 0:
 		print("First result:")
 		print(next(iter(request.records)))
 
 def try_resource():
+	# Endpoint required
 	endpoint = "object"
 	irn = 1390415
 
 	# Create the query object
 	request = Resource(api_key=api_key,
 		endpoint=endpoint,
 		irn=irn,
```

### Comparing `askCO-0.0.7/src/askCO.egg-info/PKG-INFO` & `askCO-0.0.8/src/askCO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: askCO
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python interface for Te Papa's collections API
 Author-email: Lucy Schrader <lucy@schrader.nz>
 License: MIT License
 Project-URL: Homepage, https://github.com/lucyschrader/askCO
 Keywords: python,museum,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

