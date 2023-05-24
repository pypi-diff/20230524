# Comparing `tmp/lineagex-0.0.4.tar.gz` & `tmp/lineagex-0.0.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lineagex-0.0.4.tar", max compression
+gzip compressed data, was "lineagex-0.0.5a1.tar", max compression
```

## Comparing `lineagex-0.0.4.tar` & `lineagex-0.0.5a1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       55 2023-05-12 01:58:21.769698 lineagex-0.0.4/lineagex/__init__.py
--rw-r--r--   0        0        0    54175 2023-04-22 19:33:20.371862 lineagex-0.0.4/lineagex/app.js
--rw-r--r--   0        0        0    32350 2023-05-20 01:29:26.901284 lineagex-0.0.4/lineagex/ColumnLineage.py
--rw-r--r--   0        0        0    22869 2023-05-20 01:36:05.905629 lineagex-0.0.4/lineagex/ColumnLineageNoConn.py
--rw-r--r--   0        0        0     1794 2023-05-20 01:36:11.749312 lineagex-0.0.4/lineagex/lineagex.py
--rw-r--r--   0        0        0     2389 2023-05-20 01:36:16.471395 lineagex-0.0.4/lineagex/LineageXNoConn.py
--rw-r--r--   0        0        0    13474 2023-05-20 01:36:19.877229 lineagex-0.0.4/lineagex/LineageXWithConn.py
--rw-r--r--   0        0        0     7176 2023-05-18 22:43:15.279746 lineagex-0.0.4/lineagex/SqlToDict.py
--rw-r--r--   0        0        0     1460 2023-05-08 20:36:59.378380 lineagex-0.0.4/lineagex/stack.py
--rw-r--r--   0        0        0     7305 2023-05-19 22:10:39.261810 lineagex-0.0.4/lineagex/utils.py
--rw-r--r--   0        0        0  3761177 2023-04-22 19:33:20.645016 lineagex-0.0.4/lineagex/vendor.js
--rw-r--r--   0        0        0      448 2023-05-20 01:53:08.141075 lineagex-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4158 2023-05-17 20:42:55.789941 lineagex-0.0.4/README.md
--rw-r--r--   0        0        0     4863 1970-01-01 00:00:00.000000 lineagex-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-05-12 01:58:21.769698 lineagex-0.0.5a1/lineagex/__init__.py
+-rw-r--r--   0        0        0    54175 2023-04-22 19:33:20.371862 lineagex-0.0.5a1/lineagex/app.js
+-rw-r--r--   0        0        0    32350 2023-05-20 01:29:26.901284 lineagex-0.0.5a1/lineagex/ColumnLineage.py
+-rw-r--r--   0        0        0    24066 2023-05-24 01:05:18.342710 lineagex-0.0.5a1/lineagex/ColumnLineageNoConn.py
+-rw-r--r--   0        0        0     1802 2023-05-23 23:33:11.925203 lineagex-0.0.5a1/lineagex/lineagex.py
+-rw-r--r--   0        0        0     4691 2023-05-23 23:48:42.350240 lineagex-0.0.5a1/lineagex/LineageXNoConn.py
+-rw-r--r--   0        0        0    13522 2023-05-23 21:34:23.590817 lineagex-0.0.5a1/lineagex/LineageXWithConn.py
+-rw-r--r--   0        0        0     7176 2023-05-23 22:40:25.559899 lineagex-0.0.5a1/lineagex/SqlToDict.py
+-rw-r--r--   0        0        0     1460 2023-05-08 20:36:59.378380 lineagex-0.0.5a1/lineagex/stack.py
+-rw-r--r--   0        0        0     7305 2023-05-19 22:10:39.261810 lineagex-0.0.5a1/lineagex/utils.py
+-rw-r--r--   0        0        0  3761177 2023-04-22 19:33:20.645016 lineagex-0.0.5a1/lineagex/vendor.js
+-rw-r--r--   0        0        0      456 2023-05-24 01:12:49.326096 lineagex-0.0.5a1/pyproject.toml
+-rw-r--r--   0        0        0     4158 2023-05-17 20:42:55.789941 lineagex-0.0.5a1/README.md
+-rw-r--r--   0        0        0     4865 1970-01-01 00:00:00.000000 lineagex-0.0.5a1/PKG-INFO
```

### Comparing `lineagex-0.0.4/lineagex/app.js` & `lineagex-0.0.5a1/lineagex/app.js`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.4/lineagex/ColumnLineage.py` & `lineagex-0.0.5a1/lineagex/ColumnLineage.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.4/lineagex/ColumnLineageNoConn.py` & `lineagex-0.0.5a1/lineagex/ColumnLineageNoConn.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,20 +125,32 @@
         all_cte_sub_cols = []
         # add in more conditions, including FROM/JOIN
         for cond in shared_conditions_with_table:
             for cond_sql in sql_ast.find_all(cond):
                 for sub_ast in cond_sql.find_all(exp.Select):
                     temp_sub_table = self._resolve_table(part_ast=sub_ast)
                     temp_sub_cols = []
+                    temp_dict = {}
                     for col in sub_ast.find_all(exp.Column):
-                        temp_sub_cols.extend(
-                            self._find_alias_col(
-                                col_sql=col.sql(), temp_table=temp_sub_table
+                        if col.find(exp.Star):
+                            temp_dict = self._resolve_agg_star(
+                                col_name="*",
+                                projection=col,
+                                used_tables=temp_sub_table,
+                                target_dict=temp_dict,
                             )
-                        )
+                            for _, value in temp_dict.items():
+                                temp_sub_cols.extend(value)
+                        else:
+                            temp_sub_cols.extend(
+                                self._find_alias_col(
+                                    col_sql=col.sql(), temp_table=temp_sub_table
+                                )
+                            )
+                    temp_sub_cols = list(set(temp_sub_cols))
                     all_cte_sub_table.extend(
                         self._find_all_tables(temp_table_list=temp_sub_table)
                     )
                     all_cte_sub_cols.extend(temp_sub_cols)
                     sub_ast.pop()
         return all_cte_sub_table, all_cte_sub_cols
 
@@ -199,54 +211,54 @@
         :param target_dict: the dict it is outputting to
         :param source_table: all the source tables that this column might originate from
         """
         # Resolve count(*) with no alias, potentially other aggregations, MIN, MAX, SUM
         if projection.find(exp.Star):
             if isinstance(projection, exp.Count):
                 col_name = "count"
-                self._resolve_agg_star(
+                target_dict = self._resolve_agg_star(
                     col_name=col_name,
                     projection=projection,
                     used_tables=source_table,
                     target_dict=target_dict,
                 )
             elif isinstance(projection, exp.Avg):
                 col_name = "avg"
-                self._resolve_agg_star(
+                target_dict = self._resolve_agg_star(
                     col_name=col_name,
                     projection=projection,
                     used_tables=source_table,
                     target_dict=target_dict,
                 )
             elif isinstance(projection, exp.Max):
                 col_name = "max"
-                self._resolve_agg_star(
+                target_dict = self._resolve_agg_star(
                     col_name=col_name,
                     projection=projection,
                     used_tables=source_table,
                     target_dict=target_dict,
                 )
             elif isinstance(projection, exp.Min):
                 col_name = "min"
-                self._resolve_agg_star(
+                target_dict = self._resolve_agg_star(
                     col_name=col_name,
                     projection=projection,
                     used_tables=source_table,
                     target_dict=target_dict,
                 )
             elif isinstance(projection, exp.Sum):
                 col_name = "sum"
-                self._resolve_agg_star(
+                target_dict = self._resolve_agg_star(
                     col_name=col_name,
                     projection=projection,
                     used_tables=source_table,
                     target_dict=target_dict,
                 )
             else:
-                self._resolve_agg_star(
+                target_dict = self._resolve_agg_star(
                     col_name=col_name,
                     projection=projection.unalias(),
                     used_tables=source_table,
                     target_dict=target_dict,
                 )
         else:
             proj_columns = []
@@ -431,31 +443,38 @@
                 return [deduced_table.pop() + "." + col_sql]
         elif len(temp) == 2:
             if temp[0] in self.table_alias_dict.keys():
                 t = self.table_alias_dict[temp[0]]
             else:
                 t = temp[0]
             if t in self.cte_dict.keys():
-                return self.cte_dict[t][temp[1]]
+                # CTE is stored, but the column name is not, resolve case sensitivity
+                if temp[1] not in self.cte_dict[t].keys():
+                    temp_cte_dict = {k.lower(): v for k, v in self.cte_dict[t].items()}
+                    if temp[1].lower() in temp_cte_dict.keys():
+                        return temp_cte_dict[temp[1].lower()]
+                else:
+                    return self.cte_dict[t][temp[1]]
             else:
                 return [t + "." + temp[1]]
         return [col_sql]
 
     def _resolve_agg_star(
         self,
         col_name: Optional[str] = "",
         projection: expressions = None,
         used_tables: Optional[List] = None,
         target_dict: Optional[dict] = None,
-    ):
+    ) -> dict:
         """
         Trying to resolve the * and append appropriate columns if the table is able to resolved
         :param col_name: the name of the column
         :param projection: the expression of the sql
         :param used_tables: the tables that are used
+        :param target_dict: the dict it is writing to
         """
         if projection.find(exp.Star):
             # * with a table name
             if projection.find(exp.Identifier):
                 t_name = projection.find(exp.Identifier).text("this")
                 # Resolve alias
                 if t_name in self.table_alias_dict.keys():
@@ -507,11 +526,12 @@
                         list(set(star_cols).union(self.all_used_col))
                     )
             # only star, like count(*)
             else:
                 target_dict[col_name] = sorted(
                     list(self.all_used_col) + [t + ".*" for t in used_tables]
                 )
+        return target_dict
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `lineagex-0.0.4/lineagex/lineagex.py` & `lineagex-0.0.5a1/lineagex/lineagex.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
                 conn_string=conn_string,
                 search_path_schema=search_path_schema,
             )
             self._save_js_file()
             self.output_dict = lx.output_dict
         else:
             lx = LineageXNoConn(
-                sql=sql, search_path_schema=target_schema + "," + search_path_schema
+                sql=sql, target_schema=target_schema, search_path_schema= search_path_schema
             )
             self._save_js_file()
             self.output_dict = lx.output_dict
 
     def _save_js_file(self):
         data = pkgutil.get_data(__name__, "app.js")
         js_file = open("app.js", "w", encoding="utf-8")
```

### Comparing `lineagex-0.0.4/lineagex/LineageXWithConn.py` & `lineagex-0.0.5a1/lineagex/LineageXWithConn.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
                             "{} is skipped because database returned no result on it".format(
                                 t
                             )
                         )
             cur.close()
             for name, sql in self.sql_files_dict.items():
                 try:
+                    print(name, " processing")
                     col_lineage = ColumnLineage(
                         plan=self._get_plan(sql=sql),
                         sql=sql,
                         columns=find_column(
                             table_name=name,
                             engine=self.conn,
                             search_schema=self.search_schema,
```

### Comparing `lineagex-0.0.4/lineagex/SqlToDict.py` & `lineagex-0.0.5a1/lineagex/SqlToDict.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.4/lineagex/stack.py` & `lineagex-0.0.5a1/lineagex/stack.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.4/lineagex/utils.py` & `lineagex-0.0.5a1/lineagex/utils.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.4/lineagex/vendor.js` & `lineagex-0.0.5a1/lineagex/vendor.js`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.4/README.md` & `lineagex-0.0.5a1/README.md`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.4/PKG-INFO` & `lineagex-0.0.5a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lineagex
-Version: 0.0.4
+Version: 0.0.5a1
 Summary: A column lineage tool
 License: MIT
 Author: zshandy
 Author-email: zshandy@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

