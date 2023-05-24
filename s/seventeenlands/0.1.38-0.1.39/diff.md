# Comparing `tmp/seventeenlands-0.1.38.tar.gz` & `tmp/seventeenlands-0.1.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seventeenlands-0.1.38.tar", last modified: Mon Nov 14 06:11:41 2022, max compression
+gzip compressed data, was "seventeenlands-0.1.39.tar", last modified: Wed May 24 15:03:46 2023, max compression
```

## Comparing `seventeenlands-0.1.38.tar` & `seventeenlands-0.1.39.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-11-14 06:11:41.902927 seventeenlands-0.1.38/
--rw-r--r--   0 rob       (1000) rob       (1000)    35149 2019-02-25 02:12:05.000000 seventeenlands-0.1.38/LICENSE
--rw-rw-r--   0 rob       (1000) rob       (1000)     1037 2022-11-14 06:11:41.902927 seventeenlands-0.1.38/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      585 2021-01-09 17:11:49.000000 seventeenlands-0.1.38/README.md
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2022-11-14 06:11:41.902927 seventeenlands-0.1.38/setup.cfg
--rw-rw-r--   0 rob       (1000) rob       (1000)      839 2022-11-14 06:10:33.000000 seventeenlands-0.1.38/setup.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-11-14 06:11:41.902927 seventeenlands-0.1.38/seventeenlands/
--rw-rw-r--   0 rob       (1000) rob       (1000)        0 2020-12-11 02:06:15.000000 seventeenlands-0.1.38/seventeenlands/__init__.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    48245 2022-11-14 06:09:44.000000 seventeenlands-0.1.38/seventeenlands/mtga_follower.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-11-14 06:11:41.902927 seventeenlands-0.1.38/seventeenlands.egg-info/
--rw-rw-r--   0 rob       (1000) rob       (1000)     1037 2022-11-14 06:11:41.000000 seventeenlands-0.1.38/seventeenlands.egg-info/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      315 2022-11-14 06:11:41.000000 seventeenlands-0.1.38/seventeenlands.egg-info/SOURCES.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-11-14 06:11:41.000000 seventeenlands-0.1.38/seventeenlands.egg-info/dependency_links.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       70 2022-11-14 06:11:41.000000 seventeenlands-0.1.38/seventeenlands.egg-info/entry_points.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       25 2022-11-14 06:11:41.000000 seventeenlands-0.1.38/seventeenlands.egg-info/requires.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       15 2022-11-14 06:11:41.000000 seventeenlands-0.1.38/seventeenlands.egg-info/top_level.txt
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-24 15:03:46.758864 seventeenlands-0.1.39/
+-rw-rw-r--   0 rob       (1000) rob       (1000)    35149 2023-05-24 15:00:01.000000 seventeenlands-0.1.39/LICENSE
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1037 2023-05-24 15:03:46.758864 seventeenlands-0.1.39/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      585 2023-05-24 15:00:01.000000 seventeenlands-0.1.39/README.md
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-24 15:03:46.758864 seventeenlands-0.1.39/setup.cfg
+-rw-rw-r--   0 rob       (1000) rob       (1000)      839 2023-05-24 15:03:39.000000 seventeenlands-0.1.39/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-24 15:03:46.758864 seventeenlands-0.1.39/seventeenlands/
+-rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-05-24 15:00:01.000000 seventeenlands-0.1.39/seventeenlands/__init__.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    48442 2023-05-24 15:02:09.000000 seventeenlands-0.1.39/seventeenlands/mtga_follower.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-24 15:03:46.758864 seventeenlands-0.1.39/seventeenlands.egg-info/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1037 2023-05-24 15:03:46.000000 seventeenlands-0.1.39/seventeenlands.egg-info/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      315 2023-05-24 15:03:46.000000 seventeenlands-0.1.39/seventeenlands.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-24 15:03:46.000000 seventeenlands-0.1.39/seventeenlands.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       70 2023-05-24 15:03:46.000000 seventeenlands-0.1.39/seventeenlands.egg-info/entry_points.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       25 2023-05-24 15:03:46.000000 seventeenlands-0.1.39/seventeenlands.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       15 2023-05-24 15:03:46.000000 seventeenlands-0.1.39/seventeenlands.egg-info/top_level.txt
```

### Comparing `seventeenlands-0.1.38/LICENSE` & `seventeenlands-0.1.39/LICENSE`

 * *Files identical despite different names*

### Comparing `seventeenlands-0.1.38/PKG-INFO` & `seventeenlands-0.1.39/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seventeenlands
-Version: 0.1.38
+Version: 0.1.39
 Summary: Utility to upload MTG Arena data to 17Lands.com
 Home-page: https://github.com/rconroy293/mtga-log-client
 Author: Robert Conroy
 Author-email: seventeenlands@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seventeenlands-0.1.38/README.md` & `seventeenlands-0.1.39/README.md`

 * *Files identical despite different names*

### Comparing `seventeenlands-0.1.38/setup.py` & `seventeenlands-0.1.39/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seventeenlands",
-    version="0.1.38",
+    version="0.1.39",
     author="Robert Conroy",
     author_email="seventeenlands@gmail.com",
     description="Utility to upload MTG Arena data to 17Lands.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rconroy293/mtga-log-client",
     packages=setuptools.find_packages(),
```

### Comparing `seventeenlands-0.1.38/seventeenlands/mtga_follower.py` & `seventeenlands-0.1.39/seventeenlands/mtga_follower.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 logger = logging.getLogger('17Lands')
 for handler in handlers:
     handler.setFormatter(log_formatter)
     logger.addHandler(handler)
 logger.setLevel(logging.INFO)
 logger.info(f'Saving logs to {LOG_FILENAME}')
 
-CLIENT_VERSION = '0.1.38.p'
+CLIENT_VERSION = '0.1.39.p'
 
 UPDATE_CHECK_INTERVAL = datetime.timedelta(hours=1)
 UPDATE_PROMPT_FREQUENCY = 24
 
 TOKEN_ENTRY_TITLE = 'MTGA Log Client Token'
 TOKEN_ENTRY_MESSAGE = 'Please enter your client token from 17lands.com/account: '
 TOKEN_MISSING_TITLE = 'Error: Client Token Needed'
@@ -86,15 +86,15 @@
 )
 
 POSSIBLE_CURRENT_FILEPATHS = list(map(lambda root_and_path: os.path.join(*root_and_path), itertools.product(POSSIBLE_ROOTS, (CURRENT_LOG_PATH, ))))
 POSSIBLE_PREVIOUS_FILEPATHS = list(map(lambda root_and_path: os.path.join(*root_and_path), itertools.product(POSSIBLE_ROOTS, (PREVIOUS_LOG_PATH, ))))
 
 CONFIG_FILE = os.path.join(os.path.expanduser('~'), '.mtga_follower.ini')
 
-LOG_START_REGEX_TIMED = re.compile(r'^\[(UnityCrossThreadLogger|Client GRE)\]([\d:/ .-]+(AM|PM)?)')
+LOG_START_REGEX_TIMED = re.compile(r'^\[(UnityCrossThreadLogger|Client GRE)\](\d[\d:/ .-]+(AM|PM)?)')
 LOG_START_REGEX_UNTIMED = re.compile(r'^\[(UnityCrossThreadLogger|Client GRE)\]')
 TIMESTAMP_REGEX = re.compile('^([\\d/.-]+[ T][\\d]+:[\\d]+:[\\d]+( AM| PM)?)')
 STRIPPED_TIMESTAMP_REGEX = re.compile('^(.*?)[: /]*$')
 JSON_START_REGEX = re.compile(r'[\[\{]')
 ACCOUNT_INFO_REGEX = re.compile(r'.*Updated account\. DisplayName:(.*), AccountID:(.*), Token:.*')
 MATCH_ACCOUNT_INFO_REGEX = re.compile(r'.*: ((\w+) to Match|Match to (\w+)):')
 SLEEP_TIME = 0.5
@@ -1138,32 +1138,37 @@
         logger.warning("Found no files to parse. Try to find Arena's Player.log file and pass it as an argument with -l")
 
     logger.info(f'Exiting')
 
 
 def main():
     parser = argparse.ArgumentParser(description='MTGA log follower')
+
+    config_token = get_config()
+
     parser.add_argument('-l', '--log_file',
         help=f'Log filename to process. If not specified, will try one of {POSSIBLE_CURRENT_FILEPATHS}')
     parser.add_argument('--host', default=API_ENDPOINT,
         help=f'Host to submit requests to. If not specified, will use {API_ENDPOINT}')
+    parser.add_argument('--token', default=config_token,
+                        help=f'Token of the user. If not specified, will use the token at {CONFIG_FILE}')
     parser.add_argument('--once', action='store_true',
         help='Whether to stop after parsing the file once (default is to continue waiting for updates to the file)')
 
     args = parser.parse_args()
 
     check_count = 0
     while not verify_version(
         host=args.host,
         prompt_if_update_required=check_count % UPDATE_PROMPT_FREQUENCY == 0,
     ):
         check_count += 1
         time.sleep(UPDATE_CHECK_INTERVAL.total_seconds())
 
-    token = get_config()
+    token = args.token
     logger.info(f'Using token {token[:4]}...{token[-4:]}')
 
     processing_loop(args, token)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `seventeenlands-0.1.38/seventeenlands.egg-info/PKG-INFO` & `seventeenlands-0.1.39/seventeenlands.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seventeenlands
-Version: 0.1.38
+Version: 0.1.39
 Summary: Utility to upload MTG Arena data to 17Lands.com
 Home-page: https://github.com/rconroy293/mtga-log-client
 Author: Robert Conroy
 Author-email: seventeenlands@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

