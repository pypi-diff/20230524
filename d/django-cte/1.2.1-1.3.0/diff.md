# Comparing `tmp/django-cte-1.2.1.tar.gz` & `tmp/django-cte-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cte-1.2.1.tar", last modified: Thu Jul  7 11:55:42 2022, max compression
+gzip compressed data, was "django-cte-1.3.0.tar", last modified: Wed May 24 15:12:20 2023, max compression
```

## Comparing `django-cte-1.2.1.tar` & `django-cte-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dimagi    (1001) dimagi    (1001)        0 2022-07-07 11:55:42.052360 django-cte-1.2.1/
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)     1508 2018-02-21 14:28:44.000000 django-cte-1.2.1/LICENSE
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)     2134 2022-07-07 11:55:42.052360 django-cte-1.2.1/PKG-INFO
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)      850 2022-04-26 20:01:12.000000 django-cte-1.2.1/README.md
-drwxr-xr-x   0 dimagi    (1001) dimagi    (1001)        0 2022-07-07 11:55:42.052360 django-cte-1.2.1/django_cte/
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)      158 2022-07-07 11:54:05.000000 django-cte-1.2.1/django_cte/__init__.py
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)     6231 2022-03-30 20:00:41.000000 django-cte-1.2.1/django_cte/cte.py
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)     1930 2022-07-07 11:23:10.000000 django-cte-1.2.1/django_cte/expressions.py
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)     3243 2022-03-30 20:02:49.000000 django-cte-1.2.1/django_cte/join.py
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)     3615 2022-03-28 21:00:27.000000 django-cte-1.2.1/django_cte/meta.py
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)     4682 2022-02-22 11:58:08.000000 django-cte-1.2.1/django_cte/query.py
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)     1137 2021-09-22 11:08:48.000000 django-cte-1.2.1/django_cte/raw.py
-drwxr-xr-x   0 dimagi    (1001) dimagi    (1001)        0 2022-07-07 11:55:42.052360 django-cte-1.2.1/django_cte.egg-info/
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)     2134 2022-07-07 11:55:42.000000 django-cte-1.2.1/django_cte.egg-info/PKG-INFO
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)      315 2022-07-07 11:55:42.000000 django-cte-1.2.1/django_cte.egg-info/SOURCES.txt
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)        1 2022-07-07 11:55:42.000000 django-cte-1.2.1/django_cte.egg-info/dependency_links.txt
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)       11 2022-07-07 11:55:42.000000 django-cte-1.2.1/django_cte.egg-info/top_level.txt
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)      130 2022-07-07 11:55:42.052360 django-cte-1.2.1/setup.cfg
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)     2002 2022-04-26 13:51:48.000000 django-cte-1.2.1/setup.py
+drwxr-xr-x   0 dimagi    (1001) dimagi    (1001)        0 2023-05-24 15:12:20.696809 django-cte-1.3.0/
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)     1508 2018-02-21 14:28:44.000000 django-cte-1.3.0/LICENSE
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)     2134 2023-05-24 15:12:20.696809 django-cte-1.3.0/PKG-INFO
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)      850 2022-04-26 20:01:12.000000 django-cte-1.3.0/README.md
+drwxr-xr-x   0 dimagi    (1001) dimagi    (1001)        0 2023-05-24 15:12:20.696809 django-cte-1.3.0/django_cte/
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)      158 2023-05-24 15:06:01.000000 django-cte-1.3.0/django_cte/__init__.py
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)     6574 2023-05-24 15:06:01.000000 django-cte-1.3.0/django_cte/cte.py
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)     1930 2022-07-07 11:23:10.000000 django-cte-1.3.0/django_cte/expressions.py
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)     3243 2023-05-24 15:05:55.000000 django-cte-1.3.0/django_cte/join.py
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)     3615 2023-05-24 15:05:55.000000 django-cte-1.3.0/django_cte/meta.py
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)     5642 2023-05-24 15:06:01.000000 django-cte-1.3.0/django_cte/query.py
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)     1137 2021-09-22 11:08:48.000000 django-cte-1.3.0/django_cte/raw.py
+drwxr-xr-x   0 dimagi    (1001) dimagi    (1001)        0 2023-05-24 15:12:20.696809 django-cte-1.3.0/django_cte.egg-info/
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)     2134 2023-05-24 15:12:20.000000 django-cte-1.3.0/django_cte.egg-info/PKG-INFO
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)      315 2023-05-24 15:12:20.000000 django-cte-1.3.0/django_cte.egg-info/SOURCES.txt
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)        1 2023-05-24 15:12:20.000000 django-cte-1.3.0/django_cte.egg-info/dependency_links.txt
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)       11 2023-05-24 15:12:20.000000 django-cte-1.3.0/django_cte.egg-info/top_level.txt
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)      130 2023-05-24 15:12:20.696809 django-cte-1.3.0/setup.cfg
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)     2002 2022-04-26 13:51:48.000000 django-cte-1.3.0/setup.py
```

### Comparing `django-cte-1.2.1/LICENSE` & `django-cte-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cte-1.2.1/PKG-INFO` & `django-cte-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cte
-Version: 1.2.1
+Version: 1.3.0
 Summary: Common Table Expressions (CTE) for Django
 Home-page: https://github.com/dimagi/django-cte
 Maintainer: Daniel Miller
 Maintainer-email: millerdev@gmail.com
 License: BSD License
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-cte-1.2.1/README.md` & `django-cte-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `django-cte-1.2.1/django_cte/cte.py` & `django-cte-1.3.0/django_cte/cte.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,43 +17,47 @@
 
     :param queryset: A queryset to use as the body of the CTE.
     :param name: Optional name parameter for the CTE (default: "cte").
     This must be a unique name that does not conflict with other
     entities (tables, views, functions, other CTE(s), etc.) referenced
     in the given query as well any query to which this CTE will
     eventually be added.
+    :param materialized: Optional parameter (default: False) which enforce
+    using of MATERIALIZED statement for supporting databases.
     """
 
-    def __init__(self, queryset, name="cte"):
+    def __init__(self, queryset, name="cte", materialized=False):
         self.query = None if queryset is None else queryset.query
         self.name = name
         self.col = CTEColumns(self)
+        self.materialized = materialized
 
     def __getstate__(self):
-        return (self.query, self.name)
+        return (self.query, self.name, self.materialized)
 
     def __setstate__(self, state):
-        self.query, self.name = state
+        self.query, self.name, self.materialized = state
         self.col = CTEColumns(self)
 
     def __repr__(self):
         return "<With {}>".format(self.name)
 
     @classmethod
-    def recursive(cls, make_cte_queryset, name="cte"):
+    def recursive(cls, make_cte_queryset, name="cte", materialized=False):
         """Recursive Common Table Expression: `WITH RECURSIVE ...`
 
         :param make_cte_queryset: Function taking a single argument (a
         not-yet-fully-constructed cte object) and returning a `QuerySet`
         object. The returned `QuerySet` normally consists of an initial
         statement unioned with a recursive statement.
         :param name: See `name` parameter of `__init__`.
+        :param materialized: See `materialized` parameter of `__init__`.
         :returns: The fully constructed recursive cte object.
         """
-        cte = cls(None, name)
+        cte = cls(None, name, materialized)
         cte.query = make_cte_queryset(cte).query
         return cte
 
     def join(self, model_or_queryset, *filter_q, **filter_kw):
         """Join this CTE to the given model or queryset
 
         This CTE will be refernced by the returned queryset, but the
```

### Comparing `django-cte-1.2.1/django_cte/expressions.py` & `django-cte-1.3.0/django_cte/expressions.py`

 * *Files identical despite different names*

### Comparing `django-cte-1.2.1/django_cte/join.py` & `django-cte-1.3.0/django_cte/join.py`

 * *Files identical despite different names*

### Comparing `django-cte-1.2.1/django_cte/meta.py` & `django-cte-1.3.0/django_cte/meta.py`

 * *Files identical despite different names*

### Comparing `django-cte-1.2.1/django_cte/query.py` & `django-cte-1.3.0/django_cte/query.py`

 * *Files 17% similar despite different names*

```diff
@@ -61,38 +61,64 @@
     else:
         def chain(self, klass=None):
             return self.__chain("chain", klass)
 
 
 class CTECompiler(object):
 
-    TEMPLATE = "{name} AS ({query})"
-
     @classmethod
     def generate_sql(cls, connection, query, as_sql):
         if query.combinator:
             return as_sql()
 
         ctes = []
         params = []
         for cte in query._with_ctes:
             compiler = cte.query.get_compiler(connection=connection)
             qn = compiler.quote_name_unless_alias
             cte_sql, cte_params = compiler.as_sql()
-            ctes.append(cls.TEMPLATE.format(name=qn(cte.name), query=cte_sql))
+            template = cls.get_cte_query_template(cte)
+            ctes.append(template.format(name=qn(cte.name), query=cte_sql))
             params.extend(cte_params)
 
-        # Always use WITH RECURSIVE
-        # https://www.postgresql.org/message-id/13122.1339829536%40sss.pgh.pa.us
-        sql = ["WITH RECURSIVE", ", ".join(ctes)] if ctes else []
+        explain_query = getattr(query, "explain_query", None)
+        sql = []
+        if explain_query:
+            explain_format = getattr(query, "explain_format", None)
+            explain_options = getattr(query, "explain_options", {})
+            sql.append(
+                connection.ops.explain_query_prefix(
+                    explain_format,
+                    **explain_options
+                )
+            )
+            # this needs to get set to False so that the base as_sql() doesn't
+            # insert the EXPLAIN statement where it would end up between the
+            # WITH ... clause and the final SELECT
+            query.explain_query = False
+
+        if ctes:
+            # Always use WITH RECURSIVE
+            # https://www.postgresql.org/message-id/13122.1339829536%40sss.pgh.pa.us
+            sql.extend(["WITH RECURSIVE", ", ".join(ctes)])
         base_sql, base_params = as_sql()
+
+        if explain_query:
+            query.explain_query = explain_query
+
         sql.append(base_sql)
         params.extend(base_params)
         return " ".join(sql), tuple(params)
 
+    @classmethod
+    def get_cte_query_template(cls, cte):
+        if cte.materialized:
+            return "{name} AS MATERIALIZED ({query})"
+        return "{name} AS ({query})"
+
 
 class CTEUpdateQuery(UpdateQuery, CTEQuery):
     pass
 
 
 class CTEDeleteQuery(DeleteQuery, CTEQuery):
     pass
```

### Comparing `django-cte-1.2.1/django_cte/raw.py` & `django-cte-1.3.0/django_cte/raw.py`

 * *Files identical despite different names*

### Comparing `django-cte-1.2.1/django_cte.egg-info/PKG-INFO` & `django-cte-1.3.0/django_cte.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cte
-Version: 1.2.1
+Version: 1.3.0
 Summary: Common Table Expressions (CTE) for Django
 Home-page: https://github.com/dimagi/django-cte
 Maintainer: Daniel Miller
 Maintainer-email: millerdev@gmail.com
 License: BSD License
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-cte-1.2.1/setup.py` & `django-cte-1.3.0/setup.py`

 * *Files identical despite different names*

