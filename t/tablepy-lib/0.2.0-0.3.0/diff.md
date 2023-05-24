# Comparing `tmp/tablepy_lib-0.2.0.tar.gz` & `tmp/tablepy_lib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablepy_lib-0.2.0.tar", max compression
+gzip compressed data, was "tablepy_lib-0.3.0.tar", max compression
```

## Comparing `tablepy_lib-0.2.0.tar` & `tablepy_lib-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1092 2023-05-24 20:04:11.338943 tablepy_lib-0.2.0/LICENSE
--rw-r--r--   0        0        0      488 2023-05-24 21:33:24.596761 tablepy_lib-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 19:49:50.199768 tablepy_lib-0.2.0/README.md
--rw-r--r--   0        0        0       49 2023-05-24 21:31:44.458131 tablepy_lib-0.2.0/tablepy_lib/__init__.py
--rw-r--r--   0        0        0     2699 2023-05-24 21:30:22.753208 tablepy_lib-0.2.0/tablepy_lib/consoleFormatter.py
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 tablepy_lib-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-24 20:04:11.338943 tablepy_lib-0.3.0/LICENSE
+-rw-r--r--   0        0        0      488 2023-05-24 21:38:17.333001 tablepy_lib-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 19:49:50.199768 tablepy_lib-0.3.0/README.md
+-rw-r--r--   0        0        0       49 2023-05-24 21:31:44.458131 tablepy_lib-0.3.0/tablepy_lib/__init__.py
+-rw-r--r--   0        0        0     2480 2023-05-24 21:38:03.255374 tablepy_lib-0.3.0/tablepy_lib/consoleFormatter.py
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 tablepy_lib-0.3.0/PKG-INFO
```

### Comparing `tablepy_lib-0.2.0/LICENSE` & `tablepy_lib-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tablepy_lib-0.2.0/tablepy_lib/consoleFormatter.py` & `tablepy_lib-0.3.0/tablepy_lib/consoleFormatter.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,71 +11,63 @@
             if data.empty:
                 raise ValueError("Invalid input data type. Supported types are dictionary and pandas DataFrame.")
         else:
             raise ValueError("Invalid input data type. Supported types are dictionary and pandas DataFrame.")
 
     def to_table(self):
         col_names = list(self.data.keys())
-        rows = [list(map(str, self.data[key])) for key in col_names]
-        formatted_data = [col_names] + rows
+        row_data = [list(map(str, self.data[key])) for key in col_names]
+        formatted_data = row_data
 
         # Column width calculation
-        col_widths = [0 for col in formatted_data[0]]
+        col_widths = [0 for col in col_names]
 
         # header size calculation
         for i in range(len(col_names)):
             size = len(col_names[i]) + 2
             if size > col_widths[i]:
                 col_widths[i] = size
 
-        items = len(rows[0]) - 1
-        #print(items)
-
-        # Data size calculation
-        for i in range(items):
-            for j in range(len(rows)):
-                # print(formatted_data[j][i+1])
-                size = len(formatted_data[j][i+1]) + 2
-                if (size > col_widths[i]):
-                    col_widths[i] = size
+        rows = len(row_data[0])
+        columns = len(col_names)
 
+        for row in range(rows):
+            for column in range(columns):
+                size = len(formatted_data[column][row]) + 2
+                if (size > col_widths[column]):
+                    col_widths[column] = size
+        
         # Add extra width for table borders and separators
-        # print(formatted_data[0])
 
         table_formatted = "\n"
 
         header = "| "
-        for i in range(len(formatted_data[0])):
-            size = col_widths[i] - len(formatted_data[0][i])
+        for i in range(len(col_names)):
+            size = col_widths[i] - len(col_names[i])
             filler = " " * size
-            header += formatted_data[0][i] + filler + " | "
+            header += col_names[i] + filler + " | "
 
         table_formatted += header + "\n"
 
         line = "| "
-        for i in range(len(formatted_data[0])):
+        for i in range(len(col_names)):
             size = col_widths[i]
             filler = "-" * size
             line += filler + " | "
 
         table_formatted += line + "\n"
 
-        items = len(rows[0])
-
-        print(col_widths)
-
         ta = ""
-        for i in range(items):
-            
+        
+        for row in range(rows):
             data = "| "
-            for j in range(len(rows)):
-                print(formatted_data[j][i+1])
-                size = col_widths[j] - len(formatted_data[j][i+1])
+            for column in range(columns):
+                size = col_widths[column] - len(formatted_data[column][row])
                 filler = " " * size
-                data += formatted_data[j][i+1] + filler + " | "
+                data += formatted_data[column][row] + filler + " | " 
             ta += data + "\n"
             
         table_formatted += ta  + "\n"
         return table_formatted
 
     
 def markdown(data):
```

### Comparing `tablepy_lib-0.2.0/PKG-INFO` & `tablepy_lib-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablepy-lib
-Version: 0.2.0
+Version: 0.3.0
 Summary: This is a versatile and user-friendly Python table library that can quickly render any Dictionary<TV, T> or DataFrame into a visually appealing markdown
 Author: Jordi Corbilla
 Author-email: jordi.coll.corbilla@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

