# Comparing `tmp/behave-html-pretty-formatter-1.8.2.tar.gz` & `tmp/behave-html-pretty-formatter-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "behave-html-pretty-formatter-1.8.2.tar", last modified: Mon Apr 17 09:12:31 2023, max compression
+gzip compressed data, was "behave-html-pretty-formatter-1.9.tar", last modified: Wed May 24 10:41:00 2023, max compression
```

## Comparing `behave-html-pretty-formatter-1.8.2.tar` & `behave-html-pretty-formatter-1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:12:31.813775 behave-html-pretty-formatter-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 09:12:14.000000 behave-html-pretty-formatter-1.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-17 09:12:14.000000 behave-html-pretty-formatter-1.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-04-17 09:12:31.813775 behave-html-pretty-formatter-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-04-17 09:12:14.000000 behave-html-pretty-formatter-1.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:12:31.813775 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-17 09:12:14.000000 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-04-17 09:12:14.000000 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter/behave.css
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-04-17 09:12:14.000000 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter/behave.js
--rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-04-17 09:12:14.000000 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter/behave.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-17 09:12:14.000000 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter/behave.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    39492 2023-04-17 09:12:14.000000 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter/html_pretty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:12:31.813775 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-04-17 09:12:31.000000 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-17 09:12:31.000000 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:12:31.000000 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-17 09:12:31.000000 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-17 09:12:31.000000 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-17 09:12:14.000000 behave-html-pretty-formatter-1.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 09:12:31.813775 behave-html-pretty-formatter-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-17 09:12:14.000000 behave-html-pretty-formatter-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:00.928940 behave-html-pretty-formatter-1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 10:40:41.000000 behave-html-pretty-formatter-1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-24 10:40:41.000000 behave-html-pretty-formatter-1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10423 2023-05-24 10:41:00.928940 behave-html-pretty-formatter-1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-05-24 10:40:41.000000 behave-html-pretty-formatter-1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:00.928940 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-24 10:40:41.000000 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-05-24 10:40:41.000000 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter/behave.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-24 10:40:41.000000 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter/behave.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-05-24 10:40:41.000000 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter/behave.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-05-24 10:40:41.000000 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter/behave.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    39409 2023-05-24 10:40:41.000000 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter/html_pretty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:00.928940 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10423 2023-05-24 10:41:00.000000 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-24 10:41:00.000000 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 10:41:00.000000 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-24 10:41:00.000000 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-24 10:41:00.000000 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-24 10:40:41.000000 behave-html-pretty-formatter-1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 10:41:00.928940 behave-html-pretty-formatter-1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-24 10:40:41.000000 behave-html-pretty-formatter-1.9/setup.py
```

### Comparing `behave-html-pretty-formatter-1.8.2/LICENSE` & `behave-html-pretty-formatter-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `behave-html-pretty-formatter-1.8.2/PKG-INFO` & `behave-html-pretty-formatter-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: behave-html-pretty-formatter
-Version: 1.8.2
+Version: 1.9
 Summary: Pretty HTML Formatter for Behave
 Home-page: https://github.com/behave-contrib/behave-html-pretty-formatter
 Author: Michal Odehnal
 Author-email: modehnal@redhat.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `behave-html-pretty-formatter-1.8.2/README.md` & `behave-html-pretty-formatter-1.9/README.md`

 * *Files identical despite different names*

### Comparing `behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter/behave.css` & `behave-html-pretty-formatter-1.9/behave_html_pretty_formatter/behave.css`

 * *Files 2% similar despite different names*

```diff
@@ -175,14 +175,18 @@
   margin-bottom: 5px;
   background-color: var(--feature-bg);
   color: var(--feature-color);
   justify-content: start;
   font-size: 0.8rem;
 }
 
+.feature-summary-container.collapse {
+  display: none;
+}
+
 .feature-summary-container.contrast {
   background-color: #000;
   color: rgb(248, 248, 248);
   font-size: 1rem;
 }
 
 .feature-additional-info-container {
@@ -430,14 +434,18 @@
 .embed_content {
   white-space: pre-wrap;
   word-wrap: break-word;
   font-size: 12px;
   margin: 0.5rem;
 }
 
+.embed_content.collapse {
+  display: none;
+}
+
 .embed_button {
   cursor: pointer;
   margin: 0 1rem 0.5em 0;
   text-decoration: underline;
   color: var(--strong-color);
   font-size: 12px;
   width: max-content;
```

### Comparing `behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter/behave.min.css` & `behave-html-pretty-formatter-1.9/behave_html_pretty_formatter/behave.min.css`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-@charset "utf-8"; :root{--body-color:#333;--body-bg:#fff;--strong-color:#000;--feature-bg:#eee;--feature-color:#777;--duration-color:#313131;--summary-passed:#4f8a10;--summary-passed-border:#4f8a10;--summary-failed:#d8000c;--summary-failed-border:#d8000c;--summary-undefined:#945901;--summary-undefined-border:#ffdf61;--summary-skipped:#76adff;--summary-skipped-border:#76adff;--passed-bg:#dff2bf;--passed-step-bg:#c6dba3;--passed-border:#b4cc8c;--failed-bg:#f5c9cd;--failed-step-bg:#ea868f;--failed-border:#dd7a82;--undefined-bg:#ffdf61;--undefined-step-bg:#f1cb32;--undefined-border:#917400;--skipped-bg:#eef5ff;--skipped-step-bg:#cfe2ff;--skipped-border:#b8c9e4;--commentary-bg:#b9b9b9;--table-bg-odd:#fff;--table-bg-even:#eee;--button-bg:#666;--button-color:#eee;--button-bg-active:#898989;--button-color-active:#fff}@media (prefers-color-scheme:dark){:root{--body-color:#ddd;--body-bg:#000;--strong-color:#fff;--feature-bg:#222;--feature-color:#aaa;--duration-color:#cecece;--passed-bg:#42630a;--passed-step-bg:#697e41;--passed-border:#91a86b;--failed-bg:#69272d;--failed-step-bg:#a8666c;--failed-border:#df888f;--undefined-bg:#665a2a;--undefined-step-bg:#b6940d;--undefined-border:#dbb20e;--skipped-bg:#345381;--skipped-step-bg:#3d659e;--skipped-border:#6981a8;--commentary-bg:#5c5c5c;--table-bg-odd:#555;--table-bg-even:#444;--button-bg:#555;--button-color:#cdcdcd;--button-bg-active:#898989;--button-color-active:#fff}}html,body{font-family:Arial,Helvetica,sans-serif;font-size:1rem;margin:0;padding:0;color:var(--body-color);background:var(--body-bg)}body{padding:1rem 1rem;font-size:.85rem}pre,pre *{margin:0}.embed_button::after,.scenario-name::after{position:absolute;top:-0.5em;left:-0.2em;content:"\2304";font-size:1.8em;transition:all .2s linear}.embed_button.collapse::after,.collapse .scenario-name::after{top:-0.29em;left:-0.5em;transform:rotate(-90deg);-moz-transform:rotate(-90deg);-webkit-transform:rotate(-90deg);-ms-transform:rotate(-90deg);-o-transform:rotate(-90deg)}.embed_button,.scenario-name{padding-left:1.2em;position:relative}.feature-title{font-size:1rem;display:flex;flex-wrap:wrap;align-items:center;background-color:var(--feature-bg);color:var(--feature-color);padding:.5em 1rem;margin-bottom:5px}.feature-icon{height:1.2em;display:inline-block;margin-right:.3em;text-align:center;vertical-align:middle}.feature-icon.contrast{display:none}.feature-title.contrast{font-weight:bold;font-size:1.25rem;background-color:#000;color:#fff}.feature-summary-commentary{border-left:.4rem solid var(--feature-color);background-color:var(--commentary-bg);color:var(--strong-color);word-wrap:break-word;max-width:40%;margin-right:1rem;margin-top:.2rem;margin-left:.2rem;padding:.5rem;white-space:pre-wrap}.feature-summary-commentary.contrast{background-color:#242323;color:#f8f8f8;font-size:1rem}.feature-summary-container{display:flex;flex-wrap:wrap;padding:5px;padding-right:1rem;margin-bottom:5px;background-color:var(--feature-bg);color:var(--feature-color);justify-content:start;font-size:.8rem}.feature-summary-container.contrast{background-color:#000;color:#f8f8f8;font-size:1rem}.feature-additional-info-container{padding:5px;background-color:var(--feature-bg);color:var(--feature-color);justify-content:start;font-size:.8rem;flex-basis:100%}.contrast .feature-additional-info-container{background-color:#000;color:#f8f8f8;font-size:1rem}.feature-summary-stats{margin-top:.2em}.feature-summary-stats .button{padding-left:.4em;padding-right:.4em;padding-top:.1em;padding-bottom:.1em;margin-bottom:.1em}.feature-summary-row{color:var(--feature-color);border-left:.4rem solid var(--feature-color);padding-left:.5rem;padding-top:.1em;padding-bottom:.1em;margin-bottom:.1em}.feature-summary-row.passed{color:var(--summary-passed);border-left:.4rem solid var(--summary-passed-border)}.feature-summary-row.failed{color:var(--summary-failed);border-left:.4rem solid var(--summary-failed-border)}.feature-summary-row.undefined{color:var(--summary-undefined);border-left:.4rem solid var(--summary-undefined-border)}.feature-summary-row.skipped{color:var(--summary-skipped);border-left:.4rem solid var(--summary-skipped-border)}.feature-summary-row.contrast{color:#f8f8f8;border-left:.4rem solid #f8f8f8}.feature-container{margin-bottom:2rem}.scenario-capsule{padding:1rem;padding-right:.5rem;padding-top:.3rem;margin-bottom:1rem;color:var(--strong-color)}.scenario-header{padding:1rem;padding-bottom:0;margin-top:0;margin-bottom:0;color:var(--strong-color)}.scenario-capsule:last-child{border:0}.scenario-capsule{background-color:var(--feature-bg)}.scenario-header.passed{background-color:var(--passed-step-bg)}.scenario-header.failed{background-color:var(--failed-step-bg)}.scenario-header.undefined{background-color:var(--undefined-step-bg)}.scenario-header.skipped{background-color:var(--skipped-step-bg)}.scenario-header.contrast,.scenario-capsule.contrast{background-color:#000;color:#fff}.scenario-info{display:flex;flex-wrap:wrap;font-size:1.25rem}.scenario-name{cursor:pointer;font-weight:bold;padding-bottom:.5em}.scenario-duration{align-self:center;margin-left:auto;font-size:.75rem;font-style:italic;padding:0 .5em .5em 0}.scenario-duration.contrast{font-size:1.25rem;color:#fff}.scenario-tags{color:var(--body-color);font-weight:bold;font-size:.75rem;margin:.1rem .8em .5rem 0;display:inline-block}.scenario-tags.contrast{color:white;font-weight:bold;font-size:1rem;margin:.1rem 1em .5rem 0}.step-capsule{margin:2px 0 2px 2px;padding:.5rem;color:var(--strong-color);display:flex;flex-wrap:wrap;font-size:.75rem}.step-capsule.passed{background-color:var(--passed-step-bg);border:1px solid var(--passed-border)}.step-capsule.failed{background-color:var(--failed-step-bg);border:1px solid var(--failed-border)}.step-capsule.undefined{background-color:var(--undefined-step-bg);border:1px solid var(--undefined-step-bg)}.step-capsule.skipped{background-color:var(--skipped-step-bg);border:1px solid var(--skipped-border)}.step-capsule.commentary{background-color:var(--commentary-bg);margin-left:1rem}.step-capsule.description{background-color:var(--commentary-bg);margin-left:0}.step-capsule.contrast{background-color:#242323;color:#fff;font-size:1.25rem;border:none}.step-status{display:none;padding:0 1rem 0 0;font-weight:bold;font-size:1.25rem}.step-decorator{padding:0;padding-right:1.5rem}.step-duration{color:var(--duration-color);font-style:italic;padding:0;padding-right:1.5rem}.step-duration.contrast{color:#f8f8f8}.messages{margin:0 0 4px 1em}.scenario-capsule .messages:last-child{border-bottom:1px dashed var(--strong-color)}.scenario-capsule .messages.contrast:last-child{border-bottom:1px dashed #fff}.embed-capsule{margin:.5em 0}.embed_content{white-space:pre-wrap;word-wrap:break-word;font-size:12px;margin:.5rem}.embed_button{cursor:pointer;margin:0 1rem .5em 0;text-decoration:underline;color:var(--strong-color);font-size:12px;width:max-content}.embed_button.contrast{color:#fff;font-size:20px}th,td{padding:6px}thead{background-color:#333;color:#fff;cursor:pointer}table{color:var(--body-color);margin:2px 1em 4px 1em;border-collapse:collapse;border:1px solid #000;vertical-align:middle}table.contrast{font-size:1rem}table tbody tr:nth-child(odd){background-color:var(--table-bg-odd)}table tbody tr:nth-child(even){background-color:var(--table-bg-even)}table.contrast tbody tr{background-color:#fff;color:#000;border:1px solid #000}img,video{max-width:100%;max-height:100%}a{color:inherit;text-decoration:none}a:hover{text-decoration:underline;text-decoration-color:var(--strong-color)}.contrast a:hover{color:grey;text-decoration:underline;text-decoration-color:grey}.scenario-header.collapse .scenario-tags,.scenario-capsule.collapse{display:none}.scenario-header.collapse{padding:.5rem 1rem 0 1rem;margin-bottom:1rem}.button{display:inline-block;color:var(--button-color);background-color:var(--button-bg);border-radius:.2em;font-weight:bold;text-decoration:none;padding:.5em .9em;text-align:center;cursor:pointer}.button:hover{text-decoration:none;color:var(--button-color-active);background-color:var(--button-bg-active)}.contrast .button{color:#111;background-color:#eee}.contrast .button:hover{text-decoration:none}.display-flex{display:flex}.display-block{display:block}.display-inline{display:inline}.display-block.display-inline{display:inline-block}.flex-gap{column-gap:1em;row-gap:2px}.flex-left-space{margin-left:auto}.margin-top{margin-top:15px}.no-margin-top{margin-top:0}.margin-bottom{margin-bottom:15px}@media only screen and (max-width:750px){.feature-title{flex-direction:column}.feature-summary-container{margin-left:0;margin-top:.25rem;font-size:1rem;display:block}.feature-additional-info-container{margin-left:0;margin-top:.25rem;font-size:1rem}.feature-summary-commentary{max-width:100%;margin-right:0}.flex-left-space{margin-left:initial}.feature-summary-stats{margin-left:.2rem}.scenario-capsule{padding-right:0}}
+@charset "utf-8"; :root{--body-color:#333;--body-bg:#fff;--strong-color:#000;--feature-bg:#eee;--feature-color:#777;--duration-color:#313131;--summary-passed:#4f8a10;--summary-passed-border:#4f8a10;--summary-failed:#d8000c;--summary-failed-border:#d8000c;--summary-undefined:#945901;--summary-undefined-border:#ffdf61;--summary-skipped:#76adff;--summary-skipped-border:#76adff;--passed-bg:#dff2bf;--passed-step-bg:#c6dba3;--passed-border:#b4cc8c;--failed-bg:#f5c9cd;--failed-step-bg:#ea868f;--failed-border:#dd7a82;--undefined-bg:#ffdf61;--undefined-step-bg:#f1cb32;--undefined-border:#917400;--skipped-bg:#eef5ff;--skipped-step-bg:#cfe2ff;--skipped-border:#b8c9e4;--commentary-bg:#b9b9b9;--table-bg-odd:#fff;--table-bg-even:#eee;--button-bg:#666;--button-color:#eee;--button-bg-active:#898989;--button-color-active:#fff}@media (prefers-color-scheme:dark){:root{--body-color:#ddd;--body-bg:#000;--strong-color:#fff;--feature-bg:#222;--feature-color:#aaa;--duration-color:#cecece;--passed-bg:#42630a;--passed-step-bg:#697e41;--passed-border:#91a86b;--failed-bg:#69272d;--failed-step-bg:#a8666c;--failed-border:#df888f;--undefined-bg:#665a2a;--undefined-step-bg:#b6940d;--undefined-border:#dbb20e;--skipped-bg:#345381;--skipped-step-bg:#3d659e;--skipped-border:#6981a8;--commentary-bg:#5c5c5c;--table-bg-odd:#555;--table-bg-even:#444;--button-bg:#555;--button-color:#cdcdcd;--button-bg-active:#898989;--button-color-active:#fff}}html,body{font-family:Arial,Helvetica,sans-serif;font-size:1rem;margin:0;padding:0;color:var(--body-color);background:var(--body-bg)}body{padding:1rem 1rem;font-size:.85rem}pre,pre *{margin:0}.embed_button::after,.scenario-name::after{position:absolute;top:-0.5em;left:-0.2em;content:"\2304";font-size:1.8em;transition:all .2s linear}.embed_button.collapse::after,.collapse .scenario-name::after{top:-0.29em;left:-0.5em;transform:rotate(-90deg);-moz-transform:rotate(-90deg);-webkit-transform:rotate(-90deg);-ms-transform:rotate(-90deg);-o-transform:rotate(-90deg)}.embed_button,.scenario-name{padding-left:1.2em;position:relative}.feature-title{font-size:1rem;display:flex;flex-wrap:wrap;align-items:center;background-color:var(--feature-bg);color:var(--feature-color);padding:.5em 1rem;margin-bottom:5px}.feature-icon{height:1.2em;display:inline-block;margin-right:.3em;text-align:center;vertical-align:middle}.feature-icon.contrast{display:none}.feature-title.contrast{font-weight:bold;font-size:1.25rem;background-color:#000;color:#fff}.feature-summary-commentary{border-left:.4rem solid var(--feature-color);background-color:var(--commentary-bg);color:var(--strong-color);word-wrap:break-word;max-width:40%;margin-right:1rem;margin-top:.2rem;margin-left:.2rem;padding:.5rem;white-space:pre-wrap}.feature-summary-commentary.contrast{background-color:#242323;color:#f8f8f8;font-size:1rem}.feature-summary-container{display:flex;flex-wrap:wrap;padding:5px;padding-right:1rem;margin-bottom:5px;background-color:var(--feature-bg);color:var(--feature-color);justify-content:start;font-size:.8rem}.feature-summary-container.collapse{display:none}.feature-summary-container.contrast{background-color:#000;color:#f8f8f8;font-size:1rem}.feature-additional-info-container{padding:5px;background-color:var(--feature-bg);color:var(--feature-color);justify-content:start;font-size:.8rem;flex-basis:100%}.contrast .feature-additional-info-container{background-color:#000;color:#f8f8f8;font-size:1rem}.feature-summary-stats{margin-top:.2em}.feature-summary-stats .button{padding-left:.4em;padding-right:.4em;padding-top:.1em;padding-bottom:.1em;margin-bottom:.1em}.feature-summary-row{color:var(--feature-color);border-left:.4rem solid var(--feature-color);padding-left:.5rem;padding-top:.1em;padding-bottom:.1em;margin-bottom:.1em}.feature-summary-row.passed{color:var(--summary-passed);border-left:.4rem solid var(--summary-passed-border)}.feature-summary-row.failed{color:var(--summary-failed);border-left:.4rem solid var(--summary-failed-border)}.feature-summary-row.undefined{color:var(--summary-undefined);border-left:.4rem solid var(--summary-undefined-border)}.feature-summary-row.skipped{color:var(--summary-skipped);border-left:.4rem solid var(--summary-skipped-border)}.feature-summary-row.contrast{color:#f8f8f8;border-left:.4rem solid #f8f8f8}.feature-container{margin-bottom:2rem}.scenario-capsule{padding:1rem;padding-right:.5rem;padding-top:.3rem;margin-bottom:1rem;color:var(--strong-color)}.scenario-header{padding:1rem;padding-bottom:0;margin-top:0;margin-bottom:0;color:var(--strong-color)}.scenario-capsule:last-child{border:0}.scenario-capsule{background-color:var(--feature-bg)}.scenario-header.passed{background-color:var(--passed-step-bg)}.scenario-header.failed{background-color:var(--failed-step-bg)}.scenario-header.undefined{background-color:var(--undefined-step-bg)}.scenario-header.skipped{background-color:var(--skipped-step-bg)}.scenario-header.contrast,.scenario-capsule.contrast{background-color:#000;color:#fff}.scenario-info{display:flex;flex-wrap:wrap;font-size:1.25rem}.scenario-name{cursor:pointer;font-weight:bold;padding-bottom:.5em}.scenario-duration{align-self:center;margin-left:auto;font-size:.75rem;font-style:italic;padding:0 .5em .5em 0}.scenario-duration.contrast{font-size:1.25rem;color:#fff}.scenario-tags{color:var(--body-color);font-weight:bold;font-size:.75rem;margin:.1rem .8em .5rem 0;display:inline-block}.scenario-tags.contrast{color:white;font-weight:bold;font-size:1rem;margin:.1rem 1em .5rem 0}.step-capsule{margin:2px 0 2px 2px;padding:.5rem;color:var(--strong-color);display:flex;flex-wrap:wrap;font-size:.75rem}.step-capsule.passed{background-color:var(--passed-step-bg);border:1px solid var(--passed-border)}.step-capsule.failed{background-color:var(--failed-step-bg);border:1px solid var(--failed-border)}.step-capsule.undefined{background-color:var(--undefined-step-bg);border:1px solid var(--undefined-step-bg)}.step-capsule.skipped{background-color:var(--skipped-step-bg);border:1px solid var(--skipped-border)}.step-capsule.commentary{background-color:var(--commentary-bg);margin-left:1rem}.step-capsule.description{background-color:var(--commentary-bg);margin-left:0}.step-capsule.contrast{background-color:#242323;color:#fff;font-size:1.25rem;border:none}.step-status{display:none;padding:0 1rem 0 0;font-weight:bold;font-size:1.25rem}.step-decorator{padding:0;padding-right:1.5rem}.step-duration{color:var(--duration-color);font-style:italic;padding:0;padding-right:1.5rem}.step-duration.contrast{color:#f8f8f8}.messages{margin:0 0 4px 1em}.scenario-capsule .messages:last-child{border-bottom:1px dashed var(--strong-color)}.scenario-capsule .messages.contrast:last-child{border-bottom:1px dashed #fff}.embed-capsule{margin:.5em 0}.embed_content{white-space:pre-wrap;word-wrap:break-word;font-size:12px;margin:.5rem}.embed_content.collapse{display:none}.embed_button{cursor:pointer;margin:0 1rem .5em 0;text-decoration:underline;color:var(--strong-color);font-size:12px;width:max-content}.embed_button.contrast{color:#fff;font-size:20px}th,td{padding:6px}thead{background-color:#333;color:#fff;cursor:pointer}table{color:var(--body-color);margin:2px 1em 4px 1em;border-collapse:collapse;border:1px solid #000;vertical-align:middle}table.contrast{font-size:1rem}table tbody tr:nth-child(odd){background-color:var(--table-bg-odd)}table tbody tr:nth-child(even){background-color:var(--table-bg-even)}table.contrast tbody tr{background-color:#fff;color:#000;border:1px solid #000}img,video{max-width:100%;max-height:100%}a{color:inherit;text-decoration:none}a:hover{text-decoration:underline;text-decoration-color:var(--strong-color)}.contrast a:hover{color:grey;text-decoration:underline;text-decoration-color:grey}.scenario-header.collapse .scenario-tags,.scenario-capsule.collapse{display:none}.scenario-header.collapse{padding:.5rem 1rem 0 1rem;margin-bottom:1rem}.button{display:inline-block;color:var(--button-color);background-color:var(--button-bg);border-radius:.2em;font-weight:bold;text-decoration:none;padding:.5em .9em;text-align:center;cursor:pointer}.button:hover{text-decoration:none;color:var(--button-color-active);background-color:var(--button-bg-active)}.contrast .button{color:#111;background-color:#eee}.contrast .button:hover{text-decoration:none}.display-flex{display:flex}.display-block{display:block}.display-inline{display:inline}.display-block.display-inline{display:inline-block}.flex-gap{column-gap:1em;row-gap:2px}.flex-left-space{margin-left:auto}.margin-top{margin-top:15px}.no-margin-top{margin-top:0}.margin-bottom{margin-bottom:15px}@media only screen and (max-width:750px){.feature-title{flex-direction:column}.feature-summary-container{margin-left:0;margin-top:.25rem;font-size:1rem;display:block}.feature-additional-info-container{margin-left:0;margin-top:.25rem;font-size:1rem}.feature-summary-commentary{max-width:100%;margin-right:0}.flex-left-space{margin-left:initial}.feature-summary-stats{margin-left:.2rem}.scenario-capsule{padding-right:0}}
```

### Comparing `behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter/html_pretty.py` & `behave-html-pretty-formatter-1.9/behave_html_pretty_formatter/html_pretty.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from __future__ import absolute_import
 
 import atexit
 import base64
 import os
 import time
 import traceback
+import uuid
 from collections import OrderedDict
 from datetime import datetime
 from pathlib import Path
 
 import dominate
 import markdown
 from behave.formatter.base import Formatter
@@ -182,32 +183,33 @@
 
             if self.high_contrast_button:
                 # Making sure there is a functioning button.
                 # Creating High Contrast oggle which is clickable.
                 span(
                     "High contrast toggle",
                     cls="button flex-left-space",
-                    onclick="toggle_contrast('embed')",
+                    id="high_contrast",
+                    onclick="toggle_hash('high_contrast')",
                 )
 
                 # Creating Summary which is clickable.
                 span(
                     "Summary",
                     cls="button",
-                    onclick="collapsible_summary('feature-summary-container')",
+                    id="summary",
+                    onclick="toggle_hash('summary')",
                 )
 
         # Generate summary.
-        summary_display = "display: none"
+        summary_collapse = "collapse"
         if formatter.show_summary:
-            summary_display = ""
+            summary_collapse = ""
         with div(
-            cls="feature-summary-container flex-gap",
+            cls=f"feature-summary-container flex-gap {summary_collapse}",
             id=f"f{self.counter}",
-            style=summary_display,
         ):
             # Generating feature commentary.
             flex_left_space = "flex-left-space" if self.description else ""
 
             # with div(cls=""):
             if self.description:
                 pre(
@@ -745,22 +747,22 @@
 
         with div(cls="messages"):
             with div(cls="embed-capsule"):
                 # Embed Caption.
                 div(
                     use_caption,
                     cls="embed_button collapse",
-                    onclick=f"collapsible_toggle('embed_{embed_data.uid}',this)",
+                    id=f"embed_button_{embed_data.uid}",
+                    onclick=f"toggle_hash('{embed_data.uid}')",
                 )
 
                 # Embed content.
                 with pre(
-                    cls="embed_content",
+                    cls="embed_content collapse",
                     id=f"embed_{embed_data.uid}",
-                    style="display: none",
                 ):
                     self.generate_download_button(embed_data, data, use_caption)
                     self.generate_embed_content(mime_type, data)
 
     def generate_table(self):
         """
         Converts step table into HTML.
@@ -770,16 +772,15 @@
         table_headings = self.table.headings
         table_rows = self.table.rows
 
         # Generate Table.
         with table(cls="table"):
             # Make a heading.
             with thead(
-                onclick="collapsible_toggle("
-                f"'table_{PrettyHTMLFormatter.table_number}')"
+                onclick="toggle_hash(" f"'table_{PrettyHTMLFormatter.table_number}')"
             ):
                 line = tr()
                 for heading in table_headings:
                     line += th(heading)
 
             # Make the body.
             with tbody(id=f"table_{PrettyHTMLFormatter.table_number}"):
@@ -795,15 +796,15 @@
         Converts step text into HTML.
         """
         if not self.text:
             return
         with table(cls="table"):
             # Do not make the table header.
             # with thead(
-            #     onclick="collapsible_toggle("
+            #     onclick="toggle_hash("
             #     f"'table_{PrettyHTMLFormatter.table_number}')"
             # ):
             #     line = tr()
             #     line += th("Text")
             # Make the body.
             with tbody(id=f"table_{PrettyHTMLFormatter.table_number}"):
                 # Make rows.
@@ -820,16 +821,16 @@
     """
 
     count = 0
 
     def __init__(
         self, mime_type, data, caption=None, fail_only=False, download_button=None
     ):
-        self._id = Embed.count
-        Embed.count += 1
+        # Generating unique ID.
+        self.uid = str(uuid.uuid4())[:4]
         self.set_data(mime_type, data, caption)
         self._fail_only = fail_only
         self.download_button = download_button
 
     def set_data(self, mime_type, data, caption=None):
         """
         Set data, mime_type and caption.
@@ -867,21 +868,14 @@
         return self._caption
 
     @property
     def fail_only(self):
         "Read-only fail_only access."
         return self._fail_only
 
-    @property
-    def uid(self):
-        """
-        Read-only access for embed ID.
-        """
-        return self._id
-
 
 class Tag:
     """
     Adds link to behave's tag
     """
 
     def __init__(self, behave_tag, link=None):
```

### Comparing `behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter.egg-info/PKG-INFO` & `behave-html-pretty-formatter-1.9/behave_html_pretty_formatter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: behave-html-pretty-formatter
-Version: 1.8.2
+Version: 1.9
 Summary: Pretty HTML Formatter for Behave
 Home-page: https://github.com/behave-contrib/behave-html-pretty-formatter
 Author: Michal Odehnal
 Author-email: modehnal@redhat.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter.egg-info/SOURCES.txt` & `behave-html-pretty-formatter-1.9/behave_html_pretty_formatter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `behave-html-pretty-formatter-1.8.2/setup.py` & `behave-html-pretty-formatter-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """Return the content of a file."""
     with open(filename, "r", encoding="utf-8") as file:
         return file.read()
 
 
 setuptools.setup(
     name="behave-html-pretty-formatter",
-    version="1.8.2",
+    version="1.9",
     author="Michal Odehnal",
     author_email="modehnal@redhat.com",
     description="""
 Pretty HTML Formatter for Behave
 
 Authors:
 Michal Odehnal <modehnal@redhat.com>,
```

