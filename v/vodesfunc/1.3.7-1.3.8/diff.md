# Comparing `tmp/vodesfunc-1.3.7.tar.gz` & `tmp/vodesfunc-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vodesfunc-1.3.7.tar", last modified: Fri May  5 21:26:23 2023, max compression
+gzip compressed data, was "vodesfunc-1.3.8.tar", last modified: Wed May 24 12:08:59 2023, max compression
```

## Comparing `vodesfunc-1.3.7.tar` & `vodesfunc-1.3.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 21:26:23.547751 vodesfunc-1.3.7/
--rw-rw-rw-   0        0        0     1083 2022-09-09 23:13:19.000000 vodesfunc-1.3.7/LICENSE
--rw-rw-rw-   0        0        0       60 2022-12-04 22:36:49.000000 vodesfunc-1.3.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1196 2023-05-05 21:26:23.547751 vodesfunc-1.3.7/PKG-INFO
--rw-rw-rw-   0        0        0      374 2022-12-04 22:36:49.000000 vodesfunc-1.3.7/README.md
--rw-rw-rw-   0        0        0      340 2022-12-11 22:06:28.000000 vodesfunc-1.3.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 21:26:23.548751 vodesfunc-1.3.7/setup.cfg
--rw-rw-rw-   0        0        0     1760 2022-12-04 22:36:49.000000 vodesfunc-1.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:26:23.531475 vodesfunc-1.3.7/vodesfunc/
--rw-rw-rw-   0        0        0      328 2023-03-25 20:17:58.000000 vodesfunc-1.3.7/vodesfunc/__init__.py
--rw-rw-rw-   0        0        0      362 2023-05-05 21:26:01.000000 vodesfunc-1.3.7/vodesfunc/_metadata.py
--rw-rw-rw-   0        0        0     1777 2023-01-06 15:15:08.000000 vodesfunc-1.3.7/vodesfunc/aa.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:26:23.547751 vodesfunc-1.3.7/vodesfunc/auto/
--rw-rw-rw-   0        0        0     3883 2022-11-14 21:15:19.000000 vodesfunc-1.3.7/vodesfunc/auto/convert.py
--rw-rw-rw-   0        0        0     2859 2023-01-02 21:02:04.000000 vodesfunc-1.3.7/vodesfunc/auto/download.py
--rw-rw-rw-   0        0        0    18298 2023-02-11 15:17:49.000000 vodesfunc-1.3.7/vodesfunc/auto/fonts.py
--rw-rw-rw-   0        0        0    16967 2023-04-02 20:43:50.000000 vodesfunc-1.3.7/vodesfunc/auto/muxing.py
--rw-rw-rw-   0        0        0     4772 2022-12-25 22:08:09.000000 vodesfunc-1.3.7/vodesfunc/auto/parsing.py
--rw-rw-rw-   0        0        0     1850 2022-09-09 23:21:11.000000 vodesfunc-1.3.7/vodesfunc/auto/webhook.py
--rw-rw-rw-   0        0        0    32242 2023-04-28 20:17:32.000000 vodesfunc-1.3.7/vodesfunc/automation.py
--rw-rw-rw-   0        0        0     4742 2023-05-05 21:25:21.000000 vodesfunc-1.3.7/vodesfunc/denoise.py
--rw-rw-rw-   0        0        0    12864 2023-05-04 21:46:43.000000 vodesfunc-1.3.7/vodesfunc/descale.py
--rw-rw-rw-   0        0        0     3604 2022-11-26 23:27:32.000000 vodesfunc-1.3.7/vodesfunc/misc.py
--rw-rw-rw-   0        0        0     7598 2023-04-06 21:35:28.000000 vodesfunc-1.3.7/vodesfunc/noise.py
--rw-rw-rw-   0        0        0    14121 2023-04-28 23:11:05.000000 vodesfunc-1.3.7/vodesfunc/scale.py
--rw-rw-rw-   0        0        0      650 2022-12-26 01:30:13.000000 vodesfunc-1.3.7/vodesfunc/types.py
--rw-rw-rw-   0        0        0     7717 2023-05-04 22:57:47.000000 vodesfunc-1.3.7/vodesfunc/util.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:26:23.543750 vodesfunc-1.3.7/vodesfunc.egg-info/
--rw-rw-rw-   0        0        0     1196 2023-05-05 21:26:23.000000 vodesfunc-1.3.7/vodesfunc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      593 2023-05-05 21:26:23.000000 vodesfunc-1.3.7/vodesfunc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 21:26:23.000000 vodesfunc-1.3.7/vodesfunc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      169 2023-05-05 21:26:23.000000 vodesfunc-1.3.7/vodesfunc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-05 21:26:23.000000 vodesfunc-1.3.7/vodesfunc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 12:08:59.777507 vodesfunc-1.3.8/
+-rw-rw-rw-   0        0        0     1083 2022-09-09 23:13:19.000000 vodesfunc-1.3.8/LICENSE
+-rw-rw-rw-   0        0        0       60 2022-12-04 22:36:49.000000 vodesfunc-1.3.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1196 2023-05-24 12:08:59.776176 vodesfunc-1.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2022-12-04 22:36:49.000000 vodesfunc-1.3.8/README.md
+-rw-rw-rw-   0        0        0      340 2022-12-11 22:06:28.000000 vodesfunc-1.3.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 12:08:59.777507 vodesfunc-1.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1760 2022-12-04 22:36:49.000000 vodesfunc-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:08:59.756520 vodesfunc-1.3.8/vodesfunc/
+-rw-rw-rw-   0        0        0      328 2023-03-25 20:17:58.000000 vodesfunc-1.3.8/vodesfunc/__init__.py
+-rw-rw-rw-   0        0        0      362 2023-05-24 12:08:42.000000 vodesfunc-1.3.8/vodesfunc/_metadata.py
+-rw-rw-rw-   0        0        0     1777 2023-01-06 15:15:08.000000 vodesfunc-1.3.8/vodesfunc/aa.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:08:59.775166 vodesfunc-1.3.8/vodesfunc/auto/
+-rw-rw-rw-   0        0        0     3883 2022-11-14 21:15:19.000000 vodesfunc-1.3.8/vodesfunc/auto/convert.py
+-rw-rw-rw-   0        0        0     2859 2023-01-02 21:02:04.000000 vodesfunc-1.3.8/vodesfunc/auto/download.py
+-rw-rw-rw-   0        0        0    18298 2023-02-11 15:17:49.000000 vodesfunc-1.3.8/vodesfunc/auto/fonts.py
+-rw-rw-rw-   0        0        0    16967 2023-04-02 20:43:50.000000 vodesfunc-1.3.8/vodesfunc/auto/muxing.py
+-rw-rw-rw-   0        0        0     4772 2022-12-25 22:08:09.000000 vodesfunc-1.3.8/vodesfunc/auto/parsing.py
+-rw-rw-rw-   0        0        0     1850 2022-09-09 23:21:11.000000 vodesfunc-1.3.8/vodesfunc/auto/webhook.py
+-rw-rw-rw-   0        0        0    32395 2023-05-13 20:45:39.000000 vodesfunc-1.3.8/vodesfunc/automation.py
+-rw-rw-rw-   0        0        0     4742 2023-05-05 21:25:21.000000 vodesfunc-1.3.8/vodesfunc/denoise.py
+-rw-rw-rw-   0        0        0    12864 2023-05-13 20:45:35.000000 vodesfunc-1.3.8/vodesfunc/descale.py
+-rw-rw-rw-   0        0        0     3604 2022-11-26 23:27:32.000000 vodesfunc-1.3.8/vodesfunc/misc.py
+-rw-rw-rw-   0        0        0     7598 2023-04-06 21:35:28.000000 vodesfunc-1.3.8/vodesfunc/noise.py
+-rw-rw-rw-   0        0        0    14058 2023-05-24 12:07:39.000000 vodesfunc-1.3.8/vodesfunc/scale.py
+-rw-rw-rw-   0        0        0      650 2022-12-26 01:30:13.000000 vodesfunc-1.3.8/vodesfunc/types.py
+-rw-rw-rw-   0        0        0     7717 2023-05-04 22:57:47.000000 vodesfunc-1.3.8/vodesfunc/util.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:08:59.769662 vodesfunc-1.3.8/vodesfunc.egg-info/
+-rw-rw-rw-   0        0        0     1196 2023-05-24 12:08:59.000000 vodesfunc-1.3.8/vodesfunc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2023-05-24 12:08:59.000000 vodesfunc-1.3.8/vodesfunc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 12:08:59.000000 vodesfunc-1.3.8/vodesfunc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      169 2023-05-24 12:08:59.000000 vodesfunc-1.3.8/vodesfunc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-24 12:08:59.000000 vodesfunc-1.3.8/vodesfunc.egg-info/top_level.txt
```

### Comparing `vodesfunc-1.3.7/LICENSE` & `vodesfunc-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.7/PKG-INFO` & `vodesfunc-1.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vodesfunc
-Version: 1.3.7
+Version: 1.3.8
 Summary: Vodes's Vapoursynth Functions.
 Author: Vodes
 Author-email: vodes.imp@gmail.com
 Maintainer: Vodes
 Maintainer-email: vodes.imp@gmail.com
 Project-URL: Source Code, https://github.com/Vodes/vodesfunc
 Project-URL: Contact, https://discord.gg/Kf94Nv6WVN
```

### Comparing `vodesfunc-1.3.7/setup.py` & `vodesfunc-1.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.7/vodesfunc/aa.py` & `vodesfunc-1.3.8/vodesfunc/aa.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.7/vodesfunc/auto/convert.py` & `vodesfunc-1.3.8/vodesfunc/auto/convert.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.7/vodesfunc/auto/download.py` & `vodesfunc-1.3.8/vodesfunc/auto/download.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.7/vodesfunc/auto/fonts.py` & `vodesfunc-1.3.8/vodesfunc/auto/fonts.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.7/vodesfunc/auto/muxing.py` & `vodesfunc-1.3.8/vodesfunc/auto/muxing.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.7/vodesfunc/auto/parsing.py` & `vodesfunc-1.3.8/vodesfunc/auto/parsing.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.7/vodesfunc/auto/webhook.py` & `vodesfunc-1.3.8/vodesfunc/auto/webhook.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.7/vodesfunc/automation.py` & `vodesfunc-1.3.8/vodesfunc/automation.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,27 +173,28 @@
         process.communicate()
 
         print("\nDone encoding video.")
         return str(outpath.resolve())
 
     def encode_audio(self, file: PathLike | src_file, track: int = 0, codec: str = 'opus', q: int = 200,
                      encoder_settings: str = '', trim: Trim = None, clip: vs.VideoNode | src_file = None,# use_bs_trimming: bool = False,
-                     dither_flac: bool = True, always_dither: bool = False, quiet: bool = True) -> str:
+                     dither_flac: bool = True, dither_method: str = 'triangular', always_dither: bool = False, quiet: bool = True) -> str:
         """
             Encodes the audio
 
             :param file:                Either a string based filepath, a Path object or a `src_file`
             :param track:               Audio Track Number of your input file. 0-based
             :param codec:               Either flac, opus or aac. Uses ffmpeg, opusenc or qaac respectively.
                                         'pass' and 'passthrough' also exist and do what they say
             :param q:                   Quality. Basically just the bitrate when using opus and the tVBR/-V value for qaac
             :param encoder_settings:    Arguments directly passed to opusenc or qaac
             :param trim:                Tuple of frame numbers; Can be left empty if you passed a `src_file` with trims
             :param clip:                Vapoursynth VideoNode needed when trimming; Can be left empty if you passed a `src_file`
             :param dither_flac:         Will dither your FLAC output to 16bit and 48 kHz
+            :param dither_method:       Specify the dithering algorithm used when reducing audio bit depth.
             :param always_dither:       Dithers regardless of your final output
             :param quiet:               Will print the subprocess outputs if False
             :return:                    Absolute filepath for resulting audio file
         """
         encoder_settings = ' ' + encoder_settings.strip()
         
         if trim is not None:
@@ -238,15 +239,15 @@
             return args
 
         def toflac() -> str:
             is_intermediary = codec.lower() != 'flac'
             compression_level = "10" if not is_intermediary else "0"
             commandline = f'{ffmpeg_header()} -i "{file.resolve()}" -map_metadata -1 -map_chapters -1 -map 0:a:{track} {ffmpeg_seekargs()} -f flac -compression_level {compression_level}'
             if (dither_flac and codec.lower() == 'flac') or always_dither:
-                commandline += ' -sample_fmt s16 -ar 48000 -resampler soxr -precision 28 -dither_method shibata'
+                commandline += f' -sample_fmt s16 -ar 48000 -resampler soxr -precision 28 -dither_method {dither_method}'
             if codec.lower() != 'opus':
                 _flac = base_path + ".flac"
                 if not should_create_again(_flac):
                     return _flac
                 commandline += f' "{_flac}"'
                 print(f'Creating FLAC intermediary audio track {track} for EP{self.episode}...'
                     if is_intermediary else f'Encoding audio track {track} for EP{self.episode} to FLAC...')
```

### Comparing `vodesfunc-1.3.7/vodesfunc/denoise.py` & `vodesfunc-1.3.8/vodesfunc/denoise.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.7/vodesfunc/descale.py` & `vodesfunc-1.3.8/vodesfunc/descale.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.7/vodesfunc/misc.py` & `vodesfunc-1.3.8/vodesfunc/misc.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.7/vodesfunc/noise.py` & `vodesfunc-1.3.8/vodesfunc/noise.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.7/vodesfunc/scale.py` & `vodesfunc-1.3.8/vodesfunc/scale.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,17 +46,16 @@
     def double(self, clip: vs.VideoNode, correct_shift: bool = True) -> vs.VideoNode:
         y = get_y(clip)
         # nnedi3cl needs padding, to avoid issues on edges (https://slow.pics/c/QcJef38u)
         if self.opencl:
             (left, right, top, bottom) = mod_padding(y, 2, 2)
             width = clip.width + left + right
             height = clip.height + top + bottom
-            pad = y.resize.Point(width, height, src_left=-left, src_top=-top, src_width=width, src_height=height)
-            doubled_y = pad.nnedi3cl.NNEDI3CL(dh=True, field=0, **self.ediargs).std.Transpose() \
-                .nnedi3cl.NNEDI3CL(dh=True, field=0, **self.ediargs).std.Transpose()
+            pad = y.resize.Point(width, height, src_left=-left, src_top=-top, src_width=width, src_height=height).std.Transpose()
+            doubled_y = pad.nnedi3cl.NNEDI3CL(dh=True, dw=True, field=0, **self.ediargs).std.Transpose()
             doubled_y = doubled_y.std.Crop(left * 2, right * 2, top * 2, bottom * 2)
         else:
             doubled_y = depth(y, 16).znedi3.nnedi3(dh=True, field=0, **self.ediargs).std.Transpose() \
                 .znedi3.nnedi3(dh=True, field=0, **self.ediargs).std.Transpose()
             doubled_y = depth(doubled_y, get_depth(clip))
         
         if correct_shift:
```

### Comparing `vodesfunc-1.3.7/vodesfunc/types.py` & `vodesfunc-1.3.8/vodesfunc/types.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.7/vodesfunc/util.py` & `vodesfunc-1.3.8/vodesfunc/util.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.7/vodesfunc.egg-info/PKG-INFO` & `vodesfunc-1.3.8/vodesfunc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vodesfunc
-Version: 1.3.7
+Version: 1.3.8
 Summary: Vodes's Vapoursynth Functions.
 Author: Vodes
 Author-email: vodes.imp@gmail.com
 Maintainer: Vodes
 Maintainer-email: vodes.imp@gmail.com
 Project-URL: Source Code, https://github.com/Vodes/vodesfunc
 Project-URL: Contact, https://discord.gg/Kf94Nv6WVN
```

### Comparing `vodesfunc-1.3.7/vodesfunc.egg-info/SOURCES.txt` & `vodesfunc-1.3.8/vodesfunc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

