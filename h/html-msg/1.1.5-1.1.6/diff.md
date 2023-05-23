# Comparing `tmp/html_msg-1.1.5.tar.gz` & `tmp/html_msg-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_msg-1.1.5.tar", last modified: Tue May 23 20:34:59 2023, max compression
+gzip compressed data, was "html_msg-1.1.6.tar", last modified: Tue May 23 21:58:53 2023, max compression
```

## Comparing `html_msg-1.1.5.tar` & `html_msg-1.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 20:34:59.153998 html_msg-1.1.5/
--rw-rw-rw-   0        0        0     1095 2023-05-06 11:32:57.000000 html_msg-1.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0     3988 2023-05-23 20:34:59.153998 html_msg-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3383 2023-05-09 19:29:44.000000 html_msg-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 20:34:59.147007 html_msg-1.1.5/html_msg/
--rw-rw-rw-   0        0        0      115 2023-05-23 20:34:39.000000 html_msg-1.1.5/html_msg/__init__.py
--rw-rw-rw-   0        0        0    12112 2023-05-12 12:59:50.000000 html_msg-1.1.5/html_msg/html_message.py
--rw-rw-rw-   0        0        0    15706 2023-05-23 20:34:08.000000 html_msg-1.1.5/html_msg/html_table.py
-drwxrwxrwx   0        0        0        0 2023-05-23 20:34:59.153000 html_msg-1.1.5/html_msg.egg-info/
--rw-rw-rw-   0        0        0     3988 2023-05-23 20:34:59.000000 html_msg-1.1.5/html_msg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-05-23 20:34:59.000000 html_msg-1.1.5/html_msg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 20:34:59.000000 html_msg-1.1.5/html_msg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-23 20:34:59.000000 html_msg-1.1.5/html_msg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-23 20:34:59.000000 html_msg-1.1.5/html_msg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 20:34:59.154997 html_msg-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      823 2023-05-23 20:34:17.000000 html_msg-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 21:58:53.434589 html_msg-1.1.6/
+-rw-rw-rw-   0        0        0     1095 2023-05-06 11:32:57.000000 html_msg-1.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     3988 2023-05-23 21:58:53.434589 html_msg-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3383 2023-05-09 19:29:44.000000 html_msg-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 21:58:53.429594 html_msg-1.1.6/html_msg/
+-rw-rw-rw-   0        0        0      115 2023-05-23 21:58:19.000000 html_msg-1.1.6/html_msg/__init__.py
+-rw-rw-rw-   0        0        0    12112 2023-05-12 12:59:50.000000 html_msg-1.1.6/html_msg/html_message.py
+-rw-rw-rw-   0        0        0    15528 2023-05-23 21:58:06.000000 html_msg-1.1.6/html_msg/html_table.py
+drwxrwxrwx   0        0        0        0 2023-05-23 21:58:53.434589 html_msg-1.1.6/html_msg.egg-info/
+-rw-rw-rw-   0        0        0     3988 2023-05-23 21:58:53.000000 html_msg-1.1.6/html_msg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-05-23 21:58:53.000000 html_msg-1.1.6/html_msg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 21:58:53.000000 html_msg-1.1.6/html_msg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-23 21:58:53.000000 html_msg-1.1.6/html_msg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-23 21:58:53.000000 html_msg-1.1.6/html_msg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 21:58:53.435587 html_msg-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      823 2023-05-23 21:58:31.000000 html_msg-1.1.6/setup.py
```

### Comparing `html_msg-1.1.5/LICENSE.txt` & `html_msg-1.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `html_msg-1.1.5/PKG-INFO` & `html_msg-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html_msg
-Version: 1.1.5
+Version: 1.1.6
 Summary: This tool allows you to create HTML messages using simple methods, without the need to write HTML code manually.
 Home-page: https://github.com/Sirakan-B/html_msg/
 Author: Sirakan Bagdasarian
 Author-email: bsirak@bk.ru
 License: MIT
 Download-URL: https://pypi.org/project/html-msg/
 Keywords: HTML,Message
```

### Comparing `html_msg-1.1.5/README.md` & `html_msg-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `html_msg-1.1.5/html_msg/html_message.py` & `html_msg-1.1.6/html_msg/html_message.py`

 * *Files identical despite different names*

### Comparing `html_msg-1.1.5/html_msg/html_table.py` & `html_msg-1.1.6/html_msg/html_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,21 +35,21 @@
         
         self.headers = headers
         self.cell_color_map = {}
         self.cell_style_map = {}
         self.font_family = 'Arial'
         self.font_size = '12px'
         self.font_color = 'black'
-        self.__table_align = 'margin-right: auto;'
+        self.table_align = "left"
         self.table_style = self.presets["Basic"]["table_style"]
         self.header_style = self.presets["Basic"]["header_style"]
         self.html_table  = ''
     
     def __update_table(self):
-        self.html_table = f'<table style="font-family: {self.font_family}; font-size: {self.font_size}; color: {self.font_color}; {self.__table_align}">\n'
+        self.html_table = f'<table align={self.table_align} style="font-family: {self.font_family}; font-size: {self.font_size}; color: {self.font_color}; ">\n'
         self.__update_headers()
         self.__update_rows()
         self.html_table += '</table>'
     
     def __update_headers(self):
         # Add headers if they exist
         if self.headers:
@@ -176,21 +176,17 @@
         Returns:
             None
 
         Example:
             align_table('center')
         """
 
-        position_and_css = {
-            'left': 'margin-right: auto;',
-            'right': 'margin-left: auto;',
-            'center': 'margin-right: auto; margin-left: auto;'
-        }
-        if position in position_and_css.keys():
-            self.__table_align = position_and_css[position]
+        valid_positions = ['left', 'right', 'center']
+        if position in valid_positions:
+            self.table_align = position
         else:
             raise ValueError(f"Invalid argument <{position}>. \
                              Position must be either 'left', 'right' or 'center'.")
 
     def get_cell_content(self, row_index, col_index):
         
         '''
```

### Comparing `html_msg-1.1.5/html_msg.egg-info/PKG-INFO` & `html_msg-1.1.6/html_msg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html-msg
-Version: 1.1.5
+Version: 1.1.6
 Summary: This tool allows you to create HTML messages using simple methods, without the need to write HTML code manually.
 Home-page: https://github.com/Sirakan-B/html_msg/
 Author: Sirakan Bagdasarian
 Author-email: bsirak@bk.ru
 License: MIT
 Download-URL: https://pypi.org/project/html-msg/
 Keywords: HTML,Message
```

### Comparing `html_msg-1.1.5/setup.py` & `html_msg-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 
 
 setup_args = dict(
     name='html_msg',
-    version='1.1.5',
+    version='1.1.6',
     description='This tool allows you to create HTML messages using simple methods, without the need to write HTML code manually.',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n',
     license='MIT',
     packages=find_packages(),
     author='Sirakan Bagdasarian',
     author_email='bsirak@bk.ru',
```

