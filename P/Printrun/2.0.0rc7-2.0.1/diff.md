# Comparing `tmp/Printrun-2.0.0rc7.tar.gz` & `tmp/Printrun-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Printrun-2.0.0rc7.tar", last modified: Sun Sep  6 12:00:20 2020, max compression
+gzip compressed data, was "Printrun-2.0.1.tar", last modified: Wed May 24 08:25:27 2023, max compression
```

## Comparing `Printrun-2.0.0rc7.tar` & `Printrun-2.0.1.tar`

### file list

```diff
@@ -1,137 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:20.843647 Printrun-2.0.0rc7/
--rw-r--r--   0 runner    (1001) docker     (116)    35147 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/COPYING
--rw-r--r--   0 runner    (1001) docker     (116)      169 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    53454 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/P-face.icns
--rw-r--r--   0 runner    (1001) docker     (116)    24259 2020-09-06 12:00:20.843647 Printrun-2.0.0rc7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:20.827647 Printrun-2.0.0rc7/Printrun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    24259 2020-09-06 12:00:20.000000 Printrun-2.0.0rc7/Printrun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2631 2020-09-06 12:00:20.000000 Printrun-2.0.0rc7/Printrun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-09-06 12:00:20.000000 Printrun-2.0.0rc7/Printrun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-09-06 12:00:20.000000 Printrun-2.0.0rc7/Printrun.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      261 2020-09-06 12:00:20.000000 Printrun-2.0.0rc7/Printrun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2020-09-06 12:00:20.000000 Printrun-2.0.0rc7/Printrun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/README.cleanup
--rw-r--r--   0 runner    (1001) docker     (116)     1547 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/README.i18n
--rw-r--r--   0 runner    (1001) docker     (116)    19389 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:20.831647 Printrun-2.0.0rc7/images/
--rw-r--r--   0 runner    (1001) docker     (116)     1166 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/images/arrow_down.png
--rw-r--r--   0 runner    (1001) docker     (116)     1053 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/images/arrow_keys.png
--rw-r--r--   0 runner    (1001) docker     (116)     1048 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/images/arrow_up.png
--rw-r--r--   0 runner    (1001) docker     (116)    13223 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/images/control_mini.png
--rw-r--r--   0 runner    (1001) docker     (116)    24014 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/images/control_mini.svg
--rw-r--r--   0 runner    (1001) docker     (116)    57499 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/images/control_xy.png
--rw-r--r--   0 runner    (1001) docker     (116)    72098 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/images/control_xy.svg
--rw-r--r--   0 runner    (1001) docker     (116)     9236 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/images/control_z.png
--rw-r--r--   0 runner    (1001) docker     (116)    22826 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/images/control_z.svg
--rw-r--r--   0 runner    (1001) docker     (116)     6718 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/images/control_z_mini.png
--rw-r--r--   0 runner    (1001) docker     (116)    19749 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/images/control_z_mini.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1010 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/images/edit.png
--rw-r--r--   0 runner    (1001) docker     (116)      878 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/images/fit.png
--rw-r--r--   0 runner    (1001) docker     (116)     1424 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/images/inject.png
--rw-r--r--   0 runner    (1001) docker     (116)     1194 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/images/reset.png
--rw-r--r--   0 runner    (1001) docker     (116)     1739 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/images/zoom_in.png
--rw-r--r--   0 runner    (1001) docker     (116)     1174 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/images/zoom_out.png
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:20.831647 Printrun-2.0.0rc7/locale/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:20.819646 Printrun-2.0.0rc7/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:20.831647 Printrun-2.0.0rc7/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)     1983 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/locale/ar/LC_MESSAGES/plater.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:20.819646 Printrun-2.0.0rc7/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:20.831647 Printrun-2.0.0rc7/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)     1551 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/locale/de/LC_MESSAGES/plater.mo
--rw-r--r--   0 runner    (1001) docker     (116)     1810 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/locale/de/LC_MESSAGES/plater.po
--rw-r--r--   0 runner    (1001) docker     (116)     9961 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/locale/de/LC_MESSAGES/pronterface.mo
--rw-r--r--   0 runner    (1001) docker     (116)    49442 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/locale/de/LC_MESSAGES/pronterface.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:20.819646 Printrun-2.0.0rc7/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:20.831647 Printrun-2.0.0rc7/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)     1622 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/locale/fr/LC_MESSAGES/plater.mo
--rw-r--r--   0 runner    (1001) docker     (116)     2022 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/locale/fr/LC_MESSAGES/plater.po
--rw-r--r--   0 runner    (1001) docker     (116)    40986 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/locale/fr/LC_MESSAGES/pronterface.mo
--rw-r--r--   0 runner    (1001) docker     (116)    61876 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/locale/fr/LC_MESSAGES/pronterface.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:20.819646 Printrun-2.0.0rc7/locale/hy/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:20.831647 Printrun-2.0.0rc7/locale/hy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)     2107 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/locale/hy/LC_MESSAGES/plater.po
--rw-r--r--   0 runner    (1001) docker     (116)    73573 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/locale/hy/LC_MESSAGES/pronterface.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:20.819646 Printrun-2.0.0rc7/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:20.835647 Printrun-2.0.0rc7/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)     1638 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/locale/it/LC_MESSAGES/plater.mo
--rw-r--r--   0 runner    (1001) docker     (116)     1993 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/locale/it/LC_MESSAGES/plater.po
--rw-r--r--   0 runner    (1001) docker     (116)    10146 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/locale/it/LC_MESSAGES/pronterface.mo
--rw-r--r--   0 runner    (1001) docker     (116)    49929 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/locale/it/LC_MESSAGES/pronterface.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:20.819646 Printrun-2.0.0rc7/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:20.835647 Printrun-2.0.0rc7/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)     6719 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/locale/nl/LC_MESSAGES/pronterface.mo
--rw-r--r--   0 runner    (1001) docker     (116)    48369 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/locale/nl/LC_MESSAGES/pronterface.po
--rw-r--r--   0 runner    (1001) docker     (116)     1535 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/locale/plater.pot
--rw-r--r--   0 runner    (1001) docker     (116)    41862 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/locale/pronterface.pot
--rw-r--r--   0 runner    (1001) docker     (116)      992 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/plater.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (116)      237 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/plater.desktop
--rw-r--r--   0 runner    (1001) docker     (116)    59582 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/plater.ico
--rw-r--r--   0 runner    (1001) docker     (116)     2090 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/plater.png
--rwxr-xr-x   0 runner    (1001) docker     (116)     1780 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/plater.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     3639 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printcore.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:20.839647 Printrun-2.0.0rc7/printrun/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3125 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/eventhandler.py
--rw-r--r--   0 runner    (1001) docker     (116)     4933 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/excluder.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    10956 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/gcodeplater.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    30639 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/gcoder.py
--rw-r--r--   0 runner    (1001) docker     (116)     9791 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/gcoder_line.pyx
--rw-r--r--   0 runner    (1001) docker     (116)     1016 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/gcoder_line_extra.h
--rwxr-xr-x   0 runner    (1001) docker     (116)    20251 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/gcview.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:20.839647 Printrun-2.0.0rc7/printrun/gl/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/gl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:20.839647 Printrun-2.0.0rc7/printrun/gl/libtatlin/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/gl/libtatlin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    48618 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/gl/libtatlin/actors.py
--rw-r--r--   0 runner    (1001) docker     (116)    17023 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/gl/panel.py
--rw-r--r--   0 runner    (1001) docker     (116)     2724 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/gl/trackball.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:20.843647 Printrun-2.0.0rc7/printrun/gui/
--rw-r--r--   0 runner    (1001) docker     (116)    13722 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3276 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/gui/bufferedcanvas.py
--rw-r--r--   0 runner    (1001) docker     (116)    20859 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/gui/controls.py
--rw-r--r--   0 runner    (1001) docker     (116)    21191 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/gui/graph.py
--rw-r--r--   0 runner    (1001) docker     (116)     2236 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/gui/log.py
--rw-r--r--   0 runner    (1001) docker     (116)     4251 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/gui/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (116)     1466 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/gui/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     4990 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/gui/viz.py
--rw-r--r--   0 runner    (1001) docker     (116)    16728 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/gui/widgets.py
--rw-r--r--   0 runner    (1001) docker     (116)    19954 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/gui/xybuttons.py
--rw-r--r--   0 runner    (1001) docker     (116)     6048 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/gui/zbuttons.py
--rw-r--r--   0 runner    (1001) docker     (116)    22300 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/gviz.py
--rw-r--r--   0 runner    (1001) docker     (116)     1922 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/injectgcode.py
--rw-r--r--   0 runner    (1001) docker     (116)    12188 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/objectplater.py
--rw-r--r--   0 runner    (1001) docker     (116)     7060 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/packer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:20.843647 Printrun-2.0.0rc7/printrun/plugins/
--rw-r--r--   0 runner    (1001) docker     (116)      784 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1989 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/plugins/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:20.843647 Printrun-2.0.0rc7/printrun/power/
--rw-r--r--   0 runner    (1001) docker     (116)     5183 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/power/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3105 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/power/osx.py
--rw-r--r--   0 runner    (1001) docker     (116)    31878 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/printcore.py
--rw-r--r--   0 runner    (1001) docker     (116)    38424 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/projectlayer.py
--rw-r--r--   0 runner    (1001) docker     (116)    73665 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/pronsole.py
--rw-r--r--   0 runner    (1001) docker     (116)   111761 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/pronterface.py
--rw-r--r--   0 runner    (1001) docker     (116)     4192 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/rpc.py
--rw-r--r--   0 runner    (1001) docker     (116)    17503 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:20.843647 Printrun-2.0.0rc7/printrun/spoolmanager/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/spoolmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8798 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/spoolmanager/spoolmanager.py
--rw-r--r--   0 runner    (1001) docker     (116)    25647 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/spoolmanager/spoolmanager_gui.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    21296 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/stlplater.py
--rw-r--r--   0 runner    (1001) docker     (116)    13806 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/stltool.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    18057 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/stlview.py
--rw-r--r--   0 runner    (1001) docker     (116)     9470 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     4774 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/printrun/zscaper.py
--rw-r--r--   0 runner    (1001) docker     (116)     1175 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/pronsole.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (116)      246 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/pronsole.desktop
--rw-r--r--   0 runner    (1001) docker     (116)    59582 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/pronsole.ico
--rw-r--r--   0 runner    (1001) docker     (116)     1090 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/pronsole.png
--rwxr-xr-x   0 runner    (1001) docker     (116)     2295 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/pronsole.py
--rw-r--r--   0 runner    (1001) docker     (116)     1292 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/pronterface.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (116)      351 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/pronterface.desktop
--rw-r--r--   0 runner    (1001) docker     (116)    67646 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/pronterface.ico
--rw-r--r--   0 runner    (1001) docker     (116)     9063 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/pronterface.png
--rwxr-xr-x   0 runner    (1001) docker     (116)     2428 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/pronterface.py
--rw-r--r--   0 runner    (1001) docker     (116)      289 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-09-06 12:00:20.843647 Printrun-2.0.0rc7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (116)     3253 2020-09-06 12:00:10.000000 Printrun-2.0.0rc7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:27.760574 Printrun-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-24 08:25:15.000000 Printrun-2.0.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-24 08:25:15.000000 Printrun-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    53454 2023-05-24 08:25:15.000000 Printrun-2.0.1/P-face.icns
+-rw-r--r--   0 runner    (1001) docker     (123)    22591 2023-05-24 08:25:27.760574 Printrun-2.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:27.748574 Printrun-2.0.1/Printrun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22591 2023-05-24 08:25:27.000000 Printrun-2.0.1/Printrun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-24 08:25:27.000000 Printrun-2.0.1/Printrun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 08:25:27.000000 Printrun-2.0.1/Printrun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 08:25:27.000000 Printrun-2.0.1/Printrun.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-24 08:25:27.000000 Printrun-2.0.1/Printrun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 08:25:27.000000 Printrun-2.0.1/Printrun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-24 08:25:15.000000 Printrun-2.0.1/README.cleanup
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-24 08:25:15.000000 Printrun-2.0.1/README.i18n
+-rw-r--r--   0 runner    (1001) docker     (123)    21629 2023-05-24 08:25:15.000000 Printrun-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:27.752575 Printrun-2.0.1/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-24 08:25:15.000000 Printrun-2.0.1/images/arrow_down.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-24 08:25:15.000000 Printrun-2.0.1/images/arrow_keys.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-24 08:25:15.000000 Printrun-2.0.1/images/arrow_up.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-05-24 08:25:15.000000 Printrun-2.0.1/images/control_mini.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24014 2023-05-24 08:25:15.000000 Printrun-2.0.1/images/control_mini.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    57499 2023-05-24 08:25:15.000000 Printrun-2.0.1/images/control_xy.png
+-rw-r--r--   0 runner    (1001) docker     (123)    72098 2023-05-24 08:25:15.000000 Printrun-2.0.1/images/control_xy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-05-24 08:25:15.000000 Printrun-2.0.1/images/control_z.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22826 2023-05-24 08:25:15.000000 Printrun-2.0.1/images/control_z.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-05-24 08:25:15.000000 Printrun-2.0.1/images/control_z_mini.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19749 2023-05-24 08:25:15.000000 Printrun-2.0.1/images/control_z_mini.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-24 08:25:15.000000 Printrun-2.0.1/images/edit.png
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-24 08:25:15.000000 Printrun-2.0.1/images/fit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-24 08:25:15.000000 Printrun-2.0.1/images/inject.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-24 08:25:15.000000 Printrun-2.0.1/images/reset.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-24 08:25:15.000000 Printrun-2.0.1/images/zoom_in.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-24 08:25:15.000000 Printrun-2.0.1/images/zoom_out.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:27.752575 Printrun-2.0.1/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:27.740574 Printrun-2.0.1/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:27.752575 Printrun-2.0.1/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-24 08:25:15.000000 Printrun-2.0.1/locale/ar/LC_MESSAGES/plater.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:27.740574 Printrun-2.0.1/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:27.752575 Printrun-2.0.1/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-05-24 08:25:15.000000 Printrun-2.0.1/locale/de/LC_MESSAGES/plater.po
+-rw-r--r--   0 runner    (1001) docker     (123)    77348 2023-05-24 08:25:15.000000 Printrun-2.0.1/locale/de/LC_MESSAGES/pronterface.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:27.740574 Printrun-2.0.1/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:27.752575 Printrun-2.0.1/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-24 08:25:15.000000 Printrun-2.0.1/locale/fr/LC_MESSAGES/plater.po
+-rw-r--r--   0 runner    (1001) docker     (123)    61876 2023-05-24 08:25:15.000000 Printrun-2.0.1/locale/fr/LC_MESSAGES/pronterface.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:27.740574 Printrun-2.0.1/locale/hy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:27.752575 Printrun-2.0.1/locale/hy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-24 08:25:15.000000 Printrun-2.0.1/locale/hy/LC_MESSAGES/plater.po
+-rw-r--r--   0 runner    (1001) docker     (123)    73775 2023-05-24 08:25:15.000000 Printrun-2.0.1/locale/hy/LC_MESSAGES/pronterface.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:27.740574 Printrun-2.0.1/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:27.752575 Printrun-2.0.1/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-24 08:25:15.000000 Printrun-2.0.1/locale/it/LC_MESSAGES/plater.po
+-rw-r--r--   0 runner    (1001) docker     (123)    49929 2023-05-24 08:25:15.000000 Printrun-2.0.1/locale/it/LC_MESSAGES/pronterface.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:27.740574 Printrun-2.0.1/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:27.752575 Printrun-2.0.1/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    48369 2023-05-24 08:25:15.000000 Printrun-2.0.1/locale/nl/LC_MESSAGES/pronterface.po
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-24 08:25:15.000000 Printrun-2.0.1/locale/plater.pot
+-rw-r--r--   0 runner    (1001) docker     (123)    52224 2023-05-24 08:25:15.000000 Printrun-2.0.1/locale/pronterface.pot
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-24 08:25:15.000000 Printrun-2.0.1/plater.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-24 08:25:15.000000 Printrun-2.0.1/plater.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)    59582 2023-05-24 08:25:15.000000 Printrun-2.0.1/plater.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-24 08:25:15.000000 Printrun-2.0.1/plater.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1780 2023-05-24 08:25:15.000000 Printrun-2.0.1/plater.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3641 2023-05-24 08:25:15.000000 Printrun-2.0.1/printcore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:27.756574 Printrun-2.0.1/printrun/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/eventhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/excluder.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10956 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/gcodeplater.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29995 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/gcoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/gcoder_line.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/gcoder_line_extra.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21150 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/gcview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:27.756574 Printrun-2.0.1/printrun/gl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/gl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:27.756574 Printrun-2.0.1/printrun/gl/libtatlin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/gl/libtatlin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48911 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/gl/libtatlin/actors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17232 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/gl/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/gl/trackball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:27.760574 Printrun-2.0.1/printrun/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)    13721 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/gui/bufferedcanvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/gui/controls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21456 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/gui/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/gui/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/gui/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/gui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/gui/viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16728 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/gui/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19964 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/gui/xybuttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/gui/zbuttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22401 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/gviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/injectgcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/objectplater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/packer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:27.760574 Printrun-2.0.1/printrun/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/plugins/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:27.760574 Printrun-2.0.1/printrun/power/
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/power/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/power/osx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31902 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/printcore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38586 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/projectlayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73665 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/pronsole.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120260 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/pronterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:27.760574 Printrun-2.0.1/printrun/spoolmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/spoolmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/spoolmanager/spoolmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25647 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/spoolmanager/spoolmanager_gui.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21298 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/stlplater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/stltool.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18146 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/stlview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12247 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-24 08:25:15.000000 Printrun-2.0.1/printrun/zscaper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-24 08:25:15.000000 Printrun-2.0.1/pronsole.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-24 08:25:15.000000 Printrun-2.0.1/pronsole.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)    59582 2023-05-24 08:25:15.000000 Printrun-2.0.1/pronsole.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-24 08:25:15.000000 Printrun-2.0.1/pronsole.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2295 2023-05-24 08:25:15.000000 Printrun-2.0.1/pronsole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-24 08:25:15.000000 Printrun-2.0.1/pronterface.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-24 08:25:15.000000 Printrun-2.0.1/pronterface.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)    67646 2023-05-24 08:25:15.000000 Printrun-2.0.1/pronterface.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-05-24 08:25:15.000000 Printrun-2.0.1/pronterface.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2428 2023-05-24 08:25:15.000000 Printrun-2.0.1/pronterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-24 08:25:15.000000 Printrun-2.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 08:25:27.760574 Printrun-2.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3253 2023-05-24 08:25:15.000000 Printrun-2.0.1/setup.py
```

### Comparing `Printrun-2.0.0rc7/COPYING` & `Printrun-2.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/P-face.icns` & `Printrun-2.0.1/P-face.icns`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/Printrun.egg-info/SOURCES.txt` & `Printrun-2.0.1/Printrun.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -44,29 +44,22 @@
 images/inject.png
 images/reset.png
 images/zoom_in.png
 images/zoom_out.png
 locale/plater.pot
 locale/pronterface.pot
 locale/ar/LC_MESSAGES/plater.po
-locale/de/LC_MESSAGES/plater.mo
 locale/de/LC_MESSAGES/plater.po
-locale/de/LC_MESSAGES/pronterface.mo
 locale/de/LC_MESSAGES/pronterface.po
-locale/fr/LC_MESSAGES/plater.mo
 locale/fr/LC_MESSAGES/plater.po
-locale/fr/LC_MESSAGES/pronterface.mo
 locale/fr/LC_MESSAGES/pronterface.po
 locale/hy/LC_MESSAGES/plater.po
 locale/hy/LC_MESSAGES/pronterface.po
-locale/it/LC_MESSAGES/plater.mo
 locale/it/LC_MESSAGES/plater.po
-locale/it/LC_MESSAGES/pronterface.mo
 locale/it/LC_MESSAGES/pronterface.po
-locale/nl/LC_MESSAGES/pronterface.mo
 locale/nl/LC_MESSAGES/pronterface.po
 printrun/__init__.py
 printrun/eventhandler.py
 printrun/excluder.py
 printrun/gcodeplater.py
 printrun/gcoder.py
 printrun/gcoder_line.pyx
```

### Comparing `Printrun-2.0.0rc7/README.cleanup` & `Printrun-2.0.1/README.cleanup`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 To add spaces around each ==:
 sed -e "s/\(\w\)==\(\w\)/\1 == \2/g" -i *.py printrun/*.py printrun/*/*.py
 sed -e "s/\(\w\)==\(\"\)/\1 == \2/g" -i *.py printrun/*.py printrun/*/*.py
 sed -e "s/\(\w\)==\((\)/\1 == \2/g" -i *.py printrun/*.py printrun/*/*.py
 sed -e "s/\()\)==\(\w\)/\1 == \2/g" -i *.py printrun/*.py printrun/*/*.py
 sed -e "s/\()\)==\((\)/\1 == \2/g" -i *.py printrun/*.py printrun/*/*.py
 
-Obviously this is not a perfect solution, it WILL break the code. Juste check the diff and fix what's wrong before commiting.
+Obviously this is not a perfect solution, it WILL break the code. Juste check the diff and fix what's wrong before committing.
 
 Flake8 checking:
 Flake8 can be used to check the coding style of the project.
 The current source code (as of July 23rd 2013) has been checked using the following command:
     flake8 . --statistics --count --ignore=E251,E701,E302,E501 --exclude=.svn,CVS,.bzr,.hg,.git,__pycache__,./printrun/cairosvg
 This call ignores 4 kind of errors (E501: line being greater than 80 chars,
 E701: multiple statements on one line (usually this is if ...: ...), E302:
```

### Comparing `Printrun-2.0.0rc7/README.i18n` & `Printrun-2.0.1/README.i18n`

 * *Files 12% similar despite different names*

```diff
@@ -8,25 +8,27 @@
 
 The pronterface.py now uses gettext for the messages it generates.
 The corresponding pronterface.pot file is at locale/pronterface.pot
 and was generated using 
 
   pygettext -o locale/pronterface.pot *.py printrun/*.py printrun/*/*.py
 
+on some systems you have to replace the pygettext with pygettext2 or pygettext3..
+
 followed by minor edits to the generated header.
 
-This template is the basis for all pronterface mesage catalogs.  Right
+This template is the basis for all pronterface message catalogs.  Right
 now there is only one, for German.  New ones can be created:
 
   # Create new pronterface message catalog for a different language
   newlang="es"  # use the correct code for your language
   mkdir -p locale/${newlang}/LC_MESSAGES
   cp locale/pronterface.pot locale/${newlanguage}/LC_MESSAGES/pronterface.po
   cd locale/${newlanguage}/LC_MESSAGES/
-  # Edit the .po file to add messages for newlang
+  # Edit the .po file to add messages for newlang (debian offers e.g.: poedit or gtranslator)
   msgfmt -o pronterface.mo pronterface.po
 
 To update a previously created message catalog from the template, use :
 
   msgmerge -U locale/fr/LC_MESSAGES/pronterface.po locale/pronterface.pot
 
 As currently coded, the default location for these message catalogs is
```

### Comparing `Printrun-2.0.0rc7/README.md` & `Printrun-2.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,88 @@
+Metadata-Version: 2.1
+Name: Printrun
+Version: 2.0.1
+Summary: Host software for 3D printers
+Home-page: http://github.com/kliment/Printrun/
+Author: Kliment Yanev, Guillaume Seguin and others
+License: GPLv3+
+Classifier: Environment :: X11 Applications :: GTK
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Manufacturing
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Printing
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: COPYING
+
 # PRINTRUN 2.X
 
-The master branch holds the development of Printrun 2.x. This new version of Printrun supports Python 3 and wxPython 4. All new features and developments should be merged to it.
+The master branch holds the development of Printrun 2.x. This version of Printrun supports Python 3 and wxPython 4. All new features and developments should be merged to it.
 
 Printrun consists of printcore, pronsole and pronterface, and a small collection of helpful scripts.
 
   * printcore.py is a library that makes writing reprap hosts easy
   * pronsole.py is an interactive command-line host software with tabcompletion goodness
   * pronterface.py is a graphical host software with the same functionality as pronsole
 
-# GETTING PRINTRUN
+# CONTRIBUTORS
+
+An enormous number of people helped make Printrun. See the list
+[here](CONTRIBUTORS.md).
 
-This section suggests using precompiled binaries, this way you get everything bundled into one single package for an easy installation.
+# GETTING PRINTRUN
 
-If you want the newest, shiniest features, you can run Printrun from source using the instructions further down this README.
+This section suggests using precompiled binaries, this way you get everything
+bundled into one single package for an easy installation. If you want the
+newest, shiniest features, you can [run Printrun from
+source](#running-from-source).
 
 ## Windows
 
-A precompiled version is available at http://koti.kapsi.fi/~kliment/printrun/
+A precompiled version is available at https://github.com/kliment/Printrun/releases
 
-## Mac OS X
+## MacOS
 
-A precompiled version is available at http://koti.kapsi.fi/~kliment/printrun/
+A precompiled version is available at https://github.com/kliment/Printrun/releases
 
-Note for OSX users: if OSX tells you the file is corrupted, you don't need to redownload it. Instead, you need to allow OSX to run unsigned apps. To do this, run 
-`sudo spctl --master-disable`
+Note for OSX users: if OSX tells you `"pronterface.app" cannot be opened because the developer cannot be verified.`, you don't need to redownload it. Instead, you need to allow OSX to run the unsigned app. To do this, right click the application in Finder and select `Open`. Then click `Open` in the popup window that appears. You only need to do this once.
 
 
 ## Linux
 ### Ubuntu/Debian
 
-There is currently no package for Printrun 2. It must be [run from source](https://github.com/kliment/Printrun/tree/master#running-from-source).
+You can install Printrun from official packages. Install the whole package
+using:
+
+```
+sudo apt update
+sudo apt install printrun
+```
+
+Or get only apps you need by
+
+`sudo apt install pronsole` or `pronterface` or `plater`
 
-### Chrome OS 
+### Chrome OS
 
 You can use Printrun via crouton ( https://github.com/dnschneid/crouton ). Assuming you want Ubuntu Trusty, you used probably `sudo sh -e ~/Downloads/crouton -r trusty -t xfce` to install Ubuntu. Fetch and install printrun with the line given above for Ubuntu/Debian.
 
 By default you have no access to the serial port under Chrome OS crouton, so you cannot connect to your 3D printer. Add yourself to the serial group within the linux environment to fix this
 
-`sudo usermod -G serial -a <username>` 
+`sudo usermod -G serial -a <username>`
 
-where `<username>` should be your username. Log out and in to make this group change active and allow communication with your printer. 
+where `<username>` should be your username. Log out and in to make this group change active and allow communication with your printer.
 
 ### Fedora
 
 You can install Printrun from official packages. Install the whole package using
 
 `sudo dnf install printrun`
 
@@ -66,42 +105,42 @@
 
 Run Printrun for source if you want to test out the latest features.
 
 ### Dependencies
 
 To use pronterface, you need:
 
-  * Python 3 (ideally 3.6),
+  * Python 3 (ideally 3.10),
   * pyserial (or python3-serial on ubuntu/debian)
   * pyreadline (not needed on Linux)
   * wxPython 4
   * pyglet
   * appdirs
   * numpy (for 3D view)
   * pycairo (to use Projector feature)
   * cairosvg (to use Projector feature)
-  * dbus (to inhibit sleep on some Linux systems) 
+  * dbus (to inhibit sleep on some Linux systems)
 
 ### Use Python virtual environment
 
 Easiest way to run Printrun from source is to create and use a Python [virtual environment](https://docs.python.org/3/tutorial/venv.html).
-The following section assumes Linux. Please see specific instructions for Windows and macOS X below.
+The following section assumes Linux. Please see specific instructions for Windows and macOS below.
 
 **Ubuntu/Debian note:** You might need to install `python3-venv` first.
 
-**Note:** wxPython4 doesn't have Linux wheels available from the Python Package Index yet. Find a proper wheel for your distro at [extras.wxpython.org](https://extras.wxpython.org/wxPython4/extras/linux/gtk3/) and substitute the link in the bellow example. You might skip the wheel installation, but that results in compiling wxPython4 from source, which can be time and resource consuming and might fail.
+**Note:** wxPython4 doesn't have Linux wheels available from the Python Package Index yet. Find a proper wheel for your distro at [extras.wxpython.org](https://extras.wxpython.org/wxPython4/extras/linux/gtk3/) and substitute the link in the below example. You might skip the wheel installation, but that results in compiling wxPython4 from source, which can be time and resource consuming and might fail.
 
 
 ```console
 $ git clone https://github.com/kliment/Printrun.git  # clone the repository
 $ cd Printrun  # change to Printrun directory
 $ python3 -m venv venv  # create an virtual environment
 $ . venv/bin/activate  # activate the virtual environment (notice the space after the dot)
 (venv) $ python -m pip install https://extras.wxpython.org/wxPython4/extras/linux/gtk3/fedora-27/wxPython-4.0.1-cp36-cp36m-linux_x86_64.whl  # replace the link with yours
-(venv) $ python -m pip install -r requirements.txt  # intall the rest of dependencies
+(venv) $ python -m pip install -r requirements.txt  # install the rest of dependencies
 (venv) $ python pronterface.py  # run Pronterface
 ```
 
 ### Cython-based G-Code parser
 
 Printrun default G-Code parser is quite memory hungry, but we also provide a much lighter one which just needs an extra build-time dependency (Cython), plus compiling the extension with:
 
@@ -136,32 +175,59 @@
 sudo apt install git
 git clone https://github.com/kliment/Printrun.git
 cd Printrun
 ```
 
 ### Windows
 
-Download and install [Python 3.6](https://www.python.org/downloads/) and follow the **Python virtual environment** section above except use the following to create and activate the virtual environment and install dependencies:
+First download and install [GIT for Windows](https://git-scm.com/downloads), [Python 3.10](https://www.python.org/downloads/) and a [C-compiler environment](https://wiki.python.org/moin/WindowsCompilers/).
+For the next steps we need a CMD window or a PowerShell window. You can use Windows Terminal for this as well.
+Create and navigate to a directory of your choice where you want to download the source files of this repository and follow the next steps:
 
+CMD
 ```cmd
-> py -3 -m venv venv
-> venv\Scripts\activate
-> python -m pip install -r requirements.txt
+> git clone https://github.com/kliment/Printrun.git
+> cd Printrun
+> git submodule update --init --recursive
+> release_windows.bat
+```
+
+PowerShell:
+```ps
+> git clone https://github.com/kliment/Printrun.git
+> cd Printrun
+> git submodule update --init --recursive
+> ./release_windows.bat
 ```
 
+The script above will clone this repository and the submodule PrintrunGTK3. The script 'release_windows.bat' will install a virtual environment named v3, download all needed python libraries and compile the binaries for Pronterface.exe and Pronsole.exe.
+You will find the files in the new created directory 'dist'. You will find further and more detailed information in the script release_windows.bat. Further information for the linked submodul: [PrintrunGTK3](https://github.com/DivingDuck/PrintrunGTK3)
+Run Pronterface or Pronsole from the binary files or from source calling pronterface.py for the GUI version and pronsole.py for the commandline version.
 
-### macOS X
+Run 'release_windows.bat' when ever you make changes or updates. With each new run it will compile the binaries and update all involved libraries in the virtual environment if needed. Delete the virtual environment if you have problems with it. Use 'git submodule update --init --recursive' for updating the submodule
+
+### macOS
 
 Install Python 3, you can use Brew:
 
 ```console
 $ brew install python3
 ```
 
-And follow the above **Python virtual environment** section. You don't need to search for wxPython wheel, macOS wheels are available from the Python Package Index.
+Then continue to install and set up Printrun:
+
+```console
+$ git clone https://github.com/kliment/Printrun.git  # clone the repository
+$ cd Printrun  # change to Printrun directory
+$ python3 -m venv venv  # create an virtual environment
+$ . venv/bin/activate  # activate the virtual environment (notice the space after the dot)
+(venv) $ python -m pip install -r requirements.txt  # install the rest of dependencies
+# follow instructions for cython gcoder here if desired
+(venv) $ python pronterface.py  # run Pronterface
+```
 
 
 # USING PRINTRUN
 
 ## USING PRONTERFACE
 
 When you're done setting up Printrun, you can start pronterface.py in the directory you unpacked it.
@@ -178,37 +244,43 @@
 
 If the Slic3r integration option (_Settings_ > _Options_ > _User interface_ > _Enable Slic3r integration_) is checked a new menu will appear after application restart which will allow you to choose among your previously saved Slic3r Print/Filament/Printer settings.
 
 ## USING PRONSOLE
 
 To use pronsole, you need:
 
-  * Python 3 (ideally 3.6),
+  * Python 3 (ideally 3.10),
   * pyserial (or python3-serial on ubuntu/debian) and
   * pyreadline (not needed on Linux)
 
 Start pronsole and you will be greeted with a command prompt. Type help to view the available commands.
 All commands have internal help, which you can access by typing "help commandname", for example "help connect"
 
 If you want to load stl files, you need to put a version of skeinforge (doesn't matter which one) in a folder called "skeinforge".
 The "skeinforge" folder must be in the same folder as pronsole.py
 
 ## USING PRINTCORE
 
-To use printcore you need Python 3 (ideally 3.6) and pyserial (or python3-serial on ubuntu/debian)
+To use printcore you need Python 3 (ideally 3.10) and pyserial (or python3-serial on ubuntu/debian)
 See pronsole for an example of a full-featured host, the bottom of printcore.py for a simple command-line
 sender, or the following code example:
 
 ```python
 #to send a file of gcode to the printer
 from printrun.printcore import printcore
 from printrun import gcoder
-p=printcore('/dev/ttyUSB0',115200) # or p.printcore('COM3',115200) on Windows
+import time
+p=printcore('/dev/ttyUSB0', 115200) # or p.printcore('COM3',115200) on Windows
 gcode=[i.strip() for i in open('filename.gcode')] # or pass in your own array of gcode lines instead of reading from a file
 gcode = gcoder.LightGCode(gcode)
+
+# startprint silently exits if not connected yet
+while not p.online:
+  time.sleep(0.1)
+
 p.startprint(gcode) # this will start a print
 
 #If you need to interact with the printer:
 p.send_now("M105") # this will send M105 immediately, ahead of the rest of the print
 p.pause() # use these to pause/resume the current print
 p.resume()
 p.disconnect() # this is how you disconnect from the printer once you are done. This will also stop running prints.
@@ -389,34 +461,34 @@
 !else:
   !self.p.loud = 1
   !print("Diagnostic information ON")
 ```
 
 Macro parameters are available in '!'-escaped python code as locally defined list variable: arg[0] arg[1] ... arg[N]
 
-All python code is executed in the context of the pronsole (or PronterWindow) object, 
+All python code is executed in the context of the pronsole (or PronterWindow) object,
 so it is possible to use all internal variables and methods, which provide great deal of functionality.
 However the internal variables and methods are not very well documented and may be subject of change, as the program is developed.
 Therefore it is best to use pronsole commands, which easily contain majority of the functionality that might be needed.
 
 Some useful python-mode-only variables:
 
 ```python
-!self.settings - contains all settings, e.g. 
+!self.settings - contains all settings, e.g.
   port (!self.settings.port), baudrate, xy_feedrate, e_feedrate, slicecommand, final_command, build_dimensions
   You can set them also via pronsole command "set", but you can query the values only via python code.
 !self.p - printcore object (see USING PRINTCORE section for using printcore object)
 !self.cur_button - if macro was invoked via custom button, the number of the custom button, e.g. for usage in "button" command
 !self.gwindow - wx graphical interface object for pronterface (highly risky to use because the GUI implementation details may change a lot between versions)
 ```
 
 Some useful methods:
 
 ```python
-!self.onecmd - invokes raw command, e.g. 
+!self.onecmd - invokes raw command, e.g.
     !self.onecmd("move x 10")
     !self.onecmd("!print self.p.loud")
     !self.onecmd("button "+self.cur_button+" fanOFF /C cyan M107")
 !self.project - invoke Projector
 ```
 
 ## USING HOST COMMANDS
@@ -463,15 +535,15 @@
 - `home [axis]`
 - `off`: turns off fans, motors, extruder, heatbed, power supply
 - `exit`
 
 # LICENSE
 
 ```
-Copyright (C) 2011-2020 Kliment Yanev, Guillaume Seguin
+Copyright (C) 2011-2022 Kliment Yanev, Guillaume Seguin, and the other contributors listed in CONTRIBUTORS.md
 
 Printrun is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 Printrun is distributed in the hope that it will be useful,
@@ -480,8 +552,7 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with Printrun.  If not, see <http://www.gnu.org/licenses/>.
 ```
 
 All scripts should contain this license note, if not, feel free to ask us. Please note that files where it is difficult to state this license note (such as images) are distributed under the same terms.
-
```

### Comparing `Printrun-2.0.0rc7/images/arrow_down.png` & `Printrun-2.0.1/images/arrow_down.png`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/images/arrow_keys.png` & `Printrun-2.0.1/images/arrow_keys.png`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/images/arrow_up.png` & `Printrun-2.0.1/images/arrow_up.png`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/images/control_mini.png` & `Printrun-2.0.1/images/control_mini.png`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/images/control_mini.svg` & `Printrun-2.0.1/images/control_mini.svg`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/images/control_xy.png` & `Printrun-2.0.1/images/control_xy.png`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/images/control_xy.svg` & `Printrun-2.0.1/images/control_xy.svg`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/images/control_z.png` & `Printrun-2.0.1/images/control_z.png`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/images/control_z.svg` & `Printrun-2.0.1/images/control_z.svg`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/images/control_z_mini.png` & `Printrun-2.0.1/images/control_z_mini.png`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/images/control_z_mini.svg` & `Printrun-2.0.1/images/control_z_mini.svg`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/images/edit.png` & `Printrun-2.0.1/images/edit.png`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/images/fit.png` & `Printrun-2.0.1/images/fit.png`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/images/inject.png` & `Printrun-2.0.1/images/inject.png`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/images/reset.png` & `Printrun-2.0.1/images/reset.png`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/images/zoom_in.png` & `Printrun-2.0.1/images/zoom_in.png`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/images/zoom_out.png` & `Printrun-2.0.1/images/zoom_out.png`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/locale/ar/LC_MESSAGES/plater.po` & `Printrun-2.0.1/locale/ar/LC_MESSAGES/plater.po`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/locale/de/LC_MESSAGES/plater.po` & `Printrun-2.0.1/locale/fr/LC_MESSAGES/plater.po`

 * *Files 17% similar despite different names*

```diff
@@ -1,89 +1,95 @@
+# French Plater Message Catalog
+# Copyright (C) 2012 Guillaume Seguin
+# Guillaume Seguin <guillaume@segu.in>, 2012.
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: Plater\n"
-"POT-Creation-Date: 2012-01-09 15:07+CET\n"
-"PO-Revision-Date: \n"
-"Last-Translator: Christian Metzen <metzench@ccux-linux.de>\n"
-"Language-Team:  <LL@li.org>\n"
+"POT-Creation-Date: 2012-08-04 21:53+CEST\n"
+"PO-Revision-Date: 2012-02-26 02:41+0100\n"
+"Last-Translator: Guillaume Seguin <guillaume@segu.in>\n"
+"Language-Team: FR <guillaume@segu.in>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Poedit-Language: German\n"
-"X-Poedit-Country: GERMANY\n"
+"Generated-By: pygettext.py 1.5\n"
 
-#: plater.py:223
+#: plater.py:246
 msgid "Plate building tool"
-msgstr "Plate building tool"
+msgstr "Outil d'assemblage de plateau"
 
-#: plater.py:229
+#: plater.py:252
 msgid "Clear"
-msgstr "Löschen"
+msgstr "Vider"
 
-#: plater.py:230
+#: plater.py:253
 msgid "Load"
-msgstr "Laden"
+msgstr "Charger"
 
-#: plater.py:232
+#: plater.py:255 plater.py:258
 msgid "Export"
-msgstr "Exportieren"
+msgstr "Exporter"
 
-#: plater.py:235
+#: plater.py:260
 msgid "Done"
-msgstr "Fertig"
+msgstr "Terminé"
 
-#: plater.py:237
+#: plater.py:262
 msgid "Cancel"
-msgstr "Abbrechen"
+msgstr "Annuler"
 
-#: plater.py:239
+#: plater.py:264
 msgid "Snap to Z = 0"
-msgstr "Einrasten auf Z = 0"
+msgstr "Poser en Z = 0"
 
-#: plater.py:240
+#: plater.py:265
 msgid "Put at 100, 100"
-msgstr "Auf 100, 100 setzen"
+msgstr "Placer en 100, 100"
 
-#: plater.py:241
+#: plater.py:266
 msgid "Delete"
-msgstr "Löschen"
+msgstr "Supprimer"
 
-#: plater.py:242
+#: plater.py:267
 msgid "Auto"
 msgstr "Auto"
 
-#: plater.py:266
+#: plater.py:291
 msgid "Autoplating"
-msgstr "Autoplating"
+msgstr "Placement auto"
 
-#: plater.py:294
+#: plater.py:319
 msgid "Bed full, sorry sir :("
-msgstr "Das Druckbett ist voll! Sorry."
+msgstr "Le lit est plein, désolé :("
 
-#: plater.py:304
-msgid "Are you sure you want to clear the grid? All unsaved changes will be lost."
-msgstr "Bist du sicher dass du das Raster leeren willst? Alle ungesicherten Änderungen gehen verloren."
+#: plater.py:329
+msgid ""
+"Are you sure you want to clear the grid? All unsaved changes will be lost."
+msgstr ""
+"Êtes vous sur de vouloir vider la grille ? Toutes les modifications non "
+"enregistrées seront perdues."
 
-#: plater.py:304
+#: plater.py:329
 msgid "Clear the grid?"
-msgstr "Raster leeren?"
+msgstr "Vider la grille ?"
 
-#: plater.py:346
+#: plater.py:371
 msgid "Pick file to save to"
-msgstr "Wähle die zu sichernde Datei"
+msgstr "Choisir le fichier dans lequel enregistrer"
 
-#: plater.py:347
-msgid "STL files (;*.stl;)"
-msgstr "STL Dateien (;*.stl;)"
+#: plater.py:372
+msgid "STL files (;*.stl;*.STL;)"
+msgstr "Fichiers STL (;*.stl;*.STL;)"
 
-#: plater.py:367
-msgid "wrote "
-msgstr "geschrieben"
+#: plater.py:393
+msgid "wrote %s"
+msgstr "%s écrit"
 
-#: plater.py:370
+#: plater.py:396
 msgid "Pick file to load"
-msgstr "Wähle die zu ladende Datei"
-
-#: plater.py:371
-msgid "STL files (;*.stl;)|*.stl|OpenSCAD files (;*.scad;)|*.scad"
-msgstr "STL Dateien (;*.stl;)|*.stl|OpenSCAD Dateien (;*.scad;)|*.scad"
+msgstr "Choisir le fichier à charger"
 
+#: plater.py:397
+msgid "STL files (;*.stl;*.STL;)|*.stl|OpenSCAD files (;*.scad;)|*.scad"
+msgstr "Fichiers STL (;*.stl;*.STL;)|*.stl|Fichiers OpenSCAD (;*.scad;)|*.scad"
```

### Comparing `Printrun-2.0.0rc7/locale/de/LC_MESSAGES/pronterface.po` & `Printrun-2.0.1/locale/nl/LC_MESSAGES/pronterface.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Pronterface
-# Copyright (C) 2011 Jonathan Marsden
-# Jonathan Marsden <jmarsden@fastmail.fm>, 2011.
+# Pronterface Message Catalog Dutch
+# Copyright (C) 2011 Ruben Lubbes
+# Ruben Lubbes <ruben.lubbes@gmx.net>, 2011.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: Pronterface jm1\n"
+"Project-Id-Version: Pronterface rl1\n"
 "POT-Creation-Date: 2014-03-30 14:35+CEST\n"
-"PO-Revision-Date: 2012-01-23 10:01+0100\n"
-"Last-Translator: Christian Metzen <metzench@ccux-linux.de>\n"
-"Language-Team: DE <LL@li.org>\n"
+"PO-Revision-Date: 2011-09-06 16:31+0100\n"
+"Last-Translator: Ruben Lubbes <ruben.lubbes@gmx.net>\n"
+"Language-Team: NL <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
 
 #: printrun/excluder.py:26
@@ -42,65 +42,63 @@
 
 #: printrun/gcview.py:353
 msgid "Fit to plate [F]"
 msgstr ""
 
 #: printrun/gui/__init__.py:19 printrun/pronterface.py:45
 msgid "WX is not installed. This program requires WX to run."
-msgstr "WX ist nicht installiert. Dieses Programm erfordert WX zum Starten."
+msgstr "WX is niet geïnstalleerd. Dit programma vereist WX."
 
 #: printrun/gui/__init__.py:159
 #, fuzzy
 msgid "Commands"
-msgstr "Kommando"
+msgstr "Commando"
 
 #: printrun/gui/__init__.py:160
 msgid "Status"
 msgstr ""
 
 #: printrun/gui/controls.py:126
 #, fuzzy
 msgid "Heat:"
-msgstr "Heizelement:"
+msgstr "Element:"
 
 #: printrun/gui/controls.py:129
 msgid "Switch Hotend Off"
 msgstr ""
 
 #: printrun/gui/controls.py:129 printrun/gui/controls.py:149
 #: printrun/gui/toolbar.py:85
 msgid "Off"
-msgstr "Aus"
+msgstr ""
 
 #: printrun/gui/controls.py:137
-#, fuzzy
 msgid "Select Temperature for Hotend"
-msgstr "Letzte Hotend Temperatur"
+msgstr ""
 
 #: printrun/gui/controls.py:141
 msgid "Switch Hotend On"
 msgstr ""
 
 #: printrun/gui/controls.py:141 printrun/gui/controls.py:161
 #: printrun/gui/controls.py:198
 msgid "Set"
-msgstr "Ein"
+msgstr "Stel in"
 
 #: printrun/gui/controls.py:146 printrun/gui/controls.py:215
 msgid "Bed:"
-msgstr "Heizbett:"
+msgstr "Bed:"
 
 #: printrun/gui/controls.py:149
 msgid "Switch Heated Bed Off"
 msgstr ""
 
 #: printrun/gui/controls.py:157
-#, fuzzy
 msgid "Select Temperature for Heated Bed"
-msgstr "Letzte gesetzte Temperatur für das Heizbett"
+msgstr ""
 
 #: printrun/gui/controls.py:161
 msgid "Switch Heated Bed On"
 msgstr ""
 
 #: printrun/gui/controls.py:187
 msgid "Print speed:"
@@ -112,15 +110,15 @@
 
 #: printrun/gui/controls.py:198
 msgid "Set print speed factor"
 msgstr ""
 
 #: printrun/gui/controls.py:213
 msgid "Heater:"
-msgstr "Heizelement:"
+msgstr "Element:"
 
 #: printrun/gui/controls.py:265
 msgid "Length:"
 msgstr ""
 
 #: printrun/gui/controls.py:267
 msgid "mm"
@@ -186,20 +184,20 @@
 "Send commands to printer\n"
 "(Type 'help' for simple\n"
 "help function)"
 msgstr ""
 
 #: printrun/gui/log.py:39
 msgid "Send"
-msgstr "Senden"
+msgstr "Zend"
 
 #: printrun/gui/log.py:39
 #, fuzzy
 msgid "Send Command to Printer"
-msgstr "Drucker überwachen"
+msgstr "Printercommunicatie volgen"
 
 #: printrun/gui/toolbar.py:23
 msgid "Lock"
 msgstr ""
 
 #: printrun/gui/toolbar.py:25
 msgid "Lock graphical interface"
@@ -209,79 +207,79 @@
 msgid ""
 "Communication Settings\n"
 "Click to rescan ports"
 msgstr ""
 
 #: printrun/gui/toolbar.py:32
 msgid "Port"
-msgstr "Port:"
+msgstr "Poort"
 
 #: printrun/gui/toolbar.py:37
 msgid "Select Port Printer is connected to"
 msgstr ""
 
 #: printrun/gui/toolbar.py:46
 msgid "Select Baud rate for printer communication"
 msgstr ""
 
 #: printrun/gui/toolbar.py:55 printrun/pronterface.py:1052
 msgid "Connect"
-msgstr "Verbinden"
+msgstr "Verbind"
 
 #: printrun/gui/toolbar.py:55 printrun/pronterface.py:1053
 msgid "Connect to the printer"
-msgstr "Drucker Verbinden"
+msgstr "Verbind met printer"
 
 #: printrun/gui/toolbar.py:61
 msgid "Reset"
-msgstr "Zurücksetzen"
+msgstr "Reset"
 
 #: printrun/gui/toolbar.py:61
 #, fuzzy
 msgid "Reset the printer"
-msgstr "Drucker Verbinden"
+msgstr "Verbind met printer"
 
 #: printrun/gui/toolbar.py:69
 #, fuzzy
 msgid "Load a 3D model file"
-msgstr "Datei laden"
+msgstr "open bestand"
 
 #: printrun/gui/toolbar.py:69
 msgid "Load file"
-msgstr "Datei laden"
+msgstr "open bestand"
 
 #: printrun/gui/toolbar.py:70
 msgid "SD"
-msgstr "SD"
+msgstr ""
 
 #: printrun/gui/toolbar.py:70
 #, fuzzy
 msgid "SD Card Printing"
-msgstr "SD Drucken"
+msgstr "Afdruk van SD"
 
 #: printrun/gui/toolbar.py:74
 msgid "Start Printing Loaded File"
 msgstr ""
 
 #: printrun/gui/toolbar.py:74 printrun/pronterface.py:1003
 #: printrun/pronterface.py:1062 printrun/pronterface.py:1078
 #: printrun/pronterface.py:1363 printrun/pronterface.py:1445
 msgid "Print"
-msgstr "Drucken"
+msgstr "Printen"
 
 #: printrun/gui/toolbar.py:80
 msgid "Pause Current Print"
 msgstr ""
 
 #: printrun/gui/toolbar.py:80 printrun/pronterface.py:1002
 #: printrun/pronterface.py:1061 printrun/pronterface.py:1081
 #: printrun/pronterface.py:1091 printrun/pronterface.py:1172
 #: printrun/pronterface.py:1364
 msgid "Pause"
-msgstr "Pause"
+msgstr "Pauze"
 
 #: printrun/gui/toolbar.py:85
 msgid "Turn printer off"
 msgstr ""
 
 #: printrun/gui/viz.py:65
 msgid ""
@@ -291,70 +289,69 @@
 
 #: printrun/gui/widgets.py:36
 msgid "Find"
 msgstr ""
 
 #: printrun/gui/widgets.py:38
 msgid "Save"
-msgstr "Speichern"
+msgstr ""
 
 #: printrun/gui/widgets.py:43 printrun/objectplater.py:76
 #: printrun/pronterface.py:1257 printrun/pronterface.py:2017
 msgid "Cancel"
-msgstr "Abbrechen"
+msgstr "Annuleer"
 
 #: printrun/gui/widgets.py:70
 #, fuzzy
 msgid "Not Found!"
-msgstr "Datei nicht gefunden!"
+msgstr "Bestand niet gevonden!"
 
 #: printrun/gui/widgets.py:124
 #, fuzzy
 msgid "Printer settings"
-msgstr "Einstellungen bearbeiten"
+msgstr "Wijzig instellingen"
 
 #: printrun/gui/widgets.py:125
 #, fuzzy
 msgid "User interface"
 msgstr "Printer Interface"
 
 #: printrun/gui/widgets.py:126
 #, fuzzy
 msgid "Colors"
-msgstr "Farbe"
+msgstr "Kleur"
 
 #: printrun/gui/widgets.py:127
-#, fuzzy
 msgid "External commands"
-msgstr "Kommando ausführen:"
+msgstr ""
 
 #: printrun/gui/widgets.py:132
 msgid "Edit settings"
-msgstr "Einstellungen bearbeiten"
+msgstr "Wijzig instellingen"
 
 #: printrun/gui/widgets.py:135
 #, fuzzy
 msgid "Settings"
-msgstr "&Einstellungen"
+msgstr "&Instellingen"
 
 #: printrun/gui/widgets.py:187
 msgid "Custom button"
-msgstr "Individueller Button"
+msgstr "Gedefinieerde knop"
 
 #: printrun/gui/widgets.py:193
 msgid "Button title"
-msgstr "Button Titel"
+msgstr "Knoptitel"
 
 #: printrun/gui/widgets.py:196
 msgid "Command"
-msgstr "Kommando"
+msgstr "Commando"
 
 #: printrun/gui/widgets.py:205
 msgid "Color"
-msgstr "Farbe"
+msgstr "Kleur"
 
 #: printrun/gviz.py:29
 msgid "Layer number and Z position show here when you scroll"
 msgstr ""
 
 #: printrun/gviz.py:39
 msgid "Zoom In [+]"
@@ -371,15 +368,15 @@
 #: printrun/gviz.py:43
 msgid "Move Down a Layer [D]"
 msgstr ""
 
 #: printrun/gviz.py:44
 #, fuzzy
 msgid "Reset view"
-msgstr "Zurücksetzen"
+msgstr "Reset"
 
 #: printrun/gviz.py:68
 msgid "Gcode view, shift to move view, mousewheel to set layer"
 msgstr ""
 
 #: printrun/gviz.py:105 printrun/gviz.py:241
 msgid "Layer %d - Going Up - Z = %.03f mm"
@@ -438,47 +435,47 @@
 msgid ""
 "Are you sure you want to clear the grid? All unsaved changes will be lost."
 msgstr ""
 
 #: printrun/objectplater.py:210
 #, fuzzy
 msgid "Clear the grid?"
-msgstr " Schliesst das Fenster"
+msgstr " Sluit het venster"
 
 #: printrun/objectplater.py:256
 #, fuzzy
 msgid "Pick file to load"
-msgstr "Wähle SD Datei"
+msgstr "Kies bestand op SD"
 
 #: printrun/objectplater.py:267
 #, fuzzy
 msgid "Pick file to save to"
-msgstr "Wähle SD Dateiname"
+msgstr "Kies bestandsnaam op SD"
 
 #: printrun/plater.py:212
 msgid "STL files (*.stl;*.STL)|*.stl;*.STL|OpenSCAD files (*.scad)|*.scad"
 msgstr ""
 
 #: printrun/plater.py:213
 msgid "STL files (*.stl;*.STL)|*.stl;*.STL"
 msgstr ""
 
 #: printrun/plater.py:244
 #, fuzzy
 msgid "Loading STL file failed"
-msgstr "Datei öffnen fehlgeschlagen."
+msgstr "Bestand openen mislukt"
 
 #: printrun/plater.py:244 printrun/plater.py:251
 msgid "Error"
 msgstr ""
 
 #: printrun/plater.py:251
 #, fuzzy
 msgid "Loading OpenSCAD file failed"
-msgstr "Datei öffnen fehlgeschlagen."
+msgstr "Bestand openen mislukt"
 
 #: printrun/plater.py:284
 msgid "Couldn't load non-existing file %s"
 msgstr ""
 
 #: printrun/plater.py:360
 msgid "Wrote plate to %s"
@@ -546,15 +543,15 @@
 msgstr ""
 
 #: printrun/printcore.py:462 printrun/printcore.py:470
 #: printrun/pronsole.py:1192 printrun/pronsole.py:1250
 #: printrun/pronterface.py:209 printrun/pronterface.py:962
 #: printrun/pronterface.py:1111 printrun/pronterface.py:1178
 msgid "Not connected to printer."
-msgstr "Keine Verbindung zum Drucker."
+msgstr "Printer is niet verbonden."
 
 #: printrun/printcore.py:479
 msgid "Print start callback failed with:"
 msgstr ""
 
 #: printrun/printcore.py:490
 msgid "Print end callback failed with:"
@@ -583,25 +580,25 @@
 #: printrun/printcore.py:610
 msgid "Socket connection broken, disconnected. ({0}): {1}"
 msgstr ""
 
 #: printrun/pronsole.py:72
 #, fuzzy
 msgid "Default: "
-msgstr "Standardwerte"
+msgstr "Standaardinstelling"
 
 #: printrun/pronsole.py:73
 msgid "(Control-doubleclick to reset to default value)"
 msgstr ""
 
 #: printrun/pronsole.py:108
 #, fuzzy
 msgid ""
 "Are you sure you want to reset the setting to the default value: {0!r} ?"
-msgstr "Möchten Sie den Drucker wirklich zurücksetzen?"
+msgstr "Weet je zeker dat je de printer wilt resetten?"
 
 #: printrun/pronsole.py:108
 msgid "Confirm set default"
 msgstr ""
 
 #: printrun/pronsole.py:258
 msgid "Width"
@@ -636,29 +633,29 @@
 msgstr ""
 
 #: printrun/pronsole.py:282
 msgid "Z home pos."
 msgstr ""
 
 #: printrun/pronsole.py:301
+#, fuzzy
 msgid "Port used to communicate with printer"
-msgstr "Port für Druckerkommunikation"
+msgstr "Printer is niet verbonden."
 
 #: printrun/pronsole.py:301
 msgid "Serial port"
 msgstr ""
 
 #: printrun/pronsole.py:302
 msgid "Baud rate"
 msgstr ""
 
 #: printrun/pronsole.py:302
-#, fuzzy
 msgid "Communications Speed"
-msgstr "Kommunikationsgeschwindigkeit (Vorgabe: 115200)"
+msgstr ""
 
 #: printrun/pronsole.py:303
 msgid "TCP streaming mode"
 msgstr ""
 
 #: printrun/pronsole.py:303
 msgid ""
@@ -668,147 +665,130 @@
 msgstr ""
 
 #: printrun/pronsole.py:304
 msgid "Bed temperature for ABS"
 msgstr ""
 
 #: printrun/pronsole.py:304
-#, fuzzy
 msgid "Heated Build Platform temp for ABS (deg C)"
-msgstr "Heizbett Temp. für ABS (Vorgabe: 110 Grad Celsius)"
+msgstr ""
 
 #: printrun/pronsole.py:305
 msgid "Bed temperature for PLA"
 msgstr ""
 
 #: printrun/pronsole.py:305
-#, fuzzy
 msgid "Heated Build Platform temp for PLA (deg C)"
-msgstr "Heizbett Temp. für PLA (Vorgabe: 60 Grad Celsius)"
+msgstr ""
 
 #: printrun/pronsole.py:306
-#, fuzzy
 msgid "Extruder temp for ABS (deg C)"
-msgstr "Extruder Temperatur für ABS (Vorgabe: 230 Grad Celsius)"
+msgstr ""
 
 #: printrun/pronsole.py:306
-#, fuzzy
 msgid "Extruder temperature for ABS"
-msgstr "Extruder Temperatur für ABS (Vorgabe: 230 Grad Celsius)"
+msgstr ""
 
 #: printrun/pronsole.py:307
-#, fuzzy
 msgid "Extruder temp for PLA (deg C)"
-msgstr "Extruder Temperatur für PLA (Vorgabe: 185 Grad Celsius)"
+msgstr ""
 
 #: printrun/pronsole.py:307
-#, fuzzy
 msgid "Extruder temperature for PLA"
-msgstr "Extruder Temperatur für PLA (Vorgabe: 185 Grad Celsius)"
+msgstr ""
 
 #: printrun/pronsole.py:308
-#, fuzzy
 msgid "Feedrate for Control Panel Moves in X and Y (mm/min)"
-msgstr "Vorschub Control Panel Bewegungen X und Y (Vorgabe: 3000mm/min)"
+msgstr ""
 
 #: printrun/pronsole.py:308
 msgid "X && Y manual feedrate"
 msgstr ""
 
 #: printrun/pronsole.py:309
-#, fuzzy
 msgid "Feedrate for Control Panel Moves in Z (mm/min)"
-msgstr "Vorschub Control Panel Bewegungen Z (Vorgabe: 200mm/min)"
+msgstr ""
 
 #: printrun/pronsole.py:309
 msgid "Z manual feedrate"
 msgstr ""
 
 #: printrun/pronsole.py:310
 msgid "E manual feedrate"
 msgstr ""
 
 #: printrun/pronsole.py:310
-#, fuzzy
 msgid "Feedrate for Control Panel Moves in Extrusions (mm/min)"
-msgstr "Vorschub Control Panel Bewegungen Extrudierung (Vorgabe: 300mm/min)"
+msgstr ""
 
 #: printrun/pronsole.py:311
 #, fuzzy
 msgid "Slice command"
-msgstr "Kommando ausführen:"
+msgstr "Commando"
 
 #: printrun/pronsole.py:312
 #, fuzzy
 msgid "Slice settings command"
-msgstr "Slicing Einstellungen"
+msgstr "SFACT Instellingen"
 
 #: printrun/pronsole.py:312
 msgid "Slicer options command"
 msgstr ""
 
 #: printrun/pronsole.py:313
 msgid "Executable to run when the print is finished"
 msgstr ""
 
 #: printrun/pronsole.py:313
 #, fuzzy
 msgid "Final command"
-msgstr "Kommando"
+msgstr "Commando"
 
 #: printrun/pronsole.py:314
 #, fuzzy
 msgid "Error command"
-msgstr "Kommando ausführen:"
+msgstr "Commando"
 
 #: printrun/pronsole.py:314
 msgid "Executable to run when an error occurs"
 msgstr ""
 
 #: printrun/pronsole.py:381
 msgid "Failed to run callback after setting \"%s\":"
 msgstr ""
 
 #: printrun/pronsole.py:469
 msgid "Build dimensions"
 msgstr ""
 
 #: printrun/pronsole.py:469
-#, fuzzy
 msgid ""
 "Dimensions of Build Platform\n"
 " & optional offset of origin\n"
 " & optional switch position\n"
 "\n"
 "Examples:\n"
 "   XXXxYYY\n"
 "   XXX,YYY,ZZZ\n"
 "   XXXxYYYxZZZ+OffX+OffY+OffZ\n"
 "XXXxYYYxZZZ+OffX+OffY+OffZ+HomeX+HomeY+HomeZ"
 msgstr ""
-"Abmessungen der Bauplattform\n"
-" & optional Versatz vom Ausgangspunkt\n"
-"\n"
-"Beispiel:\n"
-"   XXXxYYY\n"
-"   XXX,YYY,ZZZ\n"
-"   XXXxYYYxZZZ+OffX+OffY+OffZ"
 
 #: printrun/pronsole.py:495
 msgid ""
 "Welcome to the printer console! Type \"help\" for a list of available "
 "commands."
 msgstr ""
 
 #: printrun/pronsole.py:657 printrun/pronsole.py:665 printrun/pronsole.py:673
 #: printrun/pronsole.py:1519 printrun/pronsole.py:1546
 #: printrun/pronsole.py:1618 printrun/pronterface.py:357
 #: printrun/pronterface.py:377 printrun/pronterface.py:394
 msgid "Printer is not online."
-msgstr "Drucker ist nicht online."
+msgstr "Printer is niet verbonden."
 
 #: printrun/pronsole.py:692
 msgid "Exiting program. Goodbye!"
 msgstr ""
 
 #: printrun/pronsole.py:697
 msgid "Disconnects from the printer and exits the program."
@@ -829,51 +809,50 @@
 #: printrun/pronsole.py:976
 msgid "file to load"
 msgstr ""
 
 #: printrun/pronsole.py:1104
 #, fuzzy
 msgid "Loaded %s, %d lines."
-msgstr "Geladen %s, %d Zeilen"
+msgstr "Geladen %s, %d regels"
 
 #: printrun/pronsole.py:1105 printrun/pronterface.py:1381
-#, fuzzy
 msgid "Estimated duration: %d layers, %s"
-msgstr "Geschätze Dauer (pessimistisch): "
+msgstr ""
 
 #: printrun/pronsole.py:1134
 msgid "No file name given."
 msgstr ""
 
 #: printrun/pronsole.py:1140
 msgid "Skeining file: %s"
 msgstr ""
 
 #: printrun/pronsole.py:1142 printrun/pronterface.py:1305
 msgid "File not found!"
-msgstr "Datei nicht gefunden!"
+msgstr "Bestand niet gevonden!"
 
 #: printrun/pronsole.py:1147
 msgid "Entering slicer settings: %s"
 msgstr ""
 
 #: printrun/pronsole.py:1151
 #, fuzzy
 msgid "Slicing: "
-msgstr "Slicing"
+msgstr "Skeinforge draait"
 
 #: printrun/pronsole.py:1158
 #, fuzzy
 msgid "Loading sliced file."
-msgstr "Datei laden"
+msgstr "open bestand"
 
 #: printrun/pronsole.py:1161
 #, fuzzy
 msgid "Slicing failed: %s"
-msgstr "Slicing"
+msgstr "Skeinforge draait"
 
 #: printrun/pronsole.py:1174
 msgid ""
 "Creates a gcode file from an stl model using the slicer (with tab-completion)"
 msgstr ""
 
 #: printrun/pronsole.py:1175
@@ -885,15 +864,15 @@
 "slice filename.stl view - create gcode file and view using skeiniso (if "
 "using skeinforge)"
 msgstr ""
 
 #: printrun/pronsole.py:1177
 #, fuzzy
 msgid "slice set - adjust slicer settings"
-msgstr " Slicing Einstellungen anpassen"
+msgstr "Instellen SFACT"
 
 #: printrun/pronsole.py:1189
 msgid "Please enter target name in 8.3 format."
 msgstr ""
 
 #: printrun/pronsole.py:1195
 msgid "Uploading as %s"
@@ -936,33 +915,33 @@
 #: printrun/pronsole.py:1243
 msgid "Send a loaded gcode file to the printer. You have %s loaded right now."
 msgstr ""
 
 #: printrun/pronsole.py:1247 printrun/pronterface.py:730
 #: printrun/pronterface.py:1108
 msgid "No file loaded. Please use load first."
-msgstr "Keine Datei geladen. Benutze zuerst laden."
+msgstr "Geen bestand geladen. Eerst bestand inladen."
 
 #: printrun/pronsole.py:1252
 #, fuzzy
 msgid "Printing %s"
-msgstr " Drucken:%04.2f %% |"
+msgstr " Printen:%04.2f %% |"
 
 #: printrun/pronsole.py:1253
 msgid "You can monitor the print with the monitor command."
 msgstr ""
 
 #: printrun/pronsole.py:1261
 msgid "Not printing, cannot pause."
 msgstr ""
 
 #: printrun/pronsole.py:1267
 #, fuzzy
 msgid "Pauses a running print"
-msgstr "Starte Druck"
+msgstr "Start het printen"
 
 #: printrun/pronsole.py:1274
 msgid "Not paused, unable to resume. Start a print first."
 msgstr ""
 
 #: printrun/pronsole.py:1284
 msgid "Resumes a paused print."
@@ -972,37 +951,37 @@
 msgid "Files on SD card:"
 msgstr ""
 
 #: printrun/pronsole.py:1307 printrun/pronsole.py:1349
 #: printrun/pronsole.py:1562
 #, fuzzy
 msgid "Printer is not online. Please connect to it first."
-msgstr "Drucker ist nicht online."
+msgstr "Printer is niet verbonden."
 
 #: printrun/pronsole.py:1312
 msgid "Lists files on the SD card"
 msgstr ""
 
 #: printrun/pronsole.py:1316 printrun/pronterface.py:1645
 msgid "Opening file failed."
-msgstr "Datei öffnen fehlgeschlagen."
+msgstr "Bestand openen mislukt"
 
 #: printrun/pronsole.py:1322 printrun/pronterface.py:1651
 msgid "Starting print"
-msgstr "Starte Druck"
+msgstr "Start het printen"
 
 #: printrun/pronsole.py:1345
 #, fuzzy
 msgid "Resets the printer."
-msgstr "Drucker Verbinden"
+msgstr "Verbind met printer"
 
 #: printrun/pronsole.py:1355
 #, fuzzy
 msgid "File is not present on card. Please upload it first."
-msgstr "Keine Datei geladen. Benutze zuerst laden."
+msgstr "Geen bestand geladen. Eerst bestand inladen."
 
 #: printrun/pronsole.py:1359
 msgid "Printing file: %s from SD card."
 msgstr ""
 
 #: printrun/pronsole.py:1360
 msgid "Requesting SD print..."
@@ -1037,101 +1016,100 @@
 msgstr ""
 
 #: printrun/pronsole.py:1457
 msgid "Printer is not currently printing. No ETA available."
 msgstr ""
 
 #: printrun/pronsole.py:1460
-#, fuzzy
 msgid "Est: %s of %s remaining"
-msgstr " Erw: %s von %s verbleibend | "
+msgstr ""
 
 #: printrun/pronsole.py:1465
 msgid "Displays estimated remaining print time."
 msgstr ""
 
 #: printrun/pronsole.py:1498
 #, fuzzy
 msgid "Read the extruder and bed temperature."
-msgstr "Sie müssen eine Temperatur eingeben."
+msgstr "Er moet een temperatuur worden ingesteld."
 
 #: printrun/pronsole.py:1507 printrun/pronsole.py:1540
 msgid "You must enter a temperature."
-msgstr "Sie müssen eine Temperatur eingeben."
+msgstr "Er moet een temperatuur worden ingesteld."
 
 #: printrun/pronsole.py:1512
 msgid ""
 "%s is a high temperature to set your extruder to. Are you sure you want to "
 "do that?"
 msgstr ""
 
 #: printrun/pronsole.py:1517
 #, fuzzy
 msgid "Setting hotend temperature to %s degrees Celsius."
-msgstr "Setze Hotend Temperatur auf %f Grad Celsius."
+msgstr "Stel elementtemperatuur in op %f graden Celsius."
 
 #: printrun/pronsole.py:1521 printrun/pronterface.py:359
 msgid ""
 "You cannot set negative temperatures. To turn the hotend off entirely, set "
 "its temperature to 0."
 msgstr ""
-"Sie können keine negativen Temperaturen einstellen. Um das Hotend ganz "
-"auszuschalten, Temperatur auf 0 setzen."
+"Negatieve temperatuur is niet instelbaar. Om het element uit te schakelen "
+"wordt temperatuur 0 ingesteld."
 
 #: printrun/pronsole.py:1524
 #, fuzzy
 msgid "Sets the hotend temperature to the value entered."
-msgstr "Setze Hotend Temperatur auf %f Grad Celsius."
+msgstr "Stel elementtemperatuur in op %f graden Celsius."
 
 #: printrun/pronsole.py:1525 printrun/pronsole.py:1552
 msgid "Enter either a temperature in celsius or one of the following keywords"
 msgstr ""
 
 #: printrun/pronsole.py:1544
 #, fuzzy
 msgid "Setting bed temperature to %s degrees Celsius."
-msgstr "Setze Heizbett Temperatur auf %f Grad Celsius."
+msgstr "Bed teperatuur ingesteld op %f graden Celsius."
 
 #: printrun/pronsole.py:1548 printrun/pronterface.py:379
 msgid ""
 "You cannot set negative temperatures. To turn the bed off entirely, set its "
 "temperature to 0."
 msgstr ""
-"Sie können keine negativen Temperaturen einstellen. Um das Heizbett ganz "
-"auszuschalten, Temperatur auf 0 setzen."
+"Negatieve temperatuur is niet instelbaar. Om het printbed uit te schakelen "
+"wordt temperatuur 0 ingesteld."
 
 #: printrun/pronsole.py:1551
 #, fuzzy
 msgid "Sets the bed temperature to the value entered."
-msgstr "Setze Heizbett Temperatur auf %f Grad Celsius."
+msgstr "Bed teperatuur ingesteld op %f graden Celsius."
 
 #: printrun/pronsole.py:1565
 msgid "Printer is not printing. Please print something before monitoring."
 msgstr ""
 
 #: printrun/pronsole.py:1567
 #, fuzzy
 msgid "Monitoring printer, use ^C to interrupt."
-msgstr "Überwache Drucker."
+msgstr "Printercommunicatie wordt gevolgd."
 
 #: printrun/pronsole.py:1572 printrun/pronterface.py:329
 msgid "Invalid period given."
-msgstr "Ungültiger Abschnitt angegeben."
+msgstr "Foute gegevens ingevoerd"
 
 #: printrun/pronsole.py:1573
 msgid "Updating values every %f seconds."
 msgstr ""
 
 #: printrun/pronsole.py:1584 printrun/pronsole.py:1587
 msgid "Print progress: "
 msgstr ""
 
 #: printrun/pronsole.py:1595 printrun/pronterface.py:333
 msgid "Done monitoring."
-msgstr "Überwachung abgeschlossen."
+msgstr "Klaar met volgen."
 
 #: printrun/pronsole.py:1599
 msgid "Monitor a machine's temperatures and an SD print's status."
 msgstr ""
 
 #: printrun/pronsole.py:1600
 msgid ""
@@ -1172,15 +1150,15 @@
 "Printer is currently printing. Please pause the print before you issue "
 "manual commands."
 msgstr ""
 
 #: printrun/pronsole.py:1633 printrun/pronsole.py:1759
 #, fuzzy
 msgid "Printer is not online. Unable to move."
-msgstr "Drucker ist nicht online."
+msgstr "Printer is niet verbonden."
 
 #: printrun/pronsole.py:1649
 msgid "Unknown axis."
 msgstr ""
 
 #: printrun/pronsole.py:1654
 msgid "Invalid distance"
@@ -1208,20 +1186,20 @@
 #: printrun/pronsole.py:1669
 msgid "Common amounts are in the tabcomplete list."
 msgstr ""
 
 #: printrun/pronsole.py:1699 printrun/pronsole.py:1742
 #, fuzzy
 msgid "Invalid length given."
-msgstr "Ungültiger Abschnitt angegeben."
+msgstr "Foute gegevens ingevoerd"
 
 #: printrun/pronsole.py:1704 printrun/pronsole.py:1747
 #, fuzzy
 msgid "Invalid speed given."
-msgstr "Ungültiger Abschnitt angegeben."
+msgstr "Foute gegevens ingevoerd"
 
 #: printrun/pronsole.py:1712
 msgid "Extruding %fmm of filament."
 msgstr ""
 
 #: printrun/pronsole.py:1714
 msgid "Reversing %fmm of filament."
@@ -1252,15 +1230,15 @@
 #: printrun/pronsole.py:1726
 msgid "extrude 10 210 - extrudes 10mm of filament at 210mm/min (3.5mm/s)"
 msgstr ""
 
 #: printrun/pronsole.py:1732
 #, fuzzy
 msgid "Printer is not online. Unable to reverse."
-msgstr "Drucker ist nicht online."
+msgstr "Printer is niet verbonden."
 
 #: printrun/pronsole.py:1751
 msgid ""
 "Reverses the extruder, 5mm by default, or the number of mm given as a "
 "parameter"
 msgstr ""
 
@@ -1279,15 +1257,15 @@
 #: printrun/pronsole.py:1755
 msgid "reverse -5 - EXTRUDES 5mm of filament at 300mm/min (5mm/s)"
 msgstr ""
 
 #: printrun/pronsole.py:1777
 #, fuzzy
 msgid "Homes the printer"
-msgstr "Drucker Verbinden"
+msgstr "Verbind met printer"
 
 #: printrun/pronsole.py:1778
 msgid "home - homes all axes and zeroes the extruder(Using G28 and G92)"
 msgstr ""
 
 #: printrun/pronsole.py:1779
 msgid "home xy - homes x and y axes (Using G28)"
@@ -1304,20 +1282,20 @@
 #: printrun/pronsole.py:1782
 msgid "home xyze - homes all axes and zeroes the extruder (Using G28 and G92)"
 msgstr ""
 
 #: printrun/pronsole.py:1790
 #, fuzzy
 msgid "; Motors off"
-msgstr "Motoren aus"
+msgstr "Motoren uit"
 
 #: printrun/pronsole.py:1792
 #, fuzzy
 msgid "; Extruder off"
-msgstr "Extrudieren"
+msgstr "Extruden"
 
 #: printrun/pronsole.py:1794
 msgid "; Heatbed off"
 msgstr ""
 
 #: printrun/pronsole.py:1796
 msgid "; Fan off"
@@ -1326,15 +1304,15 @@
 #: printrun/pronsole.py:1798
 msgid "; Power supply off"
 msgstr ""
 
 #: printrun/pronsole.py:1801
 #, fuzzy
 msgid "Printer is not online. Unable to turn it off."
-msgstr "Drucker ist nicht online."
+msgstr "Printer is niet verbonden."
 
 #: printrun/pronsole.py:1804
 msgid "Turns off everything on the printer"
 msgstr ""
 
 #: printrun/pronsole.py:1815
 msgid "G-Code calling host command \"%s\""
@@ -1349,31 +1327,31 @@
 msgid ""
 "Runs a custom script which output gcode which will in turn be executed. "
 "Current gcode filename can be given using %s token."
 msgstr ""
 
 #: printrun/pronterface.py:149
 msgid "Motors off"
-msgstr "Motoren aus"
+msgstr "Motoren uit"
 
 #: printrun/pronterface.py:149
 msgid "Switch all motors off"
 msgstr ""
 
 #: printrun/pronterface.py:150
 msgid "Advance extruder by set length"
 msgstr ""
 
 #: printrun/pronterface.py:150
 msgid "Extrude"
-msgstr "Extrudieren"
+msgstr "Extruden"
 
 #: printrun/pronterface.py:151
 msgid "Reverse"
-msgstr "Rückwärts"
+msgstr "Terug"
 
 #: printrun/pronterface.py:151
 msgid "Reverse extruder by set length"
 msgstr ""
 
 #: printrun/pronterface.py:165
 #, fuzzy
@@ -1382,57 +1360,56 @@
 
 #: printrun/pronterface.py:192
 msgid ""
 "# I moved all your custom buttons into .pronsolerc.\n"
 "# Please don't add them here any more.\n"
 "# Backup of your old buttons is in custombtn.old\n"
 msgstr ""
-"# Alle individuellen Buttons in .pronsolerc eingetragen.\n"
-"# Bitte fügen Sie sie hier nicht mehr ein.\n"
-"# Backup Ihrer alten Buttons befindet sich in custombtn.old\n"
+"# Gedefinieerde knoppen zijn verplaatst naar .pronsolerc.\n"
+"# Hier geen nieuwe knoppen definiëren.\n"
+"# Een backup van de oude knoppen staat in custombtn.old\n"
 
 #: printrun/pronterface.py:197
 msgid ""
 "Note!!! You have specified custom buttons in both custombtn.txt and ."
 "pronsolerc"
 msgstr ""
-"Achtung! Sie haben benutzerdefinierte Buttons in custombtn.txt und ."
-"pronsolerc angegeben"
+"Let op!!! Er zijn gedefinieerde knoppen in zowel custombtn.txt en .pronsolerc"
 
 #: printrun/pronterface.py:198
 msgid ""
 "Ignoring custombtn.txt. Remove all current buttons to revert to custombtn.txt"
 msgstr ""
-"Ignoriere custombtn.txt. Alle aktuellen Buttons entfernen um wieder zu "
-"custombtn.txt zurückzukehren"
+"Negeer custombtn.txt. Verwijder alle gedefinieerde knoppen om gebruik te "
+"maken van custombtn.txt"
 
 #: printrun/pronterface.py:331
 msgid "Monitoring printer."
-msgstr "Überwache Drucker."
+msgstr "Printercommunicatie wordt gevolgd."
 
 #: printrun/pronterface.py:354
 msgid "Setting hotend temperature to %f degrees Celsius."
-msgstr "Setze Hotend Temperatur auf %f Grad Celsius."
+msgstr "Stel elementtemperatuur in op %f graden Celsius."
 
 #: printrun/pronterface.py:361 printrun/pronterface.py:381
 msgid "You must enter a temperature. (%s)"
-msgstr "Sie müssen eine Temperatur eingeben. (%s)"
+msgstr "Er moet een temperatuur worden ingesteld. (%s)"
 
 #: printrun/pronterface.py:374
 msgid "Setting bed temperature to %f degrees Celsius."
-msgstr "Setze Heizbett Temperatur auf %f Grad Celsius."
+msgstr "Bed teperatuur ingesteld op %f graden Celsius."
 
 #: printrun/pronterface.py:392
 msgid "Setting print speed factor to %d%%."
 msgstr ""
 
 #: printrun/pronterface.py:396
 #, fuzzy
 msgid "You must enter a speed. (%s)"
-msgstr "Sie müssen eine Temperatur eingeben. (%s)"
+msgstr "Er moet een temperatuur worden ingesteld. (%s)"
 
 #: printrun/pronterface.py:470
 msgid "Plate function activated"
 msgstr ""
 
 #: printrun/pronterface.py:479
 msgid "G-Code plate function activated"
@@ -1440,19 +1417,19 @@
 
 #: printrun/pronterface.py:486
 msgid "Plated %s"
 msgstr ""
 
 #: printrun/pronterface.py:500
 msgid "SD Upload"
-msgstr "SD Laden"
+msgstr "uploaden naar SD"
 
 #: printrun/pronterface.py:504
 msgid "SD Print"
-msgstr "SD Drucken"
+msgstr "Afdruk van SD"
 
 #: printrun/pronterface.py:565
 msgid ""
 "Manual move outside of the build volume prevented (see the \"Clamp manual "
 "moves\" option)."
 msgstr ""
 
@@ -1460,56 +1437,56 @@
 msgid ""
 "Attempted to write invalid text to console, which could be due to an invalid "
 "baudrate"
 msgstr ""
 
 #: printrun/pronterface.py:655
 msgid " Opens file"
-msgstr " Öffnet eine Datei"
+msgstr " Opent bestand"
 
 #: printrun/pronterface.py:655
 msgid "&Open..."
-msgstr "&Öffnen..."
+msgstr "&Open..."
 
 #: printrun/pronterface.py:663
 msgid " Clear output console"
-msgstr " Ausgabe Konsole leeren"
+msgstr ""
 
 #: printrun/pronterface.py:663
 msgid "Clear console"
-msgstr "Konsole leeren"
+msgstr ""
 
 #: printrun/pronterface.py:664
 msgid " Closes the Window"
-msgstr " Schliesst das Fenster"
+msgstr " Sluit het venster"
 
 #: printrun/pronterface.py:664
 msgid "E&xit"
-msgstr "&Verlassen"
+msgstr "&Stoppen"
 
 #: printrun/pronterface.py:665
 msgid "&File"
-msgstr "&Datei"
+msgstr ""
 
 #: printrun/pronterface.py:668
 msgid " Edit open file"
-msgstr " Offene Datei bearbeiten"
+msgstr " Wijzig geopend bestand"
 
 #: printrun/pronterface.py:668
 msgid "&Edit..."
-msgstr "&Bearbeiten..."
+msgstr "&Wijzig..."
 
 #: printrun/pronterface.py:669
 msgid " Compose 3D models into a single plate"
 msgstr ""
 
 #: printrun/pronterface.py:669
 #, fuzzy
 msgid "Plater"
-msgstr "Heizelement:"
+msgstr "Element:"
 
 #: printrun/pronterface.py:670
 msgid " Compose G-Codes into a single plate"
 msgstr ""
 
 #: printrun/pronterface.py:670
 msgid "G-Code Plater"
@@ -1521,19 +1498,19 @@
 
 #: printrun/pronterface.py:671
 msgid "Excluder"
 msgstr ""
 
 #: printrun/pronterface.py:672
 msgid " Project slices"
-msgstr " Projekt Slices"
+msgstr ""
 
 #: printrun/pronterface.py:672
 msgid "Projector"
-msgstr "Projektor"
+msgstr ""
 
 #: printrun/pronterface.py:673
 msgid "&Tools"
 msgstr ""
 
 #: printrun/pronterface.py:676
 msgid ""
@@ -1548,75 +1525,75 @@
 #: printrun/pronterface.py:679
 msgid "&Advanced"
 msgstr ""
 
 #: printrun/pronterface.py:686
 #, fuzzy
 msgid "Print &settings"
-msgstr "Einstellungen bearbeiten"
+msgstr "Wijzig instellingen"
 
 #: printrun/pronterface.py:687
-#, fuzzy
 msgid "&Filament"
-msgstr "&Datei"
+msgstr ""
 
 #: printrun/pronterface.py:688
 #, fuzzy
 msgid "&Printer"
-msgstr "Drucken"
+msgstr "&Printen"
 
 #: printrun/pronterface.py:694
 msgid "&Slic3r"
 msgstr ""
 
 #: printrun/pronterface.py:696
 msgid "Failed to load Slic3r configuration:"
 msgstr ""
 
 #: printrun/pronterface.py:702
 msgid "&Macros"
-msgstr "&Makros"
+msgstr "&Macros"
 
 #: printrun/pronterface.py:703
 msgid "<&New...>"
-msgstr "<&Neu...>"
+msgstr "<&Nieuw...>"
 
 #: printrun/pronterface.py:704
 msgid " Options dialog"
-msgstr " Optionen Dialog"
+msgstr "Optievenster"
 
 #: printrun/pronterface.py:704
 msgid "&Options"
-msgstr "&Optionen"
+msgstr "&Opties"
 
 #: printrun/pronterface.py:706
+#, fuzzy
 msgid " Adjust slicing settings"
-msgstr " Slicing Einstellungen anpassen"
+msgstr "Instellen SFACT"
 
 #: printrun/pronterface.py:706
 #, fuzzy
 msgid "Slicing settings"
-msgstr "Slicing Einstellungen"
+msgstr "SFACT Instellingen"
 
 #: printrun/pronterface.py:708
 msgid "Debug communications"
 msgstr ""
 
 #: printrun/pronterface.py:709
 msgid "Print all G-code sent to and received from the printer."
 msgstr ""
 
 #: printrun/pronterface.py:713
 msgid "&Settings"
-msgstr "&Einstellungen"
+msgstr "&Instellingen"
 
 #: printrun/pronterface.py:719
 #, fuzzy
 msgid "&About Printrun"
-msgstr "Drucker überwachen"
+msgstr "Printercommunicatie volgen"
 
 #: printrun/pronterface.py:719
 msgid "Show about dialog"
 msgstr ""
 
 #: printrun/pronterface.py:720
 msgid "&Help"
@@ -1626,20 +1603,20 @@
 msgid ""
 "Printrun is a pure Python 3D printing (and other types of CNC) host software."
 msgstr ""
 
 #: printrun/pronterface.py:750
 #, fuzzy
 msgid "%.02fmm of filament have been extruded during prints"
-msgstr "mm Filament in Druck genutzt\n"
+msgstr "mm fillament wordt gebruikt in deze print\n"
 
 #: printrun/pronterface.py:781
 #, fuzzy
 msgid "Monitor printer status"
-msgstr "Drucker überwachen"
+msgstr "Printercommunicatie volgen"
 
 #: printrun/pronterface.py:781
 msgid ""
 "Regularly monitor printer temperatures (required to have functional "
 "temperature graph or gauges)"
 msgstr ""
 
@@ -1658,15 +1635,15 @@
 #: printrun/pronterface.py:783
 msgid "Draw a circular (or oval) build platform instead of a rectangular one"
 msgstr ""
 
 #: printrun/pronterface.py:784
 #, fuzzy
 msgid "Extruders count"
-msgstr "Extrudieren"
+msgstr "Extruden"
 
 #: printrun/pronterface.py:784
 msgid "Number of extruders"
 msgstr ""
 
 #: printrun/pronterface.py:785
 msgid "Clamp manual moves"
@@ -1675,15 +1652,15 @@
 #: printrun/pronterface.py:785
 msgid "Prevent manual moves from leaving the specified build dimensions"
 msgstr ""
 
 #: printrun/pronterface.py:786
 #, fuzzy
 msgid "Interface mode"
-msgstr "Makro Name eingeben"
+msgstr "Voer macronaam in"
 
 #: printrun/pronterface.py:786
 msgid ""
 "Standard interface is a one-page, three columns layout with controls/"
 "visualization/log\n"
 "Compact mode is a one-page, two columns layout with controls + log/"
 "visualization\n"
@@ -1787,46 +1764,40 @@
 msgstr ""
 
 #: printrun/pronterface.py:804
 msgid "Preview extrusion width"
 msgstr ""
 
 #: printrun/pronterface.py:804
-#, fuzzy
 msgid "Width of Extrusion in Preview"
-msgstr "Vorschaubreite der Extrudierung (Vorgabe: 0.5)"
+msgstr ""
 
 #: printrun/pronterface.py:805
-#, fuzzy
 msgid "Fine Grid Spacing"
-msgstr "Feiner Rasterabstand (Vorgabe: 10)"
+msgstr ""
 
 #: printrun/pronterface.py:805
-#, fuzzy
 msgid "Fine grid spacing"
-msgstr "Feiner Rasterabstand (Vorgabe: 10)"
+msgstr ""
 
 #: printrun/pronterface.py:806
-#, fuzzy
 msgid "Coarse Grid Spacing"
-msgstr "Grober Rasterabstand (Vorgabe: 50)"
+msgstr ""
 
 #: printrun/pronterface.py:806
-#, fuzzy
 msgid "Coarse grid spacing"
-msgstr "Grober Rasterabstand (Vorgabe: 50)"
+msgstr ""
 
 #: printrun/pronterface.py:807
 msgid "Background color"
 msgstr ""
 
 #: printrun/pronterface.py:807
-#, fuzzy
 msgid "Pronterface background color"
-msgstr "Pronterface Hintergrundfarbe (Vorgabe: #FFFFFF)"
+msgstr ""
 
 #: printrun/pronterface.py:808
 msgid "3D view background color"
 msgstr ""
 
 #: printrun/pronterface.py:808
 msgid "Color of the 3D view background"
@@ -1895,33 +1866,33 @@
 #: printrun/pronterface.py:835 printrun/pronterface.py:1316
 msgid "Failed to load recent files list:"
 msgstr ""
 
 #: printrun/pronterface.py:916
 #, fuzzy
 msgid "SD upload: %04.2f%% |"
-msgstr "SD Drucken:%04.2f %%"
+msgstr " SD printen:%04.2f %%"
 
 #: printrun/pronterface.py:917 printrun/pronterface.py:922
 msgid " Line# %d of %d lines |"
-msgstr " Zeile# %d von %d Zeilen |"
+msgstr ""
 
 #: printrun/pronterface.py:919
 #, fuzzy
 msgid "SD printing: %04.2f%% |"
-msgstr "SD Drucken:%04.2f %%"
+msgstr " SD printen:%04.2f %%"
 
 #: printrun/pronterface.py:921
 #, fuzzy
 msgid "Printing: %04.2f%% |"
-msgstr " Drucken:%04.2f %% |"
+msgstr " Printen:%04.2f %% |"
 
 #: printrun/pronterface.py:924
 msgid " Est: %s of %s remaining | "
-msgstr " Erw: %s von %s verbleibend | "
+msgstr ""
 
 #: printrun/pronterface.py:926
 #, fuzzy
 msgid " Z: %.3f mm"
 msgstr " Z: %0.2f mm"
 
 #: printrun/pronterface.py:931
@@ -1932,19 +1903,20 @@
 #, fuzzy
 msgid "Locking interface."
 msgstr "Printer Interface"
 
 #: printrun/pronterface.py:976
 #, fuzzy
 msgid "Unlocking interface."
-msgstr "Überwache Drucker."
+msgstr "Printercommunicatie wordt gevolgd."
 
 #: printrun/pronterface.py:985
+#, fuzzy
 msgid "Connecting..."
-msgstr "Verbinde..."
+msgstr "Verbind"
 
 #: printrun/pronterface.py:997
 msgid "Could not parse baud rate: "
 msgstr ""
 
 #: printrun/pronterface.py:1013 printrun/pronterface.py:1023
 msgid "Error: You are trying to connect to a non-existing port."
@@ -1955,257 +1927,328 @@
 msgstr ""
 
 #: printrun/pronterface.py:1016
 msgid "You might need to add yourself to the dialout group."
 msgstr ""
 
 #: printrun/pronterface.py:1043
+#, fuzzy
 msgid "Disconnected."
-msgstr "Getrennt."
+msgstr "Ontkoppel"
 
 #: printrun/pronterface.py:1071
+#, fuzzy
 msgid "Reset."
-msgstr "Zurücksetzen."
+msgstr "Reset"
 
 #: printrun/pronterface.py:1072
 msgid "Are you sure you want to reset the printer?"
-msgstr "Möchten Sie den Drucker wirklich zurücksetzen?"
+msgstr "Weet je zeker dat je de printer wilt resetten?"
 
 #: printrun/pronterface.py:1072
 msgid "Reset?"
-msgstr "Zurücksetzen?"
+msgstr "resetten?"
 
 #: printrun/pronterface.py:1093
 msgid "Restart"
-msgstr "Neustart"
+msgstr "Herstart"
 
 #: printrun/pronterface.py:1126
 msgid "Pick SD filename"
-msgstr "Wähle SD Dateiname"
+msgstr "Kies bestandsnaam op SD"
 
 #: printrun/pronterface.py:1144
 msgid "File upload complete"
-msgstr "Datei Upload komplett"
+msgstr "Bestandsupload voltooid"
 
 #: printrun/pronterface.py:1151
 msgid "Print paused at: %s"
 msgstr ""
 
 #: printrun/pronterface.py:1163
 msgid "Resume"
-msgstr "Fortsetzen"
+msgstr "Hervat"
 
 #: printrun/pronterface.py:1166
 #, fuzzy
 msgid "Resuming."
-msgstr "Fortsetzen"
+msgstr "Hervat"
 
 #: printrun/pronterface.py:1192
 msgid "Pick SD file"
-msgstr "Wähle SD Datei"
+msgstr "Kies bestand op SD"
 
 #: printrun/pronterface.py:1192
 msgid "Select the file to print"
-msgstr "Wähle Druckdatei"
+msgstr "Kies het te printen bestand"
 
 #: printrun/pronterface.py:1228 printrun/pronterface.py:1259
+#, fuzzy
 msgid "Slicing "
-msgstr "Slicing"
+msgstr "Skeinforge draait"
 
 #: printrun/pronterface.py:1237
 msgid "Failed to execute slicing software: "
-msgstr "Fehler beim Ausführen der Slicing Software:"
+msgstr ""
 
 #: printrun/pronterface.py:1244
+#, fuzzy
 msgid "Slicing..."
-msgstr "Slicing..."
+msgstr "Skeinforge draait..."
 
 #: printrun/pronterface.py:1296
 msgid "Open file to print"
-msgstr "Öffne zu druckende Datei"
+msgstr "Open het te printen bestand"
 
 #: printrun/pronterface.py:1297
 #, fuzzy
 msgid ""
 "OBJ, STL, and GCODE files (*.gcode;*.gco;*.g;*.stl;*.STL;*.obj;*.OBJ)|*."
 "gcode;*.gco;*.g;*.stl;*.STL;*.obj;*.OBJ|All Files (*.*)|*.*"
-msgstr ""
-"OBJ,STL und GCODE Dateien  (;*.gcode;*.gco;*.g;*.stl;*.STL;*.obj;*.OBJ;)"
+msgstr "STL en GCODE bestanden (;*.gcode;*.g;*.stl;*.STL;)"
 
 #: printrun/pronterface.py:1325
 msgid "Could not update recent files list:"
 msgstr ""
 
 #: printrun/pronterface.py:1359
 msgid "Loaded %s, %d lines"
-msgstr "Geladen %s, %d Zeilen"
+msgstr "Geladen %s, %d regels"
 
 #: printrun/pronterface.py:1362
+#, fuzzy
 msgid "Load File"
-msgstr "Datei laden"
+msgstr "open bestand"
 
 #: printrun/pronterface.py:1376
 #, fuzzy
 msgid "%.2fmm of filament used in this print"
-msgstr "mm Filament in Druck genutzt\n"
+msgstr "mm fillament wordt gebruikt in deze print\n"
 
 #: printrun/pronterface.py:1377
 msgid "The print goes:"
 msgstr ""
 
 #: printrun/pronterface.py:1378
-#, fuzzy
 msgid "- from %.2f mm to %.2f mm in X and is %.2f mm wide"
 msgstr ""
-"Der Druck verläuft von %f mm bis %f mm in X\n"
-"und ist %f mm breit\n"
 
 #: printrun/pronterface.py:1379
-#, fuzzy
 msgid "- from %.2f mm to %.2f mm in Y and is %.2f mm deep"
 msgstr ""
-"Der Druck verläuft von %f mm bis %f mm in Y\n"
-"und ist %f mm breit\n"
 
 #: printrun/pronterface.py:1380
-#, fuzzy
 msgid "- from %.2f mm to %.2f mm in Z and is %.2f mm high"
 msgstr ""
-"Der Druck verläuft von %f mm bis %f mm in Z\n"
-"und ist %f mm hoch\n"
 
 #: printrun/pronterface.py:1450
 msgid "Printer is now online."
-msgstr "Drucker ist jetzt Online."
+msgstr "Printer is nu verbonden."
 
 #: printrun/pronterface.py:1455
 msgid "Disconnect"
-msgstr "Trennen"
+msgstr "Ontkoppel"
 
 #: printrun/pronterface.py:1688
+#, fuzzy
 msgid "click to add new custom button"
-msgstr "Individuellen Button hinzufügen"
+msgstr "Definieer eigen knop."
 
 #: printrun/pronterface.py:1694
 msgid "Execute command: "
-msgstr "Kommando ausführen:"
+msgstr ""
 
 #: printrun/pronterface.py:1714
 msgid ""
 "Defines custom button. Usage: button <num> \"title\" [/c \"colour\"] command"
 msgstr ""
-"Definiert einen individuellen Button. Nutzung: button <num> \"title\" [/c "
-"\"colour\"] command"
+"Definieert eigen knop. Gebruik: knop <num> \"titel\" [/c \"kleur\"] commando"
 
 #: printrun/pronterface.py:1736
 msgid "Custom button number should be between 0 and 63"
-msgstr "Nummer des individuellen Button sollte zwischen 0 und 63 sein."
+msgstr "Knopnummer moet tussen 0 en 63 zijn"
 
 #: printrun/pronterface.py:1827
 msgid "Edit custom button '%s'"
-msgstr "Individuellen Button '%s' bearbeiten"
+msgstr "Wijzig gedefineerde knop '%s'"
 
 #: printrun/pronterface.py:1829
 msgid "Move left <<"
-msgstr "Links bewegen <<"
+msgstr "Verplaats links <<"
 
 #: printrun/pronterface.py:1832
 msgid "Move right >>"
-msgstr "Rechts bewegen >>"
+msgstr "Verplaats rechts >>"
 
 #: printrun/pronterface.py:1836
 msgid "Remove custom button '%s'"
-msgstr "Individuellen Button '%s' entfernen"
+msgstr "Verwijder gedefinieerde knop '%s'"
 
 #: printrun/pronterface.py:1839
 msgid "Add custom button"
-msgstr "Individuellen Button hinzufuegen"
+msgstr "Definieer eigen knop."
 
 #: printrun/pronterface.py:1972
 msgid "event object missing"
-msgstr "Ereigniss Objekt fehlt"
+msgstr "vermist object"
 
 #: printrun/pronterface.py:1985
 msgid "Do you want to erase the macro?"
-msgstr "Möchten Sie das Makro löschen?"
+msgstr "Wilt u de macro verwijderen?"
 
 #: printrun/pronterface.py:1989
 msgid "Cancelled."
-msgstr "Abgebrochen."
+msgstr "Afgebroken"
 
 #: printrun/pronterface.py:2007
 msgid "Enter macro name"
-msgstr "Makro Name eingeben"
+msgstr "Voer macronaam in"
 
 #: printrun/pronterface.py:2010
 msgid "Macro name:"
-msgstr "Makro Name:"
+msgstr "Macronaam:"
 
 #: printrun/pronterface.py:2013
 msgid "Ok"
 msgstr "Ok"
 
 #: printrun/pronterface.py:2035
-#, fuzzy
 msgid "Macro name may contain only ASCII alphanumeric symbols and underscores"
-msgstr "Makro Name darf nur alphanumerische Zeichen und Unterstriche enthalten"
+msgstr ""
 
 #: printrun/pronterface.py:2038
 msgid "Name '%s' is being used by built-in command"
-msgstr "Name '%s' wird durch eingebautes Kommando genutzt"
+msgstr "Naam '%s' wordt gebruikt door ingebouwde instructie"
 
 #: pronsole.py:31
 msgid "Caught an exception, exiting:"
 msgstr ""
 
-#~ msgid "Folder of last opened file"
-#~ msgstr "Verzeichniss der zuletzt geöffneten Datei"
-
 #~ msgid "Check temp"
-#~ msgstr "Temperatur prüfen"
+#~ msgstr "Controleer Temp."
 
 #~ msgid "Mini mode"
-#~ msgstr "Mini-Modus"
-
-#~ msgid "Compose"
-#~ msgstr "Zusammenstellen"
+#~ msgstr "Mini-venster"
 
 #~ msgid "Z:"
 #~ msgstr "Z:"
 
 #~ msgid "Full mode"
-#~ msgstr "Voll-Modus"
+#~ msgstr "Volledig venster"
 
 #~ msgid "Printer is online. "
-#~ msgstr "Drucker ist online. "
+#~ msgstr "Printer is verbonden. "
 
 #~ msgid "Bed"
-#~ msgstr "Heizbett"
+#~ msgstr "Bed"
 
 #~ msgid "Hotend"
-#~ msgstr "Hotend"
+#~ msgstr "Element"
 
 #~ msgid ", %d lines"
-#~ msgstr ", %d Zeilen"
+#~ msgstr ", %d regels"
 
+#, fuzzy
 #~ msgid "Paused."
-#~ msgstr "Pausiert."
+#~ msgstr "Pauze"
 
-#~ msgid ""
-#~ "Slice command\n"
-#~ "   default:\n"
-#~ "       python skeinforge/skeinforge_application/skeinforge_utilities/"
-#~ "skeinforge_craft.py $s)"
-#~ msgstr ""
-#~ "Kommando Slicing\n"
-#~ "   Vorgabe:\n"
-#~ "       python skeinforge/skeinforge_application/skeinforge_utilities/"
-#~ "skeinforge_craft.py $s)"
+#~ msgid "X+100"
+#~ msgstr "X+100"
+
+#~ msgid "X+10"
+#~ msgstr "X+10"
+
+#~ msgid "X+1"
+#~ msgstr "X+1"
+
+#~ msgid "X+0.1"
+#~ msgstr "X+0.1"
+
+#~ msgid "HomeX"
+#~ msgstr "0-puntX"
+
+#~ msgid "X-0.1"
+#~ msgstr "X-0.1"
+
+#~ msgid "X-1"
+#~ msgstr "X-1"
+
+#~ msgid "X-10"
+#~ msgstr "X-10"
+
+#~ msgid "X-100"
+#~ msgstr "X-100"
+
+#~ msgid "Y+100"
+#~ msgstr "Y+100"
+
+#~ msgid "Y+10"
+#~ msgstr "Y+10"
+
+#~ msgid "Y+1"
+#~ msgstr "Y+1"
+
+#~ msgid "Y+0.1"
+#~ msgstr "Y+0.1"
+
+#~ msgid "HomeY"
+#~ msgstr "0-puntY"
+
+#~ msgid "Y-0.1"
+#~ msgstr "Y-0.1"
+
+#~ msgid "Y-1"
+#~ msgstr "Y-1"
+
+#~ msgid "Y-10"
+#~ msgstr "Y-10"
+
+#~ msgid "Y-100"
+#~ msgstr "Y-100"
+
+#~ msgid "Z+10"
+#~ msgstr "Z+10"
+
+#~ msgid "Z+1"
+#~ msgstr "Z+1"
+
+#~ msgid "Z+0.1"
+#~ msgstr "Z+0.1"
+
+#~ msgid "HomeZ"
+#~ msgstr "0-puntZ"
+
+#~ msgid "Z-0.1"
+#~ msgstr "Z-0.1"
+
+#~ msgid "Z-1"
+#~ msgstr "Z-1"
+
+#~ msgid "Z-10"
+#~ msgstr "Z-10"
+
+#~ msgid "Home"
+#~ msgstr "0-punt"
+
+#~ msgid " degrees Celsius."
+#~ msgstr " graden Celsius."
+
+#~ msgid "SFACT Quick Settings"
+#~ msgstr "SFACT Snelinstelling"
+
+#~ msgid " Quickly adjust SFACT settings for active profile"
+#~ msgstr " Eenvoudig SFACT's huidige profiel instellen"
+
+#~ msgid "Name '"
+#~ msgstr "Naam '"
+
+#~ msgid "Skeinforge execution failed."
+#~ msgstr "Skeinforge was niet succesvol."
 
 #~ msgid ""
-#~ "Slice settings command\n"
-#~ "   default:\n"
-#~ "       python skeinforge/skeinforge_application/skeinforge.py"
+#~ "Skeinforge not found. \n"
+#~ "Please copy Skeinforge into a directory named \"skeinforge\" in the same "
+#~ "directory as this file."
 #~ msgstr ""
-#~ "Kommando Slicing Einstellungen\n"
-#~ "   Vorgabe:\n"
-#~ "       python skeinforge/skeinforge_application/skeinforge.py"
+#~ "Skeinforge niet gevonden.\n"
+#~ "Plaats Skeinforge in een map met de naam \"skeinforge\" in dezelfde map "
+#~ "als dit bestand."
```

### Comparing `Printrun-2.0.0rc7/locale/fr/LC_MESSAGES/pronterface.po` & `Printrun-2.0.1/locale/fr/LC_MESSAGES/pronterface.po`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/locale/hy/LC_MESSAGES/plater.po` & `Printrun-2.0.1/locale/hy/LC_MESSAGES/plater.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Armenian Plater Message Catalog
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Plater\n"
 "POT-Creation-Date: 2012-08-04 21:53+CEST\n"
-"PO-Revision-Date: 2020-18-04 11:16+CEST\n"
-"Last-Translator: Avag Sayan <info@armath.am>\n"
+"PO-Revision-Date: 2022-02-27 18:34+0400\n"
+"Last-Translator: Ավագ Սայան <info@armath.am>\n"
 "Language-Team: Armath Engineering Labs, info@armath.am\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
 "Language: hy_AM\n"
-
+"X-Generator: Poedit 2.4.2\n"
 
 #: plater.py:246
 msgid "Plate building tool"
 msgstr "Հատակը կառուցելու գործիք"
 
 #: plater.py:252
 msgid "Clear"
@@ -32,15 +32,15 @@
 
 #: plater.py:260
 msgid "Done"
 msgstr "Կատարված"
 
 #: plater.py:262
 msgid "Cancel"
-msgstr ""
+msgstr "Չեղարկել"
 
 #: plater.py:264
 msgid "Snap to Z = 0"
 msgstr "Փակցնել Z = 0"
 
 #: plater.py:265
 msgid "Put at 100, 100"
```

### Comparing `Printrun-2.0.0rc7/locale/hy/LC_MESSAGES/pronterface.po` & `Printrun-2.0.1/locale/hy/LC_MESSAGES/pronterface.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-# Armenian Pronterface Message Catalog
-#
+# Pronterface
+# Copyright (C) 2011 Jonathan Marsden
+# Jonathan Marsden <jmarsden@fastmail.fm>, 2011.
+# Armenian pronterface translation
 msgid ""
 msgstr ""
 "Project-Id-Version: Pronterface\n"
-"POT-Creation-Date: 2014-03-30 14:35+CEST\n"
-"PO-Revision-Date: 2020-04-17 22:36+0400\n"
+"POT-Creation-Date: 2021-01-21 02:35+0100\n"
+"PO-Revision-Date: 2022-02-27 18:29+0400\n"
+"Last-Translator: Ավագ Սայան <info@armath.am>\n"
+"Language-Team: HY <info@armath.am>\n"
+"Language: hy\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
-"Last-Translator: Avag Sayan <info@armath.am>\n"
-"Language-Team: Armath Engineering Labs, info@armath.am\n"
-"X-Generator: Poedit 2.0.6\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
-"Language: hy_AM\n"
+"X-Generator: Poedit 2.4.2\n"
 
 #: printrun/excluder.py:26
 msgid "Part excluder: draw rectangles where print instructions should be ignored"
 msgstr "Դետալի բացառում` գծել ուղղանկյունի, որտեղ տպման հրահանգները կանտեսվեն"
 
 #: printrun/excluder.py:27 printrun/excluder.py:29
 msgid "Reset selection"
@@ -57,53 +58,53 @@
 
 #: printrun/gui/controls.py:126
 msgid "Heat:"
 msgstr "Գլխիկ՝"
 
 #: printrun/gui/controls.py:129
 msgid "Switch Hotend Off"
-msgstr "Անջատել տաքացումը"
+msgstr "Անջատել գլխիկի տաքացումը"
 
 #: printrun/gui/controls.py:129 printrun/gui/controls.py:149
 #: printrun/gui/toolbar.py:85
 msgid "Off"
-msgstr "ԱՆջատել"
+msgstr "Անջ․"
 
 #: printrun/gui/controls.py:137
 msgid "Select Temperature for Hotend"
 msgstr "Նշել Ջերմաստիճանը Hotend-ի համար"
 
 #: printrun/gui/controls.py:141
 msgid "Switch Hotend On"
-msgstr "Միացնել գլխիկը"
+msgstr "Միացնել գլխիկի տաքացումը"
 
 #: printrun/gui/controls.py:141 printrun/gui/controls.py:161
 #: printrun/gui/controls.py:198
 msgid "Set"
-msgstr "Հաստատել"
+msgstr "Գործել"
 
 #: printrun/gui/controls.py:146 printrun/gui/controls.py:215
 msgid "Bed:"
-msgstr "Հարթակ՝"
+msgstr "Հատակ՝"
 
 #: printrun/gui/controls.py:149
 msgid "Switch Heated Bed Off"
-msgstr "Անջատել տաքացվող հարթակը"
+msgstr "Անջատել հարթակի տաքացումը"
 
 #: printrun/gui/controls.py:157
 msgid "Select Temperature for Heated Bed"
 msgstr "Նշել Տաքացվող հարթակի Ջերմաստիճանը"
 
 #: printrun/gui/controls.py:161
 msgid "Switch Heated Bed On"
-msgstr "Միացնել տաքացվող հարթակը"
+msgstr "Միացնել հարթակը տաքացումը"
 
 #: printrun/gui/controls.py:187
 msgid "Print speed:"
-msgstr "Տպիչի արագություն ՝"
+msgstr "Տպիչի արագ.՝"
 
 #: printrun/gui/controls.py:192 printrun/gui/controls.py:207
 msgid "%d%%"
 msgstr "%d%%"
 
 #: printrun/gui/controls.py:198
 msgid "Set print speed factor"
@@ -111,15 +112,15 @@
 
 #: printrun/gui/controls.py:213
 msgid "Heater:"
 msgstr "Տաքացուցիչ`"
 
 #: printrun/gui/controls.py:265
 msgid "Length:"
-msgstr "Երկարություն`"
+msgstr "Երկ.`"
 
 #: printrun/gui/controls.py:267
 msgid "mm"
 msgstr "մմ"
 
 #: printrun/gui/controls.py:267
 msgid "mm @"
@@ -131,21 +132,23 @@
 
 #: printrun/gui/controls.py:272
 msgid "Extrude / Retract speed (mm/min)"
 msgstr "Դուրս մղել / Հետ քաշել (մմ/ր)"
 
 #: printrun/gui/controls.py:278
 msgid "Speed:"
-msgstr "Արագություն:"
+msgstr "Արագ.`"
 
 #: printrun/gui/controls.py:279
 msgid ""
 "mm/\n"
 "min"
-msgstr " մմ/ր"
+msgstr ""
+"մմ/\n"
+"ր"
 
 #: printrun/gui/controls.py:290
 msgid "Tool:"
 msgstr "Գործիք`"
 
 #: printrun/gui/controls.py:293
 msgid "Click to switch current extruder"
@@ -203,23 +206,23 @@
 
 #: printrun/gui/toolbar.py:32
 msgid ""
 "Communication Settings\n"
 "Click to rescan ports"
 msgstr ""
 "Հաղորդակցման կարգավորումներ\n"
-"Կտտացրեք port-ը կրկին սկանավորելու համար"
+"Սեղմեք կայանը կրկին սկանավորելու համար"
 
 #: printrun/gui/toolbar.py:32
 msgid "Port"
-msgstr "Port"
+msgstr "Կայան"
 
 #: printrun/gui/toolbar.py:37
 msgid "Select Port Printer is connected to"
-msgstr "Տպիչի նշված Port-ը միացված է"
+msgstr "Տպիչի տվյալ կայանըը միացված է"
 
 #: printrun/gui/toolbar.py:46
 msgid "Select Baud rate for printer communication"
 msgstr "Տպիչի հաղորդակցման համար ընտրել փոխանցման արագությունը"
 
 #: printrun/gui/toolbar.py:55 printrun/pronterface.py:1052
 msgid "Connect"
@@ -413,15 +416,15 @@
 
 #: printrun/objectplater.py:73
 msgid "Done"
 msgstr "Կատարված"
 
 #: printrun/objectplater.py:151
 msgid "Autoplating"
-msgstr "Autoplating"
+msgstr "Ինքապատում"
 
 #: printrun/objectplater.py:199
 msgid "Bed full, sorry sir :("
 msgstr "Կներեք, բայց հարթակը լիքն է :("
 
 #: printrun/objectplater.py:209
 msgid "Are you sure you want to clear the grid? All unsaved changes will be lost."
@@ -493,15 +496,15 @@
 
 #: printrun/printcore.py:191 printrun/printcore.py:196
 msgid "Could not connect to %s at baudrate %s:"
 msgstr "Անհնար է միանալ %s  %sbaudrate-ին`"
 
 #: printrun/printcore.py:192
 msgid "Serial error: %s"
-msgstr "Serial-ի սխալ` %s "
+msgstr "Serial-ի սխալ` %s"
 
 #: printrun/printcore.py:197
 msgid "IO error: %s"
 msgstr "IO սխալ ՝ %s"
 
 #: printrun/printcore.py:231
 msgid "Can't read from printer (disconnected?) (SelectError {0}): {1}"
@@ -560,15 +563,15 @@
 
 #: printrun/printcore.py:607
 msgid "Can't write to printer (disconnected?) (SerialException): {0}"
 msgstr "Հնարավոր չէ գրանցել տպիչը (մի գուցե միացված չէ) (SerialException): {0}"
 
 #: printrun/printcore.py:610
 msgid "Socket connection broken, disconnected. ({0}): {1}"
-msgstr "Աղբյուրի միացումը անջատվեց, միացված չե: ({0}): {1}"
+msgstr "Միացման աղբյուրն անջատվեց, միացված չէ: ({0}): {1}"
 
 #: printrun/pronsole.py:72
 msgid "Default: "
 msgstr "Լռելայն ՝"
 
 #: printrun/pronsole.py:73
 msgid "(Control-doubleclick to reset to default value)"
@@ -576,15 +579,15 @@
 
 #: printrun/pronsole.py:108
 msgid "Are you sure you want to reset the setting to the default value: {0!r} ?"
 msgstr "Իրոք ցանկանում եք զրոացնել կարգավորումները բերելով լռելայն արժեքների `{0!r} ?"
 
 #: printrun/pronsole.py:108
 msgid "Confirm set default"
-msgstr "Հաստատել լռելայնի անցումը"
+msgstr "Հաստատել սկզբնադիր սահմանումը"
 
 #: printrun/pronsole.py:258
 msgid "Width"
 msgstr "Հաստություն"
 
 #: printrun/pronsole.py:261
 msgid "Depth"
@@ -592,23 +595,23 @@
 
 #: printrun/pronsole.py:264
 msgid "Height"
 msgstr "Բարձրություն"
 
 #: printrun/pronsole.py:267
 msgid "X offset"
-msgstr "X offset"
+msgstr "X֊ի զրո"
 
 #: printrun/pronsole.py:270
 msgid "Y offset"
-msgstr "Y offset"
+msgstr "Y֊ի զրո"
 
 #: printrun/pronsole.py:273
 msgid "Z offset"
-msgstr "Y offset"
+msgstr "Z-ի զրո"
 
 #: printrun/pronsole.py:276
 msgid "X home pos."
 msgstr "X սկզբնական դիրք"
 
 #: printrun/pronsole.py:279
 msgid "Y home pos."
@@ -616,19 +619,19 @@
 
 #: printrun/pronsole.py:282
 msgid "Z home pos."
 msgstr "Z սկզբնական դիրք"
 
 #: printrun/pronsole.py:301
 msgid "Port used to communicate with printer"
-msgstr "Port-ը օգտագործվում է տպիչին միանալու համար"
+msgstr "Կայանը օգտագործման մեջ է և կապակցված է տպիչին"
 
 #: printrun/pronsole.py:301
 msgid "Serial port"
-msgstr "Հաջորդական port"
+msgstr "Հաջորդական կայան"
 
 #: printrun/pronsole.py:302
 msgid "Baud rate"
 msgstr "Փոխանցման արագություն"
 
 #: printrun/pronsole.py:302
 msgid "Communications Speed"
@@ -1352,15 +1355,15 @@
 
 #: printrun/pronterface.py:655
 msgid " Opens file"
 msgstr "Բացում է նիշքը"
 
 #: printrun/pronterface.py:655
 msgid "&Open..."
-msgstr "&Բացել…"
+msgstr "Բացել…"
 
 #: printrun/pronterface.py:663
 msgid " Clear output console"
 msgstr "Մաքրել վահանակի ելքը"
 
 #: printrun/pronterface.py:663
 msgid "Clear console"
@@ -1372,23 +1375,23 @@
 
 #: printrun/pronterface.py:664
 msgid "E&xit"
 msgstr "Ելք"
 
 #: printrun/pronterface.py:665
 msgid "&File"
-msgstr "&Նիշք"
+msgstr "Նիշք"
 
 #: printrun/pronterface.py:668
 msgid " Edit open file"
 msgstr "Խմբագրել բացվող նիշքը"
 
 #: printrun/pronterface.py:668
 msgid "&Edit..."
-msgstr "&Խմբագրել…"
+msgstr "Խմբագրել…"
 
 #: printrun/pronterface.py:669
 msgid " Compose 3D models into a single plate"
 msgstr "Կազմավորել 3D մոդելները մեկ հարթության մեջ"
 
 #: printrun/pronterface.py:669
 msgid "Plater"
@@ -1416,63 +1419,63 @@
 
 #: printrun/pronterface.py:672
 msgid "Projector"
 msgstr "Պրոյեկտոր"
 
 #: printrun/pronterface.py:673
 msgid "&Tools"
-msgstr "&Գործիքներ"
+msgstr "Գործիքներ"
 
 #: printrun/pronterface.py:676
 msgid " Recover previous print after a disconnect (homes X, Y, restores Z and E status)"
 msgstr "Վերականգնել նախավերջին տպագրությունը (զրոյացնու է դիրքը X, Y, վերականգնում է Z ու E -ի ստատուսը)"
 
 #: printrun/pronterface.py:676
 msgid "Recover"
 msgstr "Վերականգնել"
 
 #: printrun/pronterface.py:679
 msgid "&Advanced"
-msgstr "&Ընդլայնված"
+msgstr "Ընդլայնված"
 
 #: printrun/pronterface.py:686
 msgid "Print &settings"
 msgstr "Տպիչի &կարգավորումներ"
 
 #: printrun/pronterface.py:687
 msgid "&Filament"
-msgstr "&Լցանյութ"
+msgstr "Լցանյութ"
 
 #: printrun/pronterface.py:688
 msgid "&Printer"
-msgstr "&Տպիչ"
+msgstr "Տպիչ"
 
 #: printrun/pronterface.py:694
 msgid "&Slic3r"
-msgstr "&Slic3r"
+msgstr "Slic3r"
 
 #: printrun/pronterface.py:696
 msgid "Failed to load Slic3r configuration:"
 msgstr "Չհաջողվեց բեռնել Slic3r -ի կարգաբերումը:"
 
 #: printrun/pronterface.py:702
 msgid "&Macros"
-msgstr "&Macros"
+msgstr "Macros"
 
 #: printrun/pronterface.py:703
 msgid "<&New...>"
-msgstr "<&Նոր…>"
+msgstr "<Նոր…>"
 
 #: printrun/pronterface.py:704
 msgid " Options dialog"
 msgstr "Ընտրանքի զրուցարան"
 
 #: printrun/pronterface.py:704
 msgid "&Options"
-msgstr "&Ընտրանքներ"
+msgstr "Ընտրանքներ"
 
 #: printrun/pronterface.py:706
 msgid " Adjust slicing settings"
 msgstr "Ճշգրտել շերտավորման կարգավորումը"
 
 #: printrun/pronterface.py:706
 msgid "Slicing settings"
@@ -1484,27 +1487,27 @@
 
 #: printrun/pronterface.py:709
 msgid "Print all G-code sent to and received from the printer."
 msgstr "Տպել տպիչից ուղարկած և ստացած բոլոր G-code-ը"
 
 #: printrun/pronterface.py:713
 msgid "&Settings"
-msgstr "&Կարգավորումներ"
+msgstr "Կարգավորումներ"
 
 #: printrun/pronterface.py:719
 msgid "&About Printrun"
-msgstr "&Printrun-ի մասին"
+msgstr "Printrun-ի մասին"
 
 #: printrun/pronterface.py:719
 msgid "Show about dialog"
 msgstr "Ցուցադրել «մեր մասին» երկխոսությունը"
 
 #: printrun/pronterface.py:720
 msgid "&Help"
-msgstr "&Օգնություն"
+msgstr "Օգնություն"
 
 #: printrun/pronterface.py:746
 msgid "Printrun is a pure Python 3D printing (and other types of CNC) host software."
 msgstr "Printrun-ը Python-ով աշխատող 3D տպագրության (և այլ տիպի CNC-ի համար) ծրագրային ապահովում է:"
 
 #: printrun/pronterface.py:750
 msgid "%.02fmm of filament have been extruded during prints"
@@ -1516,17 +1519,15 @@
 
 #: printrun/pronterface.py:781
 msgid "Regularly monitor printer temperatures (required to have functional temperature graph or gauges)"
 msgstr "Պարբերաբար դիտարկել տպիչի ջերմաստիճանները (պահանջում է ունենալ գործառնական ջերմաստիճանային գրաֆիկա և մեծություններ)"
 
 #: printrun/pronterface.py:782
 msgid "Path to the simarrange binary to use in the STL plater"
-msgstr ""
-"Путь к двоичному файлу симарранж для использования в платтере STL\n"
-"STL նիշքի հարթության համահարթեցման երկուական ուղղությունը:"
+msgstr "STL նիշքի հարթության համահարթեցման երկուական ուղղությունը:"
 
 #: printrun/pronterface.py:782
 msgid "Simarrange command"
 msgstr "Համահարթեցման հրաման"
 
 #: printrun/pronterface.py:783
 msgid "Circular build platform"
@@ -1660,19 +1661,19 @@
 
 #: printrun/pronterface.py:804
 msgid "Width of Extrusion in Preview"
 msgstr "Արտամղման հաստության նախադիտում"
 
 #: printrun/pronterface.py:805
 msgid "Fine Grid Spacing"
-msgstr "Fine Grid Spacing"
+msgstr "Ցանցի փոքր տարածություն"
 
 #: printrun/pronterface.py:805
 msgid "Fine grid spacing"
-msgstr "Fine grid spacing"
+msgstr "Ցանցի փոքր տարածություն"
 
 #: printrun/pronterface.py:806
 msgid "Coarse Grid Spacing"
 msgstr "Կոշտացնել Ցանցի Տարածությունը"
 
 #: printrun/pronterface.py:806
 msgid "Coarse grid spacing"
@@ -1746,14 +1747,22 @@
 msgid "Changing most settings here will require restart to get effect"
 msgstr "Հիմնական կարգավորումների փոփոխությունը կպահանջի վերագործարկել ծրագիրը"
 
 #: printrun/pronterface.py:815
 msgid "Note:"
 msgstr "Նշում ՝"
 
+#: printrun/pronterface.py:820
+msgid "&Recent Files"
+msgstr "Վերջին նիշքերը"
+
+#: printrun/pronterface.py:821
+msgid "Clear console\tCtrl+L"
+msgstr "Մաքրել տերմինալը\tCtrl+L"
+
 #: printrun/pronterface.py:822
 msgid "automatically try to connect to printer on startup"
 msgstr "մեկնարկի ժամանակ ինքնեկ կերպով փորձել միանալ տպիչին"
 
 #: printrun/pronterface.py:835 printrun/pronterface.py:1316
 msgid "Failed to load recent files list:"
 msgstr "Ձախողվեց բեռնել վերջին նիշքերի ցանկը ՝"
@@ -1800,15 +1809,15 @@
 
 #: printrun/pronterface.py:997
 msgid "Could not parse baud rate: "
 msgstr "Չհաջողվեց վերլուծել և ստանալ baud rate-ը:"
 
 #: printrun/pronterface.py:1013 printrun/pronterface.py:1023
 msgid "Error: You are trying to connect to a non-existing port."
-msgstr "Սխալ` դուք ցանկանում եք միանալ գոյություն չունեցող տպիչի port-ին."
+msgstr "Սխալ` դուք ցանկանում եք միանալ գոյություն չունեցող տպիչի կայանին։"
 
 #: printrun/pronterface.py:1015
 msgid "Error: You don't have permission to open %s."
 msgstr "Սխալ` դուք չունեք թույլտվություն բացել %s-ը:"
 
 #: printrun/pronterface.py:1016
 msgid "You might need to add yourself to the dialout group."
@@ -1824,15 +1833,15 @@
 
 #: printrun/pronterface.py:1072
 msgid "Are you sure you want to reset the printer?"
 msgstr "Իրո՞ք ցանկանում եք վերատեղադրել տպիչը:"
 
 #: printrun/pronterface.py:1072
 msgid "Reset?"
-msgstr "Վերատեղադրել?"
+msgstr "Վերատեղադրե՞լ"
 
 #: printrun/pronterface.py:1093
 msgid "Restart"
 msgstr "Վերագործարկել"
 
 #: printrun/pronterface.py:1126
 msgid "Pick SD filename"
@@ -1976,15 +1985,15 @@
 
 #: printrun/pronterface.py:2010
 msgid "Macro name:"
 msgstr "Macro-ի անուն`"
 
 #: printrun/pronterface.py:2013
 msgid "Ok"
-msgstr "Ok"
+msgstr "Լավ"
 
 #: printrun/pronterface.py:2035
 msgid "Macro name may contain only ASCII alphanumeric symbols and underscores"
 msgstr "Macro -ի անունը կարող է պարունակել միայն ASCII այբենական-թվային սիմվոլներ և ընդգծումներ"
 
 #: printrun/pronterface.py:2038
 msgid "Name '%s' is being used by built-in command"
```

### Comparing `Printrun-2.0.0rc7/locale/it/LC_MESSAGES/plater.po` & `Printrun-2.0.1/locale/it/LC_MESSAGES/plater.po`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/locale/it/LC_MESSAGES/pronterface.po` & `Printrun-2.0.1/locale/it/LC_MESSAGES/pronterface.po`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/locale/nl/LC_MESSAGES/pronterface.po` & `Printrun-2.0.1/locale/pronterface.pot`

 * *Files 25% similar despite different names*

```diff
@@ -1,2254 +1,2471 @@
-# Pronterface Message Catalog Dutch
-# Copyright (C) 2011 Ruben Lubbes
-# Ruben Lubbes <ruben.lubbes@gmx.net>, 2011.
+# SOME DESCRIPTIVE TITLE.
+# Copyright (C) YEAR ORGANIZATION
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: Pronterface rl1\n"
-"POT-Creation-Date: 2014-03-30 14:35+CEST\n"
-"PO-Revision-Date: 2011-09-06 16:31+0100\n"
-"Last-Translator: Ruben Lubbes <ruben.lubbes@gmx.net>\n"
-"Language-Team: NL <LL@li.org>\n"
-"Language: \n"
+"Project-Id-Version: PACKAGE VERSION\n"
+"POT-Creation-Date: 2023-02-04 17:27+0100\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=cp1252\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
 
-#: printrun/excluder.py:26
-msgid ""
-"Part excluder: draw rectangles where print instructions should be ignored"
+
+#: printrun\excluder.py:26
+msgid "Part excluder: draw rectangles where print instructions should be ignored"
 msgstr ""
 
-#: printrun/excluder.py:27 printrun/excluder.py:29
+#: printrun\excluder.py:27 printrun\excluder.py:29
 msgid "Reset selection"
 msgstr ""
 
-#: printrun/gcodeplater.py:43 printrun/gcodeplater.py:44
+#: printrun\gcodeplater.py:77 printrun\gcodeplater.py:78
 msgid "GCODE files (*.gcode;*.GCODE;*.g)"
 msgstr ""
 
-#: printrun/gcodeplater.py:112 printrun/gcodeplater.py:152
-msgid "Warning: no rotation support for now, object won't be correctly rotated"
+#: printrun\gcodeplater.py:199 printrun\gcodeplater.py:236
+msgid "Exported merged G-Codes to %s"
+msgstr ""
+
+#: printrun\gcview.py:108
+msgid "Invalid layer for injection"
 msgstr ""
 
-#: printrun/gcodeplater.py:141 printrun/gcodeplater.py:178
-msgid "Exported merged G-Codes to %s"
+#: printrun\gcview.py:116
+msgid "Invalid layer for edition"
 msgstr ""
 
-#: printrun/gcview.py:352
+#: printrun\gcview.py:439
 msgid "Fit to plate"
 msgstr ""
 
-#: printrun/gcview.py:353
+#: printrun\gcview.py:440
 msgid "Fit to plate [F]"
 msgstr ""
 
-#: printrun/gui/__init__.py:19 printrun/pronterface.py:45
-msgid "WX is not installed. This program requires WX to run."
-msgstr "WX is niet geïnstalleerd. Dit programma vereist WX."
+#: printrun\gcview.py:468
+msgid "Layer %d -%s Z = %.03f mm"
+msgstr ""
+
+#: printrun\gcview.py:470 printrun\gcview.py:502
+msgid "Entire object"
+msgstr ""
 
-#: printrun/gui/__init__.py:159
-#, fuzzy
+#: printrun\gcview.py:482
+msgid "G-Code view, can't process slider. Please wait until model is loaded completely."
+msgstr ""
+
+#: printrun\gl\panel.py:172
+msgid "OpenGL failed, disabling it:"
+msgstr ""
+
+#: printrun\gui\__init__.py:23 printrun\pronterface.py:49
+msgid "WX >= 4 is not installed. This program requires WX >= 4 to run."
+msgstr ""
+
+#: printrun\gui\__init__.py:185
 msgid "Commands"
-msgstr "Commando"
+msgstr ""
 
-#: printrun/gui/__init__.py:160
+#: printrun\gui\__init__.py:186
 msgid "Status"
 msgstr ""
 
-#: printrun/gui/controls.py:126
-#, fuzzy
+#: printrun\gui\__init__.py:187 printrun\pronterface.py:290
+#: printrun\pronterface.py:627
+msgid "Tabbed with platers"
+msgstr ""
+
+#: printrun\gui\__init__.py:203 printrun\pronterface.py:830
+msgid "Plater"
+msgstr ""
+
+#: printrun\gui\__init__.py:204 printrun\pronterface.py:831
+msgid "G-Code Plater"
+msgstr ""
+
+#: printrun\gui\controls.py:32
+msgid "[J]og controls. (Shift)+TAB ESC Shift/Ctrl+(arrows PgUp/PgDn)"
+msgstr ""
+
+#: printrun\gui\controls.py:131
 msgid "Heat:"
-msgstr "Element:"
+msgstr ""
 
-#: printrun/gui/controls.py:129
+#: printrun\gui\controls.py:133
 msgid "Switch Hotend Off"
 msgstr ""
 
-#: printrun/gui/controls.py:129 printrun/gui/controls.py:149
-#: printrun/gui/toolbar.py:85
+#: printrun\gui\controls.py:133 printrun\gui\controls.py:149
+#: printrun\gui\toolbar.py:86
 msgid "Off"
 msgstr ""
 
-#: printrun/gui/controls.py:137
-msgid "Select Temperature for Hotend"
+#: printrun\gui\controls.py:138
+msgid "Select Temperature for [H]otend"
 msgstr ""
 
-#: printrun/gui/controls.py:141
+#: printrun\gui\controls.py:142
 msgid "Switch Hotend On"
 msgstr ""
 
-#: printrun/gui/controls.py:141 printrun/gui/controls.py:161
-#: printrun/gui/controls.py:198
+#: printrun\gui\controls.py:142 printrun\gui\controls.py:158
+#: printrun\gui\controls.py:191 printrun\gui\controls.py:225
 msgid "Set"
-msgstr "Stel in"
+msgstr ""
 
-#: printrun/gui/controls.py:146 printrun/gui/controls.py:215
+#: printrun\gui\controls.py:147 printrun\gui\controls.py:250
 msgid "Bed:"
-msgstr "Bed:"
+msgstr ""
 
-#: printrun/gui/controls.py:149
+#: printrun\gui\controls.py:149
 msgid "Switch Heated Bed Off"
 msgstr ""
 
-#: printrun/gui/controls.py:157
-msgid "Select Temperature for Heated Bed"
+#: printrun\gui\controls.py:154
+msgid "Select Temperature for Heated [B]ed"
 msgstr ""
 
-#: printrun/gui/controls.py:161
+#: printrun\gui\controls.py:158
 msgid "Switch Heated Bed On"
 msgstr ""
 
-#: printrun/gui/controls.py:187
+#: printrun\gui\controls.py:177
 msgid "Print speed:"
 msgstr ""
 
-#: printrun/gui/controls.py:192 printrun/gui/controls.py:207
-msgid "%d%%"
+#: printrun\gui\controls.py:185 printrun\gui\controls.py:219
+msgid "%"
 msgstr ""
 
-#: printrun/gui/controls.py:198
+#: printrun\gui\controls.py:191
 msgid "Set print speed factor"
 msgstr ""
 
-#: printrun/gui/controls.py:213
+#: printrun\gui\controls.py:212
+msgid "Print flow:"
+msgstr ""
+
+#: printrun\gui\controls.py:225
+msgid "Set print flow factor"
+msgstr ""
+
+#: printrun\gui\controls.py:246
 msgid "Heater:"
-msgstr "Element:"
+msgstr ""
 
-#: printrun/gui/controls.py:265
+#: printrun\gui\controls.py:307
 msgid "Length:"
 msgstr ""
 
-#: printrun/gui/controls.py:267
+#: printrun\gui\controls.py:309
 msgid "mm"
-msgstr "mm"
+msgstr ""
 
-#: printrun/gui/controls.py:267
+#: printrun\gui\controls.py:309
 msgid "mm @"
 msgstr ""
 
-#: printrun/gui/controls.py:269
+#: printrun\gui\controls.py:311
 msgid "Amount to Extrude or Retract (mm)"
 msgstr ""
 
-#: printrun/gui/controls.py:272
+#: printrun\gui\controls.py:316
 msgid "Extrude / Retract speed (mm/min)"
 msgstr ""
 
-#: printrun/gui/controls.py:278
+#: printrun\gui\controls.py:321
 msgid "Speed:"
 msgstr ""
 
-#: printrun/gui/controls.py:279
+#: printrun\gui\controls.py:322
 msgid ""
 "mm/\n"
 "min"
 msgstr ""
 
-#: printrun/gui/controls.py:290
+#: printrun\gui\controls.py:333
 msgid "Tool:"
 msgstr ""
 
-#: printrun/gui/controls.py:293
+#: printrun\gui\controls.py:336
 msgid "Click to switch current extruder"
 msgstr ""
 
-#: printrun/gui/controls.py:310
+#: printrun\gui\controls.py:353
 msgid "Select current extruder"
 msgstr ""
 
-#: printrun/gui/controls.py:371
+#: printrun\gui\controls.py:414
 msgid "Set Maximum Speed for X & Y axes (mm/min)"
 msgstr ""
 
-#: printrun/gui/controls.py:372
+#: printrun\gui\controls.py:415
 msgid "XY:"
-msgstr "XY:"
+msgstr ""
 
-#: printrun/gui/controls.py:374
-#, fuzzy
+#: printrun\gui\controls.py:417
 msgid "mm/min Z:"
-msgstr "mm/min"
+msgstr ""
 
-#: printrun/gui/controls.py:376
+#: printrun\gui\controls.py:419
 msgid "Set Maximum Speed for Z axis (mm/min)"
 msgstr ""
 
-#: printrun/gui/graph.py:28
+#: printrun\gui\graph.py:27
 msgid "Temperature graph"
 msgstr ""
 
-#: printrun/gui/log.py:32
+#: printrun\gui\log.py:32
 msgid ""
 "Send commands to printer\n"
 "(Type 'help' for simple\n"
 "help function)"
 msgstr ""
 
-#: printrun/gui/log.py:39
+#: printrun\gui\log.py:46
 msgid "Send"
-msgstr "Zend"
+msgstr ""
 
-#: printrun/gui/log.py:39
-#, fuzzy
+#: printrun\gui\log.py:46
 msgid "Send Command to Printer"
-msgstr "Printercommunicatie volgen"
+msgstr ""
 
-#: printrun/gui/toolbar.py:23
+#: printrun\gui\toolbar.py:23
 msgid "Lock"
 msgstr ""
 
-#: printrun/gui/toolbar.py:25
+#: printrun\gui\toolbar.py:25
 msgid "Lock graphical interface"
 msgstr ""
 
-#: printrun/gui/toolbar.py:32
+#: printrun\gui\toolbar.py:32
 msgid ""
 "Communication Settings\n"
 "Click to rescan ports"
 msgstr ""
 
-#: printrun/gui/toolbar.py:32
+#: printrun\gui\toolbar.py:32
 msgid "Port"
-msgstr "Poort"
+msgstr ""
 
-#: printrun/gui/toolbar.py:37
+#: printrun\gui\toolbar.py:37
 msgid "Select Port Printer is connected to"
 msgstr ""
 
-#: printrun/gui/toolbar.py:46
+#: printrun\gui\toolbar.py:46
 msgid "Select Baud rate for printer communication"
 msgstr ""
 
-#: printrun/gui/toolbar.py:55 printrun/pronterface.py:1052
-msgid "Connect"
-msgstr "Verbind"
+#: printrun\gui\toolbar.py:56 printrun\pronterface.py:1370
+msgid "&Connect"
+msgstr ""
 
-#: printrun/gui/toolbar.py:55 printrun/pronterface.py:1053
+#: printrun\gui\toolbar.py:56 printrun\pronterface.py:1371
 msgid "Connect to the printer"
-msgstr "Verbind met printer"
+msgstr ""
 
-#: printrun/gui/toolbar.py:61
+#: printrun\gui\toolbar.py:62
 msgid "Reset"
-msgstr "Reset"
+msgstr ""
 
-#: printrun/gui/toolbar.py:61
-#, fuzzy
+#: printrun\gui\toolbar.py:62
 msgid "Reset the printer"
-msgstr "Verbind met printer"
+msgstr ""
 
-#: printrun/gui/toolbar.py:69
-#, fuzzy
+#: printrun\gui\toolbar.py:70
 msgid "Load a 3D model file"
-msgstr "open bestand"
+msgstr ""
 
-#: printrun/gui/toolbar.py:69
+#: printrun\gui\toolbar.py:70 printrun\pronterface.py:1578
 msgid "Load file"
-msgstr "open bestand"
+msgstr ""
 
-#: printrun/gui/toolbar.py:70
+#: printrun\gui\toolbar.py:71
 msgid "SD"
 msgstr ""
 
-#: printrun/gui/toolbar.py:70
-#, fuzzy
+#: printrun\gui\toolbar.py:71
 msgid "SD Card Printing"
-msgstr "Afdruk van SD"
-
-#: printrun/gui/toolbar.py:74
-msgid "Start Printing Loaded File"
 msgstr ""
 
-#: printrun/gui/toolbar.py:74 printrun/pronterface.py:1003
-#: printrun/pronterface.py:1062 printrun/pronterface.py:1078
-#: printrun/pronterface.py:1363 printrun/pronterface.py:1445
+#: printrun\gui\toolbar.py:75
 msgid "Print"
-msgstr "Printen"
+msgstr ""
 
-#: printrun/gui/toolbar.py:80
-msgid "Pause Current Print"
+#: printrun\gui\toolbar.py:75
+msgid "Start Printing Loaded File"
 msgstr ""
 
-#: printrun/gui/toolbar.py:80 printrun/pronterface.py:1002
-#: printrun/pronterface.py:1061 printrun/pronterface.py:1081
-#: printrun/pronterface.py:1091 printrun/pronterface.py:1172
-#: printrun/pronterface.py:1364
+#: printrun\gui\toolbar.py:81
 msgid "Pause"
-msgstr "Pauze"
+msgstr ""
 
-#: printrun/gui/toolbar.py:85
+#: printrun\gui\toolbar.py:81
+msgid "Pause Current Print"
+msgstr ""
+
+#: printrun\gui\toolbar.py:86
 msgid "Turn printer off"
 msgstr ""
 
-#: printrun/gui/viz.py:65
+#: printrun\gui\viz.py:91
 msgid ""
 "Click to examine / edit\n"
 "  layers of loaded file"
 msgstr ""
 
-#: printrun/gui/widgets.py:36
+#: printrun\gui\widgets.py:35
 msgid "Find"
 msgstr ""
 
-#: printrun/gui/widgets.py:38
+#: printrun\gui\widgets.py:37
 msgid "Save"
 msgstr ""
 
-#: printrun/gui/widgets.py:43 printrun/objectplater.py:76
-#: printrun/pronterface.py:1257 printrun/pronterface.py:2017
+#: printrun\gui\widgets.py:42 printrun\objectplater.py:79
+#: printrun\pronterface.py:1581 printrun\pronterface.py:2427
 msgid "Cancel"
-msgstr "Annuleer"
+msgstr ""
 
-#: printrun/gui/widgets.py:70
-#, fuzzy
+#: printrun\gui\widgets.py:68
 msgid "Not Found!"
-msgstr "Bestand niet gevonden!"
+msgstr ""
 
-#: printrun/gui/widgets.py:124
-#, fuzzy
+#: printrun\gui\widgets.py:119
 msgid "Printer settings"
-msgstr "Wijzig instellingen"
+msgstr ""
 
-#: printrun/gui/widgets.py:125
-#, fuzzy
+#: printrun\gui\widgets.py:120
 msgid "User interface"
-msgstr "Printer Interface"
+msgstr ""
 
-#: printrun/gui/widgets.py:126
-#, fuzzy
+#: printrun\gui\widgets.py:121
+msgid "Viewer"
+msgstr ""
+
+#: printrun\gui\widgets.py:122
 msgid "Colors"
-msgstr "Kleur"
+msgstr ""
 
-#: printrun/gui/widgets.py:127
+#: printrun\gui\widgets.py:123
 msgid "External commands"
 msgstr ""
 
-#: printrun/gui/widgets.py:132
+#: printrun\gui\widgets.py:128
 msgid "Edit settings"
-msgstr "Wijzig instellingen"
+msgstr ""
 
-#: printrun/gui/widgets.py:135
-#, fuzzy
+#: printrun\gui\widgets.py:131
 msgid "Settings"
-msgstr "&Instellingen"
+msgstr ""
 
-#: printrun/gui/widgets.py:187
+#: printrun\gui\widgets.py:202
 msgid "Custom button"
-msgstr "Gedefinieerde knop"
+msgstr ""
 
-#: printrun/gui/widgets.py:193
+#: printrun\gui\widgets.py:208
 msgid "Button title"
-msgstr "Knoptitel"
+msgstr ""
 
-#: printrun/gui/widgets.py:196
+#: printrun\gui\widgets.py:211
 msgid "Command"
-msgstr "Commando"
+msgstr ""
 
-#: printrun/gui/widgets.py:205
+#: printrun\gui\widgets.py:220
 msgid "Color"
-msgstr "Kleur"
+msgstr ""
 
-#: printrun/gviz.py:29
+#: printrun\gviz.py:31
 msgid "Layer number and Z position show here when you scroll"
 msgstr ""
 
-#: printrun/gviz.py:39
+#: printrun\gviz.py:41
 msgid "Zoom In [+]"
 msgstr ""
 
-#: printrun/gviz.py:40
+#: printrun\gviz.py:42
 msgid "Zoom Out [-]"
 msgstr ""
 
-#: printrun/gviz.py:42
+#: printrun\gviz.py:44
 msgid "Move Up a Layer [U]"
 msgstr ""
 
-#: printrun/gviz.py:43
+#: printrun\gviz.py:45
 msgid "Move Down a Layer [D]"
 msgstr ""
 
-#: printrun/gviz.py:44
-#, fuzzy
+#: printrun\gviz.py:46
 msgid "Reset view"
-msgstr "Reset"
-
-#: printrun/gviz.py:68
-msgid "Gcode view, shift to move view, mousewheel to set layer"
 msgstr ""
 
-#: printrun/gviz.py:105 printrun/gviz.py:241
-msgid "Layer %d - Going Up - Z = %.03f mm"
+#: printrun\gviz.py:48
+msgid "Inject G-Code"
 msgstr ""
 
-#: printrun/gviz.py:250
-msgid "Layer %d - Going Down - Z = %.03f mm"
+#: printrun\gviz.py:48
+msgid "Insert code at the beginning of this layer"
 msgstr ""
 
-#: printrun/objectplater.py:35
-msgid "Plate building tool"
+#: printrun\gviz.py:49
+msgid "Edit layer"
 msgstr ""
 
-#: printrun/objectplater.py:45
-msgid "Clear"
+#: printrun\gviz.py:49
+msgid "Edit the G-Code of this layer"
 msgstr ""
 
-#: printrun/objectplater.py:49
-#, fuzzy
-msgid "Load"
-msgstr "Geladen "
-
-#: printrun/objectplater.py:53
-msgid "Snap to Z = 0"
+#: printrun\gviz.py:73
+msgid "Gcode view, shift to move view, mousewheel to set layer"
 msgstr ""
 
-#: printrun/objectplater.py:57
-msgid "Put at center"
+#: printrun\gviz.py:109
+msgid "Layer %d - Z = %.03f mm"
 msgstr ""
 
-#: printrun/objectplater.py:61
-msgid "Delete"
+#: printrun\gviz.py:251
+msgid "Layer %d - Going Up - Z = %.03f mm"
 msgstr ""
 
-#: printrun/objectplater.py:65
-msgid "Auto arrange"
+#: printrun\gviz.py:260
+msgid "Layer %d - Going Down - Z = %.03f mm"
 msgstr ""
 
-#: printrun/objectplater.py:69
-msgid "Export"
+#: printrun\injectgcode.py:27
+msgid "Inject G-Code at layer %d (Z = %.03f)"
 msgstr ""
 
-#: printrun/objectplater.py:73
-msgid "Done"
+#: printrun\injectgcode.py:35
+msgid "Edit G-Code of layer %d (Z = %.03f)"
 msgstr ""
 
-#: printrun/objectplater.py:151
-msgid "Autoplating"
+#: printrun\injectgcode.py:40
+msgid "Successfully injected %d lines at beginning of layer %d"
 msgstr ""
 
-#: printrun/objectplater.py:199
-msgid "Bed full, sorry sir :("
+#: printrun\injectgcode.py:45
+msgid "Successfully edited layer %d (which now contains %d lines)"
 msgstr ""
 
-#: printrun/objectplater.py:209
-msgid ""
-"Are you sure you want to clear the grid? All unsaved changes will be lost."
+#: printrun\objectplater.py:44
+msgid "Load"
 msgstr ""
 
-#: printrun/objectplater.py:210
-#, fuzzy
-msgid "Clear the grid?"
-msgstr " Sluit het venster"
+#: printrun\objectplater.py:48
+msgid "Export"
+msgstr ""
 
-#: printrun/objectplater.py:256
-#, fuzzy
-msgid "Pick file to load"
-msgstr "Kies bestand op SD"
+#: printrun\objectplater.py:56
+msgid "Clear"
+msgstr ""
 
-#: printrun/objectplater.py:267
-#, fuzzy
-msgid "Pick file to save to"
-msgstr "Kies bestandsnaam op SD"
+#: printrun\objectplater.py:60
+msgid "Snap to Z = 0"
+msgstr ""
 
-#: printrun/plater.py:212
-msgid "STL files (*.stl;*.STL)|*.stl;*.STL|OpenSCAD files (*.scad)|*.scad"
+#: printrun\objectplater.py:64
+msgid "Put at center"
 msgstr ""
 
-#: printrun/plater.py:213
-msgid "STL files (*.stl;*.STL)|*.stl;*.STL"
+#: printrun\objectplater.py:68
+msgid "Delete"
 msgstr ""
 
-#: printrun/plater.py:244
-#, fuzzy
-msgid "Loading STL file failed"
-msgstr "Bestand openen mislukt"
+#: printrun\objectplater.py:72
+msgid "Auto arrange"
+msgstr ""
 
-#: printrun/plater.py:244 printrun/plater.py:251
-msgid "Error"
+#: printrun\objectplater.py:76
+msgid "Done"
 msgstr ""
 
-#: printrun/plater.py:251
-#, fuzzy
-msgid "Loading OpenSCAD file failed"
-msgstr "Bestand openen mislukt"
+#: printrun\objectplater.py:150
+msgid "Autoplating"
+msgstr ""
 
-#: printrun/plater.py:284
-msgid "Couldn't load non-existing file %s"
+#: printrun\objectplater.py:197
+msgid "Bed full, sorry sir :("
 msgstr ""
 
-#: printrun/plater.py:360
-msgid "Wrote plate to %s"
+#: printrun\objectplater.py:209
+msgid "Are you sure you want to clear the grid? All unsaved changes will be lost."
 msgstr ""
 
-#: printrun/plater.py:367
-msgid ""
-"Failed to use simarrange for plating, falling back to the standard method"
+#: printrun\objectplater.py:210
+msgid "Clear the grid?"
 msgstr ""
 
-#: printrun/plater.py:372
-msgid "Autoplating using simarrange"
+#: printrun\objectplater.py:260
+msgid "Pick file to load"
 msgstr ""
 
-#: printrun/plater.py:387
-msgid "Plate full, please remove some objects"
+#: printrun\objectplater.py:271
+msgid "Pick file to save to"
 msgstr ""
 
-#: printrun/plater.py:404
-msgid "simarrange failed"
+#: printrun\objectplater.py:288
+msgid "Plate building tool"
 msgstr ""
 
-#: printrun/printcore.py:177
+#: printrun\printcore.py:235
 msgid "Could not connect to %s:%s:"
 msgstr ""
 
-#: printrun/printcore.py:178
+#: printrun\printcore.py:236
 msgid "Socket error %s:"
 msgstr ""
 
-#: printrun/printcore.py:191 printrun/printcore.py:196
+#: printrun\printcore.py:264 printrun\printcore.py:269
 msgid "Could not connect to %s at baudrate %s:"
 msgstr ""
 
-#: printrun/printcore.py:192
+#: printrun\printcore.py:265
 msgid "Serial error: %s"
 msgstr ""
 
-#: printrun/printcore.py:197
+#: printrun\printcore.py:270
 msgid "IO error: %s"
 msgstr ""
 
-#: printrun/printcore.py:231
-msgid "Can't read from printer (disconnected?) (SelectError {0}): {1}"
+#: printrun\printcore.py:335
+msgid "Can't read from printer (disconnected?). line_bytes is None"
 msgstr ""
 
-#: printrun/printcore.py:234
-msgid "SelectError ({0}): {1}"
+#: printrun\printcore.py:350
+msgid "Got rubbish reply from %s at baudrate %s:"
+msgstr ""
+
+#: printrun\printcore.py:351
+msgid "Maybe a bad baudrate?"
 msgstr ""
 
-#: printrun/printcore.py:237
+#: printrun\printcore.py:354
 msgid "Can't read from printer (disconnected?) (SerialException): {0}"
 msgstr ""
 
-#: printrun/printcore.py:240
+#: printrun\printcore.py:357
 msgid "Can't read from printer (disconnected?) (Socket error {0}): {1}"
 msgstr ""
 
-#: printrun/printcore.py:245
+#: printrun\printcore.py:364
+msgid "Can't read from printer (disconnected?) (SelectError {0}): {1}"
+msgstr ""
+
+#: printrun\printcore.py:367
+msgid "SelectError ({0}): {1}"
+msgstr ""
+
+#: printrun\printcore.py:373
 msgid "Can't read from printer (disconnected?) (OS Error {0}): {1}"
 msgstr ""
 
-#: printrun/printcore.py:259
+#: printrun\printcore.py:387
 msgid "Aborting connection attempt after 4 failed writes."
 msgstr ""
 
-#: printrun/printcore.py:462 printrun/printcore.py:470
-#: printrun/pronsole.py:1192 printrun/pronsole.py:1250
-#: printrun/pronterface.py:209 printrun/pronterface.py:962
-#: printrun/pronterface.py:1111 printrun/pronterface.py:1178
+#: printrun\printcore.py:594 printrun\printcore.py:602
+#: printrun\pronsole.py:1043 printrun\pronsole.py:1101
+#: printrun\pronterface.py:223 printrun\pronterface.py:1293
+#: printrun\pronterface.py:1429 printrun\pronterface.py:1502
 msgid "Not connected to printer."
-msgstr "Printer is niet verbonden."
+msgstr ""
 
-#: printrun/printcore.py:479
+#: printrun\printcore.py:614
 msgid "Print start callback failed with:"
 msgstr ""
 
-#: printrun/printcore.py:490
+#: printrun\printcore.py:628
 msgid "Print end callback failed with:"
 msgstr ""
 
-#: printrun/printcore.py:493
+#: printrun\printcore.py:631
 msgid "Print thread died due to the following error:"
 msgstr ""
 
-#: printrun/printcore.py:584
+#: printrun\printcore.py:735
 msgid "Could not analyze command %s:"
 msgstr ""
 
-#: printrun/printcore.py:601
+#: printrun\printcore.py:756
 msgid "Can't write to printer (disconnected ?):"
 msgstr ""
 
-#: printrun/printcore.py:604
+#: printrun\printcore.py:759
 msgid "Can't write to printer (disconnected?) (Socket error {0}): {1}"
 msgstr ""
 
-#: printrun/printcore.py:607
+#: printrun\printcore.py:762
 msgid "Can't write to printer (disconnected?) (SerialException): {0}"
 msgstr ""
 
-#: printrun/printcore.py:610
+#: printrun\printcore.py:765
 msgid "Socket connection broken, disconnected. ({0}): {1}"
 msgstr ""
 
-#: printrun/pronsole.py:72
-#, fuzzy
-msgid "Default: "
-msgstr "Standaardinstelling"
-
-#: printrun/pronsole.py:73
-msgid "(Control-doubleclick to reset to default value)"
+#: printrun\pronsole.py:183
+msgid "Build dimensions"
 msgstr ""
 
-#: printrun/pronsole.py:108
-#, fuzzy
+#: printrun\pronsole.py:183
 msgid ""
-"Are you sure you want to reset the setting to the default value: {0!r} ?"
-msgstr "Weet je zeker dat je de printer wilt resetten?"
-
-#: printrun/pronsole.py:108
-msgid "Confirm set default"
-msgstr ""
-
-#: printrun/pronsole.py:258
-msgid "Width"
-msgstr ""
-
-#: printrun/pronsole.py:261
-msgid "Depth"
-msgstr ""
-
-#: printrun/pronsole.py:264
-msgid "Height"
-msgstr ""
-
-#: printrun/pronsole.py:267
-msgid "X offset"
-msgstr ""
-
-#: printrun/pronsole.py:270
-msgid "Y offset"
-msgstr ""
-
-#: printrun/pronsole.py:273
-msgid "Z offset"
-msgstr ""
-
-#: printrun/pronsole.py:276
-msgid "X home pos."
-msgstr ""
-
-#: printrun/pronsole.py:279
-msgid "Y home pos."
-msgstr ""
-
-#: printrun/pronsole.py:282
-msgid "Z home pos."
-msgstr ""
-
-#: printrun/pronsole.py:301
-#, fuzzy
-msgid "Port used to communicate with printer"
-msgstr "Printer is niet verbonden."
-
-#: printrun/pronsole.py:301
-msgid "Serial port"
-msgstr ""
-
-#: printrun/pronsole.py:302
-msgid "Baud rate"
+"Dimensions of Build Platform\n"
+" & optional offset of origin\n"
+" & optional switch position\n"
+"\n"
+"Examples:\n"
+"   XXXxYYY\n"
+"   XXX,YYY,ZZZ\n"
+"   XXXxYYYxZZZ+OffX+OffY+OffZ\n"
+"XXXxYYYxZZZ+OffX+OffY+OffZ+HomeX+HomeY+HomeZ"
 msgstr ""
 
-#: printrun/pronsole.py:302
-msgid "Communications Speed"
+#: printrun\pronsole.py:213
+msgid "Welcome to the printer console! Type \"help\" for a list of available commands."
 msgstr ""
 
-#: printrun/pronsole.py:303
-msgid "TCP streaming mode"
+#: printrun\pronsole.py:401 printrun\pronsole.py:409 printrun\pronsole.py:1452
+#: printrun\pronsole.py:1479 printrun\pronsole.py:1551
+#: printrun\pronterface.py:472 printrun\pronterface.py:492
+#: printrun\pronterface.py:509 printrun\pronterface.py:524
+msgid "Printer is not online."
 msgstr ""
 
-#: printrun/pronsole.py:303
+#: printrun\pronsole.py:424
 msgid ""
-"When using a TCP connection to the printer, the streaming mode will not wait "
-"for acks from the printer to send new commands. This will break things such "
-"as ETA prediction, but can result in smoother prints."
-msgstr ""
-
-#: printrun/pronsole.py:304
-msgid "Bed temperature for ABS"
-msgstr ""
-
-#: printrun/pronsole.py:304
-msgid "Heated Build Platform temp for ABS (deg C)"
-msgstr ""
-
-#: printrun/pronsole.py:305
-msgid "Bed temperature for PLA"
-msgstr ""
-
-#: printrun/pronsole.py:305
-msgid "Heated Build Platform temp for PLA (deg C)"
-msgstr ""
-
-#: printrun/pronsole.py:306
-msgid "Extruder temp for ABS (deg C)"
-msgstr ""
-
-#: printrun/pronsole.py:306
-msgid "Extruder temperature for ABS"
+"Are you sure you want to exit while printing?\n"
+"(this will terminate the print)."
 msgstr ""
 
-#: printrun/pronsole.py:307
-msgid "Extruder temp for PLA (deg C)"
-msgstr ""
-
-#: printrun/pronsole.py:307
-msgid "Extruder temperature for PLA"
-msgstr ""
-
-#: printrun/pronsole.py:308
-msgid "Feedrate for Control Panel Moves in X and Y (mm/min)"
+#: printrun\pronsole.py:428
+msgid "Exiting program. Goodbye!"
 msgstr ""
 
-#: printrun/pronsole.py:308
-msgid "X && Y manual feedrate"
+#: printrun\pronsole.py:434
+msgid "Disconnects from the printer and exits the program."
 msgstr ""
 
-#: printrun/pronsole.py:309
-msgid "Feedrate for Control Panel Moves in Z (mm/min)"
+#: printrun\pronsole.py:591
+msgid "Unknown variable '%s'"
 msgstr ""
 
-#: printrun/pronsole.py:309
-msgid "Z manual feedrate"
+#: printrun\pronsole.py:594
+msgid "Bad value %s for variable '%s': %s"
 msgstr ""
 
-#: printrun/pronsole.py:310
-msgid "E manual feedrate"
+#: printrun\pronsole.py:596
+msgid "Bad value for variable '%s', expecting %s (%s)"
 msgstr ""
 
-#: printrun/pronsole.py:310
-msgid "Feedrate for Control Panel Moves in Extrusions (mm/min)"
+#: printrun\pronsole.py:752
+msgid "increase verbosity"
 msgstr ""
 
-#: printrun/pronsole.py:311
-#, fuzzy
-msgid "Slice command"
-msgstr "Commando"
-
-#: printrun/pronsole.py:312
-#, fuzzy
-msgid "Slice settings command"
-msgstr "SFACT Instellingen"
-
-#: printrun/pronsole.py:312
-msgid "Slicer options command"
+#: printrun\pronsole.py:753
+msgid "load this file on startup instead of .pronsolerc ; you may chain config files, if so settings auto-save will use the last specified file"
 msgstr ""
 
-#: printrun/pronsole.py:313
-msgid "Executable to run when the print is finished"
+#: printrun\pronsole.py:754
+msgid "executes command after configuration/.pronsolerc is loaded ; macros/settings from these commands are not autosaved"
 msgstr ""
 
-#: printrun/pronsole.py:313
-#, fuzzy
-msgid "Final command"
-msgstr "Commando"
-
-#: printrun/pronsole.py:314
-#, fuzzy
-msgid "Error command"
-msgstr "Commando"
-
-#: printrun/pronsole.py:314
-msgid "Executable to run when an error occurs"
-msgstr ""
-
-#: printrun/pronsole.py:381
-msgid "Failed to run callback after setting \"%s\":"
-msgstr ""
-
-#: printrun/pronsole.py:469
-msgid "Build dimensions"
-msgstr ""
-
-#: printrun/pronsole.py:469
-msgid ""
-"Dimensions of Build Platform\n"
-" & optional offset of origin\n"
-" & optional switch position\n"
-"\n"
-"Examples:\n"
-"   XXXxYYY\n"
-"   XXX,YYY,ZZZ\n"
-"   XXXxYYYxZZZ+OffX+OffY+OffZ\n"
-"XXXxYYYxZZZ+OffX+OffY+OffZ+HomeX+HomeY+HomeZ"
-msgstr ""
-
-#: printrun/pronsole.py:495
-msgid ""
-"Welcome to the printer console! Type \"help\" for a list of available "
-"commands."
+#: printrun\pronsole.py:755
+msgid "file to load"
 msgstr ""
 
-#: printrun/pronsole.py:657 printrun/pronsole.py:665 printrun/pronsole.py:673
-#: printrun/pronsole.py:1519 printrun/pronsole.py:1546
-#: printrun/pronsole.py:1618 printrun/pronterface.py:357
-#: printrun/pronterface.py:377 printrun/pronterface.py:394
-msgid "Printer is not online."
-msgstr "Printer is niet verbonden."
-
-#: printrun/pronsole.py:692
-msgid "Exiting program. Goodbye!"
+#: printrun\pronsole.py:799 printrun\pronsole.py:809
+msgid "Error: You are trying to connect to a non-existing port."
 msgstr ""
 
-#: printrun/pronsole.py:697
-msgid "Disconnects from the printer and exits the program."
+#: printrun\pronsole.py:801
+msgid "Error: You don't have permission to open %s."
 msgstr ""
 
-#: printrun/pronsole.py:974
-msgid ""
-"load this file on startup instead of .pronsolerc ; you may chain config "
-"files, if so settings auto-save will use the last specified file"
+#: printrun\pronsole.py:802
+msgid "You might need to add yourself to the dialout group."
 msgstr ""
 
-#: printrun/pronsole.py:975
-msgid ""
-"executes command after configuration/.pronsolerc is loaded ; macros/settings "
-"from these commands are not autosaved"
+#: printrun\pronsole.py:911
+msgid "Disconnecting after 4 failed writes."
 msgstr ""
 
-#: printrun/pronsole.py:976
-msgid "file to load"
+#: printrun\pronsole.py:951 printrun\pronterface.py:1666
+msgid "Loading file: %s"
 msgstr ""
 
-#: printrun/pronsole.py:1104
-#, fuzzy
+#: printrun\pronsole.py:956
 msgid "Loaded %s, %d lines."
-msgstr "Geladen %s, %d regels"
+msgstr ""
 
-#: printrun/pronsole.py:1105 printrun/pronterface.py:1381
+#: printrun\pronsole.py:957 printrun\pronterface.py:1773
 msgid "Estimated duration: %d layers, %s"
 msgstr ""
 
-#: printrun/pronsole.py:1134
+#: printrun\pronsole.py:986
 msgid "No file name given."
 msgstr ""
 
-#: printrun/pronsole.py:1140
-msgid "Skeining file: %s"
+#: printrun\pronsole.py:992
+msgid "Slicing file: %s"
 msgstr ""
 
-#: printrun/pronsole.py:1142 printrun/pronterface.py:1305
+#: printrun\pronsole.py:994 printrun\pronterface.py:1634
 msgid "File not found!"
-msgstr "Bestand niet gevonden!"
+msgstr ""
 
-#: printrun/pronsole.py:1147
+#: printrun\pronsole.py:999
 msgid "Entering slicer settings: %s"
 msgstr ""
 
-#: printrun/pronsole.py:1151
-#, fuzzy
-msgid "Slicing: "
-msgstr "Skeinforge draait"
-
-#: printrun/pronsole.py:1158
-#, fuzzy
+#: printrun\pronsole.py:1009
 msgid "Loading sliced file."
-msgstr "open bestand"
+msgstr ""
 
-#: printrun/pronsole.py:1161
-#, fuzzy
+#: printrun\pronsole.py:1012
 msgid "Slicing failed: %s"
-msgstr "Skeinforge draait"
+msgstr ""
 
-#: printrun/pronsole.py:1174
-msgid ""
-"Creates a gcode file from an stl model using the slicer (with tab-completion)"
+#: printrun\pronsole.py:1025
+msgid "Creates a gcode file from an stl model using the slicer (with tab-completion)"
 msgstr ""
 
-#: printrun/pronsole.py:1175
+#: printrun\pronsole.py:1026
 msgid "slice filename.stl - create gcode file"
 msgstr ""
 
-#: printrun/pronsole.py:1176
-msgid ""
-"slice filename.stl view - create gcode file and view using skeiniso (if "
-"using skeinforge)"
+#: printrun\pronsole.py:1027
+msgid "slice filename.stl view - create gcode file and view using skeiniso (if using skeinforge)"
 msgstr ""
 
-#: printrun/pronsole.py:1177
-#, fuzzy
+#: printrun\pronsole.py:1028
 msgid "slice set - adjust slicer settings"
-msgstr "Instellen SFACT"
+msgstr ""
 
-#: printrun/pronsole.py:1189
+#: printrun\pronsole.py:1040
 msgid "Please enter target name in 8.3 format."
 msgstr ""
 
-#: printrun/pronsole.py:1195
+#: printrun\pronsole.py:1046
 msgid "Uploading as %s"
 msgstr ""
 
-#: printrun/pronsole.py:1196
+#: printrun\pronsole.py:1047
 msgid "Uploading %s"
 msgstr ""
 
-#: printrun/pronsole.py:1198
+#: printrun\pronsole.py:1049
 msgid "Press Ctrl-C to interrupt upload."
 msgstr ""
 
-#: printrun/pronsole.py:1201
+#: printrun\pronsole.py:1052
 msgid "Progress: "
 msgstr ""
 
-#: printrun/pronsole.py:1212
+#: printrun\pronsole.py:1063
 msgid "Upload completed. %s should now be on the card."
 msgstr ""
 
-#: printrun/pronsole.py:1216
+#: printrun\pronsole.py:1067
 msgid "...interrupted!"
 msgstr ""
 
-#: printrun/pronsole.py:1218
+#: printrun\pronsole.py:1069
 msgid "Something wrong happened while uploading:"
 msgstr ""
 
-#: printrun/pronsole.py:1224
+#: printrun\pronsole.py:1075
 msgid "A partial file named %s may have been written to the sd card."
 msgstr ""
 
-#: printrun/pronsole.py:1241
-msgid ""
-"Send a loaded gcode file to the printer. Load a file with the load command "
-"first."
+#: printrun\pronsole.py:1092
+msgid "Send a loaded gcode file to the printer. Load a file with the load command first."
 msgstr ""
 
-#: printrun/pronsole.py:1243
+#: printrun\pronsole.py:1094
 msgid "Send a loaded gcode file to the printer. You have %s loaded right now."
 msgstr ""
 
-#: printrun/pronsole.py:1247 printrun/pronterface.py:730
-#: printrun/pronterface.py:1108
+#: printrun\pronsole.py:1098 printrun\pronterface.py:901
+#: printrun\pronterface.py:1426
 msgid "No file loaded. Please use load first."
-msgstr "Geen bestand geladen. Eerst bestand inladen."
+msgstr ""
 
-#: printrun/pronsole.py:1252
-#, fuzzy
+#: printrun\pronsole.py:1103
 msgid "Printing %s"
-msgstr " Printen:%04.2f %% |"
+msgstr ""
 
-#: printrun/pronsole.py:1253
+#: printrun\pronsole.py:1104
 msgid "You can monitor the print with the monitor command."
 msgstr ""
 
-#: printrun/pronsole.py:1261
+#: printrun\pronsole.py:1113
 msgid "Not printing, cannot pause."
 msgstr ""
 
-#: printrun/pronsole.py:1267
-#, fuzzy
+#: printrun\pronsole.py:1119
 msgid "Pauses a running print"
-msgstr "Start het printen"
+msgstr ""
 
-#: printrun/pronsole.py:1274
+#: printrun\pronsole.py:1126
 msgid "Not paused, unable to resume. Start a print first."
 msgstr ""
 
-#: printrun/pronsole.py:1284
+#: printrun\pronsole.py:1136
 msgid "Resumes a paused print."
 msgstr ""
 
-#: printrun/pronsole.py:1293
+#: printrun\pronsole.py:1145
 msgid "Files on SD card:"
 msgstr ""
 
-#: printrun/pronsole.py:1307 printrun/pronsole.py:1349
-#: printrun/pronsole.py:1562
-#, fuzzy
+#: printrun\pronsole.py:1160 printrun\pronsole.py:1202
+#: printrun\pronsole.py:1495
 msgid "Printer is not online. Please connect to it first."
-msgstr "Printer is niet verbonden."
+msgstr ""
 
-#: printrun/pronsole.py:1312
+#: printrun\pronsole.py:1165
 msgid "Lists files on the SD card"
 msgstr ""
 
-#: printrun/pronsole.py:1316 printrun/pronterface.py:1645
+#: printrun\pronsole.py:1169 printrun\pronterface.py:2092
 msgid "Opening file failed."
-msgstr "Bestand openen mislukt"
+msgstr ""
 
-#: printrun/pronsole.py:1322 printrun/pronterface.py:1651
+#: printrun\pronsole.py:1175 printrun\pronterface.py:2098
 msgid "Starting print"
-msgstr "Start het printen"
+msgstr ""
 
-#: printrun/pronsole.py:1345
-#, fuzzy
+#: printrun\pronsole.py:1198
 msgid "Resets the printer."
-msgstr "Verbind met printer"
+msgstr ""
 
-#: printrun/pronsole.py:1355
-#, fuzzy
+#: printrun\pronsole.py:1208
 msgid "File is not present on card. Please upload it first."
-msgstr "Geen bestand geladen. Eerst bestand inladen."
+msgstr ""
 
-#: printrun/pronsole.py:1359
+#: printrun\pronsole.py:1212
 msgid "Printing file: %s from SD card."
 msgstr ""
 
-#: printrun/pronsole.py:1360
+#: printrun\pronsole.py:1213
 msgid "Requesting SD print..."
 msgstr ""
 
-#: printrun/pronsole.py:1364
+#: printrun\pronsole.py:1217
 msgid "Print a file from the SD card. Tab completes with available file names."
 msgstr ""
 
-#: printrun/pronsole.py:1365
+#: printrun\pronsole.py:1218
 msgid "sdprint filename.g"
 msgstr ""
 
-#: printrun/pronsole.py:1382
+#: printrun\pronsole.py:1235
 msgid "Print resumed at: %s"
 msgstr ""
 
-#: printrun/pronsole.py:1384
+#: printrun\pronsole.py:1237
 msgid "Print started at: %s"
 msgstr ""
 
-#: printrun/pronsole.py:1392
-msgid "Failed to inhibit sleep:"
+#: printrun\pronsole.py:1253 printrun\pronsole.py:1260
+msgid "Failed to set power settings:"
 msgstr ""
 
-#: printrun/pronsole.py:1399
-msgid "Failed to uninhibit sleep:"
+#: printrun\pronsole.py:1264
+msgid "Print ended at: %(end_time)s and took %(duration)s"
 msgstr ""
 
-#: printrun/pronsole.py:1403
-msgid "Print ended at: %(end_time)s and took %(duration)s"
+#: printrun\pronsole.py:1324 printrun\pronterface.py:2051
+msgid "Received command %s"
 msgstr ""
 
-#: printrun/pronsole.py:1457
+#: printrun\pronsole.py:1390
 msgid "Printer is not currently printing. No ETA available."
 msgstr ""
 
-#: printrun/pronsole.py:1460
+#: printrun\pronsole.py:1393
 msgid "Est: %s of %s remaining"
 msgstr ""
 
-#: printrun/pronsole.py:1465
+#: printrun\pronsole.py:1398
 msgid "Displays estimated remaining print time."
 msgstr ""
 
-#: printrun/pronsole.py:1498
-#, fuzzy
+#: printrun\pronsole.py:1425 printrun\pronsole.py:1427
+msgid "Hotend: %s%s/%s%s"
+msgstr ""
+
+#: printrun\pronsole.py:1428
+msgid "Bed:    %s%s/%s%s"
+msgstr ""
+
+#: printrun\pronsole.py:1431
 msgid "Read the extruder and bed temperature."
-msgstr "Er moet een temperatuur worden ingesteld."
+msgstr ""
 
-#: printrun/pronsole.py:1507 printrun/pronsole.py:1540
+#: printrun\pronsole.py:1440 printrun\pronsole.py:1473
 msgid "You must enter a temperature."
-msgstr "Er moet een temperatuur worden ingesteld."
+msgstr ""
 
-#: printrun/pronsole.py:1512
-msgid ""
-"%s is a high temperature to set your extruder to. Are you sure you want to "
-"do that?"
+#: printrun\pronsole.py:1445
+msgid "%s is a high temperature to set your extruder to. Are you sure you want to do that?"
 msgstr ""
 
-#: printrun/pronsole.py:1517
-#, fuzzy
+#: printrun\pronsole.py:1450
 msgid "Setting hotend temperature to %s degrees Celsius."
-msgstr "Stel elementtemperatuur in op %f graden Celsius."
+msgstr ""
 
-#: printrun/pronsole.py:1521 printrun/pronterface.py:359
-msgid ""
-"You cannot set negative temperatures. To turn the hotend off entirely, set "
-"its temperature to 0."
+#: printrun\pronsole.py:1454 printrun\pronterface.py:474
+msgid "You cannot set negative temperatures. To turn the hotend off entirely, set its temperature to 0."
 msgstr ""
-"Negatieve temperatuur is niet instelbaar. Om het element uit te schakelen "
-"wordt temperatuur 0 ingesteld."
 
-#: printrun/pronsole.py:1524
-#, fuzzy
+#: printrun\pronsole.py:1457
 msgid "Sets the hotend temperature to the value entered."
-msgstr "Stel elementtemperatuur in op %f graden Celsius."
+msgstr ""
 
-#: printrun/pronsole.py:1525 printrun/pronsole.py:1552
+#: printrun\pronsole.py:1458 printrun\pronsole.py:1485
 msgid "Enter either a temperature in celsius or one of the following keywords"
 msgstr ""
 
-#: printrun/pronsole.py:1544
-#, fuzzy
+#: printrun\pronsole.py:1477
 msgid "Setting bed temperature to %s degrees Celsius."
-msgstr "Bed teperatuur ingesteld op %f graden Celsius."
+msgstr ""
 
-#: printrun/pronsole.py:1548 printrun/pronterface.py:379
-msgid ""
-"You cannot set negative temperatures. To turn the bed off entirely, set its "
-"temperature to 0."
+#: printrun\pronsole.py:1481 printrun\pronterface.py:494
+msgid "You cannot set negative temperatures. To turn the bed off entirely, set its temperature to 0."
 msgstr ""
-"Negatieve temperatuur is niet instelbaar. Om het printbed uit te schakelen "
-"wordt temperatuur 0 ingesteld."
 
-#: printrun/pronsole.py:1551
-#, fuzzy
+#: printrun\pronsole.py:1484
 msgid "Sets the bed temperature to the value entered."
-msgstr "Bed teperatuur ingesteld op %f graden Celsius."
+msgstr ""
 
-#: printrun/pronsole.py:1565
+#: printrun\pronsole.py:1498
 msgid "Printer is not printing. Please print something before monitoring."
 msgstr ""
 
-#: printrun/pronsole.py:1567
-#, fuzzy
+#: printrun\pronsole.py:1500
 msgid "Monitoring printer, use ^C to interrupt."
-msgstr "Printercommunicatie wordt gevolgd."
+msgstr ""
 
-#: printrun/pronsole.py:1572 printrun/pronterface.py:329
+#: printrun\pronsole.py:1505 printrun\pronterface.py:438
 msgid "Invalid period given."
-msgstr "Foute gegevens ingevoerd"
+msgstr ""
 
-#: printrun/pronsole.py:1573
+#: printrun\pronsole.py:1506
 msgid "Updating values every %f seconds."
 msgstr ""
 
-#: printrun/pronsole.py:1584 printrun/pronsole.py:1587
+#: printrun\pronsole.py:1516
 msgid "Print progress: "
 msgstr ""
 
-#: printrun/pronsole.py:1595 printrun/pronterface.py:333
+#: printrun\pronsole.py:1519
+msgid "SD print progress: "
+msgstr ""
+
+#: printrun\pronsole.py:1527 printrun\pronterface.py:442
 msgid "Done monitoring."
-msgstr "Klaar met volgen."
+msgstr ""
 
-#: printrun/pronsole.py:1599
+#: printrun\pronsole.py:1531
 msgid "Monitor a machine's temperatures and an SD print's status."
 msgstr ""
 
-#: printrun/pronsole.py:1600
-msgid ""
-"monitor - Reports temperature and SD print status (if SD printing) every 5 "
-"seconds"
+#: printrun\pronsole.py:1532
+msgid "monitor - Reports temperature and SD print status (if SD printing) every 5 seconds"
 msgstr ""
 
-#: printrun/pronsole.py:1601
-msgid ""
-"monitor 2 - Reports temperature and SD print status (if SD printing) every 2 "
-"seconds"
+#: printrun\pronsole.py:1533
+msgid "monitor 2 - Reports temperature and SD print status (if SD printing) every 2 seconds"
 msgstr ""
 
-#: printrun/pronsole.py:1612
+#: printrun\pronsole.py:1544
 msgid "You must specify the tool index as an integer."
 msgstr ""
 
-#: printrun/pronsole.py:1616
+#: printrun\pronsole.py:1548
 msgid "Using tool %d."
 msgstr ""
 
-#: printrun/pronsole.py:1620
+#: printrun\pronsole.py:1553
 msgid "You cannot set negative tool numbers."
 msgstr ""
 
-#: printrun/pronsole.py:1623
-msgid ""
-"Switches to the specified tool (e.g. doing tool 1 will emit a T1 G-Code)."
+#: printrun\pronsole.py:1556
+msgid "Switches to the specified tool (e.g. doing tool 1 will emit a T1 G-Code)."
 msgstr ""
 
-#: printrun/pronsole.py:1627
+#: printrun\pronsole.py:1560
 msgid "No move specified."
 msgstr ""
 
-#: printrun/pronsole.py:1630 printrun/pronsole.py:1692
-#: printrun/pronsole.py:1735 printrun/pronsole.py:1762
-msgid ""
-"Printer is currently printing. Please pause the print before you issue "
-"manual commands."
+#: printrun\pronsole.py:1563 printrun\pronsole.py:1625
+#: printrun\pronsole.py:1674 printrun\pronsole.py:1701
+msgid "Printer is currently printing. Please pause the print before you issue manual commands."
 msgstr ""
 
-#: printrun/pronsole.py:1633 printrun/pronsole.py:1759
-#, fuzzy
+#: printrun\pronsole.py:1566 printrun\pronsole.py:1698
 msgid "Printer is not online. Unable to move."
-msgstr "Printer is niet verbonden."
+msgstr ""
 
-#: printrun/pronsole.py:1649
+#: printrun\pronsole.py:1582
 msgid "Unknown axis."
 msgstr ""
 
-#: printrun/pronsole.py:1654
+#: printrun\pronsole.py:1587
 msgid "Invalid distance"
 msgstr ""
 
-#: printrun/pronsole.py:1665
+#: printrun\pronsole.py:1598
 msgid "Move an axis. Specify the name of the axis and the amount. "
 msgstr ""
 
-#: printrun/pronsole.py:1666
-msgid ""
-"move X 10 will move the X axis forward by 10mm at %s mm/min (default XY "
-"speed)"
+#: printrun\pronsole.py:1599
+msgid "move X 10 will move the X axis forward by 10mm at %s mm/min (default XY speed)"
 msgstr ""
 
-#: printrun/pronsole.py:1667
+#: printrun\pronsole.py:1600
 msgid "move Y 10 5000 will move the Y axis forward by 10mm at 5000mm/min"
 msgstr ""
 
-#: printrun/pronsole.py:1668
-msgid ""
-"move Z -1 will move the Z axis down by 1mm at %s mm/min (default Z speed)"
+#: printrun\pronsole.py:1601
+msgid "move Z -1 will move the Z axis down by 1mm at %s mm/min (default Z speed)"
 msgstr ""
 
-#: printrun/pronsole.py:1669
+#: printrun\pronsole.py:1602
 msgid "Common amounts are in the tabcomplete list."
 msgstr ""
 
-#: printrun/pronsole.py:1699 printrun/pronsole.py:1742
-#, fuzzy
+#: printrun\pronsole.py:1632 printrun\pronsole.py:1681
 msgid "Invalid length given."
-msgstr "Foute gegevens ingevoerd"
+msgstr ""
 
-#: printrun/pronsole.py:1704 printrun/pronsole.py:1747
-#, fuzzy
+#: printrun\pronsole.py:1637 printrun\pronsole.py:1686
 msgid "Invalid speed given."
-msgstr "Foute gegevens ingevoerd"
+msgstr ""
 
-#: printrun/pronsole.py:1712
+#: printrun\pronsole.py:1645
 msgid "Extruding %fmm of filament."
 msgstr ""
 
-#: printrun/pronsole.py:1714
+#: printrun\pronsole.py:1647
 msgid "Reversing %fmm of filament."
 msgstr ""
 
-#: printrun/pronsole.py:1716
+#: printrun\pronsole.py:1649
 msgid "Length is 0, not doing anything."
 msgstr ""
 
-#: printrun/pronsole.py:1722
-msgid ""
-"Extrudes a length of filament, 5mm by default, or the number of mm given as "
-"a parameter"
+#: printrun\pronsole.py:1661
+msgid "Extrudes a length of filament, 5mm by default, or the number of mm given as a parameter"
 msgstr ""
 
-#: printrun/pronsole.py:1723
+#: printrun\pronsole.py:1662
 msgid "extrude - extrudes 5mm of filament at 300mm/min (5mm/s)"
 msgstr ""
 
-#: printrun/pronsole.py:1724
+#: printrun\pronsole.py:1663
 msgid "extrude 20 - extrudes 20mm of filament at 300mm/min (5mm/s)"
 msgstr ""
 
-#: printrun/pronsole.py:1725
+#: printrun\pronsole.py:1664
 msgid "extrude -5 - REVERSES 5mm of filament at 300mm/min (5mm/s)"
 msgstr ""
 
-#: printrun/pronsole.py:1726
+#: printrun\pronsole.py:1665
 msgid "extrude 10 210 - extrudes 10mm of filament at 210mm/min (3.5mm/s)"
 msgstr ""
 
-#: printrun/pronsole.py:1732
-#, fuzzy
+#: printrun\pronsole.py:1671
 msgid "Printer is not online. Unable to reverse."
-msgstr "Printer is niet verbonden."
+msgstr ""
 
-#: printrun/pronsole.py:1751
-msgid ""
-"Reverses the extruder, 5mm by default, or the number of mm given as a "
-"parameter"
+#: printrun\pronsole.py:1690
+msgid "Reverses the extruder, 5mm by default, or the number of mm given as a parameter"
 msgstr ""
 
-#: printrun/pronsole.py:1752
+#: printrun\pronsole.py:1691
 msgid "reverse - reverses 5mm of filament at 300mm/min (5mm/s)"
 msgstr ""
 
-#: printrun/pronsole.py:1753
+#: printrun\pronsole.py:1692
 msgid "reverse 20 - reverses 20mm of filament at 300mm/min (5mm/s)"
 msgstr ""
 
-#: printrun/pronsole.py:1754
+#: printrun\pronsole.py:1693
 msgid "reverse 10 210 - extrudes 10mm of filament at 210mm/min (3.5mm/s)"
 msgstr ""
 
-#: printrun/pronsole.py:1755
+#: printrun\pronsole.py:1694
 msgid "reverse -5 - EXTRUDES 5mm of filament at 300mm/min (5mm/s)"
 msgstr ""
 
-#: printrun/pronsole.py:1777
-#, fuzzy
+#: printrun\pronsole.py:1716
 msgid "Homes the printer"
-msgstr "Verbind met printer"
+msgstr ""
 
-#: printrun/pronsole.py:1778
+#: printrun\pronsole.py:1717
 msgid "home - homes all axes and zeroes the extruder(Using G28 and G92)"
 msgstr ""
 
-#: printrun/pronsole.py:1779
+#: printrun\pronsole.py:1718
 msgid "home xy - homes x and y axes (Using G28)"
 msgstr ""
 
-#: printrun/pronsole.py:1780
+#: printrun\pronsole.py:1719
 msgid "home z - homes z axis only (Using G28)"
 msgstr ""
 
-#: printrun/pronsole.py:1781
+#: printrun\pronsole.py:1720
 msgid "home e - set extruder position to zero (Using G92)"
 msgstr ""
 
-#: printrun/pronsole.py:1782
+#: printrun\pronsole.py:1721
 msgid "home xyze - homes all axes and zeroes the extruder (Using G28 and G92)"
 msgstr ""
 
-#: printrun/pronsole.py:1790
-#, fuzzy
+#: printrun\pronsole.py:1729
 msgid "; Motors off"
-msgstr "Motoren uit"
+msgstr ""
 
-#: printrun/pronsole.py:1792
-#, fuzzy
+#: printrun\pronsole.py:1731
 msgid "; Extruder off"
-msgstr "Extruden"
+msgstr ""
 
-#: printrun/pronsole.py:1794
+#: printrun\pronsole.py:1733
 msgid "; Heatbed off"
 msgstr ""
 
-#: printrun/pronsole.py:1796
+#: printrun\pronsole.py:1735
 msgid "; Fan off"
 msgstr ""
 
-#: printrun/pronsole.py:1798
+#: printrun\pronsole.py:1737
 msgid "; Power supply off"
 msgstr ""
 
-#: printrun/pronsole.py:1801
-#, fuzzy
+#: printrun\pronsole.py:1740
 msgid "Printer is not online. Unable to turn it off."
-msgstr "Printer is niet verbonden."
+msgstr ""
 
-#: printrun/pronsole.py:1804
+#: printrun\pronsole.py:1743
 msgid "Turns off everything on the printer"
 msgstr ""
 
-#: printrun/pronsole.py:1815
+#: printrun\pronsole.py:1754
 msgid "G-Code calling host command \"%s\""
 msgstr ""
 
-#: printrun/pronsole.py:1824
-msgid ""
-"Runs a custom script. Current gcode filename can be given using %s token."
+#: printrun\pronsole.py:1763
+msgid "Runs a custom script. Current gcode filename can be given using $s token."
 msgstr ""
 
-#: printrun/pronsole.py:1832
-msgid ""
-"Runs a custom script which output gcode which will in turn be executed. "
-"Current gcode filename can be given using %s token."
+#: printrun\pronsole.py:1773
+msgid "Runs a custom script which output gcode which will in turn be executed. Current gcode filename can be given using $s token."
 msgstr ""
 
-#: printrun/pronterface.py:149
+#: printrun\pronterface.py:160
 msgid "Motors off"
-msgstr "Motoren uit"
+msgstr ""
 
-#: printrun/pronterface.py:149
+#: printrun\pronterface.py:160
 msgid "Switch all motors off"
 msgstr ""
 
-#: printrun/pronterface.py:150
+#: printrun\pronterface.py:161
 msgid "Advance extruder by set length"
 msgstr ""
 
-#: printrun/pronterface.py:150
+#: printrun\pronterface.py:161
 msgid "Extrude"
-msgstr "Extruden"
+msgstr ""
 
-#: printrun/pronterface.py:151
+#: printrun\pronterface.py:162
 msgid "Reverse"
-msgstr "Terug"
+msgstr ""
 
-#: printrun/pronterface.py:151
+#: printrun\pronterface.py:162
 msgid "Reverse extruder by set length"
 msgstr ""
 
-#: printrun/pronterface.py:165
-#, fuzzy
+#: printrun\pronterface.py:183
 msgid "Pronterface"
-msgstr "Printer Interface"
+msgstr ""
 
-#: printrun/pronterface.py:192
+#: printrun\pronterface.py:208
 msgid ""
 "# I moved all your custom buttons into .pronsolerc.\n"
 "# Please don't add them here any more.\n"
 "# Backup of your old buttons is in custombtn.old\n"
 msgstr ""
-"# Gedefinieerde knoppen zijn verplaatst naar .pronsolerc.\n"
-"# Hier geen nieuwe knoppen definiëren.\n"
-"# Een backup van de oude knoppen staat in custombtn.old\n"
 
-#: printrun/pronterface.py:197
-msgid ""
-"Note!!! You have specified custom buttons in both custombtn.txt and ."
-"pronsolerc"
+#: printrun\pronterface.py:213
+msgid "Note!!! You have specified custom buttons in both custombtn.txt and .pronsolerc"
 msgstr ""
-"Let op!!! Er zijn gedefinieerde knoppen in zowel custombtn.txt en .pronsolerc"
 
-#: printrun/pronterface.py:198
-msgid ""
-"Ignoring custombtn.txt. Remove all current buttons to revert to custombtn.txt"
+#: printrun\pronterface.py:214
+msgid "Ignoring custombtn.txt. Remove all current buttons to revert to custombtn.txt"
+msgstr ""
+
+#: printrun\pronterface.py:290 printrun\pronterface.py:627
+msgid "Tabbed"
 msgstr ""
-"Negeer custombtn.txt. Verwijder alle gedefinieerde knoppen om gebruik te "
-"maken van custombtn.txt"
 
-#: printrun/pronterface.py:331
+#: printrun\pronterface.py:293 printrun\pronterface.py:1085
+msgid "Compact"
+msgstr ""
+
+#: printrun\pronterface.py:399
+msgid "Exit"
+msgstr ""
+
+#: printrun\pronterface.py:399
+msgid "Print in progress ! Are you really sure you want to quit ?"
+msgstr ""
+
+#: printrun\pronterface.py:440
 msgid "Monitoring printer."
-msgstr "Printercommunicatie wordt gevolgd."
+msgstr ""
+
+#: printrun\pronterface.py:446
+msgid "Please pause or stop print before extruding."
+msgstr ""
+
+#: printrun\pronterface.py:453
+msgid "Please pause or stop print before reversing."
+msgstr ""
 
-#: printrun/pronterface.py:354
-msgid "Setting hotend temperature to %f degrees Celsius."
-msgstr "Stel elementtemperatuur in op %f graden Celsius."
+#: printrun\pronterface.py:469
+msgid "Setting hotend temperature to %g degrees Celsius."
+msgstr ""
 
-#: printrun/pronterface.py:361 printrun/pronterface.py:381
+#: printrun\pronterface.py:476 printrun\pronterface.py:496
 msgid "You must enter a temperature. (%s)"
-msgstr "Er moet een temperatuur worden ingesteld. (%s)"
+msgstr ""
 
-#: printrun/pronterface.py:374
-msgid "Setting bed temperature to %f degrees Celsius."
-msgstr "Bed teperatuur ingesteld op %f graden Celsius."
+#: printrun\pronterface.py:489
+msgid "Setting bed temperature to %g degrees Celsius."
+msgstr ""
 
-#: printrun/pronterface.py:392
+#: printrun\pronterface.py:507
 msgid "Setting print speed factor to %d%%."
 msgstr ""
 
-#: printrun/pronterface.py:396
-#, fuzzy
+#: printrun\pronterface.py:511
 msgid "You must enter a speed. (%s)"
-msgstr "Er moet een temperatuur worden ingesteld. (%s)"
+msgstr ""
+
+#: printrun\pronterface.py:522
+msgid "Setting print flow factor to %d%%."
+msgstr ""
 
-#: printrun/pronterface.py:470
+#: printrun\pronterface.py:526
+msgid "You must enter a flow. (%s)"
+msgstr ""
+
+#: printrun\pronterface.py:607
 msgid "Plate function activated"
 msgstr ""
 
-#: printrun/pronterface.py:479
+#: printrun\pronterface.py:617
 msgid "G-Code plate function activated"
 msgstr ""
 
-#: printrun/pronterface.py:486
+#: printrun\pronterface.py:625
 msgid "Plated %s"
 msgstr ""
 
-#: printrun/pronterface.py:500
+#: printrun\pronterface.py:642
 msgid "SD Upload"
-msgstr "uploaden naar SD"
+msgstr ""
 
-#: printrun/pronterface.py:504
+#: printrun\pronterface.py:646
 msgid "SD Print"
-msgstr "Afdruk van SD"
+msgstr ""
 
-#: printrun/pronterface.py:565
-msgid ""
-"Manual move outside of the build volume prevented (see the \"Clamp manual "
-"moves\" option)."
+#: printrun\pronterface.py:710
+msgid "Manual move outside of the build volume prevented (see the \"Clamp manual moves\" option)."
 msgstr ""
 
-#: printrun/pronterface.py:621
-msgid ""
-"Attempted to write invalid text to console, which could be due to an invalid "
-"baudrate"
+#: printrun\pronterface.py:779
+msgid "Attempted to write invalid text to console, which could be due to an invalid baudrate"
+msgstr ""
+
+#: printrun\pronterface.py:781
+msgid "Unhanded exception: "
 msgstr ""
 
-#: printrun/pronterface.py:655
-msgid " Opens file"
-msgstr " Opent bestand"
+#: printrun\pronterface.py:812
+msgid " Open file"
+msgstr ""
+
+#: printrun\pronterface.py:812
+msgid "&Open...\tCtrl+O"
+msgstr ""
 
-#: printrun/pronterface.py:655
-msgid "&Open..."
-msgstr "&Open..."
+#: printrun\pronterface.py:813
+msgid " Save file"
+msgstr ""
+
+#: printrun\pronterface.py:813
+msgid "&Save..."
+msgstr ""
+
+#: printrun\pronterface.py:822
+msgid "&Recent Files"
+msgstr ""
 
-#: printrun/pronterface.py:663
+#: printrun\pronterface.py:823
 msgid " Clear output console"
 msgstr ""
 
-#: printrun/pronterface.py:663
-msgid "Clear console"
+#: printrun\pronterface.py:823
+msgid "Clear console\tCtrl+L"
 msgstr ""
 
-#: printrun/pronterface.py:664
+#: printrun\pronterface.py:824
 msgid " Closes the Window"
-msgstr " Sluit het venster"
+msgstr ""
 
-#: printrun/pronterface.py:664
+#: printrun\pronterface.py:824
 msgid "E&xit"
-msgstr "&Stoppen"
+msgstr ""
 
-#: printrun/pronterface.py:665
+#: printrun\pronterface.py:825
 msgid "&File"
 msgstr ""
 
-#: printrun/pronterface.py:668
+#: printrun\pronterface.py:829
 msgid " Edit open file"
-msgstr " Wijzig geopend bestand"
+msgstr ""
 
-#: printrun/pronterface.py:668
+#: printrun\pronterface.py:829
 msgid "&Edit..."
-msgstr "&Wijzig..."
+msgstr ""
 
-#: printrun/pronterface.py:669
+#: printrun\pronterface.py:830
 msgid " Compose 3D models into a single plate"
 msgstr ""
 
-#: printrun/pronterface.py:669
-#, fuzzy
-msgid "Plater"
-msgstr "Element:"
-
-#: printrun/pronterface.py:670
+#: printrun\pronterface.py:831
 msgid " Compose G-Codes into a single plate"
 msgstr ""
 
-#: printrun/pronterface.py:670
-msgid "G-Code Plater"
-msgstr ""
-
-#: printrun/pronterface.py:671
+#: printrun\pronterface.py:832
 msgid " Exclude parts of the bed from being printed"
 msgstr ""
 
-#: printrun/pronterface.py:671
+#: printrun\pronterface.py:832
 msgid "Excluder"
 msgstr ""
 
-#: printrun/pronterface.py:672
+#: printrun\pronterface.py:833
 msgid " Project slices"
 msgstr ""
 
-#: printrun/pronterface.py:672
+#: printrun\pronterface.py:833
 msgid "Projector"
 msgstr ""
 
-#: printrun/pronterface.py:673
+#: printrun\pronterface.py:836
+msgid "Spool Manager"
+msgstr ""
+
+#: printrun\pronterface.py:837
+msgid " Manage different spools of filament"
+msgstr ""
+
+#: printrun\pronterface.py:838
 msgid "&Tools"
 msgstr ""
 
-#: printrun/pronterface.py:676
-msgid ""
-" Recover previous print after a disconnect (homes X, Y, restores Z and E "
-"status)"
+#: printrun\pronterface.py:842
+msgid " Recover previous print after a disconnect (homes X, Y, restores Z and E status)"
 msgstr ""
 
-#: printrun/pronterface.py:676
+#: printrun\pronterface.py:842
 msgid "Recover"
 msgstr ""
 
-#: printrun/pronterface.py:679
+#: printrun\pronterface.py:845
 msgid "&Advanced"
 msgstr ""
 
-#: printrun/pronterface.py:686
-#, fuzzy
+#: printrun\pronterface.py:852
 msgid "Print &settings"
-msgstr "Wijzig instellingen"
+msgstr ""
 
-#: printrun/pronterface.py:687
+#: printrun\pronterface.py:853
 msgid "&Filament"
 msgstr ""
 
-#: printrun/pronterface.py:688
-#, fuzzy
+#: printrun\pronterface.py:854
 msgid "&Printer"
-msgstr "&Printen"
+msgstr ""
 
-#: printrun/pronterface.py:694
+#: printrun\pronterface.py:860
 msgid "&Slic3r"
 msgstr ""
 
-#: printrun/pronterface.py:696
+#: printrun\pronterface.py:862
 msgid "Failed to load Slic3r configuration:"
 msgstr ""
 
-#: printrun/pronterface.py:702
+#: printrun\pronterface.py:868
 msgid "&Macros"
-msgstr "&Macros"
+msgstr ""
 
-#: printrun/pronterface.py:703
+#: printrun\pronterface.py:869
 msgid "<&New...>"
-msgstr "<&Nieuw...>"
+msgstr ""
 
-#: printrun/pronterface.py:704
+#: printrun\pronterface.py:870
 msgid " Options dialog"
-msgstr "Optievenster"
+msgstr ""
 
-#: printrun/pronterface.py:704
+#: printrun\pronterface.py:870
 msgid "&Options"
-msgstr "&Opties"
+msgstr ""
 
-#: printrun/pronterface.py:706
-#, fuzzy
+#: printrun\pronterface.py:872
 msgid " Adjust slicing settings"
-msgstr "Instellen SFACT"
+msgstr ""
 
-#: printrun/pronterface.py:706
-#, fuzzy
+#: printrun\pronterface.py:872
 msgid "Slicing settings"
-msgstr "SFACT Instellingen"
+msgstr ""
 
-#: printrun/pronterface.py:708
+#: printrun\pronterface.py:874
 msgid "Debug communications"
 msgstr ""
 
-#: printrun/pronterface.py:709
+#: printrun\pronterface.py:875
 msgid "Print all G-code sent to and received from the printer."
 msgstr ""
 
-#: printrun/pronterface.py:713
+#: printrun\pronterface.py:879
+msgid "Don't autoscroll"
+msgstr ""
+
+#: printrun\pronterface.py:880
+msgid "Disables automatic scrolling of the console when new text is added"
+msgstr ""
+
+#: printrun\pronterface.py:884
 msgid "&Settings"
-msgstr "&Instellingen"
+msgstr ""
 
-#: printrun/pronterface.py:719
-#, fuzzy
+#: printrun\pronterface.py:890
 msgid "&About Printrun"
-msgstr "Printercommunicatie volgen"
+msgstr ""
 
-#: printrun/pronterface.py:719
+#: printrun\pronterface.py:890
 msgid "Show about dialog"
 msgstr ""
 
-#: printrun/pronterface.py:720
+#: printrun\pronterface.py:891
 msgid "&Help"
 msgstr ""
 
-#: printrun/pronterface.py:746
-msgid ""
-"Printrun is a pure Python 3D printing (and other types of CNC) host software."
+#: printrun\pronterface.py:922
+msgid "Printrun is a pure Python 3D printing (and other types of CNC) host software."
 msgstr ""
 
-#: printrun/pronterface.py:750
-#, fuzzy
+#: printrun\pronterface.py:926
 msgid "%.02fmm of filament have been extruded during prints"
-msgstr "mm fillament wordt gebruikt in deze print\n"
+msgstr ""
 
-#: printrun/pronterface.py:781
-#, fuzzy
+#: printrun\pronterface.py:1077
 msgid "Monitor printer status"
-msgstr "Printercommunicatie volgen"
+msgstr ""
 
-#: printrun/pronterface.py:781
-msgid ""
-"Regularly monitor printer temperatures (required to have functional "
-"temperature graph or gauges)"
+#: printrun\pronterface.py:1077
+msgid "Regularly monitor printer temperatures (required to have functional temperature graph or gauges)"
 msgstr ""
 
-#: printrun/pronterface.py:782
+#: printrun\pronterface.py:1078
 msgid "Path to the simarrange binary to use in the STL plater"
 msgstr ""
 
-#: printrun/pronterface.py:782
+#: printrun\pronterface.py:1078
 msgid "Simarrange command"
 msgstr ""
 
-#: printrun/pronterface.py:783
+#: printrun\pronterface.py:1079
 msgid "Circular build platform"
 msgstr ""
 
-#: printrun/pronterface.py:783
+#: printrun\pronterface.py:1079
 msgid "Draw a circular (or oval) build platform instead of a rectangular one"
 msgstr ""
 
-#: printrun/pronterface.py:784
-#, fuzzy
+#: printrun\pronterface.py:1080
 msgid "Extruders count"
-msgstr "Extruden"
+msgstr ""
 
-#: printrun/pronterface.py:784
+#: printrun\pronterface.py:1080
 msgid "Number of extruders"
 msgstr ""
 
-#: printrun/pronterface.py:785
+#: printrun\pronterface.py:1081
 msgid "Clamp manual moves"
 msgstr ""
 
-#: printrun/pronterface.py:785
+#: printrun\pronterface.py:1081
 msgid "Prevent manual moves from leaving the specified build dimensions"
 msgstr ""
 
-#: printrun/pronterface.py:786
-#, fuzzy
+#: printrun\pronterface.py:1082
+msgid "Display progress on printer"
+msgstr ""
+
+#: printrun\pronterface.py:1082
+msgid "Show progress on printers display (sent via M117, might not be supported by all printers)"
+msgstr ""
+
+#: printrun\pronterface.py:1083
+msgid "Interval in which pronterface sends the progress to the printer if enabled, in seconds"
+msgstr ""
+
+#: printrun\pronterface.py:1083
+msgid "Printer progress update interval"
+msgstr ""
+
+#: printrun\pronterface.py:1084
+msgid "Display cutting moves"
+msgstr ""
+
+#: printrun\pronterface.py:1084
+msgid "Show moves where spindle is active as printing moves"
+msgstr ""
+
+#: printrun\pronterface.py:1085
 msgid "Interface mode"
-msgstr "Voer macronaam in"
+msgstr ""
+
+#: printrun\pronterface.py:1085
+msgid "Standard"
+msgstr ""
 
-#: printrun/pronterface.py:786
+#: printrun\pronterface.py:1085
 msgid ""
-"Standard interface is a one-page, three columns layout with controls/"
-"visualization/log\n"
-"Compact mode is a one-page, two columns layout with controls + log/"
-"visualization\n"
-"Tabbed mode is a two-pages mode, where the first page shows controls and the "
-"second one shows visualization and log."
+"Standard interface is a one-page, three columns layout with controls/visualization/log\n"
+"Compact mode is a one-page, two columns layout with controls + log/visualization"
 msgstr ""
 
-#: printrun/pronterface.py:787
+#: printrun\pronterface.py:1087
 msgid "Controls mode"
 msgstr ""
 
-#: printrun/pronterface.py:787
-msgid ""
-"Standard controls include all controls needed for printer setup and "
-"calibration, while Mini controls are limited to the ones needed for daily "
-"printing"
+#: printrun\pronterface.py:1087
+msgid "Standard controls include all controls needed for printer setup and calibration, while Mini controls are limited to the ones needed for daily printing"
 msgstr ""
 
-#: printrun/pronterface.py:788
+#: printrun\pronterface.py:1088
 msgid "Add a menu to select Slic3r profiles directly from Pronterface"
 msgstr ""
 
-#: printrun/pronterface.py:788
+#: printrun\pronterface.py:1088
 msgid "Enable Slic3r integration"
 msgstr ""
 
-#: printrun/pronterface.py:789
+#: printrun\pronterface.py:1089
 msgid "Update Slic3r default presets"
 msgstr ""
 
-#: printrun/pronterface.py:789
-msgid ""
-"When selecting a profile in Slic3r integration menu, also save it as the "
-"default Slic3r preset"
+#: printrun\pronterface.py:1089
+msgid "When selecting a profile in Slic3r integration menu, also save it as the default Slic3r preset"
 msgstr ""
 
-#: printrun/pronterface.py:790
+#: printrun\pronterface.py:1090
 msgid "Main visualization"
 msgstr ""
 
-#: printrun/pronterface.py:790
+#: printrun\pronterface.py:1090
 msgid "Select visualization for main window."
 msgstr ""
 
-#: printrun/pronterface.py:791
+#: printrun\pronterface.py:1091
 msgid "Use 3D in GCode viewer window"
 msgstr ""
 
-#: printrun/pronterface.py:791
+#: printrun\pronterface.py:1091
 msgid "Use 3D mode instead of 2D layered mode in the visualization window"
 msgstr ""
 
-#: printrun/pronterface.py:792
+#: printrun\pronterface.py:1092
+msgid "3D viewer options"
+msgstr ""
+
+#: printrun\pronterface.py:1093
 msgid "Use a lighter 3D visualization"
 msgstr ""
 
-#: printrun/pronterface.py:792
-msgid ""
-"Use a lighter visualization with simple lines instead of extruded paths for "
-"3D viewer"
+#: printrun\pronterface.py:1093
+msgid "Use a lighter visualization with simple lines instead of extruded paths for 3D viewer"
+msgstr ""
+
+#: printrun\pronterface.py:1094
+msgid "A perspective view looks more realistic, but is a bit more confusing to navigate"
+msgstr ""
+
+#: printrun\pronterface.py:1094
+msgid "Use a perspective view instead of orthographic"
+msgstr ""
+
+#: printrun\pronterface.py:1095
+msgid "Amount of anti-aliasing samples used in the 3D viewer"
 msgstr ""
 
-#: printrun/pronterface.py:793
+#: printrun\pronterface.py:1095
+msgid "Number of anti-aliasing samples"
+msgstr ""
+
+#: printrun\pronterface.py:1096
 msgid "Track current layer in main 3D view"
 msgstr ""
 
-#: printrun/pronterface.py:793
+#: printrun\pronterface.py:1096
 msgid "Track the currently printing layer in the main 3D visualization"
 msgstr ""
 
-#: printrun/pronterface.py:794
+#: printrun\pronterface.py:1097
+msgid "Extrusion width for 3D viewer"
+msgstr ""
+
+#: printrun\pronterface.py:1097
+msgid "Width of printed path in 3D viewer"
+msgstr ""
+
+#: printrun\pronterface.py:1098
+msgid "Height of printed path in 3D viewer"
+msgstr ""
+
+#: printrun\pronterface.py:1098
+msgid "Layer height for 3D viewer"
+msgstr ""
+
+#: printrun\pronterface.py:1099
 msgid "Display temperature graph"
 msgstr ""
 
-#: printrun/pronterface.py:794
+#: printrun\pronterface.py:1099
 msgid "Display time-lapse temperature graph"
 msgstr ""
 
-#: printrun/pronterface.py:795
+#: printrun\pronterface.py:1100
 msgid "Display graphical gauges for temperatures visualization"
 msgstr ""
 
-#: printrun/pronterface.py:795
+#: printrun\pronterface.py:1100
 msgid "Display temperature gauges"
 msgstr ""
 
-#: printrun/pronterface.py:796
+#: printrun\pronterface.py:1101
 msgid "Display a checkbox that, when check, locks most of Pronterface"
 msgstr ""
 
-#: printrun/pronterface.py:796
+#: printrun\pronterface.py:1101
 msgid "Display interface lock checkbox"
 msgstr ""
 
-#: printrun/pronterface.py:797
+#: printrun\pronterface.py:1102
 msgid "If lock checkbox is enabled, lock the interface when starting a print"
 msgstr ""
 
-#: printrun/pronterface.py:797
+#: printrun\pronterface.py:1102
 msgid "Lock interface upon print start"
 msgstr ""
 
-#: printrun/pronterface.py:804
+#: printrun\pronterface.py:1103
+msgid "Regularly update visualization during the load of a G-Code file"
+msgstr ""
+
+#: printrun\pronterface.py:1103
+msgid "Update UI during G-Code load"
+msgstr ""
+
+#: printrun\pronterface.py:1112
+msgid "2D viewer options"
+msgstr ""
+
+#: printrun\pronterface.py:1113
 msgid "Preview extrusion width"
 msgstr ""
 
-#: printrun/pronterface.py:804
+#: printrun\pronterface.py:1113
 msgid "Width of Extrusion in Preview"
 msgstr ""
 
-#: printrun/pronterface.py:805
+#: printrun\pronterface.py:1114
 msgid "Fine Grid Spacing"
 msgstr ""
 
-#: printrun/pronterface.py:805
+#: printrun\pronterface.py:1114
 msgid "Fine grid spacing"
 msgstr ""
 
-#: printrun/pronterface.py:806
+#: printrun\pronterface.py:1115
 msgid "Coarse Grid Spacing"
 msgstr ""
 
-#: printrun/pronterface.py:806
+#: printrun\pronterface.py:1115
 msgid "Coarse grid spacing"
 msgstr ""
 
-#: printrun/pronterface.py:807
+#: printrun\pronterface.py:1116
 msgid "Background color"
 msgstr ""
 
-#: printrun/pronterface.py:807
+#: printrun\pronterface.py:1116
 msgid "Pronterface background color"
 msgstr ""
 
-#: printrun/pronterface.py:808
+#: printrun\pronterface.py:1117
+msgid "Color of the temperature graph background"
+msgstr ""
+
+#: printrun\pronterface.py:1117
+msgid "Graph background color"
+msgstr ""
+
+#: printrun\pronterface.py:1118
+msgid "Color of the temperature graph text"
+msgstr ""
+
+#: printrun\pronterface.py:1118
+msgid "Graph text color"
+msgstr ""
+
+#: printrun\pronterface.py:1119
+msgid "Color of the temperature graph grid"
+msgstr ""
+
+#: printrun\pronterface.py:1119
+msgid "Graph grid color"
+msgstr ""
+
+#: printrun\pronterface.py:1120
+msgid "Color of the temperature graph fan speed line"
+msgstr ""
+
+#: printrun\pronterface.py:1120
+msgid "Graph fan line color"
+msgstr ""
+
+#: printrun\pronterface.py:1121
+msgid "Color of the temperature graph bed temperature line"
+msgstr ""
+
+#: printrun\pronterface.py:1121
+msgid "Graph bed line color"
+msgstr ""
+
+#: printrun\pronterface.py:1122
+msgid "Color of the temperature graph bed temperature target line"
+msgstr ""
+
+#: printrun\pronterface.py:1122
+msgid "Graph bed target line color"
+msgstr ""
+
+#: printrun\pronterface.py:1123
+msgid "Color of the temperature graph extruder 0 temperature line"
+msgstr ""
+
+#: printrun\pronterface.py:1123
+msgid "Graph ex0 line color"
+msgstr ""
+
+#: printrun\pronterface.py:1124
+msgid "Color of the temperature graph extruder 0 target temperature line"
+msgstr ""
+
+#: printrun\pronterface.py:1124
+msgid "Graph ex0 target line color"
+msgstr ""
+
+#: printrun\pronterface.py:1125
+msgid "Color of the temperature graph extruder 1 temperature line"
+msgstr ""
+
+#: printrun\pronterface.py:1125
+msgid "Graph ex1 line color color"
+msgstr ""
+
+#: printrun\pronterface.py:1126
+msgid "Color of the temperature graph extruder 1 temperature target line"
+msgstr ""
+
+#: printrun\pronterface.py:1126
+msgid "Graph ex1 target line color"
+msgstr ""
+
+#: printrun\pronterface.py:1127
 msgid "3D view background color"
 msgstr ""
 
-#: printrun/pronterface.py:808
+#: printrun\pronterface.py:1127
 msgid "Color of the 3D view background"
 msgstr ""
 
-#: printrun/pronterface.py:809
+#: printrun\pronterface.py:1128
 msgid "3D view travel moves color"
 msgstr ""
 
-#: printrun/pronterface.py:809
+#: printrun\pronterface.py:1128
 msgid "Color of travel moves in 3D view"
 msgstr ""
 
-#: printrun/pronterface.py:810
+#: printrun\pronterface.py:1129
 msgid "3D view print moves color"
 msgstr ""
 
-#: printrun/pronterface.py:810
+#: printrun\pronterface.py:1129
 msgid "Color of print moves with tool 0 in 3D view"
 msgstr ""
 
-#: printrun/pronterface.py:811
+#: printrun\pronterface.py:1130
 msgid "3D view tool 1 moves color"
 msgstr ""
 
-#: printrun/pronterface.py:811
+#: printrun\pronterface.py:1130
 msgid "Color of print moves with tool 1 in 3D view"
 msgstr ""
 
-#: printrun/pronterface.py:812
+#: printrun\pronterface.py:1131
+msgid "3D view tool 2 moves color"
+msgstr ""
+
+#: printrun\pronterface.py:1131
+msgid "Color of print moves with tool 2 in 3D view"
+msgstr ""
+
+#: printrun\pronterface.py:1132
+msgid "3D view tool 3 moves color"
+msgstr ""
+
+#: printrun\pronterface.py:1132
+msgid "Color of print moves with tool 3 in 3D view"
+msgstr ""
+
+#: printrun\pronterface.py:1133
+msgid "3D view tool 4 moves color"
+msgstr ""
+
+#: printrun\pronterface.py:1133
+msgid "Color of print moves with tool 4 in 3D view"
+msgstr ""
+
+#: printrun\pronterface.py:1134
 msgid "3D view printed moves color"
 msgstr ""
 
-#: printrun/pronterface.py:812
+#: printrun\pronterface.py:1134
 msgid "Color of printed moves in 3D view"
 msgstr ""
 
-#: printrun/pronterface.py:813
+#: printrun\pronterface.py:1135
 msgid "3D view current layer moves color"
 msgstr ""
 
-#: printrun/pronterface.py:813
+#: printrun\pronterface.py:1135
 msgid "Color of moves in current layer in 3D view"
 msgstr ""
 
-#: printrun/pronterface.py:814
+#: printrun\pronterface.py:1136
 msgid "3D view printed current layer moves color"
 msgstr ""
 
-#: printrun/pronterface.py:814
+#: printrun\pronterface.py:1136
 msgid "Color of already printed moves from current layer in 3D view"
 msgstr ""
 
-#: printrun/pronterface.py:815
-msgid "Changing most settings here will require restart to get effect"
+#: printrun\pronterface.py:1137
+msgid "Changing some of these settings might require a restart to get effect"
 msgstr ""
 
-#: printrun/pronterface.py:815
+#: printrun\pronterface.py:1137
 msgid "Note:"
 msgstr ""
 
-#: printrun/pronterface.py:822
+#: printrun\pronterface.py:1151
 msgid "automatically try to connect to printer on startup"
 msgstr ""
 
-#: printrun/pronterface.py:835 printrun/pronterface.py:1316
+#: printrun\pronterface.py:1164 printrun\pronterface.py:1645
 msgid "Failed to load recent files list:"
 msgstr ""
 
-#: printrun/pronterface.py:916
-#, fuzzy
+#: printrun\pronterface.py:1257
 msgid "SD upload: %04.2f%% |"
-msgstr " SD printen:%04.2f %%"
+msgstr ""
 
-#: printrun/pronterface.py:917 printrun/pronterface.py:922
+#: printrun\pronterface.py:1258 printrun\pronterface.py:1263
 msgid " Line# %d of %d lines |"
 msgstr ""
 
-#: printrun/pronterface.py:919
-#, fuzzy
+#: printrun\pronterface.py:1260
 msgid "SD printing: %04.2f%% |"
-msgstr " SD printen:%04.2f %%"
+msgstr ""
 
-#: printrun/pronterface.py:921
-#, fuzzy
+#: printrun\pronterface.py:1262
 msgid "Printing: %04.2f%% |"
-msgstr " Printen:%04.2f %% |"
+msgstr ""
 
-#: printrun/pronterface.py:924
+#: printrun\pronterface.py:1265
 msgid " Est: %s of %s remaining | "
 msgstr ""
 
-#: printrun/pronterface.py:926
-#, fuzzy
+#: printrun\pronterface.py:1267
 msgid " Z: %.3f mm"
-msgstr " Z: %0.2f mm"
-
-#: printrun/pronterface.py:931
-msgid "Disconnecting after 4 failed writes."
 msgstr ""
 
-#: printrun/pronterface.py:972
-#, fuzzy
+#: printrun\pronterface.py:1303
 msgid "Locking interface."
-msgstr "Printer Interface"
+msgstr ""
 
-#: printrun/pronterface.py:976
-#, fuzzy
+#: printrun\pronterface.py:1307
 msgid "Unlocking interface."
-msgstr "Printercommunicatie wordt gevolgd."
+msgstr ""
 
-#: printrun/pronterface.py:985
-#, fuzzy
+#: printrun\pronterface.py:1322
 msgid "Connecting..."
-msgstr "Verbind"
-
-#: printrun/pronterface.py:997
-msgid "Could not parse baud rate: "
 msgstr ""
 
-#: printrun/pronterface.py:1013 printrun/pronterface.py:1023
-msgid "Error: You are trying to connect to a non-existing port."
+#: printrun\pronterface.py:1334
+msgid "Could not parse baud rate: "
 msgstr ""
 
-#: printrun/pronterface.py:1015
-msgid "Error: You don't have permission to open %s."
+#: printrun\pronterface.py:1339 printrun\pronterface.py:1379
+#: printrun\pronterface.py:1399 printrun\pronterface.py:1409
+#: printrun\pronterface.py:1496 printrun\pronterface.py:1721
+msgid "&Pause"
 msgstr ""
 
-#: printrun/pronterface.py:1016
-msgid "You might need to add yourself to the dialout group."
+#: printrun\pronterface.py:1340 printrun\pronterface.py:1380
+#: printrun\pronterface.py:1396 printrun\pronterface.py:1720
+#: printrun\pronterface.py:1870
+msgid "&Print"
 msgstr ""
 
-#: printrun/pronterface.py:1043
-#, fuzzy
+#: printrun\pronterface.py:1360
 msgid "Disconnected."
-msgstr "Ontkoppel"
+msgstr ""
 
-#: printrun/pronterface.py:1071
-#, fuzzy
+#: printrun\pronterface.py:1389
 msgid "Reset."
-msgstr "Reset"
+msgstr ""
 
-#: printrun/pronterface.py:1072
+#: printrun\pronterface.py:1390
 msgid "Are you sure you want to reset the printer?"
-msgstr "Weet je zeker dat je de printer wilt resetten?"
+msgstr ""
 
-#: printrun/pronterface.py:1072
+#: printrun\pronterface.py:1390
 msgid "Reset?"
-msgstr "resetten?"
+msgstr ""
 
-#: printrun/pronterface.py:1093
+#: printrun\pronterface.py:1411
 msgid "Restart"
-msgstr "Herstart"
+msgstr ""
 
-#: printrun/pronterface.py:1126
+#: printrun\pronterface.py:1445
 msgid "Pick SD filename"
-msgstr "Kies bestandsnaam op SD"
+msgstr ""
 
-#: printrun/pronterface.py:1144
+#: printrun\pronterface.py:1463
 msgid "File upload complete"
-msgstr "Bestandsupload voltooid"
+msgstr ""
 
-#: printrun/pronterface.py:1151
+#: printrun\pronterface.py:1470
 msgid "Print paused at: %s"
 msgstr ""
 
-#: printrun/pronterface.py:1163
+#: printrun\pronterface.py:1484
 msgid "Resume"
-msgstr "Hervat"
+msgstr ""
 
-#: printrun/pronterface.py:1166
-#, fuzzy
+#: printrun\pronterface.py:1487
 msgid "Resuming."
-msgstr "Hervat"
+msgstr ""
 
-#: printrun/pronterface.py:1192
+#: printrun\pronterface.py:1516
 msgid "Pick SD file"
-msgstr "Kies bestand op SD"
+msgstr ""
 
-#: printrun/pronterface.py:1192
+#: printrun\pronterface.py:1516
 msgid "Select the file to print"
-msgstr "Kies het te printen bestand"
+msgstr ""
 
-#: printrun/pronterface.py:1228 printrun/pronterface.py:1259
-#, fuzzy
-msgid "Slicing "
-msgstr "Skeinforge draait"
+#: printrun\pronterface.py:1551
+msgid "Running "
+msgstr ""
 
-#: printrun/pronterface.py:1237
+#: printrun\pronterface.py:1560
 msgid "Failed to execute slicing software: "
 msgstr ""
 
-#: printrun/pronterface.py:1244
-#, fuzzy
+#: printrun\pronterface.py:1567
 msgid "Slicing..."
-msgstr "Skeinforge draait..."
+msgstr ""
+
+#: printrun\pronterface.py:1583
+msgid "Slicing "
+msgstr ""
 
-#: printrun/pronterface.py:1296
+#: printrun\pronterface.py:1620
 msgid "Open file to print"
-msgstr "Open het te printen bestand"
+msgstr ""
 
-#: printrun/pronterface.py:1297
-#, fuzzy
-msgid ""
-"OBJ, STL, and GCODE files (*.gcode;*.gco;*.g;*.stl;*.STL;*.obj;*.OBJ)|*."
-"gcode;*.gco;*.g;*.stl;*.STL;*.obj;*.OBJ|All Files (*.*)|*.*"
-msgstr "STL en GCODE bestanden (;*.gcode;*.g;*.stl;*.STL;)"
+#: printrun\pronterface.py:1621
+msgid "OBJ, STL, and GCODE files (*.gcode;*.gco;*.g;*.stl;*.STL;*.obj;*.OBJ)|*.gcode;*.gco;*.g;*.stl;*.STL;*.obj;*.OBJ|GCODE files (*.gcode;*.gco;*.g)|*.gcode;*.gco;*.g|OBJ, STL files (*.stl;*.STL;*.obj;*.OBJ)|*.stl;*.STL;*.obj;*.OBJ|All Files (*.*)|*.*"
+msgstr ""
 
-#: printrun/pronterface.py:1325
+#: printrun\pronterface.py:1654
 msgid "Could not update recent files list:"
 msgstr ""
 
-#: printrun/pronterface.py:1359
+#: printrun\pronterface.py:1691
+msgid "Loading %s: %d layers loaded (%d lines)"
+msgstr ""
+
+#: printrun\pronterface.py:1700
+msgid "Loading %s..."
+msgstr ""
+
+#: printrun\pronterface.py:1714
+msgid "Pronterface - %s"
+msgstr ""
+
+#: printrun\pronterface.py:1715
 msgid "Loaded %s, %d lines"
-msgstr "Geladen %s, %d regels"
+msgstr ""
 
-#: printrun/pronterface.py:1362
-#, fuzzy
+#: printrun\pronterface.py:1719
 msgid "Load File"
-msgstr "open bestand"
+msgstr ""
+
+#: printrun\pronterface.py:1751
+msgid "%s of filament used in this print"
+msgstr ""
 
-#: printrun/pronterface.py:1376
-#, fuzzy
-msgid "%.2fmm of filament used in this print"
-msgstr "mm fillament wordt gebruikt in deze print\n"
+#: printrun\pronterface.py:1764
+msgid "Using spool '%s' (%s of filament will remain)"
+msgstr ""
 
-#: printrun/pronterface.py:1377
+#: printrun\pronterface.py:1769
 msgid "The print goes:"
 msgstr ""
 
-#: printrun/pronterface.py:1378
+#: printrun\pronterface.py:1770
 msgid "- from %.2f mm to %.2f mm in X and is %.2f mm wide"
 msgstr ""
 
-#: printrun/pronterface.py:1379
+#: printrun\pronterface.py:1771
 msgid "- from %.2f mm to %.2f mm in Y and is %.2f mm deep"
 msgstr ""
 
-#: printrun/pronterface.py:1380
+#: printrun\pronterface.py:1772
 msgid "- from %.2f mm to %.2f mm in Z and is %.2f mm high"
 msgstr ""
 
-#: printrun/pronterface.py:1450
+#: printrun\pronterface.py:1835
+msgid "Save as"
+msgstr ""
+
+#: printrun\pronterface.py:1836
+msgid "GCODE files (*.gcode;*.gco;*.g)|*.gcode;*.gco;*.g|All Files (*.*)|*.*"
+msgstr ""
+
+#: printrun\pronterface.py:1840
+msgid "G-Code successfully saved to %s"
+msgstr ""
+
+#: printrun\pronterface.py:1875
 msgid "Printer is now online."
-msgstr "Printer is nu verbonden."
+msgstr ""
 
-#: printrun/pronterface.py:1455
-msgid "Disconnect"
-msgstr "Ontkoppel"
+#: printrun\pronterface.py:1880
+msgid "Dis&connect"
+msgstr ""
+
+#: printrun\pronterface.py:2010
+msgid "Heater%s:"
+msgstr ""
 
-#: printrun/pronterface.py:1688
-#, fuzzy
+#: printrun\pronterface.py:2134
 msgid "click to add new custom button"
-msgstr "Definieer eigen knop."
+msgstr ""
 
-#: printrun/pronterface.py:1694
+#: printrun\pronterface.py:2140
 msgid "Execute command: "
 msgstr ""
 
-#: printrun/pronterface.py:1714
-msgid ""
-"Defines custom button. Usage: button <num> \"title\" [/c \"colour\"] command"
+#: printrun\pronterface.py:2160
+msgid "Defines custom button. Usage: button <num> \"title\" [/c \"colour\"] command"
 msgstr ""
-"Definieert eigen knop. Gebruik: knop <num> \"titel\" [/c \"kleur\"] commando"
 
-#: printrun/pronterface.py:1736
+#: printrun\pronterface.py:2182
 msgid "Custom button number should be between 0 and 63"
-msgstr "Knopnummer moet tussen 0 en 63 zijn"
+msgstr ""
 
-#: printrun/pronterface.py:1827
+#: printrun\pronterface.py:2266
 msgid "Edit custom button '%s'"
-msgstr "Wijzig gedefineerde knop '%s'"
+msgstr ""
 
-#: printrun/pronterface.py:1829
+#: printrun\pronterface.py:2268
 msgid "Move left <<"
-msgstr "Verplaats links <<"
+msgstr ""
 
-#: printrun/pronterface.py:1832
+#: printrun\pronterface.py:2271
 msgid "Move right >>"
-msgstr "Verplaats rechts >>"
+msgstr ""
 
-#: printrun/pronterface.py:1836
+#: printrun\pronterface.py:2275
 msgid "Remove custom button '%s'"
-msgstr "Verwijder gedefinieerde knop '%s'"
+msgstr ""
 
-#: printrun/pronterface.py:1839
+#: printrun\pronterface.py:2278
 msgid "Add custom button"
-msgstr "Definieer eigen knop."
+msgstr ""
 
-#: printrun/pronterface.py:1972
-msgid "event object missing"
-msgstr "vermist object"
+#: printrun\pronterface.py:2386
+msgid "Failed to handle button"
+msgstr ""
 
-#: printrun/pronterface.py:1985
+#: printrun\pronterface.py:2399
 msgid "Do you want to erase the macro?"
-msgstr "Wilt u de macro verwijderen?"
+msgstr ""
 
-#: printrun/pronterface.py:1989
+#: printrun\pronterface.py:2403
 msgid "Cancelled."
-msgstr "Afgebroken"
+msgstr ""
 
-#: printrun/pronterface.py:2007
+#: printrun\pronterface.py:2421
 msgid "Enter macro name"
-msgstr "Voer macronaam in"
+msgstr ""
 
-#: printrun/pronterface.py:2010
+#: printrun\pronterface.py:2422
 msgid "Macro name:"
-msgstr "Macronaam:"
+msgstr ""
 
-#: printrun/pronterface.py:2013
+#: printrun\pronterface.py:2424
 msgid "Ok"
-msgstr "Ok"
+msgstr ""
 
-#: printrun/pronterface.py:2035
+#: printrun\pronterface.py:2464
 msgid "Macro name may contain only ASCII alphanumeric symbols and underscores"
 msgstr ""
 
-#: printrun/pronterface.py:2038
+#: printrun\pronterface.py:2467
 msgid "Name '%s' is being used by built-in command"
-msgstr "Naam '%s' wordt gebruikt door ingebouwde instructie"
+msgstr ""
 
-#: pronsole.py:31
-msgid "Caught an exception, exiting:"
+#: printrun\rpc.py:39
+msgid "RPC server bound on non-default port %d"
 msgstr ""
 
-#~ msgid "Check temp"
-#~ msgstr "Controleer Temp."
+#: printrun\settings.py:36
+msgid "Default: "
+msgstr ""
 
-#~ msgid "Mini mode"
-#~ msgstr "Mini-venster"
+#: printrun\settings.py:37
+msgid "(Control-doubleclick to reset to default value)"
+msgstr ""
 
-#~ msgid "Z:"
-#~ msgstr "Z:"
+#: printrun\settings.py:288
+msgid "Width"
+msgstr ""
 
-#~ msgid "Full mode"
-#~ msgstr "Volledig venster"
+#: printrun\settings.py:291
+msgid "Depth"
+msgstr ""
 
-#~ msgid "Printer is online. "
-#~ msgstr "Printer is verbonden. "
+#: printrun\settings.py:294
+msgid "Height"
+msgstr ""
 
-#~ msgid "Bed"
-#~ msgstr "Bed"
+#: printrun\settings.py:297
+msgid "X offset"
+msgstr ""
 
-#~ msgid "Hotend"
-#~ msgstr "Element"
+#: printrun\settings.py:300
+msgid "Y offset"
+msgstr ""
 
-#~ msgid ", %d lines"
-#~ msgstr ", %d regels"
+#: printrun\settings.py:303
+msgid "Z offset"
+msgstr ""
 
-#, fuzzy
-#~ msgid "Paused."
-#~ msgstr "Pauze"
+#: printrun\settings.py:306
+msgid "X home pos."
+msgstr ""
 
-#~ msgid "X+100"
-#~ msgstr "X+100"
+#: printrun\settings.py:309
+msgid "Y home pos."
+msgstr ""
 
-#~ msgid "X+10"
-#~ msgstr "X+10"
+#: printrun\settings.py:312
+msgid "Z home pos."
+msgstr ""
 
-#~ msgid "X+1"
-#~ msgstr "X+1"
+#: printrun\settings.py:327
+msgid "Port used to communicate with printer"
+msgstr ""
 
-#~ msgid "X+0.1"
-#~ msgstr "X+0.1"
+#: printrun\settings.py:327
+msgid "Serial port"
+msgstr ""
 
-#~ msgid "HomeX"
-#~ msgstr "0-puntX"
+#: printrun\settings.py:328
+msgid "Baud rate"
+msgstr ""
 
-#~ msgid "X-0.1"
-#~ msgstr "X-0.1"
+#: printrun\settings.py:328
+msgid "Communications Speed"
+msgstr ""
 
-#~ msgid "X-1"
-#~ msgstr "X-1"
+#: printrun\settings.py:329
+msgid "TCP streaming mode"
+msgstr ""
 
-#~ msgid "X-10"
-#~ msgstr "X-10"
+#: printrun\settings.py:329
+msgid "When using a TCP connection to the printer, the streaming mode will not wait for acks from the printer to send new commands. This will break things such as ETA prediction, but can result in smoother prints."
+msgstr ""
 
-#~ msgid "X-100"
-#~ msgstr "X-100"
+#: printrun\settings.py:330
+msgid "Enable RPC server to allow remotely querying print status"
+msgstr ""
 
-#~ msgid "Y+100"
-#~ msgstr "Y+100"
+#: printrun\settings.py:330
+msgid "RPC server"
+msgstr ""
 
-#~ msgid "Y+10"
-#~ msgstr "Y+10"
+#: printrun\settings.py:331
+msgid "DTR"
+msgstr ""
 
-#~ msgid "Y+1"
-#~ msgstr "Y+1"
+#: printrun\settings.py:331
+msgid "Disabling DTR would prevent Arduino (RAMPS) from resetting upon connection"
+msgstr ""
 
-#~ msgid "Y+0.1"
-#~ msgstr "Y+0.1"
+#: printrun\settings.py:333
+msgid "Custom device pattern: for example /dev/3DP_* "
+msgstr ""
 
-#~ msgid "HomeY"
-#~ msgstr "0-puntY"
+#: printrun\settings.py:333
+msgid "Device name pattern"
+msgstr ""
 
-#~ msgid "Y-0.1"
-#~ msgstr "Y-0.1"
+#: printrun\settings.py:334
+msgid "Bed temperature for ABS"
+msgstr ""
 
-#~ msgid "Y-1"
-#~ msgstr "Y-1"
+#: printrun\settings.py:334
+msgid "Heated Build Platform temp for ABS (deg C)"
+msgstr ""
 
-#~ msgid "Y-10"
-#~ msgstr "Y-10"
+#: printrun\settings.py:335
+msgid "Bed temperature for PLA"
+msgstr ""
 
-#~ msgid "Y-100"
-#~ msgstr "Y-100"
+#: printrun\settings.py:335
+msgid "Heated Build Platform temp for PLA (deg C)"
+msgstr ""
 
-#~ msgid "Z+10"
-#~ msgstr "Z+10"
+#: printrun\settings.py:336
+msgid "Extruder temp for ABS (deg C)"
+msgstr ""
 
-#~ msgid "Z+1"
-#~ msgstr "Z+1"
+#: printrun\settings.py:336
+msgid "Extruder temperature for ABS"
+msgstr ""
 
-#~ msgid "Z+0.1"
-#~ msgstr "Z+0.1"
+#: printrun\settings.py:337
+msgid "Extruder temp for PLA (deg C)"
+msgstr ""
 
-#~ msgid "HomeZ"
-#~ msgstr "0-puntZ"
+#: printrun\settings.py:337
+msgid "Extruder temperature for PLA"
+msgstr ""
 
-#~ msgid "Z-0.1"
-#~ msgstr "Z-0.1"
+#: printrun\settings.py:338
+msgid "Feedrate for Control Panel Moves in X and Y (mm/min)"
+msgstr ""
 
-#~ msgid "Z-1"
-#~ msgstr "Z-1"
+#: printrun\settings.py:338
+msgid "X && Y manual feedrate"
+msgstr ""
 
-#~ msgid "Z-10"
-#~ msgstr "Z-10"
+#: printrun\settings.py:339
+msgid "Feedrate for Control Panel Moves in Z (mm/min)"
+msgstr ""
 
-#~ msgid "Home"
-#~ msgstr "0-punt"
+#: printrun\settings.py:339
+msgid "Z manual feedrate"
+msgstr ""
 
-#~ msgid " degrees Celsius."
-#~ msgstr " graden Celsius."
+#: printrun\settings.py:340
+msgid "E manual feedrate"
+msgstr ""
 
-#~ msgid "SFACT Quick Settings"
-#~ msgstr "SFACT Snelinstelling"
+#: printrun\settings.py:340
+msgid "Feedrate for Control Panel Moves in Extrusions (mm/min)"
+msgstr ""
 
-#~ msgid " Quickly adjust SFACT settings for active profile"
-#~ msgstr " Eenvoudig SFACT's huidige profiel instellen"
+#: printrun\settings.py:347
+msgid "Path to slicer"
+msgstr ""
 
-#~ msgid "Name '"
-#~ msgstr "Naam '"
+#: printrun\settings.py:349
+msgid "Slice command"
+msgstr ""
 
-#~ msgid "Skeinforge execution failed."
-#~ msgstr "Skeinforge was niet succesvol."
+#: printrun\settings.py:350
+msgid "Slice settings command"
+msgstr ""
+
+#: printrun\settings.py:350
+msgid "Slicer options command"
+msgstr ""
+
+#: printrun\settings.py:351
+msgid "Executable to run when the print is started"
+msgstr ""
+
+#: printrun\settings.py:351
+msgid "Start command"
+msgstr ""
+
+#: printrun\settings.py:352
+msgid "Executable to run when the print is finished"
+msgstr ""
+
+#: printrun\settings.py:352
+msgid "Final command"
+msgstr ""
+
+#: printrun\settings.py:353
+msgid "Error command"
+msgstr ""
+
+#: printrun\settings.py:353
+msgid "Executable to run when an error occurs"
+msgstr ""
+
+#: printrun\settings.py:354
+msgid "Log path"
+msgstr ""
+
+#: printrun\settings.py:354
+msgid "Path to the log file. An empty path will log to the console."
+msgstr ""
+
+#: printrun\settings.py:423
+msgid "Failed to run callback after setting \"%s\":"
+msgstr ""
+
+#: printrun\stlplater.py:218
+msgid "STL files (*.stl;*.STL)|*.stl;*.STL|OpenSCAD files (*.scad)|*.scad"
+msgstr ""
+
+#: printrun\stlplater.py:219
+msgid "STL files (*.stl;*.STL)|*.stl;*.STL"
+msgstr ""
+
+#: printrun\stlplater.py:235
+msgid "Cut along:"
+msgstr ""
+
+#: printrun\stlplater.py:237
+msgid "Confirm cut"
+msgstr ""
+
+#: printrun\stlplater.py:245
+msgid ">X"
+msgstr ""
+
+#: printrun\stlplater.py:248
+msgid ">Y"
+msgstr ""
+
+#: printrun\stlplater.py:251
+msgid ">Z"
+msgstr ""
+
+#: printrun\stlplater.py:254
+msgid "<X"
+msgstr ""
+
+#: printrun\stlplater.py:257
+msgid "<Y"
+msgstr ""
+
+#: printrun\stlplater.py:260
+msgid "<Z"
+msgstr ""
+
+#: printrun\stlplater.py:291
+msgid "Cutting %s alongside %s axis"
+msgstr ""
+
+#: printrun\stlplater.py:374
+msgid "Loading STL file failed"
+msgstr ""
+
+#: printrun\stlplater.py:375 printrun\stlplater.py:385
+msgid "Error:"
+msgstr ""
+
+#: printrun\stlplater.py:378
+msgid "Loading STL file failed:"
+msgstr ""
+
+#: printrun\stlplater.py:384
+msgid "Loading OpenSCAD file failed"
+msgstr ""
+
+#: printrun\stlplater.py:388
+msgid "Loading OpenSCAD file failed:"
+msgstr ""
+
+#: printrun\stlplater.py:420
+msgid "Couldn't load non-existing file %s"
+msgstr ""
+
+#: printrun\stlplater.py:470
+msgid "Wrote plate to %s"
+msgstr ""
+
+#: printrun\stlplater.py:477
+msgid "Failed to use simarrange for plating, falling back to the standard method. The error was: "
+msgstr ""
+
+#: printrun\stlplater.py:485
+msgid "Autoplating using simarrange"
+msgstr ""
+
+#: printrun\stlplater.py:500
+msgid "Plate full, please remove some objects"
+msgstr ""
+
+#: printrun\stlplater.py:517
+msgid "simarrange failed"
+msgstr ""
+
+#: printrun\utils.py:292
+msgid "Color must be specified as #RGB"
+msgstr ""
+
+#: printrun\utils.py:298
+msgid "Color must be specified as #RGBA"
+msgstr ""
+
+#: pronsole.py:58
+msgid "Caught an exception, exiting:"
+msgstr ""
 
-#~ msgid ""
-#~ "Skeinforge not found. \n"
-#~ "Please copy Skeinforge into a directory named \"skeinforge\" in the same "
-#~ "directory as this file."
-#~ msgstr ""
-#~ "Skeinforge niet gevonden.\n"
-#~ "Plaats Skeinforge in een map met de naam \"skeinforge\" in dezelfde map "
-#~ "als dit bestand."
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Printrun-2.0.0rc7/plater.appdata.xml` & `Printrun-2.0.1/plater.appdata.xml`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/plater.ico` & `Printrun-2.0.1/plater.ico`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/plater.png` & `Printrun-2.0.1/plater.png`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/plater.py` & `Printrun-2.0.1/plater.py`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/printcore.py` & `Printrun-2.0.1/printcore.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         elif o in ('-b','--baud'):
             try:
                 baud = int(a)
             except ValueError:
                 print("ValueError:")
                 print("\tInvalid BAUD_RATE value '%s'" % a)
                 print("\tBAUD_RATE must be an integer\n")
-                # FIXME: This should output a more apropiate error message when
+                # FIXME: This should output a more appropriate error message when
                 #        not a good baud rate is passed as an argument
                 #        i.e: when baud <= 1000 or > 225000
                 print(usage)
                 sys.exit(2)
         elif o in ('-v', '--verbose'):
             loud = True
         elif o in ('-s', '--statusreport'):
```

### Comparing `Printrun-2.0.0rc7/printrun/eventhandler.py` & `Printrun-2.0.1/printrun/eventhandler.py`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/printrun/excluder.py` & `Printrun-2.0.1/printrun/excluder.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,23 +71,28 @@
                 y1 = max(self.initpos[1], pos[1])
                 self.parent.rectangles[-1] = (x0, y0, x1, y1)
             wx.CallAfter(self.p.Refresh)
         else:
             event.Skip()
 
     def _line_scaler(self, orig):
+        # Arguments:
+        #   orig: coordinates of two corners of a rectangle (x0, y0, x1, y1)
+        # Returns:
+        #   rectangle coordinates as (x, y, width, height)
         x0, y0 = self.gcode_to_real(orig[0], orig[1])
         x0 = self.p.scale[0] * x0 + self.p.translate[0]
         y0 = self.p.scale[1] * y0 + self.p.translate[1]
         x1, y1 = self.gcode_to_real(orig[2], orig[3])
         x1 = self.p.scale[0] * x1 + self.p.translate[0]
         y1 = self.p.scale[1] * y1 + self.p.translate[1]
         width = max(x0, x1) - min(x0, x1) + 1
         height = max(y0, y1) - min(y0, y1) + 1
-        return (min(x0, x1), min(y0, y1), width, height,)
+        rectangle = (min(x0, x1), min(y0, y1), width, height)
+        return tuple(map(int, rectangle))
 
     def paint_selection(self, dc):
         dc = wx.GCDC(dc)
         dc.SetPen(wx.TRANSPARENT_PEN)
         dc.DrawRectangleList([self._line_scaler(rect)
                               for rect in self.parent.rectangles],
                              None, wx.Brush((200, 200, 200, 150)))
```

### Comparing `Printrun-2.0.0rc7/printrun/gcodeplater.py` & `Printrun-2.0.1/printrun/gcodeplater.py`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/printrun/gcoder.py` & `Printrun-2.0.1/printrun/gcoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 import re
 import math
 import datetime
 import logging
 from array import array
 
 gcode_parsed_args = ["x", "y", "e", "f", "z", "i", "j"]
-gcode_parsed_nonargs = ["g", "t", "m", "n"]
-to_parse = "".join(gcode_parsed_args + gcode_parsed_nonargs)
+gcode_parsed_nonargs = 'gtmnd'
+to_parse = "".join(gcode_parsed_args) + gcode_parsed_nonargs
 gcode_exp = re.compile("\([^\(\)]*\)|;.*|[/\*].*\n|([%s])\s*([-+]?[0-9]*\.?[0-9]*)" % to_parse)
 gcode_strip_comment_exp = re.compile("\([^\(\)]*\)|;.*|[/\*].*\n")
 m114_exp = re.compile("\([^\(\)]*\)|[/\*].*\n|([XYZ]):?([-+]?[0-9]*\.?[0-9]*)")
 specific_exp = "(?:\([^\(\)]*\))|(?:;.*)|(?:[/\*].*\n)|(%s[-+]?[0-9]*\.?[0-9]*)"
 move_gcodes = ["G0", "G1", "G2", "G3"]
 
 class PyLine:
@@ -104,14 +104,15 @@
 class Layer(list):
 
     __slots__ = ("duration", "z")
 
     def __init__(self, lines, z = None):
         super(Layer, self).__init__(lines)
         self.z = z
+        self.duration = 0
 
 class GCode:
 
     line_class = Line
 
     lines = None
     layers = None
@@ -370,15 +371,16 @@
             ymax_e = float("-inf")
 
             # Duration estimation
             # TODO:
             # get device caps from firmware: max speed, acceleration/axis
             # (including extruder)
             # calculate the maximum move duration accounting for above ;)
-            lastx = lasty = lastz = laste = lastf = 0.0
+            lastx = lasty = lastz = None
+            laste = lastf = 0
             lastdx = 0
             lastdy = 0
             x = y = e = f = 0.0
             currenttravel = 0.0
             moveduration = 0.0
             totalduration = 0.0
             acceleration = 2000.0  # mm/s^2
@@ -386,23 +388,50 @@
 
             # Initialize layers
             all_layers = self.all_layers = []
             all_zs = self.all_zs = set()
             layer_idxs = self.layer_idxs = []
             line_idxs = self.line_idxs = []
 
-            layer_id = 0
-            layer_line = 0
 
             last_layer_z = None
             prev_z = None
-            prev_base_z = (None, None)
             cur_z = None
             cur_lines = []
 
+            def append_lines(lines, isEnd):
+                if not build_layers:
+                    return
+                nonlocal layerbeginduration, last_layer_z
+                if cur_layer_has_extrusion and prev_z != last_layer_z \
+                        or not all_layers:
+                    layer = Layer([], prev_z)
+                    last_layer_z = prev_z
+                    finished_layer = len(all_layers)-1 if all_layers else None
+                    all_layers.append(layer)
+                    all_zs.add(prev_z)
+                else:
+                    layer = all_layers[-1]
+                    finished_layer = None
+                layer_id = len(all_layers)-1
+                layer_line = len(layer)
+                for i, ln in enumerate(lines):
+                    layer.append(ln)
+                    layer_idxs.append(layer_id)
+                    line_idxs.append(layer_line+i)
+                layer.duration += totalduration - layerbeginduration
+                layerbeginduration = totalduration
+                if layer_callback:
+                    # we finish a layer when inserting the next
+                    if finished_layer is not None:
+                        layer_callback(self, finished_layer)
+                    # notify about end layer, there will not be next
+                    if isEnd:
+                        layer_callback(self, layer_id)
+
         if self.line_class != Line:
             get_line = lambda l: Line(l.raw)
         else:
             get_line = lambda l: l
         for true_line in lines:
             # # Parse line
             # Use a heavy copy of the light line to preprocess
@@ -429,15 +458,15 @@
                 elif line.command == "M83":
                     relative_e = True
                 elif line.command[0] == "T":
                     try:
                         current_tool = int(line.command[1:])
                     except:
                         pass #handle T? by treating it as no tool change
-                    while(current_tool+1>len(self.current_e_multi)):
+                    while current_tool+1 > len(self.current_e_multi):
                         self.current_e_multi+=[0]
                         self.offset_e_multi+=[0]
                         self.total_e_multi+=[0]
                         self.max_e_multi+=[0]
                 elif line.command == "M3" or line.command == "M4":
                     cutting = True
                 elif line.command == "M5":
@@ -511,15 +540,15 @@
                             current_e = new_e
                             new_e_multi = line.e + offset_e_multi
                             total_e_multi += new_e_multi - current_e_multi
                             current_e_multi = new_e_multi
 
                         max_e = max(max_e, total_e)
                         max_e_multi=max(max_e_multi, total_e_multi)
-                        cur_layer_has_extrusion |= line.extruding
+                        cur_layer_has_extrusion |= line.extruding and (line.x is not None or line.y is not None)
                     elif line.command == "G92":
                         offset_e = current_e - line.e
                         offset_e_multi = current_e_multi - line.e
                 if cutting and self.cutting_as_extrusion:
                     line.extruding = True
 
                 self.current_e_multi[current_tool]=current_e_multi
@@ -529,32 +558,33 @@
 
                 # # Create layers and perform global computations
                 if build_layers:
                     # Update bounding box
                     if line.is_move:
                         if line.extruding:
                             if line.current_x is not None:
-                                xmin_e = min(xmin_e, line.current_x)
-                                xmax_e = max(xmax_e, line.current_x)
+                                # G0 X10 ; G1 X20 E5 results in 10..20 even as G0 is not extruding
+                                xmin_e = min(xmin_e, line.current_x, xmin_e if lastx is None else lastx)
+                                xmax_e = max(xmax_e, line.current_x, xmax_e if lastx is None else lastx)
                             if line.current_y is not None:
-                                ymin_e = min(ymin_e, line.current_y)
-                                ymax_e = max(ymax_e, line.current_y)
+                                ymin_e = min(ymin_e, line.current_y, ymin_e if lasty is None else lasty)
+                                ymax_e = max(ymax_e, line.current_y, ymax_e if lasty is None else lasty)
                         if max_e <= 0:
                             if line.current_x is not None:
                                 xmin = min(xmin, line.current_x)
                                 xmax = max(xmax, line.current_x)
                             if line.current_y is not None:
                                 ymin = min(ymin, line.current_y)
                                 ymax = max(ymax, line.current_y)
 
                     # Compute duration
                     if line.command == "G0" or line.command == "G1":
-                        x = line.x if line.x is not None else lastx
-                        y = line.y if line.y is not None else lasty
-                        z = line.z if line.z is not None else lastz
+                        x = line.x if line.x is not None else (lastx or 0)
+                        y = line.y if line.y is not None else (lasty or 0)
+                        z = line.z if line.z is not None else (lastz or 0)
                         e = line.e if line.e is not None else laste
                         # mm/s vs mm/m => divide by 60
                         f = line.f / 60.0 if line.f is not None else lastf
 
                         # given last feedrate and current feedrate calculate the
                         # distance needed to achieve current feedrate.
                         # if travel is longer than req'd distance, then subtract
@@ -566,23 +596,23 @@
                         # FIXME: this code has been proven to be super wrong when 2
                         # subsquent moves are in opposite directions, as requested
                         # speed is constant but printer has to fully decellerate
                         # and reaccelerate
                         # The following code tries to fix it by forcing a full
                         # reacceleration if this move is in the opposite direction
                         # of the previous one
-                        dx = x - lastx
-                        dy = y - lasty
+                        dx = x - (lastx or 0)
+                        dy = y - (lasty or 0)
                         if dx * lastdx + dy * lastdy <= 0:
                             lastf = 0
 
                         currenttravel = math.hypot(dx, dy)
                         if currenttravel == 0:
                             if line.z is not None:
-                                currenttravel = abs(line.z) if line.relative else abs(line.z - lastz)
+                                currenttravel = abs(line.z) if line.relative else abs(line.z - (lastz or 0))
                             elif line.e is not None:
                                 currenttravel = abs(line.e) if line.relative_e else abs(line.e - laste)
                         # Feedrate hasn't changed, no acceleration/decceleration planned
                         if f == lastf:
                             moveduration = currenttravel / f if f != 0 else 0.
                         else:
                             # FIXME: review this better
@@ -619,55 +649,21 @@
                             cur_z = line.z
                         elif line.is_move:
                             if line.relative and cur_z is not None:
                                 cur_z += line.z
                             else:
                                 cur_z = line.z
 
-                    # FIXME: the logic behind this code seems to work, but it might be
-                    # broken
-                    if cur_z != prev_z:
-                        if prev_z is not None and last_layer_z is not None:
-                            offset = self.est_layer_height if self.est_layer_height else 0.01
-                            if abs(prev_z - last_layer_z) < offset:
-                                if self.est_layer_height is None:
-                                    zs = sorted([l.z for l in all_layers if l.z is not None])
-                                    heights = [round(zs[i + 1] - zs[i], 3) for i in range(len(zs) - 1)]
-                                    heights = [height for height in heights if height]
-                                    if len(heights) >= 2: self.est_layer_height = heights[1]
-                                    elif heights: self.est_layer_height = heights[0]
-                                    else: self.est_layer_height = 0.1
-                                base_z = round(prev_z - (prev_z % self.est_layer_height), 2)
-                            else:
-                                base_z = round(prev_z, 2)
-                        else:
-                            base_z = prev_z
-
-                        if base_z != prev_base_z:
-                            new_layer = Layer(cur_lines, base_z)
-                            new_layer.duration = totalduration - layerbeginduration
-                            layerbeginduration = totalduration
-                            all_layers.append(new_layer)
-                            if cur_layer_has_extrusion and prev_z not in all_zs:
-                                all_zs.add(prev_z)
-                            cur_lines = []
-                            cur_layer_has_extrusion = False
-                            layer_id += 1
-                            layer_line = 0
-                            last_layer_z = base_z
-                            if layer_callback is not None:
-                                layer_callback(self, len(all_layers) - 1)
-
-                        prev_base_z = base_z
+                    if cur_z != prev_z and cur_layer_has_extrusion:
+                        append_lines(cur_lines, False)
+                        cur_lines = []
+                        cur_layer_has_extrusion = False
 
             if build_layers:
                 cur_lines.append(true_line)
-                layer_idxs.append(layer_id)
-                line_idxs.append(layer_line)
-                layer_line += 1
                 prev_z = cur_z
             # ## Loop done
 
         # Store current status
         self.imperial = imperial
         self.relative = relative
         self.relative_e = relative_e
@@ -688,20 +684,15 @@
         self.total_e_multi[current_tool]=total_e_multi
         self.cutting = cutting
 
 
         # Finalize layers
         if build_layers:
             if cur_lines:
-                new_layer = Layer(cur_lines, prev_z)
-                new_layer.duration = totalduration - layerbeginduration
-                layerbeginduration = totalduration
-                all_layers.append(new_layer)
-                if cur_layer_has_extrusion and prev_z not in all_zs:
-                    all_zs.add(prev_z)
+                append_lines(cur_lines, True)
 
             self.append_layer_id = len(all_layers)
             self.append_layer = Layer([])
             self.append_layer.duration = 0
             all_layers.append(self.append_layer)
             self.layer_idxs = array('I', layer_idxs)
             self.line_idxs = array('I', line_idxs)
```

### Comparing `Printrun-2.0.0rc7/printrun/gcoder_line.pyx` & `Printrun-2.0.1/printrun/gcoder_line.pyx`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/printrun/gcoder_line_extra.h` & `Printrun-2.0.1/printrun/gcoder_line_extra.h`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/printrun/gcview.py` & `Printrun-2.0.1/printrun/gcview.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,17 @@
 CURRENT_LAYER_KEYS = [ord('C')]
 RESET_KEYS = [ord('R')]
 
 class GcodeViewPanel(wxGLPanel):
 
     def __init__(self, parent,
                  build_dimensions = (200, 200, 100, 0, 0, 0),
-                 realparent = None, antialias_samples = 0):
+                 realparent = None, antialias_samples = 0, perspective=False):
+        if perspective:
+            self.orthographic=False
         super().__init__(parent, wx.DefaultPosition,
                                              wx.DefaultSize, 0,
                                              antialias_samples = antialias_samples)
         self.canvas.Bind(wx.EVT_MOUSE_EVENTS, self.move)
         self.canvas.Bind(wx.EVT_LEFT_DCLICK, self.double)
         # self.canvas.Bind(wx.EVT_KEY_DOWN, self.keypress)
         # in Windows event inspector shows only EVT_CHAR_HOOK events
@@ -146,17 +148,22 @@
         # Move origin to bottom left of platform
         platformx0 = -self.build_dimensions[3] - self.parent.platform.width / 2
         platformy0 = -self.build_dimensions[4] - self.parent.platform.depth / 2
         glTranslatef(platformx0, platformy0, 0)
 
         for obj in self.parent.objects:
             if not obj.model \
-               or not obj.model.loaded \
-               or not obj.model.initialized:
+               or not obj.model.loaded:
                 continue
+            # Skip (comment out) initialized check, which safely causes empty 
+            # model during progressive load. This can cause exceptions/garbage
+            # render, but seems fine for now
+            # May need to lock init() and draw_objects() together
+            # if not obj.model.initialized:
+            #     continue
             glPushMatrix()
             glTranslatef(*(obj.offsets))
             glRotatef(obj.rot, 0.0, 0.0, 1.0)
             glTranslatef(*(obj.centeroffset))
             glScalef(*obj.scale)
 
             obj.model.display()
@@ -223,28 +230,35 @@
             return
         current_layer = self.parent.model.num_layers_to_draw
         new_layer = max(1, current_layer - 1)
         self.parent.model.num_layers_to_draw = new_layer
         self.parent.setlayercb(new_layer)
         wx.CallAfter(self.Refresh)
 
+    wheelTimestamp = None
     def handle_wheel(self, event):
+        if self.wheelTimestamp == event.Timestamp:
+            # filter duplicate event delivery in Ubuntu, Debian issue #1110
+            return  
+
+        self.wheelTimestamp = event.Timestamp
+
         delta = event.GetWheelRotation()
         factor = 1.05
         if event.ControlDown():
             factor = 1.02
         if hasattr(self.parent, "model") and event.ShiftDown():
             if not self.parent.model:
                 return
             count = 1 if not event.ControlDown() else 10
             for i in range(count):
                 if delta > 0: self.layerup()
                 else: self.layerdown()
             return
-        x, y = event.GetPosition()
+        x, y = event.GetPosition() * self.GetContentScaleFactor()
         x, y, _ = self.mouse_to_3d(x, y)
         if delta > 0:
             self.zoom(factor, (x, y))
         else:
             self.zoom(1 / factor, (x, y))
 
     def wheel(self, event):
@@ -348,19 +362,19 @@
 
     def set_gcview_params(self, path_width, path_height):
         return set_gcview_params(self, path_width, path_height)
 
 from printrun.gviz import BaseViz
 class GcodeViewMainWrapper(GcodeViewLoader, BaseViz):
 
-    def __init__(self, parent, build_dimensions, root, circular, antialias_samples, grid):
+    def __init__(self, parent, build_dimensions, root, circular, antialias_samples, grid, perspective=False):
         self.root = root
         self.glpanel = GcodeViewPanel(parent, realparent = self,
                                       build_dimensions = build_dimensions,
-                                      antialias_samples = antialias_samples)
+                                      antialias_samples = antialias_samples, perspective=perspective)
         self.glpanel.SetMinSize((150, 150))
         if self.root and hasattr(self.root, "gcview_color_background"):
             self.glpanel.color_background = self.root.gcview_color_background
         self.clickcb = None
         self.widget = self.glpanel
         self.refresh_timer = wx.CallLater(100, self.Refresh)
         self.p = self  # Hack for backwards compatibility with gviz API
@@ -403,15 +417,15 @@
 class GcodeViewFrame(GvizBaseFrame, GcodeViewLoader):
     '''A simple class for using OpenGL with wxPython.'''
 
     def __init__(self, parent, ID, title, build_dimensions, objects = None,
                  pos = wx.DefaultPosition, size = wx.DefaultSize,
                  style = wx.DEFAULT_FRAME_STYLE, root = None, circular = False,
                  antialias_samples = 0,
-                 grid = (1, 10)):
+                 grid = (1, 10), perspective=False):
         GvizBaseFrame.__init__(self, parent, ID, title,
                                pos, size, style)
         self.root = root
 
         panel, vbox = self.create_base_ui()
 
         self.refresh_timer = wx.CallLater(100, self.Refresh)
@@ -425,15 +439,15 @@
         self.toolbar.InsertTool(6, 8, " " + _("Fit to plate"), fit_image,
                                      shortHelp = _("Fit to plate [F]"),
                                      longHelp = '')
         self.toolbar.Realize()
         self.glpanel = GcodeViewPanel(panel,
                                       build_dimensions = build_dimensions,
                                       realparent = self,
-                                      antialias_samples = antialias_samples)
+                                      antialias_samples = antialias_samples, perspective=perspective)
         vbox.Add(self.glpanel, 1, flag = wx.EXPAND)
 
         self.Bind(wx.EVT_TOOL, lambda x: self.glpanel.zoom_to_center(1.2), id = 1)
         self.Bind(wx.EVT_TOOL, lambda x: self.glpanel.zoom_to_center(1 / 1.2), id = 2)
         self.Bind(wx.EVT_TOOL, lambda x: self.glpanel.layerup(), id = 3)
         self.Bind(wx.EVT_TOOL, lambda x: self.glpanel.layerdown(), id = 4)
         self.Bind(wx.EVT_TOOL, lambda x: self.glpanel.resetview(), id = 5)
@@ -453,20 +467,23 @@
             z = self.model.gcode.all_layers[true_layer].z
             message = _("Layer %d -%s Z = %.03f mm") % (layer, extra, z)
         else:
             message = _("Entire object")
         wx.CallAfter(self.SetStatusText, message, 0)
 
     def process_slider(self, event):
-        new_layer = self.layerslider.GetValue()
-        new_layer = min(self.model.max_layers + 1, new_layer)
-        new_layer = max(1, new_layer)
-        self.model.num_layers_to_draw = new_layer
-        self.update_status("")
-        wx.CallAfter(self.Refresh)
+        if self.model is not None:
+            new_layer = self.layerslider.GetValue()
+            new_layer = min(self.model.max_layers + 1, new_layer)
+            new_layer = max(1, new_layer)
+            self.model.num_layers_to_draw = new_layer
+            self.update_status("")
+            wx.CallAfter(self.Refresh)
+        else:
+            logging.info(_("G-Code view, can't process slider. Please wait until model is loaded completely."))
 
     def set_current_gline(self, gline):
         if gline.is_move and gline.gcview_end_vertex is not None \
            and self.model and self.model.loaded:
             self.model.printed_until = gline.gcview_end_vertex
             if not self.refresh_timer.IsRunning():
                 self.refresh_timer.Start()
```

### Comparing `Printrun-2.0.0rc7/printrun/gl/libtatlin/actors.py` & `Printrun-2.0.1/printrun/gl/libtatlin/actors.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,22 +342,22 @@
         segments = math.ceil(abs(a_delta) * r * 2 / 0.5)
         if segments > 100:
             segments = 100
 
         for t in range(segments):
             a = t / segments * a_delta + a_start
 
-            mid = (
+            mid = ((
                 cx + math.cos(a) * r,
                 cy + math.sin(a) * r,
                 z0 + t / segments * dz
-            )
+            ), True)
             yield mid
 
-    yield (gline.current_x, gline.current_y, gline.current_z)
+    yield ((gline.current_x, gline.current_y, gline.current_z), False) # last segment of this line
 
 
 class GcodeModel(Model):
     """
     Model for displaying Gcode data.
     """
 
@@ -440,14 +440,15 @@
         self.layer_stops = [0]
 
         prev_move_normal_x = None
         prev_move_normal_y = None
         prev_move_angle = None
         prev_pos = (0, 0, 0)
         prev_gline = None
+        prev_extruding = False
         layer_idx = 0
 
         self.printed_until = 0
         self.only_current = False
 
         twopi = 2 * math.pi
 
@@ -469,18 +470,18 @@
                     self.normals.resize(ncoords, refcheck = False)
                     self.indices.resize(nindices, refcheck = False)
                 layer = model_data.all_layers[layer_idx]
                 has_movement = False
                 for gline_idx, gline in enumerate(layer):
                     if not gline.is_move:
                         continue
-                    if gline.x is None and gline.y is None and gline.z is None:
+                    if gline.x is None and gline.y is None and gline.z is None and gline.j is None and gline.i is None:
                         continue
                     has_movement = True
-                    for current_pos in interpolate_arcs(gline, prev_gline):
+                    for (current_pos, interpolated) in interpolate_arcs(gline, prev_gline):
                         if not gline.extruding:
                             if self.travels.size < (travel_vertex_k + 100 * 6):
                                 # arc interpolation extra points allocation
                                 # if not enough room for another 100 points now,
                                 # allocate enough and 50% extra to minimize separate allocations
                                 ratio = (travel_vertex_k + 100 * 6) / self.travels.size * 1.5
                                 # print(f"gl realloc travel {self.travels.size} -> {int(self.travels.size * ratio)}")
@@ -503,15 +504,15 @@
                             # FIXME: compute these dynamically
                             path_halfwidth = self.path_halfwidth * 1.2
                             path_halfheight = self.path_halfheight * 1.2
 
                             new_indices = []
                             new_vertices = []
                             new_normals = []
-                            if prev_gline and prev_gline.extruding:
+                            if prev_gline and prev_gline.extruding or prev_extruding:
                                 # Store previous vertices indices
                                 prev_id = vertex_k // 3 - 4
                                 avg_move_normal_x = (prev_move_normal_x + move_normal_x) / 2
                                 avg_move_normal_y = (prev_move_normal_y + move_normal_y) / 2
                                 norm = avg_move_normal_x * avg_move_normal_x + avg_move_normal_y * avg_move_normal_y
                                 if norm == 0:
                                     avg_move_normal_x = move_normal_x
@@ -601,15 +602,15 @@
                                 new_normals.extend((0, 0, -1))
                                 new_normals.extend((move_normal_x, move_normal_y, 0))
                                 first = vertex_k // 3
                                 new_indices = triangulate_rectangle(first, first + 1,
                                                                     first + 2, first + 3)
 
                             next_move = get_next_move(model_data, layer_idx, gline_idx)
-                            next_is_extruding = next_move and next_move.extruding
+                            next_is_extruding = interpolated or next_move and next_move.extruding
                             if not next_is_extruding:
                                 # Compute caps and link everything
                                 p1x = current_pos[0] - path_halfwidth * move_normal_x
                                 p2x = current_pos[0] + path_halfwidth * move_normal_x
                                 p1y = current_pos[1] - path_halfwidth * move_normal_y
                                 p2y = current_pos[1] + path_halfwidth * move_normal_y
                                 new_vertices.extend((current_pos[0], current_pos[1], current_pos[2] + path_halfheight))
@@ -643,26 +644,29 @@
 
                             new_vertices_len = len(new_vertices)
                             vertices[vertex_k:vertex_k+new_vertices_len] = new_vertices
                             normals[vertex_k:vertex_k+new_vertices_len] = new_normals
                             vertex_k += new_vertices_len
 
                             new_vertices_count = new_vertices_len//coordspervertex
-                            # settings support alpha (transperancy), but it is ignored here
+                            # settings support alpha (transparency), but it is ignored here
                             gline_color = self.movement_color(gline)[:buffered_color_len]
                             for vi in range(new_vertices_count):
                                 colors[color_k:color_k+buffered_color_len] = gline_color
                                 color_k += buffered_color_len
 
                             prev_move_normal_x = move_normal_x
                             prev_move_normal_y = move_normal_y
                             prev_move_angle = move_angle
 
                         prev_pos = current_pos
+                        prev_extruding = gline.extruding
+
                     prev_gline = gline
+                    prev_extruding = gline.extruding
                     count_travel_indices.append(travel_vertex_k // 3)
                     count_print_indices.append(index_k)
                     count_print_vertices.append(vertex_k // 3)
                     gline.gcview_end_vertex = len(count_print_indices) - 1
 
                 if has_movement:
                     self.layer_stops.append(len(count_print_indices) - 1)
@@ -950,15 +954,15 @@
                 for gline in layer:
                     if not gline.is_move:
                         continue
                     if gline.x is None and gline.y is None and gline.z is None:
                         continue
 
                     has_movement = True
-                    for current_pos in interpolate_arcs(gline, prev_gline):
+                    for (current_pos, interpolated) in interpolate_arcs(gline, prev_gline):
 
                         if self.vertices.size < (vertex_k + 100 * 6):
                             # arc interpolation extra points allocation
                             ratio = (vertex_k + 100 * 6) / self.vertices.size * 1.5
                             # print(f"gl realloc lite {self.vertices.size} -> {int(self.vertices.size * ratio)}")
                             self.vertices.resize(int(self.vertices.size * ratio), refcheck = False)
                             self.colors.resize(int(self.colors.size * ratio), refcheck = False)
```

### Comparing `Printrun-2.0.0rc7/printrun/gl/panel.py` & `Printrun-2.0.1/printrun/gl/panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,15 +201,15 @@
         glEnable(GL_BLEND)
         glBlendFunc(GL_SRC_ALPHA, GL_ONE_MINUS_SRC_ALPHA)
         if call_reshape:
             self.OnReshape()
 
     def OnReshape(self):
         """Reshape the OpenGL viewport based on the size of the window"""
-        size = self.GetClientSize()
+        size = self.GetClientSize() * self.GetContentScaleFactor()
         oldwidth, oldheight = self.width, self.height
         width, height = size.width, size.height
         if width < 1 or height < 1:
             return
         self.width = max(float(width), 1.0)
         self.height = max(float(height), 1.0)
         self.OnInitGL(call_reshape = False)
@@ -264,22 +264,22 @@
         glEnable(GL_NORMALIZE)
         glShadeModel(GL_SMOOTH)
 
     def reset_mview(self, factor):
         glMatrixMode(GL_MODELVIEW)
         glLoadIdentity()
         self.setup_lights()
-        if self.orthographic:
-            wratio = self.width / self.dist
-            hratio = self.height / self.dist
-            minratio = float(min(wratio, hratio))
-            self.zoom_factor = 1.0
-            self.zoomed_width = wratio / minratio
-            self.zoomed_height = hratio / minratio
-            glScalef(factor * minratio, factor * minratio, 1)
+
+        wratio = self.width / self.dist
+        hratio = self.height / self.dist
+        minratio = float(min(wratio, hratio))
+        self.zoom_factor = 1.0
+        self.zoomed_width = wratio / minratio
+        self.zoomed_height = hratio / minratio
+        glScalef(factor * minratio, factor * minratio, 1)
 
     def DrawCanvas(self):
         """Draw the window."""
         #import time
         #start = time.perf_counter()
         # print('DrawCanvas', self.canvas.GetClientRect())
         self.pygletcontext.set_current()
@@ -322,15 +322,15 @@
     # To be implemented by a sub class
     # ==========================================================================
     def create_objects(self):
         '''create opengl objects when opengl is initialized'''
         pass
 
     def update_object_resize(self):
-        '''called when the window recieves only if opengl is initialized'''
+        '''called when the window receives only if opengl is initialized'''
         pass
 
     def draw_objects(self):
         '''called in the middle of ondraw after the buffer has been cleared'''
         pass
 
     # ==========================================================================
@@ -424,38 +424,40 @@
 
         rx = p2y-p1y
         self.angle_x+=rx
         rota = axis_to_quat([1.0,0.0,0.0],self.angle_x)
         return mulquat(rotz,rota)
 
     def handle_rotation(self, event):
+        content_scale_factor = self.GetContentScaleFactor()
         if self.initpos is None:
-            self.initpos = event.GetPosition()
+            self.initpos = event.GetPosition() * content_scale_factor
         else:
             p1 = self.initpos
-            p2 = event.GetPosition()
-            sz = self.GetClientSize()
+            p2 = event.GetPosition() * content_scale_factor
+            sz = self.GetClientSize() * content_scale_factor
             p1x = p1[0] / (sz[0] / 2) - 1
             p1y = 1 - p1[1] / (sz[1] / 2)
             p2x = p2[0] / (sz[0] / 2) - 1
             p2y = 1 - p2[1] / (sz[1] / 2)
             quat = trackball(p1x, p1y, p2x, p2y, self.dist / 250.0)
             with self.rot_lock:
                 if self.orbit_control:
                     self.basequat = self.orbit(p1x, p1y, p2x, p2y)
                 else:
                     self.basequat = mulquat(self.basequat, quat)
             self.initpos = p2
 
     def handle_translation(self, event):
+        content_scale_factor = self.GetContentScaleFactor()
         if self.initpos is None:
-            self.initpos = event.GetPosition()
+            self.initpos = event.GetPosition() * content_scale_factor
         else:
             p1 = self.initpos
-            p2 = event.GetPosition()
+            p2 = event.GetPosition() * content_scale_factor
             if self.orthographic:
                 x1, y1, _ = self.mouse_to_3d(p1[0], p1[1])
                 x2, y2, _ = self.mouse_to_3d(p2[0], p2[1])
                 glTranslatef(x2 - x1, y2 - y1, 0)
             else:
                 glTranslatef(p2[0] - p1[0], -(p2[1] - p1[1]), 0)
             self.initpos = p2
```

### Comparing `Printrun-2.0.0rc7/printrun/gl/trackball.py` & `Printrun-2.0.1/printrun/gl/trackball.py`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/printrun/gui/__init__.py` & `Printrun-2.0.1/printrun/gui/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,15 @@
             self.lowersizer.Add(rightpanel, 1, wx.EXPAND)
         self.mainsizer.Add(upperpanel, 0, wx.EXPAND)
         self.mainsizer.Add(lowerpanel, 1, wx.EXPAND)
         self.panel.SetSizer(self.mainsizer)
         self.panel.Bind(wx.EVT_MOUSE_EVENTS, self.editbutton)
 
         self.mainsizer.Layout()
-        # This prevents resizing below a reasonnable value
+        # This prevents resizing below a reasonable value
         # We sum the lowersizer (left pane / viz / log) min size
         # the toolbar height and the statusbar/menubar sizes
         minsize = [0, 0]
         minsize[0] = self.lowersizer.GetMinSize()[0]  # lower pane
         minsize[1] = max(viz_pane.GetMinSize()[1], controls_sizer.GetMinSize()[1])
         minsize[1] += self.toolbarsizer.GetMinSize()[1]  # toolbar height
         displaysize = wx.DisplaySize()
```

### Comparing `Printrun-2.0.0rc7/printrun/gui/bufferedcanvas.py` & `Printrun-2.0.1/printrun/gui/bufferedcanvas.py`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/printrun/gui/controls.py` & `Printrun-2.0.1/printrun/gui/controls.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
     speedsizer.Add(root.speed_setbtn, flag = wx.ALIGN_CENTER)
     speedpanel.SetSizer(speedsizer)
     add("speedcontrol", speedpanel, flag = wx.EXPAND)
 
     def speedslider_spin(event):
         value = root.speed_spin.GetValue()
         root.speed_setbtn.SetBackgroundColour("red")
-        root.speed_slider.SetValue(value)
+        root.speed_slider.SetValue(int(value))
     root.speed_spin.Bind(wx.EVT_SPINCTRLDOUBLE, speedslider_spin)
 
     def speedslider_scroll(event):
         value = root.speed_slider.GetValue()
         root.speed_setbtn.SetBackgroundColour("red")
         root.speed_spin.SetValue(value)
     root.speed_slider.Bind(wx.EVT_SCROLL, speedslider_scroll)
@@ -227,15 +227,15 @@
     flowsizer.Add(root.flow_setbtn, flag = wx.ALIGN_CENTER)
     flowpanel.SetSizer(flowsizer)
     add("flowcontrol", flowpanel, flag = wx.EXPAND)
 
     def flowslider_spin(event):
         value = root.flow_spin.GetValue()
         root.flow_setbtn.SetBackgroundColour("red")
-        root.flow_slider.SetValue(value)
+        root.flow_slider.SetValue(int(value))
     root.flow_spin.Bind(wx.EVT_SPINCTRLDOUBLE, flowslider_spin)
 
     def flowslider_scroll(event):
         value = root.flow_slider.GetValue()
         root.flow_setbtn.SetBackgroundColour("red")
         root.flow_spin.SetValue(value)
     root.flow_slider.Bind(wx.EVT_SCROLL, flowslider_scroll)
```

### Comparing `Printrun-2.0.0rc7/printrun/gui/graph.py` & `Printrun-2.0.1/printrun/gui/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,34 +136,34 @@
 
         # gc.SetBrush(gc.CreateBrush(wx.Brush(wx.Colour(0, 0, 0, 255))))
         gc.SetPen(wx.Pen(wx.Colour(255, 0, 0, 255), 1))
 
         # gc.DrawLines(wx.Point(0, 0), wx.Point(50, 10))
 
         font = wx.Font(10, wx.DEFAULT, wx.NORMAL, wx.BOLD)
-        gc.SetFont(font, wx.Colour(23, 44, 44))
+        gc.SetFont(font, wx.Colour(self.root.settings.graph_color_text))
 
         # draw vertical bars
-        dc.SetPen(wx.Pen(wx.Colour(225, 225, 225), 1))
+        dc.SetPen(wx.Pen(wx.Colour(self.root.settings.graph_color_grid), 1))
         xscale = float(self.width - 1) / (self.xbars - 1)
         for x in range(self.xbars + 1):
             x = x * xscale
-            dc.DrawLine(x, 0, x, self.height)
+            dc.DrawLine(int(x), 0, int(x), self.height)
 
         # draw horizontal bars
         spacing = self._calculate_spacing()  # spacing between bars, in degrees
         yspan = self.maxyvalue - self.minyvalue
         ybars = int(yspan / spacing)  # Should be close to self.ybars
         firstbar = int(ceil(self.minyvalue / spacing))  # in degrees
-        dc.SetPen(wx.Pen(wx.Colour(225, 225, 225), 1))
+        dc.SetPen(wx.Pen(wx.Colour(self.root.settings.graph_color_grid), 1))
         for y in range(firstbar, firstbar + ybars + 1):
             # y_pos = y*(float(self.height)/self.ybars)
             degrees = y * spacing
             y_pos = self._y_pos(degrees)
-            dc.DrawLine(0, y_pos, self.width, y_pos)
+            dc.DrawLine(0, int(y_pos), self.width, int(y_pos))
             label = str(y * spacing)
             label_y = y_pos - font.GetPointSize() / 2
             self.layoutText(label, 1, label_y, gc)
             gc.DrawText(label, 1, label_y)
 
         if not self.timer.IsRunning():
             font = wx.Font(14, wx.DEFAULT, wx.NORMAL, wx.BOLD)
@@ -203,48 +203,47 @@
             return 25 * 10 ** (exponent - 1)
         elif log25_5 <= log_yspan - exponent < log5_10:
             return 5 * 10 ** exponent
         else:
             return 10 ** (exponent + 1)
 
     def drawtemperature(self, dc, gc, temperature_list,
-                        text, text_xoffset, r, g, b, a):
-        color = self.timer.IsRunning() and (r, g, b, a) or [128] * 4
-        dc.SetPen(wx.Pen(color, 1))
+                        text, text_xoffset, color):
+        rgba = wx.Colour(color if self.timer.IsRunning() else '#80808080')
+        dc.SetPen(wx.Pen(rgba, 1))
 
         x_add = float(self.width) / self.xsteps
         x_pos = 0.0
         lastxvalue = 0.0
         lastyvalue = temperature_list[-1]
 
         for temperature in temperature_list:
             y_pos = self._y_pos(temperature)
             if x_pos > 0:  # One need 2 points to draw a line.
-                dc.DrawLine(lastxvalue, lastyvalue, x_pos, y_pos)
+                dc.DrawLine(int(lastxvalue), int(lastyvalue), int(x_pos), int(y_pos))
 
             lastxvalue = x_pos
             x_pos += x_add
             lastyvalue = y_pos
 
         if text:
             font = wx.Font(8, wx.DEFAULT, wx.NORMAL, wx.BOLD)
             # font = wx.Font(8, wx.DEFAULT, wx.NORMAL, wx.NORMAL)
-            gc.SetFont(font, color[:3])
+            gc.SetFont(font, wx.Colour(rgba.RGB))
 
-            text_size = len(text) * text_xoffset + 1
             pos = self.layoutText(text, lastxvalue, lastyvalue, gc)
             gc.DrawText(text, pos.x, pos.y)
 
     def layoutRect(self, rc):
         res = LtRect(rc)
         reserved = sorted((rs for rs in self.reserved
             if not (rc.bottom < rs.top or rc.top > rs.bottom)),
             key=wx.Rect.GetLeft)
         self.boundRect(res)
-        # search to the left for gaps large enough to accomodate res
+        # search to the left for gaps large enough to accommodate res
         rci = bisect_left(reserved, res)
 
         for i in range(rci, len(reserved)-1):
             res.x = reserved[i].right + 1
             if res.right < reserved[i+1].left:
                 #found good res
                 break
@@ -288,45 +287,45 @@
                 res.y = bottom+1
                 if res.bottom >= self.height:
                     res.y = rc.y
         return res
 
     def layoutText(self, text, x, y, gc):
         ext = gc.GetTextExtent(text)
-        rc = self.layoutRect(wx.Rect(x, y, *ext))
+        rc = self.layoutRect(wx.Rect(int(x), int(y), int(ext[0]), int(ext[1])))
         # print('layoutText', text, rc.TopLeft)
         return rc
 
     def drawfanpower(self, dc, gc):
         self.drawtemperature(dc, gc, self.fanpowers,
-                             "Fan", 1, 0, 0, 0, 128)
+                             "Fan", 1, self.root.settings.graph_color_fan)
 
     def drawbedtemp(self, dc, gc):
         self.drawtemperature(dc, gc, self.bedtemps,
-                             "Bed", 2, 255, 0, 0, 128)
+                             "Bed", 2, self.root.settings.graph_color_bedtemp)
 
     def drawbedtargettemp(self, dc, gc):
         self.drawtemperature(dc, gc, self.bedtargettemps,
-                             "Bed Target", 2, 255, 120, 0, 128)
+                             "Bed Target", 2, self.root.settings.graph_color_bedtarget)
 
     def drawextruder0temp(self, dc, gc):
         self.drawtemperature(dc, gc, self.extruder0temps,
-                             "Ex0", 1, 0, 155, 255, 128)
+                             "Ex0", 1, self.root.settings.graph_color_ex0temp)
 
     def drawextruder0targettemp(self, dc, gc):
         self.drawtemperature(dc, gc, self.extruder0targettemps,
-                             "Ex0 Target", 2, 0, 5, 255, 128)
+                             "Ex0 Target", 2, self.root.settings.graph_color_ex0target)
 
     def drawextruder1temp(self, dc, gc):
         self.drawtemperature(dc, gc, self.extruder1temps,
-                             "Ex1", 3, 55, 55, 0, 128)
+                             "Ex1", 3, self.root.settings.graph_color_ex1temp)
 
     def drawextruder1targettemp(self, dc, gc):
         self.drawtemperature(dc, gc, self.extruder1targettemps,
-                             "Ex1 Target", 2, 55, 55, 0, 128)
+                             "Ex1 Target", 2, self.root.settings.graph_color_ex1target)
 
     def SetFanPower(self, value):
         self.fanpowers.pop()
         self.fanpowers.append(value)
 
     def AddFanPower(self, value):
         self.fanpowers.append(value)
@@ -419,15 +418,15 @@
         self.drawextruder0targettemp(dc, gc)
         self.drawextruder0temp(dc, gc)
         if self.extruder1targettemps[-1]>0 or self.extruder1temps[-1]>5:
             self.drawextruder1targettemp(dc, gc)
             self.drawextruder1temp(dc, gc)
 
     class _YBounds:
-        """Small helper class to claculate y bounds dynamically"""
+        """Small helper class to calculate y bounds dynamically"""
 
         def __init__(self, graph, minimum_scale=5.0, buffer=0.10):
             """_YBounds(Graph,float,float)
 
             graph           parent object to calculate scales for
             minimum_scale   minimum range to show on the graph
             buffer          amount of padding to add above & below the
```

### Comparing `Printrun-2.0.0rc7/printrun/gui/log.py` & `Printrun-2.0.1/printrun/gui/log.py`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/printrun/gui/toolbar.py` & `Printrun-2.0.1/printrun/gui/toolbar.py`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/printrun/gui/utils.py` & `Printrun-2.0.1/printrun/gui/utils.py`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/printrun/gui/viz.py` & `Printrun-2.0.1/printrun/gui/viz.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,16 @@
                 import printrun.gcview
                 root.gviz = printrun.gcview.GcodeViewMainWrapper(
                     parentpanel,
                     root.build_dimensions_list,
                     root = root,
                     circular = root.settings.circular_bed,
                     antialias_samples = int(root.settings.antialias3dsamples),
-                    grid = (root.settings.preview_grid_step1, root.settings.preview_grid_step2))
+                    grid = (root.settings.preview_grid_step1, root.settings.preview_grid_step2),
+                    perspective = root.settings.perspective)
                 root.gviz.clickcb = root.show_viz_window
             except:
                 use2dview = True
                 logging.error("3D view mode requested, but we failed to initialize it.\n"
                               + "Falling back to 2D view, and here is the backtrace:\n"
                               + traceback.format_exc())
         if use2dview:
@@ -100,15 +101,16 @@
                 root.gwindow = printrun.gcview.GcodeViewFrame(None, wx.ID_ANY, 'Gcode view, shift to move view, mousewheel to set layer',
                     size = (600, 600),
                     build_dimensions = root.build_dimensions_list,
                     objects = objects,
                     root = root,
                     circular = root.settings.circular_bed,
                     antialias_samples = int(root.settings.antialias3dsamples),
-                    grid = (root.settings.preview_grid_step1, root.settings.preview_grid_step2))
+                    grid = (root.settings.preview_grid_step1, root.settings.preview_grid_step2),
+                    perspective=root.settings.perspective)
             except:
                 use3dview = False
                 logging.error("3D view mode requested, but we failed to initialize it.\n"
                               + "Falling back to 2D view, and here is the backtrace:\n"
                               + traceback.format_exc())
         if not use3dview:
             from printrun import gviz
```

### Comparing `Printrun-2.0.0rc7/printrun/gui/widgets.py` & `Printrun-2.0.1/printrun/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/printrun/gui/xybuttons.py` & `Printrun-2.0.1/printrun/gui/xybuttons.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
         for idx, kpos in self.keypad_positions.items():
             radius = self.distanceToPoint(mpos[0], mpos[1], kpos[0], kpos[1])
             if radius < XYButtons.keypad_radius:
                 return idx
         return None
 
     def drawPartialPie(self, gc, center, r1, r2, angle1, angle2):
-        p1 = wx.Point(center.x + r1 * math.cos(angle1), center.y + r1 * math.sin(angle1))
+        p1 = wx.Point(int(center.x + r1 * math.cos(angle1)), int(center.y + r1 * math.sin(angle1)))
 
         path = gc.CreatePath()
         path.MoveToPoint(p1.x, p1.y)
         path.AddArc(center.x, center.y, r1, angle1, angle2, True)
         path.AddArc(center.x, center.y, r2, angle2, angle1, False)
         path.AddLineToPoint(p1.x, p1.y)
         gc.DrawPath(path)
```

### Comparing `Printrun-2.0.0rc7/printrun/gui/zbuttons.py` & `Printrun-2.0.1/printrun/gui/zbuttons.py`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/printrun/gviz.py` & `Printrun-2.0.1/printrun/gviz.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,15 @@
         self.hilightarcs = deque()
         self.hilightqueue = Queue(0)
         self.hilightarcsqueue = Queue(0)
         self.clear()
         self.filament_width = extrusion_width  # set it to 0 to disable scaling lines with zoom
         self.update_basescale()
         self.scale = self.basescale
-        penwidth = max(1.0, self.filament_width * ((self.scale[0] + self.scale[1]) / 2.0))
+        penwidth = max(1, int(self.filament_width * ((self.scale[0] + self.scale[1]) / 2.0)))
         self.translate = [0.0, 0.0]
         self.mainpen = wx.Pen(wx.Colour(0, 0, 0), penwidth)
         self.arcpen = wx.Pen(wx.Colour(255, 0, 0), penwidth)
         self.travelpen = wx.Pen(wx.Colour(10, 80, 80), penwidth)
         self.hlpen = wx.Pen(wx.Colour(200, 50, 50), penwidth)
         self.fades = [wx.Pen(wx.Colour(int(250 - 0.6 ** i * 100), int(250 - 0.6 ** i * 100), int(200 - 0.4 ** i * 50)), penwidth) for i in range(6)]
         self.penslist = [self.mainpen, self.arcpen, self.travelpen, self.hlpen] + self.fades
@@ -288,25 +288,25 @@
         if x == -1 and y == -1:
             side = min(self.size)
             x = y = side / 2
         self.scale = [s * factor for s in self.scale]
 
         self.translate = [x - (x - self.translate[0]) * factor,
                           y - (y - self.translate[1]) * factor]
-        penwidth = max(1.0, self.filament_width * ((self.scale[0] + self.scale[1]) / 2.0))
+        penwidth = max(1, int(self.filament_width * ((self.scale[0] + self.scale[1]) / 2.0)))
         for pen in self.penslist:
             pen.SetWidth(penwidth)
         self.dirty = True
         wx.CallAfter(self.Refresh)
 
     def _line_scaler(self, x):
-        return (self.scale[0] * x[0],
-                self.scale[1] * x[1],
-                self.scale[0] * x[2],
-                self.scale[1] * x[3],)
+        return (int(self.scale[0] * x[0]),
+                int(self.scale[1] * x[1]),
+                int(self.scale[0] * x[2]),
+                int(self.scale[1] * x[3]),)
 
     def _arc_scaler(self, x):
         return (self.scale[0] * x[0],
                 self.scale[1] * x[1],
                 self.scale[0] * x[2],
                 self.scale[1] * x[3],
                 self.scale[0] * x[4],
@@ -322,37 +322,37 @@
         for i in range(len(scaled_arcs)):
             dc.SetPen(pens[i] if isinstance(pens, numpy.ndarray) else pens)
             dc.DrawArc(*scaled_arcs[i])
 
     def repaint_everything(self):
         width = self.scale[0] * self.build_dimensions[0]
         height = self.scale[1] * self.build_dimensions[1]
-        self.blitmap = wx.Bitmap(width + 1, height + 1, -1)
+        self.blitmap = wx.Bitmap(int(width) + 1, int(height) + 1, -1)
         dc = wx.MemoryDC()
         dc.SelectObject(self.blitmap)
         dc.SetBackground(wx.Brush((250, 250, 200)))
         dc.Clear()
         dc.SetPen(wx.Pen(wx.Colour(180, 180, 150)))
         for grid_unit in self.grid:
             if grid_unit > 0:
                 for x in range(int(self.build_dimensions[0] / grid_unit) + 1):
                     draw_x = self.scale[0] * x * grid_unit
-                    dc.DrawLine(draw_x, 0, draw_x, height)
+                    dc.DrawLine(int(draw_x), 0, int(draw_x), int(height))
                 for y in range(int(self.build_dimensions[1] / grid_unit) + 1):
                     draw_y = self.scale[1] * (self.build_dimensions[1] - y * grid_unit)
-                    dc.DrawLine(0, draw_y, width, draw_y)
+                    dc.DrawLine(0, int(draw_y), int(width), int(draw_y))
             dc.SetPen(wx.Pen(wx.Colour(0, 0, 0)))
 
         if not self.showall:
             # Draw layer gauge
             dc.SetBrush(wx.Brush((43, 144, 255)))
-            dc.DrawRectangle(width - 15, 0, 15, height)
+            dc.DrawRectangle(int(width) - 15, 0, 15, int(height))
             dc.SetBrush(wx.Brush((0, 255, 0)))
             if self.layers:
-                dc.DrawRectangle(width - 14, (1.0 - (1.0 * (self.layerindex + 1)) / len(self.layers)) * height, 13, height - 1)
+                dc.DrawRectangle(int(width) - 14, int((1.0 - (1.0 * (self.layerindex + 1)) / len(self.layers)) * height), 13, int(height) - 1)
 
         if self.showall:
             for i in range(len(self.layersz)):
                 self.painted_layers.add(i)
                 self._drawlines(dc, self.lines[i], self.pens[i])
                 self._drawarcs(dc, self.arcs[i], self.arcpens[i])
             dc.SelectObject(wx.NullBitmap)
@@ -406,15 +406,15 @@
         elif self.partial:
             self.partial = False
             self.repaint_partial()
         self.paint_hilights()
         dc = wx.PaintDC(self)
         dc.SetBackground(wx.Brush(self.bgcolor))
         dc.Clear()
-        dc.DrawBitmap(self.blitmap, self.translate[0], self.translate[1])
+        dc.DrawBitmap(self.blitmap, int(self.translate[0]), int(self.translate[1]))
         if self.paint_overlay:
             self.paint_overlay(dc)
 
     def addfile_perlayer(self, gcode, showall = False):
         self.clear()
         self.gcode = gcode
         self.showall = showall
```

### Comparing `Printrun-2.0.0rc7/printrun/injectgcode.py` & `Printrun-2.0.1/printrun/injectgcode.py`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/printrun/objectplater.py` & `Printrun-2.0.1/printrun/objectplater.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         model.offsets = [model.offsets[0] + delta[0],
                          model.offsets[1] + delta[1],
                          model.offsets[2]
                          ]
         return True
 
     def rotate_shape(self, angle):
-        """rotates acive shape
+        """rotates active shape
         positive angle is clockwise
         """
         name = self.l.GetSelection()
         if name == wx.NOT_FOUND:
             return False
         name = self.l.GetString(name)
         model = self.models[name]
```

### Comparing `Printrun-2.0.0rc7/printrun/packer.py` & `Printrun-2.0.1/printrun/packer.py`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/printrun/plugins/__init__.py` & `Printrun-2.0.1/printrun/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/printrun/plugins/sample.py` & `Printrun-2.0.1/printrun/plugins/sample.py`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/printrun/power/__init__.py` & `Printrun-2.0.1/printrun/power/__init__.py`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/printrun/power/osx.py` & `Printrun-2.0.1/printrun/power/osx.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 
 import ctypes
 import CoreFoundation
 import objc
 
 def SetUpIOFramework():
     # load the IOKit library
-    framework = ctypes.cdll.LoadLibrary(
-        '/System/Library/Frameworks/IOKit.framework/IOKit')
+    framework = ctypes.cdll.LoadLibrary('/System/Library/Frameworks/IOKit.framework/IOKit')
 
     # declare parameters as described in IOPMLib.h
     framework.IOPMAssertionCreateWithName.argtypes = [
         ctypes.c_void_p,  # CFStringRef
         ctypes.c_uint32,  # IOPMAssertionLevel
         ctypes.c_void_p,  # CFStringRef
         ctypes.POINTER(ctypes.c_uint32)]  # IOPMAssertionID
```

### Comparing `Printrun-2.0.0rc7/printrun/printcore.py` & `Printrun-2.0.1/printrun/printcore.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Printrun.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = "2.0.0rc7"
+__version__ = "2.0.1"
 
 import sys
 if sys.version_info.major < 3:
     print("You need to run this on Python 3")
     sys.exit(-1)
 
 from serial import Serial, SerialException, PARITY_ODD, PARITY_NONE
@@ -346,32 +346,36 @@
                     except: self.logError(traceback.format_exc())
                 if self.loud: logging.info("RECV: %s" % line.rstrip())
             return line
         except UnicodeDecodeError:
             self.logError(_("Got rubbish reply from %s at baudrate %s:") % (self.port, self.baud) +
                               "\n" + _("Maybe a bad baudrate?"))
             return None
-        except SelectError as e:
-            if 'Bad file descriptor' in e.args[1]:
-                self.logError(_("Can't read from printer (disconnected?) (SelectError {0}): {1}").format(e.errno, decode_utf8(e.strerror)))
-                return None
-            else:
-                self.logError(_("SelectError ({0}): {1}").format(e.errno, decode_utf8(e.strerror)))
-                raise
         except SerialException as e:
             self.logError(_("Can't read from printer (disconnected?) (SerialException): {0}").format(decode_utf8(str(e))))
             return None
         except socket.error as e:
             self.logError(_("Can't read from printer (disconnected?) (Socket error {0}): {1}").format(e.errno, decode_utf8(e.strerror)))
             return None
-        except OSError as e:
-            if e.errno == errno.EAGAIN:  # Not a real error, no data was available
-                return ""
-            self.logError(_("Can't read from printer (disconnected?) (OS Error {0}): {1}").format(e.errno, e.strerror))
-            return None
+        except (OSError, SelectError) as e:
+            # OSError and SelectError are the same thing since python 3.3
+            if self.printer_tcp:
+                # SelectError branch, assume select is used only for socket printers
+                if len(e.args) > 1 and 'Bad file descriptor' in e.args[1]:
+                    self.logError(_("Can't read from printer (disconnected?) (SelectError {0}): {1}").format(e.errno, decode_utf8(e.strerror)))
+                    return None
+                else:
+                    self.logError(_("SelectError ({0}): {1}").format(e.errno, decode_utf8(e.strerror)))
+                    raise
+            else:
+                # OSError branch, serial printers
+                if e.errno == errno.EAGAIN:  # Not a real error, no data was available
+                    return ""
+                self.logError(_("Can't read from printer (disconnected?) (OS Error {0}): {1}").format(e.errno, e.strerror))
+                return None
 
     def _listen_can_continue(self):
         if self.printer_tcp:
             return not self.stop_read_thread and self.printer
         return (not self.stop_read_thread
                 and self.printer
                 and self.printer.is_open)
@@ -489,18 +493,20 @@
         if self.printing or not self.online or not self.printer:
             return False
         self.queueindex = startindex
         self.mainqueue = gcode
         self.printing = True
         self.lineno = 0
         self.resendfrom = -1
-        self._send("M110", -1, True)
         if not gcode or not gcode.lines:
             return True
+
         self.clear = False
+        self._send("M110", -1, True)
+
         resuming = (startindex != 0)
         self.print_thread = threading.Thread(target = self._print,
                                              name = 'print thread',
                                              kwargs = {"resuming": resuming})
         self.print_thread.start()
         return True
 
@@ -508,78 +514,69 @@
         self.pause()
         self.paused = False
         self.mainqueue = None
         self.clear = True
 
     # run a simple script if it exists, no multithreading
     def runSmallScript(self, filename):
-        if filename is None: return
-        f = None
+        if not filename: return
         try:
             with open(filename) as f:
                 for i in f:
                     l = i.replace("\n", "")
-                    l = l[:l.find(";")]  # remove comments
+                    l = l.partition(';')[0]  # remove comments
                     self.send_now(l)
         except:
             pass
 
     def pause(self):
         """Pauses the print, saving the current position.
         """
         if not self.printing: return False
         self.paused = True
         self.printing = False
 
-        # try joining the print thread: enclose it in try/except because we
-        # might be calling it from the thread itself
-        try:
-            self.print_thread.join()
-        except RuntimeError as e:
-            if e.message == "cannot join current thread":
-                pass
-            else:
+        # ';@pause' in the gcode file calls pause from the print thread
+        if not threading.current_thread() is self.print_thread:
+            try:
+                self.print_thread.join()
+            except:
                 self.logError(traceback.format_exc())
-        except:
-            self.logError(traceback.format_exc())
 
         self.print_thread = None
 
         # saves the status
         self.pauseX = self.analyzer.abs_x
         self.pauseY = self.analyzer.abs_y
         self.pauseZ = self.analyzer.abs_z
         self.pauseE = self.analyzer.abs_e
         self.pauseF = self.analyzer.current_f
         self.pauseRelative = self.analyzer.relative
+        self.pauseRelativeE = self.analyzer.relative_e
 
     def resume(self):
-        """Resumes a paused print.
-        """
+        """Resumes a paused print."""
         if not self.paused: return False
-        if self.paused:
-            # restores the status
-            self.send_now("G90")  # go to absolute coordinates
-
-            xyFeedString = ""
-            zFeedString = ""
-            if self.xy_feedrate is not None:
-                xyFeedString = " F" + str(self.xy_feedrate)
-            if self.z_feedrate is not None:
-                zFeedString = " F" + str(self.z_feedrate)
-
-            self.send_now("G1 X%s Y%s%s" % (self.pauseX, self.pauseY,
-                                            xyFeedString))
-            self.send_now("G1 Z" + str(self.pauseZ) + zFeedString)
-            self.send_now("G92 E" + str(self.pauseE))
-
-            # go back to relative if needed
-            if self.pauseRelative: self.send_now("G91")
-            # reset old feed rate
-            self.send_now("G1 F" + str(self.pauseF))
+        # restores the status
+        self.send_now("G90")  # go to absolute coordinates
+
+        xyFeed = '' if self.xy_feedrate is None else ' F' + str(self.xy_feedrate)
+        zFeed = '' if self.z_feedrate is None else ' F' + str(self.z_feedrate)
+
+        self.send_now("G1 X%s Y%s%s" % (self.pauseX, self.pauseY, xyFeed))
+        self.send_now("G1 Z" + str(self.pauseZ) + zFeed)
+        self.send_now("G92 E" + str(self.pauseE))
+
+        # go back to relative if needed
+        if self.pauseRelative:
+            self.send_now("G91")
+        if self.pauseRelativeE:
+            self.send_now('M83')
+        # reset old feed rate
+        self.send_now("G1 F" + str(self.pauseF))
 
         self.paused = False
         self.printing = True
         self.print_thread = threading.Thread(target = self._print,
                                              name = 'print thread',
                                              kwargs = {"resuming": True})
         self.print_thread.start()
```

### Comparing `Printrun-2.0.0rc7/printrun/projectlayer.py` & `Printrun-2.0.1/printrun/projectlayer.py`

 * *Files 26% similar despite different names*

```diff
@@ -86,99 +86,103 @@
             dc.SelectObject(self.bitmap)
             dc.SetBackground(wx.Brush("black"))
             dc.Clear()
 
             if self.slicer == 'Slic3r' or self.slicer == 'Skeinforge':
 
                 if self.scale != 1.0:
-                    layercopy = copy.deepcopy(image)
-                    height = float(layercopy.get('height').replace('m', ''))
-                    width = float(layercopy.get('width').replace('m', ''))
-
-                    layercopy.set('height', str(height * self.scale) + 'mm')
-                    layercopy.set('width', str(width * self.scale) + 'mm')
-                    layercopy.set('viewBox', '0 0 ' + str(width * self.scale) + ' ' + str(height * self.scale))
+                    image = copy.deepcopy(image)
+                    height = float(image.get('height').replace('m', ''))
+                    width = float(image.get('width').replace('m', ''))
+
+                    image.set('height', str(height * self.scale) + 'mm')
+                    image.set('width', str(width * self.scale) + 'mm')
+                    image.set('viewBox', '0 0 ' + str(width * self.scale) + ' ' + str(height * self.scale))
 
-                    g = layercopy.find("{http://www.w3.org/2000/svg}g")
+                    g = image.find("{http://www.w3.org/2000/svg}g")
                     g.set('transform', 'scale(' + str(self.scale) + ')')
-                    stream = io.StringIO(PNGSurface.convert(dpi = self.dpi, bytestring = xml.etree.ElementTree.tostring(layercopy)))
-                else:
-                    stream = io.StringIO(PNGSurface.convert(dpi = self.dpi, bytestring = xml.etree.ElementTree.tostring(image)))
 
-                pngImage = wx.ImageFromStream(stream)
+                pngbytes = PNGSurface.convert(dpi = self.dpi, bytestring = xml.etree.ElementTree.tostring(image))
+                pngImage = wx.Image(io.BytesIO(pngbytes))
 
-                # print "w:", pngImage.Width, ", dpi:", self.dpi, ", w (mm): ",(pngImage.Width / self.dpi) * 25.4
+                #print("w:", pngImage.Width, ", dpi:", self.dpi, ", w (mm): ",(pngImage.Width / self.dpi) * 25.4)
 
                 if self.layer_red:
                     pngImage = pngImage.AdjustChannels(1, 0, 0, 1)
 
-                dc.DrawBitmap(wx.BitmapFromImage(pngImage), self.offset[0], self.offset[1], True)
+                # AGE2022-07-31 Python 3.10 and DrawBitmap expects offset 
+                # as integer value. Convert float values to int
+                dc.DrawBitmap(wx.Bitmap(pngImage), int(self.offset[0]), int(self.offset[1]), True)
 
             elif self.slicer == 'bitmap':
                 if isinstance(image, str):
                     image = wx.Image(image)
                 if self.layer_red:
                     image = image.AdjustChannels(1, 0, 0, 1)
-                dc.DrawBitmap(wx.BitmapFromImage(image.Scale(image.Width * self.scale, image.Height * self.scale)), self.offset[0], -self.offset[1], True)
+                bitmap = wx.Bitmap(image.Scale(image.Width * self.scale, image.Height * self.scale))
+                dc.DrawBitmap(bitmap, self.offset[0], -self.offset[1], True)
             else:
                 raise Exception(self.slicer + " is an unknown method.")
 
             self.pic.SetBitmap(self.bitmap)
             self.pic.Show()
             self.Refresh()
 
         except:
             raise
             pass
 
     def show_img_delay(self, image):
-        print("Showing", str(time.clock()))
+        print("Showing", str(time.perf_counter()))
         self.control_frame.set_current_layer(self.index)
         self.draw_layer(image)
-        wx.FutureCall(1000 * self.interval, self.hide_pic_and_rise)
+        # AGe 2022-07-31 Python 3.10 and CallLater expects delay in millyseconds as 
+        # integer value instead of float. Convert float value to int
+        wx.CallLater(int(1000 * self.interval), self.hide_pic_and_rise)
 
     def rise(self):
-        if (self.direction == "Top Down"):
-            print("Lowering", str(time.clock()))
+        if self.direction == "Top Down":
+            print("Lowering", str(time.perf_counter()))
         else:
-            print("Rising", str(time.clock()))
+            print("Rising", str(time.perf_counter()))
 
         if self.printer is not None and self.printer.online:
             self.printer.send_now("G91")
 
-            if (self.prelift_gcode):
+            if self.prelift_gcode:
                 for line in self.prelift_gcode.split('\n'):
                     if line:
                         self.printer.send_now(line)
 
-            if (self.direction == "Top Down"):
+            if self.direction == "Top Down":
                 self.printer.send_now("G1 Z-%f F%g" % (self.overshoot, self.z_axis_rate,))
                 self.printer.send_now("G1 Z%f F%g" % (self.overshoot - self.thickness, self.z_axis_rate,))
             else:  # self.direction == "Bottom Up"
                 self.printer.send_now("G1 Z%f F%g" % (self.overshoot, self.z_axis_rate,))
                 self.printer.send_now("G1 Z-%f F%g" % (self.overshoot - self.thickness, self.z_axis_rate,))
 
-            if (self.postlift_gcode):
+            if self.postlift_gcode:
                 for line in self.postlift_gcode.split('\n'):
                     if line:
                         self.printer.send_now(line)
 
             self.printer.send_now("G90")
         else:
             time.sleep(self.pause)
 
-        wx.FutureCall(1000 * self.pause, self.next_img)
+        # AGe 2022-07-31 Python 3.10 expects delay in millyseconds as integer value instead of float. Convert float value to int
+        wx.CallLater(int(1000 * self.pause), self.next_img)
 
     def hide_pic(self):
-        print("Hiding", str(time.clock()))
+        print("Hiding", str(time.perf_counter()))
         self.pic.Hide()
 
     def hide_pic_and_rise(self):
         wx.CallAfter(self.hide_pic)
-        wx.FutureCall(500, self.rise)
+        wx.CallLater(500, self.rise)
 
     def next_img(self):
         if not self.running:
             return
         if self.index < len(self.layers):
             print(self.index)
             wx.CallAfter(self.show_img_delay, self.layers[self.index])
@@ -235,229 +239,231 @@
             except AttributeError:
                 return val
         else:
             return val
 
     def __init__(self, parent, printer = None):
         wx.Frame.__init__(self, parent, title = "ProjectLayer Control", style = (wx.DEFAULT_FRAME_STYLE | wx.WS_EX_CONTEXTHELP))
-        self.SetExtraStyle(wx.FRAME_EX_CONTEXTHELP)
         self.pronterface = parent
         self.display_frame = DisplayFrame(self, title = "ProjectLayer Display", printer = printer)
 
         self.panel = wx.Panel(self)
 
-        vbox = wx.BoxSizer(wx.VERTICAL)
-        buttonbox = wx.StaticBoxSizer(wx.StaticBox(self.panel, label = "Controls"), wx.HORIZONTAL)
+        # In wxPython 4.1.0 gtk3 (phoenix) wxWidgets 3.1.4
+        # Layout() breaks before Show(), invoke once after Show()
+        def fit(ev):
+            self.Fit()
+            self.Unbind(wx.EVT_ACTIVATE, handler=fit)
+        self.Bind(wx.EVT_ACTIVATE, fit)
+
+        buttonGroup = wx.StaticBox(self.panel, label = "Controls")
+        buttonbox = wx.StaticBoxSizer(buttonGroup, wx.HORIZONTAL)
 
-        load_button = wx.Button(self.panel, -1, "Load")
+        load_button = wx.Button(buttonGroup, -1, "Load")
         load_button.Bind(wx.EVT_BUTTON, self.load_file)
-        load_button.SetHelpText("Choose an SVG file created from Slic3r or Skeinforge, or a zip file of bitmap images (with extension: .3dlp.zip).")
+        load_button.SetToolTip("Choose an SVG file created from Slic3r or Skeinforge, or a zip file of bitmap images (with extension: .3dlp.zip).")
         buttonbox.Add(load_button, flag = wx.LEFT | wx.RIGHT | wx.BOTTOM, border = 5)
 
-        present_button = wx.Button(self.panel, -1, "Present")
+        present_button = wx.Button(buttonGroup, -1, "Present")
         present_button.Bind(wx.EVT_BUTTON, self.start_present)
-        present_button.SetHelpText("Starts the presentation of the slices.")
+        present_button.SetToolTip("Starts the presentation of the slices.")
         buttonbox.Add(present_button, flag = wx.LEFT | wx.RIGHT | wx.BOTTOM, border = 5)
 
-        self.pause_button = wx.Button(self.panel, -1, "Pause")
+        self.pause_button = wx.Button(buttonGroup, -1, "Pause")
         self.pause_button.Bind(wx.EVT_BUTTON, self.pause_present)
-        self.pause_button.SetHelpText("Pauses the presentation. Can be resumed afterwards by clicking this button, or restarted by clicking present again.")
+        self.pause_button.SetToolTip("Pauses the presentation. Can be resumed afterwards by clicking this button, or restarted by clicking present again.")
         buttonbox.Add(self.pause_button, flag = wx.LEFT | wx.RIGHT | wx.BOTTOM, border = 5)
 
-        stop_button = wx.Button(self.panel, -1, "Stop")
+        stop_button = wx.Button(buttonGroup, -1, "Stop")
         stop_button.Bind(wx.EVT_BUTTON, self.stop_present)
-        stop_button.SetHelpText("Stops presenting the slices.")
+        stop_button.SetToolTip("Stops presenting the slices.")
         buttonbox.Add(stop_button, flag = wx.LEFT | wx.RIGHT | wx.BOTTOM, border = 5)
 
-        self.help_button = wx.ContextHelpButton(self.panel)
-        buttonbox.Add(self.help_button, flag = wx.LEFT | wx.RIGHT | wx.BOTTOM, border = 5)
-
-        fieldboxsizer = wx.StaticBoxSizer(wx.StaticBox(self.panel, label = "Settings"), wx.VERTICAL)
+        settingsGroup = wx.StaticBox(self.panel, label = "Settings")
+        fieldboxsizer = wx.StaticBoxSizer(settingsGroup, wx.VERTICAL)
         fieldsizer = wx.GridBagSizer(10, 10)
 
         # Left Column
 
-        fieldsizer.Add(wx.StaticText(self.panel, -1, "Layer (mm):"), pos = (0, 0), flag = wx.ALIGN_CENTER_VERTICAL)
-        self.thickness = wx.TextCtrl(self.panel, -1, str(self._get_setting("project_layer", "0.1")), size = (125, -1))
+        fieldsizer.Add(wx.StaticText(settingsGroup, -1, "Layer (mm):"), pos = (0, 0), flag = wx.ALIGN_CENTER_VERTICAL)
+        self.thickness = wx.TextCtrl(settingsGroup, -1, str(self._get_setting("project_layer", "0.1")), size = (125, -1))
         self.thickness.Bind(wx.EVT_TEXT, self.update_thickness)
-        self.thickness.SetHelpText("The thickness of each slice. Should match the value used to slice the model.  SVG files update this value automatically, 3dlp.zip files have to be manually entered.")
+        self.thickness.SetToolTip("The thickness of each slice. Should match the value used to slice the model.  SVG files update this value automatically, 3dlp.zip files have to be manually entered.")
         fieldsizer.Add(self.thickness, pos = (0, 1))
 
-        fieldsizer.Add(wx.StaticText(self.panel, -1, "Exposure (s):"), pos = (1, 0), flag = wx.ALIGN_CENTER_VERTICAL)
-        self.interval = wx.TextCtrl(self.panel, -1, str(self._get_setting("project_interval", "0.5")), size = (125, -1))
+        fieldsizer.Add(wx.StaticText(settingsGroup, -1, "Exposure (s):"), pos = (1, 0), flag = wx.ALIGN_CENTER_VERTICAL)
+        self.interval = wx.TextCtrl(settingsGroup, -1, str(self._get_setting("project_interval", "0.5")), size = (125, -1))
         self.interval.Bind(wx.EVT_TEXT, self.update_interval)
-        self.interval.SetHelpText("How long each slice should be displayed.")
+        self.interval.SetToolTip("How long each slice should be displayed.")
         fieldsizer.Add(self.interval, pos = (1, 1))
 
-        fieldsizer.Add(wx.StaticText(self.panel, -1, "Blank (s):"), pos = (2, 0), flag = wx.ALIGN_CENTER_VERTICAL)
-        self.pause = wx.TextCtrl(self.panel, -1, str(self._get_setting("project_pause", "0.5")), size = (125, -1))
+        fieldsizer.Add(wx.StaticText(settingsGroup, -1, "Blank (s):"), pos = (2, 0), flag = wx.ALIGN_CENTER_VERTICAL)
+        self.pause = wx.TextCtrl(settingsGroup, -1, str(self._get_setting("project_pause", "0.5")), size = (125, -1))
         self.pause.Bind(wx.EVT_TEXT, self.update_pause)
-        self.pause.SetHelpText("The pause length between slices. This should take into account any movement of the Z axis, plus time to prepare the resin surface (sliding, tilting, sweeping, etc).")
+        self.pause.SetToolTip("The pause length between slices. This should take into account any movement of the Z axis, plus time to prepare the resin surface (sliding, tilting, sweeping, etc).")
         fieldsizer.Add(self.pause, pos = (2, 1))
 
-        fieldsizer.Add(wx.StaticText(self.panel, -1, "Scale:"), pos = (3, 0), flag = wx.ALIGN_CENTER_VERTICAL)
-        self.scale = wx.SpinCtrlDouble(self.panel, -1, initial = self._get_setting('project_scale', 1.0), inc = 0.1, size = (125, -1))
+        fieldsizer.Add(wx.StaticText(settingsGroup, -1, "Scale:"), pos = (3, 0), flag = wx.ALIGN_CENTER_VERTICAL)
+        self.scale = wx.SpinCtrlDouble(settingsGroup, -1, initial = self._get_setting('project_scale', 1.0), inc = 0.1, size = (125, -1))
         self.scale.SetDigits(3)
         self.scale.Bind(wx.EVT_SPINCTRLDOUBLE, self.update_scale)
-        self.scale.SetHelpText("The additional scaling of each slice.")
+        self.scale.SetToolTip("The additional scaling of each slice.")
         fieldsizer.Add(self.scale, pos = (3, 1))
 
-        fieldsizer.Add(wx.StaticText(self.panel, -1, "Direction:"), pos = (4, 0), flag = wx.ALIGN_CENTER_VERTICAL)
-        self.direction = wx.ComboBox(self.panel, -1, choices = ["Top Down", "Bottom Up"], value = self._get_setting('project_direction', "Top Down"), size = (125, -1))
+        fieldsizer.Add(wx.StaticText(settingsGroup, -1, "Direction:"), pos = (4, 0), flag = wx.ALIGN_CENTER_VERTICAL)
+        self.direction = wx.ComboBox(settingsGroup, -1, choices = ["Top Down", "Bottom Up"], value = self._get_setting('project_direction', "Top Down"), size = (125, -1))
         self.direction.Bind(wx.EVT_COMBOBOX, self.update_direction)
-        self.direction.SetHelpText("The direction the Z axis should move. Top Down is where the projector is above the model, Bottom up is where the projector is below the model.")
+        self.direction.SetToolTip("The direction the Z axis should move. Top Down is where the projector is above the model, Bottom up is where the projector is below the model.")
         fieldsizer.Add(self.direction, pos = (4, 1), flag = wx.ALIGN_CENTER_VERTICAL)
 
-        fieldsizer.Add(wx.StaticText(self.panel, -1, "Overshoot (mm):"), pos = (5, 0), flag = wx.ALIGN_CENTER_VERTICAL)
-        self.overshoot = wx.SpinCtrlDouble(self.panel, -1, initial = self._get_setting('project_overshoot', 3.0), inc = 0.1, min = 0, size = (125, -1))
+        fieldsizer.Add(wx.StaticText(settingsGroup, -1, "Overshoot (mm):"), pos = (5, 0), flag = wx.ALIGN_CENTER_VERTICAL)
+        self.overshoot = wx.SpinCtrlDouble(settingsGroup, -1, initial = self._get_setting('project_overshoot', 3.0), inc = 0.1, min = 0, size = (125, -1))
         self.overshoot.SetDigits(1)
         self.overshoot.Bind(wx.EVT_SPINCTRLDOUBLE, self.update_overshoot)
-        self.overshoot.SetHelpText("How far the axis should move beyond the next slice position for each slice. For Top Down printers this would dunk the model under the resi and then return. For Bottom Up printers this would raise the base away from the vat and then return.")
+        self.overshoot.SetToolTip("How far the axis should move beyond the next slice position for each slice. For Top Down printers this would dunk the model under the resi and then return. For Bottom Up printers this would raise the base away from the vat and then return.")
         fieldsizer.Add(self.overshoot, pos = (5, 1))
 
-        fieldsizer.Add(wx.StaticText(self.panel, -1, "Pre-lift Gcode:"), pos = (6, 0), flag = wx.ALIGN_CENTER_VERTICAL)
-        self.prelift_gcode = wx.TextCtrl(self.panel, -1, str(self._get_setting("project_prelift_gcode", "").replace("\\n", '\n')), size = (-1, 35), style = wx.TE_MULTILINE)
-        self.prelift_gcode.SetHelpText("Additional gcode to run before raising the Z axis. Be sure to take into account any additional time needed in the pause value, and be careful what gcode is added!")
+        fieldsizer.Add(wx.StaticText(settingsGroup, -1, "Pre-lift Gcode:"), pos = (6, 0), flag = wx.ALIGN_CENTER_VERTICAL)
+        self.prelift_gcode = wx.TextCtrl(settingsGroup, -1, str(self._get_setting("project_prelift_gcode", "").replace("\\n", '\n')), size = (-1, 35), style = wx.TE_MULTILINE)
+        self.prelift_gcode.SetToolTip("Additional gcode to run before raising the Z axis. Be sure to take into account any additional time needed in the pause value, and be careful what gcode is added!")
         self.prelift_gcode.Bind(wx.EVT_TEXT, self.update_prelift_gcode)
         fieldsizer.Add(self.prelift_gcode, pos = (6, 1), span = (2, 1))
 
-        fieldsizer.Add(wx.StaticText(self.panel, -1, "Post-lift Gcode:"), pos = (6, 2), flag = wx.ALIGN_CENTER_VERTICAL)
-        self.postlift_gcode = wx.TextCtrl(self.panel, -1, str(self._get_setting("project_postlift_gcode", "").replace("\\n", '\n')), size = (-1, 35), style = wx.TE_MULTILINE)
-        self.postlift_gcode.SetHelpText("Additional gcode to run after raising the Z axis. Be sure to take into account any additional time needed in the pause value, and be careful what gcode is added!")
+        fieldsizer.Add(wx.StaticText(settingsGroup, -1, "Post-lift Gcode:"), pos = (6, 2), flag = wx.ALIGN_CENTER_VERTICAL)
+        self.postlift_gcode = wx.TextCtrl(settingsGroup, -1, str(self._get_setting("project_postlift_gcode", "").replace("\\n", '\n')), size = (-1, 35), style = wx.TE_MULTILINE)
+        self.postlift_gcode.SetToolTip("Additional gcode to run after raising the Z axis. Be sure to take into account any additional time needed in the pause value, and be careful what gcode is added!")
         self.postlift_gcode.Bind(wx.EVT_TEXT, self.update_postlift_gcode)
         fieldsizer.Add(self.postlift_gcode, pos = (6, 3), span = (2, 1))
 
         # Right Column
 
-        fieldsizer.Add(wx.StaticText(self.panel, -1, "X (px):"), pos = (0, 2), flag = wx.ALIGN_CENTER_VERTICAL)
+        fieldsizer.Add(wx.StaticText(settingsGroup, -1, "X (px):"), pos = (0, 2), flag = wx.ALIGN_CENTER_VERTICAL)
         projectX = int(math.floor(float(self._get_setting("project_x", 1920))))
-        self.X = wx.SpinCtrl(self.panel, -1, str(projectX), max = 999999, size = (125, -1))
+        self.X = wx.SpinCtrl(settingsGroup, -1, str(projectX), max = 999999, size = (125, -1))
         self.X.Bind(wx.EVT_SPINCTRL, self.update_resolution)
-        self.X.SetHelpText("The projector resolution in the X axis.")
+        self.X.SetToolTip("The projector resolution in the X axis.")
         fieldsizer.Add(self.X, pos = (0, 3))
 
-        fieldsizer.Add(wx.StaticText(self.panel, -1, "Y (px):"), pos = (1, 2), flag = wx.ALIGN_CENTER_VERTICAL)
+        fieldsizer.Add(wx.StaticText(settingsGroup, -1, "Y (px):"), pos = (1, 2), flag = wx.ALIGN_CENTER_VERTICAL)
         projectY = int(math.floor(float(self._get_setting("project_y", 1200))))
-        self.Y = wx.SpinCtrl(self.panel, -1, str(projectY), max = 999999, size = (125, -1))
+        self.Y = wx.SpinCtrl(settingsGroup, -1, str(projectY), max = 999999, size = (125, -1))
         self.Y.Bind(wx.EVT_SPINCTRL, self.update_resolution)
-        self.Y.SetHelpText("The projector resolution in the Y axis.")
+        self.Y.SetToolTip("The projector resolution in the Y axis.")
         fieldsizer.Add(self.Y, pos = (1, 3))
 
-        fieldsizer.Add(wx.StaticText(self.panel, -1, "OffsetX (mm):"), pos = (2, 2), flag = wx.ALIGN_CENTER_VERTICAL)
-        self.offset_X = wx.SpinCtrlDouble(self.panel, -1, initial = self._get_setting("project_offset_x", 0.0), inc = 1, size = (125, -1))
+        fieldsizer.Add(wx.StaticText(settingsGroup, -1, "OffsetX (mm):"), pos = (2, 2), flag = wx.ALIGN_CENTER_VERTICAL)
+        self.offset_X = wx.SpinCtrlDouble(settingsGroup, -1, initial = self._get_setting("project_offset_x", 0.0), inc = 1, size = (125, -1))
         self.offset_X.SetDigits(1)
         self.offset_X.Bind(wx.EVT_SPINCTRLDOUBLE, self.update_offset)
-        self.offset_X.SetHelpText("How far the slice should be offset from the edge in the X axis.")
+        self.offset_X.SetToolTip("How far the slice should be offset from the edge in the X axis.")
         fieldsizer.Add(self.offset_X, pos = (2, 3))
 
-        fieldsizer.Add(wx.StaticText(self.panel, -1, "OffsetY (mm):"), pos = (3, 2), flag = wx.ALIGN_CENTER_VERTICAL)
-        self.offset_Y = wx.SpinCtrlDouble(self.panel, -1, initial = self._get_setting("project_offset_y", 0.0), inc = 1, size = (125, -1))
+        fieldsizer.Add(wx.StaticText(settingsGroup, -1, "OffsetY (mm):"), pos = (3, 2), flag = wx.ALIGN_CENTER_VERTICAL)
+        self.offset_Y = wx.SpinCtrlDouble(settingsGroup, -1, initial = self._get_setting("project_offset_y", 0.0), inc = 1, size = (125, -1))
         self.offset_Y.SetDigits(1)
         self.offset_Y.Bind(wx.EVT_SPINCTRLDOUBLE, self.update_offset)
-        self.offset_Y.SetHelpText("How far the slice should be offset from the edge in the Y axis.")
+        self.offset_Y.SetToolTip("How far the slice should be offset from the edge in the Y axis.")
         fieldsizer.Add(self.offset_Y, pos = (3, 3))
 
-        fieldsizer.Add(wx.StaticText(self.panel, -1, "ProjectedX (mm):"), pos = (4, 2), flag = wx.ALIGN_CENTER_VERTICAL)
-        self.projected_X_mm = wx.SpinCtrlDouble(self.panel, -1, initial = self._get_setting("project_projected_x", 505.0), inc = 1, size = (125, -1))
+        fieldsizer.Add(wx.StaticText(settingsGroup, -1, "ProjectedX (mm):"), pos = (4, 2), flag = wx.ALIGN_CENTER_VERTICAL)
+        self.projected_X_mm = wx.SpinCtrlDouble(settingsGroup, -1, initial = self._get_setting("project_projected_x", 505.0), inc = 1, size = (125, -1))
         self.projected_X_mm.SetDigits(1)
         self.projected_X_mm.Bind(wx.EVT_SPINCTRLDOUBLE, self.update_projected_Xmm)
-        self.projected_X_mm.SetHelpText("The actual width of the entire projected image. Use the Calibrate grid to show the full size of the projected image, and measure the width at the same level where the slice will be projected onto the resin.")
+        self.projected_X_mm.SetToolTip("The actual width of the entire projected image. Use the Calibrate grid to show the full size of the projected image, and measure the width at the same level where the slice will be projected onto the resin.")
         fieldsizer.Add(self.projected_X_mm, pos = (4, 3))
 
-        fieldsizer.Add(wx.StaticText(self.panel, -1, "Z Axis Speed (mm/min):"), pos = (5, 2), flag = wx.ALIGN_CENTER_VERTICAL)
-        self.z_axis_rate = wx.SpinCtrl(self.panel, -1, str(self._get_setting("project_z_axis_rate", 200)), max = 9999, size = (125, -1))
+        fieldsizer.Add(wx.StaticText(settingsGroup, -1, "Z Axis Speed (mm/min):"), pos = (5, 2), flag = wx.ALIGN_CENTER_VERTICAL)
+        self.z_axis_rate = wx.SpinCtrl(settingsGroup, -1, str(self._get_setting("project_z_axis_rate", 200)), max = 9999, size = (125, -1))
         self.z_axis_rate.Bind(wx.EVT_SPINCTRL, self.update_z_axis_rate)
-        self.z_axis_rate.SetHelpText("Speed of the Z axis in mm/minute. Take into account that slower rates may require a longer pause value.")
+        self.z_axis_rate.SetToolTip("Speed of the Z axis in mm/minute. Take into account that slower rates may require a longer pause value.")
         fieldsizer.Add(self.z_axis_rate, pos = (5, 3))
 
         fieldboxsizer.Add(fieldsizer)
 
         # Display
 
-        displayboxsizer = wx.StaticBoxSizer(wx.StaticBox(self.panel, label = "Display"), wx.VERTICAL)
+        displayGroup = wx.StaticBox(self.panel, -1, "Display")
+        displayboxsizer = wx.StaticBoxSizer(displayGroup)
         displaysizer = wx.GridBagSizer(10, 10)
 
-        displaysizer.Add(wx.StaticText(self.panel, -1, "Fullscreen:"), pos = (0, 0), flag = wx.ALIGN_CENTER_VERTICAL)
-        self.fullscreen = wx.CheckBox(self.panel, -1)
+        self.fullscreen = wx.CheckBox(displayGroup, -1, "Fullscreen")
         self.fullscreen.Bind(wx.EVT_CHECKBOX, self.update_fullscreen)
-        self.fullscreen.SetHelpText("Toggles the project screen to full size.")
-        displaysizer.Add(self.fullscreen, pos = (0, 1), flag = wx.ALIGN_CENTER_VERTICAL)
+        self.fullscreen.SetToolTip("Toggles the project screen to full size.")
+        displaysizer.Add(self.fullscreen, pos = (0, 0), flag = wx.ALIGN_CENTER_VERTICAL)
 
-        displaysizer.Add(wx.StaticText(self.panel, -1, "Calibrate:"), pos = (0, 2), flag = wx.ALIGN_CENTER_VERTICAL)
-        self.calibrate = wx.CheckBox(self.panel, -1)
+        self.calibrate = wx.CheckBox(displayGroup, -1, "Calibrate:")
         self.calibrate.Bind(wx.EVT_CHECKBOX, self.show_calibrate)
-        self.calibrate.SetHelpText("Toggles the calibration grid. Each grid should be 10mmx10mm in size. Use the grid to ensure the projected size is correct. See also the help for the ProjectedX field.")
-        displaysizer.Add(self.calibrate, pos = (0, 3), flag = wx.ALIGN_CENTER_VERTICAL)
-
-        displaysizer.Add(wx.StaticText(self.panel, -1, "1st Layer:"), pos = (0, 4), flag = wx.ALIGN_CENTER_VERTICAL)
+        self.calibrate.SetToolTip("Toggles the calibration grid. Each grid should be 10mmx10mm in size. Use the grid to ensure the projected size is correct. See also the help for the ProjectedX field.")
+        displaysizer.Add(self.calibrate, pos = (0, 1), flag = wx.ALIGN_CENTER_VERTICAL)
 
         first_layer_boxer = wx.BoxSizer(wx.HORIZONTAL)
-        self.first_layer = wx.CheckBox(self.panel, -1)
+        self.first_layer = wx.CheckBox(displayGroup, -1, "1st Layer")
         self.first_layer.Bind(wx.EVT_CHECKBOX, self.show_first_layer)
-        self.first_layer.SetHelpText("Displays the first layer of the model. Use this to project the first layer for longer so it holds to the base. Note: this value does not affect the first layer when the \"Present\" run is started, it should be used manually.")
+        self.first_layer.SetToolTip("Displays the first layer of the model. Use this to project the first layer for longer so it holds to the base. Note: this value does not affect the first layer when the \"Present\" run is started, it should be used manually.")
 
         first_layer_boxer.Add(self.first_layer, flag = wx.ALIGN_CENTER_VERTICAL)
 
-        first_layer_boxer.Add(wx.StaticText(self.panel, -1, " (s):"), flag = wx.ALIGN_CENTER_VERTICAL)
-        self.show_first_layer_timer = wx.SpinCtrlDouble(self.panel, -1, initial = -1, inc = 1, size = (125, -1))
+        first_layer_boxer.Add(wx.StaticText(displayGroup, -1, " (s):"), flag = wx.ALIGN_CENTER_VERTICAL)
+        self.show_first_layer_timer = wx.SpinCtrlDouble(displayGroup, -1, initial = -1, min=-1, inc = 1, size = (125, -1))
         self.show_first_layer_timer.SetDigits(1)
-        self.show_first_layer_timer.SetHelpText("How long to display the first layer for. -1 = unlimited.")
+        self.show_first_layer_timer.SetToolTip("How long to display the first layer for. -1 = unlimited.")
         first_layer_boxer.Add(self.show_first_layer_timer, flag = wx.ALIGN_CENTER_VERTICAL)
-        displaysizer.Add(first_layer_boxer, pos = (0, 6), flag = wx.ALIGN_CENTER_VERTICAL)
+        displaysizer.Add(first_layer_boxer, pos = (0, 2), flag = wx.ALIGN_CENTER_VERTICAL)
 
-        displaysizer.Add(wx.StaticText(self.panel, -1, "Red:"), pos = (0, 7), flag = wx.ALIGN_CENTER_VERTICAL)
-        self.layer_red = wx.CheckBox(self.panel, -1)
+        self.layer_red = wx.CheckBox(displayGroup, -1, "Red")
         self.layer_red.Bind(wx.EVT_CHECKBOX, self.show_layer_red)
-        self.layer_red.SetHelpText("Toggles whether the image should be red. Useful for positioning whilst resin is in the printer as it should not cause a reaction.")
-        displaysizer.Add(self.layer_red, pos = (0, 8), flag = wx.ALIGN_CENTER_VERTICAL)
+        self.layer_red.SetToolTip("Toggles whether the image should be red. Useful for positioning whilst resin is in the printer as it should not cause a reaction.")
+        displaysizer.Add(self.layer_red, pos = (0, 3), flag = wx.ALIGN_CENTER_VERTICAL)
 
         displayboxsizer.Add(displaysizer)
 
         # Info
-        infosizer = wx.StaticBoxSizer(wx.StaticBox(self.panel, label = "Info"), wx.VERTICAL)
+        infoGroup = wx.StaticBox(self.panel, label = "Info")
+        infosizer = wx.StaticBoxSizer(infoGroup, wx.VERTICAL)
 
         infofieldsizer = wx.GridBagSizer(10, 10)
 
-        filelabel = wx.StaticText(self.panel, -1, "File:")
-        filelabel.SetHelpText("The name of the model currently loaded.")
+        filelabel = wx.StaticText(infoGroup, -1, "File:")
+        filelabel.SetToolTip("The name of the model currently loaded.")
         infofieldsizer.Add(filelabel, pos = (0, 0))
-        self.filename = wx.StaticText(self.panel, -1, "")
-
+        self.filename = wx.StaticText(infoGroup, -1, "")
         infofieldsizer.Add(self.filename, pos = (0, 1))
 
-        totallayerslabel = wx.StaticText(self.panel, -1, "Total Layers:")
-        totallayerslabel.SetHelpText("The total number of layers found in the model.")
+        totallayerslabel = wx.StaticText(infoGroup, -1, "Total Layers:")
+        totallayerslabel.SetToolTip("The total number of layers found in the model.")
         infofieldsizer.Add(totallayerslabel, pos = (1, 0))
-        self.total_layers = wx.StaticText(self.panel, -1)
+        self.total_layers = wx.StaticText(infoGroup, -1)
 
         infofieldsizer.Add(self.total_layers, pos = (1, 1))
 
-        currentlayerlabel = wx.StaticText(self.panel, -1, "Current Layer:")
-        currentlayerlabel.SetHelpText("The current layer being displayed.")
+        currentlayerlabel = wx.StaticText(infoGroup, -1, "Current Layer:")
+        currentlayerlabel.SetToolTip("The current layer being displayed.")
         infofieldsizer.Add(currentlayerlabel, pos = (2, 0))
-        self.current_layer = wx.StaticText(self.panel, -1, "0")
+        self.current_layer = wx.StaticText(infoGroup, -1, "0")
         infofieldsizer.Add(self.current_layer, pos = (2, 1))
 
-        estimatedtimelabel = wx.StaticText(self.panel, -1, "Estimated Time:")
-        estimatedtimelabel.SetHelpText("An estimate of the remaining time until print completion.")
+        estimatedtimelabel = wx.StaticText(infoGroup, -1, "Estimated Time:")
+        estimatedtimelabel.SetToolTip("An estimate of the remaining time until print completion.")
         infofieldsizer.Add(estimatedtimelabel, pos = (3, 0))
-        self.estimated_time = wx.StaticText(self.panel, -1, "")
+        self.estimated_time = wx.StaticText(infoGroup, -1, "")
         infofieldsizer.Add(self.estimated_time, pos = (3, 1))
 
         infosizer.Add(infofieldsizer)
 
         #
-
+        vbox = wx.BoxSizer(wx.VERTICAL)
         vbox.Add(buttonbox, flag = wx.EXPAND | wx.LEFT | wx.RIGHT | wx.TOP | wx.BOTTOM, border = 10)
         vbox.Add(fieldboxsizer, flag = wx.EXPAND | wx.LEFT | wx.RIGHT | wx.BOTTOM, border = 10)
         vbox.Add(displayboxsizer, flag = wx.EXPAND | wx.LEFT | wx.RIGHT | wx.BOTTOM, border = 10)
         vbox.Add(infosizer, flag = wx.EXPAND | wx.LEFT | wx.RIGHT | wx.BOTTOM, border = 10)
 
-        self.panel.SetSizer(vbox)
-        self.panel.Fit()
+        self.panel.SetSizerAndFit(vbox)
+        bs = wx.BoxSizer(wx.VERTICAL)
+        bs.Add(self.panel, flag=wx.EXPAND)
+        self.SetSizerAndFit(bs)
         self.Fit()
         self.SetPosition((0, 0))
         self.Show()
 
     def __del__(self):
         if hasattr(self, 'image_dir') and self.image_dir != '':
             shutil.rmtree(self.image_dir)
@@ -489,15 +495,15 @@
         et = xml.etree.ElementTree.ElementTree(file = name)
         # xml.etree.ElementTree.dump(et)
 
         slicer = 'Slic3r' if et.getroot().find('{http://www.w3.org/2000/svg}metadata') is None else 'Skeinforge'
         zlast = 0
         zdiff = 0
         ol = []
-        if (slicer == 'Slic3r'):
+        if slicer == 'Slic3r':
             height = et.getroot().get('height').replace('m', '')
             width = et.getroot().get('width').replace('m', '')
 
             for i in et.findall("{http://www.w3.org/2000/svg}g"):
                 z = float(i.get('{http://slic3r.org/namespaces/slic3r}z'))
                 zdiff = z - zlast
                 zlast = z
@@ -659,26 +665,27 @@
                     dc.DrawLine(x * (pixelsXPerMM * 10), 0, x * (pixelsXPerMM * 10), resolution_y_pixels)
 
             self.first_layer.SetValue(False)
             self.display_frame.slicer = 'bitmap'
             self.display_frame.draw_layer(gridBitmap.ConvertToImage())
 
     def present_first_layer(self, event):
-        if (self.first_layer.GetValue()):
+        if self.first_layer.GetValue():
             if not hasattr(self, "layers"):
                 print("No model loaded!")
                 self.first_layer.SetValue(False)
                 return
             self.display_frame.offset = (float(self.offset_X.GetValue()), float(self.offset_Y.GetValue()))
             self.display_frame.scale = float(self.scale.GetValue())
 
             self.display_frame.slicer = self.layers[2]
             self.display_frame.dpi = self.get_dpi()
             self.display_frame.draw_layer(copy.deepcopy(self.layers[0][0]))
             self.calibrate.SetValue(False)
+            self.display_frame.Refresh()
             if self.show_first_layer_timer != -1.0:
                 def unpresent_first_layer():
                     self.display_frame.clear_layer()
                     self.first_layer.SetValue(False)
                 wx.CallLater(self.show_first_layer_timer.GetValue() * 1000, unpresent_first_layer)
 
     def update_offset(self, event):
@@ -746,15 +753,15 @@
 
     def update_direction(self, event):
         direction = self.direction.GetValue()
         self.display_frame.direction = direction
         self._set_setting('project_direction', direction)
 
     def update_fullscreen(self, event):
-        if (self.fullscreen.GetValue()):
+        if self.fullscreen.GetValue():
             self.display_frame.ShowFullScreen(1)
         else:
             self.display_frame.ShowFullScreen(0)
         self.refresh_display(event)
 
     def update_resolution(self, event):
         x = int(self.X.GetValue())
@@ -775,15 +782,15 @@
         if not hasattr(self, "layers"):
             print("No model loaded!")
             return
 
         self.pause_button.SetLabel("Pause")
         self.set_current_layer(0)
         self.display_frame.Raise()
-        if (self.fullscreen.GetValue()):
+        if self.fullscreen.GetValue():
             self.display_frame.ShowFullScreen(1)
         self.display_frame.slicer = self.layers[2]
         self.display_frame.dpi = self.get_dpi()
         self.display_frame.present(self.layers[0][:],
                                    thickness = float(self.thickness.GetValue()),
                                    interval = float(self.interval.GetValue()),
                                    scale = float(self.scale.GetValue()),
@@ -811,12 +818,10 @@
         else:
             print("Continue")
             self.pause_button.SetLabel("Pause")
             self.display_frame.running = True
             self.display_frame.next_img()
 
 if __name__ == "__main__":
-    provider = wx.SimpleHelpProvider()
-    wx.HelpProvider_Set(provider)
     a = wx.App()
-    SettingsFrame(None).Show()
+    SettingsFrame(None)
     a.MainLoop()
```

### Comparing `Printrun-2.0.0rc7/printrun/pronsole.py` & `Printrun-2.0.1/printrun/pronsole.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     try:
         readline.rl.mode.show_all_if_ambiguous = "on"  # config pyreadline on windows
     except:
         pass
 except:
     READLINE = False  # neither readline module is available
 
-tempreading_exp = re.compile("(^T:| T:)")
+tempreading_exp = re.compile('\\bT\d*:')
 
 REPORT_NONE = 0
 REPORT_POS = 1
 REPORT_TEMP = 2
 REPORT_MANUAL = 4
 DEG = "\N{DEGREE SIGN}"
 
@@ -184,15 +184,15 @@
         self.settings._port_list = self.scanserial
         self.update_build_dimensions(None, self.settings.build_dimensions)
         self.update_tcp_streaming_mode(None, self.settings.tcp_streaming_mode)
         self.monitoring = 0
         self.starttime = 0
         self.extra_print_time = 0
         self.silent = False
-        self.commandprefixes = 'MGT$'
+        self.commandprefixes = 'MGTD$'
         self.promptstrs = {"offline": "%(bold)soffline>%(normal)s ",
                            "fallback": "%(bold)s%(red)s%(port)s%(white)s PC>%(normal)s ",
                            "macro": "%(bold)s..>%(normal)s ",
                            "online": "%(bold)s%(green)s%(port)s%(white)s %(extruder_temp_fancy)s%(progress_fancy)s>%(normal)s "}
         self.spool_manager = spoolmanager.SpoolManager(self)
         self.current_tool = 0   # Keep track of the extruder being used
         self.cache_dir = os.path.join(user_cache_dir("Printrun"))
```

### Comparing `Printrun-2.0.0rc7/printrun/pronterface.py` & `Printrun-2.0.1/printrun/pronterface.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,26 @@
 
 from .gui import MainWindow
 from .settings import wxSetting, HiddenSetting, StringSetting, SpinSetting, \
     FloatSpinSetting, BooleanSetting, StaticTextSetting, ColorSetting, ComboSetting
 from printrun import gcoder
 from .pronsole import REPORT_NONE, REPORT_POS, REPORT_TEMP, REPORT_MANUAL
 
+def format_length(mm, fractional=2):
+    if mm <= 10:
+        units = mm
+        suffix = 'mm'
+    elif mm < 1000:
+        units = mm / 10
+        suffix = 'cm'
+    else:
+        units = mm / 1000
+        suffix = 'm'
+    return '%%.%df' % fractional % units + suffix
+
 class ConsoleOutputHandler:
     """Handle console output. All messages go through the logging submodule. We setup a logging handler to get logged messages and write them to both stdout (unless a log file path is specified, in which case we add another logging handler to write to this file) and the log panel.
     We also redirect stdout and stderr to ourself to catch print messages and al."""
 
     def __init__(self, target, log_path):
         self.stdout = sys.stdout
         self.stderr = sys.stderr
@@ -340,30 +352,32 @@
         if not isinstance(event.EventObject, (wx.TextCtrl, wx.ComboBox)) \
             or event.HasModifiers():
             ch = chr(event.KeyCode)
             keys = {'B': self.btemp, 'H': self.htemp, 'J': self.xyb, 'S': self.commandbox,
                 'V': self.gviz}
             widget = keys.get(ch)
             #ignore Alt+(S, H), so it can open Settings, Help menu
-            if widget and (ch not in 'SH' or not event.AltDown()):
+            if widget and (ch not in 'SH' or not event.AltDown()) \
+                and not (event.ControlDown() and ch == 'V'
+                        and event.EventObject is self.commandbox):
                 widget.SetFocus()
                 return
             # On MSWindows button mnemonics are processed only if the
             # focus is in the parent panel
             if event.AltDown() and ch < 'Z':
                 in_toolbar = self.toolbarsizer.GetItem(event.EventObject)
                 candidates = (self.connectbtn, self.connectbtn_cb_var), \
                             (self.pausebtn, self.pause), \
                             (self.printbtn, self.printfile)
                 for ctl, cb in candidates:
                     match = ('&' + ch) in ctl.Label.upper()
                     handled = in_toolbar and match
                     if handled:
                         break
-                    # react to 'P' even for 'Restrart', 'Resume'
+                    # react to 'P' even for 'Restart', 'Resume'
                     # print('match', match, 'handled', handled, ctl.Label, ctl.Enabled)
                     if (match or ch == 'P' and ctl != self.connectbtn) and ctl.Enabled:
                         # print('call', ch, cb)
                         cb()
                         # react to only 1 of 'P' buttons, prefer Resume
                         return
 
@@ -742,31 +756,33 @@
             wx.CallAfter(self.addtexttolog, l)
 
     def addtexttolog(self, text):
         try:
             max_length = 20000
             current_length = self.logbox.GetLastPosition()
             if current_length > max_length:
-                self.logbox.Remove(0, current_length / 10)
+                self.logbox.Remove(0, current_length // 10)
             currentCaretPosition = self.logbox.GetInsertionPoint()
             currentLengthOfText = self.logbox.GetLastPosition()
             if self.autoscrolldisable:
                 self.logbox.Freeze()
                 currentSelectionStart, currentSelectionEnd = self.logbox.GetSelection()
                 self.logbox.SetInsertionPointEnd()
                 self.logbox.AppendText(text)
                 self.logbox.SetInsertionPoint(currentCaretPosition)
                 self.logbox.SetSelection(currentSelectionStart, currentSelectionEnd)
                 self.logbox.Thaw()
             else:
                 self.logbox.SetInsertionPointEnd()
                 self.logbox.AppendText(text)
 
-        except:
+        except UnicodeError:
             self.log(_("Attempted to write invalid text to console, which could be due to an invalid baudrate"))
+        except Exception as e:
+            self.log(_("Unhanded exception: "), repr(e))
 
     def clear_log(self, e):
         self.logbox.Clear()
 
     def set_verbose_communications(self, e):
         self.p.loud = e.IsChecked()
 
@@ -924,17 +940,137 @@
 WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with
 Printrun. If not, see <http://www.gnu.org/licenses/>."""
 
         info.SetLicence(licence)
-        info.AddDeveloper('Kliment Yanev')
-        info.AddDeveloper('Guillaume Seguin')
-
+        info.AddDeveloper('Kliment Yanev @kliment (code)')
+        info.AddDeveloper('Guillaume Seguin @iXce (code)')
+        info.AddDeveloper('@DivingDuck (code)')
+        info.AddDeveloper('@volconst (code)')
+        info.AddDeveloper('Rock Storm @rockstorm101 (code, packaging)')
+        info.AddDeveloper('Miro Hrončok @hroncok (code, packaging)')
+        info.AddDeveloper('Rob Gilson @D1plo1d (code)')
+        info.AddDeveloper('Gary Hodgson @garyhodgson (code)')
+        info.AddDeveloper('Duane Johnson (code,graphics)')
+        info.AddDeveloper('Alessandro Ranellucci @alranel (code)')
+        info.AddDeveloper('Travis Howse @tjhowse (code)')
+        info.AddDeveloper('edef (code)')
+        info.AddDeveloper('Steven Devijver (code)')
+        info.AddDeveloper('Christopher Keller (code)')
+        info.AddDeveloper('Igor Yeremin (code)')
+        info.AddDeveloper('Jeremy Hammett @jezmy (code)')
+        info.AddDeveloper('Spencer Bliven (code)')
+        info.AddDeveloper('Václav \'ax\' Hůla  @AxTheB (code)')
+        info.AddDeveloper('Félix Sipma (code)')
+        info.AddDeveloper('Maja M. @SparkyCola (code)')
+        info.AddDeveloper('Francesco Santini @fsantini (code)')
+        info.AddDeveloper('Cristopher Olah @colah (code)')
+        
+        info.AddDeveloper('Jeremy Kajikawa (code)')
+        info.AddDeveloper('Markus Hitter (code)')
+        info.AddDeveloper('SkateBoss (code)')
+        info.AddDeveloper('Kaz Walker (code)')
+        info.AddDeveloper('Brendan Erwin (documentation)')
+        info.AddDeveloper('Elias (code)')
+        info.AddDeveloper('Jordan Miller (code)')
+        info.AddDeveloper('Mikko Sivulainen (code)')
+        info.AddDeveloper('Clarence Risher (code)')
+        info.AddDeveloper('Guillaume Revaillot (code)')
+        info.AddDeveloper('John Tapsell (code)')
+        info.AddDeveloper('Youness Alaoui (code)')
+        info.AddDeveloper('@eldir (code)')
+        info.AddDeveloper('@hg42 (code)')
+        info.AddDeveloper('@jglauche (code, documentation)')
+        info.AddDeveloper('Ahmet Cem TURAN @ahmetcemturan (icons, code)')
+        info.AddDeveloper('Andrew Dalgleish (code)')
+        info.AddDeveloper('Benny (documentation)')
+        info.AddDeveloper('Chillance (code)')
+        info.AddDeveloper('Ilya Novoselov (code)')
+        info.AddDeveloper('Joeri Hendriks (code)')
+        info.AddDeveloper('Kevin Cole (code)')
+        info.AddDeveloper('pinaise (code)')
+        info.AddDeveloper('Dratone (code)')
+        info.AddDeveloper('ERoth3 (code)')
+        info.AddDeveloper('Erik Zalm (code)')
+        info.AddDeveloper('Felipe Corrêa da Silva Sanches (code)')
+        info.AddDeveloper('Geordie Bilkey (code)')
+        info.AddDeveloper('Ken Aaker (code)')
+        info.AddDeveloper('Lawrence (documentation)')
+        info.AddDeveloper('Loxgen (code)')
+        info.AddDeveloper('Matthias Urlichs (code)')
+        info.AddDeveloper('N Oliver (code)')
+        info.AddDeveloper('@nexus511 (code)')
+        info.AddDeveloper('Sergey Shepelev (code)')
+        info.AddDeveloper('Simon Maillard (code)')
+        info.AddDeveloper('Vanessa Dannenberg (code)')
+        info.AddDeveloper('@beardface (code)')
+        info.AddDeveloper('@hurzl (code)')
+        info.AddDeveloper('Justin Hawkins @beardface (code)')
+        info.AddDeveloper('siorai (documentation)')
+        info.AddDeveloper('tobbelobb (code)')
+        info.AddDeveloper('5ilver (packaging)')
+        info.AddDeveloper('Alexander Hiam (code)')
+        info.AddDeveloper('Alexander Zangerl (code)')
+        info.AddDeveloper('Cameron Currie (code)')
+        info.AddDeveloper('Chris DeLuca (documentation)')
+        info.AddDeveloper('Colin Gilgenbach (code)')
+        info.AddDeveloper('DanLipsitt (code)')
+        info.AddDeveloper('Daniel Holth (code)')
+        info.AddDeveloper('Denis B (code)')
+        info.AddDeveloper('Erik Jonsson (code)')
+        info.AddDeveloper('Felipe Acebes (code)')
+        info.AddDeveloper('Florian Gilcher (code)')
+        info.AddDeveloper('Henrik Brix Andersen (code)')
+        info.AddDeveloper('Jan Wildeboer (documentation)')
+        info.AddDeveloper('Javier Rios (code)')
+        info.AddDeveloper('Jay Proulx (code)')
+        info.AddDeveloper('Jim Morris (code)')
+        info.AddDeveloper('Kyle Evans (code)')
+        info.AddDeveloper('Lenbok (code)')
+        info.AddDeveloper('Lukas Erlacher (code)')
+        info.AddDeveloper('Michael Andresen @blddk (code)')
+        info.AddDeveloper('NeoTheFox (code)')
+        info.AddDeveloper('Nicolas Dandrimont (documentation)')
+        info.AddDeveloper('OhmEye (code)')
+        info.AddDeveloper('OliverEngineer (code)')
+        info.AddDeveloper('Paul Telfort (code)')
+        info.AddDeveloper('Sebastian \'Swift Geek\' Grzywna (code)')
+        info.AddDeveloper('Senthil (documentation)')
+        info.AddDeveloper('Sigma-One (code)')
+        info.AddDeveloper('Spacexula (documentation)')
+        info.AddDeveloper('Stefan Glatzel (code)')
+        info.AddDeveloper('Stefanowicz (code)')
+        info.AddDeveloper('Steven (code)')
+        info.AddDeveloper('Tyler Hovanec (documentation)')
+        info.AddDeveloper('Xabi Xab (code)')
+        info.AddDeveloper('Xoan Sampaiño (code)')
+        info.AddDeveloper('Yuri D\'Elia (code)')
+        info.AddDeveloper('drf5n (code)')
+        info.AddDeveloper('evilB (documentation)')
+        info.AddDeveloper('fieldOfView (code)')
+        info.AddDeveloper('jbh (code)')
+        info.AddDeveloper('kludgineer (code)')
+        info.AddDeveloper('l4nce0 (code)')
+        info.AddDeveloper('palob (code)')
+        info.AddDeveloper('russ (code)')
+        
+        info.AddArtist('Ahmet Cem TURAN @ahmetcemturan (icons, code)')
+        info.AddArtist('Duane Johnson (code,graphics)')
+        
+        info.AddTranslator('freddii (German translation)')
+        info.AddTranslator('Christian Metzen @metzench (German translation)')
+        info.AddTranslator('Cyril Laguilhon-Debat (French translation)')
+        info.AddTranslator('@AvagSayan (Armenian translation)')
+        info.AddTranslator('Jonathan Marsden (French translation)')
+        info.AddTranslator('Ruben Lubbes (NL translation)')
+        info.AddTranslator('aboobed (Arabic translation)')
+        info.AddTranslator('Alessandro Ranellucci @alranel (Italian translation)')
+        
         wx.adv.AboutBox(info)
 
     #  --------------------------------------------------------------
     #  Settings & command line handling (including update callbacks)
     #  --------------------------------------------------------------
 
     def _add_settings(self, size):
@@ -951,14 +1087,15 @@
         self.settings._add(ComboSetting("controlsmode", "Standard", ("Standard", "Mini"), _("Controls mode"), _("Standard controls include all controls needed for printer setup and calibration, while Mini controls are limited to the ones needed for daily printing"), "UI"), self.reload_ui)
         self.settings._add(BooleanSetting("slic3rintegration", False, _("Enable Slic3r integration"), _("Add a menu to select Slic3r profiles directly from Pronterface"), "UI"), self.reload_ui)
         self.settings._add(BooleanSetting("slic3rupdate", False, _("Update Slic3r default presets"), _("When selecting a profile in Slic3r integration menu, also save it as the default Slic3r preset"), "UI"))
         self.settings._add(ComboSetting("mainviz", "3D", ("2D", "3D", "None"), _("Main visualization"), _("Select visualization for main window."), "Viewer"), self.reload_ui)
         self.settings._add(BooleanSetting("viz3d", False, _("Use 3D in GCode viewer window"), _("Use 3D mode instead of 2D layered mode in the visualization window"), "Viewer"), self.reload_ui)
         self.settings._add(StaticTextSetting("separator_3d_viewer", _("3D viewer options"), "", group = "Viewer"))
         self.settings._add(BooleanSetting("light3d", False, _("Use a lighter 3D visualization"), _("Use a lighter visualization with simple lines instead of extruded paths for 3D viewer"), "Viewer"), self.reload_ui)
+        self.settings._add(BooleanSetting("perspective", False, _("Use a perspective view instead of orthographic"), _("A perspective view looks more realistic, but is a bit more confusing to navigate"), "Viewer"), self.reload_ui)
         self.settings._add(ComboSetting("antialias3dsamples", "0", ["0", "2", "4", "8"], _("Number of anti-aliasing samples"), _("Amount of anti-aliasing samples used in the 3D viewer"), "Viewer"), self.reload_ui)
         self.settings._add(BooleanSetting("trackcurrentlayer3d", False, _("Track current layer in main 3D view"), _("Track the currently printing layer in the main 3D visualization"), "Viewer"))
         self.settings._add(FloatSpinSetting("gcview_path_width", 0.4, 0.01, 2, _("Extrusion width for 3D viewer"), _("Width of printed path in 3D viewer"), "Viewer", increment = 0.05), self.update_gcview_params)
         self.settings._add(FloatSpinSetting("gcview_path_height", 0.3, 0.01, 2, _("Layer height for 3D viewer"), _("Height of printed path in 3D viewer"), "Viewer", increment = 0.05), self.update_gcview_params)
         self.settings._add(BooleanSetting("tempgraph", True, _("Display temperature graph"), _("Display time-lapse temperature graph"), "UI"), self.reload_ui)
         self.settings._add(BooleanSetting("tempgauges", False, _("Display temperature gauges"), _("Display graphical gauges for temperatures visualization"), "UI"), self.reload_ui)
         self.settings._add(BooleanSetting("lockbox", False, _("Display interface lock checkbox"), _("Display a checkbox that, when check, locks most of Pronterface"), "UI"), self.reload_ui)
@@ -974,14 +1111,23 @@
         self.settings._add(HiddenSetting("last_temperature", 0.0))
         self.settings._add(StaticTextSetting("separator_2d_viewer", _("2D viewer options"), "", group = "Viewer"))
         self.settings._add(FloatSpinSetting("preview_extrusion_width", 0.5, 0, 10, _("Preview extrusion width"), _("Width of Extrusion in Preview"), "Viewer", increment = 0.1), self.update_gviz_params)
         self.settings._add(SpinSetting("preview_grid_step1", 10., 0, 200, _("Fine grid spacing"), _("Fine Grid Spacing"), "Viewer"), self.update_gviz_params)
         self.settings._add(SpinSetting("preview_grid_step2", 50., 0, 200, _("Coarse grid spacing"), _("Coarse Grid Spacing"), "Viewer"), self.update_gviz_params)
         self.settings._add(ColorSetting("bgcolor", self._preferred_bgcolour_hex(), _("Background color"), _("Pronterface background color"), "Colors", isRGBA=False), self.reload_ui)
         self.settings._add(ColorSetting("graph_color_background", "#FAFAC7", _("Graph background color"), _("Color of the temperature graph background"), "Colors", isRGBA=False), self.reload_ui)
+        self.settings._add(ColorSetting("graph_color_text", "#172C2C", _("Graph text color"), _("Color of the temperature graph text"), "Colors", isRGBA=False), self.reload_ui)
+        self.settings._add(ColorSetting("graph_color_grid", "#5A5A5A", _("Graph grid color"), _("Color of the temperature graph grid"), "Colors", isRGBA=False), self.reload_ui)
+        self.settings._add(ColorSetting("graph_color_fan", "#00000080", _("Graph fan line color"), _("Color of the temperature graph fan speed line"), "Colors"), self.reload_ui)
+        self.settings._add(ColorSetting("graph_color_bedtemp", "#FF000080", _("Graph bed line color"), _("Color of the temperature graph bed temperature line"), "Colors"), self.reload_ui)
+        self.settings._add(ColorSetting("graph_color_bedtarget", "#FF780080", _("Graph bed target line color"), _("Color of the temperature graph bed temperature target line"), "Colors"), self.reload_ui)
+        self.settings._add(ColorSetting("graph_color_ex0temp", "#009BFF80", _("Graph ex0 line color"), _("Color of the temperature graph extruder 0 temperature line"), "Colors"), self.reload_ui)
+        self.settings._add(ColorSetting("graph_color_ex0target", "#0005FF80", _("Graph ex0 target line color"), _("Color of the temperature graph extruder 0 target temperature line"), "Colors"), self.reload_ui)
+        self.settings._add(ColorSetting("graph_color_ex1temp", "#37370080", _("Graph ex1 line color color"), _("Color of the temperature graph extruder 1 temperature line"), "Colors"), self.reload_ui)
+        self.settings._add(ColorSetting("graph_color_ex1target", "#37370080", _("Graph ex1 target line color"), _("Color of the temperature graph extruder 1 temperature target line"), "Colors"), self.reload_ui)
         self.settings._add(ColorSetting("gcview_color_background", "#FAFAC7FF", _("3D view background color"), _("Color of the 3D view background"), "Colors"), self.update_gcview_colors)
         self.settings._add(ColorSetting("gcview_color_travel", "#99999999", _("3D view travel moves color"), _("Color of travel moves in 3D view"), "Colors"), self.update_gcview_colors)
         self.settings._add(ColorSetting("gcview_color_tool0", "#FF000099", _("3D view print moves color"), _("Color of print moves with tool 0 in 3D view"), "Colors"), self.update_gcview_colors)
         self.settings._add(ColorSetting("gcview_color_tool1", "#AC0DFF99", _("3D view tool 1 moves color"), _("Color of print moves with tool 1 in 3D view"), "Colors"), self.update_gcview_colors)
         self.settings._add(ColorSetting("gcview_color_tool2", "#FFCE0099", _("3D view tool 2 moves color"), _("Color of print moves with tool 2 in 3D view"), "Colors"), self.update_gcview_colors)
         self.settings._add(ColorSetting("gcview_color_tool3", "#FF009F99", _("3D view tool 3 moves color"), _("Color of print moves with tool 3 in 3D view"), "Colors"), self.update_gcview_colors)
         self.settings._add(ColorSetting("gcview_color_tool4", "#00FF8F99", _("3D view tool 4 moves color"), _("Color of print moves with tool 4 in 3D view"), "Colors"), self.update_gcview_colors)
@@ -1118,15 +1264,15 @@
             if progress > 0:
                 status_string += _(" Est: %s of %s remaining | ") % (format_duration(secondsremain),
                                                                      format_duration(secondsestimate))
                 status_string += _(" Z: %.3f mm") % self.curlayer
                 if self.settings.display_progress_on_printer and time.time() - self.printer_progress_time >= self.settings.printer_progress_update_interval:
                     self.printer_progress_time = time.time()
                     printer_progress_string = "M117 " + str(round(100 * float(self.p.queueindex) / len(self.p.mainqueue), 2)) + "% Est " + format_duration(secondsremain)
-                    #":" seems to be some kind of seperator for G-CODE"
+                    #":" seems to be some kind of separator for G-CODE"
                     self.p.send_now(printer_progress_string.replace(":", "."))
                     if len(printer_progress_string) > 25:
                         logging.info("Warning: The print progress message might be too long to be displayed properly")
                     #13 chars for up to 99h est.
         elif self.loading_gcode:
             status_string = self.loading_gcode_message
         wx.CallAfter(self.statusbar.SetStatusText, status_string)
@@ -1598,31 +1744,30 @@
             extruder))
         return remainder
 
     def output_gcode_stats(self):
         gcode = self.fgcode
         self.spool_manager.refresh()
 
-        self.log(_("%.2fmm of filament used in this print") % gcode.filament_length)
+        self.log(_("%s of filament used in this print") % format_length(gcode.filament_length))
 
-        if(len(gcode.filament_length_multi)>1):
+        if len(gcode.filament_length_multi) > 1:
             for i in enumerate(gcode.filament_length_multi):
                 if self.spool_manager.getSpoolName(i[0]) == None:
                     logging.info("- Extruder %d: %0.02fmm" % (i[0], i[1]))
                 else:
                     logging.info(("- Extruder %d: %0.02fmm" % (i[0], i[1]) +
                         " from spool '%s' (%.2fmm will remain)" %
                         (self.spool_manager.getSpoolName(i[0]),
                         self.calculate_remaining_filament(i[1], i[0]))))
-        else:
-            if self.spool_manager.getSpoolName(0) != None:
-                self.log(_(
-                    "Using spool '%s' (%.2fmm of filament will remain)" %
+        elif self.spool_manager.getSpoolName(0) != None:
+                self.log(
+                    _("Using spool '%s' (%s of filament will remain)") %
                     (self.spool_manager.getSpoolName(0),
-                    self.calculate_remaining_filament(
+                    format_length(self.calculate_remaining_filament(
                         gcode.filament_length, 0))))
 
         self.log(_("The print goes:"))
         self.log(_("- from %.2f mm to %.2f mm in X and is %.2f mm wide") % (gcode.xmin, gcode.xmax, gcode.width))
         self.log(_("- from %.2f mm to %.2f mm in Y and is %.2f mm deep") % (gcode.ymin, gcode.ymax, gcode.depth))
         self.log(_("- from %.2f mm to %.2f mm in Z and is %.2f mm high") % (gcode.zmin, gcode.zmax, gcode.height))
         self.log(_("Estimated duration: %d layers, %s") % gcode.estimate_duration())
@@ -1645,25 +1790,28 @@
                 while True:
                     global pronterface_quitting
                     if pronterface_quitting:
                         return
                     max_layer = self.viz_last_layer
                     if max_layer is None:
                         break
+                    start_layer = next_layer
                     while next_layer <= max_layer:
-                        assert(next(generator) == next_layer)
+                        assert next(generator) == next_layer
                         next_layer += 1
+                    if next_layer != start_layer:
+                        wx.CallAfter(self.gviz.Refresh)
                     time.sleep(0.1)
                 generator_output = next(generator)
                 while generator_output is not None:
-                    assert(generator_output in (None, next_layer))
+                    assert generator_output == next_layer
                     next_layer += 1
                     generator_output = next(generator)
             else:
-                # If GCode is not being loaded asynchroneously, it is already
+                # If GCode is not being loaded asynchronously, it is already
                 # loaded, so let's make visualization sequentially
                 gcode = self.fgcode
                 self.gviz.addfile(gcode)
             wx.CallAfter(self.gviz.Refresh)
             # Load external window sequentially now that everything is ready.
             # We can't really do any better as the 3D viewer might clone the
             # finalized model from the main visualization
@@ -1685,15 +1833,15 @@
             except:
                 pass
         dlg = wx.FileDialog(self, _("Save as"), basedir, style = wx.FD_SAVE)
         dlg.SetWildcard(_("GCODE files (*.gcode;*.gco;*.g)|*.gcode;*.gco;*.g|All Files (*.*)|*.*"))
         if dlg.ShowModal() == wx.ID_OK:
             name = dlg.GetPath()
             open(name, "w").write("\n".join((line.raw for line in self.fgcode)))
-            self.log(_("G-Code succesfully saved to %s") % name)
+            self.log(_("G-Code successfully saved to %s") % name)
         dlg.Destroy()
 
     #  --------------------------------------------------------------
     #  Printcore callbacks
     #  --------------------------------------------------------------
 
     def process_host_command(self, command):
@@ -1836,44 +1984,39 @@
         pronsole.pronsole.layer_change_cb(self, newlayer)
         if self.settings.mainviz != "3D" or self.settings.trackcurrentlayer3d:
             wx.CallAfter(self.gviz.setlayer, newlayer)
 
     def update_tempdisplay(self):
         try:
             temps = parse_temperature_report(self.tempreadings)
-            if "T0" in temps and temps["T0"][0]:
-                hotend_temp = float(temps["T0"][0])
-            elif "T" in temps and temps["T"][0]:
-                hotend_temp = float(temps["T"][0])
-            else:
-                hotend_temp = None
-            if hotend_temp is not None:
-                if self.display_graph: wx.CallAfter(self.graph.SetExtruder0Temperature, hotend_temp)
-                if self.display_gauges: wx.CallAfter(self.hottgauge.SetValue, hotend_temp)
-                setpoint = None
-                if "T0" in temps and temps["T0"][1]: setpoint = float(temps["T0"][1])
-                elif temps["T"][1]: setpoint = float(temps["T"][1])
-                if setpoint is not None:
-                    if self.display_graph: wx.CallAfter(self.graph.SetExtruder0TargetTemperature, setpoint)
-                    if self.display_gauges: wx.CallAfter(self.hottgauge.SetTarget, setpoint)
-            if "T1" in temps:
-                hotend_temp = float(temps["T1"][0])
-                if self.display_graph: wx.CallAfter(self.graph.SetExtruder1Temperature, hotend_temp)
-                setpoint = temps["T1"][1]
-                if setpoint and self.display_graph:
-                    wx.CallAfter(self.graph.SetExtruder1TargetTemperature, float(setpoint))
-            bed_temp = float(temps["B"][0]) if "B" in temps and temps["B"][0] else None
-            if bed_temp is not None:
-                if self.display_graph: wx.CallAfter(self.graph.SetBedTemperature, bed_temp)
-                if self.display_gauges: wx.CallAfter(self.bedtgauge.SetValue, bed_temp)
-                setpoint = temps["B"][1]
-                if setpoint:
-                    setpoint = float(setpoint)
-                    if self.display_graph: wx.CallAfter(self.graph.SetBedTargetTemperature, setpoint)
-                    if self.display_gauges: wx.CallAfter(self.bedtgauge.SetTarget, setpoint)
+
+            for name in 'T', 'T0', 'T1', 'B':
+                if name not in temps:
+                    continue
+                current = float(temps[name][0])
+                target = float(temps[name][1]) if temps[name][1] else None
+                if name == 'T':
+                    name = 'T0'
+                if self.display_graph:
+                    prefix = 'Set' + name.replace('T', 'Extruder').replace('B', 'Bed')
+                    wx.CallAfter(getattr(self.graph, prefix + 'Temperature'), current)
+                    if target is not None:
+                        wx.CallAfter(getattr(self.graph, prefix + 'TargetTemperature'), target)
+                if self.display_gauges:
+                    if name[0] == 'T':
+                        if name[1] == str(self.current_tool):
+                            def update(c, t):
+                                self.hottgauge.SetValue(c)
+                                self.hottgauge.SetTarget(t or 0)
+                                self.hottgauge.title = _('Heater%s:') % (str(self.current_tool) if self.settings.extruders > 1 else '')
+                            wx.CallAfter(update, current, target)
+                    else:
+                        wx.CallAfter(self.bedtgauge.SetValue, current)
+                        if target is not None:
+                            wx.CallAfter(self.bedtgauge.SetTarget, target)
         except:
             self.logError(traceback.format_exc())
 
     def update_pos(self):
         bits = gcoder.m114_exp.findall(self.posreport)
         x = None
         y = None
@@ -2431,10 +2574,14 @@
 class PronterApp(wx.App):
 
     mainwindow = None
 
     def __init__(self, *args, **kwargs):
         super(PronterApp, self).__init__(*args, **kwargs)
         self.SetAppName("Pronterface")
-        self.locale = wx.Locale(wx.Locale.GetSystemLanguage())
+        lang = wx.Locale.GetSystemLanguage()
+        # Fall back to English if unable to determine language
+        if lang == wx.LANGUAGE_UNKNOWN:
+            lang = wx.LANGUAGE_ENGLISH_US
+        self.locale = wx.Locale(lang)
         self.mainwindow = PronterWindow(self)
         self.mainwindow.Show()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Printrun-2.0.0rc7/printrun/rpc.py` & `Printrun-2.0.1/printrun/rpc.py`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/printrun/settings.py` & `Printrun-2.0.1/printrun/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import traceback
 import os
 import sys
 
 from functools import wraps
 
 from .utils import parse_build_dimensions
+from pathlib import Path
 
 def setting_add_tooltip(func):
     @wraps(func)
     def decorator(self, *args, **kwargs):
         widget = func(self, *args, **kwargs)
         helptxt = self.help or ""
         sep, deftxt = "", ""
@@ -347,15 +348,15 @@
         self._add(StringSetting("slicecommandpath", defaultslicerpath, _("Path to slicer"), _("Path to slicer"), "External"))
         slicer = 'slic3r-console' if sys.platform == 'win32' else 'slic3r'
         self._add(StringSetting("slicecommand", slicer + ' $s --output $o', _("Slice command"), _("Slice command"), "External"))
         self._add(StringSetting("sliceoptscommand", "slic3r", _("Slicer options command"), _("Slice settings command"), "External"))
         self._add(StringSetting("start_command", "", _("Start command"), _("Executable to run when the print is started"), "External"))
         self._add(StringSetting("final_command", "", _("Final command"), _("Executable to run when the print is finished"), "External"))
         self._add(StringSetting("error_command", "", _("Error command"), _("Executable to run when an error occurs"), "External"))
-        self._add(StringSetting("log_path", "", _("Log path"), _("Path to the log file. An empty path will log to the console."), "UI"))
+        self._add(StringSetting("log_path", str(Path.home()), _("Log path"), _("Path to the log file. An empty path will log to the console."), "UI"))
 
         self._add(HiddenSetting("project_offset_x", 0.0))
         self._add(HiddenSetting("project_offset_y", 0.0))
         self._add(HiddenSetting("project_interval", 2.0))
         self._add(HiddenSetting("project_pause", 2.5))
         self._add(HiddenSetting("project_scale", 1.0))
         self._add(HiddenSetting("project_x", 1024))
```

### Comparing `Printrun-2.0.0rc7/printrun/spoolmanager/spoolmanager.py` & `Printrun-2.0.1/printrun/spoolmanager/spoolmanager.py`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/printrun/spoolmanager/spoolmanager_gui.py` & `Printrun-2.0.1/printrun/spoolmanager/spoolmanager_gui.py`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/printrun/stlplater.py` & `Printrun-2.0.1/printrun/stlplater.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,24 +122,24 @@
             p = event.GetPosition()
             dc.DrawLine(self.initpos[0], self.initpos[1], p[0], p[1])
             del dc
         else:
             event.Skip()
 
     def rotate_shape(self, angle):
-        """rotates acive shape
+        """rotates active shape
         positive angle is clockwise
         """
         self.i += angle
         if not self.triggered:
             self.triggered = 1
             threading.Thread(target = self.cr).start()
 
     def keypress(self, event):
-        """gets keypress events and moves/rotates acive shape"""
+        """gets keypress events and moves/rotates active shape"""
         keycode = event.GetKeyCode()
         step = 5
         angle = 18
         if event.ControlDown():
             step = 1
             angle = 1
         # h
```

### Comparing `Printrun-2.0.0rc7/printrun/stltool.py` & `Printrun-2.0.1/printrun/stltool.py`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/printrun/stlview.py` & `Printrun-2.0.1/printrun/stlview.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,17 +68,20 @@
 class StlViewPanel(wxGLPanel):
 
     do_lights = False
 
     def __init__(self, parent, size,
                  build_dimensions = None, circular = False,
                  antialias_samples = 0,
-                 grid = (1, 10)):
+                 grid = (1, 10), perspective=False):
+        if perspective:
+            self.orthographic=False
         super().__init__(parent, wx.DefaultPosition, size, 0,
                                            antialias_samples = antialias_samples)
+        
         self.batches = []
         self.rot = 0
         self.canvas.Bind(wx.EVT_MOUSE_EVENTS, self.move)
         self.canvas.Bind(wx.EVT_MOUSEWHEEL, self.wheel)
         self.canvas.Bind(wx.EVT_LEFT_DCLICK, self.double_click)
         self.initialized = True
         self.parent = parent
@@ -199,15 +202,15 @@
         rotate object
             with shift zoom viewport
         """
         self.handle_wheel(event)
         wx.CallAfter(self.Refresh)
 
     def keypress(self, event):
-        """gets keypress events and moves/rotates acive shape"""
+        """gets keypress events and moves/rotates active shape"""
         keycode = event.GetKeyCode()
         step = 5
         angle = 18
         if event.ControlDown():
             step = 1
             angle = 1
         # h
@@ -266,15 +269,15 @@
         stlview(m.facets, batch = batch)
         m.batch = batch
         # m.animoffset = 300
         # threading.Thread(target = self.anim, args = (m, )).start()
         wx.CallAfter(self.Refresh)
 
     def update_object_resize(self):
-        '''called when the window recieves only if opengl is initialized'''
+        '''called when the window receives only if opengl is initialized'''
         pass
 
     def draw_objects(self):
         '''called in the middle of ondraw after the buffer has been cleared'''
         self.create_objects()
 
         glPushMatrix()
```

### Comparing `Printrun-2.0.0rc7/printrun/zscaper.py` & `Printrun-2.0.1/printrun/zscaper.py`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/pronsole.appdata.xml` & `Printrun-2.0.1/pronsole.appdata.xml`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/pronsole.ico` & `Printrun-2.0.1/pronsole.ico`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/pronsole.png` & `Printrun-2.0.1/pronsole.png`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/pronsole.py` & `Printrun-2.0.1/pronsole.py`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/pronterface.appdata.xml` & `Printrun-2.0.1/pronterface.appdata.xml`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/pronterface.ico` & `Printrun-2.0.1/pronterface.ico`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/pronterface.png` & `Printrun-2.0.1/pronterface.png`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/pronterface.py` & `Printrun-2.0.1/pronterface.py`

 * *Files identical despite different names*

### Comparing `Printrun-2.0.0rc7/setup.py` & `Printrun-2.0.1/setup.py`

 * *Files identical despite different names*

