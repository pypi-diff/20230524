# Comparing `tmp/jort-1.1.0.tar.gz` & `tmp/jort-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jort-1.1.0.tar", last modified: Mon May 22 22:33:07 2023, max compression
+gzip compressed data, was "jort-1.2.0.tar", last modified: Tue May 23 23:50:08 2023, max compression
```

## Comparing `jort-1.1.0.tar` & `jort-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-05-22 22:33:07.122125 jort-1.1.0/
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1070 2023-05-17 11:52:45.000000 jort-1.1.0/LICENSE
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     2317 2023-05-22 22:33:07.122125 jort-1.1.0/PKG-INFO
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1862 2023-05-22 22:30:52.000000 jort-1.1.0/README.md
-drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-05-22 22:33:07.114125 jort-1.1.0/jort/
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      232 2023-05-22 22:08:19.000000 jort-1.1.0/jort/__init__.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1872 2023-05-19 21:26:18.000000 jort-1.1.0/jort/checkpoint.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      242 2023-05-21 23:28:05.000000 jort-1.1.0/jort/config.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1330 2023-05-19 22:08:52.000000 jort-1.1.0/jort/datetime_utils.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     3978 2023-05-22 00:03:03.000000 jort-1.1.0/jort/jort_exe.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     2699 2023-05-21 23:34:09.000000 jort-1.1.0/jort/reporting_callbacks.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     5009 2023-05-20 03:41:44.000000 jort-1.1.0/jort/track_cli.py
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     5142 2023-05-22 22:27:25.000000 jort-1.1.0/jort/tracker.py
-drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-05-22 22:33:07.118125 jort-1.1.0/jort.egg-info/
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     2317 2023-05-22 22:33:06.000000 jort-1.1.0/jort.egg-info/PKG-INFO
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      349 2023-05-22 22:33:06.000000 jort-1.1.0/jort.egg-info/SOURCES.txt
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)        1 2023-05-22 22:33:06.000000 jort-1.1.0/jort.egg-info/dependency_links.txt
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       44 2023-05-22 22:33:06.000000 jort-1.1.0/jort.egg-info/entry_points.txt
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       98 2023-05-22 22:33:06.000000 jort-1.1.0/jort.egg-info/requires.txt
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)        5 2023-05-22 22:33:06.000000 jort-1.1.0/jort.egg-info/top_level.txt
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       38 2023-05-22 22:33:07.122125 jort-1.1.0/setup.cfg
--rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      953 2023-05-22 22:32:38.000000 jort-1.1.0/setup.py
+drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-05-23 23:50:08.263861 jort-1.2.0/
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1070 2023-05-17 11:52:45.000000 jort-1.2.0/LICENSE
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     2317 2023-05-23 23:50:08.263861 jort-1.2.0/PKG-INFO
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1862 2023-05-22 22:30:52.000000 jort-1.2.0/README.md
+drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-05-23 23:50:08.255861 jort-1.2.0/jort/
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      294 2023-05-23 01:49:41.000000 jort-1.2.0/jort/__init__.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1872 2023-05-19 21:26:18.000000 jort-1.2.0/jort/checkpoint.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      476 2023-05-23 23:19:43.000000 jort-1.2.0/jort/config.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     1330 2023-05-19 22:08:52.000000 jort-1.2.0/jort/datetime_utils.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      152 2023-05-23 01:48:58.000000 jort-1.2.0/jort/exceptions.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     4846 2023-05-23 23:32:29.000000 jort-1.2.0/jort/jort_exe.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     8013 2023-05-23 23:35:49.000000 jort-1.2.0/jort/reporting_callbacks.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     5019 2023-05-23 23:44:05.000000 jort-1.2.0/jort/track_cli.py
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     5228 2023-05-23 23:22:34.000000 jort-1.2.0/jort/tracker.py
+drwxrwxr-x   0 bryanb   (10072) bryanb   (10074)        0 2023-05-23 23:50:08.259861 jort-1.2.0/jort.egg-info/
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)     2317 2023-05-23 23:50:08.000000 jort-1.2.0/jort.egg-info/PKG-INFO
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      368 2023-05-23 23:50:08.000000 jort-1.2.0/jort.egg-info/SOURCES.txt
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)        1 2023-05-23 23:50:08.000000 jort-1.2.0/jort.egg-info/dependency_links.txt
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       44 2023-05-23 23:50:08.000000 jort-1.2.0/jort.egg-info/entry_points.txt
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       98 2023-05-23 23:50:08.000000 jort-1.2.0/jort.egg-info/requires.txt
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)        5 2023-05-23 23:50:08.000000 jort-1.2.0/jort.egg-info/top_level.txt
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)       38 2023-05-23 23:50:08.263861 jort-1.2.0/setup.cfg
+-rw-rw-r--   0 bryanb   (10072) bryanb   (10074)      953 2023-05-23 22:59:53.000000 jort-1.2.0/setup.py
```

### Comparing `jort-1.1.0/LICENSE` & `jort-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jort-1.1.0/PKG-INFO` & `jort-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jort
-Version: 1.1.0
+Version: 1.2.0
 Summary: Script profiler with checkpoints
 Home-page: https://github.com/bbrzycki/jort
 Author: Bryan Brzycki
 Author-email: bbrzycki@berkeley.edu
 Project-URL: Source, https://github.com/bbrzycki/jort
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jort-1.1.0/README.md` & `jort-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jort-1.1.0/jort/checkpoint.py` & `jort-1.2.0/jort/checkpoint.py`

 * *Files identical despite different names*

### Comparing `jort-1.1.0/jort/datetime_utils.py` & `jort-1.2.0/jort/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `jort-1.1.0/jort/jort_exe.py` & `jort-1.2.0/jort/jort_exe.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,14 +26,20 @@
         '-p',
         '--pid',
         nargs=1,
         type=int,
         help='PID of existing job to track',
     )
 
+    # Save stdout/stderr output
+    parser.add_argument('-o',
+                        '--output',
+                        action='store_true',
+                        help='save stdout/stderr output')
+
     # Send SMS at job completion
     parser.add_argument('-s',
                         '--sms',
                         action='store_true',
                         help='send SMS at job exit')
     
     # Send email at job completion
@@ -53,31 +59,38 @@
                         '--verbose',
                         action='store_true',
                         help='print payloads and all info')
 
     args = parser.parse_args()
 
     if args.init:
-        with open(f"{config.JORT_DIR}/config", "r") as f:
-            try:
-                config_data = json.load(f)
-            except json.decoder.JSONDecodeError:
-                config_data = {}
+        config_data = config.get_config_data()
         input_config_data = {
+            "machine": input('What name should this device go by? ({}) '
+                             .format(config_data.get("machine", ""))),
             "email": input('What email to use? ({}) '
-                           .format(config_data.get("email"))),
+                           .format(config_data.get("email", ""))),
+            "smtp_server": input('What SMTP server does your email use? ({}) '
+                                 .format(config_data.get("smtp_server", ""))),
+            "email_password": getpass.getpass('Email password? ({}) '
+                                              .format(("*"*16 
+                                                       if config_data.get("email_password", "") is not None 
+                                                       else ""))),
             "twilio_receive_number": input('What phone number to receive SMS? ({}) '
-                                           .format(config_data.get("twilio_receive_number"))),
+                                           .format(config_data.get("twilio_receive_number", ""))),
             "twilio_send_number": input('What Twilio number to send SMS? ({}) '
-                                        .format(config_data.get("twilio_send_number"))),
+                                        .format(config_data.get("twilio_send_number", ""))),
             "twilio_account_sid": input('Twilio Account SID? ({}) '
-                                        .format(config_data.get("twilio_account_sid"))),
+                                        .format(config_data.get("twilio_account_sid", ""))),
             "twilio_auth_token": getpass.getpass('Twilio Auth Token? ({}) '
-                                                 .format("*"*len(config_data.get("twilio_auth_token", "")))),
+                                                 .format(("*"*16 
+                                                         if config_data.get("twilio_auth_token", "") is not None 
+                                                         else "")))
         }
+        # Only save inputs if they aren't empty
         for key in input_config_data:
             if input_config_data[key] != "":
                 config_data[key] = input_config_data[key]
         with open(f"{config.JORT_DIR}/config", "w") as f:
             json.dump(config_data, f)
                 
     if args.command and args.pid:
@@ -86,15 +99,15 @@
         parser.print_help()
     elif args.command:
         # # Grab all aws credentials; either from file or interactively
         # aws_credentials = auth.login()
         joined_command = ' '.join(args.command)
         print(f"Tracking command '{joined_command}'")
         track_cli.track_new(joined_command,
-                            store_stdout=False,
+                            store_stdout=args.output,
                             save_filename=None,
                             send_sms=args.sms,
                             send_email=args.email,
                             verbose=args.verbose)
     elif args.pid:
         # # Grab all aws credentials; either from file or interactively
         # aws_credentials = auth.login()
```

### Comparing `jort-1.1.0/jort/track_cli.py` & `jort-1.2.0/jort/track_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -59,28 +59,27 @@
                      universal_newlines=True)
     print(f"Subprocess PID: {p.pid}\n")
 
     # Create stdout file
     if verbose:
         pprint(payload)
     if save_filename or store_stdout:
-        f = open(stdout_path, "a+")
-        f.write(f"$ {command}\n")
-        f.close()
+        with open(stdout_path, "a+") as f:
+            f.write(f"{command}\n")
+            f.write(f"--\n")
 
     buffer = ""
     temp_start = time.time()
     for line in p.stdout:
         if update_period > 0 and time.time() - temp_start >= update_period:
             if verbose:
                 print("Buffered! (Not sent)", [buffer])
             if save_filename or store_stdout:
-                f = open(stdout_path, "a+")
-                f.write(buffer)
-                f.close()
+                with open(stdout_path, "a+") as f:
+                    f.write(buffer)
 
             payload['status'] = 'running'
             datetime_utils.update_payload_times(payload)
             if verbose:
                 pprint(payload)
 
             buffer = ""
@@ -88,22 +87,23 @@
 
         sys.stdout.write(line)
         buffer += line
 
     if verbose:
         print("Buffered!", [buffer])
     if save_filename or store_stdout:
-        f = open(stdout_path, "a+")
-        f.write(buffer)
-        f.close()
+        with open(stdout_path, "a+") as f:
+            f.write(buffer)
+
+    p.wait()
 
     if verbose:
-        print("Exit code:", p.poll())
+        print(f"Exit code: {p.returncode}")
 
-    if p.returncode in [0, None]:
+    if p.returncode == 0:
         payload["status"] = "success"
     else:
         payload["status"] = "error"
         payload["error_message"] = line
     tr.stop(callbacks=callbacks)
 
     # print("")
```

### Comparing `jort-1.1.0/jort/tracker.py` & `jort-1.2.0/jort/tracker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import sys
 import time
 import logging
 import functools
 
+from . import config
 from . import checkpoint
 from . import datetime_utils
         
 
 class Tracker(object):
     def __init__(self, logname="tracker.log", verbose=0):
         """
         Create tracker object. Arguments give logging options; verbosity 0 for none, 
         1 for INFO, and 2 for DEBUG.
         """
         self.date_created = datetime_utils.get_iso_date()
+        self.machine = config.get_config_data().get("machine")
         self.checkpoints = {}
         self.open_checkpoint_payloads = {}
         self.logname = logname
         if verbose != 0:
             if verbose == 1:
                 level = logging.INFO
             else:
@@ -42,18 +44,18 @@
         else:
             start = datetime_utils.get_iso_date()
         now = datetime_utils.get_iso_date()
 
         self.open_checkpoint_payloads[name] = {
             "user_id": None,
             "job_id": None,
-            "short_name": name,
+            "name": name,
             "long_name": name,
             "status": "running",
-            "machine": None,
+            "machine": self.machine,
             "date_created": start,
             "date_modified": now,
             "runtime": datetime_utils.get_runtime(start, now),
             "stdout_fn": None,
             "unread": True,
             "error_message": None,
         }
```

### Comparing `jort-1.1.0/jort.egg-info/PKG-INFO` & `jort-1.2.0/jort.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jort
-Version: 1.1.0
+Version: 1.2.0
 Summary: Script profiler with checkpoints
 Home-page: https://github.com/bbrzycki/jort
 Author: Bryan Brzycki
 Author-email: bbrzycki@berkeley.edu
 Project-URL: Source, https://github.com/bbrzycki/jort
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jort-1.1.0/setup.py` & `jort-1.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-__version__ = '1.1.0'
+__version__ = '1.2.0'
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 entry_points = {
     'console_scripts': [
         'jort = jort.jort_exe:main'
```

