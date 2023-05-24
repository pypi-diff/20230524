# Comparing `tmp/tksheet-6.1.7.tar.gz` & `tmp/tksheet-6.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tksheet-6.1.7.tar", last modified: Tue May 23 08:14:15 2023, max compression
+gzip compressed data, was "tksheet-6.1.8.tar", last modified: Tue May 23 16:21:45 2023, max compression
```

## Comparing `tksheet-6.1.7.tar` & `tksheet-6.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 08:14:15.022253 tksheet-6.1.7/
--rw-rw-rw-   0        0        0     1101 2023-05-23 07:18:56.000000 tksheet-6.1.7/LICENSE.txt
--rw-rw-rw-   0        0        0     3657 2023-05-23 08:14:15.022253 tksheet-6.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     3007 2023-05-23 07:18:56.000000 tksheet-6.1.7/README.md
--rw-rw-rw-   0        0        0       86 2023-05-23 08:14:15.022253 tksheet-6.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1010 2023-05-23 07:43:27.000000 tksheet-6.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:14:15.014748 tksheet-6.1.7/tksheet/
--rw-rw-rw-   0        0        0     1901 2023-05-23 07:18:56.000000 tksheet-6.1.7/tksheet/__init__.py
--rw-rw-rw-   0        0        0   163926 2023-05-23 07:18:56.000000 tksheet-6.1.7/tksheet/_tksheet.py
--rw-rw-rw-   0        0        0   111612 2023-05-23 08:01:56.000000 tksheet-6.1.7/tksheet/_tksheet_column_headers.py
--rw-rw-rw-   0        0        0     8846 2023-05-23 07:18:56.000000 tksheet-6.1.7/tksheet/_tksheet_formatters.py
--rw-rw-rw-   0        0        0   329885 2023-05-23 08:10:54.000000 tksheet-6.1.7/tksheet/_tksheet_main_table.py
--rw-rw-rw-   0        0        0    12695 2023-05-23 07:18:57.000000 tksheet-6.1.7/tksheet/_tksheet_other_classes.py
--rw-rw-rw-   0        0        0   108542 2023-05-23 08:02:12.000000 tksheet-6.1.7/tksheet/_tksheet_row_index.py
--rw-rw-rw-   0        0        0     5746 2023-05-23 07:18:57.000000 tksheet-6.1.7/tksheet/_tksheet_top_left_rectangle.py
--rw-rw-rw-   0        0        0    59987 2023-05-23 07:18:57.000000 tksheet-6.1.7/tksheet/_tksheet_vars.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:14:15.022253 tksheet-6.1.7/tksheet.egg-info/
--rw-rw-rw-   0        0        0     3657 2023-05-23 08:14:14.000000 tksheet-6.1.7/tksheet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-05-23 08:14:14.000000 tksheet-6.1.7/tksheet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 08:14:14.000000 tksheet-6.1.7/tksheet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-23 08:14:14.000000 tksheet-6.1.7/tksheet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 16:21:45.498443 tksheet-6.1.8/
+-rw-rw-rw-   0        0        0     1101 2023-05-23 07:18:56.000000 tksheet-6.1.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     3657 2023-05-23 16:21:45.498443 tksheet-6.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3007 2023-05-23 07:18:56.000000 tksheet-6.1.8/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-23 16:21:45.498443 tksheet-6.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1010 2023-05-23 15:51:10.000000 tksheet-6.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:21:45.498443 tksheet-6.1.8/tksheet/
+-rw-rw-rw-   0        0        0     1901 2023-05-23 07:18:56.000000 tksheet-6.1.8/tksheet/__init__.py
+-rw-rw-rw-   0        0        0   164362 2023-05-23 15:59:10.000000 tksheet-6.1.8/tksheet/_tksheet.py
+-rw-rw-rw-   0        0        0   111722 2023-05-23 16:04:58.000000 tksheet-6.1.8/tksheet/_tksheet_column_headers.py
+-rw-rw-rw-   0        0        0     8846 2023-05-23 07:18:56.000000 tksheet-6.1.8/tksheet/_tksheet_formatters.py
+-rw-rw-rw-   0        0        0   333209 2023-05-23 16:16:46.000000 tksheet-6.1.8/tksheet/_tksheet_main_table.py
+-rw-rw-rw-   0        0        0    12695 2023-05-23 07:18:57.000000 tksheet-6.1.8/tksheet/_tksheet_other_classes.py
+-rw-rw-rw-   0        0        0   108646 2023-05-23 16:03:40.000000 tksheet-6.1.8/tksheet/_tksheet_row_index.py
+-rw-rw-rw-   0        0        0     5746 2023-05-23 07:18:57.000000 tksheet-6.1.8/tksheet/_tksheet_top_left_rectangle.py
+-rw-rw-rw-   0        0        0    59987 2023-05-23 07:18:57.000000 tksheet-6.1.8/tksheet/_tksheet_vars.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:21:45.498443 tksheet-6.1.8/tksheet.egg-info/
+-rw-rw-rw-   0        0        0     3657 2023-05-23 16:21:45.000000 tksheet-6.1.8/tksheet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-05-23 16:21:45.000000 tksheet-6.1.8/tksheet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 16:21:45.000000 tksheet-6.1.8/tksheet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-23 16:21:45.000000 tksheet-6.1.8/tksheet.egg-info/top_level.txt
```

### Comparing `tksheet-6.1.7/LICENSE.txt` & `tksheet-6.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.7/PKG-INFO` & `tksheet-6.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.1.7
+Version: 6.1.8
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.1.7.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.1.8.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `tksheet-6.1.7/README.md` & `tksheet-6.1.8/README.md`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.7/setup.py` & `tksheet-6.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding = 'utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'tksheet',
   packages = ['tksheet'],
-  version = '6.1.7',
+  version = '6.1.8',
   python_requires = '>=3.6',
   license = 'MIT',
   description = 'Tkinter table / sheet widget',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'ragardner',
   author_email = 'github@ragardner.simplelogin.com',
   url = 'https://github.com/ragardner/tksheet',
-  download_url = 'https://github.com/ragardner/tksheet/archive/6.1.7.tar.gz',
+  download_url = 'https://github.com/ragardner/tksheet/archive/6.1.8.tar.gz',
   keywords = ['tkinter', 'table', 'widget', 'sheet', 'grid', 'tk'],
   install_requires = [],
   classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License'
```

### Comparing `tksheet-6.1.7/tksheet/__init__.py` & `tksheet-6.1.8/tksheet/__init__.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.7/tksheet/_tksheet.py` & `tksheet-6.1.8/tksheet/_tksheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,16 @@
         max_header_height: str = "inf",  # str or int
         max_index_width: str = "inf",  # str or int
         row_index: list = None,
         index: list = None,
         after_redraw_time_ms: int = 20,
         row_index_width: int = None,
         auto_resize_default_row_index: bool = True,
+        auto_resize_columns: Union[int, None] = None,
+        auto_resize_rows: Union[int, None] = None,
         set_all_heights_and_widths: bool = False,
         row_height: str = "1",  # str or int
         font: tuple = get_font(),
         header_font: tuple = get_heading_font(),
         index_font: tuple = get_index_font(),  # currently has no effect
         popup_menu_font: tuple = get_font(),
         align: str = "w",
@@ -244,14 +246,16 @@
             to_clipboard_lineterminator=to_clipboard_lineterminator,
             from_clipboard_delimiters=from_clipboard_delimiters,
             column_headers_canvas=self.CH,
             row_index_canvas=self.RI,
             headers=headers,
             header=header,
             data_reference=data if data_reference is None else data_reference,
+            auto_resize_columns=auto_resize_columns,
+            auto_resize_rows=auto_resize_rows,
             total_cols=total_columns,
             total_rows=total_rows,
             row_index=row_index,
             index=index,
             font=font,
             header_font=header_font,
             index_font=index_font,
@@ -2223,14 +2227,18 @@
     def font(self, newfont=None, reset_row_positions=True):
         return self.MT.set_table_font(newfont, reset_row_positions=reset_row_positions)
 
     def header_font(self, newfont=None):
         return self.MT.set_header_font(newfont)
 
     def set_options(self, redraw=True, **kwargs):
+        if "auto_resize_columns" in kwargs:
+            self.MT.auto_resize_columns = kwargs["auto_resize_columns"]
+        if "auto_resize_rows" in kwargs:
+            self.MT.auto_resize_rows = kwargs["auto_resize_rows"]
         if "to_clipboard_delimiter" in kwargs:
             self.MT.to_clipboard_delimiter = kwargs["to_clipboard_delimiter"]
         if "to_clipboard_quotechar" in kwargs:
             self.MT.to_clipboard_quotechar = kwargs["to_clipboard_quotechar"]
         if "to_clipboard_lineterminator" in kwargs:
             self.MT.to_clipboard_lineterminator = kwargs["to_clipboard_lineterminator"]
         if "from_clipboard_delimiters" in kwargs:
```

### Comparing `tksheet-6.1.7/tksheet/_tksheet_column_headers.py` & `tksheet-6.1.8/tksheet/_tksheet_column_headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,14 +424,15 @@
             and self.width_resizing_enabled
             and self.rsz_w is not None
             and not self.currently_resizing_width
         ):
             col = self.rsz_w - 1
             old_width = self.MT.col_positions[self.rsz_w] - self.MT.col_positions[self.rsz_w - 1]
             new_width = self.set_col_width(col)
+            self.MT.allow_auto_resize_columns = False
             self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
             if self.column_width_resize_func is not None and old_width != new_width:
                 self.column_width_resize_func(ResizeEvent("column_width_resize", col, old_width, new_width))
         elif self.col_selection_enabled and self.rsz_h is None and self.rsz_w is None:
             c = self.MT.identify_col(x=event.x)
             if c < len(self.MT.col_positions) - 1:
                 if self.MT.single_selection_enabled:
@@ -825,14 +826,15 @@
                 new_col_pos = floor(self.MT.col_positions[self.rsz_w - 1] + self.MT.max_column_width)
             increment = new_col_pos - self.MT.col_positions[self.rsz_w]
             self.MT.col_positions[self.rsz_w + 1 :] = [
                 e + increment for e in islice(self.MT.col_positions, self.rsz_w + 1, len(self.MT.col_positions))
             ]
             self.MT.col_positions[self.rsz_w] = new_col_pos
             new_width = self.MT.col_positions[self.rsz_w] - self.MT.col_positions[self.rsz_w - 1]
+            self.MT.allow_auto_resize_columns = False
             self.MT.recreate_all_selection_boxes()
             self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
             if self.column_width_resize_func is not None and old_width != new_width:
                 self.column_width_resize_func(ResizeEvent("column_width_resize", self.rsz_w - 1, old_width, new_width))
         elif self.height_resizing_enabled and self.rsz_h is not None and self.currently_resizing_height:
             self.currently_resizing_height = False
             self.delete_all_resize_and_ctrl_lines(ctrl_lines=False)
```

### Comparing `tksheet-6.1.7/tksheet/_tksheet_formatters.py` & `tksheet-6.1.8/tksheet/_tksheet_formatters.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.7/tksheet/_tksheet_main_table.py` & `tksheet-6.1.8/tksheet/_tksheet_main_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,16 @@
         tk.Canvas.__init__(
             self,
             kwargs["parentframe"],
             background=kwargs["table_bg"],
             highlightthickness=0,
         )
         self.parentframe = kwargs["parentframe"]
+        self.parentframe_width = 0
+        self.parentframe_height = 0
         self.b1_pressed_loc = None
         self.existing_dropdown_canvas_id = None
         self.existing_dropdown_window = None
         self.closed_dropdown = None
         self.last_selected = tuple()
         self.centre_alignment_text_mod_indexes = (slice(1, None), slice(None, -1))
         self.c_align_cyc = cycle(self.centre_alignment_text_mod_indexes)
@@ -119,14 +121,18 @@
         )
         self.page_up_down_select_row = kwargs["page_up_down_select_row"]
         self.expand_sheet_if_paste_too_big = kwargs["expand_sheet_if_paste_too_big"]
         self.paste_insert_column_limit = kwargs["paste_insert_column_limit"]
         self.paste_insert_row_limit = kwargs["paste_insert_row_limit"]
         self.arrow_key_down_right_scroll_page = kwargs["arrow_key_down_right_scroll_page"]
         self.cell_auto_resize_enabled = kwargs["enable_edit_cell_auto_resize"]
+        self.auto_resize_columns = kwargs["auto_resize_columns"]
+        self.auto_resize_rows = kwargs["auto_resize_rows"]
+        self.allow_auto_resize_columns = True
+        self.allow_auto_resize_rows = True
         self.edit_cell_validation = kwargs["edit_cell_validation"]
         self.display_selected_fg_over_highlights = kwargs["display_selected_fg_over_highlights"]
         self.show_index = kwargs["show_index"]
         self.show_header = kwargs["show_header"]
         self.selected_rows_to_end_of_window = kwargs["selected_rows_to_end_of_window"]
         self.horizontal_grid_to_end_of_window = kwargs["horizontal_grid_to_end_of_window"]
         self.vertical_grid_to_end_of_window = kwargs["vertical_grid_to_end_of_window"]
@@ -326,20 +332,31 @@
         self.popup_menu_highlight_bg = kwargs["popup_menu_highlight_bg"]
         self.popup_menu_highlight_fg = kwargs["popup_menu_highlight_fg"]
         self.rc_popup_menu = None
         self.empty_rc_popup_menu = None
         self.basic_bindings()
         self.create_rc_menus()
 
-    def refresh(self, event=None):
+    def refresh(self, event=None) -> None:
+        self.main_table_redraw_grid_and_text(True, True)
+
+    def window_configured(self, event) -> None:
+        w = self.parentframe.winfo_width()
+        if w != self.parentframe_width:
+            self.parentframe_width = w
+            self.allow_auto_resize_columns = True
+        h = self.parentframe.winfo_height()
+        if h != self.parentframe_height:
+            self.parentframe_height = h
+            self.allow_auto_resize_rows = True
         self.main_table_redraw_grid_and_text(True, True)
 
     def basic_bindings(self, enable=True):
         if enable:
-            self.bind("<Configure>", self.refresh)
+            self.bind("<Configure>", self.window_configured)
             self.bind("<Motion>", self.mouse_motion)
             self.bind("<ButtonPress-1>", self.b1_press)
             self.bind("<B1-Motion>", self.b1_motion)
             self.bind("<ButtonRelease-1>", self.b1_release)
             self.bind("<Double-Button-1>", self.double_b1)
             self.bind("<MouseWheel>", self.mousewheel)
             if USER_OS == "linux":
@@ -4764,62 +4781,113 @@
                 else:
                     self.itemconfig(t, fill=fill, outline=outline, tag=tag, state="normal")
                 self.lift(t)
             else:
                 t = self.create_polygon(points, fill=fill, outline=outline, tag=tag, smooth=True)
             self.disp_checkbox[t] = True
 
-    def main_table_redraw_grid_and_text(self, redraw_header=False, redraw_row_index=False, redraw_table=True):
-        last_col_line_pos = self.col_positions[-1] + 1
-        last_row_line_pos = self.row_positions[-1] + 1
+    def main_table_redraw_grid_and_text(self, redraw_header=False, redraw_row_index=False, redraw_table=True,):
         try:
             can_width = self.winfo_width()
             can_height = self.winfo_height()
-            self.configure(
-                scrollregion=(
-                    0,
-                    0,
-                    last_col_line_pos + self.empty_horizontal,
-                    last_row_line_pos + self.empty_vertical,
-                )
-            )
         except Exception:
-            return
+            return False
+        row_pos_exists = self.row_positions != [0] and self.row_positions
+        col_pos_exists = self.col_positions != [0] and self.col_positions
+        resized_cols = False
+        resized_rows = False
+        if self.auto_resize_columns and self.allow_auto_resize_columns and col_pos_exists:
+            max_w = int(can_width)
+            max_w -= self.empty_horizontal
+            if (len(self.col_positions) - 1) * self.auto_resize_columns < max_w:
+                resized_cols = True
+                change = int((max_w - self.col_positions[-1]) / (len(self.col_positions) - 1))
+                widths = [
+                    int(b - a) + change - 1
+                    for a, b in zip(self.col_positions, islice(self.col_positions, 1, len(self.col_positions)))
+                ]
+                diffs = {}
+                for i, w in enumerate(widths):
+                    if w < self.auto_resize_columns:
+                        diffs[i] = self.auto_resize_columns - w
+                        widths[i] = self.auto_resize_columns
+                if diffs and len(diffs) < len(widths):
+                    change = sum(diffs.values()) / (len(widths) - len(diffs))
+                    for i, w in enumerate(widths):
+                        if i not in diffs:
+                            widths[i] -= change
+                self.col_positions = list(accumulate(chain([0], widths)))
+        if self.auto_resize_rows and self.allow_auto_resize_rows and row_pos_exists:
+            max_h = int(can_height)
+            max_h -= self.empty_vertical
+            if (len(self.row_positions) - 1) * self.auto_resize_rows < max_h:
+                resized_rows = True
+                change = int((max_h - self.row_positions[-1]) / (len(self.row_positions) - 1))
+                heights = [
+                    int(b - a) + change - 1
+                    for a, b in zip(self.row_positions, islice(self.row_positions, 1, len(self.row_positions)))
+                ]
+                diffs = {}
+                for i, h in enumerate(heights):
+                    if h < self.auto_resize_rows:
+                        diffs[i] = self.auto_resize_rows - h
+                        heights[i] = self.auto_resize_rows
+                if diffs and len(diffs) < len(heights):
+                    change = sum(diffs.values()) / (len(heights) - len(diffs))
+                    for i, h in enumerate(heights):
+                        if i not in diffs:
+                            heights[i] -= change
+                self.row_positions = list(accumulate(chain([0], heights)))
+        if resized_cols or resized_rows:
+            self.recreate_all_selection_boxes()
+        last_col_line_pos = self.col_positions[-1] + 1
+        last_row_line_pos = self.row_positions[-1] + 1
         if can_width >= last_col_line_pos + self.empty_horizontal and self.parentframe.xscroll_showing:
             self.parentframe.xscroll.grid_forget()
             self.parentframe.xscroll_showing = False
         elif (
             can_width < last_col_line_pos + self.empty_horizontal
             and not self.parentframe.xscroll_showing
             and not self.parentframe.xscroll_disabled
-            and can_height > 45
+            and can_height > 40
         ):
             self.parentframe.xscroll.grid(row=2, column=0, columnspan=2, sticky="nswe")
             self.parentframe.xscroll_showing = True
         if can_height >= last_row_line_pos + self.empty_vertical and self.parentframe.yscroll_showing:
             self.parentframe.yscroll.grid_forget()
             self.parentframe.yscroll_showing = False
         elif (
             can_height < last_row_line_pos + self.empty_vertical
             and not self.parentframe.yscroll_showing
             and not self.parentframe.yscroll_disabled
-            and can_width > 45
+            and can_width > 40
         ):
             self.parentframe.yscroll.grid(row=0, column=2, rowspan=3, sticky="nswe")
             self.parentframe.yscroll_showing = True
+        self.configure(
+            scrollregion=(
+                0,
+                0,
+                last_col_line_pos + self.empty_horizontal + 2,
+                last_row_line_pos + self.empty_vertical + 2,
+            )
+        )
         scrollpos_bot = self.canvasy(can_height)
         end_row = bisect.bisect_right(self.row_positions, scrollpos_bot)
         if not scrollpos_bot >= self.row_positions[-1]:
             end_row += 1
         if redraw_row_index and self.show_index:
             self.RI.auto_set_index_width(end_row - 1)
+            # return
         scrollpos_left = self.canvasx(0)
         scrollpos_top = self.canvasy(0)
         scrollpos_right = self.canvasx(can_width)
         start_row = bisect.bisect_left(self.row_positions, scrollpos_top)
+        start_col = bisect.bisect_left(self.col_positions, scrollpos_left)
+        end_col = bisect.bisect_right(self.col_positions, scrollpos_right)
         self.row_width_resize_bbox = (
             scrollpos_left,
             scrollpos_top,
             scrollpos_left + 2,
             scrollpos_bot,
         )
         self.header_height_resize_bbox = (
@@ -4842,28 +4910,25 @@
         self.disp_high = defaultdict(set)
         self.hidd_grid.update(self.disp_grid)
         self.disp_grid = {}
         self.hidd_dropdown.update(self.disp_dropdown)
         self.disp_dropdown = {}
         self.hidd_checkbox.update(self.disp_checkbox)
         self.disp_checkbox = {}
-        start_col = bisect.bisect_left(self.col_positions, scrollpos_left)
-        end_col = bisect.bisect_right(self.col_positions, scrollpos_right)
+
         if not scrollpos_right >= self.col_positions[-1]:
             end_col += 1
         if last_col_line_pos > scrollpos_right:
             x_stop = scrollpos_right
         else:
             x_stop = last_col_line_pos
         if last_row_line_pos > scrollpos_bot:
             y_stop = scrollpos_bot
         else:
             y_stop = last_row_line_pos
-        row_pos_exists = self.row_positions != [0] and self.row_positions
-        col_pos_exists = self.col_positions != [0] and self.col_positions
         if self.show_horizontal_grid and row_pos_exists:
             self.grid_cyc = cycle(self.grid_cyctup)
             points = []
             if self.horizontal_grid_to_end_of_window:
                 x_grid_stop = scrollpos_right + can_width
             else:
                 if last_col_line_pos > scrollpos_right:
```

### Comparing `tksheet-6.1.7/tksheet/_tksheet_other_classes.py` & `tksheet-6.1.8/tksheet/_tksheet_other_classes.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.7/tksheet/_tksheet_row_index.py` & `tksheet-6.1.8/tksheet/_tksheet_row_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,14 +370,15 @@
             and self.height_resizing_enabled
             and self.rsz_h is not None
             and not self.currently_resizing_height
         ):
             row = self.rsz_h - 1
             old_height = self.MT.row_positions[self.rsz_h] - self.MT.row_positions[self.rsz_h - 1]
             new_height = self.set_row_height(row)
+            self.MT.allow_auto_resize_rows = False
             self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
             if self.row_height_resize_func is not None and old_height != new_height:
                 self.row_height_resize_func(ResizeEvent("row_height_resize", row, old_height, new_height))
         elif self.width_resizing_enabled and self.rsz_h is None and self.rsz_w:
             self.set_width_of_index_to_text()
         elif self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None:
             r = self.MT.identify_row(y=event.y)
@@ -779,14 +780,15 @@
             elif size > self.MT.max_row_height:
                 new_row_pos = floor(self.MT.row_positions[self.rsz_h - 1] + self.MT.max_row_height)
             increment = new_row_pos - self.MT.row_positions[self.rsz_h]
             self.MT.row_positions[self.rsz_h + 1 :] = [
                 e + increment for e in islice(self.MT.row_positions, self.rsz_h + 1, len(self.MT.row_positions))
             ]
             self.MT.row_positions[self.rsz_h] = new_row_pos
+            self.MT.allow_auto_resize_rows = False
             new_height = self.MT.row_positions[self.rsz_h] - self.MT.row_positions[self.rsz_h - 1]
             self.MT.recreate_all_selection_boxes()
             self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
             if self.row_height_resize_func is not None and old_height != new_height:
                 self.row_height_resize_func(ResizeEvent("row_height_resize", self.rsz_h - 1, old_height, new_height))
         elif self.width_resizing_enabled and self.rsz_w is not None and self.currently_resizing_width:
             self.currently_resizing_width = False
```

### Comparing `tksheet-6.1.7/tksheet/_tksheet_top_left_rectangle.py` & `tksheet-6.1.8/tksheet/_tksheet_top_left_rectangle.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.7/tksheet/_tksheet_vars.py` & `tksheet-6.1.8/tksheet/_tksheet_vars.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.7/tksheet.egg-info/PKG-INFO` & `tksheet-6.1.8/tksheet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.1.7
+Version: 6.1.8
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.1.7.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.1.8.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

