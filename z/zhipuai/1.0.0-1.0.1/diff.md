# Comparing `tmp/zhipuai-1.0.0.tar.gz` & `tmp/zhipuai-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zhipuai-1.0.0.tar", last modified: Wed Apr 26 13:26:26 2023, max compression
+gzip compressed data, was "dist/zhipuai-1.0.1.tar", last modified: Wed May 24 11:25:36 2023, max compression
```

## Comparing `zhipuai-1.0.0.tar` & `zhipuai-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-04-26 13:26:26.290473 zhipuai-1.0.0/
--rw-r--r--   0 haowangai   (501) staff       (20)      525 2023-04-26 13:26:26.290280 zhipuai-1.0.0/PKG-INFO
--rw-r--r--   0 haowangai   (501) staff       (20)       11 2023-04-26 12:22:24.000000 zhipuai-1.0.0/README.md
--rw-r--r--   0 haowangai   (501) staff       (20)       38 2023-04-26 13:26:26.290526 zhipuai-1.0.0/setup.cfg
--rw-r--r--   0 haowangai   (501) staff       (20)      881 2023-04-26 13:26:17.000000 zhipuai-1.0.0/setup.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-04-26 13:26:26.287991 zhipuai-1.0.0/tests/
--rw-r--r--   0 haowangai   (501) staff       (20)        0 2023-04-26 12:22:24.000000 zhipuai-1.0.0/tests/__init__.py
--rw-r--r--   0 haowangai   (501) staff       (20)     2591 2023-04-26 12:29:07.000000 zhipuai-1.0.0/tests/test.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-04-26 13:26:26.288528 zhipuai-1.0.0/zhipuai/
--rw-r--r--   0 haowangai   (501) staff       (20)      272 2023-04-26 12:22:24.000000 zhipuai-1.0.0/zhipuai/__init__.py
--rw-r--r--   0 haowangai   (501) staff       (20)     1968 2023-04-26 12:22:24.000000 zhipuai-1.0.0/zhipuai/api_resource.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-04-26 13:26:26.290063 zhipuai-1.0.0/zhipuai/utils/
--rw-r--r--   0 haowangai   (501) staff       (20)        0 2023-04-26 12:22:24.000000 zhipuai-1.0.0/zhipuai/utils/__init__.py
--rw-r--r--   0 haowangai   (501) staff       (20)      131 2023-04-26 12:22:24.000000 zhipuai-1.0.0/zhipuai/utils/api_util.py
--rw-r--r--   0 haowangai   (501) staff       (20)     1758 2023-04-26 12:22:24.000000 zhipuai-1.0.0/zhipuai/utils/http_client.py
--rw-r--r--   0 haowangai   (501) staff       (20)      543 2023-04-26 12:22:24.000000 zhipuai-1.0.0/zhipuai/utils/jwt_token.py
--rw-r--r--   0 haowangai   (501) staff       (20)     4471 2023-04-26 12:22:24.000000 zhipuai-1.0.0/zhipuai/utils/sse_client.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-04-26 13:26:26.289256 zhipuai-1.0.0/zhipuai.egg-info/
--rw-r--r--   0 haowangai   (501) staff       (20)      525 2023-04-26 13:26:26.000000 zhipuai-1.0.0/zhipuai.egg-info/PKG-INFO
--rw-r--r--   0 haowangai   (501) staff       (20)      384 2023-04-26 13:26:26.000000 zhipuai-1.0.0/zhipuai.egg-info/SOURCES.txt
--rw-r--r--   0 haowangai   (501) staff       (20)        1 2023-04-26 13:26:26.000000 zhipuai-1.0.0/zhipuai.egg-info/dependency_links.txt
--rw-r--r--   0 haowangai   (501) staff       (20)       13 2023-04-26 13:26:26.000000 zhipuai-1.0.0/zhipuai.egg-info/requires.txt
--rw-r--r--   0 haowangai   (501) staff       (20)       14 2023-04-26 13:26:26.000000 zhipuai-1.0.0/zhipuai.egg-info/top_level.txt
+drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-05-24 11:25:36.823009 zhipuai-1.0.1/
+-rw-r--r--   0 haowangai   (501) staff       (20)      525 2023-05-24 11:25:36.822786 zhipuai-1.0.1/PKG-INFO
+-rw-r--r--   0 haowangai   (501) staff       (20)       11 2023-04-26 12:22:24.000000 zhipuai-1.0.1/README.md
+-rw-r--r--   0 haowangai   (501) staff       (20)       38 2023-05-24 11:25:36.823086 zhipuai-1.0.1/setup.cfg
+-rw-r--r--   0 haowangai   (501) staff       (20)      881 2023-05-24 11:13:26.000000 zhipuai-1.0.1/setup.py
+drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-05-24 11:25:36.820129 zhipuai-1.0.1/tests/
+-rw-r--r--   0 haowangai   (501) staff       (20)        0 2023-04-26 12:22:24.000000 zhipuai-1.0.1/tests/__init__.py
+-rw-r--r--   0 haowangai   (501) staff       (20)     1797 2023-05-24 11:24:35.000000 zhipuai-1.0.1/tests/test.py
+drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-05-24 11:25:36.820712 zhipuai-1.0.1/zhipuai/
+-rw-r--r--   0 haowangai   (501) staff       (20)      272 2023-04-26 12:22:24.000000 zhipuai-1.0.1/zhipuai/__init__.py
+-rw-r--r--   0 haowangai   (501) staff       (20)     1968 2023-04-26 12:22:24.000000 zhipuai-1.0.1/zhipuai/api_resource.py
+drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-05-24 11:25:36.822492 zhipuai-1.0.1/zhipuai/utils/
+-rw-r--r--   0 haowangai   (501) staff       (20)        0 2023-04-26 12:22:24.000000 zhipuai-1.0.1/zhipuai/utils/__init__.py
+-rw-r--r--   0 haowangai   (501) staff       (20)      131 2023-04-26 12:22:24.000000 zhipuai-1.0.1/zhipuai/utils/api_util.py
+-rw-r--r--   0 haowangai   (501) staff       (20)     1758 2023-04-26 12:22:24.000000 zhipuai-1.0.1/zhipuai/utils/http_client.py
+-rw-r--r--   0 haowangai   (501) staff       (20)      543 2023-05-24 11:11:12.000000 zhipuai-1.0.1/zhipuai/utils/jwt_token.py
+-rw-r--r--   0 haowangai   (501) staff       (20)     4471 2023-04-26 12:22:24.000000 zhipuai-1.0.1/zhipuai/utils/sse_client.py
+drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-05-24 11:25:36.821489 zhipuai-1.0.1/zhipuai.egg-info/
+-rw-r--r--   0 haowangai   (501) staff       (20)      525 2023-05-24 11:25:36.000000 zhipuai-1.0.1/zhipuai.egg-info/PKG-INFO
+-rw-r--r--   0 haowangai   (501) staff       (20)      384 2023-05-24 11:25:36.000000 zhipuai-1.0.1/zhipuai.egg-info/SOURCES.txt
+-rw-r--r--   0 haowangai   (501) staff       (20)        1 2023-05-24 11:25:36.000000 zhipuai-1.0.1/zhipuai.egg-info/dependency_links.txt
+-rw-r--r--   0 haowangai   (501) staff       (20)       13 2023-05-24 11:25:36.000000 zhipuai-1.0.1/zhipuai.egg-info/requires.txt
+-rw-r--r--   0 haowangai   (501) staff       (20)       14 2023-05-24 11:25:36.000000 zhipuai-1.0.1/zhipuai.egg-info/top_level.txt
```

### Comparing `zhipuai-1.0.0/PKG-INFO` & `zhipuai-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhipuai
-Version: 1.0.0
+Version: 1.0.1
 Summary: A SDK library for accessing big model apis from ZhipuAI
 Home-page: https://open.bigmodel.cn/
 Author: Zhipu AI
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `zhipuai-1.0.0/setup.py` & `zhipuai-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readme = readme_file.read()
 
 with open("requirements.txt") as requirements_file:
     requirements = requirements_file.read().splitlines()
 
 setup(
     name="zhipuai",
-    version="v1.0.0",
+    version="v1.0.1",
     description="A SDK library for accessing big model apis from ZhipuAI",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Zhipu AI",
     url="https://open.bigmodel.cn/",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `zhipuai-1.0.0/tests/test.py` & `zhipuai-1.0.1/tests/test.py`

 * *Files 27% similar despite different names*

```diff
@@ -37,19 +37,20 @@
             print(str[len(previous):], end="", flush=True)
         previous = str
 
     return print_diff
 
 
 if __name__ == "__main__":
-    zhipuai.api_key = ""
+    zhipuai.api_key = "98ecb12669e4427983de959c0a22061a.77f995116150f600"
     zhipuai.api_base = "https://test-maas.aminer.cn/stage-api/paas/v3/model-api"
+    '''
     response = zhipuai.APIResource.query_async_invoke_result("1014907516268634316357633")
     print(response)
-    '''
+   
     response = zhipuai.APIResource.invoke(
         model="title-creation",
         prompt="新闻 炸裂",
         topP=1,
         topK=3,
         temperature=1,
         presencePenalty=1,
@@ -57,32 +58,13 @@
         generatedLength=128,
     )
 
     print(response)
 
 
     '''
-'''
-client = zhipuai.APIResource.sse_invoke(model="chatGLM_6b_SSE", prompt="你都可以做些什么事",
-                                        history=[{"query": "你好", "answer": "我是人工智能助手"},
-                                                 {"query": "你叫什么名字", "answer": "我叫chatGLM"}]
-                                        )
-print_diff = prepare_print_diff(lambda e: e.data, lambda e: pprint.pprint(e.__dict__))
-print()
-print('Response: ')
-for event in client.events():
-    if (event.data):
-        event.data = punctuation_converse_auto(event.data)
-    if (event.event == "add"):
-        print_diff(event)
-    elif (event.event == "error"):
-        print_diff(event)
-    elif (event.event == "finish" or event.event == "interrupted"):
-        print_diff(event)
-    elif (event.event == "finish"):
-        print_diff(event)
-        print()
-
-    else:
-        pprint.pprint(event)
-print("-----finished--------")
-'''
+
+client = zhipuai.APIResource.invoke(
+    model="example-model",
+    prompt="人工智能"
+)
+print(client)
```

### Comparing `zhipuai-1.0.0/zhipuai/api_resource.py` & `zhipuai-1.0.1/zhipuai/api_resource.py`

 * *Files identical despite different names*

### Comparing `zhipuai-1.0.0/zhipuai/utils/http_client.py` & `zhipuai-1.0.1/zhipuai/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `zhipuai-1.0.0/zhipuai/utils/jwt_token.py` & `zhipuai-1.0.1/zhipuai/utils/jwt_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,9 +16,9 @@
         "timestamp": int(round(time.time() * 1000)),
     }
 
     return jwt.encode(
         payload,
         secret,
         algorithm="HS256",
-        headers={"alg": "HS256", "sign_type": "SING"},
+        headers={"alg": "HS256", "sign_type": "SIGN"},
     )
```

### Comparing `zhipuai-1.0.0/zhipuai/utils/sse_client.py` & `zhipuai-1.0.1/zhipuai/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `zhipuai-1.0.0/zhipuai.egg-info/PKG-INFO` & `zhipuai-1.0.1/zhipuai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhipuai
-Version: 1.0.0
+Version: 1.0.1
 Summary: A SDK library for accessing big model apis from ZhipuAI
 Home-page: https://open.bigmodel.cn/
 Author: Zhipu AI
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

