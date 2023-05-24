# Comparing `tmp/rogue_tools-1.0.8.tar.gz` & `tmp/rogue_tools-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rogue_tools-1.0.8.tar", last modified: Sun Apr 23 02:18:05 2023, max compression
+gzip compressed data, was "rogue_tools-1.0.9.tar", last modified: Wed May 24 09:28:00 2023, max compression
```

## Comparing `rogue_tools-1.0.8.tar` & `rogue_tools-1.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 02:18:05.889085 rogue_tools-1.0.8/
--rw-rw-rw-   0        0        0      517 2023-04-23 02:18:05.889085 rogue_tools-1.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-23 02:18:05.876226 rogue_tools-1.0.8/rogue_tools/
--rw-rw-rw-   0        0        0        0 2023-03-03 12:10:10.000000 rogue_tools-1.0.8/rogue_tools/__init__.py
--rw-rw-rw-   0        0        0     6206 2023-04-12 11:49:44.000000 rogue_tools-1.0.8/rogue_tools/android_tool.py
--rw-rw-rw-   0        0        0     6255 2023-04-12 11:49:44.000000 rogue_tools-1.0.8/rogue_tools/excel_tool.py
--rw-rw-rw-   0        0        0     4056 2023-04-12 11:49:44.000000 rogue_tools-1.0.8/rogue_tools/file_tool.py
--rw-rw-rw-   0        0        0     1157 2023-04-12 11:49:44.000000 rogue_tools-1.0.8/rogue_tools/filter_tool.py
--rw-rw-rw-   0        0        0     2353 2023-04-12 11:49:44.000000 rogue_tools-1.0.8/rogue_tools/ini_tool.py
--rw-rw-rw-   0        0        0    13260 2023-04-13 10:09:49.000000 rogue_tools-1.0.8/rogue_tools/path_tool.py
--rw-rw-rw-   0        0        0     2416 2023-04-12 11:49:44.000000 rogue_tools-1.0.8/rogue_tools/robot_tool.py
--rw-rw-rw-   0        0        0     4064 2023-04-12 11:49:45.000000 rogue_tools-1.0.8/rogue_tools/show_tool.py
--rw-rw-rw-   0        0        0      147 2023-04-12 11:49:45.000000 rogue_tools-1.0.8/rogue_tools/string_tool.py
--rw-rw-rw-   0        0        0     1862 2023-04-20 11:22:01.000000 rogue_tools-1.0.8/rogue_tools/time_tool.py
--rw-rw-rw-   0        0        0     2922 2023-04-12 11:49:45.000000 rogue_tools-1.0.8/rogue_tools/ui_tool.py
--rw-rw-rw-   0        0        0     2300 2023-04-23 02:16:48.000000 rogue_tools-1.0.8/rogue_tools/web_tool.py
--rw-rw-rw-   0        0        0    17995 2023-04-12 11:49:45.000000 rogue_tools-1.0.8/rogue_tools/win_tool.py
--rw-rw-rw-   0        0        0     3912 2023-04-20 09:55:42.000000 rogue_tools-1.0.8/rogue_tools/yaml_tool.py
--rw-rw-rw-   0        0        0     1260 2023-04-12 11:49:45.000000 rogue_tools-1.0.8/rogue_tools/zip_tool.py
-drwxrwxrwx   0        0        0        0 2023-04-23 02:18:05.887091 rogue_tools-1.0.8/rogue_tools.egg-info/
--rw-rw-rw-   0        0        0      517 2023-04-23 02:18:05.000000 rogue_tools-1.0.8/rogue_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      614 2023-04-23 02:18:05.000000 rogue_tools-1.0.8/rogue_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 02:18:05.000000 rogue_tools-1.0.8/rogue_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-04-23 02:18:05.000000 rogue_tools-1.0.8/rogue_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-23 02:18:05.000000 rogue_tools-1.0.8/rogue_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-23 02:18:05.000000 rogue_tools-1.0.8/rogue_tools.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-04-23 02:18:05.889085 rogue_tools-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1777 2023-04-23 02:17:59.000000 rogue_tools-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:27:59.999720 rogue_tools-1.0.9/
+-rw-rw-rw-   0        0        0      517 2023-05-24 09:27:59.965507 rogue_tools-1.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-24 09:27:59.953539 rogue_tools-1.0.9/rogue_tools/
+-rw-rw-rw-   0        0        0        0 2023-04-12 11:49:44.000000 rogue_tools-1.0.9/rogue_tools/__init__.py
+-rw-rw-rw-   0        0        0     6206 2023-04-12 11:49:44.000000 rogue_tools-1.0.9/rogue_tools/android_tool.py
+-rw-rw-rw-   0        0        0     6255 2023-04-12 11:49:44.000000 rogue_tools-1.0.9/rogue_tools/excel_tool.py
+-rw-rw-rw-   0        0        0     4056 2023-04-12 11:49:44.000000 rogue_tools-1.0.9/rogue_tools/file_tool.py
+-rw-rw-rw-   0        0        0     1157 2023-04-12 11:49:44.000000 rogue_tools-1.0.9/rogue_tools/filter_tool.py
+-rw-rw-rw-   0        0        0     2353 2023-04-12 11:49:44.000000 rogue_tools-1.0.9/rogue_tools/ini_tool.py
+-rw-rw-rw-   0        0        0    13260 2023-04-13 10:09:49.000000 rogue_tools-1.0.9/rogue_tools/path_tool.py
+-rw-rw-rw-   0        0        0     3380 2023-05-24 09:26:33.000000 rogue_tools-1.0.9/rogue_tools/robot_tool.py
+-rw-rw-rw-   0        0        0     4064 2023-04-12 11:49:45.000000 rogue_tools-1.0.9/rogue_tools/show_tool.py
+-rw-rw-rw-   0        0        0      147 2023-04-12 11:49:45.000000 rogue_tools-1.0.9/rogue_tools/string_tool.py
+-rw-rw-rw-   0        0        0     1862 2023-04-20 11:22:01.000000 rogue_tools-1.0.9/rogue_tools/time_tool.py
+-rw-rw-rw-   0        0        0     3817 2023-05-18 09:43:37.000000 rogue_tools-1.0.9/rogue_tools/ui_tool.py
+-rw-rw-rw-   0        0        0     2300 2023-04-23 02:16:48.000000 rogue_tools-1.0.9/rogue_tools/web_tool.py
+-rw-rw-rw-   0        0        0    17995 2023-04-12 11:49:45.000000 rogue_tools-1.0.9/rogue_tools/win_tool.py
+-rw-rw-rw-   0        0        0     3401 2023-05-15 13:12:33.000000 rogue_tools-1.0.9/rogue_tools/yaml_tool.py
+-rw-rw-rw-   0        0        0     1260 2023-04-12 11:49:45.000000 rogue_tools-1.0.9/rogue_tools/zip_tool.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:27:59.964510 rogue_tools-1.0.9/rogue_tools.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-05-24 09:27:59.000000 rogue_tools-1.0.9/rogue_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      614 2023-05-24 09:27:59.000000 rogue_tools-1.0.9/rogue_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 09:27:59.000000 rogue_tools-1.0.9/rogue_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-05-24 09:27:59.000000 rogue_tools-1.0.9/rogue_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-24 09:27:59.000000 rogue_tools-1.0.9/rogue_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-24 09:27:59.000000 rogue_tools-1.0.9/rogue_tools.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-05-24 09:28:00.000331 rogue_tools-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1777 2023-05-24 09:27:03.000000 rogue_tools-1.0.9/setup.py
```

### Comparing `rogue_tools-1.0.8/PKG-INFO` & `rogue_tools-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rogue_tools
-Version: 1.0.8
+Version: 1.0.9
 Summary: private tools
 Home-page: 
 Author: luohao
 Author-email: luohao@aobi.com
 License: MIT
 Classifier: Operating System :: Microsoft
 Classifier: Intended Audience :: Developers
```

### Comparing `rogue_tools-1.0.8/rogue_tools/android_tool.py` & `rogue_tools-1.0.9/rogue_tools/android_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.8/rogue_tools/excel_tool.py` & `rogue_tools-1.0.9/rogue_tools/excel_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.8/rogue_tools/file_tool.py` & `rogue_tools-1.0.9/rogue_tools/file_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.8/rogue_tools/filter_tool.py` & `rogue_tools-1.0.9/rogue_tools/filter_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.8/rogue_tools/ini_tool.py` & `rogue_tools-1.0.9/rogue_tools/ini_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.8/rogue_tools/path_tool.py` & `rogue_tools-1.0.9/rogue_tools/path_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.8/rogue_tools/show_tool.py` & `rogue_tools-1.0.9/rogue_tools/show_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.8/rogue_tools/time_tool.py` & `rogue_tools-1.0.9/rogue_tools/time_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.8/rogue_tools/ui_tool.py` & `rogue_tools-1.0.9/rogue_tools/ui_tool.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 import sys
 import time
 import traceback
 
 from PyQt5 import QtCore
 from PyQt5.QtWidgets import *
 from concurrent.futures import ThreadPoolExecutor
-
+from rogue_tools import file_tool,path_tool
 
 
 
 class mainUI():
     def __init__(self,w,h,title='PyQt5 - UI by [rogue_tools]',is_center=True):
-        
+        self.config_path        = 'save_params.text'
+        self.save_dic           = self.load_input()
         self.ui_width           = w
         self.ui_height          = h
         self.pool               = ThreadPoolExecutor(max_workers=3)
         self.app                = QApplication(sys.argv)
         self.windows            = QWidget()
         self.windows.resize(self.ui_width,self.ui_height)
         self.windows.setWindowTitle(title)
@@ -43,29 +44,49 @@
         btn = QPushButton(title,self.windows)
         btn.setGeometry(start_pos[0] , obj_h * line_index+start_pos[1] , obj_w , obj_h)
         if call_func:
             btn.clicked.connect(call_func)
         return btn
         
     def add_input_editor(self,line_index,title, start_pos = (0,0) ,edit_text='',edit_tips='',obj_w_1=70,obj_w_2=200,obj_h = 20):
+        key = f'{line_index}_{title}'
+        input_str = self.save_dic.get(key,'') if edit_text=='' else edit_text
         # 显示标签
         label = QLabel(self.windows)
         label.setGeometry(QtCore.QRect(start_pos[0] , obj_h * line_index+start_pos[1] , obj_w_1 , obj_h))
         label.setText(title)
         # 输入框
         edit = QLineEdit(self.windows)
         edit.setPlaceholderText(str(edit_tips))
-        edit.setText(str(edit_text))
+        edit.setText(str(input_str))
         edit.setGeometry(QtCore.QRect(obj_w_1+start_pos[0] , obj_h * line_index+start_pos[1] , obj_w_2 , obj_h))
+        # 管理内容
+        self.save_dic[key] = edit
         return edit
     def exit_exe(self):
         QtCore.QCoreApplication.instance().quit()
 
     def msgbox(self,msg_str,title=''):
         QMessageBox.about(self.windows, title,msg_str)
+    def save_input(self):
+        write_lines=[]
+        for key in self.save_dic:
+            write_lines.append(f'{key}={self.save_dic[key].text()}')
+        file_tool.write_lines(self.config_path,write_lines)
+    def load_input(self):
+        rs_dic = {}
+        if not path_tool.is_exists(self.config_path):
+            return rs_dic
+        lines = file_tool.read_simple_text(self.config_path)
+        
+        for line in lines:
+            temp  = line.split('=')
+            if len(temp)==2:
+                rs_dic[temp[0]]=temp[1]
+        return rs_dic
 
 if __name__ == '__main__':
     main_ui = mainUI(400,400)
     main_ui.add_btn((10,10),1,'test1')
     main_ui.add_btn((10,10),2,'test2')
     main_ui.add_input_editor((160,10),1,'测试一下','test1')
     main_ui.add_input_editor((160,10),2,'测试一下','test2')
```

### Comparing `rogue_tools-1.0.8/rogue_tools/web_tool.py` & `rogue_tools-1.0.9/rogue_tools/web_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.8/rogue_tools/win_tool.py` & `rogue_tools-1.0.9/rogue_tools/win_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.8/rogue_tools/zip_tool.py` & `rogue_tools-1.0.9/rogue_tools/zip_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.8/rogue_tools.egg-info/PKG-INFO` & `rogue_tools-1.0.9/rogue_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rogue-tools
-Version: 1.0.8
+Version: 1.0.9
 Summary: private tools
 Home-page: 
 Author: luohao
 Author-email: luohao@aobi.com
 License: MIT
 Classifier: Operating System :: Microsoft
 Classifier: Intended Audience :: Developers
```

### Comparing `rogue_tools-1.0.8/rogue_tools.egg-info/SOURCES.txt` & `rogue_tools-1.0.9/rogue_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.8/setup.py` & `rogue_tools-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,21 @@
     from distutils.core import setup
 import setuptools
 import time
 from rogue_tools import path_tool
 path_tool.del_('build')
 path_tool.del_('dist')
 path_tool.del_('rogue_tools.egg-info')
-time.sleep(1)
+time.sleep(3)
 
 
 setup(
     name='rogue_tools',  # 包的名字
     author='luohao',  # 作者
-    version='1.0.8',  # 版本号
+    version='1.0.9',  # 版本号
     license='MIT',
 
     description='private tools',  # 描述
     long_description='''long description''',
     author_email='luohao@aobi.com',  # 你的邮箱**
     url='',  # 可以写github上的地址，或者其他地址
     # 包内需要引用的文件夹
```

