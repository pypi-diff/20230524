# Comparing `tmp/roboduck-0.2.0.tar.gz` & `tmp/roboduck-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboduck-0.2.0.tar", last modified: Fri May  5 05:11:04 2023, max compression
+gzip compressed data, was "roboduck-0.3.0.tar", last modified: Wed May 24 04:02:13 2023, max compression
```

## Comparing `roboduck-0.2.0.tar` & `roboduck-0.3.0.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-05 05:11:04.461710 roboduck-0.2.0/
--rw-r--r--   0 hmamin     (501) staff       (20)      110 2023-03-29 04:32:37.000000 roboduck-0.2.0/MANIFEST.in
--rw-r--r--   0 hmamin     (501) staff       (20)      196 2023-05-05 05:11:04.461268 roboduck-0.2.0/PKG-INFO
--rw-r--r--   0 hmamin     (501) staff       (20)     5067 2023-04-24 03:54:00.000000 roboduck-0.2.0/README.md
--rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-04-30 05:54:13.000000 roboduck-0.2.0/requirements.txt
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-05 05:11:04.448877 roboduck-0.2.0/roboduck/
--rw-r--r--   0 hmamin     (501) staff       (20)      142 2023-05-05 05:10:58.000000 roboduck-0.2.0/roboduck/__init__.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-05 05:11:04.453055 roboduck-0.2.0/roboduck/cli/
--rw-r--r--   0 hmamin     (501) staff       (20)     3215 2023-04-24 03:49:53.000000 roboduck-0.2.0/roboduck/cli/cli.py
--rw-r--r--   0 hmamin     (501) staff       (20)    18834 2023-05-05 05:05:39.000000 roboduck-0.2.0/roboduck/debug.py
--rw-r--r--   0 hmamin     (501) staff       (20)     9455 2023-05-03 05:16:00.000000 roboduck-0.2.0/roboduck/decorators.py
--rw-r--r--   0 hmamin     (501) staff       (20)     9434 2023-05-03 05:15:32.000000 roboduck-0.2.0/roboduck/errors.py
--rw-r--r--   0 hmamin     (501) staff       (20)     4841 2023-05-03 05:16:35.000000 roboduck-0.2.0/roboduck/ipy_utils.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-05 05:11:04.455187 roboduck-0.2.0/roboduck/langchain/
--rw-r--r--   0 hmamin     (501) staff       (20)       79 2023-04-17 04:48:07.000000 roboduck-0.2.0/roboduck/langchain/__init__.py
--rw-r--r--   0 hmamin     (501) staff       (20)     1441 2023-04-24 03:50:43.000000 roboduck-0.2.0/roboduck/langchain/callbacks.py
--rw-r--r--   0 hmamin     (501) staff       (20)    12385 2023-05-05 05:09:51.000000 roboduck-0.2.0/roboduck/langchain/chat.py
--rw-r--r--   0 hmamin     (501) staff       (20)     2363 2023-05-05 04:36:18.000000 roboduck-0.2.0/roboduck/langchain/utils.py
--rw-r--r--   0 hmamin     (501) staff       (20)     5021 2023-05-01 06:25:10.000000 roboduck-0.2.0/roboduck/logging.py
--rw-r--r--   0 hmamin     (501) staff       (20)     5480 2023-05-01 06:27:21.000000 roboduck-0.2.0/roboduck/magic.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-05 05:11:04.456310 roboduck-0.2.0/roboduck/prompts/
--rw-r--r--   0 hmamin     (501) staff       (20)       36 2023-03-29 04:32:37.000000 roboduck-0.2.0/roboduck/prompts/__init__.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-05 05:11:04.460491 roboduck-0.2.0/roboduck/prompts/chat/
--rw-r--r--   0 hmamin     (501) staff       (20)      650 2023-04-20 04:16:32.000000 roboduck-0.2.0/roboduck/prompts/chat/__template__.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2131 2023-04-17 04:48:07.000000 roboduck-0.2.0/roboduck/prompts/chat/debug.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2178 2023-04-17 04:48:07.000000 roboduck-0.2.0/roboduck/prompts/chat/debug_full.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2106 2023-04-17 04:48:07.000000 roboduck-0.2.0/roboduck/prompts/chat/debug_full_stack_trace.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2075 2023-04-17 04:48:07.000000 roboduck-0.2.0/roboduck/prompts/chat/debug_stack_trace.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     3854 2023-04-30 05:33:59.000000 roboduck-0.2.0/roboduck/prompts/utils.py
--rw-r--r--   0 hmamin     (501) staff       (20)     1313 2023-03-17 02:32:03.000000 roboduck-0.2.0/roboduck/shell.py
--rw-r--r--   0 hmamin     (501) staff       (20)    12814 2023-05-03 05:15:32.000000 roboduck-0.2.0/roboduck/utils.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-05 05:11:04.452186 roboduck-0.2.0/roboduck.egg-info/
--rw-r--r--   0 hmamin     (501) staff       (20)      196 2023-05-05 05:11:03.000000 roboduck-0.2.0/roboduck.egg-info/PKG-INFO
--rw-r--r--   0 hmamin     (501) staff       (20)      817 2023-05-05 05:11:04.000000 roboduck-0.2.0/roboduck.egg-info/SOURCES.txt
--rw-r--r--   0 hmamin     (501) staff       (20)        1 2023-05-05 05:11:03.000000 roboduck-0.2.0/roboduck.egg-info/dependency_links.txt
--rw-r--r--   0 hmamin     (501) staff       (20)       46 2023-05-05 05:11:04.000000 roboduck-0.2.0/roboduck.egg-info/entry_points.txt
--rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-05-05 05:11:04.000000 roboduck-0.2.0/roboduck.egg-info/requires.txt
--rw-r--r--   0 hmamin     (501) staff       (20)        9 2023-05-05 05:11:04.000000 roboduck-0.2.0/roboduck.egg-info/top_level.txt
--rw-r--r--   0 hmamin     (501) staff       (20)       38 2023-05-05 05:11:04.461862 roboduck-0.2.0/setup.cfg
--rw-r--r--   0 hmamin     (501) staff       (20)      848 2023-04-30 05:56:13.000000 roboduck-0.2.0/setup.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-24 04:02:13.194975 roboduck-0.3.0/
+-rw-r--r--   0 hmamin     (501) staff       (20)      110 2023-03-29 04:32:37.000000 roboduck-0.3.0/MANIFEST.in
+-rw-r--r--   0 hmamin     (501) staff       (20)      196 2023-05-24 04:02:13.194007 roboduck-0.3.0/PKG-INFO
+-rw-r--r--   0 hmamin     (501) staff       (20)     5067 2023-04-24 03:54:00.000000 roboduck-0.3.0/README.md
+-rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-04-30 05:54:13.000000 roboduck-0.3.0/requirements.txt
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-24 04:02:13.181743 roboduck-0.3.0/roboduck/
+-rw-r--r--   0 hmamin     (501) staff       (20)      282 2023-05-24 04:01:58.000000 roboduck-0.3.0/roboduck/__init__.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-24 04:02:13.185418 roboduck-0.3.0/roboduck/cli/
+-rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-17 05:19:25.000000 roboduck-0.3.0/roboduck/cli/__init__.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     4134 2023-05-17 05:54:18.000000 roboduck-0.3.0/roboduck/cli/cli.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     6981 2023-05-16 03:52:42.000000 roboduck-0.3.0/roboduck/config.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    20177 2023-05-22 05:37:54.000000 roboduck-0.3.0/roboduck/debug.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    10255 2023-05-22 05:58:53.000000 roboduck-0.3.0/roboduck/decorators.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    11284 2023-05-18 04:08:24.000000 roboduck-0.3.0/roboduck/errors.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     5326 2023-05-16 04:48:56.000000 roboduck-0.3.0/roboduck/ipy_utils.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-24 04:02:13.187955 roboduck-0.3.0/roboduck/langchain/
+-rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-13 04:59:30.000000 roboduck-0.3.0/roboduck/langchain/__init__.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     1512 2023-05-15 05:01:22.000000 roboduck-0.3.0/roboduck/langchain/callbacks.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    14589 2023-05-23 05:07:18.000000 roboduck-0.3.0/roboduck/langchain/chat.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     1136 2023-05-15 05:02:58.000000 roboduck-0.3.0/roboduck/langchain/utils.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     6280 2023-05-19 05:20:48.000000 roboduck-0.3.0/roboduck/logging.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     5783 2023-05-18 04:01:27.000000 roboduck-0.3.0/roboduck/magic.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-24 04:02:13.188840 roboduck-0.3.0/roboduck/prompts/
+-rw-r--r--   0 hmamin     (501) staff       (20)       36 2023-03-29 04:32:37.000000 roboduck-0.3.0/roboduck/prompts/__init__.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-24 04:02:13.193391 roboduck-0.3.0/roboduck/prompts/chat/
+-rw-r--r--   0 hmamin     (501) staff       (20)      650 2023-04-20 04:16:32.000000 roboduck-0.3.0/roboduck/prompts/chat/__template__.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2131 2023-04-17 04:48:07.000000 roboduck-0.3.0/roboduck/prompts/chat/debug.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2178 2023-04-17 04:48:07.000000 roboduck-0.3.0/roboduck/prompts/chat/debug_full.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2106 2023-04-17 04:48:07.000000 roboduck-0.3.0/roboduck/prompts/chat/debug_full_stack_trace.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2075 2023-04-17 04:48:07.000000 roboduck-0.3.0/roboduck/prompts/chat/debug_stack_trace.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     3887 2023-05-15 05:03:45.000000 roboduck-0.3.0/roboduck/prompts/utils.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     1314 2023-05-16 04:49:53.000000 roboduck-0.3.0/roboduck/shell.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    14365 2023-05-16 04:13:23.000000 roboduck-0.3.0/roboduck/utils.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-24 04:02:13.184405 roboduck-0.3.0/roboduck.egg-info/
+-rw-r--r--   0 hmamin     (501) staff       (20)      196 2023-05-24 04:02:12.000000 roboduck-0.3.0/roboduck.egg-info/PKG-INFO
+-rw-r--r--   0 hmamin     (501) staff       (20)      861 2023-05-24 04:02:13.000000 roboduck-0.3.0/roboduck.egg-info/SOURCES.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)        1 2023-05-24 04:02:12.000000 roboduck-0.3.0/roboduck.egg-info/dependency_links.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)       46 2023-05-24 04:02:12.000000 roboduck-0.3.0/roboduck.egg-info/entry_points.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-05-24 04:02:12.000000 roboduck-0.3.0/roboduck.egg-info/requires.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)        9 2023-05-24 04:02:13.000000 roboduck-0.3.0/roboduck.egg-info/top_level.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)       38 2023-05-24 04:02:13.195156 roboduck-0.3.0/setup.cfg
+-rw-r--r--   0 hmamin     (501) staff       (20)      848 2023-05-17 05:17:44.000000 roboduck-0.3.0/setup.py
```

### Comparing `roboduck-0.2.0/README.md` & `roboduck-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `roboduck-0.2.0/roboduck/debug.py` & `roboduck-0.3.0/roboduck/debug.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,23 +5,27 @@
 
 Quickstart
 ----------
 Here's a broken version of bubble sort that places a `duck()` call on the
 second to last line where you might normally call `breakpoint()`.
 
 ```
-from roboduck.debug import duck
+from roboduck import duck
 
 def bubble_sort(nums):
     for i in range(len(nums)):
         for j in range(len(nums)):
             if nums[j] > nums[j + 1]:
-                nums[j + 1], nums[j] = nums[j], nums[j + 1]
+                nums[j + 1] = nums[j]
+                nums[j] = nums[j + 1]
                 duck()   # <--------------------------- instead of breakpoint()
     return nums
+
+nums = [3, 1, 9, 2, 1]
+bubble_sort(nums)
 ```
 """
 import cmd
 from functools import partial
 import inspect
 import ipynbname
 from langchain.callbacks.base import CallbackManager
@@ -37,86 +41,98 @@
 from roboduck.decorators import store_class_defaults, add_docstring
 from roboduck.ipy_utils import load_ipynb, load_current_ipython_session, \
     is_ipy_name
 
 
 @store_class_defaults(attr_filter=lambda x: x.startswith('last_'))
 class CodeCompletionCache:
-    """Just stores the last completion from DuckDB in a way that our
-    `duck` jupyter magic can access (without relying on global variable, though
-    not sure if this is meaningfully different). The magic only needs to access
-    it in insert mode (-i flag) to insert the fixed code snippet into a new
-    code cell.
+    """Stores values related to the last completion from DuckDB in a way that
+    a. our `duck` jupyter magic can access, and
+    b. allows us to easily reset all defaults
+
+    The magic only needs to access it in insert mode (-i flag) to insert
+    the fixed code snippet into a new code cell.
     """
+
+    # LLM full completion.
     last_completion = ''
+    # LLM natural language explanation.
     last_explanation = ''
+    # User code snippet.
     last_code = ''
+    # LLM generated code.
     last_new_code = ''
+    # LLM generated code with new bits highlighted (print to render correctly).
     last_code_diff = ''
+    # Allows storing extra values when passing a custom parse_func to DuckDB.
     last_extra = {}
 
 
 class DuckDB(Pdb):
-    """Conversational debugger powered by gpt models (currently codex, possibly
-    eventually chatGPT). Once you're in a debugging session, any user command
-    containing a question mark will be interpreted as a question for gpt.
-    Prefixing your question with "[dev]" will print out the full prompt before
-    making the query.
+    """Conversational debugger powered by LLM (e.g. gpt-3.5-turbo or gpt-4).
+    Once you're in a debugging session, regular pdb commands will work as usual
+    but any user command containing a question mark will be interpreted as a
+    question for the lLM. Prefixing your question with "[dev]" will print out
+    the full prompt before making the query (mostly useful when working on the
+    library).
     """
 
     def __init__(self, prompt_name='debug', max_len_per_var=79, silent=False,
                  pdb_kwargs=None, parse_func=parse_completion, color='green',
                  **chat_kwargs):
         """
         Parameters
         ----------
-        prompt_name: str
+        prompt_name : str
             Name of prompt template to use when querying chatGPT. Roboduck
             currently provides several builtin options
             (see roboduck.prompts.chat):
                 debug - for interactive debugging sessions on the relevant
                     snippet of code.
                 debug_full - for interactive debugging sessions on the whole
                     notebook (no difference from "debug" for scripts). Risks
                     creating a context that is too long.
                 debug_stack_trace - for automatic error explanations or
                     logging.
             Alternatively, can also define your own template in a yaml file
             mimicking the format of the builtin templates and pass in the
             path to that file as a string.
-        max_len_per_var: int
+        max_len_per_var : int
             Limits number of characters per variable when communicating
             current state (local or global depending on `full_context`) to
             gpt. If unbounded, that section of the prompt alone could grow
             very big . I somewhat arbitrarily set 79 as the default, i.e.
             1 line of python per variable. I figure that's usually enough to
             communicate the gist of what's happening.
-        silent: bool
+        silent : bool
             If True, print gpt completions to stdout. One example of when False
             is appropriate is our logging module - we want to get the
             explanation and update the exception message which then gets
             logged, but we don't care about typing results in real time.
-        pdb_kwargs: dict or None
+        pdb_kwargs : dict or None
             Additional kwargs for base Pdb class.
-        parse_func: function
+        parse_func : function
             This will be called on the generated text each time gpt provides a
             completion. It returns a dictionary whose values will be stored
             in CodeCompletionCache in this module. See the default function's
             docstring for guidance on writing a custom function.
-        color: str
+        color : str
             Color to print gpt completions in. Sometimes we want to change this
             to red, such as in the errors module, to make it clearer that an
             error occurred.
-        chat_kwargs: any
+        chat_kwargs : any
             Additional kwargs to configure our Chat class (passed to
-            its `from_config` factory). Common example would be setting
+            its `from_template` factory). Common example would be setting
             `chat_class=roboduck.langchain.chat.DummyChatModel`
             which mocks api calls (good for development, saves money).
         """
         super().__init__(**pdb_kwargs or {})
+        # These are prompts in the pdb sense, not the LLM sense. I.e. they
+        # are shown at the start of the line, right before the place where the
+        # user or the LLM will begin typing.
         self.prompt = '>>> '
         self.duck_prompt = '[Duck] '
         self.query_kwargs = {}
         chat_kwargs['name'] = prompt_name
         if silent:
             chat_kwargs['streaming'] = False
         else:
@@ -126,15 +142,15 @@
             )
         # Dev color is what we print the prompt in when user asks a question
         # in dev mode.
         self.color = color
         self.dev_color = 'blue' if self.color == 'red' else 'red'
         # Must create self.chat before setting _chat_prompt_keys,
         # and full_context after both of those.
-        self.chat = Chat.from_config(**chat_kwargs)
+        self.chat = Chat.from_template(**chat_kwargs)
         self.default_user_key, self.backup_user_key = self._chat_prompt_keys()
         self.full_context = 'full_code' in self.field_names()
         self.prompt_name = prompt_name
         self.repr_func = partial(truncated_repr, max_len=max_len_per_var)
         self.silent = silent
         self.parse_func = parse_func
         # This gets updated every time the user asks a question.
@@ -160,27 +176,37 @@
                 )
         return default, backup
 
     def field_names(self, key=''):
         """Get names of variables that are expected to be passed into default
         user prompt template.
 
+        Parameters
+        ----------
+        key : str
+            Determines which user prompt type to use. By default, roboduck
+            provides "contextful" (which will include the source code, variable
+            values, and the stack trace when appropriate) and "contextless"
+            (which includes only the user question). We default to
+            "contextful" here.
+
         Returns
         -------
         set[str]
         """
         return self.chat.input_variables(key)
 
     def _get_next_line(self, code_snippet):
         """Retrieve next line of code that will be executed. Must call this
-        before we remove the duck() call.
+        before we remove the duck() call. We use this in `_get_prompt_kwargs`
+        during interactive debugging sessions.
 
         Parameters
         ----------
-        code_snippet: str
+        code_snippet : str
         """
         lines = code_snippet.splitlines()
         max_idx = len(lines) - 1
 
         # Adjust f_lineno because it's 1 - indexed by default.
         # Set default next_line in case we don't find any valid line.
         line_no = self.curframe.f_lineno - 1
@@ -197,17 +223,18 @@
         """Construct a dictionary describing the current state of our code
         (variable names and values, source code, file type). This will be
         passed to our langchain chat.reply() method to fill in the debug prompt
         template.
 
         Returns
         -------
-        dict: contains keys 'code', 'local_vars', 'global_vars', 'file_type'.
-        If we specified full_context=True on init, we also include the key
-        'full_code'.
+        dict
+            contains keys 'code', 'local_vars', 'global_vars', 'file_type'.
+            If we specified full_context=True on init, we also include the key
+            'full_code'.
         """
         res = {}
 
         # Get current code snippet.
         # Fails when running code from cmd line like:
         # 'python -c "print(x)"'.
         # Haven't been able to find a way around this yet.
@@ -215,38 +242,27 @@
             # Find next line before removing duck call to avoid messing up our
             # index.
             code_snippet = inspect.getsource(self.curframe)
             res['next_line'] = self._get_next_line(code_snippet)
             res['code'] = self._remove_debugger_call(code_snippet)
         except OSError as err:
             self.error(err)
-        res['local_vars'] = type_annotated_dict_str(
-            {k: v for k, v in self.curframe_locals.items()
-             if not is_ipy_name(k)},
-            self.repr_func
-        )
 
         # Get full source code if necessary.
         if self.full_context:
             # File is a string, either a file name or something like
             # <ipython-input-50-e97ed612f523>.
             file = inspect.getsourcefile(self.curframe.f_code)
             if file.startswith('<ipython'):
                 # If we're in ipython, ipynbname.path() throws a
                 # FileNotFoundError.
                 try:
                     full_code = load_ipynb(ipynbname.path())
                     res['file_type'] = 'jupyter notebook'
                 except FileNotFoundError:
-                    # TODO: maybe ipython session needs to use a modified
-                    # version of this func regardless of self.full_context,
-                    # and should return full code as list initially and
-                    # override res['code'] with last executed cell. Otherwise
-                    # I think getsource(curframe) may load a lot more code than
-                    # we usually want in ipython session.
                     full_code = load_current_ipython_session()
                     res['file_type'] = 'ipython session'
             else:
                 with open(file, 'r') as f:
                     full_code = f.read()
                 res['file_type'] = 'python script'
             res['full_code'] = self._remove_debugger_call(full_code)
@@ -255,26 +271,42 @@
             # This is intentionally different from the used_tokens line in the
             # if clause - we only want to consider local code here.
             used_tokens = set(res['code'].split())
 
         # Namespace is often polluted with lots of unused globals (htools is
         # very much guilty of this 😬) and we don't want to clutter up the
         # prompt with these.
+        res['local_vars'] = type_annotated_dict_str(
+            {k: v for k, v in self.curframe_locals.items()
+             if k in used_tokens and not is_ipy_name(k)},
+            self.repr_func
+        )
         res['global_vars'] = type_annotated_dict_str(
             {k: v for k, v in self.curframe.f_globals.items()
              if k in used_tokens and not is_ipy_name(k)},
             self.repr_func
         )
         return res
 
     @staticmethod
     def _remove_debugger_call(code_str):
         """Remove `duck` function call (our equivalent of `breakpoint` from
         source code string. Including it introduces a slight risk that gpt
         will fixate on this mistery function as a potential bug cause.
+
+        Parameters
+        ----------
+        code_str : str
+            Source code snippet. We want to remove the `duck()` call (which
+            sometimes includes kwargs) to prevent this from distracting the
+            LLM.
+
+        Returns
+        -------
+        str
         """
         return '\n'.join(line for line in code_str.splitlines()
                          if not line.strip().startswith('duck('))
 
     def onecmd(self, line):
         """Base class describes this as follows:
 
@@ -284,15 +316,15 @@
 
         We add an extra check in the if block to check if the user asked a
         question. If so, we ask gpt. If not, we treat it as a regular pdb
         command.
 
         Parameters
         ----------
-        line: str or tuple
+        line : str or tuple
             If str, this is a regular line like in the standard debugger.
             If tuple, this contains (line str, stack trace str - see
             roboduck.errors.post_mortem for the actual insertion into the
             cmdqueue). This is for use with the debug_stack_trace mode.
         """
         if isinstance(line, tuple):
             line, stack_trace = line
@@ -311,22 +343,22 @@
 
     def ask_language_model(self, question, stack_trace='', verbose=False):
         """When the user asks a question during a debugging session, query
         gpt for the answer and type it back to them live.
 
         Parameters
         ----------
-        question: str
+        question : str
             User question, e.g. "Why are the first three values in nums equal
             to 5 when the input list only had a single 5?". (Example is from
             a faulty bubble sort implementation.)
-        stack_trace: str
+        stack_trace : str
             When using the "debug_stack_trace" prompt, we need to pass a
             stack trace string into the prompt.
-        verbose: bool
+        verbose : bool
             If True, print the full gpt prompt in red before making the api
             call. User activates this mode by prefixing their question with
             '[dev]'. This overrides self.silent.
         """
         # Don't provide long context-laden prompt if nothing has changed since
         # the user's last question. This is often a followup/clarifying
         # question.
@@ -384,17 +416,17 @@
                 print(colored(answer, self.color))
 
         parsed_kwargs = self.parse_func(answer)
         # When using the `duck` jupyter magic in "insert" mode, we reference
         # the CodeCompletionCache to populate the new code cell.
         CodeCompletionCache.last_completion = answer
         CodeCompletionCache.last_explanation = parsed_kwargs['explanation']
-        # TODO: maybe check if code or full_code is more appropriate to store
-        # as last_code, either depending on self.full_context or by doing a
-        # quick str similarity to each.
+        # Built-in prompts always ask for a fixed version of the relevant
+        # snippet, not the whole code, so that's what we store here and use for
+        # the diff operation.
         # Contextless prompt has no `code` key.
         old_code = prompt_kwargs.get('code', '')
         new_code = parsed_kwargs['code']
         CodeCompletionCache.last_code_diff = colordiff_new_str(old_code,
                                                                new_code)
         CodeCompletionCache.last_code = old_code
         CodeCompletionCache.last_new_code = new_code
@@ -403,14 +435,22 @@
 
     def precmd(self, line):
         """We need to define this to make our errors module work. Our
         post_mortem function sometimes places a tuple in our debugger's
         cmdqueue and precmd is called as part of the default cmdloop method.
         Technically it calls postcmd too but we don't need to override that
         because it does nothing with its line argument.
+
+        Parameters
+        ----------
+        line : str or tuple
+            If a tuple, it means roboduck.errors.excepthook is being called
+            and an error has occurred. The stack trace is passed in as the
+            second of two items, where the first item is the same object that
+            is normally passed in.
         """
         if isinstance(line, tuple):
             line, trace = line
             return super().precmd(line), trace
         return super().precmd(line)
 
     def print_stack_entry(self, frame_lineno, prompt_prefix='\n-> '):
@@ -419,15 +459,16 @@
 
         ```
         > <ipython-input-20-9c67d40d0f93>(2)<module>()
         -> print + 6
         ```
 
         In silent mode (like when using the roboduck logger with stdout=False),
-        we want to disable that message.
+        we want to disable that message. When silent=False, this behaves
+        identically to the standard pdb equivalent.
         """
         if self.silent:
             return
         frame, lineno = frame_lineno
         if frame is self.curframe:
             prefix = '> '
         else:
```

### Comparing `roboduck-0.2.0/roboduck/decorators.py` & `roboduck-0.3.0/roboduck/decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-"""Miscellaneous decorators used throughout the library.
-"""
+"""Miscellaneous decorators used throughout the library."""
 import warnings
 from functools import partial, wraps
 from inspect import signature, Parameter
 
 
 def typecheck(func_=None, **types):
     """Decorator to enforce type checking for a function or method. There are
     two ways to call this: either explicitly passing argument types to the
     decorator, or letting it infer them using type annotations in the function
-    that will be decorated. We allow multiple both usage methods since older
+    that will be decorated. We allow both usage methods since older
     versions of Python lack type annotations, and also because I feel the
     annotation syntax can hurt readability.
 
-    Ported from htools to avoid extra dependency.
+    Ported from [htools](https://github.com/hdmamin/htools) to avoid extra
+    dependency.
 
     Parameters
     ----------
-    func_: function
+    func_ : function
         The function to decorate. When using decorator with
         manually-specified types, this is None. Underscore is used so that
         `func` can still be used as a valid keyword argument for the wrapped
         function.
-    types: type
+    types : type
         Optional way to specify variable types. Use standard types rather than
         importing from the typing library, as subscripted generics are not
         supported (e.g. typing.List[str] will not work; typing.List will but at
         that point there is no benefit over the standard `list`).
 
     Examples
     --------
@@ -80,15 +80,29 @@
     elif not types:
         types = {k: v.annotation
                  for k, v in signature(func_).parameters.items()
                  if not v.annotation == Parameter.empty}
 
     @wraps(func_)
     def wrapper(*args, **kwargs):
-        fargs = signature(wrapper).bind(*args, **kwargs).arguments
+        sig = signature(wrapper)
+        try:
+            fargs = sig.bind(*args, **kwargs).arguments
+        except TypeError as e:
+            # Default error message is not very helpful if we don't handle this
+            # case separately.
+            expected_positional = [name for name, p in sig.parameters.items()
+                                   if 'positional' in str(p.kind).lower()]
+            if args and not expected_positional:
+                raise TypeError(
+                    'Received positional arg(s) but expected none. Expected '
+                    f'arguments: {list(sig.parameters)}'
+                )
+            else:
+                raise e
         for k, v in types.items():
             if k in fargs and not isinstance(fargs[k], v):
                 raise TypeError(
                     f'{k} must be {str(v)}, not {type(fargs[k])}.'
                 )
         return func_(*args, **kwargs)
     return wrapper
@@ -96,24 +110,24 @@
 
 def add_kwargs(func, fields, hide_fields=(), strict=False):
     """Decorator that adds parameters into the signature and docstring of a
     function that accepts **kwargs.
 
     Parameters
     ----------
-    func: function
+    func : function
         Function to decorate.
-    fields: list[str]
+    fields : list[str]
         Names of params to insert into signature + docstring.
-    hide_fields: list[str]
+    hide_fields : list[str]
         Names of params that are *already* in the function's signature that
         we want to hide. To use a non-empty value here, we must set strict=True
         and the param must have a default value, as this is what will be used
         in all subsequent calls.
-    strict: bool
+    strict : bool
         If true, we do two things:
         1. On decorated function call, check that the user provided all
         expected arguments.
         2. Enable the use of the `hide_fields` param.
 
     Returns
     -------
@@ -174,19 +188,23 @@
 
 
 def store_class_defaults(cls=None, attr_filter=None):
     """Class decorator that stores default values of class attributes (can be
     all or a subset). Default here refers to the value at class definition
     time.
 
+    Examples
+    --------
+    ```
     @store_class_defaults(attr_filter=lambda x: x.startswith('last_'))
     class Foo:
         last_bar = 3
         last_baz = 'abc'
         other = True
+    ```
 
     >>> Foo._class_defaults
 
     {'last_bar': 3, 'last_baz': 'abc'}
 
     Or use the decorator without parentheses to store all values at definition
     time. This is usually unnecessary. If you do provide an attr_filter, it
@@ -218,16 +236,15 @@
             f'Class {cls} already has attribute {name}. store_class_defaults '
             'decorator would overwrite that. Exiting.'
         )
     setattr(cls, name, defaults)
 
     @classmethod
     def reset_class_vars(cls):
-        """Reset all default class attributes to their defaults.
-        """
+        """Reset all default class attributes to their defaults."""
         for k, v in cls._class_defaults.items():
             try:
                 setattr(cls, k, v)
             except Exception as e:
                 warnings.warn(f'Could not reset class attribute {k} to its '
                               f'default value:\n\n{e}')
 
@@ -241,15 +258,21 @@
     return cls
 
 
 def add_docstring(func):
     """Add the docstring from another function/class to the decorated
     function/class.
 
-    Ported from htools to avoid extra dependency.
+    Ported from [htools](https://github.com/hdmamin/htools) to avoid extra
+    dependency.
+
+    Parameters
+    ----------
+    func : function
+        Function to decorate.
 
     Examples
     --------
     ```
     @add_docstring(nn.Conv2d)
     class ReflectionPaddedConv2d(nn.Module):
         # ...
@@ -257,8 +280,8 @@
     """
     def decorator(new_func):
         new_func.__doc__ = f'{new_func.__doc__}\n\n{func.__doc__}'
         @wraps(new_func)
         def wrapper(*args, **kwargs):
             return new_func(*args, **kwargs)
         return wrapper
-    return decorator
+    return decorator
```

### Comparing `roboduck-0.2.0/roboduck/errors.py` & `roboduck-0.3.0/roboduck/errors.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,39 +33,43 @@
 
 default_excepthook = sys.excepthook
 ipy = get_ipython()
 
 
 @add_docstring(DuckDB.__init__)
 def post_mortem(t=None, Pdb=DuckDB, trace='', prompt_name='debug_stack_trace',
-                colordiff=True, **kwargs):
+                colordiff=True, interactive=False, **kwargs):
     """Drop-in replacement (hence the slightly odd arg order, where trace is
     required but third positionally) for pdb.post_mortem that allows us to get
     both the stack trace AND global/local vars from the program state right
     before an exception occurred.
 
     Parameters
     ----------
-    t: some kind of traceback type?
-        A holdover from the default post_mortem class, not actually sure what
-        type this is but it doesn't really matter for our use.
-    Pdb: type
+    t : traceback
+        Error traceback if one is available. Single character name is a
+        holdover from the default post_mortem.
+    Pdb : type
         Debugger class. Name is capitalized to provide consistent interface
         with default post_mortem function.
-    trace: str
+    trace : str
         Stack trace formatted as a single string. Required - default value
         just helps us maintain a consistent interface with pdb.post_mortem.
-    prompt_name: str
+    prompt_name : str
         The prompt name that will be passed to our debugger class. Usually
         should leave this as the default. We expect the name to contain
         'debug' and will warn if it doesn't.
-    colordiff: bool
+    colordiff : bool
         If True, the new code snippet in the exception will print new
         parts in green.
-    kwargs: any
+    interactive : bool
+        If False, LLM will just explain the error and exit. If True, user
+        instead will be thrown into an interactive debugging session where
+        they can ask followup questions.
+    kwargs : any
         Additional kwargs to pass to debugger class constructor. The docstring
         of the default class is included below for reference.
     """
     if t is None:
         t = sys.exc_info()[2]
         assert t is not None, "post_mortem outside of exception context"
     if 'debug' not in prompt_name:
@@ -85,15 +89,18 @@
         'prompt kwargs before calling gpt. If you can read this, can you '
         'indicate that in your response?'
     )
     kwargs['color'] = kwargs.get('color', 'red')
     p = Pdb(prompt_name=prompt_name, **kwargs)
     p.reset()
     p.cmdqueue.insert(0, (dummy_question, trace))
-    p.cmdqueue.insert(1, 'q')
+    if interactive:
+        print('When done, enter `q` to quit.\n')
+    else:
+        p.cmdqueue.insert(1, 'q')
     p.interaction(None, t)
 
     # Make gpt explanation available as part of last error message,
     # accessible via sys.last_value.
     last_value = getattr(sys, 'last_value', None)
     if CodeCompletionCache.last_completion and last_value:
         code_name = 'last_code_diff' if colordiff else 'last_new_code'
@@ -137,21 +144,44 @@
 
 def excepthook(etype, val, tb, prompt_name='debug_stack_trace',
                auto=False, cls=DuckDB, **kwargs):
     """Replaces sys.excepthook when module is imported. When an error is
     thrown, the user is asked whether they want an explanation of what went
     wrong. If they enter 'y' or 'yes', it will query gpt for help. Unlike
     roboduck.debug.duck(), the user does not need to manually type a
-    question, and we don't linger in the debugger - we just write gpt's
-    explanation and exit.
+    question. By default we don't linger in the debugger - we just provide an
+    explanation and exit. Passing in interactive=True allows the user to ask
+    followup questions.
 
     Disable by calling roboduck.errors.disable().
 
     Parameters are the same as the default sys.excepthook function. Kwargs
-    are forwarded to our custom postmortem function.
+    are forwarded to our custom post_mortem function.
+
+    Parameters
+    ----------
+    etype : type
+        The class of exception that just occurred.
+    val : Exception
+        The error that just occurred.
+    tb : traceback
+        The traceback from the error that just occurred.
+    prompt_name : str
+        The roboduck prompt to use (can be a builtin option in
+        roboduck.prompts.chat or a path to a user-defined yaml file).
+    auto : bool
+        If True, automatically start explaining every error that occurs
+        (usually not recommended). If False, user will be asked to type y/n
+        before asking an LLM.
+    cls : type
+        The debugger class to use. By default it's the roboduck equivalent of
+        pdb.Pdb, but you could also subclass DuckDB and do something custom.
+    kwargs : any
+        Additional kwargs to pass to the debugger cls,
+        e.g. "model_name='gpt-4'".
     """
     sys.last_type, sys.last_value, sys.last_traceback = etype, val, tb
     trace = print_exception(etype, val, tb)
     if not kwargs.get('silent', False):
         print(trace)
     kwargs.update(prompt_name=prompt_name, trace=trace, t=tb, Pdb=cls)
     if auto:
@@ -168,25 +198,35 @@
 def enable(**kwargs):
     """Enable conversational debugging mode. This is called automatically on
     module import. However, users may wish to make changes, e.g. set auto=True
     or pass in a custom debugger cls, and this function makes that possible.
 
     Parameters
     ----------
-    kwargs: any
-        auto (bool) - if True, automatically have gpt explain every error that
-            occurs. Mostly useful for logging in production. You almost
-            certainly want to keep this as the default of False for any
+    kwargs : any
+        These are passed to our custom debugger class. Some common args are
+        below:
+
+        auto (bool) - if True, automatically have an LLM explain every error
+            that occurs without asking the user for confirmation. This is used
+            in our logging module, for instance. You almost
+            certainly want to keep this as False (the default) for any
             interactive development.
+        interactive (bool) - if True, error explanations will leave the user in
+            an interactive session where they can ask followup questions. If
+            False (the default), we will simply explain the error and exit the
+            session (more similar to standard python error handling).
         cls (type) - the debugger class to use.
         prompt_name (str) - determines what prompt/prompt_name the custom
-            debugger uses, e.g. "debug_stack_trace"
+            debugger uses, e.g. "debug_stack_trace". Users can also define
+            their own custom prompt
+            (https://hdmamin.github.io/roboduck/custom_prompts/)
+            and pass in the file path here.
         colordiff (bool) - if True, new code snippet will print new parts
             in green.
-        Or any other args that can be passed to our debugger cls.
     """
     hook = partial(excepthook, **kwargs)
 
     def ipy_excepthook(self, etype, evalue, tb, tb_offset):
         """IPython doesn't use sys.excepthook. We have to handle this case
         separately and make sure it expects the right argument names.
         """
@@ -199,34 +239,35 @@
     try:
         ipy.set_custom_exc((Exception,), ipy_excepthook)
     except AttributeError:
         pass
 
 
 def disable():
-    """Revert to default behavior when exceptions are thrown.
-    """
+    """Revert to default behavior when exceptions are thrown."""
     sys.excepthook = default_excepthook
     try:
         # Tried doing `ipy.set_custom_exc((Exception,), None)` as suggested by
         # stackoverflow and chatgpt but it didn't quite restore the default
         # behavior. Manually remove this instead. I'm assuming only one custom
         # exception handler can be assigned for any one exception type and that
         # if we call disable(), we wish to remove the handler for Exception.
         ipy.custom_exceptions = tuple(x for x in ipy.custom_exceptions
                                       if x != Exception)
     except AttributeError:
         pass
 
 
 def stack_trace():
-    # Lets us recover stack trace as string outside of the functions defined
-    # above, which generally only execute automatically when exceptions are
-    # thrown. Don't just define this as a partial because that requires
-    # sys.last_value etc. to be available at import time, which it often isn't.
+    """Lets us recover stack trace as string outside of the functions defined
+    above, which generally only execute automatically when exceptions are
+    thrown. Don't just define this as a partial because that requires
+    sys.last_value etc. to be available at import time, which it often isn't.
+    In the end I think I only used this for development purposes.
+    """
     try:
         return print_exception(sys.last_type, sys.last_value,
                                sys.last_traceback)
     except AttributeError as e:
         raise RuntimeError('No stack trace available because an error has '
                            'not been thrown.') from e
```

### Comparing `roboduck-0.2.0/roboduck/ipy_utils.py` & `roboduck-0.3.0/roboduck/ipy_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,28 +16,29 @@
 def load_ipynb(path, save_if_self=True):
     """Loads ipynb and formats cells into 1 big string.
 
     Adapted from htools.cli.ReadmeUpdater method.
 
     Parameters
     ----------
-    path: Path
+    path : Path
         Path to notebook to load.
-    save_if_self: bool
+    save_if_self : bool
         If True, check if this is being called from the current notebook. If
         so, save it. (If not, we never save - auto saving is only intended to
         address the scenario where we're in an active notebook and call this
         function before recent changes have been saved. The load_ipynb call
         itself means that at least 1 change has inevitably occurred since
         saving.)
 
     Returns
     -------
-    str: Code contents of notebook. Each cell is enclosed in triple backticks
-    and separated by newlines.
+    str
+        Code contents of notebook. Each cell is enclosed in triple backticks
+        and separated by newlines.
     """
     if save_if_self:
         try:
             self_path = ipynbname.path()
         except FileNotFoundError:
             pass
         else:
@@ -45,38 +46,45 @@
                 save_notebook(path)
 
     with open(path, 'r') as f:
         cells = json.load(f)['cells']
 
     cell_str = ''
     for cell in cells:
-        if not cell['source']: continue
+        if not cell['source']:
+            continue
         source = '\n' + ''.join(cell['source']) + '\n'
         if cell['cell_type'] == 'code':
             source = '\n```' + source + '```\n'
         cell_str += source
     return cell_str
 
 
 def load_current_ipython_session(formatted=True):
     """Load current ipython session as a list and optionally convert it to a
     nicely formatted str with each cell enclosed in triple backticks.
 
     Parameters
     ----------
-    formatted: bool
-        If True, format list of cells into a single str like:
+    formatted : bool
+        If True, format list of cells into a single str like this (note: if
+        you don't see any backticks below, know that each print statement is
+        enclosed in a separate pair of triple backticks. Rendering this nicely
+        with mkdocs is very tricky and even if it worked, it would badly mess
+        up readability for people viewing the docstring in their IDE):
 
+        '''
         ```
         print('This is cell 1 code.')
         ```
 
         ```
         print('This is cell 2 code.')
         ```
+        '''
 
         If False, leave it as a list of strings where each string contains
         content from one cell.
 
     Returns
     -------
     list or str
@@ -97,39 +105,44 @@
     return cells
 
 
 def is_ipy_name(
         name,
         count_as_true=('In', 'Out', '_dh', '_ih', '_ii', '_iii', '_oh')
 ):
-    """Check if a variable name looks like an ipython output cell, e.g.
+    """```plaintext
+    Check if a variable name looks like an ipython output cell name, e.g.
     "_49", "_", or "__".
 
-    Ported from htools to avoid extra dependency.
+    Ported from [htools](https://github.com/hdmamin/htools) to avoid extra
+    dependency.
 
     More examples:
-    Returns True for names like (technically not sure if something like "__i3"
-    is actually used in ipython, but it looks like something we probably want
-    to remove in these contexts anyway /shrug):
+    Returns True for names like this (technically not sure if something like
+    "__i3" is actually used in ipython, but it looks like something we
+    probably want to remove it in these contexts anyway.
     ['_', '__', '_i3', '__i3', '_4', '_9913', '__7', '__23874']
 
     Returns False for names like
     ['_a', 'i22', '__0i', '_03z', '__99t']
     and most "normal" variable names.
+    ```
 
     Parameters
     ----------
-    name: str
-    count_as_true: Iterable[str]
+    name : str
+        The variable name to check.
+    count_as_true : Iterable[str]
         Additional variable names that don't necessarily fit the standard
         pattern but should nonetheless return True if we encounter them.
 
     Returns
     -------
-    bool: True if it looks like an ipython output cell name, False otherwise.
+    bool
+        True if it looks like an ipython output cell name, False otherwise.
     """
     # First check if it fits the standard leading underscore format.
     # Easier to handle the "only underscores" case separately because we want
     # to limit the number of underscores for names like "_i3".
     pat = '^_{1,2}i?\\d*$'
     is_under = bool(re.match(pat, name)) or not name.strip('_')
     return is_under or name in count_as_true
@@ -139,18 +152,17 @@
     """Save a jupyter notebook. We use this in load_ipynb (optionally) to
     ensure that when we load a notebook's source
     code, we get the most up to date version. Adapted from
     https://stackoverflow.com/questions/32237275/save-an-ipython-notebook-programmatically-from-within-itself/57814673#57814673
 
     Parameters
     ----------
-    file_path: str
+    file_path : str
         Path to notebook that you want to save.
     """
-
     def file_md5(path):
         with open(path, 'rb') as f:
             text = f.read()
         return hashlib.md5(text).hexdigest()
 
     start_md5 = file_md5(file_path)
     display(Javascript('IPython.notebook.save_checkpoint();'))
```

### Comparing `roboduck-0.2.0/roboduck/langchain/callbacks.py` & `roboduck-0.3.0/roboduck/langchain/callbacks.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,29 +12,35 @@
     """Streams to stdout by types one character at a time and allows us to
     control text color and typing speed.
 
     The parent class mostly just prevents us from having to write a
     bunch of boilerplate methods that do nothing, but it does make sense
     since this callback implements a specific subcase of streaming to stdout.
     """
+
     always_verbose = True
 
     def __init__(self, color='green', sleep=.01):
         """
         Parameters
         ----------
-        color: str
+        color : str
             Color to print gpt response in. Passing in an empty str (or None)
             will use the default color.
-        sleep: float
+        sleep : float
             Time to wait after "typing" each character. Using zero pause is a
             bit annoying to read comfortably, IMO.
         """
         self.color = color
         self.sleep = sleep
 
     def on_llm_new_token(self, token, **kwargs):
-        """Runs on new LLM token. Only called when streaming is enabled."""
+        """Runs on new LLM token. Only called when streaming is enabled.
+
+        Parameters
+        ----------
+        token : str
+        """
         for char in token:
             sys.stdout.write(colored(char, self.color))
             time.sleep(self.sleep)
         sys.stdout.flush()
```

### Comparing `roboduck-0.2.0/roboduck/langchain/chat.py` & `roboduck-0.3.0/roboduck/langchain/chat.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 from langchain.callbacks.base import CallbackManager
 from langchain.chat_models import ChatOpenAI
 from langchain.schema import ChatResult, ChatGeneration, AIMessage, \
     SystemMessage
 from langchain.prompts import HumanMessagePromptTemplate
 import warnings
 
+from roboduck.config import apply_config_defaults
+from roboduck.decorators import add_kwargs
 from roboduck.langchain.callbacks import LiveTypingCallbackHandler
 from roboduck.langchain.utils import model_context_window
 from roboduck.prompts.utils import load_template
-from roboduck.decorators import add_kwargs
 
 
 class DummyChatModel:
     # Drop-in replacement for ChatOpenAI that just repeats the last message.
     # We'd have to be a bit more rigid about expects init args if we want to
     # subclass from BaseChatModel. For now this is fine.
 
@@ -56,53 +57,55 @@
 
 
 class Chat:
     """Convenience class to make it easier to interact with chat model via
     langchain. Allows you to specify reply types and kwargs via config, avoid
     manually tracking the conversation history, etc.
 
-    We recommend instantiating via the from_config factory method in most
+    We recommend instantiating via the from_template factory method in most
     cases.
     """
 
     def __init__(self, system, user, chat_class=ChatOpenAI,
                  history=(), streaming=True, **kwargs):
-        """
+        r"""
         Parameters
         ----------
-        system: str
+        system : str
             "system" message for chatGPT. This typically contains instructions
             for how GPT should behave when talking to the user.
-        user: str or dict
+        user : str or dict
             Defines one or more types of "user" messages for chatGPT. If you
             have multiple types, the keys in your dict will be used to
             define methods, so name them accordingly. E.g. if you pass in a
             dict with keys "question" and "comment", you will be able to call
             chat.comment(**kwargs) and chat.question(**kwargs).
-        chat_class: type
+        chat_class : type
             The class (usually provided by langchain) that represents the chat
             model we'll be conversing with.
-        history: listlike
+        history : listlike
             This will be used to store all the messages in our conversation.
-        streaming: bool
+            If not empty, it should contain AIMessage and HumanMessage objects
+            from a previous chat, but NOT a SystemMessage.
+        streaming : bool
             Determines whether to query the chat model in streaming mode.
             This is often desirable so that we can see incremental results
             instead of waiting for the whole completion to finish.
-        kwargs: any
+        kwargs : any
             Additional kwargs for chat_class. This can include both
             model_kwargs like temperature or top_p that affect completion
             directly, or other miscellaneous kwargs like `callback_manager`
             or `verbose`.
 
         Examples
         --------
         ```
         # Instantiate from builtin roboduck debugging prompt template (see
         # roboduck.prompts.chat.debug).
-        chat = Chat.from_config('debug')
+        chat = Chat.from_template('debug')
         message = chat.reply(
             code='a = 3\nb = ([0, 1], [2, 3])\nb[1].append(a)',
             question='I thought tuples were immutable. Why doesn\'t appending '
                      'a throw an error?',
             local_vars='{"a": 3, "b": ([0, 1], [2, 3])}',
             global_vars='{"x": True}', next_line='b[1].append(a)'
         )
@@ -119,14 +122,15 @@
             question='Could you expand on the part of your explanation where '
             'you said...'
         )
         ```
         """
         self.kwargs = dict(kwargs)
         self.kwargs.update(streaming=streaming)
+        apply_config_defaults(self.kwargs, template_only=False)
         if streaming and 'callback_manager' not in self.kwargs:
             self.kwargs['callback_manager'] = CallbackManager(
                 [LiveTypingCallbackHandler()]
             )
         self.chat = chat_class(**self.kwargs)
         self.context_window = model_context_window(
             self.kwargs.get('model_name')
@@ -155,16 +159,15 @@
         self._create_reply_methods()
 
     def _create_reply_methods(self):
         """Creates two options for user to send replies:
         1. call chat.reply(), using the key_ arg to determine which type of
         user_message is sent. The docstring shows the default user
         message type's fields but if you set the key accordingly you can pass
-        in fields for another message type. We choose not to infer key_
-        because some user_message types may accept the same fields.
+        in fields for another message type.
         2. call methods like chat.question() or chat.statement(), where 'chat'
         and 'statement' are the names of all available user message types
         (i.e. the keys of the `user` dict in the prompt config file). You can
         not pass in key_.
         """
         for k, v in self.user_templates.items():
             if hasattr(self, k):
@@ -182,100 +185,107 @@
         setattr(
             self,
             'reply',
             add_kwargs(self._reply, self.default_user_fields, strict=False)
         )
 
     @classmethod
-    def from_config(cls, name, **kwargs):
+    def from_template(cls, name, **kwargs):
         """Instantiate a Chat object from a yaml template (either builtin
         roboduck prompt templates like in roboduck.prompts.chat or a user
         defined file with the same format).
 
         Parameters
         ----------
-        name: str
+        name : str
             Name of a builtin roboduck prompt template
             (see roboduck.prompts.utils.available_templates()) or a file
             containing a user-defined prompt template.
-        kwargs: any
+        kwargs : any
             Additional kwargs to pass to constructor. These take precedence
             over the config file if their is a collision, i.e. the config
             provides the defaults but you can override them.
 
         Returns
         -------
         Chat
         """
         template = load_template(name)
+        # Important that we call this BEFORE taking user kwargs into account.
+        # Init will handle the resolution that occurs afterwards, do not make
+        # a second call to apply defaults in this method.
+        apply_config_defaults(template['kwargs'], template_only=True)
         if kwargs:
             template['kwargs'].update(kwargs)
         kwargs = template.pop('kwargs', {})
         return cls(**template, **kwargs)
 
     def user_message(self, *, key_='', **kwargs):
         """Get a fully resolved user reply as a string.
 
         Parameters
         ----------
-        key_: str
+        key_ : str
             Determines which reply type to use. If empty, falls back to default
             reply type.
-        kwargs: str
+        kwargs : str
             The required fields for the selected reply type.
 
         Returns
         -------
         str
         """
         key = key_ or self.default_user_key
         template = self.user_templates[key]
         return template.format(**kwargs)
 
     def _reply(self, *, key_='', **kwargs):
+        """The basic functionality that will underlie the dynamically generated
+        `reply` method and its other aliases. Passes user reply and
+        conversational history to an LLM for a response.
+
+        Parameters
+        ----------
+        key_: str
+            Determines which type of user reply to use. Defaults to the first
+            type defined in the prompt config.
+        kwargs: any
+            Fields expected by the relevant user prompt type. These will be
+            injected into the docstrings of our dynamically generated methods.
+
+        Returns
+        -------
+        AIMessage
+        """
         user_message = self.user_message(key_=key_, **kwargs)
         self._history.append(user_message)
-        # Technically I don't think this is the exact prompt that gets sent
-        # but it's close enough for our estimate. We're doing some pretty rough
-        # arithmetic anyway with the token->word conversions.
-        n_words = len(self.history(sep='\n').split())
-        if n_words > self.prompt_words_hard_limit:
-            raise ValueError(
-                f'Chat history contains ~{n_words:,} words which is more than '
-                f'the model can support. Context window is ~'
-                f'{self.prompt_words_hard_limit:,} words '
-                f'({self.context_window:,} tokens).'
-            )
-        elif n_words > self.prompt_words_soft_limit:
-            warnings.warn(
-                f'Chat history contains ~{n_words:,} words which means the '
-                f'model\'s context window of ~'
-                f'{self.prompt_words_hard_limit:,} words '
-                f'({self.context_window:,} tokens) will be the bigger limiting '
-                f'factor than your max_length hyperparameter.'
-            )
+        self._truncate_history()
         try:
             response = self.chat(self._history)
         except Exception as e:
             self._history.pop(-1)
             raise e
         self._history.append(response)
         return response
 
     def history(self, sep='\n\n', speaker_prefix=True):
         """Return chat history as a single string.
 
         Parameters
         ----------
-        sep: str
+        sep : str
             Character(s) used to separate conversational turns in the output.
             The default leaves 1 blank line between each turn.
-        speaker_prefix: bool
+        speaker_prefix : bool
             If True, preprend each turn with "Human" or "AI" depending on the
             speaker.
+
+        Returns
+        -------
+        str
         """
         res = []
         for row in self._history:
             reply = row.content
             if speaker_prefix:
                 speaker = type(row).__name__.split('Message')[0]
                 reply = f'{speaker}: {reply}'
@@ -283,18 +293,54 @@
         return sep.join(res)
 
     def input_variables(self, key=''):
         """Get names of fields that user has to pass in when replying.
 
         Parameters
         ----------
-        key: str
+        key : str
             Name of user reply type. Falls back to the default reply type if
             none is provided.
 
         Returns
         -------
         set[str]
         """
         template = self.user_templates[key or self.default_user_key]
         return set(template.input_variables)
 
+    def _truncate_history(self):
+        """Dynamically discard old turns until our history is an
+        acceptable size for our LLM's context window. Operates in place. Called
+        automatically by _reply.
+        """
+        # Technically I don't think this is the exact prompt that gets sent
+        # but it's close enough for our estimate. We're doing some pretty rough
+        # arithmetic anyway with the token->word conversions.
+        n_words = len(self.history(sep='\n').split())
+        while n_words > self.prompt_words_hard_limit:
+            if len(self._history) <= 2:
+                raise ValueError(
+                    f'Chat history contains ~{n_words:,} words even when only '
+                    f'including the system prompt and the latest user message,'
+                    f' which is more than this model can support. Context '
+                    f'window is ~{self.prompt_words_hard_limit:,} words '
+                    f'({self.context_window:,} tokens). You could try using '
+                    f'a different model_name with a larger context window, a '
+                    f'prompt_name corresponding to a more concise prompt, '
+                    f'a smaller max_len_per_var (default is 79), or '
+                    f'refactoring your code (this error could potentially be '
+                    f'caused by a truly enormous function).'
+                )
+            turn = self._history.pop(1)
+            # Subtract an extra 1 for the speaker prefix. This is an
+            # approximate calculation regardless so it doesn't really matter
+            # but it also shouldn't hurt.
+            n_words = n_words - len(turn.content.split()) - 1
+
+        if n_words > self.prompt_words_soft_limit:
+            warnings.warn(
+                f'Chat history contains ~{n_words:,} words which means the '
+                f'model\'s context window of ~{self.prompt_words_hard_limit:,}'
+                f' words ({self.context_window:,} tokens) will be the '
+                'bigger limiting factor than your max_length hyperparameter.'
+            )
```

### Comparing `roboduck-0.2.0/roboduck/logging.py` & `roboduck-0.3.0/roboduck/logging.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,66 +31,81 @@
 
     def __init__(self, name, colordiff=False,
                  fmt='%(asctime)s [%(levelname)s]: %(message)s', stdout=True,
                  path='', fmode='a', **kwargs):
         """
         Parameters
         ----------
-        name: str
+        name : str
             Same as base logger name arg.
-        colordiff: bool
+        colordiff : bool
             Another kwarg to pass to our excepthook function. This is separate
             from the others because we want to use a different default than the
             function has since we often log to a file, in which case
             colordiff=True may be undesirable.
-        fmt: str
+        fmt : str
             Defines logging format. The default format produces output like
             this when an error is logged:
             2023-03-08 19:20:52,514 [ERROR]: list indices must be integers or
             slices, not tuple
-        stdout: bool
+        stdout : bool
             If True, logged items will appear in stdout. You are free to log
-            to both stdout and a file, neither, or one or the other.
-        path: str or Path
+            to both stdout and a file OR just one (selecting neither will raise
+            an error because logger would be useless in that case).
+        path : str or Path
             If provided, we log to this file (the dir structure does not need
             to exist already). If None, we do not log to a file.
-        fmode: str
+        fmode : str
             Write mode used when path is not None. Usually 'a' but 'w' might
             be a reasonable choice in some circumstances.
-        kwargs: any
+        kwargs : any
             Kwargs that can be passed to our excepthook function. Most of these
             should generally be kwargs for your debugger class,
             e.g. RoboDuckDb. These will be updated with the specified
             `colordiff` as well - we want to set the default to False here
              because we often want to log to a file, where this will probably
              not render correctly.
         """
+        if not stdout and not path:
+            raise RuntimeError(
+                f'{type(self).__name__} requires that you set stdout=True '
+                f'and/or provide a non-empty path. Currently, your logger '
+                f'would do neither and be useless.'
+            )
+
         super().__init__(name)
         self.excepthook_kwargs = kwargs or {}
-        # TODO testing. Previously had silent=True hardcoded. Still considering
-        # desired behavior here.
-        defaults = dict(auto=True, sleep=0, silent=True)
+        # Always want silent=True because we don't care about live typing here.
+        # If stdout=True, our super()._log() call still ensures that we log to
+        # stdout after the gpt call completes.
+        defaults = dict(auto=True, sleep=0, silent=True, interactive=False)
         for k, v in defaults.items():
             if self.excepthook_kwargs.get(k, v) != v:
                 warnings.warn(
                     f'You tried to set {k}={self.excepthook_kwargs[k]} '
-                    f'but it must equal {v} in logger.'
+                    f'but it must equal {v} in logger. Your arg will be'
+                    f'overridden.'
                 )
         self.excepthook_kwargs.update(defaults)
         self.excepthook_kwargs['colordiff'] = self.excepthook_kwargs.get(
             'colordiff', colordiff
         )
         self._add_handlers(fmt, stdout, path, fmode)
 
     def _add_handlers(self, fmt, stdout, path, fmode):
         """Set up handlers to log to stdout and/or a file."""
         formatter = Formatter(fmt)
         handlers = []
         if stdout:
             handlers.append(StreamHandler(sys.stdout))
+        else:
+            # If we don't set this when stdout is False, the root logger ends
+            # up logging to stdout anyway.
+            self.propagate = False
+
         if path:
             path = Path(path).resolve()
             os.makedirs(path.parent, exist_ok=True)
             handlers.append(FileHandler(path, fmode))
         for handler in handlers:
             handler.setFormatter(formatter)
             self.addHandler(handler)
@@ -100,29 +115,43 @@
         """This is where we insert our custom logic to get error explanations.
         We keep the import inside the method to avoid overwriting
         sys.excepthook whenever the logging module is imported.
 
         Low-level logging routine which creates a LogRecord and then calls
         all the handlers of this logger to handle the record.
         """
-        tmp = sys.exc_info()[2]
         if isinstance(msg, Exception) and sys.exc_info()[2]:
             from roboduck import errors
             errors.excepthook(type(msg), msg, msg.__traceback__,
                               **self.excepthook_kwargs)
             msg = sys.last_value
             errors.disable()
 
         return super()._log(level, msg, args, exc_info=exc_info,
                             extra=extra, stack_info=stack_info)
 
 
 def getLogger(name=None, **kwargs):
-    """Mimics interface of builtin logging module. I.e. we can do:
+    """Mimics interface of builtin logging.getLogger, but with our custom
+    logger that ensures all errors explain themselves.
+
+    Parameters
+    ----------
+    kwargs : any
+        These are passed to roboduck.errors.post_mortem which in turn passes
+        them to our custom debugger class. The most important arg here is:
+
+        prompt_name (str) - determines what prompt/prompt_name the custom
+            debugger uses, e.g. "debug_stack_trace". Users can also define
+            their own custom prompt
+            (https://hdmamin.github.io/roboduck/custom_prompts/)
+            and pass in the file path here.
 
+    Examples
+    --------
     ```
     from roboduck import logging
 
     logger = logging.getLogger()
     ```
     """
     return DuckLogger(name=name, **kwargs)
```

### Comparing `roboduck-0.2.0/roboduck/magic.py` & `roboduck-0.3.0/roboduck/magic.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,24 +8,21 @@
 functionality.
 
 Quickstart
 ----------
 ```
 # cell 1
 from roboduck import magic
-```
 
-```
-# cell 2
 nums = [1, 2, 3]
 nums.add(4)
 ```
 
 ```
-# cell 3
+# cell 2
 %duck
 ```
 """
 
 from functools import partial
 from IPython import get_ipython
 from IPython.core.magic import line_magic, magics_class, Magics
@@ -118,14 +115,19 @@
             self.shell.debugger_cls = self.shell.InteractiveTB.debugger_cls = old_cls
         else:
             # Confine this import to this if clause rather than keeping a top
             # level import - importing this module overwrites sys.excepthook
             # which we don't necessarily want in most cases.
             # Note that this uses the `debug_stack_trace` prompt by default
             # whereas interactive mode uses `debug` by default.
+            # UPDATE: we could probably use excepthook for both cases
+            # (args.i = True or False) now that
+            # I added interactive support in the errors module. However,
+            # everything is working nicely now and I don't see a compelling
+            # reason to change things at the moment.
             from roboduck import errors
             kwargs = {'auto': True, 'color': 'green'}
             if args.prompt:
                 kwargs['prompt'] = args.prompt
             errors.excepthook(sys.last_type, sys.last_value,
                               sys.last_traceback, **kwargs)
             errors.disable()
```

### Comparing `roboduck-0.2.0/roboduck/prompts/chat/__template__.yaml` & `roboduck-0.3.0/roboduck/prompts/chat/__template__.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.2.0/roboduck/prompts/chat/debug.yaml` & `roboduck-0.3.0/roboduck/prompts/chat/debug.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.2.0/roboduck/prompts/chat/debug_full.yaml` & `roboduck-0.3.0/roboduck/prompts/chat/debug_full.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.2.0/roboduck/prompts/chat/debug_full_stack_trace.yaml` & `roboduck-0.3.0/roboduck/prompts/chat/debug_full_stack_trace.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.2.0/roboduck/prompts/chat/debug_stack_trace.yaml` & `roboduck-0.3.0/roboduck/prompts/chat/debug_stack_trace.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.2.0/roboduck/prompts/utils.py` & `roboduck-0.3.0/roboduck/prompts/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,27 +12,28 @@
 
 
 def available_templates(mode=''):
     """List names of prompts included in roboduck.
 
     Parameters
     ----------
-    mode: str
+    mode : str
         Type of prompt template to list available names for, e.g. "chat" or
         "completion". Concretely, the name of a subdir in roboduck.prompts.
         If empty, return a dict mapping mode -> set of names rather than just
         the set of names.
 
     Returns
     -------
-    dict[str, set[str]] or set[str]: If mode is an empty str, we return a dict
-    mapping keys (should be "chat" and "completion") to set of prompt name
-    strings, e.g. "debug" (notice file extension is excluded).
-    If a non-empty string is provided, we only return the set of strings for
-    the given mode, e.g. only the available chat prompts if mode='chat'.
+    dict[str, set[str]] or set[str]
+        If mode is an empty str, we return a dict mapping keys (should be
+        "chat" and "completion") to set of prompt name strings, e.g. "debug"
+        (notice file extension is excluded). If a non-empty string is provided,
+        we only return the set of strings for the given mode, e.g. only the
+        available chat prompts if mode='chat'.
     """
     def _prompt_names_in_dir(dir_):
         # Ignore files like __template__.yaml.
         return set(path.stem for path in dir_.iterdir()
                    if path.suffix == '.yaml'
                    and not path.stem.startswith('__'))
 
@@ -51,28 +52,29 @@
 
 def load_template(name, mode='chat'):
     """Load prompt template from the roboduck library or a user-provided yaml
     file.
 
     Parameters
     ----------
-    name: str or Path
+    name : str or Path
         Either the name of a prompt provided in the roboduck library, e.g.
         "debug", or the path to a yaml config file defining a custom prompt
         template.
-    mode: str
+    mode : str
         Type of prompt, currently either "chat" or "completion". As of March
         2023, we usually want to use "chat" because those models
         (gpt-3.5-turbo or gpt-4) are currently better for most tasks and,
         I believe, cheaper for a comparable model
         (e.g. gpt-3.5-turbo vs text-davinci-002).
 
     Returns
     -------
-    dict: Chat templates should have the following keys:
+    dict
+        Chat templates should have the following keys:
         "kwargs" (dict): used to instantiate a class like
         langchain.chat.ChatOpenAI. Mostly openai params but can also include
         'chat_model' for langchain. Note that unlike jabberwocky, we use the
         name max_tokens instead of max_length.
 
         "system" (str): system message (see openai chat model api docs).
         This should not contain user-specified fields.
```

### Comparing `roboduck-0.2.0/roboduck/shell.py` & `roboduck-0.3.0/roboduck/shell.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 
 class RoboDuckTerminalInteractiveShell(TerminalInteractiveShell):
     """TerminalInteractiveShell replacement class whose debugger_cls attribute
     is NOT read-only, thereby allowing our `duck` magic to overwrite it when
     necessary.
     """
 
-    debugger_cls = Pdb
+    debugger_cls = Pdb
```

### Comparing `roboduck-0.2.0/roboduck/utils.py` & `roboduck-0.3.0/roboduck/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,39 @@
-"""Utility functions used by other roboduck modules.
-"""
+"""Utility functions used by other roboduck modules."""
+
 from collections.abc import Iterable
 from colorama import Fore, Style
 import difflib
 import openai
+import os
 import pandas as pd
 from pathlib import Path
 import re
 import warnings
 import yaml
 
 
 def colored(text, color):
     """Add tags to color text and then reset color afterwards. Note that this
     does NOT actually print anything.
 
     Parameters
     ----------
-    text: str
+    text : str
         Text that should be colored.
-    color:
+    color : str
         Color name, e.g. "red". Must be available in the colorama lib. If None
         or empty str, just return the text unchanged.
 
     Returns
     -------
     str
+        Note that you need to print() the result for it to show up in the
+        desired color. Otherwise it will just have some unintelligible
+        characters appended and prepended.
     """
     if not color:
         return text
     color = getattr(Fore, color.upper())
     return f'{color}{text}{Style.RESET_ALL}'
 
 
@@ -44,24 +48,25 @@
     draw attention to the new bits.
 
     Adapted from this gist + variations in comments:
     https://gist.github.com/ines/04b47597eb9d011ade5e77a068389521
 
     Parameters
     ----------
-    old: str
+    old : str
         This is what `new` is compared to when identifying differences.
-    new: str
+    new : str
         Determines content of output str.
-    color: str
+    color : str
         Text color for new characters.
 
     Returns
     -------
-    str: Same content as `new` but color new parts in a different color.
+    str
+        Same content as `new` but color new parts in a different color.
     """
     res = []
     matcher = difflib.SequenceMatcher(None, old, new)
     for opcode, s1, e1, s2, e2 in matcher.get_opcodes():
         if opcode == 'delete':
             continue
         chunk = new[s2:e2]
@@ -73,33 +78,35 @@
 
 def type_annotated_dict_str(dict_, func=repr):
     """String representation (or repr) of a dict, where each line includes
     an inline comment showing the type of the value.
 
     Parameters
     ----------
-    dict_: dict
+    dict_ : dict
         The dict to represent.
-    func: function
+    func : function
         The function to apply to each key and value in the dict to get some
         kind of str representation. Note that it is applied to each key/value
-        as a whole, not to each item within that key/value. For example, notice
-        below how foo and cat are not in quotes but ('bar',) and ['x'] do
-        contain quotes.
-
-        >>> d = {'foo': 'cat', ('bar',): ['x']}
-        >>> type_annotated_dict_str(d, str)
-        {
-            foo: cat,   # type: str
-            ('bar',): ['x'],   # type: list
-        }
+        as a whole, not to each item within that key/value. See examples.
 
     Returns
-    --------
+    -------
     str
+
+    Examples
+    --------
+    Notice below how foo and cat are not in quotes but ('bar',) and ['x'] do
+    contain quotes.
+    >>> d = {'foo': 'cat', ('bar',): ['x']}
+    >>> type_annotated_dict_str(d, str)
+    {
+        foo: cat,   # type: str
+        ('bar',): ['x'],   # type: list
+    }
     """
     type_strs = [f'\n    {func(k)}: {func(v)},   # type: {type(v).__name__}'
                  for k, v in dict_.items()]
     return '{' + ''.join(type_strs) + '\n}'
 
 
 def truncated_repr(obj, max_len=79):
@@ -109,32 +116,33 @@
     giant data structure exists, e.g. list(range(1_000_000)). Our use
     case doesn't call for anything super precise so the max_len should be
     thought of as more of guide than an exact max. I think it's enforced but I
     didn't put a whole lot of thought or effort into confirming that.
 
     Parameters
     ----------
-    obj: any
-    max_len: int
+    obj : any
+    max_len : int
         Max number of characters for resulting repr. Think of this more as an
         estimate than a hard guarantee - precision isn't important in our use
         case. The result will likely be shorter than this because we want to
         truncate in a readable place, e.g. taking the repr of the first k items
         of a list instead of taking the repr of all items and then slicing off
         the end of the repr.
 
     Returns
     -------
-    str: Repr for obj, truncated to approximately max_len characters or fewer.
-    When possible, we insert ellipses into the repr to show that truncation
-    occurred. Technically there are some edge cases we don't handle (e.g. if
-    obj is a class with an insanely long name) but that's not a big deal, at
-    least at the moment. I can always revisit that later if necessary.
+    str
+        Repr for obj, truncated to approximately max_len characters or fewer.
+        When possible, we insert ellipses into the repr to show that truncation
+        occurred. Technically there are some edge cases we don't handle (e.g.
+        if obj is a class with an insanely long name) but that's not a big
+        deal, at least at the moment. I can always revisit that later if
+        necessary.
     """
-
     def qualname(obj):
         """Similar to type(obj).__qualname__() but that method doesn't always
         include the module(s). e.g. pandas Index has __qualname__ "Index" but
         this funnction returns "<pandas.core.indexes.base.Index>".
         """
         text = str(type(obj))
         names = re.search("<class '([a-zA-Z_.]*)'>", text).groups()
@@ -214,73 +222,109 @@
 def load_yaml(path, section=None):
     """Load a yaml file. Useful for loading prompts.
 
     Borrowed from jabberwocky.
 
     Parameters
     ----------
-    path: str or Path
-    section: str or None
+    path : str or Path
+    section : str or None
         I vaguely recall yaml files can define different subsections. This lets
         you return a specific one if you want. Usually leave as None which
         returns the whole contents.
 
     Returns
     -------
     dict
     """
     with open(path, 'r') as f:
-        data = yaml.load(f, Loader=yaml.FullLoader)
+        data = yaml.load(f, Loader=yaml.FullLoader) or {}
     return data.get(section, data)
 
 
+def update_yaml(path, delete_if_none=True, **kwargs):
+    """Update a yaml file with new values.
+
+    Parameters
+    ----------
+    path : str or Path
+        Path to yaml file to update. If it doesn't exist, it will be created.
+        Any necessary intermediate directories will be created too.
+    delete_if_none : bool
+        If True, any k-v pairs in kwargs where v is None will be treated as an
+        instruction to delete key k from the yaml file. If False, we will
+        actually set `{field}: None` in the yaml file.
+    kwargs : any
+        Key-value pairs to update the yaml file with.
+    """
+    path = Path(path).expanduser()
+    os.makedirs(path.parent, exist_ok=True)
+    try:
+        data = load_yaml(path)
+    except FileNotFoundError:
+        data = {}
+    for k, v in kwargs.items():
+        if v is None and delete_if_none:
+            data.pop(k, None)
+        else:
+            data[k] = v
+    with open(path, 'w') as f:
+        yaml.dump(data, f)
+
+
 def extract_code(text, join_multi=True, multi_prefix_template='\n\n# {i}\n'):
     """Extract code snippet from a GPT response (e.g. from our `debug` chat
     prompt. See `Examples` for expected format.
 
     Parameters
     ----------
-    text: str
-    join_multi: bool
+    text : str
+    join_multi : bool
         If multiple code snippets are found, we can either choose to join them
         into one string or return a list of strings. If the former, we prefix
         each snippet with `multi_prefix_template` to make it clearer where
         each new snippet starts.
-    multi_prefix_template: str
+    multi_prefix_template : str
         If join_multi=True and multiple code snippets are found, we prepend
         this to each code snippet before joining into a single string. It
         should accept a single parameter {i} which numbers each code snippet
         in the order they were found in `text` (1-indexed).
 
     Returns
     -------
-    str or list: code snippet from `text`. If we find multiple snippets, we
-    either join them into one big string (if join_multi is True) or return a
-    list of strings otherwise.
+    str or list
+        Code snippet from `text`. If we find multiple snippets, we either join
+        them into one big string (if join_multi is True) or return a
+        list of strings otherwise.
 
     Examples
     --------
+    ```plaintext
     text = '''Appending to a tuple is not allowed because tuples are immutable.
     However, in this code snippet, the tuple b contains two lists, and lists
     are mutable. Therefore, appending to b[1] (which is a list) does not raise
     an error. To fix this, you can either change b[1] to a tuple or create a
     new tuple that contains the original elements of b and the new list.
 
-    ```
+    ```python
     # Corrected code snippet
     a = 3
     b = ([0, 1], [2, 3])
     b = (b[0], b[1] + [a])
     ```'''
+
     print(extract_code(text))
 
-    # Corrected code snippet
+    # Extracted code snippet
+    '''
     a = 3
     b = ([0, 1], [2, 3])
     b = (b[0], b[1] + [a])
+    '''
+    ```
     """
     chunks = re.findall("(?s)```(?:python)?\n(.*?)\n```", text)
     if not join_multi:
         return chunks
     if len(chunks) > 1:
         chunks = [multi_prefix_template.format(i=i) + chunk
                   for i, chunk in enumerate(chunks, 1)]
@@ -302,15 +346,15 @@
     if you wrote a prompt that asked gpt to return valid json, you could
     potentially use json.loads() as your drop-in replacement (ignoring
     validation/error handling, which you might prefer to handle via a langchain
     chain anyway).
 
     Parameters
     ----------
-    text: str
+    text : str
         GPT completion. This should contain both a natural language explanation
         and code.
 
     Returns
     -------
     dict[str]
     """
@@ -327,21 +371,25 @@
 
 def available_models():
     """Show user available values for model_name parameter in debug.DuckDB
     class/ debug.duck function/errors.enable function etc.
 
     Returns
     -------
-    dict[str, list[str]]: Maps provider name (e.g. 'openai') to list of valid
-    model_name values. Provider name should correspond to a langchain or
-    roboduck class named like ChatOpenai (i.e. Chat{provider.title()}).
+    dict[str, list[str]]
+        Maps provider name (e.g. 'openai') to list of valid
+        model_name values. Provider name should correspond to a langchain or
+        roboduck class named like ChatOpenai (i.e. Chat{provider.title()}).
+        Eventually would like to support other providers like anthropic but
+        never got off API waitlist.
     """
+    # Weirdly, env var is set and available but openai can't seem to find it
+    # unless we explicitly set it here.
+    openai.api_key = os.environ.get('OPENAI_API_KEY')
     res = {}
 
     # This logic may not always hold but as of April 2023, this returns
     # openai's available chat models.
     openai_res = openai.Model.list()
     res['openai'] = [row['id'] for row in openai_res['data']
                      if row['id'].startswith('gpt')]
-
-    # TODO: add anthropic/cohere/other?
-    return res
+    return res
```

### Comparing `roboduck-0.2.0/roboduck.egg-info/SOURCES.txt` & `roboduck-0.3.0/roboduck.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 roboduck/__init__.py
+roboduck/config.py
 roboduck/debug.py
 roboduck/decorators.py
 roboduck/errors.py
 roboduck/ipy_utils.py
 roboduck/logging.py
 roboduck/magic.py
 roboduck/shell.py
 roboduck/utils.py
 roboduck.egg-info/PKG-INFO
 roboduck.egg-info/SOURCES.txt
 roboduck.egg-info/dependency_links.txt
 roboduck.egg-info/entry_points.txt
 roboduck.egg-info/requires.txt
 roboduck.egg-info/top_level.txt
+roboduck/cli/__init__.py
 roboduck/cli/cli.py
 roboduck/langchain/__init__.py
 roboduck/langchain/callbacks.py
 roboduck/langchain/chat.py
 roboduck/langchain/utils.py
 roboduck/prompts/__init__.py
 roboduck/prompts/utils.py
```

### Comparing `roboduck-0.2.0/setup.py` & `roboduck-0.3.0/setup.py`

 * *Files identical despite different names*

