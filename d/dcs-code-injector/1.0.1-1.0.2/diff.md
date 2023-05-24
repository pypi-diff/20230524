# Comparing `tmp/dcs-code-injector-1.0.1.tar.gz` & `tmp/dcs-code-injector-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcs-code-injector-1.0.1.tar", last modified: Wed May 24 07:50:48 2023, max compression
+gzip compressed data, was "dcs-code-injector-1.0.2.tar", last modified: Wed May 24 11:02:27 2023, max compression
```

## Comparing `dcs-code-injector-1.0.1.tar` & `dcs-code-injector-1.0.2.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:50:48.825496 dcs-code-injector-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-24 07:50:48.825496 dcs-code-injector-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:50:48.817495 dcs-code-injector-1.0.1/dcs_code_injector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/dcs_code_injector_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/log_highlighter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/lua_syntax_highlighter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/settings_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:50:48.817495 dcs-code-injector-1.0.1/dcs_code_injector/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/dcs_code_injector_settings_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/dcs_code_injector_window_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:50:48.817495 dcs-code-injector-1.0.1/dcs_code_injector/ui/icons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/icons/icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:50:48.821496 dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   629069 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/splash_01.png
--rw-r--r--   0 runner    (1001) docker     (123)   831944 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/splash_02.png
--rw-r--r--   0 runner    (1001) docker     (123)   927761 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/splash_03.png
--rw-r--r--   0 runner    (1001) docker     (123)   932507 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/splash_04.png
--rw-r--r--   0 runner    (1001) docker     (123)   723796 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/splash_05.png
--rw-r--r--   0 runner    (1001) docker     (123)   916284 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/splash_06.png
--rw-r--r--   0 runner    (1001) docker     (123)   968922 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/splash_07.png
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/variables_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:50:48.817495 dcs-code-injector-1.0.1/dcs_code_injector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-24 07:50:48.000000 dcs-code-injector-1.0.1/dcs_code_injector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-24 07:50:48.000000 dcs-code-injector-1.0.1/dcs_code_injector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:50:48.000000 dcs-code-injector-1.0.1/dcs_code_injector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-24 07:50:48.000000 dcs-code-injector-1.0.1/dcs_code_injector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-24 07:50:48.000000 dcs-code-injector-1.0.1/dcs_code_injector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 07:50:48.000000 dcs-code-injector-1.0.1/dcs_code_injector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 07:50:48.825496 dcs-code-injector-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:02:27.866660 dcs-code-injector-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-24 11:02:27.866660 dcs-code-injector-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:02:27.850660 dcs-code-injector-1.0.2/dcs_code_injector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15413 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/dcs_code_injector_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/log_highlighter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/lua_syntax_highlighter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/settings_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:02:27.854660 dcs-code-injector-1.0.2/dcs_code_injector/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/dcs_code_injector_settings_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/dcs_code_injector_window_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:02:27.858660 dcs-code-injector-1.0.2/dcs_code_injector/ui/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/icons/cloud_done.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/icons/cloud_off.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/icons/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:02:27.862660 dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   629069 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_01.png
+-rw-r--r--   0 runner    (1001) docker     (123)   831944 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_02.png
+-rw-r--r--   0 runner    (1001) docker     (123)   927761 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_03.png
+-rw-r--r--   0 runner    (1001) docker     (123)   932507 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_04.png
+-rw-r--r--   0 runner    (1001) docker     (123)   723796 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_05.png
+-rw-r--r--   0 runner    (1001) docker     (123)   916284 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_06.png
+-rw-r--r--   0 runner    (1001) docker     (123)   968922 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_07.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/variables_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:02:27.854660 dcs-code-injector-1.0.2/dcs_code_injector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-24 11:02:27.000000 dcs-code-injector-1.0.2/dcs_code_injector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-24 11:02:27.000000 dcs-code-injector-1.0.2/dcs_code_injector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 11:02:27.000000 dcs-code-injector-1.0.2/dcs_code_injector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-24 11:02:27.000000 dcs-code-injector-1.0.2/dcs_code_injector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-24 11:02:27.000000 dcs-code-injector-1.0.2/dcs_code_injector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 11:02:27.000000 dcs-code-injector-1.0.2/dcs_code_injector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 11:02:27.866660 dcs-code-injector-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/setup.py
```

### Comparing `dcs-code-injector-1.0.1/LICENSE` & `dcs-code-injector-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.1/dcs_code_injector/dcs_code_injector_window.py` & `dcs-code-injector-1.0.2/dcs_code_injector/dcs_code_injector_window.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from PySide6.QtGui import *
 from PySide6.QtCore import *
 import os
 import json
 from functools import partial
 from ez_settings import EZSettings
 from datetime import datetime, timedelta
-import ez_icons
-from ez_icons import i, c
+# import ez_icons
+# from ez_icons import i, c
 
 from .settings_dialog import SettingsDialog
 
 from .server import Server
 from .lua_syntax_highlighter import SimpleLuaHighlighter
 from .log_highlighter import LogHighlighter
 # from .variables_tree import VariablesTree
@@ -40,34 +40,28 @@
         self.last_log_file_size = 0
 
         self.log_file = EZSettings().get("log_file", "")
         self.previous = []
         LogHighlighter(self.txt_log.document())
         self.read_log()
 
-        if self.tab_widget.count() == 0:
-            EZSettings().set("Code", "log.write(\"DCS Code Injector\", log.INFO, \"Hello, DCS!\")\n")
-
-        self.tab_widget.addTab(QWidget(), "+")
-        self.tab_widget.tabBar().setTabButton(1, QTabBar.RightSide, None)
+        self.load()
 
         self.log_font_size = 10
         self.update_log_font_size()
 
-        self.load()
+        self.server = Server()
+        self.server_thread = QThread()
+        self.server.moveToThread(self.server_thread)
 
         self.timer = QTimer()
         self.timer.setInterval(500)
         self.timer.timeout.connect(self.read_log)
         self.timer.start()
 
-        self.server = Server()
-        self.server_thread = QThread()
-        self.server.moveToThread(self.server_thread)
-
         self.connect_signals()
 
         QCoreApplication.instance().aboutToQuit.connect(self.stop_server)
 
         self.connection_label = QLabel()
         self.statusbar.addWidget(self.connection_label)
         self.on_disconnected()
@@ -106,20 +100,18 @@
                     new_lines = lines[-diff:]
                     new_text = "".join(new_lines)
                 self.add_text_to_log(new_text)
             self.previous = lines
         self.last_log_file_size = file_size
 
     def connect_signals(self):
-        self.tab_widget.currentChanged.connect(self.add_new_tab)
         self.tab_widget.tabBarDoubleClicked.connect(self.rename_tab)
         self.tab_widget.tabCloseRequested.connect(self.close_tab)
         self.action_settings.triggered.connect(self.show_settings)
         self.action_clear_log.triggered.connect(self.clear_log)
-        self.action_clear_execution_file.triggered.connect(self.clear_execution_file)
         self.favorites_widget.new_button_added.connect(self.connect_favorite_button)
 
         self.server_thread.started.connect(self.server.start)
         self.server.connected.connect(self.on_connected)
         self.server.received.connect(self.on_received)
         self.server.disconnected.connect(self.on_disconnected)
         self.server_thread.start()
@@ -130,21 +122,21 @@
             if data.get("connection", "") == "not_active":
                 print("connection closed!")
 
         except json.decoder.JSONDecodeError as err:
             print(err)
 
     def on_connected(self):
-        pixmap = QPixmap(ez_icons.get(c.white, i.cloud_done))
+        pixmap = QPixmap(os.path.join(os.path.dirname(__file__), "ui", "icons", "cloud_done.png"))
         pixmap = pixmap.scaledToWidth(20, Qt.SmoothTransformation)
         self.connection_label.setPixmap(pixmap)
         self.statusbar.showMessage("Connected to DCS", 2500)
 
     def on_disconnected(self):
-        pixmap = QPixmap(ez_icons.get(c.white, i.cloud_off))
+        pixmap = QPixmap(os.path.join(os.path.dirname(__file__), "ui", "icons", "cloud_off.png"))
         pixmap = pixmap.scaledToWidth(20, Qt.SmoothTransformation)
         self.connection_label.setPixmap(pixmap)
         self.statusbar.showMessage("Disconnected from DCS", 2500)
 
     def stop_server(self):
         print("killing server")
         self.server.exit = True
@@ -153,51 +145,43 @@
 
     def clear_log(self):
         self.add_text_to_log("\n" * 60)
 
     def update_log_font_size(self):
         self.txt_log.setStyleSheet(f"font: {self.log_font_size}pt 'Courier New';")
 
-    def clear_execution_file(self):
-        self.write_dcs_file("--", add_to_log=False)
-
     def connect_favorite_button(self, favorite_button):
-        favorite_button.clicked.connect(partial(self.write_dcs_file, favorite_button.code))
-        favorite_button.open_tab_with_code.connect(partial(self.add_new_tab, 0, True))
+        favorite_button.clicked.connect(partial(self.set_server_response, favorite_button.code))
+        favorite_button.open_tab_with_code.connect(partial(self.add_new_tab))
 
     def close_tab(self, tab_index):
         answer = QMessageBox.question(self, 'Close', "Are you sure you want to remove this tab?", QMessageBox.Yes, QMessageBox.No)
         if answer == QMessageBox.Yes:
             setting_name = self.tab_widget.tabText(tab_index)
             if tab_index > 0:
                 new_index = tab_index - 1
             else:
                 new_index = 0
 
             self.tab_widget.setCurrentIndex(new_index)
             self.tab_widget.removeTab(tab_index)
             EZSettings().remove(setting_name)
 
-    def add_new_tab(self, index=None, force=False, name=None, code=None):
-        self.tab_widget.blockSignals(True)
-
-        if self.tab_widget.currentIndex() == self.tab_widget.count() - 1 or force:
-            code_text_edit = CodeTextEdit()
-            code_text_edit.textChanged.connect(self.save_code)
-            self.tab_widget.insertTab(index or self.tab_widget.count() - 1, code_text_edit, "UNNAMED")
-
-            self.tab_widget.setCurrentIndex(self.tab_widget.count() - 2)
-            if name is not None:
-                self.tab_widget.setTabText(self.tab_widget.currentIndex(), name)
-            if code is not None:
-                self.tab_widget.currentWidget().setPlainText(code)
-            else:
-                self.tab_widget.currentWidget().setPlainText("log.write(\"DCS Code Injector\", log.INFO, \"Hello, DCS!\")\n")
-
-        self.tab_widget.blockSignals(False)
+    def add_new_tab(self, name=None, code=None):
+        code_text_edit = CodeTextEdit()
+        code_text_edit.textChanged.connect(self.save_code)
+        self.tab_widget.insertTab(self.tab_widget.count() - 1, code_text_edit, "UNNAMED")
+
+        self.tab_widget.setCurrentIndex(self.tab_widget.count() - 2)
+        if name is not None:
+            self.tab_widget.setTabText(self.tab_widget.currentIndex(), name)
+        if code is not None:
+            self.tab_widget.currentWidget().setPlainText(code)
+        else:
+            self.tab_widget.currentWidget().setPlainText("log.write(\"DCS Code Injector\", log.INFO, \"Hello, DCS!\")\n")
 
     def rename_tab(self):
         name, accepted = QInputDialog().getText(self, "DCS Code Injector", "Enter a name for this tab: ", QLineEdit.Normal, "")
         if not accepted:
             return
 
         for index in range(self.tab_widget.count()):
@@ -206,39 +190,30 @@
                 name = name + "_01"
 
         self.tab_widget.setTabText(self.tab_widget.currentIndex(), name)
         self.save_code()
 
     def load(self):
         for setting in EZSettings().get_all_settings():
-            if setting != "dcs_file" and setting != "log_file" and setting != "shift_hours" and not setting.startswith("btn_"):
-                self.add_new_tab(0, force=True, name=setting, code=EZSettings().get(setting))
+            if setting != "log_file" and setting != "shift_hours" and not setting.startswith("btn_"):
+                self.add_new_tab(name=setting, code=EZSettings().get(setting))
             if setting.startswith("btn_"):
                 self.favorites_widget.add_new_button(setting.replace("btn_", ""), EZSettings().get(setting))
-        self.setWindowTitle(f"DCS Code Injector - {EZSettings().get('dcs_file', '')}")
 
     def save_code(self):
         tab_name = self.tab_widget.tabText(self.tab_widget.currentIndex())
         code = self.tab_widget.currentWidget().toPlainText()
         if code != "" and not tab_name == "UNNAMED":
             EZSettings().set(tab_name, code)
 
     def show_settings(self):
         dlg = SettingsDialog()
         dlg.exec_()
         self.setWindowTitle(f"DCS Code Injector - {dlg.txt_log_file.text()}")
 
-    def write_dcs_file(self, text, add_to_log=True):
-        if text != "":
-            file = EZSettings().get("dcs_file")
-            with open(file, "w") as writefile:
-                writefile.write(text)
-        if add_to_log:
-            self.add_code_to_log(text)
-
     def add_code_to_log(self, text):
         line_number = 1
         numbered_lines = []
         numbered_lines.append("\n------------------- CODE BLOCK -------------------")
         for line in text.split("\n"):
             line = f"{str(line_number).zfill(2)}          {line}"
             numbered_lines.append(line)
@@ -248,23 +223,29 @@
         self.add_text_to_log(complete_text)
 
     def add_text_to_log(self, complete_text):
         self.txt_log.moveCursor(QTextCursor.End)
         self.txt_log.insertPlainText(complete_text)
         self.txt_log.verticalScrollBar().setValue(self.txt_log.verticalScrollBar().maximum())
 
+    def set_server_response(self, code):
+        self.add_code_to_log(code)
+        self.server.response = code
+
     def keyPressEvent(self, event: QKeyEvent) -> None:
         if event.key() == Qt.Key_Enter or event.key() == Qt.Key_Return and event.modifiers() == Qt.ControlModifier:
             text = self.tab_widget.currentWidget().textCursor().selection().toPlainText()
-            self.server.response = text
-            self.write_dcs_file(text)
+            self.set_server_response(text)
 
         if event.key() == Qt.Key_F5:
             self.read_log()
 
+        if event.key() == Qt.Key_N and event.modifiers() == Qt.ControlModifier:
+            self.add_new_tab(name="UNNAMED", code="-- add code here")
+
         if event.key() == Qt.Key_Up and event.modifiers() == Qt.ControlModifier:
             self.tab_widget.currentWidget().font_size += 1
             self.tab_widget.currentWidget().update_document_size()
             self.log_font_size = self.tab_widget.currentWidget().font_size
             self.update_log_font_size()
         if event.key() == Qt.Key_Down and event.modifiers() == Qt.ControlModifier:
             self.tab_widget.currentWidget().font_size -= 1
```

### Comparing `dcs-code-injector-1.0.1/dcs_code_injector/log_highlighter.py` & `dcs-code-injector-1.0.2/dcs_code_injector/log_highlighter.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.1/dcs_code_injector/lua_syntax_highlighter.py` & `dcs-code-injector-1.0.2/dcs_code_injector/lua_syntax_highlighter.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.1/dcs_code_injector/server.py` & `dcs-code-injector-1.0.2/dcs_code_injector/server.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.1/dcs_code_injector/settings_dialog.py` & `dcs-code-injector-1.0.2/dcs_code_injector/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.1/dcs_code_injector/ui/dcs_code_injector_settings_ui.py` & `dcs-code-injector-1.0.2/dcs_code_injector/ui/dcs_code_injector_settings_ui.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.1/dcs_code_injector/ui/dcs_code_injector_window_ui.py` & `dcs-code-injector-1.0.2/dcs_code_injector/ui/dcs_code_injector_window_ui.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.1/dcs_code_injector/ui/icons/icon.png` & `dcs-code-injector-1.0.2/dcs_code_injector/ui/icons/icon.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/splash_01.png` & `dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_01.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/splash_02.png` & `dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_02.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/splash_03.png` & `dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_03.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/splash_04.png` & `dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_04.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/splash_05.png` & `dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_05.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/splash_06.png` & `dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_06.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/splash_07.png` & `dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_07.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.1/dcs_code_injector/variables_tree.py` & `dcs-code-injector-1.0.2/dcs_code_injector/variables_tree.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.1/dcs_code_injector.egg-info/SOURCES.txt` & `dcs-code-injector-1.0.2/dcs_code_injector.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 dcs_code_injector.egg-info/entry_points.txt
 dcs_code_injector.egg-info/requires.txt
 dcs_code_injector.egg-info/top_level.txt
 dcs_code_injector/ui/__init__.py
 dcs_code_injector/ui/dcs_code_injector_settings_ui.py
 dcs_code_injector/ui/dcs_code_injector_window_ui.py
 dcs_code_injector/ui/icons/__init__.py
+dcs_code_injector/ui/icons/cloud_done.png
+dcs_code_injector/ui/icons/cloud_off.png
 dcs_code_injector/ui/icons/icon.png
 dcs_code_injector/ui/splashscreens/__init__.py
 dcs_code_injector/ui/splashscreens/splash_01.png
 dcs_code_injector/ui/splashscreens/splash_02.png
 dcs_code_injector/ui/splashscreens/splash_03.png
 dcs_code_injector/ui/splashscreens/splash_04.png
 dcs_code_injector/ui/splashscreens/splash_05.png
```

### Comparing `dcs-code-injector-1.0.1/setup.py` & `dcs-code-injector-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-data_files_to_include = ["*.png", "*.jpg"]
+data_files_to_include = ["*.png", "*.jpg", "*.xml"]
 
 setup(
     name='dcs-code-injector',
-    version='1.0.1',
+    version='1.0.2',
     packages=find_packages(),
     package_data={
         "": data_files_to_include,
     },
     url='https://www.github.com/nielsvaes/dcs_code_injector',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

