# Comparing `tmp/templatte-0.1.tar.gz` & `tmp/templatte-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templatte-0.1.tar", last modified: Tue May 23 08:54:46 2023, max compression
+gzip compressed data, was "templatte-0.2.tar", last modified: Wed May 24 06:29:59 2023, max compression
```

## Comparing `templatte-0.1.tar` & `templatte-0.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 dbalogh    (501) staff       (20)        0 2023-05-23 08:54:46.203926 templatte-0.1/
--rw-r--r--   0 dbalogh    (501) staff       (20)     1068 2023-05-23 07:55:59.000000 templatte-0.1/LICENSE
--rw-r--r--   0 dbalogh    (501) staff       (20)      245 2023-05-23 08:54:46.203573 templatte-0.1/PKG-INFO
-drwxr-xr-x   0 dbalogh    (501) staff       (20)        0 2023-05-23 08:54:46.186163 templatte-0.1/datamodel/
--rw-r--r--   0 dbalogh    (501) staff       (20)        0 2023-05-23 07:58:02.000000 templatte-0.1/datamodel/__init__.py
--rw-r--r--   0 dbalogh    (501) staff       (20)     1890 2023-05-23 07:57:43.000000 templatte-0.1/datamodel/data_source.py
-drwxr-xr-x   0 dbalogh    (501) staff       (20)        0 2023-05-23 08:54:46.187915 templatte-0.1/environment/
--rw-r--r--   0 dbalogh    (501) staff       (20)        0 2023-05-23 06:47:17.000000 templatte-0.1/environment/__init__.py
--rw-r--r--   0 dbalogh    (501) staff       (20)      934 2023-05-23 06:50:39.000000 templatte-0.1/environment/environment.py
-drwxr-xr-x   0 dbalogh    (501) staff       (20)        0 2023-05-23 08:54:46.192229 templatte-0.1/report/
--rw-r--r--   0 dbalogh    (501) staff       (20)        0 2023-05-22 18:50:07.000000 templatte-0.1/report/__init__.py
--rw-r--r--   0 dbalogh    (501) staff       (20)     1054 2023-05-23 06:46:02.000000 templatte-0.1/report/report.py
-drwxr-xr-x   0 dbalogh    (501) staff       (20)        0 2023-05-23 08:54:46.199529 templatte-0.1/reportmodel/
--rw-r--r--   0 dbalogh    (501) staff       (20)        0 2023-05-19 12:50:56.000000 templatte-0.1/reportmodel/__init__.py
--rw-r--r--   0 dbalogh    (501) staff       (20)     3588 2023-05-23 07:08:41.000000 templatte-0.1/reportmodel/report_generator.py
--rw-r--r--   0 dbalogh    (501) staff       (20)      138 2023-05-23 06:46:02.000000 templatte-0.1/reportmodel/template.py
--rw-r--r--   0 dbalogh    (501) staff       (20)       38 2023-05-23 08:54:46.204010 templatte-0.1/setup.cfg
--rw-r--r--   0 dbalogh    (501) staff       (20)      424 2023-05-23 08:34:30.000000 templatte-0.1/setup.py
-drwxr-xr-x   0 dbalogh    (501) staff       (20)        0 2023-05-23 08:54:46.202849 templatte-0.1/templatte.egg-info/
--rw-r--r--   0 dbalogh    (501) staff       (20)      245 2023-05-23 08:54:46.000000 templatte-0.1/templatte.egg-info/PKG-INFO
--rw-r--r--   0 dbalogh    (501) staff       (20)      394 2023-05-23 08:54:46.000000 templatte-0.1/templatte.egg-info/SOURCES.txt
--rw-r--r--   0 dbalogh    (501) staff       (20)        1 2023-05-23 08:54:46.000000 templatte-0.1/templatte.egg-info/dependency_links.txt
--rw-r--r--   0 dbalogh    (501) staff       (20)       30 2023-05-23 08:54:46.000000 templatte-0.1/templatte.egg-info/requires.txt
--rw-r--r--   0 dbalogh    (501) staff       (20)       41 2023-05-23 08:54:46.000000 templatte-0.1/templatte.egg-info/top_level.txt
+drwxr-xr-x   0 dbalogh    (501) staff       (20)        0 2023-05-24 06:29:59.973780 templatte-0.2/
+-rw-r--r--   0 dbalogh    (501) staff       (20)     1068 2023-05-23 07:55:59.000000 templatte-0.2/LICENSE
+-rw-r--r--   0 dbalogh    (501) staff       (20)      245 2023-05-24 06:29:59.973362 templatte-0.2/PKG-INFO
+-rw-r--r--   0 dbalogh    (501) staff       (20)      123 2023-05-23 10:58:14.000000 templatte-0.2/README.md
+drwxr-xr-x   0 dbalogh    (501) staff       (20)        0 2023-05-24 06:29:59.959724 templatte-0.2/datamodel/
+-rw-r--r--   0 dbalogh    (501) staff       (20)        0 2023-05-23 07:58:02.000000 templatte-0.2/datamodel/__init__.py
+-rw-r--r--   0 dbalogh    (501) staff       (20)     1890 2023-05-23 11:36:17.000000 templatte-0.2/datamodel/data_source.py
+drwxr-xr-x   0 dbalogh    (501) staff       (20)        0 2023-05-24 06:29:59.960658 templatte-0.2/environment/
+-rw-r--r--   0 dbalogh    (501) staff       (20)        0 2023-05-23 06:47:17.000000 templatte-0.2/environment/__init__.py
+-rw-r--r--   0 dbalogh    (501) staff       (20)      934 2023-05-23 06:50:39.000000 templatte-0.2/environment/environment.py
+drwxr-xr-x   0 dbalogh    (501) staff       (20)        0 2023-05-24 06:29:59.966334 templatte-0.2/report/
+-rw-r--r--   0 dbalogh    (501) staff       (20)        0 2023-05-22 18:50:07.000000 templatte-0.2/report/__init__.py
+-rw-r--r--   0 dbalogh    (501) staff       (20)     1520 2023-05-24 06:12:20.000000 templatte-0.2/report/report.py
+drwxr-xr-x   0 dbalogh    (501) staff       (20)        0 2023-05-24 06:29:59.969830 templatte-0.2/reportmodel/
+-rw-r--r--   0 dbalogh    (501) staff       (20)        0 2023-05-19 12:50:56.000000 templatte-0.2/reportmodel/__init__.py
+-rw-r--r--   0 dbalogh    (501) staff       (20)     3637 2023-05-24 06:06:42.000000 templatte-0.2/reportmodel/report_generator.py
+-rw-r--r--   0 dbalogh    (501) staff       (20)      138 2023-05-23 06:46:02.000000 templatte-0.2/reportmodel/template.py
+-rw-r--r--   0 dbalogh    (501) staff       (20)       38 2023-05-24 06:29:59.973860 templatte-0.2/setup.cfg
+-rw-r--r--   0 dbalogh    (501) staff       (20)      424 2023-05-24 06:22:21.000000 templatte-0.2/setup.py
+drwxr-xr-x   0 dbalogh    (501) staff       (20)        0 2023-05-24 06:29:59.972826 templatte-0.2/templatte.egg-info/
+-rw-r--r--   0 dbalogh    (501) staff       (20)      245 2023-05-24 06:29:59.000000 templatte-0.2/templatte.egg-info/PKG-INFO
+-rw-r--r--   0 dbalogh    (501) staff       (20)      404 2023-05-24 06:29:59.000000 templatte-0.2/templatte.egg-info/SOURCES.txt
+-rw-r--r--   0 dbalogh    (501) staff       (20)        1 2023-05-24 06:29:59.000000 templatte-0.2/templatte.egg-info/dependency_links.txt
+-rw-r--r--   0 dbalogh    (501) staff       (20)       30 2023-05-24 06:29:59.000000 templatte-0.2/templatte.egg-info/requires.txt
+-rw-r--r--   0 dbalogh    (501) staff       (20)       41 2023-05-24 06:29:59.000000 templatte-0.2/templatte.egg-info/top_level.txt
```

### Comparing `templatte-0.1/LICENSE` & `templatte-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `templatte-0.1/datamodel/data_source.py` & `templatte-0.2/datamodel/data_source.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,24 +43,24 @@
 class CsvDataSource(IDataSource):
     """Data source for CSV files."""
 
     def __init__(self) -> None:
         """Initialize the CSV data source."""
         super().__init__()
 
-    def connect(self, connection: str, csv_params: dict = None) -> None:
+    def connect(self, connection: str, csv_args: dict = {}) -> None:
         """Connect to the CSV file."""
-        df = pd.read_csv(connection, **csv_params)
+        df = pd.read_csv(connection, **csv_args)
         self.data(df)
 
 
 class ExcelDataSource(IDataSource):
     """Data source for Excel files."""
 
-    def __init__(self, connection: str, excel_args: dict) -> None:
+    def __init__(self, connection: str, excel_args : dict = {}) -> None:
         """Initialize the Excel data source."""
         super().__init__()
         self.excel_args = excel_args
         self.connection = connection
 
     def connect(self) -> None:
         """Connect to the Excel file."""
```

### Comparing `templatte-0.1/environment/environment.py` & `templatte-0.2/environment/environment.py`

 * *Files identical despite different names*

### Comparing `templatte-0.1/reportmodel/report_generator.py` & `templatte-0.2/reportmodel/report_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Callable
 
 logger = environment.setup_logger()
 
 class ReportGenerator:
     """Generates reports in PDF format."""
 
-    def __init__(self, logo: Path, style: Path, template: Template = None) -> None:
+    def __init__(self, logo: Path = Path(), style: Path = Path(), template: Template = None) -> None:
         """
         Initialize the ReportGenerator object.
 
         Args:
             logo: The path to the logo file.
             style: The path to the CSS file.
             template: An optional Template object.
@@ -62,15 +62,15 @@
         """
         Set the template.
 
         Args:
             template: A Template object.
 
         """
-        self._template = Template
+        self._template = template
 
     @template.setter
     def template(self, template_folder: Path, template_file: Path) -> None:
         """
         Set the template using the template folder and file paths.
 
         Args:
@@ -112,20 +112,22 @@
         template_env = jinja2.Environment(loader=template_loader)
         template = template_env.get_template(str(self.template.template_file))
 
         # Generate the PDF
         try:
             data = self.format(data)
             output = template.render(
-                logo_path=str(self._logo.resolve()),
-                style=str(self._style.resolve()),
                 **data,
+                logo_path=str(self._logo.resolve()),
+                style=str(self._style.resolve())
             )
+            with open(f"{path}.html", "w") as html:
+                html.write(output)
             # Save the HTML to a PDF
             pdfkit.from_string(
                 output,
                 path,
                 options={"enable-local-file-access": ""},
             )
             return None
         except Exception as e:
-            logger.error(f'Error generating PDF for employee {data["user"]}: {e}')
+            logger.error(e)
```

