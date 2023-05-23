# Comparing `tmp/twitter-api-client-0.8.1.tar.gz` & `tmp/twitter-api-client-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.8.1.tar", last modified: Fri May 19 17:27:56 2023, max compression
+gzip compressed data, was "twitter-api-client-0.8.2.tar", last modified: Tue May 23 23:11:11 2023, max compression
```

## Comparing `twitter-api-client-0.8.1.tar` & `twitter-api-client-0.8.2.tar`

### file list

```diff
@@ -1,19 +1,37 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-19 17:27:56.711608 twitter-api-client-0.8.1/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-30 17:24:38.000000 twitter-api-client-0.8.1/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)     7092 2023-05-19 17:27:56.711608 twitter-api-client-0.8.1/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-05-19 17:27:56.711608 twitter-api-client-0.8.1/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)     8414 2023-05-19 17:26:23.000000 twitter-api-client-0.8.1/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-19 17:27:56.711608 twitter-api-client-0.8.1/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-30 17:24:38.000000 twitter-api-client-0.8.1/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    21951 2023-05-19 16:55:22.000000 twitter-api-client-0.8.1/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    27271 2023-04-30 17:24:38.000000 twitter-api-client-0.8.1/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     5501 2023-04-30 17:24:38.000000 twitter-api-client-0.8.1/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    11972 2023-05-19 16:55:22.000000 twitter-api-client-0.8.1/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     5193 2023-05-19 17:15:54.000000 twitter-api-client-0.8.1/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     3277 2023-04-30 17:24:38.000000 twitter-api-client-0.8.1/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-19 17:27:56.711608 twitter-api-client-0.8.1/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     7092 2023-05-19 17:27:56.000000 twitter-api-client-0.8.1/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      355 2023-05-19 17:27:56.000000 twitter-api-client-0.8.1/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-05-19 17:27:56.000000 twitter-api-client-0.8.1/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       79 2023-05-19 17:27:56.000000 twitter-api-client-0.8.1/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-05-19 17:27:56.000000 twitter-api-client-0.8.1/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-23 23:11:11.305286 twitter-api-client-0.8.2/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-30 17:24:38.000000 twitter-api-client-0.8.2/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)     8728 2023-05-23 23:11:11.305286 twitter-api-client-0.8.2/PKG-INFO
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-23 23:11:11.301953 twitter-api-client-0.8.2/protonmail/
+-rw-r--r--   0 x         (1000) x         (1000)       78 2023-04-13 08:11:01.000000 twitter-api-client-0.8.2/protonmail/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    24269 2023-04-13 08:11:01.000000 twitter-api-client-0.8.2/protonmail/api.py
+-rw-r--r--   0 x         (1000) x         (1000)     5579 2023-04-13 08:11:01.000000 twitter-api-client-0.8.2/protonmail/cert_pinning.py
+-rw-r--r--   0 x         (1000) x         (1000)     1589 2023-04-13 08:11:01.000000 twitter-api-client-0.8.2/protonmail/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     1029 2023-04-13 08:11:01.000000 twitter-api-client-0.8.2/protonmail/exceptions.py
+-rw-r--r--   0 x         (1000) x         (1000)     1397 2023-04-13 08:11:01.000000 twitter-api-client-0.8.2/protonmail/logger.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-23 23:11:11.301953 twitter-api-client-0.8.2/protonmail/metadata/
+-rw-r--r--   0 x         (1000) x         (1000)      106 2023-04-13 08:11:01.000000 twitter-api-client-0.8.2/protonmail/metadata/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)     1225 2023-04-13 08:11:01.000000 twitter-api-client-0.8.2/protonmail/metadata/_base.py
+-rw-r--r--   0 x         (1000) x         (1000)     3432 2023-04-13 08:11:01.000000 twitter-api-client-0.8.2/protonmail/metadata/textfile_metadata.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-23 23:11:11.301953 twitter-api-client-0.8.2/protonmail/srp/
+-rw-r--r--   0 x         (1000) x         (1000)      172 2023-04-13 08:11:01.000000 twitter-api-client-0.8.2/protonmail/srp/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)     9305 2023-04-13 08:11:01.000000 twitter-api-client-0.8.2/protonmail/srp/_ctsrp.py
+-rw-r--r--   0 x         (1000) x         (1000)     4426 2023-04-13 08:11:01.000000 twitter-api-client-0.8.2/protonmail/srp/_pysrp.py
+-rw-r--r--   0 x         (1000) x         (1000)      684 2023-04-13 08:11:01.000000 twitter-api-client-0.8.2/protonmail/srp/pmhash.py
+-rw-r--r--   0 x         (1000) x         (1000)     1482 2023-04-13 08:11:01.000000 twitter-api-client-0.8.2/protonmail/srp/util.py
+-rw-r--r--   0 x         (1000) x         (1000)      962 2023-04-13 08:11:01.000000 twitter-api-client-0.8.2/protonmail/utils.py
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-05-23 23:11:11.305286 twitter-api-client-0.8.2/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)    10269 2023-05-23 23:05:47.000000 twitter-api-client-0.8.2/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-23 23:11:11.305286 twitter-api-client-0.8.2/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-30 17:24:38.000000 twitter-api-client-0.8.2/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    21961 2023-05-23 20:00:03.000000 twitter-api-client-0.8.2/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    27271 2023-04-30 17:24:38.000000 twitter-api-client-0.8.2/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     7199 2023-05-23 23:05:46.000000 twitter-api-client-0.8.2/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    11982 2023-05-23 19:56:12.000000 twitter-api-client-0.8.2/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     5203 2023-05-23 20:00:03.000000 twitter-api-client-0.8.2/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     5805 2023-05-23 23:05:47.000000 twitter-api-client-0.8.2/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-23 23:11:11.305286 twitter-api-client-0.8.2/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)     8728 2023-05-23 23:11:11.000000 twitter-api-client-0.8.2/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      740 2023-05-23 23:11:11.000000 twitter-api-client-0.8.2/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-05-23 23:11:11.000000 twitter-api-client-0.8.2/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)      118 2023-05-23 23:11:11.000000 twitter-api-client-0.8.2/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)       19 2023-05-23 23:11:11.000000 twitter-api-client-0.8.2/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.8.1/LICENSE` & `twitter-api-client-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.1/PKG-INFO` & `twitter-api-client-0.8.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,39 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.8.1
+Version: 0.8.2
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 Implementation of Twitter's v1, v2, and GraphQL APIs
 
-Includes tools to **scrape**, **automate**, and **search**.
+Tools include: [Scraping](#scraping), [Account Automation](#automation), [Search](#search)
+
+Automated email challenge solvers are supported for Proton Mail accounts. See [here](#automated-solvers) for more information.
+
+* [Installation](#installation)
+* [Automation](#automation)
+* [Scraping](#scraping)
+    * [Users/Tweets data](#get-all-usertweet-data)
+    * [Search](#search)
+* [Automated Solvers](#automated-solvers)
+* [Example API Responses](#example-api-responses)
+
+### Installation
+
+```bash
+pip install twitter-api-client
+```
 
 ### Automation
 
 ```python
 from twitter.account import Account
 
 email, username, password = ..., ..., ...
@@ -192,21 +208,20 @@
 scraper.download_media([
     111111,
     222222,
     333333,
     444444,
 ])
 
-
-
 # trends
 scraper.trends()
 ```
 
 #### Resume Pagination
+Pagination is already done by default, however there are circumstances where you may need to resume pagination from a specific cursor. For example, the `Followers` endpoint only allows for 50 requests every 15 minutes. In this case, we can resume from where we left off by providing a specific cursor value. This technique applies to any other endpoint defined in `twitter.constants.Operation`.
 ```python
 from twitter.scraper import Scraper
 from twitter.constants import Operation
 
 email, username, password = ...,...,...
 scraper = Scraper(email, username, password, debug=1, save=True)
 
@@ -242,10 +257,31 @@
     'min_faves:10000 @elonmusk until:2023-02-16 since:2023-02-01',
     'brasil portugal -argentina',
     'paperswithcode -tensorflow -tf',
     'skateboarding baseball guitar',
     'cheese bread butter',
     'ios android',
     limit=100,
-    retries=11,
+    retries=7,
 )
 ```
+
+**Search Operators Reference**
+
+https://developer.twitter.com/en/docs/twitter-api/v1/rules-and-filtering/search-operators
+
+https://developer.twitter.com/en/docs/twitter-api/tweets/search/integrate/build-a-query
+
+
+### Automated Solvers
+To set up automated email confirmation/verification solvers, add your Proton Mail credentials below as shown.
+This removes the need to manually solve email challenges via the web app. These credentials can be used in `Scraper`, `Account`, and `Search` constructors.
+
+E.g.
+
+```python
+from twitter.scraper import Scraper
+
+email, username, password = ..., ..., ...
+proton_email, proton_password = ..., ...
+account = Scraper(email, username, password, debug=1, save=True, protonmail={'email':proton_email, 'password':proton_password})
+```
```

### Comparing `twitter-api-client-0.8.1/setup.py` & `twitter-api-client-0.8.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,27 +4,47 @@
 
 install_requires = [
     "nest_asyncio",
     "aiohttp",
     "httpx",
     "tqdm",
     "orjson",
+    "requests",
+    "bcrypt",
+    "python-gnupg",
+    "pyopenssl",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.8.1",
+    version="0.8.2",
     python_requires=">=3.10.10",
     description="Twitter API",
     long_description=dedent('''
     Implementation of Twitter's v1, v2, and GraphQL APIs
     
-    Includes tools to **scrape**, **automate**, and **search**.
-
+    Tools include: [Scraping](#scraping), [Account Automation](#automation), [Search](#search)
+    
+    Automated email challenge solvers are supported for Proton Mail accounts. See [here](#automated-solvers) for more information.
+    
+    * [Installation](#installation)
+    * [Automation](#automation)
+    * [Scraping](#scraping)
+        * [Users/Tweets data](#get-all-usertweet-data)
+        * [Search](#search)
+    * [Automated Solvers](#automated-solvers)
+    * [Example API Responses](#example-api-responses)
+    
+    ### Installation
+    
+    ```bash
+    pip install twitter-api-client
+    ```
+    
     ### Automation
     
     ```python
     from twitter.account import Account
     
     email, username, password = ..., ..., ...
     account = Account(email, username, password, debug=2, save=True)
@@ -198,21 +218,20 @@
     scraper.download_media([
         111111,
         222222,
         333333,
         444444,
     ])
     
-
-    
     # trends
     scraper.trends()
     ```
     
     #### Resume Pagination
+    Pagination is already done by default, however there are circumstances where you may need to resume pagination from a specific cursor. For example, the `Followers` endpoint only allows for 50 requests every 15 minutes. In this case, we can resume from where we left off by providing a specific cursor value. This technique applies to any other endpoint defined in `twitter.constants.Operation`.
     ```python
     from twitter.scraper import Scraper
     from twitter.constants import Operation
     
     email, username, password = ...,...,...
     scraper = Scraper(email, username, password, debug=1, save=True)
     
@@ -248,17 +267,38 @@
         'min_faves:10000 @elonmusk until:2023-02-16 since:2023-02-01',
         'brasil portugal -argentina',
         'paperswithcode -tensorflow -tf',
         'skateboarding baseball guitar',
         'cheese bread butter',
         'ios android',
         limit=100,
-        retries=11,
+        retries=7,
     )
     ```
+    
+    **Search Operators Reference**
+    
+    https://developer.twitter.com/en/docs/twitter-api/v1/rules-and-filtering/search-operators
+    
+    https://developer.twitter.com/en/docs/twitter-api/tweets/search/integrate/build-a-query
+    
+    
+    ### Automated Solvers
+    To set up automated email confirmation/verification solvers, add your Proton Mail credentials below as shown.
+    This removes the need to manually solve email challenges via the web app. These credentials can be used in `Scraper`, `Account`, and `Search` constructors.
+    
+    E.g.
+    
+    ```python
+    from twitter.scraper import Scraper
+    
+    email, username, password = ..., ..., ...
+    proton_email, proton_password = ..., ...
+    account = Scraper(email, username, password, debug=1, save=True, protonmail={'email':proton_email, 'password':proton_password})
+    ```
     '''),
     long_description_content_type='text/markdown',
     author="Trevor Hobenshield",
     author_email="trevorhobenshield@gmail.com",
     url="https://github.com/trevorhobenshield/twitter-api-client",
     install_requires=install_requires,
     keywords="twitter api client async search automation bot scrape",
```

### Comparing `twitter-api-client-0.8.1/twitter/account.py` & `twitter-api-client-0.8.2/twitter/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from .login import login
 from .util import find_key, get_headers, fmt_status, get_cursor, save_data
 
 
 class Account:
 
     def __init__(self, email: str, username: str, password: str, **kwargs):
-        self.session = login(email, username, password)
+        self.session = login(email, username, password, **kwargs)
         self.gql_url = 'https://twitter.com/i/api/graphql'
         self.v1_url = 'https://api.twitter.com/1.1'
         self.save = kwargs.get('save', True)
         self.debug = kwargs.get('debug', 0)
         self.logger = self.init_logger(kwargs.get('log_config', False))
 
     @staticmethod
```

### Comparing `twitter-api-client-0.8.1/twitter/constants.py` & `twitter-api-client-0.8.2/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.1/twitter/login.py` & `twitter-api-client-0.8.2/twitter/login.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import sys
-
 from httpx import Client
-
 from .constants import GREEN, YELLOW, RED, BOLD, RESET
-from .util import find_key
+from .util import find_key, get_confirmation_code, get_inbox, init_session
 
 
 def update_token(session: Client, key: str, url: str, **kwargs) -> Client:
     caller_name = sys._getframe(1).f_code.co_name
     try:
         headers = {
             'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
@@ -18,20 +16,28 @@
             'x-twitter-auth-type': 'OAuth2Client' if session.cookies.get('auth_token') else '',
             'x-twitter-active-user': 'yes',
             'x-twitter-client-language': 'en',
         }
         r = session.post(url, headers=headers, **kwargs)
         info = r.json()
 
-        for s in info.get('subtasks', []):
-            if s.get('enter_text', {}).get('keyboard_type') == 'email':
-                print(f"[{YELLOW}warning{RESET}] {' '.join(find_key(s, 'text'))}")
+        print(f'{info = }')
+
+        for task in info.get('subtasks', []):
+            if task.get('enter_text', {}).get('keyboard_type') == 'email':
+                print(f"[{YELLOW}warning{RESET}] {' '.join(find_key(task, 'text'))}")
                 session.cookies.set('confirm_email', 'true')  # signal that email challenge must be solved
 
+            if task.get('subtask_id') == 'LoginAcid':
+                if task['enter_text']['hint_text'].casefold() == 'confirmation code':
+                    print(f"[{YELLOW}warning{RESET}] email confirmation code challenge.")
+                    session.cookies.set('confirmation_code', 'true')
+
         session.cookies.set(key, info[key])
+
     except KeyError as e:
         session.cookies.set('flow_errors', 'true')  # signal that an error occurred somewhere in the flow
         print(f'[{RED}error{RESET}] failed to update token at {BOLD}{caller_name}{RESET}\n{e}')
     return session
 
 
 def init_guest_token(session: Client) -> Client:
@@ -103,34 +109,62 @@
                     "text": session.cookies.get('email'),
                     "link": "next_link"
                 }
             }]
     })
 
 
-def execute_login_flow(session: Client) -> Client:
+def solve_confirmation_challenge(session: Client, email: str, password: str) -> Client:
+    proton_session = init_session(email, password)
+    inbox = get_inbox(proton_session)
+    confirmation_code = get_confirmation_code(inbox)
+    print(f'{confirmation_code = }')
+    return update_token(session, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', json={
+        "flow_token": session.cookies.get('flow_token'),
+        'subtask_inputs': [
+            {
+                'subtask_id': 'LoginAcid',
+                'enter_text': {
+                    'text': confirmation_code,
+                    'link': 'next_link',
+                },
+            },
+        ],
+    })
+
+
+def execute_login_flow(session: Client) -> Client | None:
     session = init_guest_token(session)
     for fn in [flow_start, flow_instrumentation, flow_username, flow_password, flow_duplication_check]:
         session = fn(session)
 
     # solve email challenge
     if session.cookies.get('confirm_email') == 'true':
         session = confirm_email(session)
 
+    # solve confirmation challenge (Proton Mail only)
+    if session.cookies.get('confirmation_code') == 'true':
+        if not session.protonmail:
+            print(f'[{RED}warning{RESET}] Please check your email for a confirmation code'
+                  f' and log in again using the web app. If you wish to automatically solve'
+                  f' email confirmation challenges, add a Proton Mail account in your account settings')
+            return
+        session = solve_confirmation_challenge(session, *session.protonmail.values())
     return session
 
 
-def login(email: str, username: str, password: str) -> Client:
+def login(email: str, username: str, password: str, **kwargs) -> Client:
     session = Client()
     session.cookies.update({
         "email": email,
         "username": username,
         "password": password,
         "guest_token": None,
         "flow_token": None,
     })
+    session.protonmail = kwargs.get('protonmail')
     session = execute_login_flow(session)
-    if session.cookies.get('flow_errors') == 'true':
+    if not session or session.cookies.get('flow_errors') == 'true':
         print(f'[{RED}error{RESET}] {BOLD}{username}{RESET} login failed')
     else:
         print(f'[{GREEN}success{RESET}] {BOLD}{username}{RESET} login success')
     return session
```

### Comparing `twitter-api-client-0.8.1/twitter/scraper.py` & `twitter-api-client-0.8.2/twitter/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         uvloop.install()
     except ImportError as e:
         ...
 
 
 class Scraper:
     def __init__(self, email: str, username: str, password: str, **kwargs):
-        self.session = login(email, username, password)
+        self.session = login(email, username, password, **kwargs)
         self.api = 'https://twitter.com/i/api/graphql'
         self.save = kwargs.get('save', True)
         self.debug = kwargs.get('debug', 0)
         self.logger = self.init_logger(kwargs.get('log_config', False))
 
     @staticmethod
     def init_logger(cfg: dict) -> Logger:
```

### Comparing `twitter-api-client-0.8.1/twitter/search.py` & `twitter-api-client-0.8.2/twitter/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         uvloop.install()
     except ImportError as e:
         ...
 
 
 class Search:
     def __init__(self, email: str, username: str, password: str, **kwargs):
-        self.session = login(email, username, password)
+        self.session = login(email, username, password, **kwargs)
         self.api = 'https://api.twitter.com/2/search/adaptive.json?'
         self.save = kwargs.get('save', True)
         self.debug = kwargs.get('debug', 0)
         self.logger = self.init_logger(kwargs.get('log_config', False))
 
     @staticmethod
     def init_logger(cfg: dict) -> Logger:
```

### Comparing `twitter-api-client-0.8.1/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.8.2/twitter_api_client.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,39 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.8.1
+Version: 0.8.2
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 Implementation of Twitter's v1, v2, and GraphQL APIs
 
-Includes tools to **scrape**, **automate**, and **search**.
+Tools include: [Scraping](#scraping), [Account Automation](#automation), [Search](#search)
+
+Automated email challenge solvers are supported for Proton Mail accounts. See [here](#automated-solvers) for more information.
+
+* [Installation](#installation)
+* [Automation](#automation)
+* [Scraping](#scraping)
+    * [Users/Tweets data](#get-all-usertweet-data)
+    * [Search](#search)
+* [Automated Solvers](#automated-solvers)
+* [Example API Responses](#example-api-responses)
+
+### Installation
+
+```bash
+pip install twitter-api-client
+```
 
 ### Automation
 
 ```python
 from twitter.account import Account
 
 email, username, password = ..., ..., ...
@@ -192,21 +208,20 @@
 scraper.download_media([
     111111,
     222222,
     333333,
     444444,
 ])
 
-
-
 # trends
 scraper.trends()
 ```
 
 #### Resume Pagination
+Pagination is already done by default, however there are circumstances where you may need to resume pagination from a specific cursor. For example, the `Followers` endpoint only allows for 50 requests every 15 minutes. In this case, we can resume from where we left off by providing a specific cursor value. This technique applies to any other endpoint defined in `twitter.constants.Operation`.
 ```python
 from twitter.scraper import Scraper
 from twitter.constants import Operation
 
 email, username, password = ...,...,...
 scraper = Scraper(email, username, password, debug=1, save=True)
 
@@ -242,10 +257,31 @@
     'min_faves:10000 @elonmusk until:2023-02-16 since:2023-02-01',
     'brasil portugal -argentina',
     'paperswithcode -tensorflow -tf',
     'skateboarding baseball guitar',
     'cheese bread butter',
     'ios android',
     limit=100,
-    retries=11,
+    retries=7,
 )
 ```
+
+**Search Operators Reference**
+
+https://developer.twitter.com/en/docs/twitter-api/v1/rules-and-filtering/search-operators
+
+https://developer.twitter.com/en/docs/twitter-api/tweets/search/integrate/build-a-query
+
+
+### Automated Solvers
+To set up automated email confirmation/verification solvers, add your Proton Mail credentials below as shown.
+This removes the need to manually solve email challenges via the web app. These credentials can be used in `Scraper`, `Account`, and `Search` constructors.
+
+E.g.
+
+```python
+from twitter.scraper import Scraper
+
+email, username, password = ..., ..., ...
+proton_email, proton_password = ..., ...
+account = Scraper(email, username, password, debug=1, save=True, protonmail={'email':proton_email, 'password':proton_password})
+```
```

