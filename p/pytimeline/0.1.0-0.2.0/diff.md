# Comparing `tmp/pytimeline-0.1.0.tar.gz` & `tmp/pytimeline-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytimeline-0.1.0.tar", max compression
+gzip compressed data, was "pytimeline-0.2.0.tar", max compression
```

## Comparing `pytimeline-0.1.0.tar` & `pytimeline-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     2735 2021-12-11 00:38:25.900931 pytimeline-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      614 2021-12-11 00:39:54.243370 pytimeline-0.1.0/pytimeline/__init__.py
--rw-r--r--   0        0        0        0 2021-12-11 00:34:23.473820 pytimeline-0.1.0/pytimeline/__main__.py
--rw-r--r--   0        0        0    11736 2021-12-11 00:37:58.760630 pytimeline-0.1.0/pytimeline/structures.py
--rw-r--r--   0        0        0      374 2021-12-10 22:05:50.822292 pytimeline-0.1.0/pytimeline/utils.py
--rw-r--r--   0        0        0      679 2021-12-11 00:41:31.749550 pytimeline-0.1.0/setup.py
--rw-r--r--   0        0        0      467 2021-12-11 00:41:31.749766 pytimeline-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2021-12-11 21:40:30.997561 pytimeline-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5181 2021-12-11 23:13:14.201967 pytimeline-0.2.0/README.md
+-rw-r--r--   0        0        0     3546 2021-12-11 21:47:34.975740 pytimeline-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      614 2021-12-11 21:40:46.658458 pytimeline-0.2.0/pytimeline/__init__.py
+-rw-r--r--   0        0        0     1249 2021-12-11 22:12:35.414873 pytimeline-0.2.0/pytimeline/__main__.py
+-rw-r--r--   0        0        0    11688 2021-12-11 22:57:01.436641 pytimeline-0.2.0/pytimeline/structures.py
+-rw-r--r--   0        0        0      976 2021-12-11 21:58:08.599332 pytimeline-0.2.0/pytimeline/utils.py
+-rw-r--r--   0        0        0     6091 2021-12-11 23:14:24.278543 pytimeline-0.2.0/setup.py
+-rw-r--r--   0        0        0     6427 2021-12-11 23:14:24.278940 pytimeline-0.2.0/PKG-INFO
```

### Comparing `pytimeline-0.1.0/pyproject.toml` & `pytimeline-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,39 @@
 [tool.poetry]
 name = "pytimeline"
-version = "0.1.0"
-description = ""
-authors = ["Felix Soubelet <felix.soubelet@protonmail.com>"]
+version = "0.2.0"
+description = "A library for creating and cleaning SVG timelines."
+authors = ["Felix Soubelet <felix.soubelet@cern.ch>"]
+license = "MIT"
+packages = [{include = "pytimeline"}]
+readme = "README.md"
+repository = "https://github.com/fsoubelet/Timeline"
+keywords = ["Timeline", "SVG", "Generator"]
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: End Users/Desktop",
+    "License :: OSI Approved :: MIT License",
+    "Natural Language :: English",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Topic :: Scientific/Engineering :: Visualization",
+    "Topic :: Utilities",
+]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-svgwrite = "^1.4.1"
-pendulum = "^2.1.2"
+svgwrite = "^1.4"
+pendulum = "^2.1"
 loguru = "^0.5.3"
-click = "^8.0.3"
+click = "^8.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 isort = "^5.10.1"
 black = "^21.12b0"
 pylint = "^2.12.2"
 mypy = "^0.910"
```

### Comparing `pytimeline-0.1.0/pytimeline/__init__.py` & `pytimeline-0.2.0/pytimeline/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 """
 
 from .structures import Timeline
 
 __title__ = "pytimeline"
 __description__ = "A library for creating and cleaning SVG timelines."
 __url__ = "https://github.com/fsoubelet/Timeline"
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 __author__ = "Felix Soubelet"
 __author_email__ = "felix.soubelet@cern.ch"
 __license__ = "MIT"
```

### Comparing `pytimeline-0.1.0/pytimeline/structures.py` & `pytimeline-0.2.0/pytimeline/structures.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,69 +41,69 @@
         self.markers: Dict[str, Tuple[Marker, Marker]] = {}
         self.text_fudge = (3, 1.5)
         self.width = self.data["width"]
         self.tick_format = self.data.get("tick_format", DATE_FORMAT)
         self.max_label_height = 0  # max height of all axis labels, used for final height computation
 
         # ----- Drawing ----- #
-        logger.debug("Creating SVG drawing")
+        logger.debug("Preparing SVG drawing object")
         self.drawing = svgwrite.Drawing()
         self.drawing["width"] = self.width
         self.g_axis = self.drawing.g()
 
         logger.debug("Parsing dates")
         self.start_date: DateTime = pendulum.parse(self.data["start"], strict=False)
         self.end_date: DateTime = pendulum.parse(self.data["end"], strict=False)
         padding: Duration = 0.1 * (self.end_date - self.start_date)
         self.date0: DateTime = self.start_date - padding
         self.date1: DateTime = self.end_date + padding
         self.total_seconds: int = (self.date1 - self.date0).in_seconds()
 
         # ----- Tkinter ----- #
-        logger.debug("Initializing tkinter")
+        logger.debug("Initializing tkinter for fonts")
         self.tk_root = tkinter.Tk()
         self.fonts = {}
 
     def build(self):
         logger.info("Building timeline")
         y_era = 10  # draw era label and markers at this height
 
-        self.create_main_axis()
-        y_callouts = self.create_callouts()  # keep track of the callouts' heights
+        self._create_main_axis()
+        y_callouts = self._create_callouts()  # keep track of the callouts' heights
         y_axis = y_era + Callout.height - y_callouts  # axis position to avoid overlap with eras
         height = (
             y_axis + self.max_label_height + 4 * self.text_fudge[1]
         )  # height so that eras, callouts, axis & labels just fit
-        self.create_eras(y_era, y_axis, height)
-        self.create_era_axis_labels()
+        self._create_eras(y_era, y_axis, height)
+        self._create_era_axis_labels()
         self.g_axis.translate(0, y_axis)  # translate the axis group and add it to the drawing
         self.drawing.add(self.g_axis)
         self.drawing["height"] = height  # finally set the height on the drawing
 
     def save(self, filename: Union[str, Path]) -> None:
+        logger.info(f"Saving timeline to disk at '{filename.absolute()}'")
         self.drawing.saveas(filename)
 
     def to_string(self) -> str:
         return self.drawing.tostring()
 
-    def create_eras(self, y_era, y_axis, height):
+    def _create_eras(self, y_era, y_axis, height):
         if "eras" not in self.data:
             return
 
-        logger.debug("Drawing eras")
+        logger.info("Drawing eras")
         markers = {}
         for era in self.data["eras"]:
             name = era[0]
             t0 = pendulum.parse(era[1], strict=False)
             t1 = pendulum.parse(era[2], strict=False)
             logger.debug(f"Creating era '{name}'")
             fill_color = era[3] if len(era) > 3 else Colors.gray
 
-            logger.trace(f"Getting marker objects for era")
-            start_marker, end_marker = self.get_markers(fill_color)
+            start_marker, end_marker = self._get_markers(fill_color)
 
             logger.trace(f"Creating boundary lines")
             percent_width0 = (t0 - self.date0).in_seconds() / self.total_seconds
             percent_width1 = (t1 - self.date0).in_seconds() / self.total_seconds
             x0 = int(percent_width0 * self.width + 0.5)
             x1 = int(percent_width1 * self.width + 0.5)
             rectangle = self.drawing.add(self.drawing.rect((x0, 0), (x1 - x0, height)))
@@ -132,94 +132,92 @@
                     fill=fill_color,
                     font_family="Helevetica",
                     font_size="6pt",
                     text_anchor="middle",
                 )
             )
 
-    def get_markers(self, color: str) -> Tuple[Marker, Marker]:
-        logger.debug(f"Getting markers for color '{color}'")
+    def _get_markers(self, color: str) -> Tuple[Marker, Marker]:
+        logger.trace(f"Getting markers for color '{color}'")
         if color in self.markers:
             return self.markers[color]
 
         start_marker: Marker = self.drawing.marker(insert=(0, 3), size=(10, 10), orient="auto")
         start_marker.add(self.drawing.path("M6,0 L6,7 L0,3 L6,0", fill=color))
         self.drawing.defs.add(start_marker)
 
         end_marker = self.drawing.marker(insert=(6, 3), size=(10, 10), orient="auto")
         end_marker.add(self.drawing.path("M0,0 L0,7 L6,3 L0,0", fill=color))
         self.drawing.defs.add(end_marker)
 
         self.markers[color] = (start_marker, end_marker)
         return start_marker, end_marker
 
-    def create_main_axis(self) -> None:
-        logger.debug("Drawing main axis line")
+    def _create_main_axis(self) -> None:
+        logger.info("Drawing main axis line")
         self.g_axis.add(self.drawing.line((0, 0), (self.width, 0), stroke=Colors.black, stroke_width=3))
 
-        logger.trace("Adding tickmarks")
-        self.add_axis_label(self.start_date, self.start_date.format(DATE_FORMAT), tick=True)
-        self.add_axis_label(self.end_date, self.end_date.format(DATE_FORMAT), tick=True)
+        logger.info("Adding tickmarks")
+        self._add_axis_label(self.start_date, self.start_date.format(DATE_FORMAT), tick=True)
+        self._add_axis_label(self.end_date, self.end_date.format(DATE_FORMAT), tick=True)
 
         if "num_ticks" in self.data:
             num_ticks = int(self.data["num_ticks"])
-            logger.trace("Dividing period in {num_ticks} ticks")
+            logger.trace(f"Dividing period in {num_ticks} ticks")
             seconds = (self.end_date - self.start_date).in_seconds()
             for j in range(1, num_ticks):
                 tickmark_date: DateTime = self.start_date.add(seconds=j * seconds / num_ticks)
-                self.add_axis_label(tickmark_date, tickmark_date.format(DATE_FORMAT), tick=True)
+                self._add_axis_label(tickmark_date, tickmark_date.format(DATE_FORMAT), tick=True)
 
-    def create_era_axis_labels(self) -> None:
+    def _create_era_axis_labels(self) -> None:
         if "eras" not in self.data:
             return
 
         for era in self.data["eras"]:
             logger.trace(f"Creating axis labels for era '{era[0]}'")
             t0 = pendulum.parse(era[1], strict=False)
             t1 = pendulum.parse(era[2], strict=False)
-            self.add_axis_label(t0, t0.format(DATE_FORMAT), tick=False, fill=Colors.black)
-            self.add_axis_label(t1, t1.format(DATE_FORMAT), tick=False, fill=Colors.black)
+            self._add_axis_label(t0, t0.format(DATE_FORMAT), tick=False, fill=Colors.black)
+            self._add_axis_label(t1, t1.format(DATE_FORMAT), tick=False, fill=Colors.black)
 
-    def add_axis_label(self, dt: DateTime, label: str, **kwargs):
+    def _add_axis_label(self, dt: DateTime, label: str, **kwargs):
         logger.trace(f"Adding axis label '{label}'")
         percent_width: float = (dt - self.date0).in_seconds() / self.total_seconds
         if percent_width < 0 or percent_width > 1:
             return
 
         dy = 5
         x = int(percent_width * self.width + 0.5)
 
-        logger.trace(f"Adding tickmark")
         add_tick = kwargs.get("tick", True)
         if add_tick:
             stroke = kwargs.get("stroke", Colors.black)
             self.g_axis.add(self.drawing.line((x, -dy), (x, dy), stroke=stroke, stroke_width=2))
 
-        logger.trace(f"Adding label")
         self.g_axis.add(
             self.drawing.text(
                 label,
                 insert=(x, -2 * dy),
                 stroke="none",
                 fill=kwargs.get("fill", Colors.gray),
                 font_family="Helevetica",
                 font_size="6pt",
                 text_anchor="end",
                 writing_mode="tb",
                 transform=f"rotate(180, {x:d}, 0)",
             )
         )
-        h = self.get_text_metrics("Helevetica", 6, label)[0] + 2 * dy
+        h = self._get_text_metrics("Helevetica", 6, label)[0] + 2 * dy
         self.max_label_height = max(self.max_label_height, h)
 
-    def create_callouts(self) -> float:
+    def _create_callouts(self) -> float:
         if "callouts" not in self.data:
             return
 
-        logger.debug("Creating callouts")
+        logger.info("Adding callouts")
         callouts_data: List[str] = self.data["callouts"]
         min_y = float("inf")
         sorted_dates: List[DateTime] = []
         inv_callouts: Dict[DateTime, Tuple[str, str]] = {}  # {date: (name, color)}
 
         for callout in callouts_data:
             event_name: str = callout[0]
@@ -227,28 +225,28 @@
             event_color: str = callout[2] if len(callout) > 2 else Colors.black
             sorted_dates.append(event_date)
             if event_date not in inv_callouts:
                 inv_callouts[event_date] = []
             inv_callouts[event_date].append((event_name, event_color))
         sorted_dates.sort()
 
-        logger.debug("Adding callouts")  # one by one, making sure they don't overlap
+        # Adding callouts one by one, making sure they don't overlap
         prev_x = [float("-inf")]
         prev_level = [-1]
         for event_date in sorted_dates:
             event_name, event_color = inv_callouts[event_date].pop()  # (str, str)
             percent_width: float = (event_date - self.date0).in_seconds() / self.total_seconds
             if percent_width < 0 or percent_width > 1:
                 continue
             x = int(percent_width * self.width + 0.5)
             # figure out what 'level" to make the callout on
             k = 0
             i = len(prev_x) - 1
             left = x - (
-                self.get_text_metrics("Helevetica", 6, event_name)[0] + Callout.width + self.text_fudge[0]
+                self._get_text_metrics("Helevetica", 6, event_name)[0] + Callout.width + self.text_fudge[0]
             )
             while left < prev_x[i] and i >= 0:
                 k = max(k, prev_level[i] + 1)
                 i -= 1
             y = 0 - Callout.height - k * Callout.increment
             min_y = min(min_y, y)
             # self.drawing.add(self.drawing.circle((left, y), stroke='red', stroke_width=2))
@@ -264,23 +262,23 @@
                     stroke="none",
                     fill=event_color,
                     font_family="Helevetica",
                     font_size="6pt",
                     text_anchor="end",
                 )
             )
-            self.add_axis_label(event_date, event_date.format(DATE_FORMAT), tick=False, fill=Colors.black)
+            self._add_axis_label(event_date, event_date.format(DATE_FORMAT), tick=False, fill=Colors.black)
             self.g_axis.add(
                 self.drawing.circle((x, 0), r=4, stroke=event_color, stroke_width=1, fill="white")
             )
             prev_x.append(x)
             prev_level.append(k)
         return min_y
 
-    def get_text_metrics(self, family: str, size: int, text: str) -> Tuple[int, int]:
+    def _get_text_metrics(self, family: str, size: int, text: str) -> Tuple[int, int]:
         key = (family, size)
         if key in self.fonts:
             font = self.fonts[key]
         else:
             font = tkinter.font.Font(self.tk_root, family=family, size=size)
             self.fonts[key] = font
         assert font is not None
```

