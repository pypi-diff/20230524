# Comparing `tmp/omgifol-0.5.0.tar.gz` & `tmp/omgifol-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omgifol-0.5.0.tar", last modified: Sat Nov 19 19:36:12 2022, max compression
+gzip compressed data, was "omgifol-0.5.1.tar", last modified: Tue May 23 23:43:20 2023, max compression
```

## Comparing `omgifol-0.5.0.tar` & `omgifol-0.5.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2022-11-19 19:36:12.676401 omgifol-0.5.0/
--rw-rw-rw-   0        0        0     1078 2004-12-28 00:19:20.000000 omgifol-0.5.0/LICENSE
--rw-rw-rw-   0        0        0      492 2022-11-19 19:36:12.676401 omgifol-0.5.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-11-19 19:36:12.633259 omgifol-0.5.0/demo/
--rw-rw-rw-   0        0        0     2431 2022-08-19 02:06:26.000000 omgifol-0.5.0/demo/drawmaps.py
--rw-rw-rw-   0        0        0      998 2022-08-05 01:09:52.000000 omgifol-0.5.0/demo/listdir.py
--rw-rw-rw-   0        0        0      518 2022-08-05 01:09:52.000000 omgifol-0.5.0/demo/merge.py
--rw-rw-rw-   0        0        0     1253 2022-08-05 01:09:52.000000 omgifol-0.5.0/demo/mirror.py
-drwxrwxrwx   0        0        0        0 2022-11-19 19:36:12.669395 omgifol-0.5.0/omg/
--rw-rw-rw-   0        0        0     1370 2022-11-19 19:24:08.000000 omgifol-0.5.0/omg/__init__.py
--rw-rw-rw-   0        0        0     2427 2022-08-05 01:09:52.000000 omgifol-0.5.0/omg/colormap.py
--rw-rw-rw-   0        0        0    20767 2022-08-05 01:09:52.000000 omgifol-0.5.0/omg/lineinfo.py
--rw-rw-rw-   0        0        0    25151 2022-08-05 01:09:52.000000 omgifol-0.5.0/omg/lump.py
--rw-rw-rw-   0        0        0    18082 2022-08-05 01:09:52.000000 omgifol-0.5.0/omg/mapedit.py
--rw-rw-rw-   0        0        0    10313 2022-08-05 01:09:52.000000 omgifol-0.5.0/omg/palette.py
--rw-rw-rw-   0        0        0     2799 2022-08-05 01:09:52.000000 omgifol-0.5.0/omg/playpal.py
--rw-rw-rw-   0        0        0     3718 2022-08-05 01:09:52.000000 omgifol-0.5.0/omg/thinginfo.py
--rw-rw-rw-   0        0        0     4554 2022-08-05 01:09:52.000000 omgifol-0.5.0/omg/txdef.py
--rw-rw-rw-   0        0        0    19309 2022-08-19 02:06:26.000000 omgifol-0.5.0/omg/udmf.py
--rw-rw-rw-   0        0        0     6607 2022-08-05 01:09:52.000000 omgifol-0.5.0/omg/util.py
--rw-rw-rw-   0        0        0    12134 2022-08-19 02:06:26.000000 omgifol-0.5.0/omg/wad.py
--rw-rw-rw-   0        0        0    13213 2022-08-05 01:09:52.000000 omgifol-0.5.0/omg/wadio.py
-drwxrwxrwx   0        0        0        0 2022-11-19 19:36:12.675399 omgifol-0.5.0/omgifol.egg-info/
--rw-rw-rw-   0        0        0      492 2022-11-19 19:36:12.000000 omgifol-0.5.0/omgifol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2022-11-19 19:36:12.000000 omgifol-0.5.0/omgifol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-19 19:36:12.000000 omgifol-0.5.0/omgifol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2022-11-19 19:36:12.000000 omgifol-0.5.0/omgifol.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       59 2022-11-19 19:36:12.677400 omgifol-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0      659 2022-11-19 19:35:51.000000 omgifol-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:43:20.777173 omgifol-0.5.1/
+-rw-rw-rw-   0        0        0     1079 2023-05-23 23:35:12.000000 omgifol-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0      492 2023-05-23 23:43:20.777173 omgifol-0.5.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-23 23:43:20.757168 omgifol-0.5.1/demo/
+-rw-rw-rw-   0        0        0     2355 2023-05-23 23:35:12.000000 omgifol-0.5.1/demo/drawmaps.py
+-rw-rw-rw-   0        0        0      964 2023-05-23 23:35:12.000000 omgifol-0.5.1/demo/listdir.py
+-rw-rw-rw-   0        0        0      499 2023-05-23 23:35:12.000000 omgifol-0.5.1/demo/merge.py
+-rw-rw-rw-   0        0        0     1212 2023-05-23 23:35:12.000000 omgifol-0.5.1/demo/mirror.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:43:20.771171 omgifol-0.5.1/omg/
+-rw-rw-rw-   0        0        0     1336 2023-05-23 23:35:12.000000 omgifol-0.5.1/omg/__init__.py
+-rw-rw-rw-   0        0        0     2366 2023-05-23 23:35:12.000000 omgifol-0.5.1/omg/colormap.py
+-rw-rw-rw-   0        0        0    20153 2023-05-23 23:35:12.000000 omgifol-0.5.1/omg/lineinfo.py
+-rw-rw-rw-   0        0        0    24507 2023-05-23 23:35:12.000000 omgifol-0.5.1/omg/lump.py
+-rw-rw-rw-   0        0        0    17577 2023-05-23 23:35:12.000000 omgifol-0.5.1/omg/mapedit.py
+-rw-rw-rw-   0        0        0    10086 2023-05-23 23:35:12.000000 omgifol-0.5.1/omg/palette.py
+-rw-rw-rw-   0        0        0     2735 2023-05-23 23:35:12.000000 omgifol-0.5.1/omg/playpal.py
+-rw-rw-rw-   0        0        0     3539 2023-05-23 23:35:12.000000 omgifol-0.5.1/omg/thinginfo.py
+-rw-rw-rw-   0        0        0     4428 2023-05-23 23:35:12.000000 omgifol-0.5.1/omg/txdef.py
+-rw-rw-rw-   0        0        0    18715 2023-05-23 23:35:12.000000 omgifol-0.5.1/omg/udmf.py
+-rw-rw-rw-   0        0        0     6391 2023-05-23 23:35:12.000000 omgifol-0.5.1/omg/util.py
+-rw-rw-rw-   0        0        0    11816 2023-05-23 23:35:12.000000 omgifol-0.5.1/omg/wad.py
+-rw-rw-rw-   0        0        0    12869 2023-05-23 23:35:12.000000 omgifol-0.5.1/omg/wadio.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:43:20.776172 omgifol-0.5.1/omgifol.egg-info/
+-rw-rw-rw-   0        0        0      492 2023-05-23 23:43:20.000000 omgifol-0.5.1/omgifol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-05-23 23:43:20.000000 omgifol-0.5.1/omgifol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 23:43:20.000000 omgifol-0.5.1/omgifol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-23 23:43:20.000000 omgifol-0.5.1/omgifol.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       59 2023-05-23 23:43:20.779173 omgifol-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      636 2023-05-23 23:42:50.000000 omgifol-0.5.1/setup.py
```

### Comparing `omgifol-0.5.0/LICENSE` & `omgifol-0.5.1/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2005 Fredrik Johansson
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included
-in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN
-NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
-DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
-OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE
-USE OR OTHER DEALINGS IN THE SOFTWARE.
+Copyright (c) 2005 Fredrik Johansson, 2017 Devin Acker
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included
+in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN
+NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
+DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
+OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE
+USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `omgifol-0.5.0/demo/drawmaps.py` & `omgifol-0.5.1/demo/drawmaps.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-#!/usr/bin/env python
-
-from omg import *
-import sys
-from PIL import Image, ImageDraw
-
-def drawmap(wad, name, filename, width, format):
-    xsize = width - 8
-
-    try:
-        edit = UMapEditor(wad.udmfmaps[name])
-    except KeyError:
-        edit = UMapEditor(wad.maps[name])
-
-    xmin = ymin = float('inf')
-    xmax = ymax = float('-inf')
-    for v in edit.vertexes:
-        xmin = min(xmin, v.x)
-        xmax = max(xmax, v.x)
-        ymin = min(ymin, -v.y)
-        ymax = max(ymax, -v.y)
-
-    scale = xsize / float(xmax - xmin)
-    xmax = xmax * scale
-    xmin = xmin * scale
-    ymax = ymax * scale
-    ymin = ymin * scale
-
-    for v in edit.vertexes:
-        v.x = v.x * scale
-        v.y = -v.y * scale
-
-    im = Image.new('RGB', (int(xmax - xmin) + 8, int(ymax - ymin) + 8), (255,255,255))
-    draw = ImageDraw.Draw(im)
-
-    edit.linedefs.sort(key=lambda a: not a.twosided)
-
-    for line in edit.linedefs:
-         p1x = edit.vertexes[line.v1].x - xmin + 4
-         p1y = edit.vertexes[line.v1].y - ymin + 4
-         p2x = edit.vertexes[line.v2].x - xmin + 4
-         p2y = edit.vertexes[line.v2].y - ymin + 4
-
-         color = (0, 0, 0)
-         if line.twosided:
-             color = (144, 144, 144)
-         if line.special:
-             color = (220, 130, 50)
-
-         draw.line((p1x, p1y, p2x, p2y), fill=color)
-         draw.line((p1x+1, p1y, p2x+1, p2y), fill=color)
-         draw.line((p1x-1, p1y, p2x-1, p2y), fill=color)
-         draw.line((p1x, p1y+1, p2x, p2y+1), fill=color)
-         draw.line((p1x, p1y-1, p2x, p2y-1), fill=color)
-
-    del draw
-
-    im.save(filename, format)
-
-if (len(sys.argv) < 5):
-    print("\n    Omgifol script: draw maps to image files\n")
-    print("    Usage:")
-    print("    drawmaps.py source.wad pattern width format\n")
-    print("    Draw all maps whose names match the given pattern (eg E?M4 or MAP*)")
-    print("    to image files of a given format (PNG, BMP, etc). width specifies the")
-    print("    desired width of the output images.")
-else:
-
-    print("Loading %s..." % sys.argv[1])
-    inwad = WAD()
-    inwad.from_file(sys.argv[1])
-    width = int(sys.argv[3])
-    format = sys.argv[4].upper()
-    for name in inwad.maps.find(sys.argv[2]) + inwad.udmfmaps.find(sys.argv[2]):
-        print("Drawing %s" % name)
-        drawmap(inwad, name, name + "_map" + "." + format.lower(), width, format)
+#!/usr/bin/env python
+
+from omg import *
+import sys
+from PIL import Image, ImageDraw
+
+def drawmap(wad, name, filename, width, format):
+    xsize = width - 8
+
+    try:
+        edit = UMapEditor(wad.udmfmaps[name])
+    except KeyError:
+        edit = UMapEditor(wad.maps[name])
+
+    xmin = ymin = float('inf')
+    xmax = ymax = float('-inf')
+    for v in edit.vertexes:
+        xmin = min(xmin, v.x)
+        xmax = max(xmax, v.x)
+        ymin = min(ymin, -v.y)
+        ymax = max(ymax, -v.y)
+
+    scale = xsize / float(xmax - xmin)
+    xmax = xmax * scale
+    xmin = xmin * scale
+    ymax = ymax * scale
+    ymin = ymin * scale
+
+    for v in edit.vertexes:
+        v.x = v.x * scale
+        v.y = -v.y * scale
+
+    im = Image.new('RGB', (int(xmax - xmin) + 8, int(ymax - ymin) + 8), (255,255,255))
+    draw = ImageDraw.Draw(im)
+
+    edit.linedefs.sort(key=lambda a: not a.twosided)
+
+    for line in edit.linedefs:
+         p1x = edit.vertexes[line.v1].x - xmin + 4
+         p1y = edit.vertexes[line.v1].y - ymin + 4
+         p2x = edit.vertexes[line.v2].x - xmin + 4
+         p2y = edit.vertexes[line.v2].y - ymin + 4
+
+         color = (0, 0, 0)
+         if line.twosided:
+             color = (144, 144, 144)
+         if line.special:
+             color = (220, 130, 50)
+
+         draw.line((p1x, p1y, p2x, p2y), fill=color)
+         draw.line((p1x+1, p1y, p2x+1, p2y), fill=color)
+         draw.line((p1x-1, p1y, p2x-1, p2y), fill=color)
+         draw.line((p1x, p1y+1, p2x, p2y+1), fill=color)
+         draw.line((p1x, p1y-1, p2x, p2y-1), fill=color)
+
+    del draw
+
+    im.save(filename, format)
+
+if (len(sys.argv) < 5):
+    print("\n    Omgifol script: draw maps to image files\n")
+    print("    Usage:")
+    print("    drawmaps.py source.wad pattern width format\n")
+    print("    Draw all maps whose names match the given pattern (eg E?M4 or MAP*)")
+    print("    to image files of a given format (PNG, BMP, etc). width specifies the")
+    print("    desired width of the output images.")
+else:
+
+    print("Loading %s..." % sys.argv[1])
+    inwad = WAD()
+    inwad.from_file(sys.argv[1])
+    width = int(sys.argv[3])
+    format = sys.argv[4].upper()
+    for name in inwad.maps.find(sys.argv[2]) + inwad.udmfmaps.find(sys.argv[2]):
+        print("Drawing %s" % name)
+        drawmap(inwad, name, name + "_map" + "." + format.lower(), width, format)
```

### Comparing `omgifol-0.5.0/demo/mirror.py` & `omgifol-0.5.1/demo/mirror.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-#!/usr/bin/env python
-
-from sys import argv
-from omg import *
-from omg.mapedit import *
-
-def mirror(map):
-    ed = MapEditor(map)
-    for v in ed.vertexes:
-        v.x = -v.x
-    for l in ed.linedefs:
-        l.vx_a, l.vx_b = l.vx_b, l.vx_a
-    for t in ed.things:
-        t.x = -t.x
-        t.angle = (180 - t.angle) % 360
-    ed.nodes = []
-    return ed.to_lumps()
-
-def main(args):
-    if (len(args) < 2):
-        print("    Omgifol script: mirror maps\n")
-        print("    Usage:")
-        print("    mirror.py input.wad output.wad [pattern]\n")
-        print("    Mirror all maps or those whose name match the given pattern")
-        print("    (eg E?M4 or MAP*).")
-        print("    Note: nodes will have to be rebuilt externally.\n")
-    else:
-        print("Loading %s..." % args[0])
-        inwad = WAD()
-        outwad = WAD()
-        inwad.from_file(args[0])
-        pattern = "*"
-        if (len(args) == 3):
-            pattern = args[2]
-        for name in inwad.maps.find(pattern):
-            print("Mirroring %s" % name)
-            outwad.maps[name] = mirror(inwad.maps[name])
-        print("Saving %s..." % args[1])
-        outwad.to_file(args[1])
-
-if __name__ == "__main__": main(argv[1:])
+#!/usr/bin/env python
+
+from sys import argv
+from omg import *
+from omg.mapedit import *
+
+def mirror(map):
+    ed = MapEditor(map)
+    for v in ed.vertexes:
+        v.x = -v.x
+    for l in ed.linedefs:
+        l.vx_a, l.vx_b = l.vx_b, l.vx_a
+    for t in ed.things:
+        t.x = -t.x
+        t.angle = (180 - t.angle) % 360
+    ed.nodes = []
+    return ed.to_lumps()
+
+def main(args):
+    if (len(args) < 2):
+        print("    Omgifol script: mirror maps\n")
+        print("    Usage:")
+        print("    mirror.py input.wad output.wad [pattern]\n")
+        print("    Mirror all maps or those whose name match the given pattern")
+        print("    (eg E?M4 or MAP*).")
+        print("    Note: nodes will have to be rebuilt externally.\n")
+    else:
+        print("Loading %s..." % args[0])
+        inwad = WAD()
+        outwad = WAD()
+        inwad.from_file(args[0])
+        pattern = "*"
+        if (len(args) == 3):
+            pattern = args[2]
+        for name in inwad.maps.find(pattern):
+            print("Mirroring %s" % name)
+            outwad.maps[name] = mirror(inwad.maps[name])
+        print("Saving %s..." % args[1])
+        outwad.to_file(args[1])
+
+if __name__ == "__main__": main(argv[1:])
```

### Comparing `omgifol-0.5.0/omg/__init__.py` & `omgifol-0.5.1/omg/__init__.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-"""
-Omgifol - a Python library for Doom WAD files
-
-Website: http://fredrikj.net/
-
-Copyright (c) 2005 Fredrik Johansson
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included
-in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN
-NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
-DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
-OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE
-USE OR OTHER DEALINGS IN THE SOFTWARE.
-"""
-
-__version__ = '0.5.0'
-__author__  = 'Devin Acker, Fredrik Johansson'
-
-from omg.wadio import *
-from omg.wad import *
-from omg.lump import *
-from omg.mapedit import *
-from omg.udmf import *
+"""
+Omgifol - a Python library for Doom WAD files
+
+Website: http://fredrikj.net/
+
+Copyright (c) 2005 Fredrik Johansson
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included
+in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN
+NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
+DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
+OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE
+USE OR OTHER DEALINGS IN THE SOFTWARE.
+"""
+
+__version__ = '0.5.0'
+__author__  = 'Devin Acker, Fredrik Johansson'
+
+from omg.wadio import *
+from omg.wad import *
+from omg.lump import *
+from omg.mapedit import *
+from omg.udmf import *
```

### Comparing `omgifol-0.5.0/omg/lineinfo.py` & `omgifol-0.5.1/omg/lineinfo.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,614 +1,614 @@
-"""
-lineinfo.py -- dealing with Doom linedef trigger types.
-Provides functions to create a human-readable description
-code from a trigger number, and the inverse operation.
-
-Guide to Trigger Description Codes (R):
-
-Example:        "FLOOR SR UP SLOW CRUSH LNC-8"
-
-Categories:
-    DOOR       - Doors (regular and locked)
-    FLOOR      - Floor movers
-    CEIL       - Ceiling movers
-    PLAT       - Platforms and lifts
-    CRUSHER    - Crushers
-    STAIR      - Stair builders
-    ELEVATOR   - Boom elevators
-    LIGHT      - Light changers
-    EXIT       - Exits
-    TELEPORT   - Teleports
-    DONUT      - Donuts (lower pillar, raise surrounding sector)
-    TRANSFER   - Transfer properties (Boom)
-    SCROLL     - Scroll lines and sectors (Boom)
-
-Trigger types:
-    P1 - Push(door) trigger, works once
-    PR - Push(door) trigger, works repeatedly
-    S1 - Switch, works once
-    SR - Switch, works repeatedly
-    W1 - Walk across, works once
-    WR - Walk across, works repeatedly
-    G1 - Shoot, works once
-    GR - Shoot, works repeatedly
-
-Door locks:
-    YEL - Yellow key lock
-    RED - Red key lock
-    BLU - Blue key lock
-
-Door types:
-    OWC - Open, Wait, Close
-    CWO - Close, Wait, Open
-    OSO - Open, Stay Open
-    CSC - Close, Stay Closed
-
-Motion speed
-    SLOW - Slow
-    NORM - Normal
-    FAST - Fast
-    TURB - Turbo
-    INST - Instant
-
-Delay times
-    3SEC  - 3 seconds
-    4SEC  - 4 seconds
-    30SEC - 30 seconds
-
-Sector property changers:
-    CPYTEX           - Copy Texture
-    CPYTEX+DELTYPE   - Copy Texture, Reset type
-    CPYTEX+TYPE      - Copy Texture and Type
-
-Directions:
-    DOWN    - Down
-    UP      - Up
-    NOMOVE  - Stay (only change properties)
-
-Miscellaneous:
-    SECRET   - A secret exit
-    MONSTER  - Monsters can activate the trigger
-    LINE     - Line teleporters
-    REVERSE  - Line teleporter, reversed
-    SILENT   - Make crushers or teleporters silent
-    CRUSH    - Enable crushing (for CEILs and FLOORs,
-               not to be confused with CRUSHERs)
-
-Destinations/platforms:
-    LNF   - Lowest Neighbor Floor
-    LNC   - Lowest Neighbor Ceiling
-    HNF   - Highest Neighbor Floor
-    HNC   - Highest Neighbor Ceiling
-    NNF   - Next Neighbor Floor
-    NNC   - Next Neighbor Ceiling
-    HNF+8 - 8 above Highest neighbor Floor
-    LNC+8 - 8 under Lowest neighbor Ceiling
-    F+8   - 8 above floor
-    8     - 8 units Absolute  (STAIRs only)
-    16    - 16 units Absolute (STAIRs only)
-    24    - 24 units Absolute
-    32    - 32 units Absolute
-    512   - 512 units absolute
-    SLT   - Shortest Lower Texture
-    SUT   - Shortest Upper Texture
-    NLF   - Next Lowest neighbor Floor
-    NLC   - Next Lowest neighbor Ceiling
-    NHF   - Next Highest neighbor Floor
-    CURRF - Current Floor (ELEVATORs)
-    FLR   - Floor
-    CL    - Ceiling
-    NAF   - Next adjacent floor
-    PERP  - Perpetual
-    STOP  - Stop ongoing motion
-
-Models:
-    TRIG  - Use trigger sector as model
-    NUM   - Lookup adjacent model numerically
-
-Lighting:
-    35    - 35 units
-    255   - 255 units
-    MAXN  - Maximum Neighbor
-    MINN  - Minimum Neighbor
-    BLINK - Blinking
-
-Transfers (check boomref.txt for more info):
-    FLIGHT       - Transfer floor light level
-    CLIGHT       - Transfer ceiling light level
-    TRANSLUCENCY - Transfer line translucency
-    HEIGHTS      - The famous 242!
-    FRICTION     - Transfer friction
-    WIND         - Transfer current
-    POINTFORCE   - Transfer force point (?)
-
-Scrollers (check boomref.txt for more info):
-    CARRY       - Carry objects (conveyor)
-    WRTSECTOR   - With respect to 1st side's sector
-    ACCEL       - Accelerate scrolling
-    RIGHT       - Right direction
-    LEFT        - Left direction
-    WALL        - Scroll wall
-    SYNCED      - Sync scrolling to sector
-    OFFSETS     - Scroll by offsets
-"""
-
-from fnmatch import fnmatchcase
-
-# Define description codes for the standard triggers
-desc2num = \
-{
-  "": 0,
-  "NO ACTION":0,
-# Doors
-  "DOOR PR SLOW OWC 4SEC MONSTER":1,
-  "DOOR PR FAST OWC 4SEC":117,
-  "DOOR SR SLOW OWC 4SEC":63,
-  "DOOR SR FAST OWC 4SEC":114,
-  "DOOR S1 SLOW OWC 4SEC":29,
-  "DOOR S1 FAST OWC 4SEC":111,
-  "DOOR WR SLOW OWC 4SEC":90,
-  "DOOR WR FAST OWC 4SEC":105,
-  "DOOR W1 SLOW OWC 4SEC":4,
-  "DOOR W1 FAST OWC 4SEC":108,
-  "DOOR P1 SLOW OSO":31,
-  "DOOR P1 FAST OSO":118,
-  "DOOR SR SLOW OSO":61,
-  "DOOR SR FAST OSO":114,
-  "DOOR S1 SLOW OSO":103,
-  "DOOR S1 FAST OSO":112,
-  "DOOR WR SLOW OSO":86,
-  "DOOR WR FAST OSO":106,
-  "DOOR W1 SLOW OSO":2,
-  "DOOR W1 FAST OSO":109,
-  "DOOR GR FAST OSO":46,
-  "DOOR SR SLOW CSC":42,
-  "DOOR SR FAST CSC":116,
-  "DOOR S1 SLOW CSC":50,
-  "DOOR S1 FAST CSC":113,
-  "DOOR WR SLOW CSC":75,
-  "DOOR WR FAST CSC":107,
-  "DOOR W1 SLOW CSC":3,
-  "DOOR W1 FAST CSC":110,
-  "DOOR SR SLOW CWO 30SEC":196,
-  "DOOR S1 SLOW CWO 30SEC":175,
-  "DOOR WR SLOW CWO 30SEC":76,
-  "DOOR W1 SLOW CWO 30SEC":16,
-  "DOOR PR SLOW OWC 4SEC BLU":26,
-  "DOOR PR SLOW OWC 4SEC RED":28,
-  "DOOR PR SLOW OWC 4SEC YEL":27,
-  "DOOR P1 SLOW OSO BLU":32,
-  "DOOR P1 SLOW OSO RED":33,
-  "DOOR P1 SLOW OSO YEL":34,
-  "DOOR SR FAST OSO BLU":99,
-  "DOOR SR FAST OSO RED":134,
-  "DOOR SR FAST OSO YEL":136,
-  "DOOR S1 FAST OSO BLU":133,
-  "DOOR S1 FAST OSO RED":135,
-  "DOOR S1 FAST OSO YEL":137,
-# Floors
-  "FLOOR SR DOWN SLOW LNF":60,
-  "FLOOR S1 DOWN SLOW LNF":23,
-  "FLOOR WR DOWN SLOW LNF":82,
-  "FLOOR W1 DOWN SLOW LNF":38,
-  "FLOOR SR DOWN SLOW LNF CPYTEX+TYPE NUM":177,
-  "FLOOR S1 DOWN SLOW LNF CPYTEX+TYPE NUM":159,
-  "FLOOR WR DOWN SLOW LNF CPYTEX+TYPE NUM":84,
-  "FLOOR W1 DOWN SLOW LNF CPYTEX+TYPE NUM":37,
-  "FLOOR SR UP SLOW NNF":69,
-  "FLOOR S1 UP SLOW NNF":18,
-  "FLOOR WR UP SLOW NNF":128,
-  "FLOOR W1 UP SLOW NNF":119,
-  "FLOOR SR UP FAST NNF":132,
-  "FLOOR S1 UP FAST NNF":131,
-  "FLOOR WR UP FAST NNF":129,
-  "FLOOR W1 UP FAST NNF":130,
-  "FLOOR SR DOWN SLOW NNF":222,
-  "FLOOR S1 DOWN SLOW NNF":221,
-  "FLOOR WR DOWN SLOW NNF":220,
-  "FLOOR W1 DOWN SLOW NNF":219,
-  "FLOOR SR UP SLOW LNC":64,
-  "FLOOR S1 UP SLOW LNC":101,
-  "FLOOR WR UP SLOW LNC":91,
-  "FLOOR W1 UP SLOW LNC":5,
-  "FLOOR G1 UP SLOW LNC":24,
-  "FLOOR SR UP SLOW LNC-8 CRUSH":65,
-  "FLOOR S1 UP SLOW LNC-8 CRUSH":55,
-  "FLOOR WR UP SLOW LNC-8 CRUSH":94,
-  "FLOOR W1 UP SLOW LNC-8 CRUSH":56,
-  "FLOOR SR DOWN SLOW HNF":45,
-  "FLOOR S1 DOWN SLOW HNF":102,
-  "FLOOR WR DOWN SLOW HNF":83,
-  "FLOOR W1 DOWN SLOW HNF":19,
-  "FLOOR SR DOWN FAST HNF+8":70,
-  "FLOOR S1 DOWN FAST HNF+8":71,
-  "FLOOR WR DOWN FAST HNF+8":98,
-  "FLOOR W1 DOWN FAST HNF+8":36,
-  "FLOOR SR UP SLOW 24":180,
-  "FLOOR S1 UP SLOW 24":161,
-  "FLOOR WR UP SLOW 24":92,
-  "FLOOR W1 UP SLOW 24":58,
-  "FLOOR SR UP SLOW 24 CPYTEX+TYPE TRIG":179,
-  "FLOOR S1 UP SLOW 24 CPYTEX+TYPE TRIG":160,
-  "FLOOR WR UP SLOW 24 CPYTEX+TYPE TRIG":93,
-  "FLOOR W1 UP SLOW 24 CPYTEX+TYPE TRIG":59,
-  "FLOOR SR UP SLOW SLT":176,
-  "FLOOR S1 UP SLOW SLT":158,
-  "FLOOR WR UP SLOW SLT":96,
-  "FLOOR W1 UP SLOW SLT":30,
-  "FLOOR SR UP SLOW 512":178,
-  "FLOOR S1 UP SLOW 512":140,
-  "FLOOR WR UP SLOW 512":147,
-  "FLOOR W1 UP SLOW 512":142,
-  "FLOOR SR NOMOVE CPYTEX+TYPE SLT TRIG":190,
-  "FLOOR S1 NOMOVE CPYTEX+TYPE SLT TRIG":189,
-  "FLOOR WR NOMOVE CPYTEX+TYPE SLT TRIG":154,
-  "FLOOR W1 NOMOVE CPYTEX+TYPE SLT TRIG":153,
-  "FLOOR SR NOMOVE CPYTEX+TYPE SLT NUM":78,
-  "FLOOR S1 NOMOVE CPYTEX+TYPE SLT NUM":241,
-  "FLOOR WR NOMOVE CPYTEX+TYPE SLT NUM":240,
-  "FLOOR W1 NOMOVE CPYTEX+TYPE SLT NUM":239,
-# Ceilings
-  "CEIL SR DOWN FAST FLR":43,
-  "CEIL S1 DOWN FAST FLR":41,
-  "CEIL WR DOWN FAST FLR":152,
-  "CEIL W1 DOWN FAST FLR":145,
-  "CEIL SR UP SLOW HNC":186,
-  "CEIL S1 UP SLOW HNC":166,
-  "CEIL WR UP SLOW HNC":151,
-  "CEIL W1 UP SLOW HNC":40,
-  "CEIL SR DOWN SLOW F+8":187,
-  "CEIL S1 DOWN SLOW F+8":167,
-  "CEIL WR DOWN SLOW F+8":72,
-  "CEIL W1 DOWN SLOW F+8":44,
-  "CEIL SR DOWN SLOW LNC":205,
-  "CEIL S1 DOWN SLOW LNC":203,
-  "CEIL WR DOWN SLOW LNC":201,
-  "CEIL W1 DOWN SLOW LNC":199,
-  "CEIL SR DOWN SLOW HNF":205,
-  "CEIL S1 DOWN SLOW HNF":204,
-  "CEIL WR DOWN SLOW HNF":202,
-  "CEIL W1 DOWN SLOW HNF":200,
-# Platforms and lifts
-  "PLAT SR SLOW CPYTEX TRIG 24":66,
-  "PLAT S1 SLOW CPYTEX TRIG 24":15,
-  "PLAT WR SLOW CPYTEX TRIG 24":148,
-  "PLAT W1 SLOW CPYTEX TRIG 24":143,
-  "PLAT SR SLOW CPYTEX TRIG 32":67,
-  "PLAT S1 SLOW CPYTEX TRIG 32":14,
-  "PLAT WR SLOW CPYTEX TRIG 32":149,
-  "PLAT W1 SLOW CPYTEX TRIG 32":144,
-  "PLAT SR SLOW CPYTEX+DELTYPE TRIG NAF":68,
-  "PLAT S1 SLOW CPYTEX+DELTYPE TRIG NAF":20,
-  "PLAT WR SLOW CPYTEX+DELTYPE TRIG NAF":95,
-  "PLAT W1 SLOW CPYTEX+DELTYPE TRIG NAF":22,
-  "PLAT G1 SLOW CPYTEX+DELTYPE TRIG NAF":47,
-  "PLAT SR SLOW 3SEC PERP":181,
-  "PLAT S1 SLOW 3SEC PERP":162,
-  "PLAT WR SLOW 3SEC PERP":87,
-  "PLAT W1 SLOW 3SEC PERP":53,
-  "PLAT SR STOP":182,
-  "PLAT S1 STOP":163,
-  "PLAT WR STOP":89,
-  "PLAT W1 STOP":54,
-  "PLAT SR SLOW 3SEC LNF":62,
-  "PLAT S1 SLOW 3SEC LNF":21,
-  "PLAT WR SLOW 3SEC LNF":88,
-  "PLAT W1 SLOW 3SEC LNF":10,
-  "PLAT SR FAST 3SEC LNF":123,
-  "PLAT S1 FAST 3SEC LNF":122,
-  "PLAT WR FAST 3SEC LNF":120,
-  "PLAT W1 FAST 3SEC LNF":121,
-  "PLAT SR INST CL":211,
-  "PLAT WR INST CL":212,
-# Crushers
-  "CRUSHER SR SLOW":184,
-  "CRUSHER S1 SLOW":49,
-  "CRUSHER WR SLOW":73,
-  "CRUSHER W1 SLOW":25,
-  "CRUSHER SR FAST":183,
-  "CRUSHER S1 FAST":164,
-  "CRUSHER WR FAST":77,
-  "CRUSHER W1 FAST":6,
-  "CRUSHER SR SLOW SILENT":185,
-  "CRUSHER S1 SLOW SILENT":165,
-  "CRUSHER WR SLOW SILENT":150,
-  "CRUSHER W1 SLOW SILENT":141,
-  "CRUSHER SR STOP":188,
-  "CRUSHER S1 STOP":168,
-  "CRUSHER WR STOP":74,
-  "CRUSHER W1 STOP":57,
-# Stairs
-  "STAIR SR UP SLOW 8":258,
-  "STAIR S1 UP SLOW 8":7,
-  "STAIR WR UP SLOW 8":256,
-  "STAIR W1 UP SLOW 8":8,
-  "STAIR SR UP FAST 16":259,
-  "STAIR S1 UP FAST 16":127,
-  "STAIR WR UP FAST 16":257,
-  "STAIR W1 UP FAST 16":100,
-# Boom elevators
-  "ELEVATOR SR FAST NHF":230,
-  "ELEVATOR S1 FAST NHF":229,
-  "ELEVATOR WR FAST NHF":228,
-  "ELEVATOR W1 FAST NHF":227,
-  "ELEVATOR SR FAST NHF":234,
-  "ELEVATOR S1 FAST NLF":233,
-  "ELEVATOR WR FAST NLF":232,
-  "ELEVATOR W1 FAST NLF":231,
-  "ELEVATOR SR FAST CURRF":238,
-  "ELEVATOR S1 FAST CURRF":237,
-  "ELEVATOR WR FAST CURRF":236,
-  "ELEVATOR W1 FAST CURRF":235,
-# Lighting
-  "LIGHT SR 35":139,
-  "LIGHT S1 35":170,
-  "LIGHT WR 35":79,
-  "LIGHT W1 35":35,
-  "LIGHT SR 255":138,
-  "LIGHT S1 255":171,
-  "LIGHT WR 255":81,
-  "LIGHT W1 255":13,
-  "LIGHT SR MAXN":192,
-  "LIGHT S1 MAXN":169,
-  "LIGHT WR MAXN":80,
-  "LIGHT W1 MAXN":12,
-  "LIGHT SR MINN":194,
-  "LIGHT S1 MINN":173,
-  "LIGHT WR MINN":157,
-  "LIGHT W1 MINN":104,
-  "LIGHT SR BLINK":193,
-  "LIGHT S1 BLINK":172,
-  "LIGHT WR BLINK":156,
-  "LIGHT W1 BLINK":17,
-# Exits
-  "EXIT S1":11,
-  "EXIT W1":52,
-  "EXIT G1":197,
-  "EXIT S1 SECRET":51,
-  "EXIT W1 SECRET":124,
-  "EXIT G1 SECRET":198,
-# Teleports
-  "TELEPORT SR":195,
-  "TELEPORT S1":174,
-  "TELEPORT WR":97,
-  "TELEPORT W1":39,
-  "TELEPORT WR MONSTER":126,
-  "TELEPORT W1 MONSTER":125,
-  "TELEPORT SR MONSTER":269,
-  "TELEPORT S1 MONSTER":268,
-  "TELEPORT SR SILENT":210,
-  "TELEPORT S1 SILENT":209,
-  "TELEPORT WR SILENT":208,
-  "TELEPORT W1 SILENT":207,
-  "TELEPORT WR SILENT LINE":244,
-  "TELEPORT W1 SILENT LINE":243,
-  "TELEPORT WR SILENT LINE REVERSE":263,
-  "TELEPORT W1 SILENT LINE REVERSE":262,
-  "TELEPORT WR SILENT LINE MONSTER":267,
-  "TELEPORT W1 SILENT LINE MONSTER":266,
-  "TELEPORT WR SILENT LINE REVERSE MONSTER":265,
-  "TELEPORT W1 SILENT LINE REVERSE MONSTER":264,
-# Donuts
-  "DONUT SR":191,
-  "DONUT S1":9,
-  "DONUT WR":155,
-  "DONUT W1":146,
-# Boom property transfer
-  "TRANSFER FLIGHT":213,
-  "TRANSFER CLIGHT":261,
-  "TRANSFER TRANSLUCENCY":260,
-  "TRANSFER HEIGHTS":242,
-  "TRANSFER FRICTION":223,
-  "TRANSFER WIND":224,
-  "TRANSFER CURRENT":225,
-  "TRANSFER POINTFORCE":226,
-# Scrollers
-  "SCROLL CL":250,
-  "SCROLL FLR":251,
-  "SCROLL CARRY":252,
-  "SCROLL FLR+CARRY":253,
-  "SCROLL WALL SYNCED":254,
-  "SCROLL WALL OFFSETS":255,
-  "SCROLL WALL RIGHT":85,
-  "SCROLL WALL LEFT":48,
-  "SCROLL CL WRTSECTOR":245,
-  "SCROLL FLR WRTSECTOR":246,
-  "SCROLL CARRY WRTSECTOR":247,
-  "SCROLL F+CARRY WRTSECTOR":248,
-  "SCROLL WALL WRTSECTOR":249,
-  "SCROLL CL ACCEL":214,
-  "SCROLL FLR ACCEL":215,
-  "SCROLL CARRY ACCEL":216,
-  "SCROLL FLR+CARRY ACCEL":217,
-  "SCROLL WALL ACCEL":218
-}
-
-num2desc = {}
-for d, n in desc2num.items(): num2desc[n] = d
-del(d)
-del(n)
-
-trigcompat = \
- [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
-  1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
-  1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
-  1, 1, 1, 1, 1, 1, 1, 1, 1, 2, 1, 1, 1, 1, 1, 1, 2, 1, 1, 1, 1, 1, 1,
-  1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
-  0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
-  1, 1, 1, 1, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
-  2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
-  2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 0,
-  2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
-  0, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
-  2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2]
-
-def check_compat(num):
-    """Check the compatibility for a trigger number."""
-    if 8192 <= num < 32768:
-        return "BOOM GENERALIZED"
-    try:
-        return ["UNKNOWN", "DOOM19", "BOOM EXTENDED"][trigcompat[num]]
-    except:
-        return "UNKNOWN"
-
-def decode(n):
-    """Generate a description code for a number."""
-    d = []
-    if n < 8192:
-        if n in num2desc:
-            return num2desc[n]
-        return "UNKNOWN"
-    # Boom generalized
-    elif 0x2F80 <= n < 0x3000:
-        n -= 0x2F80
-        d += ["CRUSHER"]
-        d += [("W1","WR","S1","SR","G1","GR","P1","PR") [n&0x0007]]
-        d += [("SLOW","NORMAL","FAST","TURBO")          [(n&0x0018)>>3]]
-        d += [("MONSTER","")                            [(n&0x0020)>>5]]
-        d += [("SILENT","")                             [(n&0x00c0)>>6]]
-    elif 0x3000 <= n < 0x3400:
-        n -= 0x3000
-        d += ["STAIR"]
-        d += [("W1","WR","S1","SR","G1","GR","P1","PR") [n&0x0007]]
-        d += [("SLOW","NORMAL","FAST","TURBO")          [(n&0x0018)>>3]]
-        d += [("","MONSTER")                            [(n&0x0020)>>5]]
-        d += [("4","8","16","24")                       [(n&0x00c0)>>6]]
-        d += [("DOWN","UP")                             [(n&0x0100)>>8]]
-        d += [("", "IGNTXT")                            [(n&0x0200)>>9]]
-    elif 0x3400 <= n < 0x3800:
-        n -= 0x3400
-        d += ["PLATFORM"]
-        d += [("W1","WR","S1","SR","G1","GR","P1","PR") [n&0x0007]]
-        d += [("SLOW","NORMAL","FAST","TURBO")          [(n&0x0018)>>3]]
-        d += [("MONSTER","")                            [(n&0x0020)>>5]]
-        d += [("1","3","5","10")                        [(n&0x00c0)>>6]]
-        d += [("LNF","NNF","LNC","PERP")                [(n&0x0300)>>8]]
-    elif 0x3800 <= n < 0x3c00:
-        n -= 0x3800
-        d += ["DOOR"]
-        d += [("W1","WR","S1","SR","G1","GR","P1","PR") [n&0x0007]]
-        d += [("SLOW","NORMAL","FAST","TURBO")          [(n&0x0018)>>3]]
-        d += [("OWC","OSO")                             [(n&0x0020)>>5]]
-        d += [("ANY","RED","YELLOW","BLUE","RED",
-               "BLUE","YELLOW","ALL")                   [(n&0x01c0)>>6]]
-        d += [("3KEYS","6KEYS")                         [(n&0x0200)>>9]]
-    elif 0x3c00 <= n < 0x4000:
-        n -= 0x3c00
-        d += ["DOOR"]
-        d += [("W1","WR","S1","SR","G1","GR","P1","PR") [n&0x0007]]
-        d += [("SLOW","NORMAL","FAST","TURBO")          [(n&0x0018)>>3]]
-        d += [("OWC","OSO","CWO","CSC")                 [(n&0x0060)>>5]]
-        d += [("MONSTER","")                            [(n&0x0080)>>7]]
-        d += [("1SECS","4SECS","9SECS","30SECS")        [(n&0x0300)>>8]]
-    elif 0x4000 <= n < 0x6000:
-        n -= 0x4000
-        d += ["CEIL"]
-        d += [("W1","WR","S1","SR","G1","GR","P1","PR") [n&0x0007]]
-        d += [("SLOW","NORMAL","FAST","TURBO")          [(n&0x0018)>>3]]
-        d += [("TRIG","NUM")                            [(n&0x0020)>>5]]
-        d += [("DOWN","UP")                             [(n&0x0040)>>6]]
-        d += [("HNC","LNC","NNC","HNF","FLR",
-               "SUT","24","32")                         [(n&0x0380)>>7]]
-        d += [("","CPYTEX+DELTYPE","CPYTEX","CHGTYPE")  [(n&0x0c00)>>10]]
-        d += [("CRUSH","")                              [(n&0x1000)>>12]]
-    elif 0x6000 <= n < 0x8000:
-        n -= 0x6000
-        d += ["FLOOR"]
-        d += [("W1","WR","S1","SR","G1","GR","P1","PR") [n&0x0007]]
-        d += [("SLOW","NORMAL","FAST","TURBO")          [(n&0x0018)>>3]]
-        d += [("TRIG","NUM")                            [(n&0x0020)>>5]]
-        d += [("DOWN","UP")                             [(n&0x0040)>>6]]
-        d += [("HNF","LNF","NNF","LNC","CL",
-               "SLT","24","32")                         [(n&0x0380)>>7]]
-        d += [("","CPYTEX+DELTYPE","CPYTEX","CHGTYPE")  [(n&0x0c00)>>10]]
-        d += [("CRUSH","")                              [(n&0x1000)>>12]]
-    # Bit of a hack, but works
-    return (" ".join(d)).replace("  "," ").rstrip(" ")
-
-def encode_std(desc):
-    """Encode an exact description of a trigger into its corresponding number.
-    For inexact descriptions, use find_std."""
-    try:
-        return desc2num[desc.upper()]
-    except:
-        raise Exception("Description not recognized")
-
-def encode_gen(desc):
-    """Encode a generalized (Boom) trigger description to a trigger
-    number. Invalid or incompatible terms get converted to the default
-    value."""
-    desc = desc.upper()
-    num = 0
-    def pk(seq, shift):
-        for i in range(len(seq)):
-            if seq[i] in desc:
-                return i << shift
-        return 0
-    num |= pk(("W1","WR","S1","SR","G1","GR","P1","PR"), 0)
-    num |= pk(("SLOW","NORMAL","FAST","TURBO"), 3)
-    if ("FLOOR" in desc) or ("CEIL" in desc):
-        num |= pk(("TRIG","NUM"), 5)
-        num |= pk(("DOWN","UP"), 6)
-        num |= pk(("xx","CPYTEX+DELTYPE","CPYTEX","CHGTYPE"), 10)
-        num |= pk(("CRUSH",), 12)
-        if "FLOOR" in desc:
-            num |= pk(("HNF","LNF","NNF","LNC","CL","SLT","24","32"), 7)
-            num += 0x6000
-        else:
-            num |= pk(("HNC","LNC","NNC","HNF","FLR","SUT","24","32"), 7)
-            num += 0x4000
-    elif "CRUSHER" in desc:
-        num |= pk(("MONSTER",), 5)
-        num |= pk(("SILENT",), 6)
-        num += 0x2F80
-    elif "STAIR" in desc:
-        num |= pk(("xx","MONSTER"), 5)
-        num |= pk(("4","8","16","24"), 6)
-        num |= pk(("DOWN","UP"), 8)
-        num |= pk(("xx","IGNTXT"), 9)
-        num += 0x3000
-    elif "PLATFORM" in desc:
-        num |= pk(("MONSTER",), 5)
-        num |= pk(("1","3","5","10"), 6)
-        num |= pk(("LNF","NNF","LNC","PERP"), 8)
-        num += 0x3400
-    elif "DOOR" in desc:
-        num |= pk(("SLOW","NORMAL","FAST","TURBO"), 3)
-        if ("BLU" in desc) or ("YEL" in desc) or ("RED" in desc) or\
-           ("ALL" in desc) or ("ANY" in desc):
-            num |= pk(("OWC","OSO"), 5)
-            num |= pk(("ANY","RED","YELLOW","BLUE","RED","BLUE","YELLOW","ALL"), 6)
-            num |= pk(("3KEYS","6KEYS"), 9)
-            num += 0x3800
-        else:
-            num |= pk(("OWC","OSO","CWO","CSC"), 5)
-            num |= pk(("MONSTER",), 7)
-            num |= pk(("1SECS","4SECS","9SECS","30SECS"), 8)
-            num += 0x3c00
-    else:
-        raise LookupError("Insufficient information provided")
-    return num
-
-def find_std(desc):
-    """Search the standard (non-generalized) triggers. A list of
-    matches is returned. All terms must match. Wildcards are allowed.
-    Example:
-
-       find_std("CEIL UP S?")        should return:
-
-       ['CEIL S1 UP SLOW HNC', 'CEIL SR UP SLOW HNC']"""
-    desc = desc.upper()
-    terms = desc.split()
-    matches = []
-    for dsc in num2desc.values():
-        d = dsc.split()
-        matchedterms = 0
-        for term in terms:
-            for key in d:
-                if fnmatchcase(key, term):
-                    matchedterms += 1
-        if matchedterms == len(terms):
-            matches.append(dsc)
-    return matches
-
-__all__ = [find_std, encode_std, encode_gen, decode, check_compat]
+"""
+lineinfo.py -- dealing with Doom linedef trigger types.
+Provides functions to create a human-readable description
+code from a trigger number, and the inverse operation.
+
+Guide to Trigger Description Codes (R):
+
+Example:        "FLOOR SR UP SLOW CRUSH LNC-8"
+
+Categories:
+    DOOR       - Doors (regular and locked)
+    FLOOR      - Floor movers
+    CEIL       - Ceiling movers
+    PLAT       - Platforms and lifts
+    CRUSHER    - Crushers
+    STAIR      - Stair builders
+    ELEVATOR   - Boom elevators
+    LIGHT      - Light changers
+    EXIT       - Exits
+    TELEPORT   - Teleports
+    DONUT      - Donuts (lower pillar, raise surrounding sector)
+    TRANSFER   - Transfer properties (Boom)
+    SCROLL     - Scroll lines and sectors (Boom)
+
+Trigger types:
+    P1 - Push(door) trigger, works once
+    PR - Push(door) trigger, works repeatedly
+    S1 - Switch, works once
+    SR - Switch, works repeatedly
+    W1 - Walk across, works once
+    WR - Walk across, works repeatedly
+    G1 - Shoot, works once
+    GR - Shoot, works repeatedly
+
+Door locks:
+    YEL - Yellow key lock
+    RED - Red key lock
+    BLU - Blue key lock
+
+Door types:
+    OWC - Open, Wait, Close
+    CWO - Close, Wait, Open
+    OSO - Open, Stay Open
+    CSC - Close, Stay Closed
+
+Motion speed
+    SLOW - Slow
+    NORM - Normal
+    FAST - Fast
+    TURB - Turbo
+    INST - Instant
+
+Delay times
+    3SEC  - 3 seconds
+    4SEC  - 4 seconds
+    30SEC - 30 seconds
+
+Sector property changers:
+    CPYTEX           - Copy Texture
+    CPYTEX+DELTYPE   - Copy Texture, Reset type
+    CPYTEX+TYPE      - Copy Texture and Type
+
+Directions:
+    DOWN    - Down
+    UP      - Up
+    NOMOVE  - Stay (only change properties)
+
+Miscellaneous:
+    SECRET   - A secret exit
+    MONSTER  - Monsters can activate the trigger
+    LINE     - Line teleporters
+    REVERSE  - Line teleporter, reversed
+    SILENT   - Make crushers or teleporters silent
+    CRUSH    - Enable crushing (for CEILs and FLOORs,
+               not to be confused with CRUSHERs)
+
+Destinations/platforms:
+    LNF   - Lowest Neighbor Floor
+    LNC   - Lowest Neighbor Ceiling
+    HNF   - Highest Neighbor Floor
+    HNC   - Highest Neighbor Ceiling
+    NNF   - Next Neighbor Floor
+    NNC   - Next Neighbor Ceiling
+    HNF+8 - 8 above Highest neighbor Floor
+    LNC+8 - 8 under Lowest neighbor Ceiling
+    F+8   - 8 above floor
+    8     - 8 units Absolute  (STAIRs only)
+    16    - 16 units Absolute (STAIRs only)
+    24    - 24 units Absolute
+    32    - 32 units Absolute
+    512   - 512 units absolute
+    SLT   - Shortest Lower Texture
+    SUT   - Shortest Upper Texture
+    NLF   - Next Lowest neighbor Floor
+    NLC   - Next Lowest neighbor Ceiling
+    NHF   - Next Highest neighbor Floor
+    CURRF - Current Floor (ELEVATORs)
+    FLR   - Floor
+    CL    - Ceiling
+    NAF   - Next adjacent floor
+    PERP  - Perpetual
+    STOP  - Stop ongoing motion
+
+Models:
+    TRIG  - Use trigger sector as model
+    NUM   - Lookup adjacent model numerically
+
+Lighting:
+    35    - 35 units
+    255   - 255 units
+    MAXN  - Maximum Neighbor
+    MINN  - Minimum Neighbor
+    BLINK - Blinking
+
+Transfers (check boomref.txt for more info):
+    FLIGHT       - Transfer floor light level
+    CLIGHT       - Transfer ceiling light level
+    TRANSLUCENCY - Transfer line translucency
+    HEIGHTS      - The famous 242!
+    FRICTION     - Transfer friction
+    WIND         - Transfer current
+    POINTFORCE   - Transfer force point (?)
+
+Scrollers (check boomref.txt for more info):
+    CARRY       - Carry objects (conveyor)
+    WRTSECTOR   - With respect to 1st side's sector
+    ACCEL       - Accelerate scrolling
+    RIGHT       - Right direction
+    LEFT        - Left direction
+    WALL        - Scroll wall
+    SYNCED      - Sync scrolling to sector
+    OFFSETS     - Scroll by offsets
+"""
+
+from fnmatch import fnmatchcase
+
+# Define description codes for the standard triggers
+desc2num = \
+{
+  "": 0,
+  "NO ACTION":0,
+# Doors
+  "DOOR PR SLOW OWC 4SEC MONSTER":1,
+  "DOOR PR FAST OWC 4SEC":117,
+  "DOOR SR SLOW OWC 4SEC":63,
+  "DOOR SR FAST OWC 4SEC":114,
+  "DOOR S1 SLOW OWC 4SEC":29,
+  "DOOR S1 FAST OWC 4SEC":111,
+  "DOOR WR SLOW OWC 4SEC":90,
+  "DOOR WR FAST OWC 4SEC":105,
+  "DOOR W1 SLOW OWC 4SEC":4,
+  "DOOR W1 FAST OWC 4SEC":108,
+  "DOOR P1 SLOW OSO":31,
+  "DOOR P1 FAST OSO":118,
+  "DOOR SR SLOW OSO":61,
+  "DOOR SR FAST OSO":114,
+  "DOOR S1 SLOW OSO":103,
+  "DOOR S1 FAST OSO":112,
+  "DOOR WR SLOW OSO":86,
+  "DOOR WR FAST OSO":106,
+  "DOOR W1 SLOW OSO":2,
+  "DOOR W1 FAST OSO":109,
+  "DOOR GR FAST OSO":46,
+  "DOOR SR SLOW CSC":42,
+  "DOOR SR FAST CSC":116,
+  "DOOR S1 SLOW CSC":50,
+  "DOOR S1 FAST CSC":113,
+  "DOOR WR SLOW CSC":75,
+  "DOOR WR FAST CSC":107,
+  "DOOR W1 SLOW CSC":3,
+  "DOOR W1 FAST CSC":110,
+  "DOOR SR SLOW CWO 30SEC":196,
+  "DOOR S1 SLOW CWO 30SEC":175,
+  "DOOR WR SLOW CWO 30SEC":76,
+  "DOOR W1 SLOW CWO 30SEC":16,
+  "DOOR PR SLOW OWC 4SEC BLU":26,
+  "DOOR PR SLOW OWC 4SEC RED":28,
+  "DOOR PR SLOW OWC 4SEC YEL":27,
+  "DOOR P1 SLOW OSO BLU":32,
+  "DOOR P1 SLOW OSO RED":33,
+  "DOOR P1 SLOW OSO YEL":34,
+  "DOOR SR FAST OSO BLU":99,
+  "DOOR SR FAST OSO RED":134,
+  "DOOR SR FAST OSO YEL":136,
+  "DOOR S1 FAST OSO BLU":133,
+  "DOOR S1 FAST OSO RED":135,
+  "DOOR S1 FAST OSO YEL":137,
+# Floors
+  "FLOOR SR DOWN SLOW LNF":60,
+  "FLOOR S1 DOWN SLOW LNF":23,
+  "FLOOR WR DOWN SLOW LNF":82,
+  "FLOOR W1 DOWN SLOW LNF":38,
+  "FLOOR SR DOWN SLOW LNF CPYTEX+TYPE NUM":177,
+  "FLOOR S1 DOWN SLOW LNF CPYTEX+TYPE NUM":159,
+  "FLOOR WR DOWN SLOW LNF CPYTEX+TYPE NUM":84,
+  "FLOOR W1 DOWN SLOW LNF CPYTEX+TYPE NUM":37,
+  "FLOOR SR UP SLOW NNF":69,
+  "FLOOR S1 UP SLOW NNF":18,
+  "FLOOR WR UP SLOW NNF":128,
+  "FLOOR W1 UP SLOW NNF":119,
+  "FLOOR SR UP FAST NNF":132,
+  "FLOOR S1 UP FAST NNF":131,
+  "FLOOR WR UP FAST NNF":129,
+  "FLOOR W1 UP FAST NNF":130,
+  "FLOOR SR DOWN SLOW NNF":222,
+  "FLOOR S1 DOWN SLOW NNF":221,
+  "FLOOR WR DOWN SLOW NNF":220,
+  "FLOOR W1 DOWN SLOW NNF":219,
+  "FLOOR SR UP SLOW LNC":64,
+  "FLOOR S1 UP SLOW LNC":101,
+  "FLOOR WR UP SLOW LNC":91,
+  "FLOOR W1 UP SLOW LNC":5,
+  "FLOOR G1 UP SLOW LNC":24,
+  "FLOOR SR UP SLOW LNC-8 CRUSH":65,
+  "FLOOR S1 UP SLOW LNC-8 CRUSH":55,
+  "FLOOR WR UP SLOW LNC-8 CRUSH":94,
+  "FLOOR W1 UP SLOW LNC-8 CRUSH":56,
+  "FLOOR SR DOWN SLOW HNF":45,
+  "FLOOR S1 DOWN SLOW HNF":102,
+  "FLOOR WR DOWN SLOW HNF":83,
+  "FLOOR W1 DOWN SLOW HNF":19,
+  "FLOOR SR DOWN FAST HNF+8":70,
+  "FLOOR S1 DOWN FAST HNF+8":71,
+  "FLOOR WR DOWN FAST HNF+8":98,
+  "FLOOR W1 DOWN FAST HNF+8":36,
+  "FLOOR SR UP SLOW 24":180,
+  "FLOOR S1 UP SLOW 24":161,
+  "FLOOR WR UP SLOW 24":92,
+  "FLOOR W1 UP SLOW 24":58,
+  "FLOOR SR UP SLOW 24 CPYTEX+TYPE TRIG":179,
+  "FLOOR S1 UP SLOW 24 CPYTEX+TYPE TRIG":160,
+  "FLOOR WR UP SLOW 24 CPYTEX+TYPE TRIG":93,
+  "FLOOR W1 UP SLOW 24 CPYTEX+TYPE TRIG":59,
+  "FLOOR SR UP SLOW SLT":176,
+  "FLOOR S1 UP SLOW SLT":158,
+  "FLOOR WR UP SLOW SLT":96,
+  "FLOOR W1 UP SLOW SLT":30,
+  "FLOOR SR UP SLOW 512":178,
+  "FLOOR S1 UP SLOW 512":140,
+  "FLOOR WR UP SLOW 512":147,
+  "FLOOR W1 UP SLOW 512":142,
+  "FLOOR SR NOMOVE CPYTEX+TYPE SLT TRIG":190,
+  "FLOOR S1 NOMOVE CPYTEX+TYPE SLT TRIG":189,
+  "FLOOR WR NOMOVE CPYTEX+TYPE SLT TRIG":154,
+  "FLOOR W1 NOMOVE CPYTEX+TYPE SLT TRIG":153,
+  "FLOOR SR NOMOVE CPYTEX+TYPE SLT NUM":78,
+  "FLOOR S1 NOMOVE CPYTEX+TYPE SLT NUM":241,
+  "FLOOR WR NOMOVE CPYTEX+TYPE SLT NUM":240,
+  "FLOOR W1 NOMOVE CPYTEX+TYPE SLT NUM":239,
+# Ceilings
+  "CEIL SR DOWN FAST FLR":43,
+  "CEIL S1 DOWN FAST FLR":41,
+  "CEIL WR DOWN FAST FLR":152,
+  "CEIL W1 DOWN FAST FLR":145,
+  "CEIL SR UP SLOW HNC":186,
+  "CEIL S1 UP SLOW HNC":166,
+  "CEIL WR UP SLOW HNC":151,
+  "CEIL W1 UP SLOW HNC":40,
+  "CEIL SR DOWN SLOW F+8":187,
+  "CEIL S1 DOWN SLOW F+8":167,
+  "CEIL WR DOWN SLOW F+8":72,
+  "CEIL W1 DOWN SLOW F+8":44,
+  "CEIL SR DOWN SLOW LNC":205,
+  "CEIL S1 DOWN SLOW LNC":203,
+  "CEIL WR DOWN SLOW LNC":201,
+  "CEIL W1 DOWN SLOW LNC":199,
+  "CEIL SR DOWN SLOW HNF":205,
+  "CEIL S1 DOWN SLOW HNF":204,
+  "CEIL WR DOWN SLOW HNF":202,
+  "CEIL W1 DOWN SLOW HNF":200,
+# Platforms and lifts
+  "PLAT SR SLOW CPYTEX TRIG 24":66,
+  "PLAT S1 SLOW CPYTEX TRIG 24":15,
+  "PLAT WR SLOW CPYTEX TRIG 24":148,
+  "PLAT W1 SLOW CPYTEX TRIG 24":143,
+  "PLAT SR SLOW CPYTEX TRIG 32":67,
+  "PLAT S1 SLOW CPYTEX TRIG 32":14,
+  "PLAT WR SLOW CPYTEX TRIG 32":149,
+  "PLAT W1 SLOW CPYTEX TRIG 32":144,
+  "PLAT SR SLOW CPYTEX+DELTYPE TRIG NAF":68,
+  "PLAT S1 SLOW CPYTEX+DELTYPE TRIG NAF":20,
+  "PLAT WR SLOW CPYTEX+DELTYPE TRIG NAF":95,
+  "PLAT W1 SLOW CPYTEX+DELTYPE TRIG NAF":22,
+  "PLAT G1 SLOW CPYTEX+DELTYPE TRIG NAF":47,
+  "PLAT SR SLOW 3SEC PERP":181,
+  "PLAT S1 SLOW 3SEC PERP":162,
+  "PLAT WR SLOW 3SEC PERP":87,
+  "PLAT W1 SLOW 3SEC PERP":53,
+  "PLAT SR STOP":182,
+  "PLAT S1 STOP":163,
+  "PLAT WR STOP":89,
+  "PLAT W1 STOP":54,
+  "PLAT SR SLOW 3SEC LNF":62,
+  "PLAT S1 SLOW 3SEC LNF":21,
+  "PLAT WR SLOW 3SEC LNF":88,
+  "PLAT W1 SLOW 3SEC LNF":10,
+  "PLAT SR FAST 3SEC LNF":123,
+  "PLAT S1 FAST 3SEC LNF":122,
+  "PLAT WR FAST 3SEC LNF":120,
+  "PLAT W1 FAST 3SEC LNF":121,
+  "PLAT SR INST CL":211,
+  "PLAT WR INST CL":212,
+# Crushers
+  "CRUSHER SR SLOW":184,
+  "CRUSHER S1 SLOW":49,
+  "CRUSHER WR SLOW":73,
+  "CRUSHER W1 SLOW":25,
+  "CRUSHER SR FAST":183,
+  "CRUSHER S1 FAST":164,
+  "CRUSHER WR FAST":77,
+  "CRUSHER W1 FAST":6,
+  "CRUSHER SR SLOW SILENT":185,
+  "CRUSHER S1 SLOW SILENT":165,
+  "CRUSHER WR SLOW SILENT":150,
+  "CRUSHER W1 SLOW SILENT":141,
+  "CRUSHER SR STOP":188,
+  "CRUSHER S1 STOP":168,
+  "CRUSHER WR STOP":74,
+  "CRUSHER W1 STOP":57,
+# Stairs
+  "STAIR SR UP SLOW 8":258,
+  "STAIR S1 UP SLOW 8":7,
+  "STAIR WR UP SLOW 8":256,
+  "STAIR W1 UP SLOW 8":8,
+  "STAIR SR UP FAST 16":259,
+  "STAIR S1 UP FAST 16":127,
+  "STAIR WR UP FAST 16":257,
+  "STAIR W1 UP FAST 16":100,
+# Boom elevators
+  "ELEVATOR SR FAST NHF":230,
+  "ELEVATOR S1 FAST NHF":229,
+  "ELEVATOR WR FAST NHF":228,
+  "ELEVATOR W1 FAST NHF":227,
+  "ELEVATOR SR FAST NHF":234,
+  "ELEVATOR S1 FAST NLF":233,
+  "ELEVATOR WR FAST NLF":232,
+  "ELEVATOR W1 FAST NLF":231,
+  "ELEVATOR SR FAST CURRF":238,
+  "ELEVATOR S1 FAST CURRF":237,
+  "ELEVATOR WR FAST CURRF":236,
+  "ELEVATOR W1 FAST CURRF":235,
+# Lighting
+  "LIGHT SR 35":139,
+  "LIGHT S1 35":170,
+  "LIGHT WR 35":79,
+  "LIGHT W1 35":35,
+  "LIGHT SR 255":138,
+  "LIGHT S1 255":171,
+  "LIGHT WR 255":81,
+  "LIGHT W1 255":13,
+  "LIGHT SR MAXN":192,
+  "LIGHT S1 MAXN":169,
+  "LIGHT WR MAXN":80,
+  "LIGHT W1 MAXN":12,
+  "LIGHT SR MINN":194,
+  "LIGHT S1 MINN":173,
+  "LIGHT WR MINN":157,
+  "LIGHT W1 MINN":104,
+  "LIGHT SR BLINK":193,
+  "LIGHT S1 BLINK":172,
+  "LIGHT WR BLINK":156,
+  "LIGHT W1 BLINK":17,
+# Exits
+  "EXIT S1":11,
+  "EXIT W1":52,
+  "EXIT G1":197,
+  "EXIT S1 SECRET":51,
+  "EXIT W1 SECRET":124,
+  "EXIT G1 SECRET":198,
+# Teleports
+  "TELEPORT SR":195,
+  "TELEPORT S1":174,
+  "TELEPORT WR":97,
+  "TELEPORT W1":39,
+  "TELEPORT WR MONSTER":126,
+  "TELEPORT W1 MONSTER":125,
+  "TELEPORT SR MONSTER":269,
+  "TELEPORT S1 MONSTER":268,
+  "TELEPORT SR SILENT":210,
+  "TELEPORT S1 SILENT":209,
+  "TELEPORT WR SILENT":208,
+  "TELEPORT W1 SILENT":207,
+  "TELEPORT WR SILENT LINE":244,
+  "TELEPORT W1 SILENT LINE":243,
+  "TELEPORT WR SILENT LINE REVERSE":263,
+  "TELEPORT W1 SILENT LINE REVERSE":262,
+  "TELEPORT WR SILENT LINE MONSTER":267,
+  "TELEPORT W1 SILENT LINE MONSTER":266,
+  "TELEPORT WR SILENT LINE REVERSE MONSTER":265,
+  "TELEPORT W1 SILENT LINE REVERSE MONSTER":264,
+# Donuts
+  "DONUT SR":191,
+  "DONUT S1":9,
+  "DONUT WR":155,
+  "DONUT W1":146,
+# Boom property transfer
+  "TRANSFER FLIGHT":213,
+  "TRANSFER CLIGHT":261,
+  "TRANSFER TRANSLUCENCY":260,
+  "TRANSFER HEIGHTS":242,
+  "TRANSFER FRICTION":223,
+  "TRANSFER WIND":224,
+  "TRANSFER CURRENT":225,
+  "TRANSFER POINTFORCE":226,
+# Scrollers
+  "SCROLL CL":250,
+  "SCROLL FLR":251,
+  "SCROLL CARRY":252,
+  "SCROLL FLR+CARRY":253,
+  "SCROLL WALL SYNCED":254,
+  "SCROLL WALL OFFSETS":255,
+  "SCROLL WALL RIGHT":85,
+  "SCROLL WALL LEFT":48,
+  "SCROLL CL WRTSECTOR":245,
+  "SCROLL FLR WRTSECTOR":246,
+  "SCROLL CARRY WRTSECTOR":247,
+  "SCROLL F+CARRY WRTSECTOR":248,
+  "SCROLL WALL WRTSECTOR":249,
+  "SCROLL CL ACCEL":214,
+  "SCROLL FLR ACCEL":215,
+  "SCROLL CARRY ACCEL":216,
+  "SCROLL FLR+CARRY ACCEL":217,
+  "SCROLL WALL ACCEL":218
+}
+
+num2desc = {}
+for d, n in desc2num.items(): num2desc[n] = d
+del(d)
+del(n)
+
+trigcompat = \
+ [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+  1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+  1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+  1, 1, 1, 1, 1, 1, 1, 1, 1, 2, 1, 1, 1, 1, 1, 1, 2, 1, 1, 1, 1, 1, 1,
+  1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+  0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+  1, 1, 1, 1, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
+  2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
+  2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 0,
+  2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
+  0, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
+  2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2]
+
+def check_compat(num):
+    """Check the compatibility for a trigger number."""
+    if 8192 <= num < 32768:
+        return "BOOM GENERALIZED"
+    try:
+        return ["UNKNOWN", "DOOM19", "BOOM EXTENDED"][trigcompat[num]]
+    except:
+        return "UNKNOWN"
+
+def decode(n):
+    """Generate a description code for a number."""
+    d = []
+    if n < 8192:
+        if n in num2desc:
+            return num2desc[n]
+        return "UNKNOWN"
+    # Boom generalized
+    elif 0x2F80 <= n < 0x3000:
+        n -= 0x2F80
+        d += ["CRUSHER"]
+        d += [("W1","WR","S1","SR","G1","GR","P1","PR") [n&0x0007]]
+        d += [("SLOW","NORMAL","FAST","TURBO")          [(n&0x0018)>>3]]
+        d += [("MONSTER","")                            [(n&0x0020)>>5]]
+        d += [("SILENT","")                             [(n&0x00c0)>>6]]
+    elif 0x3000 <= n < 0x3400:
+        n -= 0x3000
+        d += ["STAIR"]
+        d += [("W1","WR","S1","SR","G1","GR","P1","PR") [n&0x0007]]
+        d += [("SLOW","NORMAL","FAST","TURBO")          [(n&0x0018)>>3]]
+        d += [("","MONSTER")                            [(n&0x0020)>>5]]
+        d += [("4","8","16","24")                       [(n&0x00c0)>>6]]
+        d += [("DOWN","UP")                             [(n&0x0100)>>8]]
+        d += [("", "IGNTXT")                            [(n&0x0200)>>9]]
+    elif 0x3400 <= n < 0x3800:
+        n -= 0x3400
+        d += ["PLATFORM"]
+        d += [("W1","WR","S1","SR","G1","GR","P1","PR") [n&0x0007]]
+        d += [("SLOW","NORMAL","FAST","TURBO")          [(n&0x0018)>>3]]
+        d += [("MONSTER","")                            [(n&0x0020)>>5]]
+        d += [("1","3","5","10")                        [(n&0x00c0)>>6]]
+        d += [("LNF","NNF","LNC","PERP")                [(n&0x0300)>>8]]
+    elif 0x3800 <= n < 0x3c00:
+        n -= 0x3800
+        d += ["DOOR"]
+        d += [("W1","WR","S1","SR","G1","GR","P1","PR") [n&0x0007]]
+        d += [("SLOW","NORMAL","FAST","TURBO")          [(n&0x0018)>>3]]
+        d += [("OWC","OSO")                             [(n&0x0020)>>5]]
+        d += [("ANY","RED","YELLOW","BLUE","RED",
+               "BLUE","YELLOW","ALL")                   [(n&0x01c0)>>6]]
+        d += [("3KEYS","6KEYS")                         [(n&0x0200)>>9]]
+    elif 0x3c00 <= n < 0x4000:
+        n -= 0x3c00
+        d += ["DOOR"]
+        d += [("W1","WR","S1","SR","G1","GR","P1","PR") [n&0x0007]]
+        d += [("SLOW","NORMAL","FAST","TURBO")          [(n&0x0018)>>3]]
+        d += [("OWC","OSO","CWO","CSC")                 [(n&0x0060)>>5]]
+        d += [("MONSTER","")                            [(n&0x0080)>>7]]
+        d += [("1SECS","4SECS","9SECS","30SECS")        [(n&0x0300)>>8]]
+    elif 0x4000 <= n < 0x6000:
+        n -= 0x4000
+        d += ["CEIL"]
+        d += [("W1","WR","S1","SR","G1","GR","P1","PR") [n&0x0007]]
+        d += [("SLOW","NORMAL","FAST","TURBO")          [(n&0x0018)>>3]]
+        d += [("TRIG","NUM")                            [(n&0x0020)>>5]]
+        d += [("DOWN","UP")                             [(n&0x0040)>>6]]
+        d += [("HNC","LNC","NNC","HNF","FLR",
+               "SUT","24","32")                         [(n&0x0380)>>7]]
+        d += [("","CPYTEX+DELTYPE","CPYTEX","CHGTYPE")  [(n&0x0c00)>>10]]
+        d += [("CRUSH","")                              [(n&0x1000)>>12]]
+    elif 0x6000 <= n < 0x8000:
+        n -= 0x6000
+        d += ["FLOOR"]
+        d += [("W1","WR","S1","SR","G1","GR","P1","PR") [n&0x0007]]
+        d += [("SLOW","NORMAL","FAST","TURBO")          [(n&0x0018)>>3]]
+        d += [("TRIG","NUM")                            [(n&0x0020)>>5]]
+        d += [("DOWN","UP")                             [(n&0x0040)>>6]]
+        d += [("HNF","LNF","NNF","LNC","CL",
+               "SLT","24","32")                         [(n&0x0380)>>7]]
+        d += [("","CPYTEX+DELTYPE","CPYTEX","CHGTYPE")  [(n&0x0c00)>>10]]
+        d += [("CRUSH","")                              [(n&0x1000)>>12]]
+    # Bit of a hack, but works
+    return (" ".join(d)).replace("  "," ").rstrip(" ")
+
+def encode_std(desc):
+    """Encode an exact description of a trigger into its corresponding number.
+    For inexact descriptions, use find_std."""
+    try:
+        return desc2num[desc.upper()]
+    except:
+        raise Exception("Description not recognized")
+
+def encode_gen(desc):
+    """Encode a generalized (Boom) trigger description to a trigger
+    number. Invalid or incompatible terms get converted to the default
+    value."""
+    desc = desc.upper()
+    num = 0
+    def pk(seq, shift):
+        for i in range(len(seq)):
+            if seq[i] in desc:
+                return i << shift
+        return 0
+    num |= pk(("W1","WR","S1","SR","G1","GR","P1","PR"), 0)
+    num |= pk(("SLOW","NORMAL","FAST","TURBO"), 3)
+    if ("FLOOR" in desc) or ("CEIL" in desc):
+        num |= pk(("TRIG","NUM"), 5)
+        num |= pk(("DOWN","UP"), 6)
+        num |= pk(("xx","CPYTEX+DELTYPE","CPYTEX","CHGTYPE"), 10)
+        num |= pk(("CRUSH",), 12)
+        if "FLOOR" in desc:
+            num |= pk(("HNF","LNF","NNF","LNC","CL","SLT","24","32"), 7)
+            num += 0x6000
+        else:
+            num |= pk(("HNC","LNC","NNC","HNF","FLR","SUT","24","32"), 7)
+            num += 0x4000
+    elif "CRUSHER" in desc:
+        num |= pk(("MONSTER",), 5)
+        num |= pk(("SILENT",), 6)
+        num += 0x2F80
+    elif "STAIR" in desc:
+        num |= pk(("xx","MONSTER"), 5)
+        num |= pk(("4","8","16","24"), 6)
+        num |= pk(("DOWN","UP"), 8)
+        num |= pk(("xx","IGNTXT"), 9)
+        num += 0x3000
+    elif "PLATFORM" in desc:
+        num |= pk(("MONSTER",), 5)
+        num |= pk(("1","3","5","10"), 6)
+        num |= pk(("LNF","NNF","LNC","PERP"), 8)
+        num += 0x3400
+    elif "DOOR" in desc:
+        num |= pk(("SLOW","NORMAL","FAST","TURBO"), 3)
+        if ("BLU" in desc) or ("YEL" in desc) or ("RED" in desc) or\
+           ("ALL" in desc) or ("ANY" in desc):
+            num |= pk(("OWC","OSO"), 5)
+            num |= pk(("ANY","RED","YELLOW","BLUE","RED","BLUE","YELLOW","ALL"), 6)
+            num |= pk(("3KEYS","6KEYS"), 9)
+            num += 0x3800
+        else:
+            num |= pk(("OWC","OSO","CWO","CSC"), 5)
+            num |= pk(("MONSTER",), 7)
+            num |= pk(("1SECS","4SECS","9SECS","30SECS"), 8)
+            num += 0x3c00
+    else:
+        raise LookupError("Insufficient information provided")
+    return num
+
+def find_std(desc):
+    """Search the standard (non-generalized) triggers. A list of
+    matches is returned. All terms must match. Wildcards are allowed.
+    Example:
+
+       find_std("CEIL UP S?")        should return:
+
+       ['CEIL S1 UP SLOW HNC', 'CEIL SR UP SLOW HNC']"""
+    desc = desc.upper()
+    terms = desc.split()
+    matches = []
+    for dsc in num2desc.values():
+        d = dsc.split()
+        matchedterms = 0
+        for term in terms:
+            for key in d:
+                if fnmatchcase(key, term):
+                    matchedterms += 1
+        if matchedterms == len(terms):
+            matches.append(dsc)
+    return matches
+
+__all__ = [find_std, encode_std, encode_gen, decode, check_compat]
```

### Comparing `omgifol-0.5.0/omg/mapedit.py` & `omgifol-0.5.1/omg/mapedit.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,505 +1,505 @@
-from omg.util import *
-from omg.lump import *
-from omg.wad import NameGroup
-
-import omg.lineinfo as lineinfo
-import omg.thinginfo as thinginfo
-
-class Vertex(WADStruct):
-    """Represents a map vertex."""
-    _fields_ = [
-        ("x", ctypes.c_int16),
-        ("y", ctypes.c_int16)
-    ]
-
-class GLVertex(WADStruct):
-    """Represents a map GL vertex."""
-    _fields_ = [
-        ("x", ctypes.c_int32),
-        ("y", ctypes.c_int32)
-    ]
-
-class Sidedef(WADStruct):
-    """Represents a map sidedef."""
-    _fields_ = [
-        ("off_x",  ctypes.c_int16),
-        ("off_y",  ctypes.c_int16),
-        ("tx_up",  ctypes.c_char * 8),
-        ("tx_low", ctypes.c_char * 8),
-        ("tx_mid", ctypes.c_char * 8),
-        ("sector", ctypes.c_uint16)
-    ]
-
-    def __init__(self, *args, **kwargs):
-        self.tx_up = self.tx_low = self.tx_mid = "-"
-        super().__init__(*args, **kwargs)
-
-class Linedef(WADStruct):
-    """
-    Represents a map linedef.
-
-    Linedef.NONE is the placeholder value for unused sidedefs.
-    Using the value -1 is no longer supported.
-    """
-    NONE = 0xffff
-
-    _flags_ = [
-        ("impassable",     1),
-        ("block_monsters", 1),
-        ("two_sided",      1),
-        ("upper_unpeg",    1),
-        ("lower_unpeg",    1),
-        ("secret",         1),
-        ("block_sound",    1),
-        ("invisible",      1),
-        ("automap",        1)
-    ]
-
-    _fields_ = [
-        ("vx_a",   ctypes.c_uint16),
-        ("vx_b",   ctypes.c_uint16),
-        ("flags",  WADFlags(_flags_)),
-        ("action", ctypes.c_uint16),
-        ("tag",    ctypes.c_uint16),
-        ("front",  ctypes.c_uint16),
-        ("back",   ctypes.c_uint16)
-    ]
-    _anonymous_ = ("flags",)
-
-    def __init__(self, *args, **kwargs):
-        self.front = self.back = Linedef.NONE
-        super().__init__(*args, **kwargs)
-
-# TODO: an enum or something for triggers
-class ZLinedef(WADStruct):
-    """
-    Represents a map linedef (Hexen / ZDoom).
-
-    Linedef.NONE is the placeholder value for unused sidedefs.
-    Using the value -1 is no longer supported.
-    """
-    _flags_ = [
-        ("impassable",     1),
-        ("block_monsters", 1),
-        ("two_sided",      1),
-        ("upper_unpeg",    1),
-        ("lower_unpeg",    1),
-        ("secret",         1),
-        ("block_sound",    1),
-        ("invisible",      1),
-        ("automap",        1),
-        ("repeat",         1),
-        ("trigger",        3),
-        ("activate_any",   1),
-        ("dummy",          1),
-        ("block_all",      1)
-    ]
-
-    _fields_ = [
-        ("vx_a",   ctypes.c_uint16),
-        ("vx_b",   ctypes.c_uint16),
-        ("flags",  WADFlags(_flags_)),
-        ("action", ctypes.c_ubyte),
-        ("arg0",   ctypes.c_ubyte),
-        ("arg1",   ctypes.c_ubyte),
-        ("arg2",   ctypes.c_ubyte),
-        ("arg3",   ctypes.c_ubyte),
-        ("arg4",   ctypes.c_ubyte),
-        ("front",  ctypes.c_uint16),
-        ("back",   ctypes.c_uint16)
-    ]
-    _anonymous_ = ("flags",)
-
-    def __init__(self, *args, **kwargs):
-        self.front = self.back = Linedef.NONE
-        super().__init__(*args, **kwargs)
-
-class Thing(WADStruct):
-    """Represents a map thing."""
-    _flags_ = [
-        ("easy",        1),
-        ("medium",      1),
-        ("hard",        1),
-        ("deaf",        1),
-        ("multiplayer", 1)
-    ]
-
-    _fields_ = [
-        ("x",     ctypes.c_int16),
-        ("y",     ctypes.c_int16),
-        ("angle", ctypes.c_uint16),
-        ("type",  ctypes.c_uint16),
-        ("flags", WADFlags(_flags_))
-    ]
-    _anonymous_ = ("flags",)
-
-class ZThing(WADStruct):
-    """Represents a map thing (Hexen / ZDoom)."""
-    _flags_ = [
-        ("easy",        1),
-        ("medium",      1),
-        ("hard",        1),
-        ("deaf",        1),
-        ("dormant",     1),
-        ("fighter",     1),
-        ("cleric",      1),
-        ("mage",        1),
-        ("solo",        1),
-        ("multiplayer", 1),
-        ("deathmatch",  1)
-    ]
-
-    _fields_ = [
-        ("tid",     ctypes.c_uint16),
-        ("x",       ctypes.c_int16),
-        ("y",       ctypes.c_int16),
-        ("height",  ctypes.c_int16),
-        ("angle",   ctypes.c_uint16),
-        ("type",    ctypes.c_uint16),
-        ("flags",   WADFlags(_flags_)),
-        ("action",  ctypes.c_ubyte),
-        ("arg0",    ctypes.c_ubyte),
-        ("arg1",    ctypes.c_ubyte),
-        ("arg2",    ctypes.c_ubyte),
-        ("arg3",    ctypes.c_ubyte),
-        ("arg4",    ctypes.c_ubyte)
-    ]
-    _anonymous_ = ("flags",)
-
-class Sector(WADStruct):
-    """Represents a map sector."""
-    _fields_ = [
-        ("z_floor",  ctypes.c_int16),
-        ("z_ceil",   ctypes.c_int16),
-        ("tx_floor", ctypes.c_char * 8),
-        ("tx_ceil",  ctypes.c_char * 8),
-        ("light",    ctypes.c_uint16),
-        ("type",     ctypes.c_uint16),
-        ("tag",      ctypes.c_uint16)
-    ]
-
-    def __init__(self, *args, **kwargs):
-        self.z_ceil = 128
-        self.light = 160
-        self.tx_floor = "FLOOR4_8"
-        self.tx_ceil = "CEIL3_5"
-        super().__init__(*args, **kwargs)
-
-class Node(WADStruct):
-    """Represents a BSP tree node."""
-    _fields_ = [
-        ("x_start",           ctypes.c_int16),
-        ("y_start",           ctypes.c_int16),
-        ("x_vector",          ctypes.c_int16),
-        ("y_vector",          ctypes.c_int16),
-        ("right_bbox_top",    ctypes.c_int16),
-        ("right_bbox_bottom", ctypes.c_int16),
-        ("right_bbox_left",   ctypes.c_int16),
-        ("right_bbox_right",  ctypes.c_int16),
-        ("left_bbox_top",     ctypes.c_int16),
-        ("left_bbox_bottom",  ctypes.c_int16),
-        ("left_bbox_left",    ctypes.c_int16),
-        ("left_bbox_right",   ctypes.c_int16),
-        ("right_index",       ctypes.c_uint16),
-        ("left_index",        ctypes.c_uint16)
-    ]
-
-class Seg(WADStruct):
-    """Represents a map seg."""
-    _fields_ = [
-        ("vx_a",   ctypes.c_uint16),
-        ("vx_b",   ctypes.c_uint16),
-        ("angle",  ctypes.c_uint16),
-        ("line",   ctypes.c_uint16),
-        ("side",   ctypes.c_uint16),
-        ("offset", ctypes.c_uint16)
-    ]
-
-class GLSeg(WADStruct):
-    """Represents a map GL seg."""
-    _fields_ = [
-        ("vx_a",    ctypes.c_uint16),
-        ("vx_b",    ctypes.c_uint16),
-        ("line",    ctypes.c_uint16),
-        ("side",    ctypes.c_uint16),
-        ("partner", ctypes.c_uint16)
-    ]
-
-class SubSector(WADStruct):
-    """Represents a map subsector."""
-    _fields_ = [
-        ("numsegs", ctypes.c_uint16),
-        ("seg_a",   ctypes.c_uint16)
-    ]
-
-class MapEditor:
-    """Doom map editor.
-
-    Data members:
-        header        Lump object consisting of data in map header (if any)
-        vertexes      List containing Vertex objects
-        sidedefs      List containing Sidedef objects
-        linedefs      List containing Linedef or ZLinedef objects
-        sectors       List containing Sector objects
-        things        List containing Thing or ZThing objects
-
-    Data members (Hexen/ZDoom formats only):
-        behavior      Lump object containing compiled ACS scripts
-        scripts       Lump object containing ACS script source
-
-    Other members:
-        Thing         alias to Thing or ZThing class, depending on format
-        Linedef       alias to Linedef or ZLinedef class, depending on format
-
-    Currently present but unused:
-        segs          List containing Seg objects
-        ssectors      List containing SubSector objects
-        nodes         List containing Node objects
-        blockmap      Lump object containing blockmap data
-        reject        Lump object containing reject table data
-        (These five lumps are not updated when saving; you will need to use
-        an external node builder utility)
-        """
-
-    def __init__(self, from_lumps=None):
-        """Create new, optionally from a lump group."""
-        if from_lumps is not None:
-            self.from_lumps(from_lumps)
-        else:
-            self.Thing   = Thing
-            self.Linedef = Linedef
-
-            self.header   = Lump()
-            self.vertexes = []
-            self.sidedefs = []
-            self.linedefs = []
-            self.sectors  = []
-            self.things   = []
-            self.segs     = []
-            self.ssectors = []
-            self.nodes    = []
-            self.blockmap = Lump("")
-            self.reject   = Lump("")
-
-    def _unpack_lump(self, class_, data):
-        s = ctypes.sizeof(class_)
-        return [class_(bytes=data[i:i+s]) for i in range(0,len(data),s)]
-
-    def from_lumps(self, lumpgroup):
-        """Load entries from a lump group."""
-        m = lumpgroup
-
-        try:
-            self.header   = m["_HEADER_"]
-
-            self.vertexes = self._unpack_lump(Vertex,    m["VERTEXES"].data)
-            self.sidedefs = self._unpack_lump(Sidedef,   m["SIDEDEFS"].data)
-            self.sectors  = self._unpack_lump(Sector,    m["SECTORS"].data)
-
-            if "BEHAVIOR" in m:
-                # Hexen / ZDoom map
-                self.Thing   = ZThing
-                self.Linedef = ZLinedef
-                self.behavior = m["BEHAVIOR"]
-                # optional script sources
-                try:
-                    self.scripts = m[wcinlist(m, "SCRIPT*")[0]]
-                except IndexError:
-                    self.scripts = Lump()
-            else:
-                self.Thing   = Thing
-                self.Linedef = Linedef
-                try:
-                    del self.behavior
-                    del self.scripts
-                except AttributeError:
-                    pass
-
-            self.things   = self._unpack_lump(self.Thing,   m["THINGS"].data)
-            self.linedefs = self._unpack_lump(self.Linedef, m["LINEDEFS"].data)
-        except KeyError as e:
-            raise ValueError("map is missing %s lump" % e)
-
-        from struct import error as StructError
-        try:
-            self.ssectors = self._unpack_lump(SubSector, m["SSECTORS"].data)
-            self.segs     = self._unpack_lump(Seg,       m["SEGS"].data)
-            self.nodes    = self._unpack_lump(Node,      m["NODES"].data)
-            self.blockmap = m["BLOCKMAP"]
-            self.reject   = m["REJECT"]
-        except (KeyError, StructError):
-            # nodes failed to build - we don't really care
-            # TODO: this also "handles" (read: ignores) expanded zdoom nodes)
-            self.ssectors = []
-            self.segs     = []
-            self.nodes    = []
-            self.blockmap = Lump()
-            self.reject   = Lump()
-
-    def load_gl(self, mapobj):
-        """Load GL nodes entries from a map."""
-        vxdata = mapobj["GL_VERT"].data[4:]  # s[:4] == "gNd3" ?
-        self.gl_vert  = self._unpack_lump(GLVertex,  vxdata)
-        self.gl_segs  = self._unpack_lump(GLSeg,     mapobj["GL_SEGS"].data)
-        self.gl_ssect = self._unpack_lump(SubSector, mapobj["GL_SSECT"].data)
-
-    def to_lumps(self):
-        m = NameGroup()
-
-        m["_HEADER_"] = self.header
-        m["VERTEXES"] = Lump(join([x.pack() for x in self.vertexes]))
-        m["THINGS"  ] = Lump(join([x.pack() for x in self.things  ]))
-        m["LINEDEFS"] = Lump(join([x.pack() for x in linedefs     ]))
-        m["SIDEDEFS"] = Lump(join([x.pack() for x in self.sidedefs]))
-        m["SECTORS" ] = Lump(join([x.pack() for x in self.sectors ]))
-        m["NODES"]    = Lump(join([x.pack() for x in self.nodes   ]))
-        m["SEGS"]     = Lump(join([x.pack() for x in self.segs    ]))
-        m["SSECTORS"] = Lump(join([x.pack() for x in self.ssectors]))
-        m["BLOCKMAP"] = self.blockmap
-        m["REJECT"]   = self.reject
-
-        # hexen / zdoom script lumps
-        try:
-            m["BEHAVIOR"] = self.behavior
-            m["SCRIPTS"]  = self.scripts
-        except AttributeError:
-            pass
-
-        return m
-
-    def draw_sector(self, vertexes, sector=None, sidedef=None):
-        """Draw a polygon from a list of vertexes. The vertexes may be
-        either Vertex objects or simple (x, y) tuples. A sector object
-        and prototype sidedef may be provided."""
-        assert len(vertexes) > 2
-        firstv = len(self.vertexes)
-        firsts = len(self.sidedefs)
-        if sector  is None: sector  = Sector()
-        if sidedef is None: sidedef = Sidedef()
-        self.sectors.append(copy(sector))
-        for i, v in enumerate(vertexes):
-            if isinstance(v, tuple):
-                x, y = v
-            else:
-                x, y = v.x, v.y
-            self.vertexes.append(Vertex(x, y))
-        for i in range(len(vertexes)):
-            side = copy(sidedef)
-            side.sector = len(self.sectors)-1
-            self.sidedefs.append(side)
-
-            #check if the new line is being written over an existing
-            #and merge them if so.
-            new_linedef = Linedef(vx_a=firstv+((i+1)%len(vertexes)),
-                                  vx_b=firstv+i, front=firsts+i, flags=1)
-            match_existing = False
-            for lc in self.linedefs:
-                if (self.compare_linedefs(new_linedef,lc) > 0):
-                    #remove midtexture and apply it to the upper/lower
-                    side.tx_low = self.sidedefs[lc.front].tx_mid
-                    side.tx_up = self.sidedefs[lc.front].tx_mid
-                    self.sidedefs[lc.front].tx_low = side.tx_mid
-                    self.sidedefs[lc.front].tx_up = side.tx_mid
-                    side.tx_mid = "-"
-                    self.sidedefs[lc.front].tx_mid = "-"
-                    lc.back = len(self.sidedefs)-1
-                    match_existing = True
-                    lc.two_sided = True
-                    lc.impassable = False
-                    break
-            if (match_existing == False):
-                self.linedefs.append(new_linedef)
-
-    def compare_vertex_positions(self,vertex1,vertex2):
-        """Compares the positions of two vertices."""
-        if (vertex1.x == vertex2.x):
-            if (vertex1.y == vertex2.y):
-                return True
-        return False
-
-    def compare_linedefs(self,linedef1,linedef2):
-        """Compare the vertex positions of two linedefs.
-        Returns 0 for mismatch.
-        Returns 1 when the vertex positions are the same.
-        Returns 2 when the vertex positions are in the same order.
-        Returns 3 when the linedefs use the same vertices, but flipped.
-        Returns 4 when the linedefs use the exact same vertices.
-        """
-        if (linedef1.vx_a == linedef2.vx_a):
-            if (linedef1.vx_b == linedef2.vx_b):
-                return 4
-
-        if (linedef1.vx_a == linedef2.vx_b):
-            if (linedef1.vx_b == linedef2.vx_a):
-                return 3
-
-        if (self.compare_vertex_positions(self.vertexes[linedef1.vx_a],
-            self.vertexes[linedef2.vx_a])):
-            if (self.compare_vertex_positions(self.vertexes[linedef1.vx_b],
-                self.vertexes[linedef2.vx_b])):
-                return 2
-
-        if (self.compare_vertex_positions(self.vertexes[linedef1.vx_a],
-            self.vertexes[linedef2.vx_b])):
-            if (self.compare_vertex_positions(self.vertexes[linedef1.vx_b],
-                self.vertexes[linedef2.vx_a])):
-                return 1
-
-        return 0
-
-    def compare_sectors(self,sect1,sect2):
-        """Compare two sectors' data and returns True when they match."""
-        if (sect1.z_floor == sect2.z_floor and
-            sect1.z_ceil == sect2.z_ceil and
-            sect1.tx_floor == sect2.tx_floor and
-            sect1.tx_ceil == sect2.tx_ceil and
-            sect1.light == sect2.light and
-            sect1.type == sect2.type and
-            sect1.tag == sect2.tag):
-            return True
-        return False
-
-    def combine_sectors(self,sector1,sector2,remove_linedefs=True):
-        """Combines two sectors together, replacing all references to
-        the second with the first. If remove_linedefs is true, any
-        linedefs that connect the two sectors will be removed."""
-        for sd in self.sidedefs:
-            if (self.sectors[sd.sector] == sector2):
-                sd.sector = self.sectors.index(sector1)
-
-                if (remove_linedefs):
-                    for lc in self.linedefs:
-                        if (lc.back != Linedef.NONE):
-                            if (self.sectors[self.sidedefs[lc.front].sector] == sector1 and
-                                self.sectors[self.sidedefs[lc.back].sector] == sector1):
-                                self.linedefs.remove(lc)
-        # we can rely on a nodebuilder to remove unused sectors
-        # self.sectors[self.sectors.index(sector2)].tx_floor = "_REMOVED"
-
-    def paste(self, other, offset=(0,0)):
-        """Insert content of another map."""
-        vlen = len(self.vertexes)
-        ilen = len(self.sidedefs)
-        slen = len(self.sectors)
-        for vx in other.vertexes:
-            x, y = vx.x, vx.y
-            self.vertexes.append(Vertex(x+offset[0], y+offset[1]))
-        for line in other.linedefs:
-            z = copy(line)
-            z.vx_a += vlen
-            z.vx_b += vlen
-            if z.front != Linedef.NONE: z.front += ilen
-            if z.back != Linedef.NONE: z.back += ilen
-            self.linedefs.append(z)
-        for side in other.sidedefs:
-            z = copy(side)
-            z.sector += slen
-            self.sidedefs.append(z)
-        for sector in other.sectors:
-            z = copy(sector)
-            self.sectors.append(z)
-        for thing in other.things:
-            z = copy(thing)
-            z.x += offset[0]
-            z.y += offset[1]
-            self.things.append(z)
+from omg.util import *
+from omg.lump import *
+from omg.wad import NameGroup
+
+import omg.lineinfo as lineinfo
+import omg.thinginfo as thinginfo
+
+class Vertex(WADStruct):
+    """Represents a map vertex."""
+    _fields_ = [
+        ("x", ctypes.c_int16),
+        ("y", ctypes.c_int16)
+    ]
+
+class GLVertex(WADStruct):
+    """Represents a map GL vertex."""
+    _fields_ = [
+        ("x", ctypes.c_int32),
+        ("y", ctypes.c_int32)
+    ]
+
+class Sidedef(WADStruct):
+    """Represents a map sidedef."""
+    _fields_ = [
+        ("off_x",  ctypes.c_int16),
+        ("off_y",  ctypes.c_int16),
+        ("tx_up",  ctypes.c_char * 8),
+        ("tx_low", ctypes.c_char * 8),
+        ("tx_mid", ctypes.c_char * 8),
+        ("sector", ctypes.c_uint16)
+    ]
+
+    def __init__(self, *args, **kwargs):
+        self.tx_up = self.tx_low = self.tx_mid = "-"
+        super().__init__(*args, **kwargs)
+
+class Linedef(WADStruct):
+    """
+    Represents a map linedef.
+
+    Linedef.NONE is the placeholder value for unused sidedefs.
+    Using the value -1 is no longer supported.
+    """
+    NONE = 0xffff
+
+    _flags_ = [
+        ("impassable",     1),
+        ("block_monsters", 1),
+        ("two_sided",      1),
+        ("upper_unpeg",    1),
+        ("lower_unpeg",    1),
+        ("secret",         1),
+        ("block_sound",    1),
+        ("invisible",      1),
+        ("automap",        1)
+    ]
+
+    _fields_ = [
+        ("vx_a",   ctypes.c_uint16),
+        ("vx_b",   ctypes.c_uint16),
+        ("flags",  WADFlags(_flags_)),
+        ("action", ctypes.c_uint16),
+        ("tag",    ctypes.c_uint16),
+        ("front",  ctypes.c_uint16),
+        ("back",   ctypes.c_uint16)
+    ]
+    _anonymous_ = ("flags",)
+
+    def __init__(self, *args, **kwargs):
+        self.front = self.back = Linedef.NONE
+        super().__init__(*args, **kwargs)
+
+# TODO: an enum or something for triggers
+class ZLinedef(WADStruct):
+    """
+    Represents a map linedef (Hexen / ZDoom).
+
+    Linedef.NONE is the placeholder value for unused sidedefs.
+    Using the value -1 is no longer supported.
+    """
+    _flags_ = [
+        ("impassable",     1),
+        ("block_monsters", 1),
+        ("two_sided",      1),
+        ("upper_unpeg",    1),
+        ("lower_unpeg",    1),
+        ("secret",         1),
+        ("block_sound",    1),
+        ("invisible",      1),
+        ("automap",        1),
+        ("repeat",         1),
+        ("trigger",        3),
+        ("activate_any",   1),
+        ("dummy",          1),
+        ("block_all",      1)
+    ]
+
+    _fields_ = [
+        ("vx_a",   ctypes.c_uint16),
+        ("vx_b",   ctypes.c_uint16),
+        ("flags",  WADFlags(_flags_)),
+        ("action", ctypes.c_ubyte),
+        ("arg0",   ctypes.c_ubyte),
+        ("arg1",   ctypes.c_ubyte),
+        ("arg2",   ctypes.c_ubyte),
+        ("arg3",   ctypes.c_ubyte),
+        ("arg4",   ctypes.c_ubyte),
+        ("front",  ctypes.c_uint16),
+        ("back",   ctypes.c_uint16)
+    ]
+    _anonymous_ = ("flags",)
+
+    def __init__(self, *args, **kwargs):
+        self.front = self.back = Linedef.NONE
+        super().__init__(*args, **kwargs)
+
+class Thing(WADStruct):
+    """Represents a map thing."""
+    _flags_ = [
+        ("easy",        1),
+        ("medium",      1),
+        ("hard",        1),
+        ("deaf",        1),
+        ("multiplayer", 1)
+    ]
+
+    _fields_ = [
+        ("x",     ctypes.c_int16),
+        ("y",     ctypes.c_int16),
+        ("angle", ctypes.c_uint16),
+        ("type",  ctypes.c_uint16),
+        ("flags", WADFlags(_flags_))
+    ]
+    _anonymous_ = ("flags",)
+
+class ZThing(WADStruct):
+    """Represents a map thing (Hexen / ZDoom)."""
+    _flags_ = [
+        ("easy",        1),
+        ("medium",      1),
+        ("hard",        1),
+        ("deaf",        1),
+        ("dormant",     1),
+        ("fighter",     1),
+        ("cleric",      1),
+        ("mage",        1),
+        ("solo",        1),
+        ("multiplayer", 1),
+        ("deathmatch",  1)
+    ]
+
+    _fields_ = [
+        ("tid",     ctypes.c_uint16),
+        ("x",       ctypes.c_int16),
+        ("y",       ctypes.c_int16),
+        ("height",  ctypes.c_int16),
+        ("angle",   ctypes.c_uint16),
+        ("type",    ctypes.c_uint16),
+        ("flags",   WADFlags(_flags_)),
+        ("action",  ctypes.c_ubyte),
+        ("arg0",    ctypes.c_ubyte),
+        ("arg1",    ctypes.c_ubyte),
+        ("arg2",    ctypes.c_ubyte),
+        ("arg3",    ctypes.c_ubyte),
+        ("arg4",    ctypes.c_ubyte)
+    ]
+    _anonymous_ = ("flags",)
+
+class Sector(WADStruct):
+    """Represents a map sector."""
+    _fields_ = [
+        ("z_floor",  ctypes.c_int16),
+        ("z_ceil",   ctypes.c_int16),
+        ("tx_floor", ctypes.c_char * 8),
+        ("tx_ceil",  ctypes.c_char * 8),
+        ("light",    ctypes.c_uint16),
+        ("type",     ctypes.c_uint16),
+        ("tag",      ctypes.c_uint16)
+    ]
+
+    def __init__(self, *args, **kwargs):
+        self.z_ceil = 128
+        self.light = 160
+        self.tx_floor = "FLOOR4_8"
+        self.tx_ceil = "CEIL3_5"
+        super().__init__(*args, **kwargs)
+
+class Node(WADStruct):
+    """Represents a BSP tree node."""
+    _fields_ = [
+        ("x_start",           ctypes.c_int16),
+        ("y_start",           ctypes.c_int16),
+        ("x_vector",          ctypes.c_int16),
+        ("y_vector",          ctypes.c_int16),
+        ("right_bbox_top",    ctypes.c_int16),
+        ("right_bbox_bottom", ctypes.c_int16),
+        ("right_bbox_left",   ctypes.c_int16),
+        ("right_bbox_right",  ctypes.c_int16),
+        ("left_bbox_top",     ctypes.c_int16),
+        ("left_bbox_bottom",  ctypes.c_int16),
+        ("left_bbox_left",    ctypes.c_int16),
+        ("left_bbox_right",   ctypes.c_int16),
+        ("right_index",       ctypes.c_uint16),
+        ("left_index",        ctypes.c_uint16)
+    ]
+
+class Seg(WADStruct):
+    """Represents a map seg."""
+    _fields_ = [
+        ("vx_a",   ctypes.c_uint16),
+        ("vx_b",   ctypes.c_uint16),
+        ("angle",  ctypes.c_uint16),
+        ("line",   ctypes.c_uint16),
+        ("side",   ctypes.c_uint16),
+        ("offset", ctypes.c_uint16)
+    ]
+
+class GLSeg(WADStruct):
+    """Represents a map GL seg."""
+    _fields_ = [
+        ("vx_a",    ctypes.c_uint16),
+        ("vx_b",    ctypes.c_uint16),
+        ("line",    ctypes.c_uint16),
+        ("side",    ctypes.c_uint16),
+        ("partner", ctypes.c_uint16)
+    ]
+
+class SubSector(WADStruct):
+    """Represents a map subsector."""
+    _fields_ = [
+        ("numsegs", ctypes.c_uint16),
+        ("seg_a",   ctypes.c_uint16)
+    ]
+
+class MapEditor:
+    """Doom map editor.
+
+    Data members:
+        header        Lump object consisting of data in map header (if any)
+        vertexes      List containing Vertex objects
+        sidedefs      List containing Sidedef objects
+        linedefs      List containing Linedef or ZLinedef objects
+        sectors       List containing Sector objects
+        things        List containing Thing or ZThing objects
+
+    Data members (Hexen/ZDoom formats only):
+        behavior      Lump object containing compiled ACS scripts
+        scripts       Lump object containing ACS script source
+
+    Other members:
+        Thing         alias to Thing or ZThing class, depending on format
+        Linedef       alias to Linedef or ZLinedef class, depending on format
+
+    Currently present but unused:
+        segs          List containing Seg objects
+        ssectors      List containing SubSector objects
+        nodes         List containing Node objects
+        blockmap      Lump object containing blockmap data
+        reject        Lump object containing reject table data
+        (These five lumps are not updated when saving; you will need to use
+        an external node builder utility)
+        """
+
+    def __init__(self, from_lumps=None):
+        """Create new, optionally from a lump group."""
+        if from_lumps is not None:
+            self.from_lumps(from_lumps)
+        else:
+            self.Thing   = Thing
+            self.Linedef = Linedef
+
+            self.header   = Lump()
+            self.vertexes = []
+            self.sidedefs = []
+            self.linedefs = []
+            self.sectors  = []
+            self.things   = []
+            self.segs     = []
+            self.ssectors = []
+            self.nodes    = []
+            self.blockmap = Lump("")
+            self.reject   = Lump("")
+
+    def _unpack_lump(self, class_, data):
+        s = ctypes.sizeof(class_)
+        return [class_(bytes=data[i:i+s]) for i in range(0,len(data),s)]
+
+    def from_lumps(self, lumpgroup):
+        """Load entries from a lump group."""
+        m = lumpgroup
+
+        try:
+            self.header   = m["_HEADER_"]
+
+            self.vertexes = self._unpack_lump(Vertex,    m["VERTEXES"].data)
+            self.sidedefs = self._unpack_lump(Sidedef,   m["SIDEDEFS"].data)
+            self.sectors  = self._unpack_lump(Sector,    m["SECTORS"].data)
+
+            if "BEHAVIOR" in m:
+                # Hexen / ZDoom map
+                self.Thing   = ZThing
+                self.Linedef = ZLinedef
+                self.behavior = m["BEHAVIOR"]
+                # optional script sources
+                try:
+                    self.scripts = m[wcinlist(m, "SCRIPT*")[0]]
+                except IndexError:
+                    self.scripts = Lump()
+            else:
+                self.Thing   = Thing
+                self.Linedef = Linedef
+                try:
+                    del self.behavior
+                    del self.scripts
+                except AttributeError:
+                    pass
+
+            self.things   = self._unpack_lump(self.Thing,   m["THINGS"].data)
+            self.linedefs = self._unpack_lump(self.Linedef, m["LINEDEFS"].data)
+        except KeyError as e:
+            raise ValueError("map is missing %s lump" % e)
+
+        from struct import error as StructError
+        try:
+            self.ssectors = self._unpack_lump(SubSector, m["SSECTORS"].data)
+            self.segs     = self._unpack_lump(Seg,       m["SEGS"].data)
+            self.nodes    = self._unpack_lump(Node,      m["NODES"].data)
+            self.blockmap = m["BLOCKMAP"]
+            self.reject   = m["REJECT"]
+        except (KeyError, StructError):
+            # nodes failed to build - we don't really care
+            # TODO: this also "handles" (read: ignores) expanded zdoom nodes)
+            self.ssectors = []
+            self.segs     = []
+            self.nodes    = []
+            self.blockmap = Lump()
+            self.reject   = Lump()
+
+    def load_gl(self, mapobj):
+        """Load GL nodes entries from a map."""
+        vxdata = mapobj["GL_VERT"].data[4:]  # s[:4] == "gNd3" ?
+        self.gl_vert  = self._unpack_lump(GLVertex,  vxdata)
+        self.gl_segs  = self._unpack_lump(GLSeg,     mapobj["GL_SEGS"].data)
+        self.gl_ssect = self._unpack_lump(SubSector, mapobj["GL_SSECT"].data)
+
+    def to_lumps(self):
+        m = NameGroup()
+
+        m["_HEADER_"] = self.header
+        m["VERTEXES"] = Lump(join([x.pack() for x in self.vertexes]))
+        m["THINGS"  ] = Lump(join([x.pack() for x in self.things  ]))
+        m["LINEDEFS"] = Lump(join([x.pack() for x in self.linedefs]))
+        m["SIDEDEFS"] = Lump(join([x.pack() for x in self.sidedefs]))
+        m["SECTORS" ] = Lump(join([x.pack() for x in self.sectors ]))
+        m["NODES"]    = Lump(join([x.pack() for x in self.nodes   ]))
+        m["SEGS"]     = Lump(join([x.pack() for x in self.segs    ]))
+        m["SSECTORS"] = Lump(join([x.pack() for x in self.ssectors]))
+        m["BLOCKMAP"] = self.blockmap
+        m["REJECT"]   = self.reject
+
+        # hexen / zdoom script lumps
+        try:
+            m["BEHAVIOR"] = self.behavior
+            m["SCRIPTS"]  = self.scripts
+        except AttributeError:
+            pass
+
+        return m
+
+    def draw_sector(self, vertexes, sector=None, sidedef=None):
+        """Draw a polygon from a list of vertexes. The vertexes may be
+        either Vertex objects or simple (x, y) tuples. A sector object
+        and prototype sidedef may be provided."""
+        assert len(vertexes) > 2
+        firstv = len(self.vertexes)
+        firsts = len(self.sidedefs)
+        if sector  is None: sector  = Sector()
+        if sidedef is None: sidedef = Sidedef()
+        self.sectors.append(copy(sector))
+        for i, v in enumerate(vertexes):
+            if isinstance(v, tuple):
+                x, y = v
+            else:
+                x, y = v.x, v.y
+            self.vertexes.append(Vertex(x, y))
+        for i in range(len(vertexes)):
+            side = copy(sidedef)
+            side.sector = len(self.sectors)-1
+            self.sidedefs.append(side)
+
+            #check if the new line is being written over an existing
+            #and merge them if so.
+            new_linedef = Linedef(vx_a=firstv+((i+1)%len(vertexes)),
+                                  vx_b=firstv+i, front=firsts+i, flags=1)
+            match_existing = False
+            for lc in self.linedefs:
+                if (self.compare_linedefs(new_linedef,lc) > 0):
+                    #remove midtexture and apply it to the upper/lower
+                    side.tx_low = self.sidedefs[lc.front].tx_mid
+                    side.tx_up = self.sidedefs[lc.front].tx_mid
+                    self.sidedefs[lc.front].tx_low = side.tx_mid
+                    self.sidedefs[lc.front].tx_up = side.tx_mid
+                    side.tx_mid = "-"
+                    self.sidedefs[lc.front].tx_mid = "-"
+                    lc.back = len(self.sidedefs)-1
+                    match_existing = True
+                    lc.two_sided = True
+                    lc.impassable = False
+                    break
+            if (match_existing == False):
+                self.linedefs.append(new_linedef)
+
+    def compare_vertex_positions(self,vertex1,vertex2):
+        """Compares the positions of two vertices."""
+        if (vertex1.x == vertex2.x):
+            if (vertex1.y == vertex2.y):
+                return True
+        return False
+
+    def compare_linedefs(self,linedef1,linedef2):
+        """Compare the vertex positions of two linedefs.
+        Returns 0 for mismatch.
+        Returns 1 when the vertex positions are the same.
+        Returns 2 when the vertex positions are in the same order.
+        Returns 3 when the linedefs use the same vertices, but flipped.
+        Returns 4 when the linedefs use the exact same vertices.
+        """
+        if (linedef1.vx_a == linedef2.vx_a):
+            if (linedef1.vx_b == linedef2.vx_b):
+                return 4
+
+        if (linedef1.vx_a == linedef2.vx_b):
+            if (linedef1.vx_b == linedef2.vx_a):
+                return 3
+
+        if (self.compare_vertex_positions(self.vertexes[linedef1.vx_a],
+            self.vertexes[linedef2.vx_a])):
+            if (self.compare_vertex_positions(self.vertexes[linedef1.vx_b],
+                self.vertexes[linedef2.vx_b])):
+                return 2
+
+        if (self.compare_vertex_positions(self.vertexes[linedef1.vx_a],
+            self.vertexes[linedef2.vx_b])):
+            if (self.compare_vertex_positions(self.vertexes[linedef1.vx_b],
+                self.vertexes[linedef2.vx_a])):
+                return 1
+
+        return 0
+
+    def compare_sectors(self,sect1,sect2):
+        """Compare two sectors' data and returns True when they match."""
+        if (sect1.z_floor == sect2.z_floor and
+            sect1.z_ceil == sect2.z_ceil and
+            sect1.tx_floor == sect2.tx_floor and
+            sect1.tx_ceil == sect2.tx_ceil and
+            sect1.light == sect2.light and
+            sect1.type == sect2.type and
+            sect1.tag == sect2.tag):
+            return True
+        return False
+
+    def combine_sectors(self,sector1,sector2,remove_linedefs=True):
+        """Combines two sectors together, replacing all references to
+        the second with the first. If remove_linedefs is true, any
+        linedefs that connect the two sectors will be removed."""
+        for sd in self.sidedefs:
+            if (self.sectors[sd.sector] == sector2):
+                sd.sector = self.sectors.index(sector1)
+
+                if (remove_linedefs):
+                    for lc in self.linedefs:
+                        if (lc.back != Linedef.NONE):
+                            if (self.sectors[self.sidedefs[lc.front].sector] == sector1 and
+                                self.sectors[self.sidedefs[lc.back].sector] == sector1):
+                                self.linedefs.remove(lc)
+        # we can rely on a nodebuilder to remove unused sectors
+        # self.sectors[self.sectors.index(sector2)].tx_floor = "_REMOVED"
+
+    def paste(self, other, offset=(0,0)):
+        """Insert content of another map."""
+        vlen = len(self.vertexes)
+        ilen = len(self.sidedefs)
+        slen = len(self.sectors)
+        for vx in other.vertexes:
+            x, y = vx.x, vx.y
+            self.vertexes.append(Vertex(x+offset[0], y+offset[1]))
+        for line in other.linedefs:
+            z = copy(line)
+            z.vx_a += vlen
+            z.vx_b += vlen
+            if z.front != Linedef.NONE: z.front += ilen
+            if z.back != Linedef.NONE: z.back += ilen
+            self.linedefs.append(z)
+        for side in other.sidedefs:
+            z = copy(side)
+            z.sector += slen
+            self.sidedefs.append(z)
+        for sector in other.sectors:
+            z = copy(sector)
+            self.sectors.append(z)
+        for thing in other.things:
+            z = copy(thing)
+            z.x += offset[0]
+            z.y += offset[1]
+            self.things.append(z)
```

### Comparing `omgifol-0.5.0/omg/palette.py` & `omgifol-0.5.1/omg/palette.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,227 +1,227 @@
-from struct   import pack, unpack
-from omg.util import *
-
-class Palette:
-
-    """Used for storing a list of colors and doing things with them
-    (such as looking up the best match for arbitrary RGB values).
-
-    Palette is distinct from Colormap and Playpal; these two provide
-    lump- and WAD-related operations while delegating (some of) their
-    color processing to Palette.
-
-    Fields containing useful public data (modifying them directly
-    probably isn't a good idea, however):
-
-        .colors       List of (r, g, b) tuples
-        .bytes        Palette's colors as a bytes object (rgbrgbrgb...)
-        .save_bytes   Same as above, but with the transparency color set;
-                      useful when saving files
-        .tran_color   (r, g, b) value for transparency
-        .tran_index   Index in palette of transparency color
-
-    The following fields are intended for internal use:
-
-        .memo         Table for RGB lookup memoization
-        .grays        List of indices of colors with zero saturation
-        .bright_lut   Brightness LUT, used internally to speed up
-                      lookups (when not memoized).
-    """
-
-    def __init__(self, colors=None, tran_index=None, tran_color=None):
-        """Creates a new Palette object. The 'colors' argument may be
-        either a list of (r,g,b) tuples or an RGBRGBRGB... string/bytes.
-        'tran_index' specifies the index in the palette where the
-        transparent color should be placed. Note that this is only used
-        when saving images, and thus doesn't affect color lookups.
-        'tran_color' is the color to use for transparency."""
-
-        colors = colors or default_colors
-        tran_index = tran_index or default_tran_index
-        tran_color = tran_color or default_tran_color
-
-        if isinstance(colors, str):
-            colors = colors.encode('latin-1')
-
-        if isinstance(colors, list):
-            self.colors = colors[:]
-        elif isinstance(colors, bytes):
-            self.colors = [unpack('BBB', colors[i:i+3]) for i in range(0,768,3)]
-        else:
-            raise TypeError("Argument 'colors' must be list or string or bytes")
-
-        # Doom graphics don't actually use indices for transparency; the
-        # following data is only used when converting between image formats.
-        self.tran_index = tran_index
-        self.tran_color = tran_color
-        self.make_bytes()
-        self.make_grays()
-
-        # Memoizing color translations can speed up RGB-to-palette
-        # conversions significantly, in particular when converting
-        # lots of graphics in one session. See docstring for build_lut
-        # below for description of what bright_lut does.
-        self.memo = {}
-        self.bright_lut = []
-        self.reset_memo()
-
-    def make_bytes(self):
-        """Create/update 'bytes' and 'save_bytes' from the current set of
-        colors and the 'tran_index' and 'tran_color' fields."""
-        self.bytes = bytes().join([pack('BBB', *rgb) for rgb in self.colors])
-        self.save_bytes = \
-            self.bytes[:self.tran_index*3] + \
-            pack('BBB', *self.tran_color) + \
-            self.bytes[(self.tran_index+1)*3:]
-
-    def make_grays(self):
-        """Create 'grays' table containing the indices of all grays
-        in the current set of colors."""
-        self.grays = [i for i, rgb in enumerate(self.colors) \
-            if (rgb[0]==rgb[1]==rgb[2])]
-
-    def reset_memo(self):
-        """Clear the memo table (but (re)add the palette's colors)"""
-        self.memo = {}
-        for i in range(len(self.colors)):
-            if i != self.tran_index:
-                self.memo[self.colors[i]] = i
-
-    def build_lut(self, distance=16):
-        """Build 256-entry LUT for looking up colors in the palette
-        close to a given brightness (range 0-255). Each entry is a
-        list of indices. No position is empty; in the worst case,
-        the closest gray can be used.
-
-        The 'distance' parameter defines what "close" is, and should
-        be an integer 0-256. Lower distance means faster lookups,
-        but worse precision.
-
-        A good value for Doom is 10. Anything over 32 only wastes time.
-        """
-        self.bright_lut = []
-        assert 0 <= distance <= 256
-        for level in range(256):
-            candidates = []
-            for j, rgb in enumerate(self.colors):
-                if abs(level - (sum(rgb) // 3)) < distance:
-                    candidates.append(j)
-            # Make sure each entry contains at least one gray
-            # color that can be relied on in the worst case
-            best_d = 256
-            best_i = 0
-            for gray_index in self.grays:
-                r, g, b = self.colors[gray_index]
-                dist = abs(r - level)
-                if dist < best_d:
-                    best_i = gray_index
-                    if dist == 0:
-                        break
-                    best_d = dist
-            if best_i not in candidates:
-                candidates.append(best_i)
-            self.bright_lut.append(candidates)
-
-    def match(self, color):
-        """Find the closest match in the palette for a color.
-        Takes an (r,g,b) tuple as argument and returns a palette index."""
-        if color == self.tran_color:
-            return self.tran_index
-        if color in self.memo:
-            return self.memo[color]
-        if len(self.bright_lut) == 0:
-            self.build_lut()
-        best_dist = 262144
-        best_i = 0
-        ar, ag, ab = color
-        candidates = self.bright_lut[int(sum(color)) // 3]
-        for i in candidates:
-            br, bg, bb = self.colors[i]
-            dr = ar-br
-            dg = ag-bg
-            db = ab-bb
-            dist = dr*dr + dg*dg + db*db
-            if dist < best_dist:
-                if dist == 0:
-                    return i
-                best_dist = dist
-                best_i = i
-        self.memo[color] = best_i
-        return best_i
-
-    def blend(self, color, intensity=0.5):
-        """Blend the entire palette against a color (given as an RGB triple).
-        Intensity must be a floating-point number in the range 0-1."""
-        assert 0.0 <= intensity <= 1.0
-        nr = color[0] * intensity
-        ng = color[1] * intensity
-        nb = color[2] * intensity
-        remain = 1.0 - intensity
-        for i in range(len(self.colors)):
-            ar, ag, ab = self.colors[i]
-            self.colors[i] = (int(ar*remain + nr),
-                              int(ag*remain + ng),
-                              int(ab*remain + nb))
-        self.make_bytes()
-        self.make_grays()
-        self.reset_memo()
-        self.bright_lut = []
-
-# Colors of the Doom palette, used by default
-default_colors = b"\
-\x00\x00\x00\x1f\x17\x0b\x17\x0f\x07\x4b\x4b\x4b\xff\xff\xff\x1b\
-\x1b\x1b\x13\x13\x13\x0b\x0b\x0b\x07\x07\x07\x2f\x37\x1f\x23\x2b\
-\x0f\x17\x1f\x07\x0f\x17\x00\x4f\x3b\x2b\x47\x33\x23\x3f\x2b\x1b\
-\xff\xb7\xb7\xf7\xab\xab\xf3\xa3\xa3\xeb\x97\x97\xe7\x8f\x8f\xdf\
-\x87\x87\xdb\x7b\x7b\xd3\x73\x73\xcb\x6b\x6b\xc7\x63\x63\xbf\x5b\
-\x5b\xbb\x57\x57\xb3\x4f\x4f\xaf\x47\x47\xa7\x3f\x3f\xa3\x3b\x3b\
-\x9b\x33\x33\x97\x2f\x2f\x8f\x2b\x2b\x8b\x23\x23\x83\x1f\x1f\x7f\
-\x1b\x1b\x77\x17\x17\x73\x13\x13\x6b\x0f\x0f\x67\x0b\x0b\x5f\x07\
-\x07\x5b\x07\x07\x53\x07\x07\x4f\x00\x00\x47\x00\x00\x43\x00\x00\
-\xff\xeb\xdf\xff\xe3\xd3\xff\xdb\xc7\xff\xd3\xbb\xff\xcf\xb3\xff\
-\xc7\xa7\xff\xbf\x9b\xff\xbb\x93\xff\xb3\x83\xf7\xab\x7b\xef\xa3\
-\x73\xe7\x9b\x6b\xdf\x93\x63\xd7\x8b\x5b\xcf\x83\x53\xcb\x7f\x4f\
-\xbf\x7b\x4b\xb3\x73\x47\xab\x6f\x43\xa3\x6b\x3f\x9b\x63\x3b\x8f\
-\x5f\x37\x87\x57\x33\x7f\x53\x2f\x77\x4f\x2b\x6b\x47\x27\x5f\x43\
-\x23\x53\x3f\x1f\x4b\x37\x1b\x3f\x2f\x17\x33\x2b\x13\x2b\x23\x0f\
-\xef\xef\xef\xe7\xe7\xe7\xdf\xdf\xdf\xdb\xdb\xdb\xd3\xd3\xd3\xcb\
-\xcb\xcb\xc7\xc7\xc7\xbf\xbf\xbf\xb7\xb7\xb7\xb3\xb3\xb3\xab\xab\
-\xab\xa7\xa7\xa7\x9f\x9f\x9f\x97\x97\x97\x93\x93\x93\x8b\x8b\x8b\
-\x83\x83\x83\x7f\x7f\x7f\x77\x77\x77\x6f\x6f\x6f\x6b\x6b\x6b\x63\
-\x63\x63\x5b\x5b\x5b\x57\x57\x57\x4f\x4f\x4f\x47\x47\x47\x43\x43\
-\x43\x3b\x3b\x3b\x37\x37\x37\x2f\x2f\x2f\x27\x27\x27\x23\x23\x23\
-\x77\xff\x6f\x6f\xef\x67\x67\xdf\x5f\x5f\xcf\x57\x5b\xbf\x4f\x53\
-\xaf\x47\x4b\x9f\x3f\x43\x93\x37\x3f\x83\x2f\x37\x73\x2b\x2f\x63\
-\x23\x27\x53\x1b\x1f\x43\x17\x17\x33\x0f\x13\x23\x0b\x0b\x17\x07\
-\xbf\xa7\x8f\xb7\x9f\x87\xaf\x97\x7f\xa7\x8f\x77\x9f\x87\x6f\x9b\
-\x7f\x6b\x93\x7b\x63\x8b\x73\x5b\x83\x6b\x57\x7b\x63\x4f\x77\x5f\
-\x4b\x6f\x57\x43\x67\x53\x3f\x5f\x4b\x37\x57\x43\x33\x53\x3f\x2f\
-\x9f\x83\x63\x8f\x77\x53\x83\x6b\x4b\x77\x5f\x3f\x67\x53\x33\x5b\
-\x47\x2b\x4f\x3b\x23\x43\x33\x1b\x7b\x7f\x63\x6f\x73\x57\x67\x6b\
-\x4f\x5b\x63\x47\x53\x57\x3b\x47\x4f\x33\x3f\x47\x2b\x37\x3f\x27\
-\xff\xff\x73\xeb\xdb\x57\xd7\xbb\x43\xc3\x9b\x2f\xaf\x7b\x1f\x9b\
-\x5b\x13\x87\x43\x07\x73\x2b\x00\xff\xff\xff\xff\xdb\xdb\xff\xbb\
-\xbb\xff\x9b\x9b\xff\x7b\x7b\xff\x5f\x5f\xff\x3f\x3f\xff\x1f\x1f\
-\xff\x00\x00\xef\x00\x00\xe3\x00\x00\xd7\x00\x00\xcb\x00\x00\xbf\
-\x00\x00\xb3\x00\x00\xa7\x00\x00\x9b\x00\x00\x8b\x00\x00\x7f\x00\
-\x00\x73\x00\x00\x67\x00\x00\x5b\x00\x00\x4f\x00\x00\x43\x00\x00\
-\xe7\xe7\xff\xc7\xc7\xff\xab\xab\xff\x8f\x8f\xff\x73\x73\xff\x53\
-\x53\xff\x37\x37\xff\x1b\x1b\xff\x00\x00\xff\x00\x00\xe3\x00\x00\
-\xcb\x00\x00\xb3\x00\x00\x9b\x00\x00\x83\x00\x00\x6b\x00\x00\x53\
-\xff\xff\xff\xff\xeb\xdb\xff\xd7\xbb\xff\xc7\x9b\xff\xb3\x7b\xff\
-\xa3\x5b\xff\x8f\x3b\xff\x7f\x1b\xf3\x73\x17\xeb\x6f\x0f\xdf\x67\
-\x0f\xd7\x5f\x0b\xcb\x57\x07\xc3\x4f\x00\xb7\x47\x00\xaf\x43\x00\
-\xff\xff\xff\xff\xff\xd7\xff\xff\xb3\xff\xff\x8f\xff\xff\x6b\xff\
-\xff\x47\xff\xff\x23\xff\xff\x00\xa7\x3f\x00\x9f\x37\x00\x93\x2f\
-\x00\x87\x23\x00\x4f\x3b\x27\x43\x2f\x1b\x37\x23\x13\x2f\x1b\x0b\
-\x00\x00\x53\x00\x00\x47\x00\x00\x3b\x00\x00\x2f\x00\x00\x23\x00\
-\x00\x17\x00\x00\x0b\x00\x00\x00\xff\x9f\x43\xff\xe7\x4b\xff\x7b\
-\xff\xff\x00\xff\xcf\x00\xcf\x9f\x00\x9b\x6f\x00\x6b\xa7\x6b\x6b\
-"
-
-# Defaults for image transparency
-default_tran_index = 247
-default_tran_color = (255, 0, 255)
-
-# Default palette object, using the default values
-default = Palette()
+from struct   import pack, unpack
+from omg.util import *
+
+class Palette:
+
+    """Used for storing a list of colors and doing things with them
+    (such as looking up the best match for arbitrary RGB values).
+
+    Palette is distinct from Colormap and Playpal; these two provide
+    lump- and WAD-related operations while delegating (some of) their
+    color processing to Palette.
+
+    Fields containing useful public data (modifying them directly
+    probably isn't a good idea, however):
+
+        .colors       List of (r, g, b) tuples
+        .bytes        Palette's colors as a bytes object (rgbrgbrgb...)
+        .save_bytes   Same as above, but with the transparency color set;
+                      useful when saving files
+        .tran_color   (r, g, b) value for transparency
+        .tran_index   Index in palette of transparency color
+
+    The following fields are intended for internal use:
+
+        .memo         Table for RGB lookup memoization
+        .grays        List of indices of colors with zero saturation
+        .bright_lut   Brightness LUT, used internally to speed up
+                      lookups (when not memoized).
+    """
+
+    def __init__(self, colors=None, tran_index=None, tran_color=None):
+        """Creates a new Palette object. The 'colors' argument may be
+        either a list of (r,g,b) tuples or an RGBRGBRGB... string/bytes.
+        'tran_index' specifies the index in the palette where the
+        transparent color should be placed. Note that this is only used
+        when saving images, and thus doesn't affect color lookups.
+        'tran_color' is the color to use for transparency."""
+
+        colors = colors or default_colors
+        tran_index = tran_index or default_tran_index
+        tran_color = tran_color or default_tran_color
+
+        if isinstance(colors, str):
+            colors = colors.encode('latin-1')
+
+        if isinstance(colors, list):
+            self.colors = colors[:]
+        elif isinstance(colors, bytes):
+            self.colors = [unpack('BBB', colors[i:i+3]) for i in range(0,768,3)]
+        else:
+            raise TypeError("Argument 'colors' must be list or string or bytes")
+
+        # Doom graphics don't actually use indices for transparency; the
+        # following data is only used when converting between image formats.
+        self.tran_index = tran_index
+        self.tran_color = tran_color
+        self.make_bytes()
+        self.make_grays()
+
+        # Memoizing color translations can speed up RGB-to-palette
+        # conversions significantly, in particular when converting
+        # lots of graphics in one session. See docstring for build_lut
+        # below for description of what bright_lut does.
+        self.memo = {}
+        self.bright_lut = []
+        self.reset_memo()
+
+    def make_bytes(self):
+        """Create/update 'bytes' and 'save_bytes' from the current set of
+        colors and the 'tran_index' and 'tran_color' fields."""
+        self.bytes = bytes().join([pack('BBB', *rgb) for rgb in self.colors])
+        self.save_bytes = \
+            self.bytes[:self.tran_index*3] + \
+            pack('BBB', *self.tran_color) + \
+            self.bytes[(self.tran_index+1)*3:]
+
+    def make_grays(self):
+        """Create 'grays' table containing the indices of all grays
+        in the current set of colors."""
+        self.grays = [i for i, rgb in enumerate(self.colors) \
+            if (rgb[0]==rgb[1]==rgb[2])]
+
+    def reset_memo(self):
+        """Clear the memo table (but (re)add the palette's colors)"""
+        self.memo = {}
+        for i in range(len(self.colors)):
+            if i != self.tran_index:
+                self.memo[self.colors[i]] = i
+
+    def build_lut(self, distance=16):
+        """Build 256-entry LUT for looking up colors in the palette
+        close to a given brightness (range 0-255). Each entry is a
+        list of indices. No position is empty; in the worst case,
+        the closest gray can be used.
+
+        The 'distance' parameter defines what "close" is, and should
+        be an integer 0-256. Lower distance means faster lookups,
+        but worse precision.
+
+        A good value for Doom is 10. Anything over 32 only wastes time.
+        """
+        self.bright_lut = []
+        assert 0 <= distance <= 256
+        for level in range(256):
+            candidates = []
+            for j, rgb in enumerate(self.colors):
+                if abs(level - (sum(rgb) // 3)) < distance:
+                    candidates.append(j)
+            # Make sure each entry contains at least one gray
+            # color that can be relied on in the worst case
+            best_d = 256
+            best_i = 0
+            for gray_index in self.grays:
+                r, g, b = self.colors[gray_index]
+                dist = abs(r - level)
+                if dist < best_d:
+                    best_i = gray_index
+                    if dist == 0:
+                        break
+                    best_d = dist
+            if best_i not in candidates:
+                candidates.append(best_i)
+            self.bright_lut.append(candidates)
+
+    def match(self, color):
+        """Find the closest match in the palette for a color.
+        Takes an (r,g,b) tuple as argument and returns a palette index."""
+        if color == self.tran_color:
+            return self.tran_index
+        if color in self.memo:
+            return self.memo[color]
+        if len(self.bright_lut) == 0:
+            self.build_lut()
+        best_dist = 262144
+        best_i = 0
+        ar, ag, ab = color
+        candidates = self.bright_lut[int(sum(color)) // 3]
+        for i in candidates:
+            br, bg, bb = self.colors[i]
+            dr = ar-br
+            dg = ag-bg
+            db = ab-bb
+            dist = dr*dr + dg*dg + db*db
+            if dist < best_dist:
+                if dist == 0:
+                    return i
+                best_dist = dist
+                best_i = i
+        self.memo[color] = best_i
+        return best_i
+
+    def blend(self, color, intensity=0.5):
+        """Blend the entire palette against a color (given as an RGB triple).
+        Intensity must be a floating-point number in the range 0-1."""
+        assert 0.0 <= intensity <= 1.0
+        nr = color[0] * intensity
+        ng = color[1] * intensity
+        nb = color[2] * intensity
+        remain = 1.0 - intensity
+        for i in range(len(self.colors)):
+            ar, ag, ab = self.colors[i]
+            self.colors[i] = (int(ar*remain + nr),
+                              int(ag*remain + ng),
+                              int(ab*remain + nb))
+        self.make_bytes()
+        self.make_grays()
+        self.reset_memo()
+        self.bright_lut = []
+
+# Colors of the Doom palette, used by default
+default_colors = b"\
+\x00\x00\x00\x1f\x17\x0b\x17\x0f\x07\x4b\x4b\x4b\xff\xff\xff\x1b\
+\x1b\x1b\x13\x13\x13\x0b\x0b\x0b\x07\x07\x07\x2f\x37\x1f\x23\x2b\
+\x0f\x17\x1f\x07\x0f\x17\x00\x4f\x3b\x2b\x47\x33\x23\x3f\x2b\x1b\
+\xff\xb7\xb7\xf7\xab\xab\xf3\xa3\xa3\xeb\x97\x97\xe7\x8f\x8f\xdf\
+\x87\x87\xdb\x7b\x7b\xd3\x73\x73\xcb\x6b\x6b\xc7\x63\x63\xbf\x5b\
+\x5b\xbb\x57\x57\xb3\x4f\x4f\xaf\x47\x47\xa7\x3f\x3f\xa3\x3b\x3b\
+\x9b\x33\x33\x97\x2f\x2f\x8f\x2b\x2b\x8b\x23\x23\x83\x1f\x1f\x7f\
+\x1b\x1b\x77\x17\x17\x73\x13\x13\x6b\x0f\x0f\x67\x0b\x0b\x5f\x07\
+\x07\x5b\x07\x07\x53\x07\x07\x4f\x00\x00\x47\x00\x00\x43\x00\x00\
+\xff\xeb\xdf\xff\xe3\xd3\xff\xdb\xc7\xff\xd3\xbb\xff\xcf\xb3\xff\
+\xc7\xa7\xff\xbf\x9b\xff\xbb\x93\xff\xb3\x83\xf7\xab\x7b\xef\xa3\
+\x73\xe7\x9b\x6b\xdf\x93\x63\xd7\x8b\x5b\xcf\x83\x53\xcb\x7f\x4f\
+\xbf\x7b\x4b\xb3\x73\x47\xab\x6f\x43\xa3\x6b\x3f\x9b\x63\x3b\x8f\
+\x5f\x37\x87\x57\x33\x7f\x53\x2f\x77\x4f\x2b\x6b\x47\x27\x5f\x43\
+\x23\x53\x3f\x1f\x4b\x37\x1b\x3f\x2f\x17\x33\x2b\x13\x2b\x23\x0f\
+\xef\xef\xef\xe7\xe7\xe7\xdf\xdf\xdf\xdb\xdb\xdb\xd3\xd3\xd3\xcb\
+\xcb\xcb\xc7\xc7\xc7\xbf\xbf\xbf\xb7\xb7\xb7\xb3\xb3\xb3\xab\xab\
+\xab\xa7\xa7\xa7\x9f\x9f\x9f\x97\x97\x97\x93\x93\x93\x8b\x8b\x8b\
+\x83\x83\x83\x7f\x7f\x7f\x77\x77\x77\x6f\x6f\x6f\x6b\x6b\x6b\x63\
+\x63\x63\x5b\x5b\x5b\x57\x57\x57\x4f\x4f\x4f\x47\x47\x47\x43\x43\
+\x43\x3b\x3b\x3b\x37\x37\x37\x2f\x2f\x2f\x27\x27\x27\x23\x23\x23\
+\x77\xff\x6f\x6f\xef\x67\x67\xdf\x5f\x5f\xcf\x57\x5b\xbf\x4f\x53\
+\xaf\x47\x4b\x9f\x3f\x43\x93\x37\x3f\x83\x2f\x37\x73\x2b\x2f\x63\
+\x23\x27\x53\x1b\x1f\x43\x17\x17\x33\x0f\x13\x23\x0b\x0b\x17\x07\
+\xbf\xa7\x8f\xb7\x9f\x87\xaf\x97\x7f\xa7\x8f\x77\x9f\x87\x6f\x9b\
+\x7f\x6b\x93\x7b\x63\x8b\x73\x5b\x83\x6b\x57\x7b\x63\x4f\x77\x5f\
+\x4b\x6f\x57\x43\x67\x53\x3f\x5f\x4b\x37\x57\x43\x33\x53\x3f\x2f\
+\x9f\x83\x63\x8f\x77\x53\x83\x6b\x4b\x77\x5f\x3f\x67\x53\x33\x5b\
+\x47\x2b\x4f\x3b\x23\x43\x33\x1b\x7b\x7f\x63\x6f\x73\x57\x67\x6b\
+\x4f\x5b\x63\x47\x53\x57\x3b\x47\x4f\x33\x3f\x47\x2b\x37\x3f\x27\
+\xff\xff\x73\xeb\xdb\x57\xd7\xbb\x43\xc3\x9b\x2f\xaf\x7b\x1f\x9b\
+\x5b\x13\x87\x43\x07\x73\x2b\x00\xff\xff\xff\xff\xdb\xdb\xff\xbb\
+\xbb\xff\x9b\x9b\xff\x7b\x7b\xff\x5f\x5f\xff\x3f\x3f\xff\x1f\x1f\
+\xff\x00\x00\xef\x00\x00\xe3\x00\x00\xd7\x00\x00\xcb\x00\x00\xbf\
+\x00\x00\xb3\x00\x00\xa7\x00\x00\x9b\x00\x00\x8b\x00\x00\x7f\x00\
+\x00\x73\x00\x00\x67\x00\x00\x5b\x00\x00\x4f\x00\x00\x43\x00\x00\
+\xe7\xe7\xff\xc7\xc7\xff\xab\xab\xff\x8f\x8f\xff\x73\x73\xff\x53\
+\x53\xff\x37\x37\xff\x1b\x1b\xff\x00\x00\xff\x00\x00\xe3\x00\x00\
+\xcb\x00\x00\xb3\x00\x00\x9b\x00\x00\x83\x00\x00\x6b\x00\x00\x53\
+\xff\xff\xff\xff\xeb\xdb\xff\xd7\xbb\xff\xc7\x9b\xff\xb3\x7b\xff\
+\xa3\x5b\xff\x8f\x3b\xff\x7f\x1b\xf3\x73\x17\xeb\x6f\x0f\xdf\x67\
+\x0f\xd7\x5f\x0b\xcb\x57\x07\xc3\x4f\x00\xb7\x47\x00\xaf\x43\x00\
+\xff\xff\xff\xff\xff\xd7\xff\xff\xb3\xff\xff\x8f\xff\xff\x6b\xff\
+\xff\x47\xff\xff\x23\xff\xff\x00\xa7\x3f\x00\x9f\x37\x00\x93\x2f\
+\x00\x87\x23\x00\x4f\x3b\x27\x43\x2f\x1b\x37\x23\x13\x2f\x1b\x0b\
+\x00\x00\x53\x00\x00\x47\x00\x00\x3b\x00\x00\x2f\x00\x00\x23\x00\
+\x00\x17\x00\x00\x0b\x00\x00\x00\xff\x9f\x43\xff\xe7\x4b\xff\x7b\
+\xff\xff\x00\xff\xcf\x00\xcf\x9f\x00\x9b\x6f\x00\x6b\xa7\x6b\x6b\
+"
+
+# Defaults for image transparency
+default_tran_index = 247
+default_tran_color = (255, 0, 255)
+
+# Default palette object, using the default values
+default = Palette()
```

### Comparing `omgifol-0.5.0/omg/playpal.py` & `omgifol-0.5.1/omg/playpal.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-from omg.lump import Lump
-from omg.util import *
-import omg.palette
-
-class Playpal:
-    """An editor for Doom's PLAYPAL lump. The PLAYPAL lump contains 14
-    palettes: the game's base palette, the palettes used when the
-    player is in pain or uses the berserk powerup, the palettes used
-    when the player picks up an item, and the palette used when the
-    player is wearing the radiation suit.
-
-    The palettes are located in a member list called 'palettes'. Each
-    palette is a Palette instance."""
-
-    def __init__(self, source=None):
-        """Construct a new EditPlaypal object. Source may be a PLAYPAL
-        lump or a Palette instance. If a Palette instance, all 14
-        palettes are set to copies of it. If no source is specified,
-        the default palette is used."""
-        if isinstance(source, Lump):
-            self.from_lump(source)
-        else:
-            self.set_base(source)
-
-    def build_defaults(self):
-        """Build all 13 extra palettes, using default values (red for
-        pain, yellow for item pickups, green for the radiation suit).
-        The values used here are not exactly the same as those in
-        Doom's PLAYPAL, but decent approximations."""
-        self.build_pain()
-        self.build_item()
-        self.build_suit()
-
-    def build_suit (self, color=(0,255,0), intensity=0.2):
-        """Set the color and intensity for the radiation suit palette."""
-        self.palettes[13].blend(color, intensity)
-
-    def build_pain (self, color=(255,0,0), minintensity=0.1, maxintensity=0.8):
-        """Set the color and intensities for the player-in-pain (also
-        used by the berserk powerup) palettes."""
-        step = (maxintensity - minintensity) / 8.0
-        for i in range(8):
-            self.palettes[i+1].blend(color, step*i + minintensity)
-
-    def build_item (self, color=(255,255,64), minintensity=0.1, maxintensity=0.3):
-        """Set color and intensity for the item pick-up palettes."""
-        step = (maxintensity - minintensity) / 3.0
-        for i in range(3):
-            self.palettes[i+10].blend(color, step * i + minintensity)
-
-    def from_lump(self, lump):
-        """Load data from a PLAYPAL lump."""
-        self.palettes = [omg.palette.Palette(lump.data[i*768:(i+1)*768], 0, 0)
-            for i in range(14)]
-
-    def to_lump(self):
-        """Compile to a Doom-ready PLAYPAL Lump."""
-        return Lump(join([p.bytes for p in self.palettes]))
-
-    def set_base(self, palette=None):
-        """Set all palettes to copies of a given Palette object. If the
-        palette parameter is not provided, the default palette is used."""
-        palette = palette or omg.palette.default
-        self.palettes = [deepcopy(palette) for i in range(14)]
+from omg.lump import Lump
+from omg.util import *
+import omg.palette
+
+class Playpal:
+    """An editor for Doom's PLAYPAL lump. The PLAYPAL lump contains 14
+    palettes: the game's base palette, the palettes used when the
+    player is in pain or uses the berserk powerup, the palettes used
+    when the player picks up an item, and the palette used when the
+    player is wearing the radiation suit.
+
+    The palettes are located in a member list called 'palettes'. Each
+    palette is a Palette instance."""
+
+    def __init__(self, source=None):
+        """Construct a new EditPlaypal object. Source may be a PLAYPAL
+        lump or a Palette instance. If a Palette instance, all 14
+        palettes are set to copies of it. If no source is specified,
+        the default palette is used."""
+        if isinstance(source, Lump):
+            self.from_lump(source)
+        else:
+            self.set_base(source)
+
+    def build_defaults(self):
+        """Build all 13 extra palettes, using default values (red for
+        pain, yellow for item pickups, green for the radiation suit).
+        The values used here are not exactly the same as those in
+        Doom's PLAYPAL, but decent approximations."""
+        self.build_pain()
+        self.build_item()
+        self.build_suit()
+
+    def build_suit (self, color=(0,255,0), intensity=0.2):
+        """Set the color and intensity for the radiation suit palette."""
+        self.palettes[13].blend(color, intensity)
+
+    def build_pain (self, color=(255,0,0), minintensity=0.1, maxintensity=0.8):
+        """Set the color and intensities for the player-in-pain (also
+        used by the berserk powerup) palettes."""
+        step = (maxintensity - minintensity) / 8.0
+        for i in range(8):
+            self.palettes[i+1].blend(color, step*i + minintensity)
+
+    def build_item (self, color=(255,255,64), minintensity=0.1, maxintensity=0.3):
+        """Set color and intensity for the item pick-up palettes."""
+        step = (maxintensity - minintensity) / 3.0
+        for i in range(3):
+            self.palettes[i+10].blend(color, step * i + minintensity)
+
+    def from_lump(self, lump):
+        """Load data from a PLAYPAL lump."""
+        self.palettes = [omg.palette.Palette(lump.data[i*768:(i+1)*768], 0, 0)
+            for i in range(14)]
+
+    def to_lump(self):
+        """Compile to a Doom-ready PLAYPAL Lump."""
+        return Lump(join([p.bytes for p in self.palettes]))
+
+    def set_base(self, palette=None):
+        """Set all palettes to copies of a given Palette object. If the
+        palette parameter is not provided, the default palette is used."""
+        palette = palette or omg.palette.default
+        self.palettes = [deepcopy(palette) for i in range(14)]
```

### Comparing `omgifol-0.5.0/omg/udmf.py` & `omgifol-0.5.1/omg/udmf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,495 +1,496 @@
-import re
-from omg.mapedit import MapEditor, Linedef
-from omg.wad import NameGroup
-from omg.lump import Lump
-
-class UBlock:
-    @staticmethod
-    def serialize(value):
-        if isinstance(value, bool):
-            return '{0}'.format(value).lower()
-        if isinstance(value, (float, int)):
-            return '{0}'.format(value)
-        if isinstance(value, str):
-            return '"{0}"'.format(re.sub(r'"', '\\"', re.sub(r'\\', '\\\\\\\\', value)))
-        raise TypeError
-
-    defaults = {}
-
-    def __init__(self, **kwargs):
-        self.__dict__.update(type(self).defaults)
-        self.__dict__.update(kwargs)
-    def __getattr__(self, name):
-        return self.__dict__.get(name, None)
-    def __setattr__(self, name, value):
-        self.__dict__[name] = value
-    def __eq__(self, other):
-        return isinstance(other, UBlock) and self.__dict__ == other.__dict__
-    def to_textmap(self, fallback = None):
-        out = '{\n'
-        for key, value in self.__dict__.items():
-            if value is None:
-                continue
-            if not isinstance(value, (float, int, bool, str)):
-                if fallback:
-                    value = fallback(value)
-                else:
-                    raise TypeError
-            key = re.sub(r'^([0-9])', r'_\1', re.sub(r'[^A-Za-z0-9_]', '_', key))
-            if key in type(self).defaults and value == type(self).defaults[key]:
-                continue
-            if isinstance(value, bool) and not value:
-                continue
-            out += '{0}={1};\n'.format(key, UBlock.serialize(value))
-
-        out += '}\n'
-        return out
-
-class UParser:
-   #IDENTIFIER_RE    = re.compile(rb'[A-Za-z_]+[A-Za-z0-9_]*')
-    IDENTIFIER_RE    = re.compile(rb'[A-Za-z0-9_]+') # allow leading digits per UDMF 1.0 (will be changed upon saving)
-    INTEGER_RE       = re.compile(rb'([+-]?[1-9]+[0-9]*)|(0[0-7]+)|(0x[0-9A-Fa-f]+)|(0)')
-    FLOAT_RE         = re.compile(rb'[+-]?[0-9]+\.[0-9]*([eE][+-]?[0-9]+)?')
-    QUOTED_STRING_RE = re.compile(rb'"([^"\\]*(\\.[^"\\]*)*)"')
-    KEYWORD_RE       = re.compile(rb'[^{}();"\'\n\t ]+')
-    WHITESPACE_RE    = re.compile(rb'(\s|(\n|^)//[^\n]+|/\*(\*(?!\/)|[^*])*\*/)+')
-    def __init__(self, blocktypes):
-        self.blocktypes = blocktypes
-        self.src = None
-        self.ptr = 0
-        self.line = 1
-        self.match = None
-
-    def skip_ws(self):
-        while True:
-            ws = UParser.WHITESPACE_RE.match(self.src[self.ptr:])
-            if ws:
-                self.line += len([x for x in ws[0] if chr(x) == '\n'])
-                self.ptr += ws.end()
-            else:
-                break
-
-    def peek(self, expr):
-        if isinstance(expr, re.Pattern):
-            return expr.match(self.src[self.ptr:])
-        return re.match(expr, self.src[self.ptr:])
-
-    def error_token(self):
-        if self.ptr == len(self.src):
-            return 'EOF'
-        else:
-            got = UParser.WHITESPACE_RE.search(self.src[self.ptr:])
-            if got:
-                got = self.src[self.ptr:self.ptr+got.start()]
-            else:
-                got = self.src[self.ptr:]
-            return "'{0}'".format(got.tobytes().decode())
-
-    def accept(self, expr):
-        match = self.peek(expr)
-        if match:
-            self.match = match
-            self.line += len([x for x in match[0] if chr(x) == '\n'])
-            self.ptr += match.end()
-            self.skip_ws()
-        return match
-
-    def expect(self, expr):
-        match = self.accept(expr)
-        if match:
-            return match
-        raise Exception("line {0}: expected '{1}', got {2}".format(self.line, expr.decode(), self.error_token()))
-
-    def parse(self, src):
-        self.src = memoryview(src)
-        self.ptr = 0
-        self.line = 1
-        toplevel = {}
-        blocks = {}
-        self.skip_ws()
-        while self.ptr < len(self.src):
-            name = self.identifier().lower()
-            if self.accept(b'='):
-                value = self.value()
-                self.expect(rb';')
-                toplevel[name] = value
-            elif self.accept(b'{'):
-                fields = self.expr_list()
-                self.expect(rb'}')
-                blockclass = self.blocktypes.get(name, UBlock)
-                group = blocks.setdefault(name, [])
-                group.append(blockclass(**fields))
-        return toplevel, blocks
-
-    def expr_list(self):
-        fields = {}
-        while self.peek(UParser.IDENTIFIER_RE):
-            key, value = self.assignment_expr()
-            fields[key] = value
-        return fields
-
-    def assignment_expr(self):
-        key = self.identifier().lower()
-        self.expect(rb'=')
-        value = self.value()
-        self.expect(rb';')
-        return key, value
-
-    def identifier(self):
-        if self.accept(UParser.IDENTIFIER_RE):
-            return self.match[0].decode()
-        raise Exception("line {0}: expected identifier, got {1}".format(self.line, self.error_token()))
-
-    def value(self):
-        if self.accept(UParser.FLOAT_RE):
-            return float(self.match[0])
-        if self.accept(UParser.INTEGER_RE):
-            if self.match[1]:
-                return int(self.match[0], 10)
-            if self.match[2]:
-                return int(self.match[0], 8)
-            if self.match[3]:
-                return int(self.match[0], 16)
-            if self.match[4]:
-                return 0
-        if self.accept(UParser.QUOTED_STRING_RE):
-            return self.match[1].decode()
-        if self.accept(UParser.KEYWORD_RE):
-            if not self.match[0] in (b'true', b'false'):
-                raise Exception("line {0}: expected bool, got '{1}'".format(self.line, self.match[0].decode()))
-            return self.match[0] == b'true'
-        raise Exception("line {0}: expected integer, float, string, or bool, got {1}".format(self.line, self.error_token()))
-
-class UVertex(UBlock):
-    storage = 'vertexes'
-    def __init__(self, x=0.0, y=0.0, **kwargs):
-        self.x = x
-        self.y = y
-        super().__init__(**kwargs)
-
-class USidedef(UBlock):
-    storage = 'sidedefs'
-    defaults = {'texturetop': '-', 'texturebottom': '-', 'texturemiddle': '-',
-            'offsetx': 0, 'offsety': 0}
-    def __init__(self, sector=None, **kwargs):
-        self.sector = sector
-        super().__init__(**kwargs)
-
-class ULinedef(UBlock):
-    storage = 'linedefs'
-    defaults = {
-            'special': 0, 'arg0': 0, 'arg1': 0, 'arg2': 0, 'arg3': 0, 'arg4': 0,
-            'sideback': -1, 'id': -1}
-    flags = {'_Base':[
-        'blocking','blockmonsters','twosided',
-        'dontpegtop','dontpegbottom','secret',
-        'blocksound','dontdraw','mapped',]}
-    flags['Doom'] = flags['_Base'] + ['passuse']
-    flags['Heretic'] = flags['_Base']
-    flags['Hexen'] = flags['_Base'] + [
-            'repeatspecial',None,None,None,
-            'monsteractivate',None,'blockeverything']
-    flags['Strife'] = flags['_Base'] + [
-            'jumpover','blockfloating',
-            'translucent','transparent']
-    flags['ZDoom'] = flags['Hexen']
-    flags['ZDoom'][14] = 'blockplayers'
-    flags['Eternity'] = flags['_Base'] + ['midtex3d']
-
-    moreflags_hexen = [
-            'zoneboundary','jumpover','blockfloaters',
-            'clipmidtex','wrapmidtex','midtex3d',
-            'checkswitchrange','firstsideonly']
-    triggers_hexen = [
-            'playercross','playeruse','monstercross','impact',
-            'playerpush','missilecross','blocking']
-
-    def __init__(self, v1=None, v2=None, sidefront=None, **kwargs):
-        self.v1 = v1
-        self.v2 = v2
-        self.sidefront = sidefront
-        super().__init__(**kwargs)
-
-class USector(UBlock):
-    storage = 'sectors'
-    defaults = {
-      'heightfloor': 0,
-      'heightceiling': 0,
-      'lightlevel': 160,
-      'special': 0,
-      'id': 0
-      }
-    def __init__(self, texturefloor='-', textureceiling='-', **kwargs):
-        self.texturefloor = texturefloor
-        self.textureceiling = textureceiling
-        super().__init__(**kwargs)
-
-class UThing(UBlock):
-    storage = 'things'
-    defaults = {
-            'id': 0, 'height': 0, 'angle': 0,
-            'special': 0, 'arg0': 0, 'arg1': 0, 'arg2': 0, 'arg3': 0, 'arg4': 0}
-    flags = {'_Base':
-            ['skill1,skill2','skill3','skill4,skill5']}
-    flags['Doom'] = flags['_Base'] + [
-            'ambush','!single','!dm','!coop','friend']
-    flags['Heretic'] = flags['_Base'] + [
-            'ambush','!single']
-    flags['Hexen'] = flags['_Base'] + [
-            'ambush','dormant',
-            'class1','class2','class3',
-            'single','coop','dm']
-    flags['Strife'] = flags['_Base'] + [
-            'standing','!single','ambush',
-            'strifeally',None,'translucent','invisible']
-    flags['ZDoom'] = flags['Hexen'] + [
-            'translucent','invisible','strifeally','standing']
-
-    def __init__(self, x=0.0, y=0.0, ednum=0, **kwargs):
-        self.x = x
-        self.y = y
-        self.type = ednum
-        super().__init__(**kwargs)
-
-udmf_types = {
-        'thing': UThing,
-        'vertex': UVertex,
-        'sidedef': USidedef,
-        'linedef': ULinedef,
-        'sector': USector}
-
-udmf_namespaces = ['Doom', 'Heretic', 'Hexen', 'Strife', 'ZDoom']
-
-class UMapEditor:
-    """UDMF map editor.
-
-    Data members:
-        vertexes      List containing UVertex objects
-        sidedefs      List containing USidedef objects
-        linedefs      List containing ULinedef objects
-        sectors       List containing USector objects
-        things        List containing UThing objects
-        behavior      Lump object containing compiled ACS scripts
-        scripts       Lump object containing ACS script source
-        namespace     Map's UDMF namespace (see omg.udmf_namespaces for recognized values)
-        """
-
-    def __init__(self, lumpgroup=None, namespace=None):
-        """Create new, optionally from a lump group.
-
-        lumpgroup can be either a UDMF map or a classic Doom or ZDoom/Hexen map.
-        Maps using the old format will be converted to UDMF automatically.
-
-        If namespace is not specified, it will use the value stored in lumpgroup,
-        if available."""
-        self.vertexes = []
-        self.sidedefs = []
-        self.linedefs = []
-        self.sectors = []
-        self.things = []
-        self.scripts = None
-        self.behavior = None
-        self.namespace = namespace
-
-        if lumpgroup is not None:
-            self.from_lump(lumpgroup, namespace)
-
-    def from_lump(self, lumpgroup, namespace=None):
-        """Load entries from a lump group.
-
-        lumpgroup can be either a UDMF map or a classic Doom or ZDoom/Hexen map.
-        Maps using the old format will be converted to UDMF automatically.
-
-        If namespace is not specified, it will use the value stored in lumpgroup,
-        if available."""
-        if 'TEXTMAP' not in lumpgroup:
-            self.from_oldformat(lumpgroup, namespace)
-            return
-
-        parser = UParser(udmf_types)
-        toplevel, blocks = parser.parse(lumpgroup["TEXTMAP"].data)
-        for (t, cls) in udmf_types.items():
-            setattr(self, cls.storage, blocks[t] if t in blocks else [])
-            if namespace is not None:
-                self.namespace = namespace
-            elif 'namespace' in toplevel:
-                self.namespace = toplevel['namespace']
-            else:
-                self.namespace = None
-
-        if 'BEHAVIOR' in lumpgroup:
-            self.behavior = lumpgroup['BEHAVIOR']
-        if 'SCRIPTS' in lumpgroup:
-            self.scripts = lumpgroup['SCRIPTS']
-
-    def from_oldformat(self, lumpgroup, namespace=None):
-        """Import a classic format (Doom or ZDoom/Hexen) map.
-
-        For ZDoom maps, deprecated line specials (such as Line_SetIdentification) will
-        automatically be translated to the UDMF equivalent.
-
-        If namespace is not specified, it will be given a default value based on the map's
-        original format (vanilla or ZDoom/Hexen)."""
-        m = MapEditor(lumpgroup)
-        self.vertexes = []
-        self.sidedefs = []
-        self.linedefs = []
-        self.sectors = []
-        self.things = []
-        self.namespace = namespace
-        
-        hexencompat = 'BEHAVIOR' in lumpgroup
-        if namespace not in udmf_namespaces:
-            namespace = 'ZDoom' if hexencompat else udmf_namespaces[0]
-        if not self.namespace:
-            self.namespace = namespace
-
-        if hexencompat:
-            try:
-                self.behavior = m.behavior
-                self.scripts = m.scripts
-            except AttributeError:
-                pass
-
-        for thing in m.things:
-            block = UThing(float(thing.x), float(thing.y), thing.type)
-            self.things.append(block)
-            
-            if thing.angle != 0:
-                block.angle = thing.angle
-
-            for f in range(len(UThing.flags[namespace])):
-                if not UThing.flags[namespace][f]:
-                    continue
-                for flag in UThing.flags[namespace][f].split(','):
-                    if flag[0] != '!':
-                        setattr(block, flag, bool(thing.flags & (1 << f)))
-                    else:
-                        setattr(block, flag[1:], not bool(thing.flags & (1 << f)))
-
-            if hexencompat:
-                block.id = thing.tid
-                block.height = float(thing.height)
-                block.special = thing.action
-                for i in range(5):
-                    key = 'arg{0}'.format(i)
-                    setattr(block, key, getattr(thing, key))
-
-        for linedef in m.linedefs:
-            block = ULinedef(linedef.vx_a, linedef.vx_b, linedef.front)
-            self.linedefs.append(block)
-
-            if linedef.back != Linedef.NONE:
-                block.sideback = linedef.back
-            
-            for f in range(len(ULinedef.flags[namespace])):
-                flag = ULinedef.flags[namespace][f]
-                if flag:
-                    setattr(block, flag, bool(linedef.flags & (1 << f)))
-                    
-            if hexencompat:
-                if linedef.action == 121: # Line_SetIdentification
-                    block.id = linedef.arg0 + linedef.arg4 * 256
-                    for f in range(len(ULinedef.moreflags_hexen)):
-                        setattr(block, ULinedef.moreflags_hexen[f], bool(linedef.arg1 & (1 << f)))
-                elif linedef.action:
-                    block.special = linedef.action
-                    for i in range(5):
-                        key = 'arg{0}'.format(i)
-                        setattr(block, key, getattr(linedef, key))
-                    
-                    trigger = ((linedef.flags & 0x1c00) >> 10)
-                    if trigger < len(ULinedef.triggers_hexen):
-                        setattr(block, ULinedef.triggers_hexen[trigger], True)
-                    
-                    # handle line specials that set a line ID, extended flags, etc. based on the zdoom udmf spec
-                    if linedef.action == 1: # Polyobj_StartLine
-                        block.id = linedef.arg3
-                        block.arg3 = 0
-                    elif linedef.action == 5: # Polyobj_ExplicitLine
-                        block.id = linedef.arg4
-                        block.arg4 = 0
-                    elif linedef.action == 160: # Sector_Set3dFloor
-                        if linedef.arg1 & 8:
-                            block.id = linedef.arg4
-                            block.arg1 &= ~8
-                        else:
-                            block.arg0 += linedef.arg4 * 256
-                        block.arg4 = 0
-                    elif linedef.action == 181: # Plane_Align
-                        block.id = linedef.arg2
-                        block.arg2 = 0
-                    elif linedef.action == 208: # TranslucentLine
-                        block.id = linedef.arg0 # preserve arg0 according to spec
-                        for f in range(len(ULinedef.moreflags_hexen)):
-                            setattr(block, ULinedef.moreflags_hexen[f], bool(linedef.arg3 & (1 << f)))
-                        block.arg3 = 0
-                    elif linedef.action == 215: # Teleport_Line
-                        block.id = linedef.arg0
-                        block.arg0 = 0
-                    elif linedef.action == 222: # Scroll_Texture_Model
-                        block.id = linedef.arg0 # preserve arg0 according to spec
-            else:
-                block.special = linedef.action
-                block.id = block.arg0 = linedef.tag
-
-        for sidedef in m.sidedefs:
-            block = USidedef(sidedef.sector)
-            self.sidedefs.append(block)
-
-            block.offsetx = sidedef.off_x
-            block.offsety = sidedef.off_y
-            block.texturetop = sidedef.tx_up
-            block.texturebottom = sidedef.tx_low
-            block.texturemiddle = sidedef.tx_mid
-
-        for vertex in m.vertexes:
-            block = UVertex(float(vertex.x), float(vertex.y))
-            self.vertexes.append(block)
-
-        for sector in m.sectors:
-            block = USector(sector.tx_floor, sector.tx_ceil)
-            self.sectors.append(block)
-
-            block.heightfloor = sector.z_floor
-            block.heightceiling = sector.z_ceil
-            block.lightlevel = sector.light
-            block.special = sector.type
-            block.id = sector.tag
-
-    def to_lumps(self):
-        m = NameGroup()
-        m['_HEADER_'] = Lump()
-        m['TEXTMAP'] = Lump(str.encode(self.to_textmap()))
-        if self.behavior:
-            m['BEHAVIOR'] = self.behavior
-        if self.scripts:
-            m['SCRIPTS'] = self.scripts
-        m['ENDMAP'] = Lump()
-        return m
-
-    def to_textmap(self):
-        fallback = lambda *args: self.serialize_field(*args)
-        out = 'namespace="{0}";\n'.format(self.namespace)
-        for thing in self.things:
-            out += 'thing ' + thing.to_textmap(fallback)
-        for vertex in self.vertexes:
-            out += 'vertex ' + vertex.to_textmap(fallback)
-        for sidedef in self.sidedefs:
-            out += 'sidedef ' + sidedef.to_textmap(fallback)
-        for linedef in self.linedefs:
-            out += 'linedef ' + linedef.to_textmap(fallback)
-        for sector in self.sectors:
-            out += 'sector ' + sector.to_textmap(fallback)
-        return out
-    def serialize_field(self, value):
-        if isinstance(value, UVertex):
-            return self.vertexes.index(value)
-        if isinstance(value, USidedef):
-            return self.sidedefs.index(value)
-        if isinstance(value, ULinedef):
-            return self.linedefs.index(value)
-        if isinstance(value, USector):
-            return self.sectors.index(value)
-        if isinstance(value, UThing):
-            return self.things.index(value)
+import re
+from omg.mapedit import MapEditor, Linedef
+from omg.wad import NameGroup
+from omg.lump import Lump
+
+class UBlock:
+    @staticmethod
+    def serialize(value):
+        if isinstance(value, bool):
+            return '{0}'.format(value).lower()
+        if isinstance(value, (float, int)):
+            return '{0}'.format(value)
+        if isinstance(value, str):
+            return '"{0}"'.format(re.sub(r'"', '\\"', re.sub(r'\\', '\\\\\\\\', value)))
+        raise TypeError
+
+    defaults = {}
+
+    def __init__(self, **kwargs):
+        self.__dict__.update(type(self).defaults)
+        self.__dict__.update(kwargs)
+    def __getattr__(self, name):
+        return self.__dict__.get(name, None)
+    def __setattr__(self, name, value):
+        self.__dict__[name] = value
+    def __eq__(self, other):
+        return isinstance(other, UBlock) and self.__dict__ == other.__dict__
+    def to_textmap(self, fallback = None):
+        out = '{\n'
+        for key, value in self.__dict__.items():
+            if value is None:
+                continue
+            if not isinstance(value, (float, int, bool, str)):
+                if fallback:
+                    value = fallback(value)
+                else:
+                    raise TypeError
+            key = re.sub(r'^([0-9])', r'_\1', re.sub(r'[^A-Za-z0-9_]', '_', key))
+            if key in type(self).defaults and value == type(self).defaults[key]:
+                continue
+            if isinstance(value, bool) and not value:
+                continue
+            out += '{0}={1};\n'.format(key, UBlock.serialize(value))
+
+        out += '}\n'
+        return out
+
+class UParser:
+   #IDENTIFIER_RE    = re.compile(rb'[A-Za-z_]+[A-Za-z0-9_]*')
+    IDENTIFIER_RE    = re.compile(rb'[A-Za-z0-9_]+') # allow leading digits per UDMF 1.0 (will be changed upon saving)
+    INTEGER_RE       = re.compile(rb'([+-]?[1-9]+[0-9]*)|(0[0-7]+)|(0x[0-9A-Fa-f]+)|(0)')
+    FLOAT_RE         = re.compile(rb'[+-]?[0-9]+\.[0-9]*([eE][+-]?[0-9]+)?')
+    QUOTED_STRING_RE = re.compile(rb'"([^"\\]*(\\.[^"\\]*)*)"')
+    KEYWORD_RE       = re.compile(rb'[^{}();"\'\n\t ]+')
+    WHITESPACE_RE    = re.compile(rb'(\s|(\n|^)//[^\n]+|/\*(\*(?!\/)|[^*])*\*/)+')
+
+    def __init__(self, blocktypes):
+        self.blocktypes = blocktypes
+        self.src = None
+        self.ptr = 0
+        self.line = 1
+        self.match = None
+
+    def skip_ws(self):
+        while True:
+            ws = UParser.WHITESPACE_RE.match(self.src[self.ptr:])
+            if ws:
+                self.line += len([x for x in ws[0] if chr(x) == '\n'])
+                self.ptr += ws.end()
+            else:
+                break
+
+    def peek(self, expr):
+        if isinstance(expr, re.Pattern):
+            return expr.match(self.src[self.ptr:])
+        return re.match(expr, self.src[self.ptr:])
+
+    def error_token(self):
+        if self.ptr == len(self.src):
+            return 'EOF'
+        else:
+            got = UParser.WHITESPACE_RE.search(self.src[self.ptr:])
+            if got:
+                got = self.src[self.ptr:self.ptr+got.start()]
+            else:
+                got = self.src[self.ptr:]
+            return "'{0}'".format(got.tobytes().decode())
+
+    def accept(self, expr):
+        match = self.peek(expr)
+        if match:
+            self.match = match
+            self.line += len([x for x in match[0] if chr(x) == '\n'])
+            self.ptr += match.end()
+            self.skip_ws()
+        return match
+
+    def expect(self, expr):
+        match = self.accept(expr)
+        if match:
+            return match
+        raise Exception("line {0}: expected '{1}', got {2}".format(self.line, expr.decode(), self.error_token()))
+
+    def parse(self, src):
+        self.src = memoryview(src)
+        self.ptr = 0
+        self.line = 1
+        toplevel = {}
+        blocks = {}
+        self.skip_ws()
+        while self.ptr < len(self.src):
+            name = self.identifier().lower()
+            if self.accept(b'='):
+                value = self.value()
+                self.expect(rb';')
+                toplevel[name] = value
+            elif self.accept(b'{'):
+                fields = self.expr_list()
+                self.expect(rb'}')
+                blockclass = self.blocktypes.get(name, UBlock)
+                group = blocks.setdefault(name, [])
+                group.append(blockclass(**fields))
+        return toplevel, blocks
+
+    def expr_list(self):
+        fields = {}
+        while self.peek(UParser.IDENTIFIER_RE):
+            key, value = self.assignment_expr()
+            fields[key] = value
+        return fields
+
+    def assignment_expr(self):
+        key = self.identifier().lower()
+        self.expect(rb'=')
+        value = self.value()
+        self.expect(rb';')
+        return key, value
+
+    def identifier(self):
+        if self.accept(UParser.IDENTIFIER_RE):
+            return self.match[0].decode()
+        raise Exception("line {0}: expected identifier, got {1}".format(self.line, self.error_token()))
+
+    def value(self):
+        if self.accept(UParser.FLOAT_RE):
+            return float(self.match[0])
+        if self.accept(UParser.INTEGER_RE):
+            if self.match[1]:
+                return int(self.match[0], 10)
+            if self.match[2]:
+                return int(self.match[0], 8)
+            if self.match[3]:
+                return int(self.match[0], 16)
+            if self.match[4]:
+                return 0
+        if self.accept(UParser.QUOTED_STRING_RE):
+            return self.match[1].decode()
+        if self.accept(UParser.KEYWORD_RE):
+            if not self.match[0] in (b'true', b'false'):
+                raise Exception("line {0}: expected bool, got '{1}'".format(self.line, self.match[0].decode()))
+            return self.match[0] == b'true'
+        raise Exception("line {0}: expected integer, float, string, or bool, got {1}".format(self.line, self.error_token()))
+
+class UVertex(UBlock):
+    storage = 'vertexes'
+
+    def __init__(self, x=0.0, y=0.0, **kwargs):
+        self.x = x
+        self.y = y
+        super().__init__(**kwargs)
+
+class USidedef(UBlock):
+    storage = 'sidedefs'
+    defaults = {'texturetop': '-', 'texturebottom': '-', 'texturemiddle': '-',
+            'offsetx': 0, 'offsety': 0}
+
+    def __init__(self, sector=None, **kwargs):
+        self.sector = sector
+        super().__init__(**kwargs)
+
+class ULinedef(UBlock):
+    storage = 'linedefs'
+    defaults = {
+            'special': 0, 'arg0': 0, 'arg1': 0, 'arg2': 0, 'arg3': 0, 'arg4': 0,
+            'sideback': -1, 'id': -1}
+    flags = {'_Base': [
+            'blocking','blockmonsters','twosided',
+            'dontpegtop','dontpegbottom','secret',
+            'blocksound','dontdraw','mapped',]}
+    flags['Doom'] = flags['_Base'] + ['passuse']
+    flags['Heretic'] = flags['_Base']
+    flags['Hexen'] = flags['_Base'] + [
+            'repeatspecial',None,None,None,
+            'monsteractivate',None,'blockeverything']
+    flags['Strife'] = flags['_Base'] + [
+            'jumpover','blockfloating',
+            'translucent','transparent']
+    flags['ZDoom'] = flags['Hexen']
+    flags['ZDoom'][14] = 'blockplayers'
+    flags['Eternity'] = flags['_Base'] + ['midtex3d']
+
+    moreflags_hexen = [
+            'zoneboundary','jumpover','blockfloaters',
+            'clipmidtex','wrapmidtex','midtex3d',
+            'checkswitchrange','firstsideonly']
+    triggers_hexen = [
+            'playercross','playeruse','monstercross','impact',
+            'playerpush','missilecross','blocking']
+
+    def __init__(self, v1=None, v2=None, sidefront=None, **kwargs):
+        self.v1 = v1
+        self.v2 = v2
+        self.sidefront = sidefront
+        super().__init__(**kwargs)
+
+class USector(UBlock):
+    storage = 'sectors'
+    defaults = {
+      'heightfloor': 0, 'heightceiling': 0,
+      'lightlevel': 160, 'special': 0, 'id': 0}
+
+    def __init__(self, texturefloor='-', textureceiling='-', **kwargs):
+        self.texturefloor = texturefloor
+        self.textureceiling = textureceiling
+        super().__init__(**kwargs)
+
+class UThing(UBlock):
+    storage = 'things'
+    defaults = {
+            'id': 0, 'height': 0, 'angle': 0,
+            'special': 0, 'arg0': 0, 'arg1': 0, 'arg2': 0, 'arg3': 0, 'arg4': 0}
+    flags = {'_Base':
+            ['skill1,skill2','skill3','skill4,skill5']}
+    flags['Doom'] = flags['_Base'] + [
+            'ambush','!single','!dm','!coop','friend']
+    flags['Heretic'] = flags['_Base'] + [
+            'ambush','!single']
+    flags['Hexen'] = flags['_Base'] + [
+            'ambush','dormant',
+            'class1','class2','class3',
+            'single','coop','dm']
+    flags['Strife'] = flags['_Base'] + [
+            'standing','!single','ambush',
+            'strifeally',None,'translucent','invisible']
+    flags['ZDoom'] = flags['Hexen'] + [
+            'translucent','invisible','strifeally','standing']
+
+    def __init__(self, x=0.0, y=0.0, ednum=0, **kwargs):
+        self.x = x
+        self.y = y
+        self.type = ednum
+        super().__init__(**kwargs)
+
+udmf_types = {
+        'thing': UThing,
+        'vertex': UVertex,
+        'sidedef': USidedef,
+        'linedef': ULinedef,
+        'sector': USector}
+
+udmf_namespaces = ['Doom', 'Heretic', 'Hexen', 'Strife', 'ZDoom']
+
+class UMapEditor:
+    """UDMF map editor.
+
+    Data members:
+        vertexes      List containing UVertex objects
+        sidedefs      List containing USidedef objects
+        linedefs      List containing ULinedef objects
+        sectors       List containing USector objects
+        things        List containing UThing objects
+        behavior      Lump object containing compiled ACS scripts
+        scripts       Lump object containing ACS script source
+        namespace     Map's UDMF namespace (see omg.udmf_namespaces for recognized values)
+        """
+
+    def __init__(self, lumpgroup=None, namespace=None):
+        """Create new, optionally from a lump group.
+
+        lumpgroup can be either a UDMF map or a classic Doom or ZDoom/Hexen map.
+        Maps using the old format will be converted to UDMF automatically.
+
+        If namespace is not specified, it will use the value stored in lumpgroup,
+        if available."""
+        self.vertexes = []
+        self.sidedefs = []
+        self.linedefs = []
+        self.sectors = []
+        self.things = []
+        self.scripts = None
+        self.behavior = None
+        self.namespace = namespace
+
+        if lumpgroup is not None:
+            self.from_lump(lumpgroup, namespace)
+
+    def from_lump(self, lumpgroup, namespace=None):
+        """Load entries from a lump group.
+
+        lumpgroup can be either a UDMF map or a classic Doom or ZDoom/Hexen map.
+        Maps using the old format will be converted to UDMF automatically.
+
+        If namespace is not specified, it will use the value stored in lumpgroup,
+        if available."""
+        if 'TEXTMAP' not in lumpgroup:
+            self.from_oldformat(lumpgroup, namespace)
+            return
+
+        parser = UParser(udmf_types)
+        toplevel, blocks = parser.parse(lumpgroup["TEXTMAP"].data)
+        for (t, cls) in udmf_types.items():
+            setattr(self, cls.storage, blocks[t] if t in blocks else [])
+            if namespace is not None:
+                self.namespace = namespace
+            elif 'namespace' in toplevel:
+                self.namespace = toplevel['namespace']
+            else:
+                self.namespace = None
+
+        if 'BEHAVIOR' in lumpgroup:
+            self.behavior = lumpgroup['BEHAVIOR']
+        if 'SCRIPTS' in lumpgroup:
+            self.scripts = lumpgroup['SCRIPTS']
+
+    def from_oldformat(self, lumpgroup, namespace=None):
+        """Import a classic format (Doom or ZDoom/Hexen) map.
+
+        For ZDoom maps, deprecated line specials (such as Line_SetIdentification)
+        will automatically be translated to the UDMF equivalent.
+
+        If namespace is not specified, it will be given a default value based on
+        the map's original format (vanilla or ZDoom/Hexen)."""
+        m = MapEditor(lumpgroup)
+        self.vertexes = []
+        self.sidedefs = []
+        self.linedefs = []
+        self.sectors = []
+        self.things = []
+        self.namespace = namespace
+
+        hexencompat = 'BEHAVIOR' in lumpgroup
+        if namespace not in udmf_namespaces:
+            namespace = 'ZDoom' if hexencompat else udmf_namespaces[0]
+        if not self.namespace:
+            self.namespace = namespace
+
+        if hexencompat:
+            try:
+                self.behavior = m.behavior
+                self.scripts = m.scripts
+            except AttributeError:
+                pass
+
+        for thing in m.things:
+            block = UThing(float(thing.x), float(thing.y), thing.type)
+            self.things.append(block)
+
+            if thing.angle != 0:
+                block.angle = thing.angle
+
+            for f in range(len(UThing.flags[namespace])):
+                if not UThing.flags[namespace][f]:
+                    continue
+                for flag in UThing.flags[namespace][f].split(','):
+                    if flag[0] != '!':
+                        setattr(block, flag, bool(thing.flags & (1 << f)))
+                    else:
+                        setattr(block, flag[1:], not bool(thing.flags & (1 << f)))
+
+            if hexencompat:
+                block.id = thing.tid
+                block.height = float(thing.height)
+                block.special = thing.action
+                for i in range(5):
+                    key = 'arg{0}'.format(i)
+                    setattr(block, key, getattr(thing, key))
+
+        for linedef in m.linedefs:
+            block = ULinedef(linedef.vx_a, linedef.vx_b, linedef.front)
+            self.linedefs.append(block)
+
+            if linedef.back != Linedef.NONE:
+                block.sideback = linedef.back
+
+            for f in range(len(ULinedef.flags[namespace])):
+                flag = ULinedef.flags[namespace][f]
+                if flag:
+                    setattr(block, flag, bool(linedef.flags & (1 << f)))
+
+            if hexencompat:
+                if linedef.action == 121: # Line_SetIdentification
+                    block.id = linedef.arg0 + linedef.arg4 * 256
+                    for f in range(len(ULinedef.moreflags_hexen)):
+                        setattr(block, ULinedef.moreflags_hexen[f], bool(linedef.arg1 & (1 << f)))
+                elif linedef.action:
+                    block.special = linedef.action
+                    for i in range(5):
+                        key = 'arg{0}'.format(i)
+                        setattr(block, key, getattr(linedef, key))
+
+                    trigger = ((linedef.flags & 0x1c00) >> 10)
+                    if trigger < len(ULinedef.triggers_hexen):
+                        setattr(block, ULinedef.triggers_hexen[trigger], True)
+
+                    # handle line specials that set a line ID, extended flags, etc. based on the zdoom udmf spec
+                    if linedef.action == 1: # Polyobj_StartLine
+                        block.id = linedef.arg3
+                        block.arg3 = 0
+                    elif linedef.action == 5: # Polyobj_ExplicitLine
+                        block.id = linedef.arg4
+                        block.arg4 = 0
+                    elif linedef.action == 160: # Sector_Set3dFloor
+                        if linedef.arg1 & 8:
+                            block.id = linedef.arg4
+                            block.arg1 &= ~8
+                        else:
+                            block.arg0 += linedef.arg4 * 256
+                        block.arg4 = 0
+                    elif linedef.action == 181: # Plane_Align
+                        block.id = linedef.arg2
+                        block.arg2 = 0
+                    elif linedef.action == 208: # TranslucentLine
+                        block.id = linedef.arg0 # preserve arg0 according to spec
+                        for f in range(len(ULinedef.moreflags_hexen)):
+                            setattr(block, ULinedef.moreflags_hexen[f], bool(linedef.arg3 & (1 << f)))
+                        block.arg3 = 0
+                    elif linedef.action == 215: # Teleport_Line
+                        block.id = linedef.arg0
+                        block.arg0 = 0
+                    elif linedef.action == 222: # Scroll_Texture_Model
+                        block.id = linedef.arg0 # preserve arg0 according to spec
+            else:
+                block.special = linedef.action
+                block.id = block.arg0 = linedef.tag
+
+        for sidedef in m.sidedefs:
+            block = USidedef(sidedef.sector)
+            self.sidedefs.append(block)
+
+            block.offsetx = sidedef.off_x
+            block.offsety = sidedef.off_y
+            block.texturetop = sidedef.tx_up
+            block.texturebottom = sidedef.tx_low
+            block.texturemiddle = sidedef.tx_mid
+
+        for vertex in m.vertexes:
+            block = UVertex(float(vertex.x), float(vertex.y))
+            self.vertexes.append(block)
+
+        for sector in m.sectors:
+            block = USector(sector.tx_floor, sector.tx_ceil)
+            self.sectors.append(block)
+
+            block.heightfloor = sector.z_floor
+            block.heightceiling = sector.z_ceil
+            block.lightlevel = sector.light
+            block.special = sector.type
+            block.id = sector.tag
+
+    def to_lumps(self):
+        m = NameGroup()
+        m['_HEADER_'] = Lump()
+        m['TEXTMAP'] = Lump(str.encode(self.to_textmap()))
+        if self.behavior:
+            m['BEHAVIOR'] = self.behavior
+        if self.scripts:
+            m['SCRIPTS'] = self.scripts
+        m['ENDMAP'] = Lump()
+        return m
+
+    def to_textmap(self):
+        fallback = lambda *args: self.serialize_field(*args)
+        out = 'namespace="{0}";\n'.format(self.namespace)
+        for thing in self.things:
+            out += 'thing ' + thing.to_textmap(fallback)
+        for vertex in self.vertexes:
+            out += 'vertex ' + vertex.to_textmap(fallback)
+        for sidedef in self.sidedefs:
+            out += 'sidedef ' + sidedef.to_textmap(fallback)
+        for linedef in self.linedefs:
+            out += 'linedef ' + linedef.to_textmap(fallback)
+        for sector in self.sectors:
+            out += 'sector ' + sector.to_textmap(fallback)
+        return out
+
+    def serialize_field(self, value):
+        if isinstance(value, UVertex):
+            return self.vertexes.index(value)
+        if isinstance(value, USidedef):
+            return self.sidedefs.index(value)
+        if isinstance(value, ULinedef):
+            return self.linedefs.index(value)
+        if isinstance(value, USector):
+            return self.sectors.index(value)
+        if isinstance(value, UThing):
+            return self.things.index(value)
```

### Comparing `omgifol-0.5.0/omg/wad.py` & `omgifol-0.5.1/omg/wad.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,318 +1,318 @@
-import os, glob
-import omg.palette
-from omg.lump  import *
-from omg.util import *
-from omg.wadio import WadIO
-
-class LumpGroup(OrderedDict):
-    """A dict-like object for holding a group of lumps."""
-
-    def __init__(self, name='data', lumptype=Lump, config=()):
-        OrderedDict.__init__(self)
-        self._name   = name
-        self.lumptype = lumptype
-        self.config = config
-        self.__init2__()
-
-    def __init2__(self):
-        pass
-
-    def load(self, filename):
-        """Load entries from a WAD file. All lumps from the same
-        section in that WAD is loaded (e.g. if this is a patch
-        section, all patches in the WAD will be loaded."""
-        w = WAD(filename)
-        self += w.__dict__[self._name].copy()
-
-    def to_file(self, filename, use_free=True):
-        """Save group as a separate WAD file.
-
-        If use_free is true, existing free space in the WAD will
-        be used, if possible."""
-        w = WadIO(filename)
-        self.save_wadio(w, use_free=use_free)
-
-    def from_glob(self, globpattern):
-        """Create lumps from files matching the glob pattern."""
-        for p in glob.glob(globpattern):
-            name = fixname(os.path.basename(p[:p.rfind('.')]))
-            self[name] = self.lumptype(from_file=p)
-
-    def save_wadio(self, wadio, use_free=True):
-        """Save to a WadIO object.
-
-        If use_free is true, existing free space in the WAD will
-        be used, if possible."""
-        for m in self:
-            wadio.insert(m, self[m].data, use_free=use_free)
-
-    def copy(self):
-        """Creates a deep copy."""
-        a = self.__class__(self._name, self.lumptype, self.config)
-        for k in self:
-            a[k] = self[k].copy()
-        return a
-
-    def __add__(self, other):
-        """Adds two dicts, copying items shallowly."""
-        c = self.__class__(self._name, self.lumptype, self.config)
-        c.update(self)
-        c.update(other)
-        return c
-
-class MarkerGroup(LumpGroup):
-    """Group for lumps found between markers, e.g. sprites."""
-
-    def __init2__(self):
-        self.prefix = self.config + "*_START"
-        self.suffix = self.config + "*_END"
-        # In case group opens with XX_ and ends with X_
-        self.abssuffix = self.config + "_END"
-
-    def load_wadio(self, wadio):
-        """Load all matching lumps that have not already
-        been flagged as read from the given WadIO object."""
-        inside = False
-        startedwith, endswith = "", ""
-        for i in range(len(wadio.entries)):
-            if wadio.entries[i].been_read:
-                inside = False
-                continue
-            name = wadio.entries[i].name
-            if inside:
-                if wccmp(name, endswith) or wccmp(name, self.abssuffix):
-                    inside = False
-                else:
-                    if wadio.entries[i].size != 0:
-                        self[name] = self.lumptype(wadio.read(i))
-                wadio.entries[i].been_read = True
-            else:
-                # print name, self.prefix, wccmp(name, self.prefix)
-                if wccmp(name, self.prefix):
-                    startedwith = name
-                    endswith = name.replace("START", "END")
-                    inside = True
-                    wadio.entries[i].been_read = True
-
-    def save_wadio(self, wadio, use_free=True):
-        """Save to a WadIO object.
-
-        If use_free is true, existing free space in the WAD will
-        be used, if possible."""
-        if len(self) == 0:
-            return
-        wadio.insert(self.prefix.replace('*', ''), bytes())
-        LumpGroup.save_wadio(self, wadio, use_free=use_free)
-        wadio.insert(self.suffix.replace('*', ''), bytes())
-
-
-class HeaderGroup(LumpGroup):
-    """Group for lumps arranged header-tail (e.g. maps)."""
-
-    def __init2__(self):
-        self.tail = self.config
-
-    def load_wadio(self, wadio):
-        """Load all matching lumps that have not already
-        been flagged as read from the given WadIO object."""
-        numlumps = len(wadio.entries)
-        i = 0
-        while i < numlumps:
-            if wadio.entries[i].been_read:
-                i += 1
-                continue
-            name = wadio.entries[i].name
-            added = False
-            # now search only using tail lumps so that any map with map lumps is loaded correctly
-            # look for at least 2 tail lumps in order to avoid false positives
-            if i < numlumps - 2 \
-               and wccmp(wadio.entries[i + 1].name, self.tail[0]) \
-               and wccmp(wadio.entries[i + 2].name, self.tail[1]):
-                added = True
-                self[name] = NameGroup()
-                self[name]["_HEADER_"] = Lump(wadio.read(i))
-                wadio.entries[i].been_read = True
-                i += 1
-                while i < numlumps and inwclist(wadio.entries[i].name, self.tail):
-                    self[name][wadio.entries[i].name] = \
-                        self.lumptype(wadio.read(i))
-                    wadio.entries[i].been_read = True
-                    i += 1
-                    if wccmp(wadio.entries[i - 1].name, self.tail[-1]):
-                        break
-            if not added:
-                i += 1
-
-    def save_wadio(self, wadio, use_free=True):
-        """Save to a WadIO object.
-
-        If use_free is true, existing free space in the WAD will
-        be used, if possible."""
-        for h in self:
-            hs = copy(self[h]) # temporary shallow copy
-            try:
-                wadio.insert(h, hs["_HEADER_"].data, use_free=use_free)
-                del hs["_HEADER_"]
-            except KeyError:
-                wadio.insert(h, bytes())
-            for t in self.tail:
-                try:
-                    # for UDMF maps, a wildcard is used to handle anything between 'TEXTMAP' and 'ENDMAP'
-                    # after writing lumps, remove them from the shallow copy so the wildcard doesn't include them again
-                    for name in wcinlist(hs, t):
-                        wadio.insert(name, hs[name].data, use_free=use_free)
-                        del hs[name]
-                except IndexError:
-                    pass
-
-
-class NameGroup(LumpGroup):
-    """Group for lumps recognized by special names."""
-
-    def __init2__(self):
-        self.names = self.config
-
-    def load_wadio(self, wadio):
-        """Load all matching lumps that have not already
-        been flagged as read from the given WadIO object."""
-        inside = False
-        for i in range(len(wadio.entries)):
-            if wadio.entries[i].been_read:
-                continue
-            name = wadio.entries[i].name
-            if inwclist(name, self.names):
-                self[name] = self.lumptype(wadio.read(i))
-                wadio.entries[i].been_read = True
-
-class TxdefGroup(NameGroup):
-    """Group for texture definition lumps."""
-    def __init2__(self):
-        self.names = ['TEXTURE?', 'PNAMES']
-    def __add__(self, other):
-        import omg.txdef
-        a = omg.txdef.Textures()
-        a.from_lumps(self)
-        a.from_lumps(other)
-        return a.to_lumps()
-
-
-#---------------------------------------------------------------------
-#
-# This defines the default structure for WAD files.
-#
-
-# First some lists...
-_maptail    = ['THINGS',   'LINEDEFS', 'SIDEDEFS', # Must be in order
-               'VERTEXES', 'SEGS',     'SSECTORS',
-               'NODES',    'SECTORS',  'REJECT',
-               'BLOCKMAP', 'BEHAVIOR', 'SCRIPT*']
-_udmfmaptail  = ['TEXTMAP', '*', 'ENDMAP']
-_glmaptail    = ['GL_VERT', 'GL_SEGS', 'GL_SSECT', 'GL_NODES']
-_graphics     = ['TITLEPIC', 'CWILV*', 'WI*', 'M_*',
-                 'INTERPIC', 'BRDR*',  'PFUB?', 'ST*',
-                 'VICTORY2', 'CREDIT', 'END?',  'WI*',
-                 'BOSSBACK', 'ENDPIC', 'HELP',  'BOX??',
-                 'AMMNUM?',  'HELP1',  'DIG*']
-
-# The default structure object.
-# Must be in order: markers first, ['*'] name group last
-defstruct = [
-    [MarkerGroup, 'sprites',   Graphic, 'S'],
-    [MarkerGroup, 'patches',   Graphic, 'P'],
-    [MarkerGroup, 'flats',     Flat,    'F'],
-    [MarkerGroup, 'colormaps', Lump,    'C'],
-    [MarkerGroup, 'ztextures', Graphic, 'TX'],
-    [HeaderGroup, 'maps',   Lump, _maptail],
-    [HeaderGroup, 'glmaps', Lump, _glmaptail],
-    [HeaderGroup, 'udmfmaps', Lump, _udmfmaptail],
-    [NameGroup,   'music',    Music, ['D_*']],
-    [NameGroup,   'sounds',   Sound, ['DS*', 'DP*']],
-    [TxdefGroup,  'txdefs',   Lump,  ['TEXTURE?', 'PNAMES']],
-    [NameGroup,   'graphics', Graphic, _graphics],
-    [NameGroup,   'data',     Lump,  ['*']]
-]
-
-write_order = ['data', 'colormaps', 'maps', 'glmaps', 'udmfmaps', 'txdefs',
-    'sounds', 'music', 'graphics', 'sprites', 'patches', 'flats',
-    'ztextures']
-
-class WAD:
-    """A memory-resident, abstract representation of a WAD file. Lumps
-    are stored in subsections of the WAD. Loading/saving and handling
-    the sections follows the structure specification.
-
-    Initialization:
-    new = WAD([from_file, structure])
-
-    Source may be a string representing a path to a file to load from.
-    By default, an empty WAD is created.
-
-    Structure may be used to specify a custom lump
-    categorization/loading configuration.
-
-    Member data:
-        .structure     Structure definition.
-        .palette       Palette
-        .sprites, etc  Sections containing lumps, as specified by
-                       the structure definition
-    """
-
-    def __init__(self, from_file=None, structure=defstruct):
-        """Create a new WAD. The optional `source` argument may be a
-        string specifying a path to a file or a WadIO object.
-        If omitted, an empty WAD is created. A WADStructure object
-        may be passed as the `structure` argument to apply a custom
-        section structure. By default, the structure specified in the
-        defdata module is used."""
-        self.__category = 'root'
-        self.palette = omg.palette.default
-        self.structure = structure
-        self.groups = []
-        for group_def in self.structure:
-            instance = group_def[0](*tuple(group_def[1:]))
-            self.__dict__[group_def[1]] = instance
-            self.groups.append(instance)
-        if from_file:
-            self.from_file(from_file)
-
-    def from_file(self, source):
-        """Load contents from a file. `source` may be a string
-        specifying a path to a file or a WadIO object."""
-        if isinstance(source, WadIO):
-            w = source
-        elif isinstance(source, str):
-            assert os.path.exists(source)
-            w = WadIO(source)
-        else:
-            raise TypeError("Expected WadIO or file path string")
-        for group in self.groups:
-            group.load_wadio(w)
-
-    def to_file(self, filename):
-        """Save contents to a WAD file. Caution: if a file with the given name
-        already exists, it will be overwritten. However, the existing file will
-        be kept as <filename>.tmp until the operation has finished, to stay safe
-        in case of failure."""
-        use_backup = os.path.exists(filename)
-        tmpfilename = filename + ".tmp"
-        if use_backup:
-            if os.path.exists(tmpfilename):
-                os.remove(tmpfilename)
-            os.rename(filename, tmpfilename)
-        w = WadIO(filename)
-        for group in write_order:
-            self.__dict__[group].save_wadio(w, use_free=False)
-        w.save()
-        if use_backup:
-            os.remove(tmpfilename)
-
-    def __add__(self, other):
-        assert isinstance(other, WAD)
-        w = WAD(structure=self.structure)
-        for group_def in self.structure:
-            name = group_def[1]
-            w.__dict__[name] = self.__dict__[name] + other.__dict__[name]
-        return w
-
-    def copy(self):
-        return deepcopy(self)
+import os, glob
+import omg.palette
+from omg.lump  import *
+from omg.util import *
+from omg.wadio import WadIO
+
+class LumpGroup(OrderedDict):
+    """A dict-like object for holding a group of lumps."""
+
+    def __init__(self, name='data', lumptype=Lump, config=()):
+        OrderedDict.__init__(self)
+        self._name   = name
+        self.lumptype = lumptype
+        self.config = config
+        self.__init2__()
+
+    def __init2__(self):
+        pass
+
+    def load(self, filename):
+        """Load entries from a WAD file. All lumps from the same
+        section in that WAD is loaded (e.g. if this is a patch
+        section, all patches in the WAD will be loaded."""
+        w = WAD(filename)
+        self += w.__dict__[self._name].copy()
+
+    def to_file(self, filename, use_free=True):
+        """Save group as a separate WAD file.
+
+        If use_free is true, existing free space in the WAD will
+        be used, if possible."""
+        w = WadIO(filename)
+        self.save_wadio(w, use_free=use_free)
+
+    def from_glob(self, globpattern):
+        """Create lumps from files matching the glob pattern."""
+        for p in glob.glob(globpattern):
+            name = fixname(os.path.basename(p[:p.rfind('.')]))
+            self[name] = self.lumptype(from_file=p)
+
+    def save_wadio(self, wadio, use_free=True):
+        """Save to a WadIO object.
+
+        If use_free is true, existing free space in the WAD will
+        be used, if possible."""
+        for m in self:
+            wadio.insert(m, self[m].data, use_free=use_free)
+
+    def copy(self):
+        """Creates a deep copy."""
+        a = self.__class__(self._name, self.lumptype, self.config)
+        for k in self:
+            a[k] = self[k].copy()
+        return a
+
+    def __add__(self, other):
+        """Adds two dicts, copying items shallowly."""
+        c = self.__class__(self._name, self.lumptype, self.config)
+        c.update(self)
+        c.update(other)
+        return c
+
+class MarkerGroup(LumpGroup):
+    """Group for lumps found between markers, e.g. sprites."""
+
+    def __init2__(self):
+        self.prefix = self.config + "*_START"
+        self.suffix = self.config + "*_END"
+        # In case group opens with XX_ and ends with X_
+        self.abssuffix = self.config + "_END"
+
+    def load_wadio(self, wadio):
+        """Load all matching lumps that have not already
+        been flagged as read from the given WadIO object."""
+        inside = False
+        startedwith, endswith = "", ""
+        for i in range(len(wadio.entries)):
+            if wadio.entries[i].been_read:
+                inside = False
+                continue
+            name = wadio.entries[i].name
+            if inside:
+                if wccmp(name, endswith) or wccmp(name, self.abssuffix):
+                    inside = False
+                else:
+                    if wadio.entries[i].size != 0:
+                        self[name] = self.lumptype(wadio.read(i))
+                wadio.entries[i].been_read = True
+            else:
+                # print name, self.prefix, wccmp(name, self.prefix)
+                if wccmp(name, self.prefix):
+                    startedwith = name
+                    endswith = name.replace("START", "END")
+                    inside = True
+                    wadio.entries[i].been_read = True
+
+    def save_wadio(self, wadio, use_free=True):
+        """Save to a WadIO object.
+
+        If use_free is true, existing free space in the WAD will
+        be used, if possible."""
+        if len(self) == 0:
+            return
+        wadio.insert(self.prefix.replace('*', ''), bytes())
+        LumpGroup.save_wadio(self, wadio, use_free=use_free)
+        wadio.insert(self.suffix.replace('*', ''), bytes())
+
+
+class HeaderGroup(LumpGroup):
+    """Group for lumps arranged header-tail (e.g. maps)."""
+
+    def __init2__(self):
+        self.tail = self.config
+
+    def load_wadio(self, wadio):
+        """Load all matching lumps that have not already
+        been flagged as read from the given WadIO object."""
+        numlumps = len(wadio.entries)
+        i = 0
+        while i < numlumps:
+            if wadio.entries[i].been_read:
+                i += 1
+                continue
+            name = wadio.entries[i].name
+            added = False
+            # now search only using tail lumps so that any map with map lumps is loaded correctly
+            # look for at least 2 tail lumps in order to avoid false positives
+            if i < numlumps - 2 \
+               and wccmp(wadio.entries[i + 1].name, self.tail[0]) \
+               and wccmp(wadio.entries[i + 2].name, self.tail[1]):
+                added = True
+                self[name] = NameGroup()
+                self[name]["_HEADER_"] = Lump(wadio.read(i))
+                wadio.entries[i].been_read = True
+                i += 1
+                while i < numlumps and inwclist(wadio.entries[i].name, self.tail):
+                    self[name][wadio.entries[i].name] = \
+                        self.lumptype(wadio.read(i))
+                    wadio.entries[i].been_read = True
+                    i += 1
+                    if wccmp(wadio.entries[i - 1].name, self.tail[-1]):
+                        break
+            if not added:
+                i += 1
+
+    def save_wadio(self, wadio, use_free=True):
+        """Save to a WadIO object.
+
+        If use_free is true, existing free space in the WAD will
+        be used, if possible."""
+        for h in self:
+            hs = copy(self[h]) # temporary shallow copy
+            try:
+                wadio.insert(h, hs["_HEADER_"].data, use_free=use_free)
+                del hs["_HEADER_"]
+            except KeyError:
+                wadio.insert(h, bytes())
+            for t in self.tail:
+                try:
+                    # for UDMF maps, a wildcard is used to handle anything between 'TEXTMAP' and 'ENDMAP'
+                    # after writing lumps, remove them from the shallow copy so the wildcard doesn't include them again
+                    for name in wcinlist(hs, t):
+                        wadio.insert(name, hs[name].data, use_free=use_free)
+                        del hs[name]
+                except IndexError:
+                    pass
+
+
+class NameGroup(LumpGroup):
+    """Group for lumps recognized by special names."""
+
+    def __init2__(self):
+        self.names = self.config
+
+    def load_wadio(self, wadio):
+        """Load all matching lumps that have not already
+        been flagged as read from the given WadIO object."""
+        inside = False
+        for i in range(len(wadio.entries)):
+            if wadio.entries[i].been_read:
+                continue
+            name = wadio.entries[i].name
+            if inwclist(name, self.names):
+                self[name] = self.lumptype(wadio.read(i))
+                wadio.entries[i].been_read = True
+
+class TxdefGroup(NameGroup):
+    """Group for texture definition lumps."""
+    def __init2__(self):
+        self.names = ['TEXTURE?', 'PNAMES']
+    def __add__(self, other):
+        import omg.txdef
+        a = omg.txdef.Textures()
+        a.from_lumps(self)
+        a.from_lumps(other)
+        return a.to_lumps()
+
+
+#---------------------------------------------------------------------
+#
+# This defines the default structure for WAD files.
+#
+
+# First some lists...
+_maptail    = ['THINGS',   'LINEDEFS', 'SIDEDEFS', # Must be in order
+               'VERTEXES', 'SEGS',     'SSECTORS',
+               'NODES',    'SECTORS',  'REJECT',
+               'BLOCKMAP', 'BEHAVIOR', 'SCRIPT*']
+_udmfmaptail  = ['TEXTMAP', '*', 'ENDMAP']
+_glmaptail    = ['GL_VERT', 'GL_SEGS', 'GL_SSECT', 'GL_NODES']
+_graphics     = ['TITLEPIC', 'CWILV*', 'WI*', 'M_*',
+                 'INTERPIC', 'BRDR*',  'PFUB?', 'ST*',
+                 'VICTORY2', 'CREDIT', 'END?',  'WI*',
+                 'BOSSBACK', 'ENDPIC', 'HELP',  'BOX??',
+                 'AMMNUM?',  'HELP1',  'DIG*']
+
+# The default structure object.
+# Must be in order: markers first, ['*'] name group last
+defstruct = [
+    [MarkerGroup, 'sprites',   Graphic, 'S'],
+    [MarkerGroup, 'patches',   Graphic, 'P'],
+    [MarkerGroup, 'flats',     Flat,    'F'],
+    [MarkerGroup, 'colormaps', Lump,    'C'],
+    [MarkerGroup, 'ztextures', Graphic, 'TX'],
+    [HeaderGroup, 'maps',   Lump, _maptail],
+    [HeaderGroup, 'glmaps', Lump, _glmaptail],
+    [HeaderGroup, 'udmfmaps', Lump, _udmfmaptail],
+    [NameGroup,   'music',    Music, ['D_*']],
+    [NameGroup,   'sounds',   Sound, ['DS*', 'DP*']],
+    [TxdefGroup,  'txdefs',   Lump,  ['TEXTURE?', 'PNAMES']],
+    [NameGroup,   'graphics', Graphic, _graphics],
+    [NameGroup,   'data',     Lump,  ['*']]
+]
+
+write_order = ['data', 'colormaps', 'maps', 'glmaps', 'udmfmaps', 'txdefs',
+    'sounds', 'music', 'graphics', 'sprites', 'patches', 'flats',
+    'ztextures']
+
+class WAD:
+    """A memory-resident, abstract representation of a WAD file. Lumps
+    are stored in subsections of the WAD. Loading/saving and handling
+    the sections follows the structure specification.
+
+    Initialization:
+    new = WAD([from_file, structure])
+
+    Source may be a string representing a path to a file to load from.
+    By default, an empty WAD is created.
+
+    Structure may be used to specify a custom lump
+    categorization/loading configuration.
+
+    Member data:
+        .structure     Structure definition.
+        .palette       Palette
+        .sprites, etc  Sections containing lumps, as specified by
+                       the structure definition
+    """
+
+    def __init__(self, from_file=None, structure=defstruct):
+        """Create a new WAD. The optional `source` argument may be a
+        string specifying a path to a file or a WadIO object.
+        If omitted, an empty WAD is created. A WADStructure object
+        may be passed as the `structure` argument to apply a custom
+        section structure. By default, the structure specified in the
+        defdata module is used."""
+        self.__category = 'root'
+        self.palette = omg.palette.default
+        self.structure = structure
+        self.groups = []
+        for group_def in self.structure:
+            instance = group_def[0](*tuple(group_def[1:]))
+            self.__dict__[group_def[1]] = instance
+            self.groups.append(instance)
+        if from_file:
+            self.from_file(from_file)
+
+    def from_file(self, source):
+        """Load contents from a file. `source` may be a string
+        specifying a path to a file or a WadIO object."""
+        if isinstance(source, WadIO):
+            w = source
+        elif isinstance(source, str):
+            assert os.path.exists(source)
+            w = WadIO(source)
+        else:
+            raise TypeError("Expected WadIO or file path string")
+        for group in self.groups:
+            group.load_wadio(w)
+
+    def to_file(self, filename):
+        """Save contents to a WAD file. Caution: if a file with the given name
+        already exists, it will be overwritten. However, the existing file will
+        be kept as <filename>.tmp until the operation has finished, to stay safe
+        in case of failure."""
+        use_backup = os.path.exists(filename)
+        tmpfilename = filename + ".tmp"
+        if use_backup:
+            if os.path.exists(tmpfilename):
+                os.remove(tmpfilename)
+            os.rename(filename, tmpfilename)
+        w = WadIO(filename)
+        for group in write_order:
+            self.__dict__[group].save_wadio(w, use_free=False)
+        w.save()
+        if use_backup:
+            os.remove(tmpfilename)
+
+    def __add__(self, other):
+        assert isinstance(other, WAD)
+        w = WAD(structure=self.structure)
+        for group_def in self.structure:
+            name = group_def[1]
+            w.__dict__[name] = self.__dict__[name] + other.__dict__[name]
+        return w
+
+    def copy(self):
+        return deepcopy(self)
```

### Comparing `omgifol-0.5.0/omg/wadio.py` & `omgifol-0.5.1/omg/wadio.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,344 +1,344 @@
-import os, hashlib, time
-from omg.util import *
-
-class Header(WADStruct):
-    """Class for WAD file headers."""
-    _fields_ = [
-        ("type",    ctypes.c_char * 4),
-        ("dir_len", ctypes.c_uint32),
-        ("dir_ptr", ctypes.c_uint32)
-    ]
-
-    def __init__(self, *args, **kwargs):
-        self.type = "PWAD"
-        super().__init__(*args, **kwargs)
-
-class Entry(WADStruct):
-    """Class for WAD file entries."""
-    _fields_ = [
-        ("ptr",  ctypes.c_uint32),
-        ("size", ctypes.c_uint32),
-        ("name", ctypes.c_char * 8),
-    ]
-
-    def __init__(self, *args, **kwargs):
-        self.been_read = False # Used by WAD loader
-        super().__init__(*args, **kwargs)
-
-# WadIO.open() behaves just like open(). Sometimes it is
-# useful to specifically either open an existing file
-# or create a new one.
-
-def open_wad():
-    """Open an existing WAD, raise IOError if not found."""
-    if not os.path.exists(location):
-        raise IOError
-    return WadIO(location)
-
-def create_wad(location):
-    """Create a new WAD, raise IOError if exists."""
-    if os.path.exists(location):
-        raise IOError
-    return WadIO(location)
-
-
-class WadIO:
-    """A WadIO object is used to open a WAD file for direct
-    reading and writing.
-
-    IMPORTANT: In case the contents of the file have been modified,
-    .save() must be called before exiting, or data will be lost/the
-    universe explodes. You can check whether the file is in need of
-    saving by reading the value of the boolean attribute .issafe
-
-    WadIO objects work on the WAD directory level. There is
-    very little magic available - you can't do things like automatic
-    merging or managing sections, and Omgifol is never aware of
-    what types lumps are. In other words, you're doing things more
-    or less manually, with the hard binary content of lumps and
-    the linear order they're stored in.
-
-    Use this for very large WADs and when only performing small/few
-    operations. For example, when you need to read a lump or two
-    from an IWAD for copying into another WAD. Also use it when
-    it is important that the saved file is identical to the opened
-    file; that is not guaranteed to work with the higher-level WAD
-    class since it sometimes modifies order.
-
-    The benefit of using this class is that you don't have to read
-    and write the whole file when opening or closing. The downside
-    is that changes can't be undone (so back up first!) and that
-    file content will get fragmented when you edit lumps (unused
-    space will appear). To get rid of the wasted space, use the
-    rewrite() method (which rewrites the entire file)."""
-
-    def __init__(self, openfrom=None):
-        self.basefile = None
-        self.issafe = True
-        self.header = Header()
-        self.entries = []
-        if openfrom is not None:
-            self.open(openfrom)
-
-    def __del__(self):
-        if self.basefile:
-            self.basefile.close()
-
-    def open(self, filename):
-        """Open a WAD file, create a new file if none exists at the path."""
-        assert not self.entries
-        if self.basefile:
-            raise IOError("The handle is already open")
-        # Open an existing WAD
-        if os.path.exists(filename):
-            try:
-                self.basefile = open(filename, 'r+b')
-            except IOError:
-                # assume file is read-only
-                self.basefile = open(filename, 'rb')
-
-            filesize = os.stat(self.basefile.name)[6]
-            self.header = h = Header(bytes=self.basefile.read(ctypes.sizeof(Header)))
-            if (not h.type in ("PWAD", "IWAD")) or filesize < 12:
-                raise IOError("The file is not a valid WAD file.")
-            if filesize < h.dir_ptr + h.dir_len*ctypes.sizeof(Entry):
-                raise IOError("Invalid directory information in header.")
-            self.basefile.seek(h.dir_ptr)
-            self.entries = [Entry(bytes=self.basefile.read(ctypes.sizeof(Entry))) \
-                for i in range(h.dir_len)]
-        # Create new
-        else:
-            self.basefile = open(filename, 'w+b')
-            self.basefile.write(Header().pack())
-            self.basefile.flush()
-
-    def close(self):
-        """Close the base file."""
-        assert self.basefile
-        # Unfortunately, a save can't be forced here.
-        if not self.issafe:
-            raise IOError(\
-                "closing a modified file may corrupt it. use save() first")
-        self.basefile.close()
-        self.basefile = None
-
-    def select(self, id):
-        """Return a valid index from a proposed index or entry name, or
-        raise LookupError in case of failure."""
-        assert self.basefile
-        if isinstance(id, int):
-            if id < len(self.entries):
-                return id
-            raise LookupError
-        elif isinstance(id, str):
-            for i in range(len(self.entries)):
-                if wccmp(self.entries[i].name, id):
-                    return i
-            raise LookupError
-        raise TypeError
-
-    def get(self, id):
-        return self.entries[self.select(id)]
-
-    def find(self, id):
-        """Search for an entry and return the index of the first match
-        or None if no matches were found. Wildcards are supported."""
-        assert self.basefile
-        try:
-            return self.select(id)
-        except LookupError:
-            return None
-
-    def multifind(self, id, start=None, end=None):
-        """Search for entries and return a list of matches. Wildcards
-        are supported."""
-        assert self.basefile
-        if start is None: start = 0
-        if end   is None: end   = len(self.entries)
-        return [i for i in range(start, end) if \
-                wccmp(self.entries[i].name, id)]
-
-    def read(self, id):
-        """Read an entry and return the data as a binary string."""
-        assert self.basefile
-        id = self.select(id)
-        self.basefile.seek(self.entries[id].ptr)
-        return self.basefile.read(self.entries[id].size)
-
-    def remove(self, id):
-        """Remove an entry."""
-        assert self.basefile
-        del (self.entries[self.select(id)])
-        self.issafe = False
-
-    def rename(self, id, new):
-        """Rename an entry."""
-        assert self.basefile
-        self.entries[self.select(id)].name = new[0:8].upper()
-        self.issafe = False
-
-    def write_at(self, pos, data):
-        """Write data at the given position."""
-        self.basefile.seek(pos)
-        self.basefile.write(data)
-
-    def write_append(self, data):
-        """Write data at the end of the file."""
-        self.basefile.seek(0, 2)
-        self.basefile.write(data)
-
-    def write_free(self, data):
-        """Write data to empty space in the file, if available,
-        otherwise write to the end of the file.
-        Returns the position that was written to.
-        """
-        self.basefile.seek(0, 2)
-        pos = self.basefile.tell()
-
-        # Find the earliest available free space
-        # (or, if free space reaches to the end of the file, use it)
-        for p in self.calc_waste()[1]:
-            if p[1] - p[0] >= len(data) or p[1] == pos:
-                pos = p[0]
-                self.basefile.seek(pos)
-                break
-
-        self.basefile.write(data)
-        return pos
-
-    def insert(self, name, data, index=None, use_free=True):
-        """Insert a new entry at the optional index (defaults to
-        appending).
-
-        If use_free is true, existing free space in the WAD will
-        be used, if possible."""
-        assert self.basefile
-        try:
-            index = self.select(index)
-        except:
-            index = None
-        self.issafe = False
-
-        if len(data) == 0:
-            pos = 0
-        elif use_free:
-            # write data to end of file or use free space if possible
-            pos = self.write_free(data)
-        else:
-            self.basefile.seek(0, 2)
-            pos = self.basefile.tell()
-            self.basefile.write(data)
-
-        if index is None:
-            self.entries.append(Entry(pos, len(data), name))
-        else:
-            self.entries.insert(index, Entry(pos, len(data), name))
-        self.basefile.flush()
-
-    def update(self, id, data):
-        """Write new data for an existing lump. If the new data is
-        bigger than what's present, a new position in the file will be
-        allocated for the lump."""
-        assert self.basefile
-        id = self.select(id)
-        if len(data) != self.entries[id].size:
-            self.issafe = False
-
-        if len(data) == 0:
-            self.entries[i].ptr = 0
-        elif len(data) <= self.entries[id].size:
-            self.write_at(self.entries[id].ptr, data)
-        else:
-            # temporarily mark existing entry as free, its current space will
-            # be combined with any adjacent free space
-            self.entries[id].size = 0
-            # write data to end of file or use free space if possible
-            self.entries[id].ptr = self.write_free(data)
-        self.entries[id].size = len(data)
-        self.basefile.flush()
-
-    def save(self):
-        """Save directory and header changes to the WAD file."""
-        assert self.basefile
-        if self.issafe: return
-        dir = join([e.pack() for e in self.entries])
-        self.header.dir_len = len(self.entries)
-        self.header.dir_ptr = self.write_free(dir)
-        self.write_at(0, self.header.pack())
-        self.basefile.flush()
-        self.issafe = True
-
-    def rewrite(self):
-        """Rewrite the entire WAD file. This removes all garbage
-        (wasted space) from the file."""
-        assert self.basefile
-        fpath = self.basefile.name
-        # Write to a temporary file and rename it when done
-        # os.tmpnam works too, but gives a security warning
-        tmppath = hashlib.md5(str(time.time())).hexdigest()[:8] + ".tmp"
-        tmppath = os.path.join(os.path.dirname(fpath), tmppath)
-        outwad = create_wad(tmppath)
-        for i in range(len(self.entries)):
-            outwad.insert(self.entries[i].name, self.read(i), use_free=False)
-        outwad.save()
-        outwad.close()
-        self.close()
-        os.remove(fpath)
-        os.rename(tmppath, fpath)
-        self.entries = []
-        self.open(fpath)
-        self.issafe = True
-
-    def calc_waste(self):
-        """Returns an (int, list) tuple containing the total amount of
-        wasted space in the WAD and a list of (start, end) tuples for
-        the spots where the wasted chunks are located."""
-        assert self.basefile
-        filesize = os.stat(self.basefile.name)[6]
-        # Create a list of (start, end) tuples to represent used space
-        chunks = []
-        # Treat the header and the end of the file as chunks of used space
-        chunks.append((0, 12))
-        chunks.append((filesize, filesize + 1))
-        # Add to the list the chunks that are occupied by lump data
-        chunks.append((self.header.dir_ptr, self.header.dir_ptr + \
-            len(self.entries)*ctypes.sizeof(Entry)))
-        for entry in self.entries:
-            if entry.size > 0:
-                chunks.append((entry.ptr, entry.ptr + entry.size))
-        # Sort it so we can go through it linearly and check for gaps
-        chunks.sort()
-        positions = []
-        space = 0
-        for i in range(0, len(chunks)-1):
-            # Check whether the end of the chunk touches the beginning of the
-            # next one. If not, there's wasted space between them.
-            if chunks[i][1] < chunks[i+1][0]:
-                positions.append((chunks[i][1], chunks[i+1][0]))
-                space += positions[-1][1] - positions[-1][0]
-        return space, positions
-
-    def info_text(self):
-        """Return printable fancy-formatted info about the WAD file."""
-        assert self.basefile
-        assert self.issafe
-        filesize = os.stat(self.basefile.name)[6]
-        s = []
-        # Main information
-        s.append("Info for %s\n\n" % self.basefile.name)
-        s.append("Type: %s\n" % self.header.type)
-        s.append("Size: %d bytes\n" % filesize)
-        s.append("Directory start: 0x%x" % self.header.dir_ptr)
-        # List all the lumps and some relevant information
-        s.append("\n\nEntries:\n\n     #  Name       Size       Position\n\n")
-        for i, entry in enumerate(self.entries):
-            s.append("%6i  %s %s 0x%x\n" %
-                (i, entry.name.ljust(10), str(entry.size).ljust(10), entry.ptr))
-        # Add info about wasted space in the WAD, to find out how much of an
-        # improvement a rewrite() would make
-        total, wasted = self.calc_waste()
-        s.append("\nWasted space:\n\n")
-        s.append("    %s bytes total\n" % str(total))
-        for w in wasted:
-            s.append("    %i bytes starting at 0x%x\n" % (w[1]-w[0], w[0]))
-        return ''.join(s)
+import os, hashlib, time
+from omg.util import *
+
+class Header(WADStruct):
+    """Class for WAD file headers."""
+    _fields_ = [
+        ("type",    ctypes.c_char * 4),
+        ("dir_len", ctypes.c_uint32),
+        ("dir_ptr", ctypes.c_uint32)
+    ]
+
+    def __init__(self, *args, **kwargs):
+        self.type = "PWAD"
+        super().__init__(*args, **kwargs)
+
+class Entry(WADStruct):
+    """Class for WAD file entries."""
+    _fields_ = [
+        ("ptr",  ctypes.c_uint32),
+        ("size", ctypes.c_uint32),
+        ("name", ctypes.c_char * 8),
+    ]
+
+    def __init__(self, *args, **kwargs):
+        self.been_read = False # Used by WAD loader
+        super().__init__(*args, **kwargs)
+
+# WadIO.open() behaves just like open(). Sometimes it is
+# useful to specifically either open an existing file
+# or create a new one.
+
+def open_wad():
+    """Open an existing WAD, raise IOError if not found."""
+    if not os.path.exists(location):
+        raise IOError
+    return WadIO(location)
+
+def create_wad(location):
+    """Create a new WAD, raise IOError if exists."""
+    if os.path.exists(location):
+        raise IOError
+    return WadIO(location)
+
+
+class WadIO:
+    """A WadIO object is used to open a WAD file for direct
+    reading and writing.
+
+    IMPORTANT: In case the contents of the file have been modified,
+    .save() must be called before exiting, or data will be lost/the
+    universe explodes. You can check whether the file is in need of
+    saving by reading the value of the boolean attribute .issafe
+
+    WadIO objects work on the WAD directory level. There is
+    very little magic available - you can't do things like automatic
+    merging or managing sections, and Omgifol is never aware of
+    what types lumps are. In other words, you're doing things more
+    or less manually, with the hard binary content of lumps and
+    the linear order they're stored in.
+
+    Use this for very large WADs and when only performing small/few
+    operations. For example, when you need to read a lump or two
+    from an IWAD for copying into another WAD. Also use it when
+    it is important that the saved file is identical to the opened
+    file; that is not guaranteed to work with the higher-level WAD
+    class since it sometimes modifies order.
+
+    The benefit of using this class is that you don't have to read
+    and write the whole file when opening or closing. The downside
+    is that changes can't be undone (so back up first!) and that
+    file content will get fragmented when you edit lumps (unused
+    space will appear). To get rid of the wasted space, use the
+    rewrite() method (which rewrites the entire file)."""
+
+    def __init__(self, openfrom=None):
+        self.basefile = None
+        self.issafe = True
+        self.header = Header()
+        self.entries = []
+        if openfrom is not None:
+            self.open(openfrom)
+
+    def __del__(self):
+        if self.basefile:
+            self.basefile.close()
+
+    def open(self, filename):
+        """Open a WAD file, create a new file if none exists at the path."""
+        assert not self.entries
+        if self.basefile:
+            raise IOError("The handle is already open")
+        # Open an existing WAD
+        if os.path.exists(filename):
+            try:
+                self.basefile = open(filename, 'r+b')
+            except IOError:
+                # assume file is read-only
+                self.basefile = open(filename, 'rb')
+
+            filesize = os.stat(self.basefile.name)[6]
+            self.header = h = Header(bytes=self.basefile.read(ctypes.sizeof(Header)))
+            if (not h.type in ("PWAD", "IWAD")) or filesize < 12:
+                raise IOError("The file is not a valid WAD file.")
+            if filesize < h.dir_ptr + h.dir_len*ctypes.sizeof(Entry):
+                raise IOError("Invalid directory information in header.")
+            self.basefile.seek(h.dir_ptr)
+            self.entries = [Entry(bytes=self.basefile.read(ctypes.sizeof(Entry))) \
+                for i in range(h.dir_len)]
+        # Create new
+        else:
+            self.basefile = open(filename, 'w+b')
+            self.basefile.write(Header().pack())
+            self.basefile.flush()
+
+    def close(self):
+        """Close the base file."""
+        assert self.basefile
+        # Unfortunately, a save can't be forced here.
+        if not self.issafe:
+            raise IOError(\
+                "closing a modified file may corrupt it. use save() first")
+        self.basefile.close()
+        self.basefile = None
+
+    def select(self, id):
+        """Return a valid index from a proposed index or entry name, or
+        raise LookupError in case of failure."""
+        assert self.basefile
+        if isinstance(id, int):
+            if id < len(self.entries):
+                return id
+            raise LookupError
+        elif isinstance(id, str):
+            for i in range(len(self.entries)):
+                if wccmp(self.entries[i].name, id):
+                    return i
+            raise LookupError
+        raise TypeError
+
+    def get(self, id):
+        return self.entries[self.select(id)]
+
+    def find(self, id):
+        """Search for an entry and return the index of the first match
+        or None if no matches were found. Wildcards are supported."""
+        assert self.basefile
+        try:
+            return self.select(id)
+        except LookupError:
+            return None
+
+    def multifind(self, id, start=None, end=None):
+        """Search for entries and return a list of matches. Wildcards
+        are supported."""
+        assert self.basefile
+        if start is None: start = 0
+        if end   is None: end   = len(self.entries)
+        return [i for i in range(start, end) if \
+                wccmp(self.entries[i].name, id)]
+
+    def read(self, id):
+        """Read an entry and return the data as a binary string."""
+        assert self.basefile
+        id = self.select(id)
+        self.basefile.seek(self.entries[id].ptr)
+        return self.basefile.read(self.entries[id].size)
+
+    def remove(self, id):
+        """Remove an entry."""
+        assert self.basefile
+        del (self.entries[self.select(id)])
+        self.issafe = False
+
+    def rename(self, id, new):
+        """Rename an entry."""
+        assert self.basefile
+        self.entries[self.select(id)].name = new[0:8].upper()
+        self.issafe = False
+
+    def write_at(self, pos, data):
+        """Write data at the given position."""
+        self.basefile.seek(pos)
+        self.basefile.write(data)
+
+    def write_append(self, data):
+        """Write data at the end of the file."""
+        self.basefile.seek(0, 2)
+        self.basefile.write(data)
+
+    def write_free(self, data):
+        """Write data to empty space in the file, if available,
+        otherwise write to the end of the file.
+        Returns the position that was written to.
+        """
+        self.basefile.seek(0, 2)
+        pos = self.basefile.tell()
+
+        # Find the earliest available free space
+        # (or, if free space reaches to the end of the file, use it)
+        for p in self.calc_waste()[1]:
+            if p[1] - p[0] >= len(data) or p[1] == pos:
+                pos = p[0]
+                self.basefile.seek(pos)
+                break
+
+        self.basefile.write(data)
+        return pos
+
+    def insert(self, name, data, index=None, use_free=True):
+        """Insert a new entry at the optional index (defaults to
+        appending).
+
+        If use_free is true, existing free space in the WAD will
+        be used, if possible."""
+        assert self.basefile
+        try:
+            index = self.select(index)
+        except:
+            index = None
+        self.issafe = False
+
+        if len(data) == 0:
+            pos = 0
+        elif use_free:
+            # write data to end of file or use free space if possible
+            pos = self.write_free(data)
+        else:
+            self.basefile.seek(0, 2)
+            pos = self.basefile.tell()
+            self.basefile.write(data)
+
+        if index is None:
+            self.entries.append(Entry(pos, len(data), name))
+        else:
+            self.entries.insert(index, Entry(pos, len(data), name))
+        self.basefile.flush()
+
+    def update(self, id, data):
+        """Write new data for an existing lump. If the new data is
+        bigger than what's present, a new position in the file will be
+        allocated for the lump."""
+        assert self.basefile
+        id = self.select(id)
+        if len(data) != self.entries[id].size:
+            self.issafe = False
+
+        if len(data) == 0:
+            self.entries[i].ptr = 0
+        elif len(data) <= self.entries[id].size:
+            self.write_at(self.entries[id].ptr, data)
+        else:
+            # temporarily mark existing entry as free, its current space will
+            # be combined with any adjacent free space
+            self.entries[id].size = 0
+            # write data to end of file or use free space if possible
+            self.entries[id].ptr = self.write_free(data)
+        self.entries[id].size = len(data)
+        self.basefile.flush()
+
+    def save(self):
+        """Save directory and header changes to the WAD file."""
+        assert self.basefile
+        if self.issafe: return
+        dir = join([e.pack() for e in self.entries])
+        self.header.dir_len = len(self.entries)
+        self.header.dir_ptr = self.write_free(dir)
+        self.write_at(0, self.header.pack())
+        self.basefile.flush()
+        self.issafe = True
+
+    def rewrite(self):
+        """Rewrite the entire WAD file. This removes all garbage
+        (wasted space) from the file."""
+        assert self.basefile
+        fpath = self.basefile.name
+        # Write to a temporary file and rename it when done
+        # os.tmpnam works too, but gives a security warning
+        tmppath = hashlib.md5(str(time.time())).hexdigest()[:8] + ".tmp"
+        tmppath = os.path.join(os.path.dirname(fpath), tmppath)
+        outwad = create_wad(tmppath)
+        for i in range(len(self.entries)):
+            outwad.insert(self.entries[i].name, self.read(i), use_free=False)
+        outwad.save()
+        outwad.close()
+        self.close()
+        os.remove(fpath)
+        os.rename(tmppath, fpath)
+        self.entries = []
+        self.open(fpath)
+        self.issafe = True
+
+    def calc_waste(self):
+        """Returns an (int, list) tuple containing the total amount of
+        wasted space in the WAD and a list of (start, end) tuples for
+        the spots where the wasted chunks are located."""
+        assert self.basefile
+        filesize = os.stat(self.basefile.name)[6]
+        # Create a list of (start, end) tuples to represent used space
+        chunks = []
+        # Treat the header and the end of the file as chunks of used space
+        chunks.append((0, 12))
+        chunks.append((filesize, filesize + 1))
+        # Add to the list the chunks that are occupied by lump data
+        chunks.append((self.header.dir_ptr, self.header.dir_ptr + \
+            len(self.entries)*ctypes.sizeof(Entry)))
+        for entry in self.entries:
+            if entry.size > 0:
+                chunks.append((entry.ptr, entry.ptr + entry.size))
+        # Sort it so we can go through it linearly and check for gaps
+        chunks.sort()
+        positions = []
+        space = 0
+        for i in range(0, len(chunks)-1):
+            # Check whether the end of the chunk touches the beginning of the
+            # next one. If not, there's wasted space between them.
+            if chunks[i][1] < chunks[i+1][0]:
+                positions.append((chunks[i][1], chunks[i+1][0]))
+                space += positions[-1][1] - positions[-1][0]
+        return space, positions
+
+    def info_text(self):
+        """Return printable fancy-formatted info about the WAD file."""
+        assert self.basefile
+        assert self.issafe
+        filesize = os.stat(self.basefile.name)[6]
+        s = []
+        # Main information
+        s.append("Info for %s\n\n" % self.basefile.name)
+        s.append("Type: %s\n" % self.header.type)
+        s.append("Size: %d bytes\n" % filesize)
+        s.append("Directory start: 0x%x" % self.header.dir_ptr)
+        # List all the lumps and some relevant information
+        s.append("\n\nEntries:\n\n     #  Name       Size       Position\n\n")
+        for i, entry in enumerate(self.entries):
+            s.append("%6i  %s %s 0x%x\n" %
+                (i, entry.name.ljust(10), str(entry.size).ljust(10), entry.ptr))
+        # Add info about wasted space in the WAD, to find out how much of an
+        # improvement a rewrite() would make
+        total, wasted = self.calc_waste()
+        s.append("\nWasted space:\n\n")
+        s.append("    %s bytes total\n" % str(total))
+        for w in wasted:
+            s.append("    %i bytes starting at 0x%x\n" % (w[1]-w[0], w[0]))
+        return ''.join(s)
```

### Comparing `omgifol-0.5.0/setup.py` & `omgifol-0.5.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-#!/usr/bin/env python
-
-from setuptools import setup, find_packages
-import glob
-
-setup(
-	name = 'omgifol',
-	version = '0.5.0',
-	description = 'A Python library for manipulation of Doom WAD files',
-	url = 'https://github.com/devinacker/omgifol',
-	author = 'Devin Acker, Fredrik Johansson',
-	author_email = 'd@revenant1.net',
-	license = 'MIT',
-	classifiers = [
-		'Development Status :: 3 - Alpha',
-		'License :: OSI Approved :: MIT License',
-		'Programming Language :: Python :: 3',
-		'Operating System :: OS Independent',
-	],
-	python_requires = ">=3.3",
-	packages = find_packages(exclude = ['demo']),
-	scripts = glob.glob("demo/*.py"),
-)
+#!/usr/bin/env python
+
+from setuptools import setup, find_packages
+import glob
+
+setup(
+	name = 'omgifol',
+	version = '0.5.1',
+	description = 'A Python library for manipulation of Doom WAD files',
+	url = 'https://github.com/devinacker/omgifol',
+	author = 'Devin Acker, Fredrik Johansson',
+	author_email = 'd@revenant1.net',
+	license = 'MIT',
+	classifiers = [
+		'Development Status :: 3 - Alpha',
+		'License :: OSI Approved :: MIT License',
+		'Programming Language :: Python :: 3',
+		'Operating System :: OS Independent',
+	],
+	python_requires = ">=3.3",
+	packages = find_packages(exclude = ['demo']),
+	scripts = glob.glob("demo/*.py"),
+)
```

