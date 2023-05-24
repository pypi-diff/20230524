# Comparing `tmp/zood-0.7.4.tar.gz` & `tmp/zood-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zood-0.7.4.tar", max compression
+gzip compressed data, was "zood-0.7.5.tar", max compression
```

## Comparing `zood-0.7.4.tar` & `zood-0.7.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      550 2023-05-19 00:23:55.203739 zood-0.7.4/pyproject.toml
--rw-r--r--   0        0        0      449 2023-01-13 08:15:49.760695 zood-0.7.4/README.md
--rw-r--r--   0        0        0       24 2023-01-06 12:50:33.818825 zood-0.7.4/zood/__init__.py
--rw-r--r--   0        0        0     6308 2023-05-19 00:23:30.751193 zood-0.7.4/zood/config/_config.yml
--rw-r--r--   0        0        0      209 2022-12-30 16:25:34.984515 zood-0.7.4/zood/config/img/after_copy.png
--rw-r--r--   0        0        0      215 2022-12-30 15:33:16.742079 zood-0.7.4/zood/config/img/before_copy.png
--rw-r--r--   0        0        0     2720 2023-01-14 08:58:35.867485 zood-0.7.4/zood/config/img/enter.png
--rw-r--r--   0        0        0      247 2023-01-14 09:31:22.970712 zood-0.7.4/zood/config/img/enter.svg
--rw-r--r--   0        0        0      454 2022-12-30 16:25:01.986421 zood-0.7.4/zood/config/img/moon.png
--rw-r--r--   0        0        0      446 2023-01-13 11:27:05.445651 zood-0.7.4/zood/config/img/search.svg
--rw-r--r--   0        0        0      428 2022-12-30 16:24:58.219147 zood-0.7.4/zood/config/img/sun.png
--rw-r--r--   0        0        0    18737 2023-05-19 00:22:38.369521 zood-0.7.4/zood/config/index.css
--rw-r--r--   0        0        0     3993 2023-04-29 02:33:40.621393 zood-0.7.4/zood/config/js/change_mode.js
--rw-r--r--   0        0        0     1039 2023-05-18 23:52:12.867359 zood-0.7.4/zood/config/js/check_box.js
--rw-r--r--   0        0        0     2654 2023-04-29 06:50:24.299560 zood-0.7.4/zood/config/js/copy_code.js
--rw-r--r--   0        0        0     2253 2023-05-19 00:21:16.921967 zood-0.7.4/zood/config/js/navigator.js
--rw-r--r--   0        0        0     1000 2023-01-01 02:18:50.438286 zood-0.7.4/zood/config/js/next_front.js
--rw-r--r--   0        0        0     1064 2023-01-02 14:54:02.515677 zood-0.7.4/zood/config/js/picture_preview.js
--rw-r--r--   0        0        0      285 2023-01-02 13:48:40.110725 zood-0.7.4/zood/config/js/picture_title.js
--rw-r--r--   0        0        0     2301 2023-02-17 14:35:29.225249 zood-0.7.4/zood/config/js/prismjs/prism.css
--rw-r--r--   0        0        0    64866 2023-04-27 06:47:33.381797 zood-0.7.4/zood/config/js/prismjs/prism.js
--rw-r--r--   0        0        0     5999 2023-04-19 11:50:00.362712 zood-0.7.4/zood/config/js/search.js
--rw-r--r--   0        0        0      546 2023-04-27 06:18:09.762970 zood-0.7.4/zood/config/template.html
--rw-r--r--   0        0        0     4224 2023-04-03 14:22:34.682079 zood-0.7.4/zood/main.py
--rw-r--r--   0        0        0     3535 2023-01-14 05:32:31.481099 zood-0.7.4/zood/md_parser.py
--rw-r--r--   0        0        0     4290 2023-04-03 14:22:32.130915 zood-0.7.4/zood/util.py
--rw-r--r--   0        0        0     8706 2023-04-29 06:09:49.501448 zood-0.7.4/zood/zood.py
--rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 zood-0.7.4/setup.py
--rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 zood-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0      550 2023-05-24 15:15:01.902988 zood-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0      449 2023-01-13 08:15:49.760695 zood-0.7.5/README.md
+-rw-r--r--   0        0        0       24 2023-01-06 12:50:33.818825 zood-0.7.5/zood/__init__.py
+-rw-r--r--   0        0        0     6308 2023-05-19 00:23:30.751193 zood-0.7.5/zood/config/_config.yml
+-rw-r--r--   0        0        0      209 2022-12-30 16:25:34.984515 zood-0.7.5/zood/config/img/after_copy.png
+-rw-r--r--   0        0        0      215 2022-12-30 15:33:16.742079 zood-0.7.5/zood/config/img/before_copy.png
+-rw-r--r--   0        0        0     2720 2023-01-14 08:58:35.867485 zood-0.7.5/zood/config/img/enter.png
+-rw-r--r--   0        0        0      247 2023-01-14 09:31:22.970712 zood-0.7.5/zood/config/img/enter.svg
+-rw-r--r--   0        0        0      454 2022-12-30 16:25:01.986421 zood-0.7.5/zood/config/img/moon.png
+-rw-r--r--   0        0        0      446 2023-01-13 11:27:05.445651 zood-0.7.5/zood/config/img/search.svg
+-rw-r--r--   0        0        0      428 2022-12-30 16:24:58.219147 zood-0.7.5/zood/config/img/sun.png
+-rw-r--r--   0        0        0    18776 2023-05-24 15:13:42.054920 zood-0.7.5/zood/config/index.css
+-rw-r--r--   0        0        0     3993 2023-04-29 02:33:40.621393 zood-0.7.5/zood/config/js/change_mode.js
+-rw-r--r--   0        0        0     1039 2023-05-18 23:52:12.867359 zood-0.7.5/zood/config/js/check_box.js
+-rw-r--r--   0        0        0     2654 2023-04-29 06:50:24.299560 zood-0.7.5/zood/config/js/copy_code.js
+-rw-r--r--   0        0        0     2253 2023-05-19 00:21:16.921967 zood-0.7.5/zood/config/js/navigator.js
+-rw-r--r--   0        0        0     1000 2023-01-01 02:18:50.438286 zood-0.7.5/zood/config/js/next_front.js
+-rw-r--r--   0        0        0     1064 2023-01-02 14:54:02.515677 zood-0.7.5/zood/config/js/picture_preview.js
+-rw-r--r--   0        0        0      285 2023-01-02 13:48:40.110725 zood-0.7.5/zood/config/js/picture_title.js
+-rw-r--r--   0        0        0     2301 2023-02-17 14:35:29.225249 zood-0.7.5/zood/config/js/prismjs/prism.css
+-rw-r--r--   0        0        0    64866 2023-04-27 06:47:33.381797 zood-0.7.5/zood/config/js/prismjs/prism.js
+-rw-r--r--   0        0        0     5999 2023-04-19 11:50:00.362712 zood-0.7.5/zood/config/js/search.js
+-rw-r--r--   0        0        0      546 2023-04-27 06:18:09.762970 zood-0.7.5/zood/config/template.html
+-rw-r--r--   0        0        0     4224 2023-04-03 14:22:34.682079 zood-0.7.5/zood/main.py
+-rw-r--r--   0        0        0     3535 2023-01-14 05:32:31.481099 zood-0.7.5/zood/md_parser.py
+-rw-r--r--   0        0        0     4290 2023-04-03 14:22:32.130915 zood-0.7.5/zood/util.py
+-rw-r--r--   0        0        0     8706 2023-04-29 06:09:49.501448 zood-0.7.5/zood/zood.py
+-rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 zood-0.7.5/setup.py
+-rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 zood-0.7.5/PKG-INFO
```

### Comparing `zood-0.7.4/pyproject.toml` & `zood-0.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zood"
-version = "0.7.4"
+version = "0.7.5"
 description = "web page documentation & comment generation documentation"
 license = "MIT"
 authors = ["kamilu <luzhixing12345@163.com>"]
 readme = "README.md"
 repository = "https://github.com/luzhixing12345/zood"
 documentation = "https://luzhixing12345.github.io/zood/"
```

### Comparing `zood-0.7.4/zood/config/_config.yml` & `zood-0.7.5/zood/config/_config.yml`

 * *Files identical despite different names*

### Comparing `zood-0.7.4/zood/config/img/enter.png` & `zood-0.7.5/zood/config/img/enter.png`

 * *Files identical despite different names*

### Comparing `zood-0.7.4/zood/config/index.css` & `zood-0.7.5/zood/config/index.css`

 * *Files 0% similar despite different names*

```diff
@@ -858,14 +858,16 @@
   font-size: "<%dir_item_font_size%>";
   letter-spacing: "<%letter_spacing%>";
   scrollbar-width: none; /* Firefox */
   -ms-overflow-style: none; /* IE 10+ */
   text-overflow: ellipsis; /*  过长文字省略号 */
   white-space: nowrap; /*禁止文字折行*/
   list-style: none;
+  max-height: 50%;
+  overflow: auto;
 }
 
 .header-navigator::-webkit-scrollbar {
   display: none; /* Chrome Safari */
 }
 
 .header-navigator a {
```

### Comparing `zood-0.7.4/zood/config/js/change_mode.js` & `zood-0.7.5/zood/config/js/change_mode.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.4/zood/config/js/check_box.js` & `zood-0.7.5/zood/config/js/check_box.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.4/zood/config/js/copy_code.js` & `zood-0.7.5/zood/config/js/copy_code.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.4/zood/config/js/navigator.js` & `zood-0.7.5/zood/config/js/navigator.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.4/zood/config/js/next_front.js` & `zood-0.7.5/zood/config/js/next_front.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.4/zood/config/js/picture_preview.js` & `zood-0.7.5/zood/config/js/picture_preview.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.4/zood/config/js/prismjs/prism.css` & `zood-0.7.5/zood/config/js/prismjs/prism.css`

 * *Files identical despite different names*

### Comparing `zood-0.7.4/zood/config/js/prismjs/prism.js` & `zood-0.7.5/zood/config/js/prismjs/prism.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.4/zood/config/js/search.js` & `zood-0.7.5/zood/config/js/search.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.4/zood/config/template.html` & `zood-0.7.5/zood/config/template.html`

 * *Files identical despite different names*

### Comparing `zood-0.7.4/zood/main.py` & `zood-0.7.5/zood/main.py`

 * *Files identical despite different names*

### Comparing `zood-0.7.4/zood/md_parser.py` & `zood-0.7.5/zood/md_parser.py`

 * *Files identical despite different names*

### Comparing `zood-0.7.4/zood/util.py` & `zood-0.7.5/zood/util.py`

 * *Files identical despite different names*

### Comparing `zood-0.7.4/zood/zood.py` & `zood-0.7.5/zood/zood.py`

 * *Files identical despite different names*

### Comparing `zood-0.7.4/setup.py` & `zood-0.7.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ['MarkdownParser', 'PyYAML>=6.0,<7.0']
 
 entry_points = \
 {'console_scripts': ['zood = zood.main:main']}
 
 setup_kwargs = {
     'name': 'zood',
-    'version': '0.7.4',
+    'version': '0.7.5',
     'description': 'web page documentation & comment generation documentation',
     'long_description': '# zood\n\nzood 是一个辅助文档生成的Python库, zood的页面风格更倾向于纯文档内容而非博客\n\n## 主题预览\n\n[![20230101121438](https://raw.githubusercontent.com/learner-lu/picbed/master/20230101121438.png)](https://luzhixing12345.github.io/zood/)\n\n## 安装与使用\n\n```bash\npip install zood\n```\n\n参见 [用户使用文档](https://luzhixing12345.github.io/zood/)\n\n## 参考\n\n- [UI](https://remixicon.com/)',
     'author': 'kamilu',
     'author_email': 'luzhixing12345@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/luzhixing12345/zood',
```

### Comparing `zood-0.7.4/PKG-INFO` & `zood-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zood
-Version: 0.7.4
+Version: 0.7.5
 Summary: web page documentation & comment generation documentation
 Home-page: https://github.com/luzhixing12345/zood
 License: MIT
 Author: kamilu
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

