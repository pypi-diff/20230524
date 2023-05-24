# Comparing `tmp/ReverseTwitterScraper-0.6.tar.gz` & `tmp/ReverseTwitterScraper-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReverseTwitterScraper-0.6.tar", last modified: Tue May  9 20:19:30 2023, max compression
+gzip compressed data, was "ReverseTwitterScraper-0.7.tar", last modified: Wed May 24 21:55:56 2023, max compression
```

## Comparing `ReverseTwitterScraper-0.6.tar` & `ReverseTwitterScraper-0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 20:19:30.383320 ReverseTwitterScraper-0.6/
--rw-rw-rw-   0        0        0     1090 2023-03-08 21:13:40.000000 ReverseTwitterScraper-0.6/LICENSE
--rw-rw-rw-   0        0        0     7671 2023-05-09 20:19:30.383320 ReverseTwitterScraper-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     7176 2023-05-04 15:26:42.000000 ReverseTwitterScraper-0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 20:19:30.363316 ReverseTwitterScraper-0.6/ReverseTwitterScraper/
--rw-rw-rw-   0        0        0    20330 2023-05-04 15:21:46.000000 ReverseTwitterScraper-0.6/ReverseTwitterScraper/Scraper.py
--rw-rw-rw-   0        0        0       37 2023-03-09 02:04:31.000000 ReverseTwitterScraper-0.6/ReverseTwitterScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 20:19:30.382320 ReverseTwitterScraper-0.6/ReverseTwitterScraper.egg-info/
--rw-rw-rw-   0        0        0     7671 2023-05-09 20:19:30.000000 ReverseTwitterScraper-0.6/ReverseTwitterScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-05-09 20:19:30.000000 ReverseTwitterScraper-0.6/ReverseTwitterScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 20:19:30.000000 ReverseTwitterScraper-0.6/ReverseTwitterScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-09 20:19:30.000000 ReverseTwitterScraper-0.6/ReverseTwitterScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-05-09 20:19:30.000000 ReverseTwitterScraper-0.6/ReverseTwitterScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 20:19:30.383320 ReverseTwitterScraper-0.6/setup.cfg
--rw-rw-rw-   0        0        0      815 2023-05-09 20:18:46.000000 ReverseTwitterScraper-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 21:55:56.674830 ReverseTwitterScraper-0.7/
+-rw-rw-rw-   0        0        0     1090 2023-03-08 21:13:40.000000 ReverseTwitterScraper-0.7/LICENSE
+-rw-rw-rw-   0        0        0     7972 2023-05-24 21:55:56.673829 ReverseTwitterScraper-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7157 2023-05-24 21:49:25.000000 ReverseTwitterScraper-0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 21:55:56.650824 ReverseTwitterScraper-0.7/ReverseTwitterScraper/
+-rw-rw-rw-   0        0        0    20277 2023-05-24 21:49:50.000000 ReverseTwitterScraper-0.7/ReverseTwitterScraper/Scraper.py
+-rw-rw-rw-   0        0        0       37 2023-03-09 02:04:31.000000 ReverseTwitterScraper-0.7/ReverseTwitterScraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 21:55:56.672829 ReverseTwitterScraper-0.7/ReverseTwitterScraper.egg-info/
+-rw-rw-rw-   0        0        0     7972 2023-05-24 21:55:56.000000 ReverseTwitterScraper-0.7/ReverseTwitterScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-05-24 21:55:56.000000 ReverseTwitterScraper-0.7/ReverseTwitterScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 21:55:56.000000 ReverseTwitterScraper-0.7/ReverseTwitterScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-24 21:55:56.000000 ReverseTwitterScraper-0.7/ReverseTwitterScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-05-24 21:55:56.000000 ReverseTwitterScraper-0.7/ReverseTwitterScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 21:55:56.674830 ReverseTwitterScraper-0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1161 2023-05-24 21:55:29.000000 ReverseTwitterScraper-0.7/setup.py
```

### Comparing `ReverseTwitterScraper-0.6/LICENSE` & `ReverseTwitterScraper-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ReverseTwitterScraper-0.6/PKG-INFO` & `ReverseTwitterScraper-0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 Metadata-Version: 2.1
 Name: ReverseTwitterScraper
-Version: 0.6
+Version: 0.7
 Summary: A Python package for scraping Twitter data without API. With proxy and account-cookie support
 Home-page: https://github.com/1220moritz/reverse-twitter-scraper
 Author: 1220moritz
+Project-URL: Documentation, https://github.com/1220moritz/reverse-twitter-scraper/blob/main/README.md
+Project-URL: Github, https://github.com/1220moritz/reverse-twitter-scraper
+Project-URL: PyPi, https://pypi.org/project/ReverseTwitterScraper/
+Project-URL: Contact, https://discordapp.com/users/713118695165263923
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -32,26 +36,22 @@
 3. Call any method of the TwitterScraper class.  
 
 Here's an example code:
 ```
 from ReverseTwitterScraper import TwitterScraper
 
 chromedriver_path = "C:/Program Files (x86)/chromedriver.exe"
-cookies = ""
-timeout = 5
+cookies = "" #no account cookies
+cookies = {'Cookie': 'your Cookie', 'X-Csrf-Token': 'your csrf token'} #with account cookie
 proxy_list = []
 
-# single account
-twitter_handle = ["elonmusk"]
-scraper = TwitterScraper(twitter_handle, chromedriver_path, cookies, proxy_list)
-tweets = scraper.getTweetsText()
 
-# multiple accounts
-twitter_handles = ["elonmusk", "POTUS", "latestinspace"]
-scraper = TwitterScraper(twitter_handles, chromedriver_path, cookies, proxy_list)
+twitter_handle = ["elonmusk"]  # single account
+twitter_handles = ["elonmusk", "POTUS", "latestinspace"]  # multiple accounts
+scraper = TwitterScraper(twitter_handle, chromedriver_path, cookies, proxy_list)
 tweets = scraper.getTweetsText()
 
 print(tweets)
 ```
 
 In the above code, we first import the TwitterScraper class from the package. Then, we create an object of the TwitterScraper class with the required parameters.
 Finally, we call the getTweetsText() method to get the tweets of the specified Twitter account.
```

### Comparing `ReverseTwitterScraper-0.6/README.md` & `ReverseTwitterScraper-0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,26 +19,22 @@
 3. Call any method of the TwitterScraper class.  
 
 Here's an example code:
 ```
 from ReverseTwitterScraper import TwitterScraper
 
 chromedriver_path = "C:/Program Files (x86)/chromedriver.exe"
-cookies = ""
-timeout = 5
+cookies = "" #no account cookies
+cookies = {'Cookie': 'your Cookie', 'X-Csrf-Token': 'your csrf token'} #with account cookie
 proxy_list = []
 
-# single account
-twitter_handle = ["elonmusk"]
-scraper = TwitterScraper(twitter_handle, chromedriver_path, cookies, proxy_list)
-tweets = scraper.getTweetsText()
 
-# multiple accounts
-twitter_handles = ["elonmusk", "POTUS", "latestinspace"]
-scraper = TwitterScraper(twitter_handles, chromedriver_path, cookies, proxy_list)
+twitter_handle = ["elonmusk"]  # single account
+twitter_handles = ["elonmusk", "POTUS", "latestinspace"]  # multiple accounts
+scraper = TwitterScraper(twitter_handle, chromedriver_path, cookies, proxy_list)
 tweets = scraper.getTweetsText()
 
 print(tweets)
 ```
 
 In the above code, we first import the TwitterScraper class from the package. Then, we create an object of the TwitterScraper class with the required parameters.
 Finally, we call the getTweetsText() method to get the tweets of the specified Twitter account.
@@ -134,8 +130,8 @@
 
 ### filterDescription(singleUserPlain)
         returns the description of an account
         :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
 
 ### getUserSpecificData(singleUserPlain)
         returns all (unfiltered) data about an account
-        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
+        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
```

### Comparing `ReverseTwitterScraper-0.6/ReverseTwitterScraper/Scraper.py` & `ReverseTwitterScraper-0.7/ReverseTwitterScraper/Scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 import traceback
-
+import json
 import asyncio
 import httpx
 from seleniumwire import webdriver
 from selenium.webdriver.chrome.options import Options
 
 
 class TwitterScraper:
@@ -24,15 +24,17 @@
         else:
             exit(
                 f"Twitter | Type: {type(cookies)} is currently unsupported for cookies, if you'd like to see it added please open an issue on Github")
 
         return cookies
 
     def changeProxy(self):
-        if type(self.proxies) is list and self.__proxyCounter < len(self.proxies) - 1:    #change to next proxy in list
+        if len(self.proxies) == 0:
+            return None
+        elif type(self.proxies) is list and self.__proxyCounter < len(self.proxies) - 1:    #change to next proxy in list
             return self.proxies[self.__proxyCounter]
         elif type(self.proxies) is list and self.__proxyCounter >= len(self.proxies) - 1: # restart with first proxy in list
             self.__proxyCounter = 0
             return self.proxies[self.__proxyCounter]
         else:
             return None
         
@@ -51,15 +53,15 @@
 
         # format proxy
         self.__proxyCounter = 0
         if proxyList != "" and proxyList != None:
             self.proxies = []
             for proxy in proxyList:
                 __split = str(proxy).replace("\n", "").split(":")
-                fProxy = {'https': f'http://{__split[2]}:{__split[3]}@{__split[0]}:{__split[1]}'}
+                fProxy = {f'all://': f'https://{__split[2]}:{__split[3]}@{__split[0]}:{__split[1]}'}
                 self.proxies.append(fProxy)
         else:
             self.proxies = None
             
             
         # convert handle to id [{"handle": handle, "id": id]}]
         if isinstance(twitterHandle, list):
@@ -87,16 +89,17 @@
                 #print(traceback.format_exc())
                 retries += 1
                 self.__proxyCounter += 1
             
         retries = 0
         while retries < 5:
             try:
-                self.__openingResp = httpx.get(url=self.__reqUrl, headers=self.__headers, cookies=self.__cookies).json()
-                self.__userResp = self.__openingResp['data']['user']['result']['timeline_v2']['timeline']['instructions'][1]['entries'][0]['content']['itemContent']['tweet_results']['result']['core']['user_results']['result']
+                resp =  httpx.get(url=self.__reqUrl, headers=self.__headers, cookies=self.__cookies)
+                if resp.status_code == 200:
+                    print("got valid meta-information")
                 break
             except:
                 #print(traceback.format_exc())
                 print("failed openingResp. Trying again with new proxy")
                 retries += 1
                 self.__proxyCounter += 1
                 self.getTwitterGuestData(cookies=self.__accCookies)
@@ -130,16 +133,15 @@
         # get driver
         options = Options()
         options.add_argument("--headless")
         driver = webdriver.Chrome(self.__chromedriverPath, options=options) #headless
         #driver = webdriver.Chrome(self.__chromedriverPath) #window
     
     
-        driver.get(f"https://twitter.com/{self.__twitterHandle[0]}")
-        #time.sleep(self.__timeout)  # sleep to let the twitter page load
+        driver.get(f"https://twitter.com/{self.__twitterHandle[0]}") 
         
         
         headersDict = {}
         for headerReq in driver.requests:
             url = headerReq.url
             if "UserTweets" in url and "cursor" not in url:
                 self.__reqUrl = url
@@ -151,27 +153,26 @@
         self.__headers = {
             'authorization': headersDict['authorization'],
             'cookie': headersDict['cookie'],
             'user-agent': headersDict['user-agent'],
             'x-csrf-token': headersDict['x-csrf-token'],
             'x-guest-token': headersDict['x-guest-token']
         }
-
         
         # check for cookies
-        if cookies != "":
-            self.__cookies = self.cookieDict(cookies)
+        if type(cookies) is dict and 'Cookie' in cookies and 'X-Csrf-Token' in cookies:
+            self.__cookies = self.cookieDict(cookies['Cookie'])
+            self.__headers['cookie'] = cookies['Cookie']
+            self.__headers['x-csrf-token'] = cookies['X-Csrf-Token']
         else:
             self.__cookies = self.cookieDict(headersDict['cookie'])
-        print("Done!")
+
 
     def __resetData(self):
         self.__headers = None
-        self.__openingResp = None
-        self.__userResp = None
         self.__reqUrl = None
         self.__cookies = None
   
     
     
     
     
@@ -300,18 +301,15 @@
                         continue
             accountTweets.append({
                 "handle": handle['handle'],
                 "id": handle['id'],
                 "tweets": tweets
             })
         return accountTweets
-  
-    
-    
-    
+
     
     # filter methodes
     ## filter Tweet data
     def filterRetweetInfo(self, singlePlainTweet, getRetweetInfo=False):
         """
         checks if the tweet is a retweet (returns True, False or the TweetInfo (if you use getRetweetInfo=True))
```

### Comparing `ReverseTwitterScraper-0.6/ReverseTwitterScraper.egg-info/PKG-INFO` & `ReverseTwitterScraper-0.7/ReverseTwitterScraper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 Metadata-Version: 2.1
 Name: ReverseTwitterScraper
-Version: 0.6
+Version: 0.7
 Summary: A Python package for scraping Twitter data without API. With proxy and account-cookie support
 Home-page: https://github.com/1220moritz/reverse-twitter-scraper
 Author: 1220moritz
+Project-URL: Documentation, https://github.com/1220moritz/reverse-twitter-scraper/blob/main/README.md
+Project-URL: Github, https://github.com/1220moritz/reverse-twitter-scraper
+Project-URL: PyPi, https://pypi.org/project/ReverseTwitterScraper/
+Project-URL: Contact, https://discordapp.com/users/713118695165263923
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -32,26 +36,22 @@
 3. Call any method of the TwitterScraper class.  
 
 Here's an example code:
 ```
 from ReverseTwitterScraper import TwitterScraper
 
 chromedriver_path = "C:/Program Files (x86)/chromedriver.exe"
-cookies = ""
-timeout = 5
+cookies = "" #no account cookies
+cookies = {'Cookie': 'your Cookie', 'X-Csrf-Token': 'your csrf token'} #with account cookie
 proxy_list = []
 
-# single account
-twitter_handle = ["elonmusk"]
-scraper = TwitterScraper(twitter_handle, chromedriver_path, cookies, proxy_list)
-tweets = scraper.getTweetsText()
 
-# multiple accounts
-twitter_handles = ["elonmusk", "POTUS", "latestinspace"]
-scraper = TwitterScraper(twitter_handles, chromedriver_path, cookies, proxy_list)
+twitter_handle = ["elonmusk"]  # single account
+twitter_handles = ["elonmusk", "POTUS", "latestinspace"]  # multiple accounts
+scraper = TwitterScraper(twitter_handle, chromedriver_path, cookies, proxy_list)
 tweets = scraper.getTweetsText()
 
 print(tweets)
 ```
 
 In the above code, we first import the TwitterScraper class from the package. Then, we create an object of the TwitterScraper class with the required parameters.
 Finally, we call the getTweetsText() method to get the tweets of the specified Twitter account.
```

### Comparing `ReverseTwitterScraper-0.6/setup.py` & `ReverseTwitterScraper-0.7/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="ReverseTwitterScraper",
-    version="0.6",
+    version="0.7",
     author="1220moritz",
     description="A Python package for scraping Twitter data without API. With proxy and account-cookie support",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/1220moritz/reverse-twitter-scraper",
       install_requires=[
           'selenium-wire',
@@ -19,8 +19,14 @@
       ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
+    project_urls={
+        "Documentation": "https://github.com/1220moritz/reverse-twitter-scraper/blob/main/README.md",
+        "Github": "https://github.com/1220moritz/reverse-twitter-scraper",
+        "PyPi": "https://pypi.org/project/ReverseTwitterScraper/",
+        "Contact": "https://discordapp.com/users/713118695165263923",
+    },
 )
```

