# Comparing `tmp/chatgpt4-cli-1.5.6.tar.gz` & `tmp/chatgpt4-cli-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt4-cli-1.5.6.tar", last modified: Thu May  4 10:36:23 2023, max compression
+gzip compressed data, was "chatgpt4-cli-1.5.7.tar", last modified: Wed May 24 10:10:20 2023, max compression
```

## Comparing `chatgpt4-cli-1.5.6.tar` & `chatgpt4-cli-1.5.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:36:23.391187 chatgpt4-cli-1.5.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:36:23.387186 chatgpt4-cli-1.5.6/GPTCLI/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-04 10:36:00.000000 chatgpt4-cli-1.5.6/GPTCLI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-04 10:36:00.000000 chatgpt4-cli-1.5.6/GPTCLI/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-04 10:36:00.000000 chatgpt4-cli-1.5.6/GPTCLI/addons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-04 10:36:00.000000 chatgpt4-cli-1.5.6/GPTCLI/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-05-04 10:36:00.000000 chatgpt4-cli-1.5.6/GPTCLI/emage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32396 2023-05-04 10:36:00.000000 chatgpt4-cli-1.5.6/GPTCLI/gptcli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-05-04 10:36:00.000000 chatgpt4-cli-1.5.6/GPTCLI/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-05-04 10:36:00.000000 chatgpt4-cli-1.5.6/GPTCLI/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-04 10:36:00.000000 chatgpt4-cli-1.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-05-04 10:36:23.391187 chatgpt4-cli-1.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14274 2023-05-04 10:36:00.000000 chatgpt4-cli-1.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:36:23.391187 chatgpt4-cli-1.5.6/chatgpt4_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-05-04 10:36:23.000000 chatgpt4-cli-1.5.6/chatgpt4_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-04 10:36:23.000000 chatgpt4-cli-1.5.6/chatgpt4_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 10:36:23.000000 chatgpt4-cli-1.5.6/chatgpt4_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-04 10:36:23.000000 chatgpt4-cli-1.5.6/chatgpt4_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-04 10:36:23.000000 chatgpt4-cli-1.5.6/chatgpt4_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 10:36:23.000000 chatgpt4-cli-1.5.6/chatgpt4_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 10:36:23.391187 chatgpt4-cli-1.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-04 10:36:00.000000 chatgpt4-cli-1.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:10:20.186661 chatgpt4-cli-1.5.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:10:20.186661 chatgpt4-cli-1.5.7/GPTCLI/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-24 10:09:54.000000 chatgpt4-cli-1.5.7/GPTCLI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-24 10:09:54.000000 chatgpt4-cli-1.5.7/GPTCLI/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-24 10:09:54.000000 chatgpt4-cli-1.5.7/GPTCLI/addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-24 10:09:54.000000 chatgpt4-cli-1.5.7/GPTCLI/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-05-24 10:09:54.000000 chatgpt4-cli-1.5.7/GPTCLI/emage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32364 2023-05-24 10:09:54.000000 chatgpt4-cli-1.5.7/GPTCLI/gptcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-05-24 10:09:54.000000 chatgpt4-cli-1.5.7/GPTCLI/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-05-24 10:09:54.000000 chatgpt4-cli-1.5.7/GPTCLI/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-24 10:09:54.000000 chatgpt4-cli-1.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-05-24 10:10:20.186661 chatgpt4-cli-1.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14252 2023-05-24 10:09:54.000000 chatgpt4-cli-1.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:10:20.186661 chatgpt4-cli-1.5.7/chatgpt4_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-05-24 10:10:20.000000 chatgpt4-cli-1.5.7/chatgpt4_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-24 10:10:20.000000 chatgpt4-cli-1.5.7/chatgpt4_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 10:10:20.000000 chatgpt4-cli-1.5.7/chatgpt4_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-24 10:10:20.000000 chatgpt4-cli-1.5.7/chatgpt4_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-24 10:10:20.000000 chatgpt4-cli-1.5.7/chatgpt4_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 10:10:20.000000 chatgpt4-cli-1.5.7/chatgpt4_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 10:10:20.190662 chatgpt4-cli-1.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-24 10:09:54.000000 chatgpt4-cli-1.5.7/setup.py
```

### Comparing `chatgpt4-cli-1.5.6/GPTCLI/__init__.py` & `chatgpt4-cli-1.5.7/GPTCLI/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.5.6"
+__version__ = "1.5.7"
 __author__ = "Smartwa Caleb"
 __repo__ = "https://github.com/Simatwa/gpt-cli"
 __info__ = "Interact with ChatGPT and Bard at the terminal."
 
 import logging
 
 logging.basicConfig(
```

### Comparing `chatgpt4-cli-1.5.6/GPTCLI/addons.py` & `chatgpt4-cli-1.5.7/GPTCLI/addons.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.6/GPTCLI/bard.py` & `chatgpt4-cli-1.5.7/GPTCLI/bard.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.6/GPTCLI/emage.py` & `chatgpt4-cli-1.5.7/GPTCLI/emage.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.6/GPTCLI/gptcli.py` & `chatgpt4-cli-1.5.7/GPTCLI/gptcli.py`

 * *Files 0% similar despite different names*

```diff
@@ -858,15 +858,15 @@
             self.bard.reset()
             chat_gpt = 'Bard'
         else:
             if gpt4:
                 chatbot.reset(system_prompt=args.system_prompt)
             else:
                 chatbot.reset()
-            chat_gpt = 'Bard'
+            chat_gpt = 'GPT'
         logging.info(f'Chat reset successfully - {chat_gpt}')
         self.do__prompt(self.prompt_disp)
 
     def do__help(self, line):
         from .helper import help
 
         rich_print(
@@ -991,13 +991,12 @@
                 run.default(prompt)
         run.cmdloop()
     except (KeyboardInterrupt, EOFError):
         progress.querying = False
         exit(logging.info("Stopping program"))
     except Exception as e:
         progress.querying = False
-        # logging.exception(e)
         logging.error(getExc(e))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `chatgpt4-cli-1.5.6/GPTCLI/helper.py` & `chatgpt4-cli-1.5.7/GPTCLI/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,18 +67,18 @@
 12. `gpt4` : Specifies to use ChatGPT in case `--bard` was made default
     e.g *gpt4 How do you make?*
 
 13. `_help` : Show this help info
 
 * You can further specify the GPT to be used by appending `--gpt4` or `--bard` in the prompt.
 
-* Use **_botchat** to let the 2 GPTs chat to each other
+* Use `_botchat` to let the 2 GPTs chat to each other
 
 * Use double `./` (fullstop and foward slash) to interact with system commands
       e.g *./ifconfig*
       
 * Use `{{f.text-filename}}` to issue prompt contained in  the 'text-filename'
 
 * Use `CTRL+C` to cancel a request 
 
-* **_exit** or `CTRL+C` or `CTRL+Z` : Quits the program.
+* `_exit` or `CTRL+C` or `CTRL+Z` : Quits the program.
         """
```

### Comparing `chatgpt4-cli-1.5.6/GPTCLI/image.py` & `chatgpt4-cli-1.5.7/GPTCLI/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
             self.args.prompt = " ".join(self.args.prompt)
         self.image_buff = self.image_saver(self.args, [])
 
     def get_args(self, args):
         resolutions = ["256x256", "512x512", "1024x1024"]
         dir = path.join(path.expanduser("~"), "Downloads/GPT")
         parser = argparse.ArgumentParser(
-            description="Text-to-Image Converter - ChatGPT"
+            description="Text-to-Image Converter - ChatGPT",
+            exit_on_error=False,
         )
         parser.add_argument("prompt", help="Description of the image", nargs="*")
         parser.add_argument(
             "-f", "--file", help="Path to text-file containing the description"
         )
         parser.add_argument(
             "-n",
```

### Comparing `chatgpt4-cli-1.5.6/LICENSE` & `chatgpt4-cli-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.6/PKG-INFO` & `chatgpt4-cli-1.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt4-cli
-Version: 1.5.6
+Version: 1.5.7
 Summary: Interact with ChatGPT and Bard at the terminal.
 Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.6&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.7&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
@@ -80,17 +80,17 @@
  ```
 
 2. Cloning locally and install
 
 ```sh
 git clone https://github.com/Simatwa/gpt-cli.git
 cd gpt-cli
-sudo python3 setup.py install
+pip install .
  #or
-python3 setup.py install
+sudo pip install .
 ```
 
 ## Usage 
 
 - Make OPENAI_API_KEY an environment variable.
 
 `$ export OPENAI_API_KEY=<openai-api-key>`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.6 Summary: Interact with
+Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.7 Summary: Interact with
 ChatGPT and Bard at the terminal. Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb License: MIT Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/
 issues/new Classifier: License :: OSI Approved :: MIT License Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: License :: Free For Home
 Use Classifier: Topic :: Home Automation Classifier: Intended Audience ::
@@ -26,32 +26,32 @@
 customizable Commandline Interface. - Interact with system commands on the fly.
 ### Prerequisites - [x] [OPENAI_API_KEY](https://platform.openai.com/account/
 api-keys) - [x] [Bard Cookies](https://bard.google.com) - [x] [Bing cookies]
 (https://bing.com) - *optional* ## Installation Either of the following ways
 will get you ready. 1. Using pip - From pypi ```sh sudo pip install chatgpt4-
 cli ``` - Installing from source ```sh sudo pip install git+https://github.com/
 Simatwa/gpt-cli.git ``` 2. Cloning locally and install ```sh git clone https://
-github.com/Simatwa/gpt-cli.git cd gpt-cli sudo python3 setup.py install #or
-python3 setup.py install ``` ## Usage - Make OPENAI_API_KEY an environment
-variable. `$ export OPENAI_API_KEY=` After that you can launch the script with
-or without a prompt > For instance : ```sh #Without a prompt $ gpt-cli # With a
-prompt $ gpt-cli Write a conversation between Sun and Pluto.` ``` - Parsing
-OPENAI_API_KEY as one of the arguments Run `$ gpt-cli -k  ` at the terminal. >
-For instance : ```sh $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB
-vulnerability using NMAP? ``` The [awesome-chatgpt-prompts](https://github.com/
-f/awesome-chatgpt-prompts) can be parsed to the script through the following
-ways: - Specifying the role - (*case-sensitive*) e.g `$ gpt-cli UX/UI
-Developer` - Specifying the index of the prompt: e.g `$ gpt-cli 29` Run `$ gpt-
-cli --dump show` to view the act,prompt and their **indexes** You can as well
-generate images using EdgeGPT (DALL-E) or ChatGPT independent of `gpt-cli`,
-uninteractively at the terminal: 1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file
-``` - Visit [EdgeGPT](https://github.com/acheong08/EdgeGPT#requirements) to
-learn more on how to get the cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY
-environment variable $ gpt-cli-image  ``` For more info run `$gpt-cli-image -h`
-or `$gpt-cli-emage -h`. ## Highlight
+github.com/Simatwa/gpt-cli.git cd gpt-cli pip install . #or sudo pip install .
+``` ## Usage - Make OPENAI_API_KEY an environment variable. `$ export
+OPENAI_API_KEY=` After that you can launch the script with or without a prompt
+> For instance : ```sh #Without a prompt $ gpt-cli # With a prompt $ gpt-cli
+Write a conversation between Sun and Pluto.` ``` - Parsing OPENAI_API_KEY as
+one of the arguments Run `$ gpt-cli -k  ` at the terminal. > For instance :
+```sh $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB vulnerability using
+NMAP? ``` The [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-
+prompts) can be parsed to the script through the following ways: - Specifying
+the role - (*case-sensitive*) e.g `$ gpt-cli UX/UI Developer` - Specifying the
+index of the prompt: e.g `$ gpt-cli 29` Run `$ gpt-cli --dump show` to view the
+act,prompt and their **indexes** You can as well generate images using EdgeGPT
+(DALL-E) or ChatGPT independent of `gpt-cli`, uninteractively at the terminal:
+1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file   ``` - Visit [EdgeGPT](https://
+github.com/acheong08/EdgeGPT#requirements) to learn more on how to get the
+cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY environment variable $ gpt-cli-
+image  ``` For more info run `$gpt-cli-image -h` or `$gpt-cli-emage -h`. ##
+Highlight
 No. Command           Action
 0   ./{command}       Run command against system
 1   img               Generate image ChatGPT based on prompt
 2   emg               Generate image with EdgeGPT based on prompt
 3   txt2img           Generate image based on GPT description
 4   _font_color       Modify font-color
 5   _background_color Modify background_color
```

### Comparing `chatgpt4-cli-1.5.6/README.md` & `chatgpt4-cli-1.5.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.6&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.7&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
@@ -53,17 +53,17 @@
  ```
 
 2. Cloning locally and install
 
 ```sh
 git clone https://github.com/Simatwa/gpt-cli.git
 cd gpt-cli
-sudo python3 setup.py install
+pip install .
  #or
-python3 setup.py install
+sudo pip install .
 ```
 
 ## Usage 
 
 - Make OPENAI_API_KEY an environment variable.
 
 `$ export OPENAI_API_KEY=<openai-api-key>`
```

#### html2text {}

```diff
@@ -12,32 +12,32 @@
 customizable Commandline Interface. - Interact with system commands on the fly.
 ### Prerequisites - [x] [OPENAI_API_KEY](https://platform.openai.com/account/
 api-keys) - [x] [Bard Cookies](https://bard.google.com) - [x] [Bing cookies]
 (https://bing.com) - *optional* ## Installation Either of the following ways
 will get you ready. 1. Using pip - From pypi ```sh sudo pip install chatgpt4-
 cli ``` - Installing from source ```sh sudo pip install git+https://github.com/
 Simatwa/gpt-cli.git ``` 2. Cloning locally and install ```sh git clone https://
-github.com/Simatwa/gpt-cli.git cd gpt-cli sudo python3 setup.py install #or
-python3 setup.py install ``` ## Usage - Make OPENAI_API_KEY an environment
-variable. `$ export OPENAI_API_KEY=` After that you can launch the script with
-or without a prompt > For instance : ```sh #Without a prompt $ gpt-cli # With a
-prompt $ gpt-cli Write a conversation between Sun and Pluto.` ``` - Parsing
-OPENAI_API_KEY as one of the arguments Run `$ gpt-cli -k  ` at the terminal. >
-For instance : ```sh $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB
-vulnerability using NMAP? ``` The [awesome-chatgpt-prompts](https://github.com/
-f/awesome-chatgpt-prompts) can be parsed to the script through the following
-ways: - Specifying the role - (*case-sensitive*) e.g `$ gpt-cli UX/UI
-Developer` - Specifying the index of the prompt: e.g `$ gpt-cli 29` Run `$ gpt-
-cli --dump show` to view the act,prompt and their **indexes** You can as well
-generate images using EdgeGPT (DALL-E) or ChatGPT independent of `gpt-cli`,
-uninteractively at the terminal: 1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file
-``` - Visit [EdgeGPT](https://github.com/acheong08/EdgeGPT#requirements) to
-learn more on how to get the cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY
-environment variable $ gpt-cli-image  ``` For more info run `$gpt-cli-image -h`
-or `$gpt-cli-emage -h`. ## Highlight
+github.com/Simatwa/gpt-cli.git cd gpt-cli pip install . #or sudo pip install .
+``` ## Usage - Make OPENAI_API_KEY an environment variable. `$ export
+OPENAI_API_KEY=` After that you can launch the script with or without a prompt
+> For instance : ```sh #Without a prompt $ gpt-cli # With a prompt $ gpt-cli
+Write a conversation between Sun and Pluto.` ``` - Parsing OPENAI_API_KEY as
+one of the arguments Run `$ gpt-cli -k  ` at the terminal. > For instance :
+```sh $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB vulnerability using
+NMAP? ``` The [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-
+prompts) can be parsed to the script through the following ways: - Specifying
+the role - (*case-sensitive*) e.g `$ gpt-cli UX/UI Developer` - Specifying the
+index of the prompt: e.g `$ gpt-cli 29` Run `$ gpt-cli --dump show` to view the
+act,prompt and their **indexes** You can as well generate images using EdgeGPT
+(DALL-E) or ChatGPT independent of `gpt-cli`, uninteractively at the terminal:
+1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file   ``` - Visit [EdgeGPT](https://
+github.com/acheong08/EdgeGPT#requirements) to learn more on how to get the
+cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY environment variable $ gpt-cli-
+image  ``` For more info run `$gpt-cli-image -h` or `$gpt-cli-emage -h`. ##
+Highlight
 No. Command           Action
 0   ./{command}       Run command against system
 1   img               Generate image ChatGPT based on prompt
 2   emg               Generate image with EdgeGPT based on prompt
 3   txt2img           Generate image based on GPT description
 4   _font_color       Modify font-color
 5   _background_color Modify background_color
```

### Comparing `chatgpt4-cli-1.5.6/chatgpt4_cli.egg-info/PKG-INFO` & `chatgpt4-cli-1.5.7/chatgpt4_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt4-cli
-Version: 1.5.6
+Version: 1.5.7
 Summary: Interact with ChatGPT and Bard at the terminal.
 Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.6&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.7&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
@@ -80,17 +80,17 @@
  ```
 
 2. Cloning locally and install
 
 ```sh
 git clone https://github.com/Simatwa/gpt-cli.git
 cd gpt-cli
-sudo python3 setup.py install
+pip install .
  #or
-python3 setup.py install
+sudo pip install .
 ```
 
 ## Usage 
 
 - Make OPENAI_API_KEY an environment variable.
 
 `$ export OPENAI_API_KEY=<openai-api-key>`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.6 Summary: Interact with
+Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.7 Summary: Interact with
 ChatGPT and Bard at the terminal. Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb License: MIT Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/
 issues/new Classifier: License :: OSI Approved :: MIT License Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: License :: Free For Home
 Use Classifier: Topic :: Home Automation Classifier: Intended Audience ::
@@ -26,32 +26,32 @@
 customizable Commandline Interface. - Interact with system commands on the fly.
 ### Prerequisites - [x] [OPENAI_API_KEY](https://platform.openai.com/account/
 api-keys) - [x] [Bard Cookies](https://bard.google.com) - [x] [Bing cookies]
 (https://bing.com) - *optional* ## Installation Either of the following ways
 will get you ready. 1. Using pip - From pypi ```sh sudo pip install chatgpt4-
 cli ``` - Installing from source ```sh sudo pip install git+https://github.com/
 Simatwa/gpt-cli.git ``` 2. Cloning locally and install ```sh git clone https://
-github.com/Simatwa/gpt-cli.git cd gpt-cli sudo python3 setup.py install #or
-python3 setup.py install ``` ## Usage - Make OPENAI_API_KEY an environment
-variable. `$ export OPENAI_API_KEY=` After that you can launch the script with
-or without a prompt > For instance : ```sh #Without a prompt $ gpt-cli # With a
-prompt $ gpt-cli Write a conversation between Sun and Pluto.` ``` - Parsing
-OPENAI_API_KEY as one of the arguments Run `$ gpt-cli -k  ` at the terminal. >
-For instance : ```sh $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB
-vulnerability using NMAP? ``` The [awesome-chatgpt-prompts](https://github.com/
-f/awesome-chatgpt-prompts) can be parsed to the script through the following
-ways: - Specifying the role - (*case-sensitive*) e.g `$ gpt-cli UX/UI
-Developer` - Specifying the index of the prompt: e.g `$ gpt-cli 29` Run `$ gpt-
-cli --dump show` to view the act,prompt and their **indexes** You can as well
-generate images using EdgeGPT (DALL-E) or ChatGPT independent of `gpt-cli`,
-uninteractively at the terminal: 1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file
-``` - Visit [EdgeGPT](https://github.com/acheong08/EdgeGPT#requirements) to
-learn more on how to get the cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY
-environment variable $ gpt-cli-image  ``` For more info run `$gpt-cli-image -h`
-or `$gpt-cli-emage -h`. ## Highlight
+github.com/Simatwa/gpt-cli.git cd gpt-cli pip install . #or sudo pip install .
+``` ## Usage - Make OPENAI_API_KEY an environment variable. `$ export
+OPENAI_API_KEY=` After that you can launch the script with or without a prompt
+> For instance : ```sh #Without a prompt $ gpt-cli # With a prompt $ gpt-cli
+Write a conversation between Sun and Pluto.` ``` - Parsing OPENAI_API_KEY as
+one of the arguments Run `$ gpt-cli -k  ` at the terminal. > For instance :
+```sh $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB vulnerability using
+NMAP? ``` The [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-
+prompts) can be parsed to the script through the following ways: - Specifying
+the role - (*case-sensitive*) e.g `$ gpt-cli UX/UI Developer` - Specifying the
+index of the prompt: e.g `$ gpt-cli 29` Run `$ gpt-cli --dump show` to view the
+act,prompt and their **indexes** You can as well generate images using EdgeGPT
+(DALL-E) or ChatGPT independent of `gpt-cli`, uninteractively at the terminal:
+1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file   ``` - Visit [EdgeGPT](https://
+github.com/acheong08/EdgeGPT#requirements) to learn more on how to get the
+cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY environment variable $ gpt-cli-
+image  ``` For more info run `$gpt-cli-image -h` or `$gpt-cli-emage -h`. ##
+Highlight
 No. Command           Action
 0   ./{command}       Run command against system
 1   img               Generate image ChatGPT based on prompt
 2   emg               Generate image with EdgeGPT based on prompt
 3   txt2img           Generate image based on GPT description
 4   _font_color       Modify font-color
 5   _background_color Modify background_color
```

### Comparing `chatgpt4-cli-1.5.6/setup.py` & `chatgpt4-cli-1.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         "numpy>=1.23.4",
         "colorama>=0.4.6",
         "openai>=0.26.4",
         "revChatGPT==4.0.6",
         "appdirs>=1.4.4",
         "requests>=2.28.2",
         "tabulate>=0.9.0",
-        "GoogleBard==1.0.0",
+        "GoogleBard==1.0.3",
         "fpdf==1.7.2",
     ],
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Development Status :: 4 - Beta",
```

