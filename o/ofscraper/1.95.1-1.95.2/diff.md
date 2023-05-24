# Comparing `tmp/ofscraper-1.95.1.tar.gz` & `tmp/ofscraper-1.95.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-1.95.1.tar", max compression
+gzip compressed data, was "ofscraper-1.95.2.tar", max compression
```

## Comparing `ofscraper-1.95.1.tar` & `ofscraper-1.95.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1067 2023-05-20 19:39:41.219814 ofscraper-1.95.1/LICENSE
--rw-r--r--   0        0        0     5177 2023-05-20 19:39:41.219814 ofscraper-1.95.1/README.md
--rw-r--r--   0        0        0      607 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/__init__.py
--rw-r--r--   0        0        0      998 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/__version__.py
--rw-r--r--   0        0        0        1 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/api/__init__.py
--rw-r--r--   0        0        0     1986 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/api/highlights.py
--rw-r--r--   0        0        0      838 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/api/init.py
--rw-r--r--   0        0        0     2243 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/api/me.py
--rw-r--r--   0        0        0     4359 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/api/messages.py
--rw-r--r--   0        0        0     1884 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/api/paid.py
--rw-r--r--   0        0        0     9170 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/api/posts.py
--rw-r--r--   0        0        0     2841 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/api/profile.py
--rw-r--r--   0        0        0     1867 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     6457 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/api/timeline.py
--rw-r--r--   0        0        0     4999 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/db/__init__.py
--rw-r--r--   0        0        0     6759 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3199 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     3611 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/interaction/like.py
--rw-r--r--   0        0        0     5477 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/prompts/prompt_functions.py
--rw-r--r--   0        0        0      359 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0    20976 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/prompts/prompts.py
--rwxr-xr-x   0        0        0    21369 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/scraper.py
--rw-r--r--   0        0        0        1 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0     3938 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/args.py
--rw-r--r--   0        0        0     8994 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/auth.py
--rw-r--r--   0        0        0    10859 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/config.py
--rw-r--r--   0        0        0      993 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    17597 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     2938 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     1926 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/filters.py
--rw-r--r--   0        0        0     4540 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/logger.py
--rw-r--r--   0        0        0     5377 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     3008 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      779 2023-05-20 19:39:42.111822 ofscraper-1.95.1/ofscraper/utils/separate.py
--rw-r--r--   0        0        0     1545 2023-05-20 19:40:15.672136 ofscraper-1.95.1/pyproject.toml
--rw-r--r--   0        0        0     6618 1970-01-01 00:00:00.000000 ofscraper-1.95.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-24 13:48:31.755754 ofscraper-1.95.2/LICENSE
+-rw-r--r--   0        0        0     5192 2023-05-24 13:48:31.755754 ofscraper-1.95.2/README.md
+-rw-r--r--   0        0        0      607 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/__init__.py
+-rw-r--r--   0        0        0      999 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/__version__.py
+-rw-r--r--   0        0        0        1 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/api/__init__.py
+-rw-r--r--   0        0        0     1986 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0      838 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/api/init.py
+-rw-r--r--   0        0        0     2243 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/api/me.py
+-rw-r--r--   0        0        0     4359 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/api/messages.py
+-rw-r--r--   0        0        0     1884 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     9170 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/api/posts.py
+-rw-r--r--   0        0        0     2841 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     1867 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     6457 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0     4999 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0     6759 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3199 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     3611 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0     5477 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/prompts/prompt_functions.py
+-rw-r--r--   0        0        0      359 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0    20976 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/prompts/prompts.py
+-rwxr-xr-x   0        0        0    21369 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/scraper.py
+-rw-r--r--   0        0        0        1 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0     3938 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/args.py
+-rw-r--r--   0        0        0     8996 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0    10859 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      993 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    17597 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     2938 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     1926 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0     4540 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0     5377 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     3008 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      779 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0     1546 2023-05-24 13:49:24.333831 ofscraper-1.95.2/pyproject.toml
+-rw-r--r--   0        0        0     6634 1970-01-01 00:00:00.000000 ofscraper-1.95.2/PKG-INFO
```

### Comparing `ofscraper-1.95.1/LICENSE` & `ofscraper-1.95.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/README.md` & `ofscraper-1.95.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 A fork of onlyfans-scraper. It has been optimized to make it more feature complete with digitalcriminal's onlyfans script.
 A matter of fact with the right settings transitioning between the two scripts should be a easy enough process
 
 In addition there are numerous filtering features to control exactly which type of content you want to scrape.
-https://github.com/datawhores/ofscraper/blob/main/CHANGES.md
+https://github.com/datawhores/OF-Scraper/blob/main/CHANGES.md
 
 <h3>DISCLAIMERS:</h3>
 <ol>
     <li>
         This tool is not affiliated, associated, or partnered with OnlyFans in any way. We are not authorized, endorsed, or sponsored by OnlyFans. All OnlyFans trademarks remain the property of Fenix International Limited.
     </li>
     <li>
@@ -32,15 +32,15 @@
 ## stable
 ```
 pip install ofscraper
 ```
 or 
 ## development
 ```
-pip install git+https://github.com/datawhores/ofscraper.git 
+pip install git+https://github.com/datawhores/OF-Scraper.git 
 ```
 or 
 ## specific version
 ```
 pip install ofscraper==x
 ```
 where x is the vesion you want to install
@@ -48,29 +48,29 @@
 
 #  macOS/Linux
 ```
 pip3 install ofscraper
 ```
 or
 ```
-pip3 install git+https://github.com/datawhores/ofscraper.git 
+pip3 install git+https://github.com/datawhores/OF-Scraper.git 
 ```
 
 or 
 ## specific version
 ```
 pip install ofscraper==x
 ```
 where x is the vesion you want to install
 
 ## Authentication
 
 You'll need to retrive your auth information 
     
-https://github.com/datawhores/ofscraper/wiki/Auth
+https://github.com/datawhores/OF-Scraper/wiki/Auth
 
 
 
 # Usage
 
 Whenever you want to run the program, all you need to do is type `ofscraper` in your terminal:
 
@@ -91,34 +91,34 @@
 
 ![image](https://user-images.githubusercontent.com/67020411/230735256-2d8aa788-53dc-49ee-ada8-5ddf5546851c.png)
 
 ## Selecting specific users
 
 The fuzzy search system can be a little confusing see
     
-https://github.com/datawhores/ofscraper/wiki/Fuzzy-Search 
+https://github.com/datawhores/OF-Scraper/wiki/Fuzzy-Search 
     
 ## Other menu options    
   
- See: https://github.com/datawhores/ofscraper/wiki/Menu-Options 
+ See: https://github.com/datawhores/OF-Scraper/wiki/Menu-Options 
  
  # commandline
  While the menu is easy to use, and convient. You may want more automation.
  
  The best way to do this is through the commandline system. This will allow you to skip the menu, and for example scrape a provided list of accounts
  
-  https://github.com/datawhores/ofscraper/wiki/command-line-args
+  https://github.com/datawhores/OF-Scraper/wiki/command-line-args
 
 # Docker Support
-https://github.com/datawhores/ofscraper/pkgs/container/ofscraper
+https://github.com/datawhores/OF-Scraper/pkgs/container/ofscraper
  
  # Customazation
     
-https://github.com/datawhores/ofscraper/wiki/Customizing-save-path
-https://github.com/datawhores/ofscraper/wiki/Config-Options
+https://github.com/datawhores/OF-Scraper/wiki/Customizing-save-path
+https://github.com/datawhores/OF-Scraper/wiki/Config-Options
 
   
 # Issues
 Open a issue in this repo, or you can mention your issue in the discord
 
 https://discord.gg/wN7uxEVHRK
     
@@ -149,17 +149,17 @@
 
 You will need to change the settings so that the metadata option is compatible with your current folders
 Additionally you might want to set the save_path, dir_path, and filename so they output similar outputs
 
 The metadata path from digitalcriminal's script is used for duplicate check so as long as your set the right path.
 Files won't download a second time
 
-https://github.com/datawhores/ofscraper/wiki/Migrating-from-DC-script
-https://github.com/datawhores/ofscraper/wiki/Config-Options
-https://github.com/datawhores/ofscraper/wiki/Customizing-save-path
+https://github.com/datawhores/OF-Scraper/wiki/Migrating-from-DC-script
+https://github.com/datawhores/OF-Scraper/wiki/Config-Options
+https://github.com/datawhores/OF-Scraper/wiki/Customizing-save-path
 
 Ask in the discord or open an issue if you need help with what to change to accomplish this
 
 
 
 # Discord
 
@@ -169,15 +169,15 @@
 buymeacoffee.com/datawhores
     
 BTC: bc1qcnnetrgmtr86rmqvukl2e24f5upghpcsqqsy87
     
 ETH: 0x1d427a6E336edF6D95e589C16cb740A1372F6609
 
 
-[![codecov](https://codecov.io/github/datawhores/ofscraper/branch/main/graph/badge.svg?token=U1F1PQ7LGM)](https://codecov.io/github/datawhores/ofscraper)
+[![codecov](https://codecov.io/github/datawhores/OF-Scraper/branch/main/graph/badge.svg?token=U1F1PQ7LGM)](https://codecov.io/github/datawhores/OF-Scraper)
```

### Comparing `ofscraper-1.95.1/ofscraper/__init__.py` & `ofscraper-1.95.2/ofscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/__version__.py` & `ofscraper-1.95.2/ofscraper/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
                  \/     \/           \/            \/       
 """
 
 __title__ = 'ofscraper'
 __author__ = 'datawhores'
 __author_email__ = 'datawhores@riseup.net'
 __description__ = 'A command-line program to quickly download,like or unlike posts, and more'
-__url__ = 'https://github.com/datawhores/ofscraper'
+__url__ = 'https://github.com/datawhores/OF-Scraper'
 __license__ = 'GNU General Public License v3 or later (GPLv3+)'
 __copyright__ = 'Copyright 2023'
 
 try:
       from dunamai import Version,Pattern
       __version__ = Version.from_git(pattern=Pattern.DefaultUnprefixed).serialize(format="{base}+{branch}.{commit}",metadata=False)
 except:
```

### Comparing `ofscraper-1.95.1/ofscraper/api/highlights.py` & `ofscraper-1.95.2/ofscraper/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/api/init.py` & `ofscraper-1.95.2/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/api/me.py` & `ofscraper-1.95.2/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/api/messages.py` & `ofscraper-1.95.2/ofscraper/api/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/api/paid.py` & `ofscraper-1.95.2/ofscraper/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/api/posts.py` & `ofscraper-1.95.2/ofscraper/api/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/api/profile.py` & `ofscraper-1.95.2/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/api/subscriptions.py` & `ofscraper-1.95.2/ofscraper/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/api/timeline.py` & `ofscraper-1.95.2/ofscraper/api/timeline.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/constants.py` & `ofscraper-1.95.2/ofscraper/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/db/operations.py` & `ofscraper-1.95.2/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/db/queries.py` & `ofscraper-1.95.2/ofscraper/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/interaction/like.py` & `ofscraper-1.95.2/ofscraper/interaction/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/prompts/prompt_functions.py` & `ofscraper-1.95.2/ofscraper/prompts/prompt_functions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/prompts/prompts.py` & `ofscraper-1.95.2/ofscraper/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/scraper.py` & `ofscraper-1.95.2/ofscraper/scraper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/utils/args.py` & `ofscraper-1.95.2/ofscraper/utils/args.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/utils/auth.py` & `ofscraper-1.95.2/ofscraper/utils/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
     auth= auth or defaultAuth
     if  browserSelect!="Enter Each Field Manually" and browserSelect!="Paste From Cookie Helper":
         temp=requests.utils.dict_from_cookiejar(getattr(browser_cookie3, browserSelect.lower())(domain_name="onlyfans"))
         auth=auth or  defaultAuth
         for key in ["sess","auth_id","auth_uid_"]:
             auth["auth"][key]=temp.get(key,"")
-        console.print("You'll need to go to onlyfans.com and retrive header information\nGo to https://github.com/datawhores/ofscraper and find the section named 'Getting Your Auth Info'\nCookie information has been retived automatically\nSo You only need to retrive the x-bc header and the user-agent",style="yellow")
+        console.print("You'll need to go to onlyfans.com and retrive header information\nGo to https://github.com/datawhores/OF-Scraper and find the section named 'Getting Your Auth Info'\nCookie information has been retived automatically\nSo You only need to retrive the x-bc header and the user-agent",style="yellow")
         if not auth["auth"].get("x-bc"):
             auth["auth"]["x-bc"]=xbc_prompt()
         auth["auth"]["user_agent"]= user_agent_prompt(auth["auth"].get("user_agent") or "")
 
 
  
     elif browserSelect=="Paste From Cookie Helper":
@@ -136,15 +136,15 @@
                 auth["auth"]["sess"]=ele.replace("sess=","")
             elif ele.find("auth_uid")!=-1:
                 auth["auth"]["auth_uid_"]=ele.replace("auth_uid_","").replace("=","")
            
 
 
     else:
-        console.print("You'll need to go to onlyfans.com and retrive header information\nGo to https://github.com/datawhores/ofscraper and find the section named 'Getting Your Auth Info'\nYou only need to retrive the x-bc header,the user-agent, and cookie information",style="yellow")
+        console.print("You'll need to go to onlyfans.com and retrive header information\nGo to https://github.com/datawhores/OF-Scraper and find the section named 'Getting Your Auth Info'\nYou only need to retrive the x-bc header,the user-agent, and cookie information",style="yellow")
         auth['auth'].update(auth_prompt(auth['auth']))
     
     console.print(f"{auth}\nWriting to {path / authFile}",style="yellow")
     with open(path / authFile, 'w') as f:
         f.write(json.dumps(auth, indent=4))
```

### Comparing `ofscraper-1.95.1/ofscraper/utils/config.py` & `ofscraper-1.95.2/ofscraper/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/utils/dates.py` & `ofscraper-1.95.2/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/utils/download.py` & `ofscraper-1.95.2/ofscraper/utils/download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/utils/encoding.py` & `ofscraper-1.95.2/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/utils/exit.py` & `ofscraper-1.95.2/ofscraper/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/utils/filters.py` & `ofscraper-1.95.2/ofscraper/utils/filters.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/utils/logger.py` & `ofscraper-1.95.2/ofscraper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/utils/paths.py` & `ofscraper-1.95.2/ofscraper/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/utils/profiles.py` & `ofscraper-1.95.2/ofscraper/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/ofscraper/utils/separate.py` & `ofscraper-1.95.2/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.1/pyproject.toml` & `ofscraper-1.95.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "1.95.1"
+version = "1.95.2"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 packages = [{include = "ofscraper"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
@@ -51,15 +51,15 @@
 [tool.poetry.scripts]
 ofscraper = "ofscraper.scraper:main"
 
 [project.scripts]
 ofscraper = "ofscraper.scraper:main"
 
 [tool.poetry.urls]
-"Homepage" = "https://github.com/datawhores/ofscraper"
+"Homepage" = "https://github.com/datawhores/OF-Scraper"
 
 # pyproject.toml
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-ra -q"
 testpaths = [
     "tests",
```

### Comparing `ofscraper-1.95.1/PKG-INFO` & `ofscraper-1.95.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 1.95.1
+Version: 1.95.2
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -27,22 +27,22 @@
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: schedule (>=1.1.0,<2.0.0)
 Requires-Dist: setuptools (>=67.6.0,<68.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: win32-setctime (>=1.1.0,<2.0.0)
 Requires-Dist: xxhash (>=3.2.0,<4.0.0)
-Project-URL: Homepage, https://github.com/datawhores/ofscraper
+Project-URL: Homepage, https://github.com/datawhores/OF-Scraper
 Description-Content-Type: text/markdown
 
 A fork of onlyfans-scraper. It has been optimized to make it more feature complete with digitalcriminal's onlyfans script.
 A matter of fact with the right settings transitioning between the two scripts should be a easy enough process
 
 In addition there are numerous filtering features to control exactly which type of content you want to scrape.
-https://github.com/datawhores/ofscraper/blob/main/CHANGES.md
+https://github.com/datawhores/OF-Scraper/blob/main/CHANGES.md
 
 <h3>DISCLAIMERS:</h3>
 <ol>
     <li>
         This tool is not affiliated, associated, or partnered with OnlyFans in any way. We are not authorized, endorsed, or sponsored by OnlyFans. All OnlyFans trademarks remain the property of Fenix International Limited.
     </li>
     <li>
@@ -68,15 +68,15 @@
 ## stable
 ```
 pip install ofscraper
 ```
 or 
 ## development
 ```
-pip install git+https://github.com/datawhores/ofscraper.git 
+pip install git+https://github.com/datawhores/OF-Scraper.git 
 ```
 or 
 ## specific version
 ```
 pip install ofscraper==x
 ```
 where x is the vesion you want to install
@@ -84,29 +84,29 @@
 
 #  macOS/Linux
 ```
 pip3 install ofscraper
 ```
 or
 ```
-pip3 install git+https://github.com/datawhores/ofscraper.git 
+pip3 install git+https://github.com/datawhores/OF-Scraper.git 
 ```
 
 or 
 ## specific version
 ```
 pip install ofscraper==x
 ```
 where x is the vesion you want to install
 
 ## Authentication
 
 You'll need to retrive your auth information 
     
-https://github.com/datawhores/ofscraper/wiki/Auth
+https://github.com/datawhores/OF-Scraper/wiki/Auth
 
 
 
 # Usage
 
 Whenever you want to run the program, all you need to do is type `ofscraper` in your terminal:
 
@@ -127,34 +127,34 @@
 
 ![image](https://user-images.githubusercontent.com/67020411/230735256-2d8aa788-53dc-49ee-ada8-5ddf5546851c.png)
 
 ## Selecting specific users
 
 The fuzzy search system can be a little confusing see
     
-https://github.com/datawhores/ofscraper/wiki/Fuzzy-Search 
+https://github.com/datawhores/OF-Scraper/wiki/Fuzzy-Search 
     
 ## Other menu options    
   
- See: https://github.com/datawhores/ofscraper/wiki/Menu-Options 
+ See: https://github.com/datawhores/OF-Scraper/wiki/Menu-Options 
  
  # commandline
  While the menu is easy to use, and convient. You may want more automation.
  
  The best way to do this is through the commandline system. This will allow you to skip the menu, and for example scrape a provided list of accounts
  
-  https://github.com/datawhores/ofscraper/wiki/command-line-args
+  https://github.com/datawhores/OF-Scraper/wiki/command-line-args
 
 # Docker Support
-https://github.com/datawhores/ofscraper/pkgs/container/ofscraper
+https://github.com/datawhores/OF-Scraper/pkgs/container/ofscraper
  
  # Customazation
     
-https://github.com/datawhores/ofscraper/wiki/Customizing-save-path
-https://github.com/datawhores/ofscraper/wiki/Config-Options
+https://github.com/datawhores/OF-Scraper/wiki/Customizing-save-path
+https://github.com/datawhores/OF-Scraper/wiki/Config-Options
 
   
 # Issues
 Open a issue in this repo, or you can mention your issue in the discord
 
 https://discord.gg/wN7uxEVHRK
     
@@ -185,17 +185,17 @@
 
 You will need to change the settings so that the metadata option is compatible with your current folders
 Additionally you might want to set the save_path, dir_path, and filename so they output similar outputs
 
 The metadata path from digitalcriminal's script is used for duplicate check so as long as your set the right path.
 Files won't download a second time
 
-https://github.com/datawhores/ofscraper/wiki/Migrating-from-DC-script
-https://github.com/datawhores/ofscraper/wiki/Config-Options
-https://github.com/datawhores/ofscraper/wiki/Customizing-save-path
+https://github.com/datawhores/OF-Scraper/wiki/Migrating-from-DC-script
+https://github.com/datawhores/OF-Scraper/wiki/Config-Options
+https://github.com/datawhores/OF-Scraper/wiki/Customizing-save-path
 
 Ask in the discord or open an issue if you need help with what to change to accomplish this
 
 
 
 # Discord
 
@@ -205,15 +205,15 @@
 buymeacoffee.com/datawhores
     
 BTC: bc1qcnnetrgmtr86rmqvukl2e24f5upghpcsqqsy87
     
 ETH: 0x1d427a6E336edF6D95e589C16cb740A1372F6609
 
 
-[![codecov](https://codecov.io/github/datawhores/ofscraper/branch/main/graph/badge.svg?token=U1F1PQ7LGM)](https://codecov.io/github/datawhores/ofscraper)
+[![codecov](https://codecov.io/github/datawhores/OF-Scraper/branch/main/graph/badge.svg?token=U1F1PQ7LGM)](https://codecov.io/github/datawhores/OF-Scraper)
```

