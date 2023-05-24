# Comparing `tmp/hiyobot-0.2.4.tar.gz` & `tmp/hiyobot-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiyobot-0.2.4.tar", last modified: Sun May 21 12:16:14 2023, max compression
+gzip compressed data, was "hiyobot-0.2.5.tar", last modified: Wed May 24 13:16:18 2023, max compression
```

## Comparing `hiyobot-0.2.4.tar` & `hiyobot-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:16:14.042590 hiyobot-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-21 12:16:00.000000 hiyobot-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-21 12:16:14.042590 hiyobot-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-21 12:16:00.000000 hiyobot-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:16:14.038589 hiyobot-0.2.4/hiyobot/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-21 12:16:00.000000 hiyobot-0.2.4/hiyobot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:16:14.042590 hiyobot-0.2.4/hiyobot/hackchat/
--rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-05-21 12:16:00.000000 hiyobot-0.2.4/hiyobot/hackchat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:16:14.042590 hiyobot-0.2.4/hiyobot/zhangchat/
--rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-05-21 12:16:00.000000 hiyobot-0.2.4/hiyobot/zhangchat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:16:14.042590 hiyobot-0.2.4/hiyobot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-21 12:16:14.000000 hiyobot-0.2.4/hiyobot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-21 12:16:14.000000 hiyobot-0.2.4/hiyobot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 12:16:14.000000 hiyobot-0.2.4/hiyobot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-21 12:16:14.000000 hiyobot-0.2.4/hiyobot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-21 12:16:14.000000 hiyobot-0.2.4/hiyobot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 12:16:14.042590 hiyobot-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-21 12:16:00.000000 hiyobot-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:16:18.870009 hiyobot-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-24 13:16:07.000000 hiyobot-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-24 13:16:18.870009 hiyobot-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-24 13:16:07.000000 hiyobot-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:16:18.870009 hiyobot-0.2.5/hiyobot/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 13:16:07.000000 hiyobot-0.2.5/hiyobot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:16:18.870009 hiyobot-0.2.5/hiyobot/hackchat/
+-rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-05-24 13:16:07.000000 hiyobot-0.2.5/hiyobot/hackchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-24 13:16:07.000000 hiyobot-0.2.5/hiyobot/hc-wait4inp.test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:16:18.870009 hiyobot-0.2.5/hiyobot/zhangchat/
+-rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-05-24 13:16:07.000000 hiyobot-0.2.5/hiyobot/zhangchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-24 13:16:07.000000 hiyobot-0.2.5/hiyobot/zhc-wait4inp.test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:16:18.870009 hiyobot-0.2.5/hiyobot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-24 13:16:18.000000 hiyobot-0.2.5/hiyobot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-24 13:16:18.000000 hiyobot-0.2.5/hiyobot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:16:18.000000 hiyobot-0.2.5/hiyobot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-24 13:16:18.000000 hiyobot-0.2.5/hiyobot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 13:16:18.000000 hiyobot-0.2.5/hiyobot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 13:16:18.870009 hiyobot-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-24 13:16:07.000000 hiyobot-0.2.5/setup.py
```

### Comparing `hiyobot-0.2.4/LICENSE` & `hiyobot-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hiyobot-0.2.4/PKG-INFO` & `hiyobot-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiyobot
-Version: 0.2.4
+Version: 0.2.5
 Summary: A simple bot framework for Hack.chat.
 Home-page: https://github.com/Hiyoteam/hiyobot
 Author: MaggieLOL
 Author-email: tanhanzesnd@gmail.com
 License: GPL-2.0
 Keywords: bot hack.chat hack.chat-bot
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hiyobot-0.2.4/README.md` & `hiyobot-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `hiyobot-0.2.4/hiyobot/hackchat/__init__.py` & `hiyobot-0.2.5/hiyobot/hackchat/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import websocket,ssl,json,threading,uuid,time,logging,re,traceback,inspect,asyncio
+import websocket,ssl,json,threading,uuid,time,logging,re,traceback,inspect,asyncio,queue
 from functools import wraps
-HIYOBOT_VERSION=(0,2,4)
+HIYOBOT_VERSION=(0,2,5)
 MAX_RECV_LOG_LIMIT=100 #0 for no limit
 def _isasync(func):
     if inspect.isasyncgenfunction(func) or inspect.iscoroutinefunction(func):
         return True
     else:
         return False
 class Bot:
@@ -108,15 +108,15 @@
                 else:
                     logging.debug(f"Recv: {dumped}")
                 session=Session(self,data)
                 logging.debug(f"Matching Checks....")
                 for check in self.checks:
                     if check[0].match_all(data):
                         logging.debug(f"Matched!")
-                        check[1](check[2],session)
+                        check[1](Data(data),check[2],session)
                         self.checks.remove(check)
                     logging.debug(f"Skipping event matching because check has matched.")
                     continue
                 logging.debug(f"Matching Event in {len(self.events)} Events...")
                 for event in self.events:
                     try:
                         event(data=Data(data),session=session)
@@ -231,38 +231,56 @@
     def export(self):
         return [self.protocol,self.host,self.port]
 class Session:
     def __init__(self,bot,data):
         logging.debug(f"Built session(bot={bot})")
         self.bot=bot
         self.data=data
-        self.extra_datas={}
         self.created_on=time.time()
         self.sessionID=str(uuid.uuid4())
-    def wait_for_input(self,prompt=None,expires=60,delay=100):
-        self.extra_datas["waitforinput"]=False
+    def wait_for_input(self,prompt=None,expires=60,checkrule=["chat","whisper"]):
+        """
+        Wait for user input, timeout in 60s.
+        """
         if prompt:
             self.bot.send(prompt)
         #bind checker
         nick=self.data["nick"]
-        checker=Matcher(Matchers.nick(nick))
-        def check(session,newsession):
+        checker=Matcher(lambda x:(x.get("cmd") == "chat" and x.get("nick") == nick) or (x.get("cmd") == "info" and x.get("type") == "whisper" and x.get("from") == nick) or (x.get("cmd") == "onlineRemove" and x.get("nick") == nick))
+        callbackq=queue.Queue()
+        def check(data,session,newsession):
             #checked:
             logging.debug(f"Callback running: {session} and new one {newsession}")
-            session.extra_datas["waitforinput"]=newsession.data.get("text")
+            if data.cmd == "onlineRemove":
+                logging.debug("Target left, kill session.")
+                callbackq.put([1]) #1=expire
+                return
+            
+            #extract
+            if data.cmd == "chat" and "chat" in checkrule:
+                #public msg
+                content=data.text
+            elif data.cmd == "info" and "whisper" in checkrule:
+                #private msg
+                content=data.text.split(" whispered: ",1)[1]
+            else:
+                #what the hell was that
+                raise NotImplementedError("Unknown message type")
+            callbackq.put([0,content,data])
         self.bot.checks.append((checker,check,self))
-        stt=time.time()
-        while (time.time()-stt)<expires:
-            time.sleep(delay/1000)
-            if self.extra_datas["waitforinput"]:
-                logging.debug("Got message!")
-                return self.extra_datas["waitforinput"]
-        logging.debug("Session expired.")
-        self.extra_datas["waitforinput"]=False
-        raise TimeoutError("Session expired.")
+        try:
+            data=callbackq.get(timeout=expires)
+            if data[0] == 0:
+                return data[1],data[2]
+            if data[0] == 1:
+                #what the hell was thatagain?
+                raise NotImplementedError("Unknown callback status")
+        except:
+            logging.debug("Session expired.")
+            raise TimeoutError("Session expired.")
 
 class Plugin:
     def __init__(self):
         self.commands=[]
     def build_event(self,matcher):
         logging.debug(f"Built event for plugin {self}")
         def decorate(func):
```

### Comparing `hiyobot-0.2.4/hiyobot/zhangchat/__init__.py` & `hiyobot-0.2.5/hiyobot/zhangchat/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import websocket,ssl,json,threading,uuid,time,logging,re,traceback,inspect,asyncio
+import websocket,ssl,json,threading,uuid,time,logging,re,traceback,inspect,asyncio,queue
 from functools import wraps
-HIYOBOT_VERSION=(0,2,4)
+HIYOBOT_VERSION=(0,2,5)
 MAX_RECV_LOG_LIMIT=100 #0 for no limit
 def _isasync(func):
     if inspect.isasyncgenfunction(func) or inspect.iscoroutinefunction(func):
         return True
     else:
         return False
 class Bot:
@@ -108,15 +108,15 @@
                 else:
                     logging.debug(f"Recv: {dumped}")
                 session=Session(self,data)
                 logging.debug(f"Matching Checks....")
                 for check in self.checks:
                     if check[0].match_all(data):
                         logging.debug(f"Matched!")
-                        check[1](check[2],session)
+                        check[1](Data(data),check[2],session)
                         self.checks.remove(check)
                     logging.debug(f"Skipping event matching because check has matched.")
                     continue
                 logging.debug(f"Matching Event in {len(self.events)} Events...")
                 for event in self.events:
                     try:
                         event(data=Data(data),session=session)
@@ -234,35 +234,54 @@
     def __init__(self,bot,data):
         logging.debug(f"Built session(bot={bot})")
         self.bot=bot
         self.data=data
         self.extra_datas={}
         self.created_on=time.time()
         self.sessionID=str(uuid.uuid4())
-    def wait_for_input(self,prompt=None,expires=60,delay=100):
-        self.extra_datas["waitforinput"]=False
+    def wait_for_input(self,prompt=None,expires=60,checkrule=["chat","whisper"]):
+        """
+        Wait for user input, timeout in 60s.
+        """
         if prompt:
             self.bot.send(prompt)
         #bind checker
         nick=self.data["nick"]
-        checker=Matcher(Matchers.nick(nick))
-        def check(session,newsession):
+        checker=Matcher(lambda x:(x.get("cmd") == "chat" and x.get("nick") == nick) or (x.get("cmd") == "info" and x.get("type") == "whisper" and x.get("from") == nick) or (x.get("cmd") == "onlineRemove" and x.get("nick") == nick))
+        callbackq=queue.Queue()
+        def check(data,session,newsession):
             #checked:
             logging.debug(f"Callback running: {session} and new one {newsession}")
-            session.extra_datas["waitforinput"]=newsession.data.get("text")
+            if data.cmd == "onlineRemove":
+                logging.debug("Target left, kill session.")
+                callbackq.put([1]) #1=expire
+                return
+            
+            #extract
+            if data.cmd == "chat" and "chat" in checkrule:
+                #public msg
+                content=data.text
+            elif data.cmd == "info" and "whisper" in checkrule:
+                #private msg
+                content=data.text.split(" 向你发送私信：",1)[1]
+            else:
+                #what the hell was that
+                raise NotImplementedError("Unknown message type")
+            callbackq.put([0,content,data])
         self.bot.checks.append((checker,check,self))
-        stt=time.time()
-        while (time.time()-stt)<expires:
-            time.sleep(delay/1000)
-            if self.extra_datas["waitforinput"]:
-                logging.debug("Got message!")
-                return self.extra_datas["waitforinput"]
-        logging.debug("Session expired.")
-        self.extra_datas["waitforinput"]=False
-        raise TimeoutError("Session expired.")
+        try:
+            data=callbackq.get(timeout=expires)
+            if data[0] == 0:
+                return data[1],data[2]
+            if data[0] == 1:
+                #what the hell was thatagain?
+                raise NotImplementedError("Unknown callback status")
+        except:
+            logging.debug("Session expired.")
+            raise TimeoutError("Session expired.")
 
 class Plugin:
     def __init__(self):
         self.commands=[]
     def build_event(self,matcher):
         logging.debug(f"Built event for plugin {self}")
         def decorate(func):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hiyobot-0.2.4/hiyobot.egg-info/PKG-INFO` & `hiyobot-0.2.5/hiyobot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiyobot
-Version: 0.2.4
+Version: 0.2.5
 Summary: A simple bot framework for Hack.chat.
 Home-page: https://github.com/Hiyoteam/hiyobot
 Author: MaggieLOL
 Author-email: tanhanzesnd@gmail.com
 License: GPL-2.0
 Keywords: bot hack.chat hack.chat-bot
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hiyobot-0.2.4/setup.py` & `hiyobot-0.2.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hiyobot', # 你的项目名称
-    version="0.2.4", # 你的项目版本
+    version="0.2.5", # 你的项目版本
     description='A simple bot framework for Hack.chat.', # 你的项目简介
     long_description=open('README.md').read(), # 你的项目详细介绍，一般从README.md文件中读取
     long_description_content_type='text/markdown', # 你的项目详细介绍的格式，一般为markdown格式
     url='https://github.com/Hiyoteam/hiyobot', # 你的项目主页，一般为github仓库地址
     author='MaggieLOL', # 你的姓名或者团队名称
     author_email='tanhanzesnd@gmail.com', # 你的邮箱或者团队邮箱
     license='GPL-2.0', # 你的项目使用的许可证，一般为MIT或者其他开源许可证
@@ -14,15 +14,15 @@
         'Development Status :: 3 - Alpha', # 开发状态，一般为Alpha（初级）、Beta（中级）或者Stable（稳定）
         'Intended Audience :: Developers', # 目标受众，一般为Developers（开发者）、End Users/Desktop（桌面端用户）等
         'Topic :: Software Development :: Libraries :: Python Modules', # 主题，一般为Software Development（软件开发）、Scientific/Engineering（科学/工程）等
         'Programming Language :: Python :: 3', # 编程语言，一般为Python :: 3或者Python :: 2
         'Programming Language :: Python :: 3.10', # 编程语言的具体版本，根据你的项目支持的python版本选择
     ],
     keywords='bot hack.chat hack.chat-bot', # 一些关键词，用于描述你的项目特点或者功能
-    packages=find_packages(include="*"), # 需要打包的python模块，一般使用find_packages函数自动查找，排除测试模块等不需要打包的模块
+    packages=find_packages(include="*",exclude=["*.test.py"]), # 需要打包的python模块，一般使用find_packages函数自动查找，排除测试模块等不需要打包的模块
     install_requires="""cffi==1.15.1
 gevent==22.10.2
 greenlet==2.0.2
 pycparser==2.21
 websocket==0.2.1
 zope.event==4.6
 zope.interface==6.0""".splitlines(),
```

