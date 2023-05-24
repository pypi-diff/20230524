# Comparing `tmp/srsgui-0.3.1.tar.gz` & `tmp/srsgui-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-muaozfbe\srsgui-0.3.1.tar", last modified: Tue May 16 20:21:57 2023, max compression
+gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-7nux2nup\srsgui-0.3.2.tar", last modified: Wed May 24 20:23:50 2023, max compression
```

## Comparing `srsgui-0.3.1.tar` & `srsgui-0.3.2.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.989693 srsgui-0.3.1/
-drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.899459 srsgui-0.3.1/.github/
-drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.910680 srsgui-0.3.1/.github/workflows/
--rw-rw-rw-   0        0        0      388 2023-05-16 19:47:28.000000 srsgui-0.3.1/.github/workflows/pages.yml
--rw-rw-rw-   0        0        0     1356 2023-05-15 17:35:24.000000 srsgui-0.3.1/.gitignore
--rw-rw-rw-   0        0        0     1113 2023-05-16 18:54:46.000000 srsgui-0.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3730 2023-05-16 20:21:57.989693 srsgui-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     2745 2023-05-16 20:18:44.000000 srsgui-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.930685 srsgui-0.3.1/docs/
--rw-rw-rw-   0        0        0      654 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.940684 srsgui-0.3.1/docs/_static/
--rw-rw-rw-   0        0        0    31067 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/_static/cg-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    27242 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/_static/cg-terminal-screen-capture.png
--rw-rw-rw-   0        0        0     5762 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/_static/connect-dialog-box-capture.png
--rw-rw-rw-   0        0        0    71070 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/_static/example-screen-capture-1.png
--rw-rw-rw-   0        0        0    71011 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/_static/example-screen-capture-2.png
--rw-rw-rw-   0        0        0    56013 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/_static/initial-screen-capture.png
--rw-rw-rw-   0        0        0    29667 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/_static/osc-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    50740 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/_static/second-task-screen-capture.png
--rw-rw-rw-   0        0        0    39412 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/_static/terminal-with-example-2.png
--rw-rw-rw-   0        0        0    37573 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/_static/terminal-with-example.png
--rw-rw-rw-   0        0        0      222 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/changelog.rst
--rw-rw-rw-   0        0        0     1957 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/conf.py
--rw-rw-rw-   0        0        0     6097 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/create-project.rst
--rw-rw-rw-   0        0        0     6656 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/create-task.rst
--rw-rw-rw-   0        0        0     6111 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/define-instrument.rst
--rw-rw-rw-   0        0        0    15640 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/example.rst
--rw-rw-rw-   0        0        0     3726 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/index.rst
--rw-rw-rw-   0        0        0     4397 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/installation.rst
--rwxrwxrwx   0        0        0      802 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/make.bat
--rw-rw-rw-   0        0        0       34 2023-05-16 19:47:28.000000 srsgui-0.3.1/docs/requirements..txt
--rw-rw-rw-   0        0        0      936 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/srsgui.inst.communications.rst
--rw-rw-rw-   0        0        0      950 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/srsgui.inst.rst
--rw-rw-rw-   0        0        0      117 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/srsgui.rst
--rw-rw-rw-   0        0        0      989 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/srsgui.task.rst
--rw-rw-rw-   0        0        0     1542 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/srsgui.ui.commandtree.rst
--rw-rw-rw-   0        0        0      557 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/srsgui.ui.qt.rst
--rw-rw-rw-   0        0        0     1761 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/srsgui.ui.rst
--rw-rw-rw-   0        0        0      465 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/troubleshooting.rst
--rw-rw-rw-   0        0        0     1511 2023-05-16 19:47:28.000000 srsgui-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.3.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 20:21:57.989693 srsgui-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.940684 srsgui-0.3.1/srsgui/
--rw-rw-rw-   0        0        0     1537 2023-05-16 20:21:14.000000 srsgui-0.3.1/srsgui/__init__.py
--rw-rw-rw-   0        0        0      314 2023-05-15 21:54:54.000000 srsgui-0.3.1/srsgui/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.910680 srsgui-0.3.1/srsgui/examples/
-drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.940684 srsgui-0.3.1/srsgui/examples/oscilloscope example/
-drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.949690 srsgui-0.3.1/srsgui/examples/oscilloscope example/instruments/
--rw-rw-rw-   0        0        0     1828 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/examples/oscilloscope example/instruments/cg635.py
--rw-rw-rw-   0        0        0     3146 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/examples/oscilloscope example/instruments/sds1202.py
--rw-rw-rw-   0        0        0     1977 2023-05-15 21:54:54.000000 srsgui-0.3.1/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
-drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.949690 srsgui-0.3.1/srsgui/examples/oscilloscope example/tasks/
--rw-rw-rw-   0        0        0     2522 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/examples/oscilloscope example/tasks/fifth.py
--rw-rw-rw-   0        0        0     1662 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/examples/oscilloscope example/tasks/first.py
--rw-rw-rw-   0        0        0     4099 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/examples/oscilloscope example/tasks/fourth.py
--rw-rw-rw-   0        0        0     2250 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/examples/oscilloscope example/tasks/second.py
--rw-rw-rw-   0        0        0     2014 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/examples/oscilloscope example/tasks/third.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.949690 srsgui-0.3.1/srsgui/inst/
--rw-rw-rw-   0        0        0     1074 2023-05-15 21:54:54.000000 srsgui-0.3.1/srsgui/inst/__init__.py
--rw-rw-rw-   0        0        0     9886 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/inst/commands.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.959694 srsgui-0.3.1/srsgui/inst/communications/
--rw-rw-rw-   0        0        0      126 2023-05-15 21:54:54.000000 srsgui-0.3.1/srsgui/inst/communications/__init__.py
--rw-rw-rw-   0        0        0     8308 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/inst/communications/interface.py
--rw-rw-rw-   0        0        0     1276 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/inst/communications/serial_ports.py
--rw-rw-rw-   0        0        0     8772 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/inst/communications/serialinterface.py
--rw-rw-rw-   0        0        0    11333 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/inst/communications/tcpipinterface.py
--rw-rw-rw-   0        0        0    14840 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/inst/component.py
--rw-rw-rw-   0        0        0      844 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/inst/exceptions.py
--rw-rw-rw-   0        0        0    10381 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/inst/indexcommands.py
--rw-rw-rw-   0        0        0     9768 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/inst/instrument.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.959694 srsgui-0.3.1/srsgui/task/
--rw-rw-rw-   0        0        0        2 2023-05-15 21:54:54.000000 srsgui-0.3.1/srsgui/task/__init__.py
--rw-rw-rw-   0        0        0      811 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/task/callbacks.py
--rw-rw-rw-   0        0        0     6606 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/task/config.py
--rw-rw-rw-   0        0        0     5322 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/task/inputs.py
--rw-rw-rw-   0        0        0     6830 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/task/sessionhandler.py
--rw-rw-rw-   0        0        0    22136 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/task/task.py
--rw-rw-rw-   0        0        0     4225 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/task/taskresult.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.969694 srsgui-0.3.1/srsgui/ui/
--rw-rw-rw-   0        0        0        0 2023-05-15 21:54:55.000000 srsgui-0.3.1/srsgui/ui/__init__.py
--rw-rw-rw-   0        0        0     3894 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/commandhandler.py
--rw-rw-rw-   0        0        0     6138 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/commandterminal.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.979694 srsgui-0.3.1/srsgui/ui/commandtree/
--rw-rw-rw-   0        0        0        0 2023-05-15 21:54:55.000000 srsgui-0.3.1/srsgui/ui/commandtree/__init__.py
--rw-rw-rw-   0        0        0     3941 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/commandtree/commanddelegate.py
--rw-rw-rw-   0        0        0     1603 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/commandtree/commandhandler.py
--rw-rw-rw-   0        0        0    12049 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/commandtree/commanditem.py
--rw-rw-rw-   0        0        0     8334 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/commandtree/commandmodel.py
--rw-rw-rw-   0        0        0     5072 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/commandtree/commandspinbox.py
--rw-rw-rw-   0        0        0     3452 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/commandtree/commandtreeview.py
--rw-rw-rw-   0        0        0     4247 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/commandtree/commandtreewidget.py
--rw-rw-rw-   0        0        0     4806 2023-05-15 21:54:55.000000 srsgui-0.3.1/srsgui/ui/commandtree/ui_commandtreewidget.py
--rw-rw-rw-   0        0        0     9798 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/connectdlg.py
--rw-rw-rw-   0        0        0     3975 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/deviceinfohandler.py
--rw-rw-rw-   0        0        0    15880 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/dockhandler.py
--rw-rw-rw-   0        0        0    13808 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/inputpanel.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.989693 srsgui-0.3.1/srsgui/ui/qt/
--rw-rw-rw-   0        0        0      799 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/qt/QtCore.py
--rw-rw-rw-   0        0        0      677 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/qt/QtGui.py
--rw-rw-rw-   0        0        0      777 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/qt/QtWidgets.py
--rw-rw-rw-   0        0        0     1457 2023-05-15 21:54:55.000000 srsgui-0.3.1/srsgui/ui/qt/__init__.py
--rw-rw-rw-   0        0        0     1285 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/qtloghandler.py
--rw-rw-rw-   0        0        0      268 2023-05-15 21:54:55.000000 srsgui-0.3.1/srsgui/ui/resource.qrc
--rw-rw-rw-   0        0        0    15479 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/resource_rc.py
--rw-rw-rw-   0        0        0     2717 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/signalhandler.py
--rw-rw-rw-   0        0        0    47891 2023-05-15 21:54:55.000000 srsgui-0.3.1/srsgui/ui/srslogo.jpg
--rw-rw-rw-   0        0        0     1005 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/stdout.py
--rw-rw-rw-   0        0        0    24814 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/taskmain.py
--rw-rw-rw-   0        0        0    10403 2023-05-15 21:54:55.000000 srsgui-0.3.1/srsgui/ui/taskmain.ui
--rw-rw-rw-   0        0        0    11293 2023-05-15 21:54:55.000000 srsgui-0.3.1/srsgui/ui/ui_taskmain.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.940684 srsgui-0.3.1/srsgui.egg-info/
--rw-rw-rw-   0        0        0     3730 2023-05-16 20:21:57.000000 srsgui-0.3.1/srsgui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3008 2023-05-16 20:21:57.000000 srsgui-0.3.1/srsgui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 20:21:57.000000 srsgui-0.3.1/srsgui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-16 20:21:57.000000 srsgui-0.3.1/srsgui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2023-05-16 20:21:57.000000 srsgui-0.3.1/srsgui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-16 20:21:57.000000 srsgui-0.3.1/srsgui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.805499 srsgui-0.3.2/
+drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.725521 srsgui-0.3.2/.github/
+drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.729527 srsgui-0.3.2/.github/workflows/
+-rw-rw-rw-   0        0        0      388 2023-05-16 19:47:28.000000 srsgui-0.3.2/.github/workflows/pages.yml
+-rw-rw-rw-   0        0        0     1356 2023-05-16 23:33:10.000000 srsgui-0.3.2/.gitignore
+-rw-rw-rw-   0        0        0     1113 2023-05-16 18:54:46.000000 srsgui-0.3.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3725 2023-05-24 20:23:50.805499 srsgui-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2745 2023-05-16 20:18:44.000000 srsgui-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.749520 srsgui-0.3.2/docs/
+-rw-rw-rw-   0        0        0      654 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.755524 srsgui-0.3.2/docs/_static/
+-rw-rw-rw-   0        0        0    31067 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/_static/cg-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    27242 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/_static/cg-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0     5762 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/_static/connect-dialog-box-capture.png
+-rw-rw-rw-   0        0        0    71070 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/_static/example-screen-capture-1.png
+-rw-rw-rw-   0        0        0    71011 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/_static/example-screen-capture-2.png
+-rw-rw-rw-   0        0        0    56013 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/_static/initial-screen-capture.png
+-rw-rw-rw-   0        0        0    29667 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/_static/osc-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    50740 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/_static/second-task-screen-capture.png
+-rw-rw-rw-   0        0        0    39412 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/_static/terminal-with-example-2.png
+-rw-rw-rw-   0        0        0    37573 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/_static/terminal-with-example.png
+-rw-rw-rw-   0        0        0      305 2023-05-23 19:19:21.000000 srsgui-0.3.2/docs/changelog.rst
+-rw-rw-rw-   0        0        0     1957 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/conf.py
+-rw-rw-rw-   0        0        0     6097 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/create-project.rst
+-rw-rw-rw-   0        0        0     6656 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/create-task.rst
+-rw-rw-rw-   0        0        0     6111 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/define-instrument.rst
+-rw-rw-rw-   0        0        0    15640 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/example.rst
+-rw-rw-rw-   0        0        0     3726 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/index.rst
+-rw-rw-rw-   0        0        0     4407 2023-05-23 19:19:21.000000 srsgui-0.3.2/docs/installation.rst
+-rwxrwxrwx   0        0        0      802 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/make.bat
+-rw-rw-rw-   0        0        0       34 2023-05-16 19:47:28.000000 srsgui-0.3.2/docs/requirements..txt
+-rw-rw-rw-   0        0        0      936 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/srsgui.inst.communications.rst
+-rw-rw-rw-   0        0        0      950 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/srsgui.inst.rst
+-rw-rw-rw-   0        0        0      113 2023-05-23 19:19:21.000000 srsgui-0.3.2/docs/srsgui.rst
+-rw-rw-rw-   0        0        0     1077 2023-05-23 19:19:21.000000 srsgui-0.3.2/docs/srsgui.task.rst
+-rw-rw-rw-   0        0        0     2065 2023-05-23 19:19:21.000000 srsgui-0.3.2/docs/srsgui.ui.commandtree.rst
+-rw-rw-rw-   0        0        0      603 2023-05-23 19:19:21.000000 srsgui-0.3.2/docs/srsgui.ui.qt.rst
+-rw-rw-rw-   0        0        0     1646 2023-05-23 19:19:21.000000 srsgui-0.3.2/docs/srsgui.ui.rst
+-rw-rw-rw-   0        0        0      465 2023-05-16 18:43:29.000000 srsgui-0.3.2/docs/troubleshooting.rst
+-rw-rw-rw-   0        0        0     1498 2023-05-23 19:19:21.000000 srsgui-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.3.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 20:23:50.805499 srsgui-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.755524 srsgui-0.3.2/srsgui/
+-rw-rw-rw-   0        0        0     1537 2023-05-24 20:05:04.000000 srsgui-0.3.2/srsgui/__init__.py
+-rw-rw-rw-   0        0        0      314 2023-05-15 21:54:54.000000 srsgui-0.3.2/srsgui/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.729527 srsgui-0.3.2/srsgui/examples/
+drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.765521 srsgui-0.3.2/srsgui/examples/oscilloscope example/
+drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.765521 srsgui-0.3.2/srsgui/examples/oscilloscope example/instruments/
+-rw-rw-rw-   0        0        0     1828 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/examples/oscilloscope example/instruments/cg635.py
+-rw-rw-rw-   0        0        0     3146 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/examples/oscilloscope example/instruments/sds1202.py
+-rw-rw-rw-   0        0        0     1977 2023-05-15 21:54:54.000000 srsgui-0.3.2/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
+drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.775516 srsgui-0.3.2/srsgui/examples/oscilloscope example/tasks/
+-rw-rw-rw-   0        0        0     2522 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/examples/oscilloscope example/tasks/fifth.py
+-rw-rw-rw-   0        0        0     1662 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/examples/oscilloscope example/tasks/first.py
+-rw-rw-rw-   0        0        0     4099 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/examples/oscilloscope example/tasks/fourth.py
+-rw-rw-rw-   0        0        0     2250 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/examples/oscilloscope example/tasks/second.py
+-rw-rw-rw-   0        0        0     2014 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/examples/oscilloscope example/tasks/third.py
+drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.775516 srsgui-0.3.2/srsgui/inst/
+-rw-rw-rw-   0        0        0     1074 2023-05-15 21:54:54.000000 srsgui-0.3.2/srsgui/inst/__init__.py
+-rw-rw-rw-   0        0        0     9907 2023-05-24 20:06:27.000000 srsgui-0.3.2/srsgui/inst/commands.py
+drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.775516 srsgui-0.3.2/srsgui/inst/communications/
+-rw-rw-rw-   0        0        0      126 2023-05-15 21:54:54.000000 srsgui-0.3.2/srsgui/inst/communications/__init__.py
+-rw-rw-rw-   0        0        0     8308 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/inst/communications/interface.py
+-rw-rw-rw-   0        0        0     1276 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/inst/communications/serial_ports.py
+-rw-rw-rw-   0        0        0     8774 2023-05-23 19:19:21.000000 srsgui-0.3.2/srsgui/inst/communications/serialinterface.py
+-rw-rw-rw-   0        0        0    11333 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/inst/communications/tcpipinterface.py
+-rw-rw-rw-   0        0        0    15009 2023-05-24 20:06:27.000000 srsgui-0.3.2/srsgui/inst/component.py
+-rw-rw-rw-   0        0        0      844 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/inst/exceptions.py
+-rw-rw-rw-   0        0        0    10410 2023-05-24 20:06:27.000000 srsgui-0.3.2/srsgui/inst/indexcommands.py
+-rw-rw-rw-   0        0        0     9823 2023-05-24 20:06:27.000000 srsgui-0.3.2/srsgui/inst/instrument.py
+drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.785510 srsgui-0.3.2/srsgui/task/
+-rw-rw-rw-   0        0        0        2 2023-05-15 21:54:54.000000 srsgui-0.3.2/srsgui/task/__init__.py
+-rw-rw-rw-   0        0        0      811 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/task/callbacks.py
+-rw-rw-rw-   0        0        0     6606 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/task/config.py
+-rw-rw-rw-   0        0        0     5417 2023-05-23 19:19:21.000000 srsgui-0.3.2/srsgui/task/inputs.py
+-rw-rw-rw-   0        0        0     6938 2023-05-23 19:19:21.000000 srsgui-0.3.2/srsgui/task/sessionhandler.py
+-rw-rw-rw-   0        0        0    23468 2023-05-23 19:19:21.000000 srsgui-0.3.2/srsgui/task/task.py
+-rw-rw-rw-   0        0        0     4225 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/task/taskresult.py
+drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.795505 srsgui-0.3.2/srsgui/ui/
+-rw-rw-rw-   0        0        0        0 2023-05-15 21:54:55.000000 srsgui-0.3.2/srsgui/ui/__init__.py
+-rw-rw-rw-   0        0        0     3894 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/commandhandler.py
+-rw-rw-rw-   0        0        0     6880 2023-05-24 20:09:40.000000 srsgui-0.3.2/srsgui/ui/commandterminal.py
+drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.805499 srsgui-0.3.2/srsgui/ui/commandtree/
+-rw-rw-rw-   0        0        0        0 2023-05-19 00:30:39.000000 srsgui-0.3.2/srsgui/ui/commandtree/__init__.py
+-rw-rw-rw-   0        0        0     3941 2023-05-23 19:11:06.000000 srsgui-0.3.2/srsgui/ui/commandtree/commanddelegate.py
+-rw-rw-rw-   0        0        0     1603 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/commandtree/commandhandler.py
+-rw-rw-rw-   0        0        0    12359 2023-05-24 20:06:27.000000 srsgui-0.3.2/srsgui/ui/commandtree/commanditem.py
+-rw-rw-rw-   0        0        0     8669 2023-05-24 20:06:27.000000 srsgui-0.3.2/srsgui/ui/commandtree/commandmodel.py
+-rw-rw-rw-   0        0        0     5109 2023-05-24 20:06:27.000000 srsgui-0.3.2/srsgui/ui/commandtree/commandspinbox.py
+-rw-rw-rw-   0        0        0     3452 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/commandtree/commandtreeview.py
+-rw-rw-rw-   0        0        0     4851 2023-05-24 20:06:27.000000 srsgui-0.3.2/srsgui/ui/commandtree/commandtreewidget.py
+-rw-rw-rw-   0        0        0     4806 2023-05-15 21:54:55.000000 srsgui-0.3.2/srsgui/ui/commandtree/ui_commandtreewidget.py
+-rw-rw-rw-   0        0        0     9798 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/connectdlg.py
+-rw-rw-rw-   0        0        0     3975 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/deviceinfohandler.py
+-rw-rw-rw-   0        0        0    15880 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/dockhandler.py
+-rw-rw-rw-   0        0        0    13826 2023-05-23 19:19:21.000000 srsgui-0.3.2/srsgui/ui/inputpanel.py
+drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.805499 srsgui-0.3.2/srsgui/ui/qt/
+-rw-rw-rw-   0        0        0      799 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/qt/QtCore.py
+-rw-rw-rw-   0        0        0      677 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/qt/QtGui.py
+-rw-rw-rw-   0        0        0      777 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/qt/QtWidgets.py
+-rw-rw-rw-   0        0        0     1449 2023-05-23 19:19:21.000000 srsgui-0.3.2/srsgui/ui/qt/__init__.py
+-rw-rw-rw-   0        0        0     1285 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/qtloghandler.py
+-rw-rw-rw-   0        0        0      268 2023-05-15 21:54:55.000000 srsgui-0.3.2/srsgui/ui/resource.qrc
+-rw-rw-rw-   0        0        0    15479 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/resource_rc.py
+-rw-rw-rw-   0        0        0     2717 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/signalhandler.py
+-rw-rw-rw-   0        0        0    47891 2023-05-15 21:54:55.000000 srsgui-0.3.2/srsgui/ui/srslogo.jpg
+-rw-rw-rw-   0        0        0     1005 2023-05-16 18:43:29.000000 srsgui-0.3.2/srsgui/ui/stdout.py
+-rw-rw-rw-   0        0        0    25599 2023-05-24 20:06:27.000000 srsgui-0.3.2/srsgui/ui/taskmain.py
+-rw-rw-rw-   0        0        0    10403 2023-05-15 21:54:55.000000 srsgui-0.3.2/srsgui/ui/taskmain.ui
+-rw-rw-rw-   0        0        0    11293 2023-05-15 21:54:55.000000 srsgui-0.3.2/srsgui/ui/ui_taskmain.py
+drwxrwxrwx   0        0        0        0 2023-05-24 20:23:50.765521 srsgui-0.3.2/srsgui.egg-info/
+-rw-rw-rw-   0        0        0     3725 2023-05-24 20:23:50.000000 srsgui-0.3.2/srsgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3008 2023-05-24 20:23:50.000000 srsgui-0.3.2/srsgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 20:23:50.000000 srsgui-0.3.2/srsgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-24 20:23:50.000000 srsgui-0.3.2/srsgui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2023-05-24 20:23:50.000000 srsgui-0.3.2/srsgui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-24 20:23:50.000000 srsgui-0.3.2/srsgui.egg-info/top_level.txt
```

### Comparing `srsgui-0.3.1/.gitignore` & `srsgui-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/LICENSE.txt` & `srsgui-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/PKG-INFO` & `srsgui-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.3.1
+Version: 0.3.2
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsgui
 Project-URL: repository, https://github.com/thinkSRS/srsgui.git
 Project-URL: documentation, https://thinksrs.github.io/srsgui
-Project-URL: changelog, https://thinksrs.github.io/srsgui/html/changelog.html
+Project-URL: changelog, https://thinksrs.github.io/srsgui/changelog.html
 Keywords: instrument control,data acquisition,data visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `srsgui-0.3.1/README.md` & `srsgui-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/docs/Makefile` & `srsgui-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/docs/_static/cg-dir-terminal-screen-capture.png` & `srsgui-0.3.2/docs/_static/cg-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/docs/_static/cg-terminal-screen-capture.png` & `srsgui-0.3.2/docs/_static/cg-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/docs/_static/connect-dialog-box-capture.png` & `srsgui-0.3.2/docs/_static/connect-dialog-box-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/docs/_static/example-screen-capture-1.png` & `srsgui-0.3.2/docs/_static/example-screen-capture-1.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/docs/_static/example-screen-capture-2.png` & `srsgui-0.3.2/docs/_static/example-screen-capture-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/docs/_static/initial-screen-capture.png` & `srsgui-0.3.2/docs/_static/initial-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/docs/_static/osc-dir-terminal-screen-capture.png` & `srsgui-0.3.2/docs/_static/osc-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/docs/_static/second-task-screen-capture.png` & `srsgui-0.3.2/docs/_static/second-task-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/docs/_static/terminal-with-example-2.png` & `srsgui-0.3.2/docs/_static/terminal-with-example-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/docs/_static/terminal-with-example.png` & `srsgui-0.3.2/docs/_static/terminal-with-example.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/docs/conf.py` & `srsgui-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/docs/create-project.rst` & `srsgui-0.3.2/docs/create-project.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/docs/create-task.rst` & `srsgui-0.3.2/docs/create-task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/docs/define-instrument.rst` & `srsgui-0.3.2/docs/define-instrument.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/docs/example.rst` & `srsgui-0.3.2/docs/example.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/docs/index.rst` & `srsgui-0.3.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/docs/installation.rst` & `srsgui-0.3.2/docs/installation.rst`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     Commands running from the command prompt shown here are assumed using
     a Windows computer system. If you use other systems, commands may be
     different. Refer to `this page. <install-packages_>`_
 
 If you have a Python older than the required version,
 `install a newer Python. <install-python_>`_
 
-Using `virtual environment <virtual-environment_>`_ avoids possible dependency
+Using `virtual environment <virtual-environment_>`_ helps to avoid possible dependency
 conflict among Python packages. If you want to use a virtual environment, create one with
 your favorite virtual environment package. If you do not have a preference,
 use Python default ``venv``.
 
 .. code-block::
 
     python -m venv env
@@ -116,8 +116,8 @@
 .. _pyserial: https://pyserial.readthedocs.io/en/latest/pyserial.html
 .. _matplotlib: https://matplotlib.org/stable/tutorials/introductory/quick_start.html
 .. _pyside6: https://wiki.qt.io/Qt_for_Python
 .. _pyside2: https://pypi.org/project/PySide2/
 .. _pyqt5: https://pypi.org/project/PyQt5/
 .. _numpy: https://numpy.org/install/
 .. _Mit: https://choosealicense.com/licenses/mit/
-.. _GPLv3: https://choosealicense.com/licenses/gpl-3.0/
+.. _GPLv3: https://choosealicense.com/licenses/gpl-3.0/
```

### Comparing `srsgui-0.3.1/docs/make.bat` & `srsgui-0.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/docs/srsgui.inst.communications.rst` & `srsgui-0.3.2/docs/srsgui.inst.communications.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/docs/srsgui.inst.rst` & `srsgui-0.3.2/docs/srsgui.inst.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/docs/srsgui.task.rst` & `srsgui-0.3.2/docs/srsgui.task.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 srsgui.task package
 ===================
 
 srsgui.task.task module
 -----------------------
 
-.. automodule:: srsgui.task.task
+.. autoclass:: srsgui.task.task.Task
    :members:
-   :undoc-members:
+   :no-undoc-members: EscapeForResult, EscapeForDevice, EscapeForStatus, EscapeForStart, EscapeForStop
    :show-inheritance:
 
 srsgui.task.callbacks module
 ----------------------------
 
 .. automodule:: srsgui.task.callbacks
    :members:
```

### Comparing `srsgui-0.3.1/docs/srsgui.ui.commandtree.rst` & `srsgui-0.3.2/docs/srsgui.ui.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,87 @@
+srsgui.ui package
+=================
 
-.. automodule:: srsgui.ui.commandtree
+.. toctree::
+   :maxdepth: 4
+
+   srsgui.ui.commandtree.rst
+
+.. toctree::
+   :maxdepth: 4
+
+   srsgui.ui.qt.rst
+
+srsgui.ui.taskmain module
+-------------------------
+
+.. automodule:: srsgui.ui.taskmain
    :members:
    :undoc-members:
    :show-inheritance:
 
-srsgui.ui.commandtree.commanditem module
------------------------------------------
+srsgui.ui.connectdlg module
+-------------------------------
 
-.. automodule:: srsgui.ui.commandtree.commanditem
+.. automodule:: srsgui.ui.connectdlg
    :members:
    :undoc-members:
+   :inherited-members:
    :show-inheritance:
 
-srsgui.ui.commandtree.commandmodel module
-------------------------------------------
+   
+srsgui.ui.commandterminal module
+--------------------------------
+
+.. automodule:: srsgui.ui.commandterminal
+   :members:
+   :undoc-members:
+   :show-inheritance:
+   
+srsgui.ui.deviceinfohandler module
+----------------------------------
 
-.. automodule:: srsgui.ui.commandtree.commandmodel
+.. automodule:: srsgui.ui.deviceinfohandler
    :members:
    :undoc-members:
    :show-inheritance:
 
-srsgui.ui.commandtree.commandhandler module
---------------------------------------------
+srsgui.ui.dockhandler module
+----------------------------
 
-.. automodule:: srsgui.ui.commandtree.commandhandler
+.. automodule:: srsgui.ui.dockhandler
    :members:
    :undoc-members:
    :show-inheritance:
 
-srsgui.ui.commandtree.commanddelegate module
----------------------------------------------
+srsgui.ui.inputpanel module
+---------------------------
 
-.. automodule:: srsgui.ui.commandtree.commanddelegate
+.. automodule:: srsgui.ui.inputpanel
    :members:
    :undoc-members:
    :show-inheritance:
 
-srsgui.ui.commandtree.commandspinbox module
---------------------------------------------
+srsgui.ui.qtloghandler module
+-----------------------------
 
-.. automodule:: srsgui.ui.commandtree.commandspinbox
+.. automodule:: srsgui.ui.qtloghandler
    :members:
    :undoc-members:
    :show-inheritance:
 
-srsgui.ui.commandtree.commandtreeview module
----------------------------------------------
+srsgui.ui.signalhandler module
+------------------------------
 
-.. automodule:: srsgui.ui.commandtree.commandtreeview
+.. automodule:: srsgui.ui.signalhandler
    :members:
    :undoc-members:
    :show-inheritance:
 
-srsgui.ui.commandtree.commandtreewidget module
------------------------------------------------
+srsgui.ui.stdout module
+-----------------------
 
-.. automodule:: srsgui.ui.commandtree.commandtreewidget
+.. automodule:: srsgui.ui.stdout
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `srsgui-0.3.1/docs/srsgui.ui.qt.rst` & `srsgui-0.3.2/docs/srsgui.ui.qt.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+srsgui.ui.qt package
+======================
 
 .. automodule:: srsgui.ui.qt
    :members:
    :undoc-members:
    :show-inheritance:
 
 srsgui.ui.qt.QtCore module
```

### Comparing `srsgui-0.3.1/pyproject.toml` & `srsgui-0.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,14 @@
 full = ['matplotlib >= 3.6.2', 'pyside6 <= 6.4.3']
 docs = ['matplotlib', 'pyside2', 'sphinx>=5', 'sphinx-rtd-theme>=1']
 
 [project.urls]
 homepage = "https://github.com/thinkSRS/srsgui"
 repository = "https://github.com/thinkSRS/srsgui.git"
 documentation = "https://thinksrs.github.io/srsgui"
-changelog = "https://thinksrs.github.io/srsgui/html/changelog.html"
+changelog = "https://thinksrs.github.io/srsgui/changelog.html"
 
 [project.scripts]
 srsgui = "srsgui.__main__:main"
 
-# ... other project metadata fields as specified in:
-#     https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
+# Other project metadata fields as specified in:
+# https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
```

### Comparing `srsgui-0.3.1/srsgui/__init__.py` & `srsgui-0.3.2/srsgui/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
                         InstLoginFailureError, InstIdError, \
                         InstSetError, InstQueryError, InstIndexError
 
 from srsgui.inst import Interface, SerialInterface, TcpipInterface
 from srsgui.inst.instrument import Instrument
 from srsgui.inst.component import Component
 
-__version__ = "0.3.1"  # Global version number
+__version__ = "0.3.2"  # Global version number
```

### Comparing `srsgui-0.3.1/srsgui/examples/oscilloscope example/instruments/cg635.py` & `srsgui-0.3.2/srsgui/examples/oscilloscope example/instruments/cg635.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/examples/oscilloscope example/instruments/sds1202.py` & `srsgui-0.3.2/srsgui/examples/oscilloscope example/instruments/sds1202.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig` & `srsgui-0.3.2/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/examples/oscilloscope example/tasks/fifth.py` & `srsgui-0.3.2/srsgui/examples/oscilloscope example/tasks/fifth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/examples/oscilloscope example/tasks/first.py` & `srsgui-0.3.2/srsgui/examples/oscilloscope example/tasks/first.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/examples/oscilloscope example/tasks/fourth.py` & `srsgui-0.3.2/srsgui/examples/oscilloscope example/tasks/fourth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/examples/oscilloscope example/tasks/second.py` & `srsgui-0.3.2/srsgui/examples/oscilloscope example/tasks/second.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/examples/oscilloscope example/tasks/third.py` & `srsgui-0.3.2/srsgui/examples/oscilloscope example/tasks/third.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/inst/__init__.py` & `srsgui-0.3.2/srsgui/inst/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/inst/commands.py` & `srsgui-0.3.2/srsgui/inst/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
     def __get__(self, instance, instance_type):
         if instance is None:
             return self
         query_string = self._get_command_format.format(self.remote_command)
         reply = None
         try:
-            reply = instance.comm.query_text(query_string).strip()
+            reply = instance.comm.query_text(query_string).strip(' \t\n\r\x0b\x0c\x00')
             if callable(self._get_convert_function):
                 self._value = self._get_convert_function(reply)
 
             else:
                 self._value = reply
         except InstCommunicationError:
             raise InstQueryError('Error during querying: CMD: {}'.format(query_string))
```

### Comparing `srsgui-0.3.1/srsgui/inst/communications/interface.py` & `srsgui-0.3.2/srsgui/inst/communications/interface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/inst/communications/serial_ports.py` & `srsgui-0.3.2/srsgui/inst/communications/serial_ports.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/inst/communications/serialinterface.py` & `srsgui-0.3.2/srsgui/inst/communications/serialinterface.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,14 +105,15 @@
         if num > 3:
             connect_parameters.append(params[3].upper == 'TRUE')  # hardware flow control
         return connect_parameters
 
     def send_break(self, duration=0.1):
         """
         Send break signal over serial interface
+
         Parameters
         -----------
             duration: float, optioanl
                 to set how long the break signal will be
         """
         self._serial.send_break(duration)
```

### Comparing `srsgui-0.3.1/srsgui/inst/communications/tcpipinterface.py` & `srsgui-0.3.2/srsgui/inst/communications/tcpipinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/inst/component.py` & `srsgui-0.3.2/srsgui/inst/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,16 @@
                       FloatCommand, DictCommand
 from .indexcommands import IndexCommand, BoolIndexCommand, IntIndexCommand, \
                            FloatIndexCommand, DictIndexCommand
 
 
 class Component(object):
     """
-    Class is used to build hierarchical structure in an instrument.
+    Class used to build hierarchical structure in an instrument.
+
     An instrument can have multiple components and each component
     can also have multiple subcomponents. All the components
     inside an instrument shares the communication interface
     of the instrument.
 
     When the communication interface of an
     instrument changed, the instrument should call
@@ -301,21 +302,24 @@
                     k = key + f' <{cmd_instance.remote_command}>'
                 else:
                     k = key
 
                 if callable(cmd_instance):
                     if issubclass(cmd_instance.__class__, type):
                         continue
+                    if cmd_instance in self.exclude_capture:
+                        if include_excluded:
+                            commands[k + '() [M][EX]'] = ''
                     if include_methods and not k.startswith('_'):
                         commands[k + '() [M]'] = ''
                     continue
 
                 if cmd_instance in self.exclude_capture:
                     if include_excluded:
-                        commands[k + ' [X]'] = ''
+                        commands[k + ' [EX]'] = ''
                     continue
 
                 if issubclass(cmd_instance.__class__, Command):
                     if include_set_only:
                         if cmd_instance._set_enable and not cmd_instance._get_enable:
                             commands[k + ' [SO]'] = ''
                             continue
```

### Comparing `srsgui-0.3.1/srsgui/inst/exceptions.py` & `srsgui-0.3.2/srsgui/inst/exceptions.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/inst/indexcommands.py` & `srsgui-0.3.2/srsgui/inst/indexcommands.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
     def __getitem__(self, index):
         converted_index = self._convert_index(index)
         query_string = '{}? {}'.format(self.remote_command, converted_index)
         reply = None
         value = None
         try:
-            reply = self._parent.comm.query_text(query_string)
+            reply = self._parent.comm.query_text(query_string).strip(' \t\n\r\x0b\x0c\x00')
             if callable(self._get_convert_function):
                 value = self._get_convert_function(reply)
 
             else:
                 value = reply
         except InstCommunicationError:
             raise InstQueryError('Error during querying: CMD: {}'.format(query_string))
```

### Comparing `srsgui-0.3.1/srsgui/inst/instrument.py` & `srsgui-0.3.2/srsgui/inst/instrument.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,7 +291,8 @@
 
             self.connect(*parameters)
         else:
             raise KeyError('Interface type {} not available for {}'
                            .format(interface_type, self.get_name()))
         return True
 
+    exclude_capture = [connect_with_parameter_string]
```

### Comparing `srsgui-0.3.1/srsgui/task/callbacks.py` & `srsgui-0.3.2/srsgui/task/callbacks.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/task/config.py` & `srsgui-0.3.2/srsgui/task/config.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/task/inputs.py` & `srsgui-0.3.2/srsgui/task/inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ##! 
 ##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
 ##! Subject to the MIT License
 ##! 
 
 """
-Interface for input variables between Task and InputPanel in GUI
+Interface for input variables between :class:`Task <srsgui.task.task.Task>` instance
+and :class:`InputPanel <srsgui.ui.inputpanel.InputPanel>` instance in GUI
 
 """
 
 
 class BaseInput:
     def __init__(self, default_value):
         self.default_value = default_value
```

### Comparing `srsgui-0.3.1/srsgui/task/sessionhandler.py` & `srsgui-0.3.2/srsgui/task/sessionhandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from srsgui.task.taskresult import TaskResult
 
 RedBold = '<font color="red"><b>{}</b></font>'
 logger = logging.getLogger(__name__)
 
 
 class SessionHandler(object):
+    FileExtension = 'sgdata'  # srsgui data
+
     def __init__(self, use_file=False, use_db=False, use_api=False):
         self.use_file = False
         self.use_db = False
         self.use_api = False
         self._is_session_open = False
         self.serial_number = None
 
@@ -83,16 +85,17 @@
             self.add_dict_to_file('TaskResult', result.__dict__)
             logger.debug('Task result Saved')
 
     def create_file(self, task_name):
         self.path = Path(self.data_dir)
         if not self.path.exists():
             self.path.mkdir(parents=True)
-        # file_name = task_name + '-' + datetime.now().strftime('%Y%m%d-%H%M%S') + '.txt'
-        file_name = '{}-{}.txt'.format(task_name, datetime.now().strftime('%Y%m%d-%H%M%S'))
+        # file_name = task_name + '-' + datetime.now().strftime('%Y%m%d-%H%M%S') + '.sgdata'
+        file_name = '{}-{}.{}'.format(task_name, datetime.now().strftime('%Y%m%d-%H%M%S'),
+                                      self.FileExtension)
         logger.debug('Output file opened as {}\\{}'.format(self.path, file_name))
         self.output_file = open(self.path / file_name, 'w', 1)
         self.is_file_open = True
         self.table_info = {}
 
     def add_dict_to_file(self, name, data_dict):
         if not self.is_file_open:
```

### Comparing `srsgui-0.3.1/srsgui/task/task.py` & `srsgui-0.3.2/srsgui/task/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,38 +47,34 @@
     the task thread dependent on (instruments, figures, session handler), and connects
     callback functions to handle the requests from the task. The task uses
     the resources and send requests without knowing much about how they are handled by the parent
     process. It makes easy to write a derived task as a simple Python script starting from
     the base class.
     """
 
+    # Exceptions for Task
     class TaskException(Exception): pass
     class TaskSetupFailed(TaskException): pass
     class TaskRunFailed(TaskException): pass
-    """
-    Exceptions for Task
-    """
 
+    # Escape strings used in stdout redirection to GUI
     EscapeForResult = '@RESULT@'
     EscapeForDevice = '@DEVICE@'
     EscapeForStatus = '@STATUS@'
     EscapeForStart = '@START@'
     EscapeForStop = '@STOP@'
-    """
-    Escape strings used in stdout redirection to GUI
-    """
 
     input_parameters = {
         # Example float parameter
             "Define parameters": FloatInput(10.0, " Hz", 1.0, 1000.0, 1.0),
             "before use!! ":     StringInput(" or empty input_parameters.")
     }
     """
     Class variable to define parameters used in the task.
-    values in input_parameters can be changed interactively from GUI before the task runs    
+    Values in input_parameters can be changed interactively from GUI before the task runs    
     IntegerInput, FloatInput, StringInput, ListInput and InstrumentInput can be used 
     as dictionary values.     
     """
 
     additional_figure_names = []  # e.g., ['Scan Plots','Temperature Plots']
     """
     Names for extra Matplotlib figures added to use in the task
@@ -119,33 +115,35 @@
         self.figure_dict = {}
         self.figure = None
 
         self.round_float_resolution = 4
 
     def setup(self):
         """
-        Subclass needs  to override this method.
-        Put all preparation for a task in the overridden method.
+        The task-specific preparation before running test() comes in here.
+        When a task starts, it runs setup() first. If setup() finished without error,
+        it runs test(), the main routine of the task.
+        If setup() finished with an error, test() will not even start.
         """
-        self.logger.info("Task.setup() is not overridden.")
+        self.logger.warning("Task.setup() is not overridden.")
 
     def test(self):
         """
-        Subclass must override this method.
-        Check if is_running() is true to continue.
-        Add data using in add_details, create_table, and add_data_to_table.
+        Test() is the main part of a Task. And a lot of times, test() takes long time to finish.
+        Check frequently if is_running() is true. If not, test() should finish voluntarily
+        as soon as possible.
         """
-        raise NotImplementedError("We need a real test() implemented!")
+        raise NotImplementedError("A test() should be implemented!")
 
     def cleanup(self):
         """
-        Subclass need to override this method
-        Put any cleanup after task in the overridden method
+        When test() is finished, cleanup() will run subsequently.
+        Any cleanup and closing routine can be added here.
         """
-        self.logger.info('Task.cleanup() is not overridden.')
+        self.logger.warning('Task.cleanup() is not overridden.')
 
     def get_logger(self, name):
         """
         Get a logger with its handler available from the parent
         """
 
         if self.logger_prefix:
@@ -231,15 +229,15 @@
         except Exception as e:
             self.logger.error('Error during basic_cleanup: {}'.format(e))
         finally:
             self.logger.removeHandler(self.result_log_handler)
 
     def run(self):
         """
-        Overrides Thread run() method. task-speciic test() runs inside this method.
+        Overrides Thread run() method. task-specific test() runs inside this method.
         """
         try:
             self.basic_setup()
             if self._keep_running:
                 self.logger.debug("{} run started".format(self.name))
             try:
                 self.setup()  # setup from the subclass
@@ -268,15 +266,15 @@
         self._keep_running = True
         self._aborted = False
         super().start()
 
     def stop(self):
         """
         Make is_running() returns False. A task should check is_running()
-        frequently. Stop if it returns False.
+        frequently. Stop() if is_running() returns False.
         """
 
         if self._keep_running:
             self._aborted = True
             self._keep_running = False
 
     def delay(self, seconds):
@@ -475,39 +473,75 @@
         self.update_status(self.name + ' stopped')
 
     # output text to UI
     def write_text(self, text):
         self.callbacks.text_available(str(text))
 
     def get_input_parameter(self, name):
+        """
+        Get the parameter value in input_parameters
+
+        Parameters
+        -----------
+            name: str
+                the key to retrieve a value from input_parameter dictionary
+        Returns
+        -------
+            The value from the dictionary
+
+        """
         if name in self.__class__.input_parameters:
             param = self.__class__.input_parameters[name]
             value = param.get_value()
             if not hasattr(self.result, name):
                 self.add_details(str(value), name)
             return value
         else:
             raise KeyError('{} not in input_parameters'.format(name))
 
     def get_all_input_parameters(self):
+        """
+        Get all the parameter values in input_parameters
+
+        Returns
+        -------
+            dict
+                All the value with key in the dictionary format
+
+        """
+
         d = {}
         for name in self.__class__.input_parameters:
             value = self.get_input_parameter(name)
             d[name] = value
         return d
 
     @classmethod
     def set_input_parameter(cls, name, value):
+        """
+        Set manually a value in input_parameters
+
+        Parameters
+        -----------
+            name: str
+                name of the key in the dictionary, input_parameters
+
+            value
+                value associated with *name* in the dictionary
+
+        """
         if name in cls.input_parameters:
             cls.input_parameters[name].set_value(value)
         else:
             raise KeyError('{} not in input_parameters'.format(name))
 
-    # Notify UI to input_parameters for display update
     def notify_parameter_changed(self):
+        """
+        Notify UI that there are changes in input_parameters for display update
+        """
         self.callbacks.parameter_changed()
 
     def request_figure_update(self, figure=None):
         if type(figure) is not Figure:
             figure = self.figure
         self.callbacks.figure_update_requested(figure)
 
@@ -526,15 +560,26 @@
         and display update. By default, it does no data handling, but figure update request.
         GUI related data processing needs to be done here to be handled
         in proper order by the GUI event loop handler.
         """
         self.request_figure_update()
 
     def get_instrument(self, name):
-        """Get an instrument from parent's inst_dict and check its validity"""
+        """
+        Get an instrument from parent's inst_dict and check its validity
+
+        Parameters
+        ----------
+            name: str
+                name of an instrument in inst_dict
+        Returns
+        --------
+            Instrument
+                an instance of Instrument in Inst_dict
+        """
 
         if name not in self.inst_dict:
             self.logger.error("{} is not in Instrument dict.".format(name))
             return None
 
         inst = self.inst_dict[name]
         if not isinstance(inst, Instrument):
```

### Comparing `srsgui-0.3.1/srsgui/task/taskresult.py` & `srsgui-0.3.2/srsgui/task/taskresult.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/ui/commandhandler.py` & `srsgui-0.3.2/srsgui/ui/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/ui/commandterminal.py` & `srsgui-0.3.2/srsgui/ui/commandterminal.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,72 +12,77 @@
 logger = logging.getLogger(__name__)
 
 
 class CommandTerminal(QFrame):
     """
     Terminal to control instruments defined in the .taskconfig file
 
-    Type a command in one of the following ways.
+    Type a command in one of the following ways:
 
-    inst_name:remote_command
+    - inst_name:remote_command
 
         'inst_name' is the first item after the prefix  "inst:" in a line in
         the .taskconfig file. 'Remote_command' after the colon is a raw remote
         command of the instrument. Terminals send the 'remote_command' directly
         to the instrument 'inst_name', and display a reply if the instrument
         sends one back.
 
-        dut:*idn?
-        dut:mi10  - This is a RGA100 command to set scan intial mass to 10
+        dut:\*idn?
 
-    inst_name.instrument_command
+        dut:mi10  - This is a RGA100 command to set scan initial mass to 10
+
+    - inst_name.instrument_command
 
         When you use .before a command, the command is interpreted as a Python
         instrument command or a method defined in the Instrument subclass,
         which is the third item in the line starting with 'inst:' used
         in .taskconfig file.
 
         inst_name.(components.)dir  - it shows all available components, commands,
         and methods in the instrument or its component as a Python dictionary.
 
                 rga.dir
+
                 rga.status.dir
 
         rga.status.id_string - this returns the id string. It is a Python instrument
         command defined in the rga.status component.
         rga.scan.initial_mass = 10  - this changes the scan initial mass to 10.
         rga.scan.get_analog_scan()  - this is a method defined in the rga.scan component.
 
         With the prefix of 'inst_name:' or 'inst_name.', you can specify which
         instrument receive the following command, as either a raw remote command or
         a instrument command defined in a Instrument subclass.
 
-    command
+    - command
 
         if you type a command without 'inst_name.' or 'inst_name:', the command goes
         to the first instrument in the .taskconfig file. A command with dot(s) is
         interpreted as a Python instrument command or a method. A command without
         any dot will be sent directly to the first instrument in the .taskconfig file
         as a raw remote command.
-
     """
+
     command_requested = Signal(str, str)
 
     def __init__(self, parent):
         super().__init__(parent)
         self.parent = parent
         if not hasattr(parent, 'inst_dict'):
             raise AttributeError('Parent has no inst_dict')
 
         self.setup_widget()
         self.history_buffer = []
         self.buffer_index = 0
         self.buffer_size = 40
 
     def setup_widget(self):
+        """
+        Set up the terminal widget
+        """
         self.tbCommand = QTextBrowser(self)
         self.pbClear = QPushButton(self)
         self.pbClear.setText('Clear')
         self.leCommand = QLineEdit(self)
         self.pbSend = QPushButton(self)
         self.pbSend.setText('Send')
 
@@ -95,44 +100,59 @@
         self.leCommand.returnPressed.connect(self.on_send)
         self.leCommand.setText("Type  'help'  for more info")
         self.leCommand.selectAll()
         self.down_key = QShortcut(QKeySequence('DOWN'), self, self.on_down_pressed)
         self.up_key = QShortcut(QKeySequence('UP'), self, self.on_up_pressed)
 
     def on_clear(self):
+        """
+        When 'Clear' button is pressed, the terminal display and command input line is cleared.
+        """
         self.tbCommand.clear()
         self.leCommand.clear()
 
     def on_up_pressed(self):
+        """
+        When the keyboard UP arrow key is pressed, the previous command in the history
+        is displayed in the command input line.
+        """
         try:
             if len(self.history_buffer) == 0:
                 return
             self.buffer_index -= 1
             if self.buffer_index >= len(self.history_buffer):
                 self.buffer_index = 0
             elif self.buffer_index < 0:
                 self.buffer_index = len(self.history_buffer) - 1
             self.leCommand.setText(self.history_buffer[self.buffer_index])
         except Exception as e:
             self.tbCommand.append('{}'.format(e))
 
     def on_down_pressed(self):
+        """
+        When the keyboard DOWN arrow key is pressed, the next command in the history
+        is displayed in the command input line.
+        """
+
         try:
             if len(self.history_buffer) == 0:
                 return
             self.buffer_index += 1
             if self.buffer_index >= len(self.history_buffer):
                 self.buffer_index = 0
             elif self.buffer_index < 0:
                 self.buffer_index = len(self.history_buffer) - 1
             self.leCommand.setText(self.history_buffer[self.buffer_index])
         except Exception as e:
             self.tbCommand.append('{}'.format(e))
 
     def on_send(self):
+        """
+        When the Send button is pressed, send the command in the command input line to the instrument.
+        """
         try:
             cmd = self.leCommand.text().strip()
             reply = ''
             # self.tbCommand.append(cmd)
             self.leCommand.clear()
 
             self.history_buffer.append(cmd)
@@ -150,14 +170,17 @@
                 return
             self.command_requested.emit(cmd, '')
 
         except Exception as e:
             self.tbCommand.append('Error: {}'.format(str(e)))
 
     def handle_command(self, cmd, reply):
+        """
+        Display the processed command to the terminal display
+        """
         try:
             if reply:
                 self.tbCommand.append(f'{cmd}   ==>   {reply}')
             else:
                 self.tbCommand.append(f'{cmd}')
 
         except Exception as e:
```

### Comparing `srsgui-0.3.1/srsgui/ui/commandtree/commanddelegate.py` & `srsgui-0.3.2/srsgui/ui/commandtree/commanddelegate.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/ui/commandtree/commandhandler.py` & `srsgui-0.3.2/srsgui/ui/commandtree/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/ui/commandtree/commanditem.py` & `srsgui-0.3.2/srsgui/ui/commandtree/commanditem.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,50 +116,52 @@
 
     def get_formatted_value(self):
         """Return formatted value of a float"""
 
         value = self.value
         if value is None:
             return None
-
-        comp = None
-        if self.comp_type == Index:
-            comp = self.parent().comp
-        elif issubclass(type(self.comp), Command) or \
-             issubclass(type(self.comp), IndexCommand):
-            comp = self.comp
-
-        fmt = comp.fmt if comp and hasattr(comp, 'fmt') else ''
-        unit = comp.unit if comp and hasattr(comp, 'unit') else ''
-
-        if comp and (issubclass(type(comp), FloatIndexCommand) or
-                     issubclass(type(comp), FloatCommand)):
-            if value == 0.0:
-                return '0' + f' {unit}'
-            step = comp.step
-            significant_figures = comp.significant_figures
-
-            decimals = math.ceil(-math.log10(step))
-            digits = math.ceil(math.log10(abs(value))) if value else 0
-            precision = min(decimals, significant_figures - digits)
-            precision = max(precision, 0)
-            if abs(value) >= 0.1 or precision < significant_figures:
-                # Remove trailing zeros and return
-                s = f'{value:.{precision}f}'
-                if '.' in s:
-                    return s.rstrip('0').rstrip('.') + f' {unit}'
+        try:
+            comp = None
+            if self.comp_type == Index:
+                comp = self.parent().comp
+            elif issubclass(type(self.comp), Command) or \
+                 issubclass(type(self.comp), IndexCommand):
+                comp = self.comp
+
+            fmt = comp.fmt if comp and hasattr(comp, 'fmt') else ''
+            unit = comp.unit if comp and hasattr(comp, 'unit') else ''
+
+            if comp and (issubclass(type(comp), FloatIndexCommand) or
+                         issubclass(type(comp), FloatCommand)):
+                if value == 0.0:
+                    return '0' + f' {unit}'
+                step = comp.step
+                significant_figures = comp.significant_figures
+
+                decimals = math.ceil(-math.log10(step))
+                digits = math.ceil(math.log10(abs(value))) if value else 0
+                precision = min(decimals, significant_figures - digits)
+                precision = max(precision, 0)
+                if abs(value) >= 0.1 or precision < significant_figures:
+                    # Remove trailing zeros and return
+                    s = f'{value:.{precision}f}'
+                    if '.' in s:
+                        return s.rstrip('0').rstrip('.') + f' {unit}'
+                    else:
+                        return s + f' {unit}'
                 else:
-                    return s + f' {unit}'
+                    v = f'{value:.{significant_figures}e}'
+                    # Remove trailing zeros before 'e' and return
+                    t = v.split('e')
+                    return f'{t[0].rstrip("0").rstrip(".")}e{t[1]}' + f'  {unit}'
             else:
-                v = f'{value:.{significant_figures}e}'
-                # Remove trailing zeros before 'e' and return
-                t = v.split('e')
-                return f'{t[0].rstrip("0").rstrip(".")}e{t[1]}' + f'  {unit}'
-        else:
-            return f'{value:{fmt}}' + f' {unit}'
+                return f'{value:{fmt}}' + f' {unit}'
+        except Exception as e:
+            print('Format error: {} {}'.format(e, self.value))
 
     def construct_set_command_string(self, value):
         """
         Construct python command string corresponding to the item
         """
         self.name_buffer = []
         self.get_name_string(self)
@@ -180,21 +182,20 @@
                 self.name_buffer.append('[{}]'.format(item.name))
         else:
             self.name_buffer.append(item.name)
         if item.parent():
             self.get_name_string(item.parent())
 
     @classmethod
-    def load(
-        cls, comp, parent: "CommandItem" = None) -> "CommandItem":
+    def load(cls, comp, parent: "CommandItem" = None) -> "CommandItem":
         """Create a 'root' CommandItem from a Component and 
         populate its subcomponent and commands recursively.
 
         Returns:
-            CommandItem: CommandItem
+            root_item: CommandItem
         """
         root_item = CommandItem(parent)
         root_item.name = "root"
         root_item.comp = comp
 
         if issubclass(comp.__class__, Component):
             root_item.name = comp.get_name()
@@ -250,14 +251,15 @@
                         child.comp = cmd_instance
                         child.comp_type = type(cmd_instance)
                         root_item.appendChild(child)
         else:
             if callable(comp):
                 root_item.comp = comp
                 root_item.comp_type = type(comp)
+                root_item.excluded = comp in root_item.parent().comp.exclude_capture
                 root_item.is_method = True
 
             elif issubclass(type(comp), Command):
                 root_item.comp = comp
                 root_item.comp_type = type(comp)
                 root_item.excluded = comp in root_item.parent().comp.exclude_capture
                 root_item.raw_remote_command = comp.remote_command
```

### Comparing `srsgui-0.3.1/srsgui/ui/commandtree/commandmodel.py` & `srsgui-0.3.2/srsgui/ui/commandtree/commandmodel.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 ##! 
 ##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
 ##! Subject to the MIT License
 ##! 
 
 import sys
+import logging
 
 from typing import Any, Iterable, List, Dict, Union
 
 from srsgui.ui.qt.QtWidgets import QTreeView, QApplication, QHeaderView
 from srsgui.ui.qt.QtGui import QBrush, QColor
 from srsgui.ui.qt.QtCore import QAbstractItemModel, QModelIndex, \
                                 QObject, Qt, Signal
 
 from srsgui import Component
 
 from .commanditem import CommandItem, Index
 from .commanddelegate import CommandDelegate
 from .commandhandler import CommandHandler
 
+logger = logging.getLogger(__name__)
+
 
 class CommandModel(QAbstractItemModel):
     """ An editable model of Command and Component """
 
     # Signal to request to process a query to an outside command processor
     query_requested = Signal(QModelIndex)
 
@@ -40,18 +43,18 @@
         self._headers = ("  Command  ", "  Value  ")
 
     def clear(self):
         """ Clear data from the model """
         self.load(Component())
 
     def load(self, document: Component):
-        """Load model from a nested dictionary returned by json.loads()
+        """Load model from a ComponentItem instance returned by CommandItem.loads()
 
         Arguments:
-            document (dict): JSON-compatible dictionary
+            document: Component instance
         """
 
         assert isinstance(
             document, Component
         ), "`document` must be a Component, " f"not {type(document)}"
 
         self.beginResetModel()
@@ -59,59 +62,62 @@
         self._rootItem = CommandItem.load(document)
         self._rootItem.value_type = type(document)
 
         self.endResetModel()
         return True
 
     def data(self, index: QModelIndex, role: Qt.ItemDataRole) -> Any:
-        """Override from QAbstractItemModel
+        """
+        Override from QAbstractItemModel
 
         Return data from an item according index and role
         """
 
         if not index.isValid():
             return None
+        try:
+            if role == Qt.DisplayRole:
+                if index.column() == 0:
+                    item = index.internalPointer()
+                    name = item.name
+
+                    if self.show_raw_remote_command:
+                        name += f' <{item.raw_remote_command}>' if item.raw_remote_command else ''
+
+                    name += ' [M]' if item.is_method else ''
+                    name += ' [EX]' if item.excluded else ''
+                    name += ' [SO]' if item.set_enable and not item.get_enable else ''
+                    name += ' [QO]' if item.get_enable and not item.set_enable else ''
+                    return name
+
+                if index.column() == 1:
+                    item = index.internalPointer()
+                    self.query_requested.emit(index)
+                    return item.get_formatted_value()
+
+            elif role == Qt.EditRole:
+                if index.column() == 1:
+                    item = index.internalPointer()
+                    self.query_requested.emit(index)
+                    return item.value
 
-        if role == Qt.DisplayRole:
-            if index.column() == 0:
+            elif role == Qt.BackgroundRole:
                 item = index.internalPointer()
-                name = item.name
-
-                if self.show_raw_remote_command:
-                    name += f' <{item.raw_remote_command}>' if item.raw_remote_command else ''
+                if item.comp_type != Index and issubclass(item.comp_type, Component):
+                    return QBrush(QColor(243, 230, 225))
+                if item.row() % 2 == 0:
+                    return QBrush(QColor(240, 240, 253))
 
-                name += ' [M]' if item.is_method else ''
-                name += ' [EX]' if item.excluded else ''
-                name += ' [SO]' if item.set_enable and not item.get_enable else ''
-                name += ' [QO]' if item.get_enable and not item.set_enable else ''
-                return name
-
-            if index.column() == 1:
+            elif role == Qt.ToolTipRole:
                 item = index.internalPointer()
-                self.query_requested.emit(index)
-                return item.get_formatted_value()
-
-        elif role == Qt.EditRole:
-            if index.column() == 1:
-                item = index.internalPointer()
-                self.query_requested.emit(index)
-                return item.value
-
-        elif role == Qt.BackgroundRole:
-            item = index.internalPointer()
-            if item.comp_type != Index and issubclass(item.comp_type, Component):
-                return QBrush(QColor(243, 230, 225))
-            if item.row() % 2 == 0:
-                return QBrush(QColor(240, 240, 253))
-
-        elif role == Qt.ToolTipRole:
-            item = index.internalPointer()
-            if item.is_method or issubclass(item.comp_type, Component):
-                if hasattr(item.comp, '__doc__') and index.column() == 0:
-                    return item.comp.__doc__
+                if item.is_method or issubclass(item.comp_type, Component):
+                    if hasattr(item.comp, '__doc__') and index.column() == 0:
+                        return item.comp.__doc__
+        except Exception as e:
+            logger.error('Error in CommandModel.Data: {}'.format(e))
 
     def setData(self, index: QModelIndex, value: Any, role: Qt.ItemDataRole):
         """Override from QAbstractItemModel
 
         Set CommandItem according to index and role
 
         Args:
@@ -213,30 +219,37 @@
 
         if index.column() == 1 and self.is_item_editable(index):
             return Qt.ItemIsEditable | flags
         else:
             return flags
 
     def is_item_editable(self, index: QModelIndex) -> bool:
-        """Return True if item is editable, False otherwise"""
+        """
+        Return True if item is editable, False otherwise
+        """
         item = index.internalPointer()
         if type(item) == CommandItem:
             return item.is_editable()
         else:
             return False
 
     def handle_command(self, cmd_tuple):
         """
         External command processor calls this slot once a command is processed
         """
-        index = cmd_tuple[0]
-        value = cmd_tuple[1]
-        changed = cmd_tuple[2]
-        if changed:
-            self.dataChanged.emit(index, index, [Qt.DisplayRole, Qt.EditRole])
+        try:
+            index = cmd_tuple[0]
+            value = cmd_tuple[1]
+            changed = cmd_tuple[2]
+            if index.isValid() and changed:
+                item = index.internalPointer()
+                if type(item) == CommandItem:
+                    self.dataChanged.emit(index, index, [Qt.DisplayRole, Qt.EditRole])
+        except Exception as e:
+            logger.error('Error in CommandModel.handle_command: {}'.format(e))
 
 
 if __name__ == "__main__":
     from srsinst.sr860 import SR860
 
     app = QApplication(sys.argv)
     view = QTreeView()
@@ -245,20 +258,13 @@
 
     view.setModel(model)
     view.setItemDelegate(delegate)
 
     inst = SR860('tcpip', '172.25.70.129')
     inst.query_text(' ')
 
-    # inst = RGA100('tcpip','172.25.70.12','admin','admin')
-    # inst = RGA120('tcpip','172.25.70.12','admin','admin')    
-    
-    # inst.comm.set_callbacks(print, print)
-    # print(inst.check_id())
-
     model.load(inst)
 
     view.show()
     view.header().setSectionResizeMode(0, QHeaderView.Stretch)
-    # view.setAlternatingRowColors(True)
     view.resize(500, 300)
     app.exec_()
```

### Comparing `srsgui-0.3.1/srsgui/ui/commandtree/commandspinbox.py` & `srsgui-0.3.2/srsgui/ui/commandtree/commandspinbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
             prec = self.significant_figures - digits
             prec = self.decis if prec > self.decis else prec
             prec = 0 if prec < 0 else prec
             self.precision = prec
             format_string = '{:.' + str(prec) + 'f}'
             text = format_string.format(value)
         except Exception as e:
-            print(e)
+            print('Error in textFromValue: {}'.format(e))
             return ''
         return text
 
     def stepBy(self, steps):
         prefix_len = len(self.prefix())
         suffix_len = len(self.suffix())
         min_pos = prefix_len + 1 if self.value() < 0 else prefix_len
```

### Comparing `srsgui-0.3.1/srsgui/ui/commandtree/commandtreeview.py` & `srsgui-0.3.2/srsgui/ui/commandtree/commandtreeview.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/ui/commandtree/commandtreewidget.py` & `srsgui-0.3.2/srsgui/ui/commandtree/commandtreewidget.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ##! 
 ##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
 ##! Subject to the MIT License
 ##! 
 
 import logging
+import time
 
 from srsgui.ui.qt.QtCore import Qt, QModelIndex
 from srsgui.ui.qt.QtWidgets import QWidget
 
 from .ui_commandtreewidget import Ui_CommandTreeWidget
 from .commandmodel import CommandModel
 from .commanddelegate import CommandDelegate
@@ -30,14 +31,17 @@
         self.name = None
         self.query_only_included = False
         self.set_only_included = False
         self.excluded_included = False
         self.method_included = False
         self.show_raw_command = False
 
+        self.capture_time = 0.0  # time of the last capture
+        self.capture_time_limit = 5.0  # seconds before a new capture
+
         self.model = CommandModel()
         self.tree_view.setItemDelegate(CommandDelegate())
         self.tree_view.setModel(self.model)
 
         self.expand_button.hide()
 
         self.query_only_checkbox.stateChanged.connect(self.on_query_only_changed)
@@ -72,14 +76,26 @@
 
     def on_raw_command_changed(self, state):
         self.tree_view.show_raw_command = state
         self.model.show_raw_remote_command = self.tree_view.show_raw_command
         self.model.dataChanged.emit(QModelIndex(), QModelIndex())
 
     def on_capture_clicked(self):
+        # Limit the frequency of new capture
+        if self.parent and hasattr(self.parent, 'is_task_running'):
+            if self.parent.is_task_running():
+                logger.warning('No capture allowed during a task running')
+                return
+
+        current_time = time.time()
+        if current_time - self.capture_time < self.capture_time_limit:
+            return
+        else:
+            self.capture_time = current_time
+
         if self.inst is not None and self.inst.is_connected():
             try:
                 self.model.show_raw_remote_command = self.show_raw_command
                 self.model.load(self.inst)
                 self.tree_view.expandToDepth(1)
                 self.tree_view.resizeColumnToContents(0)
                 # self.tree_view.collapseAll()
@@ -96,14 +112,15 @@
 
     def on_collapse_clicked(self):
         self.tree_view.collapseAll()
 
     def closeEvent(self, event) -> None:
         self.model.command_handler.stop()
 
+
 if __name__ == '__main__':
     import sys
     from srsgui.ui.qt.QtWidgets import QApplication, QHeaderView
     from srsinst.sr860 import SR860
 
     app = QApplication(sys.argv)
```

### Comparing `srsgui-0.3.1/srsgui/ui/commandtree/ui_commandtreewidget.py` & `srsgui-0.3.2/srsgui/ui/commandtree/ui_commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/ui/connectdlg.py` & `srsgui-0.3.2/srsgui/ui/connectdlg.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/ui/deviceinfohandler.py` & `srsgui-0.3.2/srsgui/ui/deviceinfohandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/ui/dockhandler.py` & `srsgui-0.3.2/srsgui/ui/dockhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/ui/inputpanel.py` & `srsgui-0.3.2/srsgui/ui/inputpanel.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 import logging
 logger = logging.getLogger(__name__)
 
 
 class InputPanel(QScrollArea):
     """
-    To build the input panel in an instance of :class:`srsgui.ui.taskmain.TaskMain` class
-    based on input_parameters of a subclass of :class:`srsgui.task.task.Task` class
+    To build the input panel in an instance of :class:`TaskMain <srsgui.ui.taskmain.TaskMain>` class
+    based on input_parameters in a subclass of :class:`Task <srsgui.task.task.Task>` class
     """
     FirstColumn = 0
     SecondColumn = 1
 
     def __init__(self, task_class: Task, parent):
         try:
             if not issubclass(task_class, Task):
```

### Comparing `srsgui-0.3.1/srsgui/ui/qt/QtCore.py` & `srsgui-0.3.2/srsgui/ui/qt/QtCore.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/ui/qt/QtGui.py` & `srsgui-0.3.2/srsgui/ui/qt/QtGui.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/ui/qt/QtWidgets.py` & `srsgui-0.3.2/srsgui/ui/qt/QtWidgets.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/ui/qt/__init__.py` & `srsgui-0.3.2/srsgui/ui/qt/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+
 """
 ``srsgui.ui.qt`` subpackage enables SRSGUI to use either PySide6, Pyside2 or PyQt5 as Qt binder for Python.
 It checks if either Qt binder is installed in the order listed above. If any found installed, it uses the one.
-If you use PyQt6 or PyQt5, the whole SRSGUI package is subjected to be used under the GPL3 license, which PyQt requires.
-When you use PySide6 or PySide2, , which is provided under the LGPL license, you can use SRSGUI under its intended MIT license.
+If you use PyQt5, the whole SRSGUI package is subjected to be used under the GPL3 license, which PyQt requires.
+When you use PySide6 or PySide2, which is provided under the LGPL license, you can use SRSGUI under its
+intended MIT license.
 """
 
 from importlib import import_module
 
 PYSIDE6 = 'PySide6'
 PYSIDE2 = 'PySide2'
 PYQT6 = 'PyQt6'
```

### Comparing `srsgui-0.3.1/srsgui/ui/qtloghandler.py` & `srsgui-0.3.2/srsgui/ui/qtloghandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/ui/resource_rc.py` & `srsgui-0.3.2/srsgui/ui/resource_rc.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/ui/signalhandler.py` & `srsgui-0.3.2/srsgui/ui/signalhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/ui/srslogo.jpg` & `srsgui-0.3.2/srsgui/ui/srslogo.jpg`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/ui/stdout.py` & `srsgui-0.3.2/srsgui/ui/stdout.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/ui/taskmain.py` & `srsgui-0.3.2/srsgui/ui/taskmain.py`

 * *Files 6% similar despite different names*

```diff
@@ -144,14 +144,20 @@
         self.menu_Help.addAction(self.about)
         self.about.triggered.connect(self.onAbout)
 
         self.menu_Tasks.triggered.connect(self.onTaskSelect)
         self.menu_Instruments.triggered.connect(self.onInstrumentSelect)
 
     def load_tasks(self):
+        """
+        Load configuration info from a .taskconfig file specified from
+            #. Command line argument
+            #. Settings saved in the registry
+            #. Application default .taskconfig file
+        """
         try:
             # Clear console and result display
             self.console.clear()
             self.taskResult.clear()
             self.terminal_widget.tbCommand.clear()
 
             if self.initial_load:
@@ -251,17 +257,14 @@
                             continue
                 action_task = QAction(self)
                 action_task.setText(name)
                 m.addAction(action_task)
         except Exception as e:
             logger.error('Error adding to Task menu Task:{}  Error: {}'.format(name, e))
 
-    def get_logo_file(self):
-        return self.LogoFile
-
     def print_redirect(self, text):
         """
         Handles text output for stdout, stderr and various text output
         from :class:`srsgui.task.task.Task`
         """
         try:
             if len(text) < 2:
@@ -348,17 +351,23 @@
             for inst in self.inst_dict:
                 self.inst_info_handler.update_info(inst)
             logger.debug('onTaskFinished finished')
         except Exception as e:
             logger.error('Error onTaskFinished: {}'.format(e))
 
     def is_task_running(self):
+        """
+        Check if a task is running
+        """
         return self._busy_flag
 
     def update_figure(self, figure):
+        """
+        Handle figure update request from a task
+        """
         self.dock_handler.update_figure(figure)
 
     def onTaskSelect(self, action):
         try:
             if self.is_task_running():  # Another task is running
                 return
 
@@ -500,22 +509,18 @@
             if self.question_result_value:
                 inst.disconnect()
                 self.inst_info_handler.update_info(inst_name)
                 logger.info('{} is disconnected'.format(inst_name))
         except Exception as e:
             logger.error(e)
 
-    def okToContinue(self):
-        if self.task and self.task.is_running():
-            self.display_question("Do you want to quit while a task is running?")
-            if not self.question_result_value:
-                return False
-        return True
-
     def display_question(self, question, return_type=bool):
+        """
+        Slot to handle a question from the :meth:`Task.ask_question<srsgui.task.task.Task.ask_question>`
+        """
         try:
             self.question_result = None
             self.question_result_value = None
             # text = '<font size=12>{}</font>'.format(question)
             text = question
             title = self.task.name if self.task is not None else ""
 
@@ -552,29 +557,45 @@
                     self.question_result_value = None
 
             else:
                 raise TypeError('Not supported type {}'.format(return_type))
         except Exception as e:
             logger.error('display_question error: {}'.format(e))
 
+    def okToContinue(self):
+        """
+        Check if ok to quit the application.
+        """
+        if self.task and self.task.is_running():
+            self.display_question("Do you want to quit while a task is running?")
+            if not self.question_result_value:
+                return False
+        return True
+
     def closeEvent(self, event):
+        """
+        Override the default closeEvent handler
+        """
         if self.okToContinue():
             # Save settings
             self.save_settings()
 
             self.dock_handler.stop_command_handlers()
 
             # Close instruments
             inst_dict = self.inst_dict
             for key in inst_dict:
                 if hasattr(inst_dict[key], "disconnect"):
                     inst_dict[key].disconnect()
         else:
             event.ignore()
 
+    def get_logo_file(self):
+        return self.LogoFile
+
     def handle_initial_image(self, task_class):
         try:
             self.dock_handler.clear_figures()
             attr = 'InitialImage'
             image_file = self.get_logo_file()
             if hasattr(task_class, attr):
                 i_file = getattr(task_class, attr)
@@ -597,14 +618,17 @@
             msg += '{} version: {}\n'.format(inst.__class__.__name__, version)
         msg += '\nSrsgui version: {}\n'.format(__version__)
         msg += '\n{} version: {}\n'.format(QT_BINDER, QT_BINDER_VERSION)
         msg += 'Python version: {}\n'.format(sys.version)
         self.display_question(msg, None)
 
     def load_settings(self):
+        """
+        Load settings from the registry
+        """
         try:
             self.default_config_file = self.settings.value("ConfigFile", "")
             sizes = self.settings.value("MainWindow/Splitter1", [100, 200, 200])
             self.splitter.setSizes([int(i) for i in sizes])
             sizes = self.settings.value("MainWindow/Splitter2", [150, 500])
             self.splitter_2.setSizes([int(i) for i in sizes])
             geo = self.settings.value("MainWindow/Geometry")
@@ -612,14 +636,17 @@
             if geo and state:
                 self.restoreGeometry(geo)
                 self.restoreState(state)
         except Exception as e:
             logger.error('During load_setting, {}'.format(e))
 
     def save_settings(self):
+        """
+        Save settings to the registry
+        """
         self.settings.setValue("ConfigFile", self.default_config_file)
         self.settings.setValue("MainWindow/Splitter1", self.splitter.sizes())
         self.settings.setValue("MainWindow/Splitter2", self.splitter_2.sizes())
 
         self.settings.setValue("MainWindow/Geometry", self.saveGeometry())
         self.settings.setValue("MainWindow/State", self.saveState())
```

### Comparing `srsgui-0.3.1/srsgui/ui/taskmain.ui` & `srsgui-0.3.2/srsgui/ui/taskmain.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui/ui/ui_taskmain.py` & `srsgui-0.3.2/srsgui/ui/ui_taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.1/srsgui.egg-info/PKG-INFO` & `srsgui-0.3.2/srsgui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.3.1
+Version: 0.3.2
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsgui
 Project-URL: repository, https://github.com/thinkSRS/srsgui.git
 Project-URL: documentation, https://thinksrs.github.io/srsgui
-Project-URL: changelog, https://thinksrs.github.io/srsgui/html/changelog.html
+Project-URL: changelog, https://thinksrs.github.io/srsgui/changelog.html
 Keywords: instrument control,data acquisition,data visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `srsgui-0.3.1/srsgui.egg-info/SOURCES.txt` & `srsgui-0.3.2/srsgui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

