# Comparing `tmp/PyForks-0.0.8.tar.gz` & `tmp/PyForks-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyForks-0.0.8.tar", last modified: Fri Oct 14 22:22:09 2022, max compression
+gzip compressed data, was "PyForks-0.0.9.tar", last modified: Sun Oct 23 17:46:37 2022, max compression
```

## Comparing `PyForks-0.0.8.tar` & `PyForks-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-10-14 22:22:09.555188 PyForks-0.0.8/
--rw-rw-rw-   0        0        0    11558 2022-10-14 16:15:34.000000 PyForks-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     2287 2022-10-14 22:22:09.555188 PyForks-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-10-14 22:22:09.543191 PyForks-0.0.8/PyForks/
--rw-rw-rw-   0        0        0        0 2022-10-14 19:30:56.000000 PyForks-0.0.8/PyForks/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-14 22:22:09.554188 PyForks-0.0.8/PyForks/_test/
--rw-rw-rw-   0        0        0        0 2022-10-14 19:31:02.000000 PyForks-0.0.8/PyForks/_test/__init__.py
--rw-rw-rw-   0        0        0     1087 2022-10-14 21:03:30.000000 PyForks-0.0.8/PyForks/_test/test_regions.py
--rw-rw-rw-   0        0        0     1476 2022-10-14 20:45:15.000000 PyForks-0.0.8/PyForks/_test/test_users.py
--rw-rw-rw-   0        0        0     6429 2022-10-14 20:41:00.000000 PyForks-0.0.8/PyForks/trailforks.py
--rw-rw-rw-   0        0        0     6056 2022-10-14 21:48:19.000000 PyForks-0.0.8/PyForks/trailforks_region.py
--rw-rw-rw-   0        0        0     6965 2022-10-14 20:33:07.000000 PyForks-0.0.8/PyForks/trailforks_user.py
-drwxrwxrwx   0        0        0        0 2022-10-14 22:22:09.552189 PyForks-0.0.8/PyForks.egg-info/
--rw-rw-rw-   0        0        0     2287 2022-10-14 22:22:09.000000 PyForks-0.0.8/PyForks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2022-10-14 22:22:09.000000 PyForks-0.0.8/PyForks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-14 22:22:09.000000 PyForks-0.0.8/PyForks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2022-10-14 22:22:09.000000 PyForks-0.0.8/PyForks.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-10-14 22:22:09.000000 PyForks-0.0.8/PyForks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1738 2022-10-14 22:17:13.000000 PyForks-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2022-10-14 22:22:09.556189 PyForks-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      932 2022-10-14 22:21:59.000000 PyForks-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-23 17:46:37.281353 PyForks-0.0.9/
+-rw-rw-rw-   0        0        0    11558 2022-10-14 16:15:34.000000 PyForks-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3784 2022-10-23 17:46:37.280353 PyForks-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-10-23 17:46:37.266353 PyForks-0.0.9/PyForks/
+-rw-rw-rw-   0        0        0        0 2022-10-14 19:30:56.000000 PyForks-0.0.9/PyForks/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-23 17:46:37.279353 PyForks-0.0.9/PyForks/_test/
+-rw-rw-rw-   0        0        0        0 2022-10-14 19:31:02.000000 PyForks-0.0.9/PyForks/_test/__init__.py
+-rw-rw-rw-   0        0        0     1828 2022-10-15 00:11:29.000000 PyForks-0.0.9/PyForks/_test/test_regions.py
+-rw-rw-rw-   0        0        0     1165 2022-10-23 17:45:34.000000 PyForks-0.0.9/PyForks/_test/test_users.py
+-rw-rw-rw-   0        0        0     6411 2022-10-14 23:50:02.000000 PyForks-0.0.9/PyForks/trailforks.py
+-rw-rw-rw-   0        0        0     8230 2022-10-23 17:21:30.000000 PyForks-0.0.9/PyForks/trailforks_region.py
+-rw-rw-rw-   0        0        0     8143 2022-10-23 17:37:36.000000 PyForks-0.0.9/PyForks/trailforks_user.py
+drwxrwxrwx   0        0        0        0 2022-10-23 17:46:37.277352 PyForks-0.0.9/PyForks.egg-info/
+-rw-rw-rw-   0        0        0     3784 2022-10-23 17:46:37.000000 PyForks-0.0.9/PyForks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2022-10-23 17:46:37.000000 PyForks-0.0.9/PyForks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-23 17:46:37.000000 PyForks-0.0.9/PyForks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2022-10-23 17:46:37.000000 PyForks-0.0.9/PyForks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2022-10-23 17:46:37.000000 PyForks-0.0.9/PyForks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3235 2022-10-23 17:41:23.000000 PyForks-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-10-23 17:46:37.281353 PyForks-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      932 2022-10-23 17:46:28.000000 PyForks-0.0.9/setup.py
```

### Comparing `PyForks-0.0.8/LICENSE` & `PyForks-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyForks-0.0.8/PKG-INFO` & `PyForks-0.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 Metadata-Version: 2.1
 Name: PyForks
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package to interface with Trailforks.com
 Home-page: http://pypi.python.org/pypi/PyForks/
 Author: Trailforks Python Library
 Author-email: MinnMTB@gmail.com
 License: LICENSE.txt
 Project-URL: Bug Reports, https://github.com/cribdragg3r/PyForks/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Source, https://github.com/cribdragg3r/PyForks
 Project-URL: Documentation, https://pyforks.mn-mtb.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a href ="https://mn-mtb.com">
   <img src="./doc/PyForks.png"
-    title="PyForks" align="left" height=75 length=75 />
+    title="PyForks" align="left" height=100 length=100 />
     </a>
 
 
 # PyForks
 
 [![PyForks Tests](https://github.com/cribdragg3r/PyForks/actions/workflows/python-app.yml/badge.svg)](https://github.com/cribdragg3r/PyForks/actions/workflows/python-app.yml)
+[![GitHub](https://img.shields.io/github/license/cribdragg3r/PyForks?style=flat-square)](https://github.com/cribdragg3r/PyForks/blob/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/PyForks?style=flat-square)](https://pypi.org/project/PyForks/)
 
-Python Trailforks Library for interacting with Trailforks.com
+
+Python Trailforks Library for interacting with Trailforks.com. Help [support](https://github.com/sponsors/cribdragg3r) this project and more.
 
 ## About
 
-PyForks has been designed to help me automate much of the manual data aggregation I was doing in order to build metrics for my local city and state trail systems. For example: [wlmt.mn-mtb.com](http://wlmt.mn-mtb.com). The end goal of this project is the ability to make it much easier to pull data down that people are interested in and analyze it in a way that non-technical individuals can digest and understand impact in hopes of additional funding and intrest. 
+PyForks has been designed to help me automate much of the manual data aggregation I was doing in order to build metrics for my local city and state trail systems. For example: [wlmt.mn-mtb.com](http://wlmt.mn-mtb.com). The end goal of this project is the ability to make it much easier to pull data down that people are interested in and analyze it in a way that non-technical individuals can digest and understand impact in hopes of additional funding and interest. 
 
 ## Installation & Documentation
 
 - Install: `pip install pyforks`
 - Documentation: [PyForks.mn-mtb.com](https://PyForks.mn-mtb.com)
 
 ### Quick Start
@@ -40,23 +43,62 @@
 **Get Information on a User**
 
 ```python
 from PyForks.trailforks_user import TrailforksUser
 from pprint import pprint
 
 # Get Basic information about a user
-tf = TrailforksUser()
-user_info = tf.get_user_info("mnmtb")
+tf_u = TrailforksUser()
+user_info = tf_u.get_user_info("mnmtb")
 pprint(user_info)
 
 # Get the User's Gear
-tf.username = "<your_username>"
-tf.password = "<your_password>"
-tf.login()
-user_gear = tf.get_user_gear("mnmtb")
+tf_u.username = "<your_username>"
+tf_u.password = "<your_password>"
+tf_u.login()
+user_gear = tf_u.get_user_gear("mnmtb")
 pprint(user_gear)
+
+"""
+EXAMPLE OUTPUT:
+{
+  'admin_region': 
+    {
+    'region_link': 'https://www.trailforks.com/region/minnesota/',
+    'region_name': 'Minnesota'
+    },
+ 'city': 'Lakeville',
+ 'country': 'USA',
+ 'is_regional_admin': True,
+ 'profile_link': 'https://www.trailforks.com/profile/mnmtb',
+ 'recent_ride_locations': ['West Lake Marion Park',
+                           'Murphy-Hanrehan Park',
+                           'Lebanon Hills',
+                           'Spirit Mountain Bike Park',
+                           'Battle Creek',
+                           'Cottage Grove Bike Park',
+                           'Lakeville'],
+ 'state': 'Minnesota',
+ 'username': 'mnmtb'}
+ """
+```
+
+**Get Information on a region**
+```python
+from PyForks.trailforks_region import TrailforksRegion
+tf_r = TrailforksRegion(username=<username>, password=<password>)
+tf_r.login()
+
+# Download All of a regions trails in CSV:
+tf_r.download_all_region_trails(region, region_id)
+
+# Download all region ridelogs in csv
+tf_r.download_all_region_ridelogs(region)
+
+# Download all region ridecounts in CSV
+tf_r.download_region_ridecounts(region)
+
 ```
-  
 
 ## Contribute
 
 Send all the pull requests you want!
```

### Comparing `PyForks-0.0.8/PyForks/trailforks.py` & `PyForks-0.0.9/PyForks/trailforks.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     Returns:
         _type_: original function
     """
     @wraps(func)
     def run_checks(self, *args, **kwargs):
         if not self.authenticated:
-            print("[!] Need Authentication:\nYou must provide the Trailforks class with a valid cookie (trailforks_cookie=<cookie>)")
+            print("[!] Need Authentication:\nYou must provide username= and password=")
             exit(1)
         return func(self, *args, **kwargs) 
     return run_checks
         
 
 class Trailforks:
     def __init__(self, username=None, password=None):
@@ -51,15 +51,15 @@
 
         payload = {
             "ripformname": "loginform",
             "formpage": "/login/#loginform",
             "fieldstack[0]": "source",
             "source-alpha": "trailforks",
             "fieldstack[1]": "redirect",
-            "redirect-textbasic": "https://www.trailforks.com/profile/mnmtb/",
+            "redirect-textbasic": f"https://www.trailforks.com/profile/{self.uri_encode(self.username)}/",
             "fieldstack[2]": "username",
             "username-login-loginlen": self.username,
             "fieldstack[3]": "password",
             "password-password-lt200": self.password,
             "fieldstack[4]": "rememberme",
             "rememberme": "",
             "fieldstack[5]": "logoutother",
```

### Comparing `PyForks-0.0.8/PyForks/trailforks_region.py` & `PyForks-0.0.9/PyForks/trailforks_region.py`

 * *Files 26% similar despite different names*

```diff
@@ -33,62 +33,92 @@
         """
         if not self.is_valid_region(region):
             print(f"[!] {region} is not a valid Trailforks Region.")
             exit(1)
         return True
 
     @authentication
-    def download_region_ridecounts(self, region: str, output_path=".") -> None:
+    def download_region_ridecounts(self, region: str, output_path=".") -> bool:
+        """
+        Downloads a regions total ridecounts is CSV format. Ideally, this should 
+        be handled by the Trailforks API but, they've not provisioning access 
+        at this point (https://www.trailforks.com/about/api/)
+
+        Args:
+            region (str): Trailforks region name per URI
+            output_path (str, optional): Where to store CSV Defaults to ".".
+
+        Returns:
+            bool: true:CSV written to disk;False:failed to write CSV
+        """
+        success = False
         self.check_region(region)
         uri = f"https://www.trailforks.com/region/{region}/ridelogcountscsv/"
         r = self.trailforks_session.get(uri, allow_redirects=True)
         raw_csv_data = r.text
         
-        open(f"{output_path}/{region}_ridelogcounts.csv", "w").write(raw_csv_data)
+        if "date,rides" in raw_csv_data:
+            open(f"{output_path}/{region}_ridelogcounts.csv", "w").write(raw_csv_data)
+            success = True
+        else:
+            if self._check_requires_region_admin(r.text):
+                print(f"[!] Error: You need to be an Admin for {region} to download Trail Ridecounts")
+
+        return success
 
     @authentication
     def download_all_region_trails(self, region: str, region_id: str, output_path=".") -> bool:
         """
         Each region has a CSV export capability to export all trails within the region.
         This function automates that export for the end user and saves a csv to local
-        disk.
+        disk. Ideally, this should be handled by the Trailforks API but,
+        they've not provisioning access at this point (https://www.trailforks.com/about/api/)
 
         Args:
             region (str): region name as is shows on a URI
             region_id (str): this is the integer (string representation) of the region
             output_path (str, optional): output directory for the CSV. Defaults to ".".
 
         Returns:
-            bool: True:export successful;False:export failed.
+            bool: true:CSV written to disk;False:failed to write CSV
         """
+        success = False
         self.check_region(region)
         uri = f"https://www.trailforks.com/tools/trailspreadsheet_csv/?cols=trailid,title,aka,activitytype,difficulty,status,condition,region_title,rid,difficulty_system,trailtype,usage,direction,season,unsanctioned,hidden,rating,ridden,total_checkins,total_reports,total_photos,total_videos,faved,views,global_rank,created,land_manager,closed,wet_weather,distance,time,alt_change,alt_max,alt_climb,alt_descent,grade,dst_climb,dst_descent,dst_flat,alias,inventory_exclude,trail_association,sponsors,builders,maintainers&rid={region_id}"
         r = self.trailforks_session.get(uri, allow_redirects=True)
         raw_csv_data = r.text
         clean_data = re.sub(r'[aA-zZ]\n', "\",", raw_csv_data)
 
-        open(f"{output_path}/{region}_trail_listing.csv", "w").write(clean_data)
+        if "trailid,title" in clean_data:
+            success = True
+            open(f"{output_path}/{region}_trail_listing.csv", "w").write(clean_data)
+        else:
+            if self._check_requires_region_admin(r.text):
+                print(f"[!] Error: You need to be an Admin for {region} to download Trail Data")
+
+        return success
 
     @authentication
     def download_all_region_ridelogs(self, region: str, output_path=".") -> bool:
         """
         Downloads all of the trail ridelogs since the begining of the 
         trails existance and stores the results in CSV format on the 
-        local disk
+        local disk. Ideally, this should be handled by the Trailforks API but,
+        they've not provisioning access at this point (https://www.trailforks.com/about/api)
 
         Args:
             region (str): region name as is shows on a URI
             output_path (str, optional): Path to store csv. Defaults to ".".
-
+            
         Returns:
-            bool: True:successfully saved data;False:failed
+            bool: true:CSV written to disk;False:failed to write CSV
         """
         self.check_region(region)
         region_info = self._get_region_info(region)
-        total_pages = round(region_info["total_ridelogs"]/30)
+        total_pages = round(region_info["total_ridelogs"]/90)
         dataframes_list = []
 
         pbar = tqdm(total=total_pages, desc=f"Enumerating {region} Rider Pages")
         for i in range(1, total_pages + 1):
             try:
                 domain = f"https://www.trailforks.com/region/{region}/ridelogs/?viewMode=table&page={i}"
                 tmp_df = pd.read_html(domain, index_col=None, header=0)
@@ -105,17 +135,21 @@
 
                 pbar.update(1)
             except Exception as e:
                 pbar.update(1)
                 break
         pbar.close()
 
-        df = pd.concat(dataframes_list, axis=0, ignore_index=True)
-        df.to_csv(f"{output_path}/{region}_scraped_riders.csv")
-        
+        try:
+            df = pd.concat(dataframes_list, axis=0, ignore_index=True)
+            df.to_csv(f"{output_path}/{region}_scraped_riders.csv")
+            return True
+        except:
+            return False
+
 
     def _get_region_info(self, region: str) -> dict:
         """
         Pulls region specific metrics from the region page
 
         Args:
             region (str): region name as is shows on a URI
@@ -139,7 +173,24 @@
         }
         region_vars = ["total_ridelogs", "unique_riders", "trails_ridden", "average_trails_per_ride"]
 
         for i, item in enumerate(list_items):
             region_info[region_vars[i]] = int(re.search(r'>([0-9].*)<', str(item)).groups()[0].replace(",",""))
         
         return region_info
+
+
+    def _check_requires_region_admin(self, error_message: str) -> bool:
+        """
+        If we get an error on an authenticated function, it might be because
+        the user in question is not a admin for the local trail/region and
+        are just a standard user. This function determines this by looking at
+        known error codes.
+
+        Args:
+            error_message (str): RAW Html error page 
+
+        Returns:
+            bool: True:action requires admin;False:action doesn't need admin
+        """
+        error_messages = ["Only trusted users can export"]
+        return any([x in error_message for x in error_messages])
```

### Comparing `PyForks-0.0.8/PyForks/trailforks_user.py` & `PyForks-0.0.9/PyForks/trailforks_user.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,19 @@
             "recent_ride_locations": self.__get_user_recent_rides(user),
         }
         (
             user_data["city"],
             user_data["state"],
             user_data["country"],
         ) = self.__get_user_city_state_country(user)
+
+        (
+            user_data["admin_region"],
+            user_data["is_regional_admin"]
+        ) = self.is_regional_admin(user)
         return user_data
 
     @authentication
     def rescan_ridelogs_for_badges(self, ride_ids: list) -> bool:
         """
         If you add a new badge or new badges have been added that your
         old rides are currently not counting for, you can rescan them to
@@ -59,15 +64,15 @@
                 }
                 r = self.trailforks_session.get(uri)
             return True
         except Exception as e:
             print(e)
             return False
 
-    def get_user_all_ridelogs(self, user: str) -> pd.DataFrame:
+    def get_user_ridelogs_all(self, user: str) -> pd.DataFrame:
         """
         Scrape all of the users ridelogs and throw that into a pandas
         dataframe.
 
         Args:
             user (str): A Trailforks username
 
@@ -181,14 +186,15 @@
         """
         # get the users most recent (current year) riding locations
         try:
             activity_uri = f"https://www.trailforks.com/profile/{self.uri_encode(user)}/ridelog/?sort=l.timestamp&activitytype=1&year=0&bikeid=0"
             activity_df = pd.read_html(activity_uri)[0]
             activity_df = activity_df.fillna('')
             recent_ride_locations = activity_df.location.unique().tolist()
+            recent_ride_locations.remove('')
         except ValueError as e:
             recent_ride_locations = []
 
         return recent_ride_locations
 
     @authentication
     def get_user_gear(self, user: str) -> list:
@@ -206,8 +212,35 @@
         try:
             df = pd.read_html(r.text)[0]
             df = df[df["model"].notna()]
             user_gear = list(zip(df.brand, df.model))
         except ValueError as e:
             user_gear = []
         return user_gear
+
+
+    def is_regional_admin(self, user: str) -> tuple:
+        """
+        Determines if a user is a regional admin and returns
+        the region they're an admin of (link and name)
+
+        Args:
+            user (str): Trailforks username
+
+        Returns:
+            tuple: ({region_link, region_name}, is_admin bool)
+        """
+        uri = f"https://www.trailforks.com/profile/{self.uri_encode(user)}/"
+        r = requests.get(uri)
+        try:
+            soup = BeautifulSoup(r.text, "html.parser")
+            col_5 = soup.find('div', {'class', 'col-5'})
+            region_link, region_name = re.search(
+                r'Admin</h4>.*<a href="(https.*)">([aA0-zZ9]+)</a>', 
+                str(col_5), 
+                re.DOTALL|re.MULTILINE
+                ).groups()
+            return ({"region_link": region_link, "region_name": region_name}, True)
+        except AttributeError:
+            return ({"region_link": "", "region_name": ""}, False)
+
```

### Comparing `PyForks-0.0.8/PyForks.egg-info/PKG-INFO` & `PyForks-0.0.9/PyForks.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 Metadata-Version: 2.1
 Name: PyForks
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package to interface with Trailforks.com
 Home-page: http://pypi.python.org/pypi/PyForks/
 Author: Trailforks Python Library
 Author-email: MinnMTB@gmail.com
 License: LICENSE.txt
 Project-URL: Bug Reports, https://github.com/cribdragg3r/PyForks/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Source, https://github.com/cribdragg3r/PyForks
 Project-URL: Documentation, https://pyforks.mn-mtb.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a href ="https://mn-mtb.com">
   <img src="./doc/PyForks.png"
-    title="PyForks" align="left" height=75 length=75 />
+    title="PyForks" align="left" height=100 length=100 />
     </a>
 
 
 # PyForks
 
 [![PyForks Tests](https://github.com/cribdragg3r/PyForks/actions/workflows/python-app.yml/badge.svg)](https://github.com/cribdragg3r/PyForks/actions/workflows/python-app.yml)
+[![GitHub](https://img.shields.io/github/license/cribdragg3r/PyForks?style=flat-square)](https://github.com/cribdragg3r/PyForks/blob/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/PyForks?style=flat-square)](https://pypi.org/project/PyForks/)
 
-Python Trailforks Library for interacting with Trailforks.com
+
+Python Trailforks Library for interacting with Trailforks.com. Help [support](https://github.com/sponsors/cribdragg3r) this project and more.
 
 ## About
 
-PyForks has been designed to help me automate much of the manual data aggregation I was doing in order to build metrics for my local city and state trail systems. For example: [wlmt.mn-mtb.com](http://wlmt.mn-mtb.com). The end goal of this project is the ability to make it much easier to pull data down that people are interested in and analyze it in a way that non-technical individuals can digest and understand impact in hopes of additional funding and intrest. 
+PyForks has been designed to help me automate much of the manual data aggregation I was doing in order to build metrics for my local city and state trail systems. For example: [wlmt.mn-mtb.com](http://wlmt.mn-mtb.com). The end goal of this project is the ability to make it much easier to pull data down that people are interested in and analyze it in a way that non-technical individuals can digest and understand impact in hopes of additional funding and interest. 
 
 ## Installation & Documentation
 
 - Install: `pip install pyforks`
 - Documentation: [PyForks.mn-mtb.com](https://PyForks.mn-mtb.com)
 
 ### Quick Start
@@ -40,23 +43,62 @@
 **Get Information on a User**
 
 ```python
 from PyForks.trailforks_user import TrailforksUser
 from pprint import pprint
 
 # Get Basic information about a user
-tf = TrailforksUser()
-user_info = tf.get_user_info("mnmtb")
+tf_u = TrailforksUser()
+user_info = tf_u.get_user_info("mnmtb")
 pprint(user_info)
 
 # Get the User's Gear
-tf.username = "<your_username>"
-tf.password = "<your_password>"
-tf.login()
-user_gear = tf.get_user_gear("mnmtb")
+tf_u.username = "<your_username>"
+tf_u.password = "<your_password>"
+tf_u.login()
+user_gear = tf_u.get_user_gear("mnmtb")
 pprint(user_gear)
+
+"""
+EXAMPLE OUTPUT:
+{
+  'admin_region': 
+    {
+    'region_link': 'https://www.trailforks.com/region/minnesota/',
+    'region_name': 'Minnesota'
+    },
+ 'city': 'Lakeville',
+ 'country': 'USA',
+ 'is_regional_admin': True,
+ 'profile_link': 'https://www.trailforks.com/profile/mnmtb',
+ 'recent_ride_locations': ['West Lake Marion Park',
+                           'Murphy-Hanrehan Park',
+                           'Lebanon Hills',
+                           'Spirit Mountain Bike Park',
+                           'Battle Creek',
+                           'Cottage Grove Bike Park',
+                           'Lakeville'],
+ 'state': 'Minnesota',
+ 'username': 'mnmtb'}
+ """
+```
+
+**Get Information on a region**
+```python
+from PyForks.trailforks_region import TrailforksRegion
+tf_r = TrailforksRegion(username=<username>, password=<password>)
+tf_r.login()
+
+# Download All of a regions trails in CSV:
+tf_r.download_all_region_trails(region, region_id)
+
+# Download all region ridelogs in csv
+tf_r.download_all_region_ridelogs(region)
+
+# Download all region ridecounts in CSV
+tf_r.download_region_ridecounts(region)
+
 ```
-  
 
 ## Contribute
 
 Send all the pull requests you want!
```

### Comparing `PyForks-0.0.8/setup.py` & `PyForks-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='PyForks',
-    version='0.0.8',
+    version='0.0.9',
     author='Trailforks Python Library',
     author_email='MinnMTB@gmail.com',
     packages=['PyForks', 'PyForks._test'],
     #scripts=['bin/script1','bin/script2'],
      project_urls={  # Optional
         "Bug Reports": "https://github.com/cribdragg3r/PyForks/issues",
         "Funding": "https://donate.pypi.org",
```

