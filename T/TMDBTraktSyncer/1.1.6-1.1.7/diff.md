# Comparing `tmp/TMDBTraktSyncer-1.1.6.tar.gz` & `tmp/TMDBTraktSyncer-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMDBTraktSyncer-1.1.6.tar", last modified: Sat May 20 21:44:11 2023, max compression
+gzip compressed data, was "TMDBTraktSyncer-1.1.7.tar", last modified: Wed May 24 01:35:14 2023, max compression
```

## Comparing `TMDBTraktSyncer-1.1.6.tar` & `TMDBTraktSyncer-1.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 21:44:11.632901 TMDBTraktSyncer-1.1.6/
--rw-rw-rw-   0        0        0     1079 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.6/LICENSE
--rw-rw-rw-   0        0        0     6468 2023-05-20 21:44:11.631913 TMDBTraktSyncer-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     5795 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 21:44:11.611759 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/
--rw-rw-rw-   0        0        0     5677 2023-05-20 20:12:07.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/TMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1928 2023-05-20 19:53:06.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     8916 2023-05-20 19:53:06.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     2918 2023-05-20 20:21:56.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/tmdbData.py
--rw-rw-rw-   0        0        0     2263 2023-05-20 21:38:06.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     1834 2023-05-20 19:53:05.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-20 21:44:11.629900 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     6468 2023-05-20 21:44:11.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      481 2023-05-20 21:44:11.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 21:44:11.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-20 21:44:11.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 21:44:11.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-20 21:44:11.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 21:44:11.632901 TMDBTraktSyncer-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1291 2023-05-20 21:44:05.000000 TMDBTraktSyncer-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 01:35:14.424027 TMDBTraktSyncer-1.1.7/
+-rw-rw-rw-   0        0        0     1079 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.1.7/LICENSE
+-rw-rw-rw-   0        0        0     7257 2023-05-24 01:35:14.423026 TMDBTraktSyncer-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6555 2023-05-24 01:34:43.000000 TMDBTraktSyncer-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 01:35:14.394903 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    10142 2023-05-24 01:26:25.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/TMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1928 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     8916 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     3952 2023-05-24 00:42:48.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/tmdbData.py
+-rw-rw-rw-   0        0        0     3037 2023-05-24 00:45:06.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     3325 2023-05-24 00:34:12.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-24 01:35:14.421027 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     7257 2023-05-24 01:35:14.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2023-05-24 01:35:14.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 01:35:14.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-24 01:35:14.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-24 01:35:14.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-24 01:35:14.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 01:35:14.424027 TMDBTraktSyncer-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1311 2023-05-24 01:30:39.000000 TMDBTraktSyncer-1.1.7/setup.py
```

### Comparing `TMDBTraktSyncer-1.1.6/LICENSE` & `TMDBTraktSyncer-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.6/PKG-INFO` & `TMDBTraktSyncer-1.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.1.6
-Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
+Version: 1.1.7
+Summary: This python script syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # TMDB-Trakt-Syncer
 
-This Python script syncs user ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Ratings already set will not be overwritten. The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
+This Python script syncs user watchlist and ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Data already set will not be overwritten. Ratings are synced by default and watchlist sync is optional. The user will be prompted to enter their preferences and api keys on first run. 
+
+The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
 
 ## Installation Instructions:
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
 2. Install the script by running `python -m pip install TMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDbTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
    - Type of use: `Personal`
@@ -68,14 +70,21 @@
    - Application URL: `localhost`
    - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`
    - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
 5. Run `TMDBTraktSyncer.py` or open the terminal and navigate to the folder where `TMDBTraktSyncer.py` is located, then run `TMDBTraktSyncer.py` in the terminal.
 6. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
 7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
 
+## For Setting Up Automation See the Following Wiki Pages:
+- Setup Automation for:
+   - [Windows](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
+   - [Linux](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
+   - [macOS](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
+- Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
+
 ## Troubleshooting, Known Issues, Workarounds & Future Outlook:
 * Add support for review/comment sync [Issue #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1)
 * If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
 
 ## Screenshot:
 ![Demo](https://i.imgur.com/5LI04O2.png)
```

### Comparing `TMDBTraktSyncer-1.1.6/README.md` & `TMDBTraktSyncer-1.1.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # TMDB-Trakt-Syncer
 
-This Python script syncs user ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Ratings already set will not be overwritten. The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
+This Python script syncs user watchlist and ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Data already set will not be overwritten. Ratings are synced by default and watchlist sync is optional. The user will be prompted to enter their preferences and api keys on first run. 
+
+The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
 
 ## Installation Instructions:
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
 2. Install the script by running `python -m pip install TMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDbTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
    - Type of use: `Personal`
@@ -53,14 +55,21 @@
    - Application URL: `localhost`
    - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`
    - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
 5. Run `TMDBTraktSyncer.py` or open the terminal and navigate to the folder where `TMDBTraktSyncer.py` is located, then run `TMDBTraktSyncer.py` in the terminal.
 6. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
 7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
 
+## For Setting Up Automation See the Following Wiki Pages:
+- Setup Automation for:
+   - [Windows](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
+   - [Linux](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
+   - [macOS](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
+- Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
+
 ## Troubleshooting, Known Issues, Workarounds & Future Outlook:
 * Add support for review/comment sync [Issue #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1)
 * If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
 
 ## Screenshot:
 ![Demo](https://i.imgur.com/5LI04O2.png)
```

### Comparing `TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/authTrakt.py` & `TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/errorHandling.py` & `TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/tmdbData.py` & `TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/tmdbData.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,50 +10,81 @@
     response = EH.make_tmdb_request(url)
     json_data = json.loads(response.text)
     results = json_data['results']
     total_pages = json_data['total_pages']
     current_page = json_data['page']
     return results, total_pages, current_page
 
-def getTMDBRatings(tmdb_v4_token):
-    # Get TMDB Ratings
-    print('Processing TMDB Ratings')
+def getTMDBRatings():
+    print('Processing TMDB Data')
 
+    # Fetch Account ID
     response = EH.make_tmdb_request('https://api.themoviedb.org/3/account')
     json_data = json.loads(response.text)
     account_id = json_data['id']
+    
+    # Fetch Movies Watchlist
+    movie_watchlist = []
+    page = 1
+    total_pages = 1
+
+    while page <= total_pages:
+        url = f'https://api.themoviedb.org/3/account/{account_id}/watchlist/movies?page={page}'
+        results, total_pages, _ = fetch_data(url)
+        
+        for movie in results:
+            movie_watchlist.append({'Title': movie['title'], 'Year': movie['release_date'][:4], 'ID': movie['id'], 'Type': 'movie'})
+        
+        page += 1
+
+    # Fetch TV Show Watchlist
+    show_watchlist = []
+    page = 1
+    total_pages = 1
+
+    while page <= total_pages:
+        url = f'https://api.themoviedb.org/3/account/{account_id}/watchlist/tv?page={page}'
+        results, total_pages, _ = fetch_data(url)
+        
+        for show in results:
+            show_watchlist.append({'Title': show['name'], 'Year': show['first_air_date'][:4], 'ID': show['id'], 'Type': 'show'})
+        
+        page += 1
+
+    tmdb_watchlist = movie_watchlist + show_watchlist
 
+    # Fetch Movie Ratings
     movie_ratings = []
     page = 1
     total_pages = 1
 
     while page <= total_pages:
         url = f'https://api.themoviedb.org/3/account/{account_id}/rated/movies?page={page}'
         results, total_pages, _ = fetch_data(url)
         
         for movie in results:
             movie_ratings.append({'Title': movie['title'], 'Year': movie['release_date'][:4], 'Rating': movie['rating'], 'ID': movie['id'], 'Type': 'movie'})
         
         page += 1
 
-    # Fetch TV show ratings
+    # Fetch TV Show Ratings
     show_ratings = []
     page = 1
     total_pages = 1
 
     while page <= total_pages:
         url = f'https://api.themoviedb.org/3/account/{account_id}/rated/tv?page={page}'
         results, total_pages, _ = fetch_data(url)
         
         for show in results:
             show_ratings.append({'Title': show['name'], 'Year': show['first_air_date'][:4], 'Rating': show['rating'], 'ID': show['id'], 'Type': 'show'})
         
         page += 1
 
-    # Fetch episode ratings
+    # Fetch Episode Ratings
     episode_ratings = []
     page = 1
     total_pages = 1
 
     while page <= total_pages:
         url = f'https://api.themoviedb.org/3/account/{account_id}/rated/tv/episodes?page={page}'
         results, total_pages, _ = fetch_data(url)
@@ -75,10 +106,10 @@
                 'Type': 'episode'
             })
             
             page += 1
 
     tmdb_ratings = movie_ratings + show_ratings + episode_ratings
 
-    print('Processing TMDB Ratings Complete')
+    print('Processing TMDB Data Complete')
 
-    return tmdb_ratings
+    return tmdb_watchlist, tmdb_ratings
```

### Comparing `TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/traktData.py` & `TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/traktData.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,22 +2,40 @@
 import requests
 import urllib.parse
 try:
     from TMDBTraktSyncer import errorHandling as EH
 except ImportError:
     import errorHandling as EH
 
-def getTraktRatings(trakt_client_id, trakt_access_token):
-    # Get Trakt Ratings
-    print('Processing Trakt Ratings')
+def getTraktData():
+    # Process Trakt Ratings and Comments
+    print('Processing Trakt Data')
 
     response = EH.make_trakt_request('https://api.trakt.tv/users/me')
     json_data = json.loads(response.text)
     username_slug = json_data['ids']['slug']
     encoded_username = urllib.parse.quote(username_slug)
+    
+    # Get Trakt Watchlist Items
+    response = EH.make_trakt_request(f'https://api.trakt.tv/users/{encoded_username}/watchlist?sort=added,asc')
+    json_data = json.loads(response.text)
+
+    trakt_watchlist = []
+
+    for item in json_data:
+        if item['type'] == 'movie':
+            movie = item.get('movie')
+            movie_id = movie.get('ids', {}).get('tmdb')
+            trakt_watchlist.append({'Title': movie.get('title'), 'Year': movie.get('year'), 'ID': movie_id, 'Type': 'movie'})
+        elif item['type'] == 'show':
+            show = item.get('show')
+            show_id = show.get('ids', {}).get('tmdb')
+            trakt_watchlist.append({'Title': show.get('title'), 'Year': show.get('year'), 'ID': show_id, 'Type': 'show'})
+
+    # Get Trakt Ratings
     response = EH.make_trakt_request(f'https://api.trakt.tv/users/{encoded_username}/ratings')
     json_data = json.loads(response.text)
 
     movie_ratings = []
     show_ratings = []
     episode_ratings = []
 
@@ -46,10 +64,10 @@
                 'Episode': episode.get('number'),
                 'ShowID': show_tmdb_id,
                 'Type': 'episode'
             })
 
     trakt_ratings = movie_ratings + show_ratings + episode_ratings
 
-    print('Processing Trakt Ratings Complete')
+    print('Processing Trakt Data')
     
-    return trakt_ratings
+    return trakt_watchlist, trakt_ratings
```

### Comparing `TMDBTraktSyncer-1.1.6/TMDBTraktSyncer.egg-info/PKG-INFO` & `TMDBTraktSyncer-1.1.7/TMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.1.6
-Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
+Version: 1.1.7
+Summary: This python script syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # TMDB-Trakt-Syncer
 
-This Python script syncs user ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Ratings already set will not be overwritten. The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
+This Python script syncs user watchlist and ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Data already set will not be overwritten. Ratings are synced by default and watchlist sync is optional. The user will be prompted to enter their preferences and api keys on first run. 
+
+The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
 
 ## Installation Instructions:
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
 2. Install the script by running `python -m pip install TMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDbTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
    - Type of use: `Personal`
@@ -68,14 +70,21 @@
    - Application URL: `localhost`
    - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`
    - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
 5. Run `TMDBTraktSyncer.py` or open the terminal and navigate to the folder where `TMDBTraktSyncer.py` is located, then run `TMDBTraktSyncer.py` in the terminal.
 6. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
 7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
 
+## For Setting Up Automation See the Following Wiki Pages:
+- Setup Automation for:
+   - [Windows](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
+   - [Linux](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
+   - [macOS](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
+- Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
+
 ## Troubleshooting, Known Issues, Workarounds & Future Outlook:
 * Add support for review/comment sync [Issue #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1)
 * If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
 
 ## Screenshot:
 ![Demo](https://i.imgur.com/5LI04O2.png)
```

### Comparing `TMDBTraktSyncer-1.1.6/setup.py` & `TMDBTraktSyncer-1.1.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.6'
-DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.'
+VERSION = '1.1.7'
+DESCRIPTION = 'This python script syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.'
 
 # Setting up
 setup(
     name="TMDBTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
```

