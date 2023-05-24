# Comparing `tmp/volare-0.7.2.tar.gz` & `tmp/volare-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/volare-0.7.2.tar", last modified: Thu May 11 10:02:08 2023, max compression
+gzip compressed data, was "dist/volare-0.7.3.tar", last modified: Wed May 24 15:16:24 2023, max compression
```

## Comparing `volare-0.7.2.tar` & `volare-0.7.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:02:08.000000 volare-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 10:02:08.000000 volare-0.7.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)      931 2023-05-11 10:01:50.000000 volare-0.7.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     8665 2023-05-11 10:02:08.000000 volare-0.7.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:02:08.000000 volare-0.7.2/volare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-11 10:02:08.000000 volare-0.7.2/volare.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-11 10:02:08.000000 volare-0.7.2/volare.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 10:02:08.000000 volare-0.7.2/volare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)     8665 2023-05-11 10:02:08.000000 volare-0.7.2/volare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-11 10:02:08.000000 volare-0.7.2/volare.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      491 2023-05-11 10:02:08.000000 volare-0.7.2/volare.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:02:08.000000 volare-0.7.2/volare/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:02:08.000000 volare-0.7.2/volare/build/
--rw-r--r--   0 runner    (1001) docker     (122)     7450 2023-05-11 10:01:50.000000 volare-0.7.2/volare/build/git_multi_clone.py
--rw-r--r--   0 runner    (1001) docker     (122)     9219 2023-05-11 10:01:50.000000 volare-0.7.2/volare/build/gf180mcu.py
--rw-r--r--   0 runner    (1001) docker     (122)     4931 2023-05-11 10:01:50.000000 volare-0.7.2/volare/build/asap7.py
--rw-r--r--   0 runner    (1001) docker     (122)    13938 2023-05-11 10:01:50.000000 volare-0.7.2/volare/build/sky130.py
--rw-r--r--   0 runner    (1001) docker     (122)     3559 2023-05-11 10:01:50.000000 volare-0.7.2/volare/build/magic.py
--rw-r--r--   0 runner    (1001) docker     (122)     5550 2023-05-11 10:01:50.000000 volare-0.7.2/volare/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-05-11 10:01:50.000000 volare-0.7.2/volare/families.py
--rw-r--r--   0 runner    (1001) docker     (122)    13864 2023-05-11 10:01:50.000000 volare-0.7.2/volare/manage.py
--rw-r--r--   0 runner    (1001) docker     (122)      671 2023-05-11 10:01:50.000000 volare-0.7.2/volare/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 10:01:50.000000 volare-0.7.2/volare/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     7734 2023-05-11 10:01:50.000000 volare-0.7.2/volare/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     3289 2023-05-11 10:01:50.000000 volare-0.7.2/volare/click_common.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1667 2023-05-11 10:01:50.000000 volare-0.7.2/volare/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      766 2023-05-11 10:01:50.000000 volare-0.7.2/volare/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:16:24.000000 volare-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-24 15:16:24.000000 volare-0.7.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)      931 2023-05-24 15:16:04.000000 volare-0.7.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8665 2023-05-24 15:16:24.000000 volare-0.7.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:16:24.000000 volare-0.7.3/volare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-24 15:16:23.000000 volare-0.7.3/volare.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-24 15:16:23.000000 volare-0.7.3/volare.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 15:16:23.000000 volare-0.7.3/volare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8665 2023-05-24 15:16:23.000000 volare-0.7.3/volare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-24 15:16:23.000000 volare-0.7.3/volare.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      491 2023-05-24 15:16:24.000000 volare-0.7.3/volare.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:16:24.000000 volare-0.7.3/volare/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:16:24.000000 volare-0.7.3/volare/build/
+-rw-r--r--   0 runner    (1001) docker     (122)     7450 2023-05-24 15:16:04.000000 volare-0.7.3/volare/build/git_multi_clone.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9219 2023-05-24 15:16:04.000000 volare-0.7.3/volare/build/gf180mcu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4931 2023-05-24 15:16:04.000000 volare-0.7.3/volare/build/asap7.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13938 2023-05-24 15:16:04.000000 volare-0.7.3/volare/build/sky130.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3559 2023-05-24 15:16:04.000000 volare-0.7.3/volare/build/magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5550 2023-05-24 15:16:04.000000 volare-0.7.3/volare/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-05-24 15:16:04.000000 volare-0.7.3/volare/families.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13864 2023-05-24 15:16:04.000000 volare-0.7.3/volare/manage.py
+-rw-r--r--   0 runner    (1001) docker     (122)      671 2023-05-24 15:16:04.000000 volare-0.7.3/volare/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 15:16:04.000000 volare-0.7.3/volare/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     7777 2023-05-24 15:16:04.000000 volare-0.7.3/volare/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3289 2023-05-24 15:16:04.000000 volare-0.7.3/volare/click_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1667 2023-05-24 15:16:04.000000 volare-0.7.3/volare/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      766 2023-05-24 15:16:04.000000 volare-0.7.3/volare/__init__.py
```

### Comparing `volare-0.7.2/setup.py` & `volare-0.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.2/PKG-INFO` & `volare-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volare
-Version: 0.7.2
+Version: 0.7.3
 Summary: An open_pdks PDK builder/version manager
 Home-page: UNKNOWN
 Author: Efabless Corporation
 Author-email: donn@efabless.com
 License: UNKNOWN
 Description: <h1 align="center">⛰️ Volare</h1>
         <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: volare Version: 0.7.2 Summary: An open_pdks PDK
+Metadata-Version: 2.1 Name: volare Version: 0.7.3 Summary: An open_pdks PDK
 builder/version manager Home-page: UNKNOWN Author: Efabless Corporation Author-
 email: donn@efabless.com License: UNKNOWN Description:
                           ****** â°ï¸ Volare ******
   [License:_Apache_2.0] [CI Status] [Invite_to_the_Skywater_PDK_Slack] [Code
                                  Style:_Black]
 Volare is a version manager (and builder) for builds of Google_open-source_PDKs
                                using open_pdks.
```

### Comparing `volare-0.7.2/volare.egg-info/PKG-INFO` & `volare-0.7.3/volare.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volare
-Version: 0.7.2
+Version: 0.7.3
 Summary: An open_pdks PDK builder/version manager
 Home-page: UNKNOWN
 Author: Efabless Corporation
 Author-email: donn@efabless.com
 License: UNKNOWN
 Description: <h1 align="center">⛰️ Volare</h1>
         <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: volare Version: 0.7.2 Summary: An open_pdks PDK
+Metadata-Version: 2.1 Name: volare Version: 0.7.3 Summary: An open_pdks PDK
 builder/version manager Home-page: UNKNOWN Author: Efabless Corporation Author-
 email: donn@efabless.com License: UNKNOWN Description:
                           ****** â°ï¸ Volare ******
   [License:_Apache_2.0] [CI Status] [Invite_to_the_Skywater_PDK_Slack] [Code
                                  Style:_Black]
 Volare is a version manager (and builder) for builds of Google_open-source_PDKs
                                using open_pdks.
```

### Comparing `volare-0.7.2/volare/build/git_multi_clone.py` & `volare-0.7.3/volare/build/git_multi_clone.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.2/volare/build/gf180mcu.py` & `volare-0.7.3/volare/build/gf180mcu.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.2/volare/build/asap7.py` & `volare-0.7.3/volare/build/asap7.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.2/volare/build/sky130.py` & `volare-0.7.3/volare/build/sky130.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.2/volare/build/magic.py` & `volare-0.7.3/volare/build/magic.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.2/volare/build/__init__.py` & `volare-0.7.3/volare/build/__init__.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.2/volare/families.py` & `volare-0.7.3/volare/families.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.2/volare/manage.py` & `volare-0.7.3/volare/manage.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.2/volare/__version__.py` & `volare-0.7.3/volare/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.7.2"
+__version__ = "0.7.3"
 
 if __name__ == "__main__":
     print(__version__, end="")
```

### Comparing `volare-0.7.2/volare/common.py` & `volare-0.7.3/volare/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,10 +240,14 @@
     ]
 
 
 def get_current_version(pdk_root: str, pdk: str) -> str:
     current_file = os.path.join(get_volare_dir(pdk_root, pdk), "current")
     current_file_dir = os.path.dirname(current_file)
     mkdirp(current_file_dir)
-    pathlib.Path(current_file).touch(exist_ok=True)
+    version = ""
+    try:
+        version = open(current_file).read().strip()
+    except FileNotFoundError:
+        pass
 
-    return open(current_file).read().strip()
+    return version
```

### Comparing `volare-0.7.2/volare/click_common.py` & `volare-0.7.3/volare/click_common.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.2/volare/__main__.py` & `volare-0.7.3/volare/__main__.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.2/volare/__init__.py` & `volare-0.7.3/volare/__init__.py`

 * *Files identical despite different names*

