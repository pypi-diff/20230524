# Comparing `tmp/code_sage-0.1.1.tar.gz` & `tmp/code_sage-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_sage-0.1.1.tar", max compression
+gzip compressed data, was "code_sage-0.1.2.tar", max compression
```

## Comparing `code_sage-0.1.1.tar` & `code_sage-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-05-23 19:19:06.749230 code_sage-0.1.1/LICENSE
--rw-r--r--   0        0        0      282 2023-05-23 20:33:51.559904 code_sage-0.1.1/README.md
--rw-r--r--   0        0        0      127 2023-05-23 20:45:08.068876 code_sage-0.1.1/code_sage/__init__.py
--rw-r--r--   0        0        0     2359 2023-05-23 20:29:32.511020 code_sage-0.1.1/code_sage/middleware.py
--rw-r--r--   0        0        0      312 2023-05-23 19:57:43.075199 code_sage-0.1.1/code_sage/utils.py
--rw-r--r--   0        0        0      398 2023-05-23 20:45:08.084877 code_sage-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 code_sage-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-23 19:19:06.749230 code_sage-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2255 2023-05-24 04:04:17.268952 code_sage-0.1.2/README.md
+-rw-r--r--   0        0        0      127 2023-05-24 03:45:26.872891 code_sage-0.1.2/code_sage/__init__.py
+-rw-r--r--   0        0        0     2652 2023-05-24 03:45:26.864891 code_sage-0.1.2/code_sage/middleware.py
+-rw-r--r--   0        0        0      312 2023-05-23 19:57:43.075199 code_sage-0.1.2/code_sage/utils.py
+-rw-r--r--   0        0        0      398 2023-05-24 03:45:26.888891 code_sage-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2673 1970-01-01 00:00:00.000000 code_sage-0.1.2/PKG-INFO
```

### Comparing `code_sage-0.1.1/LICENSE` & `code_sage-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `code_sage-0.1.1/code_sage/middleware.py` & `code_sage-0.1.2/code_sage/middleware.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 import logging
 from utils import get_setting, hash_string
 
 logger = logging.getLogger(__name__)
 
 OPEN_AI_API_KEY = get_setting(name="OPEN_AI_API_KEY")
 CODE_SAGE_ENABLED = get_setting(name="OPEN_AI_API_KEY") or False
-RESPONSE_WORD_LIMIT = get_setting(name="RESPONSE_WORD_LIMIT") or 120
+CODE_SAGE_SUGGESTION_WORD_LIMIT = get_setting(name="CODE_SAGE_SUGGESTION_WORD_LIMIT") or 120
 
 
 if OPEN_AI_API_KEY:
     openai.api_key = OPEN_AI_API_KEY
 else:
-    logger.error(
-        "CHAT_GPT_API_KEY has not been set in django settings or as an environment variable"
+    logger.warning(
+        "OPEN_AI_API_KEY has not been set in django settings or as an environment variable. code_sage requires this in"
+        " order to provide suggestions to resolve unhandled errors."
     )
 
-
 # Questions sent to OpenAI and the answers given will be stored in this dictionary for caching
 # They will be in the format:  {"{hashed_question}": "{answer_from_open_ai}", ..., ...}
 CACHED_ERROR_SOLUTIONS = {}
 
 
 def get_gpt_error_solution_suggestion(error: Exception) -> str:
     error_text = repr(error)
     prompt = (
-        f"In {RESPONSE_WORD_LIMIT} words or less, tell me how I can fix the following python exception error: "
-        f"\n {error_text}"
+        f"In {CODE_SAGE_SUGGESTION_WORD_LIMIT} words or less, tell me how I can fix the following python exception error: \n"
+        f"{error_text} \n"
         f"\n"
-        f"The traceback for the error is the following:"
+        f"The traceback for the error is the following: \n"
         f"{traceback.format_exc()}"
     )
     hashed_prompt = hash_string(prompt)
 
     if hashed_prompt in CACHED_ERROR_SOLUTIONS:
         return CACHED_ERROR_SOLUTIONS[hashed_prompt]
 
@@ -59,14 +59,16 @@
     def __call__(self, request):
         response = self.get_response(request)
         return response
 
     def process_exception(self, request, exception):
         # If the chat gpt api key is set, inject a solution suggestion into the logs
         if OPEN_AI_API_KEY and CODE_SAGE_ENABLED:
+            logger.info("Calling OpenAI for suggestions on how to address an unhandled error. "
+                        "(this may take a few seconds.)"),
             logger.exception(
                 f"An unexpected error occurred. {exception}",
                 extra={
                     "error": repr(exception),
                     "suggestion": get_gpt_error_solution_suggestion(error=exception),
                     "traceback": traceback.format_exc(),
                 },
```

