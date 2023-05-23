# Comparing `tmp/IMDBTraktSyncer-1.2.5.tar.gz` & `tmp/IMDBTraktSyncer-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.2.5.tar", last modified: Sat May 20 22:19:45 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.2.6.tar", last modified: Tue May 23 23:44:42 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.2.5.tar` & `IMDBTraktSyncer-1.2.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 22:19:45.664542 IMDBTraktSyncer-1.2.5/
-drwxrwxrwx   0        0        0        0 2023-05-20 22:19:45.642543 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    16437 2023-05-20 20:44:52.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1913 2023-05-20 20:45:01.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4079 2023-05-16 01:53:33.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     3845 2023-05-20 20:45:06.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     5388 2023-05-20 20:44:48.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0     4612 2023-05-20 22:17:55.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     5488 2023-05-20 20:44:57.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-20 22:19:45.662542 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     7755 2023-05-20 22:19:45.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2023-05-20 22:19:45.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 22:19:45.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-20 22:19:45.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-05-20 22:19:45.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-20 22:19:45.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.2.5/LICENSE
--rw-rw-rw-   0        0        0     7755 2023-05-20 22:19:45.664542 IMDBTraktSyncer-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     7095 2023-05-20 18:20:58.000000 IMDBTraktSyncer-1.2.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 22:19:45.665544 IMDBTraktSyncer-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-05-20 22:19:34.000000 IMDBTraktSyncer-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:44:42.957660 IMDBTraktSyncer-1.2.6/
+drwxrwxrwx   0        0        0        0 2023-05-23 23:44:42.934671 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    21642 2023-05-23 23:30:49.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1900 2023-05-23 23:43:19.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4079 2023-05-16 01:53:33.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     3845 2023-05-20 20:45:06.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     7405 2023-05-23 21:38:34.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0     5841 2023-05-23 23:18:31.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     6981 2023-05-23 22:09:09.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:44:42.954670 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     8525 2023-05-23 23:44:42.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2023-05-23 23:44:42.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 23:44:42.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-23 23:44:42.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-05-23 23:44:42.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-23 23:44:42.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.2.6/LICENSE
+-rw-rw-rw-   0        0        0     8525 2023-05-23 23:44:42.956660 IMDBTraktSyncer-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7855 2023-05-23 23:42:16.000000 IMDBTraktSyncer-1.2.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-23 23:44:42.957660 IMDBTraktSyncer-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-05-23 23:37:34.000000 IMDBTraktSyncer-1.2.6/setup.py
```

### Comparing `IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import requests
 import time
 import logging
 from selenium import webdriver
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.by import By
-from selenium.common.exceptions import StaleElementReferenceException
+from selenium.common.exceptions import NoSuchElementException, TimeoutException, StaleElementReferenceException
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.common.exceptions import SessionNotCreatedException
 try:
     from IMDBTraktSyncer import checkChromedriver
     from IMDBTraktSyncer import verifyCredentials as VC
@@ -64,15 +64,15 @@
                 extract_message = error_message.split("Stacktrace:")[0].replace("Message: session not created:", "").strip()
                 print(f"Error: {extract_message}")
                 print("See this link for details on how to fix: https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/16")
                 raise SystemExit
             else:
                 raise
 
-        wait = WebDriverWait(driver, 20)
+        wait = WebDriverWait(driver, 10)
 
         driver.get('https://www.imdb.com/registration/signin')
 
         # wait for sign in link to appear and then click it
         sign_in_link = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, 'a.list-group-item > .auth-provider-text')))
         if 'IMDb' in sign_in_link.text:
             sign_in_link.click()
@@ -101,39 +101,185 @@
             print("\nPossible IMDB captcha check or IMDB login incorrect.")
             print("\nIf your login is correct then an IMDB captcha check likely the cause of this error. To fix this, simply login to the IMDB website in your browser, preferably Chrome, and from the same computer. If logged in, log out and log back in. It may ask you to fill in a captcha; complete it and finish logging in. After logging in successfully on your browser, run the script again and it should work. You may need to repeat this step once or twice if it still gives you issues.")
             print("\nIf your IMDB login is incorrect, simply edit the credentials.txt file with the correct login or delete the credentials file and run the script again.")
             print("\nSee this GitHub link for more details: https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/2")
             print("\nStopping script...")
             raise SystemExit
         
-        trakt_ratings, trakt_reviews = traktData.getTraktData()
-        imdb_ratings, imdb_reviews = imdbData.getImdbData(imdb_username, imdb_password, driver, directory, wait)
+        trakt_watchlist, trakt_ratings, trakt_reviews = traktData.getTraktData()
+        imdb_watchlist, imdb_ratings, imdb_reviews = imdbData.getImdbData(imdb_username, imdb_password, driver, directory, wait)
 
         #Get trakt and imdb ratings and filter out trakt ratings with missing imdb id
         trakt_ratings = [rating for rating in trakt_ratings if rating['ID'] is not None]
         imdb_ratings = [rating for rating in imdb_ratings if rating['ID'] is not None]
         trakt_reviews = [review for review in trakt_reviews if review['ID'] is not None]
         imdb_reviews = [review for review in imdb_reviews if review['ID'] is not None]
+        trakt_watchlist = [item for item in trakt_watchlist if item['ID'] is not None]
+        imdb_watchlist = [item for item in imdb_watchlist if item['ID'] is not None]
         #Filter out ratings already set
         imdb_ratings_to_set = [rating for rating in trakt_ratings if rating['ID'] not in [imdb_rating['ID'] for imdb_rating in imdb_ratings]]
         trakt_ratings_to_set = [rating for rating in imdb_ratings if rating['ID'] not in [trakt_rating['ID'] for trakt_rating in trakt_ratings]]
         imdb_reviews_to_set = [review for review in trakt_reviews if review['ID'] not in [imdb_review['ID'] for imdb_review in imdb_reviews]]
         trakt_reviews_to_set = [review for review in imdb_reviews if review['ID'] not in [trakt_review['ID'] for trakt_review in trakt_reviews]]
+        imdb_watchlist_to_set = [item for item in trakt_watchlist if item['ID'] not in [imdb_item['ID'] for imdb_item in imdb_watchlist]]
+        trakt_watchlist_to_set = [item for item in imdb_watchlist if item['ID'] not in [trakt_item['ID'] for trakt_item in trakt_watchlist]]
         # Remove duplicate reviews and filter by out any items for imdb_reviews_to_set where comment length is less than 600 characters
         def remove_duplicates_and_filter(lst, key, min_comment_length=None):
             seen = set()
             result = []
             for item in lst:
                 if item[key] not in seen and (min_comment_length is None or ('Comment' in item and len(item['Comment']) >= min_comment_length)):
                     seen.add(item[key])
                     result.append(item)
             return result
 
         imdb_reviews_to_set = remove_duplicates_and_filter(imdb_reviews_to_set, 'ID', 600)
         trakt_reviews_to_set = remove_duplicates_and_filter(trakt_reviews_to_set, 'ID')
+        
+        # If sync_watchlist_value is true
+        if VC.sync_watchlist_value:
+            # Set Trakt Watchlist Items
+            if trakt_watchlist_to_set:
+                print('Setting Trakt Watchlist Items')
+
+                # Count the total number of items
+                num_items = len(trakt_watchlist_to_set)
+                item_count = 0
+
+                for item in trakt_watchlist_to_set:
+                    item_count += 1
+                    imdb_id = item['ID']
+                    media_type = item['Type']  # 'movie', 'show', or 'episode'
+
+                    url = f"https://api.trakt.tv/sync/watchlist"
+
+                    data = {
+                        "movies": [],
+                        "shows": [],
+                        "episodes": []
+                    }
+
+                    if media_type == 'movie':
+                        data['movies'].append({
+                            "ids": {
+                                "imdb": imdb_id
+                            }
+                        })
+                    elif media_type == 'show':
+                        data['shows'].append({
+                            "ids": {
+                                "imdb": imdb_id
+                            }
+                        })
+                    elif media_type == 'episode':
+                        data['episodes'].append({
+                            "ids": {
+                                "imdb": imdb_id
+                            }
+                        })
+
+                    response = EH.make_trakt_request(url, payload=data)
+                    if response:
+                        print(f"Adding item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist")
+                    else:
+                        print(f"Failed to add item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist")
+                        print("Error Response:", response.content, response.status_code)
+
+                print('Trakt Watchlist Items Set Successfully')
+            else:
+                print('No Trakt Watchlist Items To Set')
+
+            # Set IMDB Watchlist Items
+            if imdb_watchlist_to_set:
+                print('Setting IMDB Watchlist Items')
+                
+                # Count the total number of items
+                num_items = len(imdb_watchlist_to_set)
+                item_count = 0
+                
+                for item in imdb_watchlist_to_set:
+                    try:
+                        item_count += 1
+                        year_str = f' ({item["Year"]})' if item["Year"] is not None else '' # sometimes year is None for episodes from trakt so remove it from the print string
+                        print(f"Adding item ({item_count} of {num_items}): {item['Title']}{year_str} to IMDB Watchlist")
+                        
+                        driver.get(f'https://www.imdb.com/title/{item["ID"]}/')
+                                            
+                        watchlist_button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"]')))
+                        
+                        # Check if item is already in watchlist otherwise skip it
+                        if 'ipc-icon--done' not in watchlist_button.get_attribute('innerHTML'):
+                            watchlist_button.click()
+                            time.sleep(1)
+                    except (NoSuchElementException, TimeoutException):
+                        print(f"Failed to add item ({item_count} of {num_items}): {item['Title']}{year_str} to IMDB Watchlist ({item['ID']})")
+                        pass
+
+                
+                print('Setting IMDB Watchlist Items Complete')
+            else:
+                print('No IMDB Watchlist Items To Set')
+
+        #Set Trakt Ratings
+        if trakt_ratings_to_set:
+            print('Setting Trakt Ratings')
+
+            # Set the API endpoints
+            rate_url = "https://api.trakt.tv/sync/ratings"
+            
+            # Count the total number of items
+            num_items = len(trakt_ratings_to_set)
+            item_count = 0
+                    
+            # Loop through your data table and rate each item on Trakt
+            for item in trakt_ratings_to_set:
+                item_count += 1
+                if item["Type"] == "show":
+                    # This is a TV show
+                    data = {
+                        "shows": [{
+                            "ids": {
+                                "imdb": item["ID"]
+                            },
+                            "rating": item["Rating"]
+                        }]
+                    }
+                    print(f"Rating TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
+                elif item["Type"] == "movie":
+                    # This is a movie
+                    data = {
+                        "movies": [{
+                            "ids": {
+                                "imdb": item["ID"]
+                            },
+                            "rating": item["Rating"]
+                        }]
+                    }
+                    print(f"Rating movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
+                elif item["Type"] == "episode":
+                    # This is an episode
+                    data = {
+                        "episodes": [{
+                            "ids": {
+                                "imdb": item["ID"]
+                            },
+                            "rating": item["Rating"]
+                        }]
+                    }
+                    print(f"Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
+
+                # Make the API call to rate the item
+                response = EH.make_trakt_request(rate_url, payload=data)
+
+                if response is None:
+                    print(f"Error rating {item}: {response.content}")
+
+            print('Setting Trakt Ratings Complete')
+        else:
+            print('No Trakt Ratings To Set')
 
         #Set IMDB Ratings
         if imdb_ratings_to_set:
             print('Setting IMDB Ratings')
 
             # loop through each movie and TV show rating and submit rating on IMDB website
             for i, item in enumerate(imdb_ratings_to_set, 1):
@@ -148,120 +294,29 @@
                     if element_rating_bar:
                         driver.execute_script("arguments[0].click();", button)
                         rating_option_element = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, f'button[aria-label="Rate {item["Rating"]}"]')))
                         driver.execute_script("arguments[0].click();", rating_option_element)
                         submit_element = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button.ipc-rating-prompt__rate-button')))
                         submit_element.click()
                         time.sleep(1)
-                except:
+                except (NoSuchElementException, TimeoutException):
+                    print(f'Failed to rate {item["Type"]}: ({i} of {len(imdb_ratings_to_set)}) {item["Title"]}{year_str}: {item["Rating"]}/10 on IMDB ({item["ID"]})')
                     pass
 
             print('Setting IMDB Ratings Complete')
         else:
             print('No IMDB Ratings To Set')
 
+        # If sync_reviews_value is true
         if VC.sync_reviews_value:
-            #Set Trakt Ratings
-            if trakt_ratings_to_set:
-                print('Setting Trakt Ratings')
-
-                # Set the API endpoints
-                rate_url = "https://api.trakt.tv/sync/ratings"
-                
-                # Count the total number of items to rate
-                num_items = len(trakt_ratings_to_set)
-                item_count = 0
-                        
-                # Loop through your data table and rate each item on Trakt
-                for item in trakt_ratings_to_set:
-                    item_count += 1
-                    if item["Type"] == "show":
-                        # This is a TV show
-                        data = {
-                            "shows": [{
-                                "ids": {
-                                    "imdb": item["ID"]
-                                },
-                                "rating": item["Rating"]
-                            }]
-                        }
-                        print(f"Rating TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
-                    elif item["Type"] == "movie":
-                        # This is a movie
-                        data = {
-                            "movies": [{
-                                "ids": {
-                                    "imdb": item["ID"]
-                                },
-                                "rating": item["Rating"]
-                            }]
-                        }
-                        print(f"Rating movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
-                    elif item["Type"] == "episode":
-                        # This is an episode
-                        data = {
-                            "episodes": [{
-                                "ids": {
-                                    "imdb": item["ID"]
-                                },
-                                "rating": item["Rating"]
-                            }]
-                        }
-                        print(f"Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
-
-                    # Make the API call to rate the item
-                    response = EH.make_trakt_request(rate_url, payload=data)
-
-                    if response is None:
-                        print(f"Error rating {item}: {response.content}")
-
-                print('Setting Trakt Ratings Complete')
-            else:
-                print('No Trakt Ratings To Set')
-            
-            if imdb_reviews_to_set:
-                # Call the check_last_run() function
-                if VC.check_imdb_reviews_last_submitted():
-                    print('Setting IMDB Reviews')
-                    
-                    for review in imdb_reviews_to_set:
-                    
-                        driver.get(f'https://contribute.imdb.com/review/{review["ID"]}/add?bus=imdb')
-                        
-                        review_title_input = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "input.klondike-input")))
-                        review_input = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "textarea.klondike-textarea")))
-                        
-                        review_title_input.send_keys("My Review")
-                        review_input.send_keys(review["Comment"])
-                        
-                        no_element = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "ul.klondike-userreview-spoiler li:nth-child(2)")))
-                        yes_element = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "ul.klondike-userreview-spoiler li:nth-child(1)")))
-                        
-                        if review["Spoiler"]:
-                            yes_element.click()                        
-                        else:
-                            no_element.click()
-                                                
-                        submit_button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "input.a-button-input[type='submit']")))
-
-                        submit_button.click()
-                        
-                        time.sleep(1)
-                    
-                    print('Setting IMDB Reviews Complete')
-                else:
-                    print('IMDB reviews were submitted within the last 7 days. Skipping IMDB review submission.')
-            else:
-                print('No IMDB Reviews To Set')
-
             # Set Trakt Reviews
             if trakt_reviews_to_set:
                 print('Setting Trakt Reviews')
 
-                # Count the total number of items to rate
+                # Count the total number of items
                 num_items = len(trakt_reviews_to_set)
                 item_count = 0
 
                 for review in trakt_reviews_to_set:
                     item_count += 1
                     imdb_id = review['ID']
                     comment = review['Comment']
@@ -299,14 +354,59 @@
                         print(f"Failed to submit comment ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on Trakt")
                         print("Error Response:", response.content, response.status_code)
 
                 print('Trakt Reviews Set Successfully')
             else:
                 print('No Trakt Reviews To Set')
 
+            # Set IMDB Reviews
+            if imdb_reviews_to_set:
+                # Call the check_last_run() function
+                if VC.check_imdb_reviews_last_submitted():
+                    print('Setting IMDB Reviews')
+                    
+                    # Count the total number of items
+                    num_items = len(trakt_reviews_to_set)
+                    item_count = 0
+                    
+                    for review in imdb_reviews_to_set:
+                        item_count += 1
+                        try:
+                            print(f"Submitting review ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on IMDB")
+                            driver.get(f'https://contribute.imdb.com/review/{review["ID"]}/add?bus=imdb')
+                            
+                            review_title_input = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "input.klondike-input")))
+                            review_input = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "textarea.klondike-textarea")))
+                            
+                            review_title_input.send_keys("My Review")
+                            review_input.send_keys(review["Comment"])
+                            
+                            no_element = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "ul.klondike-userreview-spoiler li:nth-child(2)")))
+                            yes_element = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "ul.klondike-userreview-spoiler li:nth-child(1)")))
+                            
+                            if review["Spoiler"]:
+                                yes_element.click()                        
+                            else:
+                                no_element.click()
+                                                    
+                            submit_button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "input.a-button-input[type='submit']")))
+
+                            submit_button.click()
+                            
+                            time.sleep(1)
+                        except (NoSuchElementException, TimeoutException):
+                            print(f"Failed to submit review ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on IMDB ({item['ID']})")
+                            pass
+                    
+                    print('Setting IMDB Reviews Complete')
+                else:
+                    print('IMDB reviews were submitted within the last 7 days. Skipping IMDB review submission.')
+            else:
+                print('No IMDB Reviews To Set')
+
         #Close web driver
         print("Closing webdriver...")
         driver.quit()
         service.stop()
     
     except Exception as e:
         error_message = "An error occurred while running the script."
```

### Comparing `IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/authTrakt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import requests
-import time
 try:
     from IMDBTraktSyncer import errorHandling as EH
 except ImportError:
     import errorHandling as EH
 
 def authenticate(client_id, client_secret):
     CLIENT_ID = client_id
```

### Comparing `IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/errorHandling.py` & `IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/imdbData.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,74 +12,125 @@
 from chromedriver_py import binary_path
 try:
     from IMDBTraktSyncer import errorHandling as EH
 except ImportError:
     import errorHandling as EH
 
 def getImdbData(imdb_username, imdb_password, driver, directory, wait):
-    # Process IMDB Ratings and Reviews
-    print('Processing IMDB Ratings and Reviews')
+    # Process IMDB Ratings Reviews & Watchlist
+    print('Processing IMDB Data')
+    
+    #Get IMDB Watchlist Items
+    try:
+        driver.get('https://www.imdb.com/list/watchlist')
 
-    driver.get('https://www.imdb.com/list/ratings')
+        csv_link = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, ".export a")))
+        csv_link.click()
 
-    dropdown = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, ".circle")))
-    dropdown.click()
+        #Wait for csv download to complete
+        time.sleep(8)
 
-    csv_link = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, ".pop-up-menu-list-items a.pop-up-menu-list-item-link")))
-    csv_link.click()
+        imdb_watchlist = []
 
-    #Wait for csv download to complete
-    time.sleep(8)
+        # Read the watchlist items from the CSV file
+        here = os.path.abspath(os.path.dirname(__file__))
+        watchlist_path = os.path.join(here, 'WATCHLIST.csv')
+        try:
+            with open(watchlist_path, 'r') as file:
+                reader = csv.reader(file)
+                header = next(reader)  # skip the header row
+                for row in reader:
+                    title = row[5]
+                    year = row[10]
+                    imdb_id = row[1]
+                    if "tvSeries" in row[7] or "tvMiniSeries" in row[7]:
+                        type = "show"
+                    elif "tvEpisode" in row[7]:
+                        type = "episode"
+                    elif "movie" in row[7]:
+                        type = "movie"
+                    else:
+                        type = "unknown"
+                    imdb_watchlist.append({'Title': title, 'Year': year, 'ID': imdb_id, 'Type': type})
+        except FileNotFoundError:
+            print('Ratings file not found')
+            
+        # Delete csv files
+        for file in os.listdir(directory):
+            if file.endswith('.csv') and 'WATCHLIST' in file:
+                os.remove(os.path.join(directory, file))
+
+    except (NoSuchElementException, TimeoutException):
+        # No IMDB Watchlist Items
+        imdb_watchlist = []
+        pass
+    
+    # Get IMDB Ratings
+    try:
+        driver.get('https://www.imdb.com/list/ratings')
 
-    imdb_ratings = []
+        dropdown = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, ".circle")))
+        dropdown.click()
 
-    # Read the ratings from the CSV file
-    here = os.path.abspath(os.path.dirname(__file__))
-    ratings_path = os.path.join(here, 'ratings.csv')
-    try:
-        with open(ratings_path, 'r') as file:
-            reader = csv.reader(file)
-            header = next(reader)  # skip the header row
-            for row in reader:
-                title = row[3]
-                year = row[8]
-                rating = row[1]
-                imdb_id = row[0]
-                if "tvSeries" in row[5] or "tvMiniSeries" in row[5]:
-                    type = "show"
-                elif "tvEpisode" in row[5]:
-                    type = "episode"
-                elif "movie" in row[5]:
-                    type = "movie"
-                else:
-                    type = "unknown"
-                imdb_ratings.append({'Title': title, 'Year': year, 'Rating': rating, 'ID': imdb_id, 'Type': type})
-    except FileNotFoundError:
-        print('Ratings file not found')
-        
-    # Delete csv files
-    for file in os.listdir(directory):
-        if file.endswith('.csv') and 'ratings' in file:
-            os.remove(os.path.join(directory, file))
+        csv_link = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, ".pop-up-menu-list-items a.pop-up-menu-list-item-link")))
+        csv_link.click()
 
-    #Get IMDB Reviews
-    driver.get('https://www.imdb.com/profile')
-    reviews_link = driver.find_element(By.CSS_SELECTOR, "div.aux-content-widget-2 div.subNavItem a[href*='comments-index']")
-    reviews_link.click()
-    
+        #Wait for csv download to complete
+        time.sleep(8)
+
+        imdb_ratings = []
+
+        # Read the ratings from the CSV file
+        here = os.path.abspath(os.path.dirname(__file__))
+        ratings_path = os.path.join(here, 'ratings.csv')
+        try:
+            with open(ratings_path, 'r') as file:
+                reader = csv.reader(file)
+                header = next(reader)  # skip the header row
+                for row in reader:
+                    title = row[3]
+                    year = row[8]
+                    rating = row[1]
+                    imdb_id = row[0]
+                    if "tvSeries" in row[5] or "tvMiniSeries" in row[5]:
+                        type = "show"
+                    elif "tvEpisode" in row[5]:
+                        type = "episode"
+                    elif "movie" in row[5]:
+                        type = "movie"
+                    else:
+                        type = "unknown"
+                    imdb_ratings.append({'Title': title, 'Year': year, 'Rating': rating, 'ID': imdb_id, 'Type': type})
+        except FileNotFoundError:
+            print('Ratings file not found')
+            
+        # Delete csv files
+        for file in os.listdir(directory):
+            if file.endswith('.csv') and 'ratings' in file:
+                os.remove(os.path.join(directory, file))
+    except (NoSuchElementException, TimeoutException):
+        # No IMDB Ratings
+        imdb_ratings = []
+        pass
+            
     def get_media_type(imdb_id):
         url = f"https://api.trakt.tv/search/imdb/{imdb_id}"
         response = EH.make_trakt_request(url)
         if response:
             results = response.json()
             if results:
                 media_type = results[0].get('type')
                 return media_type
         return None
 
+    #Get IMDB Reviews
+    driver.get('https://www.imdb.com/profile')
+    reviews_link = driver.find_element(By.CSS_SELECTOR, "div.aux-content-widget-2 div.subNavItem a[href*='comments-index']")
+    reviews_link.click()
+
     reviews = []
 
     while True:
         try:
             review_elements = wait.until(EC.presence_of_all_elements_located((By.CSS_SELECTOR, ".imdb-user-review")))
             if not review_elements:
                 break  # No review elements found, exit the loop
@@ -121,10 +172,10 @@
                 break  # "Next" link not found or timed out waiting for the 'Next' link, exit the loop
         except Exception as e:
             print(f"Exception occurred: {e}")
             break
 
     imdb_reviews = reviews
 
-    print('Processing IMDB Ratings and Reviews Complete')
+    print('Processing IMDB Data Complete')
     
-    return imdb_ratings, imdb_reviews
+    return imdb_watchlist, imdb_ratings, imdb_reviews
```

### Comparing `IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/traktData.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,21 +5,46 @@
 try:
     from IMDBTraktSyncer import errorHandling as EH
 except ImportError:
     import errorHandling as EH
 
 def getTraktData():
     # Process Trakt Ratings and Comments
-    print('Processing Trakt Ratings and Comments')
+    print('Processing Trakt Data')
 
     response = EH.make_trakt_request('https://api.trakt.tv/users/me')
     json_data = json.loads(response.text)
     username_slug = json_data['ids']['slug']
     encoded_username = urllib.parse.quote(username_slug)
-    response = EH.make_trakt_request(f'https://api.trakt.tv/users/{encoded_username}/ratings')
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
+            movie_id = movie.get('ids', {}).get('imdb')
+            trakt_watchlist.append({'Title': movie.get('title'), 'Year': movie.get('year'), 'ID': movie_id, 'Type': 'movie'})
+        elif item['type'] == 'show':
+            show = item.get('show')
+            show_id = show.get('ids', {}).get('imdb')
+            trakt_watchlist.append({'Title': show.get('title'), 'Year': show.get('year'), 'ID': show_id, 'Type': 'show'})
+        elif item['type'] == 'episode':
+            show = item.get('show')
+            show_title = show.get('title')
+            episode = item.get('episode')
+            episode_id = episode.get('ids', {}).get('imdb')
+            episode_title = f'{show_title}: {episode.get("title")}'
+            trakt_watchlist.append({'Title': episode_title, 'Year': episode.get('year'), 'ID': episode_id, 'Type': 'episode'})
+    
+    # Get Trakt Ratings
+    response = EH.make_trakt_request(f'https://api.trakt.tv/users/{encoded_username}/ratings?sort=newest')
     json_data = json.loads(response.text)
 
     movie_ratings = []
     show_ratings = []
     episode_ratings = []
 
     for item in json_data:
@@ -38,15 +63,15 @@
             episode_id = episode.get('ids', {}).get('imdb')
             episode_title = f'{show_title}: {episode.get("title")}'
             episode_ratings.append({'Title': episode_title, 'Year': episode.get('year'), 'Rating': item.get('rating'), 'ID': episode_id, 'Type': 'episode'})
 
     trakt_ratings = movie_ratings + show_ratings + episode_ratings
 
     # Get Trakt Comments
-    response = EH.make_trakt_request(f'https://api.trakt.tv/users/{encoded_username}/comments')
+    response = EH.make_trakt_request(f'https://api.trakt.tv/users/{encoded_username}/comments?sort=newest')
     json_data = json.loads(response.text)
     total_pages = response.headers.get('X-Pagination-Page-Count')
     trakt_comments = []
 
     for page in range(1, int(total_pages) + 1):
         response = EH.make_trakt_request(f'https://api.trakt.tv/users/{encoded_username}/comments', params={'page': page})
         json_data = json.loads(response.text)
@@ -92,10 +117,10 @@
                 'ID': show_movie_or_episode_imdb_id,
                 'TraktCommentID': trakt_comment_id,
                 'Comment': trakt_comment,
                 'Spoiler': spoiler,
                 'Type': comment_type
             })
 
-    print('Processing Trakt Ratings and Comments Complete')
+    print('Processing Trakt Data Complete')
 
-    return trakt_ratings, trakt_comments
+    return trakt_watchlist, trakt_ratings, trakt_comments
```

### Comparing `IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/verifyCredentials.py`

 * *Files 18% similar despite different names*

```diff
@@ -55,14 +55,63 @@
     client_id = values["trakt_client_id"]
     client_secret = values["trakt_client_secret"]
     trakt_access_token = authTrakt.authenticate(client_id, client_secret)
     values["trakt_access_token"] = trakt_access_token
     with open(file_path, "w") as f:
         json.dump(values, f)
 
+
+def prompt_sync_watchlist():
+    # Define the file path
+    here = os.path.abspath(os.path.dirname(__file__))
+    file_path = os.path.join(here, 'credentials.txt')
+
+    # Check if credentials file exists
+    try:
+        with open(file_path, 'r') as file:
+            credentials = json.load(file)
+            sync_watchlist_value = credentials.get('sync_watchlist')
+            if sync_watchlist_value is not None:
+                return sync_watchlist_value
+    except FileNotFoundError:
+        pass
+
+    while True:
+        # Prompt the user for input
+        print("Do you want to sync watchlists? (y/n)")
+        user_input = input("Enter your choice: ")
+
+        # Validate user input
+        if user_input.lower() == 'y':
+            sync_watchlist_value = True
+            break
+        elif user_input.lower() == 'n':
+            sync_watchlist_value = False
+            break
+        else:
+            # Invalid input, ask again
+            print("Invalid input. Please enter 'y' or 'n'.")
+
+    # Update the value in the JSON file
+    credentials = {}
+    try:
+        with open(file_path, 'r') as file:
+            credentials = json.load(file)
+    except FileNotFoundError:
+        pass
+
+    credentials['sync_watchlist'] = sync_watchlist_value
+
+    with open(file_path, 'w') as file:
+        json.dump(credentials, file)
+
+    # return true or false
+    return sync_watchlist_value
+sync_watchlist_value = prompt_sync_watchlist()
+
 # Last run function, used to determine when the last time IMDB reviews were submitted    
 def check_imdb_reviews_last_submitted():
     # Load credentials from credentials.txt
     if os.path.exists(file_path):
         with open(file_path, 'r') as file:
             credentials = json.load(file)
     else:
```

### Comparing `IMDBTraktSyncer-1.2.5/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.2.6/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.2.5
+Version: 1.2.6
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # IMDB-Trakt-Syncer
-This Python script syncs user ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Ratings and comments already set will not be overwritten. The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux, Mac, and ChromeOS). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
+This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Data already set will not be overwritten. Ratings are synced by default. Watchlist and comment/review sync is optional. The user will be prompted to enter their settings and credentials on first run.
+
+The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux, Mac, and ChromeOS). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
 
 ## Installation Instructions
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run the script by executing `IMDBTraktSyncer` in the command line.
 5. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your IMDB username and password. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
@@ -55,14 +57,21 @@
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/).  _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) and extract it to the desired directory.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run `IMDBTraktSyncer.py` or open the terminal and navigate to the folder where `IMDBTraktSyncer.py` is located. Run `IMDBTraktSyncer.py` in the terminal.
 5. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your IMDB username and password. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
 6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
 
+## For Setting Up Automation See the Following Wiki Pages:
+- Setup Automation for:
+   - [Windows](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
+   - [Linux](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
+   - [macOS](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
+- Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
+
 ## Troubleshooting, Known Issues, Workarounds & Future Outlook
 - If IMDB requires a captcha on login, and you see "Not signed in" appear in the script, the captcha is likely the cause. To fix this, navigate to the IMDB website in your browser (preferably Chrome) from the same computer. If you're already logged in, log out and log back in. It may ask you to fill in a captcha. Complete the captcha and finish logging in. After successfully logging in on your browser, run the script again, and it should work. You may need to repeat this step once or twice if the issue persists. Adding a captcha solver to the script is being considered but not currently implemented. [Issue #2](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/2)
 - If you see an error about having the incorrect version of Chromedriver, uninstall it by running the following command in the command line: `python -m pip uninstall chromedriver-py`. In your Chrome browser, go to Settings > About Chrome and check the prefix for your version (e.g., 112... or 111). If the prefix matches your Chrome version, navigate to the [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that matches the prefix for your Chrome version. Copy the version number you need (e.g 113.0.5672.63), then run the following command in the command line: `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct version of Chromedriver. Run the script again, and it should work. [Issue #16](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/16)
 - If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
 - Due to IMDB's lack of API and rating import ability, this script uses an unconventional method that mimics using a web browser to set ratings on IMDB. Therefore, there are many points of failure that could arise. The script will be updated as best as possible.
 
 ## Screenshot
@@ -78,7 +87,8 @@
 - Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
 
 ## Also Posted On
 - [PyPi](https://pypi.org/project/IMDBTraktSyncer/)
 - [Reddit](https://www.reddit.com/r/trakt/comments/132heo0/IMDB_trakt_rating_syncer_tool_sync_both_ways/)
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
```

### Comparing `IMDBTraktSyncer-1.2.5/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.2.6/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.5/LICENSE` & `IMDBTraktSyncer-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.5/PKG-INFO` & `IMDBTraktSyncer-1.2.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.2.5
+Version: 1.2.6
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # IMDB-Trakt-Syncer
-This Python script syncs user ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Ratings and comments already set will not be overwritten. The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux, Mac, and ChromeOS). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
+This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Data already set will not be overwritten. Ratings are synced by default. Watchlist and comment/review sync is optional. The user will be prompted to enter their settings and credentials on first run.
+
+The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux, Mac, and ChromeOS). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
 
 ## Installation Instructions
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run the script by executing `IMDBTraktSyncer` in the command line.
 5. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your IMDB username and password. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
@@ -55,14 +57,21 @@
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/).  _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) and extract it to the desired directory.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run `IMDBTraktSyncer.py` or open the terminal and navigate to the folder where `IMDBTraktSyncer.py` is located. Run `IMDBTraktSyncer.py` in the terminal.
 5. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your IMDB username and password. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
 6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
 
+## For Setting Up Automation See the Following Wiki Pages:
+- Setup Automation for:
+   - [Windows](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
+   - [Linux](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
+   - [macOS](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
+- Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
+
 ## Troubleshooting, Known Issues, Workarounds & Future Outlook
 - If IMDB requires a captcha on login, and you see "Not signed in" appear in the script, the captcha is likely the cause. To fix this, navigate to the IMDB website in your browser (preferably Chrome) from the same computer. If you're already logged in, log out and log back in. It may ask you to fill in a captcha. Complete the captcha and finish logging in. After successfully logging in on your browser, run the script again, and it should work. You may need to repeat this step once or twice if the issue persists. Adding a captcha solver to the script is being considered but not currently implemented. [Issue #2](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/2)
 - If you see an error about having the incorrect version of Chromedriver, uninstall it by running the following command in the command line: `python -m pip uninstall chromedriver-py`. In your Chrome browser, go to Settings > About Chrome and check the prefix for your version (e.g., 112... or 111). If the prefix matches your Chrome version, navigate to the [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that matches the prefix for your Chrome version. Copy the version number you need (e.g 113.0.5672.63), then run the following command in the command line: `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct version of Chromedriver. Run the script again, and it should work. [Issue #16](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/16)
 - If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
 - Due to IMDB's lack of API and rating import ability, this script uses an unconventional method that mimics using a web browser to set ratings on IMDB. Therefore, there are many points of failure that could arise. The script will be updated as best as possible.
 
 ## Screenshot
@@ -78,7 +87,8 @@
 - Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
 
 ## Also Posted On
 - [PyPi](https://pypi.org/project/IMDBTraktSyncer/)
 - [Reddit](https://www.reddit.com/r/trakt/comments/132heo0/IMDB_trakt_rating_syncer_tool_sync_both_ways/)
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
```

### Comparing `IMDBTraktSyncer-1.2.5/README.md` & `IMDBTraktSyncer-1.2.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # IMDB-Trakt-Syncer
-This Python script syncs user ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Ratings and comments already set will not be overwritten. The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux, Mac, and ChromeOS). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
+This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Data already set will not be overwritten. Ratings are synced by default. Watchlist and comment/review sync is optional. The user will be prompted to enter their settings and credentials on first run.
+
+The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux, Mac, and ChromeOS). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
 
 ## Installation Instructions
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run the script by executing `IMDBTraktSyncer` in the command line.
 5. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your IMDB username and password. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
@@ -40,14 +42,21 @@
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/).  _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) and extract it to the desired directory.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run `IMDBTraktSyncer.py` or open the terminal and navigate to the folder where `IMDBTraktSyncer.py` is located. Run `IMDBTraktSyncer.py` in the terminal.
 5. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your IMDB username and password. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
 6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
 
+## For Setting Up Automation See the Following Wiki Pages:
+- Setup Automation for:
+   - [Windows](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
+   - [Linux](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
+   - [macOS](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
+- Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
+
 ## Troubleshooting, Known Issues, Workarounds & Future Outlook
 - If IMDB requires a captcha on login, and you see "Not signed in" appear in the script, the captcha is likely the cause. To fix this, navigate to the IMDB website in your browser (preferably Chrome) from the same computer. If you're already logged in, log out and log back in. It may ask you to fill in a captcha. Complete the captcha and finish logging in. After successfully logging in on your browser, run the script again, and it should work. You may need to repeat this step once or twice if the issue persists. Adding a captcha solver to the script is being considered but not currently implemented. [Issue #2](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/2)
 - If you see an error about having the incorrect version of Chromedriver, uninstall it by running the following command in the command line: `python -m pip uninstall chromedriver-py`. In your Chrome browser, go to Settings > About Chrome and check the prefix for your version (e.g., 112... or 111). If the prefix matches your Chrome version, navigate to the [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that matches the prefix for your Chrome version. Copy the version number you need (e.g 113.0.5672.63), then run the following command in the command line: `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct version of Chromedriver. Run the script again, and it should work. [Issue #16](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/16)
 - If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
 - Due to IMDB's lack of API and rating import ability, this script uses an unconventional method that mimics using a web browser to set ratings on IMDB. Therefore, there are many points of failure that could arise. The script will be updated as best as possible.
 
 ## Screenshot
@@ -63,7 +72,8 @@
 - Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
 
 ## Also Posted On
 - [PyPi](https://pypi.org/project/IMDBTraktSyncer/)
 - [Reddit](https://www.reddit.com/r/trakt/comments/132heo0/IMDB_trakt_rating_syncer_tool_sync_both_ways/)
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
```

### Comparing `IMDBTraktSyncer-1.2.5/setup.py` & `IMDBTraktSyncer-1.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.2.5'
+VERSION = '1.2.6'
 DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

