# Comparing `tmp/nico-font-tool-0.0.2.tar.gz` & `tmp/nico-font-tool-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nico-font-tool-0.0.2.tar", last modified: Mon May  8 11:34:25 2023, max compression
+gzip compressed data, was "nico-font-tool-0.0.3.tar", last modified: Wed May 24 06:44:47 2023, max compression
```

## Comparing `nico-font-tool-0.0.2.tar` & `nico-font-tool-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:34:25.692727 nico-font-tool-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 11:34:09.000000 nico-font-tool-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-08 11:34:25.692727 nico-font-tool-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-08 11:34:09.000000 nico-font-tool-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-08 11:34:09.000000 nico-font-tool-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 11:34:25.692727 nico-font-tool-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:34:25.688727 nico-font-tool-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:34:25.692727 nico-font-tool-0.0.2/src/nico_font_tool/
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-08 11:34:09.000000 nico-font-tool-0.0.2/src/nico_font_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-08 11:34:09.000000 nico-font-tool-0.0.2/src/nico_font_tool/bdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-08 11:34:09.000000 nico-font-tool-0.0.2/src/nico_font_tool/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-08 11:34:09.000000 nico-font-tool-0.0.2/src/nico_font_tool/nicofont.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-08 11:34:09.000000 nico-font-tool-0.0.2/src/nico_font_tool/opentype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:34:25.692727 nico-font-tool-0.0.2/src/nico_font_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-08 11:34:25.000000 nico-font-tool-0.0.2/src/nico_font_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-08 11:34:25.000000 nico-font-tool-0.0.2/src/nico_font_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:34:25.000000 nico-font-tool-0.0.2/src/nico_font_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-08 11:34:25.000000 nico-font-tool-0.0.2/src/nico_font_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-08 11:34:25.000000 nico-font-tool-0.0.2/src/nico_font_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 11:34:25.000000 nico-font-tool-0.0.2/src/nico_font_tool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:34:25.692727 nico-font-tool-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-08 11:34:09.000000 nico-font-tool-0.0.2/tests/test_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:44:47.740398 nico-font-tool-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-24 06:44:32.000000 nico-font-tool-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-24 06:44:47.740398 nico-font-tool-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-24 06:44:32.000000 nico-font-tool-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-24 06:44:32.000000 nico-font-tool-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 06:44:47.740398 nico-font-tool-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:44:47.736398 nico-font-tool-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:44:47.740398 nico-font-tool-0.0.3/src/nico_font_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-24 06:44:32.000000 nico-font-tool-0.0.3/src/nico_font_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-24 06:44:32.000000 nico-font-tool-0.0.3/src/nico_font_tool/bdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-24 06:44:32.000000 nico-font-tool-0.0.3/src/nico_font_tool/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-24 06:44:32.000000 nico-font-tool-0.0.3/src/nico_font_tool/nicofont.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-24 06:44:32.000000 nico-font-tool-0.0.3/src/nico_font_tool/opentype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:44:47.740398 nico-font-tool-0.0.3/src/nico_font_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-24 06:44:47.000000 nico-font-tool-0.0.3/src/nico_font_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-24 06:44:47.000000 nico-font-tool-0.0.3/src/nico_font_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 06:44:47.000000 nico-font-tool-0.0.3/src/nico_font_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 06:44:47.000000 nico-font-tool-0.0.3/src/nico_font_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-24 06:44:47.000000 nico-font-tool-0.0.3/src/nico_font_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 06:44:47.000000 nico-font-tool-0.0.3/src/nico_font_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:44:47.740398 nico-font-tool-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-24 06:44:32.000000 nico-font-tool-0.0.3/tests/test_.py
```

### Comparing `nico-font-tool-0.0.2/LICENSE` & `nico-font-tool-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nico-font-tool-0.0.2/PKG-INFO` & `nico-font-tool-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nico-font-tool
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool for converting fonts to NICO Game Framework format fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/nico-font-tool.python
 Project-URL: source, https://github.com/TakWolf/nico-font-tool.python
 Project-URL: issues, https://github.com/TakWolf/nico-font-tool.python/issues
@@ -33,34 +33,40 @@
 ## Usage
 
 ### Command
 
 Use `nicofont -h` to learn more.
 
 ```commandline
-nicofont ./assets/fonts/quan/quan.ttf ./build/quan quan --font_size 8 -gaw -1
+nicofont assets/fonts/quan/quan.ttf build/demo quan --font_size 8
 ```
 
 ### Scripts
 
-See: [Demo](examples/demo.py)
+See: [demo](examples/demo.py)
 
 ```python
+import nico_font_tool
+
 sheet_data, alphabet = nico_font_tool.create_sheet(
-    font_file_path,
-    font_size,
-    glyph_offset_x,
-    glyph_offset_y,
-    glyph_adjust_width,
-    glyph_adjust_height,
+    font_file_path='your/font/file/path.ttf', 
+    font_size=8,
 )
 
-nico_font_tool.save_palette_png(sheet_data, outputs_dir, outputs_name)
-nico_font_tool.save_dat_file(alphabet, outputs_dir, outputs_name)
+nico_font_tool.save_palette_png(sheet_data, 'outputs/palette/dir', 'outputs_name')
+nico_font_tool.save_dat_file(alphabet, 'outputs/palette/dir', 'outputs_name')
     
-nico_font_tool.save_rgba_png(sheet_data, outputs_dir, outputs_name)
-nico_font_tool.save_dat_file(alphabet, outputs_dir, outputs_name)
+nico_font_tool.save_rgba_png(sheet_data, 'outputs/rgba/dir', 'outputs_name')
+nico_font_tool.save_dat_file(alphabet, 'outputs/rgba/dir', 'outputs_name')
 ```
 
+## Dependencies
+
+- [FontTools](https://github.com/fonttools/fonttools)
+- [Brotli](https://github.com/google/brotli)
+- [BdfFont](https://github.com/TakWolf/bdffont)
+- [Pillow](https://github.com/python-pillow/Pillow)
+- [PyPNG](https://gitlab.com/drj11/pypng)
+
 ## License
 
 Under the [MIT license](LICENSE).
```

### Comparing `nico-font-tool-0.0.2/pyproject.toml` & `nico-font-tool-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nico-font-tool"
-version = "0.0.2"
+version = "0.0.3"
 description = "A tool for converting fonts to NICO Game Framework format fonts."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
```

### Comparing `nico-font-tool-0.0.2/src/nico_font_tool/__init__.py` & `nico-font-tool-0.0.3/src/nico_font_tool/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             font_file_path,
             glyph_offset_x,
             glyph_offset_y,
             glyph_adjust_width,
             glyph_adjust_height,
         )
     else:
-        raise Exception(f'Font file type not supported: {font_ext}')
+        raise Exception(f'font file type not supported: {font_ext}')
     logger.info(f'loaded font file: {font_file_path}')
 
     # 图集对象，初始化左边界
     sheet_data = [[_glyph_data_border] for _ in range(font_rasterizer.adjusted_line_height)]
 
     # 字母表
     alphabet = []
```

### Comparing `nico-font-tool-0.0.2/src/nico_font_tool/bdf.py` & `nico-font-tool-0.0.3/src/nico_font_tool/bdf.py`

 * *Files identical despite different names*

### Comparing `nico-font-tool-0.0.2/src/nico_font_tool/font.py` & `nico-font-tool-0.0.3/src/nico_font_tool/font.py`

 * *Files identical despite different names*

### Comparing `nico-font-tool-0.0.2/src/nico_font_tool/nicofont.py` & `nico-font-tool-0.0.3/src/nico_font_tool/nicofont.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,35 +12,35 @@
     outputs_dir = args.outputs_dir
     outputs_name = args.outputs_name
     font_size = args.font_size
     glyph_offset_x = args.glyph_offset_x
     glyph_offset_y = args.glyph_offset_y
     glyph_adjust_width = args.glyph_adjust_width
     glyph_adjust_height = args.glyph_adjust_height
-    png_type = args.png_type = args.png_type
+    mode = args.mode
 
-    if png_type != 'palette' and png_type != 'rgba':
-        raise Exception(f"Unsupported png type: '{png_type}'")
+    if mode != 'palette' and mode != 'rgba':
+        raise Exception(f"unsupported png mode: '{mode}'")
 
     if not os.path.exists(outputs_dir):
         os.makedirs(outputs_dir)
 
     sheet_data, alphabet = nico_font_tool.create_sheet(
         font_file_path,
         font_size,
         glyph_offset_x,
         glyph_offset_y,
         glyph_adjust_width,
         glyph_adjust_height,
     )
 
-    if png_type == 'palette':
+    if mode == 'palette':
         nico_font_tool.save_palette_png(sheet_data, outputs_dir, outputs_name)
         nico_font_tool.save_dat_file(alphabet, outputs_dir, outputs_name)
-    elif png_type == 'rgba':
+    elif mode == 'rgba':
         nico_font_tool.save_rgba_png(sheet_data, outputs_dir, outputs_name)
         nico_font_tool.save_dat_file(alphabet, outputs_dir, outputs_name)
 
 
 def main():
     parser = argparse.ArgumentParser(
         prog='NICO Font Tool',
@@ -50,13 +50,13 @@
     parser.add_argument('outputs_dir', type=str, help='Output files dir.')
     parser.add_argument('outputs_name', type=str, help='Output files name.')
     parser.add_argument('-fs', '--font_size', type=int, help='Glyph rasterize size when using OpenType font.')
     parser.add_argument('-gox', '--glyph_offset_x', type=int, default=0, help='Glyph offset x.')
     parser.add_argument('-goy', '--glyph_offset_y', type=int, default=0, help='Glyph offset y.')
     parser.add_argument('-gaw', '--glyph_adjust_width', type=int, default=0, help='Glyph adjust width.')
     parser.add_argument('-gah', '--glyph_adjust_height', type=int, default=0, help='Glyph adjust height.')
-    parser.add_argument('-pt', '--png_type', type=str, default='palette', help="Png sheet color type, can be 'palette' or 'rgba', default is 'palette'")
+    parser.add_argument('-m', '--mode', type=str, default='palette', help="Png sheet color mode, can be 'palette' or 'rgba', default is 'palette'.")
     execute(parser.parse_args())
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `nico-font-tool-0.0.2/src/nico_font_tool/opentype.py` & `nico-font-tool-0.0.3/src/nico_font_tool/opentype.py`

 * *Files identical despite different names*

### Comparing `nico-font-tool-0.0.2/src/nico_font_tool.egg-info/PKG-INFO` & `nico-font-tool-0.0.3/src/nico_font_tool.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nico-font-tool
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool for converting fonts to NICO Game Framework format fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/nico-font-tool.python
 Project-URL: source, https://github.com/TakWolf/nico-font-tool.python
 Project-URL: issues, https://github.com/TakWolf/nico-font-tool.python/issues
@@ -33,34 +33,40 @@
 ## Usage
 
 ### Command
 
 Use `nicofont -h` to learn more.
 
 ```commandline
-nicofont ./assets/fonts/quan/quan.ttf ./build/quan quan --font_size 8 -gaw -1
+nicofont assets/fonts/quan/quan.ttf build/demo quan --font_size 8
 ```
 
 ### Scripts
 
-See: [Demo](examples/demo.py)
+See: [demo](examples/demo.py)
 
 ```python
+import nico_font_tool
+
 sheet_data, alphabet = nico_font_tool.create_sheet(
-    font_file_path,
-    font_size,
-    glyph_offset_x,
-    glyph_offset_y,
-    glyph_adjust_width,
-    glyph_adjust_height,
+    font_file_path='your/font/file/path.ttf', 
+    font_size=8,
 )
 
-nico_font_tool.save_palette_png(sheet_data, outputs_dir, outputs_name)
-nico_font_tool.save_dat_file(alphabet, outputs_dir, outputs_name)
+nico_font_tool.save_palette_png(sheet_data, 'outputs/palette/dir', 'outputs_name')
+nico_font_tool.save_dat_file(alphabet, 'outputs/palette/dir', 'outputs_name')
     
-nico_font_tool.save_rgba_png(sheet_data, outputs_dir, outputs_name)
-nico_font_tool.save_dat_file(alphabet, outputs_dir, outputs_name)
+nico_font_tool.save_rgba_png(sheet_data, 'outputs/rgba/dir', 'outputs_name')
+nico_font_tool.save_dat_file(alphabet, 'outputs/rgba/dir', 'outputs_name')
 ```
 
+## Dependencies
+
+- [FontTools](https://github.com/fonttools/fonttools)
+- [Brotli](https://github.com/google/brotli)
+- [BdfFont](https://github.com/TakWolf/bdffont)
+- [Pillow](https://github.com/python-pillow/Pillow)
+- [PyPNG](https://gitlab.com/drj11/pypng)
+
 ## License
 
 Under the [MIT license](LICENSE).
```

