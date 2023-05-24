# Comparing `tmp/openai-pygenerator-0.2.2.tar.gz` & `tmp/openai-pygenerator-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-pygenerator-0.2.2.tar", last modified: Sat May 20 09:24:39 2023, max compression
+gzip compressed data, was "openai-pygenerator-0.3.0.tar", last modified: Wed May 24 10:24:15 2023, max compression
```

## Comparing `openai-pygenerator-0.2.2.tar` & `openai-pygenerator-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:24:39.474436 openai-pygenerator-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:24:39.470436 openai-pygenerator-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:24:39.474436 openai-pygenerator-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-20 09:24:29.000000 openai-pygenerator-0.2.2/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-20 09:24:29.000000 openai-pygenerator-0.2.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 09:24:29.000000 openai-pygenerator-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-20 09:24:29.000000 openai-pygenerator-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21334 2023-05-20 09:24:29.000000 openai-pygenerator-0.2.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-20 09:24:29.000000 openai-pygenerator-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-20 09:24:39.474436 openai-pygenerator-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-20 09:24:29.000000 openai-pygenerator-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 09:24:29.000000 openai-pygenerator-0.2.2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-20 09:24:29.000000 openai-pygenerator-0.2.2/mypy-tests.ini
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-20 09:24:29.000000 openai-pygenerator-0.2.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-20 09:24:29.000000 openai-pygenerator-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-20 09:24:39.474436 openai-pygenerator-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-20 09:24:29.000000 openai-pygenerator-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:24:39.470436 openai-pygenerator-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:24:39.474436 openai-pygenerator-0.2.2/src/openai_pygenerator/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-20 09:24:29.000000 openai-pygenerator-0.2.2/src/openai_pygenerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-20 09:24:29.000000 openai-pygenerator-0.2.2/src/openai_pygenerator/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-20 09:24:29.000000 openai-pygenerator-0.2.2/src/openai_pygenerator/openai_pygenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:24:39.474436 openai-pygenerator-0.2.2/src/openai_pygenerator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-20 09:24:39.000000 openai-pygenerator-0.2.2/src/openai_pygenerator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-20 09:24:39.000000 openai-pygenerator-0.2.2/src/openai_pygenerator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 09:24:39.000000 openai-pygenerator-0.2.2/src/openai_pygenerator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-20 09:24:39.000000 openai-pygenerator-0.2.2/src/openai_pygenerator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-20 09:24:39.000000 openai-pygenerator-0.2.2/src/openai_pygenerator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-20 09:24:39.000000 openai-pygenerator-0.2.2/src/openai_pygenerator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:24:39.474436 openai-pygenerator-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-20 09:24:29.000000 openai-pygenerator-0.2.2/tests/test_gpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:24:15.700676 openai-pygenerator-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:24:15.696676 openai-pygenerator-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:24:15.700676 openai-pygenerator-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-24 10:24:15.700676 openai-pygenerator-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/mypy-tests.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-24 10:24:15.704676 openai-pygenerator-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:24:15.700676 openai-pygenerator-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:24:15.700676 openai-pygenerator-0.3.0/src/openai_pygenerator/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/src/openai_pygenerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/src/openai_pygenerator/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/src/openai_pygenerator/openai_pygenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:24:15.700676 openai-pygenerator-0.3.0/src/openai_pygenerator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-24 10:24:15.000000 openai-pygenerator-0.3.0/src/openai_pygenerator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-24 10:24:15.000000 openai-pygenerator-0.3.0/src/openai_pygenerator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 10:24:15.000000 openai-pygenerator-0.3.0/src/openai_pygenerator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-24 10:24:15.000000 openai-pygenerator-0.3.0/src/openai_pygenerator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-24 10:24:15.000000 openai-pygenerator-0.3.0/src/openai_pygenerator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-24 10:24:15.000000 openai-pygenerator-0.3.0/src/openai_pygenerator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:24:15.700676 openai-pygenerator-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/tests/test_gpt.py
```

### Comparing `openai-pygenerator-0.2.2/.github/workflows/python-package.yml` & `openai-pygenerator-0.3.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.2.2/.github/workflows/python-publish.yml` & `openai-pygenerator-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.2.2/.pre-commit-config.yaml` & `openai-pygenerator-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.2.2/.pylintrc` & `openai-pygenerator-0.3.0/.pylintrc`

 * *Files 2% similar despite different names*

```diff
@@ -632,8 +632,9 @@
 init-import=no
 
 # List of qualified module names which can have objects that can redefine
 # builtins.
 redefining-builtins-modules=six.moves,past.builtins,future.builtins,builtins,io
 
 [MASTER]
+init-hook='import sys; sys.path.append("./src")'
 disable=C0114,C0116,C0115,R0902,R0913,R1735,R0903,C0103,R1705,W0621
```

### Comparing `openai-pygenerator-0.2.2/LICENSE.txt` & `openai-pygenerator-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.2.2/PKG-INFO` & `openai-pygenerator-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-pygenerator
-Version: 0.2.2
+Version: 0.3.0
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai-pygenerator-0.2.2/README.md` & `openai-pygenerator-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.2.2/pyproject.toml` & `openai-pygenerator-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.2.2/src/openai_pygenerator/example.py` & `openai-pygenerator-0.3.0/src/openai_pygenerator/example.py`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.2.2/src/openai_pygenerator/openai_pygenerator.py` & `openai-pygenerator-0.3.0/src/openai_pygenerator/openai_pygenerator.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 from typing import Callable, Dict, Iterable, Iterator, List, NewType, TypeVar
 
 import openai
 from openai.error import APIError, RateLimitError
 
 Completion = Dict[str, str]
 Seconds = NewType("Seconds", int)
-Conversation = Iterator[Completion]
+Completions = Iterator[Completion]
 History = Iterable[Completion]
+Completer = Callable[[History, int], Completions]
 T = TypeVar("T")
 
 
 def var(name: str, to_type: Callable[[str], T], default: T) -> T:
     result = os.environ.get(name)
     if result is None:
         return default
-    else:
-        return to_type(result)
+    return to_type(result)
 
 
 GPT_MODEL = var("GPT_MODEL", str, "gpt-3.5-turbo")
 GPT_TEMPERATURE = var("GPT_TEMPERATURE", float, 0.2)
 GPT_MAX_TOKENS = var("GPT_MAX_TOKENS", int, 100)
 GPT_MAX_RETRIES = var("GPT_MAX_RETRIES", int, 5)
 GPT_RETRY_EXPONENT_SECONDS = Seconds(var("GPT_RETRY_EXPONENT_SECONDS", int, 2))
@@ -35,16 +35,16 @@
 def completer(
     model: str = GPT_MODEL,
     max_tokens: int = GPT_MAX_TOKENS,
     temperature: float = GPT_TEMPERATURE,
     max_retries: int = GPT_MAX_RETRIES,
     retry_base: Seconds = GPT_RETRY_BASE_SECONDS,
     retry_exponent: Seconds = GPT_RETRY_EXPONENT_SECONDS,
-) -> Callable[[History, int], Conversation]:
-    def f(messages: History, n: int = 1) -> Conversation:
+) -> Completer:
+    def f(messages: History, n: int = 1) -> Completions:
         return generate_completions(
             messages,
             model,
             max_tokens,
             temperature,
             max_retries,
             retry_base,
@@ -64,15 +64,15 @@
     max_tokens: int,
     temperature: float,
     max_retries: int,
     retry_base: Seconds,
     retry_exponent: Seconds,
     n: int = 1,
     retries: int = 0,
-) -> Conversation:
+) -> Completions:
     logger.debug("messages = %s", messages)
     try:
         result = openai.ChatCompletion.create(
             model=model,
             messages=messages,
             max_tokens=max_tokens,
             n=n,
@@ -111,21 +111,31 @@
 
 
 def transcript(messages: History) -> List[str]:
     return [r["content"] for r in messages]
 
 
 class ChatSession:
-    def __init__(
-        self, generate: Callable[[History, int], Conversation] = gpt_completions
-    ):
+    """Encapsulates chat session state
+
+    :param generate: A function to generate completions from a history
+    """
+
+    def __init__(self, generate: Completer = gpt_completions):
         self._messages: List[Completion] = []
         self._generate = generate
 
     def ask(self, prompt: str) -> str:
+        """
+        Submit a message in the user-role to the chatbot,
+        and record both the user message and assistant
+        response in the chat history.
+        :param prompt: The user message
+        :return: The assistant response
+        """
         message = user_message(prompt)
         self._messages.append(message)
         completions = self._generate(self.messages, 1)
         response = next(completions)
         self._messages.append(response)
         return response["content"]
```

### Comparing `openai-pygenerator-0.2.2/src/openai_pygenerator.egg-info/PKG-INFO` & `openai-pygenerator-0.3.0/src/openai_pygenerator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-pygenerator
-Version: 0.2.2
+Version: 0.3.0
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai-pygenerator-0.2.2/src/openai_pygenerator.egg-info/SOURCES.txt` & `openai-pygenerator-0.3.0/src/openai_pygenerator.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 .pylintrc
 LICENSE.txt
 README.md
 conftest.py
 mypy-tests.ini
 mypy.ini
 pyproject.toml
+requirements.txt
 setup.cfg
 setup.py
 .github/workflows/python-package.yml
 .github/workflows/python-publish.yml
 src/openai_pygenerator/__init__.py
 src/openai_pygenerator/example.py
 src/openai_pygenerator/openai_pygenerator.py
```

### Comparing `openai-pygenerator-0.2.2/tests/test_gpt.py` & `openai-pygenerator-0.3.0/tests/test_gpt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,33 @@
-from typing import Callable, Iterable
+# pylint: disable=redefined-outer-name
+
+from typing import Iterable
 
 import pytest
 from openai.error import APIError, RateLimitError
 from openai.openai_object import OpenAIObject
 
 from openai_pygenerator import (
     GPT_MAX_RETRIES,
     ChatSession,
-    Conversation,
+    Completer,
+    Completions,
     gpt_completions,
     transcript,
     user_message,
 )
 
 
 def aio(text: str) -> OpenAIObject:
     result = OpenAIObject()
     result["message"] = text
     return result
 
 
+# pylint: disable=too-few-public-methods
 class MockChoices:
     def __init__(self, responses: Iterable[str]):
         self.choices = [aio(text) for text in responses]
 
 
 @pytest.fixture
 def mock_openai(mocker):
@@ -85,16 +89,16 @@
     test_messages = [user_message(test_message(i)) for i in range(10)]
     result = list(transcript(iter(test_messages)))
     for i in range(10):
         assert result[i] == test_message(i)
 
 
 def test_chat_session():
-    def completer(response: str) -> Callable[[Conversation, int], Conversation]:
-        def mock_complete(_history: Conversation, _n: int) -> Conversation:
+    def completer(response: str) -> Completer:
+        def mock_complete(_history: Completions, _n: int) -> Completions:
             yield {"role": "assistant", "content": response}
 
         return mock_complete
 
     session = ChatSession(completer("response1"))
     result = session.ask("First question")
     assert result == "response1"
```

