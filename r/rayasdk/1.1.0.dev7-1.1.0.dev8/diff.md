# Comparing `tmp/rayasdk-1.1.0.dev7.tar.gz` & `tmp/rayasdk-1.1.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rayasdk-1.1.0.dev7.tar", last modified: Thu May 18 19:52:12 2023, max compression
+gzip compressed data, was "rayasdk-1.1.0.dev8.tar", last modified: Wed May 24 18:48:06 2023, max compression
```

## Comparing `rayasdk-1.1.0.dev7.tar` & `rayasdk-1.1.0.dev8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 19:52:12.813964 rayasdk-1.1.0.dev7/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     6569 2023-05-18 19:52:12.813964 rayasdk-1.1.0.dev7/PKG-INFO
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     6219 2023-05-11 21:39:47.000000 rayasdk-1.1.0.dev7/README.md
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 19:52:12.813964 rayasdk-1.1.0.dev7/rayasdk/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      546 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev7/rayasdk/__init__.py
--rwxrwxr-x   0 camilo    (1000) camilo    (1000)     4901 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/__main__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     5407 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/connect.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     3381 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/constants.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 19:52:12.813964 rayasdk-1.1.0.dev7/rayasdk/container_handlers/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev7/rayasdk/container_handlers/__init__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     7391 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/container_handlers/docker_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2787 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/initializer.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1439 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/killer.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1513 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev7/rayasdk/logger.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      819 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev7/rayasdk/messages.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     6355 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/runner.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     4398 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/scanner.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     5413 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/simulator.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2657 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/sshKeyGen.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 19:52:12.813964 rayasdk-1.1.0.dev7/rayasdk/template/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      244 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev7/rayasdk/template/__main__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      551 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev7/rayasdk/template/app.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      399 2023-04-17 17:27:42.000000 rayasdk-1.1.0.dev7/rayasdk/template/launch.json
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      108 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev7/rayasdk/template/manifest.json
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1775 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/utils.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)    10212 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/vcs.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 19:52:12.813964 rayasdk-1.1.0.dev7/rayasdk.egg-info/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     6569 2023-05-18 19:52:12.000000 rayasdk-1.1.0.dev7/rayasdk.egg-info/PKG-INFO
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      683 2023-05-18 19:52:12.000000 rayasdk-1.1.0.dev7/rayasdk.egg-info/SOURCES.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        1 2023-05-18 19:52:12.000000 rayasdk-1.1.0.dev7/rayasdk.egg-info/dependency_links.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       51 2023-05-18 19:52:12.000000 rayasdk-1.1.0.dev7/rayasdk.egg-info/entry_points.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      103 2023-05-18 19:52:12.000000 rayasdk-1.1.0.dev7/rayasdk.egg-info/requires.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        8 2023-05-18 19:52:12.000000 rayasdk-1.1.0.dev7/rayasdk.egg-info/top_level.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       79 2023-05-18 19:52:12.813964 rayasdk-1.1.0.dev7/setup.cfg
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1101 2023-05-18 19:50:57.000000 rayasdk-1.1.0.dev7/setup.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-24 18:48:06.605626 rayasdk-1.1.0.dev8/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6569 2023-05-24 18:48:06.605626 rayasdk-1.1.0.dev8/PKG-INFO
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6219 2023-05-11 21:39:47.000000 rayasdk-1.1.0.dev8/README.md
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-24 18:48:06.605626 rayasdk-1.1.0.dev8/rayasdk/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      546 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev8/rayasdk/__init__.py
+-rwxrwxr-x   0 camilo    (1000) camilo    (1000)     5077 2023-05-23 18:09:34.000000 rayasdk-1.1.0.dev8/rayasdk/__main__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     5324 2023-05-23 18:09:34.000000 rayasdk-1.1.0.dev8/rayasdk/connect.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     3381 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev8/rayasdk/constants.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-24 18:48:06.605626 rayasdk-1.1.0.dev8/rayasdk/container_handlers/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev8/rayasdk/container_handlers/__init__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     7391 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev8/rayasdk/container_handlers/docker_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2787 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev8/rayasdk/initializer.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1439 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev8/rayasdk/killer.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     4123 2023-05-23 18:09:34.000000 rayasdk-1.1.0.dev8/rayasdk/logger.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1235 2023-05-23 18:09:34.000000 rayasdk-1.1.0.dev8/rayasdk/messages.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6664 2023-05-23 18:10:01.000000 rayasdk-1.1.0.dev8/rayasdk/runner.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     4354 2023-05-23 18:09:34.000000 rayasdk-1.1.0.dev8/rayasdk/scanner.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     5536 2023-05-23 18:09:34.000000 rayasdk-1.1.0.dev8/rayasdk/simulator.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2657 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev8/rayasdk/sshKeyGen.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-24 18:48:06.605626 rayasdk-1.1.0.dev8/rayasdk/template/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      244 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev8/rayasdk/template/__main__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      551 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev8/rayasdk/template/app.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      399 2023-04-17 17:27:42.000000 rayasdk-1.1.0.dev8/rayasdk/template/launch.json
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      108 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev8/rayasdk/template/manifest.json
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1775 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev8/rayasdk/utils.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)    11638 2023-05-23 18:09:34.000000 rayasdk-1.1.0.dev8/rayasdk/vcs.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-24 18:48:06.605626 rayasdk-1.1.0.dev8/rayasdk.egg-info/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6569 2023-05-24 18:48:06.000000 rayasdk-1.1.0.dev8/rayasdk.egg-info/PKG-INFO
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      683 2023-05-24 18:48:06.000000 rayasdk-1.1.0.dev8/rayasdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        1 2023-05-24 18:48:06.000000 rayasdk-1.1.0.dev8/rayasdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       51 2023-05-24 18:48:06.000000 rayasdk-1.1.0.dev8/rayasdk.egg-info/entry_points.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      103 2023-05-24 18:48:06.000000 rayasdk-1.1.0.dev8/rayasdk.egg-info/requires.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        8 2023-05-24 18:48:06.000000 rayasdk-1.1.0.dev8/rayasdk.egg-info/top_level.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       79 2023-05-24 18:48:06.605626 rayasdk-1.1.0.dev8/setup.cfg
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1101 2023-05-24 18:47:19.000000 rayasdk-1.1.0.dev8/setup.py
```

### Comparing `rayasdk-1.1.0.dev7/PKG-INFO` & `rayasdk-1.1.0.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayasdk
-Version: 1.1.0.dev7
+Version: 1.1.0.dev8
 Summary: Raya SDK - Unlimited Robotics Software Development Kit
 Home-page: UNKNOWN
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: MIT
 Keywords: robotics,unlimited-robotics,gary
 Platform: UNKNOWN
```

### Comparing `rayasdk-1.1.0.dev7/README.md` & `rayasdk-1.1.0.dev8/README.md`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev7/rayasdk/__init__.py` & `rayasdk-1.1.0.dev8/rayasdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev7/rayasdk/__main__.py` & `rayasdk-1.1.0.dev8/rayasdk/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import platform
 import subprocess
 
 import rayasdk.constants as constants
 from rayasdk.connect import URConnect
 from rayasdk.vcs import URVCS, check_simulation_versions, check_sdk_version
 from rayasdk.logger import log_error, log_verbose, log_info, set_logger_level
+from rayasdk.logger import log_success
 from rayasdk.scanner import URScanner
 from rayasdk.initializer import URInitializer
 from rayasdk.runner import URRunner
 from rayasdk.simulator import URSimulator
 from rayasdk.killer import URKiller
 
 
@@ -71,20 +72,24 @@
             os.makedirs(constants.SIMS_APPS, exist_ok=True)
             os.makedirs(constants.SIMS_DATA_APPS, exist_ok=True)
             os.makedirs(constants.SIMS_DATA_APPS_DEVEL, exist_ok=True)
             # if ur_root not exist or is empty clone it
             if not os.path.exists(constants.RAYAENV_DOCKER_UR_ROOT) or len(
                     os.listdir(constants.RAYAENV_DOCKER_UR_ROOT)) == 0:
                 log_info('Preparing UR user folder...')
-                subprocess.call(
+                clone_repo = subprocess.Popen(
                         args=constants.RAYAENV_DOCKER_UR_ROOT_REPO,
                         shell=True,
                         stderr=subprocess.PIPE
                     )
-                log_info('Done')
+                if clone_repo.returncode == 0:
+                    log_success('Done')
+                else:
+                    _, err = clone_repo.communicate()
+                    log_error(err.decode("utf-8"))
 
         except OSError as exc:
             log_error(exc)
             return False
         return True
 
     def init_ursdk_folder(self):
@@ -101,18 +106,18 @@
             log_verbose(f'Folder {constants.URSDK_TEMP_PATH} found.')
             return True
 
     def run(self):
         try:
             # Check if sdk have an update
             check_sdk_version()
-            # Check simulation version on simulator and update command
+            # Check simulation version on simulator command
             if self.args.command == URSimulator().COMMAND:
                 updated = check_simulation_versions()
-                if not updated and self.args.command == URSimulator().COMMAND:
+                if not updated:
                     log_error('RayaOS is not up to date. To update run "rayasdk update"')
                     return False
             # Execute Command
             for obj in self.command_objects:
                 if self.args.command == type(obj).COMMAND:
                     return obj.run(self.args, self.unknownargs)
         except Exception as e:
```

### Comparing `rayasdk-1.1.0.dev7/rayasdk/connect.py` & `rayasdk-1.1.0.dev8/rayasdk/connect.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,28 +88,26 @@
                 # Send ssh key to robot
                 SshKeyGen(user=constants.SSH_USER,
                           host=robot_connection[constants.JSON_EXECINFO_ROBIP],
                           port=constants.SSH_PORT)
                 log_info(f'You have successfully connected to '
                          f'{robot_connection[constants.JSON_EXECINFO_ROBID]}')
 
+            
             # Save connection globally
             with open(constants.CONNECTION_SETTINGS_PATH, 'w', encoding='utf-8') as f:
                 settings = dict()
                 settings[constants.JSON_EXECINFO_SIM] = exec_settings[constants.JSON_EXECINFO_SIM]
                 settings[constants.JSON_EXECINFO_ROBCONN] = exec_settings[
                     constants.JSON_EXECINFO_ROBCONN]
                 json.dump(settings, f, ensure_ascii=False, indent=4)
 
         except FileNotFoundError:
-            raise Exception(
-                f'Could not write file "{constants.CONNECTION_SETTINGS_FILE}".')
-        except OSError:
-            raise Exception((f'Could not get scanning info, '
-                             'execute "rayasdk scan" before this command.'))
+            raise Exception((f'Last scan was empty or wasn\'t executed, '
+                             'execute "rayasdk scan" and check if the robot is appears in the scan.'))
         except subprocess.SubprocessError:
             raise Exception("SSH Key not send, Check if raya_os is running")
         except NameError as error:
             raise Exception(str(error))
         except KeyError as error:
             log_info(error)
             raise Exception((f'Scanning info malformed, '
```

### Comparing `rayasdk-1.1.0.dev7/rayasdk/constants.py` & `rayasdk-1.1.0.dev8/rayasdk/constants.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev7/rayasdk/container_handlers/docker_handler.py` & `rayasdk-1.1.0.dev8/rayasdk/container_handlers/docker_handler.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev7/rayasdk/initializer.py` & `rayasdk-1.1.0.dev8/rayasdk/initializer.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev7/rayasdk/killer.py` & `rayasdk-1.1.0.dev8/rayasdk/killer.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev7/rayasdk/messages.py` & `rayasdk-1.1.0.dev8/rayasdk/messages.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,7 +14,25 @@
 MSG_FULL_UPDATE = ('\nWe have a new version of RayaOS available\n'
                    'Would you like to update?[Y/n]\n')
 
 MSG_MINOR_UPDATE = (f'\nRayaOS found a minor version change\n'
                     'Would you like to update?[Y/n]\n')
 
 MSG_NO_UPDATES = ('It seems there are no updates available\n')
+
+MSG_NO_VCS = ('Could get VCS')
+
+# runner
+MSG_LAUNCHING_APP = ('Launching app...')
+
+MSG_SYNC_APP_SIM = ('Syncing the app on the simulation...')
+
+MSG_SYNC_APP_ROBOT = ('Syncing the app on the host')
+
+MSG_WAIT_DEBUG_CLIENT = ('Waiting for debug client (VSCode)...')
+
+MSG_APP_FINISHED = ('App finished')
+
+# simulator 
+MSG_RAYA_OS_IMAGE = ('Opening RayaOS image...')
+
+MSG_UNITY_SIM = ('Opening Raya unity simulator...')
```

### Comparing `rayasdk-1.1.0.dev7/rayasdk/runner.py` & `rayasdk-1.1.0.dev8/rayasdk/runner.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import json
 import subprocess
 import os
 from pathlib import Path
 
 import rayasdk.constants as constants
-from rayasdk.logger import log_error, log_info, log_warning
+from rayasdk.messages import *
+from rayasdk.logger import log_error, log_info, log_warning, log_status
 from rayasdk.utils import open_connection_file, validate_app_id_and_folder_name
 from rayasdk.container_handlers.docker_handler import DockerHandler
 
 
 class URRunner:
 
     COMMAND = 'run'
@@ -64,62 +65,66 @@
         return True
 
     def run_app_on_simulation(self, exec_settings, connection_settings):
         app_id = exec_settings[constants.JSON_EXECINFO_APPID]
         origin_path = os.getcwd()
 
         # Sync the app in the folder of the simulation
+        log_status(MSG_SYNC_APP_SIM)
         command = \
             f'rsync --archive --delete {origin_path}/ {constants.SIMS_APPS}/{app_id}'
         subprocess.call(command, shell=True)
 
         if self.args.debug:
-            log_info('Waiting for debug client (VSCode)...')
+            log_status(MSG_WAIT_DEBUG_CLIENT)
 
+        log_status(MSG_LAUNCHING_APP)
         self.docker_handler.launch_app_on_sim(
                 app_id=app_id,
                 args=self.unknownargs,
                 debug=self.args.debug
             )
+        log_status(MSG_APP_FINISHED)
 
     def run_app_on_remote(self, exec_settings, connection_settings):
         app_id = exec_settings[constants.JSON_EXECINFO_APPID]
         robot_id = connection_settings[constants.JSON_EXECINFO_ROBCONN]\
                                                         [constants.JSON_EXECINFO_ROBID]
         host = connection_settings[constants.JSON_EXECINFO_ROBCONN][constants.JSON_EXECINFO_ROBIP]
         hostname = f'{constants.SSH_USER}@{host}'
-
+        log_status(f'{MSG_SYNC_APP_ROBOT} \'{hostname}\'...')
+        
         while True:
             try:
                 origin_path = os.getcwd()
                 command = (('rsync '
                             '--archive '
                             '--delete '
                             f'--rsh=\'ssh -p{constants.SSH_PORT}\' '
                             f'{origin_path}/ '
                             f'{hostname}:{constants.SSH_APP_FOLDER}/{app_id}'))
                 subprocess.run(command, shell=True,
                                capture_output=True).check_returncode()
 
             except subprocess.CalledProcessError as e:
                 if 'REMOTE HOST IDENTIFICATION HAS CHANGED' in str(e.stderr):
-                    log_info()
+                    log_info('')
                     log_warning(
                         ('Host ID have changed, run \'rayasdk connect\' '
                          'again'))
                     command = (('ssh-keygen '
                                 f'-f "{Path.home()/".ssh"/"known_hosts"}" '
                                 f'-R "[{host}]:{constants.SSH_PORT}"'))
                     subprocess.run(
                         command,
                         shell=True,
                         stdout=subprocess.DEVNULL,
                         stderr=subprocess.DEVNULL).check_returncode()
                     return
-                log_info()
+                log_info('')
                 log_error('Can not send the app to the robot')
                 if 'No route to host' in str(e.stderr):
                     log_info(('No toute to host. Check that the robot is powered'
                            ' on'))
                 elif 'Connection refused' in str(e.stderr):
                     log_info(
                         ('Connection refused. Check that the Ra-Ya system is '
@@ -128,16 +133,18 @@
                     log_info('Check that the robot is powered on')
                 log_info(f'Trying to connect to: {robot_id} / {host}')
                 return
 
             except Exception as error:
                 log_error(error)
                 return
-
+            
+            log_status(MSG_LAUNCHING_APP)
             self.launch_app(app_id, hostname, self.unknownargs)
+            log_status(MSG_APP_FINISHED)
             return
 
     def launch_app(self, app_id, host_url, args):
         execution_route = f'%s%s' % (constants.SSH_APP_FOLDER, app_id)
 
         if self.args.debug:
             cmd = (f'python3 -m debugpy --listen 5678 --wait-for-client '
```

### Comparing `rayasdk-1.1.0.dev7/rayasdk/scanner.py` & `rayasdk-1.1.0.dev8/rayasdk/scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     def run(self, args, unknownargs):
         self.args = args
         self.unknownargs = unknownargs
         zeroconf = Zeroconf()
         listener = MyListener(print=True)
         ServiceBrowser(Zeroconf(), '_gary-robot._tcp.local.', listener)
         try:
+            update_table()
             while True:
                 if select.select([
                         sys.stdin,
                 ], [], [], 0.0)[0]:
                     input_str = sys.stdin.readline().strip()
                     if input_str == '':
                         break
@@ -111,28 +112,25 @@
         if self.print:
             update_table()
 
 
 def update_table():
     global robots_info
     # Screen out all the robot found in scan
+    list_robots = []
     if len(robots_info) > 0:
         clear()
-        list_robots = []
         for robot in list(robots_info.items()):
             for address in list(robot[1].items()):
                 list_robots.append(address[1].values())
-
-        log_info('Press enter to exit...\n')
-        log_info(
-            tabulate(list_robots, headers=['Robot ID', 'Serial',
-                                           'IP Address']))
-        log_info('')
-    else:
-        log_info('No robots found.')
+    log_info('Press enter to exit...\n')
+    log_info(
+        tabulate(list_robots, headers=['Robot ID', 'Serial',
+                                        'IP Address']))
+    log_info('')
 
 
 def clear():
     # for windows
     if name == 'nt':
         _ = system('cls')
```

### Comparing `rayasdk-1.1.0.dev7/rayasdk/simulator.py` & `rayasdk-1.1.0.dev8/rayasdk/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 import re
 
 from simple_file_checksum import get_checksum
 from time import sleep
 from pathlib import Path
 
 import rayasdk.constants as constants
+from rayasdk.messages import *
 from rayasdk.utils import run_simulator_bridge, MyProgressBar
-from rayasdk.logger import log_error, log_info
+from rayasdk.logger import log_error, log_info, log_status
 
 
 class URSimulator:
 
     COMMAND = 'simulator'
 
     def __init__(self):
@@ -78,22 +79,24 @@
             log_error('Simulator not found, run rayasdk update to download it')
             return False
 
         # If debug flag not set run container
         container_process = None
         if not self.args.debug:
             try:
+                log_status(MSG_RAYA_OS_IMAGE)
                 container_process = run_simulator_bridge()
                 if type(container_process) == bool:
                     return False
                 sleep(5)
             except KeyboardInterrupt:
                 pass
 
         # Run unity simulation
+        log_status(MSG_UNITY_SIM)
         simulator_process = subprocess.Popen([str(self.SIM_BINARY)] +
                                              self.unknownargs,
                                              stdout=subprocess.PIPE)
 
         if container_process is not None:
             while True:
                 if container_process.poll() is not None:
```

### Comparing `rayasdk-1.1.0.dev7/rayasdk/sshKeyGen.py` & `rayasdk-1.1.0.dev8/rayasdk/sshKeyGen.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev7/rayasdk/template/app.py` & `rayasdk-1.1.0.dev8/rayasdk/template/app.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev7/rayasdk/utils.py` & `rayasdk-1.1.0.dev8/rayasdk/utils.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev7/rayasdk/vcs.py` & `rayasdk-1.1.0.dev8/rayasdk/vcs.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,46 +6,52 @@
 from rayasdk.logger import log_error, log_info, log_success, log_warning
 from rayasdk.messages import *
 from rayasdk.container_handlers.docker_handler import DockerHandler
 from rayasdk.simulator import URSimulator
 
 
 def check_simulation_versions():
-    vcs = URVCS()
-    # If there is a patch update available, update
-    if not vcs.patch_updated():
-        for raya_component in constants.RAYA_OS_COMPONENTS:
-            # Do not check SDK
-            if raya_component == 'SDK':
-                continue
-            if not vcs.patch_updated(raya_component):
-                log_info(f'Updating {raya_component}')
-                if not vcs.update_patch(raya_component):
-                    log_error(f'Could not update {raya_component}')
+    try:
+        vcs = URVCS()
+        # If there is a patch update available, update
+        if not vcs.patch_updated():
+            for raya_component in constants.RAYA_OS_COMPONENTS:
+                # Do not check SDK
+                if raya_component == 'SDK':
+                    continue
+                if not vcs.patch_updated(raya_component, show_msg=False):
+                    log_info(f'Updating {raya_component}')
+                    if not vcs.update_patch(raya_component):
+                        log_error(f'Could not update {raya_component}')
+                        return False
+                    log_info('Run the command again')
                     return False
-                log_info('Run the command again')
-                return False
-        log_info("All components are up to date.")
-    # If there is a major/minor version let the user know
-    if not vcs.full_updated() or not vcs.minor_updated():
-        return False
-    else:
+            log_info("All components are up to date.")
+        # If there is a major/minor version let the user know
+        if not vcs.full_updated() or not vcs.minor_updated():
+            return False
+        else:
+            return True
+    except requests.exceptions.ConnectionError:
         return True
 
 
 def check_sdk_version():
-    vcs = URVCS()
-    component='SDK'
-    if not vcs.full_updated(component=component) or not vcs.minor_updated(component=component):
-        latest = vcs.get_latest_version(component=component)
-        log_warning((
-                'RayaSDK is not up to date. To update run '
-                f'\'pip install rayasdk=={latest}\''
-            ))
-    return True
+    try:
+        vcs = URVCS()
+        component='SDK'
+        if not vcs.full_updated(component=component) or not vcs.minor_updated(component=component):
+            latest = vcs.get_latest_version(component=component)
+            log_warning((
+                    'RayaSDK is not up to date. To update run '
+                    f'\'pip install rayasdk=={latest}\''
+                ))
+        return True
+    except requests.exceptions.ConnectionError:
+        return True
 
 
 class URVCS:
 
     COMMAND = 'update'
 
     def __init__(self):
@@ -57,48 +63,50 @@
 
 
     def init_parser(self, subparser):
         self.parser = subparser.add_parser(
             type(self).COMMAND, help='Update the SDK, Unity or Docker')
     
     
-    
-
-
     def run(self, args, unknownargs):
         self.args = args
         self.unknownargs = unknownargs
         log_info('Checking for updates...')
-        
-        if not self.full_updated() or self.simulator.simulator_not_found() or self.docker_handler.RayaOS_not_found():
-            download_input = input(f'Do you want to download the Simulator and RayaOS? [Y/n]')
-            if download_input not in ['y', 'Y', 'yes', 'Yes', 'YES', '']:
-                return False
-        
-        if self.update_full():
+        try:
+            if not self.full_updated() or not self.minor_updated() or not self.patch_updated() or self.simulator.simulator_not_found() or self.docker_handler.RayaOS_not_found():
+                download_input = input(f'Do you want to download the Simulator and/or RayaOS? [Y/n]')
+                if download_input not in ['y', 'Y', 'yes', 'Yes', 'YES', '']:
+                    return False
+                if not self.update_full():
+                    log_error('Update failed.')
+                    return False
             log_success('Everything is up to date')
             return True
-        else:
-            log_error('Update failed.')
+        except requests.exceptions.ConnectionError:
+            log_error('There was a Connection Error, The Version Control System does not respond.')
             return False
 
 
     def __get_major(self, version):
         return int(version.split('.')[0])
 
 
     def __get_minor(self, version):
         return int(version.split('.')[1])
 
 
     def __get_patch(self, version):
-        patch = version.split('.')[2]
-        if patch:
-            return str(patch)
-        return '0'
+        try:
+            patch = version.split('.')[2]
+            if patch:
+                patch_version = str(patch)
+                patch_version = re.findall(r'^(\d+)', patch_version)[0]
+                return patch_version 
+        except:
+            return '0'
 
 
     def __local_version(self, component):
         '''
         Return the local version of the component
         '''
         if component == 'SDK':
@@ -114,150 +122,168 @@
 
     def __get_latest_version(self, component):
         '''
         Return the latest version of the component
         '''
         # response = requests.request("GET", f'{VCS_URL}/latest/{component}')
         # return(data['versionId'])
-        response = requests.request("GET", f'{constants.VCS_URL}')
-        data = response.json()
-        for raya_component in data:
+        response = self.get_VCS_json(type_version='latest', component=component)
+        for raya_component in response:
             if raya_component['name'] == component:
                 return raya_component['versionId']
        
             
-    def full_updated(self, component=None):
+    def full_updated(self, component=None, show_msg= True):
         if component:
             local = self.__local_version(component)
             latest = self.__get_latest_version(component)
             diff_major = self.__get_major(latest) > self.__get_major(local)
             if diff_major:
-                log_warning((f'{component} have a major update, '
-                        f'current: \'{local}\' -> latest: \'{latest}\''))
+                if show_msg:
+                    log_warning((f'{component} have a major update, '
+                            f'current: \'{local}\' -> latest: \'{latest}\''))
                 return False
             else:
                 return True
         
         updated = True
         for raya_component in constants.RAYA_OS_COMPONENTS:
             local = self.__local_version(raya_component)
             latest = self.__get_latest_version(raya_component)
             diff_major = self.__get_major(latest) > self.__get_major(local)
             if diff_major:
-                log_warning((f'{raya_component} have a major update, '
-                        f'current: \'{local}\' -> latest: \'{latest}\''))
+                if show_msg:
+                    log_warning((f'{raya_component} have a major update, '
+                            f'current: \'{local}\' -> latest: \'{latest}\''))
                 updated = False
         return updated
 
 
     def update_full(self):
         # Update Unity
         if self.__get_latest_version('Unity') != self.__local_version(
                 'Unity') or self.simulator.simulator_not_found():
-            response = requests.request("GET", constants.VCS_URL)
-            if not self.simulator.download_simulator(response=response.json()):
+            response = self.get_VCS_json(type_version='latest', component='Unity')
+            if not self.simulator.download_simulator(response=response):
                 return False
             log_success('Simulator updated successfully')
 
         # Update Docker
         if self.__get_latest_version('Docker') != self.__local_version(
                 'Docker') or self.docker_handler.RayaOS_not_found():
             version = self.__get_latest_version('Docker')
             if not self.docker_handler.download_raya_image(version):
                 return False
             log_success('Raya_OS updated successfully')
 
         return True
 
 
-    def minor_updated(self, component=None):
+    def minor_updated(self, component=None, show_msg= True):
         '''Function to check if the latest version is a minor version'''
         if component:
             local = self.__local_version(component)
             latest = self.__get_latest_version(component)
             same_major = self.__get_major(latest) == self.__get_major(local)
             diff_minor = self.__get_minor(latest) > self.__get_minor(local)
             if same_major and diff_minor:
-                log_warning((f'{component} have a minor update, '
-                        f'current: \'{local}\' -> latest: \'{latest}\''))
+                if show_msg:
+                    log_warning((f'{component} have a minor update, '
+                            f'current: \'{local}\' -> latest: \'{latest}\''))
                 return False
             else:
                 return True
         
         updated = True
         for raya_component in constants.RAYA_OS_COMPONENTS:
             local = self.__local_version(raya_component)
             latest = self.__get_latest_version(raya_component)
             same_major = self.__get_major(latest) == self.__get_major(local)
             diff_minor = self.__get_minor(latest) > self.__get_minor(local)
             if same_major and diff_minor:
-                log_warning((f'{raya_component} have a minor update, '
-                        f'current: \'{local}\' -> latest: \'{latest}\''))
+                if show_msg:
+                    log_warning((f'{raya_component} have a minor update, '
+                            f'current: \'{local}\' -> latest: \'{latest}\''))
                 updated = False
         return updated
 
 
     def update_minor(self, component):
         download_input = input(f'Do you want to download the Simulator and the Docker Image? [Y/n]\'')
         if download_input not in ['y', 'Y', 'yes', 'Yes', 'YES', '']:
             return False
         
         '''Update the component and return True if the update was successful'''
         if component == 'Unity':
-            response = requests.request("GET", constants.VCS_URL)
+            response = self.get_VCS_json(type_version='minor', component='Unity')
             version = self.__get_latest_version(component)
-            if self.simulator.download_simulator(response=response.json()):
+            if self.simulator.download_simulator(response=response):
                 return True
         elif component == 'Docker':
             version = self.__get_latest_version(component)
             if self.docker_handler.download_raya_image(version):
                 return True
         return False
 
 
-    def patch_updated(self, component=None):
+    def patch_updated(self, component=None, show_msg= True):
         '''Function to check if the latest version is a patch'''
         if component:
             local = self.__local_version(component)
             latest = self.__get_latest_version(component)
             same_major = self.__get_major(latest) == self.__get_major(local)
             same_minor = self.__get_minor(latest) == self.__get_minor(local)
-            diff_patch = self.__get_patch(local) != self.__get_patch(latest)
+            diff_patch = self.__get_patch(local) < self.__get_patch(latest)
             if same_major and same_minor and diff_patch:
-                log_warning(
-                    (f'{component} have an patch update it is going to be'
-                     f' updated to version \'{latest}\', current \'{local}\''))
+                if show_msg:
+                    log_warning(
+                        (f'{component} have an patch update it is going to be'
+                        f' updated to version \'{latest}\', '
+                        f'current \'{local}\''))
                 return False
             else:
                 return True
 
         updated = True
         for raya_component in constants.RAYA_OS_COMPONENTS:
             local = self.__local_version(raya_component)
             latest = self.__get_latest_version(raya_component)
             same_major = self.__get_major(latest) == self.__get_major(local)
             same_minor = self.__get_minor(latest) == self.__get_minor(local)
-            diff_patch = self.__get_patch(local) != self.__get_patch(latest)
+            diff_patch = self.__get_patch(local) < self.__get_patch(latest)
             if same_major and same_minor and diff_patch:
-                log_warning(
-                    (f'{raya_component} have an patch update it is going to be'
-                     f' updated to version \'{latest}\', current \'{local}\''))
+                if show_msg:
+                    log_warning(
+                        (f'{raya_component} have an patch update it is going to be'
+                        f' updated to version \'{latest}\', '
+                        f'current \'{local}\''))
                 updated = False
         return updated
 
 
     def update_patch(self, component):
         '''Update the component and return True if the update was successful'''
         if component == 'Unity':
-            response = requests.request("GET", constants.VCS_URL)
+            response = self.get_VCS_json(type_version='patch', component='Unity')
             version = self.__get_latest_version(component)
-            if self.simulator.download_simulator(response=response.json()):
+            if self.simulator.download_simulator(response=response):
                 return True
         elif component == 'Docker':
             version = self.__get_latest_version(component)
             if self.docker_handler.download_raya_image(version):
                 return True
         return False
 
 
     def get_latest_version(self, component):
         return self.__get_latest_version(component=component)
+    
+    
+    def get_VCS_json(self, type_version: str = 'latest', component: str = None) -> ( list | None ):
+        try:
+            response = requests.request("GET", constants.VCS_URL)
+            return response.json()
+        except requests.exceptions.ConnectionError as e:
+            raise e
+        except Exception as e:
+            log_error(e)
+        return None
```

### Comparing `rayasdk-1.1.0.dev7/rayasdk.egg-info/PKG-INFO` & `rayasdk-1.1.0.dev8/rayasdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayasdk
-Version: 1.1.0.dev7
+Version: 1.1.0.dev8
 Summary: Raya SDK - Unlimited Robotics Software Development Kit
 Home-page: UNKNOWN
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: MIT
 Keywords: robotics,unlimited-robotics,gary
 Platform: UNKNOWN
```

### Comparing `rayasdk-1.1.0.dev7/rayasdk.egg-info/SOURCES.txt` & `rayasdk-1.1.0.dev8/rayasdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev7/setup.py` & `rayasdk-1.1.0.dev8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 from pip_tools import get_last_release_version, get_last_prerelease_version
 
-VERSION = '1.1.0.dev7'
+VERSION = '1.1.0.dev8'
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='rayasdk',
     packages=find_packages(),
```

