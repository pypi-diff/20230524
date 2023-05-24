# Comparing `tmp/nonebot-plugin-helloworld-0.1.0.tar.gz` & `tmp/nonebot-plugin-helloworld-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-helloworld-0.1.0.tar", last modified: Sun Mar 26 09:40:12 2023, max compression
+gzip compressed data, was "nonebot-plugin-helloworld-0.2.0.tar", last modified: Wed May 24 11:29:33 2023, max compression
```

## Comparing `nonebot-plugin-helloworld-0.1.0.tar` & `nonebot-plugin-helloworld-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1064 2023-03-26 09:40:03.697066 nonebot-plugin-helloworld-0.1.0/LICENSE
--rw-r--r--   0        0        0     1902 2023-03-26 09:40:03.697066 nonebot-plugin-helloworld-0.1.0/README.md
--rw-r--r--   0        0        0      199 2023-03-26 09:40:03.697066 nonebot-plugin-helloworld-0.1.0/nonebot_plugin_helloworld/__init__.py
--rw-r--r--   0        0        0      540 2023-03-26 09:40:03.697066 nonebot-plugin-helloworld-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2282 1970-01-01 00:00:00.000000 nonebot-plugin-helloworld-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-24 11:29:25.601167 nonebot-plugin-helloworld-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1975 2023-05-24 11:29:25.601167 nonebot-plugin-helloworld-0.2.0/README.md
+-rw-r--r--   0        0        0      413 2023-05-24 11:29:25.601167 nonebot-plugin-helloworld-0.2.0/nonebot_plugin_helloworld/__init__.py
+-rw-r--r--   0        0        0      540 2023-05-24 11:29:25.601167 nonebot-plugin-helloworld-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 nonebot-plugin-helloworld-0.2.0/PKG-INFO
```

### Comparing `nonebot-plugin-helloworld-0.1.0/LICENSE` & `nonebot-plugin-helloworld-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-helloworld-0.1.0/README.md` & `nonebot-plugin-helloworld-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+<!-- markdownlint-disable MD033 MD036 MD041 -->
+
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # nonebot-plugin-helloworld
 
 _✨ Hello World! ✨_
 
-
 <a href="./LICENSE">
     <img src="https://img.shields.io/github/license/A-kirami/nonebot-plugin-helloworld.svg" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-helloworld">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-helloworld.svg" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
@@ -39,35 +40,41 @@
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
 
 <details>
 <summary>pip</summary>
 
     pip install nonebot-plugin-helloworld
+
 </details>
 <details>
 <summary>pdm</summary>
 
     pdm add nonebot-plugin-helloworld
+
 </details>
 <details>
 <summary>poetry</summary>
 
     poetry add nonebot-plugin-helloworld
+
 </details>
 <details>
 <summary>conda</summary>
 
     conda install nonebot-plugin-helloworld
+
 </details>
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
     plugins = ["nonebot_plugin_helloworld"]
 
 </details>
 
 ## 🎉 使用
+
 ### 指令表
-| 指令 | 权限 | 需要@ | 范围 | 说明 |
-|:-----:|:----:|:----:|:----:|:----:|
-| hello | 无 | 否 | 私聊/群聊 | world |
+
+| 指令  | 权限 | 需要@ |   范围    | 说明  |
+| :---: | :--: | :---: | :-------: | :---: |
+| hello |  无  |  否   | 私聊/群聊 | world |
```

#### html2text {}

```diff
@@ -6,9 +6,10 @@
 nb plugin install nonebot-plugin-helloworld   ä½¿ç¨åç®¡çå¨å®è£ å¨
 nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
 æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install
 nonebot-plugin-helloworld   pdm pdm add nonebot-plugin-helloworld   poetry
 poetry add nonebot-plugin-helloworld   conda conda install nonebot-plugin-
 helloworld  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨
 `[tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_helloworld"]  ##
-ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:---
---:|:----:|:----:|:----:|:----:| | hello | æ  | å¦ | ç§è/ç¾¤è | world |
+ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | | :--
+-: | :--: | :---: | :-------: | :---: | | hello | æ  | å¦ | ç§è/ç¾¤è |
+world |
```

### Comparing `nonebot-plugin-helloworld-0.1.0/pyproject.toml` & `nonebot-plugin-helloworld-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-helloworld"
-version = "0.1.0"
+version = "0.2.0"
 description = "NoneBot2 Hello World"
 authors = [
     { name = "Akirami", email = "Akiramiaya@outlook.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc3",
 ]
```

### Comparing `nonebot-plugin-helloworld-0.1.0/PKG-INFO` & `nonebot-plugin-helloworld-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-helloworld
-Version: 0.1.0
+Version: 0.2.0
 Summary: NoneBot2 Hello World
 License: MIT
 Author-email: Akirami <Akiramiaya@outlook.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/A-kirami/nonebot-plugin-helloworld
 Project-URL: Repository, https://github.com/A-kirami/nonebot-plugin-helloworld
 Description-Content-Type: text/markdown
 
+<!-- markdownlint-disable MD033 MD036 MD041 -->
+
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # nonebot-plugin-helloworld
 
 _✨ Hello World! ✨_
 
-
 <a href="./LICENSE">
     <img src="https://img.shields.io/github/license/A-kirami/nonebot-plugin-helloworld.svg" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-helloworld">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-helloworld.svg" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
@@ -50,36 +51,42 @@
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
 
 <details>
 <summary>pip</summary>
 
     pip install nonebot-plugin-helloworld
+
 </details>
 <details>
 <summary>pdm</summary>
 
     pdm add nonebot-plugin-helloworld
+
 </details>
 <details>
 <summary>poetry</summary>
 
     poetry add nonebot-plugin-helloworld
+
 </details>
 <details>
 <summary>conda</summary>
 
     conda install nonebot-plugin-helloworld
+
 </details>
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
     plugins = ["nonebot_plugin_helloworld"]
 
 </details>
 
 ## 🎉 使用
+
 ### 指令表
-| 指令 | 权限 | 需要@ | 范围 | 说明 |
-|:-----:|:----:|:----:|:----:|:----:|
-| hello | 无 | 否 | 私聊/群聊 | world |
+
+| 指令  | 权限 | 需要@ |   范围    | 说明  |
+| :---: | :--: | :---: | :-------: | :---: |
+| hello |  无  |  否   | 私聊/群聊 | world |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-helloworld Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-helloworld Version: 0.2.0 Summary:
 NoneBot2 Hello World License: MIT Author-email: Akirami
 outlook.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 A-kirami/nonebot-plugin-helloworld Project-URL: Repository, https://github.com/
 A-kirami/nonebot-plugin-helloworld Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-helloworld _â¨ Hello World! â¨_ [license] [pypi] [python]
@@ -11,9 +11,10 @@
 nb plugin install nonebot-plugin-helloworld   ä½¿ç¨åç®¡çå¨å®è£ å¨
 nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
 æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install
 nonebot-plugin-helloworld   pdm pdm add nonebot-plugin-helloworld   poetry
 poetry add nonebot-plugin-helloworld   conda conda install nonebot-plugin-
 helloworld  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨
 `[tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_helloworld"]  ##
-ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:---
---:|:----:|:----:|:----:|:----:| | hello | æ  | å¦ | ç§è/ç¾¤è | world |
+ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | | :--
+-: | :--: | :---: | :-------: | :---: | | hello | æ  | å¦ | ç§è/ç¾¤è |
+world |
```

