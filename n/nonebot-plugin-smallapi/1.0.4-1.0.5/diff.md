# Comparing `tmp/nonebot_plugin_smallapi-1.0.4.tar.gz` & `tmp/nonebot_plugin_smallapi-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_smallapi-1.0.4.tar", last modified: Tue May 23 15:23:11 2023, max compression
+gzip compressed data, was "nonebot_plugin_smallapi-1.0.5.tar", last modified: Tue May 23 22:20:36 2023, max compression
```

## Comparing `nonebot_plugin_smallapi-1.0.4.tar` & `nonebot_plugin_smallapi-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:23:11.667311 nonebot_plugin_smallapi-1.0.4/
--rwxr-xr-x   0 root         (0) root         (0)     1072 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      484 2023-05-23 15:23:11.667311 nonebot_plugin_smallapi-1.0.4/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     4993 2023-05-23 15:19:42.000000 nonebot_plugin_smallapi-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:23:11.664311 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/
--rw-r--r--   0 root         (0) root         (0)      503 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1980 2023-05-23 15:12:35.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/api_menu.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-05-23 15:00:36.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/api_pic.py
--rw-r--r--   0 root         (0) root         (0)     5426 2023-05-23 15:11:46.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/api_site.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-05-23 15:05:23.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/api_text.py
--rw-r--r--   0 root         (0) root         (0)     2204 2023-05-23 15:01:55.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/hander.py
--rw-r--r--   0 root         (0) root         (0)     1940 2023-05-23 15:02:43.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/hander_site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:23:11.666311 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      484 2023-05-23 15:23:11.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2023-05-23 15:23:11.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 15:23:11.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-05-23 15:23:11.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-23 15:23:11.000000 nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)      918 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 15:23:11.667311 nonebot_plugin_smallapi-1.0.4/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1074 2023-05-23 15:14:44.000000 nonebot_plugin_smallapi-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 22:20:36.701962 nonebot_plugin_smallapi-1.0.5/
+-rwxr-xr-x   0 root         (0) root         (0)     1072 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      484 2023-05-23 22:20:36.699962 nonebot_plugin_smallapi-1.0.5/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     5066 2023-05-23 22:16:25.000000 nonebot_plugin_smallapi-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 22:20:36.695962 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/
+-rw-r--r--   0 root         (0) root         (0)      503 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1980 2023-05-23 15:12:35.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/api_menu.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-05-23 15:00:36.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/api_pic.py
+-rw-r--r--   0 root         (0) root         (0)     6026 2023-05-23 22:13:37.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/api_site.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-05-23 15:05:23.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/api_text.py
+-rw-r--r--   0 root         (0) root         (0)     2204 2023-05-23 15:01:55.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/hander.py
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-05-23 15:02:43.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/hander_site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 22:20:36.698962 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      484 2023-05-23 22:20:36.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2023-05-23 22:20:36.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 22:20:36.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-05-23 22:20:36.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-23 22:20:36.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)      921 2023-05-23 22:18:40.000000 nonebot_plugin_smallapi-1.0.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 22:20:36.701962 nonebot_plugin_smallapi-1.0.5/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1074 2023-05-23 22:14:40.000000 nonebot_plugin_smallapi-1.0.5/setup.py
```

### Comparing `nonebot_plugin_smallapi-1.0.4/LICENSE` & `nonebot_plugin_smallapi-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.4/README.md` & `nonebot_plugin_smallapi-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 ## 📝 更新日志
 
 <details>
 <summary>展开/收起</summary>
 
 ### 1.0.0
 
--
+- 插件初次发布
 
 ### 1.0.1
 
 - 修复依赖问题  
 
 ### 1.0.2
   
@@ -145,12 +145,17 @@
 ### 1.0.3  
   
 - 梅开三度，终于修好了依赖
 
 ### 1.0.4
 
 - 更换稳定API, 修复部分Bug
+
+### 1.0.5
+
+- 修复ip查询中的致命语法错误
+
 </details>
 
 ## 致谢
 - [借鉴的代码](https://github.com/lgc-NB2Dev/ShigureBot/blob/main/src/plugins/shigure_bot/plugins/site_tool/__main__.py)
 - [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template)
```

#### html2text {}

```diff
@@ -36,13 +36,14 @@
 å¥½ä½¿çç½ç«å·¥å·ç³»ç» ## ð å½ä»¤ PS:
 è¯·æ¥çä½ envä¸­èµ·å§ç¬¦çéç½®(é»è®¤```/```) 1. APIå¾çç³»ç»
 (å¾çç³»ç») 2. APIæå­ç³»ç»(æå­ç³»ç») 3. APIç«ç¹ç³»ç»
 (ç«ç¹ç³»ç») ### APIå¾çç³»ç» å½ä»¤ç»æï¼```(/)APIå¾çç³»ç»```
 ä¾å¦ï¼```APIå¾çç³»ç»``` ### APIæå­ç³»ç» å½ä»¤ç»æï¼```(/
 )APIæå­ç³»ç»``` ä¾å¦ï¼```APIæå­ç³»ç»``` ### APIç«ç¹ç³»ç»
 å½ä»¤ç»æï¼```(/)APIç«ç¹ç³»ç»``` ä¾å¦ï¼```APIç«ç¹ç³»ç»``` ## â
-æå± è¿æ²¡æå¢ï½ ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 1.0.0 - ###
-1.0.1 - ä¿®å¤ä¾èµé®é¢ ### 1.0.2 - æ¢å¼äºåº¦ ### 1.0.3 -
-æ¢å¼ä¸åº¦ï¼ç»äºä¿®å¥½äºä¾èµ ### 1.0.4 - æ´æ¢ç¨³å®API,
-ä¿®å¤é¨åBug  ## è´è°¢ - [åé´çä»£ç ](https://github.com/lgc-NB2Dev/
-ShigureBot/blob/main/src/plugins/shigure_bot/plugins/site_tool/__main__.py) -
-[nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template)
+æå± è¿æ²¡æå¢ï½ ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 1.0.0 -
+æä»¶åæ¬¡åå¸ ### 1.0.1 - ä¿®å¤ä¾èµé®é¢ ### 1.0.2 - æ¢å¼äºåº¦ ###
+1.0.3 - æ¢å¼ä¸åº¦ï¼ç»äºä¿®å¥½äºä¾èµ ### 1.0.4 - æ´æ¢ç¨³å®API,
+ä¿®å¤é¨åBug ### 1.0.5 - ä¿®å¤ipæ¥è¯¢ä¸­çè´å½è¯­æ³éè¯¯  ## è´è°¢ -
+[åé´çä»£ç ](https://github.com/lgc-NB2Dev/ShigureBot/blob/main/src/
+plugins/shigure_bot/plugins/site_tool/__main__.py) - [nonebot-plugin-template]
+(https://github.com/A-kirami/nonebot-plugin-template)
```

### Comparing `nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/api_menu.py` & `nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/api_menu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/api_pic.py` & `nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/api_pic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/api_site.py` & `nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/api_site.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,42 @@
         await matcher.finish("请输入IP/域名")
 
     await matcher.finish(
         format_return(
             await get_api_resp("IP", {"ip": arg}),
             lambda ret_web: (
                 f'查询目标：{ret_web["ip"]}\n'
-                f'IP地址：{(ret_web["location"].get("ip"))}\n'
-                f'IP类型：{ret_web["isp"]}\n'
-                f'IP地区：{ret_web["country"]}\n'
-                f'IP段起始: {ret_web["range.start"]}\n'
-                f'IP段结束: {ret_web["range.end"]}'
-                f'更多信息：{ret_web["area"]}'
+                f'IP地址：{ret_web["location"].get("ip")}\n'
+                #f'IP类型：{ret_web["location"].get("isp")}\n'
+                f'IP地区：{ret_web["location"].get("country")}\n'
+                f'IP段起始: {ret_web["location"].get("range").get("start")}\n'
+                f'IP段结束: {ret_web["location"].get("range").get("end")}\n'
+                f'更多信息：{ret_web["location"].get("area")}'
             ),
         ),
         at_sender=True,
     )
+"""
+@on_command("网站测速", aliases={"web测速", "WEB测速"}).handle()
+@error_handle()
+async def _(matcher: Matcher, args: Message = CommandArg()):
+    if not (arg := args.extract_plain_text()):
+        await matcher.finish("请输入域名")
+
+    await matcher.finish(
+        format_return(
+            await get_api_resp("speed", {"url": "http://" + arg}),
+            lambda ret_web: (
+                f'访问速度：{ret_web}'
+                ),
+        ),
+        at_sender=True,
+    )
+"""
+
 
 @on_command("ping", aliases={"Ping", "PING"}).handle()
 @error_handle()
 async def _(matcher: Matcher, args: Message = CommandArg()):
     if not (arg := args.extract_plain_text()):
         await matcher.finish("请输入IP/域名")
```

### Comparing `nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/api_text.py` & `nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/api_text.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/hander.py` & `nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/hander.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi/hander_site.py` & `nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/hander_site.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.4/nonebot_plugin_smallapi.egg-info/SOURCES.txt` & `nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.4/pyproject.toml` & `nonebot_plugin_smallapi-1.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "nonebot_plugin_smallapi"
-version = "0.0.1"
-description = "高效，快速的小小API调用插件！"
+version = "1.0.5"
+description = "高效，快速的小小WEBAPI调用插件！"
 authors = ["Chaichaisi <chaichaisi@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_smallapi"}]
 homepage = "https://github.com/chaichaisi/nonebot_plugin_smallapi"
 repository = "https://github.com/chaichaisi/nonebot_plugin_smallapi"
 documentation = "https://github.com/chaichaisi/nonebot_plugin_smallapi/blob/master/README.md"
```

### Comparing `nonebot_plugin_smallapi-1.0.4/setup.py` & `nonebot_plugin_smallapi-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools #导入setuptools打包工具
 
 setuptools.setup(
     install_requires=['jsonpath','nonebot2[aiohttp]','nonebot-adapter-onebot','nonebot2[httpx]'],
     name="nonebot_plugin_smallapi", # 用自己的名替换其中的YOUR_USERNAME_
-    version="1.0.4",    #包版本号，便于维护版本
+    version="1.0.5",    #包版本号，便于维护版本
     author="Chaichaisi",    #作者，可以写自己的姓名
     author_email="chaichaisi@qq.com",    #作者联系方式，可写自己的邮箱地址
     description="A small nonebot_plugin_smallapi plugin",#包的简述
     long_description="come in to read more",    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/chaichaisi/nonebot_plugin_smallapi",    #自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

