# Comparing `tmp/natalify-2.6.tar.gz` & `tmp/natalify-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "natalify-2.6.tar", last modified: Mon May 22 21:19:27 2023, max compression
+gzip compressed data, was "natalify-2.8.tar", last modified: Wed May 24 08:35:04 2023, max compression
```

## Comparing `natalify-2.6.tar` & `natalify-2.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 21:19:27.893522 natalify-2.6/
--rw-rw-rw-   0        0        0     1344 2023-05-22 10:26:13.000000 natalify-2.6/LICENSE
--rw-rw-rw-   0        0        0     2163 2023-05-22 21:19:27.893522 natalify-2.6/PKG-INFO
--rw-rw-rw-   0        0        0     1664 2023-05-22 11:28:41.000000 natalify-2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 21:19:27.883172 natalify-2.6/natalify/
--rw-rw-rw-   0        0        0       25 2023-05-22 10:10:51.000000 natalify-2.6/natalify/__init__.py
--rw-rw-rw-   0        0        0       37 2023-05-22 10:11:37.000000 natalify-2.6/natalify/__main__.py
--rw-rw-rw-   0        0        0    63378 2023-05-22 21:16:12.000000 natalify-2.6/natalify/natalify.py
-drwxrwxrwx   0        0        0        0 2023-05-22 21:19:27.893522 natalify-2.6/natalify.egg-info/
--rw-rw-rw-   0        0        0     2163 2023-05-22 21:19:27.000000 natalify-2.6/natalify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-05-22 21:19:27.000000 natalify-2.6/natalify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 21:19:27.000000 natalify-2.6/natalify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-05-22 21:19:27.000000 natalify-2.6/natalify.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 21:19:27.000000 natalify-2.6/natalify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 21:19:27.893522 natalify-2.6/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-05-22 21:19:22.000000 natalify-2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 08:35:04.071459 natalify-2.8/
+-rw-rw-rw-   0        0        0     1344 2023-05-22 10:26:13.000000 natalify-2.8/LICENSE
+-rw-rw-rw-   0        0        0     2184 2023-05-24 08:35:04.071459 natalify-2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1664 2023-05-22 11:28:41.000000 natalify-2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 08:35:04.055836 natalify-2.8/natalify/
+-rw-rw-rw-   0        0        0       25 2023-05-22 10:10:51.000000 natalify-2.8/natalify/__init__.py
+-rw-rw-rw-   0        0        0       37 2023-05-22 10:11:37.000000 natalify-2.8/natalify/__main__.py
+-rw-rw-rw-   0        0        0    64029 2023-05-24 08:33:11.000000 natalify-2.8/natalify/natalify.py
+drwxrwxrwx   0        0        0        0 2023-05-24 08:35:04.071459 natalify-2.8/natalify.egg-info/
+-rw-rw-rw-   0        0        0     2184 2023-05-24 08:35:02.000000 natalify-2.8/natalify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-05-24 08:35:03.000000 natalify-2.8/natalify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 08:35:02.000000 natalify-2.8/natalify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-05-24 08:35:02.000000 natalify-2.8/natalify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-24 08:35:02.000000 natalify-2.8/natalify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 08:35:04.071459 natalify-2.8/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-05-24 08:34:30.000000 natalify-2.8/setup.py
```

### Comparing `natalify-2.6/LICENSE` & `natalify-2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `natalify-2.6/PKG-INFO` & `natalify-2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: natalify
-Version: 2.6
+Version: 2.8
 Summary: A simple automation software for various tasks
 Author: jack
 Author-email: kinginjack@gmail.com
 License: GPL-3.0
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -72,7 +73,8 @@
 
 ## Contact
 
 For any inquiries or feedback, please contact the author:
 
 Name: Jack.
 Email: kinginjack@gmail.com
+
```

### Comparing `natalify-2.6/README.md` & `natalify-2.8/README.md`

 * *Files identical despite different names*

### Comparing `natalify-2.6/natalify/natalify.py` & `natalify-2.8/natalify/natalify.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from cryptography import fernet
 from selenium.webdriver.common.keys import Keys
 from webdriver_manager.chrome import ChromeDriverManager
 import sys
 import platform
 from tinydb import TinyDB, Query,where
 import traceback
+import argparse
 
 db = TinyDB(fr'rem_db.json')
 User = Query()
 
 colorama.init()
 
 
@@ -279,33 +280,53 @@
         else:
             await self.my_account()
 
             self.block_thread=True
 
 
     async def logout_my_account(self):
-        account_tag = "/html/body/div[1]/div/div/div/div[1]/div/div/div/div[1]/section/nav/div[2]/div/div/div[3]/div/div[6]"
-        account = WebDriverWait(self.driver, 50).until(
-            EC.presence_of_element_located((By.XPATH, account_tag)))
         
-        self.sleep_ = random.randrange(1, 5)
+        await self.my_account()
+
+        buttons = WebDriverWait(self.driver, 20).until(
+                            EC.presence_of_all_elements_located((By.CSS_SELECTOR, "button[class='_abl-']")))
+        
+        self.sleep_ = random.randrange(2, 5)
         self.seconds = time.perf_counter()
-        self.status = f"Getting my account ( {self.username} ) info"
+        self.status = f"Logging out of {self.username} step 1"
         await asyncio.sleep(self.sleep_)
-        account.click()
 
-        account_profile = WebDriverWait(self.driver, 50).until(
-            EC.presence_of_element_located((By.XPATH, "//*[contains(text(),'Log Out')]")))
+        
+        for element in buttons:
+
+            if "Options" in element.get_attribute("innerHTML"):
+        
+                element.click()
+
+                break
+
         self.sleep_ = random.randrange(2, 7)
         self.seconds = time.perf_counter()
-        self.status = f"Logging out of {self.username}"
+        self.status = f"Logging out of {self.username} step 2"
         await asyncio.sleep(self.sleep_)
-        account_profile.click()
 
 
+        
+                # Wait for the button to be visible
+        wait = WebDriverWait(self.driver, 10)
+        button = wait.until(EC.element_to_be_clickable((By.XPATH, '//button[text()="Log Out"]')))
+
+
+        # Click the button
+        button.click()
+            
+
+        
+        
+       
     async def my_account(self):
 
                 # Find all elements that match the selector
         wait = WebDriverWait(self.driver, 10)  # Adjust the timeout as needed
         elements = wait.until(EC.presence_of_all_elements_located((By.CSS_SELECTOR, "div.x1n2onr6 a.x1i10hfl")))
 
         # Desired href value
@@ -1393,19 +1414,26 @@
         os_detected = "WINDOWS OS"
     if platform.system() == "Linux":
         os_detected = "LINUX OS"
 
     figlet_color = ["cyan", "yellow", "green", "magenta"]
     random.shuffle(figlet_color)
     ascii_ = f'''                          
-    |_ _|  | \| |   / __|  |_   _|  /   \   / __|   | _ \   /   \ |  \/  |    o O O  | _ )   / _ \  |_   _| 
-    | |   | .` |   \__ \    | |    | - |  | (_ |   |   /   | - | | |\/| |   o       | _ \  | (_) |   | |         
-    |___|  |_|\_|   |___/   _|_|_   |_|_|   \___|   |_|_\   |_|_| |_|__|_|  TS__[O]  |___/   \___/   _|_|_     {time.ctime()}
-_|"""""|_|"""""|_|"""""|_|"""""|_|"""""|_|"""""|_|"""""|_|"""""|_|"""""| [======|_|"""""|_|"""""|"""""|
-"`-0-0-'"`-0-0-'"`-0-0-'"`-0-0-'"`-0-0-'"`-0-0-'"`-0-0-'"`-0-0-'"`-0-0-'./o--000'"`-0-0-'"`-0-0-'"`-0-0-'
+      
+     _____                              
+    (, /                                
+      / __   _  _/_ _   _   __  _  ___  
+  ___/__/ (_/_)_(__(_(_(_/_/ (_(_(_// (_
+(__ /                 .-/               
+                     (_/                
+             ______                     
+            (, /    )                   
+              /---(  ____/_              {time.ctime()}
+           ) / ____)(_) (__             
+          (_/ (                         
 
         '''
     if os_detected == "WINDOWS OS":
         clear_console = "cls"
     else:
         clear_console = "clear"
 
@@ -1427,27 +1455,35 @@
 
 
     
 def logout_user(comment,window,run_hashtags,run_target_accounts,logout):
     encrypt_creds = fernet.Fernet(encryption_key)
     credentials = db.search(User.credentials == 'true')
     if credentials:
+        # print(credentials)
+        encrypted_creds=credentials[0].get("encrypted")
+
+        decrypt_credentials=credentials[0].get("encrypted").encode()
+
+        encrypted = encrypt_creds.decrypt(decrypt_credentials)
+        decrypt_pickle2 = pickle.loads(encrypted)
+        username = decrypt_pickle2.get("username", "specify a username")
+        password = decrypt_pickle2.get("password", "specify a password")
 
-        Bot(comment, window, use_hashtags=run_hashtags, use_target_users=run_target_accounts, logout=logout)
+        Bot(comment, window,username,password,encrypted_creds, use_hashtags=run_hashtags, use_target_users=run_target_accounts, logout=logout)
 
         decrypt_credentials = credentials[0].get("encrypted").encode()
 
         decrypt_cryptography = encrypt_creds.decrypt(decrypt_credentials)
         decrypt_pickle2 = pickle.loads(decrypt_cryptography)
         username = decrypt_pickle2.get("username", "specify a username")
 
         db.remove(where("credentials") == 'true')
-        db.remove(where("last_settings") == 'true')
-
-        print(colored(f"Logged out {username} and deleted all settings data except for daily liked and comment count","yellow"))
+       
+        print(colored(f"\nLogged out {username} and deleted all settings","green"))
         exit()
     else:
         print(colored("No logged in users ","cyan"))
         print("\nlogin")
 
 
 
@@ -1618,17 +1654,20 @@
         run_hashtags = False
 
     if run_target_accounts=="Y":
         run_target_accounts=True
     else:
         run_target_accounts = False
 
-    if len(sys.argv) >= 2:
-        if sys.argv[1] == "-logout":
-            print(colored("You'll be logged out of your account","red"))
-            logout_user(comment,window,run_hashtags,run_target_accounts,True)
+    parser = argparse.ArgumentParser()
+    parser.add_argument('-logout', action='store_true', help="Logout from the account")
+    args = parser.parse_args()
+
+    if args.logout:
+        print(colored("You'll be logged out of your account", "red"))
+        logout_user(comment, window, run_hashtags, run_target_accounts, True)
     else:
         Bot(comment,window,username,password,encrypted_creds,use_hashtags=run_hashtags,use_target_users=run_target_accounts)
 
-# if __name__=="__main__":
-#     start()
+if __name__=="__main__":
+    start()
```

### Comparing `natalify-2.6/natalify.egg-info/PKG-INFO` & `natalify-2.8/natalify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: natalify
-Version: 2.6
+Version: 2.8
 Summary: A simple automation software for various tasks
 Author: jack
 Author-email: kinginjack@gmail.com
 License: GPL-3.0
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -72,7 +73,8 @@
 
 ## Contact
 
 For any inquiries or feedback, please contact the author:
 
 Name: Jack.
 Email: kinginjack@gmail.com
+
```

### Comparing `natalify-2.6/setup.py` & `natalify-2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='natalify',
-    version='2.6',
+    version='2.8',
     packages=setuptools.find_packages(),
     license='GPL-3.0',
     author='jack',
     author_email='kinginjack@gmail.com',
     description='A simple automation software for various tasks',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

