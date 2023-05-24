# Comparing `tmp/mtv_dl-0.8.tar.gz` & `tmp/mtv_dl-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mtv_dl-0.8.tar", last modified: Mon Feb  4 06:22:41 2019, max compression
+gzip compressed data, was "dist/mtv_dl-0.9.tar", last modified: Tue Oct  1 06:46:04 2019, max compression
```

## Comparing `mtv_dl-0.8.tar` & `mtv_dl-0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 fnk        (502) staff       (20)        0 2019-02-04 06:22:41.000000 mtv_dl-0.8/
--rw-r--r--   0 fnk        (502) staff       (20)      599 2019-02-04 06:22:41.000000 mtv_dl-0.8/PKG-INFO
--rw-r--r--   0 fnk        (502) staff       (20)      130 2017-08-22 12:55:28.000000 mtv_dl-0.8/requirements.txt
--rwxr-xr-x   0 fnk        (502) staff       (20)    39887 2019-02-04 06:21:26.000000 mtv_dl-0.8/mtv_dl.py
--rw-r--r--   0 fnk        (502) staff       (20)       25 2017-08-10 10:30:30.000000 mtv_dl-0.8/MANIFEST.in
--rw-r--r--   0 fnk        (502) staff       (20)     3954 2018-09-17 11:20:19.000000 mtv_dl-0.8/README
--rw-r--r--   0 fnk        (502) staff       (20)     1277 2019-02-04 06:19:55.000000 mtv_dl-0.8/setup.py
-drwxr-xr-x   0 fnk        (502) staff       (20)        0 2019-02-04 06:22:41.000000 mtv_dl-0.8/mtv_dl.egg-info/
--rw-r--r--   0 fnk        (502) staff       (20)      599 2019-02-04 06:22:41.000000 mtv_dl-0.8/mtv_dl.egg-info/PKG-INFO
--rw-r--r--   0 fnk        (502) staff       (20)      236 2019-02-04 06:22:41.000000 mtv_dl-0.8/mtv_dl.egg-info/SOURCES.txt
--rw-r--r--   0 fnk        (502) staff       (20)       40 2019-02-04 06:22:41.000000 mtv_dl-0.8/mtv_dl.egg-info/entry_points.txt
--rw-r--r--   0 fnk        (502) staff       (20)      130 2019-02-04 06:22:41.000000 mtv_dl-0.8/mtv_dl.egg-info/requires.txt
--rw-r--r--   0 fnk        (502) staff       (20)        7 2019-02-04 06:22:41.000000 mtv_dl-0.8/mtv_dl.egg-info/top_level.txt
--rw-r--r--   0 fnk        (502) staff       (20)        1 2019-02-04 06:22:41.000000 mtv_dl-0.8/mtv_dl.egg-info/dependency_links.txt
--rw-r--r--   0 fnk        (502) staff       (20)       38 2019-02-04 06:22:41.000000 mtv_dl-0.8/setup.cfg
+drwxr-xr-x   0 fnk        (502) staff       (20)        0 2019-10-01 06:46:04.000000 mtv_dl-0.9/
+-rw-r--r--   0 fnk        (502) staff       (20)       25 2017-08-10 10:30:30.000000 mtv_dl-0.9/MANIFEST.in
+-rw-r--r--   0 fnk        (502) staff       (20)      599 2019-10-01 06:46:04.000000 mtv_dl-0.9/PKG-INFO
+-rw-r--r--   0 fnk        (502) staff       (20)     3974 2019-10-01 06:40:31.000000 mtv_dl-0.9/README
+drwxr-xr-x   0 fnk        (502) staff       (20)        0 2019-10-01 06:46:04.000000 mtv_dl-0.9/mtv_dl.egg-info/
+-rw-r--r--   0 fnk        (502) staff       (20)      599 2019-10-01 06:46:04.000000 mtv_dl-0.9/mtv_dl.egg-info/PKG-INFO
+-rw-r--r--   0 fnk        (502) staff       (20)      236 2019-10-01 06:46:04.000000 mtv_dl-0.9/mtv_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 fnk        (502) staff       (20)        1 2019-10-01 06:46:04.000000 mtv_dl-0.9/mtv_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 fnk        (502) staff       (20)       40 2019-10-01 06:46:04.000000 mtv_dl-0.9/mtv_dl.egg-info/entry_points.txt
+-rw-r--r--   0 fnk        (502) staff       (20)      145 2019-10-01 06:46:04.000000 mtv_dl-0.9/mtv_dl.egg-info/requires.txt
+-rw-r--r--   0 fnk        (502) staff       (20)        7 2019-10-01 06:46:04.000000 mtv_dl-0.9/mtv_dl.egg-info/top_level.txt
+-rwxr-xr-x   0 fnk        (502) staff       (20)    42338 2019-10-01 06:35:42.000000 mtv_dl-0.9/mtv_dl.py
+-rw-r--r--   0 fnk        (502) staff       (20)      145 2019-10-01 05:31:02.000000 mtv_dl-0.9/requirements.txt
+-rw-r--r--   0 fnk        (502) staff       (20)       38 2019-10-01 06:46:04.000000 mtv_dl-0.9/setup.cfg
+-rw-r--r--   0 fnk        (502) staff       (20)     1277 2019-10-01 06:39:01.000000 mtv_dl-0.9/setup.py
```

### Comparing `mtv_dl-0.8/PKG-INFO` & `mtv_dl-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mtv_dl
-Version: 0.8
+Version: 0.9
 Summary: MediathekView Downloader
 Home-page: https://github.com/efenka/mtv_dl
 Author: Frank Epperlein
 Author-email: frank+mtv_dl@epperle.in
 License: UNKNOWN
 Description: Command line tool to download videos from sources available through MediathekView.
 Platform: UNKNOWN
```

### Comparing `mtv_dl-0.8/mtv_dl.py` & `mtv_dl-0.9/mtv_dl.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,15 @@
                                         name extension including the dot), and all fields from
                                         the listing plus {{date}} and {{time}} (the single parts
                                         of {{start}}).
                                         [default: {{dir}}/{{channel}}/{{topic}}/{{start}} {{title}}{{ext}}]
   --mark-only                           Do not download any show, but mark it as downloaded
                                         in the history. This is to initialize a new filter
                                         if upcoming shows are wanted.
+  --no-subtitles                        Do not try to download subtitles.
   -s <file>, --sets=<file>              A file to load different sets of filters (see below
                                         for details). In the file every different filter set
                                         is expected to be on a new line.
 
   WARNING: Please be aware that ancient RTMP streams are not supported
            They will not even get listed.
 
@@ -156,14 +157,15 @@
 import iso8601
 import pytz
 import requests
 import rfc6266
 import tzlocal
 import xxhash
 import yaml
+from bs4 import BeautifulSoup
 from pydash import py_
 from terminaltables import AsciiTable
 from tinydb import TinyDB, Query as TinyQuery
 from tinydb_serialization import SerializationMiddleware as TinySerializationMiddleware
 from tinydb_serialization import Serializer as TinySerializer
 from tqdm import tqdm
 from yaml.error import YAMLError
@@ -202,14 +204,15 @@
     'count': int,
     'dir': str,
     'high': bool,
     'include-future': bool,
     'logfile': str,
     'low': bool,
     'no-bar': bool,
+    'no-subtitles': bool,
     'quiet': bool,
     'refresh-after': int,
     'target': str,
     'verbose': bool
 }
 
 
@@ -700,15 +703,21 @@
                 with destination_file_path.open('wb') as fh:
                     for data in response.iter_content(CHUNK_SIZE):
                         progress_bar.update(len(data))
                         fh.write(data)
 
                 yield destination_file_path
 
-    def _move_to_user_target(self, source_path: Path, cwd: Path, target: Path, file_name: str, file_extension: str):
+    def _move_to_user_target(self,
+                             source_path: Path,
+                             cwd: Path,
+                             target: Path,
+                             file_name: str,
+                             file_extension: str,
+                             media_type: str):
 
         escaped_show_details = {k: str(v).replace(os.path.sep, '_') for k, v in self.items()}
         destination_file_path = Path(target.as_posix().format(dir=cwd,
                                                               filename=file_name,
                                                               ext=file_extension,
                                                               date=self['start'].date().isoformat(),
                                                               time=self['start'].strftime('%H:%M'),
@@ -716,15 +725,15 @@
 
         destination_file_path.parent.mkdir(parents=True, exist_ok=True)
         try:
             shutil.move(source_path.as_posix(), destination_file_path.as_posix())
         except OSError as e:
             logger.warning('Skipped %s: %s', self.label, str(e))
         else:
-            logger.info('Saved %s to %r.', self.label, destination_file_path)
+            logger.info('Saved %s %s to %r.', media_type, self.label, destination_file_path)
 
     @staticmethod
     def _get_m3u8_segments(base_url: str, hls_file_path: Path) -> Generator[Dict[str, Any], None, None]:
 
         with hls_file_path.open('r+') as fh:
             segment = {}  # type: Dict
             for line in fh:
@@ -787,18 +796,56 @@
                     out_fh.write(in_fh.read())
 
                 # delete the segment file immediately to save disk space
                 segment_file_path.unlink()
 
         return temp_file_path
 
+    @staticmethod
+    def _convert_subtitles_xml_to_srt(subtitles_xml_path: Path) -> Path:
+
+        subtitles_srt_path = subtitles_xml_path.parent / (subtitles_xml_path.stem + '.srt')
+        soup = BeautifulSoup(subtitles_xml_path.read_text(), "html.parser")
+
+        colour_to_rgb = {
+            "textBlack": "#000000",
+            "textRed": "#FF0000",
+            "textGreen": "#00FF00",
+            "textYellow": "#FFFF00",
+            "textBlue": "#0000FF",
+            "textMagenta": "#FF00FF",
+            "textCyan": "#00FFFF",
+            "textWhite": "#FFFFFF"}
+
+        def font_colour(text, colour):
+            return "<font color=\"%s\">%s</font>\n" % (colour_to_rgb[colour], text)
+
+        with subtitles_srt_path.open('w') as srt:
+            for p_tag in soup.findAll("tt:p"):
+                # noinspection PyBroadException
+                try:
+                    srt.write(str(int(p_tag.get("xml:id").replace("sub", "")) + 1) + "\n")
+                    srt.write(f"{p_tag['begin'].replace('.', ',')} --> {p_tag['end'].replace('.', ',')}\n")
+                    for span_tag in p_tag.findAll('tt:span'):
+                        srt.write(font_colour(span_tag.text, span_tag.get('style')).replace("&apos", "'"))
+                    srt.write('\n\n')
+                except Exception:
+                    logging.debug('Unexpected data in subtitle xml file: %s', p_tag)
+
+        return subtitles_srt_path
+
     def __init__(self, show: Dict[str, Any], **kwargs: Dict) -> None:
         super().__init__(show, **kwargs)
 
-    def download(self, quality: Tuple[str, str, str], cwd: Path, target: Path) -> Union[Path, None]:
+    def download(self,
+                 quality: Tuple[str, str, str],
+                 cwd: Path,
+                 target: Path,
+                 *,
+                 include_subtitles: bool = True) -> Union[Path, None]:
         temp_path = Path(tempfile.mkdtemp(prefix='.tmp'))
         try:
 
             # show url based on quality preference
             show_url = self["url_http%s" % quality[0]] \
                        or self["url_http%s" % quality[1]] \
                        or self["url_http%s" % quality[2]]
@@ -809,25 +856,32 @@
             if '.' in show_file_name:
                 show_file_extension = show_file_path.suffix
                 show_file_name = show_file_path.stem
             else:
                 show_file_extension = ''
 
             if show_file_extension in ('.mp4', '.flv', '.mp3'):
-                self._move_to_user_target(show_file_path, cwd, target, show_file_name, show_file_extension)
-                return show_file_path
+                self._move_to_user_target(show_file_path, cwd, target, show_file_name, show_file_extension, 'show')
 
             # TODO: consider to remove hsl/m3u8 downloads ("./mtv_dl.py dump url='[^(mp4|flv|mp3)]$'" is empty)
             elif show_file_extension == '.m3u8':
                 ts_file_path = self._download_hls_target(temp_path, show_url, quality, show_file_path)
-                self._move_to_user_target(ts_file_path, cwd, target, show_file_name, '.ts')
-                return show_file_path
+                self._move_to_user_target(ts_file_path, cwd, target, show_file_name, '.ts', 'show')
 
             else:
                 logger.error('File extension %s of %s not supported.', show_file_extension, self.label)
+                return None
+
+            if include_subtitles and self['url_subtitles']:
+                logger.debug('Downloading subtitles for %s from %r.', self.label, self['url_subtitles'])
+                subtitles_xml_path = list(self._download_files(temp_path, [self['url_subtitles']]))[0]
+                subtitles_srt_path = self._convert_subtitles_xml_to_srt(subtitles_xml_path)
+                self._move_to_user_target(subtitles_srt_path, cwd, target, show_file_name, '.srt', 'subtitles')
+
+            return show_file_path
 
         except (requests.exceptions.RequestException, OSError) as e:
             logger.error('Download of %s failed: %s', self.label, str(e))
         finally:
             shutil.rmtree(temp_path)
 
         return None
@@ -963,15 +1017,16 @@
                         if not arguments['--mark-only']:
                             if arguments['--high']:
                                 quality_preference = ('_hd', '', '_small')
                             elif arguments['--low']:
                                 quality_preference = ('_small', '', '_hd')
                             else:
                                 quality_preference = ('', '_hd', '_small')
-                            show.download(quality_preference, cw_dir, target_dir)
+                            show.download(quality_preference, cw_dir, target_dir,
+                                          include_subtitles=not arguments['--no-subtitles'])
                             item['downloaded'] = now
                             history.insert(item)
                         else:
                             show['downloaded'] = now
                             history.insert(show)
                             logger.info('Marked %s from %s as downloaded.', show.label)
                     else:
```

### Comparing `mtv_dl-0.8/README` & `mtv_dl-0.9/README`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 Features
 --------
 
 - No GUI or web interface. Less then 1000 lines of code. Only python dependencies.
 - Powerful filter system for lists and download selection.
-- Download .mp4, .flv and .m3u8 (HLS) media.
+- Download .mp4, .flv and .m3u8 (HLS) media inclusive subtitles.
 - Keep track of downloaded files and don't download them again.
 - Template naming of the downloaded files.
 
 
 Usage examples
 --------------
```

### Comparing `mtv_dl-0.8/setup.py` & `mtv_dl-0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     from pip._internal.req import parse_requirements
 except ImportError: # for pip <= 9.0.3
     from pip.req import parse_requirements
 
 requirements = parse_requirements(Path(__file__).parent.joinpath('requirements.txt').as_posix(), session='dummy')
 
 setup(name='mtv_dl',
-      version='0.8',
+      version='0.9',
       description='MediathekView Downloader',
       long_description='Command line tool to download videos from sources available through MediathekView.',
       author='Frank Epperlein',
       author_email='frank+mtv_dl@epperle.in',
       url='https://github.com/efenka/mtv_dl',
       py_modules=['mtv_dl'],
       entry_points={
```

### Comparing `mtv_dl-0.8/mtv_dl.egg-info/PKG-INFO` & `mtv_dl-0.9/mtv_dl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mtv-dl
-Version: 0.8
+Version: 0.9
 Summary: MediathekView Downloader
 Home-page: https://github.com/efenka/mtv_dl
 Author: Frank Epperlein
 Author-email: frank+mtv_dl@epperle.in
 License: UNKNOWN
 Description: Command line tool to download videos from sources available through MediathekView.
 Platform: UNKNOWN
```

