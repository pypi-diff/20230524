# Comparing `tmp/geniusdotpy-0.1.8.1.tar.gz` & `tmp/geniusdotpy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geniusdotpy-0.1.8.1.tar", last modified: Wed Dec 28 01:38:02 2022, max compression
+gzip compressed data, was "geniusdotpy-0.9.0.tar", last modified: Wed May 24 04:03:13 2023, max compression
```

## Comparing `geniusdotpy-0.1.8.1.tar` & `geniusdotpy-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 01:38:02.004637 geniusdotpy-0.1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2022-12-28 01:37:52.000000 geniusdotpy-0.1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2022-12-28 01:38:02.004637 geniusdotpy-0.1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2022-12-28 01:37:52.000000 geniusdotpy-0.1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 01:38:02.004637 geniusdotpy-0.1.8.1/geniusdotpy/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2022-12-28 01:37:52.000000 geniusdotpy-0.1.8.1/geniusdotpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2022-12-28 01:37:52.000000 geniusdotpy-0.1.8.1/geniusdotpy/album.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2022-12-28 01:37:52.000000 geniusdotpy-0.1.8.1/geniusdotpy/artist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2022-12-28 01:37:52.000000 geniusdotpy-0.1.8.1/geniusdotpy/genius_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2022-12-28 01:37:52.000000 geniusdotpy-0.1.8.1/geniusdotpy/lyrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2022-12-28 01:37:52.000000 geniusdotpy-0.1.8.1/geniusdotpy/track.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2022-12-28 01:37:52.000000 geniusdotpy-0.1.8.1/geniusdotpy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 01:38:02.004637 geniusdotpy-0.1.8.1/geniusdotpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2022-12-28 01:38:01.000000 geniusdotpy-0.1.8.1/geniusdotpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2022-12-28 01:38:01.000000 geniusdotpy-0.1.8.1/geniusdotpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-28 01:38:01.000000 geniusdotpy-0.1.8.1/geniusdotpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-28 01:38:01.000000 geniusdotpy-0.1.8.1/geniusdotpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-28 01:38:01.000000 geniusdotpy-0.1.8.1/geniusdotpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-28 01:38:02.004637 geniusdotpy-0.1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2022-12-28 01:37:52.000000 geniusdotpy-0.1.8.1/setup.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-24 04:03:13.433619 geniusdotpy-0.9.0/
+-rw-r--r--   0 joel      (1000) joel      (1000)     1061 2023-05-24 03:59:34.000000 geniusdotpy-0.9.0/LICENSE
+-rw-r--r--   0 joel      (1000) joel      (1000)     1957 2023-05-24 04:03:13.433619 geniusdotpy-0.9.0/PKG-INFO
+-rw-r--r--   0 joel      (1000) joel      (1000)     1377 2023-05-24 03:35:41.000000 geniusdotpy-0.9.0/README.md
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-24 04:03:13.432619 geniusdotpy-0.9.0/geniusdotpy/
+-rw-r--r--   0 joel      (1000) joel      (1000)      243 2023-05-24 03:44:26.000000 geniusdotpy-0.9.0/geniusdotpy/__init__.py
+-rw-r--r--   0 joel      (1000) joel      (1000)      986 2023-05-24 03:42:25.000000 geniusdotpy-0.9.0/geniusdotpy/album.py
+-rw-r--r--   0 joel      (1000) joel      (1000)      652 2023-05-24 03:42:26.000000 geniusdotpy-0.9.0/geniusdotpy/artist.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     2991 2023-05-24 03:44:20.000000 geniusdotpy-0.9.0/geniusdotpy/genius_builder.py
+-rw-r--r--   0 joel      (1000) joel      (1000)      380 2023-05-24 03:47:26.000000 geniusdotpy-0.9.0/geniusdotpy/lyrics.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     3360 2023-05-24 03:42:32.000000 geniusdotpy-0.9.0/geniusdotpy/track.py
+-rw-r--r--   0 joel      (1000) joel      (1000)      251 2023-05-24 03:43:51.000000 geniusdotpy-0.9.0/geniusdotpy/utils.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-24 04:03:13.433619 geniusdotpy-0.9.0/geniusdotpy.egg-info/
+-rw-r--r--   0 joel      (1000) joel      (1000)     1957 2023-05-24 04:03:13.000000 geniusdotpy-0.9.0/geniusdotpy.egg-info/PKG-INFO
+-rw-r--r--   0 joel      (1000) joel      (1000)      361 2023-05-24 04:03:13.000000 geniusdotpy-0.9.0/geniusdotpy.egg-info/SOURCES.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)        1 2023-05-24 04:03:13.000000 geniusdotpy-0.9.0/geniusdotpy.egg-info/dependency_links.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       24 2023-05-24 04:03:13.000000 geniusdotpy-0.9.0/geniusdotpy.egg-info/requires.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       12 2023-05-24 04:03:13.000000 geniusdotpy-0.9.0/geniusdotpy.egg-info/top_level.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       38 2023-05-24 04:03:13.433619 geniusdotpy-0.9.0/setup.cfg
+-rw-r--r--   0 joel      (1000) joel      (1000)      998 2023-05-24 04:01:26.000000 geniusdotpy-0.9.0/setup.py
```

### Comparing `geniusdotpy-0.1.8.1/LICENSE` & `geniusdotpy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geniusdotpy-0.1.8.1/PKG-INFO` & `geniusdotpy-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: geniusdotpy
-Version: 0.1.8.1
+Version: 0.9.0
 Summary: Python wrapper for Genius API
 Home-page: https://github.com/jjoeldaniel/genius.py
 Author: jjoeldaniel
 Author-email: <joeldanielrico@gmail.com>
 Keywords: python,genius,api-wrapper
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **genius.py**
 
 [![PyPI version](https://img.shields.io/pypi/v/geniusdotpy)](https://pypi.org/project/geniusdotpy/)
 [![Python 3.x version](https://img.shields.io/badge/python-3.x-brightgreen.svg)](https://www.python.org/downloads/)
 [![Wiki Link](https://img.shields.io/badge/wiki-documentation-forestgreen)](https://github.com/jjoeldaniel/genius.py/wiki)
+[![Downloads](https://static.pepy.tech/badge/geniusdotpy)](https://pepy.tech/project/geniusdotpy)
 
 > Python wrapper for Genius API
 
 With genius.py, enjoy an easy-to-use interface to interact with [Genius API](https://docs.genius.com)
 
 ## Table of Contents
```

### Comparing `geniusdotpy-0.1.8.1/README.md` & `geniusdotpy-0.9.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # **genius.py**
 
 [![PyPI version](https://img.shields.io/pypi/v/geniusdotpy)](https://pypi.org/project/geniusdotpy/)
 [![Python 3.x version](https://img.shields.io/badge/python-3.x-brightgreen.svg)](https://www.python.org/downloads/)
 [![Wiki Link](https://img.shields.io/badge/wiki-documentation-forestgreen)](https://github.com/jjoeldaniel/genius.py/wiki)
+[![Downloads](https://static.pepy.tech/badge/geniusdotpy)](https://pepy.tech/project/geniusdotpy)
 
 > Python wrapper for Genius API
 
 With genius.py, enjoy an easy-to-use interface to interact with [Genius API](https://docs.genius.com)
 
 ## Table of Contents
```

### Comparing `geniusdotpy-0.1.8.1/geniusdotpy/album.py` & `geniusdotpy-0.9.0/geniusdotpy/album.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-from geniusdotpy.utils import *
+from geniusdotpy.utils import format_json
 
-class Album:
 
+class Album:
     def __init__(self, album_info):
         self.album_info = album_info
-        self.id = album_info['id']
-        self.url = album_info['url']
-        self.path = album_info['api_path']
+        self.id = album_info["id"]
+        self.url = album_info["url"]
+        self.path = album_info["api_path"]
 
-        if 'cover_art_url' in album_info:
-            self.cover_art_url = album_info['cover_art_url']
+        if "cover_art_url" in album_info:
+            self.cover_art_url = album_info["cover_art_url"]
         else:
             self.cover_art_url = None
 
         # Fallback name to full_title if name is not present and vice versa
-        if 'name' in album_info:
-            self.name = album_info['name']
+        if "name" in album_info:
+            self.name = album_info["name"]
         else:
-            self.name = album_info['full_title']
+            self.name = album_info["full_title"]
 
-        if 'full_title' in album_info:
-            self.full_title = album_info['full_title']
+        if "full_title" in album_info:
+            self.full_title = album_info["full_title"]
         else:
-            self.full_title = album_info['name']
-
+            self.full_title = album_info["name"]
 
     def __str__(self):
         return self.name
 
     def to_json(self):
         """Convert album info to JSON.
-        
+
         Returns:
             JSON object
         """
 
         return format_json(self.album_info)
```

### Comparing `geniusdotpy-0.1.8.1/geniusdotpy/artist.py` & `geniusdotpy-0.9.0/geniusdotpy/artist.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from geniusdotpy.track import Track
-from geniusdotpy.utils import *
+from geniusdotpy.utils import format_json
 
 
 class Artist:
-
     def __init__(self, artist_info, tracks_info):
         self.artist_info = artist_info
         self.tracks_info = tracks_info
         self.tracks = [Track(track_info=track_info) for track_info in self.tracks_info]
-        self.id = self.artist_info['id']
-        self.name = self.artist_info['name']
-        self.url = self.artist_info['url']
-        self.path = self.artist_info['api_path']
+        self.id = self.artist_info["id"]
+        self.name = self.artist_info["name"]
+        self.url = self.artist_info["url"]
+        self.path = self.artist_info["api_path"]
 
     def to_json(self):
         """Convert artist info to JSON.
 
         Returns:
             JSON object
         """
```

### Comparing `geniusdotpy-0.1.8.1/geniusdotpy/genius_builder.py` & `geniusdotpy-0.9.0/geniusdotpy/genius_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import requests
 from geniusdotpy.track import Track
 from geniusdotpy.artist import Artist
 from geniusdotpy.album import Album
 
 
 class GeniusBuilder:
-    endpoint = 'https://api.genius.com'
+    endpoint = "https://api.genius.com"
 
     def __init__(self, client_access_token):
         """GeniusBuilder constructor.
-        
+
         Keyword arguments:
             client_access_token -- The client access token from https://genius.com/api-clients
 
         Returns:
             GeniusBuilder object
         """
 
@@ -25,83 +25,83 @@
         Keyword arguments:
             track_id -- The ID of the song
 
         Returns:
             Track object
         """
 
-        endpoint = f'{self.endpoint}/songs/{track_id}'
-        headers = {'Authorization': f'Bearer {self.client_access_token}'}
+        endpoint = f"{self.endpoint}/songs/{track_id}"
+        headers = {"Authorization": f"Bearer {self.client_access_token}"}
 
         response = requests.get(endpoint, headers=headers)
         response.raise_for_status()
 
-        return Track(track_info=response.json()['response']['song'])
+        return Track(track_info=response.json()["response"]["song"])
 
     def search(self, query):
         """Search for a track by query.
-        
+
         Keyword arguments:
             query -- The query to search for
-        
+
         Returns:
             List of Track objects
         """
 
-        endpoint = f'{self.endpoint}/search'
-        data = {'q': query}
-        headers = {'Authorization': f'Bearer {self.client_access_token}'}
+        endpoint = f"{self.endpoint}/search"
+        data = {"q": query}
+        headers = {"Authorization": f"Bearer {self.client_access_token}"}
 
         response = requests.get(endpoint, params=data, headers=headers)
         response.raise_for_status()
 
         tracks = []
 
-        for hits in response.json()['response']['hits']:
-            track = Track(track_info=hits['result'])
+        for hits in response.json()["response"]["hits"]:
+            track = Track(track_info=hits["result"])
             tracks.append(track)
 
         return tracks
 
     def search_artist(self, artist_id):
         """Search for an artist by ID.
-        
+
         Keyword arguments:
             artist_id -- The ID of the artist
 
         Returns:
             Artist object
         """
 
-        endpoint = f'{self.endpoint}/artists/{artist_id}/songs'
-        headers = {'Authorization': f'Bearer {self.client_access_token}'}
+        endpoint = f"{self.endpoint}/artists/{artist_id}/songs"
+        headers = {"Authorization": f"Bearer {self.client_access_token}"}
 
         response = requests.get(endpoint, headers=headers)
         response.raise_for_status()
-        tracks_info = response.json()['response']['songs']
+        tracks_info = response.json()["response"]["songs"]
 
-        endpoint = f'{self.endpoint}/artists/{artist_id}'
+        endpoint = f"{self.endpoint}/artists/{artist_id}"
         response = requests.get(endpoint, headers=headers)
         response.raise_for_status()
-        artist_info = response.json()['response']['artist']
+        artist_info = response.json()["response"]["artist"]
 
         return Artist(artist_info=artist_info, tracks_info=tracks_info)
 
     def search_album(self, album_id):
         """Search for an album by ID.
-        
+
         Keyword arguments:
             album_id -- The ID of the album
 
         Returns:
             Album object
         """
 
-        endpoint = f'{self.endpoint}/albums/{album_id}'
-        headers = {'Authorization': f'Bearer {self.client_access_token}'}
+        endpoint = f"{self.endpoint}/albums/{album_id}"
+        headers = {"Authorization": f"Bearer {self.client_access_token}"}
 
         response = requests.get(endpoint, headers=headers)
         response.raise_for_status()
 
-        album_info = response.json()['response']['album']
+        album_info = response.json()["response"]["album"]
 
         return Album(album_info=album_info)
```

### Comparing `geniusdotpy-0.1.8.1/geniusdotpy/track.py` & `geniusdotpy-0.9.0/geniusdotpy/track.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,103 +1,104 @@
 import datetime
 from geniusdotpy.lyrics import Lyrics
 from geniusdotpy.album import Album
-from geniusdotpy.utils import *
+from geniusdotpy.utils import format_json
 
 
 class Track:
-
     def __init__(self, track_info):
         self.track_info = track_info
-        self.artist = track_info['primary_artist']['name']
-        self.artist_id = track_info['primary_artist']['id']
-        self.title = track_info['title']
-        self.path = track_info['path']
-        self.title_with_featured = track_info['title_with_featured']
-        self.full_title = track_info['full_title']
-        self.url = track_info['url']
-        self.id = track_info['id']
-        self.featured_artists = track_info['featured_artists']
+        self.artist = track_info["primary_artist"]["name"]
+        self.artist_id = track_info["primary_artist"]["id"]
+        self.title = track_info["title"]
+        self.path = track_info["path"]
+        self.title_with_featured = track_info["title_with_featured"]
+        self.full_title = track_info["full_title"]
+        self.url = track_info["url"]
+        self.id = track_info["id"]
+        self.featured_artists = track_info["featured_artists"]
         self.__date = datetime.datetime(1, 1, 1)
         self.lyrics = Lyrics(track_url=self.url).content
-        self.lyrics_by_line = self.lyrics.split('\n')
+        self.lyrics_by_line = self.lyrics.split("\n")
 
-        if 'album' in track_info:
-            self.album = Album(album_info=track_info['album'])
+        if "album" in track_info:
+            self.album = Album(album_info=track_info["album"])
         else:
             self.album = None
 
-        if 'language' in track_info:
-            self.language = track_info['language']
+        if "language" in track_info:
+            self.language = track_info["language"]
         else:
             self.language = None
 
-        if 'header_image_thumbnail_url' in track_info:
-            self.header_image_thumbnail_url = track_info['header_image_thumbnail_url']
+        if "header_image_thumbnail_url" in track_info:
+            self.header_image_thumbnail_url = track_info["header_image_thumbnail_url"]
         else:
             self.header_image_thumbnail_url = None
 
-        if 'header_image_url' in track_info:
-            self.header_image_url = track_info['header_image_url']
+        if "header_image_url" in track_info:
+            self.header_image_url = track_info["header_image_url"]
         else:
             self.header_image_url = None
 
-        if 'song_art_image_thumbnail_url' in track_info:
-            self.song_art_image_thumbnail_url = track_info['song_art_image_thumbnail_url']
+        if "song_art_image_thumbnail_url" in track_info:
+            self.song_art_image_thumbnail_url = track_info[
+                "song_art_image_thumbnail_url"
+            ]
         else:
             self.song_art_image_thumbnail_url = None
 
-        if 'song_art_image_url' in track_info:
-            self.art_image_url = track_info['song_art_image_url']
+        if "song_art_image_url" in track_info:
+            self.art_image_url = track_info["song_art_image_url"]
         else:
             self.art_image_url = None
 
-        if 'pageviews' in track_info['stats']:
-            self.page_views = track_info['stats']['pageviews']
+        if "pageviews" in track_info["stats"]:
+            self.page_views = track_info["stats"]["pageviews"]
         else:
             self.page_views = None
 
-        if 'media' in track_info:
-            for media in track_info['media']:
-                if media['provider'] == 'youtube':
-                    self.youtube_url = media['url']
+        if "media" in track_info:
+            for media in track_info["media"]:
+                if media["provider"] == "youtube":
+                    self.youtube_url = media["url"]
                 else:
                     self.youtube_url = None
 
-                if media['provider'] == 'spotify':
-                    self.spotify_url = media['url']
+                if media["provider"] == "spotify":
+                    self.spotify_url = media["url"]
                 else:
                     self.spotify_url = None
 
-                if media['provider'] == 'soundcloud':
-                    self.soundcloud_url = media['url']
+                if media["provider"] == "soundcloud":
+                    self.soundcloud_url = media["url"]
                 else:
                     self.soundcloud_url = None
 
     def __str__(self):
         return self.full_title
 
     def to_json(self):
         """Convert track info to JSON.
-        
+
         Returns:
             JSON object
         """
 
         return format_json(self.track_info)
 
     def release_date(self):
         """Get the release date of the track.
-        
+
         Returns:
             datetime object
         """
 
         if self.__date.year != 1:
             return self.__date
 
-        year = self.track_info['release_date_components']['year']
-        month = self.track_info['release_date_components']['month']
-        day = self.track_info['release_date_components']['day']
+        year = self.track_info["release_date_components"]["year"]
+        month = self.track_info["release_date_components"]["month"]
+        day = self.track_info["release_date_components"]["day"]
         self.__date = datetime.datetime(year, month, day)
 
         return self.__date
```

### Comparing `geniusdotpy-0.1.8.1/geniusdotpy.egg-info/PKG-INFO` & `geniusdotpy-0.9.0/geniusdotpy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: geniusdotpy
-Version: 0.1.8.1
+Version: 0.9.0
 Summary: Python wrapper for Genius API
 Home-page: https://github.com/jjoeldaniel/genius.py
 Author: jjoeldaniel
 Author-email: <joeldanielrico@gmail.com>
 Keywords: python,genius,api-wrapper
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **genius.py**
 
 [![PyPI version](https://img.shields.io/pypi/v/geniusdotpy)](https://pypi.org/project/geniusdotpy/)
 [![Python 3.x version](https://img.shields.io/badge/python-3.x-brightgreen.svg)](https://www.python.org/downloads/)
 [![Wiki Link](https://img.shields.io/badge/wiki-documentation-forestgreen)](https://github.com/jjoeldaniel/genius.py/wiki)
+[![Downloads](https://static.pepy.tech/badge/geniusdotpy)](https://pepy.tech/project/geniusdotpy)
 
 > Python wrapper for Genius API
 
 With genius.py, enjoy an easy-to-use interface to interact with [Genius API](https://docs.genius.com)
 
 ## Table of Contents
```

### Comparing `geniusdotpy-0.1.8.1/setup.py` & `geniusdotpy-0.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 import codecs
 import os
 
 this_directory = Path(__file__).parent
 
-VERSION = '0.1.8.1'
-DESCRIPTION = 'Python wrapper for Genius API'
+VERSION = "0.9.0"
+DESCRIPTION = "Python wrapper for Genius API"
 long_description = (this_directory / "README.md").read_text()
 
 # Setting up
 setup(
     name="geniusdotpy",
     version=VERSION,
     author="jjoeldaniel",
     author_email="<joeldanielrico@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://github.com/jjoeldaniel/genius.py",
     packages=find_packages(),
-    install_requires=['requests', 'beautifulsoup4'],
-    keywords=['python', 'genius', 'api-wrapper'],
+    install_requires=["requests", "beautifulsoup4"],
+    keywords=["python", "genius", "api-wrapper"],
     classifiers=[
-        "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
-    ]
+    ],
 )
```

