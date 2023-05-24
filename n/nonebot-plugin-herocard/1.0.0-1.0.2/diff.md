# Comparing `tmp/nonebot_plugin_herocard-1.0.0.tar.gz` & `tmp/nonebot_plugin_herocard-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_herocard-1.0.0.tar", last modified: Wed May 24 07:23:09 2023, max compression
+gzip compressed data, was "nonebot_plugin_herocard-1.0.2.tar", last modified: Wed May 24 07:33:08 2023, max compression
```

## Comparing `nonebot_plugin_herocard-1.0.0.tar` & `nonebot_plugin_herocard-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 07:23:09.384449 nonebot_plugin_herocard-1.0.0/
--rw-rw-rw-   0        0        0     2125 2023-05-24 07:23:09.381453 nonebot_plugin_herocard-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1678 2023-05-24 07:22:44.000000 nonebot_plugin_herocard-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 07:23:09.270792 nonebot_plugin_herocard-1.0.0/nonebot_plugin_herocard/
--rw-rw-rw-   0        0        0     2704 2023-05-24 05:34:54.000000 nonebot_plugin_herocard-1.0.0/nonebot_plugin_herocard/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:23:09.347542 nonebot_plugin_herocard-1.0.0/nonebot_plugin_herocard.egg-info/
--rw-rw-rw-   0        0        0     2125 2023-05-24 07:23:09.000000 nonebot_plugin_herocard-1.0.0/nonebot_plugin_herocard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-05-24 07:23:09.000000 nonebot_plugin_herocard-1.0.0/nonebot_plugin_herocard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 07:23:09.000000 nonebot_plugin_herocard-1.0.0/nonebot_plugin_herocard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-24 07:23:09.000000 nonebot_plugin_herocard-1.0.0/nonebot_plugin_herocard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 07:23:09.384449 nonebot_plugin_herocard-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1137 2023-05-24 07:22:51.000000 nonebot_plugin_herocard-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:33:08.324732 nonebot_plugin_herocard-1.0.2/
+-rw-rw-rw-   0        0        0     2205 2023-05-24 07:33:08.322736 nonebot_plugin_herocard-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1754 2023-05-24 07:32:41.000000 nonebot_plugin_herocard-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 07:33:08.214767 nonebot_plugin_herocard-1.0.2/nonebot_plugin_herocard/
+-rw-rw-rw-   0        0        0     2704 2023-05-24 05:34:54.000000 nonebot_plugin_herocard-1.0.2/nonebot_plugin_herocard/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:33:08.292586 nonebot_plugin_herocard-1.0.2/nonebot_plugin_herocard.egg-info/
+-rw-rw-rw-   0        0        0     2205 2023-05-24 07:33:08.000000 nonebot_plugin_herocard-1.0.2/nonebot_plugin_herocard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-05-24 07:33:08.000000 nonebot_plugin_herocard-1.0.2/nonebot_plugin_herocard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 07:33:08.000000 nonebot_plugin_herocard-1.0.2/nonebot_plugin_herocard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-24 07:33:08.000000 nonebot_plugin_herocard-1.0.2/nonebot_plugin_herocard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 07:33:08.324732 nonebot_plugin_herocard-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1137 2023-05-24 07:32:57.000000 nonebot_plugin_herocard-1.0.2/setup.py
```

### Comparing `nonebot_plugin_herocard-1.0.0/PKG-INFO` & `nonebot_plugin_herocard-1.0.2/nonebot_plugin_herocard.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
-Name: nonebot_plugin_herocard
-Version: 1.0.0
+Name: nonebot-plugin-herocard
+Version: 1.0.2
 Summary: nonebot小插件，提供简单的文本提取功能
 Author: Xie-Tiao
 Author-email: 1183004468@qq.com
 Keywords: python,hero,nonebot,nonebot2,tieba,hiragana,katakana,benzi
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 
 <h1 align="center">NoneBot Plugin HeroCard</h1></br>
 
 <p align="center"> 用于提取本子🥵标题关键词的 NoneBot2 插件</p></br>
 
 <p align="center">
-  <a href="https://pypi.python.org/pypi/nonebot_plugin_herocard">
-    <img src="https://img.shields.io/pypi/v/nonebot_plugin_herocard?style=flat-square" alt="pypi">
+  <a href="https://pypi.python.org/pypi/nonebot-plugin-herocard">
+    <img alt="PyPI" src="https://img.shields.io/pypi/v/nonebot-plugin-herocard?color=%23da3f3d">
   </a>
   <img src="https://img.shields.io/badge/python-3.9-blue?style=flat" alt="python"><br />
 </p></br>
 
 **安装方法**
 
 使用以下命令之一快速安装：
 
 ``` 
-nb plugin install nonebot_plugin_herocard
+nb plugin install nonebot-plugin-herocard
 
-pip install --upgrade nonebot_plugin_herocard
+pip install --upgrade nonebot-plugin-herocard
 ```
 重启 Bot 即可体验此插件。
 
 **使用方法**
 
  - 发送 `[作者さん]テーマ[中国翻訳] [DL版]`格式消息即可收到回复
  - 发送 `(2020 Summer)テーマ(subtitle) (31P) (完)`格式消息即可收到回复
@@ -48,8 +48,12 @@
 [@nonebot/nonebot2](https://github.com/nonebot/nonebot2/) | [@Mrs4s/go-cqhttp](https://github.com/Mrs4s/go-cqhttp) | [@monsterxcn/nonebot_plugin_epicfree](https://github.com/monsterxcn/nonebot_plugin_epicfree) 
 
 
 > 新人ざぁこ♡一枚，代码写的烂，最好别指望我能修什么bug！Ciallo～(∠・ω< )⌒☆
 
 **更新日志**
 
+`1.0.2` 修复一点README.md问题
+
+`1.0.1` 修复一点README.md问题
+
 `1.0.0` 首次发布，完善了README.md
```

#### html2text {}

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_herocard Version: 1.0.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-herocard Version: 1.0.2 Summary:
 nonebotå°æä»¶ï¼æä¾ç®åçææ¬æååè½ Author: Xie-Tiao Author-
 email: 1183004468@qq.com Keywords:
 python,hero,nonebot,nonebot2,tieba,hiragana,katakana,benzi Classifier:
 Programming Language :: Python :: 3.9 Classifier: Operating System :: Microsoft
 :: Windows Description-Content-Type: text/markdown
                      ****** NoneBot Plugin HeroCard ******
            ç¨äºæåæ¬å­ð¥µæ é¢å³é®è¯ç NoneBot2 æä»¶
-                                [pypi] [python]
+                                [PyPI] [python]
 **å®è£æ¹æ³** ä½¿ç¨ä»¥ä¸å½ä»¤ä¹ä¸å¿«éå®è£ï¼ ``` nb plugin install
-nonebot_plugin_herocard pip install --upgrade nonebot_plugin_herocard ```
+nonebot-plugin-herocard pip install --upgrade nonebot-plugin-herocard ```
 éå¯ Bot å³å¯ä½éªæ­¤æä»¶ã **ä½¿ç¨æ¹æ³** - åé `
 [ä½èãã]ãã¼ã[ä¸­å½ç¿»è¨³] [DLç]`æ ¼å¼æ¶æ¯å³å¯æ¶å°åå¤ -
 åé `(2020 Summer)ãã¼ã(subtitle) (31P)
 (å®)`æ ¼å¼æ¶æ¯å³å¯æ¶å°åå¤ *\*
 æä»¶ååºåºäºæ­£åå¹éï¼æä»¥ï¼çè³`åé¦lz
 [ä½èãã]ãã¼ã (31P)ææè§å¾é¡¶`è¿æ ·çæä»¤é½å¯ç¨ï¼* -
 **æ³¨æï¼** 1. åéæ¶æ¯ä¸­**ä¸å®**è¦åå«**æ¥æåå**ï¼ä¸è®º
 *å¹³åå* è¿æ¯ *çåå* ï¼å¦åæä»¶ä¸çæ 2.
 è¥åºç°`None`åå¤ææ¯`ä¸åå¤`ï¼å¯ä»¥èèå¨æ¨**æ³è¦æåææ¬**çååå ä¸`ã`/
 `.` =>ä¸­è±æå¥å·åå¯ **ç¹å«é¸£è°¢** [@nonebot/nonebot2](https://
 github.com/nonebot/nonebot2/) | [@Mrs4s/go-cqhttp](https://github.com/Mrs4s/go-
 cqhttp) | [@monsterxcn/nonebot_plugin_epicfree](https://github.com/monsterxcn/
 nonebot_plugin_epicfree) >
 æ°äººãããâ¡ä¸æï¼ä»£ç åççï¼æå¥½å«æææè½ä¿®ä»ä¹bugï¼Cialloï½
-(â ã»Ï< )ââ **æ´æ°æ¥å¿** `1.0.0` é¦æ¬¡åå¸ï¼å®åäºREADME.md
+(â ã»Ï< )ââ **æ´æ°æ¥å¿** `1.0.2` ä¿®å¤ä¸ç¹README.mdé®é¢ `1.0.1`
+ä¿®å¤ä¸ç¹README.mdé®é¢ `1.0.0` é¦æ¬¡åå¸ï¼å®åäºREADME.md
```

### Comparing `nonebot_plugin_herocard-1.0.0/README.md` & `nonebot_plugin_herocard-1.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <h1 align="center">NoneBot Plugin HeroCard</h1></br>
 
 <p align="center"> 用于提取本子🥵标题关键词的 NoneBot2 插件</p></br>
 
 <p align="center">
-  <a href="https://pypi.python.org/pypi/nonebot_plugin_herocard">
-    <img src="https://img.shields.io/pypi/v/nonebot_plugin_herocard?style=flat-square" alt="pypi">
+  <a href="https://pypi.python.org/pypi/nonebot-plugin-herocard">
+    <img alt="PyPI" src="https://img.shields.io/pypi/v/nonebot-plugin-herocard?color=%23da3f3d">
   </a>
   <img src="https://img.shields.io/badge/python-3.9-blue?style=flat" alt="python"><br />
 </p></br>
 
 **安装方法**
 
 使用以下命令之一快速安装：
 
 ``` 
-nb plugin install nonebot_plugin_herocard
+nb plugin install nonebot-plugin-herocard
 
-pip install --upgrade nonebot_plugin_herocard
+pip install --upgrade nonebot-plugin-herocard
 ```
 重启 Bot 即可体验此插件。
 
 **使用方法**
 
  - 发送 `[作者さん]テーマ[中国翻訳] [DL版]`格式消息即可收到回复
  - 发送 `(2020 Summer)テーマ(subtitle) (31P) (完)`格式消息即可收到回复
@@ -36,8 +36,12 @@
 [@nonebot/nonebot2](https://github.com/nonebot/nonebot2/) | [@Mrs4s/go-cqhttp](https://github.com/Mrs4s/go-cqhttp) | [@monsterxcn/nonebot_plugin_epicfree](https://github.com/monsterxcn/nonebot_plugin_epicfree) 
 
 
 > 新人ざぁこ♡一枚，代码写的烂，最好别指望我能修什么bug！Ciallo～(∠・ω< )⌒☆
 
 **更新日志**
 
+`1.0.2` 修复一点README.md问题
+
+`1.0.1` 修复一点README.md问题
+
 `1.0.0` 首次发布，完善了README.md
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
                      ****** NoneBot Plugin HeroCard ******
            ç¨äºæåæ¬å­ð¥µæ é¢å³é®è¯ç NoneBot2 æä»¶
-                                [pypi] [python]
+                                [PyPI] [python]
 **å®è£æ¹æ³** ä½¿ç¨ä»¥ä¸å½ä»¤ä¹ä¸å¿«éå®è£ï¼ ``` nb plugin install
-nonebot_plugin_herocard pip install --upgrade nonebot_plugin_herocard ```
+nonebot-plugin-herocard pip install --upgrade nonebot-plugin-herocard ```
 éå¯ Bot å³å¯ä½éªæ­¤æä»¶ã **ä½¿ç¨æ¹æ³** - åé `
 [ä½èãã]ãã¼ã[ä¸­å½ç¿»è¨³] [DLç]`æ ¼å¼æ¶æ¯å³å¯æ¶å°åå¤ -
 åé `(2020 Summer)ãã¼ã(subtitle) (31P)
 (å®)`æ ¼å¼æ¶æ¯å³å¯æ¶å°åå¤ *\*
 æä»¶ååºåºäºæ­£åå¹éï¼æä»¥ï¼çè³`åé¦lz
 [ä½èãã]ãã¼ã (31P)ææè§å¾é¡¶`è¿æ ·çæä»¤é½å¯ç¨ï¼* -
 **æ³¨æï¼** 1. åéæ¶æ¯ä¸­**ä¸å®**è¦åå«**æ¥æåå**ï¼ä¸è®º
 *å¹³åå* è¿æ¯ *çåå* ï¼å¦åæä»¶ä¸çæ 2.
 è¥åºç°`None`åå¤ææ¯`ä¸åå¤`ï¼å¯ä»¥èèå¨æ¨**æ³è¦æåææ¬**çååå ä¸`ã`/
 `.` =>ä¸­è±æå¥å·åå¯ **ç¹å«é¸£è°¢** [@nonebot/nonebot2](https://
 github.com/nonebot/nonebot2/) | [@Mrs4s/go-cqhttp](https://github.com/Mrs4s/go-
 cqhttp) | [@monsterxcn/nonebot_plugin_epicfree](https://github.com/monsterxcn/
 nonebot_plugin_epicfree) >
 æ°äººãããâ¡ä¸æï¼ä»£ç åççï¼æå¥½å«æææè½ä¿®ä»ä¹bugï¼Cialloï½
-(â ã»Ï< )ââ **æ´æ°æ¥å¿** `1.0.0` é¦æ¬¡åå¸ï¼å®åäºREADME.md
+(â ã»Ï< )ââ **æ´æ°æ¥å¿** `1.0.2` ä¿®å¤ä¸ç¹README.mdé®é¢ `1.0.1`
+ä¿®å¤ä¸ç¹README.mdé®é¢ `1.0.0` é¦æ¬¡åå¸ï¼å®åäºREADME.md
```

### Comparing `nonebot_plugin_herocard-1.0.0/nonebot_plugin_herocard/__init__.py` & `nonebot_plugin_herocard-1.0.2/nonebot_plugin_herocard/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_herocard-1.0.0/nonebot_plugin_herocard.egg-info/PKG-INFO` & `nonebot_plugin_herocard-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
-Name: nonebot-plugin-herocard
-Version: 1.0.0
+Name: nonebot_plugin_herocard
+Version: 1.0.2
 Summary: nonebot小插件，提供简单的文本提取功能
 Author: Xie-Tiao
 Author-email: 1183004468@qq.com
 Keywords: python,hero,nonebot,nonebot2,tieba,hiragana,katakana,benzi
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 
 <h1 align="center">NoneBot Plugin HeroCard</h1></br>
 
 <p align="center"> 用于提取本子🥵标题关键词的 NoneBot2 插件</p></br>
 
 <p align="center">
-  <a href="https://pypi.python.org/pypi/nonebot_plugin_herocard">
-    <img src="https://img.shields.io/pypi/v/nonebot_plugin_herocard?style=flat-square" alt="pypi">
+  <a href="https://pypi.python.org/pypi/nonebot-plugin-herocard">
+    <img alt="PyPI" src="https://img.shields.io/pypi/v/nonebot-plugin-herocard?color=%23da3f3d">
   </a>
   <img src="https://img.shields.io/badge/python-3.9-blue?style=flat" alt="python"><br />
 </p></br>
 
 **安装方法**
 
 使用以下命令之一快速安装：
 
 ``` 
-nb plugin install nonebot_plugin_herocard
+nb plugin install nonebot-plugin-herocard
 
-pip install --upgrade nonebot_plugin_herocard
+pip install --upgrade nonebot-plugin-herocard
 ```
 重启 Bot 即可体验此插件。
 
 **使用方法**
 
  - 发送 `[作者さん]テーマ[中国翻訳] [DL版]`格式消息即可收到回复
  - 发送 `(2020 Summer)テーマ(subtitle) (31P) (完)`格式消息即可收到回复
@@ -48,8 +48,12 @@
 [@nonebot/nonebot2](https://github.com/nonebot/nonebot2/) | [@Mrs4s/go-cqhttp](https://github.com/Mrs4s/go-cqhttp) | [@monsterxcn/nonebot_plugin_epicfree](https://github.com/monsterxcn/nonebot_plugin_epicfree) 
 
 
 > 新人ざぁこ♡一枚，代码写的烂，最好别指望我能修什么bug！Ciallo～(∠・ω< )⌒☆
 
 **更新日志**
 
+`1.0.2` 修复一点README.md问题
+
+`1.0.1` 修复一点README.md问题
+
 `1.0.0` 首次发布，完善了README.md
```

#### html2text {}

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-herocard Version: 1.0.0 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_herocard Version: 1.0.2 Summary:
 nonebotå°æä»¶ï¼æä¾ç®åçææ¬æååè½ Author: Xie-Tiao Author-
 email: 1183004468@qq.com Keywords:
 python,hero,nonebot,nonebot2,tieba,hiragana,katakana,benzi Classifier:
 Programming Language :: Python :: 3.9 Classifier: Operating System :: Microsoft
 :: Windows Description-Content-Type: text/markdown
                      ****** NoneBot Plugin HeroCard ******
            ç¨äºæåæ¬å­ð¥µæ é¢å³é®è¯ç NoneBot2 æä»¶
-                                [pypi] [python]
+                                [PyPI] [python]
 **å®è£æ¹æ³** ä½¿ç¨ä»¥ä¸å½ä»¤ä¹ä¸å¿«éå®è£ï¼ ``` nb plugin install
-nonebot_plugin_herocard pip install --upgrade nonebot_plugin_herocard ```
+nonebot-plugin-herocard pip install --upgrade nonebot-plugin-herocard ```
 éå¯ Bot å³å¯ä½éªæ­¤æä»¶ã **ä½¿ç¨æ¹æ³** - åé `
 [ä½èãã]ãã¼ã[ä¸­å½ç¿»è¨³] [DLç]`æ ¼å¼æ¶æ¯å³å¯æ¶å°åå¤ -
 åé `(2020 Summer)ãã¼ã(subtitle) (31P)
 (å®)`æ ¼å¼æ¶æ¯å³å¯æ¶å°åå¤ *\*
 æä»¶ååºåºäºæ­£åå¹éï¼æä»¥ï¼çè³`åé¦lz
 [ä½èãã]ãã¼ã (31P)ææè§å¾é¡¶`è¿æ ·çæä»¤é½å¯ç¨ï¼* -
 **æ³¨æï¼** 1. åéæ¶æ¯ä¸­**ä¸å®**è¦åå«**æ¥æåå**ï¼ä¸è®º
 *å¹³åå* è¿æ¯ *çåå* ï¼å¦åæä»¶ä¸çæ 2.
 è¥åºç°`None`åå¤ææ¯`ä¸åå¤`ï¼å¯ä»¥èèå¨æ¨**æ³è¦æåææ¬**çååå ä¸`ã`/
 `.` =>ä¸­è±æå¥å·åå¯ **ç¹å«é¸£è°¢** [@nonebot/nonebot2](https://
 github.com/nonebot/nonebot2/) | [@Mrs4s/go-cqhttp](https://github.com/Mrs4s/go-
 cqhttp) | [@monsterxcn/nonebot_plugin_epicfree](https://github.com/monsterxcn/
 nonebot_plugin_epicfree) >
 æ°äººãããâ¡ä¸æï¼ä»£ç åççï¼æå¥½å«æææè½ä¿®ä»ä¹bugï¼Cialloï½
-(â ã»Ï< )ââ **æ´æ°æ¥å¿** `1.0.0` é¦æ¬¡åå¸ï¼å®åäºREADME.md
+(â ã»Ï< )ââ **æ´æ°æ¥å¿** `1.0.2` ä¿®å¤ä¸ç¹README.mdé®é¢ `1.0.1`
+ä¿®å¤ä¸ç¹README.mdé®é¢ `1.0.0` é¦æ¬¡åå¸ï¼å®åäºREADME.md
```

### Comparing `nonebot_plugin_herocard-1.0.0/setup.py` & `nonebot_plugin_herocard-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # these things are needed for the README.md show on pypi (if you dont need delete it)
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 # you need to change all these
-VERSION = '1.0.0'
+VERSION = '1.0.2'
 DESCRIPTION = 'nonebot小插件，提供简单的文本提取功能'
 LONG_DESCRIPTION = 'nonebot插件【herocard】，用于提取含“平假名/片假名”文本中的关键文本，使用方法详见README.md'
 
 setup(
     name="nonebot_plugin_herocard",
     version=VERSION,
     author="Xie-Tiao",
```

