# Comparing `tmp/qecore-3.8.tar.gz` & `tmp/qecore-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qecore-3.8.tar", last modified: Mon May 10 06:35:51 2021, max compression
+gzip compressed data, was "dist/qecore-3.9.tar", last modified: Fri Sep 17 06:41:31 2021, max compression
```

## Comparing `qecore-3.8.tar` & `qecore-3.9.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 modehnal  (1000) modehnal  (1000)        0 2021-05-10 06:35:51.000000 qecore-3.8/
-drwxr-xr-x   0 modehnal  (1000) modehnal  (1000)        0 2021-05-10 06:35:51.000000 qecore-3.8/__testing__/
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)        0 2021-03-23 12:03:18.000000 qecore-3.8/__testing__/__init__.py
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)    31205 2021-04-13 08:24:28.000000 qecore-3.8/__testing__/api.py
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)     1039 2021-05-06 10:51:59.000000 qecore-3.8/__testing__/reproducer.py
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)    27806 2021-03-19 16:49:36.000000 qecore-3.8/__testing__/z.py
-drwxr-xr-x   0 modehnal  (1000) modehnal  (1000)        0 2021-05-10 06:35:51.000000 qecore-3.8/qecore/
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)      597 2021-05-10 06:35:06.000000 qecore-3.8/qecore/__init__.py
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)    16710 2021-05-10 06:35:06.000000 qecore-3.8/qecore/application.py
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)    17518 2021-05-10 06:35:06.000000 qecore-3.8/qecore/common_steps.py
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)     4533 2021-02-22 18:48:17.000000 qecore-3.8/qecore/flatpak.py
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)    12652 2021-02-22 18:48:17.000000 qecore-3.8/qecore/get_node.py
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)    14757 2020-11-09 10:20:36.000000 qecore-3.8/qecore/icons.py
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)     9941 2021-01-19 13:21:50.000000 qecore-3.8/qecore/image_matching.py
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)     2843 2021-05-10 06:35:06.000000 qecore-3.8/qecore/logger.py
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)    21561 2021-05-10 06:35:06.000000 qecore-3.8/qecore/online_accounts.py
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)    51570 2021-05-10 06:35:06.000000 qecore-3.8/qecore/sandbox.py
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)     6181 2020-06-17 08:42:21.000000 qecore-3.8/qecore/step_matcher.py
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)     9177 2021-05-10 06:35:06.000000 qecore-3.8/qecore/utility.py
-drwxr-xr-x   0 modehnal  (1000) modehnal  (1000)        0 2021-05-10 06:35:51.000000 qecore-3.8/qecore.egg-info/
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)      452 2021-05-10 06:35:50.000000 qecore-3.8/qecore.egg-info/PKG-INFO
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)      704 2021-05-10 06:35:50.000000 qecore-3.8/qecore.egg-info/SOURCES.txt
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)        1 2021-05-10 06:35:50.000000 qecore-3.8/qecore.egg-info/dependency_links.txt
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)       46 2021-05-10 06:35:50.000000 qecore-3.8/qecore.egg-info/requires.txt
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)       19 2021-05-10 06:35:50.000000 qecore-3.8/qecore.egg-info/top_level.txt
-drwxr-xr-x   0 modehnal  (1000) modehnal  (1000)        0 2021-05-10 06:35:51.000000 qecore-3.8/scripts/
--rwxr-xr-x   0 modehnal  (1000) modehnal  (1000)    17747 2020-11-09 10:20:36.000000 qecore-3.8/scripts/qecore
--rwxr-xr-x   0 modehnal  (1000) modehnal  (1000)    27608 2021-05-10 06:35:06.000000 qecore-3.8/scripts/qecore-headless
--rwxr-xr-x   0 modehnal  (1000) modehnal  (1000)       35 2020-11-09 10:20:36.000000 qecore-3.8/scripts/qecore-runtest
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)      481 2020-11-09 10:20:36.000000 qecore-3.8/scripts/qecore_bash_completion
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)      233 2020-04-29 19:30:43.000000 qecore-3.8/scripts/qecore_get_active_display
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)       61 2020-04-29 19:30:43.000000 qecore-3.8/scripts/qecore_help
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)      671 2020-04-29 19:30:43.000000 qecore-3.8/scripts/qecore_start_keyring
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)      254 2020-04-29 19:30:43.000000 qecore-3.8/scripts/qecore_start_recording
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)      503 2020-09-17 14:20:50.000000 qecore-3.8/README.md
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)     1008 2021-05-10 06:35:06.000000 qecore-3.8/setup.py
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)      452 2021-05-10 06:35:51.000000 qecore-3.8/PKG-INFO
--rw-r--r--   0 modehnal  (1000) modehnal  (1000)       38 2021-05-10 06:35:51.000000 qecore-3.8/setup.cfg
+drwxr-xr-x   0 modehnal  (1000) modehnal  (1000)        0 2021-09-17 06:41:31.000000 qecore-3.9/
+drwxr-xr-x   0 modehnal  (1000) modehnal  (1000)        0 2021-09-17 06:41:31.000000 qecore-3.9/__testing__/
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)        0 2021-03-23 12:03:18.000000 qecore-3.9/__testing__/__init__.py
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)    31205 2021-04-13 08:24:28.000000 qecore-3.9/__testing__/api.py
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)     2089 2021-07-12 11:59:46.000000 qecore-3.9/__testing__/coredump.py
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)     1039 2021-05-06 10:51:59.000000 qecore-3.9/__testing__/reproducer.py
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)    27806 2021-03-19 16:49:36.000000 qecore-3.9/__testing__/z.py
+drwxr-xr-x   0 modehnal  (1000) modehnal  (1000)        0 2021-09-17 06:41:31.000000 qecore-3.9/qecore/
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)      597 2021-09-06 12:42:54.000000 qecore-3.9/qecore/__init__.py
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)    16724 2021-09-06 10:20:28.000000 qecore-3.9/qecore/application.py
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)    17479 2021-09-06 10:21:03.000000 qecore-3.9/qecore/common_steps.py
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)     4535 2021-09-06 10:56:13.000000 qecore-3.9/qecore/flatpak.py
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)    12652 2021-09-06 09:58:28.000000 qecore-3.9/qecore/get_node.py
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)    14757 2021-09-06 09:58:32.000000 qecore-3.9/qecore/icons.py
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)     9941 2021-09-06 09:58:35.000000 qecore-3.9/qecore/image_matching.py
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)     2843 2021-09-06 09:58:38.000000 qecore-3.9/qecore/logger.py
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)    21561 2021-09-06 09:58:42.000000 qecore-3.9/qecore/online_accounts.py
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)    62100 2021-09-06 12:56:10.000000 qecore-3.9/qecore/sandbox.py
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)     6190 2021-09-06 10:45:13.000000 qecore-3.9/qecore/step_matcher.py
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)     9160 2021-09-06 10:54:47.000000 qecore-3.9/qecore/utility.py
+drwxr-xr-x   0 modehnal  (1000) modehnal  (1000)        0 2021-09-17 06:41:31.000000 qecore-3.9/qecore.egg-info/
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)      452 2021-09-17 06:41:30.000000 qecore-3.9/qecore.egg-info/PKG-INFO
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)      767 2021-09-17 06:41:30.000000 qecore-3.9/qecore.egg-info/SOURCES.txt
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)        1 2021-09-17 06:41:30.000000 qecore-3.9/qecore.egg-info/dependency_links.txt
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)       46 2021-09-17 06:41:30.000000 qecore-3.9/qecore.egg-info/requires.txt
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)       19 2021-09-17 06:41:30.000000 qecore-3.9/qecore.egg-info/top_level.txt
+drwxr-xr-x   0 modehnal  (1000) modehnal  (1000)        0 2021-09-17 06:41:31.000000 qecore-3.9/scripts/
+-rwxr-xr-x   0 modehnal  (1000) modehnal  (1000)    17747 2021-09-06 10:59:24.000000 qecore-3.9/scripts/qecore
+-rwxr-xr-x   0 modehnal  (1000) modehnal  (1000)    27576 2021-09-06 09:59:33.000000 qecore-3.9/scripts/qecore-headless
+-rwxr-xr-x   0 modehnal  (1000) modehnal  (1000)       35 2020-11-09 10:20:36.000000 qecore-3.9/scripts/qecore-runtest
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)     5330 2021-09-06 09:59:17.000000 qecore-3.9/scripts/qecore_backtrace_from_coredump
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)      481 2021-09-06 09:59:20.000000 qecore-3.9/scripts/qecore_bash_completion
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)      230 2021-09-06 09:59:23.000000 qecore-3.9/scripts/qecore_get_active_display
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)       61 2021-09-06 09:59:26.000000 qecore-3.9/scripts/qecore_help
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)      671 2021-09-06 09:59:28.000000 qecore-3.9/scripts/qecore_start_keyring
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)      254 2020-04-29 19:30:43.000000 qecore-3.9/scripts/qecore_start_recording
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)      503 2020-09-17 14:20:50.000000 qecore-3.9/README.md
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)     1008 2021-09-06 12:42:58.000000 qecore-3.9/setup.py
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)      452 2021-09-17 06:41:31.000000 qecore-3.9/PKG-INFO
+-rw-r--r--   0 modehnal  (1000) modehnal  (1000)       38 2021-09-17 06:41:31.000000 qecore-3.9/setup.cfg
```

### Comparing `qecore-3.8/__testing__/api.py` & `qecore-3.9/__testing__/api.py`

 * *Files identical despite different names*

### Comparing `qecore-3.8/__testing__/reproducer.py` & `qecore-3.9/__testing__/reproducer.py`

 * *Files identical despite different names*

### Comparing `qecore-3.8/__testing__/z.py` & `qecore-3.9/__testing__/z.py`

 * *Files identical despite different names*

### Comparing `qecore-3.8/qecore/__init__.py` & `qecore-3.9/qecore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 __author__ = """Michal Odehnal <modehnal@redhat.com>"""
-__version__ = "3.8"
+__version__ = "3.9"
 __copyright__ = "Copyright © 2018-2020 Red Hat, Inc."
 __license__ = "GPL"
 __all__ = ("application",
            "common_steps",
            "flatpak",
            "get_node",
            "image_matching",
```

### Comparing `qecore-3.8/qecore/application.py` & `qecore-3.9/qecore/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
         :type desktop_file_name: str
         :param desktop_file_name: Name of desktop file if not same as component.
 
         :type app_process_name: str
         :param app_process_name: Name of application process if not same as component.
         """
-       
+
         log.info(" ".join((
                 f"__init__(self, component={component}, a11y_app_name={a11y_app_name},",
                 f"desktop_file_exists={desktop_file_exists},",
                 f"desktop_file_name={desktop_file_name},",
                 f"desktop_file_path={desktop_file_path},",
                 f"app_process_name={app_process_name}, shell='shell',",
                 f"session_type={session_type}, session_desktop={session_desktop})"
@@ -63,15 +63,15 @@
         self.desktop_file_path = desktop_file_path
         self.application_list = []
         self.app_process_name = app_process_name if app_process_name else component
         self.icon = None
         self.get_desktop_file_data()
 
         if 'Flatpak' not in f'{type(self)}':
-            # Preserving old api names of functions
+            # Preserving old api names of functions.
             self.getDesktopFileData = self.get_desktop_file_data
             self.getRoot = self.get_root
             self.isRunning = self.is_running
             self.getPidList = self.get_pid_list
             self.getAllKillCandidates = self.get_all_kill_candidates
 
 
@@ -82,15 +82,16 @@
         .. note::
 
             Do **NOT** call this by yourself. This method is called by :func:`__init__`.
         """
 
         log.info(f"{self.component} get_desktop_file_data(self)")
 
-        if self.desktop_file_exists: # zenity/gnome-shell do not have desktop file
+        # zenity/gnome-shell do not have desktop file.
+        if self.desktop_file_exists:
             if self.desktop_file_path:
                 desktop_file = self.desktop_file_path
             else:
                 desktop_run = run(" ".join((
                     f"rpm -qlf $(which {self.component}) |",
                     "grep /usr/share/applications/ |",
                     "grep .desktop |",
@@ -298,15 +299,15 @@
         :rtype: bool
 
         This method is used by various other methods in this class to ensure correct behaviour.
         You do not need to use this by yourself, but can be useful in some situations.
         """
 
         log.info(f"{self.component} is_running(self)")
-            
+
         is_running = False
 
         try:
             self.application_list = [x.name for x in root.applications()]
             for _ in range(3):
                 is_running = self.a11y_app_name in self.application_list
                 if is_running:
@@ -370,15 +371,16 @@
                     ("behave" in process) or \
                     ("dogtail" in process) or \
                     (process == "/usr/bin/gnome-shell")):
                 extracted_pid = process.split(" ", 1)[0]
                 try:
                     final_pid_list.append(int(extracted_pid))
                 except ValueError:
-                    pass # skip non-digits
+                    # Skip non-digits.
+                    pass
         return final_pid_list
 
 
     def kill_application(self):
         """
         Kill application.
 
@@ -444,15 +446,15 @@
                 return
 
         assert False, "".join((
             f"Application '{self.a11y_app_name}' was still found in application tree: '{self.application_list}'."
         ))
 
 
-    #Using properties to preserve old api of attributes
+    # Using properties to preserve old api of attributes.
     @property
     def a11yAppName(self):
         return self.a11y_app_name
     @a11yAppName.setter
     def a11yAppName(self, value):
         self.a11y_app_name = value
```

### Comparing `qecore-3.8/qecore/common_steps.py` & `qecore-3.9/qecore/common_steps.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
 __author__ = """
 Filip Pokryvka <fpokryvk@redhat.com>,
 Michal Odehnal <modehnal@redhat.com>,
 Bohdan Milar <bmilar@redhat.com>
 """
 
-use_step_matcher("qecore")  # to stop using "qecore" matcher use matcher "parse"
+# To stop using "qecore" matcher use matcher "parse".
+use_step_matcher("qecore")
 
 """
 This allows multiple decorator definitions on one line separated by ' | '
 EXAMPLE:
 This decorator:
     @step('Item "{name}" "{role_name}" | with description "{description}" | that is "{attr}"')
 
@@ -145,15 +146,16 @@
             assert False, error
         except Exception:
             application.start_via_command(command=command, in_session=session, kill=kill)
     else:
         raise AssertionError("Only defined options are 'command' and 'menu'.")
 
 
-use_step_matcher("parse")  # stop using qecore matcher
+# Stop using qecore matcher.
+use_step_matcher("parse")
 
 
 @step('Close application "{application}" via "{close_via}"')
 def application_in_not_running(context, application=None, close_via="gnome panel"):
     application = get_application(context, application)
 
     if close_via == "gnome panel":
@@ -274,15 +276,15 @@
         application.wait_before_app_starts(15)
 
 
 @step('Run and save command output: "{command}"')
 def run_and_save(context, command):
     """
     Run a shell command and store its returncode, stdour and stderr to context.
-    
+
     :type command: str
     :param command: Command line to be executed and result stored.
     """
 
     process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, encoding="utf-8")
     try:
         stdout, stderr = process.communicate(timeout=5)
@@ -291,27 +293,27 @@
         stdout, stderr = process.communicate()
 
     context.command = command
     context.command_stdout = stdout
     context.command_stderr = stderr
     context.command_return_code = process.returncode
 
-    
+
 @step('Last command output "{operand}" "{expected_output}"')
 def verify_content_in_output(context, operand, expected_output):
     """
     Verify that the result of last command has a certain data as a result.
-    
+
     :type operand: str
     :param operand: String specifying what operation to do.
-    
+
     :type expected_output: str
     :param expected_output: Expected data to be compared to the command output.
-    """    
-    
+    """
+
     assert hasattr(context, "command_stdout"), "".join((
         "\nYou have not saved a command output to be checked.",
         "\nTo do that use '* Run and save command output: \"<command>\"'"
     ))
 
     valid_operands = ("is", "is not", "contains", "does not contain", "begins with",
                       "does not begin with", "ends with", "does not end with")
@@ -370,22 +372,22 @@
         ))
 
 
 @step('Return code of last command output "{operand}" "{expected_return_code}"')
 def verify_return_code_of_command(context, operand, expected_return_code):
     """
     Verify the return code of last command.
-    
+
     :type operand: str
     :param operand: String specifying what operation to do.
-    
+
     :type expected_return_code: str
     :param expected_return_code: Expected data to be compared to the command output.
-    """   
-    
+    """
+
     assert hasattr(context, "command_stdout"), "".join((
         "\nYou have not saved a command output to be checked.",
         "\nTo do that use '* Run and save command output: \"<command>\"'"
     ))
 
     valid_operands = ("is", "is not")
     assert operand in valid_operands, "".join((
```

### Comparing `qecore-3.8/qecore/flatpak.py` & `qecore-3.9/qecore/flatpak.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 
     def kill_application(self):
         """
         Killing via 'flatpak kill <flatpak_id>', sudo for @system flatpaks
         """
 
         if self.is_running() and self.kill:
-            # kills a flatpak installed @System
+            # Kills a flatpak installed @System.
             run(f"sudo flatpak kill {self.component}")
-            # kills a flatpak installed @User
+            # Kills a flatpak installed @User.
             run(f"flatpak kill {self.component}")
 
 
     def get_desktop_file_data(self):
         """
         Provide information from .desktop file, two possible locations:
             * flatpak installed as *--user*::
```

### Comparing `qecore-3.8/qecore/get_node.py` & `qecore-3.9/qecore/get_node.py`

 * *Files identical despite different names*

### Comparing `qecore-3.8/qecore/icons.py` & `qecore-3.9/qecore/icons.py`

 * *Files identical despite different names*

### Comparing `qecore-3.8/qecore/image_matching.py` & `qecore-3.9/qecore/image_matching.py`

 * *Files identical despite different names*

### Comparing `qecore-3.8/qecore/logger.py` & `qecore-3.9/qecore/logger.py`

 * *Files identical despite different names*

### Comparing `qecore-3.8/qecore/online_accounts.py` & `qecore-3.9/qecore/online_accounts.py`

 * *Files identical despite different names*

### Comparing `qecore-3.8/qecore/sandbox.py` & `qecore-3.9/qecore/sandbox.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import re
 import base64
 import traceback
 import signal
 import atexit
 import behave
 import xml.etree.ElementTree as ET
+import time
 from time import sleep
 from subprocess import Popen
 from mimetypes import MimeTypes
 from dogtail.utils import config, isA11yEnabled, enableA11y
 from dogtail.rawinput import keyCombo
 from qecore.utility import run
 
@@ -56,18 +57,22 @@
             You are able to use logging via debug variable: QECORE_DEBUG=yes behave -kt <test_name>
 
             You are able to use general logging via variable: LOGGING=yes behave -kt <test_name>
 
             You can enforce embedding for testing purposes via debug variable: QECORE_EMBED_ALL=yes
         """
 
-        assert isinstance(logging, bool), "Unexpected argument, logging should be bool"
+        assert isinstance(logging, bool), "".join((
+            "Unexpected argument, logging should be bool"
+        ))
+
         if context is not None:
-            assert isinstance(context, behave.runner.Context), \
+            assert isinstance(context, behave.runner.Context), "".join((
                 "Unexpected argument, context should be <behave.runner.Context> instance"
+            ))
 
         self._embed_all = os.environ.get("QECORE_EMBED_ALL", "").lower() not in NO_VALUES
         self._logging_env = os.environ.get("QECORE_DEBUG", "").lower() not in NO_VALUES
         self._logging_generic = os.environ.get("LOGGING", "").lower() not in NO_VALUES
 
         log.logger.disabled = not (logging or self._logging_env)
         generic_log.logger.disabled = True
@@ -101,20 +106,26 @@
 
         self.attach_video = True
         self.attach_video_on_pass = False
 
         self.attach_journal = True
         self.attach_journal_on_pass = False
 
+        self.attach_coredump = False
+        self.attach_coredump_on_pass = True
+        self.attach_coredump_file_check = False
+
         self.attach_screenshot = True
         self.failed_test = False
 
         self.attach_faf = True
         self.attach_faf_on_pass = True
+
         self.logging_cursor = None
+        self.test_execution_start = None
 
         self.workspace_return = False
 
         self.set_keyring = True
         self.keyring_process_pid = None
 
         self.wait_for_stable_video = True
@@ -122,24 +133,27 @@
         self.production = True
 
         self.timeout_handling = True
 
         self._after_scenario_hooks = []
         self.reverse_after_scenario_hooks = False
 
+        self.html_report_links = True
+
         self.embed_separate = False
         self.change_title = True
         self.session_icon_to_title = True
         self.default_application_icon_to_title = False
 
         self.applications = []
         self.default_application = None
 
         self._set_up_scenario_skip_check()
         self._retrieve_session_data()
+        self._check_for_coredump_fetching()
         self._set_g_debug_environment_variable()
         self._wait_until_shell_becomes_responsive()
 
         self.shell = root.application("gnome-shell")
 
 
     def before_scenario(self, context, scenario):
@@ -151,39 +165,32 @@
 
         :type scenario: <Scenario>
         :param scenario: Pass this object from environment file.
 
         .. note::
 
             You can enforce embedding for testing purposes via debug variable: QECORE_EMBED_ALL=yes
-
-        .. note::
-            Do **NOT** call this, if you provided context to :func:`__init__`.
         """
 
         log.info(f"before_scenario(self, context, scenario) test: {scenario.tags[-1]}")
 
-        if getattr(context, "before_scenario_executed", False):
-            print("before_scenario was already executed! If sandbox constructed with context, remove it in environment.py")
-            return
-
-        context.before_scenario_executed = True
         self._scenario_skipped = False
 
         self.failed_test = False
 
-        # if QECORE_EMBED_ALL is set, set production to True
+        # If QECORE_EMBED_ALL is set, set production to True.
         self.production = self.production or self._embed_all
 
         self._set_welcome_tour()
 
         self._set_animations()
 
         self.current_scenario = scenario.tags[-1]
-        self._set_log_start_time()
+        self._set_journal_log_start_time()
+        self._set_coredump_log_start_time()
         self.overview_action("hide")
         self.set_typing_delay(0.2)
         self.set_debug_to_stdout_as(False)
         self._close_yelp()
         self._close_initial_setup()
         self._copy_data_folder()
         self.set_blank_screen_to_never()
@@ -208,27 +215,18 @@
         Actions that are to be executed after every scenario.
 
         :type context: <behave.runner.Context>
         :param context: Pass this object from environment file.
 
         :type scenario: <Scenario>
         :param scenario: Pass this object from environment file.
-
-        .. note::
-            Do **NOT** call this, if you provided context to :func:`__init__`.
         """
 
         log.info(f"after_scenario(self, context, scenario) test: {scenario.tags[0]}")
 
-        if getattr(context, "after_scenario_executed", False):
-            print("after_scenario was already executed! If sandbox constructed with context, remove it in environment.py")
-            return
-
-        context.after_scenario_executed = True
-
         if scenario.status == "failed":
             self.failed_test = True
 
         self._capture_image()
 
         if self.background_image_revert:
             self._revert_background_image()
@@ -241,29 +239,34 @@
         for application in self.applications:
             application.kill_application()
 
         self._attach_screenshot_to_report(context)
 
         self._attach_journal_to_report(context)
 
+        self._attach_coredump_log_to_report(context)
+
         self._attach_video_to_report(context)
 
         self._attach_abrt_link_to_report(context)
 
         self._process_after_scenario_hooks(context)
 
         self._process_embeds(context)
 
+        if self.html_report_links:
+            self._html_report_links(context)
+
 
     def _after_all(self, context):
         """
         This is executed as behave after_all hook, if context is proved in :func:`__init__`.
 
         :type context: <behave.runner.Context>
-        :param context: Pass this object from environment file.
+        :param context: Object is passed from the function that is calling it.
 
         .. note::
             Do **NOT** call this, if you provided context to :func:`__init__`.
         """
 
         self._scenario_skip_check_cb(do_assert=True)
 
@@ -280,15 +283,15 @@
         log.info(f"_scenario_skip_check_cb(self, do_assert={do_assert})")
 
         if do_assert:
             assert not self._scenario_skipped, "No scenario matched tags"
         else:
             if self._scenario_skipped:
                 print("No scenario matched tags, exiting with error code 1.")
-                # sys.exit, raise, assert do not work in an atexit hook
+                # sys.exit, raise, assert do not work in an atexit hook.
                 os._exit(1)
 
 
     def _set_up_scenario_skip_check(self):
         """
         Remember in sandbox if any scenario (:func:`before_scenario`) was executed.
 
@@ -501,15 +504,16 @@
         if self.session_type == "x11":
             for _ in range(60):
                 if not "gnome-shell" in [x.name for x in root.applications()]:
                     sleep(0.5)
                 else:
                     break
         else:
-            sleep(1) # in wayland there is no way to make sure the session is loaded, so just sleep
+            # Under Wayland there is no way to make sure the session is loaded, so just sleep.
+            sleep(1)
 
 
     def _retrieve_session_data(self):
         """
         Get session/system data.
 
         .. note::
@@ -704,31 +708,46 @@
                 "set",
                 "org.gnome.desktop.interface",
                 "enable-animations",
                 "true" if self.enable_animations else "false"
             )))
 
 
-    def _set_log_start_time(self):
+    def _set_journal_log_start_time(self):
         """
         Save time.
         Will be used to retrieve logs from journal.
 
         .. note::
 
             Do **NOT** call this by yourself. This method is called by :func:`before_scenario`.
         """
 
-        log.info("_set_log_start_time(self)")
+        log.info("_set_journal_log_start_time(self)")
 
         initial_cursor_output = run("sudo journalctl --lines=0 --show-cursor").strip()
         cursor_target = initial_cursor_output.split("cursor: ", 1)[-1]
         self.logging_cursor = f"\"--after-cursor={cursor_target}\""
 
 
+    def _set_coredump_log_start_time(self):
+        """
+        Save time.
+        Will be used to retrieve coredumpctl list.
+
+        .. note::
+
+            Do **NOT** call this by yourself. This method is called by :func:`before_scenario`.
+        """
+
+        log.info("_set_coredump_log_start_time(self)")
+
+        self.test_execution_start = run("date +\%\s").strip("\n")
+
+
     def _close_yelp(self):
         """
         Close yelp application that is opened after fresh system installation.
 
         .. note::
 
             Do **NOT** call this by yourself. This method is called by :func:`before_scenario`.
@@ -930,26 +949,40 @@
             return
 
         log.info("_capture_image(self)")
 
         self.screenshot_run_result = run("gnome-screenshot -f /tmp/screenshot.png", verbose=True)
 
 
+    def _check_for_coredump_fetching(self):
+        """
+        Set attach_coredump variable if set in Jenkins - tested via file existance.
+
+        .. note::
+
+            Do **NOT** call this by yourself. This method is called by :func:`__init__`.
+        """
+
+        log.info("_check_for_coredump_fetching(self)")
+
+        self.attach_coredump_file_check = os.path.exists("/tmp/qecore_coredump_fetch")
+
+
     def _set_g_debug_environment_variable(self):
         """
         Setup environment variable G_DEBUG as 'fatal-criticals'.
 
         .. note::
 
             Do **NOT** call this by yourself. This method is called by :func:`__init__`.
         """
 
         log.info("_set_g_debug_environment_variable(self)")
 
-        # Environment value set upon checked field in Jenkins
+        # Environment value set upon checked field in Jenkins.
         if os.path.isfile("/tmp/headless_enable_fatal_critical"):
             os.environ["G_DEBUG"] = "fatal-criticals"
 
         # Fatal_wanings has bigger priority than criticals.
         # Should both options be set in Jenkins the warning will overwrite the variable.
         if os.path.isfile("/tmp/headless_enable_fatal_warnings"):
             os.environ["G_DEBUG"] = "fatal-warnings"
@@ -1183,14 +1216,140 @@
                           data=open("/tmp/journalctl_short.log", "r").read(),
                           caption="journalctl",
                           fail_only=not self.attach_journal_on_pass)
 
         run("rm /tmp/journalctl_short.log")
 
 
+    def _attach_coredump_log_to_report(self, context):
+        """
+        Attach coredump log to the html report upon failed test.
+
+        :type context: <behave.runner.Context>
+        :param context: Passed object.
+
+        .. note::
+
+            Do **NOT** call this by yourself. This method is called by :func:`after_scenario`.
+        """
+
+        if not self.production:
+            return
+
+        if not (self.attach_coredump or self.attach_coredump_file_check or self._embed_all):
+            return
+
+        if not (self.attach_coredump_on_pass or self.failed_test or self._embed_all):
+            return
+
+        log.info("_attach_coredump_log_to_report(self, context)")
+
+        # Get coredump list results only from duration of the test.
+        coredump_list = run(f"sudo coredumpctl list --since=@{self.test_execution_start}")
+
+        # If there are no coredumps end right here.
+        if "No coredumps found." in coredump_list:
+            return
+
+        coredump_log = "/tmp/qecore_coredump.log"
+        debuginfo_install_log = "/tmp/qecore_debuginfo_install.log"
+
+        # Empty the coredump file logs.
+        if os.path.isfile(coredump_log):
+            run(f">{coredump_log}")
+
+        # Do not empty debuginfo log - the content is desired in all possible tests.
+        if not os.path.isfile(debuginfo_install_log):
+            run(f"touch {debuginfo_install_log}")
+
+        # Get packages to be installed from gdb.
+        def get_packages_from_coredump(pid):
+            # Get first gdb output and load it to file to parse over.
+            run(f"echo 'q' | sudo coredumpctl gdb {pid} 2&> {coredump_log}")
+
+            # Set the base variable to return with all data.
+            desired_data = ""
+
+            # Open the file and iterate over its lines.
+            with open(coredump_log, "r") as f:
+                # Loading one line at a time.
+                next_line = f.readline()
+
+                # Loop until there is no next line.
+                while next_line:
+                    # Parse correct lines to fetch debuginfo packages.
+                    if "debug" in next_line and "install" in next_line:
+                        _, target = next_line.split("install ", 1)
+                        desired_data += target.strip("\n") + " "
+
+                    # If there is no coredump file present there si nothing to fetch.
+                    elif "Coredump entry has no core attached." in next_line:
+                        return None
+
+                    # Load the next line.
+                    next_line = f.readline()
+
+            return desired_data
+
+
+        # Install all packages that gdb desires.
+        def install_debuginfo_packages(pid):
+            # We need gdb to be installed.
+            if "not installed" in run("rpm -q gdb"):
+                run(f"sudo dnf install -y gdb >> {debuginfo_install_log}")
+
+            # Iterate a few times over the gdb to get packages and install them.
+            packages_installed_in_last_attempt = ""
+            for _ in range(20):
+                packages_to_install = get_packages_from_coredump(pid)
+
+                # Install required packages but break if packages were already attempted to be installed.
+                if packages_to_install and (packages_to_install != packages_installed_in_last_attempt):
+                    packages_installed_in_last_attempt = packages_to_install
+                    run(f"sudo dnf debuginfo-install -y {packages_to_install} >> {debuginfo_install_log}")
+                else:
+                    break
+
+
+        # Load coredump lines as provided.
+        list_of_results = coredump_list.rstrip("\n").split("\n")[1:]
+        for coredump_line in list_of_results:
+            starting_time = time.time()
+
+            coredump_line_split = coredump_line.split(" ")
+            coredump_line_filtered = [x for x in coredump_line_split if x]
+            coredump_pid_to_investigate = coredump_line_filtered[4]
+
+            # Check if coredump file does not exist.
+            if coredump_line_filtered[8] == "none" or coredump_line_filtered[8] != "present":
+                # Attach data to html report.
+                context.embed(mime_type="text/plain",
+                              data="Coredump entry has no core attached.",
+                              caption=f"CoredumpLog")
+                break
+
+            # Install all debuginfos given by coredump file with found pid.
+            install_debuginfo_packages(coredump_pid_to_investigate)
+
+            # All debuginfo packages should be installed now - get the backtrace and attach it to report.
+            run(f"echo 'thread apply all bt full' | sudo coredumpctl gdb {coredump_pid_to_investigate} 2&> {coredump_log}")
+
+            # Calculate the total execution time of coredump fetch.
+            coredump_fetch_time = time.time()-starting_time
+
+            context.embed(mime_type="text/plain",
+                        data=open(coredump_log, "r").read(),
+                        caption=f"CoredumpLog{coredump_pid_to_investigate}+{coredump_fetch_time:.1f}s")
+
+
+        context.embed(mime_type="text/plain",
+                    data=open(debuginfo_install_log, "r").read(),
+                    caption=f"DebugInfoInstallLog")
+
+
     def _attach_abrt_link_to_report(self, context):
         """
         Attach abrt link to the html report upon detected abrt FAF report.
 
         :type context: <behave.runner.Context>
         :param context: Passed object.
 
@@ -1291,28 +1450,152 @@
 
         scenario_fail = self.failed_test or self._embed_all
 
         embeds = getattr(context, "_to_embed", [])
         log.info(f" process {len(embeds)} embeds")
 
         for kwargs in embeds:
-            # execute postponed "call"s
+            # Execute postponed "call"s.
             if kwargs["mime_type"] == "call":
-                # "data" is function, "caption" is args, function returns triple
+                # "data" is function, "caption" is args, function returns triple.
                 mime_type, data, caption = kwargs["data"](*kwargs["caption"])
                 kwargs["mime_type"], kwargs["data"], kwargs["caption"] = mime_type, data, caption
             # skip "fail_only" when scenario passed
             if not scenario_fail and kwargs["fail_only"]:
                 continue
-            # reset "fail_only" to prevent loop
+            # Reset "fail_only" to prevent loop.
             kwargs["fail_only"] = False
             context.embed(**kwargs)
         context._to_embed = []
 
 
+    def _html_report_links(self, context):
+        """
+        Fetch a tag link to the git repository in current commit.
+
+        :type context: <behave.runner.Context>
+        :param context: Passed object.
+
+
+        .. note::
+
+            Do **NOT** call this by yourself. This method is called by :func:`after_scenario`.
+        """
+
+        git_url = self.project_git_url
+        git_commit = self.project_git_commit
+        if not git_url or not git_commit:
+            return
+        project_url_base = f"{self.project_git_url}/-/tree/{self.project_git_commit}/"
+        qecore_url_base = "/".join((
+            "https://gitlab.com",
+            "dogtail/qecore/-/tree/master/qecore/"
+        ))
+        nmci_url_base = "/".join((
+            "https://gitlab.freedesktop.org",
+            "NetworkManager/NetworkManager-ci/-/tree/master/"
+        ))
+
+        # Search for links in scenario HTML element.
+        if getattr(context, "html_formatter", None) is None:
+            return
+        scenario_el = context.html_formatter.scenario_el
+        scenario_file = scenario_el.find(".//span[@class='scenario_file']")
+        step_files = scenario_el.findall(".//div[@class='step_file']/span")
+        tags_el = scenario_el.find(".//span[@class='tag']")
+
+        # Link tags to scenario (.feature file).
+        if tags_el is not None:
+            tags = tags_el.text.split()
+            tags.reverse()
+            tags_el.text = ""
+            scenario_name = True
+
+            for tag in tags:
+                if tag.startswith("@rhbz"):
+                    bug_id = tag.replace("@rhbz", "").rstrip(",")
+                    link_el = ET.Element(
+                        "a",
+                        {
+                            "href": "https://bugzilla.redhat.com/" + bug_id,
+                            "target": "_blank",
+                            "style": "color:inherit",
+                        },
+                    )
+                    link_el.text = tag
+                    tags_el.insert(0, link_el)
+                elif scenario_name:
+                    scenario_name = False
+                    if scenario_file is not None:
+                        file_name, line = scenario_file.text.split(":", 2)
+                        link_el = ET.Element(
+                            "a",
+                            {
+                                "href": project_url_base + file_name + "#L" + line,
+                                "target": "_blank",
+                                "style": "color:inherit",
+                            },
+                        )
+                        link_el.text = tag
+                        tags_el.insert(0, link_el)
+
+                else:
+                    span_el = ET.Element("span")
+                    span_el.text = tag
+                    tags_el.insert(0, span_el)
+
+        # Link files.
+        for file_el in [scenario_file] + step_files:
+            if file_el is not None:
+                file_name, line = file_el.text.split(":", 2)
+                if file_name.startswith("NMci"):
+                    url = nmci_url_base + file_name.replace("NMci/", "", 1)
+                elif "/site-packages/qecore/" in file_name:
+                    url = qecore_url_base + file_name.split("/site-packages/qecore/")[-1]
+                else:
+                    url = project_url_base + file_name
+                link = ET.SubElement(
+                    file_el,
+                    "a",
+                    {
+                        "href": url + "#L" + line,
+                        "target": "_blank",
+                        "style": "color:inherit",
+                    },
+                )
+                link.text = file_el.text
+                file_el.text = ""
+
+
+    @property
+    def project_git_url(self):
+        remote = getattr(self, "_project_git_url", None)
+        if remote is None:
+            remote, return_code, _ = run("git config --get remote.origin.url", verbose=True)
+            remote = remote.strip("\n")[:-4]
+            if return_code != 0:
+                remote = False
+            elif remote.startswith("git@"):
+                remote = remote.replace(":", "/").replace("git@", "https://")
+            self._project_git_url = remote
+        return remote
+
+
+    @property
+    def project_git_commit(self):
+        commit = getattr(self, "_project_git_commit", None)
+        if commit is None:
+            commit, return_code, _ = run("git rev-parse HEAD", verbose=True)
+            commit = commit.strip("\n")
+            if return_code != 0:
+                commit = False
+            self._project_git_commit = commit
+        return commit
+
+
     def _revert_background_image(self):
         """
         Revert background image to the before-test state.
 
         .. note::
 
             Do **NOT** call this by yourself. This method is called by :func:`after_scenario`.
@@ -1473,15 +1756,15 @@
         else:
             assert False, "".join((
                 "Unknown option, only defined ones are 'show' or 'hide'.",
                 f"You tried to use: '{action}'"
             ))
 
 
-    #Using properties to preserve old api of attributes
+    # Using properties to preserve old api of attributes.
     @property
     def recordVideo(self):
         return self.record_video
     @recordVideo.setter
     def recordVideo(self, value):
         self.record_video = value
```

### Comparing `qecore-3.8/qecore/step_matcher.py` & `qecore-3.9/qecore/step_matcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         :type pattern: str
         :param pattern: Decorator of step function.
 
         :type step_type: str
         :param step_type: Type of behave step.
         """
         super(QecoreMatcher, self).__init__(func, pattern, step_type)
-        # note the space at the end of patterns (to make sure whole words are matched)
+        # Note the space at the end of patterns (to make sure whole words are matched).
         self.patterns = [f"{self.start_phrase}{p.strip()} " for p in pattern.split(self.delimiter)]
         self.parsers = {}
         for patt in self.patterns:
             self.parsers[patt] = self.parser_class(patt, self.custom_types)
 
 
     def check_match(self, step):
@@ -83,17 +83,17 @@
         :type step: str
         :param step: Step definiton to be matched
 
         :return: List of matched arguments if `step` matches, `None` otherwise.
         """
 
         args = []
-        # escaped quotes and append space (because patterns end with space)
+        # Escaped quotes and append space (because patterns end with space).
         step_suffix = self.start_phrase + step.replace('\\"', "''") + " "
-        # to calculate positions in step argument - used for keword highlights
+        # To calculate positions in step argument - used for keword highlights.
         offset = - len(self.start_phrase)
 
 
         def fix_escape_quotes(value, text_repr):
             """
             Replace two consecutive single qoutes ('') back to double quote.
             Do not escape double quotes.
@@ -139,44 +139,44 @@
                 start, end = result.spans[index]
                 value, text_repr = fix_escape_quotes(value, step_suffix[start:end])
                 args.append(Argument(start+offset, end+offset, text_repr, value))
             for name, value in result.named.items():
                 start, end = result.spans[name]
                 value, text_repr = fix_escape_quotes(value, step_suffix[start:end])
                 args.append(Argument(start+offset, end+offset, text_repr, value, name))
-            # matched part of the step
+            # Matched part of the step.
             pattern_filled = pattern.format_map(result.named)
-            # remove matched part and append start_phrase
+            # Remove matched part and append start_phrase.
             old_len = len(step_suffix)
             step_suffix = self.start_phrase + step_suffix.replace(pattern_filled, "").lstrip(" |")
             new_len = len(step_suffix)
-            # calculate offset
+            # Calculate offset.
             offset += old_len - new_len
             return (step_suffix, offset, args)
 
-        # check that the first part is first, finish if step does not match
+        # Check that the first part is first, finish if step does not match.
         pattern = self.patterns[0]
         if len(self.patterns) == 1:
             result = self.parsers[pattern].parse(step_suffix)
         else:
             result = self.parsers[pattern].search(step_suffix)
 
         if result is None:
             return None
         step_suffix, offset, args = process_result(step_suffix, offset, args, result, pattern)
 
-        # match rest of the step
+        # Match rest of the step.
         patterns = self.patterns[1:]
         while len(step_suffix) > len(self.start_phrase):
             found = False
             for pattern in patterns:
                 result = self.parsers[pattern].search(step_suffix)
                 if result is None:
                     continue
-                # remove pattern as it was used
+                # Remove pattern as it was used.
                 patterns.remove(pattern)
                 step_suffix, offset, args = process_result(step_suffix, offset,
                                                            args, result, pattern)
                 found = True
             if not found:
                 return None
```

### Comparing `qecore-3.8/qecore/utility.py` & `qecore-3.9/qecore/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,19 @@
     .. note::
 
         Do **NOT** call this by yourself. This function is called by :mod:`common_steps`.
     """
 
     app_class_to_return = None
     try:
-        app_class_to_return = getattr(context, application) # get app from environment file
+        # Get app from environment file.
+        app_class_to_return = getattr(context, application)
     except AttributeError:
-        for app in context.sandbox.applications: # get app from sandbox application list
+        # Get app from sandbox application list.
+        for app in context.sandbox.applications:
             if app.component == application:
                 app_class_to_return = app
                 break
     except TypeError:
         app_class_to_return = context.sandbox.default_application
         assert context.sandbox.default_application is not None, "\n".join((
             "Default application was not found. Check your environment file!"
@@ -135,15 +137,15 @@
 
     context.embed("text/plain", f"$?={return_code}", caption=f"{command} result")
     context.embed("text/plain", output, caption=f"{command} output")
 
     return (error.output, error.returncode, error)
 
 
-#behave-common-steps leftover
+# behave-common-steps leftover.
 def wait_until(tested, element=None, timeout=30, period=0.25, params_in_list=False):
     """
     This function keeps running lambda with specified params until the
     result is True or timeout is reached. Instead of lambda, Boolean variable
     can be used instead.
 
     Sample usages::
@@ -160,33 +162,33 @@
         >>> wait_until(dialog.dead)
         Wait until the dialog is dead
 
     """
 
     if isinstance(tested, bool):
         curried_func = lambda: tested
-    # or if callable(tested) and element is a list or a tuple
+    # Or if callable(tested) and element is a list or a tuple.
     elif isinstance(tested, FunctionType) and \
             isinstance(element, (tuple, list)) and params_in_list:
         curried_func = partial(tested, *element)
-    # or if callable(tested) and element is not None?
+    # Or if callable(tested) and element is not None?
     elif isinstance(tested, FunctionType) and element is not None:
         curried_func = partial(tested, element)
     else:
         curried_func = tested
 
     exception_thrown = None
     mustend = int(time()) + timeout
     while int(time()) < mustend:
         try:
             if curried_func():
                 return True
         except Exception as error:  # pylint: disable=broad-except
             # If lambda has thrown the exception we'll re-raise it later
-            # and forget about if lambda passes
+            # and forget about if lambda passes.
             exception_thrown = error
         sleep(period)
     if exception_thrown is not None:
         raise exception_thrown  # pylint: disable=raising-bad-type
     else:
         return False
 
@@ -288,13 +290,12 @@
 
     def crawl(node, depth):
         dump(node, depth)
         for child in node.children:
             crawl(child, depth + 1)
 
     def dump_std_out(item, depth):
-        # str wont possibly work in p3
         print(SPACER * depth + str(item) + \
             f"     [p:{item.position}, s:{item.size}, vis:{item.visible}, show:{item.showing}]")
 
     dump = dump_std_out
     crawl(node, 0)
```

### Comparing `qecore-3.8/qecore.egg-info/SOURCES.txt` & `qecore-3.9/qecore.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 setup.py
 __testing__/__init__.py
 __testing__/api.py
+__testing__/coredump.py
 __testing__/reproducer.py
 __testing__/z.py
 qecore/__init__.py
 qecore/application.py
 qecore/common_steps.py
 qecore/flatpak.py
 qecore/get_node.py
@@ -20,12 +21,13 @@
 qecore.egg-info/SOURCES.txt
 qecore.egg-info/dependency_links.txt
 qecore.egg-info/requires.txt
 qecore.egg-info/top_level.txt
 scripts/qecore
 scripts/qecore-headless
 scripts/qecore-runtest
+scripts/qecore_backtrace_from_coredump
 scripts/qecore_bash_completion
 scripts/qecore_get_active_display
 scripts/qecore_help
 scripts/qecore_start_keyring
 scripts/qecore_start_recording
```

### Comparing `qecore-3.8/scripts/qecore` & `qecore-3.9/scripts/qecore`

 * *Files identical despite different names*

### Comparing `qecore-3.8/scripts/qecore-headless` & `qecore-3.9/scripts/qecore-headless`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     at_spi_result = run(at_spi_command)
     print("".join((
         "\nExpecting running processes to be\n",
         "'/usr/libexec/at-spi-bus-launcher'\n",
         "'/usr/libexec/at-spi2-registryd'\n"
     )))
     print(f"Actual running processes:\n'{at_spi_result}'")
-    
+
     # Important variables
     display = os.getenv("DISPLAY")
     xauthority = os.getenv("XAUTHORITY")
     dbus_session_bus_address = os.getenv("DBUS_SESSION_BUS_ADDRESS")
     print("".join((
         f"\nDISPLAY = '{display}'"
         f"\nXAUTHORITY = '{xauthority}'"
@@ -113,19 +113,19 @@
     )))
 
 
 def verify_file_ownership():
     # Verify ownership of the dconf file.
     user_id = os.getuid()
     file_owner_command = f"sudo stat -c '%U %G' /run/user/{user_id}/dconf/user"
-    
+
     if not os.path.isfile(f"/run/user/{user_id}/dconf/user"):
         return
-    
-    file_owner_command_result = run(file_owner_command, verbose=True)    
+
+    file_owner_command_result = run(file_owner_command, verbose=True)
 
     if file_owner_command_result[1] == 0 and "root" in file_owner_command_result[0]:
         print("headless: Attempting to restore dconf file ownership.")
         run(f"sudo rm -rf /run/user/{user_id}/dconf/user")
     elif file_owner_command_result[1] != 0:
         print(f"headless: Issue was detected and might need attention - {file_owner_command_result}")
 
@@ -187,15 +187,15 @@
         self.enable_stop = enable_stop
         self.gdm_restart = gdm_restart
 
         self.display_manager = "gdm"
         self.session_type = session_type # xorg, wayland, None -> respect setting of the system
         self.session_desktop = session_desktop # gnome gnome-classic, None -> respect setting of the system
         self.session_started_indicator = "/usr/libexec/gnome-session-binary"
-        
+
         self.user = run("whoami")
         self.user_id = run(f"id -u {self.user}")
 
         self.config_file = "/etc/gdm/custom.conf"
         self.temporary_config_file = f"/tmp/{os.path.basename(self.config_file)}"
 
         self.restart_needed = False
@@ -336,15 +336,15 @@
 
         # Start gdm if gdm is not active already.
         is_display_manager_active = run("systemctl is-active gdm")
         if is_display_manager_active != "active":
             print("headless: Starting Display Manager")
             run("sudo systemctl start gdm")
             time.sleep(4)
-        
+
         # But the session must be running.
         if not self.wait_until_process_is_running(self.session_started_indicator):
             print("headless: Running session indicator not detected running - restart required")
             print("headless: Attempt to restore headless - stopping gdm")
             run("sudo systemctl stop gdm")
             print("headless: Attempt to restore headless - starting gdm")
             run("sudo systemctl start gdm")
```

### Comparing `qecore-3.8/scripts/qecore_start_keyring` & `qecore-3.9/scripts/qecore_start_keyring`

 * *Files identical despite different names*

### Comparing `qecore-3.8/setup.py` & `qecore-3.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     for file in scripts_list:
         result = result + ["scripts/" + file]
     return result
 
 
 setuptools.setup(
     name="qecore",
-    version="3.8",
+    version="3.9",
     author="Michal Odehnal",
     author_email="modehnal@redhat.com",
     description="DesktopQE Tool for unified test execution",
     url="https://gitlab.com/dogtail/qecore",
     packages=setuptools.find_packages(),
     scripts=scripts(),
     install_requires=["behave",
```

