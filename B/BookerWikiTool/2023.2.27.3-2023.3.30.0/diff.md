# Comparing `tmp/BookerWikiTool-2023.2.27.3.tar.gz` & `tmp/BookerWikiTool-2023.3.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\BookerWikiTool-2023.2.27.3.tar", last modified: Fri Mar 10 08:18:51 2023, max compression
+gzip compressed data, was "dist\BookerWikiTool-2023.3.30.0.tar", last modified: Thu Mar 30 02:25:33 2023, max compression
```

## Comparing `BookerWikiTool-2023.2.27.3.tar` & `BookerWikiTool-2023.3.30.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-03-10 08:18:51.000000 BookerWikiTool-2023.2.27.3/
-drwxrwxrwx   0        0        0        0 2023-03-10 08:18:51.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/
--rw-rw-rw-   0        0        0      218 2023-03-10 08:18:47.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/__init__.py
--rw-rw-rw-   0        0        0    13361 2023-03-09 07:36:02.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/__main__.py
-drwxrwxrwx   0        0        0        0 2023-03-10 08:18:51.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/assets/
--rw-rw-rw-   0        0        0  1799680 2023-02-08 16:53:32.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/assets/7z.dll
--rwxrwxrwx   0        0        0   545280 2023-02-08 16:53:32.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/assets/7z.exe
--rwxrwxrwx   0        0        0 13910016 2023-02-08 16:53:32.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/assets/Pdg2Pic.exe
--rw-rw-rw-   0        0        0    44789 2023-03-02 07:04:12.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/assets/Pdg2Pic.htm
--rw-rw-rw-   0        0        0      348 2023-02-08 16:53:32.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/assets/Pdg2Pic.ini
--rw-rw-rw-   0        0        0   607222 2023-03-02 07:04:12.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/assets/PwdDic.txt
--rw-rw-rw-   0        0        0        0 2023-02-10 20:19:40.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/assets/__init__.py
--rwxrwxrwx   0        0        0   786446 2011-09-06 03:13:53.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/assets/jbig2.exe
--rw-rw-rw-   0        0        0    16896 2012-02-01 02:37:04.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/assets/jbig2enc.dll
--rwxrwxrwx   0        0        0   413336 2023-02-08 16:53:32.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/assets/unrar.exe
--rw-rw-rw-   0        0        0      672 2023-03-02 07:04:12.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/chatgpt.py
--rw-rw-rw-   0        0        0     2262 2023-03-02 07:04:12.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/codelint.py
--rw-rw-rw-   0        0        0     1645 2023-03-02 07:04:12.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/crawl_wx.py
--rw-rw-rw-   0        0        0     6111 2023-03-04 13:49:27.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/epub_tool.py
--rw-rw-rw-   0        0        0     4520 2023-03-09 07:36:02.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/fetch_links.py
--rw-rw-rw-   0        0        0      732 2023-03-02 07:04:12.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/flatten.py
--rw-rw-rw-   0        0        0     3843 2023-03-02 07:04:12.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/fmt.py
--rw-rw-rw-   0        0        0    10726 2023-03-05 10:59:24.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/md_tool.py
--rw-rw-rw-   0        0        0    15643 2023-03-02 07:04:12.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/pdf_tool.py
--rw-rw-rw-   0        0        0     1357 2023-03-02 07:04:12.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/pdg_tool.py
--rw-rw-rw-   0        0        0     1217 2023-03-02 07:04:12.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/toggle_bw.py
--rw-rw-rw-   0        0        0     3738 2023-03-02 07:04:12.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/tomd.js
--rw-rw-rw-   0        0        0     4221 2023-03-02 07:04:12.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/util.py
--rw-rw-rw-   0        0        0      998 2023-03-02 07:04:12.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/wx_external.py
--rw-rw-rw-   0        0        0     1652 2023-03-02 07:04:12.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool/zip_tool.py
-drwxrwxrwx   0        0        0        0 2023-03-10 08:18:51.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool.egg-info/
--rw-rw-rw-   0        0        0     2259 2023-03-10 08:18:51.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1025 2023-03-10 08:18:51.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-10 08:18:51.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2023-03-10 08:18:51.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      126 2023-03-10 08:18:51.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-03-10 08:18:51.000000 BookerWikiTool-2023.2.27.3/BookerWikiTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2259 2023-03-10 08:18:51.000000 BookerWikiTool-2023.2.27.3/PKG-INFO
--rw-rw-rw-   0        0        0      667 2022-04-23 14:51:24.000000 BookerWikiTool-2023.2.27.3/README.md
--rw-rw-rw-   0        0        0       42 2023-03-10 08:18:51.000000 BookerWikiTool-2023.2.27.3/setup.cfg
--rw-rw-rw-   0        0        0     1926 2022-04-23 14:55:30.000000 BookerWikiTool-2023.2.27.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-30 02:25:33.000000 BookerWikiTool-2023.3.30.0/
+drwxrwxrwx   0        0        0        0 2023-03-30 02:25:33.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/
+-rw-rw-rw-   0        0        0      218 2023-03-30 02:25:12.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/__init__.py
+-rw-rw-rw-   0        0        0    13702 2023-03-13 01:34:21.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/__main__.py
+drwxrwxrwx   0        0        0        0 2023-03-30 02:25:33.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/assets/
+-rw-rw-rw-   0        0        0  1799680 2023-02-08 16:53:32.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/assets/7z.dll
+-rwxrwxrwx   0        0        0   545280 2023-02-08 16:53:32.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/assets/7z.exe
+-rwxrwxrwx   0        0        0 13910016 2023-02-08 16:53:32.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/assets/Pdg2Pic.exe
+-rw-rw-rw-   0        0        0    44789 2023-03-02 07:04:12.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/assets/Pdg2Pic.htm
+-rw-rw-rw-   0        0        0      348 2023-02-08 16:53:32.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/assets/Pdg2Pic.ini
+-rw-rw-rw-   0        0        0   607222 2023-03-02 07:04:12.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/assets/PwdDic.txt
+-rw-rw-rw-   0        0        0        0 2023-02-10 20:19:40.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/assets/__init__.py
+-rwxrwxrwx   0        0        0   786446 2011-09-06 03:13:53.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/assets/jbig2.exe
+-rw-rw-rw-   0        0        0    16896 2012-02-01 02:37:04.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/assets/jbig2enc.dll
+-rwxrwxrwx   0        0        0   413336 2023-02-08 16:53:32.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/assets/unrar.exe
+-rw-rw-rw-   0        0        0      672 2023-03-02 07:04:12.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/chatgpt.py
+-rw-rw-rw-   0        0        0     2262 2023-03-02 07:04:12.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/codelint.py
+-rw-rw-rw-   0        0        0     1645 2023-03-02 07:04:12.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/crawl_wx.py
+-rw-rw-rw-   0        0        0     6111 2023-03-04 13:49:27.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/epub_tool.py
+-rw-rw-rw-   0        0        0     4771 2023-03-14 05:26:01.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/fetch_links.py
+-rw-rw-rw-   0        0        0      732 2023-03-02 07:04:12.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/flatten.py
+-rw-rw-rw-   0        0        0     4927 2023-03-13 01:34:21.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/fmt.py
+-rw-rw-rw-   0        0        0    11107 2023-03-14 05:26:01.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/md_tool.py
+-rw-rw-rw-   0        0        0    15723 2023-03-30 02:23:24.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/pdf_tool.py
+-rw-rw-rw-   0        0        0     1370 2023-03-30 02:24:02.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/pdg_tool.py
+-rw-rw-rw-   0        0        0     1174 2023-03-13 01:34:21.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/toggle_bw.py
+-rw-rw-rw-   0        0        0     3738 2023-03-02 07:04:12.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/tomd.js
+-rw-rw-rw-   0        0        0     4671 2023-03-13 01:34:21.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/util.py
+-rw-rw-rw-   0        0        0      998 2023-03-02 07:04:12.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/wx_external.py
+-rw-rw-rw-   0        0        0     1652 2023-03-02 07:04:12.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool/zip_tool.py
+drwxrwxrwx   0        0        0        0 2023-03-30 02:25:33.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool.egg-info/
+-rw-rw-rw-   0        0        0     2259 2023-03-30 02:25:33.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1025 2023-03-30 02:25:33.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-30 02:25:33.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2023-03-30 02:25:33.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      108 2023-03-30 02:25:33.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-03-30 02:25:33.000000 BookerWikiTool-2023.3.30.0/BookerWikiTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2259 2023-03-30 02:25:33.000000 BookerWikiTool-2023.3.30.0/PKG-INFO
+-rw-rw-rw-   0        0        0      667 2022-04-23 14:51:24.000000 BookerWikiTool-2023.3.30.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-03-30 02:25:33.000000 BookerWikiTool-2023.3.30.0/setup.cfg
+-rw-rw-rw-   0        0        0     1926 2022-04-23 14:55:30.000000 BookerWikiTool-2023.3.30.0/setup.py
```

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool/__main__.py` & `BookerWikiTool-2023.3.30.0/BookerWikiTool/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from collections import OrderedDict
 from EpubCrawler.img import process_img
 from EpubCrawler.util import safe_mkdir
 from . import __version__
 from .util import *
 from .epub_tool import *
 from .md_tool import *
+from .fmt import *
 from .fetch_links import *
 from .pdf_tool import *
 from .zip_tool import *
 from .flatten import *
 from .toggle_bw import *
 from .crawl_wx import *
 from .codelint import *
@@ -48,14 +49,19 @@
     wiki_sum_parser = subparsers.add_parser("wiki-summary", help="generate wiki summary")
     wiki_sum_parser.set_defaults(func=wiki_summary_handle)
     
     summary_parser = subparsers.add_parser("summary", help="generate summary")
     summary_parser.add_argument("dir", help="dir")
     summary_parser.set_defaults(func=summary_handle)
     
+    rm_suff_parser = subparsers.add_parser("rm-suff", help="remove suffix of HTML titles")
+    rm_suff_parser.add_argument("dir", help="dir")
+    rm_suff_parser.add_argument("-r", "--rate", type=float, default=0.5, help="rate of suffix in HTML titles")
+    rm_suff_parser.set_defaults(func=rm_suffix)
+    
     ren_parser = subparsers.add_parser("ren-md", help="rename md fname")
     ren_parser.add_argument("fname", help="file for dir name")
     ren_parser.add_argument("-t", "--threads", type=int, default=8, help="num of threads")
     ren_parser.add_argument("-b", "--by", type=str, choices=['title', 'src'], default='src', help="where to extract fname")
     ren_parser.set_defaults(func=ren_md_handle)
     
     acc_parser = subparsers.add_parser("account", help="account words")
@@ -149,20 +155,20 @@
     fetch_links_parser.add_argument("-H", "--headers", help="headers in JSON")
     fetch_links_parser.add_argument("-J", "--json", action='store_true', help="treat output as JSON not HTML")
     fetch_links_parser.set_defaults(func=fetch_links)
 
     fetch_sitemap_parser = subparsers.add_parser("fetch-sitemap", help="fetch links in sitemap")
     fetch_sitemap_parser.add_argument("url", help="sitemap url")
     fetch_sitemap_parser.add_argument("-r", "--regex", default="/blog/", help="link regex")
-    fetch_sitemap_parser.add_argument("ofname", help="output file name")
+    fetch_sitemap_parser.add_argument("-o", "--ofname", help="output file name")
     fetch_sitemap_parser.set_defaults(func=fetch_sitemap_handle)
 
     batch_links_parser = subparsers.add_parser("batch-links", help="batch download links to epub")
-    batch_links_parser.add_argument("name", help="epub name")
     batch_links_parser.add_argument("links", help="name of file storing links")
+    batch_links_parser.add_argument("--name", help="epub name")
     batch_links_parser.add_argument("-t", "--title", default="", help="title selector")
     batch_links_parser.add_argument("-c", "--content", default="", help="content selector")
     batch_links_parser.add_argument("-r", "--remove", default="", help="remove elems selector")
     batch_links_parser.add_argument("-n", "--num", default=500, type=int, help="num of articles in one epub")
     batch_links_parser.add_argument("-m", "--opti-mode", default='quant', help="img optimization mode")
     batch_links_parser.add_argument("-l", "--size-limit", default='100m', help="epub size limit")
     batch_links_parser.add_argument("-g", "--time-regex", default=r'(\d+)-(\d+)-(\d+)', help="time regex")
```

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool/assets/7z.dll` & `BookerWikiTool-2023.3.30.0/BookerWikiTool/assets/7z.dll`

 * *Files identical despite different names*

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool/assets/7z.exe` & `BookerWikiTool-2023.3.30.0/BookerWikiTool/assets/7z.exe`

 * *Files identical despite different names*

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool/assets/Pdg2Pic.exe` & `BookerWikiTool-2023.3.30.0/BookerWikiTool/assets/Pdg2Pic.exe`

 * *Files identical despite different names*

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool/assets/Pdg2Pic.htm` & `BookerWikiTool-2023.3.30.0/BookerWikiTool/assets/Pdg2Pic.htm`

 * *Files identical despite different names*

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool/assets/PwdDic.txt` & `BookerWikiTool-2023.3.30.0/BookerWikiTool/assets/PwdDic.txt`

 * *Files identical despite different names*

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool/assets/jbig2.exe` & `BookerWikiTool-2023.3.30.0/BookerWikiTool/assets/jbig2.exe`

 * *Files identical despite different names*

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool/assets/jbig2enc.dll` & `BookerWikiTool-2023.3.30.0/BookerWikiTool/assets/jbig2enc.dll`

 * *Files identical despite different names*

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool/assets/unrar.exe` & `BookerWikiTool-2023.3.30.0/BookerWikiTool/assets/unrar.exe`

 * *Files identical despite different names*

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool/chatgpt.py` & `BookerWikiTool-2023.3.30.0/BookerWikiTool/chatgpt.py`

 * *Files identical despite different names*

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool/codelint.py` & `BookerWikiTool-2023.3.30.0/BookerWikiTool/codelint.py`

 * *Files identical despite different names*

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool/crawl_wx.py` & `BookerWikiTool-2023.3.30.0/BookerWikiTool/crawl_wx.py`

 * *Files identical despite different names*

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool/epub_tool.py` & `BookerWikiTool-2023.3.30.0/BookerWikiTool/epub_tool.py`

 * *Files identical despite different names*

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool/fetch_links.py` & `BookerWikiTool-2023.3.30.0/BookerWikiTool/fetch_links.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from urllib.parse import urljoin
+from urllib.parse import urljoin, urlparse
 from EpubCrawler.util import request_retry
 from pyquery import PyQuery as pq
 import json
 import re
 import subprocess as subp
 from .util import *
 
@@ -85,37 +85,38 @@
         if len(toc) == 0: break
         for it in toc:
             print(it)
             ofile.write(it + '\n')
     
     ofile.close()
 
-def time_match_to_str(m):
+def get_date_from_url(url, rgx):
+    m = re.search('#' + rgx, url)
+    if not m: return '000101'
     yr = m.group(1)
     mon = m.group(2)
     if len(mon) == 1: mon = '0' + mon
     return yr + mon
 
 def batch_links(args):
     num = args.num
+    if not args.name:
+        args.name = re.sub(r'\.\w+$', '', path.basename(args.links))
     links = open(args.links, encoding='utf8').read().split('\n')
     links = list(filter(None, links))
     
-    dates = [re.search('#' + args.time_regex, l) for l in links]
-    if not all(dates):
-        print('未能提取文章发布时间')
-        return
+    dates = [get_date_from_url(l, args.time_regex) for l in links]
     
     for i in range(0, len(links), args.num):
-        st = time_match_to_str(dates[i])
-        ed = time_match_to_str(dates[i:i+args.num][-1])
+        st = dates[i]
+        ed = dates[i:i+args.num][-1]
         if st > ed: st, ed = ed, st
         
         cfg = {
-            'name': f'{args.name} {st}-{ed}',
+            'name': f'{args.name}_{st}_{ed}',
             'url': links[i],
             'title': args.title,
             'content': args.content,
             'remove': args.remove,
             'optiMode': args.opti_mode,
             'list': links[i:i+args.num],
             'sizeLimit': args.size_limit,
@@ -125,26 +126,31 @@
         open(cfg_fname, 'w', encoding='utf8').write(json.dumps(cfg))
         print(cfg_fname)
         if args.exec:
             subp.Popen(['crawl-epub', cfg_fname], shell=True).communicate()
         
         
 def fetch_sitemap_handle(args):
+    if not args.ofname:
+        args.ofname = urlparse(args.url) \
+            .hostname \
+            .replace('.', '_') + '.txt'
     url, regex, ofname = args.url, args.regex, args.ofname
     urls = fetch_sitemap(url, regex)
     f = open(ofname, 'w', encoding='utf8')
     for u in urls:
         f.write(u + '\n')
         print(u)
     f.close()
 
         
 def fetch_sitemap(url, rgx):
-    xml = request_retry('GET', url).text
+    xml = request_retry('GET', url, headers=config['headers']).text
     urls = re.findall(r'<loc>(.+?)</loc>', xml)
+    urls = [u.strip() for u in urls]
     subs = [
         u for u in urls
         if u.endswith('.xml')
     ]
     res = []
     for s in subs:
         res += fetch_sitemap(s, rgx)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool/flatten.py` & `BookerWikiTool-2023.3.30.0/BookerWikiTool/flatten.py`

 * *Files identical despite different names*

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool/md_tool.py` & `BookerWikiTool-2023.3.30.0/BookerWikiTool/md_tool.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,671 +1,695 @@
-00000000: 696d 706f 7274 2061 7267 7061 7273 650a  import argparse.
-00000010: 696d 706f 7274 2072 6571 7565 7374 730a  import requests.
-00000020: 6672 6f6d 2072 6561 6461 6269 6c69 7479  from readability
-00000030: 2069 6d70 6f72 7420 446f 6375 6d65 6e74   import Document
-00000040: 0a69 6d70 6f72 7420 7465 6d70 6669 6c65  .import tempfile
-00000050: 0a69 6d70 6f72 7420 7575 6964 0a69 6d70  .import uuid.imp
-00000060: 6f72 7420 7375 6270 726f 6365 7373 2061  ort subprocess a
-00000070: 7320 7375 6270 0a69 6d70 6f72 7420 7265  s subp.import re
-00000080: 0a69 6d70 6f72 7420 6f73 0a69 6d70 6f72  .import os.impor
-00000090: 7420 7368 7574 696c 0a69 6d70 6f72 7420  t shutil.import 
-000000a0: 6a73 6f6e 0a69 6d70 6f72 7420 7961 6d6c  json.import yaml
-000000b0: 0a69 6d70 6f72 7420 7472 6163 6562 6163  .import tracebac
-000000c0: 6b0a 696d 706f 7274 2063 6f70 790a 6672  k.import copy.fr
-000000d0: 6f6d 206d 756c 7469 7072 6f63 6573 7369  om multiprocessi
-000000e0: 6e67 2069 6d70 6f72 7420 506f 6f6c 0a66  ng import Pool.f
-000000f0: 726f 6d20 7572 6c6c 6962 2e70 6172 7365  rom urllib.parse
-00000100: 2069 6d70 6f72 7420 7175 6f74 655f 706c   import quote_pl
-00000110: 7573 0a66 726f 6d20 6f73 2069 6d70 6f72  us.from os impor
-00000120: 7420 7061 7468 0a66 726f 6d20 7079 7175  t path.from pyqu
-00000130: 6572 7920 696d 706f 7274 2050 7951 7565  ery import PyQue
-00000140: 7279 2061 7320 7071 0a66 726f 6d20 6461  ry as pq.from da
-00000150: 7465 7469 6d65 2069 6d70 6f72 7420 6461  tetime import da
-00000160: 7465 7469 6d65 0a66 726f 6d20 636f 6c6c  tetime.from coll
-00000170: 6563 7469 6f6e 7320 696d 706f 7274 204f  ections import O
-00000180: 7264 6572 6564 4469 6374 0a66 726f 6d20  rderedDict.from 
-00000190: 4570 7562 4372 6177 6c65 722e 696d 6720  EpubCrawler.img 
-000001a0: 696d 706f 7274 2070 726f 6365 7373 5f69  import process_i
-000001b0: 6d67 0a66 726f 6d20 4570 7562 4372 6177  mg.from EpubCraw
-000001c0: 6c65 722e 7574 696c 2069 6d70 6f72 7420  ler.util import 
-000001d0: 7361 6665 5f6d 6b64 6972 0a66 726f 6d20  safe_mkdir.from 
-000001e0: 2e75 7469 6c20 696d 706f 7274 202a 0a66  .util import *.f
-000001f0: 726f 6d20 2e66 6d74 2069 6d70 6f72 7420  rom .fmt import 
-00000200: 2a0a 0a64 6566 2061 6363 6f75 6e74 5f68  *..def account_h
-00000210: 616e 646c 6528 6172 6773 293a 0a20 2020  andle(args):.   
-00000220: 2069 6620 6e6f 7420 6172 6773 2e66 696c   if not args.fil
-00000230: 652e 656e 6473 7769 7468 2827 2e6d 6427  e.endswith('.md'
-00000240: 293a 0a20 2020 2020 2020 2070 7269 6e74  ):.        print
-00000250: 2827 e8af b7e6 8f90 e4be 9b20 6d61 726b  ('......... mark
-00000260: 646f 776e 20e6 9687 e4bb b627 290a 2020  down ......').  
-00000270: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-00000280: 2070 7269 6e74 2861 7267 732e 6669 6c65   print(args.file
-00000290: 290a 2020 2020 636f 6e74 203d 206f 7065  ).    cont = ope
-000002a0: 6e28 6172 6773 2e66 696c 652c 2065 6e63  n(args.file, enc
-000002b0: 6f64 696e 673d 2775 7466 3827 292e 7265  oding='utf8').re
-000002c0: 6164 2829 0a20 2020 2074 6f74 616c 2c20  ad().    total, 
-000002d0: 7a68 5f63 6f75 6e74 2c20 656e 5f63 6f75  zh_count, en_cou
-000002e0: 6e74 203d 2061 6363 6f75 6e74 5f77 6f72  nt = account_wor
-000002f0: 6473 2863 6f6e 7429 0a20 2020 2070 7269  ds(cont).    pri
-00000300: 6e74 2866 27e4 b8ad e696 87e5 ad97 e695  nt(f'...........
-00000310: b0ef bc9a 7b7a 685f 636f 756e 747d 5c6e  ....{zh_count}\n
-00000320: e88b b1e6 9687 e5ad 97e6 95b0 efbc 9a7b  ...............{
-00000330: 656e 5f63 6f75 6e74 7d5c 6ee6 80bb e5ad  en_count}\n.....
-00000340: 97e6 95b0 efbc 9a7b 746f 7461 6c7d 2729  .......{total}')
-00000350: 0a0a 6465 6620 7265 6e5f 6d64 5f68 616e  ..def ren_md_han
-00000360: 646c 6528 6172 6773 293a 0a20 2020 2069  dle(args):.    i
-00000370: 6620 7061 7468 2e69 7364 6972 2861 7267  f path.isdir(arg
-00000380: 732e 666e 616d 6529 3a0a 2020 2020 2020  s.fname):.      
-00000390: 2020 7265 6e5f 6d64 5f64 6972 2861 7267    ren_md_dir(arg
-000003a0: 7329 0a20 2020 2065 6c73 653a 0a20 2020  s).    else:.   
-000003b0: 2020 2020 2072 656e 5f6d 645f 6669 6c65       ren_md_file
-000003c0: 2861 7267 7329 0a0a 6465 6620 7265 6e5f  (args)..def ren_
-000003d0: 6d64 5f64 6972 2861 7267 7329 3a0a 2020  md_dir(args):.  
-000003e0: 2020 6469 7220 3d20 6172 6773 2e66 6e61    dir = args.fna
-000003f0: 6d65 0a20 2020 2066 6e61 6d65 7320 3d20  me.    fnames = 
-00000400: 6f73 2e6c 6973 7464 6972 2864 6972 290a  os.listdir(dir).
-00000410: 2020 2020 706f 6f6c 203d 2050 6f6f 6c28      pool = Pool(
-00000420: 6172 6773 2e74 6872 6561 6473 290a 2020  args.threads).  
-00000430: 2020 666f 7220 6620 696e 2066 6e61 6d65    for f in fname
-00000440: 733a 0a20 2020 2020 2020 2061 7267 7320  s:.        args 
-00000450: 3d20 636f 7079 2e64 6565 7063 6f70 7928  = copy.deepcopy(
-00000460: 6172 6773 290a 2020 2020 2020 2020 6172  args).        ar
-00000470: 6773 2e66 6e61 6d65 203d 2070 6174 682e  gs.fname = path.
-00000480: 6a6f 696e 2864 6972 2c20 6629 0a20 2020  join(dir, f).   
-00000490: 2020 2020 2070 6f6f 6c2e 6170 706c 795f       pool.apply_
-000004a0: 6173 796e 6328 7265 6e5f 6d64 5f66 696c  async(ren_md_fil
-000004b0: 655f 7361 6665 2c20 5b61 7267 735d 290a  e_safe, [args]).
-000004c0: 2020 2020 706f 6f6c 2e63 6c6f 7365 2829      pool.close()
-000004d0: 0a20 2020 2070 6f6f 6c2e 6a6f 696e 2829  .    pool.join()
-000004e0: 0a0a 6465 6620 7265 6e5f 6d64 5f66 696c  ..def ren_md_fil
-000004f0: 655f 7361 6665 2861 7267 7329 3a0a 2020  e_safe(args):.  
-00000500: 2020 7472 793a 2072 656e 5f6d 645f 6669    try: ren_md_fi
-00000510: 6c65 2861 7267 7329 0a20 2020 2065 7863  le(args).    exc
-00000520: 6570 743a 2074 7261 6365 6261 636b 2e70  ept: traceback.p
-00000530: 7269 6e74 5f65 7863 2829 0a0a 6465 6620  rint_exc()..def 
-00000540: 7265 6e5f 6d64 5f66 696c 6528 6172 6773  ren_md_file(args
-00000550: 293a 0a20 2020 2066 6e61 6d65 203d 2061  ):.    fname = a
-00000560: 7267 732e 666e 616d 650a 2020 2020 6966  rgs.fname.    if
-00000570: 206e 6f74 2066 6e61 6d65 2e65 6e64 7377   not fname.endsw
-00000580: 6974 6828 272e 6d64 2729 3a0a 2020 2020  ith('.md'):.    
-00000590: 2020 2020 7072 696e 7428 27e8 afb7 e68f      print('.....
-000005a0: 90e4 be9b 206d 6172 6b64 6f77 6e20 e696  .... markdown ..
-000005b0: 87e4 bbb6 2729 0a20 2020 2020 2020 2072  ....').        r
-000005c0: 6574 7572 6e0a 2020 2020 636f 6e74 203d  eturn.    cont =
-000005d0: 206f 7065 6e28 666e 616d 652c 2065 6e63   open(fname, enc
-000005e0: 6f64 696e 673d 2775 7466 3827 292e 7265  oding='utf8').re
-000005f0: 6164 2829 0a20 2020 2064 6972 203d 2070  ad().    dir = p
-00000600: 6174 682e 6469 726e 616d 6528 666e 616d  ath.dirname(fnam
-00000610: 6529 0a20 2020 2052 4520 3d20 5245 5f53  e).    RE = RE_S
-00000620: 4f55 5243 4520 6966 2061 7267 732e 6279  OURCE if args.by
-00000630: 203d 3d20 2773 7263 2720 656c 7365 2052   == 'src' else R
-00000640: 455f 5449 544c 450a 2020 2020 726d 203d  E_TITLE.    rm =
-00000650: 2072 652e 7365 6172 6368 2852 452c 2063   re.search(RE, c
-00000660: 6f6e 742c 2066 6c61 6773 3d72 652e 4d29  ont, flags=re.M)
-00000670: 0a20 2020 2069 6620 6e6f 7420 726d 3a20  .    if not rm: 
-00000680: 0a20 2020 2020 2020 2070 7269 6e74 2866  .        print(f
-00000690: 277b 666e 616d 657d 20e6 9caa e689 bee5  '{fname} .......
-000006a0: 88b0 e696 87e4 bbb6 e590 8d27 290a 2020  ...........').  
-000006b0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-000006c0: 206e 666e 616d 6520 3d20 726d 2e67 726f   nfname = rm.gro
-000006d0: 7570 2831 290a 2020 2020 6e66 6e61 6d65  up(1).    nfname
-000006e0: 203d 2072 652e 7375 6228 7227 5c73 272c   = re.sub(r'\s',
-000006f0: 2027 2d27 2c20 666e 616d 655f 6573 6361   '-', fname_esca
-00000700: 7065 286e 666e 616d 6529 2920 2b20 272e  pe(nfname)) + '.
-00000710: 6d64 270a 2020 2020 6e66 6e61 6d65 203d  md'.    nfname =
-00000720: 2070 6174 682e 6a6f 696e 2864 6972 2c20   path.join(dir, 
-00000730: 6e66 6e61 6d65 290a 2020 2020 7072 696e  nfname).    prin
-00000740: 7428 6e66 6e61 6d65 290a 2020 2020 7368  t(nfname).    sh
-00000750: 7574 696c 2e6d 6f76 6528 666e 616d 652c  util.move(fname,
-00000760: 206e 666e 616d 6529 0a0a 6465 6620 646f   nfname)..def do
-00000770: 776e 6c6f 6164 5f68 616e 646c 6528 6172  wnload_handle(ar
-00000780: 6773 293a 0a20 2020 2068 746d 6c20 3d20  gs):.    html = 
-00000790: 7265 7175 6573 7473 2e67 6574 280a 2020  requests.get(.  
-000007a0: 2020 2020 2020 6172 6773 2e75 726c 2c0a        args.url,.
-000007b0: 2020 2020 2020 2020 6865 6164 6572 733d          headers=
-000007c0: 6465 6661 756c 745f 6864 7273 2c0a 2020  default_hdrs,.  
-000007d0: 2020 292e 636f 6e74 656e 742e 6465 636f    ).content.deco
-000007e0: 6465 2861 7267 732e 656e 636f 6469 6e67  de(args.encoding
-000007f0: 2c20 2769 676e 6f72 6527 290a 2020 2020  , 'ignore').    
-00000800: 0a20 2020 2023 20e8 a7a3 e69e 90e6 a087  .    # .........
-00000810: e9a2 980a 2020 2020 7274 203d 2070 7128  ....    rt = pq(
-00000820: 6874 6d6c 290a 2020 2020 656c 5f74 6974  html).    el_tit
-00000830: 6c65 203d 2072 742e 6669 6e64 2861 7267  le = rt.find(arg
-00000840: 732e 7469 746c 6529 2e65 7128 3029 0a20  s.title).eq(0). 
-00000850: 2020 2074 6974 6c65 203d 2065 6c5f 7469     title = el_ti
-00000860: 746c 652e 7465 7874 2829 2e73 7472 6970  tle.text().strip
-00000870: 2829 0a20 2020 2065 6c5f 7469 746c 652e  ().    el_title.
-00000880: 7265 6d6f 7665 2829 0a20 2020 200a 2020  remove().    .  
-00000890: 2020 2320 e588 a4e6 96ad e698 afe5 90a6    # ............
-000008a0: e987 8de5 a48d 0a20 2020 2074 6974 6c65  .......    title
-000008b0: 5f65 7363 203d 2072 652e 7375 6228 7227  _esc = re.sub(r'
-000008c0: 5c73 272c 2027 2d27 2c20 666e 616d 655f  \s', '-', fname_
-000008d0: 6573 6361 7065 2874 6974 6c65 2929 0a20  escape(title)). 
-000008e0: 2020 2066 6e61 6d65 203d 2066 2764 6f63     fname = f'doc
-000008f0: 732f 7b74 6974 6c65 5f65 7363 7d2e 6d64  s/{title_esc}.md
-00000900: 270a 2020 2020 6966 2070 6174 682e 6973  '.    if path.is
-00000910: 6669 6c65 2866 6e61 6d65 293a 0a20 2020  file(fname):.   
+00000000: 696d 706f 7274 2061 7267 7061 7273 650d  import argparse.
+00000010: 0a69 6d70 6f72 7420 7265 7175 6573 7473  .import requests
+00000020: 0d0a 6672 6f6d 2072 6561 6461 6269 6c69  ..from readabili
+00000030: 7479 2069 6d70 6f72 7420 446f 6375 6d65  ty import Docume
+00000040: 6e74 0d0a 696d 706f 7274 2074 656d 7066  nt..import tempf
+00000050: 696c 650d 0a69 6d70 6f72 7420 7575 6964  ile..import uuid
+00000060: 0d0a 696d 706f 7274 2073 7562 7072 6f63  ..import subproc
+00000070: 6573 7320 6173 2073 7562 700d 0a69 6d70  ess as subp..imp
+00000080: 6f72 7420 7265 0d0a 696d 706f 7274 206f  ort re..import o
+00000090: 730d 0a69 6d70 6f72 7420 7368 7574 696c  s..import shutil
+000000a0: 0d0a 696d 706f 7274 206a 736f 6e0d 0a69  ..import json..i
+000000b0: 6d70 6f72 7420 7961 6d6c 0d0a 696d 706f  mport yaml..impo
+000000c0: 7274 2074 7261 6365 6261 636b 0d0a 696d  rt traceback..im
+000000d0: 706f 7274 2063 6f70 790d 0a66 726f 6d20  port copy..from 
+000000e0: 6d75 6c74 6970 726f 6365 7373 696e 6720  multiprocessing 
+000000f0: 696d 706f 7274 2050 6f6f 6c0d 0a66 726f  import Pool..fro
+00000100: 6d20 7572 6c6c 6962 2e70 6172 7365 2069  m urllib.parse i
+00000110: 6d70 6f72 7420 7175 6f74 655f 706c 7573  mport quote_plus
+00000120: 0d0a 6672 6f6d 206f 7320 696d 706f 7274  ..from os import
+00000130: 2070 6174 680d 0a66 726f 6d20 7079 7175   path..from pyqu
+00000140: 6572 7920 696d 706f 7274 2050 7951 7565  ery import PyQue
+00000150: 7279 2061 7320 7071 0d0a 6672 6f6d 2064  ry as pq..from d
+00000160: 6174 6574 696d 6520 696d 706f 7274 2064  atetime import d
+00000170: 6174 6574 696d 650d 0a66 726f 6d20 636f  atetime..from co
+00000180: 6c6c 6563 7469 6f6e 7320 696d 706f 7274  llections import
+00000190: 204f 7264 6572 6564 4469 6374 0d0a 6672   OrderedDict..fr
+000001a0: 6f6d 2045 7075 6243 7261 776c 6572 2e69  om EpubCrawler.i
+000001b0: 6d67 2069 6d70 6f72 7420 7072 6f63 6573  mg import proces
+000001c0: 735f 696d 670d 0a66 726f 6d20 4570 7562  s_img..from Epub
+000001d0: 4372 6177 6c65 722e 7574 696c 2069 6d70  Crawler.util imp
+000001e0: 6f72 7420 7361 6665 5f6d 6b64 6972 0d0a  ort safe_mkdir..
+000001f0: 6672 6f6d 202e 7574 696c 2069 6d70 6f72  from .util impor
+00000200: 7420 2a0d 0a66 726f 6d20 2e66 6d74 2069  t *..from .fmt i
+00000210: 6d70 6f72 7420 2a0d 0a0d 0a64 6566 2061  mport *....def a
+00000220: 6363 6f75 6e74 5f68 616e 646c 6528 6172  ccount_handle(ar
+00000230: 6773 293a 0d0a 2020 2020 6966 206e 6f74  gs):..    if not
+00000240: 2061 7267 732e 6669 6c65 2e65 6e64 7377   args.file.endsw
+00000250: 6974 6828 272e 6d64 2729 3a0d 0a20 2020  ith('.md'):..   
+00000260: 2020 2020 2070 7269 6e74 2827 e8af b7e6       print('....
+00000270: 8f90 e4be 9b20 6d61 726b 646f 776e 20e6  ..... markdown .
+00000280: 9687 e4bb b627 290d 0a20 2020 2020 2020  .....')..       
+00000290: 2072 6574 7572 6e0d 0a20 2020 2070 7269   return..    pri
+000002a0: 6e74 2861 7267 732e 6669 6c65 290d 0a20  nt(args.file).. 
+000002b0: 2020 2063 6f6e 7420 3d20 6f70 656e 2861     cont = open(a
+000002c0: 7267 732e 6669 6c65 2c20 656e 636f 6469  rgs.file, encodi
+000002d0: 6e67 3d27 7574 6638 2729 2e72 6561 6428  ng='utf8').read(
+000002e0: 290d 0a20 2020 2074 6f74 616c 2c20 7a68  )..    total, zh
+000002f0: 5f63 6f75 6e74 2c20 656e 5f63 6f75 6e74  _count, en_count
+00000300: 203d 2061 6363 6f75 6e74 5f77 6f72 6473   = account_words
+00000310: 2863 6f6e 7429 0d0a 2020 2020 7072 696e  (cont)..    prin
+00000320: 7428 6627 e4b8 ade6 9687 e5ad 97e6 95b0  t(f'............
+00000330: efbc 9a7b 7a68 5f63 6f75 6e74 7d5c 6ee8  ...{zh_count}\n.
+00000340: 8bb1 e696 87e5 ad97 e695 b0ef bc9a 7b65  ..............{e
+00000350: 6e5f 636f 756e 747d 5c6e e680 bbe5 ad97  n_count}\n......
+00000360: e695 b0ef bc9a 7b74 6f74 616c 7d27 290d  ......{total}').
+00000370: 0a0d 0a64 6566 2072 656e 5f6d 645f 6861  ...def ren_md_ha
+00000380: 6e64 6c65 2861 7267 7329 3a0d 0a20 2020  ndle(args):..   
+00000390: 2069 6620 7061 7468 2e69 7364 6972 2861   if path.isdir(a
+000003a0: 7267 732e 666e 616d 6529 3a0d 0a20 2020  rgs.fname):..   
+000003b0: 2020 2020 2072 656e 5f6d 645f 6469 7228       ren_md_dir(
+000003c0: 6172 6773 290d 0a20 2020 2065 6c73 653a  args)..    else:
+000003d0: 0d0a 2020 2020 2020 2020 7265 6e5f 6d64  ..        ren_md
+000003e0: 5f66 696c 6528 6172 6773 290d 0a0d 0a64  _file(args)....d
+000003f0: 6566 2072 656e 5f6d 645f 6469 7228 6172  ef ren_md_dir(ar
+00000400: 6773 293a 0d0a 2020 2020 6469 7220 3d20  gs):..    dir = 
+00000410: 6172 6773 2e66 6e61 6d65 0d0a 2020 2020  args.fname..    
+00000420: 666e 616d 6573 203d 206f 732e 6c69 7374  fnames = os.list
+00000430: 6469 7228 6469 7229 0d0a 2020 2020 706f  dir(dir)..    po
+00000440: 6f6c 203d 2050 6f6f 6c28 6172 6773 2e74  ol = Pool(args.t
+00000450: 6872 6561 6473 290d 0a20 2020 2066 6f72  hreads)..    for
+00000460: 2066 2069 6e20 666e 616d 6573 3a0d 0a20   f in fnames:.. 
+00000470: 2020 2020 2020 2061 7267 7320 3d20 636f         args = co
+00000480: 7079 2e64 6565 7063 6f70 7928 6172 6773  py.deepcopy(args
+00000490: 290d 0a20 2020 2020 2020 2061 7267 732e  )..        args.
+000004a0: 666e 616d 6520 3d20 7061 7468 2e6a 6f69  fname = path.joi
+000004b0: 6e28 6469 722c 2066 290d 0a20 2020 2020  n(dir, f)..     
+000004c0: 2020 2070 6f6f 6c2e 6170 706c 795f 6173     pool.apply_as
+000004d0: 796e 6328 7265 6e5f 6d64 5f66 696c 652c  ync(ren_md_file,
+000004e0: 205b 6172 6773 5d29 0d0a 2020 2020 706f   [args])..    po
+000004f0: 6f6c 2e63 6c6f 7365 2829 0d0a 2020 2020  ol.close()..    
+00000500: 706f 6f6c 2e6a 6f69 6e28 290d 0a0d 0a23  pool.join()....#
+00000510: 2040 7361 6665 2829 0d0a 6465 6620 7265   @safe()..def re
+00000520: 6e5f 6d64 5f66 696c 6528 6172 6773 293a  n_md_file(args):
+00000530: 0d0a 2020 2020 666e 616d 6520 3d20 6172  ..    fname = ar
+00000540: 6773 2e66 6e61 6d65 0d0a 2020 2020 6966  gs.fname..    if
+00000550: 206e 6f74 2066 6e61 6d65 2e65 6e64 7377   not fname.endsw
+00000560: 6974 6828 272e 6d64 2729 3a0d 0a20 2020  ith('.md'):..   
+00000570: 2020 2020 2070 7269 6e74 2827 e8af b7e6       print('....
+00000580: 8f90 e4be 9b20 6d61 726b 646f 776e 20e6  ..... markdown .
+00000590: 9687 e4bb b627 290d 0a20 2020 2020 2020  .....')..       
+000005a0: 2072 6574 7572 6e0d 0a20 2020 2063 6f6e   return..    con
+000005b0: 7420 3d20 6f70 656e 2866 6e61 6d65 2c20  t = open(fname, 
+000005c0: 656e 636f 6469 6e67 3d27 7574 6638 2729  encoding='utf8')
+000005d0: 2e72 6561 6428 290d 0a20 2020 2064 6972  .read()..    dir
+000005e0: 203d 2070 6174 682e 6469 726e 616d 6528   = path.dirname(
+000005f0: 666e 616d 6529 0d0a 2020 2020 5245 203d  fname)..    RE =
+00000600: 2052 455f 534f 5552 4345 2069 6620 6172   RE_SOURCE if ar
+00000610: 6773 2e62 7920 3d3d 2027 7372 6327 2065  gs.by == 'src' e
+00000620: 6c73 6520 5245 5f54 4954 4c45 0d0a 2020  lse RE_TITLE..  
+00000630: 2020 726d 203d 2072 652e 7365 6172 6368    rm = re.search
+00000640: 2852 452c 2063 6f6e 742c 2066 6c61 6773  (RE, cont, flags
+00000650: 3d72 652e 4d29 0d0a 2020 2020 6966 206e  =re.M)..    if n
+00000660: 6f74 2072 6d3a 200d 0a20 2020 2020 2020  ot rm: ..       
+00000670: 2070 7269 6e74 2866 277b 666e 616d 657d   print(f'{fname}
+00000680: 20e6 9caa e689 bee5 88b0 e696 87e4 bbb6   ...............
+00000690: e590 8d27 290d 0a20 2020 2020 2020 2072  ...')..        r
+000006a0: 6574 7572 6e0d 0a20 2020 206e 666e 616d  eturn..    nfnam
+000006b0: 6520 3d20 726d 2e67 726f 7570 2831 290d  e = rm.group(1).
+000006c0: 0a20 2020 206e 666e 616d 6520 3d20 7265  .    nfname = re
+000006d0: 2e73 7562 2872 275c 7327 2c20 272d 272c  .sub(r'\s', '-',
+000006e0: 2066 6e61 6d65 5f65 7363 6170 6528 6e66   fname_escape(nf
+000006f0: 6e61 6d65 2929 202b 2027 2e6d 6427 0d0a  name)) + '.md'..
+00000700: 2020 2020 6e66 6e61 6d65 203d 2070 6174      nfname = pat
+00000710: 682e 6a6f 696e 2864 6972 2c20 6e66 6e61  h.join(dir, nfna
+00000720: 6d65 290d 0a20 2020 2070 7269 6e74 286e  me)..    print(n
+00000730: 666e 616d 6529 0d0a 2020 2020 7368 7574  fname)..    shut
+00000740: 696c 2e6d 6f76 6528 666e 616d 652c 206e  il.move(fname, n
+00000750: 666e 616d 6529 0d0a 0d0a 6465 6620 646f  fname)....def do
+00000760: 776e 6c6f 6164 5f68 616e 646c 6528 6172  wnload_handle(ar
+00000770: 6773 293a 0d0a 2020 2020 6874 6d6c 203d  gs):..    html =
+00000780: 2072 6571 7565 7374 732e 6765 7428 0d0a   requests.get(..
+00000790: 2020 2020 2020 2020 6172 6773 2e75 726c          args.url
+000007a0: 2c0d 0a20 2020 2020 2020 2068 6561 6465  ,..        heade
+000007b0: 7273 3d64 6566 6175 6c74 5f68 6472 732c  rs=default_hdrs,
+000007c0: 0d0a 2020 2020 292e 636f 6e74 656e 742e  ..    ).content.
+000007d0: 6465 636f 6465 2861 7267 732e 656e 636f  decode(args.enco
+000007e0: 6469 6e67 2c20 2769 676e 6f72 6527 290d  ding, 'ignore').
+000007f0: 0a20 2020 200d 0a20 2020 2023 20e8 a7a3  .    ..    # ...
+00000800: e69e 90e6 a087 e9a2 980d 0a20 2020 2072  ...........    r
+00000810: 7420 3d20 7071 2868 746d 6c29 0d0a 2020  t = pq(html)..  
+00000820: 2020 656c 5f74 6974 6c65 203d 2072 742e    el_title = rt.
+00000830: 6669 6e64 2861 7267 732e 7469 746c 6529  find(args.title)
+00000840: 2e65 7128 3029 0d0a 2020 2020 7469 746c  .eq(0)..    titl
+00000850: 6520 3d20 656c 5f74 6974 6c65 2e74 6578  e = el_title.tex
+00000860: 7428 292e 7374 7269 7028 290d 0a20 2020  t().strip()..   
+00000870: 2065 6c5f 7469 746c 652e 7265 6d6f 7665   el_title.remove
+00000880: 2829 0d0a 2020 2020 0d0a 2020 2020 2320  ()..    ..    # 
+00000890: e588 a4e6 96ad e698 afe5 90a6 e987 8de5  ................
+000008a0: a48d 0d0a 2020 2020 7469 746c 655f 6573  ....    title_es
+000008b0: 6320 3d20 7265 2e73 7562 2872 275c 7327  c = re.sub(r'\s'
+000008c0: 2c20 272d 272c 2066 6e61 6d65 5f65 7363  , '-', fname_esc
+000008d0: 6170 6528 7469 746c 6529 290d 0a20 2020  ape(title))..   
+000008e0: 2066 6e61 6d65 203d 2066 2764 6f63 732f   fname = f'docs/
+000008f0: 7b74 6974 6c65 5f65 7363 7d2e 6d64 270d  {title_esc}.md'.
+00000900: 0a20 2020 2069 6620 7061 7468 2e69 7366  .    if path.isf
+00000910: 696c 6528 666e 616d 6529 3a0d 0a20 2020  ile(fname):..   
 00000920: 2020 2020 2070 7269 6e74 2866 277b 7469       print(f'{ti
 00000930: 746c 657d 20e5 b7b2 e5ad 98e5 9ca8 2729  tle} .........')
-00000940: 0a20 2020 2020 2020 2072 6574 7572 6e0a  .        return.
-00000950: 2020 2020 0a20 2020 2023 20e8 a7a3 e69e      .    # .....
-00000960: 90e5 8685 e5ae b9e5 b9b6 e4b8 8be8 bdbd  ................
-00000970: e59b bee7 8987 0a20 2020 2069 6620 6172  .......    if ar
-00000980: 6773 2e62 6f64 793a 0a20 2020 2020 2020  gs.body:.       
-00000990: 2063 6f20 3d20 7274 2e66 696e 6428 6172   co = rt.find(ar
-000009a0: 6773 2e62 6f64 7929 2e68 746d 6c28 290a  gs.body).html().
-000009b0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000009c0: 2020 636f 203d 2044 6f63 756d 656e 7428    co = Document(
-000009d0: 7374 7228 7274 2929 2e73 756d 6d61 7279  str(rt)).summary
-000009e0: 2829 0a20 2020 2020 2020 2063 6f20 3d20  ().        co = 
-000009f0: 7071 2863 6f29 2e66 696e 6428 2762 6f64  pq(co).find('bod
-00000a00: 7927 292e 6874 6d6c 2829 0a20 2020 2069  y').html().    i
-00000a10: 6620 6e6f 7420 636f 3a20 0a20 2020 2020  f not co: .     
-00000a20: 2020 2070 7269 6e74 2827 e69c aae8 8eb7     print('......
-00000a30: e58f 96e5 88b0 e586 85e5 aeb9 efbc 8127  ...............'
-00000a40: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00000a50: 200a 2020 2020 696d 6773 203d 207b 7d0a   .    imgs = {}.
-00000a60: 2020 2020 636f 203d 2070 726f 6365 7373      co = process
-00000a70: 5f69 6d67 2863 6f2c 2069 6d67 732c 2069  _img(co, imgs, i
-00000a80: 6d67 5f70 7265 6669 783d 2769 6d67 2f27  mg_prefix='img/'
-00000a90: 2c20 7061 6765 5f75 726c 3d61 7267 732e  , page_url=args.
-00000aa0: 7572 6c29 0a20 2020 2068 746d 6c20 3d20  url).    html = 
-00000ab0: 6627 2727 0a20 2020 203c 6874 6d6c 3e3c  f'''.    <html><
-00000ac0: 626f 6479 3e0a 2020 2020 3c68 313e 7b74  body>.    <h1>{t
-00000ad0: 6974 6c65 7d3c 2f68 313e 0a20 2020 203c  itle}</h1>.    <
-00000ae0: 626c 6f63 6b71 756f 7465 3e0a 2020 2020  blockquote>.    
-00000af0: e69d a5e6 ba90 efbc 9a3c 6120 6872 6566  .........<a href
-00000b00: 3d27 7b61 7267 732e 7572 6c7d 273e 7b61  ='{args.url}'>{a
-00000b10: 7267 732e 7572 6c7d 3c2f 613e 0a20 2020  rgs.url}</a>.   
-00000b20: 203c 2f62 6c6f 636b 7175 6f74 653e 0a20   </blockquote>. 
-00000b30: 2020 207b 636f 7d3c 2f62 6f64 793e 3c2f     {co}</body></
-00000b40: 6874 6d6c 3e0a 2020 2020 2727 270a 2020  html>.    '''.  
-00000b50: 2020 0a20 2020 2023 20e8 bdac e68d a220    .    # ...... 
-00000b60: 6d64 0a20 2020 206d 6420 3d20 746f 6d64  md.    md = tomd
-00000b70: 2868 746d 6c29 0a20 2020 2023 206d 6420  (html).    # md 
-00000b80: 3d20 7265 2e73 7562 2852 455f 434f 4445  = re.sub(RE_CODE
-00000b90: 5f42 4c4f 434b 2c20 636f 6465 5f72 6570  _BLOCK, code_rep
-00000ba0: 6c61 6365 5f66 756e 632c 206d 6429 0a20  lace_func, md). 
-00000bb0: 2020 2079 616d 6c5f 6865 6164 203d 2027     yaml_head = '
-00000bc0: 5c6e 272e 6a6f 696e 285b 0a20 2020 2020  \n'.join([.     
-00000bd0: 2020 2027 3c21 2d2d 796d 6c27 2c0a 2020     '<!--yml',.  
-00000be0: 2020 2020 2020 2763 6174 6567 6f72 793a        'category:
-00000bf0: 2027 202b 2061 7267 732e 6361 7465 676f   ' + args.catego
-00000c00: 7279 2c0a 2020 2020 2020 2020 2764 6174  ry,.        'dat
-00000c10: 653a 2027 202b 2064 6174 6574 696d 652e  e: ' + datetime.
-00000c20: 6e6f 7728 292e 7374 7266 7469 6d65 2827  now().strftime('
-00000c30: 2559 2d25 6d2d 2564 2025 483a 254d 3a25  %Y-%m-%d %H:%M:%
-00000c40: 5327 292c 0a20 2020 2020 2020 2027 2d2d  S'),.        '--
-00000c50: 3e27 2c0a 2020 2020 5d29 0a20 2020 206d  >',.    ]).    m
-00000c60: 6420 3d20 6627 7b79 616d 6c5f 6865 6164  d = f'{yaml_head
-00000c70: 7d5c 6e5c 6e7b 6d64 7d27 0a20 2020 200a  }\n\n{md}'.    .
-00000c80: 2020 2020 2320 e586 99e5 85a5 e7a1 ace7      # ..........
-00000c90: 9b98 0a20 2020 2073 6166 655f 6d6b 6469  ...    safe_mkdi
-00000ca0: 7228 2764 6f63 7327 290a 2020 2020 7361  r('docs').    sa
-00000cb0: 6665 5f6d 6b64 6972 2827 646f 6373 2f69  fe_mkdir('docs/i
-00000cc0: 6d67 2729 0a20 2020 206f 7065 6e28 666e  mg').    open(fn
-00000cd0: 616d 652c 2027 7727 2c20 656e 636f 6469  ame, 'w', encodi
-00000ce0: 6e67 3d27 7574 662d 3827 292e 7772 6974  ng='utf-8').writ
-00000cf0: 6528 6d64 290a 2020 2020 666f 7220 6e61  e(md).    for na
-00000d00: 6d65 2c20 6461 7461 2069 6e20 696d 6773  me, data in imgs
-00000d10: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-00000d20: 2020 6f70 656e 2866 2764 6f63 732f 696d    open(f'docs/im
-00000d30: 672f 7b6e 616d 657d 272c 2027 7762 2729  g/{name}', 'wb')
-00000d40: 2e77 7269 7465 2864 6174 6129 0a20 2020  .write(data).   
-00000d50: 2020 2020 200a 2020 2020 7072 696e 7428       .    print(
-00000d60: 27e5 b7b2 e5ae 8ce6 8890 2729 0a20 2020  '.........').   
-00000d70: 200a 6465 6620 7375 6d6d 6172 795f 6861   .def summary_ha
-00000d80: 6e64 6c65 2861 7267 7329 3a0a 2020 2020  ndle(args):.    
-00000d90: 2320 e8af bbe5 85a5 e696 87e4 bbb6 e588  # ..............
-00000da0: 97e8 a1a8 0a20 2020 2064 6972 203d 2061  .....    dir = a
-00000db0: 7267 732e 6469 720a 2020 2020 666e 616d  rgs.dir.    fnam
-00000dc0: 6573 203d 205b 6620 666f 7220 6620 696e  es = [f for f in
-00000dd0: 206f 732e 6c69 7374 6469 7228 6469 7229   os.listdir(dir)
-00000de0: 2069 6620 662e 656e 6473 7769 7468 2827   if f.endswith('
-00000df0: 2e6d 6427 295d 0a20 2020 2074 6f63 203d  .md')].    toc =
-00000e00: 205b 5d0a 2020 2020 666f 7220 6620 696e   [].    for f in
-00000e10: 2066 6e61 6d65 733a 0a20 2020 2020 2020   fnames:.       
-00000e20: 2066 756c 6c66 203d 2070 6174 682e 6a6f   fullf = path.jo
-00000e30: 696e 2864 6972 2c20 6629 0a20 2020 2020  in(dir, f).     
-00000e40: 2020 2070 7269 6e74 2866 756c 6c66 290a     print(fullf).
-00000e50: 2020 2020 2020 2020 636f 6e74 203d 206f          cont = o
-00000e60: 7065 6e28 6675 6c6c 662c 2065 6e63 6f64  pen(fullf, encod
-00000e70: 696e 673d 2775 7466 3827 292e 7265 6164  ing='utf8').read
-00000e80: 2829 0a20 2020 2020 2020 206d 203d 2072  ().        m = r
-00000e90: 652e 7365 6172 6368 2852 455f 5449 544c  e.search(RE_TITL
-00000ea0: 452c 2063 6f6e 742c 2066 6c61 6773 3d72  E, cont, flags=r
-00000eb0: 652e 4d29 0a20 2020 2020 2020 2069 6620  e.M).        if 
-00000ec0: 6e6f 7420 6d3a 2063 6f6e 7469 6e75 650a  not m: continue.
-00000ed0: 2020 2020 2020 2020 7469 746c 6520 3d20          title = 
-00000ee0: 6d2e 6772 6f75 7028 3129 0a20 2020 2020  m.group(1).     
-00000ef0: 2020 2074 6f63 2e61 7070 656e 6428 6627     toc.append(f'
-00000f00: 2b20 2020 5b7b 7469 746c 657d 5d28 7b66  +   [{title}]({f
-00000f10: 7d29 2729 0a20 2020 2073 756d 6d61 7279  })').    summary
-00000f20: 203d 2027 5c6e 272e 6a6f 696e 2874 6f63   = '\n'.join(toc
-00000f30: 290a 2020 2020 6f70 656e 2870 6174 682e  ).    open(path.
-00000f40: 6a6f 696e 2864 6972 2c20 2753 554d 4d41  join(dir, 'SUMMA
-00000f50: 5259 2e6d 6427 292c 2027 7727 2c20 656e  RY.md'), 'w', en
-00000f60: 636f 6469 6e67 3d27 7574 6638 2729 2e77  coding='utf8').w
-00000f70: 7269 7465 2873 756d 6d61 7279 290a 2020  rite(summary).  
-00000f80: 2020 0a64 6566 2077 696b 695f 7375 6d6d    .def wiki_summ
-00000f90: 6172 795f 6861 6e64 6c65 2861 7267 7329  ary_handle(args)
-00000fa0: 3a0a 2020 2020 2320 e8af bbe5 85a5 e696  :.    # ........
-00000fb0: 87e4 bbb6 e588 97e8 a1a8 0a20 2020 2066  ...........    f
-00000fc0: 6e61 6d65 7320 3d20 5b66 2066 6f72 2066  names = [f for f
-00000fd0: 2069 6e20 6f73 2e6c 6973 7464 6972 2827   in os.listdir('
-00000fe0: 646f 6373 2729 2069 6620 662e 656e 6473  docs') if f.ends
-00000ff0: 7769 7468 2827 2e6d 6427 295d 0a20 2020  with('.md')].   
-00001000: 2074 6f63 203d 204f 7264 6572 6564 4469   toc = OrderedDi
-00001010: 6374 2829 0a20 2020 2066 6f72 2066 6e61  ct().    for fna
-00001020: 6d65 2069 6e20 666e 616d 6573 3a0a 2020  me in fnames:.  
-00001030: 2020 2020 2020 7072 696e 7428 666e 616d        print(fnam
-00001040: 6529 0a20 2020 2020 2020 206d 6420 3d20  e).        md = 
-00001050: 6f70 656e 2870 6174 682e 6a6f 696e 2827  open(path.join('
-00001060: 646f 6373 272c 2066 6e61 6d65 292c 2065  docs', fname), e
-00001070: 6e63 6f64 696e 673d 2775 7466 3827 292e  ncoding='utf8').
-00001080: 7265 6164 2829 0a20 2020 2020 2020 2023  read().        #
-00001090: 20e6 8f90 e58f 96e5 8583 e4bf a1e6 81af   ...............
-000010a0: 0a20 2020 2020 2020 206d 203d 2072 652e  .        m = re.
-000010b0: 7365 6172 6368 2852 455f 5941 4d4c 5f4d  search(RE_YAML_M
-000010c0: 4554 412c 206d 6429 0a20 2020 2020 2020  ETA, md).       
-000010d0: 2069 6620 6e6f 7420 6d3a 200a 2020 2020   if not m: .    
-000010e0: 2020 2020 2020 2020 7072 696e 7428 27e6          print('.
-000010f0: 9caa e689 bee5 88b0 e585 83e4 bfa1 e681  ................
-00001100: afef bc8c e5b7 b2e8 b7b3 e8bf 8727 290a  .............').
-00001110: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00001120: 696e 7565 0a20 2020 2020 2020 2074 7279  inue.        try
-00001130: 3a0a 2020 2020 2020 2020 2020 2020 6d65  :.            me
-00001140: 7461 203d 2079 616d 6c2e 7361 6665 5f6c  ta = yaml.safe_l
-00001150: 6f61 6428 6d2e 6772 6f75 7028 3129 290a  oad(m.group(1)).
-00001160: 2020 2020 2020 2020 6578 6365 7074 2045          except E
-00001170: 7863 6570 7469 6f6e 2061 7320 6578 3a20  xception as ex: 
-00001180: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
-00001190: 6365 6261 636b 2e70 7269 6e74 5f65 7863  ceback.print_exc
-000011a0: 2829 0a20 2020 2020 2020 2020 2020 2063  ().            c
-000011b0: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
-000011c0: 6474 203d 206d 6574 612e 6765 7428 2764  dt = meta.get('d
-000011d0: 6174 6527 2c20 2730 3030 312d 3031 2d30  ate', '0001-01-0
-000011e0: 3120 3030 3a30 303a 3030 2729 0a20 2020  1 00:00:00').   
-000011f0: 2020 2020 2063 6174 6520 3d20 6d65 7461       cate = meta
-00001200: 2e67 6574 2827 6361 7465 676f 7279 272c  .get('category',
-00001210: 2027 e69c aae5 8886 e7b1 bb27 290a 2020   '.........').  
-00001220: 2020 2020 2020 2320 e68f 90e5 8f96 e6a0        # ........
-00001230: 87e9 a298 0a20 2020 2020 2020 206d 203d  .....        m =
-00001240: 2072 652e 7365 6172 6368 2852 455f 5449   re.search(RE_TI
-00001250: 544c 452c 206d 642c 2066 6c61 6773 3d72  TLE, md, flags=r
-00001260: 652e 4d29 0a20 2020 2020 2020 2069 6620  e.M).        if 
-00001270: 6e6f 7420 6d3a 200a 2020 2020 2020 2020  not m: .        
-00001280: 2020 2020 7072 696e 7428 27e6 9caa e689      print('.....
-00001290: bee5 88b0 e6a0 87e9 a298 efbc 8ce5 b7b2  ................
-000012a0: e8b7 b3e8 bf87 2729 0a20 2020 2020 2020  ......').       
-000012b0: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
-000012c0: 2020 2020 2020 7469 746c 6520 3d20 6d2e        title = m.
-000012d0: 6772 6f75 7028 3129 0a20 2020 2020 2020  group(1).       
-000012e0: 2074 6f63 2e73 6574 6465 6661 756c 7428   toc.setdefault(
-000012f0: 6361 7465 2c20 5b5d 290a 2020 2020 2020  cate, []).      
-00001300: 2020 746f 635b 6361 7465 5d2e 6170 7065    toc[cate].appe
-00001310: 6e64 287b 0a20 2020 2020 2020 2020 2020  nd({.           
-00001320: 2027 7469 746c 6527 3a20 7469 746c 652c   'title': title,
-00001330: 0a20 2020 2020 2020 2020 2020 2027 6669  .            'fi
-00001340: 6c65 273a 2066 6e61 6d65 2c0a 2020 2020  le': fname,.    
-00001350: 2020 2020 2020 2020 2764 6174 6527 3a20          'date': 
-00001360: 6474 2c0a 2020 2020 2020 2020 7d29 0a20  dt,.        }). 
-00001370: 2020 200a 2020 2020 2320 e794 9fe6 8890     .    # ......
-00001380: e79b aee5 bd95 e696 87e4 bbb6 0a20 2020  .............   
-00001390: 2073 756d 6d61 7279 203d 2027 270a 2020   summary = ''.  
-000013a0: 2020 666f 7220 6361 7465 2c20 7375 6220    for cate, sub 
-000013b0: 696e 2074 6f63 2e69 7465 6d73 2829 3a0a  in toc.items():.
-000013c0: 2020 2020 2020 2020 7375 6d6d 6172 7920          summary 
-000013d0: 2b3d 2066 272b 2020 207b 6361 7465 7d5c  += f'+   {cate}\
-000013e0: 6e27 0a20 2020 2020 2020 2066 6f72 2061  n'.        for a
-000013f0: 7274 2069 6e20 7375 623a 0a20 2020 2020  rt in sub:.     
-00001400: 2020 2020 2020 2074 6974 6c65 203d 2061         title = a
-00001410: 7274 5b27 7469 746c 6527 5d0a 2020 2020  rt['title'].    
-00001420: 2020 2020 2020 2020 6669 6c65 203d 2071          file = q
-00001430: 756f 7465 5f70 6c75 7328 6172 745b 2766  uote_plus(art['f
-00001440: 696c 6527 5d29 0a20 2020 2020 2020 2020  ile']).         
-00001450: 2020 2073 756d 6d61 7279 202b 3d20 6627     summary += f'
-00001460: 2020 2020 2b20 2020 5b7b 7469 746c 657d      +   [{title}
-00001470: 5d28 646f 6373 2f7b 6669 6c65 7d29 5c6e  ](docs/{file})\n
-00001480: 270a 2020 2020 6f70 656e 2827 5355 4d4d  '.    open('SUMM
-00001490: 4152 592e 6d64 272c 2027 7727 2c20 656e  ARY.md', 'w', en
-000014a0: 636f 6469 6e67 3d27 7574 6638 2729 2e77  coding='utf8').w
-000014b0: 7269 7465 2873 756d 6d61 7279 290a 2020  rite(summary).  
-000014c0: 2020 0a64 6566 2074 6f6d 645f 6469 7228    .def tomd_dir(
-000014d0: 6172 6773 293a 0a20 2020 2064 6972 203d  args):.    dir =
-000014e0: 2061 7267 732e 666e 616d 650a 2020 2020   args.fname.    
-000014f0: 666e 616d 6573 203d 206f 732e 6c69 7374  fnames = os.list
-00001500: 6469 7228 6469 7229 0a20 2020 2070 6f6f  dir(dir).    poo
-00001510: 6c20 3d20 506f 6f6c 2861 7267 732e 7468  l = Pool(args.th
-00001520: 7265 6164 7329 0a20 2020 2066 6f72 2066  reads).    for f
-00001530: 6e61 6d65 2069 6e20 666e 616d 6573 3a0a  name in fnames:.
-00001540: 2020 2020 2020 2020 6172 6773 203d 2063          args = c
-00001550: 6f70 792e 6465 6570 636f 7079 2861 7267  opy.deepcopy(arg
-00001560: 7329 0a20 2020 2020 2020 2061 7267 732e  s).        args.
-00001570: 666e 616d 6520 3d20 7061 7468 2e6a 6f69  fname = path.joi
-00001580: 6e28 6469 722c 2066 6e61 6d65 290a 2020  n(dir, fname).  
-00001590: 2020 2020 2020 2320 746f 6d64 5f66 696c        # tomd_fil
-000015a0: 6528 6172 6773 290a 2020 2020 2020 2020  e(args).        
-000015b0: 706f 6f6c 2e61 7070 6c79 5f61 7379 6e63  pool.apply_async
-000015c0: 2874 6f6d 645f 6669 6c65 5f73 6166 652c  (tomd_file_safe,
-000015d0: 205b 6172 6773 5d29 0a20 2020 2070 6f6f   [args]).    poo
-000015e0: 6c2e 636c 6f73 6528 290a 2020 2020 706f  l.close().    po
-000015f0: 6f6c 2e6a 6f69 6e28 290a 0a64 6566 2074  ol.join()..def t
-00001600: 6f6d 645f 6669 6c65 5f73 6166 6528 6172  omd_file_safe(ar
-00001610: 6773 293a 0a20 2020 2074 7279 3a20 746f  gs):.    try: to
-00001620: 6d64 5f66 696c 6528 6172 6773 290a 2020  md_file(args).  
-00001630: 2020 6578 6365 7074 3a20 7472 6163 6562    except: traceb
-00001640: 6163 6b2e 7072 696e 745f 6578 6328 290a  ack.print_exc().
-00001650: 0a64 6566 2074 6f6d 645f 6669 6c65 2861  .def tomd_file(a
-00001660: 7267 7329 3a0a 2020 2020 6966 206e 6f74  rgs):.    if not
-00001670: 2061 7267 732e 666e 616d 652e 656e 6473   args.fname.ends
-00001680: 7769 7468 2827 2e68 746d 6c27 293a 0a20  with('.html'):. 
-00001690: 2020 2020 2020 2070 7269 6e74 2827 e8af         print('..
-000016a0: b7e6 8f90 e4be 9b20 4854 4d4c 20e6 9687  ....... HTML ...
-000016b0: e4bb b627 290a 2020 2020 2020 2020 7265  ...').        re
-000016c0: 7475 726e 0a20 2020 2070 7269 6e74 2861  turn.    print(a
-000016d0: 7267 732e 666e 616d 6529 0a20 2020 2068  rgs.fname).    h
-000016e0: 746d 6c20 3d20 6f70 656e 2861 7267 732e  tml = open(args.
-000016f0: 666e 616d 652c 2065 6e63 6f64 696e 673d  fname, encoding=
-00001700: 2775 7466 3827 292e 7265 6164 2829 0a20  'utf8').read(). 
-00001710: 2020 206d 6420 3d20 746f 6d64 2868 746d     md = tomd(htm
-00001720: 6c29 0a20 2020 206f 666e 616d 6520 3d20  l).    ofname = 
-00001730: 7265 2e73 7562 2872 275c 2e68 746d 6c24  re.sub(r'\.html$
-00001740: 272c 2027 272c 2061 7267 732e 666e 616d  ', '', args.fnam
-00001750: 6529 202b 2027 2e6d 6427 0a20 2020 206f  e) + '.md'.    o
-00001760: 7065 6e28 6f66 6e61 6d65 2c20 2777 272c  pen(ofname, 'w',
-00001770: 2065 6e63 6f64 696e 673d 2775 7466 3827   encoding='utf8'
-00001780: 292e 7772 6974 6528 6d64 290a 0a64 6566  ).write(md)..def
-00001790: 2074 6f6d 645f 6861 6e64 6c65 2861 7267   tomd_handle(arg
-000017a0: 7329 3a0a 2020 2020 6966 2070 6174 682e  s):.    if path.
-000017b0: 6973 6469 7228 6172 6773 2e66 6e61 6d65  isdir(args.fname
-000017c0: 293a 0a20 2020 2020 2020 2074 6f6d 645f  ):.        tomd_
-000017d0: 6469 7228 6172 6773 290a 2020 2020 656c  dir(args).    el
-000017e0: 7365 3a0a 2020 2020 2020 2020 746f 6d64  se:.        tomd
-000017f0: 5f66 696c 6528 6172 6773 290a 0a64 6566  _file(args)..def
-00001800: 2066 6d74 5f64 6972 2861 7267 7329 3a0a   fmt_dir(args):.
-00001810: 2020 2020 6469 7220 3d20 6172 6773 2e66      dir = args.f
-00001820: 6e61 6d65 0a20 2020 2066 6e61 6d65 7320  name.    fnames 
-00001830: 3d20 6f73 2e6c 6973 7464 6972 2864 6972  = os.listdir(dir
-00001840: 290a 2020 2020 706f 6f6c 203d 2050 6f6f  ).    pool = Poo
-00001850: 6c28 6172 6773 2e74 6872 6561 6473 290a  l(args.threads).
-00001860: 2020 2020 666f 7220 666e 616d 6520 696e      for fname in
-00001870: 2066 6e61 6d65 733a 0a20 2020 2020 2020   fnames:.       
-00001880: 2061 7267 7320 3d20 636f 7079 2e64 6565   args = copy.dee
-00001890: 7063 6f70 7928 6172 6773 290a 2020 2020  pcopy(args).    
-000018a0: 2020 2020 6172 6773 2e66 6e61 6d65 203d      args.fname =
-000018b0: 2070 6174 682e 6a6f 696e 2864 6972 2c20   path.join(dir, 
-000018c0: 666e 616d 6529 0a20 2020 2020 2020 2070  fname).        p
-000018d0: 6f6f 6c2e 6170 706c 795f 6173 796e 6328  ool.apply_async(
-000018e0: 666d 745f 6669 6c65 5f73 6166 652c 205b  fmt_file_safe, [
-000018f0: 6172 6773 5d29 0a20 2020 2070 6f6f 6c2e  args]).    pool.
-00001900: 636c 6f73 6528 290a 2020 2020 706f 6f6c  close().    pool
-00001910: 2e6a 6f69 6e28 290a 2020 2020 0a64 6566  .join().    .def
-00001920: 2066 6d74 5f66 696c 655f 7361 6665 2861   fmt_file_safe(a
-00001930: 7267 7329 3a0a 2020 2020 7472 793a 2066  rgs):.    try: f
-00001940: 6d74 5f66 696c 6528 6172 6773 290a 2020  mt_file(args).  
-00001950: 2020 6578 6365 7074 3a20 7472 6163 6562    except: traceb
-00001960: 6163 6b2e 7072 696e 745f 6578 6328 290a  ack.print_exc().
-00001970: 2020 2020 0a64 6566 2066 6d74 5f66 696c      .def fmt_fil
-00001980: 6528 6172 6773 293a 0a20 2020 206d 6f64  e(args):.    mod
-00001990: 6520 3d20 6172 6773 2e6d 6f64 650a 2020  e = args.mode.  
-000019a0: 2020 6966 206e 6f74 2061 7267 732e 666e    if not args.fn
-000019b0: 616d 652e 656e 6473 7769 7468 2827 2e68  ame.endswith('.h
-000019c0: 746d 6c27 2920 616e 6420 5c0a 2020 2020  tml') and \.    
-000019d0: 2020 2020 6e6f 7420 6172 6773 2e66 6e61      not args.fna
-000019e0: 6d65 2e65 6e64 7377 6974 6828 272e 6d64  me.endswith('.md
-000019f0: 2729 3a0a 2020 2020 2020 2020 7072 696e  '):.        prin
-00001a00: 7428 27e8 afb7 e68f 90e4 be9b 2048 544d  t('......... HTM
-00001a10: 4c20 e688 9620 4d44 20e6 9687 e4bb b627  L ... MD ......'
-00001a20: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00001a30: 0a20 2020 2070 7269 6e74 2861 7267 732e  .    print(args.
-00001a40: 666e 616d 6529 0a20 2020 2074 6578 7420  fname).    text 
-00001a50: 3d20 6f70 656e 2861 7267 732e 666e 616d  = open(args.fnam
-00001a60: 652c 2065 6e63 6f64 696e 673d 2775 7466  e, encoding='utf
-00001a70: 3827 292e 7265 6164 2829 0a20 2020 2069  8').read().    i
-00001a80: 6620 6d6f 6465 203d 3d20 277a 6827 3a0a  f mode == 'zh':.
-00001a90: 2020 2020 2020 2020 7465 7874 203d 2066          text = f
-00001aa0: 6d74 5f7a 6828 7465 7874 290a 2020 2020  mt_zh(text).    
-00001ab0: 656c 6966 206d 6f64 6520 3d3d 2027 7061  elif mode == 'pa
-00001ac0: 636b 7427 3a0a 2020 2020 2020 2020 7465  ckt':.        te
-00001ad0: 7874 203d 2066 6d74 5f70 6163 6b74 2874  xt = fmt_packt(t
-00001ae0: 6578 7429 0a20 2020 206f 7065 6e28 6172  ext).    open(ar
-00001af0: 6773 2e66 6e61 6d65 2c20 2777 272c 2065  gs.fname, 'w', e
-00001b00: 6e63 6f64 696e 673d 2775 7466 3827 292e  ncoding='utf8').
-00001b10: 7772 6974 6528 7465 7874 290a 0a64 6566  write(text)..def
-00001b20: 2066 6d74 5f68 616e 646c 6528 6172 6773   fmt_handle(args
-00001b30: 293a 0a20 2020 2069 6620 7061 7468 2e69  ):.    if path.i
-00001b40: 7364 6972 2861 7267 732e 666e 616d 6529  sdir(args.fname)
-00001b50: 3a0a 2020 2020 2020 2020 666d 745f 6469  :.        fmt_di
-00001b60: 7228 6172 6773 290a 2020 2020 656c 7365  r(args).    else
-00001b70: 3a0a 2020 2020 2020 2020 666d 745f 6669  :.        fmt_fi
-00001b80: 6c65 2861 7267 7329 0a0a 6465 6620 6f70  le(args)..def op
-00001b90: 7469 5f6d 645f 6669 6c65 5f73 6166 6528  ti_md_file_safe(
-00001ba0: 6172 6773 293a 0a20 2020 2074 7279 3a20  args):.    try: 
-00001bb0: 6f70 7469 5f6d 645f 6669 6c65 2861 7267  opti_md_file(arg
-00001bc0: 7329 0a20 2020 2065 7863 6570 743a 2074  s).    except: t
-00001bd0: 7261 6365 6261 636b 2e70 7269 6e74 5f65  raceback.print_e
-00001be0: 7863 2829 0a0a 6465 6620 6f70 7469 5f6d  xc()..def opti_m
-00001bf0: 645f 6669 6c65 2861 7267 7329 3a0a 2020  d_file(args):.  
-00001c00: 2020 5245 5f53 5243 5f46 554c 4c20 3d20    RE_SRC_FULL = 
-00001c10: 7227 e58e 9fe6 9687 5b3a efbc 9a5d 5c5b  r'......[:...]\[
-00001c20: 2e2b 3f5c 5d5c 2828 2e2b 3f29 5c29 270a  .+?\]\((.+?)\)'.
-00001c30: 2020 2020 5245 5f53 5243 5f46 554c 4c5f      RE_SRC_FULL_
-00001c40: 5245 5020 3d20 7227 e58e 9fe6 9687 efbc  REP = r'........
-00001c50: 9a3c 5c31 3e27 0a20 2020 2052 455f 5052  .<\1>'.    RE_PR
-00001c60: 455f 4845 4144 203d 2072 275e 5c78 3230  E_HEAD = r'^\x20
-00001c70: 2a5c 2a2b 5c78 3230 2a60 6060 270a 2020  *\*+\x20*```'.  
-00001c80: 2020 5245 5f4c 4547 5f54 4f4b 454e 203d    RE_LEG_TOKEN =
-00001c90: 2072 2754 5c64 2be3 8091 270a 2020 2020   r'T\d+...'.    
-00001ca0: 5245 5f50 5245 5f48 4541 4432 203d 2072  RE_PRE_HEAD2 = r
-00001cb0: 2760 6060 5c2a 2b7c 5c2a 2b60 6060 270a  '```\*+|\*+```'.
-00001cc0: 2020 2020 666e 616d 6520 3d20 6172 6773      fname = args
-00001cd0: 2e66 6e61 6d65 0a20 2020 2069 6620 6e6f  .fname.    if no
-00001ce0: 7420 666e 616d 652e 656e 6473 7769 7468  t fname.endswith
-00001cf0: 2827 2e6d 6427 293a 0a20 2020 2020 2020  ('.md'):.       
-00001d00: 2070 7269 6e74 2827 e8af b7e6 8f90 e4be   print('........
-00001d10: 9b20 4d61 726b 646f 776e 20e6 9687 e4bb  . Markdown .....
-00001d20: b627 290a 2020 2020 2020 2020 7265 7475  .').        retu
-00001d30: 726e 0a20 2020 2070 7269 6e74 2866 6e61  rn.    print(fna
-00001d40: 6d65 290a 2020 2020 636f 6e74 203d 206f  me).    cont = o
-00001d50: 7065 6e28 666e 616d 652c 2065 6e63 6f64  pen(fname, encod
-00001d60: 696e 673d 2775 7466 3827 292e 7265 6164  ing='utf8').read
-00001d70: 2829 0a20 2020 2063 6f6e 7420 3d20 636f  ().    cont = co
-00001d80: 6e74 2e72 6570 6c61 6365 2827 2e2e 2f49  nt.replace('../I
-00001d90: 6d61 6765 732f 272c 2027 696d 672f 2729  mages/', 'img/')
-00001da0: 0a20 2020 2063 6f6e 7420 3d20 7265 2e73  .    cont = re.s
-00001db0: 7562 2852 455f 4c45 475f 544f 4b45 4e2c  ub(RE_LEG_TOKEN,
-00001dc0: 2027 272c 2063 6f6e 7429 0a20 2020 2063   '', cont).    c
-00001dd0: 6f6e 7420 3d20 7265 2e73 7562 2852 455f  ont = re.sub(RE_
-00001de0: 5352 435f 4655 4c4c 2c20 5245 5f53 5243  SRC_FULL, RE_SRC
-00001df0: 5f46 554c 4c5f 5245 502c 2063 6f6e 7429  _FULL_REP, cont)
-00001e00: 0a20 2020 2063 6f6e 7420 3d20 7265 2e73  .    cont = re.s
-00001e10: 7562 2872 2723 5c64 2b5c 2d5c 642b 5c2d  ub(r'#\d+\-\d+\-
-00001e20: 5c64 2b28 3f3d 3e29 272c 2027 272c 2063  \d+(?=>)', '', c
-00001e30: 6f6e 7429 0a20 2020 2063 6f6e 7420 3d20  ont).    cont = 
-00001e40: 7265 2e73 7562 2852 455f 5052 455f 4845  re.sub(RE_PRE_HE
-00001e50: 4144 2c20 2760 6060 272c 2063 6f6e 742c  AD, '```', cont,
-00001e60: 2066 6c61 6773 3d72 652e 4d29 0a20 2020   flags=re.M).   
-00001e70: 2063 6f6e 7420 3d20 7265 2e73 7562 2852   cont = re.sub(R
-00001e80: 455f 5052 455f 4845 4144 322c 2027 6060  E_PRE_HEAD2, '``
-00001e90: 6027 2c20 636f 6e74 290a 2020 2020 6f70  `', cont).    op
-00001ea0: 656e 2866 6e61 6d65 2c20 2777 272c 2065  en(fname, 'w', e
-00001eb0: 6e63 6f64 696e 673d 2775 7466 3827 292e  ncoding='utf8').
-00001ec0: 7772 6974 6528 636f 6e74 290a 2020 200a  write(cont).   .
-00001ed0: 0a0a 6465 6620 6f70 7469 5f6d 645f 6861  ..def opti_md_ha
-00001ee0: 6e64 6c65 2861 7267 7329 3a0a 2020 2020  ndle(args):.    
-00001ef0: 6966 2070 6174 682e 6973 6469 7228 6172  if path.isdir(ar
-00001f00: 6773 2e66 6e61 6d65 293a 0a20 2020 2020  gs.fname):.     
-00001f10: 2020 206f 7074 695f 6d64 5f64 6972 2861     opti_md_dir(a
-00001f20: 7267 7329 0a20 2020 2065 6c73 653a 0a20  rgs).    else:. 
-00001f30: 2020 2020 2020 206f 7074 695f 6d64 5f66         opti_md_f
-00001f40: 696c 6528 6172 6773 290a 0a64 6566 206f  ile(args)..def o
-00001f50: 7074 695f 6d64 5f64 6972 2861 7267 7329  pti_md_dir(args)
-00001f60: 3a0a 2020 2020 6469 7220 3d20 6172 6773  :.    dir = args
-00001f70: 2e66 6e61 6d65 0a20 2020 2066 6e61 6d65  .fname.    fname
-00001f80: 7320 3d20 6f73 2e6c 6973 7464 6972 2864  s = os.listdir(d
-00001f90: 6972 290a 2020 2020 706f 6f6c 203d 2050  ir).    pool = P
-00001fa0: 6f6f 6c28 6172 6773 2e74 6872 6561 6473  ool(args.threads
-00001fb0: 290a 2020 2020 666f 7220 666e 616d 6520  ).    for fname 
-00001fc0: 696e 2066 6e61 6d65 733a 0a20 2020 2020  in fnames:.     
-00001fd0: 2020 2061 7267 7320 3d20 636f 7079 2e64     args = copy.d
-00001fe0: 6565 7063 6f70 7928 6172 6773 290a 2020  eepcopy(args).  
-00001ff0: 2020 2020 2020 6172 6773 2e66 6e61 6d65        args.fname
-00002000: 203d 2070 6174 682e 6a6f 696e 2864 6972   = path.join(dir
-00002010: 2c20 666e 616d 6529 0a20 2020 2020 2020  , fname).       
-00002020: 2023 2074 6f6d 645f 6669 6c65 2861 7267   # tomd_file(arg
-00002030: 7329 0a20 2020 2020 2020 2070 6f6f 6c2e  s).        pool.
-00002040: 6170 706c 795f 6173 796e 6328 6f70 7469  apply_async(opti
-00002050: 5f6d 645f 6669 6c65 5f73 6166 652c 205b  _md_file_safe, [
-00002060: 6172 6773 5d29 0a20 2020 2070 6f6f 6c2e  args]).    pool.
-00002070: 636c 6f73 6528 290a 2020 2020 706f 6f6c  close().    pool
-00002080: 2e6a 6f69 6e28 290a 0a0a 6465 6620 636f  .join()...def co
-00002090: 6e66 6967 5f70 726f 6a28 6172 6773 293a  nfig_proj(args):
-000020a0: 0a20 2020 2064 6972 203d 2070 6174 682e  .    dir = path.
-000020b0: 6162 7370 6174 6828 6172 6773 2e64 6972  abspath(args.dir
-000020c0: 290a 2020 2020 6966 206e 6f74 2070 6174  ).    if not pat
-000020d0: 682e 6973 6469 7228 6469 7229 3a0a 2020  h.isdir(dir):.  
-000020e0: 2020 2020 2020 7072 696e 7428 27e8 afb7        print('...
-000020f0: e68f 90e4 be9b e79b aee5 bd95 2729 0a20  ............'). 
-00002100: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-00002110: 2020 666e 616d 6573 203d 206f 732e 6c69    fnames = os.li
-00002120: 7374 6469 7228 6469 7229 0a20 2020 2069  stdir(dir).    i
-00002130: 6620 2752 4541 444d 452e 6d64 2720 6e6f  f 'README.md' no
-00002140: 7420 696e 2066 6e61 6d65 7320 6f72 205c  t in fnames or \
-00002150: 0a20 2020 2020 2020 2027 696e 6465 782e  .        'index.
-00002160: 6874 6d6c 2720 6e6f 7420 696e 2066 6e61  html' not in fna
-00002170: 6d65 7320 6f72 205c 0a20 2020 2020 2020  mes or \.       
-00002180: 2027 434e 414d 4527 206e 6f74 2069 6e20   'CNAME' not in 
-00002190: 666e 616d 6573 3a0a 2020 2020 2020 2020  fnames:.        
-000021a0: 7072 696e 7428 27e7 bcba e5b0 9120 5245  print('...... RE
-000021b0: 4144 4d45 2e6d 64ef bc8c 696e 6465 782e  ADME.md...index.
-000021c0: 6874 6d6c 20e6 8896 2043 4e41 4d45 20e6  html ... CNAME .
-000021d0: 9687 e4bb b627 290a 2020 2020 2020 2020  .....').        
-000021e0: 7265 7475 726e 0a20 2020 206e 616d 6520  return.    name 
-000021f0: 3d20 696e 7075 7428 27e8 afb7 e8be 93e5  = input('.......
-00002200: 85a5 e4b8 ade6 9687 e590 8de7 a7b0 efbc  ................
-00002210: 9a27 292e 7374 7269 7028 2920 6f72 2027  .').strip() or '
-00002220: 7b6e 616d 657d 270a 2020 2020 6e61 6d65  {name}'.    name
-00002230: 5f65 6e20 3d20 696e 7075 7428 27e8 afb7  _en = input('...
-00002240: e8be 93e5 85a5 e88b b1e6 9687 e590 8de7  ................
-00002250: a7b0 efbc 9a27 292e 7374 7269 7028 2920  .....').strip() 
-00002260: 6f72 2027 7b6e 616d 6545 6e7d 270a 2020  or '{nameEn}'.  
-00002270: 2020 7572 6c5f 656e 203d 2069 6e70 7574    url_en = input
-00002280: 2827 e8af b7e8 be93 e585 a5e8 8bb1 e696  ('..............
-00002290: 87e9 93be e68e a5ef bc9a 2729 2e73 7472  ..........').str
-000022a0: 6970 2829 206f 7220 277b 7572 6c45 6e7d  ip() or '{urlEn}
-000022b0: 270a 2020 2020 646f 6d61 696e 203d 2069  '.    domain = i
-000022c0: 6e70 7574 2827 e8af b7e8 be93 e585 a5e5  nput('..........
-000022d0: 9f9f e590 8de5 898d e7bc 80ef bc9a 2729  ..............')
-000022e0: 2e73 7472 6970 2829 206f 7220 277b 646f  .strip() or '{do
-000022f0: 6d61 696e 7d27 0a20 2020 2063 6f6c 6f72  main}'.    color
-00002300: 203d 2069 6e70 7574 2827 e8af b7e8 be93   = input('......
-00002310: e585 a5e9 a29c e889 b2ef bc9a 2729 2e73  ............').s
-00002320: 7472 6970 2829 206f 7220 277b 636f 6c6f  trip() or '{colo
-00002330: 727d 270a 2020 2020 7265 706f 203d 2070  r}'.    repo = p
-00002340: 6174 682e 6261 7365 6e61 6d65 2864 6972  ath.basename(dir
-00002350: 290a 2020 2020 0a20 2020 2063 6f6e 7473  ).    .    conts
-00002360: 203d 207b 0a20 2020 2020 2020 2027 5245   = {.        'RE
-00002370: 4144 4d45 2e6d 6427 3a20 6f70 656e 2870  ADME.md': open(p
-00002380: 6174 682e 6a6f 696e 2864 6972 2c20 2752  ath.join(dir, 'R
-00002390: 4541 444d 452e 6d64 2729 2c20 656e 636f  EADME.md'), enco
-000023a0: 6469 6e67 3d27 7574 6638 2729 2e72 6561  ding='utf8').rea
-000023b0: 6428 292c 0a20 2020 2020 2020 2027 696e  d(),.        'in
-000023c0: 6465 782e 6874 6d6c 273a 206f 7065 6e28  dex.html': open(
-000023d0: 7061 7468 2e6a 6f69 6e28 6469 722c 2027  path.join(dir, '
-000023e0: 696e 6465 782e 6874 6d6c 2729 2c20 656e  index.html'), en
-000023f0: 636f 6469 6e67 3d27 7574 6638 2729 2e72  coding='utf8').r
-00002400: 6561 6428 292c 0a20 2020 2020 2020 2027  ead(),.        '
-00002410: 434e 414d 4527 3a20 6f70 656e 2870 6174  CNAME': open(pat
-00002420: 682e 6a6f 696e 2864 6972 2c20 2743 4e41  h.join(dir, 'CNA
-00002430: 4d45 2729 2c20 656e 636f 6469 6e67 3d27  ME'), encoding='
-00002440: 7574 6638 2729 2e72 6561 6428 292c 0a20  utf8').read(),. 
-00002450: 2020 207d 0a20 2020 2066 6f72 2066 6e61     }.    for fna
-00002460: 6d65 2c20 636f 6e74 2069 6e20 636f 6e74  me, cont in cont
-00002470: 732e 6974 656d 7328 293a 0a20 2020 2020  s.items():.     
-00002480: 2020 2063 6f6e 7420 3d20 280a 2020 2020     cont = (.    
-00002490: 2020 2020 2020 2020 636f 6e74 2e72 6570          cont.rep
-000024a0: 6c61 6365 2827 7b6e 616d 657d 272c 206e  lace('{name}', n
-000024b0: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
-000024c0: 2020 2020 202e 7265 706c 6163 6528 277b       .replace('{
-000024d0: 6e61 6d65 456e 7d27 2c20 6e61 6d65 5f65  nameEn}', name_e
-000024e0: 6e29 0a20 2020 2020 2020 2020 2020 2020  n).             
-000024f0: 2020 202e 7265 706c 6163 6528 277b 7572     .replace('{ur
-00002500: 6c45 6e7d 272c 2075 726c 5f65 6e29 0a20  lEn}', url_en). 
-00002510: 2020 2020 2020 2020 2020 2020 2020 202e                 .
-00002520: 7265 706c 6163 6528 277b 7572 6c45 6e7d  replace('{urlEn}
-00002530: 272c 2075 726c 5f65 6e29 0a20 2020 2020  ', url_en).     
-00002540: 2020 2020 2020 2020 2020 202e 7265 706c             .repl
-00002550: 6163 6528 277b 646f 6d61 696e 7d27 2c20  ace('{domain}', 
-00002560: 646f 6d61 696e 290a 2020 2020 2020 2020  domain).        
-00002570: 2020 2020 2020 2020 2e72 6570 6c61 6365          .replace
-00002580: 2827 7b63 6f6c 6f72 7d27 2c20 636f 6c6f  ('{color}', colo
-00002590: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
-000025a0: 2020 202e 7265 706c 6163 6528 277b 6164     .replace('{ad
-000025b0: 6d69 6e4e 616d 657d 272c 2027 e9a3 9ee9  minName}', '....
-000025c0: be99 2729 0a20 2020 2020 2020 2020 2020  ..').           
-000025d0: 2020 2020 202e 7265 706c 6163 6528 277b       .replace('{
-000025e0: 6164 6d69 6e55 6e7d 272c 2027 7769 7a61  adminUn}', 'wiza
-000025f0: 7264 666f 7263 656c 2729 0a20 2020 2020  rdforcel').     
-00002600: 2020 2020 2020 2020 2020 202e 7265 706c             .repl
-00002610: 6163 6528 277b 6164 6d69 6e51 717d 272c  ace('{adminQq}',
-00002620: 2027 3536 3238 3236 3137 3927 290a 2020   '562826179').  
-00002630: 2020 2020 2020 2020 2020 2020 2020 2e72                .r
-00002640: 6570 6c61 6365 2827 7b72 6570 6f7d 272c  eplace('{repo}',
-00002650: 2072 6570 6f29 0a20 2020 2020 2020 2020   repo).         
-00002660: 2020 2020 2020 202e 7265 706c 6163 6528         .replace(
-00002670: 277b 646f 636b 6572 4e61 6d65 7d27 2c20  '{dockerName}', 
-00002680: 7265 706f 290a 2020 2020 2020 2020 2020  repo).          
-00002690: 2020 2020 2020 2e72 6570 6c61 6365 2827        .replace('
-000026a0: 7b70 7970 694e 616d 657d 272c 2072 6570  {pypiName}', rep
-000026b0: 6f29 0a20 2020 2020 2020 2020 2020 2020  o).             
-000026c0: 2020 202e 7265 706c 6163 6528 277b 6e70     .replace('{np
-000026d0: 6d4e 616d 657d 272c 2072 6570 6f29 0a20  mName}', repo). 
-000026e0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000026f0: 206f 7065 6e28 7061 7468 2e6a 6f69 6e28   open(path.join(
-00002700: 6469 722c 2066 6e61 6d65 292c 2027 7727  dir, fname), 'w'
-00002710: 2c20 656e 636f 6469 6e67 3d27 7574 6638  , encoding='utf8
-00002720: 2729 2e77 7269 7465 2863 6f6e 7429 0a0a  ').write(cont)..
-00002730: 6465 6620 636f 6e76 6572 745f 6364 7269  def convert_cdri
-00002740: 7665 5f6c 6f67 2861 7267 7329 3a0a 2020  ve_log(args):.  
-00002750: 2020 5245 5f49 4e46 4f20 3d20 7227 5c5b    RE_INFO = r'\[
-00002760: 282e 2b3f 295c 5d28 5b5e 5c5b 5d2b 2927  (.+?)\]([^\[]+)'
-00002770: 0a20 2020 2052 455f 5449 544c 4520 3d20  .    RE_TITLE = 
-00002780: 7227 e4b8 8ae4 bca0 3a20 282e 2b3f 2920  r'......: (.+?) 
-00002790: 5c28 5b5c 645c 2e5d 2b20 5c77 2b5c 295c  \([\d\.]+ \w+\)\
-000027a0: 6e27 0a20 2020 2052 455f 4d45 5441 203d  n'.    RE_META =
-000027b0: 2072 274d 4554 4120 5552 4c20 2d3e 2028   r'META URL -> (
-000027c0: 5c53 2b29 270a 2020 2020 0a20 2020 2066  \S+)'.    .    f
-000027d0: 6e61 6d65 203d 2061 7267 732e 666e 616d  name = args.fnam
-000027e0: 650a 2020 2020 636f 203d 206f 7065 6e28  e.    co = open(
-000027f0: 666e 616d 652c 2065 6e63 6f64 696e 673d  fname, encoding=
-00002800: 2775 7466 3827 292e 7265 6164 2829 0a20  'utf8').read(). 
-00002810: 2020 2063 6f73 203d 2063 6f2e 7370 6c69     cos = co.spli
-00002820: 7428 2720 e4b8 8ae4 bca0 3a20 2729 0a20  t(' ......: '). 
-00002830: 2020 2072 6573 203d 205b 277c 20e6 9687     res = ['| ...
-00002840: e4bb b620 7c20 e993 bee6 8ea5 207c 5c6e  ... | ...... |\n
-00002850: 7c20 2d2d 2d20 7c20 2d2d 2d20 7c5c 6e27  | --- | --- |\n'
-00002860: 5d0a 2020 2020 666f 7220 696e 666f 2069  ].    for info i
-00002870: 6e20 636f 733a 0a20 2020 2020 2020 2069  n cos:.        i
-00002880: 6e66 6f20 3d20 2720 e4b8 8ae4 bca0 3a20  nfo = ' ......: 
-00002890: 2720 2b20 696e 666f 0a20 2020 2020 2020  ' + info.       
-000028a0: 2074 6974 6c65 203d 2072 652e 7365 6172   title = re.sear
-000028b0: 6368 2852 455f 5449 544c 452c 2069 6e66  ch(RE_TITLE, inf
-000028c0: 6f29 0a20 2020 2020 2020 206d 6574 6120  o).        meta 
-000028d0: 3d20 7265 2e73 6561 7263 6828 5245 5f4d  = re.search(RE_M
-000028e0: 4554 412c 2069 6e66 6f29 0a20 2020 2020  ETA, info).     
-000028f0: 2020 2069 6620 6e6f 7420 7469 746c 653a     if not title:
-00002900: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
-00002910: 2020 7469 746c 6520 3d20 7469 746c 652e    title = title.
-00002920: 6772 6f75 7028 3129 0a20 2020 2020 2020  group(1).       
-00002930: 206d 6574 6120 3d20 6d65 7461 2e67 726f   meta = meta.gro
-00002940: 7570 2831 2920 6966 206d 6574 6120 656c  up(1) if meta el
-00002950: 7365 2027 e69c aae4 b88a e4bc a027 0a20  se '.........'. 
-00002960: 2020 2020 2020 2072 6573 2e61 7070 656e         res.appen
-00002970: 6428 6627 7c20 7b74 6974 6c65 7d20 7c20  d(f'| {title} | 
-00002980: 7b6d 6574 617d 207c 5c6e 2729 0a20 2020  {meta} |\n').   
-00002990: 2020 2020 200a 2020 2020 7265 7320 3d20       .    res = 
-000029a0: 2727 2e6a 6f69 6e28 7265 7329 0a20 2020  ''.join(res).   
-000029b0: 206f 7065 6e28 666e 616d 6520 2b20 272e   open(fname + '.
-000029c0: 6d64 272c 2027 7727 2c20 656e 636f 6469  md', 'w', encodi
-000029d0: 6e67 3d27 7574 6638 2729 2e77 7269 7465  ng='utf8').write
-000029e0: 2872 6573 290a                           (res).
+00000940: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00000950: 0d0a 2020 2020 0d0a 2020 2020 2320 e8a7  ..    ..    # ..
+00000960: a3e6 9e90 e586 85e5 aeb9 e5b9 b6e4 b88b  ................
+00000970: e8bd bde5 9bbe e789 870d 0a20 2020 2069  ...........    i
+00000980: 6620 6172 6773 2e62 6f64 793a 0d0a 2020  f args.body:..  
+00000990: 2020 2020 2020 636f 203d 2072 742e 6669        co = rt.fi
+000009a0: 6e64 2861 7267 732e 626f 6479 292e 6874  nd(args.body).ht
+000009b0: 6d6c 2829 0d0a 2020 2020 656c 7365 3a0d  ml()..    else:.
+000009c0: 0a20 2020 2020 2020 2063 6f20 3d20 446f  .        co = Do
+000009d0: 6375 6d65 6e74 2873 7472 2872 7429 292e  cument(str(rt)).
+000009e0: 7375 6d6d 6172 7928 290d 0a20 2020 2020  summary()..     
+000009f0: 2020 2063 6f20 3d20 7071 2863 6f29 2e66     co = pq(co).f
+00000a00: 696e 6428 2762 6f64 7927 292e 6874 6d6c  ind('body').html
+00000a10: 2829 0d0a 2020 2020 6966 206e 6f74 2063  ()..    if not c
+00000a20: 6f3a 200d 0a20 2020 2020 2020 2070 7269  o: ..        pri
+00000a30: 6e74 2827 e69c aae8 8eb7 e58f 96e5 88b0  nt('............
+00000a40: e586 85e5 aeb9 efbc 8127 290d 0a20 2020  .........')..   
+00000a50: 2020 2020 2072 6574 7572 6e20 0d0a 2020       return ..  
+00000a60: 2020 696d 6773 203d 207b 7d0d 0a20 2020    imgs = {}..   
+00000a70: 2063 6f20 3d20 7072 6f63 6573 735f 696d   co = process_im
+00000a80: 6728 636f 2c20 696d 6773 2c20 696d 675f  g(co, imgs, img_
+00000a90: 7072 6566 6978 3d27 696d 672f 272c 2070  prefix='img/', p
+00000aa0: 6167 655f 7572 6c3d 6172 6773 2e75 726c  age_url=args.url
+00000ab0: 290d 0a20 2020 2068 746d 6c20 3d20 6627  )..    html = f'
+00000ac0: 2727 0d0a 2020 2020 3c68 746d 6c3e 3c62  ''..    <html><b
+00000ad0: 6f64 793e 0d0a 2020 2020 3c68 313e 7b74  ody>..    <h1>{t
+00000ae0: 6974 6c65 7d3c 2f68 313e 0d0a 2020 2020  itle}</h1>..    
+00000af0: 3c62 6c6f 636b 7175 6f74 653e 0d0a 2020  <blockquote>..  
+00000b00: 2020 e69d a5e6 ba90 efbc 9a3c 6120 6872    .........<a hr
+00000b10: 6566 3d27 7b61 7267 732e 7572 6c7d 273e  ef='{args.url}'>
+00000b20: 7b61 7267 732e 7572 6c7d 3c2f 613e 0d0a  {args.url}</a>..
+00000b30: 2020 2020 3c2f 626c 6f63 6b71 756f 7465      </blockquote
+00000b40: 3e0d 0a20 2020 207b 636f 7d3c 2f62 6f64  >..    {co}</bod
+00000b50: 793e 3c2f 6874 6d6c 3e0d 0a20 2020 2027  y></html>..    '
+00000b60: 2727 0d0a 2020 2020 0d0a 2020 2020 2320  ''..    ..    # 
+00000b70: e8bd ace6 8da2 206d 640d 0a20 2020 206d  ...... md..    m
+00000b80: 6420 3d20 746f 6d64 2868 746d 6c29 0d0a  d = tomd(html)..
+00000b90: 2020 2020 2320 6d64 203d 2072 652e 7375      # md = re.su
+00000ba0: 6228 5245 5f43 4f44 455f 424c 4f43 4b2c  b(RE_CODE_BLOCK,
+00000bb0: 2063 6f64 655f 7265 706c 6163 655f 6675   code_replace_fu
+00000bc0: 6e63 2c20 6d64 290d 0a20 2020 2079 616d  nc, md)..    yam
+00000bd0: 6c5f 6865 6164 203d 2027 5c6e 272e 6a6f  l_head = '\n'.jo
+00000be0: 696e 285b 0d0a 2020 2020 2020 2020 273c  in([..        '<
+00000bf0: 212d 2d79 6d6c 272c 0d0a 2020 2020 2020  !--yml',..      
+00000c00: 2020 2763 6174 6567 6f72 793a 2027 202b    'category: ' +
+00000c10: 2061 7267 732e 6361 7465 676f 7279 2c0d   args.category,.
+00000c20: 0a20 2020 2020 2020 2027 6461 7465 3a20  .        'date: 
+00000c30: 2720 2b20 6461 7465 7469 6d65 2e6e 6f77  ' + datetime.now
+00000c40: 2829 2e73 7472 6674 696d 6528 2725 592d  ().strftime('%Y-
+00000c50: 256d 2d25 6420 2548 3a25 4d3a 2553 2729  %m-%d %H:%M:%S')
+00000c60: 2c0d 0a20 2020 2020 2020 2027 2d2d 3e27  ,..        '-->'
+00000c70: 2c0d 0a20 2020 205d 290d 0a20 2020 206d  ,..    ])..    m
+00000c80: 6420 3d20 6627 7b79 616d 6c5f 6865 6164  d = f'{yaml_head
+00000c90: 7d5c 6e5c 6e7b 6d64 7d27 0d0a 2020 2020  }\n\n{md}'..    
+00000ca0: 0d0a 2020 2020 2320 e586 99e5 85a5 e7a1  ..    # ........
+00000cb0: ace7 9b98 0d0a 2020 2020 7361 6665 5f6d  ......    safe_m
+00000cc0: 6b64 6972 2827 646f 6373 2729 0d0a 2020  kdir('docs')..  
+00000cd0: 2020 7361 6665 5f6d 6b64 6972 2827 646f    safe_mkdir('do
+00000ce0: 6373 2f69 6d67 2729 0d0a 2020 2020 6f70  cs/img')..    op
+00000cf0: 656e 2866 6e61 6d65 2c20 2777 272c 2065  en(fname, 'w', e
+00000d00: 6e63 6f64 696e 673d 2775 7466 2d38 2729  ncoding='utf-8')
+00000d10: 2e77 7269 7465 286d 6429 0d0a 2020 2020  .write(md)..    
+00000d20: 666f 7220 6e61 6d65 2c20 6461 7461 2069  for name, data i
+00000d30: 6e20 696d 6773 2e69 7465 6d73 2829 3a0d  n imgs.items():.
+00000d40: 0a20 2020 2020 2020 206f 7065 6e28 6627  .        open(f'
+00000d50: 646f 6373 2f69 6d67 2f7b 6e61 6d65 7d27  docs/img/{name}'
+00000d60: 2c20 2777 6227 292e 7772 6974 6528 6461  , 'wb').write(da
+00000d70: 7461 290d 0a20 2020 2020 2020 200d 0a20  ta)..        .. 
+00000d80: 2020 2070 7269 6e74 2827 e5b7 b2e5 ae8c     print('......
+00000d90: e688 9027 290d 0a20 2020 200d 0a64 6566  ...')..    ..def
+00000da0: 2073 756d 6d61 7279 5f68 616e 646c 6528   summary_handle(
+00000db0: 6172 6773 293a 0d0a 2020 2020 2320 e8af  args):..    # ..
+00000dc0: bbe5 85a5 e696 87e4 bbb6 e588 97e8 a1a8  ................
+00000dd0: 0d0a 2020 2020 6469 7220 3d20 6172 6773  ..    dir = args
+00000de0: 2e64 6972 0d0a 2020 2020 666e 616d 6573  .dir..    fnames
+00000df0: 203d 205b 6620 666f 7220 6620 696e 206f   = [f for f in o
+00000e00: 732e 6c69 7374 6469 7228 6469 7229 2069  s.listdir(dir) i
+00000e10: 6620 662e 656e 6473 7769 7468 2827 2e6d  f f.endswith('.m
+00000e20: 6427 295d 0d0a 2020 2020 746f 6320 3d20  d')]..    toc = 
+00000e30: 5b5d 0d0a 2020 2020 666f 7220 6620 696e  []..    for f in
+00000e40: 2066 6e61 6d65 733a 0d0a 2020 2020 2020   fnames:..      
+00000e50: 2020 6675 6c6c 6620 3d20 7061 7468 2e6a    fullf = path.j
+00000e60: 6f69 6e28 6469 722c 2066 290d 0a20 2020  oin(dir, f)..   
+00000e70: 2020 2020 2070 7269 6e74 2866 756c 6c66       print(fullf
+00000e80: 290d 0a20 2020 2020 2020 2063 6f6e 7420  )..        cont 
+00000e90: 3d20 6f70 656e 2866 756c 6c66 2c20 656e  = open(fullf, en
+00000ea0: 636f 6469 6e67 3d27 7574 6638 2729 2e72  coding='utf8').r
+00000eb0: 6561 6428 290d 0a20 2020 2020 2020 206d  ead()..        m
+00000ec0: 203d 2072 652e 7365 6172 6368 2852 455f   = re.search(RE_
+00000ed0: 5449 544c 452c 2063 6f6e 742c 2066 6c61  TITLE, cont, fla
+00000ee0: 6773 3d72 652e 4d29 0d0a 2020 2020 2020  gs=re.M)..      
+00000ef0: 2020 6966 206e 6f74 206d 3a20 636f 6e74    if not m: cont
+00000f00: 696e 7565 0d0a 2020 2020 2020 2020 7469  inue..        ti
+00000f10: 746c 6520 3d20 6d2e 6772 6f75 7028 3129  tle = m.group(1)
+00000f20: 0d0a 2020 2020 2020 2020 746f 632e 6170  ..        toc.ap
+00000f30: 7065 6e64 2866 272b 2020 205b 7b74 6974  pend(f'+   [{tit
+00000f40: 6c65 7d5d 287b 667d 2927 290d 0a20 2020  le}]({f})')..   
+00000f50: 2073 756d 6d61 7279 203d 2027 5c6e 272e   summary = '\n'.
+00000f60: 6a6f 696e 2874 6f63 290d 0a20 2020 206f  join(toc)..    o
+00000f70: 7065 6e28 7061 7468 2e6a 6f69 6e28 6469  pen(path.join(di
+00000f80: 722c 2027 5355 4d4d 4152 592e 6d64 2729  r, 'SUMMARY.md')
+00000f90: 2c20 2777 272c 2065 6e63 6f64 696e 673d  , 'w', encoding=
+00000fa0: 2775 7466 3827 292e 7772 6974 6528 7375  'utf8').write(su
+00000fb0: 6d6d 6172 7929 0d0a 2020 2020 0d0a 6465  mmary)..    ..de
+00000fc0: 6620 7769 6b69 5f73 756d 6d61 7279 5f68  f wiki_summary_h
+00000fd0: 616e 646c 6528 6172 6773 293a 0d0a 2020  andle(args):..  
+00000fe0: 2020 2320 e8af bbe5 85a5 e696 87e4 bbb6    # ............
+00000ff0: e588 97e8 a1a8 0d0a 2020 2020 666e 616d  ........    fnam
+00001000: 6573 203d 205b 6620 666f 7220 6620 696e  es = [f for f in
+00001010: 206f 732e 6c69 7374 6469 7228 2764 6f63   os.listdir('doc
+00001020: 7327 2920 6966 2066 2e65 6e64 7377 6974  s') if f.endswit
+00001030: 6828 272e 6d64 2729 5d0d 0a20 2020 2074  h('.md')]..    t
+00001040: 6f63 203d 204f 7264 6572 6564 4469 6374  oc = OrderedDict
+00001050: 2829 0d0a 2020 2020 666f 7220 666e 616d  ()..    for fnam
+00001060: 6520 696e 2066 6e61 6d65 733a 0d0a 2020  e in fnames:..  
+00001070: 2020 2020 2020 7072 696e 7428 666e 616d        print(fnam
+00001080: 6529 0d0a 2020 2020 2020 2020 6d64 203d  e)..        md =
+00001090: 206f 7065 6e28 7061 7468 2e6a 6f69 6e28   open(path.join(
+000010a0: 2764 6f63 7327 2c20 666e 616d 6529 2c20  'docs', fname), 
+000010b0: 656e 636f 6469 6e67 3d27 7574 6638 2729  encoding='utf8')
+000010c0: 2e72 6561 6428 290d 0a20 2020 2020 2020  .read()..       
+000010d0: 2023 20e6 8f90 e58f 96e5 8583 e4bf a1e6   # .............
+000010e0: 81af 0d0a 2020 2020 2020 2020 6d20 3d20  ....        m = 
+000010f0: 7265 2e73 6561 7263 6828 5245 5f59 414d  re.search(RE_YAM
+00001100: 4c5f 4d45 5441 2c20 6d64 290d 0a20 2020  L_META, md)..   
+00001110: 2020 2020 2069 6620 6e6f 7420 6d3a 200d       if not m: .
+00001120: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00001130: 6e74 2827 e69c aae6 89be e588 b0e5 8583  nt('............
+00001140: e4bf a1e6 81af efbc 8ce5 b7b2 e8b7 b3e8  ................
+00001150: bf87 2729 0d0a 2020 2020 2020 2020 2020  ..')..          
+00001160: 2020 636f 6e74 696e 7565 0d0a 2020 2020    continue..    
+00001170: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00001180: 2020 2020 2020 6d65 7461 203d 2079 616d        meta = yam
+00001190: 6c2e 7361 6665 5f6c 6f61 6428 6d2e 6772  l.safe_load(m.gr
+000011a0: 6f75 7028 3129 290d 0a20 2020 2020 2020  oup(1))..       
+000011b0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+000011c0: 6e20 6173 2065 783a 200d 0a20 2020 2020  n as ex: ..     
+000011d0: 2020 2020 2020 2074 7261 6365 6261 636b         traceback
+000011e0: 2e70 7269 6e74 5f65 7863 2829 0d0a 2020  .print_exc()..  
+000011f0: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+00001200: 7565 0d0a 2020 2020 2020 2020 6474 203d  ue..        dt =
+00001210: 206d 6574 612e 6765 7428 2764 6174 6527   meta.get('date'
+00001220: 2c20 2730 3030 312d 3031 2d30 3120 3030  , '0001-01-01 00
+00001230: 3a30 303a 3030 2729 0d0a 2020 2020 2020  :00:00')..      
+00001240: 2020 6361 7465 203d 206d 6574 612e 6765    cate = meta.ge
+00001250: 7428 2763 6174 6567 6f72 7927 2c20 27e6  t('category', '.
+00001260: 9caa e588 86e7 b1bb 2729 0d0a 2020 2020  ........')..    
+00001270: 2020 2020 2320 e68f 90e5 8f96 e6a0 87e9      # ..........
+00001280: a298 0d0a 2020 2020 2020 2020 6d20 3d20  ....        m = 
+00001290: 7265 2e73 6561 7263 6828 5245 5f54 4954  re.search(RE_TIT
+000012a0: 4c45 2c20 6d64 2c20 666c 6167 733d 7265  LE, md, flags=re
+000012b0: 2e4d 290d 0a20 2020 2020 2020 2069 6620  .M)..        if 
+000012c0: 6e6f 7420 6d3a 200d 0a20 2020 2020 2020  not m: ..       
+000012d0: 2020 2020 2070 7269 6e74 2827 e69c aae6       print('....
+000012e0: 89be e588 b0e6 a087 e9a2 98ef bc8c e5b7  ................
+000012f0: b2e8 b7b3 e8bf 8727 290d 0a20 2020 2020  .......')..     
+00001300: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
+00001310: 0a20 2020 2020 2020 2074 6974 6c65 203d  .        title =
+00001320: 206d 2e67 726f 7570 2831 290d 0a20 2020   m.group(1)..   
+00001330: 2020 2020 2074 6f63 2e73 6574 6465 6661       toc.setdefa
+00001340: 756c 7428 6361 7465 2c20 5b5d 290d 0a20  ult(cate, []).. 
+00001350: 2020 2020 2020 2074 6f63 5b63 6174 655d         toc[cate]
+00001360: 2e61 7070 656e 6428 7b0d 0a20 2020 2020  .append({..     
+00001370: 2020 2020 2020 2027 7469 746c 6527 3a20         'title': 
+00001380: 7469 746c 652c 0d0a 2020 2020 2020 2020  title,..        
+00001390: 2020 2020 2766 696c 6527 3a20 666e 616d      'file': fnam
+000013a0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+000013b0: 2764 6174 6527 3a20 6474 2c0d 0a20 2020  'date': dt,..   
+000013c0: 2020 2020 207d 290d 0a20 2020 200d 0a20       })..    .. 
+000013d0: 2020 2023 20e7 949f e688 90e7 9bae e5bd     # ...........
+000013e0: 95e6 9687 e4bb b60d 0a20 2020 2073 756d  .........    sum
+000013f0: 6d61 7279 203d 2027 270d 0a20 2020 2066  mary = ''..    f
+00001400: 6f72 2063 6174 652c 2073 7562 2069 6e20  or cate, sub in 
+00001410: 746f 632e 6974 656d 7328 293a 0d0a 2020  toc.items():..  
+00001420: 2020 2020 2020 7375 6d6d 6172 7920 2b3d        summary +=
+00001430: 2066 272b 2020 207b 6361 7465 7d5c 6e27   f'+   {cate}\n'
+00001440: 0d0a 2020 2020 2020 2020 666f 7220 6172  ..        for ar
+00001450: 7420 696e 2073 7562 3a0d 0a20 2020 2020  t in sub:..     
+00001460: 2020 2020 2020 2074 6974 6c65 203d 2061         title = a
+00001470: 7274 5b27 7469 746c 6527 5d0d 0a20 2020  rt['title']..   
+00001480: 2020 2020 2020 2020 2066 696c 6520 3d20           file = 
+00001490: 7175 6f74 655f 706c 7573 2861 7274 5b27  quote_plus(art['
+000014a0: 6669 6c65 275d 290d 0a20 2020 2020 2020  file'])..       
+000014b0: 2020 2020 2073 756d 6d61 7279 202b 3d20       summary += 
+000014c0: 6627 2020 2020 2b20 2020 5b7b 7469 746c  f'    +   [{titl
+000014d0: 657d 5d28 646f 6373 2f7b 6669 6c65 7d29  e}](docs/{file})
+000014e0: 5c6e 270d 0a20 2020 206f 7065 6e28 2753  \n'..    open('S
+000014f0: 554d 4d41 5259 2e6d 6427 2c20 2777 272c  UMMARY.md', 'w',
+00001500: 2065 6e63 6f64 696e 673d 2775 7466 3827   encoding='utf8'
+00001510: 292e 7772 6974 6528 7375 6d6d 6172 7929  ).write(summary)
+00001520: 0d0a 2020 2020 0d0a 6465 6620 746f 6d64  ..    ..def tomd
+00001530: 5f64 6972 2861 7267 7329 3a0d 0a20 2020  _dir(args):..   
+00001540: 2064 6972 203d 2061 7267 732e 666e 616d   dir = args.fnam
+00001550: 650d 0a20 2020 2066 6e61 6d65 7320 3d20  e..    fnames = 
+00001560: 6f73 2e6c 6973 7464 6972 2864 6972 290d  os.listdir(dir).
+00001570: 0a20 2020 2070 6f6f 6c20 3d20 506f 6f6c  .    pool = Pool
+00001580: 2861 7267 732e 7468 7265 6164 7329 0d0a  (args.threads)..
+00001590: 2020 2020 666f 7220 666e 616d 6520 696e      for fname in
+000015a0: 2066 6e61 6d65 733a 0d0a 2020 2020 2020   fnames:..      
+000015b0: 2020 6172 6773 203d 2063 6f70 792e 6465    args = copy.de
+000015c0: 6570 636f 7079 2861 7267 7329 0d0a 2020  epcopy(args)..  
+000015d0: 2020 2020 2020 6172 6773 2e66 6e61 6d65        args.fname
+000015e0: 203d 2070 6174 682e 6a6f 696e 2864 6972   = path.join(dir
+000015f0: 2c20 666e 616d 6529 0d0a 2020 2020 2020  , fname)..      
+00001600: 2020 2320 746f 6d64 5f66 696c 6528 6172    # tomd_file(ar
+00001610: 6773 290d 0a20 2020 2020 2020 2070 6f6f  gs)..        poo
+00001620: 6c2e 6170 706c 795f 6173 796e 6328 746f  l.apply_async(to
+00001630: 6d64 5f66 696c 652c 205b 6172 6773 5d29  md_file, [args])
+00001640: 0d0a 2020 2020 706f 6f6c 2e63 6c6f 7365  ..    pool.close
+00001650: 2829 0d0a 2020 2020 706f 6f6c 2e6a 6f69  ()..    pool.joi
+00001660: 6e28 290d 0a0d 0a23 2040 7361 6665 2829  n()....# @safe()
+00001670: 0d0a 6465 6620 746f 6d64 5f66 696c 6528  ..def tomd_file(
+00001680: 6172 6773 293a 0d0a 2020 2020 6966 206e  args):..    if n
+00001690: 6f74 2061 7267 732e 666e 616d 652e 656e  ot args.fname.en
+000016a0: 6473 7769 7468 2827 2e68 746d 6c27 293a  dswith('.html'):
+000016b0: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+000016c0: 27e8 afb7 e68f 90e4 be9b 2048 544d 4c20  '......... HTML 
+000016d0: e696 87e4 bbb6 2729 0d0a 2020 2020 2020  ......')..      
+000016e0: 2020 7265 7475 726e 0d0a 2020 2020 7072    return..    pr
+000016f0: 696e 7428 6172 6773 2e66 6e61 6d65 290d  int(args.fname).
+00001700: 0a20 2020 2068 746d 6c20 3d20 6f70 656e  .    html = open
+00001710: 2861 7267 732e 666e 616d 652c 2065 6e63  (args.fname, enc
+00001720: 6f64 696e 673d 2775 7466 3827 292e 7265  oding='utf8').re
+00001730: 6164 2829 0d0a 2020 2020 6d64 203d 2074  ad()..    md = t
+00001740: 6f6d 6428 6874 6d6c 290d 0a20 2020 206f  omd(html)..    o
+00001750: 666e 616d 6520 3d20 7265 2e73 7562 2872  fname = re.sub(r
+00001760: 275c 2e68 746d 6c24 272c 2027 272c 2061  '\.html$', '', a
+00001770: 7267 732e 666e 616d 6529 202b 2027 2e6d  rgs.fname) + '.m
+00001780: 6427 0d0a 2020 2020 6f70 656e 286f 666e  d'..    open(ofn
+00001790: 616d 652c 2027 7727 2c20 656e 636f 6469  ame, 'w', encodi
+000017a0: 6e67 3d27 7574 6638 2729 2e77 7269 7465  ng='utf8').write
+000017b0: 286d 6429 0d0a 0d0a 6465 6620 746f 6d64  (md)....def tomd
+000017c0: 5f68 616e 646c 6528 6172 6773 293a 0d0a  _handle(args):..
+000017d0: 2020 2020 6966 2070 6174 682e 6973 6469      if path.isdi
+000017e0: 7228 6172 6773 2e66 6e61 6d65 293a 0d0a  r(args.fname):..
+000017f0: 2020 2020 2020 2020 746f 6d64 5f64 6972          tomd_dir
+00001800: 2861 7267 7329 0d0a 2020 2020 656c 7365  (args)..    else
+00001810: 3a0d 0a20 2020 2020 2020 2074 6f6d 645f  :..        tomd_
+00001820: 6669 6c65 2861 7267 7329 0d0a 0d0a 2320  file(args)....# 
+00001830: 4073 6166 6528 290d 0a64 6566 206f 7074  @safe()..def opt
+00001840: 695f 6d64 5f66 696c 6528 6172 6773 293a  i_md_file(args):
+00001850: 0d0a 2020 2020 5245 5f53 5243 5f46 554c  ..    RE_SRC_FUL
+00001860: 4c20 3d20 7227 e58e 9fe6 9687 5b3a efbc  L = r'......[:..
+00001870: 9a5d 5c5b 2e2b 3f5c 5d5c 2828 2e2b 3f29  .]\[.+?\]\((.+?)
+00001880: 5c29 270d 0a20 2020 2052 455f 5352 435f  \)'..    RE_SRC_
+00001890: 4655 4c4c 5f52 4550 203d 2072 27e5 8e9f  FULL_REP = r'...
+000018a0: e696 87ef bc9a 3c5c 313e 270d 0a20 2020  ......<\1>'..   
+000018b0: 2052 455f 5052 455f 4845 4144 203d 2072   RE_PRE_HEAD = r
+000018c0: 275e 5c78 3230 2a5c 2a2b 5c78 3230 2a60  '^\x20*\*+\x20*`
+000018d0: 6060 270d 0a20 2020 2052 455f 4c45 475f  ``'..    RE_LEG_
+000018e0: 544f 4b45 4e20 3d20 7227 545c 642b e380  TOKEN = r'T\d+..
+000018f0: 9127 0d0a 2020 2020 5245 5f50 5245 5f48  .'..    RE_PRE_H
+00001900: 4541 4432 203d 2072 2760 6060 5c2a 2b7c  EAD2 = r'```\*+|
+00001910: 5c2a 2b60 6060 270d 0a20 2020 2066 6e61  \*+```'..    fna
+00001920: 6d65 203d 2061 7267 732e 666e 616d 650d  me = args.fname.
+00001930: 0a20 2020 2069 6620 6e6f 7420 666e 616d  .    if not fnam
+00001940: 652e 656e 6473 7769 7468 2827 2e6d 6427  e.endswith('.md'
+00001950: 293a 0d0a 2020 2020 2020 2020 7072 696e  ):..        prin
+00001960: 7428 27e8 afb7 e68f 90e4 be9b 204d 6172  t('......... Mar
+00001970: 6b64 6f77 6e20 e696 87e4 bbb6 2729 0d0a  kdown ......')..
+00001980: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
+00001990: 2020 2020 7072 696e 7428 666e 616d 6529      print(fname)
+000019a0: 0d0a 2020 2020 636f 6e74 203d 206f 7065  ..    cont = ope
+000019b0: 6e28 666e 616d 652c 2065 6e63 6f64 696e  n(fname, encodin
+000019c0: 673d 2775 7466 3827 292e 7265 6164 2829  g='utf8').read()
+000019d0: 0d0a 2020 2020 636f 6e74 203d 2063 6f6e  ..    cont = con
+000019e0: 742e 7265 706c 6163 6528 272e 2e2f 496d  t.replace('../Im
+000019f0: 6167 6573 2f27 2c20 2769 6d67 2f27 290d  ages/', 'img/').
+00001a00: 0a20 2020 2063 6f6e 7420 3d20 7265 2e73  .    cont = re.s
+00001a10: 7562 2852 455f 4c45 475f 544f 4b45 4e2c  ub(RE_LEG_TOKEN,
+00001a20: 2027 272c 2063 6f6e 7429 0d0a 2020 2020   '', cont)..    
+00001a30: 636f 6e74 203d 2072 652e 7375 6228 5245  cont = re.sub(RE
+00001a40: 5f53 5243 5f46 554c 4c2c 2052 455f 5352  _SRC_FULL, RE_SR
+00001a50: 435f 4655 4c4c 5f52 4550 2c20 636f 6e74  C_FULL_REP, cont
+00001a60: 290d 0a20 2020 2063 6f6e 7420 3d20 7265  )..    cont = re
+00001a70: 2e73 7562 2872 2723 5c64 2b5c 2d5c 642b  .sub(r'#\d+\-\d+
+00001a80: 5c2d 5c64 2b28 3f3d 3e29 272c 2027 272c  \-\d+(?=>)', '',
+00001a90: 2063 6f6e 7429 0d0a 2020 2020 636f 6e74   cont)..    cont
+00001aa0: 203d 2072 652e 7375 6228 5245 5f50 5245   = re.sub(RE_PRE
+00001ab0: 5f48 4541 442c 2027 6060 6027 2c20 636f  _HEAD, '```', co
+00001ac0: 6e74 2c20 666c 6167 733d 7265 2e4d 290d  nt, flags=re.M).
+00001ad0: 0a20 2020 2063 6f6e 7420 3d20 7265 2e73  .    cont = re.s
+00001ae0: 7562 2852 455f 5052 455f 4845 4144 322c  ub(RE_PRE_HEAD2,
+00001af0: 2027 6060 6027 2c20 636f 6e74 290d 0a20   '```', cont).. 
+00001b00: 2020 206f 7065 6e28 666e 616d 652c 2027     open(fname, '
+00001b10: 7727 2c20 656e 636f 6469 6e67 3d27 7574  w', encoding='ut
+00001b20: 6638 2729 2e77 7269 7465 2863 6f6e 7429  f8').write(cont)
+00001b30: 0d0a 2020 200d 0a0d 0a0d 0a64 6566 206f  ..   ......def o
+00001b40: 7074 695f 6d64 5f68 616e 646c 6528 6172  pti_md_handle(ar
+00001b50: 6773 293a 0d0a 2020 2020 6966 2070 6174  gs):..    if pat
+00001b60: 682e 6973 6469 7228 6172 6773 2e66 6e61  h.isdir(args.fna
+00001b70: 6d65 293a 0d0a 2020 2020 2020 2020 6f70  me):..        op
+00001b80: 7469 5f6d 645f 6469 7228 6172 6773 290d  ti_md_dir(args).
+00001b90: 0a20 2020 2065 6c73 653a 0d0a 2020 2020  .    else:..    
+00001ba0: 2020 2020 6f70 7469 5f6d 645f 6669 6c65      opti_md_file
+00001bb0: 2861 7267 7329 0d0a 0d0a 6465 6620 6f70  (args)....def op
+00001bc0: 7469 5f6d 645f 6469 7228 6172 6773 293a  ti_md_dir(args):
+00001bd0: 0d0a 2020 2020 6469 7220 3d20 6172 6773  ..    dir = args
+00001be0: 2e66 6e61 6d65 0d0a 2020 2020 666e 616d  .fname..    fnam
+00001bf0: 6573 203d 206f 732e 6c69 7374 6469 7228  es = os.listdir(
+00001c00: 6469 7229 0d0a 2020 2020 706f 6f6c 203d  dir)..    pool =
+00001c10: 2050 6f6f 6c28 6172 6773 2e74 6872 6561   Pool(args.threa
+00001c20: 6473 290d 0a20 2020 2066 6f72 2066 6e61  ds)..    for fna
+00001c30: 6d65 2069 6e20 666e 616d 6573 3a0d 0a20  me in fnames:.. 
+00001c40: 2020 2020 2020 2061 7267 7320 3d20 636f         args = co
+00001c50: 7079 2e64 6565 7063 6f70 7928 6172 6773  py.deepcopy(args
+00001c60: 290d 0a20 2020 2020 2020 2061 7267 732e  )..        args.
+00001c70: 666e 616d 6520 3d20 7061 7468 2e6a 6f69  fname = path.joi
+00001c80: 6e28 6469 722c 2066 6e61 6d65 290d 0a20  n(dir, fname).. 
+00001c90: 2020 2020 2020 2023 2074 6f6d 645f 6669         # tomd_fi
+00001ca0: 6c65 2861 7267 7329 0d0a 2020 2020 2020  le(args)..      
+00001cb0: 2020 706f 6f6c 2e61 7070 6c79 5f61 7379    pool.apply_asy
+00001cc0: 6e63 286f 7074 695f 6d64 5f66 696c 652c  nc(opti_md_file,
+00001cd0: 205b 6172 6773 5d29 0d0a 2020 2020 706f   [args])..    po
+00001ce0: 6f6c 2e63 6c6f 7365 2829 0d0a 2020 2020  ol.close()..    
+00001cf0: 706f 6f6c 2e6a 6f69 6e28 290d 0a0d 0a0d  pool.join().....
+00001d00: 0a64 6566 2063 6f6e 6669 675f 7072 6f6a  .def config_proj
+00001d10: 2861 7267 7329 3a0d 0a20 2020 2064 6972  (args):..    dir
+00001d20: 203d 2070 6174 682e 6162 7370 6174 6828   = path.abspath(
+00001d30: 6172 6773 2e64 6972 290d 0a20 2020 2069  args.dir)..    i
+00001d40: 6620 6e6f 7420 7061 7468 2e69 7364 6972  f not path.isdir
+00001d50: 2864 6972 293a 0d0a 2020 2020 2020 2020  (dir):..        
+00001d60: 7072 696e 7428 27e8 afb7 e68f 90e4 be9b  print('.........
+00001d70: e79b aee5 bd95 2729 0d0a 2020 2020 2020  ......')..      
+00001d80: 2020 7265 7475 726e 0d0a 2020 2020 666e    return..    fn
+00001d90: 616d 6573 203d 206f 732e 6c69 7374 6469  ames = os.listdi
+00001da0: 7228 6469 7229 0d0a 2020 2020 6966 2027  r(dir)..    if '
+00001db0: 5245 4144 4d45 2e6d 6427 206e 6f74 2069  README.md' not i
+00001dc0: 6e20 666e 616d 6573 206f 7220 5c0d 0a20  n fnames or \.. 
+00001dd0: 2020 2020 2020 2027 696e 6465 782e 6874         'index.ht
+00001de0: 6d6c 2720 6e6f 7420 696e 2066 6e61 6d65  ml' not in fname
+00001df0: 7320 6f72 205c 0d0a 2020 2020 2020 2020  s or \..        
+00001e00: 2743 4e41 4d45 2720 6e6f 7420 696e 2066  'CNAME' not in f
+00001e10: 6e61 6d65 733a 0d0a 2020 2020 2020 2020  names:..        
+00001e20: 7072 696e 7428 27e7 bcba e5b0 9120 5245  print('...... RE
+00001e30: 4144 4d45 2e6d 64ef bc8c 696e 6465 782e  ADME.md...index.
+00001e40: 6874 6d6c 20e6 8896 2043 4e41 4d45 20e6  html ... CNAME .
+00001e50: 9687 e4bb b627 290d 0a20 2020 2020 2020  .....')..       
+00001e60: 2072 6574 7572 6e0d 0a20 2020 206e 616d   return..    nam
+00001e70: 6520 3d20 696e 7075 7428 27e8 afb7 e8be  e = input('.....
+00001e80: 93e5 85a5 e4b8 ade6 9687 e590 8de7 a7b0  ................
+00001e90: efbc 9a27 292e 7374 7269 7028 2920 6f72  ...').strip() or
+00001ea0: 2027 7b6e 616d 657d 270d 0a20 2020 206e   '{name}'..    n
+00001eb0: 616d 655f 656e 203d 2069 6e70 7574 2827  ame_en = input('
+00001ec0: e8af b7e8 be93 e585 a5e8 8bb1 e696 87e5  ................
+00001ed0: 908d e7a7 b0ef bc9a 2729 2e73 7472 6970  ........').strip
+00001ee0: 2829 206f 7220 277b 6e61 6d65 456e 7d27  () or '{nameEn}'
+00001ef0: 0d0a 2020 2020 7572 6c5f 656e 203d 2069  ..    url_en = i
+00001f00: 6e70 7574 2827 e8af b7e8 be93 e585 a5e8  nput('..........
+00001f10: 8bb1 e696 87e9 93be e68e a5ef bc9a 2729  ..............')
+00001f20: 2e73 7472 6970 2829 206f 7220 277b 7572  .strip() or '{ur
+00001f30: 6c45 6e7d 270d 0a20 2020 2064 6f6d 6169  lEn}'..    domai
+00001f40: 6e20 3d20 696e 7075 7428 27e8 afb7 e8be  n = input('.....
+00001f50: 93e5 85a5 e59f 9fe5 908d e589 8de7 bc80  ................
+00001f60: efbc 9a27 292e 7374 7269 7028 2920 6f72  ...').strip() or
+00001f70: 2027 7b64 6f6d 6169 6e7d 270d 0a20 2020   '{domain}'..   
+00001f80: 2063 6f6c 6f72 203d 2069 6e70 7574 2827   color = input('
+00001f90: e8af b7e8 be93 e585 a5e9 a29c e889 b2ef  ................
+00001fa0: bc9a 2729 2e73 7472 6970 2829 206f 7220  ..').strip() or 
+00001fb0: 277b 636f 6c6f 727d 270d 0a20 2020 2072  '{color}'..    r
+00001fc0: 6570 6f20 3d20 7061 7468 2e62 6173 656e  epo = path.basen
+00001fd0: 616d 6528 6469 7229 0d0a 2020 2020 0d0a  ame(dir)..    ..
+00001fe0: 2020 2020 636f 6e74 7320 3d20 7b0d 0a20      conts = {.. 
+00001ff0: 2020 2020 2020 2027 5245 4144 4d45 2e6d         'README.m
+00002000: 6427 3a20 6f70 656e 2870 6174 682e 6a6f  d': open(path.jo
+00002010: 696e 2864 6972 2c20 2752 4541 444d 452e  in(dir, 'README.
+00002020: 6d64 2729 2c20 656e 636f 6469 6e67 3d27  md'), encoding='
+00002030: 7574 6638 2729 2e72 6561 6428 292c 0d0a  utf8').read(),..
+00002040: 2020 2020 2020 2020 2769 6e64 6578 2e68          'index.h
+00002050: 746d 6c27 3a20 6f70 656e 2870 6174 682e  tml': open(path.
+00002060: 6a6f 696e 2864 6972 2c20 2769 6e64 6578  join(dir, 'index
+00002070: 2e68 746d 6c27 292c 2065 6e63 6f64 696e  .html'), encodin
+00002080: 673d 2775 7466 3827 292e 7265 6164 2829  g='utf8').read()
+00002090: 2c0d 0a20 2020 2020 2020 2027 434e 414d  ,..        'CNAM
+000020a0: 4527 3a20 6f70 656e 2870 6174 682e 6a6f  E': open(path.jo
+000020b0: 696e 2864 6972 2c20 2743 4e41 4d45 2729  in(dir, 'CNAME')
+000020c0: 2c20 656e 636f 6469 6e67 3d27 7574 6638  , encoding='utf8
+000020d0: 2729 2e72 6561 6428 292c 0d0a 2020 2020  ').read(),..    
+000020e0: 7d0d 0a20 2020 2066 6f72 2066 6e61 6d65  }..    for fname
+000020f0: 2c20 636f 6e74 2069 6e20 636f 6e74 732e  , cont in conts.
+00002100: 6974 656d 7328 293a 0d0a 2020 2020 2020  items():..      
+00002110: 2020 636f 6e74 203d 2028 0d0a 2020 2020    cont = (..    
+00002120: 2020 2020 2020 2020 636f 6e74 2e72 6570          cont.rep
+00002130: 6c61 6365 2827 7b6e 616d 657d 272c 206e  lace('{name}', n
+00002140: 616d 6529 0d0a 2020 2020 2020 2020 2020  ame)..          
+00002150: 2020 2020 2020 2e72 6570 6c61 6365 2827        .replace('
+00002160: 7b6e 616d 6545 6e7d 272c 206e 616d 655f  {nameEn}', name_
+00002170: 656e 290d 0a20 2020 2020 2020 2020 2020  en)..           
+00002180: 2020 2020 202e 7265 706c 6163 6528 277b       .replace('{
+00002190: 7572 6c45 6e7d 272c 2075 726c 5f65 6e29  urlEn}', url_en)
+000021a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000021b0: 2020 2e72 6570 6c61 6365 2827 7b75 726c    .replace('{url
+000021c0: 456e 7d27 2c20 7572 6c5f 656e 290d 0a20  En}', url_en).. 
+000021d0: 2020 2020 2020 2020 2020 2020 2020 202e                 .
+000021e0: 7265 706c 6163 6528 277b 646f 6d61 696e  replace('{domain
+000021f0: 7d27 2c20 646f 6d61 696e 290d 0a20 2020  }', domain)..   
+00002200: 2020 2020 2020 2020 2020 2020 202e 7265               .re
+00002210: 706c 6163 6528 277b 636f 6c6f 727d 272c  place('{color}',
+00002220: 2063 6f6c 6f72 290d 0a20 2020 2020 2020   color)..       
+00002230: 2020 2020 2020 2020 202e 7265 706c 6163           .replac
+00002240: 6528 277b 6164 6d69 6e4e 616d 657d 272c  e('{adminName}',
+00002250: 2027 e9a3 9ee9 be99 2729 0d0a 2020 2020   '......')..    
+00002260: 2020 2020 2020 2020 2020 2020 2e72 6570              .rep
+00002270: 6c61 6365 2827 7b61 646d 696e 556e 7d27  lace('{adminUn}'
+00002280: 2c20 2777 697a 6172 6466 6f72 6365 6c27  , 'wizardforcel'
+00002290: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000022a0: 2020 202e 7265 706c 6163 6528 277b 6164     .replace('{ad
+000022b0: 6d69 6e51 717d 272c 2027 3536 3238 3236  minQq}', '562826
+000022c0: 3137 3927 290d 0a20 2020 2020 2020 2020  179')..         
+000022d0: 2020 2020 2020 202e 7265 706c 6163 6528         .replace(
+000022e0: 277b 7265 706f 7d27 2c20 7265 706f 290d  '{repo}', repo).
+000022f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002300: 202e 7265 706c 6163 6528 277b 646f 636b   .replace('{dock
+00002310: 6572 4e61 6d65 7d27 2c20 7265 706f 290d  erName}', repo).
+00002320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002330: 202e 7265 706c 6163 6528 277b 7079 7069   .replace('{pypi
+00002340: 4e61 6d65 7d27 2c20 7265 706f 290d 0a20  Name}', repo).. 
+00002350: 2020 2020 2020 2020 2020 2020 2020 202e                 .
+00002360: 7265 706c 6163 6528 277b 6e70 6d4e 616d  replace('{npmNam
+00002370: 657d 272c 2072 6570 6f29 0d0a 2020 2020  e}', repo)..    
+00002380: 2020 2020 290d 0a20 2020 2020 2020 206f      )..        o
+00002390: 7065 6e28 7061 7468 2e6a 6f69 6e28 6469  pen(path.join(di
+000023a0: 722c 2066 6e61 6d65 292c 2027 7727 2c20  r, fname), 'w', 
+000023b0: 656e 636f 6469 6e67 3d27 7574 6638 2729  encoding='utf8')
+000023c0: 2e77 7269 7465 2863 6f6e 7429 0d0a 0d0a  .write(cont)....
+000023d0: 6465 6620 636f 6e76 6572 745f 6364 7269  def convert_cdri
+000023e0: 7665 5f6c 6f67 2861 7267 7329 3a0d 0a20  ve_log(args):.. 
+000023f0: 2020 2052 455f 494e 464f 203d 2072 275c     RE_INFO = r'\
+00002400: 5b28 2e2b 3f29 5c5d 285b 5e5c 5b5d 2b29  [(.+?)\]([^\[]+)
+00002410: 270d 0a20 2020 2052 455f 5449 544c 4520  '..    RE_TITLE 
+00002420: 3d20 7227 e4b8 8ae4 bca0 3a20 282e 2b3f  = r'......: (.+?
+00002430: 2920 5c28 5b5c 645c 2e5d 2b20 5c77 2b5c  ) \([\d\.]+ \w+\
+00002440: 295c 6e27 0d0a 2020 2020 5245 5f4d 4554  )\n'..    RE_MET
+00002450: 4120 3d20 7227 4d45 5441 2055 524c 202d  A = r'META URL -
+00002460: 3e20 285c 532b 2927 0d0a 2020 2020 0d0a  > (\S+)'..    ..
+00002470: 2020 2020 666e 616d 6520 3d20 6172 6773      fname = args
+00002480: 2e66 6e61 6d65 0d0a 2020 2020 636f 203d  .fname..    co =
+00002490: 206f 7065 6e28 666e 616d 652c 2065 6e63   open(fname, enc
+000024a0: 6f64 696e 673d 2775 7466 3827 292e 7265  oding='utf8').re
+000024b0: 6164 2829 0d0a 2020 2020 636f 7320 3d20  ad()..    cos = 
+000024c0: 636f 2e73 706c 6974 2827 20e4 b88a e4bc  co.split(' .....
+000024d0: a03a 2027 290d 0a20 2020 2072 6573 203d  .: ')..    res =
+000024e0: 205b 277c 20e6 9687 e4bb b620 7c20 e993   ['| ...... | ..
+000024f0: bee6 8ea5 207c 5c6e 7c20 2d2d 2d20 7c20  .... |\n| --- | 
+00002500: 2d2d 2d20 7c5c 6e27 5d0d 0a20 2020 2066  --- |\n']..    f
+00002510: 6f72 2069 6e66 6f20 696e 2063 6f73 3a0d  or info in cos:.
+00002520: 0a20 2020 2020 2020 2069 6e66 6f20 3d20  .        info = 
+00002530: 2720 e4b8 8ae4 bca0 3a20 2720 2b20 696e  ' ......: ' + in
+00002540: 666f 0d0a 2020 2020 2020 2020 7469 746c  fo..        titl
+00002550: 6520 3d20 7265 2e73 6561 7263 6828 5245  e = re.search(RE
+00002560: 5f54 4954 4c45 2c20 696e 666f 290d 0a20  _TITLE, info).. 
+00002570: 2020 2020 2020 206d 6574 6120 3d20 7265         meta = re
+00002580: 2e73 6561 7263 6828 5245 5f4d 4554 412c  .search(RE_META,
+00002590: 2069 6e66 6f29 0d0a 2020 2020 2020 2020   info)..        
+000025a0: 6966 206e 6f74 2074 6974 6c65 3a20 636f  if not title: co
+000025b0: 6e74 696e 7565 0d0a 2020 2020 2020 2020  ntinue..        
+000025c0: 7469 746c 6520 3d20 7469 746c 652e 6772  title = title.gr
+000025d0: 6f75 7028 3129 0d0a 2020 2020 2020 2020  oup(1)..        
+000025e0: 6d65 7461 203d 206d 6574 612e 6772 6f75  meta = meta.grou
+000025f0: 7028 3129 2069 6620 6d65 7461 2065 6c73  p(1) if meta els
+00002600: 6520 27e6 9caa e4b8 8ae4 bca0 270d 0a20  e '.........'.. 
+00002610: 2020 2020 2020 2072 6573 2e61 7070 656e         res.appen
+00002620: 6428 6627 7c20 7b74 6974 6c65 7d20 7c20  d(f'| {title} | 
+00002630: 7b6d 6574 617d 207c 5c6e 2729 0d0a 2020  {meta} |\n')..  
+00002640: 2020 2020 2020 0d0a 2020 2020 7265 7320        ..    res 
+00002650: 3d20 2727 2e6a 6f69 6e28 7265 7329 0d0a  = ''.join(res)..
+00002660: 2020 2020 6f70 656e 2866 6e61 6d65 202b      open(fname +
+00002670: 2027 2e6d 6427 2c20 2777 272c 2065 6e63   '.md', 'w', enc
+00002680: 6f64 696e 673d 2775 7466 3827 292e 7772  oding='utf8').wr
+00002690: 6974 6528 7265 7329 0d0a 0d0a 6465 6620  ite(res)....def 
+000026a0: 726d 5f73 7566 6669 7828 6172 6773 293a  rm_suffix(args):
+000026b0: 0d0a 2020 2020 6469 7220 3d20 6172 6773  ..    dir = args
+000026c0: 2e64 6972 0d0a 2020 2020 6966 206e 6f74  .dir..    if not
+000026d0: 2070 6174 682e 6973 6469 7228 6469 7229   path.isdir(dir)
+000026e0: 3a0d 0a20 2020 2020 2020 2070 7269 6e74  :..        print
+000026f0: 2827 e8af b7e6 8f90 e4be 9be7 9bae e5bd  ('..............
+00002700: 9527 290d 0a20 2020 2020 2020 2072 6574  .')..        ret
+00002710: 7572 6e0d 0a20 2020 2068 746d 6c5f 666e  urn..    html_fn
+00002720: 616d 6573 203d 205b 0d0a 2020 2020 2020  ames = [..      
+00002730: 2020 6620 666f 7220 6620 696e 206f 732e    f for f in os.
+00002740: 6c69 7374 6469 7228 6469 7229 200d 0a20  listdir(dir) .. 
+00002750: 2020 2020 2020 2069 6620 662e 656e 6473         if f.ends
+00002760: 7769 7468 2827 2e68 746d 6c27 290d 0a20  with('.html').. 
+00002770: 2020 205d 0d0a 2020 2020 7375 6666 5f63     ]..    suff_c
+00002780: 6e74 203d 207b 7d0d 0a20 2020 2066 6f72  nt = {}..    for
+00002790: 2066 2069 6e20 6874 6d6c 5f66 6e61 6d65   f in html_fname
+000027a0: 733a 0d0a 2020 2020 2020 2020 636f 6e74  s:..        cont
+000027b0: 203d 206f 7065 6e28 7061 7468 2e6a 6f69   = open(path.joi
+000027c0: 6e28 6469 722c 2066 292c 2065 6e63 6f64  n(dir, f), encod
+000027d0: 696e 673d 2775 7466 3827 292e 7265 6164  ing='utf8').read
+000027e0: 2829 0d0a 2020 2020 2020 2020 636f 6e74  ()..        cont
+000027f0: 203d 2072 652e 7375 6228 7227 3c5c 3f78   = re.sub(r'<\?x
+00002800: 6d6c 5b5e 3e5d 2a3e 272c 2027 272c 2063  ml[^>]*>', '', c
+00002810: 6f6e 7429 0d0a 2020 2020 2020 2020 636f  ont)..        co
+00002820: 6e74 203d 2072 652e 7375 6228 7227 786d  nt = re.sub(r'xm
+00002830: 6c6e 733d 222e 2b3f 2227 2c20 2727 2c20  lns=".+?"', '', 
+00002840: 636f 6e74 290d 0a20 2020 2020 2020 2074  cont)..        t
+00002850: 6974 6c65 203d 2070 7128 636f 6e74 292e  itle = pq(cont).
+00002860: 6669 6e64 2827 6831 2729 2e65 7128 3029  find('h1').eq(0)
+00002870: 2e74 6578 7428 290d 0a20 2020 2020 2020  .text()..       
+00002880: 2069 6620 6e6f 7420 7469 746c 653a 2063   if not title: c
+00002890: 6f6e 7469 6e75 650d 0a20 2020 2020 2020  ontinue..       
+000028a0: 206d 203d 2072 652e 7365 6172 6368 2872   m = re.search(r
+000028b0: 275b 5c2d 5c7c 5d5c 735b 5e5c 2d5c 7c5d  '[\-\|]\s[^\-\|]
+000028c0: 2b24 272c 2074 6974 6c65 290d 0a20 2020  +$', title)..   
+000028d0: 2020 2020 2069 6620 6e6f 7420 6d3a 2063       if not m: c
+000028e0: 6f6e 7469 6e75 650d 0a20 2020 2020 2020  ontinue..       
+000028f0: 2073 7566 6620 3d20 6d2e 6772 6f75 7028   suff = m.group(
+00002900: 290d 0a20 2020 2020 2020 2073 7566 665f  )..        suff_
+00002910: 636e 745b 7375 6666 5d20 3d20 7375 6666  cnt[suff] = suff
+00002920: 5f63 6e74 2e67 6574 2873 7566 662c 2030  _cnt.get(suff, 0
+00002930: 2920 2b20 310d 0a20 2020 2020 2020 2070  ) + 1..        p
+00002940: 7269 6e74 2866 2766 696c 653a 207b 667d  rint(f'file: {f}
+00002950: 2c20 7469 746c 653a 2022 7b74 6974 6c65  , title: "{title
+00002960: 7d22 2c20 7375 6666 6978 3a20 227b 7375  }", suffix: "{su
+00002970: 6666 7d22 2729 0d0a 2020 2020 0d0a 2020  ff}"')..    ..  
+00002980: 2020 666f 7220 7375 6666 2c20 636e 7420    for suff, cnt 
+00002990: 696e 206c 6973 7428 7375 6666 5f63 6e74  in list(suff_cnt
+000029a0: 2e69 7465 6d73 2829 293a 0d0a 2020 2020  .items()):..    
+000029b0: 2020 2020 6966 2063 6e74 203e 206c 656e      if cnt > len
+000029c0: 2868 746d 6c5f 666e 616d 6573 2920 2a20  (html_fnames) * 
+000029d0: 6172 6773 2e72 6174 653a 0d0a 2020 2020  args.rate:..    
+000029e0: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
+000029f0: e6a3 80e6 b58b e588 b0e5 908e e7bc 8020  ............... 
+00002a00: 7b73 7566 667d 2729 0d0a 2020 2020 2020  {suff}')..      
+00002a10: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00002a20: 2020 2020 2064 656c 2073 7566 665f 636e       del suff_cn
+00002a30: 745b 7375 6666 5d0d 0a20 2020 200d 0a20  t[suff]..    .. 
+00002a40: 2020 2069 6620 6c65 6e28 7375 6666 5f63     if len(suff_c
+00002a50: 6e74 2920 3d3d 2030 3a20 7265 7475 726e  nt) == 0: return
+00002a60: 0d0a 2020 2020 666f 7220 6620 696e 2068  ..    for f in h
+00002a70: 746d 6c5f 666e 616d 6573 3a0d 0a20 2020  tml_fnames:..   
+00002a80: 2020 2020 2066 6620 3d20 7061 7468 2e6a       ff = path.j
+00002a90: 6f69 6e28 6469 722c 2066 290d 0a20 2020  oin(dir, f)..   
+00002aa0: 2020 2020 2070 7269 6e74 2866 6629 0d0a       print(ff)..
+00002ab0: 2020 2020 2020 2020 636f 6e74 203d 206f          cont = o
+00002ac0: 7065 6e28 6666 2c20 656e 636f 6469 6e67  pen(ff, encoding
+00002ad0: 3d27 7574 6638 2729 2e72 6561 6428 290d  ='utf8').read().
+00002ae0: 0a20 2020 2020 2020 2066 6f72 2073 7566  .        for suf
+00002af0: 6620 696e 2073 7566 665f 636e 743a 0d0a  f in suff_cnt:..
+00002b00: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+00002b10: 203d 2063 6f6e 742e 7265 706c 6163 6528   = cont.replace(
+00002b20: 7375 6666 2c20 2727 290d 0a20 2020 2020  suff, '')..     
+00002b30: 2020 206f 7065 6e28 6666 2c20 2777 272c     open(ff, 'w',
+00002b40: 2065 6e63 6f64 696e 673d 2775 7466 3827   encoding='utf8'
+00002b50: 292e 7772 6974 6528 636f 6e74 290d 0a20  ).write(cont).. 
+00002b60: 2020 20
```

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool/pdf_tool.py` & `BookerWikiTool-2023.3.30.0/BookerWikiTool/pdf_tool.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,542 +1,530 @@
-import fitz
-import win32com.client
-import subprocess as subp
-import sys
-from os import path
-from pyquery import PyQuery as pq
-import re
-import os
-import shutil
-import copy
-import tempfile
-import uuid
-import traceback
-from PIL import Image, ImageFile
-from multiprocessing import Pool
-from imgyaso import pngquant_bts
-import img2pdf
-from io import BytesIO
-from .util import *
-
-ImageFile.LOAD_TRUNCATED_IMAGES = True
-fitz.Document.is_image = fitz.Document.xref_is_image
-
-app_map = {
-    'ppt': ['PowerPoint.Application', 'Presentations'],
-    'pptx': ['PowerPoint.Application', 'Presentations'],
-    'doc': ['Word.Application', 'Documents'],
-    'docx': ['Word.Application', 'Documents'],
-    'xls': ['Excel.Application', 'Workbooks'],
-    'xlsx': ['Excel.Application', 'Workbooks'],
-}
-
-code_fonts = ['Courier', 'Mocano', 'Consolas', 'Monospace', 'Menlo']
-
-def comp_pdf(args):
-    fname = args.fname
-    if not fname.endswith('.pdf'):
-        print('请提供 PDF 文件')
-        return
-    print(f'file: {fname}')
-    doc = fitz.open("pdf", open(fname, 'rb').read())
-    for i, p in enumerate(doc):
-        print(f'page: {i+1}')
-        imgs = p.get_images()
-        for ii, info in enumerate(imgs):
-            xref = info[0]
-            print(f'image: {ii+1}, xref: {xref}')
-            img = fitz.Pixmap(doc, xref)
-            data = img.pil_tobytes(format="JPEG", quality=100)
-            data = pngquant_bts(data)
-            p.replace_image(xref, stream=data)
-    doc.save(fname, clean=True, garbage=4, deflate=True, linear=True)
-    doc.close()
-
-def process_el_code(rt):
-    el_spans = rt('span')
-    for el in el_spans:
-        el = pq(el)
-        # 如果 SPAN 的字体是等宽字体之一，就认为是内联代码
-        style = el.attr('style') or ''
-        is_code = any([
-            f.lower() in style.lower() 
-            for f in code_fonts
-        ])
-        if not is_code: continue
-        el_code = rt('<code></code>')
-        el_code.text(el.text())
-        el_code.attr('style', el.attr('style'))
-        el.replace_with(el_code)
-
-def process_el_pre(rt):
-    el_paras = rt('p')
-    for el in el_paras:
-        el = pq(el)
-        # 如果段落只包含内联代码，就认为是代码块
-        is_pre = all([pq(ch).is_('code') for ch in el.children()])
-        if not is_pre: continue
-        el_pre = rt('<pre></pre>')
-        # 移除里面的所有 CODE 标签但保留内容
-        for el_code in el.children():
-            el_code = pq(el_code)
-            el_span = rt('<span></span>')
-            el_span.text(el_code.text() or '')
-            el_code.replace_with(el_span)
-        el_pre.text(el.text().replace('\n', ''))
-        el_pre.attr('style', el.attr('style'))
-        el.replace_with(el_pre)
-
-def process_el_heading(rt):
-    def get_font_size(el):
-        style = el.attr('style') or ''
-        m = re.search(r'font-size:\s*(\d+\.\d+)', style)
-        if not m: return 0
-        else: return float(m.group(1))
-    el_paras = rt('p')
-    for el in el_paras:
-        el = pq(el)
-        # 如果字体大于等于 16，则认为它是标题
-        el_spans = el.find('span')
-        is_heading = (
-            get_font_size(el) >= 16 or
-            any([get_font_size(pq(el)) >= 16 for el in el_spans])
-        )
-        if not is_heading: continue
-        el_h2 = rt('<h2></h2>')
-        el_h2.html(el.html() or '')
-        el_h2.attr('style', el.attr('style'))
-        el.replace_with(el_h2)
-
-def process_pre_indent(rt):
-    def get_indent(el):
-        style = el.attr('style') or ''
-        m = re.search(r'left:\s*(\d+\.\d+)', style)
-        if not m: return 0
-        else: return float(m.group(1))
-    inds = [get_indent(pq(el)) for el in rt('pre')]
-    inds_uni = list({x for x in inds if x != 0})
-    inds_uni.sort()
-    if len(inds_uni) <= 1: return
-    # 计算基址和偏移，转换为空格数
-    diff = inds_uni[1] - inds_uni[0]
-    base = inds_uni[0]
-    for i, el in enumerate(rt('pre')):
-        if inds[i] == 0: continue
-        nspace = int((inds[i] - base) // diff) * 4
-        el = pq(el)
-        el.text(' ' * nspace + (el.text() or ''))
-
-
-def process_html_code(html):
-    rt = pq(html)
-    process_el_code(rt)
-    # process_el_pre(rt)
-    process_pre_indent(rt)
-    process_el_heading(rt)
-    # 处理缩进
-    html = rt('body').html() if rt('body') else str(rt)
-    # 合并连续的 PRE
-    # html = re.sub(r'</pre>\s*<pre[^>]*>', '\n', html)
-    # 合并段落内的换行
-    # html = re.sub(r'(?<![\.\?!:])</p>\s*<p [^>]*>', ' ', html)
-    # html = re.sub(r'</?span[^>]*>', '' ,html)
-    # html = re.sub(r'style=".+?"', '' ,html)
-    return html
-
-def pdf2html_file(args):
-    fname, dir = args.fname, args.dir
-    if not fname.endswith('.pdf'):
-        print('请提供 PDF 文件')
-        return
-    print(f'file: {fname}')
-    title = path.basename(fname)[:-4]
-    doc = fitz.open(fname)
-    lp = len(str(len(doc)))
-    for ip, p in enumerate(doc):
-        print(f'page: {ip + 1}')
-        html = process_html_code(p.get_text("html"))
-        # html = (p.get_text("html"))
-        html_fname = path.join(dir, f'{title}_{ip+1:0{lp}d}.html')
-        print(f'save: {html_fname}')
-        open(html_fname, 'w', encoding='utf8').write(html)
-
-    doc.close()
-
-def pdf2html_dir(args):
-    dir = args.fname
-    for fname in os.listdir(dir):
-        try:
-            ffname = path.join(dir, fname)
-            args.fname = ffname
-            pdf2html_file(args)
-        except: traceback.print_exc()
-
-def pdf2html(args):
-    if path.isdir(args.fname):
-        pdf2html_dir(args)
-    else:
-        pdf2html_file(args)
-
-
-def ext_pdf(args):
-    if path.isdir(args.fname):
-        ext_pdf_dir(args)
-    else:
-        ext_pdf_file(args)
-
-def ext_pdf_dir(args):
-    dir = args.fname
-    for fname in os.listdir(dir):
-        try:
-            ffname = path.join(dir, fname)
-            args.fname = ffname
-            ext_pdf_file(args)
-        except: traceback.print_exc()
-
-def ext_pdf_file(args):
-    fname, dir = args.fname, args.dir
-    if not fname.endswith('.pdf'):
-        print('请提供 PDF 文件')
-        return
-    print(f'file: {fname}')
-    title = path.basename(fname)[:-4]
-
-    doc = fitz.open(fname)
-    lp = len(str(len(doc)))
-    for ip, p in enumerate(doc):
-        print(f'page: {ip + 1}')
-        
-        # 判断是否整页截图
-        if args.whole:
-            img = p.get_pixmap(dpi=400)
-            imgname = path.join(dir, f'{title}_{ip+1:0{lp}d}.png')
-            print(f'save: {imgname}')
-            img.save(imgname)
-            continue
-        
-        imgs = p.get_images()
-        limg = len(str(len(imgs)))
-        for ii, info in enumerate(imgs):
-            xref = info[0]
-            print(f'img: {ii + 1}, xref: {xref}')
-            img = fitz.Pixmap(doc, xref)
-            imgname = path.join(dir, f'{title}_{ip+1:0{lp}d}_{ii+1:0{limg}d}.png')
-            print(f'save: {imgname}')
-            img.save(imgname)
-    
-    doc.close()
-
-def get_scale_by_width(wid):
-    if wid < 800:
-        return 4
-    elif wid < 900:
-        return 3.5
-    elif wid < 1000:
-        return 3
-    elif wid < 1200:
-        return 2.5
-    elif wid < 1600:
-        return 2
-    elif wid < 2000:
-        return 1.5
-    elif wid < 3200:
-        return 1
-    elif wid < 4200:
-        return 0.75
-    else:
-        return 0.5
-
-def pack_pdf(args):
-    dir, rgx = args.dir, args.regex
-    if dir.endswith('/') or \
-        dir.endswith('\\'):
-        dir = dir[:-1]
-    
-    fnames = filter(is_pic, os.listdir(dir))
-    if not rgx:
-        fnames = [path.join(dir, f) for f in fnames]
-        pdf = img2pdf.convert(fnames)
-        fname = dir + '.pdf'
-        print(fname)
-        open(fname, 'wb').write(pdf)
-        return
-        
-    d = {}
-    for fname in fnames:
-        m = re.search(rgx, fname)
-        if not m: continue
-        kw = m.group(0)
-        d.setdefault(kw, [])
-        d[kw].append(fname)
-        
-    for kw, fnames in d.items():
-        fnames = [path.join(dir, f) for f in fnames]
-        pdf = img2pdf.convert(fnames)
-        fname = path.join(dir, kw + '.pdf')
-        print(fname)
-        open(fname, 'wb').write(pdf)
-
-def office2pdf(fname, ofname):
-    m = re.search(r'\.(\w+)$', fname)
-    ext = m.group(1) if m else ""
-    if ext not in app_map:
-        raise FileError(f'{fname} 不是 DOC、XLS 或 PPT 文件')
-    app = win32com.client.Dispatch(app_map[ext][0])
-    ppt = getattr(app, app_map[ext][1]).Open(fname)
-    ppt.SaveAs(ofname, 32)
-    app.Quit()
-    
-def office2pdf_file(args):
-    fname = args.fname
-    print(fname)
-    m = re.search(r'\.(\w+)$', fname)
-    ext = m.group(1) if m else ""
-    if ext not in app_map:
-        print('请提供 DOC、XLS 或 PPT 文件')
-        return
-    fname = path.join(os.getcwd(), fname)
-    ofname = re.sub(r'\.\w+$', '', fname) + '.pdf'
-    office2pdf(fname, ofname)
-    print("转换成功！")
-
-def office2pdf_dir(args):
-    dir = args.fname
-    fnames = os.listdir(dir)
-    for f in fnames:
-        ff = path.join(dir, f)
-        args.fname = ff
-        try: office2pdf_file(args)
-        except Exception as ex: traceback.print_exc()
-
-def waifu2x_auto_file_safe(args):
-    try: waifu2x_auto_file(args)
-    except Exception as ex: traceback.print_exc()
-
-def waifu2x_auto_file(args):
-    fname = args.fname
-    if not is_pic(fname):
-        print('请提供图像')
-        return
-    print(fname)
-    try: img = Image.open(fname)
-    except: 
-        print('文件无法打开')
-        return
-    width = min(img.size[0], img.size[1])
-    scale = get_scale_by_width(width)
-    img.close()
-    p = find_cmd_path('waifu2x-converter-cpp')
-    cmd = [
-        'waifu2x-converter-cpp', 
-        '-m', 'noise-scale',
-        '--noise-level', '2',
-        '--scale-ratio', str(scale),
-        '--block-size', '256',
-        '-i', fname,
-        '-o', fname,
-        '--model-dir', path.join(p, 'models_rgb'),
-        '--disable-gpu',
-    ]
-    print(f'cmd: {cmd}')
-    r = subp.Popen(
-        cmd, 
-        shell=True,
-        stdout=subp.PIPE,
-        stderr=subp.PIPE,
-    ).communicate()
-    open(fname, 'ab').close() # touch
-    print(r[0].decode('utf8', 'ignore') or 
-        r[1].decode('utf8', 'ignore'))
-
-def waifu2x_auto_dir(args):
-    dir = args.fname
-    fnames = os.listdir(dir)
-    pool = Pool(args.threads)
-    for f in fnames:
-        ff = path.join(dir, f)
-        args = copy.deepcopy(args)
-        args.fname = ff
-        pool.apply_async(waifu2x_auto_file_safe, [args])
-    pool.close()
-    pool.join()
-    
-def waifu2x_auto_handle(args):
-    # 检查 waifu2x
-    if not find_cmd_path('waifu2x-converter-cpp'): 
-        print('waifu2x-converter-cpp 未找到，请下载并将其目录添加到系统变量 PATH 中')
-        return
-    if path.isdir(args.fname):
-        waifu2x_auto_dir(args)
-    else:
-        waifu2x_auto_file(args)
-        
-def office2pdf_handle(args):
-    if path.isdir(args.fname):
-        office2pdf_dir(args)
-    else:
-        office2pdf_file(args)
-
-def anime4k_auto_file(args):
-    fname = args.fname
-    if not is_pic(fname):
-        print('请提供图像')
-        return
-    print(fname)
-    try: img = Image.open(fname)
-    except: 
-        print('文件无法打开')
-        return
-    width = min(img.size[0], img.size[1])
-    scale = get_scale_by_width(width)
-    img.close()
-    cmd = [
-        'Anime4KCPP_CLI', 
-        '-t', str(args.threads),
-        '-z', str(scale),
-        '-i', fname,
-        '-o', fname,
-        "-w", "-H",
-        "-L", "3",
-    ]
-    if args.gpu: cmd.append('-q')
-    print(f'cmd: {cmd}')
-    r = subp.Popen(
-        cmd, 
-        shell=True,
-        stdout=subp.PIPE,
-        stderr=subp.PIPE,
-        cwd=find_cmd_path('Anime4KCPP_CLI'),
-    ).communicate()
-    open(fname, 'ab').close() # touch
-    print(r[0].decode('utf8', 'ignore') or 
-        r[1].decode('utf8', 'ignore'))
-        
-def anime4k_auto_file_safe(args):
-    try: anime4k_auto_file(args)
-    except Exception as ex: traceback.print_exc()
-
-def anime4k_auto_dir(args):
-    dir = args.fname
-    fnames = os.listdir(dir)
-    for f in fnames:
-        ff = path.join(dir, f)
-        args.fname = ff
-        anime4k_auto_file_safe(args)
-
-def anime4k_auto_handle(args):
-    # 检查 waifu2x
-    if not find_cmd_path('Anime4KCPP_CLI'): 
-        print('Anime4KCPP_CLI 未找到，请下载并将其目录添加到系统变量 PATH 中')
-        return
-    if path.isdir(args.fname):
-        anime4k_auto_dir(args)
-    else:
-        anime4k_auto_file(args)
-
-def pdf_auto_file(args):
-    fname = args.fname
-    threads = args.threads
-    if not fname.endswith('.pdf'):
-        print('请提供 PDF 文件')
-        return
-    print(f'file: {fname}')
-    tmpdir = path.join(tempfile.gettempdir(), uuid.uuid4().hex)
-    safe_mkdir(tmpdir)
-    
-    cmds = [
-        ['wiki-tool', 'ext-pdf', '-d', tmpdir, fname],
-        ['wiki-tool', 'tog-bw', '-t', str(threads), tmpdir],
-        ['wiki-tool', 'anime4k-auto', '-t', str(threads), tmpdir],
-        ['imgyaso', '-m', 'thres', '-t', str(threads), tmpdir],
-        ['wiki-tool', 'pack-pdf', tmpdir],
-    ]
-    if args.gpu: cmds[2].append('-G')
-    if args.whole: cmds[0].append('-w')
-    for cmd in cmds:
-        subp.Popen(cmd, shell=True).communicate()
-    if path.isfile(fname + '.bak'): os.unlink(fname + '.bak')
-    shutil.move(fname, fname + '.bak')
-    shutil.move(path.abspath(tmpdir) + '.pdf', fname)
-    
-    safe_rmdir(tmpdir)
-    
-def pdf_auto_dir(args):
-    dir = args.fname
-    fnames = os.listdir(dir)
-    for f in fnames:
-        ff = path.join(dir, f)
-        args.fname = ff
-        pdf_auto_file_safe(args)
-
-def pdf_auto_file_safe(args):
-    try: pdf_auto_file(args)
-    except Exception as ex: traceback.print_exc()
-    
-
-def pdf_auto_handle(args):
-    if path.isdir(args.fname):
-        pdf_auto_dir(args)
-    else:
-        pdf_auto_file(args)
-
-def pg_all_imgs_area(pg):
-    rects = [
-        pg.get_image_rects(info[0])
-        for info in pg.get_images()
-    ]
-    rects = [r[0] for r in rects if r]
-    return sum([(r[2] - r[0]) * (r[3] - r[1]) for r in rects])
-
-def pg_area(pg):
-    return (pg.rect[2] - pg.rect[0]) * (pg.rect[3] - pg.rect[1])
-
-def is_scanned_pdf(fname, imgs_area_rate=0.8, scanned_pg_rate=0.8):
-    doc = fitz.open("pdf", open(fname, 'rb').read())
-    rate = sum([
-        pg_all_imgs_area(pg) >= pg_area(pg) * imgs_area_rate
-        for pg in doc
-    ]) / len(doc)
-    return rate >= scanned_pg_rate
-    
-def tr_pick_scanned_pdf(fname, odirs, imgs_area_rate, scanned_pg_rate):
-    scanned = is_scanned_pdf(
-        fname, 
-        imgs_area_rate=imgs_area_rate, 
-        scanned_pg_rate=scanned_pg_rate,
-    )
-    rtext = '扫描版' if scanned else '文字版'
-    print(f'{fname}：{rtext}')
-    if scanned:
-        shutil.move(fname, path.join(odirs[0], path.basename(fname)))
-    else:
-        shutil.move(fname, path.join(odirs[1], path.basename(fname)))
-    
-def tr_pick_scanned_pdf_safe(*args, **kw):
-    try: tr_pick_scanned_pdf(*args, **kw)
-    except: traceback.print_exc()
-    
-def pick_scanned_pdf(args):
-    dir = args.dir
-    if not path.isdir(dir):
-        print('请提供目录')
-        return
-    odir0 = path.join(dir, '扫描版')
-    odir1 = path.join(dir, '文字版')
-    safe_mkdir(odir0)
-    safe_mkdir(odir1)
-    pool = Pool(args.threads)
-    for f in os.listdir(dir):
-        if not f.endswith('.pdf'):
-            continue
-        ff = path.join(dir, f)
-        pool.apply_async(
-            tr_pick_scanned_pdf_safe, 
-            [
-                ff, [odir0, odir1], 
-                args.imgs_area_rate, 
-                args.scanned_pg_rate
-            ]
-        )
-    pool.close()
-    pool.join()
-        
+import fitz
+import subprocess as subp
+import sys
+from os import path
+from pyquery import PyQuery as pq
+import re
+import os
+import shutil
+import copy
+import tempfile
+import uuid
+import traceback
+from PIL import Image, ImageFile
+from multiprocessing import Pool
+from imgyaso import pngquant_bts
+import img2pdf
+from io import BytesIO
+from .util import *
+
+ImageFile.LOAD_TRUNCATED_IMAGES = True
+fitz.Document.is_image = fitz.Document.xref_is_image
+
+app_map = {
+    'ppt': ['PowerPoint.Application', 'Presentations'],
+    'pptx': ['PowerPoint.Application', 'Presentations'],
+    'doc': ['Word.Application', 'Documents'],
+    'docx': ['Word.Application', 'Documents'],
+    'xls': ['Excel.Application', 'Workbooks'],
+    'xlsx': ['Excel.Application', 'Workbooks'],
+}
+
+code_fonts = ['Courier', 'Mocano', 'Consolas', 'Monospace', 'Menlo']
+
+def comp_pdf(args):
+    fname = args.fname
+    if not fname.endswith('.pdf'):
+        print('请提供 PDF 文件')
+        return
+    print(f'file: {fname}')
+    doc = fitz.open("pdf", open(fname, 'rb').read())
+    for i, p in enumerate(doc):
+        print(f'page: {i+1}')
+        imgs = p.get_images()
+        for ii, info in enumerate(imgs):
+            xref = info[0]
+            print(f'image: {ii+1}, xref: {xref}')
+            img = fitz.Pixmap(doc, xref)
+            data = img.pil_tobytes(format="JPEG", quality=100)
+            data = pngquant_bts(data)
+            p.replace_image(xref, stream=data)
+    doc.save(fname, clean=True, garbage=4, deflate=True, linear=True)
+    doc.close()
+
+def process_el_code(rt):
+    el_spans = rt('span')
+    for el in el_spans:
+        el = pq(el)
+        # 如果 SPAN 的字体是等宽字体之一，就认为是内联代码
+        style = el.attr('style') or ''
+        is_code = any([
+            f.lower() in style.lower() 
+            for f in code_fonts
+        ])
+        if not is_code: continue
+        el_code = rt('<code></code>')
+        el_code.text(el.text())
+        el_code.attr('style', el.attr('style'))
+        el.replace_with(el_code)
+
+def process_el_pre(rt):
+    el_paras = rt('p')
+    for el in el_paras:
+        el = pq(el)
+        # 如果段落只包含内联代码，就认为是代码块
+        is_pre = all([pq(ch).is_('code') for ch in el.children()])
+        if not is_pre: continue
+        el_pre = rt('<pre></pre>')
+        # 移除里面的所有 CODE 标签但保留内容
+        for el_code in el.children():
+            el_code = pq(el_code)
+            el_span = rt('<span></span>')
+            el_span.text(el_code.text() or '')
+            el_code.replace_with(el_span)
+        el_pre.text(el.text().replace('\n', ''))
+        el_pre.attr('style', el.attr('style'))
+        el.replace_with(el_pre)
+
+def process_el_heading(rt):
+    def get_font_size(el):
+        style = el.attr('style') or ''
+        m = re.search(r'font-size:\s*(\d+\.\d+)', style)
+        if not m: return 0
+        else: return float(m.group(1))
+    el_paras = rt('p')
+    for el in el_paras:
+        el = pq(el)
+        # 如果字体大于等于 16，则认为它是标题
+        el_spans = el.find('span')
+        is_heading = (
+            get_font_size(el) >= 16 or
+            any([get_font_size(pq(el)) >= 16 for el in el_spans])
+        )
+        if not is_heading: continue
+        el_h2 = rt('<h2></h2>')
+        el_h2.html(el.html() or '')
+        el_h2.attr('style', el.attr('style'))
+        el.replace_with(el_h2)
+
+def process_pre_indent(rt):
+    def get_indent(el):
+        style = el.attr('style') or ''
+        m = re.search(r'left:\s*(\d+\.\d+)', style)
+        if not m: return 0
+        else: return float(m.group(1))
+    inds = [get_indent(pq(el)) for el in rt('pre')]
+    inds_uni = list({x for x in inds if x != 0})
+    inds_uni.sort()
+    if len(inds_uni) <= 1: return
+    # 计算基址和偏移，转换为空格数
+    diff = inds_uni[1] - inds_uni[0]
+    base = inds_uni[0]
+    for i, el in enumerate(rt('pre')):
+        if inds[i] == 0: continue
+        nspace = int((inds[i] - base) // diff) * 4
+        el = pq(el)
+        el.text(' ' * nspace + (el.text() or ''))
+
+
+def process_html_code(html):
+    rt = pq(html)
+    process_el_code(rt)
+    # process_el_pre(rt)
+    process_pre_indent(rt)
+    process_el_heading(rt)
+    # 处理缩进
+    html = rt('body').html() if rt('body') else str(rt)
+    # 合并连续的 PRE
+    # html = re.sub(r'</pre>\s*<pre[^>]*>', '\n', html)
+    # 合并段落内的换行
+    # html = re.sub(r'(?<![\.\?!:])</p>\s*<p [^>]*>', ' ', html)
+    # html = re.sub(r'</?span[^>]*>', '' ,html)
+    # html = re.sub(r'style=".+?"', '' ,html)
+    return html
+
+def pdf2html_file(args):
+    fname, dir = args.fname, args.dir
+    if not fname.endswith('.pdf'):
+        print('请提供 PDF 文件')
+        return
+    print(f'file: {fname}')
+    title = path.basename(fname)[:-4]
+    doc = fitz.open(fname)
+    lp = len(str(len(doc)))
+    for ip, p in enumerate(doc):
+        print(f'page: {ip + 1}')
+        html = process_html_code(p.get_text("html"))
+        # html = (p.get_text("html"))
+        html_fname = path.join(dir, f'{title}_{ip+1:0{lp}d}.html')
+        print(f'save: {html_fname}')
+        open(html_fname, 'w', encoding='utf8').write(html)
+
+    doc.close()
+
+def pdf2html_dir(args):
+    dir = args.fname
+    for fname in os.listdir(dir):
+        try:
+            ffname = path.join(dir, fname)
+            args.fname = ffname
+            pdf2html_file(args)
+        except: traceback.print_exc()
+
+def pdf2html(args):
+    if path.isdir(args.fname):
+        pdf2html_dir(args)
+    else:
+        pdf2html_file(args)
+
+
+def ext_pdf(args):
+    if path.isdir(args.fname):
+        ext_pdf_dir(args)
+    else:
+        ext_pdf_file(args)
+
+def ext_pdf_dir(args):
+    dir = args.fname
+    for fname in os.listdir(dir):
+        try:
+            ffname = path.join(dir, fname)
+            args.fname = ffname
+            ext_pdf_file(args)
+        except: traceback.print_exc()
+
+def ext_pdf_file(args):
+    fname, dir = args.fname, args.dir
+    if not fname.endswith('.pdf'):
+        print('请提供 PDF 文件')
+        return
+    print(f'file: {fname}')
+    title = path.basename(fname)[:-4]
+
+    doc = fitz.open(fname)
+    lp = len(str(len(doc)))
+    for ip, p in enumerate(doc):
+        print(f'page: {ip + 1}')
+        
+        # 判断是否整页截图
+        if args.whole:
+            img = p.get_pixmap(dpi=400)
+            imgname = path.join(dir, f'{title}_{ip+1:0{lp}d}.png')
+            print(f'save: {imgname}')
+            img.save(imgname)
+            continue
+        
+        imgs = p.get_images()
+        limg = len(str(len(imgs)))
+        for ii, info in enumerate(imgs):
+            xref = info[0]
+            print(f'img: {ii + 1}, xref: {xref}')
+            img = fitz.Pixmap(doc, xref)
+            imgname = path.join(dir, f'{title}_{ip+1:0{lp}d}_{ii+1:0{limg}d}.png')
+            print(f'save: {imgname}')
+            img.save(imgname)
+    
+    doc.close()
+
+def get_scale_by_width(wid):
+    if wid < 800:
+        return 4
+    elif wid < 900:
+        return 3.5
+    elif wid < 1000:
+        return 3
+    elif wid < 1200:
+        return 2.5
+    elif wid < 1600:
+        return 2
+    elif wid < 2000:
+        return 1.5
+    elif wid < 3200:
+        return 1
+    elif wid < 4200:
+        return 0.75
+    else:
+        return 0.5
+
+def pack_pdf(args):
+    dir, rgx = args.dir, args.regex
+    if dir.endswith('/') or \
+        dir.endswith('\\'):
+        dir = dir[:-1]
+    
+    fnames = filter(is_pic, os.listdir(dir))
+    if not rgx:
+        fnames = [path.join(dir, f) for f in fnames]
+        pdf = img2pdf.convert(fnames)
+        fname = dir + '.pdf'
+        print(fname)
+        open(fname, 'wb').write(pdf)
+        return
+        
+    d = {}
+    for fname in fnames:
+        m = re.search(rgx, fname)
+        if not m: continue
+        kw = m.group(0)
+        d.setdefault(kw, [])
+        d[kw].append(fname)
+        
+    for kw, fnames in d.items():
+        fnames = [path.join(dir, f) for f in fnames]
+        pdf = img2pdf.convert(fnames)
+        fname = path.join(dir, kw + '.pdf')
+        print(fname)
+        open(fname, 'wb').write(pdf)
+
+def office2pdf(fname, ofname):
+    import win32com.client
+    m = re.search(r'\.(\w+)$', fname)
+    ext = m.group(1) if m else ""
+    if ext not in app_map:
+        raise FileError(f'{fname} 不是 DOC、XLS 或 PPT 文件')
+    app = win32com.client.Dispatch(app_map[ext][0])
+    ppt = getattr(app, app_map[ext][1]).Open(fname)
+    ppt.SaveAs(ofname, 32)
+    app.Quit()
+    
+def office2pdf_file(args):
+    fname = args.fname
+    print(fname)
+    m = re.search(r'\.(\w+)$', fname)
+    ext = m.group(1) if m else ""
+    if ext not in app_map:
+        print('请提供 DOC、XLS 或 PPT 文件')
+        return
+    fname = path.join(os.getcwd(), fname)
+    ofname = re.sub(r'\.\w+$', '', fname) + '.pdf'
+    office2pdf(fname, ofname)
+    print("转换成功！")
+
+def office2pdf_dir(args):
+    dir = args.fname
+    fnames = os.listdir(dir)
+    for f in fnames:
+        ff = path.join(dir, f)
+        args.fname = ff
+        try: office2pdf_file(args)
+        except Exception as ex: traceback.print_exc()
+
+# @safe()
+def waifu2x_auto_file(args):
+    fname = args.fname
+    if not is_pic(fname):
+        print('请提供图像')
+        return
+    print(fname)
+    try: img = Image.open(fname)
+    except: 
+        print('文件无法打开')
+        return
+    width = min(img.size[0], img.size[1])
+    scale = get_scale_by_width(width)
+    img.close()
+    p = find_cmd_path('waifu2x-converter-cpp')
+    cmd = [
+        'waifu2x-converter-cpp', 
+        '-m', 'noise-scale',
+        '--noise-level', '2',
+        '--scale-ratio', str(scale),
+        '--block-size', '256',
+        '-i', fname,
+        '-o', fname,
+        '--model-dir', path.join(p, 'models_rgb'),
+        '--disable-gpu',
+    ]
+    print(f'cmd: {cmd}')
+    r = subp.Popen(
+        cmd, 
+        shell=True,
+        stdout=subp.PIPE,
+        stderr=subp.PIPE,
+    ).communicate()
+    open(fname, 'ab').close() # touch
+    print(r[0].decode('utf8', 'ignore') or 
+        r[1].decode('utf8', 'ignore'))
+
+def waifu2x_auto_dir(args):
+    dir = args.fname
+    fnames = os.listdir(dir)
+    pool = Pool(args.threads)
+    for f in fnames:
+        ff = path.join(dir, f)
+        args = copy.deepcopy(args)
+        args.fname = ff
+        pool.apply_async(waifu2x_auto_file, [args])
+    pool.close()
+    pool.join()
+    
+def waifu2x_auto_handle(args):
+    # 检查 waifu2x
+    if not find_cmd_path('waifu2x-converter-cpp'): 
+        print('waifu2x-converter-cpp 未找到，请下载并将其目录添加到系统变量 PATH 中')
+        return
+    if path.isdir(args.fname):
+        waifu2x_auto_dir(args)
+    else:
+        waifu2x_auto_file(args)
+        
+def office2pdf_handle(args):
+    if path.isdir(args.fname):
+        office2pdf_dir(args)
+    else:
+        office2pdf_file(args)
+
+# @safe()
+def anime4k_auto_file(args):
+    fname = args.fname
+    if not is_pic(fname):
+        print('请提供图像')
+        return
+    print(fname)
+    try: img = Image.open(fname)
+    except: 
+        print('文件无法打开')
+        return
+    width = min(img.size[0], img.size[1])
+    scale = get_scale_by_width(width)
+    img.close()
+    cmd = [
+        'Anime4KCPP_CLI', 
+        '-t', str(args.threads),
+        '-z', str(scale),
+        '-i', fname,
+        '-o', fname,
+        "-w", "-H",
+        "-L", "3",
+    ]
+    if args.gpu: cmd.append('-q')
+    print(f'cmd: {cmd}')
+    r = subp.Popen(
+        cmd, 
+        shell=True,
+        stdout=subp.PIPE,
+        stderr=subp.PIPE,
+        cwd=find_cmd_path('Anime4KCPP_CLI'),
+    ).communicate()
+    open(fname, 'ab').close() # touch
+    print(r[0].decode('utf8', 'ignore') or 
+        r[1].decode('utf8', 'ignore'))
+        
+def anime4k_auto_dir(args):
+    dir = args.fname
+    fnames = os.listdir(dir)
+    for f in fnames:
+        ff = path.join(dir, f)
+        args.fname = ff
+        anime4k_auto_file(args)
+
+def anime4k_auto_handle(args):
+    # 检查 waifu2x
+    if not find_cmd_path('Anime4KCPP_CLI'): 
+        print('Anime4KCPP_CLI 未找到，请下载并将其目录添加到系统变量 PATH 中')
+        return
+    if path.isdir(args.fname):
+        anime4k_auto_dir(args)
+    else:
+        anime4k_auto_file(args)
+
+# @safe()
+def pdf_auto_file(args):
+    fname = args.fname
+    threads = args.threads
+    if not fname.endswith('.pdf'):
+        print('请提供 PDF 文件')
+        return
+    print(f'file: {fname}')
+    tmpdir = path.join(tempfile.gettempdir(), uuid.uuid4().hex)
+    safe_mkdir(tmpdir)
+    
+    cmds = [
+        ['wiki-tool', 'ext-pdf', '-d', tmpdir, fname],
+        ['wiki-tool', 'tog-bw', '-t', str(threads), tmpdir],
+        ['wiki-tool', 'anime4k-auto', '-t', str(threads), tmpdir],
+        ['imgyaso', '-m', 'thres', '-t', str(threads), tmpdir],
+        ['wiki-tool', 'pack-pdf', tmpdir],
+    ]
+    if args.gpu: cmds[2].append('-G')
+    if args.whole: cmds[0].append('-w')
+    for cmd in cmds:
+        subp.Popen(cmd, shell=True).communicate()
+    if path.isfile(fname + '.bak'): os.unlink(fname + '.bak')
+    shutil.move(fname, fname + '.bak')
+    shutil.move(path.abspath(tmpdir) + '.pdf', fname)
+    
+    safe_rmdir(tmpdir)
+    
+def pdf_auto_dir(args):
+    dir = args.fname
+    fnames = os.listdir(dir)
+    for f in fnames:
+        ff = path.join(dir, f)
+        args.fname = ff
+        pdf_auto_file(args)
+
+
+def pdf_auto_handle(args):
+    if path.isdir(args.fname):
+        pdf_auto_dir(args)
+    else:
+        pdf_auto_file(args)
+
+def pg_all_imgs_area(pg):
+    rects = [
+        pg.get_image_rects(info[0])
+        for info in pg.get_images()
+    ]
+    rects = [r[0] for r in rects if r]
+    return sum([(r[2] - r[0]) * (r[3] - r[1]) for r in rects])
+
+def pg_area(pg):
+    return (pg.rect[2] - pg.rect[0]) * (pg.rect[3] - pg.rect[1])
+
+def is_scanned_pdf(fname, imgs_area_rate=0.8, scanned_pg_rate=0.8):
+    doc = fitz.open("pdf", open(fname, 'rb').read())
+    rate = sum([
+        pg_all_imgs_area(pg) >= pg_area(pg) * imgs_area_rate
+        for pg in doc
+    ]) / len(doc)
+    return rate >= scanned_pg_rate
+    
+# @safe()
+def tr_pick_scanned_pdf(fname, odirs, imgs_area_rate, scanned_pg_rate):
+    scanned = is_scanned_pdf(
+        fname, 
+        imgs_area_rate=imgs_area_rate, 
+        scanned_pg_rate=scanned_pg_rate,
+    )
+    rtext = '扫描版' if scanned else '文字版'
+    print(f'{fname}：{rtext}')
+    if scanned:
+        shutil.move(fname, path.join(odirs[0], path.basename(fname)))
+    else:
+        shutil.move(fname, path.join(odirs[1], path.basename(fname)))
+    
+def pick_scanned_pdf(args):
+    dir = args.dir
+    if not path.isdir(dir):
+        print('请提供目录')
+        return
+    odir0 = path.join(dir, '扫描版')
+    odir1 = path.join(dir, '文字版')
+    safe_mkdir(odir0)
+    safe_mkdir(odir1)
+    pool = Pool(args.threads)
+    for f in os.listdir(dir):
+        if not f.endswith('.pdf'):
+            continue
+        ff = path.join(dir, f)
+        pool.apply_async(
+            tr_pick_scanned_pdf, 
+            [
+                ff, [odir0, odir1], 
+                args.imgs_area_rate, 
+                args.scanned_pg_rate
+            ]
+        )
+    pool.close()
+    pool.join()
+
```

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool/pdg_tool.py` & `BookerWikiTool-2023.3.30.0/BookerWikiTool/pdg_tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 from os import path
-from pywinauto.application import Application
-from pywinauto.keyboard import send_keys
 from time import sleep
 
 def pdg2pdf(args):
+    from pywinauto.application import Application
+    from pywinauto.keyboard import send_keys
+    
     dir = args.dir
     if not path.isdir(dir):
         print('请提供目录')
         return
     fnames = os.listdir(dir)
     has_pdg = any([f.endswith('.pdg') for f in fnames])
     if not has_pdg:
```

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool/tomd.js` & `BookerWikiTool-2023.3.30.0/BookerWikiTool/tomd.js`

 * *Files identical despite different names*

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool/util.py` & `BookerWikiTool-2023.3.30.0/BookerWikiTool/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,264 +1,292 @@
-00000000: 696d 706f 7274 2074 656d 7066 696c 650a  import tempfile.
-00000010: 696d 706f 7274 2075 7569 640a 696d 706f  import uuid.impo
-00000020: 7274 2073 7562 7072 6f63 6573 7320 6173  rt subprocess as
-00000030: 2073 7562 700a 696d 706f 7274 2072 650a   subp.import re.
-00000040: 696d 706f 7274 206f 730a 696d 706f 7274  import os.import
-00000050: 2073 6875 7469 6c0a 696d 706f 7274 206a   shutil.import j
-00000060: 736f 6e0a 696d 706f 7274 2079 616d 6c0a  son.import yaml.
-00000070: 6672 6f6d 2066 756e 6374 6f6f 6c73 2069  from functools i
-00000080: 6d70 6f72 7420 7265 6475 6365 0a66 726f  mport reduce.fro
-00000090: 6d20 7572 6c6c 6962 2e70 6172 7365 2069  m urllib.parse i
-000000a0: 6d70 6f72 7420 7175 6f74 655f 706c 7573  mport quote_plus
-000000b0: 0a66 726f 6d20 6f73 2069 6d70 6f72 7420  .from os import 
-000000c0: 7061 7468 0a66 726f 6d20 7079 7175 6572  path.from pyquer
-000000d0: 7920 696d 706f 7274 2050 7951 7565 7279  y import PyQuery
-000000e0: 2061 7320 7071 0a66 726f 6d20 6461 7465   as pq.from date
-000000f0: 7469 6d65 2069 6d70 6f72 7420 6461 7465  time import date
-00000100: 7469 6d65 0a66 726f 6d20 636f 6c6c 6563  time.from collec
-00000110: 7469 6f6e 7320 696d 706f 7274 204f 7264  tions import Ord
-00000120: 6572 6564 4469 6374 0a69 6d70 6f72 7420  eredDict.import 
-00000130: 696d 6779 6173 6f0a 0a52 455f 5941 4d4c  imgyaso..RE_YAML
-00000140: 5f4d 4554 4120 3d20 7227 3c21 2d2d 796d  _META = r'<!--ym
-00000150: 6c28 5b5c 735c 535d 2b3f 292d 2d3e 270a  l([\s\S]+?)-->'.
-00000160: 5245 5f54 4954 4c45 203d 2072 275e 232b  RE_TITLE = r'^#+
-00000170: 2028 2e2b 3f29 2427 0a52 455f 534f 5552   (.+?)$'.RE_SOUR
-00000180: 4345 203d 2072 272f 285b 5e2f 5c6e 5d2b  CE = r'/([^/\n]+
-00000190: 3f29 2f3f 3e27 0a52 455f 434f 4445 5f42  ?)/?>'.RE_CODE_B
-000001a0: 4c4f 434b 203d 2072 2760 6060 5b5c 735c  LOCK = r'```[\s\
-000001b0: 535d 2b3f 6060 6027 0a52 455f 494d 4720  S]+?```'.RE_IMG 
-000001c0: 3d20 7227 215c 5b2e 2a3f 5c5d 5c28 2e2a  = r'!\[.*?\]\(.*
-000001d0: 3f5c 2927 0a23 2057 6f72 6420 e5ad 97e6  ?\)'.# Word ....
-000001e0: 95b0 e7bb 9fe8 aea1 e6a0 87e5 8786 efbc  ................
-000001f0: 9a0a 2320 e4b8 80e4 b8aa e6b1 89e5 ad97  ..# ............
-00000200: e688 96e4 b8ad e696 87e6 a087 e782 b9e7  ................
-00000210: ae97 e4b8 80e4 b8aa e5ad 970a 2320 e4b8  ............# ..
-00000220: 80e4 b8aa e8bf 9ee7 bbad e79a 84e8 8bb1  ................
-00000230: e696 87e5 ad97 e6af 8de3 8081 e6a0 87e7  ................
-00000240: 82b9 e592 8ce6 95b0 e5ad 97e5 ba8f e588  ................
-00000250: 97e7 ae97 e4b8 80e4 b8aa e5ad 970a 5245  ..............RE
-00000260: 5f5a 485f 574f 5244 203d 2072 275b 5c75  _ZH_WORD = r'[\u
-00000270: 3230 3138 2d5c 7532 3031 645c 7533 3030  2018-\u201d\u300
-00000280: 312d 5c75 3330 3163 5c75 3465 3030 2d5c  1-\u301c\u4e00-\
-00000290: 7539 6666 665c 7566 6630 312d 5c75 6666  u9fff\uff01-\uff
-000002a0: 3635 5d27 0a52 455f 454e 5f57 4f52 4420  65]'.RE_EN_WORD 
-000002b0: 3d20 7227 5b5c 7832 312d 5c78 3765 5d2b  = r'[\x21-\x7e]+
-000002c0: 270a 5245 5f49 4652 414d 4520 3d20 7227  '.RE_IFRAME = r'
-000002d0: 3c69 6672 616d 655b 5e3e 5d2a 7372 633d  <iframe[^>]*src=
-000002e0: 2228 2e2b 3f29 225b 5e3e 5d2a 3e27 0a52  "(.+?)"[^>]*>'.R
-000002f0: 455f 4946 5241 4d45 5f41 4c4c 203d 2072  E_IFRAME_ALL = r
-00000300: 273c 2f3f 6966 7261 6d65 5b5e 3e5d 2a3e  '</?iframe[^>]*>
-00000310: 270a 5245 5f49 4652 414d 455f 5245 504c  '.RE_IFRAME_REPL
-00000320: 203d 2072 273c 6272 2f3e 3c62 722f 3e3c   = r'<br/><br/><
-00000330: 6120 6872 6566 3d22 5c31 223e 5c31 3c2f  a href="\1">\1</
-00000340: 613e 3c62 722f 3e3c 6272 2f3e 270a 0a44  a><br/><br/>'..D
-00000350: 4952 203d 2070 6174 682e 6469 726e 616d  IR = path.dirnam
-00000360: 6528 7061 7468 2e61 6273 7061 7468 285f  e(path.abspath(_
-00000370: 5f66 696c 655f 5f29 290a 0a64 6566 6175  _file__))..defau
-00000380: 6c74 5f68 6472 7320 3d20 7b0a 2020 2020  lt_hdrs = {.    
-00000390: 2755 7365 722d 4167 656e 7427 3a20 274d  'User-Agent': 'M
-000003a0: 6f7a 696c 6c61 2f35 2e30 2028 5769 6e64  ozilla/5.0 (Wind
-000003b0: 6f77 7320 4e54 2031 302e 303b 2057 696e  ows NT 10.0; Win
-000003c0: 3634 3b20 7836 3429 2041 7070 6c65 5765  64; x64) AppleWe
-000003d0: 624b 6974 2f35 3337 2e33 3620 284b 4854  bKit/537.36 (KHT
-000003e0: 4d4c 2c20 6c69 6b65 2047 6563 6b6f 2920  ML, like Gecko) 
-000003f0: 4368 726f 6d65 2f38 302e 302e 3339 3837  Chrome/80.0.3987
-00000400: 2e31 3332 2053 6166 6172 692f 3533 372e  .132 Safari/537.
-00000410: 3336 272c 0a7d 0a0a 6865 6164 6572 7320  36',.}..headers 
-00000420: 3d20 7b0a 2020 2020 2755 7365 722d 4167  = {.    'User-Ag
-00000430: 656e 7427 3a20 2750 6f73 746d 616e 5275  ent': 'PostmanRu
-00000440: 6e74 696d 652f 372e 3236 2e38 272c 0a20  ntime/7.26.8',. 
-00000450: 2020 2027 5265 6665 7265 7227 3a20 2768     'Referer': 'h
-00000460: 7474 7073 3a2f 2f77 7777 2e62 696c 6962  ttps://www.bilib
-00000470: 696c 692e 636f 6d2f 272c 0a7d 0a0a 0a64  ili.com/',.}...d
-00000480: 6566 2064 286e 616d 6529 3a0a 2020 2020  ef d(name):.    
-00000490: 7265 7475 726e 2070 6174 682e 6a6f 696e  return path.join
-000004a0: 2844 4952 2c20 6e61 6d65 290a 0a64 6566  (DIR, name)..def
-000004b0: 2061 7373 6574 286e 616d 653d 2727 293a   asset(name=''):
-000004c0: 0a20 2020 2072 6574 7572 6e20 7061 7468  .    return path
-000004d0: 2e6a 6f69 6e28 4449 522c 2027 6173 7365  .join(DIR, 'asse
-000004e0: 7473 272c 206e 616d 6529 0a0a 6465 6620  ts', name)..def 
-000004f0: 6f70 7469 5f69 6d67 2869 6d67 2c20 6d6f  opti_img(img, mo
-00000500: 6465 2c20 636f 6c6f 7273 293a 0a20 2020  de, colors):.   
-00000510: 2069 6620 6d6f 6465 203d 3d20 2771 7561   if mode == 'qua
-00000520: 6e74 273a 0a20 2020 2020 2020 2072 6574  nt':.        ret
-00000530: 7572 6e20 696d 6779 6173 6f2e 706e 6771  urn imgyaso.pngq
-00000540: 7561 6e74 5f62 7473 2869 6d67 2c20 636f  uant_bts(img, co
-00000550: 6c6f 7273 290a 2020 2020 656c 6966 206d  lors).    elif m
-00000560: 6f64 6520 3d3d 2027 6772 6964 273a 0a20  ode == 'grid':. 
-00000570: 2020 2020 2020 2072 6574 7572 6e20 696d         return im
-00000580: 6779 6173 6f2e 6772 6964 5f62 7473 2869  gyaso.grid_bts(i
-00000590: 6d67 290a 2020 2020 656c 6966 206d 6f64  mg).    elif mod
-000005a0: 6520 3d3d 2027 7472 756e 6327 3a0a 2020  e == 'trunc':.  
-000005b0: 2020 2020 2020 7265 7475 726e 2069 6d67        return img
-000005c0: 7961 736f 2e74 7275 6e63 5f62 7473 2869  yaso.trunc_bts(i
-000005d0: 6d67 2c20 636f 6c6f 7273 290a 2020 2020  mg, colors).    
-000005e0: 656c 6966 206d 6f64 6520 3d3d 2027 7468  elif mode == 'th
-000005f0: 7265 7327 3a0a 2020 2020 2020 2020 7265  res':.        re
-00000600: 7475 726e 2069 6d67 7961 736f 2e61 6461  turn imgyaso.ada
-00000610: 7468 7265 735f 6274 7328 696d 6729 0a20  thres_bts(img). 
-00000620: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00000630: 2072 6574 7572 6e20 696d 670a 0a64 6566   return img..def
-00000640: 2074 6f6d 6428 6874 6d6c 293a 0a20 2020   tomd(html):.   
-00000650: 2023 20e5 a484 e790 8620 4946 5241 4d45   # ...... IFRAME
-00000660: 0a20 2020 2068 746d 6c20 3d20 7265 2e73  .    html = re.s
-00000670: 7562 2852 455f 4946 5241 4d45 2c20 5245  ub(RE_IFRAME, RE
-00000680: 5f49 4652 414d 455f 5245 504c 2c20 6874  _IFRAME_REPL, ht
-00000690: 6d6c 290a 2020 2020 6874 6d6c 203d 2072  ml).    html = r
-000006a0: 652e 7375 6228 5245 5f49 4652 414d 455f  e.sub(RE_IFRAME_
-000006b0: 414c 4c2c 2027 272c 2068 746d 6c29 0a20  ALL, '', html). 
-000006c0: 2020 206a 735f 666e 616d 6520 3d20 6428     js_fname = d(
-000006d0: 2774 6f6d 642e 6a73 2729 0a20 2020 2068  'tomd.js').    h
-000006e0: 746d 6c5f 666e 616d 6520 3d20 7061 7468  tml_fname = path
-000006f0: 2e6a 6f69 6e28 7465 6d70 6669 6c65 2e67  .join(tempfile.g
-00000700: 6574 7465 6d70 6469 7228 292c 2075 7569  ettempdir(), uui
-00000710: 642e 7575 6964 3428 292e 6865 7820 2b20  d.uuid4().hex + 
-00000720: 272e 6874 6d6c 2729 0a20 2020 206f 7065  '.html').    ope
-00000730: 6e28 6874 6d6c 5f66 6e61 6d65 2c20 2777  n(html_fname, 'w
-00000740: 272c 2065 6e63 6f64 696e 673d 2775 7466  ', encoding='utf
-00000750: 3827 292e 7772 6974 6528 6874 6d6c 290a  8').write(html).
-00000760: 2020 2020 7375 6270 2e50 6f70 656e 280a      subp.Popen(.
-00000770: 2020 2020 2020 2020 5b22 6e6f 6465 222c          ["node",
-00000780: 206a 735f 666e 616d 652c 2068 746d 6c5f   js_fname, html_
-00000790: 666e 616d 655d 2c0a 2020 2020 2020 2020  fname],.        
-000007a0: 7368 656c 6c3d 5472 7565 2c0a 2020 2020  shell=True,.    
-000007b0: 292e 636f 6d6d 756e 6963 6174 6528 290a  ).communicate().
-000007c0: 2020 2020 6d64 5f66 6e61 6d65 203d 2072      md_fname = r
-000007d0: 652e 7375 6228 7227 5c2e 6874 6d6c 2427  e.sub(r'\.html$'
-000007e0: 2c20 2727 2c20 6874 6d6c 5f66 6e61 6d65  , '', html_fname
-000007f0: 2920 2b20 272e 6d64 270a 2020 2020 6d64  ) + '.md'.    md
-00000800: 203d 206f 7065 6e28 6d64 5f66 6e61 6d65   = open(md_fname
-00000810: 2c20 656e 636f 6469 6e67 3d27 7574 6638  , encoding='utf8
-00000820: 2729 2e72 6561 6428 290a 2020 2020 6f73  ').read().    os
-00000830: 2e72 656d 6f76 6528 6874 6d6c 5f66 6e61  .remove(html_fna
-00000840: 6d65 290a 2020 2020 7265 7475 726e 206d  me).    return m
-00000850: 640a 0a64 6566 2066 6e61 6d65 5f65 7363  d..def fname_esc
-00000860: 6170 6528 6e61 6d65 293a 0a20 2020 2072  ape(name):.    r
-00000870: 6574 7572 6e20 6e61 6d65 2e72 6570 6c61  eturn name.repla
-00000880: 6365 2827 5c5c 272c 2027 efbc bc27 2920  ce('\\', '...') 
-00000890: 5c0a 2020 2020 2020 2020 2020 2020 2020  \.              
-000008a0: 202e 7265 706c 6163 6528 272f 272c 2027   .replace('/', '
-000008b0: efbc 8f27 2920 5c0a 2020 2020 2020 2020  ...') \.        
-000008c0: 2020 2020 2020 202e 7265 706c 6163 6528         .replace(
-000008d0: 273a 272c 2027 efbc 9a27 2920 5c0a 2020  ':', '...') \.  
-000008e0: 2020 2020 2020 2020 2020 2020 202e 7265               .re
-000008f0: 706c 6163 6528 272a 272c 2027 efbc 8a27  place('*', '...'
-00000900: 2920 5c0a 2020 2020 2020 2020 2020 2020  ) \.            
-00000910: 2020 202e 7265 706c 6163 6528 273f 272c     .replace('?',
-00000920: 2027 efbc 9f27 2920 5c0a 2020 2020 2020   '...') \.      
-00000930: 2020 2020 2020 2020 202e 7265 706c 6163           .replac
-00000940: 6528 2722 272c 2027 efbc 8227 2920 5c0a  e('"', '...') \.
-00000950: 2020 2020 2020 2020 2020 2020 2020 202e                 .
-00000960: 7265 706c 6163 6528 273c 272c 2027 efbc  replace('<', '..
-00000970: 9c27 2920 5c0a 2020 2020 2020 2020 2020  .') \.          
-00000980: 2020 2020 202e 7265 706c 6163 6528 273e       .replace('>
-00000990: 272c 2027 efbc 9e27 2920 5c0a 2020 2020  ', '...') \.    
-000009a0: 2020 2020 2020 2020 2020 202e 7265 706c             .repl
-000009b0: 6163 6528 277c 272c 2027 efbd 9c27 290a  ace('|', '...').
-000009c0: 2020 2020 2020 2020 2020 2020 2020 200a                 .
-000009d0: 6465 6620 6163 636f 756e 745f 776f 7264  def account_word
-000009e0: 7328 636f 6e74 293a 0a20 2020 2023 20e5  s(cont):.    # .
-000009f0: 8ebb e68e 89e4 bba3 e7a0 81e5 9d97 e592  ................
-00000a00: 8ce5 9bbe e789 870a 2020 2020 636f 6e74  ........    cont
-00000a10: 203d 2072 652e 7375 6228 5245 5f43 4f44   = re.sub(RE_COD
-00000a20: 455f 424c 4f43 4b2c 2027 272c 2063 6f6e  E_BLOCK, '', con
-00000a30: 7429 0a20 2020 2063 6f6e 7420 3d20 7265  t).    cont = re
-00000a40: 2e73 7562 2852 455f 494d 472c 2027 272c  .sub(RE_IMG, '',
-00000a50: 2063 6f6e 7429 0a20 2020 207a 685f 636f   cont).    zh_co
-00000a60: 756e 7420 3d20 6c65 6e28 7265 2e66 696e  unt = len(re.fin
-00000a70: 6461 6c6c 2852 455f 5a48 5f57 4f52 442c  dall(RE_ZH_WORD,
-00000a80: 2063 6f6e 7429 290a 2020 2020 656e 5f63   cont)).    en_c
-00000a90: 6f75 6e74 203d 206c 656e 2872 652e 6669  ount = len(re.fi
-00000aa0: 6e64 616c 6c28 5245 5f45 4e5f 574f 5244  ndall(RE_EN_WORD
-00000ab0: 2c20 636f 6e74 2929 0a20 2020 2074 6f74  , cont)).    tot
-00000ac0: 616c 203d 207a 685f 636f 756e 7420 2b20  al = zh_count + 
-00000ad0: 656e 5f63 6f75 6e74 0a20 2020 2072 6574  en_count.    ret
-00000ae0: 7572 6e20 2874 6f74 616c 2c20 7a68 5f63  urn (total, zh_c
-00000af0: 6f75 6e74 2c20 656e 5f63 6f75 6e74 290a  ount, en_count).
-00000b00: 2020 2020 0a64 6566 2073 6166 655f 6d6b      .def safe_mk
-00000b10: 6469 7228 6469 7229 3a0a 2020 2020 7472  dir(dir):.    tr
-00000b20: 793a 206f 732e 6d61 6b65 6469 7273 2864  y: os.makedirs(d
-00000b30: 6972 290a 2020 2020 6578 6365 7074 3a20  ir).    except: 
-00000b40: 7061 7373 0a20 2020 200a 6465 6620 7361  pass.    .def sa
-00000b50: 6665 5f72 6d64 6972 2864 6972 293a 0a20  fe_rmdir(dir):. 
-00000b60: 2020 2074 7279 3a20 7368 7574 696c 2e72     try: shutil.r
-00000b70: 6d74 7265 6528 6469 7229 0a20 2020 2065  mtree(dir).    e
-00000b80: 7863 6570 743a 2070 6173 730a 0a64 6566  xcept: pass..def
-00000b90: 2069 735f 635f 7374 796c 655f 636f 6465   is_c_style_code
-00000ba0: 2866 6e61 6d65 293a 0a20 2020 2065 7874  (fname):.    ext
-00000bb0: 203d 205b 0a20 2020 2020 2020 2027 6327   = [.        'c'
-00000bc0: 2c20 2763 7070 272c 2027 6378 7827 2c20  , 'cpp', 'cxx', 
-00000bd0: 2768 272c 2027 6870 7027 2c0a 2020 2020  'h', 'hpp',.    
-00000be0: 2020 2020 276a 6176 6127 2c20 276b 7427      'java', 'kt'
-00000bf0: 2c20 2773 6361 6c61 272c 200a 2020 2020  , 'scala', .    
-00000c00: 2020 2020 2763 7327 2c20 276a 7327 2c20      'cs', 'js', 
-00000c10: 276a 736f 6e27 2c20 2774 7327 2c20 0a20  'json', 'ts', . 
-00000c20: 2020 2020 2020 2027 7068 7027 2c20 2767         'php', 'g
-00000c30: 6f27 2c20 2772 7573 7427 2c20 2773 7769  o', 'rust', 'swi
-00000c40: 6674 272c 0a20 2020 205d 0a20 2020 206d  ft',.    ].    m
-00000c50: 203d 2072 652e 7365 6172 6368 2872 275c   = re.search(r'\
-00000c60: 2e28 5c77 2b29 2427 2c20 666e 616d 6529  .(\w+)$', fname)
-00000c70: 0a20 2020 2072 6574 7572 6e20 626f 6f6c  .    return bool
-00000c80: 286d 2061 6e64 206d 2e67 726f 7570 2831  (m and m.group(1
-00000c90: 2920 696e 2065 7874 290a 0a64 6566 2069  ) in ext)..def i
-00000ca0: 735f 7069 6328 666e 616d 6529 3a0a 2020  s_pic(fname):.  
-00000cb0: 2020 6578 7420 3d20 5b0a 2020 2020 2020    ext = [.      
-00000cc0: 2020 276a 7067 272c 2027 6a70 6567 272c    'jpg', 'jpeg',
-00000cd0: 2027 6a66 6966 272c 2027 706e 6727 2c20   'jfif', 'png', 
-00000ce0: 0a20 2020 2020 2020 2027 6769 6627 2c20  .        'gif', 
-00000cf0: 2774 6966 6627 2c20 2777 6562 7027 0a20  'tiff', 'webp'. 
-00000d00: 2020 205d 0a20 2020 206d 203d 2072 652e     ].    m = re.
-00000d10: 7365 6172 6368 2872 275c 2e28 5c77 2b29  search(r'\.(\w+)
-00000d20: 2427 2c20 666e 616d 6529 0a20 2020 2072  $', fname).    r
-00000d30: 6574 7572 6e20 626f 6f6c 286d 2061 6e64  eturn bool(m and
-00000d40: 206d 2e67 726f 7570 2831 2920 696e 2065   m.group(1) in e
-00000d50: 7874 290a 0a64 6566 2066 696e 645f 636d  xt)..def find_cm
-00000d60: 645f 7061 7468 286e 616d 6529 3a0a 2020  d_path(name):.  
-00000d70: 2020 666f 7220 7020 696e 206f 732e 656e    for p in os.en
-00000d80: 7669 726f 6e2e 6765 7428 2750 4154 4827  viron.get('PATH'
-00000d90: 2c20 2727 292e 7370 6c69 7428 273b 2729  , '').split(';')
-00000da0: 3a0a 2020 2020 2020 2020 6966 2070 6174  :.        if pat
-00000db0: 682e 6973 6669 6c65 2870 6174 682e 6a6f  h.isfile(path.jo
-00000dc0: 696e 2870 2c20 6e61 6d65 2929 206f 7220  in(p, name)) or 
-00000dd0: 5c0a 2020 2020 2020 2020 2020 2020 7061  \.            pa
-00000de0: 7468 2e69 7366 696c 6528 7061 7468 2e6a  th.isfile(path.j
-00000df0: 6f69 6e28 702c 206e 616d 6520 2b20 272e  oin(p, name + '.
-00000e00: 6578 6527 2929 3a0a 2020 2020 2020 2020  exe')):.        
-00000e10: 2020 2020 7265 7475 726e 2070 0a20 2020      return p.   
-00000e20: 2072 6574 7572 6e20 2727 0a20 2020 200a   return ''.    .
-00000e30: 6465 6620 6973 5f76 6964 656f 2866 6e61  def is_video(fna
-00000e40: 6d65 293a 0a20 2020 2065 7874 203d 205b  me):.    ext = [
-00000e50: 0a20 2020 2020 2020 2027 6d70 3427 2c20  .        'mp4', 
-00000e60: 276d 3476 272c 2027 3367 7027 2c20 276d  'm4v', '3gp', 'm
-00000e70: 7067 272c 2027 666c 7627 2c20 2766 3476  pg', 'flv', 'f4v
-00000e80: 272c 200a 2020 2020 2020 2020 2773 7766  ', .        'swf
-00000e90: 272c 2027 6176 6927 2c20 2767 6966 272c  ', 'avi', 'gif',
-00000ea0: 2027 776d 7627 2c20 2772 6d76 6227 2c20   'wmv', 'rmvb', 
-00000eb0: 276d 6f76 272c 200a 2020 2020 2020 2020  'mov', .        
-00000ec0: 276d 7473 272c 2027 6d32 7427 2c20 2777  'mts', 'm2t', 'w
-00000ed0: 6562 6d27 2c20 276f 6767 272c 2027 6d6b  ebm', 'ogg', 'mk
-00000ee0: 7627 2c20 276d 7033 272c 200a 2020 2020  v', 'mp3', .    
-00000ef0: 2020 2020 2761 6163 272c 2027 6170 6527      'aac', 'ape'
-00000f00: 2c20 2766 6c61 6327 2c20 2777 6176 272c  , 'flac', 'wav',
-00000f10: 2027 776d 6127 2c20 2761 6d72 272c 2027   'wma', 'amr', '
-00000f20: 6d69 6427 2c0a 2020 2020 5d0a 2020 2020  mid',.    ].    
-00000f30: 6d20 3d20 7265 2e73 6561 7263 6828 7227  m = re.search(r'
-00000f40: 5c2e 285c 772b 2924 272c 2066 6e61 6d65  \.(\w+)$', fname
-00000f50: 290a 2020 2020 7265 7475 726e 2062 6f6f  ).    return boo
-00000f60: 6c28 6d20 616e 6420 6d2e 6772 6f75 7028  l(m and m.group(
-00000f70: 3129 2069 6e20 6578 7429 0a20 2020 200a  1) in ext).    .
-00000f80: 6465 6620 6469 6374 5f67 6574 5f72 6563  def dict_get_rec
-00000f90: 7572 286f 626a 2c20 6b65 7973 293a 0a20  ur(obj, keys):. 
-00000fa0: 2020 2072 6573 203d 205b 6f62 6a5d 0a20     res = [obj]. 
-00000fb0: 2020 2066 6f72 206b 2069 6e20 6b65 7973     for k in keys
-00000fc0: 2e73 706c 6974 2827 2e27 293a 0a20 2020  .split('.'):.   
-00000fd0: 2020 2020 206b 203d 206b 2e73 7472 6970       k = k.strip
-00000fe0: 2829 0a20 2020 2020 2020 2069 6620 6b20  ().        if k 
-00000ff0: 3d3d 2027 2a27 3a0a 2020 2020 2020 2020  == '*':.        
-00001000: 2020 2020 7265 7320 3d20 7265 6475 6365      res = reduce
-00001010: 286c 616d 6264 6120 782c 2079 3a20 7820  (lambda x, y: x 
-00001020: 2b20 792c 7265 732c 205b 5d29 0a20 2020  + y,res, []).   
-00001030: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00001040: 2020 2020 2020 2072 6573 203d 205b 6f2e         res = [o.
-00001050: 6765 7428 6b29 2066 6f72 206f 2069 6e20  get(k) for o in 
-00001060: 7265 7320 6966 206b 2069 6e20 6f5d 0a20  res if k in o]. 
-00001070: 2020 2072 6574 7572 6e20 7265 73            return res
+00000000: 696d 706f 7274 2074 656d 7066 696c 650d  import tempfile.
+00000010: 0a69 6d70 6f72 7420 7575 6964 0d0a 696d  .import uuid..im
+00000020: 706f 7274 2073 7562 7072 6f63 6573 7320  port subprocess 
+00000030: 6173 2073 7562 700d 0a69 6d70 6f72 7420  as subp..import 
+00000040: 7265 0d0a 696d 706f 7274 206f 730d 0a69  re..import os..i
+00000050: 6d70 6f72 7420 7368 7574 696c 0d0a 696d  mport shutil..im
+00000060: 706f 7274 206a 736f 6e0d 0a69 6d70 6f72  port json..impor
+00000070: 7420 7961 6d6c 0d0a 696d 706f 7274 2074  t yaml..import t
+00000080: 7261 6365 6261 636b 0d0a 6672 6f6d 2066  raceback..from f
+00000090: 756e 6374 6f6f 6c73 2069 6d70 6f72 7420  unctools import 
+000000a0: 7265 6475 6365 0d0a 6672 6f6d 2075 726c  reduce..from url
+000000b0: 6c69 622e 7061 7273 6520 696d 706f 7274  lib.parse import
+000000c0: 2071 756f 7465 5f70 6c75 730d 0a66 726f   quote_plus..fro
+000000d0: 6d20 6f73 2069 6d70 6f72 7420 7061 7468  m os import path
+000000e0: 0d0a 6672 6f6d 2070 7971 7565 7279 2069  ..from pyquery i
+000000f0: 6d70 6f72 7420 5079 5175 6572 7920 6173  mport PyQuery as
+00000100: 2070 710d 0a66 726f 6d20 6461 7465 7469   pq..from dateti
+00000110: 6d65 2069 6d70 6f72 7420 6461 7465 7469  me import dateti
+00000120: 6d65 0d0a 6672 6f6d 2063 6f6c 6c65 6374  me..from collect
+00000130: 696f 6e73 2069 6d70 6f72 7420 4f72 6465  ions import Orde
+00000140: 7265 6444 6963 740d 0a69 6d70 6f72 7420  redDict..import 
+00000150: 696d 6779 6173 6f0d 0a0d 0a52 455f 5941  imgyaso....RE_YA
+00000160: 4d4c 5f4d 4554 4120 3d20 7227 3c21 2d2d  ML_META = r'<!--
+00000170: 796d 6c28 5b5c 735c 535d 2b3f 292d 2d3e  yml([\s\S]+?)-->
+00000180: 270d 0a52 455f 5449 544c 4520 3d20 7227  '..RE_TITLE = r'
+00000190: 5e23 2b20 282e 2b3f 2924 270d 0a52 455f  ^#+ (.+?)$'..RE_
+000001a0: 534f 5552 4345 203d 2072 272f 285b 5e2f  SOURCE = r'/([^/
+000001b0: 5c6e 5d2b 3f29 2f3f 3e27 0d0a 5245 5f43  \n]+?)/?>'..RE_C
+000001c0: 4f44 455f 424c 4f43 4b20 3d20 7227 6060  ODE_BLOCK = r'``
+000001d0: 605b 5c73 5c53 5d2b 3f60 6060 270d 0a52  `[\s\S]+?```'..R
+000001e0: 455f 494d 4720 3d20 7227 215c 5b2e 2a3f  E_IMG = r'!\[.*?
+000001f0: 5c5d 5c28 2e2a 3f5c 2927 0d0a 2320 576f  \]\(.*?\)'..# Wo
+00000200: 7264 20e5 ad97 e695 b0e7 bb9f e8ae a1e6  rd .............
+00000210: a087 e587 86ef bc9a 0d0a 2320 e4b8 80e4  ..........# ....
+00000220: b8aa e6b1 89e5 ad97 e688 96e4 b8ad e696  ................
+00000230: 87e6 a087 e782 b9e7 ae97 e4b8 80e4 b8aa  ................
+00000240: e5ad 970d 0a23 20e4 b880 e4b8 aae8 bf9e  .....# .........
+00000250: e7bb ade7 9a84 e88b b1e6 9687 e5ad 97e6  ................
+00000260: af8d e380 81e6 a087 e782 b9e5 928c e695  ................
+00000270: b0e5 ad97 e5ba 8fe5 8897 e7ae 97e4 b880  ................
+00000280: e4b8 aae5 ad97 0d0a 5245 5f5a 485f 574f  ........RE_ZH_WO
+00000290: 5244 203d 2072 275b 5c75 3230 3138 2d5c  RD = r'[\u2018-\
+000002a0: 7532 3031 645c 7533 3030 312d 5c75 3330  u201d\u3001-\u30
+000002b0: 3163 5c75 3465 3030 2d5c 7539 6666 665c  1c\u4e00-\u9fff\
+000002c0: 7566 6630 312d 5c75 6666 3635 5d27 0d0a  uff01-\uff65]'..
+000002d0: 5245 5f45 4e5f 574f 5244 203d 2072 275b  RE_EN_WORD = r'[
+000002e0: 5c78 3231 2d5c 7837 655d 2b27 0d0a 5245  \x21-\x7e]+'..RE
+000002f0: 5f49 4652 414d 4520 3d20 7227 3c69 6672  _IFRAME = r'<ifr
+00000300: 616d 655b 5e3e 5d2a 7372 633d 2228 2e2b  ame[^>]*src="(.+
+00000310: 3f29 225b 5e3e 5d2a 3e27 0d0a 5245 5f49  ?)"[^>]*>'..RE_I
+00000320: 4652 414d 455f 414c 4c20 3d20 7227 3c2f  FRAME_ALL = r'</
+00000330: 3f69 6672 616d 655b 5e3e 5d2a 3e27 0d0a  ?iframe[^>]*>'..
+00000340: 5245 5f49 4652 414d 455f 5245 504c 203d  RE_IFRAME_REPL =
+00000350: 2072 273c 6272 2f3e 3c62 722f 3e3c 6120   r'<br/><br/><a 
+00000360: 6872 6566 3d22 5c31 223e 5c31 3c2f 613e  href="\1">\1</a>
+00000370: 3c62 722f 3e3c 6272 2f3e 270d 0a0d 0a44  <br/><br/>'....D
+00000380: 4952 203d 2070 6174 682e 6469 726e 616d  IR = path.dirnam
+00000390: 6528 7061 7468 2e61 6273 7061 7468 285f  e(path.abspath(_
+000003a0: 5f66 696c 655f 5f29 290d 0a0d 0a64 6566  _file__))....def
+000003b0: 6175 6c74 5f68 6472 7320 3d20 7b0d 0a20  ault_hdrs = {.. 
+000003c0: 2020 2027 5573 6572 2d41 6765 6e74 273a     'User-Agent':
+000003d0: 2027 4d6f 7a69 6c6c 612f 352e 3020 2857   'Mozilla/5.0 (W
+000003e0: 696e 646f 7773 204e 5420 3130 2e30 3b20  indows NT 10.0; 
+000003f0: 5769 6e36 343b 2078 3634 2920 4170 706c  Win64; x64) Appl
+00000400: 6557 6562 4b69 742f 3533 372e 3336 2028  eWebKit/537.36 (
+00000410: 4b48 544d 4c2c 206c 696b 6520 4765 636b  KHTML, like Geck
+00000420: 6f29 2043 6872 6f6d 652f 3830 2e30 2e33  o) Chrome/80.0.3
+00000430: 3938 372e 3133 3220 5361 6661 7269 2f35  987.132 Safari/5
+00000440: 3337 2e33 3627 2c0d 0a7d 0d0a 0d0a 6865  37.36',..}....he
+00000450: 6164 6572 7320 3d20 7b0d 0a20 2020 2027  aders = {..    '
+00000460: 5573 6572 2d41 6765 6e74 273a 2027 506f  User-Agent': 'Po
+00000470: 7374 6d61 6e52 756e 7469 6d65 2f37 2e32  stmanRuntime/7.2
+00000480: 362e 3827 2c0d 0a20 2020 2027 5265 6665  6.8',..    'Refe
+00000490: 7265 7227 3a20 2768 7474 7073 3a2f 2f77  rer': 'https://w
+000004a0: 7777 2e62 696c 6962 696c 692e 636f 6d2f  ww.bilibili.com/
+000004b0: 272c 0d0a 7d0d 0a0d 0a0d 0a64 6566 2064  ',..}......def d
+000004c0: 286e 616d 6529 3a0d 0a20 2020 2072 6574  (name):..    ret
+000004d0: 7572 6e20 7061 7468 2e6a 6f69 6e28 4449  urn path.join(DI
+000004e0: 522c 206e 616d 6529 0d0a 0d0a 6465 6620  R, name)....def 
+000004f0: 6173 7365 7428 6e61 6d65 3d27 2729 3a0d  asset(name=''):.
+00000500: 0a20 2020 2072 6574 7572 6e20 7061 7468  .    return path
+00000510: 2e6a 6f69 6e28 4449 522c 2027 6173 7365  .join(DIR, 'asse
+00000520: 7473 272c 206e 616d 6529 0d0a 0d0a 6465  ts', name)....de
+00000530: 6620 6f70 7469 5f69 6d67 2869 6d67 2c20  f opti_img(img, 
+00000540: 6d6f 6465 2c20 636f 6c6f 7273 293a 0d0a  mode, colors):..
+00000550: 2020 2020 6966 206d 6f64 6520 3d3d 2027      if mode == '
+00000560: 7175 616e 7427 3a0d 0a20 2020 2020 2020  quant':..       
+00000570: 2072 6574 7572 6e20 696d 6779 6173 6f2e   return imgyaso.
+00000580: 706e 6771 7561 6e74 5f62 7473 2869 6d67  pngquant_bts(img
+00000590: 2c20 636f 6c6f 7273 290d 0a20 2020 2065  , colors)..    e
+000005a0: 6c69 6620 6d6f 6465 203d 3d20 2767 7269  lif mode == 'gri
+000005b0: 6427 3a0d 0a20 2020 2020 2020 2072 6574  d':..        ret
+000005c0: 7572 6e20 696d 6779 6173 6f2e 6772 6964  urn imgyaso.grid
+000005d0: 5f62 7473 2869 6d67 290d 0a20 2020 2065  _bts(img)..    e
+000005e0: 6c69 6620 6d6f 6465 203d 3d20 2774 7275  lif mode == 'tru
+000005f0: 6e63 273a 0d0a 2020 2020 2020 2020 7265  nc':..        re
+00000600: 7475 726e 2069 6d67 7961 736f 2e74 7275  turn imgyaso.tru
+00000610: 6e63 5f62 7473 2869 6d67 2c20 636f 6c6f  nc_bts(img, colo
+00000620: 7273 290d 0a20 2020 2065 6c69 6620 6d6f  rs)..    elif mo
+00000630: 6465 203d 3d20 2774 6872 6573 273a 0d0a  de == 'thres':..
+00000640: 2020 2020 2020 2020 7265 7475 726e 2069          return i
+00000650: 6d67 7961 736f 2e61 6461 7468 7265 735f  mgyaso.adathres_
+00000660: 6274 7328 696d 6729 0d0a 2020 2020 656c  bts(img)..    el
+00000670: 7365 3a0d 0a20 2020 2020 2020 2072 6574  se:..        ret
+00000680: 7572 6e20 696d 670d 0a0d 0a64 6566 2074  urn img....def t
+00000690: 6f6d 6428 6874 6d6c 293a 0d0a 2020 2020  omd(html):..    
+000006a0: 2320 e5a4 84e7 9086 2049 4652 414d 450d  # ...... IFRAME.
+000006b0: 0a20 2020 2068 746d 6c20 3d20 7265 2e73  .    html = re.s
+000006c0: 7562 2852 455f 4946 5241 4d45 2c20 5245  ub(RE_IFRAME, RE
+000006d0: 5f49 4652 414d 455f 5245 504c 2c20 6874  _IFRAME_REPL, ht
+000006e0: 6d6c 290d 0a20 2020 2068 746d 6c20 3d20  ml)..    html = 
+000006f0: 7265 2e73 7562 2852 455f 4946 5241 4d45  re.sub(RE_IFRAME
+00000700: 5f41 4c4c 2c20 2727 2c20 6874 6d6c 290d  _ALL, '', html).
+00000710: 0a20 2020 206a 735f 666e 616d 6520 3d20  .    js_fname = 
+00000720: 6428 2774 6f6d 642e 6a73 2729 0d0a 2020  d('tomd.js')..  
+00000730: 2020 6874 6d6c 5f66 6e61 6d65 203d 2070    html_fname = p
+00000740: 6174 682e 6a6f 696e 2874 656d 7066 696c  ath.join(tempfil
+00000750: 652e 6765 7474 656d 7064 6972 2829 2c20  e.gettempdir(), 
+00000760: 7575 6964 2e75 7569 6434 2829 2e68 6578  uuid.uuid4().hex
+00000770: 202b 2027 2e68 746d 6c27 290d 0a20 2020   + '.html')..   
+00000780: 206f 7065 6e28 6874 6d6c 5f66 6e61 6d65   open(html_fname
+00000790: 2c20 2777 272c 2065 6e63 6f64 696e 673d  , 'w', encoding=
+000007a0: 2775 7466 3827 292e 7772 6974 6528 6874  'utf8').write(ht
+000007b0: 6d6c 290d 0a20 2020 2073 7562 702e 506f  ml)..    subp.Po
+000007c0: 7065 6e28 0d0a 2020 2020 2020 2020 5b22  pen(..        ["
+000007d0: 6e6f 6465 222c 206a 735f 666e 616d 652c  node", js_fname,
+000007e0: 2068 746d 6c5f 666e 616d 655d 2c0d 0a20   html_fname],.. 
+000007f0: 2020 2020 2020 2073 6865 6c6c 3d54 7275         shell=Tru
+00000800: 652c 0d0a 2020 2020 292e 636f 6d6d 756e  e,..    ).commun
+00000810: 6963 6174 6528 290d 0a20 2020 206d 645f  icate()..    md_
+00000820: 666e 616d 6520 3d20 7265 2e73 7562 2872  fname = re.sub(r
+00000830: 275c 2e68 746d 6c24 272c 2027 272c 2068  '\.html$', '', h
+00000840: 746d 6c5f 666e 616d 6529 202b 2027 2e6d  tml_fname) + '.m
+00000850: 6427 0d0a 2020 2020 6d64 203d 206f 7065  d'..    md = ope
+00000860: 6e28 6d64 5f66 6e61 6d65 2c20 656e 636f  n(md_fname, enco
+00000870: 6469 6e67 3d27 7574 6638 2729 2e72 6561  ding='utf8').rea
+00000880: 6428 290d 0a20 2020 206f 732e 7265 6d6f  d()..    os.remo
+00000890: 7665 2868 746d 6c5f 666e 616d 6529 0d0a  ve(html_fname)..
+000008a0: 2020 2020 7265 7475 726e 206d 640d 0a0d      return md...
+000008b0: 0a64 6566 2066 6e61 6d65 5f65 7363 6170  .def fname_escap
+000008c0: 6528 6e61 6d65 293a 0d0a 2020 2020 7265  e(name):..    re
+000008d0: 7475 726e 206e 616d 652e 7265 706c 6163  turn name.replac
+000008e0: 6528 275c 5c27 2c20 27ef bcbc 2729 205c  e('\\', '...') \
+000008f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000900: 202e 7265 706c 6163 6528 272f 272c 2027   .replace('/', '
+00000910: efbc 8f27 2920 5c0d 0a20 2020 2020 2020  ...') \..       
+00000920: 2020 2020 2020 2020 2e72 6570 6c61 6365          .replace
+00000930: 2827 3a27 2c20 27ef bc9a 2729 205c 0d0a  (':', '...') \..
+00000940: 2020 2020 2020 2020 2020 2020 2020 202e                 .
+00000950: 7265 706c 6163 6528 272a 272c 2027 efbc  replace('*', '..
+00000960: 8a27 2920 5c0d 0a20 2020 2020 2020 2020  .') \..         
+00000970: 2020 2020 2020 2e72 6570 6c61 6365 2827        .replace('
+00000980: 3f27 2c20 27ef bc9f 2729 205c 0d0a 2020  ?', '...') \..  
+00000990: 2020 2020 2020 2020 2020 2020 202e 7265               .re
+000009a0: 706c 6163 6528 2722 272c 2027 efbc 8227  place('"', '...'
+000009b0: 2920 5c0d 0a20 2020 2020 2020 2020 2020  ) \..           
+000009c0: 2020 2020 2e72 6570 6c61 6365 2827 3c27      .replace('<'
+000009d0: 2c20 27ef bc9c 2729 205c 0d0a 2020 2020  , '...') \..    
+000009e0: 2020 2020 2020 2020 2020 202e 7265 706c             .repl
+000009f0: 6163 6528 273e 272c 2027 efbc 9e27 2920  ace('>', '...') 
+00000a00: 5c0d 0a20 2020 2020 2020 2020 2020 2020  \..             
+00000a10: 2020 2e72 6570 6c61 6365 2827 7c27 2c20    .replace('|', 
+00000a20: 27ef bd9c 2729 0d0a 2020 2020 2020 2020  '...')..        
+00000a30: 2020 2020 2020 200d 0a64 6566 2061 6363         ..def acc
+00000a40: 6f75 6e74 5f77 6f72 6473 2863 6f6e 7429  ount_words(cont)
+00000a50: 3a0d 0a20 2020 2023 20e5 8ebb e68e 89e4  :..    # .......
+00000a60: bba3 e7a0 81e5 9d97 e592 8ce5 9bbe e789  ................
+00000a70: 870d 0a20 2020 2063 6f6e 7420 3d20 7265  ...    cont = re
+00000a80: 2e73 7562 2852 455f 434f 4445 5f42 4c4f  .sub(RE_CODE_BLO
+00000a90: 434b 2c20 2727 2c20 636f 6e74 290d 0a20  CK, '', cont).. 
+00000aa0: 2020 2063 6f6e 7420 3d20 7265 2e73 7562     cont = re.sub
+00000ab0: 2852 455f 494d 472c 2027 272c 2063 6f6e  (RE_IMG, '', con
+00000ac0: 7429 0d0a 2020 2020 7a68 5f63 6f75 6e74  t)..    zh_count
+00000ad0: 203d 206c 656e 2872 652e 6669 6e64 616c   = len(re.findal
+00000ae0: 6c28 5245 5f5a 485f 574f 5244 2c20 636f  l(RE_ZH_WORD, co
+00000af0: 6e74 2929 0d0a 2020 2020 656e 5f63 6f75  nt))..    en_cou
+00000b00: 6e74 203d 206c 656e 2872 652e 6669 6e64  nt = len(re.find
+00000b10: 616c 6c28 5245 5f45 4e5f 574f 5244 2c20  all(RE_EN_WORD, 
+00000b20: 636f 6e74 2929 0d0a 2020 2020 746f 7461  cont))..    tota
+00000b30: 6c20 3d20 7a68 5f63 6f75 6e74 202b 2065  l = zh_count + e
+00000b40: 6e5f 636f 756e 740d 0a20 2020 2072 6574  n_count..    ret
+00000b50: 7572 6e20 2874 6f74 616c 2c20 7a68 5f63  urn (total, zh_c
+00000b60: 6f75 6e74 2c20 656e 5f63 6f75 6e74 290d  ount, en_count).
+00000b70: 0a20 2020 200d 0a64 6566 2073 6166 655f  .    ..def safe_
+00000b80: 6d6b 6469 7228 6469 7229 3a0d 0a20 2020  mkdir(dir):..   
+00000b90: 2074 7279 3a20 6f73 2e6d 616b 6564 6972   try: os.makedir
+00000ba0: 7328 6469 7229 0d0a 2020 2020 6578 6365  s(dir)..    exce
+00000bb0: 7074 3a20 7061 7373 0d0a 2020 2020 0d0a  pt: pass..    ..
+00000bc0: 6465 6620 7361 6665 5f72 6d64 6972 2864  def safe_rmdir(d
+00000bd0: 6972 293a 0d0a 2020 2020 7472 793a 2073  ir):..    try: s
+00000be0: 6875 7469 6c2e 726d 7472 6565 2864 6972  hutil.rmtree(dir
+00000bf0: 290d 0a20 2020 2065 7863 6570 743a 2070  )..    except: p
+00000c00: 6173 730d 0a0d 0a64 6566 2069 735f 635f  ass....def is_c_
+00000c10: 7374 796c 655f 636f 6465 2866 6e61 6d65  style_code(fname
+00000c20: 293a 0d0a 2020 2020 6578 7420 3d20 5b0d  ):..    ext = [.
+00000c30: 0a20 2020 2020 2020 2027 6327 2c20 2763  .        'c', 'c
+00000c40: 7070 272c 2027 6378 7827 2c20 2768 272c  pp', 'cxx', 'h',
+00000c50: 2027 6870 7027 2c0d 0a20 2020 2020 2020   'hpp',..       
+00000c60: 2027 6a61 7661 272c 2027 6b74 272c 2027   'java', 'kt', '
+00000c70: 7363 616c 6127 2c20 0d0a 2020 2020 2020  scala', ..      
+00000c80: 2020 2763 7327 2c20 276a 7327 2c20 276a    'cs', 'js', 'j
+00000c90: 736f 6e27 2c20 2774 7327 2c20 0d0a 2020  son', 'ts', ..  
+00000ca0: 2020 2020 2020 2770 6870 272c 2027 676f        'php', 'go
+00000cb0: 272c 2027 7275 7374 272c 2027 7377 6966  ', 'rust', 'swif
+00000cc0: 7427 2c0d 0a20 2020 205d 0d0a 2020 2020  t',..    ]..    
+00000cd0: 6d20 3d20 7265 2e73 6561 7263 6828 7227  m = re.search(r'
+00000ce0: 5c2e 285c 772b 2924 272c 2066 6e61 6d65  \.(\w+)$', fname
+00000cf0: 290d 0a20 2020 2072 6574 7572 6e20 626f  )..    return bo
+00000d00: 6f6c 286d 2061 6e64 206d 2e67 726f 7570  ol(m and m.group
+00000d10: 2831 2920 696e 2065 7874 290d 0a0d 0a64  (1) in ext)....d
+00000d20: 6566 2069 735f 7069 6328 666e 616d 6529  ef is_pic(fname)
+00000d30: 3a0d 0a20 2020 2065 7874 203d 205b 0d0a  :..    ext = [..
+00000d40: 2020 2020 2020 2020 276a 7067 272c 2027          'jpg', '
+00000d50: 6a70 6567 272c 2027 6a66 6966 272c 2027  jpeg', 'jfif', '
+00000d60: 706e 6727 2c20 0d0a 2020 2020 2020 2020  png', ..        
+00000d70: 2767 6966 272c 2027 7469 6666 272c 2027  'gif', 'tiff', '
+00000d80: 7765 6270 270d 0a20 2020 205d 0d0a 2020  webp'..    ]..  
+00000d90: 2020 6d20 3d20 7265 2e73 6561 7263 6828    m = re.search(
+00000da0: 7227 5c2e 285c 772b 2924 272c 2066 6e61  r'\.(\w+)$', fna
+00000db0: 6d65 290d 0a20 2020 2072 6574 7572 6e20  me)..    return 
+00000dc0: 626f 6f6c 286d 2061 6e64 206d 2e67 726f  bool(m and m.gro
+00000dd0: 7570 2831 2920 696e 2065 7874 290d 0a0d  up(1) in ext)...
+00000de0: 0a64 6566 2066 696e 645f 636d 645f 7061  .def find_cmd_pa
+00000df0: 7468 286e 616d 6529 3a0d 0a20 2020 2066  th(name):..    f
+00000e00: 6f72 2070 2069 6e20 6f73 2e65 6e76 6972  or p in os.envir
+00000e10: 6f6e 2e67 6574 2827 5041 5448 272c 2027  on.get('PATH', '
+00000e20: 2729 2e73 706c 6974 2827 3b27 293a 0d0a  ').split(';'):..
+00000e30: 2020 2020 2020 2020 6966 2070 6174 682e          if path.
+00000e40: 6973 6669 6c65 2870 6174 682e 6a6f 696e  isfile(path.join
+00000e50: 2870 2c20 6e61 6d65 2929 206f 7220 5c0d  (p, name)) or \.
+00000e60: 0a20 2020 2020 2020 2020 2020 2070 6174  .            pat
+00000e70: 682e 6973 6669 6c65 2870 6174 682e 6a6f  h.isfile(path.jo
+00000e80: 696e 2870 2c20 6e61 6d65 202b 2027 2e65  in(p, name + '.e
+00000e90: 7865 2729 293a 0d0a 2020 2020 2020 2020  xe')):..        
+00000ea0: 2020 2020 7265 7475 726e 2070 0d0a 2020      return p..  
+00000eb0: 2020 7265 7475 726e 2027 270d 0a20 2020    return ''..   
+00000ec0: 200d 0a64 6566 2069 735f 7669 6465 6f28   ..def is_video(
+00000ed0: 666e 616d 6529 3a0d 0a20 2020 2065 7874  fname):..    ext
+00000ee0: 203d 205b 0d0a 2020 2020 2020 2020 276d   = [..        'm
+00000ef0: 7034 272c 2027 6d34 7627 2c20 2733 6770  p4', 'm4v', '3gp
+00000f00: 272c 2027 6d70 6727 2c20 2766 6c76 272c  ', 'mpg', 'flv',
+00000f10: 2027 6634 7627 2c20 0d0a 2020 2020 2020   'f4v', ..      
+00000f20: 2020 2773 7766 272c 2027 6176 6927 2c20    'swf', 'avi', 
+00000f30: 2767 6966 272c 2027 776d 7627 2c20 2772  'gif', 'wmv', 'r
+00000f40: 6d76 6227 2c20 276d 6f76 272c 200d 0a20  mvb', 'mov', .. 
+00000f50: 2020 2020 2020 2027 6d74 7327 2c20 276d         'mts', 'm
+00000f60: 3274 272c 2027 7765 626d 272c 2027 6f67  2t', 'webm', 'og
+00000f70: 6727 2c20 276d 6b76 272c 2027 6d70 3327  g', 'mkv', 'mp3'
+00000f80: 2c20 0d0a 2020 2020 2020 2020 2761 6163  , ..        'aac
+00000f90: 272c 2027 6170 6527 2c20 2766 6c61 6327  ', 'ape', 'flac'
+00000fa0: 2c20 2777 6176 272c 2027 776d 6127 2c20  , 'wav', 'wma', 
+00000fb0: 2761 6d72 272c 2027 6d69 6427 2c0d 0a20  'amr', 'mid',.. 
+00000fc0: 2020 205d 0d0a 2020 2020 6d20 3d20 7265     ]..    m = re
+00000fd0: 2e73 6561 7263 6828 7227 5c2e 285c 772b  .search(r'\.(\w+
+00000fe0: 2924 272c 2066 6e61 6d65 290d 0a20 2020  )$', fname)..   
+00000ff0: 2072 6574 7572 6e20 626f 6f6c 286d 2061   return bool(m a
+00001000: 6e64 206d 2e67 726f 7570 2831 2920 696e  nd m.group(1) in
+00001010: 2065 7874 290d 0a20 2020 200d 0a64 6566   ext)..    ..def
+00001020: 2064 6963 745f 6765 745f 7265 6375 7228   dict_get_recur(
+00001030: 6f62 6a2c 206b 6579 7329 3a0d 0a20 2020  obj, keys):..   
+00001040: 2072 6573 203d 205b 6f62 6a5d 0d0a 2020   res = [obj]..  
+00001050: 2020 666f 7220 6b20 696e 206b 6579 732e    for k in keys.
+00001060: 7370 6c69 7428 272e 2729 3a0d 0a20 2020  split('.'):..   
+00001070: 2020 2020 206b 203d 206b 2e73 7472 6970       k = k.strip
+00001080: 2829 0d0a 2020 2020 2020 2020 6966 206b  ()..        if k
+00001090: 203d 3d20 272a 273a 0d0a 2020 2020 2020   == '*':..      
+000010a0: 2020 2020 2020 7265 7320 3d20 7265 6475        res = redu
+000010b0: 6365 286c 616d 6264 6120 782c 2079 3a20  ce(lambda x, y: 
+000010c0: 7820 2b20 792c 7265 732c 205b 5d29 0d0a  x + y,res, [])..
+000010d0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+000010e0: 2020 2020 2020 2020 2020 2072 6573 203d             res =
+000010f0: 205b 6f2e 6765 7428 6b29 2066 6f72 206f   [o.get(k) for o
+00001100: 2069 6e20 7265 7320 6966 206b 2069 6e20   in res if k in 
+00001110: 6f5d 0d0a 2020 2020 7265 7475 726e 2072  o]..    return r
+00001120: 6573 0d0a 2020 2020 0d0a 6465 6620 7361  es..    ..def sa
+00001130: 6665 2864 6566 6175 6c74 3d4e 6f6e 6529  fe(default=None)
+00001140: 3a0d 0a20 2020 2064 6566 206f 7574 6572  :..    def outer
+00001150: 2866 293a 0d0a 2020 2020 2020 2020 6465  (f):..        de
+00001160: 6620 696e 6e65 7228 2a61 7267 732c 202a  f inner(*args, *
+00001170: 2a6b 7729 3a0d 0a20 2020 2020 2020 2020  *kw):..         
+00001180: 2020 2070 7269 6e74 2831 3233 3132 3329     print(123123)
+00001190: 0d0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
+000011a0: 793a 2072 6574 7572 6e20 6628 2a61 7267  y: return f(*arg
+000011b0: 732c 202a 2a6b 7729 0d0a 2020 2020 2020  s, **kw)..      
+000011c0: 2020 2020 2020 6578 6365 7074 3a20 0d0a        except: ..
+000011d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011e0: 7472 6163 6562 6163 6b2e 7072 696e 745f  traceback.print_
+000011f0: 6578 6328 290d 0a20 2020 2020 2020 2020  exc()..         
+00001200: 2020 2020 2020 2072 6574 7572 6e20 6465         return de
+00001210: 6661 756c 740d 0a20 2020 2020 2020 2072  fault..        r
+00001220: 6574 7572 6e20 696e 6e65 720d 0a20 2020  eturn inner..   
+00001230: 2072 6574 7572 6e20 6f75 7465 720d 0a     return outer..
```

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool/wx_external.py` & `BookerWikiTool-2023.3.30.0/BookerWikiTool/wx_external.py`

 * *Files identical despite different names*

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool/zip_tool.py` & `BookerWikiTool-2023.3.30.0/BookerWikiTool/zip_tool.py`

 * *Files identical despite different names*

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool.egg-info/PKG-INFO` & `BookerWikiTool-2023.3.30.0/BookerWikiTool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BookerWikiTool
-Version: 2023.2.27.3
+Version: 2023.3.30.0
 Summary: iBooker/ApacheCN 知识库抓取工具
 Home-page: https://github.com/apachecn/BookerWikiTool
 Author: ApacheCN
 Author-email: apachecn@163.com
 License: UNKNOWN
 Description: # BookerWikiTool
```

### Comparing `BookerWikiTool-2023.2.27.3/BookerWikiTool.egg-info/SOURCES.txt` & `BookerWikiTool-2023.3.30.0/BookerWikiTool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BookerWikiTool-2023.2.27.3/PKG-INFO` & `BookerWikiTool-2023.3.30.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BookerWikiTool
-Version: 2023.2.27.3
+Version: 2023.3.30.0
 Summary: iBooker/ApacheCN 知识库抓取工具
 Home-page: https://github.com/apachecn/BookerWikiTool
 Author: ApacheCN
 Author-email: apachecn@163.com
 License: UNKNOWN
 Description: # BookerWikiTool
```

### Comparing `BookerWikiTool-2023.2.27.3/README.md` & `BookerWikiTool-2023.3.30.0/README.md`

 * *Files identical despite different names*

### Comparing `BookerWikiTool-2023.2.27.3/setup.py` & `BookerWikiTool-2023.3.30.0/setup.py`

 * *Files identical despite different names*

