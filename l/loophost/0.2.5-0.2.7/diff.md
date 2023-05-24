# Comparing `tmp/loophost-0.2.5.tar.gz` & `tmp/loophost-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loophost-0.2.5.tar", max compression
+gzip compressed data, was "loophost-0.2.7.tar", max compression
```

## Comparing `loophost-0.2.5.tar` & `loophost-0.2.7.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0       68 2023-05-22 20:54:45.002992 loophost-0.2.5/README.md
--rw-r--r--   0        0        0        5 2023-05-22 23:20:34.487182 loophost-0.2.5/VERSION
--rw-r--r--   0        0        0      666 2023-05-20 06:37:17.640351 loophost-0.2.5/build.py
--rw-r--r--   0        0        0      669 2023-05-22 23:20:37.041067 loophost-0.2.5/loophost/__init__.py
--rw-r--r--   0        0        0     3370 2023-05-22 20:58:52.834903 loophost-0.2.5/loophost/flingroute.py
--rw-r--r--   0        0        0     1029 2023-05-22 23:20:15.232936 loophost-0.2.5/loophost/launchd_plist.py
--rwxr-xr-x   0        0        0  8301536 2023-05-22 21:35:10.810528 loophost-0.2.5/loophost/loopproxy
--rw-r--r--   0        0        0      904 2023-05-22 21:02:29.003769 loophost-0.2.5/loophost/plist/hub.plist.template
--rw-r--r--   0        0        0      771 2023-05-22 20:59:18.324250 loophost-0.2.5/loophost/plist/loophost.plist.template
--rw-r--r--   0        0        0     1249 2023-05-22 22:47:19.211207 loophost-0.2.5/loophost/plist/ssh.plist.template
--rw-r--r--   0        0        0     3532 2023-05-22 23:04:25.023331 loophost-0.2.5/loophost/postinstall.py
--rw-r--r--   0        0        0    95159 2023-04-07 23:50:14.944549 loophost-0.2.5/loophost/static/fling-logo-dark.png
--rw-r--r--   0        0        0   265670 2023-04-08 00:23:03.250215 loophost-0.2.5/loophost/static/fling-logo-light.png
--rw-r--r--   0        0        0     3834 2023-05-12 22:43:40.802704 loophost-0.2.5/loophost/static/logo-hc.txt
--rw-r--r--   0        0        0    34153 2023-05-21 23:31:29.960428 loophost-0.2.5/loophost/static/logo-square.png
--rw-r--r--   0        0        0     1759 2023-05-22 18:09:46.308757 loophost-0.2.5/loophost/templates/admin.html
--rw-r--r--   0        0        0     2667 2023-05-21 23:39:30.263833 loophost-0.2.5/loophost/templates/local.html
--rw-r--r--   0        0        0     1476 2023-05-22 19:26:55.811597 loophost-0.2.5/loophost/templates/partials/apptable.html
--rw-r--r--   0        0        0      289 2023-05-21 21:12:35.820099 loophost-0.2.5/loophost/templates/partials/upgrade.html
--rw-r--r--   0        0        0     1167 2023-05-22 23:20:27.101419 loophost-0.2.5/pyproject.toml
--rw-r--r--   0        0        0       39 2023-05-20 00:34:26.794307 loophost-0.2.5/setup.py
--rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 loophost-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0       68 2023-05-22 20:54:45.002992 loophost-0.2.7/README.md
+-rw-r--r--   0        0        0        5 2023-05-23 06:12:41.204649 loophost-0.2.7/VERSION
+-rw-r--r--   0        0        0      666 2023-05-20 06:37:17.640351 loophost-0.2.7/build.py
+-rw-r--r--   0        0        0      669 2023-05-23 06:12:46.289089 loophost-0.2.7/loophost/__init__.py
+-rw-r--r--   0        0        0     3679 2023-05-23 00:49:51.617384 loophost-0.2.7/loophost/flingroute.py
+-rw-r--r--   0        0        0     1281 2023-05-23 04:59:46.905055 loophost-0.2.7/loophost/launchd_plist.py
+-rwxr-xr-x   0        0        0  8045858 2023-05-23 06:12:56.942402 loophost-0.2.7/loophost/loopproxy
+-rw-r--r--   0        0        0      904 2023-05-22 21:02:29.003769 loophost-0.2.7/loophost/plist/hub.plist.template
+-rw-r--r--   0        0        0      771 2023-05-22 20:59:18.324250 loophost-0.2.7/loophost/plist/loophost.plist.template
+-rw-r--r--   0        0        0     1150 2023-05-23 00:41:15.244678 loophost-0.2.7/loophost/plist/ssh.plist.template
+-rw-r--r--   0        0        0     3739 2023-05-23 04:54:00.628797 loophost-0.2.7/loophost/postinstall.py
+-rw-r--r--   0        0        0    95159 2023-04-07 23:50:14.944549 loophost-0.2.7/loophost/static/fling-logo-dark.png
+-rw-r--r--   0        0        0   265670 2023-04-08 00:23:03.250215 loophost-0.2.7/loophost/static/fling-logo-light.png
+-rw-r--r--   0        0        0     3834 2023-05-12 22:43:40.802704 loophost-0.2.7/loophost/static/logo-hc.txt
+-rw-r--r--   0        0        0    34153 2023-05-21 23:31:29.960428 loophost-0.2.7/loophost/static/logo-square.png
+-rw-r--r--   0        0        0     1759 2023-05-22 18:09:46.308757 loophost-0.2.7/loophost/templates/admin.html
+-rw-r--r--   0        0        0     2667 2023-05-21 23:39:30.263833 loophost-0.2.7/loophost/templates/local.html
+-rw-r--r--   0        0        0     1476 2023-05-22 19:26:55.811597 loophost-0.2.7/loophost/templates/partials/apptable.html
+-rw-r--r--   0        0        0      289 2023-05-21 21:12:35.820099 loophost-0.2.7/loophost/templates/partials/upgrade.html
+-rw-r--r--   0        0        0     1604 2023-05-23 04:10:54.125164 loophost-0.2.7/loophost/uninstall.py
+-rw-r--r--   0        0        0     1187 2023-05-23 06:12:36.179597 loophost-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-05-20 00:34:26.794307 loophost-0.2.7/setup.py
+-rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 loophost-0.2.7/PKG-INFO
```

### Comparing `loophost-0.2.5/build.py` & `loophost-0.2.7/build.py`

 * *Files identical despite different names*

### Comparing `loophost-0.2.5/loophost/__init__.py` & `loophost-0.2.7/loophost/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2.5'
+__version__ = '0.2.7'
 
 import os
 import pathlib
 import sys
 
 
 LOOPHOST_DOMAIN = "loophost.dev"
```

### Comparing `loophost-0.2.5/loophost/flingroute.py` & `loophost-0.2.7/loophost/flingroute.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import json
 import pathlib
 from fling.start import start
 from flask import Flask, request, render_template, redirect
 from flask_bootstrap import Bootstrap5
 from flask_caching import Cache
-from loophost.launchd_plist import register_tunnel, unregister_tunnel
+from loophost.launchd_plist import register_tunnel, unregister_tunnel, generate_keys
 from loophost import HUBDIR, __version__, DATA_FILE_PATH
 from lastversion import has_update
 from fling_cli import get_fling_client
 from fling_client.api.loophost import expose_app_expose_app_put
 
 
 config = json.loads(pathlib.Path.read_text(DATA_FILE_PATH))
@@ -53,23 +53,32 @@
     project = request.args.get("project")
     target = pathlib.Path(
         pathlib.Path.home(),
         "Library",
         "LaunchAgents",
         f"dev.fling.hub.ssh.{project}.plist",
     )
+
+    if not os.path.exists("tunnelkey.pub"):
+        # TODO(JMC): Don't do this so often
+        fling_client = get_fling_client(require_auth=True)
+        pub, priv = generate_keys()
+        with open("tunnelkey.pub", "w+") as pubfile:
+            pubfile.write(pub)
+        with open("tunnelkey", "w+") as privfile:
+            privfile.write(priv)
+        os.chmod("tunnelkey", 0o600)
+        expose_app_expose_app_put.sync(client=fling_client, app_name=project, ssh_public_key=pub)
+
     if project and project in config.get("share", {}):
         del config["share"][project]
         unregister_tunnel(target)
     elif project:
         if not config.get("share"):
             config["share"] = {}
-            # TODO(JMC): Don't do this so often
-            fling_client = get_fling_client(require_auth=True)
-            expose_app_expose_app_put.sync(client=fling_client, app_name=project)
         config["share"][project] = "public"
         register_tunnel(
             project, pathlib.Path(HUBDIR, "plist", "ssh.plist.template"), target
         )
     with open(DATA_FILE_PATH, "w+") as appjson:
         appjson.write(json.dumps(config))
     return redirect("/")
```

### Comparing `loophost-0.2.5/loophost/launchd_plist.py` & `loophost-0.2.7/loophost/launchd_plist.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,21 @@
+from io import StringIO
 import pathlib
 import shutil
 from loophost import LOOPHOST_DOMAIN, TUNNEL_DOMAIN, TARGET_DIR, PYEX, HUBDIR, USERNAME
 from string import Template
 from subprocess import run
+import paramiko
+
+
+def generate_keys():
+    key = paramiko.RSAKey.generate(2048)
+    privateString = StringIO()
+    key.write_private_key(privateString)
+    return f"{key.get_name()} {key.get_base64()}", privateString.getvalue()
 
 
 def register_tunnel(project, template_path, target_path):
     shutil.copy2(template_path, TARGET_DIR)
 
     d = {"CWD": TARGET_DIR,
          "USERNAME": USERNAME,
```

### Comparing `loophost-0.2.5/loophost/plist/hub.plist.template` & `loophost-0.2.7/loophost/plist/hub.plist.template`

 * *Files identical despite different names*

### Comparing `loophost-0.2.5/loophost/plist/loophost.plist.template` & `loophost-0.2.7/loophost/plist/loophost.plist.template`

 * *Files identical despite different names*

### Comparing `loophost-0.2.5/loophost/plist/ssh.plist.template` & `loophost-0.2.7/loophost/plist/ssh.plist.template`

 * *Files 7% similar despite different names*

#### Comparing `loophost-0.2.5/loophost/plist/ssh.plist.template` & `loophost-0.2.7/loophost/plist/ssh.plist.template`

```diff
@@ -5,22 +5,20 @@
 <plist version="1.0">
   <dict>
     <key>Label</key>
     <string>dev.fling.hub.ssh.${PROJECT}</string>
     <key>ProgramArguments</key>
     <array>
       <string>ssh</string>
-      <string>-F</string>
-      <string>/Users/${LOCAL_USER}/.ssh/config</string>
       <string>-o ServerAliveInterval=60</string>
       <string>-o ExitOnForwardFailure=yes</string>
       <string>-o UserKnownHostsFile=/dev/null</string>
       <string>-o StrictHostKeyChecking=no</string>
       <string>-i</string>
-      <string>/Users/${LOCAL_USER}/.ssh/id_rsa</string>
+      <string>${CWD}/tunnelkey</string>
       <string>-p 2222</string>
       <string>-R ${PROJECT}:443:localhost:4433</string>
       <string>${USERNAME}@${TUNNEL_DOMAIN}</string>
     </array>
     <key>WorkingDirectory</key>
     <string>${CWD}</string>
     <key>UserName</key>
```

### Comparing `loophost-0.2.5/loophost/postinstall.py` & `loophost-0.2.7/loophost/postinstall.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,20 +13,23 @@
     HUBDIR,
     USERNAME,
     DATA_FILE_PATH,
 )
 
 
 def post_install_one():
+    global USERNAME
     print("Installing LoopHost...")
-    os.makedirs(pathlib.Path(TARGET_DIR, "certs"), exist_ok=True)
+    os.makedirs(pathlib.Path(TARGET_DIR), exist_ok=True)
     os.chdir(TARGET_DIR)
     with open("localuser.txt", "w+") as userfile:
         userfile.write(os.getenv("USER"))
     authenticate_with_fling()
+    with open(pathlib.Path(TARGET_DIR, "flinguser.txt"), "r") as userfile:
+        USERNAME = userfile.read()
     issue_certs()
     create_update_loophost_json()
     register_tunnel(
         "flinghub",
         pathlib.Path(HUBDIR, "plist", "loophost.plist.template"),
         pathlib.Path(
             pathlib.Path.home(), "Library/LaunchAgents/dev.fling.hub.local.plist"
@@ -61,14 +64,15 @@
             "--logs-dir ./",
             "--non-interactive",
             "--expand",
             "--agree-tos",
             f"-m webmaster@{LOOPHOST_DOMAIN}",
             "--authenticator=fling_authenticator",
             f'-d "*.{USERNAME}.{LOOPHOST_DOMAIN}"',
+            f'-d "*.{USERNAME}.{TUNNEL_DOMAIN}"',
             f'-d "{USERNAME}.{LOOPHOST_DOMAIN}"',
             # "--force-renewal",
             "--fling_authenticator-propagation-seconds=15",
         ]
     )
     print(cmd)
     run(
@@ -108,15 +112,16 @@
     )
     print("All done.")
 
 
 def restart_as_sudo():
     global USERNAME
     print(
-        "Switching to root user to install web services (you will be prompted for your password)"
+        """Switching to root user to install web services on ports 443 and 80\n\r
+        (you will be prompted for your password)"""
     )
     run(
         "sudo python3 -m loophost.postinstall",
         shell=True,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         stdin=subprocess.PIPE,
```

### Comparing `loophost-0.2.5/loophost/static/fling-logo-dark.png` & `loophost-0.2.7/loophost/static/fling-logo-dark.png`

 * *Files identical despite different names*

### Comparing `loophost-0.2.5/loophost/static/fling-logo-light.png` & `loophost-0.2.7/loophost/static/fling-logo-light.png`

 * *Files identical despite different names*

### Comparing `loophost-0.2.5/loophost/static/logo-hc.txt` & `loophost-0.2.7/loophost/static/logo-hc.txt`

 * *Files identical despite different names*

### Comparing `loophost-0.2.5/loophost/static/logo-square.png` & `loophost-0.2.7/loophost/static/logo-square.png`

 * *Files identical despite different names*

### Comparing `loophost-0.2.5/loophost/templates/admin.html` & `loophost-0.2.7/loophost/templates/admin.html`

 * *Files identical despite different names*

### Comparing `loophost-0.2.5/loophost/templates/local.html` & `loophost-0.2.7/loophost/templates/local.html`

 * *Files identical despite different names*

### Comparing `loophost-0.2.5/loophost/templates/partials/apptable.html` & `loophost-0.2.7/loophost/templates/partials/apptable.html`

 * *Files identical despite different names*

### Comparing `loophost-0.2.5/pyproject.toml` & `loophost-0.2.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "poetry>=0.12", "setuptools", "wheel", "setuptools-cpp", "setuptools-golang"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "loophost"
-version = "0.2.5"
+version = "0.2.7"
 description = "Loophost: for a better local dev"
 authors = [
     "Joshua McKenty <jmckenty@gmail.com>",
 ]
 readme = "README.md"
 license = "Apache-2.0"
 include = [{ path = "VERSION" }, 
@@ -31,12 +31,13 @@
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 setuptools = "*"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-fling-start = "^0.1.13"
+fling-start = "^0.1.14"
 fling-cli = "^0.1.5"
 certbot = "^2.6.0"
 flask = "^2.3.2"
 lastversion = "^2.4.15"
+paramiko = "^3.1.0"
```

### Comparing `loophost-0.2.5/PKG-INFO` & `loophost-0.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: loophost
-Version: 0.2.5
+Version: 0.2.7
 Summary: Loophost: for a better local dev
 License: Apache-2.0
 Author: Joshua McKenty
 Author-email: jmckenty@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: certbot (>=2.6.0,<3.0.0)
 Requires-Dist: flask (>=2.3.2,<3.0.0)
 Requires-Dist: fling-cli (>=0.1.5,<0.2.0)
-Requires-Dist: fling-start (>=0.1.13,<0.2.0)
+Requires-Dist: fling-start (>=0.1.14,<0.2.0)
 Requires-Dist: lastversion (>=2.4.15,<3.0.0)
+Requires-Dist: paramiko (>=3.1.0,<4.0.0)
 Project-URL: documentation, https://readthedocs.org/loophost
 Project-URL: homepage, https://loophost.dev
 Project-URL: repository, https://github.com/delving-co/loophost.git
 Description-Content-Type: text/markdown
 
 # Loophost
 ### The secure local web dev experience you always wanted
```

