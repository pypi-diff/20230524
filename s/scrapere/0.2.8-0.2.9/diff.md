# Comparing `tmp/scrapere-0.2.8.tar.gz` & `tmp/scrapere-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapere-0.2.8.tar", last modified: Tue May 16 12:19:15 2023, max compression
+gzip compressed data, was "scrapere-0.2.9.tar", last modified: Wed May 24 15:48:02 2023, max compression
```

## Comparing `scrapere-0.2.8.tar` & `scrapere-0.2.9.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 12:19:15.551021 scrapere-0.2.8/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)     1035 2023-05-16 12:19:15.551021 scrapere-0.2.8/PKG-INFO
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      799 2023-05-16 12:19:10.000000 scrapere-0.2.8/README.md
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 12:19:15.547021 scrapere-0.2.8/scrapere/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       22 2023-05-16 10:14:19.000000 scrapere-0.2.8/scrapere/__init__.py
--rw-rw-r--   0 vpere     (1000) vpere     (1000)     5435 2023-05-16 12:18:50.000000 scrapere-0.2.8/scrapere/toolbox.py
--rw-rw-r--   0 vpere     (1000) vpere     (1000)  2656639 2023-05-16 10:19:54.000000 scrapere-0.2.8/scrapere/user_agents.txt
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 12:19:15.551021 scrapere-0.2.8/scrapere.egg-info/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)     1035 2023-05-16 12:19:15.000000 scrapere-0.2.8/scrapere.egg-info/PKG-INFO
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      243 2023-05-16 12:19:15.000000 scrapere-0.2.8/scrapere.egg-info/SOURCES.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)        1 2023-05-16 12:19:15.000000 scrapere-0.2.8/scrapere.egg-info/dependency_links.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       39 2023-05-16 12:19:15.000000 scrapere-0.2.8/scrapere.egg-info/requires.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)        9 2023-05-16 12:19:15.000000 scrapere-0.2.8/scrapere.egg-info/top_level.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       38 2023-05-16 12:19:15.551021 scrapere-0.2.8/setup.cfg
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      727 2023-05-16 12:19:10.000000 scrapere-0.2.8/setup.py
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-24 15:48:02.629835 scrapere-0.2.9/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)     1086 2023-05-24 15:48:02.629835 scrapere-0.2.9/PKG-INFO
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      850 2023-05-24 15:47:56.000000 scrapere-0.2.9/README.md
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-24 15:48:02.613835 scrapere-0.2.9/scrapere/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       22 2023-05-16 10:14:19.000000 scrapere-0.2.9/scrapere/__init__.py
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)    11696 2023-05-24 15:46:47.000000 scrapere-0.2.9/scrapere/browser_agents.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)     5874 2023-05-24 15:46:47.000000 scrapere-0.2.9/scrapere/toolbox.py
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)  2656639 2023-05-16 10:19:54.000000 scrapere-0.2.9/scrapere/user_agents.txt
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-24 15:48:02.625836 scrapere-0.2.9/scrapere.egg-info/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)     1086 2023-05-24 15:48:02.000000 scrapere-0.2.9/scrapere.egg-info/PKG-INFO
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      271 2023-05-24 15:48:02.000000 scrapere-0.2.9/scrapere.egg-info/SOURCES.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)        1 2023-05-24 15:48:02.000000 scrapere-0.2.9/scrapere.egg-info/dependency_links.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       39 2023-05-24 15:48:02.000000 scrapere-0.2.9/scrapere.egg-info/requires.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)        9 2023-05-24 15:48:02.000000 scrapere-0.2.9/scrapere.egg-info/top_level.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       38 2023-05-24 15:48:02.629835 scrapere-0.2.9/setup.cfg
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      727 2023-05-24 15:47:53.000000 scrapere-0.2.9/setup.py
```

### Comparing `scrapere-0.2.8/PKG-INFO` & `scrapere-0.2.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: scrapere
-Version: 0.2.8
+Version: 0.2.9
 Summary: Small set of my web scraping python tools
 Home-page: https://github.com/vPere/scrapere
 Author: vPere
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Scraping libary
 
 This is a simple toolbox for scraping info from websites which includes methods for generating headers with a random user agent picked from a list of more than 24k user agents, a method for waiting a random time between 1 and 3 seconds, a progress bar for it to look cool ;) and a couple of methods that will help you retreive email addresses and spanish phone numbers from a given url.
 
 As this package may be useful for a bunch of legitimate and non-legitimate use cases, I'm not responsible of whatever you do with it.
 
-## Version 0.2.8 features:
+## Version 0.2.9 features:
  - Improves the email regex.
+ - Adds a method to get random browser user agents
 
-## Version 0.2.8 issues:
+## Version 0.2.9 issues:
 - There are no tests...
 - scrap_phones() only works for spanish phone numbers
 
 As this is my first python package, I might not mantain it, so better try finding another one...
```

### Comparing `scrapere-0.2.8/README.md` & `scrapere-0.2.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Scraping libary
 
 This is a simple toolbox for scraping info from websites which includes methods for generating headers with a random user agent picked from a list of more than 24k user agents, a method for waiting a random time between 1 and 3 seconds, a progress bar for it to look cool ;) and a couple of methods that will help you retreive email addresses and spanish phone numbers from a given url.
 
 As this package may be useful for a bunch of legitimate and non-legitimate use cases, I'm not responsible of whatever you do with it.
 
-## Version 0.2.8 features:
+## Version 0.2.9 features:
  - Improves the email regex.
+ - Adds a method to get random browser user agents
 
-## Version 0.2.8 issues:
+## Version 0.2.9 issues:
 - There are no tests...
 - scrap_phones() only works for spanish phone numbers
 
 As this is my first python package, I might not mantain it, so better try finding another one...
```

### Comparing `scrapere-0.2.8/scrapere/toolbox.py` & `scrapere-0.2.9/scrapere/toolbox.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,36 +20,50 @@
     with open(csv_file) as fp:
         total = 0
         for _ in fp:
             total += 1
     return total
 
 
-def get_user_agent_list():
+def get_crawler_user_agent_list():
     user_agent_list = []
     file_path = pkg_resources.resource_filename(__name__, 'user_agents.txt')
     with open(file_path, 'r') as f:
         for line in f:
             user_agent_list.append(line.strip())
     return user_agent_list
 
 
-def get_random_user_agent():
-    user_agent_list = get_user_agent_list()
+def get_random_crawler_user_agent():
+    user_agent_list = get_crawler_user_agent_list()
     return user_agent_list[0]
 
 
+def get_browser_user_agent_list():
+    user_agent_list = []
+    file_path = pkg_resources.resource_filename(__name__, 'browser_user_agents.txt')
+    with open(file_path, 'r') as f:
+        for line in f:
+            user_agent_list.append(line.strip())
+    return user_agent_list
+
+
+def get_random_user_agent():
+    user_agent_list = get_browser_user_agent_list()
+    return random.choice(user_agent_list)
+
+
 def generate_header():
     headers = {
         'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9',
         'Accept-Encoding': 'gzip, deflate',
         'Accept-Language': 'en-GB,en-US;q=0.9,en;q=0.8',
         'Dnt': '1',
         'Upgrade-Insecure-Requests': '1',
-        'User-Agent': get_random_user_agent(),
+        'User-Agent': get_random_crawler_user_agent(),
         'X-Amzn-Trace-Id': 'Root=1-5ee7bae0-82260c065baf5ad7f0b3a3e3'
     }
     header = {'headers': headers}
     return header
 
 
 def wait_random_time():
```

### Comparing `scrapere-0.2.8/scrapere/user_agents.txt` & `scrapere-0.2.9/scrapere/user_agents.txt`

 * *Files identical despite different names*

### Comparing `scrapere-0.2.8/scrapere.egg-info/PKG-INFO` & `scrapere-0.2.9/scrapere.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: scrapere
-Version: 0.2.8
+Version: 0.2.9
 Summary: Small set of my web scraping python tools
 Home-page: https://github.com/vPere/scrapere
 Author: vPere
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Scraping libary
 
 This is a simple toolbox for scraping info from websites which includes methods for generating headers with a random user agent picked from a list of more than 24k user agents, a method for waiting a random time between 1 and 3 seconds, a progress bar for it to look cool ;) and a couple of methods that will help you retreive email addresses and spanish phone numbers from a given url.
 
 As this package may be useful for a bunch of legitimate and non-legitimate use cases, I'm not responsible of whatever you do with it.
 
-## Version 0.2.8 features:
+## Version 0.2.9 features:
  - Improves the email regex.
+ - Adds a method to get random browser user agents
 
-## Version 0.2.8 issues:
+## Version 0.2.9 issues:
 - There are no tests...
 - scrap_phones() only works for spanish phone numbers
 
 As this is my first python package, I might not mantain it, so better try finding another one...
```

### Comparing `scrapere-0.2.8/setup.py` & `scrapere-0.2.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='scrapere',
     packages=find_packages(),
-    version='0.2.8',
+    version='0.2.9',
     description='Small set of my web scraping python tools',
     author='vPere',
     license='MIT',
     readme='README.md',
     install_requires=[
         'requests',
         'beautifulsoup4',
```

