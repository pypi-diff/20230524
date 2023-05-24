# Comparing `tmp/tkblock-2.0.0.tar.gz` & `tmp/tkblock-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkblock-2.0.0.tar", last modified: Sun May 21 23:51:33 2023, max compression
+gzip compressed data, was "tkblock-2.1.0.tar", last modified: Mon May 22 13:41:30 2023, max compression
```

## Comparing `tkblock-2.0.0.tar` & `tkblock-2.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 23:51:33.170749 tkblock-2.0.0/
--rw-rw-rw-   0        0        0     1077 2023-03-07 11:27:05.000000 tkblock-2.0.0/LICENSE
--rw-rw-rw-   0        0        0    14648 2023-05-21 23:51:33.166758 tkblock-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    13939 2023-05-21 23:48:51.000000 tkblock-2.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-21 23:51:33.171747 tkblock-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1017 2023-05-21 23:50:22.000000 tkblock-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 23:51:33.145379 tkblock-2.0.0/tkblock/
--rw-rw-rw-   0        0        0      584 2023-05-19 17:11:52.000000 tkblock-2.0.0/tkblock/__init__.py
--rw-rw-rw-   0        0        0     3408 2023-05-19 17:11:52.000000 tkblock-2.0.0/tkblock/block_framebase.py
--rw-rw-rw-   0        0        0    21644 2023-05-19 17:11:52.000000 tkblock-2.0.0/tkblock/block_framework.py
--rw-rw-rw-   0        0        0    38937 2023-05-19 17:11:52.000000 tkblock-2.0.0/tkblock/block_service.py
--rw-rw-rw-   0        0        0      426 2023-05-19 17:11:52.000000 tkblock-2.0.0/tkblock/block_util.py
--rw-rw-rw-   0        0        0     1418 2023-05-19 17:11:52.000000 tkblock-2.0.0/tkblock/canvas.py
--rw-rw-rw-   0        0        0      494 2023-05-19 17:11:53.000000 tkblock-2.0.0/tkblock/layout.py
--rw-rw-rw-   0        0        0      368 2023-05-19 17:11:53.000000 tkblock-2.0.0/tkblock/scrollbar.py
-drwxrwxrwx   0        0        0        0 2023-05-21 23:51:33.161683 tkblock-2.0.0/tkblock.egg-info/
--rw-rw-rw-   0        0        0    14648 2023-05-21 23:51:32.000000 tkblock-2.0.0/tkblock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-05-21 23:51:32.000000 tkblock-2.0.0/tkblock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 23:51:32.000000 tkblock-2.0.0/tkblock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-21 23:51:32.000000 tkblock-2.0.0/tkblock.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 13:41:30.640934 tkblock-2.1.0/
+-rw-rw-rw-   0        0        0     1077 2023-03-07 11:27:05.000000 tkblock-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0    14649 2023-05-22 13:41:30.639936 tkblock-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13940 2023-05-22 12:58:56.000000 tkblock-2.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 13:41:30.640934 tkblock-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1017 2023-05-22 13:40:50.000000 tkblock-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 13:41:30.623462 tkblock-2.1.0/tkblock/
+-rw-rw-rw-   0        0        0      584 2023-05-19 17:11:52.000000 tkblock-2.1.0/tkblock/__init__.py
+-rw-rw-rw-   0        0        0     3408 2023-05-19 17:11:52.000000 tkblock-2.1.0/tkblock/block_framebase.py
+-rw-rw-rw-   0        0        0    21644 2023-05-19 17:11:52.000000 tkblock-2.1.0/tkblock/block_framework.py
+-rw-rw-rw-   0        0        0    39843 2023-05-22 13:08:08.000000 tkblock-2.1.0/tkblock/block_service.py
+-rw-rw-rw-   0        0        0      426 2023-05-19 17:11:52.000000 tkblock-2.1.0/tkblock/block_util.py
+-rw-rw-rw-   0        0        0     1418 2023-05-19 17:11:52.000000 tkblock-2.1.0/tkblock/canvas.py
+-rw-rw-rw-   0        0        0      494 2023-05-19 17:11:53.000000 tkblock-2.1.0/tkblock/layout.py
+-rw-rw-rw-   0        0        0      368 2023-05-19 17:11:53.000000 tkblock-2.1.0/tkblock/scrollbar.py
+drwxrwxrwx   0        0        0        0 2023-05-22 13:41:30.636944 tkblock-2.1.0/tkblock.egg-info/
+-rw-rw-rw-   0        0        0    14649 2023-05-22 13:41:30.000000 tkblock-2.1.0/tkblock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-05-22 13:41:30.000000 tkblock-2.1.0/tkblock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 13:41:30.000000 tkblock-2.1.0/tkblock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-22 13:41:30.000000 tkblock-2.1.0/tkblock.egg-info/top_level.txt
```

### Comparing `tkblock-2.0.0/LICENSE` & `tkblock-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tkblock-2.0.0/PKG-INFO` & `tkblock-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkblock
-Version: 2.0.0
+Version: 2.1.0
 Summary: tkinter block framework
 Home-page: https://github.com/kuri-pome/tkblock
 Author: kuri_pome
 License: MIT
 Keywords: tkinter place widget easy
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
@@ -298,15 +298,15 @@
 In the above figure, 30px vertical and horizontal scrollbars are placed.
 The code for this is shown below.
 
 ```python
 root = BlockService.init("test_scrollbar", 5, 5, 600, 400, is_debug=True)
 frame = BlockService.create_frame("test_scrollbar")
 listbox_list = tuple([str(x) for x in range(0, 100)] + ["aabfsdgadfsgasdfkj;adsfadsj;kjfeijof"])
-_, listbox_var = tk.Listbox(frame, 1, 2, 1, 4, str_value=listbox_list)
+_, listbox_var = tk.Listbox(frame, 1, 2, 1, 4, init_value=listbox_list)
 listbox.scrollbar = BlockService.scrollbar(frame, x_enable=True, y_enable=True, size=30)
 BlockService.place_frame_widget()
 root.mainloop()
 ```
 
 The basic usage of the scrollbar is the same. If you want the scrollbar to be placed automatically, you can place it by linking the scrollbar to the widget.  
 If you wish to manually place it anywhere you wish, simply specify the layout as you would for a normal widget.
```

### Comparing `tkblock-2.0.0/README.md` & `tkblock-2.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,15 @@
 In the above figure, 30px vertical and horizontal scrollbars are placed.
 The code for this is shown below.
 
 ```python
 root = BlockService.init("test_scrollbar", 5, 5, 600, 400, is_debug=True)
 frame = BlockService.create_frame("test_scrollbar")
 listbox_list = tuple([str(x) for x in range(0, 100)] + ["aabfsdgadfsgasdfkj;adsfadsj;kjfeijof"])
-_, listbox_var = tk.Listbox(frame, 1, 2, 1, 4, str_value=listbox_list)
+_, listbox_var = tk.Listbox(frame, 1, 2, 1, 4, init_value=listbox_list)
 listbox.scrollbar = BlockService.scrollbar(frame, x_enable=True, y_enable=True, size=30)
 BlockService.place_frame_widget()
 root.mainloop()
 ```
 
 The basic usage of the scrollbar is the same. If you want the scrollbar to be placed automatically, you can place it by linking the scrollbar to the widget.  
 If you wish to manually place it anywhere you wish, simply specify the layout as you would for a normal widget.
```

### Comparing `tkblock-2.0.0/setup.py` & `tkblock-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 # README.mdをlong_discriptionにするために読み込む
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 setup(
     name=package_name,
-    version="2.0.0",
+    version="2.1.0",
     description="tkinter block framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kuri-pome/tkblock",
     author="kuri_pome",
     license="MIT",
     keywords="tkinter place widget easy",
```

### Comparing `tkblock-2.0.0/tkblock/__init__.py` & `tkblock-2.1.0/tkblock/__init__.py`

 * *Files identical despite different names*

### Comparing `tkblock-2.0.0/tkblock/block_framebase.py` & `tkblock-2.1.0/tkblock/block_framebase.py`

 * *Files identical despite different names*

### Comparing `tkblock-2.0.0/tkblock/block_framework.py` & `tkblock-2.1.0/tkblock/block_framework.py`

 * *Files identical despite different names*

### Comparing `tkblock-2.0.0/tkblock/block_service.py` & `tkblock-2.1.0/tkblock/block_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -315,15 +315,15 @@
         row_start,
         row_end,
         *args,
         pad_left=0.0,
         pad_right=0.0,
         pad_up=0.0,
         pad_down=0.0,
-        str_value="",
+        init_value="",
         **kwargs,
     ):
         """BlockEntryを作成する
 
         textvariableというオプション引数にtk.StringVarをセットすることも可能。
 
         例
@@ -336,24 +336,24 @@
             col_end (int): 列の終了位置
             row_start (int): 行の開始位置
             row_end (int): 行の終了位置
             pad_left (float, optional): 横幅の左側の隙間(0~1). Defaults to 0.0.
             pad_right (float, optional): 横幅の右側の隙間(0~1). Defaults to 0.0.
             pad_up (float, optional): 立幅の上側の隙間(0~1). Defaults to 0.0.
             pad_down (float, optional): 立幅の下側の隙間(0~1). Defaults to 0.0.
-            str_value (str, optional): 初期値. Defaults to "".
+            init_value (str, optional): 初期値. Defaults to "".
 
         Returns:
             BlockEntry: BlockEntry
             tk.StringVar: string_var
         """
         if "textvariable" in kwargs:
             string_var = kwargs["textvariable"]
         else:
-            string_var = tk.StringVar(value=str_value)
+            string_var = tk.StringVar(value=init_value)
             kwargs["textvariable"] = string_var
         entry = BlockEntry(frame, *args, **kwargs)
         entry.layout = cls.layout(
             col_start,
             col_end,
             row_start,
             row_end,
@@ -378,16 +378,25 @@
         pad_up=0.0,
         pad_down=0.0,
         **kwargs,
     ):
         """BlockTextを作成する
 
         例
-        text1 = BlockService.create_text(self.frame, 30, 40, 15, 20, name="text1")
+        def echo_text(_):
+            print(text1.get("1.0", "end - 1c"))
+
+        text1 = BlockService.create_text(
+            self.frame, 30, 40, 15, 20, name="text1", wrap="none"
+        )
+        text1.scrollbar = BlockService.scrollbar(
+            self.frame, x_enable=True, y_enable=True
+        )
         text1.insert(tk.END, "hoge\nfuga")
+        BlockService.create_button(self.frame, 30, 40, 20, 21, function=echo_text)
 
         Args:
             frame (Any): 親フレーム
             col_start (int): 列の開始位置
             col_end (int): 列の終了位置
             row_start (int): 行の開始位置
             row_end (int): 行の終了位置
@@ -421,45 +430,45 @@
         row_start,
         row_end,
         *args,
         pad_left=0.0,
         pad_right=0.0,
         pad_up=0.0,
         pad_down=0.0,
-        str_value="",
+        init_value="",
         **kwargs,
     ):
         """BlockListboxを作成する
 
         listvariableというオプション引数にtk.StringVarをセットすることも可能。
 
         例
-        listbox, _ = BlockService.create_listbox(self.frame, 0, 5, 3, 10, str_value=("tkinter", "os", "datetime", "math"), name="listbox")
+        listbox, _ = BlockService.create_listbox(self.frame, 0, 5, 3, 10, init_value=("tkinter", "os", "datetime", "math"), name="listbox")
         listbox.insert(2, "hogehoge")
 
         Args:
             frame (Any): 親フレーム
             col_start (int): 列の開始位置
             col_end (int): 列の終了位置
             row_start (int): 行の開始位置
             row_end (int): 行の終了位置
             pad_left (float, optional): 横幅の左側の隙間(0~1). Defaults to 0.0.
             pad_right (float, optional): 横幅の右側の隙間(0~1). Defaults to 0.0.
             pad_up (float, optional): 立幅の上側の隙間(0~1). Defaults to 0.0.
             pad_down (float, optional): 立幅の下側の隙間(0~1). Defaults to 0.0.
-            str_value (str, optional): 初期値. Defaults to "".
+            init_value (str, optional): 初期値. Defaults to "".
 
         Returns:
             BlockListbox: BlockListbox
             tk.StringVar: string_var
         """
         if "listvariable" in kwargs:
             string_var = kwargs["listvariable"]
         else:
-            string_var = tk.StringVar(value=str_value)
+            string_var = tk.StringVar(value=init_value)
             kwargs["listvariable"] = string_var
         listbox = BlockListbox(frame, *args, **kwargs)
         listbox.layout = cls.layout(
             col_start,
             col_end,
             row_start,
             row_end,
@@ -480,83 +489,104 @@
         row_start,
         row_end,
         *args,
         pad_left=0.0,
         pad_right=0.0,
         pad_up=0.0,
         pad_down=0.0,
-        int_value=0,
+        init_value=False,
         **kwargs,
     ):
         """BlockCheckbuttonを作成する
 
         textvariableというオプション引数にtk.IntVarをセットすることも可能。
 
         例
-        def echo_checkbutton():
-            print(checkbutton_var.get())
-
-        _, checkbutton_var = BlockService.create_checkbutton(
-            self.frame, 14, 20, 0, 2, name="checkbutton", text="checkbutton", int_value=0, command=echo_checkbutton)
+        def echo_checkbutton(_):
+            print(checkbutton1_var.get())
+            print(checkbutton2_var.get())
+
+        _, checkbutton1_var = BlockService.create_checkbutton(
+            self.frame,
+            14,
+            20,
+            0,
+            1,
+            name="checkbutton1",
+            text="checkbutton1",
+            init_value=True,
+        )
+        _, checkbutton2_var = BlockService.create_checkbutton(
+            self.frame,
+            14,
+            20,
+            1,
+            2,
+            name="checkbutton2",
+            text="checkbutton2",
+            init_value=False,
+        )
+        BlockService.create_button(self.frame, 14, 20, 2, 3, function=echo_checkbutton)
 
         Args:
             frame (Any): 親フレーム
             col_start (int): 列の開始位置
             col_end (int): 列の終了位置
             row_start (int): 行の開始位置
             row_end (int): 行の終了位置
             pad_left (float, optional): 横幅の左側の隙間(0~1). Defaults to 0.0.
             pad_right (float, optional): 横幅の右側の隙間(0~1). Defaults to 0.0.
             pad_up (float, optional): 立幅の上側の隙間(0~1). Defaults to 0.0.
             pad_down (float, optional): 立幅の下側の隙間(0~1). Defaults to 0.0.
+            init_value (bool, optional): チェックなし. Defaults to False.
 
         Returns:
             BlockCheckbutton: BlockCheckbutton
-            tk.IntVar: int_var
+            tk.BooleanVar: bool_var
         """
-        if "textvariable" in kwargs:
-            int_var = kwargs["textvariable"]
+        if "variable" in kwargs:
+            bool_var = kwargs["variable"]
         else:
-            int_var = tk.IntVar(value=int_value)
-            kwargs["textvariable"] = int_var
+            bool_var = tk.BooleanVar(value=init_value)
+            kwargs["variable"] = bool_var
         checkbutton = BlockCheckbutton(frame, *args, **kwargs)
         checkbutton.layout = cls.layout(
             col_start,
             col_end,
             row_start,
             row_end,
             pad_left=pad_left,
             pad_right=pad_right,
             pad_up=pad_up,
             pad_down=pad_down,
         )
-        return checkbutton, int_var
+        return checkbutton, bool_var
 
     @classmethod
     def create_radiobutton(
         cls,
         frame,
         col_start,
         col_end,
         row_start,
         row_end,
         *args,
         pad_left=0.0,
         pad_right=0.0,
         pad_up=0.0,
         pad_down=0.0,
-        int_value=0,
+        init_value=0,
         **kwargs,
     ):
         """BlockRadiobuttonを作成する
 
         textvariableというオプション引数にtk.IntVarをセットすることも可能。
 
         例
-        _, radiobutton_var = BlockService.create_radiobutton(self.frame, 6, 15, 5, 7, int_value=0, name="radiobutton1_1", text="radiobutton1_1", value=10)
+        _, radiobutton_var = BlockService.create_radiobutton(self.frame, 6, 15, 5, 7, init_value=0, name="radiobutton1_1", text="radiobutton1_1", value=10)
         _, _ = BlockService.create_radiobutton(self.frame, 6, 15, 7, 10, name="radiobutton1_2", text="radiobutton1_2", value=20, variable=radiobutton_var)
         BlockService.create_label(self.frame, 6, 15, 3, 5, name="radiobutton1_label", textvariable=radiobutton_var)
 
         Args:
             frame (Any): 親フレーム
             col_start (int): 列の開始位置
             col_end (int): 列の終了位置
@@ -570,15 +600,15 @@
         Returns:
             BlockRadiobutton: BlockRadiobutton
             tk.IntVar: int_var
         """
         if "variable" in kwargs:
             int_var = kwargs["variable"]
         else:
-            int_var = tk.IntVar(value=int_value)
+            int_var = tk.IntVar(value=init_value)
             kwargs["variable"] = int_var
         radiobutton = BlockRadiobutton(frame, *args, **kwargs)
         radiobutton.layout = cls.layout(
             col_start,
             col_end,
             row_start,
             row_end,
@@ -598,45 +628,45 @@
         row_start,
         row_end,
         *args,
         pad_left=0.0,
         pad_right=0.0,
         pad_up=0.0,
         pad_down=0.0,
-        str_value="",
+        init_value="",
         **kwargs,
     ):
         """BlockScaleを作成する
 
         varというオプション引数にtk.StringVarをセットすることも可能。
 
         例
-        _, scale_var = BlockService.create_scale(self.frame, 16, 20, 5, 10, str_value="", name="scale1")
+        _, scale_var = BlockService.create_scale(self.frame, 16, 20, 5, 10, init_value="", name="scale1")
         BlockService.create_label(self.frame, 16, 20, 3, 5, name="scale_label", textvariable=scale_var)
 
         Args:
             frame (Any): 親フレーム
             col_start (int): 列の開始位置
             col_end (int): 列の終了位置
             row_start (int): 行の開始位置
             row_end (int): 行の終了位置
             pad_left (float, optional): 横幅の左側の隙間(0~1). Defaults to 0.0.
             pad_right (float, optional): 横幅の右側の隙間(0~1). Defaults to 0.0.
             pad_up (float, optional): 立幅の上側の隙間(0~1). Defaults to 0.0.
             pad_down (float, optional): 立幅の下側の隙間(0~1). Defaults to 0.0.
-            str_value (str, optional): 初期値. Defaults to "".
+            init_value (str, optional): 初期値. Defaults to "".
 
         Returns:
             BlockScale: BlockScale
             tk.StringVar: string_var
         """
         if "var" in kwargs:
             string_var = kwargs["var"]
         else:
-            string_var = tk.StringVar(value=str_value)
+            string_var = tk.StringVar(value=init_value)
             kwargs["var"] = string_var
         scale = BlockScale(frame, *args, **kwargs)
         scale.layout = cls.layout(
             col_start,
             col_end,
             row_start,
             row_end,
@@ -703,23 +733,23 @@
         row_start,
         row_end,
         *args,
         pad_left=0.0,
         pad_right=0.0,
         pad_up=0.0,
         pad_down=0.0,
-        int_value=0,
+        init_value=0,
         **kwargs,
     ):
         """BlockSpinboxを作成する
 
         textvariableというオプション引数にtk.IntVarをセットすることも可能。
 
         例
-        _, spinbox1_var = BlockService.create_spinbox(self.frame, 16, 25, 21, 23, int_value=0, from_=-10, to=10, increment=1)
+        _, spinbox1_var = BlockService.create_spinbox(self.frame, 16, 25, 21, 23, init_value=0, from_=-10, to=10, increment=1)
         _ = BlockService.create_label(self.frame, 16, 25, 23, 25, textvariable=spinbox1_var)
 
         Args:
             frame (Any): 親フレーム
             col_start (int): 列の開始位置
             col_end (int): 列の終了位置
             row_start (int): 行の開始位置
@@ -732,15 +762,15 @@
         Returns:
             BlockSpinbox: BlockSpinbox
             tk.IntVar: int_var
         """
         if "textvariable" in kwargs:
             int_var = kwargs["textvariable"]
         else:
-            int_var = tk.IntVar(value=int_value)
+            int_var = tk.IntVar(value=init_value)
             kwargs["textvariable"] = int_var
         spinbox = BlockSpinbox(frame, *args, **kwargs)
         spinbox.layout = cls.layout(
             col_start,
             col_end,
             row_start,
             row_end,
@@ -754,15 +784,15 @@
     @classmethod
     def create_scrollbar(cls, frame, *args, layout=None, **kwargs):
         """BlockScrollbarを作成する（非推奨）
 
         BlockService.scrollbarの戻り地をwidget.scrollbarに指定することで自動で作成されるので、そちらを推奨
 
         例
-        scrollbar1_listbox, _ = BlockService.create_listbox(self.frame, 30, 40, 0, 10, str_value=tuple([str(x) for x in range(0, 100)]), name="scrollbar1_listbox")
+        scrollbar1_listbox, _ = BlockService.create_listbox(self.frame, 30, 40, 0, 10, init_value=tuple([str(x) for x in range(0, 100)]), name="scrollbar1_listbox")
         layout = BlockService.layout(40, 41, 0, 10)
         scrollbar1 = BlockService.create_scrollbar(self.frame, layout=layout, orient=tk.VERTICAL)
         scrollbar1.config(command=scrollbar1_listbox.yview)
         scrollbar1_listbox.config(yscrollcommand=scrollbar1.set)
 
         Args:
             frame (Any): 親フレーム
@@ -846,15 +876,15 @@
         row_start,
         row_end,
         *args,
         pad_left=0.0,
         pad_right=0.0,
         pad_up=0.0,
         pad_down=0.0,
-        str_value="",
+        init_value="",
         function=None,
         **kwargs,
     ):
         """BlockComboboxを作成する
 
         textvariableというオプション引数にtk.StringVarをセットすることも可能。
 
@@ -867,25 +897,25 @@
             col_end (int): 列の終了位置
             row_start (int): 行の開始位置
             row_end (int): 行の終了位置
             pad_left (float, optional): 横幅の左側の隙間(0~1). Defaults to 0.0.
             pad_right (float, optional): 横幅の右側の隙間(0~1). Defaults to 0.0.
             pad_up (float, optional): 立幅の上側の隙間(0~1). Defaults to 0.0.
             pad_down (float, optional): 立幅の下側の隙間(0~1). Defaults to 0.0.
-            str_value (str, optional): 初期値. Defaults to "".
+            init_value (str, optional): 初期値. Defaults to "".
             function (None, function): 押下のbindする関数. Defaults to None.
 
         Returns:
             BlockCombobox: BlockCombobox
             tk.StringVar: string_var
         """
         if "textvariable" in kwargs:
             string_var = kwargs["textvariable"]
         else:
-            string_var = tk.StringVar(value=str_value)
+            string_var = tk.StringVar(value=init_value)
             kwargs["textvariable"] = string_var
         combobox = BlockCombobox(frame, *args, **kwargs)
         combobox.layout = cls.layout(
             col_start,
             col_end,
             row_start,
             row_end,
```

### Comparing `tkblock-2.0.0/tkblock/canvas.py` & `tkblock-2.1.0/tkblock/canvas.py`

 * *Files identical despite different names*

### Comparing `tkblock-2.0.0/tkblock.egg-info/PKG-INFO` & `tkblock-2.1.0/tkblock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkblock
-Version: 2.0.0
+Version: 2.1.0
 Summary: tkinter block framework
 Home-page: https://github.com/kuri-pome/tkblock
 Author: kuri_pome
 License: MIT
 Keywords: tkinter place widget easy
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
@@ -298,15 +298,15 @@
 In the above figure, 30px vertical and horizontal scrollbars are placed.
 The code for this is shown below.
 
 ```python
 root = BlockService.init("test_scrollbar", 5, 5, 600, 400, is_debug=True)
 frame = BlockService.create_frame("test_scrollbar")
 listbox_list = tuple([str(x) for x in range(0, 100)] + ["aabfsdgadfsgasdfkj;adsfadsj;kjfeijof"])
-_, listbox_var = tk.Listbox(frame, 1, 2, 1, 4, str_value=listbox_list)
+_, listbox_var = tk.Listbox(frame, 1, 2, 1, 4, init_value=listbox_list)
 listbox.scrollbar = BlockService.scrollbar(frame, x_enable=True, y_enable=True, size=30)
 BlockService.place_frame_widget()
 root.mainloop()
 ```
 
 The basic usage of the scrollbar is the same. If you want the scrollbar to be placed automatically, you can place it by linking the scrollbar to the widget.  
 If you wish to manually place it anywhere you wish, simply specify the layout as you would for a normal widget.
```

