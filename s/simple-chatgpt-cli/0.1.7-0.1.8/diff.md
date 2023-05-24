# Comparing `tmp/simple_chatgpt_cli-0.1.7.tar.gz` & `tmp/simple_chatgpt_cli-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_chatgpt_cli-0.1.7.tar", max compression
+gzip compressed data, was "simple_chatgpt_cli-0.1.8.tar", max compression
```

## Comparing `simple_chatgpt_cli-0.1.7.tar` & `simple_chatgpt_cli-0.1.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1429 2023-05-12 22:45:32.387874 simple_chatgpt_cli-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-05-12 12:32:57.857467 simple_chatgpt_cli-0.1.7/chatgpt_cli/__init__.py
--rw-r--r--   0        0        0     6758 2023-05-12 22:48:55.832214 simple_chatgpt_cli-0.1.7/chatgpt_cli/main.py
--rw-r--r--   0        0        0      701 2023-05-12 22:52:08.737344 simple_chatgpt_cli-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1875 1970-01-01 00:00:00.000000 simple_chatgpt_cli-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1431 2023-05-13 20:16:11.168124 simple_chatgpt_cli-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-05-12 12:32:57.857467 simple_chatgpt_cli-0.1.8/chatgpt_cli/__init__.py
+-rw-r--r--   0        0        0     6998 2023-05-23 13:20:50.908136 simple_chatgpt_cli-0.1.8/chatgpt_cli/main.py
+-rw-r--r--   0        0        0      701 2023-05-24 02:08:23.182621 simple_chatgpt_cli-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1877 1970-01-01 00:00:00.000000 simple_chatgpt_cli-0.1.8/PKG-INFO
```

### Comparing `simple_chatgpt_cli-0.1.7/README.md` & `simple_chatgpt_cli-0.1.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Simple-ChatGPT-CLI
 
-I believe many others have implement more sophisticated ChatGPT CLI tool. But this is a super simple one without fancy features that I created with Python for my own use case.
-My motivation was that using OpenAI API could be much cheaper than subscribing ChatGPT Plus, and is claimed to be more privacy friendly by some legal experts.
+I believe many others have implemented more sophisticated ChatGPT CLI tools. But this is a super simple one without fancy features that I created with Python for my use case.
+My motivation was that using OpenAI API could be much cheaper than subscribing to ChatGPT Plus, and is claimed to be more privacy friendly by some legal experts.
 
-I'm not planning adding fancy features unless I start to feel some feature would be a big plus to my productivity in my own use case. But everyone are welcomed to use this basic version or fork it to add their own features.
+I'm not planning to add fancy features unless I start to feel some feature would be a big plus to my productivity in my use case. But everyone is welcome to use this basic version or fork it to add their features.
 
 ## Installation
 
 ```bash
 pip install simple-chatgpt-cli
 ```
 
@@ -20,16 +20,14 @@
 
 You must either set/save the key following the CLI prompts (recommended) or set an environment variable `OPENAI_API_KEY`.
 
 ![screenshot](screenshot.png)
 
 ## Tips
 
-Use `#multiline` to enter multiline mode. This is useful when you want to enter messages with line breaks.
+- Use `#multiline` to enter multiline mode. This is useful when you want to enter messages with line breaks.
 
-Use `#startover` to start a new conversation whenever you switch to a new topic and the bot doesn't need previous context anymore. This helps reduce your OpenAI bill.
-
-The program will remind you this if you come back to an idle conversation after more than 5 minutes.
+- Use `#startover` to start a new conversation whenever you switch to a new topic and the bot doesn't need the previous context anymore. This helps reduce your OpenAI bill. The program will remind you of this if you come back to an idle conversation after more than 5 minutes.
 
 ## Development
 
 This project was initialized by my [Python project boilerplate](https://github.com/tailaiw/python-boilerplate). So you will need all the prerequisites of that project.
```

### Comparing `simple_chatgpt_cli-0.1.7/chatgpt_cli/main.py` & `simple_chatgpt_cli-0.1.8/chatgpt_cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,36 +7,37 @@
 import openai
 from rich import print
 from rich.prompt import Confirm, Prompt
 
 # disable CTRL+C
 signal.signal(signal.SIGINT, lambda signum, frame: None)
 
-# OpenAI API key
-key_file_path = os.path.join(
-    os.path.expanduser("~"), ".config/simple_chatgpt_cli/openai_api_key"
-)
-if os.getenv("OPENAI_API_KEY") is None and not os.path.exists(key_file_path):
-    openai_api_key = Prompt.ask(
-        "OpenAI API key not found. Press Enter it here to continue", password=True
-    )
-    openai.api_key = openai_api_key
-    confirm_save_key = Confirm.ask(
-        f"Do you want to save the key to {key_file_path} so you don't have to enter it again next time?",
-        default=True,
+
+def setup_openai_key() -> None:
+    key_file_path = os.path.join(
+        os.path.expanduser("~"), ".config/simple_chatgpt_cli/openai_api_key"
     )
-    if confirm_save_key:
-        os.makedirs(os.path.dirname(key_file_path), exist_ok=True)
-        with open(key_file_path, "w") as f:
-            f.write(openai_api_key)
-elif os.getenv("OPENAI_API_KEY") is None and os.path.exists(key_file_path):
-    with open(key_file_path, "r") as f:
-        openai.api_key = f.read().strip()
-else:
-    openai.api_key = os.getenv("OPENAI_API_KEY")
+    if os.getenv("OPENAI_API_KEY") is None and not os.path.exists(key_file_path):
+        openai_api_key = Prompt.ask(
+            "OpenAI API key not found. Press Enter it here to continue", password=True
+        )
+        openai.api_key = openai_api_key
+        confirm_save_key = Confirm.ask(
+            f"Do you want to save the key to {key_file_path} so you don't have to enter it again next time?",
+            default=True,
+        )
+        if confirm_save_key:
+            os.makedirs(os.path.dirname(key_file_path), exist_ok=True)
+            with open(key_file_path, "w") as f:
+                f.write(openai_api_key)
+    elif os.getenv("OPENAI_API_KEY") is None and os.path.exists(key_file_path):
+        with open(key_file_path, "r") as f:
+            openai.api_key = f.read().strip()
+    else:
+        openai.api_key = os.getenv("OPENAI_API_KEY")
 
 
 class Role(Enum):
     SYSTEM = "system"
     ASSISTANT = "assistant"
     USER = "user"
 
@@ -49,15 +50,20 @@
 
 
 class ChatExitReason(Enum):
     EXIT = "#exit"
     START_OVER = "#startover"
 
 
-ALLOWED_MODELS = ["gpt-3.5-turbo", "gpt-4"]
+class AllowedModels(Enum):
+    GPT_3_5_TURBO = "gpt-3.5-turbo"
+    GPT_4 = "gpt-4"
+
+
+ALLOWED_MODELS = [model.value for model in AllowedModels]
 WARNING_PREFIX = ":small_red_triangle:"
 INFO_PREFIX = ":small_blue_diamond:"
 BYE_PREFIX = ":wave:"
 USER_DISPLAY_NAME = "[yellow3][b]You[/b][/yellow3] :smiley:"
 BOT_DISPLAY_NAME = "[deep_sky_blue3][bold]Bot[/bold][/deep_sky_blue3] :robot:"
 SYS_CONVERSATION_INITIATION_MESSAGE = Message(
     role=Role.SYSTEM,
@@ -67,15 +73,15 @@
 CONVERSATION_SOFT_TIMEOUT_SECONDS = 300
 TEMPERATURE = 0.5
 
 
 def select_model() -> str:
     model = Prompt.ask(
         f"{INFO_PREFIX} Please select the model you want to use",
-        default="gpt-3.5-turbo",
+        default=AllowedModels.GPT_4.value,
         choices=ALLOWED_MODELS,
     )
     print(f"{INFO_PREFIX} You selected [bold cyan]{model}[/bold cyan].")
     return model
 
 
 def request_user_input() -> str:
@@ -110,33 +116,33 @@
         except EOFError:
             pass
 
     return user_input
 
 
 def chat(
-    model: str, has_previous_chat: bool, roller_message: Message | None = None
+    model: str, has_previous_chat: bool, rollover_message: Message | None = None
 ) -> tuple[ChatExitReason, Message | None]:
     # welcome console message
     if not has_previous_chat:
         print(
             f"{INFO_PREFIX} You can now start chatting with the bot. \n"
             f"Type '{ChatExitReason.EXIT.value}' to exit. "
             f"Type '{ChatExitReason.START_OVER.value}' to start a new conversation (a new conversation will lose all previous context). "
             f"Type '#multiline' to enter multiline mode."
         )
     else:
         print(
             f"{INFO_PREFIX} A new conversation started. The bot forgot all previous context."
         )
 
-    if roller_message is None:
+    if rollover_message is None:
         messages = [SYS_CONVERSATION_INITIATION_MESSAGE]
     else:
-        messages = [SYS_CONVERSATION_INITIATION_MESSAGE, roller_message]
+        messages = [SYS_CONVERSATION_INITIATION_MESSAGE, rollover_message]
 
     while True:
         if messages[-1].role != Role.USER:
             user_input = request_user_input()
             if user_input == ChatExitReason.EXIT.value:
                 return ChatExitReason.EXIT, None
             if user_input == ChatExitReason.START_OVER.value:
@@ -186,14 +192,15 @@
             Prompt.ask(
                 f"{WARNING_PREFIX} The total token count exceeds the maximum. You must start a new conversation. Press Enter to continue",
             )
             return ChatExitReason.START_OVER, None
 
 
 def run() -> None:
+    setup_openai_key()
     model = select_model()
     chat_exit_reason, rollover_message = chat(model, has_previous_chat=False)
     while chat_exit_reason == ChatExitReason.START_OVER:
         chat_exit_reason, rollover_message = chat(
-            model, has_previous_chat=True, roller_message=rollover_message
+            model, has_previous_chat=True, rollover_message=rollover_message
         )
     print(f"{BYE_PREFIX} Bye!")
```

### Comparing `simple_chatgpt_cli-0.1.7/pyproject.toml` & `simple_chatgpt_cli-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 wrap-descriptions = 88
 
 [tool.poetry.scripts]
 chatgpt = 'chatgpt_cli.main:run'
 
 [tool.poetry]
 name = "simple-chatgpt-cli"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["tailaiw <29800495+tailaiw@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "chatgpt_cli" }]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```

### Comparing `simple_chatgpt_cli-0.1.7/PKG-INFO` & `simple_chatgpt_cli-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: simple-chatgpt-cli
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: tailaiw
 Author-email: 29800495+tailaiw@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=0.27.6,<0.28.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Description-Content-Type: text/markdown
 
 # Simple-ChatGPT-CLI
 
-I believe many others have implement more sophisticated ChatGPT CLI tool. But this is a super simple one without fancy features that I created with Python for my own use case.
-My motivation was that using OpenAI API could be much cheaper than subscribing ChatGPT Plus, and is claimed to be more privacy friendly by some legal experts.
+I believe many others have implemented more sophisticated ChatGPT CLI tools. But this is a super simple one without fancy features that I created with Python for my use case.
+My motivation was that using OpenAI API could be much cheaper than subscribing to ChatGPT Plus, and is claimed to be more privacy friendly by some legal experts.
 
-I'm not planning adding fancy features unless I start to feel some feature would be a big plus to my productivity in my own use case. But everyone are welcomed to use this basic version or fork it to add their own features.
+I'm not planning to add fancy features unless I start to feel some feature would be a big plus to my productivity in my use case. But everyone is welcome to use this basic version or fork it to add their features.
 
 ## Installation
 
 ```bash
 pip install simple-chatgpt-cli
 ```
 
@@ -34,17 +34,15 @@
 
 You must either set/save the key following the CLI prompts (recommended) or set an environment variable `OPENAI_API_KEY`.
 
 ![screenshot](screenshot.png)
 
 ## Tips
 
-Use `#multiline` to enter multiline mode. This is useful when you want to enter messages with line breaks.
+- Use `#multiline` to enter multiline mode. This is useful when you want to enter messages with line breaks.
 
-Use `#startover` to start a new conversation whenever you switch to a new topic and the bot doesn't need previous context anymore. This helps reduce your OpenAI bill.
-
-The program will remind you this if you come back to an idle conversation after more than 5 minutes.
+- Use `#startover` to start a new conversation whenever you switch to a new topic and the bot doesn't need the previous context anymore. This helps reduce your OpenAI bill. The program will remind you of this if you come back to an idle conversation after more than 5 minutes.
 
 ## Development
 
 This project was initialized by my [Python project boilerplate](https://github.com/tailaiw/python-boilerplate). So you will need all the prerequisites of that project.
```

