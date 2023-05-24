# Comparing `tmp/pyviz_comms-2.2.1rc1.tar.gz` & `tmp/pyviz_comms-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyviz_comms-2.2.1rc1.tar", last modified: Thu Aug 18 23:01:35 2022, max compression
+gzip compressed data, was "dist/pyviz_comms-2.3.0.tar", last modified: Wed May 24 18:22:47 2023, max compression
```

## Comparing `pyviz_comms-2.2.1rc1.tar` & `pyviz_comms-2.3.0.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 23:01:35.000000 pyviz_comms-2.2.1rc1/
--rw-r--r--   0 runner    (1001) docker     (121)     1499 2022-08-18 22:53:27.000000 pyviz_comms-2.2.1rc1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-08-18 22:53:27.000000 pyviz_comms-2.2.1rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4888 2022-08-18 23:01:35.000000 pyviz_comms-2.2.1rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3754 2022-08-18 22:53:27.000000 pyviz_comms-2.2.1rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-08-18 22:53:27.000000 pyviz_comms-2.2.1rc1/install.json
--rw-r--r--   0 runner    (1001) docker     (121)     3179 2022-08-18 23:00:33.000000 pyviz_comms-2.2.1rc1/package.json
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-08-18 22:53:27.000000 pyviz_comms-2.2.1rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 23:01:35.000000 pyviz_comms-2.2.1rc1/pyviz_comms/
--rw-r--r--   0 runner    (1001) docker     (121)    19734 2022-08-18 22:53:27.000000 pyviz_comms-2.2.1rc1/pyviz_comms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      439 2022-08-18 22:53:27.000000 pyviz_comms-2.2.1rc1/pyviz_comms/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 23:01:35.000000 pyviz_comms-2.2.1rc1/pyviz_comms/labextension/
--rw-r--r--   0 runner    (1001) docker     (121)     3321 2022-08-18 23:01:34.000000 pyviz_comms-2.2.1rc1/pyviz_comms/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 23:01:35.000000 pyviz_comms-2.2.1rc1/pyviz_comms/labextension/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 23:01:35.000000 pyviz_comms-2.2.1rc1/pyviz_comms/labextension/schemas/@pyviz/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 23:01:35.000000 pyviz_comms-2.2.1rc1/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/
--rw-r--r--   0 runner    (1001) docker     (121)     3179 2022-08-18 23:01:33.000000 pyviz_comms-2.2.1rc1/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/package.json.orig
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-08-18 23:01:33.000000 pyviz_comms-2.2.1rc1/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 23:01:35.000000 pyviz_comms-2.2.1rc1/pyviz_comms/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (121)    14875 2022-08-18 23:01:34.000000 pyviz_comms-2.2.1rc1/pyviz_comms/labextension/static/445.e0d338852f1bcbe1aa57.js
--rw-r--r--   0 runner    (1001) docker     (121)     3379 2022-08-18 23:01:34.000000 pyviz_comms-2.2.1rc1/pyviz_comms/labextension/static/747.872484f6c86b06b5c3f4.js
--rw-r--r--   0 runner    (1001) docker     (121)     7753 2022-08-18 23:01:34.000000 pyviz_comms-2.2.1rc1/pyviz_comms/labextension/static/remoteEntry.bcb3e162c12e67a67d56.js
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-08-18 23:01:33.000000 pyviz_comms-2.2.1rc1/pyviz_comms/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (121)     2452 2022-08-18 23:01:34.000000 pyviz_comms-2.2.1rc1/pyviz_comms/labextension/static/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (121)     4976 2022-08-18 22:53:27.000000 pyviz_comms-2.2.1rc1/pyviz_comms/notebook.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 23:01:35.000000 pyviz_comms-2.2.1rc1/pyviz_comms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4888 2022-08-18 23:01:35.000000 pyviz_comms-2.2.1rc1/pyviz_comms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-08-18 23:01:35.000000 pyviz_comms-2.2.1rc1/pyviz_comms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-18 23:01:35.000000 pyviz_comms-2.2.1rc1/pyviz_comms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-08-18 23:01:35.000000 pyviz_comms-2.2.1rc1/pyviz_comms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-18 23:01:35.000000 pyviz_comms-2.2.1rc1/pyviz_comms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-18 23:01:35.000000 pyviz_comms-2.2.1rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3252 2022-08-18 22:53:27.000000 pyviz_comms-2.2.1rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 23:01:35.000000 pyviz_comms-2.2.1rc1/src/
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-08-18 22:53:27.000000 pyviz_comms-2.2.1rc1/src/icons.ts
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-08-18 22:53:27.000000 pyviz_comms-2.2.1rc1/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-08-18 22:53:27.000000 pyviz_comms-2.2.1rc1/src/manager.ts
--rw-r--r--   0 runner    (1001) docker     (121)    10389 2022-08-18 22:53:27.000000 pyviz_comms-2.2.1rc1/src/plugin.ts
--rw-r--r--   0 runner    (1001) docker     (121)     4702 2022-08-18 22:53:27.000000 pyviz_comms-2.2.1rc1/src/preview.tsx
--rw-r--r--   0 runner    (1001) docker     (121)    10214 2022-08-18 22:53:27.000000 pyviz_comms-2.2.1rc1/src/renderer.ts
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-08-18 22:53:27.000000 pyviz_comms-2.2.1rc1/src/svg.d.ts
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-08-18 22:53:27.000000 pyviz_comms-2.2.1rc1/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/
+-rw-r--r--   0 runner    (1001) docker     (123)    19946 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/pyviz_comms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/pyviz_comms/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/schemas/@pyviz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-24 18:22:45.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/package.json.orig
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-24 18:22:45.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/static/445.482ccf5e3a3952a8b415.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/static/747.872484f6c86b06b5c3f4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/static/remoteEntry.febb837ab3b6ef743bf7.js
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-24 18:22:45.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/pyviz_comms/notebook.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/pyviz_comms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/pyviz_comms/tests/test_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/src/icons.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/src/manager.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/src/plugin.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/src/preview.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/src/renderer.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/src/svg.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/tsconfig.json
```

### Comparing `pyviz_comms-2.2.1rc1/LICENSE.txt` & `pyviz_comms-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.2.1rc1/PKG-INFO` & `pyviz_comms-2.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: pyviz_comms
-Version: 2.2.1rc1
+Version: 2.3.0
 Summary: Bidirectional communication for the HoloViz ecosystem.
 Home-page: https://holoviz.org
 Author: Philipp Rudiger
 Author-email: philipp.jfr@gmail.com
 Maintainer: HoloViz
 Maintainer-email: developers@holoviz.org
 License: BSD
 Platform: Windows
 Platform: Mac OS X
 Platform: Linux
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: build
 Provides-Extra: all
 License-File: LICENSE.txt
 
 # pyviz_comms
@@ -119,9 +121,7 @@
 With the watch command running, every saved change will immediately be built locally and available in your running JupyterLab. Refresh JupyterLab to load the change in your browser (you may need to wait several seconds for the extension to be rebuilt).
 
 By default, the `jlpm run build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:
 
 ```bash
 jupyter lab build --minimize=False
 ```
-
-
```

### Comparing `pyviz_comms-2.2.1rc1/README.md` & `pyviz_comms-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.2.1rc1/package.json` & `pyviz_comms-2.3.0/pyviz_comms/labextension/package.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8893086080586081%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^3.1.0', '@jupyterlab/apputils': '^3.1.0', "*

 * *                   "'@jupyterlab/docregistry': '^3.1.0', '@jupyterlab/fileeditor': '^3.1.0', "*

 * *                   "'@jupyterlab/mainmenu': '^3.1.0', '@jupyterlab/notebook': '^3.1.0', "*

 * *                   "'@jupyterlab/settingregistry': '^3.1.0', '@jupyterlab/ui-components': "*

 * *                   "'^3.1.0', delete: ['react', 'react-dom']}",*

 * * "'devDependencies'": "{'@jupyter-widgets/jupyterlab-manager': '^5.0.7', "*

 * *   […]*

```diff
@@ -1,56 +1,64 @@
 {
     "author": "Philipp Rudiger",
     "bugs": {
         "url": "https://github.com/holoviz/pyviz_comms/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.0.0",
-        "@jupyterlab/apputils": "^3.0.0",
+        "@jupyterlab/application": "^3.1.0",
+        "@jupyterlab/apputils": "^3.1.0",
         "@jupyterlab/coreutils": "^5.0.0",
-        "@jupyterlab/docregistry": "^3.0.0",
-        "@jupyterlab/fileeditor": "^3.0.0",
-        "@jupyterlab/mainmenu": "^3.0.0",
-        "@jupyterlab/notebook": "^3.0.0",
-        "@jupyterlab/settingregistry": "^3.0.0",
-        "@jupyterlab/ui-components": "^3.0.0",
+        "@jupyterlab/docregistry": "^3.1.0",
+        "@jupyterlab/fileeditor": "^3.1.0",
+        "@jupyterlab/mainmenu": "^3.1.0",
+        "@jupyterlab/notebook": "^3.1.0",
+        "@jupyterlab/settingregistry": "^3.1.0",
+        "@jupyterlab/ui-components": "^3.1.0",
         "@lumino/coreutils": "^1.5.3",
-        "@lumino/signaling": "^1.4.3",
-        "react": "^17.0.1",
-        "react-dom": "^17.0.1"
+        "@lumino/signaling": "^1.4.3"
     },
     "description": "A JupyterLab extension for rendering HoloViz content.",
     "devDependencies": {
-        "@jupyter-widgets/jupyterlab-manager": "^3.1.1",
+        "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6",
+        "@jupyter-widgets/jupyterlab-manager": "^5.0.7",
         "@jupyterlab/builder": "^3.0.0",
         "@jupyterlab/testutils": "^3.0.0",
         "@types/node": "^14.14.16",
         "@types/react": "^17.0.0",
         "@types/react-dom": "^17.0.0",
-        "@typescript-eslint/eslint-plugin": "^2.27.0",
-        "@typescript-eslint/parser": "^2.27.0",
-        "eslint": "^7.5.0",
+        "@typescript-eslint/eslint-plugin": "^2.34.0",
+        "@typescript-eslint/parser": "^2.34.0",
+        "eslint": "^6.0.0",
         "eslint-config-prettier": "^6.10.1",
         "eslint-plugin-prettier": "^3.1.2",
         "npm-run-all": "^4.1.5",
         "prettier": "^1.19.0",
         "rimraf": "^3.0.2",
         "typescript": "~4.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/holoviz/pyviz_comms",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.febb837ab3b6ef743bf7.js",
+            "style": "./style"
+        },
         "extension": true,
         "outputDir": "pyviz_comms/labextension",
         "schemaDir": "schema",
         "sharedPackages": {
+            "@jupyter-widgets/base": {
+                "bundled": false,
+                "singleton": true
+            },
             "@jupyter-widgets/jupyterlab-manager": {
                 "bundled": false,
                 "singleton": true
             }
         }
     },
     "keywords": [
@@ -58,20 +66,26 @@
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "@pyviz/jupyterlab_pyviz",
     "peerDependencies": {
-        "@jupyter-widgets/jupyterlab-manager": "^3.0.0"
+        "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6",
+        "@jupyter-widgets/jupyterlab-manager": "^5.0.4"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/holoviz/pyviz_comms.git"
     },
+    "resolutions": {
+        "@lumino/widgets": "^1.37.2",
+        "react": "^17.0.1",
+        "react-dom": "^17.0.1"
+    },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:prod": "jlpm run build:lib && jlpm run build:labextension",
         "clean": "jlpm run clean:lib",
@@ -89,9 +103,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.2.1-rc1"
+    "version": "2.3.0"
 }
```

### Comparing `pyviz_comms-2.2.1rc1/pyviz_comms/__init__.py` & `pyviz_comms-2.3.0/pyviz_comms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,48 +291,42 @@
         self._on_msg = on_msg
         self._on_error = on_error
         self._on_stdout = on_stdout
         self._on_open = on_open
         self._comm = None
         super(Comm, self).__init__(id = id if id else uuid.uuid4().hex)
 
-
     def init(self, on_msg=None):
         """
         Initializes comms channel.
         """
 
-
     def close(self):
         """
         Closes the comm connection
         """
 
-
     def send(self, data=None, metadata=None, buffers=[]):
         """
         Sends data to the frontend
         """
 
-
     @classmethod
     def decode(cls, msg):
         """
         Decode incoming message, e.g. by parsing json.
         """
         return msg
 
-
     @property
     def comm(self):
         if not self._comm:
             raise ValueError('Comm has not been initialized')
         return self._comm
 
-
     def _handle_msg(self, msg):
         """
         Decode received message before passing it to on_msg callback
         if it has been defined.
         """
         comm_id = None
         try:
@@ -409,42 +403,38 @@
         if self._comm:
             return
         self._comm = IPyComm(target_name=self.id, data={})
         self._comm.on_msg(self._handle_msg)
         if self._on_open:
             self._on_open({})
 
-
     @classmethod
     def decode(cls, msg):
         """
         Decodes messages following Jupyter messaging protocol.
         If JSON decoding fails data is assumed to be a regular string.
         """
         return msg['content']['data']
 
-
     def close(self):
         """
         Closes the comm connection
         """
         if self._comm:
             self._comm.close()
 
-
     def send(self, data=None, metadata=None, buffers=[]):
         """
         Pushes data across comm socket.
         """
         if not self._comm:
             self.init()
         self.comm.send(data, metadata=metadata, buffers=buffers)
 
 
-
 class JupyterCommJS(JupyterComm):
     """
     JupyterCommJS provides a comms channel for the Jupyter notebook,
     which is initialized on the frontend. This allows sending events
     initiated on the frontend to python.
     """
 
@@ -456,14 +446,21 @@
         {msg_handler}
       }}
       var comm = window.PyViz.comm_manager.get_client_comm("{comm_id}");
       comm.on_msg(msg_handler);
     </script>
     """
 
+    @classmethod
+    def decode(cls, msg):
+        decoded = dict(msg['content']['data'])
+        if 'buffers' in msg:
+            decoded['_buffers'] = {i: v for i, v in enumerate(msg['buffers'])}
+        return decoded
+
     def __init__(self, id=None, on_msg=None, on_error=None, on_stdout=None, on_open=None):
         """
         Initializes a Comms object
         """
         from IPython import get_ipython
         super(JupyterCommJS, self).__init__(id, on_msg, on_error, on_stdout, on_open)
         self.manager = get_ipython().kernel.comm_manager
```

### Comparing `pyviz_comms-2.2.1rc1/pyviz_comms/labextension/package.json` & `pyviz_comms-2.3.0/package.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8893086080586081%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^3.1.0', '@jupyterlab/apputils': '^3.1.0', "*

 * *                   "'@jupyterlab/docregistry': '^3.1.0', '@jupyterlab/fileeditor': '^3.1.0', "*

 * *                   "'@jupyterlab/mainmenu': '^3.1.0', '@jupyterlab/notebook': '^3.1.0', "*

 * *                   "'@jupyterlab/settingregistry': '^3.1.0', '@jupyterlab/ui-components': "*

 * *                   "'^3.1.0', delete: ['react', 'react-dom']}",*

 * * "'devDependencies'": "{'@jupyter-widgets/jupyterlab-manager': '^5.0.7', "*

 * *   […]*

```diff
@@ -1,61 +1,59 @@
 {
     "author": "Philipp Rudiger",
     "bugs": {
         "url": "https://github.com/holoviz/pyviz_comms/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.0.0",
-        "@jupyterlab/apputils": "^3.0.0",
+        "@jupyterlab/application": "^3.1.0",
+        "@jupyterlab/apputils": "^3.1.0",
         "@jupyterlab/coreutils": "^5.0.0",
-        "@jupyterlab/docregistry": "^3.0.0",
-        "@jupyterlab/fileeditor": "^3.0.0",
-        "@jupyterlab/mainmenu": "^3.0.0",
-        "@jupyterlab/notebook": "^3.0.0",
-        "@jupyterlab/settingregistry": "^3.0.0",
-        "@jupyterlab/ui-components": "^3.0.0",
+        "@jupyterlab/docregistry": "^3.1.0",
+        "@jupyterlab/fileeditor": "^3.1.0",
+        "@jupyterlab/mainmenu": "^3.1.0",
+        "@jupyterlab/notebook": "^3.1.0",
+        "@jupyterlab/settingregistry": "^3.1.0",
+        "@jupyterlab/ui-components": "^3.1.0",
         "@lumino/coreutils": "^1.5.3",
-        "@lumino/signaling": "^1.4.3",
-        "react": "^17.0.1",
-        "react-dom": "^17.0.1"
+        "@lumino/signaling": "^1.4.3"
     },
     "description": "A JupyterLab extension for rendering HoloViz content.",
     "devDependencies": {
-        "@jupyter-widgets/jupyterlab-manager": "^3.1.1",
+        "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6",
+        "@jupyter-widgets/jupyterlab-manager": "^5.0.7",
         "@jupyterlab/builder": "^3.0.0",
         "@jupyterlab/testutils": "^3.0.0",
         "@types/node": "^14.14.16",
         "@types/react": "^17.0.0",
         "@types/react-dom": "^17.0.0",
-        "@typescript-eslint/eslint-plugin": "^2.27.0",
-        "@typescript-eslint/parser": "^2.27.0",
-        "eslint": "^7.5.0",
+        "@typescript-eslint/eslint-plugin": "^2.34.0",
+        "@typescript-eslint/parser": "^2.34.0",
+        "eslint": "^6.0.0",
         "eslint-config-prettier": "^6.10.1",
         "eslint-plugin-prettier": "^3.1.2",
         "npm-run-all": "^4.1.5",
         "prettier": "^1.19.0",
         "rimraf": "^3.0.2",
         "typescript": "~4.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/holoviz/pyviz_comms",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.bcb3e162c12e67a67d56.js",
-            "style": "./style"
-        },
         "extension": true,
         "outputDir": "pyviz_comms/labextension",
         "schemaDir": "schema",
         "sharedPackages": {
+            "@jupyter-widgets/base": {
+                "bundled": false,
+                "singleton": true
+            },
             "@jupyter-widgets/jupyterlab-manager": {
                 "bundled": false,
                 "singleton": true
             }
         }
     },
     "keywords": [
@@ -63,20 +61,26 @@
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "@pyviz/jupyterlab_pyviz",
     "peerDependencies": {
-        "@jupyter-widgets/jupyterlab-manager": "^3.0.0"
+        "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6",
+        "@jupyter-widgets/jupyterlab-manager": "^5.0.4"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/holoviz/pyviz_comms.git"
     },
+    "resolutions": {
+        "@lumino/widgets": "^1.37.2",
+        "react": "^17.0.1",
+        "react-dom": "^17.0.1"
+    },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:prod": "jlpm run build:lib && jlpm run build:labextension",
         "clean": "jlpm run clean:lib",
@@ -94,9 +98,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.2.1-rc1"
+    "version": "2.3.0"
 }
```

### Comparing `pyviz_comms-2.2.1rc1/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/package.json.orig` & `pyviz_comms-2.3.0/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/package.json.orig`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8937728937728938%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^3.1.0', '@jupyterlab/apputils': '^3.1.0', "*

 * *                   "'@jupyterlab/docregistry': '^3.1.0', '@jupyterlab/fileeditor': '^3.1.0', "*

 * *                   "'@jupyterlab/mainmenu': '^3.1.0', '@jupyterlab/notebook': '^3.1.0', "*

 * *                   "'@jupyterlab/settingregistry': '^3.1.0', '@jupyterlab/ui-components': "*

 * *                   "'^3.1.0', delete: ['react', 'react-dom']}",*

 * * "'devDependencies'": "{'@jupyter-widgets/jupyterlab-manager': '^5.0.7', "*

 * *   […]*

```diff
@@ -1,38 +1,37 @@
 {
     "author": "Philipp Rudiger",
     "bugs": {
         "url": "https://github.com/holoviz/pyviz_comms/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.0.0",
-        "@jupyterlab/apputils": "^3.0.0",
+        "@jupyterlab/application": "^3.1.0",
+        "@jupyterlab/apputils": "^3.1.0",
         "@jupyterlab/coreutils": "^5.0.0",
-        "@jupyterlab/docregistry": "^3.0.0",
-        "@jupyterlab/fileeditor": "^3.0.0",
-        "@jupyterlab/mainmenu": "^3.0.0",
-        "@jupyterlab/notebook": "^3.0.0",
-        "@jupyterlab/settingregistry": "^3.0.0",
-        "@jupyterlab/ui-components": "^3.0.0",
+        "@jupyterlab/docregistry": "^3.1.0",
+        "@jupyterlab/fileeditor": "^3.1.0",
+        "@jupyterlab/mainmenu": "^3.1.0",
+        "@jupyterlab/notebook": "^3.1.0",
+        "@jupyterlab/settingregistry": "^3.1.0",
+        "@jupyterlab/ui-components": "^3.1.0",
         "@lumino/coreutils": "^1.5.3",
-        "@lumino/signaling": "^1.4.3",
-        "react": "^17.0.1",
-        "react-dom": "^17.0.1"
+        "@lumino/signaling": "^1.4.3"
     },
     "description": "A JupyterLab extension for rendering HoloViz content.",
     "devDependencies": {
-        "@jupyter-widgets/jupyterlab-manager": "^3.1.1",
+        "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6",
+        "@jupyter-widgets/jupyterlab-manager": "^5.0.7",
         "@jupyterlab/builder": "^3.0.0",
         "@jupyterlab/testutils": "^3.0.0",
         "@types/node": "^14.14.16",
         "@types/react": "^17.0.0",
         "@types/react-dom": "^17.0.0",
-        "@typescript-eslint/eslint-plugin": "^2.27.0",
-        "@typescript-eslint/parser": "^2.27.0",
-        "eslint": "^7.5.0",
+        "@typescript-eslint/eslint-plugin": "^2.34.0",
+        "@typescript-eslint/parser": "^2.34.0",
+        "eslint": "^6.0.0",
         "eslint-config-prettier": "^6.10.1",
         "eslint-plugin-prettier": "^3.1.2",
         "npm-run-all": "^4.1.5",
         "prettier": "^1.19.0",
         "rimraf": "^3.0.2",
         "typescript": "~4.1.3"
     },
@@ -43,14 +42,18 @@
     ],
     "homepage": "https://github.com/holoviz/pyviz_comms",
     "jupyterlab": {
         "extension": true,
         "outputDir": "pyviz_comms/labextension",
         "schemaDir": "schema",
         "sharedPackages": {
+            "@jupyter-widgets/base": {
+                "bundled": false,
+                "singleton": true
+            },
             "@jupyter-widgets/jupyterlab-manager": {
                 "bundled": false,
                 "singleton": true
             }
         }
     },
     "keywords": [
@@ -58,20 +61,26 @@
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "@pyviz/jupyterlab_pyviz",
     "peerDependencies": {
-        "@jupyter-widgets/jupyterlab-manager": "^3.0.0"
+        "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6",
+        "@jupyter-widgets/jupyterlab-manager": "^5.0.4"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/holoviz/pyviz_comms.git"
     },
+    "resolutions": {
+        "@lumino/widgets": "^1.37.2",
+        "react": "^17.0.1",
+        "react-dom": "^17.0.1"
+    },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:prod": "jlpm run build:lib && jlpm run build:labextension",
         "clean": "jlpm run clean:lib",
@@ -89,9 +98,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.2.1-rc1"
+    "version": "2.3.0"
 }
```

### Comparing `pyviz_comms-2.2.1rc1/pyviz_comms/labextension/static/445.e0d338852f1bcbe1aa57.js` & `pyviz_comms-2.3.0/pyviz_comms/labextension/static/445.482ccf5e3a3952a8b415.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,28 +1,28 @@
 "use strict";
 (self.webpackChunk_pyviz_jupyterlab_pyviz = self.webpackChunk_pyviz_jupyterlab_pyviz || []).push([
     [445], {
         445: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => N
             });
-            var o = n(972),
-                i = n(493),
-                s = n(991),
-                r = n(921),
-                a = n(19),
-                d = n(74),
-                c = n(484),
-                l = n(923),
-                m = n(912);
-            const p = new m.LabIcon({
+            var o = n(123),
+                i = n(687),
+                s = n(33),
+                r = n(142),
+                a = n(986),
+                d = n(38),
+                l = n(344),
+                c = n(923),
+                m = n(502);
+            const h = new m.LabIcon({
                 name: "@pyviz/jupyterlab_pyviz:panel",
-                svgstr: '<?xml version="1.0" encoding="UTF-8" standalone="no"?>\n<svg\n   xmlns:dc="http://purl.org/dc/elements/1.1/"\n   xmlns:cc="http://creativecommons.org/ns#"\n   xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"\n   xmlns:svg="http://www.w3.org/2000/svg"\n   xmlns="http://www.w3.org/2000/svg"\n   xmlns:sodipodi="http://sodipodi.sourceforge.net/DTD/sodipodi-0.dtd"\n   xmlns:inkscape="http://www.inkscape.org/namespaces/inkscape"\n   width="63.84808mm"\n   height="63.912464mm"\n   viewBox="0 0 63.84808 63.912464"\n   version="1.1"\n   id="svg909"\n   inkscape:version="1.0.2 (e86c8708, 2021-01-15)">\n  <defs\n     id="defs903" />\n  <sodipodi:namedview\n     id="base"\n     pagecolor="#ffffff"\n     bordercolor="#666666"\n     borderopacity="1.0"\n     inkscape:pageopacity="0.0"\n     inkscape:pageshadow="2"\n     inkscape:zoom="0.35"\n     inkscape:cx="-50.770794"\n     inkscape:cy="0.77943717"\n     inkscape:document-units="mm"\n     inkscape:current-layer="layer1"\n     inkscape:document-rotation="0"\n     showgrid="false"\n     fit-margin-top="0"\n     fit-margin-left="0"\n     fit-margin-right="0"\n     fit-margin-bottom="0"\n     inkscape:window-width="1252"\n     inkscape:window-height="943"\n     inkscape:window-x="0"\n     inkscape:window-y="0"\n     inkscape:window-maximized="0" />\n  <metadata\n     id="metadata906">\n    <rdf:RDF>\n      <cc:Work\n         rdf:about="">\n        <dc:format>image/svg+xml</dc:format>\n        <dc:type\n           rdf:resource="http://purl.org/dc/dcmitype/StillImage" />\n        <dc:title></dc:title>\n      </cc:Work>\n    </rdf:RDF>\n  </metadata>\n  <g\n     inkscape:label="Layer 1"\n     inkscape:groupmode="layer"\n     id="layer1"\n     transform="translate(-119.26644,-147.96044)">\n    <g\n       transform="matrix(0.56444446,0,0,0.56444446,897.60207,-494.80999)"\n       id="g5614">\n      <rect\n         style="opacity:1;fill:#00aa44;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none"\n         id="rect4136-8-8-1"\n         width="113.11668"\n         height="113.23074"\n         x="-1378.941"\n         y="1138.7665" />\n      <g\n         id="g5603">\n        <g\n           id="g5591">\n          <rect\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none"\n             id="rect4327-3-71"\n             width="78.055412"\n             height="8"\n             x="-1361.4104"\n             y="1165.5731" />\n          <circle\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none"\n             id="path4355-79-2"\n             cx="-1341.4192"\n             cy="1169.5731"\n             r="9" />\n        </g>\n        <g\n           id="g5595">\n          <rect\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none"\n             id="rect4327-5-1-0"\n             width="78.055412"\n             height="8"\n             x="-1361.4104"\n             y="1191.3817" />\n          <circle\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none"\n             id="path4355-7-3-7"\n             cx="-1305.4111"\n             cy="1195.3817"\n             r="9" />\n        </g>\n        <g\n           id="g5599">\n          <rect\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:1;stroke-miterlimit:4;stroke-dasharray:none"\n             id="rect4327-54-6-2"\n             width="78.055412"\n             height="8"\n             x="-1361.4104"\n             y="1217.1904" />\n          <circle\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none"\n             id="path4355-3-9-8"\n             cx="-1341.4274"\n             cy="1221.1904"\n             r="9" />\n        </g>\n      </g>\n    </g>\n  </g>\n</svg>\n'
+                svgstr: '<?xml version="1.0" encoding="UTF-8" standalone="no"?>\n<svg\n   xmlns:dc="http://purl.org/dc/elements/1.1/"\n   xmlns:cc="http://creativecommons.org/ns#"\n   xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"\n   xmlns:svg="http://www.w3.org/2000/svg"\n   xmlns="http://www.w3.org/2000/svg"\n   width="63.84808mm"\n   height="63.912464mm"\n   viewBox="0 0 63.84808 63.912464"\n   version="1.1"\n   id="svg867">\n  <defs\n     id="defs861" />\n  <metadata\n     id="metadata864">\n    <rdf:RDF>\n      <cc:Work\n         rdf:about="">\n        <dc:format>image/svg+xml</dc:format>\n        <dc:type\n           rdf:resource="http://purl.org/dc/dcmitype/StillImage" />\n        <dc:title></dc:title>\n      </cc:Work>\n    </rdf:RDF>\n  </metadata>\n  <g\n     id="layer1"\n     transform="translate(-41.403339,-133.59734)">\n    <g\n       id="g5614"\n       transform="matrix(0.56444446,0,0,0.56444446,819.73897,-509.17309)">\n      <rect\n         y="1138.7665"\n         x="-1378.941"\n         height="113.23074"\n         width="113.11668"\n         id="rect4136-8-8-1"\n         style="opacity:1;fill:#0072b5;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none"\n         ry="9.4330282" />\n      <g\n         id="g5603">\n        <g\n           id="g5591">\n          <rect\n             y="1165.5731"\n             x="-1361.4104"\n             height="8"\n             width="78.055412"\n             id="rect4327-3-71"\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none" />\n          <circle\n             r="9"\n             cy="1169.5731"\n             cx="-1341.4192"\n             id="path4355-79-2"\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none" />\n        </g>\n        <g\n           id="g5595">\n          <rect\n             y="1191.3817"\n             x="-1361.4104"\n             height="8"\n             width="78.055412"\n             id="rect4327-5-1-0"\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none" />\n          <circle\n             r="9"\n             cy="1195.3817"\n             cx="-1305.4111"\n             id="path4355-7-3-7"\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none" />\n        </g>\n        <g\n           id="g5599">\n          <rect\n             y="1217.1904"\n             x="-1361.4104"\n             height="8"\n             width="78.055412"\n             id="rect4327-54-6-2"\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:1;stroke-miterlimit:4;stroke-dasharray:none" />\n          <circle\n             r="9"\n             cy="1221.1904"\n             cx="-1341.4274"\n             id="path4355-3-9-8"\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none" />\n        </g>\n      </g>\n    </g>\n  </g>\n</svg>\n'
             });
-            class h {
+            class p {
                 constructor(e, t) {
                     this._context = e, this._wManager = t, this._comm = null, e.sessionContext.statusChanged.connect(((e, t) => {
                         "restarting" !== t && "dead" !== t || (this._comm = null)
                     }), this)
                 }
                 get context() {
                     return this._context
@@ -37,20 +37,20 @@
                 get isDisposed() {
                     return null === this._context
                 }
                 dispose() {
                     this.isDisposed || (this._context = null, this._comm = null)
                 }
             }
-            var u = n(46),
-                g = n(526),
-                w = n(840),
-                _ = n(271);
-            const y = new g.Token("@pyviz/jupyterlab_pyviz:IPanelPreviewTracker");
-            class v extends u.DocumentWidget {
+            var u = n(819),
+                _ = n(526),
+                g = n(840),
+                w = n(271);
+            const v = new _.Token("@pyviz/jupyterlab_pyviz:IPanelPreviewTracker");
+            class y extends u.DocumentWidget {
                 constructor(e) {
                     super(Object.assign(Object.assign({}, e), {
                         content: new s.IFrame({
                             sandbox: ["allow-same-origin", "allow-scripts", "allow-downloads"]
                         })
                     })), window.onmessage = e => {
                         var t, n, o, i, s;
@@ -72,27 +72,27 @@
                         }
                     };
                     const {
                         getPanelUrl: t,
                         context: n,
                         renderOnSave: o
                     } = e;
-                    this.content.url = t(n.path), this.content.title.icon = p, this._renderOnSave = null != o && o, n.pathChanged.connect((() => {
+                    this.content.url = t(n.path), this.content.title.icon = h, this._renderOnSave = null != o && o, n.pathChanged.connect((() => {
                         this.content.url = t(n.path)
                     }));
                     const i = new s.ToolbarButton({
                             icon: m.refreshIcon,
                             tooltip: "Reload Preview",
                             onClick: () => {
                                 this.reload()
                             }
                         }),
-                        r = s.ReactWidget.create(_.createElement("label", {
+                        r = s.ReactWidget.create(w.createElement("label", {
                             className: "jp-PanelPreview-renderOnSave"
-                        }, _.createElement("input", {
+                        }, w.createElement("input", {
                             style: {
                                 verticalAlign: "middle"
                             },
                             name: "renderOnSave",
                             type: "checkbox",
                             defaultChecked: o,
                             onChange: e => {
@@ -102,63 +102,64 @@
                     this.toolbar.addItem("reload", i), n && (this.toolbar.addItem("renderOnSave", r), n.ready.then((() => {
                         n.fileChanged.connect((() => {
                             this.renderOnSave && this.reload()
                         }))
                     })))
                 }
                 dispose() {
-                    this.isDisposed || (super.dispose(), w.Signal.clearData(this))
+                    this.isDisposed || (super.dispose(), g.Signal.clearData(this))
                 }
                 reload() {
                     const e = this.content.node.querySelector("iframe");
                     null != e.contentWindow && e.contentWindow.location.reload()
                 }
                 get renderOnSave() {
                     return this._renderOnSave
                 }
                 set renderOnSave(e) {
                     this._renderOnSave = e
                 }
             }
-            class k extends u.ABCWidgetFactory {
+            class x extends u.ABCWidgetFactory {
                 constructor(e, t) {
                     super(t), this.getPanelUrl = e, this.defaultRenderOnSave = !1
                 }
                 createNewWidget(e) {
-                    return new v({
+                    return new y({
                         context: e,
                         getPanelUrl: this.getPanelUrl,
                         renderOnSave: this.defaultRenderOnSave
                     })
                 }
             }
-            var x = n(992);
-            const f = "application/vnd.holoviews_load.v0+json",
+            var f = n(832);
+            const k = "application/vnd.holoviews_load.v0+json",
                 b = "application/vnd.holoviews_exec.v0+json";
-            class C extends x.Widget {
+            class C extends f.Widget {
                 constructor(e, t) {
-                    super(), this._load_mimetype = f, this._script_element = document.createElement("script"), this._manager = t
+                    super(), this._load_mimetype = k, this._script_element = document.createElement("script"), this._manager = t
                 }
                 renderModel(e) {
                     const t = e.data[this._load_mimetype];
                     return this._script_element.textContent = t, this.node.appendChild(this._script_element), this._manager.comm, Promise.resolve()
                 }
             }
-            class P extends x.Widget {
+            class P extends f.Widget {
                 constructor(e, t) {
                     super(), this._html_mimetype = "text/html", this._js_mimetype = "application/javascript", this._exec_mimetype = b, this._createNodes(), this._manager = t, this._displayed = !1, this._dispose = !0
                 }
                 _createNodes() {
                     this._div_element = document.createElement("div"), this._script_element = document.createElement("script"), this._script_element.setAttribute("type", "text/javascript")
                 }
                 _registerKernel(e) {
                     var t;
                     const n = {
                         create_view: (e, t) => this._manager._wManager.create_view(e, t),
-                        set_state: e => this._manager._wManager.set_state(e)
+                        set_state: e => this._manager._wManager.set_state(e),
+                        display_view: (e, t) => this._manager._wManager.display_view(e, t)
                     };
                     window.PyViz.widget_manager = n;
                     const o = null === (t = this._manager.context.sessionContext.session) || void 0 === t ? void 0 : t.kernel,
                         i = {
                             connectToComm: (e, t) => {
                                 if (void 0 === o) return console.log("Kernel not found, could not connect to comm target ", e), {
                                     open: function() {},
@@ -250,15 +251,15 @@
                 }
                 dispose() {
                     this.isDisposed || (super.dispose(), this._disposePlot(), this._manager = null)
                 }
             }
             let R = null;
             try {
-                const e = n(292);
+                const e = n(294);
                 R = e.registerWidgetManager
             } catch (e) {
                 console.log("Could not load ipywidgets support for @pyviz/jupyterlab_pyviz")
             }
             var O;
             ! function(e) {
                 e.panelRender = "notebook:render-with-panel", e.panelOpen = "notebook:open-with-panel", e.lumenRender = "notebook:render-with-lumen", e.lumenOpen = "notebook:open-with-lumen"
@@ -267,15 +268,15 @@
                 constructor(e) {
                     this._commands = e
                 }
                 createNew(e) {
                     const t = new s.ToolbarButton({
                         className: "panelRender",
                         tooltip: "Render with Panel",
-                        icon: p,
+                        icon: h,
                         onClick: () => {
                             this._commands.execute(O.panelRender)
                         }
                     });
                     return e.toolbar.insertAfter("cellType", "panelRender", t), t
                 }
             }
@@ -283,162 +284,162 @@
                 constructor(e) {
                     this._commands = e
                 }
                 createNew(e) {
                     const t = new s.ToolbarButton({
                         className: "lumenRender",
                         tooltip: "Render with Lumen",
-                        icon: p,
+                        icon: h,
                         onClick: () => {
                             this._commands.execute(O.lumenRender)
                         }
                     });
                     return e.toolbar.addItem("lumenRender", t), t
                 }
             }
             class W {
                 createNew(e, t) {
                     const n = this._docmanager._findContext(t.path, "notebook"),
                         o = {
                             manager: null
                         };
                     null != R && R(n, e.content.rendermime, [o]);
-                    const i = new h(t, o.manager);
+                    const i = new p(t, o.manager);
                     return e.content.rendermime.addFactory({
                         safe: !1,
-                        mimeTypes: [f],
+                        mimeTypes: [k],
                         createRenderer: e => new C(e, i)
                     }, -1), e.content.rendermime.addFactory({
                         safe: !1,
                         mimeTypes: [b],
                         createRenderer: e => new P(e, i)
-                    }, -1), new l.DisposableDelegate((() => {
+                    }, -1), new c.DisposableDelegate((() => {
                         e.content.rendermime && e.content.rendermime.removeMimeType(b), i.dispose()
                     }))
                 }
             }
             const S = {
                     id: "@pyviz/jupyterlab_pyviz:plugin",
                     autoStart: !0,
-                    requires: [c.IDocumentManager, o.INotebookTracker],
-                    optional: [s.ICommandPalette, i.ILayoutRestorer, d.IMainMenu, r.ISettingRegistry],
-                    provides: y,
-                    activate: (e, t, n, o, i, r, d) => {
-                        const c = new W;
-                        c._docmanager = t, e.docRegistry.addWidgetExtension("Notebook", c);
-                        const l = new s.WidgetTracker({
+                    requires: [a.IDocumentManager, o.INotebookTracker],
+                    optional: [s.ICommandPalette, i.ILayoutRestorer, l.IMainMenu, d.ISettingRegistry],
+                    provides: v,
+                    activate: (e, t, n, o, i, a, d) => {
+                        const l = new W;
+                        l._docmanager = t, e.docRegistry.addWidgetExtension("Notebook", l);
+                        const c = new s.WidgetTracker({
                             namespace: "panel-preview"
                         });
 
                         function m(t) {
                             const o = n.currentWidget;
                             return !1 !== t.activate && o && e.shell.activateById(o.id), o
                         }
 
-                        function p() {
+                        function h() {
                             const t = e.shell.currentWidget;
                             return null != t && null != t.context && (t.context.path.endsWith(".yaml") || t.context.path.endsWith(".yml") || null !== n.currentWidget && n.currentWidget === t)
                         }
 
-                        function h(e) {
-                            return `${a.PageConfig.getBaseUrl()}panel-preview/render/${e}`
+                        function p(e) {
+                            return `${r.PageConfig.getBaseUrl()}panel-preview/render/${e}`
                         }
-                        i && i.restore(l, {
+                        i && i.restore(c, {
                             command: "docmanager:open",
                             args: e => ({
                                 path: e.context.path,
                                 factory: u.name
                             }),
                             name: e => e.context.path,
                             when: e.serviceManager.ready
                         });
-                        const u = new k(h, {
+                        const u = new x(p, {
                                 name: "Panel-preview",
                                 fileTypes: ["notebook"],
                                 modelName: "notebook"
                             }),
-                            g = new k(h, {
+                            _ = new x(p, {
                                 name: "Lumen-preview",
                                 fileTypes: ["yaml", "yml", "text", "py"],
                                 modelName: "text"
                             });
                         u.widgetCreated.connect(((e, t) => {
                             t.context.pathChanged.connect((() => {
-                                l.save(t)
-                            })), l.add(t)
-                        })), g.widgetCreated.connect(((e, t) => {
-                            l.add(t)
+                                c.save(t)
+                            })), c.add(t)
+                        })), _.widgetCreated.connect(((e, t) => {
+                            c.add(t)
                         }));
-                        const w = e => {
+                        const g = e => {
                             u.defaultRenderOnSave = e.get("renderOnSave").composite
                         };
                         d && Promise.all([d.load(S.id), e.restored]).then((([e]) => {
-                            w(e), e.changed.connect(w)
+                            g(e), e.changed.connect(g)
                         })).catch((e => {
                             console.error(e.message)
-                        })), e.docRegistry.addWidgetFactory(u), e.docRegistry.addWidgetFactory(g);
+                        })), e.docRegistry.addWidgetFactory(u), e.docRegistry.addWidgetFactory(_);
                         const {
-                            commands: _,
-                            docRegistry: y
+                            commands: w,
+                            docRegistry: v
                         } = e;
-                        if (_.addCommand(O.panelRender, {
+                        if (w.addCommand(O.panelRender, {
                                 label: "Render Notebook with Panel",
                                 execute: async e => {
                                     const t = m(e);
                                     let n;
-                                    t && (n = t.context, await n.save(), _.execute("docmanager:open", {
+                                    t && (n = t.context, await n.save(), w.execute("docmanager:open", {
                                         path: n.path,
                                         factory: "Panel-preview",
                                         options: {
                                             mode: "split-right"
                                         }
                                     }))
                                 },
-                                isEnabled: p
-                            }), _.addCommand(O.lumenRender, {
+                                isEnabled: h
+                            }), w.addCommand(O.lumenRender, {
                                 label: "Render Yaml with Lumen",
                                 execute: async t => {
                                     const n = e.shell.currentWidget;
                                     let o;
-                                    n && (o = n.context, await o.save(), _.execute("docmanager:open", {
+                                    n && (o = n.context, await o.save(), w.execute("docmanager:open", {
                                         path: o.path,
                                         factory: "Lumen-preview",
                                         options: {
                                             mode: "split-right"
                                         }
                                     }))
                                 },
-                                isEnabled: p
-                            }), _.addCommand(O.panelOpen, {
+                                isEnabled: h
+                            }), w.addCommand(O.panelOpen, {
                                 label: "Open with Panel in New Browser Tab",
                                 execute: async e => {
                                     const t = m(e);
                                     if (!t) return;
                                     await t.context.save();
-                                    const n = h(t.context.path);
+                                    const n = p(t.context.path);
                                     window.open(n)
                                 },
-                                isEnabled: p
+                                isEnabled: h
                             }), o) {
                             const e = "Notebook Operations";
                             [O.panelRender, O.panelOpen].forEach((t => {
                                 o.addItem({
                                     command: t,
                                     category: e
                                 })
                             }))
                         }
-                        r && r.viewMenu.addGroup([{
+                        a && a.viewMenu.addGroup([{
                             command: O.panelRender
                         }, {
                             command: O.panelOpen
                         }], 1e3);
-                        const v = new z(_);
-                        y.addWidgetExtension("Notebook", v);
-                        const x = new T(_);
-                        return y.addWidgetExtension("Editor", x), l
+                        const y = new z(w);
+                        v.addWidgetExtension("Notebook", y);
+                        const f = new T(w);
+                        return v.addWidgetExtension("Editor", f), c
                     }
                 },
                 N = S
         }
     }
 ]);
```

### Comparing `pyviz_comms-2.2.1rc1/pyviz_comms/labextension/static/747.872484f6c86b06b5c3f4.js` & `pyviz_comms-2.3.0/pyviz_comms/labextension/static/747.872484f6c86b06b5c3f4.js`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.2.1rc1/pyviz_comms/labextension/static/remoteEntry.bcb3e162c12e67a67d56.js` & `pyviz_comms-2.3.0/pyviz_comms/labextension/static/remoteEntry.febb837ab3b6ef743bf7.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,296 +1,299 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, f, p, d, c, v, h, y, b, g, m, j, w = {
+    var e, r, t, n, a, o, i, u, l, s, f, d, p, c, v, h, y, b, g, m, j, w, S = {
             281: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(445).then((() => () => t(445))),
                         "./extension": () => t.e(445).then((() => () => t(445))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
-                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    a = (e, r) => {
+                    o = (e, r) => {
                         if (t.S) {
                             var n = "default",
-                                o = t.S[n];
-                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                                a = t.S[n];
+                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => o,
-                    init: () => a
+                    get: () => a,
+                    init: () => o
                 })
             }
         },
-        S = {};
+        _ = {};
 
-    function _(e) {
-        var r = S[e];
+    function k(e) {
+        var r = _[e];
         if (void 0 !== r) return r.exports;
-        var t = S[e] = {
+        var t = _[e] = {
             id: e,
             exports: {}
         };
-        return w[e](t, t.exports, _), t.exports
+        return S[e](t, t.exports, k), t.exports
     }
-    _.m = w, _.c = S, _.n = e => {
+    k.m = S, k.c = _, k.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return _.d(r, {
+        return k.d(r, {
             a: r
         }), r
-    }, _.d = (e, r) => {
-        for (var t in r) _.o(r, t) && !_.o(e, t) && Object.defineProperty(e, t, {
+    }, k.d = (e, r) => {
+        for (var t in r) k.o(r, t) && !k.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, _.f = {}, _.e = e => Promise.all(Object.keys(_.f).reduce(((r, t) => (_.f[t](e, r), r)), [])), _.u = e => e + "." + {
-        445: "e0d338852f1bcbe1aa57",
+    }, k.f = {}, k.e = e => Promise.all(Object.keys(k.f).reduce(((r, t) => (k.f[t](e, r), r)), [])), k.u = e => e + "." + {
+        445: "482ccf5e3a3952a8b415",
         747: "872484f6c86b06b5c3f4"
     } [e] + ".js?v=" + {
-        445: "e0d338852f1bcbe1aa57",
+        445: "482ccf5e3a3952a8b415",
         747: "872484f6c86b06b5c3f4"
-    } [e], _.g = function() {
+    } [e], k.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), _.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@pyviz/jupyterlab_pyviz:", _.l = (t, n, o, a) => {
+    }(), k.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@pyviz/jupyterlab_pyviz:", k.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
-            if (void 0 !== o)
+            if (void 0 !== a)
                 for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
                     var f = l[s];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + a) {
                         i = f;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, _.nc && i.setAttribute("nonce", _.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var p = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(d);
-                    var o = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, k.nc && i.setAttribute("nonce", k.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
+            var d = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(p);
+                    var a = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
-                d = setTimeout(p.bind(null, void 0, {
+                p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = p.bind(null, i.onerror), i.onload = p.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, _.r = e => {
+    }, k.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        _.S = {};
+        k.S = {};
         var e = {},
             r = {};
-        _.I = (t, n) => {
+        k.I = (t, n) => {
             n || (n = []);
-            var o = r[t];
-            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
-                if (n.push(o), e[t]) return e[t];
-                _.o(_.S, t) || (_.S[t] = {});
-                var a = _.S[t],
+            var a = r[t];
+            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
+                if (n.push(a), e[t]) return e[t];
+                k.o(k.S, t) || (k.S[t] = {});
+                var o = k.S[t],
                     i = "@pyviz/jupyterlab_pyviz",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
-                    var o = a[e] = a[e] || {},
-                        u = o[r];
-                    (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
-                        get: () => _.e(445).then((() => () => _(445))),
+                    var a = o[e] = o[e] || {},
+                        u = a[r];
+                    (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (a[r] = {
+                        get: () => k.e(445).then((() => () => k(445))),
                         from: i,
                         eager: !1
                     })
-                })("@pyviz/jupyterlab_pyviz", "2.2.1-rc1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("@pyviz/jupyterlab_pyviz", "2.3.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        _.g.importScripts && (e = _.g.location + "");
-        var r = _.g.document;
+        k.g.importScripts && (e = k.g.location + "");
+        var r = k.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
-            t.length && (e = t[t.length - 1].src)
+            if (t.length)
+                for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), _.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), k.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var o = e[n],
-                a = (typeof o)[0];
-            if (n >= r.length) return "u" == a;
+            var a = e[n],
+                o = (typeof a)[0];
+            if (n >= r.length) return "u" == o;
             var i = r[n],
                 u = (typeof i)[0];
-            if (a != u) return "o" == a && "n" == u || "s" == u || "u" == a;
-            if ("o" != a && "u" != a && o != i) return o < i;
+            if (o != u) return "o" == o && "n" == u || "s" == u || "u" == o;
+            if ("o" != o && "u" != o && a != i) return a < i;
             n++
         }
-    }, o = e => {
+    }, a = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
+            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(u = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var i = [];
-        for (a = 1; a < e.length; a++) {
-            var u = e[a];
-            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
+        for (o = 1; o < e.length; o++) {
+            var u = e[o];
+            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : a(u))
         }
         return l();
 
         function l() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, a = (e, r) => {
+    }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
-                o = n < 0;
-            o && (n = -n - 1);
+                a = n < 0;
+            a && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, f, p = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == p ? u > n && !o : "" == p != o);
+                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > n && !a : "" == d != a);
                 if ("u" == f) {
-                    if (!l || "u" != p) return !1
+                    if (!l || "u" != d) return !1
                 } else if (l)
-                    if (p == f)
+                    if (d == f)
                         if (u <= n) {
                             if (s != e[u]) return !1
                         } else {
-                            if (o ? s > e[u] : s < e[u]) return !1;
+                            if (a ? s > e[u] : s < e[u]) return !1;
                             s != e[u] && (l = !1)
                         }
-                else if ("s" != p && "n" != p) {
-                    if (o || u <= n) return !1;
+                else if ("s" != d && "n" != d) {
+                    if (a || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || f < p != o) return !1;
+                    if (u <= n || f < d != a) return !1;
                     l = !1
-                } else "s" != p && "n" != p && (l = !1, u--)
+                } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
-        var d = [],
-            c = d.pop.bind(d);
+        var p = [],
+            c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var v = e[i];
-            d.push(1 == v ? c() | c() : 2 == v ? c() & c() : v ? a(v, r) : !c())
+            p.push(1 == v ? c() | c() : 2 == v ? c() & c() : v ? o(v, r) : !c())
         }
         return !!c()
     }, i = (e, r) => {
-        var t = _.S[e];
-        if (!t || !_.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = k.S[e];
+        if (!t || !k.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
-        var o = l(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(s(e, t, o, n)), v(e[t][o])
-    }, p = (e, r, t) => {
-        var o = e[r];
-        return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, d = (e, r, t, n) => {
-        var a = e[t];
-        return "No satisfying version (" + o(n) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(a).map((e => e + " from " + a[e].from)).join(", ")
-    }, c = (e, r, t, n) => {
-        "undefined" != typeof console && console.warn && console.warn(d(e, r, t, n))
-    }, v = e => (e.loaded = 1, e.get()), y = (h = e => function(r, t, n, o) {
-        var a = _.I(r);
-        return a && a.then ? a.then(e.bind(e, r, _.S[r], t, n, o)) : e(r, _.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), v(p(r, t, n) || c(r, e, t, n) || u(r, t))))), b = h(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), g = {}, m = {
-        19: () => b("default", "@jupyterlab/coreutils", [1, 5, 4, 5]),
-        46: () => y("default", "@jupyterlab/docregistry", [1, 3, 4, 5]),
-        74: () => b("default", "@jupyterlab/mainmenu", [1, 3, 4, 5]),
-        271: () => b("default", "react", [1, 17, 0, 1]),
-        292: () => b("default", "@jupyter-widgets/jupyterlab-manager", [1, 3, 0, 0]),
-        484: () => b("default", "@jupyterlab/docmanager", [1, 3, 4, 5]),
-        493: () => b("default", "@jupyterlab/application", [1, 3, 4, 5]),
-        526: () => b("default", "@lumino/coreutils", [1, 1, 11, 0]),
-        840: () => b("default", "@lumino/signaling", [1, 1, 10, 0]),
-        912: () => b("default", "@jupyterlab/ui-components", [1, 3, 4, 5]),
-        921: () => b("default", "@jupyterlab/settingregistry", [1, 3, 4, 5]),
-        923: () => b("default", "@lumino/disposable", [1, 1, 10, 0]),
-        972: () => b("default", "@jupyterlab/notebook", [1, 3, 4, 5]),
-        991: () => b("default", "@jupyterlab/apputils", [1, 3, 4, 5]),
-        992: () => b("default", "@lumino/widgets", [1, 1, 33, 0])
-    }, j = {
-        445: [19, 46, 74, 271, 292, 484, 493, 526, 840, 912, 921, 923, 972, 991, 992]
-    }, _.f.consumes = (e, r) => {
-        _.o(j, e) && j[e].forEach((e => {
-            if (_.o(g, e)) return r.push(g[e]);
+    }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", f = (e, r, t, n) => {
+        var a = l(e, t);
+        return o(n, a) || c(s(e, t, a, n)), h(e[t][a])
+    }, d = (e, r, t) => {
+        var a = e[r];
+        return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
+    }, p = (e, r, t, n) => {
+        var o = e[t];
+        return "No satisfying version (" + a(n) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
+    }, c = e => {
+        "undefined" != typeof console && console.warn && console.warn(e)
+    }, v = (e, r, t, n) => {
+        c(p(e, r, t, n))
+    }, h = e => (e.loaded = 1, e.get()), b = (y = e => function(r, t, n, a) {
+        var o = k.I(r);
+        return o && o.then ? o.then(e.bind(e, r, k.S[r], t, n, a)) : e(r, k.S[r], t, n, a)
+    })(((e, r, t, n) => (i(e, t), h(d(r, t, n) || v(r, e, t, n) || u(r, t))))), g = y(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), m = {}, j = {
+        33: () => g("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
+        38: () => g("default", "@jupyterlab/settingregistry", [1, 3, 6, 3]),
+        123: () => g("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
+        142: () => g("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
+        271: () => g("default", "react", [1, 17, 0, 1]),
+        294: () => g("default", "@jupyter-widgets/jupyterlab-manager", [1, 5, 0, 4]),
+        344: () => g("default", "@jupyterlab/mainmenu", [1, 3, 6, 3]),
+        502: () => g("default", "@jupyterlab/ui-components", [1, 3, 6, 3]),
+        526: () => g("default", "@lumino/coreutils", [1, 1, 11, 0]),
+        687: () => g("default", "@jupyterlab/application", [1, 3, 6, 3]),
+        819: () => b("default", "@jupyterlab/docregistry", [1, 3, 6, 3]),
+        832: () => g("default", "@lumino/widgets", [1, 1, 37, 2]),
+        840: () => g("default", "@lumino/signaling", [1, 1, 10, 0]),
+        923: () => g("default", "@lumino/disposable", [1, 1, 10, 0]),
+        986: () => g("default", "@jupyterlab/docmanager", [1, 3, 6, 3])
+    }, w = {
+        445: [33, 38, 123, 142, 271, 294, 344, 502, 526, 687, 819, 832, 840, 923, 986]
+    }, k.f.consumes = (e, r) => {
+        k.o(w, e) && w[e].forEach((e => {
+            if (k.o(m, e)) return r.push(m[e]);
             var t = r => {
-                    g[e] = 0, _.m[e] = t => {
-                        delete _.c[e], t.exports = r()
+                    m[e] = 0, k.m[e] = t => {
+                        delete k.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete g[e], _.m[e] = t => {
-                        throw delete _.c[e], r
+                    delete m[e], k.m[e] = t => {
+                        throw delete k.c[e], r
                     }
                 };
             try {
-                var o = m[e]();
-                o.then ? r.push(g[e] = o.then(t).catch(n)) : t(o)
+                var a = j[e]();
+                a.then ? r.push(m[e] = a.then(t).catch(n)) : t(a)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             924: 0
         };
-        _.f.j = (r, t) => {
-            var n = _.o(e, r) ? e[r] : void 0;
+        k.f.j = (r, t) => {
+            var n = k.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
-                    var o = new Promise(((t, o) => n = e[r] = [t, o]));
-                    t.push(n[2] = o);
-                    var a = _.p + _.u(r),
+                    var a = new Promise(((t, a) => n = e[r] = [t, a]));
+                    t.push(n[2] = a);
+                    var o = k.p + k.u(r),
                         i = new Error;
-                    _.l(a, (t => {
-                        if (_.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                            var o = t && ("load" === t.type ? "missing" : t.type),
-                                a = t && t.target && t.target.src;
-                            i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
+                    k.l(o, (t => {
+                        if (k.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                            var a = t && ("load" === t.type ? "missing" : t.type),
+                                o = t && t.target && t.target.src;
+                            i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, o, [a, i, u] = t,
+                var n, a, [o, i, u] = t,
                     l = 0;
-                if (a.some((r => 0 !== e[r]))) {
-                    for (n in i) _.o(i, n) && (_.m[n] = i[n]);
-                    u && u(_)
+                if (o.some((r => 0 !== e[r]))) {
+                    for (n in i) k.o(i, n) && (k.m[n] = i[n]);
+                    u && u(k)
                 }
-                for (r && r(t); l < a.length; l++) o = a[l], _.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); l < o.length; l++) a = o[l], k.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunk_pyviz_jupyterlab_pyviz = self.webpackChunk_pyviz_jupyterlab_pyviz || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), _.nc = void 0;
-    var k = _(281);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@pyviz/jupyterlab_pyviz"] = k
+    })(), k.nc = void 0;
+    var E = k(281);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@pyviz/jupyterlab_pyviz"] = E
 })();
```

### Comparing `pyviz_comms-2.2.1rc1/pyviz_comms/labextension/static/third-party-licenses.json` & `pyviz_comms-2.3.0/pyviz_comms/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.2.1rc1/pyviz_comms/notebook.js` & `pyviz_comms-2.3.0/pyviz_comms/notebook.js`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.2.1rc1/pyviz_comms.egg-info/PKG-INFO` & `pyviz_comms-2.3.0/pyviz_comms.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: pyviz-comms
-Version: 2.2.1rc1
+Version: 2.3.0
 Summary: Bidirectional communication for the HoloViz ecosystem.
 Home-page: https://holoviz.org
 Author: Philipp Rudiger
 Author-email: philipp.jfr@gmail.com
 Maintainer: HoloViz
 Maintainer-email: developers@holoviz.org
 License: BSD
 Platform: Windows
 Platform: Mac OS X
 Platform: Linux
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: build
 Provides-Extra: all
 License-File: LICENSE.txt
 
 # pyviz_comms
@@ -119,9 +121,7 @@
 With the watch command running, every saved change will immediately be built locally and available in your running JupyterLab. Refresh JupyterLab to load the change in your browser (you may need to wait several seconds for the extension to be rebuilt).
 
 By default, the `jlpm run build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:
 
 ```bash
 jupyter lab build --minimize=False
 ```
-
-
```

### Comparing `pyviz_comms-2.2.1rc1/pyviz_comms.egg-info/SOURCES.txt` & `pyviz_comms-2.3.0/pyviz_comms.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 pyviz_comms.egg-info/SOURCES.txt
 pyviz_comms.egg-info/dependency_links.txt
 pyviz_comms.egg-info/requires.txt
 pyviz_comms.egg-info/top_level.txt
 pyviz_comms/labextension/package.json
 pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/package.json.orig
 pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/plugin.json
-pyviz_comms/labextension/static/445.e0d338852f1bcbe1aa57.js
+pyviz_comms/labextension/static/445.482ccf5e3a3952a8b415.js
 pyviz_comms/labextension/static/747.872484f6c86b06b5c3f4.js
-pyviz_comms/labextension/static/remoteEntry.bcb3e162c12e67a67d56.js
+pyviz_comms/labextension/static/remoteEntry.febb837ab3b6ef743bf7.js
 pyviz_comms/labextension/static/style.js
 pyviz_comms/labextension/static/third-party-licenses.json
+pyviz_comms/tests/__init__.py
+pyviz_comms/tests/test_extension.py
 src/icons.ts
 src/index.ts
 src/manager.ts
 src/plugin.ts
 src/preview.tsx
 src/renderer.ts
 src/svg.d.ts
```

### Comparing `pyviz_comms-2.2.1rc1/setup.py` & `pyviz_comms-2.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import json
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
+from setuptools import find_packages
+
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 # The name of the project
 name = "pyviz_comms"
 
 # Get our version
 with open(os.path.join(HERE, 'package.json')) as f:
@@ -62,15 +64,15 @@
         cmdclass["jsdeps"] = skip_if_exists(jstargets, js_command)
 except:
     cmdclass = {}
 
 extras_require = {
     'tests': ['flake8', 'pytest'],
     'build': [
-        'setuptools>=40.8.0,<61',
+        'setuptools>=40.8.0',
         'jupyterlab ~=3.0',
         'jupyter-packaging ~=0.7.9',
         'twine',
         'rfc3986',
         'keyring'
     ]
 }
@@ -81,39 +83,41 @@
     long_description = fh.read()
 
 install_requires = ['param']
 
 setup_args = dict(
     name=name,
     version=version,
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=install_requires,
     extras_require=extras_require,
     tests_require=extras_require['tests'],
     description='Bidirectional communication for the HoloViz ecosystem.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     cmdclass=cmdclass,
     author="Philipp Rudiger",
     author_email= "philipp.jfr@gmail.com",
     maintainer= "HoloViz",
     maintainer_email= "developers@holoviz.org",
     platforms=['Windows', 'Mac OS X', 'Linux'],
     license='BSD',
     url='https://holoviz.org',
-    packages = ["pyviz_comms"],
+    packages = find_packages(),
     include_package_data=True,
     classifiers = [
         "License :: OSI Approved :: BSD License",
         "Development Status :: 5 - Production/Stable",
+        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Topic :: Scientific/Engineering",
         "Topic :: Software Development :: Libraries"]
 )
```

### Comparing `pyviz_comms-2.2.1rc1/src/manager.ts` & `pyviz_comms-2.3.0/src/manager.ts`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.2.1rc1/src/plugin.ts` & `pyviz_comms-2.3.0/src/plugin.ts`

 * *Files 3% similar despite different names*

```diff
@@ -12,23 +12,25 @@
 
 import {
   ICommandPalette,
   WidgetTracker,
   ToolbarButton
 } from '@jupyterlab/apputils';
 
-import { ISettingRegistry } from '@jupyterlab/settingregistry';
-
 import { PageConfig } from '@jupyterlab/coreutils';
 
+import { IDocumentManager } from '@jupyterlab/docmanager';
+
 import { DocumentRegistry } from '@jupyterlab/docregistry';
 
+import { ISettingRegistry } from '@jupyterlab/settingregistry';
+
 import { IMainMenu } from '@jupyterlab/mainmenu';
 
-import { IDocumentManager } from '@jupyterlab/docmanager';
+import { IRenderMime } from '@jupyterlab/rendermime-interfaces';
 
 import { CommandRegistry } from '@lumino/commands';
 
 import { ReadonlyPartialJSONObject } from '@lumino/coreutils';
 
 import { IDisposable, DisposableDelegate } from '@lumino/disposable';
 
@@ -163,24 +165,32 @@
 
     const manager = new ContextManager(context, renderer.manager);
 
     nb.content.rendermime.addFactory(
       {
         safe: false,
         mimeTypes: [HV_LOAD_MIME_TYPE],
-        createRenderer: (options: any) => new HVJSLoad(options, manager)
+        createRenderer: (
+          options: IRenderMime.IRendererOptions
+        ): IRenderMime.IRenderer => {
+          return new HVJSLoad(options, manager);
+        }
       },
       -1
     );
 
     nb.content.rendermime.addFactory(
       {
         safe: false,
         mimeTypes: [HV_EXEC_MIME_TYPE],
-        createRenderer: (options: any) => new HVJSExec(options, manager)
+        createRenderer: (
+          options: IRenderMime.IRendererOptions
+        ): IRenderMime.IRenderer => {
+          return new HVJSExec(options, manager);
+        }
       },
       -1
     );
 
     return new DisposableDelegate(() => {
       if (nb.content.rendermime) {
         nb.content.rendermime.removeMimeType(HV_EXEC_MIME_TYPE);
```

### Comparing `pyviz_comms-2.2.1rc1/src/preview.tsx` & `pyviz_comms-2.3.0/src/preview.tsx`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.2.1rc1/src/renderer.ts` & `pyviz_comms-2.3.0/src/renderer.ts`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     callback: (comm: Kernel.IComm, msg: KernelMessage.ICommOpenMsg) => void
   ): void;
   connectToComm(targetName: string, commId?: string): ICommProxy;
 }
 
 export declare interface IWidgetManagerProxy {
   create_view(model: any): any;
+  display_view(view: any, el: any): any;
   set_state(state: any): Promise<any[]>;
 }
 
 /**
  * The MIME types for PyViz
  */
 const HTML_MIME_TYPE = 'text/html';
@@ -104,15 +105,22 @@
   _registerKernel(id: string): void {
     const set_state = (state: any): Promise<any[]> => {
       return this._manager._wManager.set_state(state);
     };
     const create_view = (model: any, options?: any): any => {
       return this._manager._wManager.create_view(model, options);
     };
-    const widget_manager: IWidgetManagerProxy = { create_view, set_state };
+    const display_view = (view: any, el: any): any => {
+      return this._manager._wManager.display_view(view, el);
+    };
+    const widget_manager: IWidgetManagerProxy = {
+      create_view,
+      set_state,
+      display_view
+    };
     (window as any).PyViz.widget_manager = widget_manager;
 
     const manager = this._manager;
     const kernel = manager!.context.sessionContext.session?.kernel;
     const registerClosure = (
       targetName: string,
       callback: (comm: Kernel.IComm, msg: KernelMessage.ICommOpenMsg) => void
```

### Comparing `pyviz_comms-2.2.1rc1/tsconfig.json` & `pyviz_comms-2.3.0/tsconfig.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'compilerOptions'": "{'skipLibCheck': True}"}*

```diff
@@ -11,14 +11,15 @@
         "noEmitOnError": true,
         "noImplicitAny": true,
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
+        "skipLibCheck": true,
         "strict": true,
         "strictNullChecks": false,
         "target": "es2017",
         "types": [
             "node"
         ]
     },
```

