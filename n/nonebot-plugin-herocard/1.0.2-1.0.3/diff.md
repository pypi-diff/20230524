# Comparing `tmp/nonebot_plugin_herocard-1.0.2.tar.gz` & `tmp/nonebot-plugin-herocard-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_herocard-1.0.2.tar", last modified: Wed May 24 07:33:08 2023, max compression
+gzip compressed data, was "nonebot-plugin-herocard-1.0.3.tar", last modified: Wed May 24 15:23:32 2023, max compression
```

## Comparing `nonebot_plugin_herocard-1.0.2.tar` & `nonebot-plugin-herocard-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,4 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 07:33:08.324732 nonebot_plugin_herocard-1.0.2/
--rw-rw-rw-   0        0        0     2205 2023-05-24 07:33:08.322736 nonebot_plugin_herocard-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1754 2023-05-24 07:32:41.000000 nonebot_plugin_herocard-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 07:33:08.214767 nonebot_plugin_herocard-1.0.2/nonebot_plugin_herocard/
--rw-rw-rw-   0        0        0     2704 2023-05-24 05:34:54.000000 nonebot_plugin_herocard-1.0.2/nonebot_plugin_herocard/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:33:08.292586 nonebot_plugin_herocard-1.0.2/nonebot_plugin_herocard.egg-info/
--rw-rw-rw-   0        0        0     2205 2023-05-24 07:33:08.000000 nonebot_plugin_herocard-1.0.2/nonebot_plugin_herocard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-05-24 07:33:08.000000 nonebot_plugin_herocard-1.0.2/nonebot_plugin_herocard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 07:33:08.000000 nonebot_plugin_herocard-1.0.2/nonebot_plugin_herocard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-24 07:33:08.000000 nonebot_plugin_herocard-1.0.2/nonebot_plugin_herocard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 07:33:08.324732 nonebot_plugin_herocard-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1137 2023-05-24 07:32:57.000000 nonebot_plugin_herocard-1.0.2/setup.py
+-rw-r--r--   0        0        0     1707 2023-05-24 15:23:22.964186 nonebot-plugin-herocard-1.0.3/README.md
+-rw-r--r--   0        0        0     2704 2023-05-24 15:23:22.964186 nonebot-plugin-herocard-1.0.3/nonebot_plugin_herocard/__init__.py
+-rw-r--r--   0        0        0      588 2023-05-24 15:23:22.964186 nonebot-plugin-herocard-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2113 1970-01-01 00:00:00.000000 nonebot-plugin-herocard-1.0.3/PKG-INFO
```

### Comparing `nonebot_plugin_herocard-1.0.2/README.md` & `nonebot-plugin-herocard-1.0.3/README.md`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-<h1 align="center">NoneBot Plugin HeroCard</h1></br>
-
-<p align="center"> 用于提取本子🥵标题关键词的 NoneBot2 插件</p></br>
-
-<p align="center">
-  <a href="https://pypi.python.org/pypi/nonebot-plugin-herocard">
-    <img alt="PyPI" src="https://img.shields.io/pypi/v/nonebot-plugin-herocard?color=%23da3f3d">
-  </a>
-  <img src="https://img.shields.io/badge/python-3.9-blue?style=flat" alt="python"><br />
-</p></br>
-
-**安装方法**
-
-使用以下命令之一快速安装：
-
-``` 
-nb plugin install nonebot-plugin-herocard
-
-pip install --upgrade nonebot-plugin-herocard
-```
-重启 Bot 即可体验此插件。
-
-**使用方法**
-
- - 发送 `[作者さん]テーマ[中国翻訳] [DL版]`格式消息即可收到回复
- - 发送 `(2020 Summer)テーマ(subtitle) (31P) (完)`格式消息即可收到回复
-
-*\* 插件响应基于正则匹配，所以，甚至`回馈lz[作者さん]テーマ (31P)我感觉很顶`这样的指令都可用！*
-- **注意：** 
-  1.  发送消息中**一定**要包含**日文假名**，不论 *平假名* 还是 *片假名* ，否则插件不生效 
-  2.  若出现`None`回复或是`不回复`，可以考虑在您**想要提取文本**的前后加上`。`/`.` =>中英文句号均可
-
-
-**特别鸣谢**
-
-[@nonebot/nonebot2](https://github.com/nonebot/nonebot2/) | [@Mrs4s/go-cqhttp](https://github.com/Mrs4s/go-cqhttp) | [@monsterxcn/nonebot_plugin_epicfree](https://github.com/monsterxcn/nonebot_plugin_epicfree) 
-
-
-> 新人ざぁこ♡一枚，代码写的烂，最好别指望我能修什么bug！Ciallo～(∠・ω< )⌒☆
-
-**更新日志**
-
-`1.0.2` 修复一点README.md问题
-
-`1.0.1` 修复一点README.md问题
-
-`1.0.0` 首次发布，完善了README.md
+<h1 align="center">NoneBot Plugin HeroCard</h1></br>
+
+<p align="center"> 用于提取本子🥵标题关键词的 NoneBot2 插件</p></br>
+
+<p align="center">
+  <a href="https://pypi.python.org/pypi/nonebot-plugin-herocard">
+    <img alt="PyPI" src="https://img.shields.io/pypi/v/nonebot-plugin-herocard?color=%23da3f3d">
+  </a>
+  <img src="https://img.shields.io/badge/python-3.9-blue?style=flat" alt="python"><br />
+</p></br>
+
+**安装方法**
+
+使用以下命令之一快速安装：
+
+``` 
+nb plugin install nonebot-plugin-herocard
+
+pip install --upgrade nonebot-plugin-herocard
+```
+重启 Bot 即可体验此插件。
+
+**使用方法**
+
+ - 发送 `[作者さん]テーマ[中国翻訳] [DL版]`格式消息即可收到回复
+ - 发送 `(2020 Summer)テーマ(subtitle) (31P) (完)`格式消息即可收到回复
+
+*\* 插件响应基于正则匹配，所以，甚至`回馈lz[作者さん]テーマ (31P)我感觉很顶`这样的指令都可用！*
+- **注意：** 
+  1.  发送消息中**一定**要包含**日文假名**，不论 *平假名* 还是 *片假名* ，否则插件不生效 
+  2.  若出现`None`回复或是`不回复`，可以考虑在您**想要提取文本**的前后加上`。`/`.` =>中英文句号均可
+
+
+**特别鸣谢**
+
+[@nonebot/nonebot2](https://github.com/nonebot/nonebot2/) | [@Mrs4s/go-cqhttp](https://github.com/Mrs4s/go-cqhttp) | [@monsterxcn/nonebot_plugin_epicfree](https://github.com/monsterxcn/nonebot_plugin_epicfree) 
+
+
+> 新人ざぁこ♡一枚，代码写的烂，最好别指望我能修什么bug！Ciallo～(∠・ω< )⌒☆
+
+**更新日志**
+
+`1.0.2` 修复一点README.md问题
+
+`1.0.1` 修复一点README.md问题
+
+`1.0.0` 首次发布，完善了README.md
```

### Comparing `nonebot_plugin_herocard-1.0.2/nonebot_plugin_herocard/__init__.py` & `nonebot-plugin-herocard-1.0.3/nonebot_plugin_herocard/__init__.py`

 * *Files identical despite different names*

