# Comparing `tmp/pyttygif-0.3.1.tar.gz` & `tmp/pyttygif-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyttygif-0.3.1.tar", last modified: Tue Oct 25 22:05:13 2022, max compression
+gzip compressed data, was "pyttygif-0.3.2.tar", last modified: Wed May 24 16:08:24 2023, max compression
```

## Comparing `pyttygif-0.3.1.tar` & `pyttygif-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 administrator  (1000) administrator  (1000)        0 2022-10-25 22:05:13.910299 pyttygif-0.3.1/
--rw-r--r--   0 administrator  (1000) administrator  (1000)     1203 2019-07-01 06:53:22.000000 pyttygif-0.3.1/.gitignore
--rw-r--r--   0 administrator  (1000) administrator  (1000)    35149 2019-07-01 06:53:22.000000 pyttygif-0.3.1/LICENSE
--rw-r--r--   0 administrator  (1000) administrator  (1000)       43 2019-07-03 06:36:33.000000 pyttygif-0.3.1/MANIFEST.in
--rw-r--r--   0 administrator  (1000) administrator  (1000)     9801 2022-10-25 22:05:13.910299 pyttygif-0.3.1/PKG-INFO
--rw-r--r--   0 administrator  (1000) administrator  (1000)     9109 2022-10-25 21:24:28.000000 pyttygif-0.3.1/README.md
-drwxr-xr-x   0 administrator  (1000) administrator  (1000)        0 2022-10-25 22:05:13.909299 pyttygif-0.3.1/pyttygif/
--rw-r--r--   0 administrator  (1000) administrator  (1000)      713 2019-06-28 19:41:32.000000 pyttygif-0.3.1/pyttygif/__init__.py
--rw-r--r--   0 administrator  (1000) administrator  (1000)    11432 2022-10-25 22:02:57.000000 pyttygif-0.3.1/pyttygif/__main__.py
--rw-r--r--   0 administrator  (1000) administrator  (1000)     2394 2019-07-02 18:55:18.000000 pyttygif-0.3.1/pyttygif/capture.py
--rw-r--r--   0 administrator  (1000) administrator  (1000)     4908 2019-09-02 17:34:42.000000 pyttygif-0.3.1/pyttygif/gifbuilder.py
--rw-r--r--   0 administrator  (1000) administrator  (1000)     5892 2022-10-25 20:55:58.000000 pyttygif-0.3.1/pyttygif/ttyplay.py
-drwxr-xr-x   0 administrator  (1000) administrator  (1000)        0 2022-10-25 22:05:13.909299 pyttygif-0.3.1/pyttygif.egg-info/
--rw-r--r--   0 administrator  (1000) administrator  (1000)     9801 2022-10-25 22:05:13.000000 pyttygif-0.3.1/pyttygif.egg-info/PKG-INFO
--rw-r--r--   0 administrator  (1000) administrator  (1000)      282 2022-10-25 22:05:13.000000 pyttygif-0.3.1/pyttygif.egg-info/SOURCES.txt
--rw-r--r--   0 administrator  (1000) administrator  (1000)        1 2022-10-25 22:05:13.000000 pyttygif-0.3.1/pyttygif.egg-info/dependency_links.txt
--rw-r--r--   0 administrator  (1000) administrator  (1000)        9 2022-10-25 22:05:13.000000 pyttygif-0.3.1/pyttygif.egg-info/top_level.txt
--rw-r--r--   0 administrator  (1000) administrator  (1000)       38 2022-10-25 22:05:13.910299 pyttygif-0.3.1/setup.cfg
--rw-r--r--   0 administrator  (1000) administrator  (1000)      898 2022-10-25 22:04:49.000000 pyttygif-0.3.1/setup.py
+drwxr-xr-x   0 administrator  (1000) administrator  (1000)        0 2023-05-24 16:08:24.688837 pyttygif-0.3.2/
+-rw-r--r--   0 administrator  (1000) administrator  (1000)     1203 2019-07-01 06:53:22.000000 pyttygif-0.3.2/.gitignore
+-rw-r--r--   0 administrator  (1000) administrator  (1000)    35149 2019-07-01 06:53:22.000000 pyttygif-0.3.2/LICENSE
+-rw-r--r--   0 administrator  (1000) administrator  (1000)       43 2019-07-03 06:36:33.000000 pyttygif-0.3.2/MANIFEST.in
+-rw-r--r--   0 administrator  (1000) administrator  (1000)     9645 2023-05-24 16:08:24.688837 pyttygif-0.3.2/PKG-INFO
+-rw-r--r--   0 administrator  (1000) administrator  (1000)     8953 2023-05-24 15:47:02.000000 pyttygif-0.3.2/README.md
+drwxr-xr-x   0 administrator  (1000) administrator  (1000)        0 2023-05-24 16:08:24.688837 pyttygif-0.3.2/pyttygif/
+-rw-r--r--   0 administrator  (1000) administrator  (1000)      713 2019-06-28 19:41:32.000000 pyttygif-0.3.2/pyttygif/__init__.py
+-rw-r--r--   0 administrator  (1000) administrator  (1000)    11465 2023-05-24 15:43:57.000000 pyttygif-0.3.2/pyttygif/__main__.py
+-rw-r--r--   0 administrator  (1000) administrator  (1000)     2394 2023-05-24 15:43:00.000000 pyttygif-0.3.2/pyttygif/capture.py
+-rw-r--r--   0 administrator  (1000) administrator  (1000)     4908 2023-05-24 15:43:00.000000 pyttygif-0.3.2/pyttygif/gifbuilder.py
+-rw-r--r--   0 administrator  (1000) administrator  (1000)     5892 2022-10-25 20:55:58.000000 pyttygif-0.3.2/pyttygif/ttyplay.py
+drwxr-xr-x   0 administrator  (1000) administrator  (1000)        0 2023-05-24 16:08:24.688837 pyttygif-0.3.2/pyttygif.egg-info/
+-rw-r--r--   0 administrator  (1000) administrator  (1000)     9645 2023-05-24 16:08:24.000000 pyttygif-0.3.2/pyttygif.egg-info/PKG-INFO
+-rw-r--r--   0 administrator  (1000) administrator  (1000)      282 2023-05-24 16:08:24.000000 pyttygif-0.3.2/pyttygif.egg-info/SOURCES.txt
+-rw-r--r--   0 administrator  (1000) administrator  (1000)        1 2023-05-24 16:08:24.000000 pyttygif-0.3.2/pyttygif.egg-info/dependency_links.txt
+-rw-r--r--   0 administrator  (1000) administrator  (1000)        9 2023-05-24 16:08:24.000000 pyttygif-0.3.2/pyttygif.egg-info/top_level.txt
+-rw-r--r--   0 administrator  (1000) administrator  (1000)       38 2023-05-24 16:08:24.688837 pyttygif-0.3.2/setup.cfg
+-rw-r--r--   0 administrator  (1000) administrator  (1000)      898 2023-05-24 15:47:07.000000 pyttygif-0.3.2/setup.py
```

### Comparing `pyttygif-0.3.1/.gitignore` & `pyttygif-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyttygif-0.3.1/LICENSE` & `pyttygif-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyttygif-0.3.1/PKG-INFO` & `pyttygif-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyttygif
-Version: 0.3.1
+Version: 0.3.2
 Summary: ttyrec to GIF converter
 Home-page: https://github.com/tmp6154/pyttygif
 Author: Vitaly Ostrosablin
 Author-email: tmp6154@yandex.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -58,15 +58,15 @@
 
     python3 -m pyttygif sample.ttyrec ./sample.gif
 
 ## Usage
 
     usage: __main__.py [-h] [-s SPEED] [-l LOOP] [-L LASTFRAME] [-m]
                        [-o {0,1,2,3}] [-S] [-b MAX_BACKLOG] [-D] [-f FPS]
-                       [-c DELAYCAP] [-x LOSSY] [-e ENCODING] [-C [LOGARITHMIC]]
+                       [-c DELAYCAP] [-x LOSSY] [-e ENCODING] [-C]
                        input output
 
     Convert ttyrec to GIF animation
 
     options:
       -h, --help            show this help message and exit
 
@@ -92,31 +92,31 @@
       -f FPS, --fps FPS     How many frames to screenshot per second
       -c DELAYCAP, --delaycap DELAYCAP
                             Cap the display time of single frame (in seconds)
       -x LOSSY, --lossy LOSSY
                             Use gifsicle lossy GIF compression mode
       -e ENCODING, --encoding ENCODING
                             Reencode ttyrec to match terminal (source:target)
-      -C [LOGARITHMIC], --logarithmic [LOGARITHMIC]
-                            Enable logarithmic time compression (default base = e)
+      -C, --logarithmic
+                            Enable logarithmic time compression (base = e)
 
 For the most basic usage, you only need to specify the required positional arguments (input ttyrec file path and output GIF file path). You can also specify **-s** to pass (floating point) speed multiplier to speed up or slow down the output GIF and **-l** to specify number of times to play the GIF (0 = infinity).
 
 There's also a number of advanced options available.
 
 * ttyrec format doesn't define display time of the last frame. However, you can alter display time of the last frame of the GIF with **-L** option (floating point number). It defaults to 5 seconds.
 * pyttygif defaults to try to reduce RAM usage. If you want to speed up the conversion though, you can try to use **-m** flag (tells gifsicle to keep frames in RAM) and **-b** option, which adjusts the maximum number of frames to queue in RAM and defaults to the number of logical cores in the machine. It's not recommended to set it to less than number of cores. You can also set it to 0 (unlimited), however this is also not recommended because if your machine is unable to process all frames in time - it could eat all available RAM with a sufficiently long ttyrec.
 * gifsicle optimization level defaults to 2, however you can override it with **-o** option and set it within range of 0-3 (where 0 is no optimization at all, tends to create huge GIFs, and 3 is maximum, but possibly slower).
 * pyttygif attempts to inhibit screensaver by default (so that you don't have to move mouse during recording of the GIF to prevent screenlocker). However, if you don't want that for some reason (or don't have xdg-screensaver installed) - you might want to override it with **-S** flag.
 * pyttygif clears the screen before recording it. However, if you want previous terminal content to be captured, you can pass in **-D** flag.
 * pyttygif doesn't have any way to sync to the terminal emulator (and it also wants to be as much terminal-agnostic as possible), so the only way around this problem is to sleep a fixed amount of time after each displayed frame to give the terminal emulator some time to render the contents. pyttygif defaults to the more or less safe value of 25 FPS (which is 0.04 seconds of sleep after each frame). However, depending on your machine, you might want to override this, for example, with 60 FPS. You can specify the FPS with **-f** option. But beware of setting this value too high - it's possible that pyttygif would actually capture the previous frame, which would cause stutters and frame skips in the output GIF.
 * If there's an excessively long delays in the input ttyrec (such as when user goes away from keyboard) - it's possible to cap such delays by passing **-c** option and specifying a maximum time in seconds that frame can take (floating point number). If any frame exceeds specified time - it's forcibly capped at that time. It defaults to positive infinity, that is, no capping.
 * If you have gifsicle 1.92 or newer, you can use lossy compression mode, which allows to produce even smaller GIFs by passing **-x** option and specify compression level, where higher level produces smaller GIFs at the cost of more artifacts.
 * If your ttyrecs are in different encoding that your terminal (e.g. NetHack IBMgraphics aka CP437), you can re-encode ttyrec on-the-fly by passing **-e** option and specifying ttyrec encoding, followed by colon-separated current terminal encoding (e.g. **-e=cp437:utf-8**).
-* If your ttyrecs contain large inactivity periods, you might want to enable logarithmic time compression by passing **-C** option. By default, natural logarithm (base e) is used, like in IPBT, however you may optionally specify any other valid base (e.g. **-C=2** for base 2 logarithm). This option will cause delays to be scaled non-linearly. Extremely large delays will be compressed significantly (e.g. hour-long delay will turn into several seconds), while small delays will have negligible difference. It works together with speed adjustment, too.
+* If your ttyrecs contain large inactivity periods, you might want to enable logarithmic time compression by passing **-C** option. Like in IPBT, natural logarithm (base e) is used. This option will cause delays to be scaled non-linearly. Extremely large delays will be compressed significantly (e.g. hour-long delay will turn into several seconds), while small delays will have negligible difference. It works together with speed adjustment, too.
 
 Delay transform order:
 
 First, we apply logarithmic time compression (**-C**) if enabled. Then, speed multiplier (**-s**) will be applied to adjust delays to desired speed. Finally, delays are hard-capped (**-c**), so that if any delay exceeds the cap value (which is positive infinity by default), it will be replaced with cap value.
 
 ## License
```

### Comparing `pyttygif-0.3.1/README.md` & `pyttygif-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     python3 -m pyttygif sample.ttyrec ./sample.gif
 
 ## Usage
 
     usage: __main__.py [-h] [-s SPEED] [-l LOOP] [-L LASTFRAME] [-m]
                        [-o {0,1,2,3}] [-S] [-b MAX_BACKLOG] [-D] [-f FPS]
-                       [-c DELAYCAP] [-x LOSSY] [-e ENCODING] [-C [LOGARITHMIC]]
+                       [-c DELAYCAP] [-x LOSSY] [-e ENCODING] [-C]
                        input output
 
     Convert ttyrec to GIF animation
 
     options:
       -h, --help            show this help message and exit
 
@@ -74,31 +74,31 @@
       -f FPS, --fps FPS     How many frames to screenshot per second
       -c DELAYCAP, --delaycap DELAYCAP
                             Cap the display time of single frame (in seconds)
       -x LOSSY, --lossy LOSSY
                             Use gifsicle lossy GIF compression mode
       -e ENCODING, --encoding ENCODING
                             Reencode ttyrec to match terminal (source:target)
-      -C [LOGARITHMIC], --logarithmic [LOGARITHMIC]
-                            Enable logarithmic time compression (default base = e)
+      -C, --logarithmic
+                            Enable logarithmic time compression (base = e)
 
 For the most basic usage, you only need to specify the required positional arguments (input ttyrec file path and output GIF file path). You can also specify **-s** to pass (floating point) speed multiplier to speed up or slow down the output GIF and **-l** to specify number of times to play the GIF (0 = infinity).
 
 There's also a number of advanced options available.
 
 * ttyrec format doesn't define display time of the last frame. However, you can alter display time of the last frame of the GIF with **-L** option (floating point number). It defaults to 5 seconds.
 * pyttygif defaults to try to reduce RAM usage. If you want to speed up the conversion though, you can try to use **-m** flag (tells gifsicle to keep frames in RAM) and **-b** option, which adjusts the maximum number of frames to queue in RAM and defaults to the number of logical cores in the machine. It's not recommended to set it to less than number of cores. You can also set it to 0 (unlimited), however this is also not recommended because if your machine is unable to process all frames in time - it could eat all available RAM with a sufficiently long ttyrec.
 * gifsicle optimization level defaults to 2, however you can override it with **-o** option and set it within range of 0-3 (where 0 is no optimization at all, tends to create huge GIFs, and 3 is maximum, but possibly slower).
 * pyttygif attempts to inhibit screensaver by default (so that you don't have to move mouse during recording of the GIF to prevent screenlocker). However, if you don't want that for some reason (or don't have xdg-screensaver installed) - you might want to override it with **-S** flag.
 * pyttygif clears the screen before recording it. However, if you want previous terminal content to be captured, you can pass in **-D** flag.
 * pyttygif doesn't have any way to sync to the terminal emulator (and it also wants to be as much terminal-agnostic as possible), so the only way around this problem is to sleep a fixed amount of time after each displayed frame to give the terminal emulator some time to render the contents. pyttygif defaults to the more or less safe value of 25 FPS (which is 0.04 seconds of sleep after each frame). However, depending on your machine, you might want to override this, for example, with 60 FPS. You can specify the FPS with **-f** option. But beware of setting this value too high - it's possible that pyttygif would actually capture the previous frame, which would cause stutters and frame skips in the output GIF.
 * If there's an excessively long delays in the input ttyrec (such as when user goes away from keyboard) - it's possible to cap such delays by passing **-c** option and specifying a maximum time in seconds that frame can take (floating point number). If any frame exceeds specified time - it's forcibly capped at that time. It defaults to positive infinity, that is, no capping.
 * If you have gifsicle 1.92 or newer, you can use lossy compression mode, which allows to produce even smaller GIFs by passing **-x** option and specify compression level, where higher level produces smaller GIFs at the cost of more artifacts.
 * If your ttyrecs are in different encoding that your terminal (e.g. NetHack IBMgraphics aka CP437), you can re-encode ttyrec on-the-fly by passing **-e** option and specifying ttyrec encoding, followed by colon-separated current terminal encoding (e.g. **-e=cp437:utf-8**).
-* If your ttyrecs contain large inactivity periods, you might want to enable logarithmic time compression by passing **-C** option. By default, natural logarithm (base e) is used, like in IPBT, however you may optionally specify any other valid base (e.g. **-C=2** for base 2 logarithm). This option will cause delays to be scaled non-linearly. Extremely large delays will be compressed significantly (e.g. hour-long delay will turn into several seconds), while small delays will have negligible difference. It works together with speed adjustment, too.
+* If your ttyrecs contain large inactivity periods, you might want to enable logarithmic time compression by passing **-C** option. Like in IPBT, natural logarithm (base e) is used. This option will cause delays to be scaled non-linearly. Extremely large delays will be compressed significantly (e.g. hour-long delay will turn into several seconds), while small delays will have negligible difference. It works together with speed adjustment, too.
 
 Delay transform order:
 
 First, we apply logarithmic time compression (**-C**) if enabled. Then, speed multiplier (**-s**) will be applied to adjust delays to desired speed. Finally, delays are hard-capped (**-c**), so that if any delay exceeds the cap value (which is positive infinity by default), it will be replaced with cap value.
 
 ## License
```

### Comparing `pyttygif-0.3.1/pyttygif/__init__.py` & `pyttygif-0.3.2/pyttygif/__init__.py`

 * *Files identical despite different names*

### Comparing `pyttygif-0.3.1/pyttygif/__main__.py` & `pyttygif-0.3.2/pyttygif/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,19 +138,17 @@
                       help="How many frames to screenshot per second")
 advgroup.add_argument('-c', '--delaycap', default=float('+inf'), type=float,
                       help="Cap the display time of single frame (in seconds)")
 advgroup.add_argument('-x', '--lossy', default=None, type=int,
                       help="Use gifsicle lossy GIF compression mode")
 advgroup.add_argument('-e', '--encoding', default=None,
                       help="Reencode ttyrec to match terminal (source:target)")
-advgroup.add_argument(
-    '-C', '--logarithmic', const=math.e, default=0,
-    type=float, nargs="?",
-    help="Enable logarithmic time compression (default base = e)"
-)
+advgroup.add_argument('-C', '--logarithmic', const=math.e, default=0,
+                      type=float, action="store_const",
+                      help="Enable logarithmic time compression (base = e)")
 
 try:
     args = parser.parse_args()
 except argparse.ArgumentError:
     parser.print_help()
     sys.exit(0)
```

### Comparing `pyttygif-0.3.1/pyttygif/capture.py` & `pyttygif-0.3.2/pyttygif/capture.py`

 * *Files identical despite different names*

### Comparing `pyttygif-0.3.1/pyttygif/gifbuilder.py` & `pyttygif-0.3.2/pyttygif/gifbuilder.py`

 * *Files identical despite different names*

### Comparing `pyttygif-0.3.1/pyttygif/ttyplay.py` & `pyttygif-0.3.2/pyttygif/ttyplay.py`

 * *Files identical despite different names*

### Comparing `pyttygif-0.3.1/pyttygif.egg-info/PKG-INFO` & `pyttygif-0.3.2/pyttygif.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyttygif
-Version: 0.3.1
+Version: 0.3.2
 Summary: ttyrec to GIF converter
 Home-page: https://github.com/tmp6154/pyttygif
 Author: Vitaly Ostrosablin
 Author-email: tmp6154@yandex.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -58,15 +58,15 @@
 
     python3 -m pyttygif sample.ttyrec ./sample.gif
 
 ## Usage
 
     usage: __main__.py [-h] [-s SPEED] [-l LOOP] [-L LASTFRAME] [-m]
                        [-o {0,1,2,3}] [-S] [-b MAX_BACKLOG] [-D] [-f FPS]
-                       [-c DELAYCAP] [-x LOSSY] [-e ENCODING] [-C [LOGARITHMIC]]
+                       [-c DELAYCAP] [-x LOSSY] [-e ENCODING] [-C]
                        input output
 
     Convert ttyrec to GIF animation
 
     options:
       -h, --help            show this help message and exit
 
@@ -92,31 +92,31 @@
       -f FPS, --fps FPS     How many frames to screenshot per second
       -c DELAYCAP, --delaycap DELAYCAP
                             Cap the display time of single frame (in seconds)
       -x LOSSY, --lossy LOSSY
                             Use gifsicle lossy GIF compression mode
       -e ENCODING, --encoding ENCODING
                             Reencode ttyrec to match terminal (source:target)
-      -C [LOGARITHMIC], --logarithmic [LOGARITHMIC]
-                            Enable logarithmic time compression (default base = e)
+      -C, --logarithmic
+                            Enable logarithmic time compression (base = e)
 
 For the most basic usage, you only need to specify the required positional arguments (input ttyrec file path and output GIF file path). You can also specify **-s** to pass (floating point) speed multiplier to speed up or slow down the output GIF and **-l** to specify number of times to play the GIF (0 = infinity).
 
 There's also a number of advanced options available.
 
 * ttyrec format doesn't define display time of the last frame. However, you can alter display time of the last frame of the GIF with **-L** option (floating point number). It defaults to 5 seconds.
 * pyttygif defaults to try to reduce RAM usage. If you want to speed up the conversion though, you can try to use **-m** flag (tells gifsicle to keep frames in RAM) and **-b** option, which adjusts the maximum number of frames to queue in RAM and defaults to the number of logical cores in the machine. It's not recommended to set it to less than number of cores. You can also set it to 0 (unlimited), however this is also not recommended because if your machine is unable to process all frames in time - it could eat all available RAM with a sufficiently long ttyrec.
 * gifsicle optimization level defaults to 2, however you can override it with **-o** option and set it within range of 0-3 (where 0 is no optimization at all, tends to create huge GIFs, and 3 is maximum, but possibly slower).
 * pyttygif attempts to inhibit screensaver by default (so that you don't have to move mouse during recording of the GIF to prevent screenlocker). However, if you don't want that for some reason (or don't have xdg-screensaver installed) - you might want to override it with **-S** flag.
 * pyttygif clears the screen before recording it. However, if you want previous terminal content to be captured, you can pass in **-D** flag.
 * pyttygif doesn't have any way to sync to the terminal emulator (and it also wants to be as much terminal-agnostic as possible), so the only way around this problem is to sleep a fixed amount of time after each displayed frame to give the terminal emulator some time to render the contents. pyttygif defaults to the more or less safe value of 25 FPS (which is 0.04 seconds of sleep after each frame). However, depending on your machine, you might want to override this, for example, with 60 FPS. You can specify the FPS with **-f** option. But beware of setting this value too high - it's possible that pyttygif would actually capture the previous frame, which would cause stutters and frame skips in the output GIF.
 * If there's an excessively long delays in the input ttyrec (such as when user goes away from keyboard) - it's possible to cap such delays by passing **-c** option and specifying a maximum time in seconds that frame can take (floating point number). If any frame exceeds specified time - it's forcibly capped at that time. It defaults to positive infinity, that is, no capping.
 * If you have gifsicle 1.92 or newer, you can use lossy compression mode, which allows to produce even smaller GIFs by passing **-x** option and specify compression level, where higher level produces smaller GIFs at the cost of more artifacts.
 * If your ttyrecs are in different encoding that your terminal (e.g. NetHack IBMgraphics aka CP437), you can re-encode ttyrec on-the-fly by passing **-e** option and specifying ttyrec encoding, followed by colon-separated current terminal encoding (e.g. **-e=cp437:utf-8**).
-* If your ttyrecs contain large inactivity periods, you might want to enable logarithmic time compression by passing **-C** option. By default, natural logarithm (base e) is used, like in IPBT, however you may optionally specify any other valid base (e.g. **-C=2** for base 2 logarithm). This option will cause delays to be scaled non-linearly. Extremely large delays will be compressed significantly (e.g. hour-long delay will turn into several seconds), while small delays will have negligible difference. It works together with speed adjustment, too.
+* If your ttyrecs contain large inactivity periods, you might want to enable logarithmic time compression by passing **-C** option. Like in IPBT, natural logarithm (base e) is used. This option will cause delays to be scaled non-linearly. Extremely large delays will be compressed significantly (e.g. hour-long delay will turn into several seconds), while small delays will have negligible difference. It works together with speed adjustment, too.
 
 Delay transform order:
 
 First, we apply logarithmic time compression (**-C**) if enabled. Then, speed multiplier (**-s**) will be applied to adjust delays to desired speed. Finally, delays are hard-capped (**-c**), so that if any delay exceeds the cap value (which is positive infinity by default), it will be replaced with cap value.
 
 ## License
```

### Comparing `pyttygif-0.3.1/setup.py` & `pyttygif-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyttygif",
-    version="0.3.1",
+    version="0.3.2",
     author="Vitaly Ostrosablin",
     author_email="tmp6154@yandex.ru",
     description="ttyrec to GIF converter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tmp6154/pyttygif",
     packages=setuptools.find_packages(),
```

