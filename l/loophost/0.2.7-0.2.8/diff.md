# Comparing `tmp/loophost-0.2.7.tar.gz` & `tmp/loophost-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loophost-0.2.7.tar", max compression
+gzip compressed data, was "loophost-0.2.8.tar", max compression
```

## Comparing `loophost-0.2.7.tar` & `loophost-0.2.8.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0       68 2023-05-22 20:54:45.002992 loophost-0.2.7/README.md
--rw-r--r--   0        0        0        5 2023-05-23 06:12:41.204649 loophost-0.2.7/VERSION
--rw-r--r--   0        0        0      666 2023-05-20 06:37:17.640351 loophost-0.2.7/build.py
--rw-r--r--   0        0        0      669 2023-05-23 06:12:46.289089 loophost-0.2.7/loophost/__init__.py
--rw-r--r--   0        0        0     3679 2023-05-23 00:49:51.617384 loophost-0.2.7/loophost/flingroute.py
--rw-r--r--   0        0        0     1281 2023-05-23 04:59:46.905055 loophost-0.2.7/loophost/launchd_plist.py
--rwxr-xr-x   0        0        0  8045858 2023-05-23 06:12:56.942402 loophost-0.2.7/loophost/loopproxy
--rw-r--r--   0        0        0      904 2023-05-22 21:02:29.003769 loophost-0.2.7/loophost/plist/hub.plist.template
--rw-r--r--   0        0        0      771 2023-05-22 20:59:18.324250 loophost-0.2.7/loophost/plist/loophost.plist.template
--rw-r--r--   0        0        0     1150 2023-05-23 00:41:15.244678 loophost-0.2.7/loophost/plist/ssh.plist.template
--rw-r--r--   0        0        0     3739 2023-05-23 04:54:00.628797 loophost-0.2.7/loophost/postinstall.py
--rw-r--r--   0        0        0    95159 2023-04-07 23:50:14.944549 loophost-0.2.7/loophost/static/fling-logo-dark.png
--rw-r--r--   0        0        0   265670 2023-04-08 00:23:03.250215 loophost-0.2.7/loophost/static/fling-logo-light.png
--rw-r--r--   0        0        0     3834 2023-05-12 22:43:40.802704 loophost-0.2.7/loophost/static/logo-hc.txt
--rw-r--r--   0        0        0    34153 2023-05-21 23:31:29.960428 loophost-0.2.7/loophost/static/logo-square.png
--rw-r--r--   0        0        0     1759 2023-05-22 18:09:46.308757 loophost-0.2.7/loophost/templates/admin.html
--rw-r--r--   0        0        0     2667 2023-05-21 23:39:30.263833 loophost-0.2.7/loophost/templates/local.html
--rw-r--r--   0        0        0     1476 2023-05-22 19:26:55.811597 loophost-0.2.7/loophost/templates/partials/apptable.html
--rw-r--r--   0        0        0      289 2023-05-21 21:12:35.820099 loophost-0.2.7/loophost/templates/partials/upgrade.html
--rw-r--r--   0        0        0     1604 2023-05-23 04:10:54.125164 loophost-0.2.7/loophost/uninstall.py
--rw-r--r--   0        0        0     1187 2023-05-23 06:12:36.179597 loophost-0.2.7/pyproject.toml
--rw-r--r--   0        0        0       39 2023-05-20 00:34:26.794307 loophost-0.2.7/setup.py
--rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 loophost-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0       68 2023-05-22 20:54:45.002992 loophost-0.2.8/README.md
+-rw-r--r--   0        0        0        5 2023-05-23 23:58:56.663830 loophost-0.2.8/VERSION
+-rw-r--r--   0        0        0      666 2023-05-20 06:37:17.640351 loophost-0.2.8/build.py
+-rw-r--r--   0        0        0      669 2023-05-23 23:58:53.657355 loophost-0.2.8/loophost/__init__.py
+-rw-r--r--   0        0        0     3762 2023-05-23 22:36:10.606608 loophost-0.2.8/loophost/flingroute.py
+-rw-r--r--   0        0        0     1281 2023-05-23 04:59:46.905055 loophost-0.2.8/loophost/launchd_plist.py
+-rwxr-xr-x   0        0        0  8045858 2023-05-23 06:12:56.942402 loophost-0.2.8/loophost/loopproxy
+-rw-r--r--   0        0        0      904 2023-05-22 21:02:29.003769 loophost-0.2.8/loophost/plist/hub.plist.template
+-rw-r--r--   0        0        0      771 2023-05-22 20:59:18.324250 loophost-0.2.8/loophost/plist/loophost.plist.template
+-rw-r--r--   0        0        0     1150 2023-05-23 00:41:15.244678 loophost-0.2.8/loophost/plist/ssh.plist.template
+-rw-r--r--   0        0        0     3739 2023-05-23 04:54:00.628797 loophost-0.2.8/loophost/postinstall.py
+-rw-r--r--   0        0        0    95159 2023-04-07 23:50:14.944549 loophost-0.2.8/loophost/static/fling-logo-dark.png
+-rw-r--r--   0        0        0   265670 2023-04-08 00:23:03.250215 loophost-0.2.8/loophost/static/fling-logo-light.png
+-rw-r--r--   0        0        0     3834 2023-05-12 22:43:40.802704 loophost-0.2.8/loophost/static/logo-hc.txt
+-rw-r--r--   0        0        0    34153 2023-05-21 23:31:29.960428 loophost-0.2.8/loophost/static/logo-square.png
+-rw-r--r--   0        0        0      828 2023-05-23 21:16:55.287812 loophost-0.2.8/loophost/templates/admin.html
+-rw-r--r--   0        0        0     1606 2023-05-23 21:15:55.482064 loophost-0.2.8/loophost/templates/base.html
+-rw-r--r--   0        0        0     1257 2023-05-23 21:14:15.086302 loophost-0.2.8/loophost/templates/local.html
+-rw-r--r--   0        0        0     1474 2023-05-23 21:13:30.120822 loophost-0.2.8/loophost/templates/partials/apptable.html
+-rw-r--r--   0        0        0      289 2023-05-21 21:12:35.820099 loophost-0.2.8/loophost/templates/partials/upgrade.html
+-rw-r--r--   0        0        0     1604 2023-05-23 04:10:54.125164 loophost-0.2.8/loophost/uninstall.py
+-rw-r--r--   0        0        0     1187 2023-05-23 23:59:02.011715 loophost-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-05-20 00:34:26.794307 loophost-0.2.8/setup.py
+-rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 loophost-0.2.8/PKG-INFO
```

### Comparing `loophost-0.2.7/build.py` & `loophost-0.2.8/build.py`

 * *Files identical despite different names*

### Comparing `loophost-0.2.7/loophost/flingroute.py` & `loophost-0.2.8/loophost/flingroute.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,17 @@
         fling_client = get_fling_client(require_auth=True)
         pub, priv = generate_keys()
         with open("tunnelkey.pub", "w+") as pubfile:
             pubfile.write(pub)
         with open("tunnelkey", "w+") as privfile:
             privfile.write(priv)
         os.chmod("tunnelkey", 0o600)
-        expose_app_expose_app_put.sync(client=fling_client, app_name=project, ssh_public_key=pub)
+        expose_app_expose_app_put.sync(
+            client=fling_client, app_name=project, ssh_public_key=pub
+        )
 
     if project and project in config.get("share", {}):
         del config["share"][project]
         unregister_tunnel(target)
     elif project:
         if not config.get("share"):
             config["share"] = {}
@@ -80,38 +82,41 @@
             project, pathlib.Path(HUBDIR, "plist", "ssh.plist.template"), target
         )
     with open(DATA_FILE_PATH, "w+") as appjson:
         appjson.write(json.dumps(config))
     return redirect("/")
 
 
+@admin.route("/config/<project>", methods=["GET", "POST"])
+def config_page(project):
+    if request.form.get("application_port"):
+        config["apps"][project] = request.form.get("application_port")
+        with open(DATA_FILE_PATH, "w+") as appjson:
+            appjson.write(json.dumps(config))
+
+    return render_template(
+        "local.html",
+        config=config,
+        apps=config["apps"],
+        share=config.get("share"),
+        project=project,
+    )
+
+
 @admin.route("/", defaults={"path": ""}, methods=["GET", "POST"])
 @admin.route("/<path:path>", methods=["GET", "POST"])
 def admin_page(path):
     fqdn = request.host.split(".")
     if len(fqdn) < 4:
         return render_template(
             "admin.html",
             config=config,
             apps=config["apps"],
             share=config.get("share"),
             fqdn=".".join(fqdn),
         )
     project = fqdn.pop(0)
-    if request.form.get("application_port"):
-        config["apps"][project] = request.form.get("application_port")
-        with open(DATA_FILE_PATH, "w+") as appjson:
-            appjson.write(json.dumps(config))
-        return redirect(f"https://{project}.{'.'.join(fqdn)}")
-
-    return render_template(
-        "local.html",
-        config=config,
-        apps=config["apps"],
-        share=config.get("share"),
-        project=project,
-        fqdn=".".join(fqdn),
-    )
+    return redirect(f"https://{config['fqdn']}/config/{project}")
 
 
 if __name__ == "__main__":
     admin.run(host=f"unix://{os.getcwd()}/loophost.soc")
```

### Comparing `loophost-0.2.7/loophost/launchd_plist.py` & `loophost-0.2.8/loophost/launchd_plist.py`

 * *Files identical despite different names*

### Comparing `loophost-0.2.7/loophost/loopproxy` & `loophost-0.2.8/loophost/loopproxy`

 * *Files identical despite different names*

### Comparing `loophost-0.2.7/loophost/plist/hub.plist.template` & `loophost-0.2.8/loophost/plist/hub.plist.template`

 * *Files identical despite different names*

### Comparing `loophost-0.2.7/loophost/plist/loophost.plist.template` & `loophost-0.2.8/loophost/plist/loophost.plist.template`

 * *Files identical despite different names*

### Comparing `loophost-0.2.7/loophost/plist/ssh.plist.template` & `loophost-0.2.8/loophost/plist/ssh.plist.template`

 * *Files identical despite different names*

### Comparing `loophost-0.2.7/loophost/postinstall.py` & `loophost-0.2.8/loophost/postinstall.py`

 * *Files identical despite different names*

### Comparing `loophost-0.2.7/loophost/static/fling-logo-dark.png` & `loophost-0.2.8/loophost/static/fling-logo-dark.png`

 * *Files identical despite different names*

### Comparing `loophost-0.2.7/loophost/static/fling-logo-light.png` & `loophost-0.2.8/loophost/static/fling-logo-light.png`

 * *Files identical despite different names*

### Comparing `loophost-0.2.7/loophost/static/logo-hc.txt` & `loophost-0.2.8/loophost/static/logo-hc.txt`

 * *Files identical despite different names*

### Comparing `loophost-0.2.7/loophost/static/logo-square.png` & `loophost-0.2.8/loophost/static/logo-square.png`

 * *Files identical despite different names*

### Comparing `loophost-0.2.7/loophost/templates/partials/apptable.html` & `loophost-0.2.8/loophost/templates/partials/apptable.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-<div>
-        Your local apps:<br/>
+<div class="p-2">
+        <h1>Your local apps:</h1>
         {% if not apps %}
             <h2>No local apps set up yet!</h2>
         {% else %}
         <div class="table-responsive">
                 <table class="table-dark table table-bordered table-striped table-hover">
                 <thead>
                         <tr>
                         <th scope="col">Project Name</th>
                         <th scope="col">Location</th>
                         <th scope="col">Toggle Sharing</th>
-                        <th scope="col">Unbind?</th>
+                        <th scope="col">Config</th>
                         </tr>
                         </thead>
                         <tbody>
         {% for x in apps %}
         <tr>
                 <th scope="row"><a href="https://{{x}}.{{fqdn}}">{{x}}</a>&nbsp;&nbsp;
                 {% if share[x] %} <a href="https://{{x}}.{{config["tunnel"]}}">(shareable)</a>  {% endif %}
@@ -23,16 +23,15 @@
                 <td>
                         {% if config["tunnel"] %}
                         <a href="/share?project={{x}}">{% if share[x] %}Disable {% else %}Enable {% endif %}</a>
                         {% else %}
                                 <a href="https://loophost.dev/upgrade.html">Enable</a>
                         {% endif %}
                 </td>
-                <td><a href="/unbind?project={{x}}">X</a></td>
+                <td><a href="/config/{{x}}">config</a></td>
         </tr>
         {% endfor %}
         </tbody>
         </table>
         </div>
         {% endif %}
-        </ul>
 </div>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Your local apps:
+****** Your local apps: ******
 {% if not apps %}
 ***** No local apps set up yet! *****
 {% else %}
-Project Name                 Location    Toggle Sharing                Unbind?
-{{x}}   {% if share[x] %}              {% if config["tunnel"] %} {%
-]}}">(shareable)             {{apps[x]}} if_share[x]_%}Disable_{%_else X
- {% endif %}                             %}Enable_{%_endif_%} {% else
-                                         %} Enable {% endif %}
+Project Name                 Location    Toggle Sharing                  Config
+{{x}}   {% if share[x] %}              {% if config["tunnel"] %} {%_if
+]}}">(shareable)             {{apps[x]}} share[x]_%}Disable_{%_else      config
+ {% endif %}                             %}Enable_{%_endif_%} {% else %}
+                                         Enable {% endif %}
 {% endif %}
```

### Comparing `loophost-0.2.7/loophost/uninstall.py` & `loophost-0.2.8/loophost/uninstall.py`

 * *Files identical despite different names*

### Comparing `loophost-0.2.7/pyproject.toml` & `loophost-0.2.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "poetry>=0.12", "setuptools", "wheel", "setuptools-cpp", "setuptools-golang"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "loophost"
-version = "0.2.7"
+version = "0.2.8"
 description = "Loophost: for a better local dev"
 authors = [
     "Joshua McKenty <jmckenty@gmail.com>",
 ]
 readme = "README.md"
 license = "Apache-2.0"
 include = [{ path = "VERSION" },
```

### Comparing `loophost-0.2.7/PKG-INFO` & `loophost-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loophost
-Version: 0.2.7
+Version: 0.2.8
 Summary: Loophost: for a better local dev
 License: Apache-2.0
 Author: Joshua McKenty
 Author-email: jmckenty@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

