# Comparing `tmp/easy_gpt_utils-0.1.8.tar.gz` & `tmp/easy_gpt_utils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_gpt_utils-0.1.8.tar", last modified: Wed May 10 10:56:11 2023, max compression
+gzip compressed data, was "easy_gpt_utils-0.1.9.tar", last modified: Fri May 12 04:43:58 2023, max compression
```

## Comparing `easy_gpt_utils-0.1.8.tar` & `easy_gpt_utils-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-10 10:56:11.820075 easy_gpt_utils-0.1.8/
--rw-rw-r--   0 houwei    (1001) houwei    (1001)    11357 2023-05-08 01:56:20.000000 easy_gpt_utils-0.1.8/LICENSE
--rw-rw-r--   0 houwei    (1001) houwei    (1001)      761 2023-05-10 10:56:11.819075 easy_gpt_utils-0.1.8/PKG-INFO
--rw-rw-r--   0 houwei    (1001) houwei    (1001)      156 2023-05-08 01:56:20.000000 easy_gpt_utils-0.1.8/README.md
-drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-10 10:56:11.803075 easy_gpt_utils-0.1.8/easy_gpt_utils/
--rw-rw-r--   0 houwei    (1001) houwei    (1001)      130 2023-05-10 03:18:02.000000 easy_gpt_utils-0.1.8/easy_gpt_utils/__init__.py
--rw-r--r--   0 houwei    (1001) houwei    (1001)     5221 2023-05-10 10:36:22.000000 easy_gpt_utils-0.1.8/easy_gpt_utils/embedding.py
--rw-rw-r--   0 houwei    (1001) houwei    (1001)    40471 2023-05-10 10:55:14.000000 easy_gpt_utils-0.1.8/easy_gpt_utils/gpt.py
--rw-rw-r--   0 houwei    (1001) houwei    (1001)     5309 2023-05-10 03:32:16.000000 easy_gpt_utils-0.1.8/easy_gpt_utils/vector_database.py
-drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-10 10:56:11.807075 easy_gpt_utils-0.1.8/easy_gpt_utils.egg-info/
--rw-rw-r--   0 houwei    (1001) houwei    (1001)      761 2023-05-10 10:56:11.000000 easy_gpt_utils-0.1.8/easy_gpt_utils.egg-info/PKG-INFO
--rw-rw-r--   0 houwei    (1001) houwei    (1001)      453 2023-05-10 10:56:11.000000 easy_gpt_utils-0.1.8/easy_gpt_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 houwei    (1001) houwei    (1001)        1 2023-05-10 10:56:11.000000 easy_gpt_utils-0.1.8/easy_gpt_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 houwei    (1001) houwei    (1001)       22 2023-05-10 10:56:11.000000 easy_gpt_utils-0.1.8/easy_gpt_utils.egg-info/requires.txt
--rw-rw-r--   0 houwei    (1001) houwei    (1001)       34 2023-05-10 10:56:11.000000 easy_gpt_utils-0.1.8/easy_gpt_utils.egg-info/top_level.txt
-drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-10 10:56:11.817075 easy_gpt_utils-0.1.8/easy_gpt_utils_bak/
--rw-rw-r--   0 houwei    (1001) houwei    (1001)      130 2023-05-10 10:53:38.000000 easy_gpt_utils-0.1.8/easy_gpt_utils_bak/__init__.py
--rw-r--r--   0 houwei    (1001) houwei    (1001)     5221 2023-05-10 10:53:38.000000 easy_gpt_utils-0.1.8/easy_gpt_utils_bak/embedding.py
--rw-r--r--   0 houwei    (1001) houwei    (1001)    29324 2023-05-10 10:53:38.000000 easy_gpt_utils-0.1.8/easy_gpt_utils_bak/gpt.py
--rw-rw-r--   0 houwei    (1001) houwei    (1001)     5309 2023-05-10 10:53:38.000000 easy_gpt_utils-0.1.8/easy_gpt_utils_bak/vector_database.py
--rw-rw-r--   0 houwei    (1001) houwei    (1001)       38 2023-05-10 10:56:11.820075 easy_gpt_utils-0.1.8/setup.cfg
--rw-rw-r--   0 houwei    (1001) houwei    (1001)      803 2023-05-10 10:55:46.000000 easy_gpt_utils-0.1.8/setup.py
+drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-12 04:43:58.633231 easy_gpt_utils-0.1.9/
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)    11357 2023-05-08 01:56:20.000000 easy_gpt_utils-0.1.9/LICENSE
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)     1537 2023-05-12 04:43:58.633231 easy_gpt_utils-0.1.9/PKG-INFO
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)      932 2023-05-10 11:01:37.000000 easy_gpt_utils-0.1.9/README.md
+drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-12 04:43:58.605231 easy_gpt_utils-0.1.9/easy_gpt_utils/
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)      130 2023-05-10 03:18:02.000000 easy_gpt_utils-0.1.9/easy_gpt_utils/__init__.py
+-rw-r--r--   0 houwei    (1001) houwei    (1001)     6206 2023-05-12 04:40:57.000000 easy_gpt_utils-0.1.9/easy_gpt_utils/embedding.py
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)    28433 2023-05-12 04:32:17.000000 easy_gpt_utils-0.1.9/easy_gpt_utils/gpt.py
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)     5809 2023-05-12 04:00:37.000000 easy_gpt_utils-0.1.9/easy_gpt_utils/vector_database.py
+drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-12 04:43:58.623231 easy_gpt_utils-0.1.9/easy_gpt_utils.egg-info/
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)     1537 2023-05-12 04:43:58.000000 easy_gpt_utils-0.1.9/easy_gpt_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)      453 2023-05-12 04:43:58.000000 easy_gpt_utils-0.1.9/easy_gpt_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)        1 2023-05-12 04:43:58.000000 easy_gpt_utils-0.1.9/easy_gpt_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)       22 2023-05-12 04:43:58.000000 easy_gpt_utils-0.1.9/easy_gpt_utils.egg-info/requires.txt
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)       34 2023-05-12 04:43:58.000000 easy_gpt_utils-0.1.9/easy_gpt_utils.egg-info/top_level.txt
+drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-12 04:43:58.632231 easy_gpt_utils-0.1.9/easy_gpt_utils_bak/
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)      130 2023-05-10 10:53:38.000000 easy_gpt_utils-0.1.9/easy_gpt_utils_bak/__init__.py
+-rw-r--r--   0 houwei    (1001) houwei    (1001)     5221 2023-05-10 10:53:38.000000 easy_gpt_utils-0.1.9/easy_gpt_utils_bak/embedding.py
+-rw-r--r--   0 houwei    (1001) houwei    (1001)    29324 2023-05-10 10:53:38.000000 easy_gpt_utils-0.1.9/easy_gpt_utils_bak/gpt.py
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)     5309 2023-05-10 10:53:38.000000 easy_gpt_utils-0.1.9/easy_gpt_utils_bak/vector_database.py
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)       38 2023-05-12 04:43:58.633231 easy_gpt_utils-0.1.9/setup.cfg
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)      803 2023-05-12 04:43:14.000000 easy_gpt_utils-0.1.9/setup.py
```

### Comparing `easy_gpt_utils-0.1.8/LICENSE` & `easy_gpt_utils-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_gpt_utils-0.1.8/easy_gpt_utils/embedding.py` & `easy_gpt_utils-0.1.9/easy_gpt_utils_bak/embedding.py`

 * *Files identical despite different names*

### Comparing `easy_gpt_utils-0.1.8/easy_gpt_utils/gpt.py` & `easy_gpt_utils-0.1.9/easy_gpt_utils_bak/gpt.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,22 +4,29 @@
 import openai
 import tiktoken
 import argparse
 import re
 import logging
 
 class GPT():
-    def __init__(self, model = "gpt-3.5-turbo", temperature = 0.0, system_prompt = "", post_prompt = "", use_history = False):
+    def __init__(self, model = "gpt-3.5-turbo", 
+                 api_type="open_ai", api_base=None, api_key=None, api_version=None,
+                 temperature = 0.0, system_prompt = "", post_prompt = "", use_history = False):
         self.model = model
+        self.engine = model
+        self.api_type = api_type
+        self.api_base = api_base
+        self.api_key = api_key
+        self.api_version = api_version
         self.temperature = temperature
         self.system_prompt = system_prompt
         self.post_prompt = post_prompt
         self.use_history = use_history
         self.history = []
-        openai.api_key = os.getenv("OPENAI_API_KEY")
+        #openai.api_key = os.getenv("OPENAI_API_KEY")
     
     def set_system_prompt(self, system_prompt):
         self.system_prompt = system_prompt
     
     def set_post_prompt(self, post_prompt):
         self.post_prompt = post_prompt
     
@@ -136,28 +143,38 @@
                 'content': f'{self.system_prompt} {text}'},
                 *self.history,
                 {'role': 'user', 'content': query_text + self.post_prompt},
             ]
             logging.debug(query_message)
             response = openai.ChatCompletion.create(
                 model=self.model,
+                engine=self.engine,
+                api_type=self.api_type, 
+                api_key=self.api_key, 
+                api_base=self.api_base, 
+                api_version=self.api_version,
                 temperature=self.temperature,
                 messages=query_message
             )
             self.history.append({'role': 'user', 'content': query_text})
             self.history.append({'role': 'assistant', 'content': response.choices[0].message.content})
         else:
             query_message = [
                 {'role': 'system',
                 'content': f'{self.system_prompt} {text}'},
                 {'role': 'user', 'content': query_text + self.post_prompt},
             ]
             logging.debug(query_message)
             response = openai.ChatCompletion.create(
                 model=self.model,
+                engine=self.engine,
+                api_type=self.api_type, 
+                api_key=self.api_key, 
+                api_base=self.api_base, 
+                api_version=self.api_version,
                 temperature=self.temperature,
                 messages=query_message
             )
 
         logging.debug(response)
 
         return response.choices[0].message.content
@@ -232,37 +249,82 @@
 '''
     result6 = gpt.split_text(text5)
     print("len(result6):", len(result6))
     assert len(result6) == 1
 
     print("All test cases passed.")
 
+import os
+import openai
+openai.api_type = "azure"
+openai.api_base = "https://ninebot-rd-openai-1.openai.azure.com/"
+openai.api_version = "2022-12-01"
+openai.api_key = os.getenv("OPENAI_API_KEY")
+
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description="GPT")
     parser.add_argument("--model", default="gpt-3.5-turbo", dest="model", type=str,help="GPT model")
     parser.add_argument("--temperature", default=0.0, dest="temperature", type=float,help="GPT temperature")
     parser.add_argument("--system_prompt", default="You are a customer service agent for company 9. You need to reply to the customer based on the context information below.", dest="system_prompt", type=str,help="GPT system prompt")
     parser.add_argument("--post_prompt", default="Please reply to the customer.", dest="post_prompt", type=str,help="GPT post prompt")
     parser.add_argument("--use_history", default=False, dest="use_history", type=bool,help="GPT use history")
     parser.add_argument("--history", default=[], dest="history", type=list,help="GPT history")
     args = parser.parse_args()
-    gpt = GPT(args.model, args.temperature, args.system_prompt, args.post_prompt, args.use_history)
+    
+    logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+
+    if False:
+        #test for openai
+        gpt = GPT(model = args.model, temperature = args.temperature, system_prompt = args.system_prompt, post_prompt = args.post_prompt, use_history = args.use_history)
+    else:
+        # test for azure
+        gpt = GPT(
+            model="model-gpt-35-turbo-0301", 
+            api_type="azure", 
+            api_base = "https://ninebot-rd-openai-1.openai.azure.com/",
+            api_version = "2022-12-01",
+            temperature = args.temperature, 
+            system_prompt = args.system_prompt, 
+            post_prompt = args.post_prompt, 
+            use_history = args.use_history)
 
     # tests
 
     # test 1 split_text
-    test_split_text(gpt)
-    exit()
+    #test_split_text(gpt)
+    #exit()
 
     gpt.set_system_prompt("You are a customer service agent for Segway. You need to reply to the customer based on the context information below:")
     gpt.set_post_prompt("Reply '我不清楚您的问题' on unrelated to context.")
 
-    print(gpt.num_tokens_from_string("asdfawefasdfasdf我不清楚您的问题。asdfawef我不清楚您的问题。我想要买车很抱歉，Segway不是汽车，它是一种电动平衡车。如果您对Segway感兴趣，可以前往长安街上的Segway店铺购买。真的吗我不清楚您的问题。那好吧,我应该去哪里买segway您可以前往长安街上的Segway店铺购买Segway。他们会为您提供更多的信息和帮助。it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beauti我不清楚您的问题。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beauti很抱歉，我之前的回复与您的信息无关。如果您有任何问题或需要帮助，请告诉我，我会尽力回答您的疑问。it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. 我不清楚您的问题，因为您的信息似乎与任何具体问题或主题无关。如果您有任何问题或需要帮助，请告诉我，我会尽力回答您的疑问。it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. 我不清楚您的问题，因为您的信息似乎与任何具体问题或主题无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与任何具体问题或主题无关。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautifulday.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.我不清楚您的问题。it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. 我不清"))
+    #gpt.set_history([{'role':'user', 'content':'asdfawefasdfasdf我不清楚您的问题。asdfawef我不清楚您的问题。我想要买车很抱歉，Segway不是汽车，它是一种电动平衡车。如果您对Segway感兴趣，可以前往长安街上的Segway店铺购买。真的吗我不清楚您的问题。那好吧,我应该去哪里买segway您可以前往长安街上的Segway店铺购买Segway。他们会为您提供更多的信息和帮助。it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beauti我不清楚您的问题。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beauti很抱歉，我之前的回复与您的信息无关。如果您有任何问题或需要帮助，请告诉我，我会尽力回答您的疑问。it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. 我不清楚您的问题，因为您的信息似乎与任何具体问题或主题无关。如果您有任何问题或需要帮助，请告诉我，我会尽力回答您的疑问。it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. 我不清楚您的问题，因为您的信息似乎与任何具体问题或主题无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与任何具体问题或主题无关。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautifulday.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.我不清楚您的问题。it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. 我不清'}])
+
+    response = openai.Completion.create(
+        engine="model-gpt-35-turbo-0301",
+        prompt="Write a product launch email for new AI-powered headphones that are priced at $79.99 and available at Best Buy, Target and Amazon.com. The target audience is tech-savvy music lovers and the tone is friendly and exciting.\n\n1. What should be the subject line of the email?  \n2. What should be the body of the email?",
+        temperature=1,
+        max_tokens=350,
+        top_p=1,
+        frequency_penalty=0,
+        presence_penalty=0,
+        stop=None)
+
+    print(response)
+
+
+    print ("dp",openai.Completion.create(
+                #model="model-gpt-35-turbo-0301", 
+                engine="model-gpt-35-turbo-0301", 
+                api_type="azure", 
+                api_base = "https://ninebot-rd-openai-1.openai.azure.com/",
+                api_version = "2022-12-01",
+                temperature=0.0,
+                prompt='hello'
+            ))
 
-    gpt.set_history([{'role':'user', 'content':'asdfawefasdfasdf我不清楚您的问题。asdfawef我不清楚您的问题。我想要买车很抱歉，Segway不是汽车，它是一种电动平衡车。如果您对Segway感兴趣，可以前往长安街上的Segway店铺购买。真的吗我不清楚您的问题。那好吧,我应该去哪里买segway您可以前往长安街上的Segway店铺购买Segway。他们会为您提供更多的信息和帮助。it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beauti我不清楚您的问题。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beauti很抱歉，我之前的回复与您的信息无关。如果您有任何问题或需要帮助，请告诉我，我会尽力回答您的疑问。it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. 我不清楚您的问题，因为您的信息似乎与任何具体问题或主题无关。如果您有任何问题或需要帮助，请告诉我，我会尽力回答您的疑问。it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. 我不清楚您的问题，因为您的信息似乎与任何具体问题或主题无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与任何具体问题或主题无关。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautifulday.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.我不清楚您的问题。it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. 我不清'}])
 
     while True:
         query = input("请输入问题：")
         if query == "exit":
             break
         print(gpt.query(["Segway在长安街上有一家店，你可以去那里买Segway。"], query))
         print(gpt.get_token_limit())
```

### Comparing `easy_gpt_utils-0.1.8/easy_gpt_utils/vector_database.py` & `easy_gpt_utils-0.1.9/easy_gpt_utils_bak/vector_database.py`

 * *Files identical despite different names*

### Comparing `easy_gpt_utils-0.1.8/easy_gpt_utils_bak/embedding.py` & `easy_gpt_utils-0.1.9/easy_gpt_utils/embedding.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 import argparse
 import pickle
 
 # this python script is used to generate the embedding of the input file or folder
 
 class Embedding():
     def __init__(self, model="text-embedding-ada-002", api_type="open_ai", api_base=None, api_key=None, api_version=None):
+        if (api_type != "open_ai") and (api_type != "azure"):
+            raise Exception("api_type should be open_ai or azure")
+
         self.model = model
         self.engine = model
         self.api_type = api_type
         self.api_base = api_base
         self.api_key = api_key
         self.api_version = api_version
     
@@ -26,34 +29,51 @@
     # return embedding of the input text list
     def get_embedding(self, input_text_list):
         # if input_text_list is not a list throw an exception
         if not isinstance(input_text_list, list):
             raise TypeError("input_text_list should be a list")
 
         # openai api do not allow set model and engine at the same time
-        # by testing, set engine only
-        embedding = openai.Embedding.create(
-            #model=self.model, 
-            input=input_text_list, 
-            engine=self.engine,
-            api_type=self.api_type, 
-            api_key=self.api_key, 
-            api_base=self.api_base, 
-            api_version=self.api_version)
+        if (self.api_type == "open_ai"):
+            embedding = openai.Embedding.create(
+                model=self.model, 
+                input=input_text_list, 
+                api_type=self.api_type, 
+                api_key=self.api_key, 
+                api_base=self.api_base, 
+                api_version=self.api_version)
+        elif (self.api_type == "azure"):
+            embedding = openai.Embedding.create(
+                input=input_text_list, 
+                engine=self.engine,
+                api_type=self.api_type, 
+                api_key=self.api_key, 
+                api_base=self.api_base, 
+                api_version=self.api_version)
         return [(text, data.embedding) for text, data in zip(input_text_list, embedding.data)], embedding.usage.total_tokens
 
     def get_raw_embedding(self, raw_text: str):
-        embedding = openai.Embedding.create(
-            #model=self.model, 
-            input=raw_text,
-            engine=self.engine,
-            api_type=self.api_type, 
-            api_key=self.api_key, 
-            api_base=self.api_base, 
-            api_version=self.api_version)
+         # openai api do not allow set model and engine at the same time
+        if (self.api_type == "open_ai"):
+            embedding = openai.Embedding.create(
+                model=self.model, 
+                input=raw_text,
+                api_type=self.api_type, 
+                api_key=self.api_key, 
+                api_base=self.api_base, 
+                api_version=self.api_version)
+        elif (self.api_type == "azure"):
+            embedding = openai.Embedding.create(
+                input=raw_text,
+                engine=self.engine,
+                api_type=self.api_type, 
+                api_key=self.api_key, 
+                api_base=self.api_base, 
+                api_version=self.api_version)
+            
         return list(embedding.data[0].embedding)
     
     def create_embeddings(self, input_text_list):
         # if input_text_list is not a list throw an exception
         if not isinstance(input_text_list, list):
             raise TypeError("input_text_list should be a list")
 
@@ -121,20 +141,22 @@
 
     #embedding = Embedding(model=args.model)
     #print(embedding.create_embeddings(args.input))
     #print(embedding("hello world"))
     #print(embedding.create_embedding_from_file(args.input, args.output))
     #print(embedding.create_embedding_from_file_save_to_file(args.input, args.output))
     
-    if False:
+    use_openai = True
+    if use_openai:
         # test for openai
         embedding = Embedding()
     else :
         # test for azure
         embedding = Embedding(
             model="model-text-embedding-ada-002", 
             api_type="azure", 
+            api_key = os.getenv("AZURE_API_KEY"),
             api_base = "https://ninebot-rd-openai-1.openai.azure.com/",
             api_version = "2022-12-01")
     
     print(embedding.create_embeddings_from_text(args.input))
     print(embedding.get_raw_embedding(args.input))
```

### Comparing `easy_gpt_utils-0.1.8/easy_gpt_utils_bak/gpt.py` & `easy_gpt_utils-0.1.9/easy_gpt_utils/gpt.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,26 +7,28 @@
 import re
 import logging
 
 class GPT():
     def __init__(self, model = "gpt-3.5-turbo", 
                  api_type="open_ai", api_base=None, api_key=None, api_version=None,
                  temperature = 0.0, system_prompt = "", post_prompt = "", use_history = False):
+        if (api_type != "open_ai") and (api_type != "azure"):
+            raise Exception("api_type should be open_ai or azure")
+
         self.model = model
         self.engine = model
         self.api_type = api_type
         self.api_base = api_base
         self.api_key = api_key
         self.api_version = api_version
         self.temperature = temperature
         self.system_prompt = system_prompt
         self.post_prompt = post_prompt
         self.use_history = use_history
         self.history = []
-        #openai.api_key = os.getenv("OPENAI_API_KEY")
     
     def set_system_prompt(self, system_prompt):
         self.system_prompt = system_prompt
     
     def set_post_prompt(self, post_prompt):
         self.post_prompt = post_prompt
     
@@ -50,15 +52,15 @@
             # for gpt-3.5-turbo, the max_tokens is 4096
             max_tokens = 4096
         # todo: debug when using gpt-4
         elif self.model == "gpt-4":
             max_tokens = 8192
         else:
             max_tokens = 4096
-        logging.debug("history:", self.history)
+        logging.debug("history: %s", self.history)
         #print("content:", str(text.get('content')) for text in self.history)
         for text in self.history:
             logging.debug(text.get('content'))
         history_token = sum([self.num_tokens_from_string(str(text)) for text in self.history])
         
         # 50 is for fixed system prompt and post prompt
         return max_tokens - history_token - 50
@@ -129,57 +131,60 @@
 
         return chunks
 
     # context_info is a list of strings
     # query_text is a string
     def query(self, context_info, query_text):
         # todo: check query_message length if it is over 4096 the throw exception  
-        if (context_info is None) or (context_info == ""):
+        if (context_info is None) or (context_info == "") or (len(context_info) == 0):
             text = ""
         else:
             text = "Please reply based on the context information below:\n".join(f"{index}. {text}" for index, text in enumerate(context_info))
+
         if self.use_history:
             query_message = [
                 {'role': 'system',
                 'content': f'{self.system_prompt} {text}'},
                 *self.history,
                 {'role': 'user', 'content': query_text + self.post_prompt},
             ]
-            logging.debug(query_message)
-            response = openai.ChatCompletion.create(
-                model=self.model,
-                engine=self.engine,
-                api_type=self.api_type, 
-                api_key=self.api_key, 
-                api_base=self.api_base, 
-                api_version=self.api_version,
-                temperature=self.temperature,
-                messages=query_message
-            )
-            self.history.append({'role': 'user', 'content': query_text})
-            self.history.append({'role': 'assistant', 'content': response.choices[0].message.content})
         else:
             query_message = [
                 {'role': 'system',
                 'content': f'{self.system_prompt} {text}'},
                 {'role': 'user', 'content': query_text + self.post_prompt},
             ]
-            logging.debug(query_message)
+
+        logging.debug(f"send query: {query_message}")
+        if (self.api_type == 'open_ai'):
             response = openai.ChatCompletion.create(
                 model=self.model,
+                api_type=self.api_type, 
+                api_key=self.api_key, 
+                api_base=self.api_base, 
+                api_version=self.api_version,
+                temperature=self.temperature,
+                messages=query_message)
+        elif (self.api_type == 'azure'):
+            response = openai.ChatCompletion.create(
                 engine=self.engine,
                 api_type=self.api_type, 
                 api_key=self.api_key, 
                 api_base=self.api_base, 
                 api_version=self.api_version,
                 temperature=self.temperature,
-                messages=query_message
-            )
+                messages=query_message)
+        else:
+            raise Exception("api_type not supported")
 
-        logging.debug(response)
+        logging.debug(f"got response: {response}")
+
+        if self.use_history:
+            self.history.append({'role': 'user', 'content': query_text})
+            self.history.append({'role': 'assistant', 'content': response.choices[0].message.content})
 
         return response.choices[0].message.content
 
 # test cases
 def test_split_text(gpt):
     # 测试用例 1： 简单文本，无需拆分
     text1 = "This is a short text. It doesn't need to be split."
@@ -249,43 +254,38 @@
 '''
     result6 = gpt.split_text(text5)
     print("len(result6):", len(result6))
     assert len(result6) == 1
 
     print("All test cases passed.")
 
-import os
-import openai
-openai.api_type = "azure"
-openai.api_base = "https://ninebot-rd-openai-1.openai.azure.com/"
-openai.api_version = "2022-12-01"
-openai.api_key = os.getenv("OPENAI_API_KEY")
-
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description="GPT")
     parser.add_argument("--model", default="gpt-3.5-turbo", dest="model", type=str,help="GPT model")
     parser.add_argument("--temperature", default=0.0, dest="temperature", type=float,help="GPT temperature")
     parser.add_argument("--system_prompt", default="You are a customer service agent for company 9. You need to reply to the customer based on the context information below.", dest="system_prompt", type=str,help="GPT system prompt")
     parser.add_argument("--post_prompt", default="Please reply to the customer.", dest="post_prompt", type=str,help="GPT post prompt")
     parser.add_argument("--use_history", default=False, dest="use_history", type=bool,help="GPT use history")
     parser.add_argument("--history", default=[], dest="history", type=list,help="GPT history")
     args = parser.parse_args()
     
     logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 
-    if False:
+    use_openai = False
+    if use_openai:
         #test for openai
         gpt = GPT(model = args.model, temperature = args.temperature, system_prompt = args.system_prompt, post_prompt = args.post_prompt, use_history = args.use_history)
     else:
         # test for azure
         gpt = GPT(
             model="model-gpt-35-turbo-0301", 
             api_type="azure", 
             api_base = "https://ninebot-rd-openai-1.openai.azure.com/",
-            api_version = "2022-12-01",
+            api_version = "2023-03-15-preview",
+            api_key = os.getenv("AZURE_API_KEY"),
             temperature = args.temperature, 
             system_prompt = args.system_prompt, 
             post_prompt = args.post_prompt, 
             use_history = args.use_history)
 
     # tests
 
@@ -294,38 +294,14 @@
     #exit()
 
     gpt.set_system_prompt("You are a customer service agent for Segway. You need to reply to the customer based on the context information below:")
     gpt.set_post_prompt("Reply '我不清楚您的问题' on unrelated to context.")
 
     #gpt.set_history([{'role':'user', 'content':'asdfawefasdfasdf我不清楚您的问题。asdfawef我不清楚您的问题。我想要买车很抱歉，Segway不是汽车，它是一种电动平衡车。如果您对Segway感兴趣，可以前往长安街上的Segway店铺购买。真的吗我不清楚您的问题。那好吧,我应该去哪里买segway您可以前往长安街上的Segway店铺购买Segway。他们会为您提供更多的信息和帮助。it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beauti我不清楚您的问题。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beauti很抱歉，我之前的回复与您的信息无关。如果您有任何问题或需要帮助，请告诉我，我会尽力回答您的疑问。it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. 我不清楚您的问题，因为您的信息似乎与任何具体问题或主题无关。如果您有任何问题或需要帮助，请告诉我，我会尽力回答您的疑问。it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. 我不清楚您的问题，因为您的信息似乎与任何具体问题或主题无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与任何具体问题或主题无关。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautifulday.我不清楚您的问题，因为您的信息似乎与之前的上下文无关。请提供相关的问题或信息，我会尽力回答您的疑问。it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.我不清楚您的问题。it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.it’s a beautiful day.我不清楚您的问题。it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. it’s a beautiful day. 我不清'}])
 
-    response = openai.Completion.create(
-        engine="model-gpt-35-turbo-0301",
-        prompt="Write a product launch email for new AI-powered headphones that are priced at $79.99 and available at Best Buy, Target and Amazon.com. The target audience is tech-savvy music lovers and the tone is friendly and exciting.\n\n1. What should be the subject line of the email?  \n2. What should be the body of the email?",
-        temperature=1,
-        max_tokens=350,
-        top_p=1,
-        frequency_penalty=0,
-        presence_penalty=0,
-        stop=None)
-
-    print(response)
-
-
-    print ("dp",openai.Completion.create(
-                #model="model-gpt-35-turbo-0301", 
-                engine="model-gpt-35-turbo-0301", 
-                api_type="azure", 
-                api_base = "https://ninebot-rd-openai-1.openai.azure.com/",
-                api_version = "2022-12-01",
-                temperature=0.0,
-                prompt='hello'
-            ))
-
 
     while True:
         query = input("请输入问题：")
         if query == "exit":
             break
         print(gpt.query(["Segway在长安街上有一家店，你可以去那里买Segway。"], query))
         print(gpt.get_token_limit())
-
```

### Comparing `easy_gpt_utils-0.1.8/easy_gpt_utils_bak/vector_database.py` & `easy_gpt_utils-0.1.9/easy_gpt_utils/vector_database.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import pinecone
 import uuid
 from enum import Enum
 from typing import Union, List, Tuple, Optional, Dict, Any
 
 # namespaces
 class NamesSpaces(Enum):
@@ -82,28 +83,39 @@
               id: Optional[str] = None,
               filter: Optional[Dict[str, Union[str, float, int, bool, List, dict]]] = None):
         return [{'score':result['score'], 'metadata': result['metadata']} for result in 
             self.index.query(namespace = namespace, top_k = top_k, vector=vector, id=id, filter=filter, include_metadata=True)['matches'] if result['score'] > threshold]
 
 
 # TODO: test code should move to unit test
-define_test = False
+define_test = True
 if define_test:
     try:
         from .embedding import Embedding  # for when the module is imported
     except ImportError:
         from embedding import Embedding  # for when the module is run directly
 
     testcase = [
     'withstand voltage	耐压',
     'fingerprint U-lock	指纹U型锁',
     'No rider detected	未触发站人模式'
     ]
 
-    embedding_instance = Embedding()
+    use_openai = False
+    if use_openai:
+        # test for openai
+        embedding_instance = Embedding()
+    else :
+        # test for azure
+        embedding_instance = Embedding(
+            model="model-text-embedding-ada-002", 
+            api_type="azure", 
+            api_key = os.getenv("AZURE_API_KEY"),
+            api_base = "https://ninebot-rd-openai-1.openai.azure.com/",
+            api_version = "2022-12-01")
 
     my_pinecone = Pinecone(index = 'segway-knowledge-base', environment='asia-southeast1-gcp')
     #print ("delete", my_pinecone.delete(namespace = NamesSpaces.Glossary.value, ids = ['id0']))
     #print ("my_pinecone: ", my_pinecone.fetch(namespace = NamesSpaces.Glossary.value, ids = ['id0', 'id1']))
     #print ("update test", my_pinecone.update(namespace = NamesSpaces.Glossary.value, id = 'id0', metadata = {'category': 'nihkao'}))
     #print ("delete all", my_pinecone.delete(namespace = NamesSpaces.Glossary.value, deleteAll = 'true'))
 
@@ -114,8 +126,10 @@
 
         to_upsert = list(zip(ids, vectors, metas))
 
         my_pinecone.upsert(namespace = NamesSpaces.Glossary.value, items = to_upsert)
         print ("my_pinecone: ", my_pinecone.fetch(namespace = NamesSpaces.Glossary.value, ids = ['id0', 'id1']))
 
     embe = embedding_instance.get_raw_embedding("withstand voltage")
-    print ("querytest: ", my_pinecone.query_meta(namespace = NamesSpaces.Glossary.value, threshold = 0.8, vector = embe, top_k = 5))
+    data = my_pinecone.query_meta(namespace = NamesSpaces.Glossary.value, threshold = 0.0, vector = embe, top_k = 5)
+    print ("querytest: ", data)
+    print ("content str", "\n".join(item['metadata']['content'] for item in data))
```

### Comparing `easy_gpt_utils-0.1.8/setup.py` & `easy_gpt_utils-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="easy_gpt_utils",
-    version="0.1.8",
+    version="0.1.9",
     packages=find_packages(),
     install_requires=[
         "openai",
         "tiktoken",
         "numpy"
     ],
     author="Hou Wei",
```

