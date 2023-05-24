# Comparing `tmp/oobabot-0.1.7.tar.gz` & `tmp/oobabot-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oobabot-0.1.7.tar", max compression
+gzip compressed data, was "oobabot-0.1.8.tar", max compression
```

## Comparing `oobabot-0.1.7.tar` & `oobabot-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1067 2023-05-03 00:11:59.534663 oobabot-0.1.7/LICENSE
--rw-r--r--   0        0        0    14228 2023-05-17 14:39:21.124910 oobabot-0.1.7/README.md
--rw-r--r--   0        0        0     1240 2023-05-17 14:40:10.716786 oobabot-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      104 2023-05-17 14:40:16.710666 oobabot-0.1.7/src/oobabot/__init__.py
--rw-r--r--   0        0        0       93 2023-05-14 14:34:31.204759 oobabot-0.1.7/src/oobabot/__main__.py
--rw-r--r--   0        0        0     6141 2023-05-16 18:04:52.618218 oobabot-0.1.7/src/oobabot/bot_commands.py
--rw-r--r--   0        0        0     7132 2023-05-16 18:45:57.071008 oobabot-0.1.7/src/oobabot/decide_to_respond.py
--rw-r--r--   0        0        0    17606 2023-05-17 13:55:33.467250 oobabot-0.1.7/src/oobabot/discord_bot.py
--rw-r--r--   0        0        0     2227 2023-05-17 06:48:28.290145 oobabot-0.1.7/src/oobabot/discord_utils.py
--rw-r--r--   0        0        0     1557 2023-05-14 14:34:31.203723 oobabot-0.1.7/src/oobabot/fancy_logger.py
--rw-r--r--   0        0        0     2602 2023-05-14 14:34:31.197932 oobabot-0.1.7/src/oobabot/http_client.py
--rw-r--r--   0        0        0    10740 2023-05-16 12:52:44.722682 oobabot-0.1.7/src/oobabot/image_generator.py
--rw-r--r--   0        0        0     7927 2023-05-17 06:48:28.291422 oobabot-0.1.7/src/oobabot/ooba_client.py
--rwxr-xr-x   0        0        0     7376 2023-05-17 07:24:58.226500 oobabot-0.1.7/src/oobabot/oobabot.py
--rw-r--r--   0        0        0     9557 2023-05-17 15:18:05.783839 oobabot-0.1.7/src/oobabot/overengineered_settings_parser.py
--rw-r--r--   0        0        0     8197 2023-05-17 06:48:28.292148 oobabot-0.1.7/src/oobabot/prompt_generator.py
--rw-r--r--   0        0        0     2893 2023-05-14 14:34:31.197478 oobabot-0.1.7/src/oobabot/repetition_tracker.py
--rw-r--r--   0        0        0     6583 2023-05-14 14:34:31.198417 oobabot-0.1.7/src/oobabot/response_stats.py
--rw-r--r--   0        0        0     9430 2023-05-17 13:29:23.484593 oobabot-0.1.7/src/oobabot/sd_client.py
--rw-r--r--   0        0        0    24621 2023-05-17 15:18:56.717729 oobabot-0.1.7/src/oobabot/settings.py
--rw-r--r--   0        0        0     8910 2023-05-17 13:25:50.645781 oobabot-0.1.7/src/oobabot/templates.py
--rw-r--r--   0        0        0     1153 2023-05-17 06:48:28.293012 oobabot-0.1.7/src/oobabot/types.py
--rw-r--r--   0        0        0    15065 1970-01-01 00:00:00.000000 oobabot-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-03 00:11:59.534663 oobabot-0.1.8/LICENSE
+-rw-r--r--   0        0        0    15491 2023-05-24 01:57:57.638210 oobabot-0.1.8/README.md
+-rw-r--r--   0        0        0     1222 2023-05-22 15:16:17.945097 oobabot-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-05-19 20:38:41.345994 oobabot-0.1.8/src/oobabot/__init__.py
+-rw-r--r--   0        0        0      121 2023-05-18 18:14:55.125650 oobabot-0.1.8/src/oobabot/__main__.py
+-rw-r--r--   0        0        0     6457 2023-05-22 15:03:15.709636 oobabot-0.1.8/src/oobabot/bot_commands.py
+-rw-r--r--   0        0        0     6873 2023-05-22 15:03:19.938322 oobabot-0.1.8/src/oobabot/decide_to_respond.py
+-rw-r--r--   0        0        0    29147 2023-05-22 15:12:32.817542 oobabot-0.1.8/src/oobabot/discord_bot.py
+-rw-r--r--   0        0        0     6906 2023-05-22 13:58:48.609231 oobabot-0.1.8/src/oobabot/discord_utils.py
+-rw-r--r--   0        0        0     8405 2023-05-23 05:48:45.666973 oobabot-0.1.8/src/oobabot/fancy_logger.py
+-rw-r--r--   0        0        0     3106 2023-05-18 18:20:12.856052 oobabot-0.1.8/src/oobabot/http_client.py
+-rw-r--r--   0        0        0    13406 2023-05-22 14:46:56.313942 oobabot-0.1.8/src/oobabot/image_generator.py
+-rw-r--r--   0        0        0    10159 2023-05-23 05:48:45.668106 oobabot-0.1.8/src/oobabot/ooba_client.py
+-rwxr-xr-x   0        0        0    13626 2023-05-24 00:48:55.123541 oobabot-0.1.8/src/oobabot/oobabot.py
+-rw-r--r--   0        0        0    12812 2023-05-23 05:48:45.669521 oobabot-0.1.8/src/oobabot/overengineered_settings_parser.py
+-rw-r--r--   0        0        0     4353 2023-05-21 10:37:28.483174 oobabot-0.1.8/src/oobabot/persona.py
+-rw-r--r--   0        0        0     7774 2023-05-23 05:48:45.670867 oobabot-0.1.8/src/oobabot/prompt_generator.py
+-rw-r--r--   0        0        0     3243 2023-05-18 18:22:10.143873 oobabot-0.1.8/src/oobabot/repetition_tracker.py
+-rw-r--r--   0        0        0     6736 2023-05-22 14:11:01.702461 oobabot-0.1.8/src/oobabot/response_stats.py
+-rw-r--r--   0        0        0     9758 2023-05-21 10:37:28.483908 oobabot-0.1.8/src/oobabot/sd_client.py
+-rw-r--r--   0        0        0    30229 2023-05-23 05:48:45.672008 oobabot-0.1.8/src/oobabot/settings.py
+-rw-r--r--   0        0        0    10906 2023-05-19 17:11:29.625366 oobabot-0.1.8/src/oobabot/templates.py
+-rw-r--r--   0        0        0     1481 2023-05-18 17:46:10.237360 oobabot-0.1.8/src/oobabot/types.py
+-rw-r--r--   0        0        0    16328 1970-01-01 00:00:00.000000 oobabot-0.1.8/PKG-INFO
```

### Comparing `oobabot-0.1.7/LICENSE` & `oobabot-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.7/README.md` & `oobabot-0.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -69,86 +69,102 @@
 
 ~: oobabot --base-url ws://oobabooga-hostname:5005/ --ai-name YourBotsName --persona "You are a cat named YourBotsName"
 ```
 
 You should now be able to run oobabot from wherever pip installed it.
 
 ```none
-usage: oobabot [-h] [-c CONFIG] [--generate-config] [--ai-name AI_NAME] [--persona PERSONA]
-               [--wakewords [WAKEWORDS ...]] [--discord-token DISCORD_TOKEN]
-               [--dont-split-responses] [--history-lines HISTORY_LINES] [--ignore-dms]
-               [--reply-in-thread] [--stream-responses] [--base-url BASE_URL]
-               [--log-all-the-things] [--image-words [IMAGE_WORDS ...]]
+  ³ oobabot  ~/oobabot        oobabot --help         383ms  Tue May 23 18:56:42 2023
+usage: oobabot [-h] [-c CONFIG] [--generate-config] [--invite-url] [--ai-name AI_NAME]
+               [--persona PERSONA] [--wakewords [WAKEWORDS ...]]
+               [--discord-token DISCORD_TOKEN] [--dont-split-responses]
+               [--history-lines HISTORY_LINES] [--ignore-dms] [--reply-in-thread]
+               [--stream-responses] [--base-url BASE_URL] [--log-all-the-things]
+               [--message-regex MESSAGE_REGEX] [--image-words [IMAGE_WORDS ...]]
                [--stable-diffusion-url STABLE_DIFFUSION_URL]
-               [--extra-prompt-text EXTRA_PROMPT_TEXT]
+               [--extra-prompt-text EXTRA_PROMPT_TEXT] [--use-ai-generated-keywords]
 
-oobabot v0.1.7: Discord bot for oobabooga's text-generation-webui
+oobabot v0.1.8: Discord bot for oobabooga's text-generation-webui
 
 General Settings:
 
   -h, --help
   -c CONFIG, --config CONFIG
                         Path to a config file to read settings from. Command line settings
                         will override settings in this file. (default: config.yml)
   --generate-config     If set, oobabot will print its configuration as a .yml file, then
                         exit. Any command-line settings also passed will be reflected in
                         this file. (default: False)
+  --invite-url          Print a URL which can be used to invite the bot to a Discord
+                        server. Requires that the Discord token is set. (default: False)
 
 Persona:
 
   --ai-name AI_NAME     Name the AI will use to refer to itself (default: oobabot)
   --persona PERSONA     This prefix will be added in front of every user-supplied request.
                         This is useful for setting up a 'character' for the bot to play.
                         Alternatively, this can be set with the OOBABOT_PERSONA environment
                         variable. (default: )
   --wakewords [WAKEWORDS ...]
                         One or more words that the bot will listen for. The bot will listen
-                        in all discord channels can access for one of these words to be
+                        in all discord channels it can access for one of these words to be
                         mentioned, then reply to any messages it sees with a matching word.
                         The bot will always reply to @-mentions and direct messages, even
                         if no wakewords are supplied. (default: ['oobabot'])
 
 Discord:
 
   --discord-token DISCORD_TOKEN
                         Token to log into Discord with. For security purposes it's strongly
                         recommended that you set this via the DISCORD_TOKEN environment
                         variable instead, if possible. (default: )
   --dont-split-responses
                         Post the entire response as a single message, rather than splitting
-                        it into seperate messages by sentence. (default: False)
+                        it into separate messages by sentence. (default: False)
   --history-lines HISTORY_LINES
                         Number of lines of chat history the AI will see when generating a
                         response. (default: 7)
   --ignore-dms          If set, the bot will not respond to direct messages. (default:
                         False)
   --reply-in-thread     If set, the bot will generate a thread to respond in if it is not
                         already in one. (default: False)
-  --stream-responses    Stream responses into a single message as they are generated.
-                        (default: False)
+  --stream-responses    FEATURE PREVIEW: Stream responses into a single message as they are
+                        generated. Note: may be janky (default: False)
 
 Oobabooga:
 
   --base-url BASE_URL   Base URL for the oobabooga instance. This should be
                         ws://hostname[:port] for plain websocket connections, or
                         wss://hostname[:port] for websocket connections over TLS. (default:
                         ws://localhost:5005)
   --log-all-the-things  Print all AI input and output to STDOUT. (default: False)
+  --message-regex MESSAGE_REGEX
+                        A regex that will be used to extract message lines from the AI's
+                        output. The first capture group will be used as the message. If
+                        this is not set, the entire output will be used as the message.
+                        (default: )
 
 Stable Diffusion:
 
   --image-words [IMAGE_WORDS ...]
                         When one of these words is used in a message, the bot will generate
-                        an image. (default: ['drawing', 'photo', 'pic', 'picture', 'image',
-                        'sketch'])
+                        an image. (default: ['draw me', 'drawing', 'photo', 'pic',
+                        'picture', 'image', 'sketch'])
   --stable-diffusion-url STABLE_DIFFUSION_URL
                         URL for an AUTOMATIC1111 Stable Diffusion server. (default: )
   --extra-prompt-text EXTRA_PROMPT_TEXT
                         This will be appended to every image generation prompt sent to
                         Stable Diffusion. (default: )
+  --use-ai-generated-keywords
+                        FEATURE PREVIEW: If set, the bot will ask Oobabooga to generate
+                        image keywords from a user's message. It will then pass the
+                        keywords that Oobabooga produces to Stable Diffusion to finally
+                        generate an image. Otherwise, the bot will simply extract keywords
+                        directly from the user's message using a simple regex. (default:
+                        False)
 
 
 Additional settings can be set in config.yml.  Use the --generate-config option to print a
 new copy of this file to STDOUT.
 
 Please set the 'DISCORD_TOKEN' environment variable to your bot's discord token.
 ```
```

### Comparing `oobabot-0.1.7/pyproject.toml` & `oobabot-0.1.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oobabot"
-version = "0.1.7"
+version = "0.1.8"
 description = "A Discord bot which talks to Large Language Model AIs running on oobabooga's text-generation-webui"
 authors = ["Christopher Rude <chris@rudesoftware.net>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/chrisrude/oobabot"
 
 [tool.poetry.dependencies]
@@ -45,9 +45,9 @@
 
 [tool.pylint.'MAIN']
 py-version = '3.8.1'
 j = 8
 
 [tool.pylint.'MESSAGES CONTROL']
 max-line-length = 88
-disable = "C0103,C0114,C0115,C0116,R0902,R0903,R0913,R0914,W0201,W0511,W0621"
+disable = "C0116,R0902,R0903,R0912,R0913,R0914,W0511,W0621"
 include-naming-hint = true
```

### Comparing `oobabot-0.1.7/src/oobabot/bot_commands.py` & `oobabot-0.1.8/src/oobabot/bot_commands.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 # -*- coding: utf-8 -*-
+"""
+Implementation of the bot's slash commands.
+"""
 import typing
 
 import discord
 
 from oobabot import decide_to_respond
 from oobabot import discord_utils
 from oobabot import fancy_logger
+from oobabot import persona
 from oobabot import repetition_tracker
 from oobabot import templates
 
 
 class BotCommands:
+    """
+    Implementation of the bot's slash commands.
+    """
+
     def __init__(
         self,
         decide_to_respond: decide_to_respond.DecideToRespond,
         repetition_tracker: repetition_tracker.RepetitionTracker,
-        persona_settings: dict,
+        persona: persona.Persona,
         discord_settings: dict,
         template_store: templates.TemplateStore,
     ):
-        self.ai_name = persona_settings["ai_name"]
         self.decide_to_respond = decide_to_respond
         self.repetition_tracker = repetition_tracker
+        self.persona = persona
         self.reply_in_thread = discord_settings["reply_in_thread"]
         self.template_store = template_store
 
     async def on_ready(self, client: discord.Client):
         """
         Register commands with Discord.
         """
@@ -72,49 +80,54 @@
                         return channel
                     if isinstance(channel, discord.GroupChannel):
                         return channel
             return None
 
         @discord.app_commands.command(
             name="say",
-            description=f"Force {self.ai_name} to say the provided message.",
+            description=f"Force {self.persona.ai_name} to say the provided message.",
         )
         @discord.app_commands.rename(text_to_send="message")
         @discord.app_commands.describe(
-            text_to_send=f"Message to force {self.ai_name} to say."
+            text_to_send=f"Message to force {self.persona.ai_name} to say."
         )
         async def say(interaction: discord.Interaction, text_to_send: str):
             if interaction.channel_id is None:
                 await fail(interaction)
                 return
 
             # if reply_in_thread is True, we don't want our bot to
             # speak in guild channels, only threads and private messages
             if self.reply_in_thread:
                 channel = await get_messageable(interaction)
                 if channel is None or isinstance(channel, discord.TextChannel):
-                    await fail(interaction, f"{self.ai_name} may only speak in threads")
+                    await fail(
+                        interaction, f"{self.persona.ai_name} may only speak in threads"
+                    )
                     return
 
             fancy_logger.get().debug(
                 "/say called by user '%s' in channel #%d",
                 interaction.user.name,
                 interaction.channel_id,
             )
             # this will cause the bot to monitor the channel
             # and consider unsolicited responses
-            self.decide_to_respond.log_mention_raw(
+            self.decide_to_respond.log_mention(
                 channel_id=interaction.channel_id,
                 send_timestamp=interaction.created_at.timestamp(),
             )
-            await interaction.response.send_message(text_to_send)
+            await interaction.response.send_message(
+                text_to_send,
+                suppress_embeds=True,
+            )
 
         @discord.app_commands.command(
             name="lobotomize",
-            description=f"Erase {self.ai_name}'s memory of any message "
+            description=f"Erase {self.persona.ai_name}'s memory of any message "
             + "before now in this channel.",
         )
         async def lobotomize(interaction: discord.Interaction):
             channel = await get_messageable(interaction)
             if channel is None:
                 await fail(interaction)
                 return
@@ -133,21 +146,22 @@
                     channel_id=channel.id,
                     message_id=message.id,
                 )
 
             response = self.template_store.format(
                 template_name=templates.Templates.COMMAND_LOBOTOMIZE_RESPONSE,
                 format_args={
-                    templates.TemplateToken.AI_NAME: self.ai_name,
+                    templates.TemplateToken.AI_NAME: self.persona.ai_name,
                     templates.TemplateToken.USER_NAME: interaction.user.name,
                 },
             )
             await interaction.response.send_message(
                 response,
                 silent=True,
+                suppress_embeds=True,
             )
 
         fancy_logger.get().debug(
             "Registering commands, sometimes this takes a while..."
         )
 
         tree = discord.app_commands.CommandTree(client)
```

### Comparing `oobabot-0.1.7/src/oobabot/decide_to_respond.py` & `oobabot-0.1.8/src/oobabot/decide_to_respond.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # -*- coding: utf-8 -*-
+"""
+Decides whether the bot responds to a message.
+"""
+
 import random
-import re
 import typing
 
 from oobabot import fancy_logger
+from oobabot import persona
 from oobabot import types
 
 
 class LastReplyTimes(dict):
     """
     A dictionary that keeps track of the last time we were mentioned
     in a channel.
@@ -43,32 +47,26 @@
     """
     Decide whether to respond to a message.
     """
 
     def __init__(
         self,
         discord_settings: dict,
-        persona_settings: dict,
+        persona: persona.Persona,
         interrobang_bonus: float,
         time_vs_response_chance: typing.List[typing.Tuple[float, float]],
     ):
-        self.wakewords = persona_settings["wakewords"]
         self.ignore_dms = discord_settings["ignore_dms"]
         self.interrobang_bonus = interrobang_bonus
+        self.persona = persona
         self.time_vs_response_chance = time_vs_response_chance
 
         last_reply_cache_timeout = max(time for time, _ in time_vs_response_chance)
         self.last_reply_times = LastReplyTimes(last_reply_cache_timeout)
 
-        # match messages that include any `wakeword`, but not as part of
-        # another word
-        self.wakeword_patterns = [
-            re.compile(rf"\b{wakeword}\b", re.IGNORECASE) for wakeword in self.wakewords
-        ]
-
     def is_directly_mentioned(
         self, our_user_id: int, message: types.GenericMessage
     ) -> bool:
         """
         Returns True if the message is a direct message to us, or if it
         mentions us by @name or wakeword.
         """
@@ -81,17 +79,16 @@
 
         # reply to all messages in which we're @-mentioned
         if isinstance(message, types.ChannelMessage):
             if message.is_mentioned(our_user_id):
                 return True
 
         # reply to all messages that include a wakeword
-        for wakeword_pattern in self.wakeword_patterns:
-            if wakeword_pattern.search(message.body_text):
-                return True
+        if self.persona.contains_wakeword(message.body_text):
+            return True
 
         return False
 
     def calc_base_chance_of_unsolicited_reply(
         self, message: types.ChannelMessage
     ) -> float:
         """
@@ -108,14 +105,19 @@
                 response_chance = chance
                 break
         return response_chance
 
     def provide_unsolicited_reply_in_channel(
         self, our_user_id: int, message: types.ChannelMessage
     ) -> bool:
+        """
+        Returns True if we should respond to the message, even
+        though we weren't directly mentioned.
+        """
+
         # if we're not at-mentioned but others are, don't reply
         if message.mentions and not message.is_mentioned(our_user_id):
             return False
 
         # if message is empty, don't reply.  This can happen if someone
         # posts an image or an attachment without a comment.
         if message.is_empty():
@@ -185,12 +187,9 @@
         if isinstance(message, types.ChannelMessage):
             if self.provide_unsolicited_reply_in_channel(our_user_id, message):
                 return (True, False)
 
         # ignore anything else
         return (False, False)
 
-    def log_mention(self, message: types.ChannelMessage) -> None:
-        self.last_reply_times.log_mention(message.channel_id, message.send_timestamp)
-
-    def log_mention_raw(self, channel_id: int, send_timestamp: float) -> None:
+    def log_mention(self, channel_id: int, send_timestamp: float) -> None:
         self.last_reply_times.log_mention(channel_id, send_timestamp)
```

### Comparing `oobabot-0.1.7/src/oobabot/image_generator.py` & `oobabot-0.1.8/src/oobabot/image_generator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 # -*- coding: utf-8 -*-
+"""
+Generates images from Stable Diffusion
+"""
+
 import asyncio
 import io
 import re
 import typing
 
 import discord
 
+from oobabot import discord_utils
 from oobabot import fancy_logger
 from oobabot import http_client
+from oobabot import ooba_client
+from oobabot import prompt_generator
 from oobabot import sd_client
 from oobabot import templates
 
 
 async def image_task_to_file(image_task: "asyncio.Task[bytes]", image_request: str):
     await image_task
     img_bytes = image_task.result()
@@ -181,17 +188,17 @@
 
     async def diy_interaction_check(self, interaction: discord.Interaction) -> bool:
         """
         Only allow the requesting user to interact with this view.
         """
         if interaction.user.id == self.requesting_user_id:
             return True
-        error_mesage = self._get_message(templates.Templates.IMAGE_UNAUTHORIZED)
+        error_message = self._get_message(templates.Templates.IMAGE_UNAUTHORIZED)
         await interaction.response.send_message(
-            content=error_mesage,
+            content=error_message,
             ephemeral=True,
         )
         return False
 
     def get_image_message_text(self) -> str:
         return self._get_message(templates.Templates.IMAGE_CONFIRMATION)
 
@@ -205,39 +212,75 @@
                 templates.TemplateToken.USER_NAME: self.requesting_user_name,
                 templates.TemplateToken.IMAGE_PROMPT: self.image_prompt,
             },
         )
 
 
 class ImageGenerator:
+    """
+    Generates images from a given prompt, and posts that image as a
+    message to a given channel.
+    """
+
+    # if a potential image prompt is shorter than this, we will
+    # conclude that it is not an image prompt.
+    MIN_IMAGE_PROMPT_LENGTH = 3
+
     def __init__(
         self,
+        ooba_client: ooba_client.OobaClient,
+        persona_settings: typing.Dict[str, typing.Any],
+        prompt_generator: prompt_generator.PromptGenerator,
+        sd_settings: typing.Dict[str, typing.Any],
         stable_diffusion_client: sd_client.StableDiffusionClient,
-        image_words: typing.List[str],
         template_store: templates.TemplateStore,
     ):
+        self.ai_name = persona_settings.get("ai_name", "")
+        self.ooba_client = ooba_client
+        self.image_words = sd_settings.get("image_words", [])
+        self.prompt_generator = prompt_generator
         self.stable_diffusion_client = stable_diffusion_client
         self.template_store = template_store
+        self.use_ai_generated_keywords = sd_settings.get("use_ai_generated_keywords")
+
         self.image_patterns = [
             re.compile(
                 r"^.*\b" + image_word + r"\b[\s]*(of|with)?[\s]*[:]?(.*)$",
                 re.IGNORECASE,
             )
-            for image_word in image_words
+            for image_word in self.image_words
         ]
 
+    def on_ready(self):
+        """
+        Called when the bot is connected to Discord.
+        """
+        if self.use_ai_generated_keywords:
+            fancy_logger.get().debug(
+                "Stable Diffusion: image prompts generated with AI preprocessing"
+            )
+        else:
+            fancy_logger.get().debug(
+                "Stable Diffusion: image prompts extracted with regex"
+            )
+
+        fancy_logger.get().debug(
+            "Stable Diffusion: image keywords: %s",
+            ", ".join(self.image_words),
+        )
+
     async def _generate_image(
         self,
         image_prompt: str,
         raw_message: discord.Message,
         response_channel: discord.abc.Messageable,
     ) -> discord.Message:
         is_channel_nsfw = False
 
-        # note: public threads in NSFW chanels are not considered here
+        # note: public threads in NSFW channels are not considered here
         if isinstance(raw_message.channel, discord.TextChannel):
             is_channel_nsfw = raw_message.channel.is_nsfw()
 
         image_task = self.stable_diffusion_client.generate_image(
             image_prompt, is_channel_nsfw=is_channel_nsfw
         )
         try:
@@ -281,28 +324,57 @@
     def maybe_get_image_prompt(
         self, raw_message: discord.Message
     ) -> typing.Optional[str]:
         for image_pattern in self.image_patterns:
             match = image_pattern.search(raw_message.content)
             if match:
                 image_prompt = match.group(2)
+                if len(image_prompt) < self.MIN_IMAGE_PROMPT_LENGTH:
+                    continue
                 fancy_logger.get().debug("Found image prompt: %s", image_prompt)
                 return image_prompt
         return None
 
     async def generate_image(
         self,
-        image_prompt: str,
+        user_image_keywords: str,
         raw_message: discord.Message,
         response_channel: discord.abc.Messageable,
-    ) -> typing.Optional["asyncio.Task[discord.Message]"]:
+    ) -> "asyncio.Task[discord.Message]":
         """
-        If the message contains a photo word, kick off a task
-        to generate an image, post it to the channel, and return
-        the generated message.
-
-        If the message does not contain a photo word, return None.
+        Kick off a task to generate an image, post it to the channel,
+        and return message the image is posted in.
         """
-        create_image_task = asyncio.create_task(
-            self._generate_image(image_prompt, raw_message, response_channel)
+
+        if self.use_ai_generated_keywords:
+            # ignore the prompt extracted above, and instead pass
+            # the raw message back to Oobabooga and ask it to
+            # generate keywords.  Then pass those keywords to
+            # the image generator.
+            return asyncio.create_task(
+                self._generate_keywords_then_image(
+                    raw_message,
+                    response_channel,
+                )
+            )
+
+        return asyncio.create_task(
+            self._generate_image(user_image_keywords, raw_message, response_channel)
+        )
+
+    async def _generate_keywords_then_image(
+        self,
+        raw_message: discord.Message,
+        response_channel: discord.abc.Messageable,
+    ) -> "discord.Message":
+        message = discord_utils.discord_message_to_generic_message(raw_message)
+        # remove the bot's name from the body text, so it doesn't
+        # pollute the keywords
+        message.body_text = message.body_text.replace(self.ai_name, "")
+        keyword_generation_prompt = self.prompt_generator.keyword_generation_prompt(
+            message
+        )
+        ai_keywords = await self.ooba_client.request_as_string(
+            keyword_generation_prompt
         )
-        return create_image_task
+        fancy_logger.get().debug("AI-generated keywords: %s", ai_keywords)
+        return await self._generate_image(ai_keywords, raw_message, response_channel)
```

### Comparing `oobabot-0.1.7/src/oobabot/ooba_client.py` & `oobabot-0.1.8/src/oobabot/ooba_client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # -*- coding: utf-8 -*-
-# Purpose: Streaming client for the Ooba API.
-# Can provide the response by token or by sentence.
-#
-
-# Purpose: Split a string into sentences, based on a set of terminators.
-#          This is a helper class for ooba_client.py.
+"""
+Client for the Ooba API.
+Can provide the response by token or by sentence.
+"""
+import abc
 import json
+import re
 import time
 import typing
 
 import aiohttp
 import pysbd
 
 from oobabot import fancy_logger
 from oobabot import http_client
 
 
-class SentenceSplitter:
+class MessageSplitter(abc.ABC):
     """
-    Purpose: Split an English string into sentences.
+    Split a response into separate messages.
     """
 
     # anything that can't be in a real response
     END_OF_INPUT = ""
 
     def __init__(self):
         self.printed_idx = 0
         self.full_response = ""
-        self.segmenter = pysbd.Segmenter(language="en", clean=False, char_span=True)
 
-    def by_sentence(self, new_token: str) -> typing.Generator[str, None, None]:
+    def next(self, new_token: str) -> typing.Generator[str, None, None]:
         """
-        Collects tokens into a single string, looks for ends of english
-        sentences, then yields each sentence as soon as it's found.
+        Collects tokens into a single string, splits into messages
+        by the subclass's logic, then yields each message as soon
+        as it's found.
 
         Parameters:
             new_token: str, the next token to add to the string
 
         Returns:
             Generator[str, None, None], yields each sentence
 
         Note:
         When there is no longer any input, the caller must pass
-        SentenceSplitter.END_OF_INPUT to this function.  This
+        MessageSplitter.END_OF_INPUT to this function.  This
         function will then yield any remaining text, even if it
         doesn't look like a full sentence.
         """
 
         self.full_response += new_token
         unseen = self.full_response[self.printed_idx :]
 
@@ -55,14 +55,52 @@
         if self.END_OF_INPUT == new_token:
             to_print = unseen.strip()
             if to_print:
                 yield unseen
             self.printed_idx += len(unseen)
             return
 
+        yield from self.partition(unseen)
+
+    @abc.abstractmethod
+    def partition(self, unseen: str) -> typing.Generator[str, None, None]:
+        pass
+
+
+class RegexSplitter(MessageSplitter):
+    """
+    Split a response into separate messages using a regex.
+    """
+
+    def __init__(self, regex: str):
+        super().__init__()
+        self.pattern = re.compile(regex)
+
+    def partition(self, unseen: str) -> typing.Generator[str, None, None]:
+        while True:
+            match = self.pattern.match(unseen)
+            if not match:
+                break
+            to_print = match.group(1)
+            yield to_print
+            self.printed_idx += match.end()
+            unseen = self.full_response[self.printed_idx :]
+
+
+class SentenceSplitter(MessageSplitter):
+    """
+    Split a response into separate messages using English
+    sentence word breaks.
+    """
+
+    def __init__(self):
+        super().__init__()
+        self.segmenter = pysbd.Segmenter(language="en", clean=False, char_span=True)
+
+    def partition(self, unseen: str) -> typing.Generator[str, None, None]:
         segments = self.segmenter.segment(unseen)
 
         # any remaining non-sentence things will be in the last element
         # of the list.  Don't print that yet.  At the very worst, we'll
         # print it when the END_OF_INPUT signal is reached.
         for sentence_w_char_spans in segments[:-1]:
             # sentence_w_char_spans is a class with the following fields:
@@ -77,55 +115,89 @@
             if to_print.endswith("\n"):
                 to_print = to_print[:-1]
 
             yield to_print
 
         # since we've printed all the previous segments,
         # the start of the last segment becomes the starting
-        # point for the next roud.
+        # point for the next round.
         if len(segments) > 0:
             self.printed_idx += segments[-1].start  # type: ignore
 
 
 class OobaClient(http_client.SerializedHttpClient):
-    # Purpose: Streaming client for the Ooba API.
-    # Can provide the response by token or by sentence.
+    """
+    Client for the Ooba API.  Can provide the response by token or by sentence.
+    """
 
     SERVICE_NAME = "Oobabooga"
 
     OOBABOOGA_STREAMING_URI_PATH: str = "/api/v1/stream"
 
     def __init__(
         self,
         settings: typing.Dict[str, typing.Any],
     ):
         super().__init__(self.SERVICE_NAME, settings["base_url"])
         self.total_response_tokens = 0
+        self.message_regex = settings["message_regex"]
         self.request_params = settings["request_params"]
         self.log_all_the_things = settings["log_all_the_things"]
 
+        if self.message_regex:
+            self.fn_new_splitter = lambda: RegexSplitter(self.message_regex)
+        else:
+            self.fn_new_splitter = SentenceSplitter
+
+    def on_ready(self):
+        """
+        Called when the client is ready to start.
+        Used to log our configuration.
+        """
+        if self.message_regex:
+            fancy_logger.get().debug(
+                "Ooba Client: Splitting responses into messages " + "with: %s",
+                self.message_regex,
+            )
+        else:
+            fancy_logger.get().debug(
+                "Ooba Client: Splitting responses into messages "
+                + "by English sentence.",
+            )
+
     async def _setup(self):
-        async with self.get_session().ws_connect(self.OOBABOOGA_STREAMING_URI_PATH):
+        async with self._get_session().ws_connect(self.OOBABOOGA_STREAMING_URI_PATH):
             return
 
-    async def request_by_sentence(self, prompt: str) -> typing.AsyncIterator[str]:
+    def get_stopping_strings(self) -> typing.List[str]:
         """
-        Yields each complete sentence of the response as it arrives.
+        Returns a list of strings that indicate the end of a response.
+        Taken from the yaml `stopping_strings` within our
+        response_params.
         """
+        return self.request_params.get("stopping_strings", [])
 
-        splitter = SentenceSplitter()
+    async def request_by_message(self, prompt: str) -> typing.AsyncIterator[str]:
+        """
+        Yields individual messages from the response as it arrives.
+        These can be split by a regex or by sentence.
+        """
+        splitter = self.fn_new_splitter()
         async for new_token in self.request_by_token(prompt):
-            for sentence in splitter.by_sentence(new_token):
+            for sentence in splitter.next(new_token):
+                # remove "### Assistant: " from strings
+                if sentence.startswith("### Assistant: "):
+                    sentence = sentence[len("### Assistant: ") :]
                 yield sentence
 
-    async def request_as_string(self, prompt: str) -> typing.AsyncIterator[str]:
+    async def request_as_string(self, prompt: str) -> str:
         """
         Yields the entire response as a single string.
         """
-        yield "".join([token async for token in self.request_by_token(prompt)])
+        return "".join([token async for token in self.request_by_token(prompt)])
 
     async def request_as_grouped_tokens(
         self,
         prompt: str,
         interval: float = 0.2,
     ) -> typing.AsyncIterator[str]:
         """
@@ -155,15 +227,15 @@
         request: dict[
             str, typing.Union[bool, float, int, str, typing.List[typing.Any]]
         ] = {
             "prompt": prompt,
         }
         request.update(self.request_params)
 
-        async with self.get_session().ws_connect(
+        async with self._get_session().ws_connect(
             self.OOBABOOGA_STREAMING_URI_PATH
         ) as websocket:
             await websocket.send_json(request)
             if self.log_all_the_things:
                 print(f"Sent request:\n{json.dumps(request, indent=1)}")
                 print(f"Prompt:\n{request['prompt']}")
 
@@ -190,14 +262,16 @@
                             if self.log_all_the_things:
                                 print(text, end="", flush=True)
 
                             yield text
 
                     elif "stream_end" == incoming_data["event"]:
                         # Make sure any unprinted text is flushed.
+                        if self.log_all_the_things:
+                            print("", flush=True)
                         yield SentenceSplitter.END_OF_INPUT
                         return
 
                     else:
                         fancy_logger.get().warning(
                             "Unexpected event: %s", incoming_data
                         )
```

### Comparing `oobabot-0.1.7/src/oobabot/prompt_generator.py` & `oobabot-0.1.8/src/oobabot/prompt_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # -*- coding: utf-8 -*-
-# purpose: generate a prompt for the AI to respond to, given
-# the message history and persona.
+"""
+Generate a prompt for the AI to respond to, given the
+message history and persona.
+"""
 import typing
 
 from oobabot import fancy_logger
+from oobabot import persona
 from oobabot import templates
 from oobabot import types
 
 
 class PromptGenerator:
     """
     Purpose: generate a prompt for the AI to use, given
@@ -18,15 +21,15 @@
     # it will understand before it starts to ignore
     # the rest of the prompt_prefix
     # note: we don't currently measure tokens, we just
     # count characters. This is a rough estimate.
     EST_CHARACTERS_PER_TOKEN = 3
 
     # the estimated number of characters in a line of message history
-    # this is used to rougly calculate whether we'll have enough space
+    # this is used to roughly calculate whether we'll have enough space
     # to supply the requested number of lines of history.
     #
     # in practice, we will look at the actual number of characters to
     # see what we can fit.
     #
     # note that we're doing calculations in characters, not in tokens,
     # so even counting characters exactly is still an estimate.
@@ -37,39 +40,38 @@
     # so we use a different estimate
     EST_CHARACTERS_PER_HISTORY_LINE_NOT_SPLITTING_RESPONSES = 180
 
     def __init__(
         self,
         discord_settings: dict,
         oobabooga_settings: dict,
-        persona_settings: dict,
+        persona: persona.Persona,
         template_store: templates.TemplateStore,
     ):
-        self.ai_name = persona_settings["ai_name"]
         self.dont_split_responses = discord_settings["dont_split_responses"]
         self.history_lines = discord_settings["history_lines"]
-        self.persona = persona_settings["persona"]
         self.token_space = oobabooga_settings["request_params"]["truncation_length"]
 
+        self.persona = persona
         self.template_store = template_store
 
         # this will be also used when sending message
         # to suppress sending the prompt text to the user
         self.bot_prompt_line = self.template_store.format(
             templates.Templates.PROMPT_HISTORY_LINE,
             {
-                templates.TemplateToken.USER_NAME: self.ai_name,
+                templates.TemplateToken.USER_NAME: self.persona.ai_name,
                 templates.TemplateToken.USER_MESSAGE: "",
             },
         ).strip()
 
         self.image_request_made = self.template_store.format(
             templates.Templates.PROMPT_IMAGE_COMING,
             {
-                templates.TemplateToken.AI_NAME: self.ai_name,
+                templates.TemplateToken.AI_NAME: self.persona.ai_name,
             },
         )
 
         self._init_history_available_chars()
 
     def _init_history_available_chars(self) -> None:
         """
@@ -102,29 +104,27 @@
             chars_per_history_line = (
                 self.EST_CHARACTERS_PER_HISTORY_LINE_NOT_SPLITTING_RESPONSES
             )
 
         required_history_size_chars = self.history_lines * chars_per_history_line
 
         if available_chars_for_history < required_history_size_chars:
-            raise ValueError(
+            fancy_logger.get().warning(
                 "AI token space is too small for prompt_prefix and history "
-                + "by an estimated "
-                + f"{required_history_size_chars - available_chars_for_history}"
+                + "by an estimated %d"
                 + " characters.  You may lose history context.  You can save space"
                 + " by shortening the persona or reducing the requested number of"
-                + " lines of history."
+                + " lines of history.",
+                required_history_size_chars - available_chars_for_history,
             )
         self.max_history_chars = available_chars_for_history
 
     async def _render_history(
         self,
-        ai_user_id: int,
         message_history: typing.AsyncIterator[types.GenericMessage],
-        stop_before_message_id: typing.Optional[int],
     ) -> str:
         # add on more history, but only if we have room
         # if we don't have room, we'll just truncate the history
         # by discarding the oldest messages first
         # this is s
         # it will understand before ignore
         #
@@ -132,39 +132,21 @@
 
         # history_lines is newest first, so figure out
         # how many we can take, then append them in
         # reverse order
         history_lines = []
 
         async for message in message_history:
-            # if we've hit the throttle message, stop and don't add any
-            # more history
-            if stop_before_message_id and message.message_id == stop_before_message_id:
-                break
-
-            adjusted_author_name = message.author_name
-            if message.author_id == ai_user_id:
-                # make sure the AI always sees its persona name
-                # in the transcript, even if the chat program
-                # has it under a different account name
-                adjusted_author_name = self.ai_name
-
-                # we'll ignore any messages we generate which refer
-                # another message, since those are ones our image
-                # generation code generated
-                if message.reference_message_id:
-                    continue
-
             if not message.body_text:
                 continue
 
             line = self.template_store.format(
                 templates.Templates.PROMPT_HISTORY_LINE,
                 {
-                    templates.TemplateToken.USER_NAME: adjusted_author_name,
+                    templates.TemplateToken.USER_NAME: message.author_name,
                     templates.TemplateToken.USER_MESSAGE: message.body_text,
                 },
             )
 
             if len(line) > prompt_len_remaining:
                 num_discarded_lines = self.history_lines - len(history_lines)
                 fancy_logger.get().warning(
@@ -183,34 +165,48 @@
         self,
         message_history_txt: str,
         image_coming: str,
     ) -> str:
         prompt = self.template_store.format(
             templates.Templates.PROMPT,
             {
-                templates.TemplateToken.AI_NAME: self.ai_name,
-                templates.TemplateToken.PERSONA: self.persona,
+                templates.TemplateToken.AI_NAME: self.persona.ai_name,
+                templates.TemplateToken.PERSONA: self.persona.persona,
                 templates.TemplateToken.MESSAGE_HISTORY: message_history_txt,
                 templates.TemplateToken.IMAGE_COMING: image_coming,
             },
         )
-        # todo: make this part of the template?
         prompt += self.bot_prompt_line + "\n"
         return prompt
 
     async def generate(
         self,
-        ai_user_id: int,
         message_history: typing.Optional[typing.AsyncIterator[types.GenericMessage]],
         image_requested: bool,
-        throttle_message_id: int,
     ) -> str:
         """
         Generate a prompt for the AI to respond to.
         """
         message_history_txt = ""
         if message_history is not None:
             message_history_txt = await self._render_history(
-                ai_user_id, message_history, throttle_message_id
+                message_history,
             )
         image_coming = self.image_request_made if image_requested else ""
         return self._generate(message_history_txt, image_coming)
+
+    def keyword_generation_prompt(
+        self,
+        image_request_message: types.GenericMessage,
+    ) -> str:
+        """
+        given a message that requests an image, generate a prompt
+        to the AI to take that message text and generate a set of
+        keywords describing that image
+        """
+        return self.template_store.format(
+            templates.Templates.PROMPT_IMAGE_KEYWORDS,
+            {
+                templates.TemplateToken.AI_NAME: self.persona.ai_name,
+                templates.TemplateToken.USER_MESSAGE: image_request_message.body_text,
+            },
+        )
```

### Comparing `oobabot-0.1.7/src/oobabot/repetition_tracker.py` & `oobabot-0.1.8/src/oobabot/repetition_tracker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 # -*- coding: utf-8 -*-
+"""
+Detects when the bot is repeating previous messages, and attempts
+to fix this by hiding the messages that it's repeating from its view
+of the chat history.
+
+Is also used to implement the /lobotomize command, which is the same
+thing except it's triggered by a command instead of automatically.
+"""
 import typing
 
 from oobabot import fancy_logger
 from oobabot import types
 
 
 class RepetitionTracker:
-    # how many times the bot can repeat the same thing before we
-    # throttle history
+    """
+    Tracks the last message the bot posted in each channel, and
+    the number of times in a row it has been repeated.
+    """
 
     def __init__(self, repetition_threshold: int) -> None:
         self.repetition_threshold = repetition_threshold
 
         # stores a map of channel_id ->
-        #   (last_message, throttle_message_id, repetion_count)
+        #   (last_message, throttle_message_id, repetition_count)
 
         self.repetition_count: typing.Dict[int, typing.Tuple[str, int, int]] = {}
 
     def get_throttle_message_id(self, channel_id: int) -> int:
         """
         Returns the message ID of the last message that should be throttled, or 0
         if no throttling is needed
```

### Comparing `oobabot-0.1.7/src/oobabot/response_stats.py` & `oobabot-0.1.8/src/oobabot/response_stats.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 # -*- coding: utf-8 -*-
+"""
+Purpose: collects timing and rate statistics for the bot's responses
+"""
+
 import time
 import typing
 
 from oobabot import fancy_logger
 
 
 class ResponseStats:
@@ -133,14 +137,16 @@
     def average_tokens_per_second(self) -> float:
         """
         Returns the average rate at which tokens were generated,
         in tokens per second.
         """
         if 0 == self.total_successful_responses:
             return 0.0
+        if 0.0 == self.total_response_time_seconds:
+            return 0.0
         return self.fn_get_total_tokens() / self.total_response_time_seconds
 
     def average_prompt_length(self) -> float:
         """
         Returns the average prompt length in characters.
         """
         if 0 == self.total_requests_received:
@@ -153,15 +159,15 @@
         Call this after all AggregateResponseStats have been handled.
         """
         if 0 == self.total_requests_received:
             fancy_logger.get().info("No requests handled")
             return
 
         fancy_logger.get().info(
-            f"Recevied {self.total_requests_received} request(s), "
+            f"Received {self.total_requests_received} request(s), "
             + f"sent {self.total_successful_responses} successful responses "
             + f"and failed to send one {self.total_failed_responses} times(s)"
         )
 
         if self.total_failed_responses > 0:
             fancy_logger.get().error(
                 "Error rate:                  %0.2f%%", self.error_rate()
```

### Comparing `oobabot-0.1.7/src/oobabot/sd_client.py` & `oobabot-0.1.8/src/oobabot/sd_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
-# Purpose: Client for generating images using the AUTOMATIC1111
-# API.  Takes a prompt and returns image binary data in PNG format.
-#
+"""
+Client for generating images using the AUTOMATIC1111
+API.  Takes a prompt and returns image binary data in PNG format.
+"""
 
 import asyncio
 import base64
 import time
 import typing
 
 import aiohttp
@@ -95,68 +96,69 @@
         # reasons;
         #  - show the user exactly what we changed, if anything
         #  - some versions of the API don't support the
         #    "do_not_add_watermark" option, so we need to
         #    check if it's there before we try to set it
         #
         current_options = None
-        async with self.get_session().get(url) as response:
+        async with self._get_session().get(url) as response:
             if response.status != 200:
                 raise http_client.OobaHttpClientError(response)
             current_options = await response.json()
 
-        # now, set the options
         options_to_set = {}
-        for k, v in self.DEFAULT_OPTIONS.items():
-            if k not in current_options:
+        for option_name, option_value in self.DEFAULT_OPTIONS.items():
+            if option_name not in current_options:
                 continue
-            if v == current_options[k]:
+            if option_value == current_options[option_name]:
                 continue
-            options_to_set[k] = v
+            options_to_set[option_name] = option_value
             fancy_logger.get().info(
                 "Stable Diffusion:  changing option '%s' from to '%s' to '%s'",
-                k,
-                current_options[k],
-                v,
+                option_name,
+                current_options[option_name],
+                option_value,
             )
 
         if not options_to_set:
             fancy_logger.get().debug(
                 "Stable Diffusion: Options are already set correctly, no changes made."
             )
             return
 
-        async with self.get_session().post(url, json=options_to_set) as response:
+        async with self._get_session().post(url, json=options_to_set) as response:
             if response.status != 200:
                 raise http_client.OobaHttpClientError(response)
             await response.json()
 
     async def get_samplers(self) -> typing.List[str]:
         url = self.API_COMMAND_URLS["get_samplers"]
-        async with self.get_session().get(url) as response:
+        async with self._get_session().get(url) as response:
             if response.status != 200:
                 raise http_client.OobaHttpClientError(response)
             response = await response.json()
             samplers = [str(sampler["name"]) for sampler in response]
             return samplers
 
     def generate_image(
         self,
         prompt: str,
         is_channel_nsfw: bool = False,
     ) -> "asyncio.Task[bytes]":
-        # Purpose: Generate an image from a prompt.
-        # Args:
-        #     prompt: The prompt to generate an image from.
-        #     is_channel_nsfw: Whether the channel is NSFW.
-        #     this will change the negative prompt.
-        # Returns:
-        #     The image as bytes.
-        # Raises:
-        #     OobaHttpClientError, if the request fails.
+        """
+        Generate an image from a prompt.
+        Args:
+            prompt: The prompt to generate an image from.
+            is_channel_nsfw: Whether the channel is NSFW.
+            this will change the negative prompt.
+        Returns:
+            The image as bytes.
+        Raises:
+            OobaHttpClientError, if the request fails.
+        """
         request = self.request_params.copy()
         request["prompt"] = prompt
         if is_channel_nsfw:
             request["negative_prompt"] = self.negative_prompt_nsfw
 
         if self.extra_prompt_text:
             request["prompt"] += ", " + self.extra_prompt_text
@@ -165,15 +167,15 @@
             fancy_logger.get().debug(
                 "Stable Diffusion: Image request (nsfw: %r): %s",
                 is_channel_nsfw,
                 request["prompt"],
             )
             start_time = time.time()
 
-            async with self.get_session().post(
+            async with self._get_session().post(
                 self.API_COMMAND_URLS["txt2img"],
                 json=request,
             ) as response:
                 if response.status != 200:
                     raise http_client.OobaHttpClientError(response)
                 duration = time.time() - start_time
                 json_body = await response.json()
@@ -187,17 +189,25 @@
 
         # works around aiohttp being bad
         async def do_post_with_retry() -> bytes:
             tries = 0
             while True:
                 try:
                     return await do_post()
-                except aiohttp.ClientError as err:
-                    if tries > 2 or err.__cause__ is not ConnectionResetError:
-                        raise http_client.OobaHttpClientError(err) from err
+                except (aiohttp.ClientError, aiohttp.ClientOSError) as err:
+                    retry = False
+                    if err.__cause__ is ConnectionResetError:
+                        retry = True
+                    if isinstance(err, aiohttp.ClientOSError) and 104 == err.errno:
+                        retry = True
+                    if tries > 2:
+                        retry = False
+                    if not retry:
+                        raise
+
                     fancy_logger.get().warning(
                         "Stable Diffusion: Connection reset error: %s, "
                         + "retrying in 1 second",
                         err,
                     )
                     await asyncio.sleep(1)
                     tries += 1
```

### Comparing `oobabot-0.1.7/src/oobabot/settings.py` & `oobabot-0.1.8/src/oobabot/settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,56 @@
 # -*- coding: utf-8 -*-
+"""
+Documents all the settings for the bot.  Allows for settings
+to be loaded from the environment, command line and config file.
+
+Methods:
+    - load:
+        loads settings from the environment, command line and config file
+
+    - write_to_stream:
+        writes the current config file to the given stream
+
+    - write_to_file:
+        writes the current config file to the given file path
+
+Attributes:
+    - setting_groups:
+        a list of all the setting groups
+
+    - discord_settings:
+        a setting group for settings related to Discord
+
+    - oobabooga_settings:
+        a setting group for settings related to the oobabooga API
+
+    - stable_diffusion_settings:
+        a setting group for settings related to the stable diffusion API
+
+    - general_settings:
+        a setting group for settings that are not included in the config file
+"""
 import os
 import shutil
 import sys
 import textwrap
 import typing
 
 from oobabot import templates
 import oobabot.overengineered_settings_parser as oesp
 
 
-def console_wrapped(message):
+def _console_wrapped(message):
     width = shutil.get_terminal_size().columns
     return "\n".join(textwrap.wrap(message, width))
 
 
-def make_template_comment(
+def _make_template_comment(
     name: str,
-    tokens_desc_tuple: typing.Tuple[typing.List[templates.TemplateToken], str],
+    tokens_desc_tuple: typing.Tuple[typing.List[templates.TemplateToken], str, bool],
 ) -> typing.List[str]:
     return [
         f"Path to a file containing the {name} template.",
         tokens_desc_tuple[1],
         ".",
         f"Allowed tokens: {', '.join([str(t) for t in tokens_desc_tuple[0]])}",
         ".",
@@ -108,14 +138,15 @@
         "width": 512,
         "height": 512,
         "sampler": "",
     }
     # words to look for in the prompt to indicate that the user
     # wants to generate an image
     DEFAULT_IMAGE_WORDS: typing.List[str] = [
+        "draw me",
         "drawing",
         "photo",
         "pic",
         "picture",
         "image",
         "sketch",
     ]
@@ -123,14 +154,15 @@
     # ENVIRONMENT VARIABLES ####
     DISCORD_TOKEN_ENV_VAR: str = "DISCORD_TOKEN"
     OOBABOT_PERSONA_ENV_VAR: str = "OOBABOT_PERSONA"
 
     def __init__(self):
         self._settings = None
 
+        self.arg_parser = None
         self.setting_groups: typing.List[oesp.ConfigSettingGroup] = []
 
         ###########################################################
         # General Settings
         #  won't be included in the config.yaml
 
         self.general_settings = oesp.ConfigSettingGroup(
@@ -169,14 +201,30 @@
                         then exit.  Any command-line settings also passed will be
                         reflected in this file.
                         """
                     )
                 ],
             )
         )
+        self.general_settings.add_setting(
+            oesp.ConfigSetting[bool](
+                name="invite_url",
+                default=False,
+                description_lines=[
+                    textwrap.dedent(
+                        """
+                        Print a URL which can be used to invite the
+                        bot to a Discord server.  Requires that
+                        the Discord token is set.
+                        """
+                    ),
+                ],
+                cli_args=["--invite-url"],
+            )
+        )
 
         ###########################################################
         # Persona Settings
 
         self.persona_settings = oesp.ConfigSettingGroup("Persona")
         self.setting_groups.append(self.persona_settings)
 
@@ -202,23 +250,46 @@
                         {self.OOBABOT_PERSONA_ENV_VAR} environment variable.
                         """
                     )
                 ],
                 show_default_in_yaml=False,
             )
         )
+        # path to a json or txt file containing persona
+        self.persona_settings.add_setting(
+            oesp.ConfigSetting[str](
+                name="persona_file",
+                default="",
+                description_lines=[
+                    textwrap.dedent(
+                        """
+                        Path to a file containing a persona.  This can be just a
+                        single string, a json file in the common "tavern" formats,
+                        or a yaml file in the Oobabooga format.
+
+                        With a single string, the persona will be set to that string.
+
+                        Otherwise, the ai_name and persona will be overwritten with
+                        the values in the file.  Also, the wakewords will be
+                        extended to include the character's own name.
+                        """
+                    )
+                ],
+                include_in_argparse=False,
+            )
+        )
         self.persona_settings.add_setting(
             oesp.ConfigSetting[typing.List[str]](
                 name="wakewords",
                 default=["oobabot"],
                 description_lines=[
                     textwrap.dedent(
                         """
                         One or more words that the bot will listen for.
-                        The bot will listen in all discord channels can
+                        The bot will listen in all discord channels it can
                         access for one of these words to be mentioned, then reply
                         to any messages it sees with a matching word.
                         The bot will always reply to @-mentions and
                         direct messages, even if no wakewords are supplied.
                         """
                     )
                 ],
@@ -243,25 +314,26 @@
                         {self.DISCORD_TOKEN_ENV_VAR} environment variable
                         instead, if possible.
                         """
                     )
                 ],
                 cli_args=["--discord-token"],
                 show_default_in_yaml=False,
+                place_default_in_yaml=True,
             )
         )
         self.discord_settings.add_setting(
             oesp.ConfigSetting[bool](
                 name="dont_split_responses",
                 default=False,
                 description_lines=[
                     textwrap.dedent(
                         """
                         Post the entire response as a single message, rather than
-                        splitting it into seperate messages by sentence.
+                        splitting it into separate messages by sentence.
                         """
                     )
                 ],
             )
         )
         self.discord_settings.add_setting(
             oesp.ConfigSetting[int](
@@ -286,14 +358,26 @@
                         """
                         If set, the bot will not respond to direct messages.
                         """
                     )
                 ],
             )
         )
+        # log level
+        self.discord_settings.add_setting(
+            oesp.ConfigSetting[str](
+                name="log_level",
+                default="DEBUG",
+                description_lines=[
+                    "Set the log level.  Valid values are: ",
+                    "CRITICAL, ERROR, WARNING, INFO, DEBUG",
+                ],
+                include_in_argparse=False,
+            )
+        )
         self.discord_settings.add_setting(
             oesp.ConfigSetting[bool](
                 name="reply_in_thread",
                 default=False,
                 description_lines=[
                     textwrap.dedent(
                         """
@@ -325,15 +409,17 @@
         self.discord_settings.add_setting(
             oesp.ConfigSetting[bool](
                 name="stream_responses",
                 default=False,
                 description_lines=[
                     textwrap.dedent(
                         """
-                        Stream responses into a single message as they are generated.
+                        FEATURE PREVIEW: Stream responses into a single message
+                        as they are generated.
+                        Note: may be janky
                         """
                     )
                 ],
             )
         )
 
         ###########################################################
@@ -366,14 +452,31 @@
                         """
                         Print all AI input and output to STDOUT.
                         """
                     )
                 ],
             )
         )
+        # get a regex for filtering a message
+        self.oobabooga_settings.add_setting(
+            oesp.ConfigSetting[str](
+                name="message_regex",
+                default="",
+                description_lines=[
+                    textwrap.dedent(
+                        """
+                        A regex that will be used to extract message lines
+                        from the AI's output.  The first capture group will
+                        be used as the message.  If this is not set, the
+                        entire output will be used as the message.
+                        """
+                    )
+                ],
+            )
+        )
         self.oobabooga_settings.add_setting(
             oesp.ConfigSetting[oesp.SettingDictType](
                 name="request_params",
                 default=self.OOBABOOGA_DEFAULT_REQUEST_PARAMS,
                 description_lines=[
                     textwrap.dedent(
                         """
@@ -383,14 +486,15 @@
                         See Oobabooga's documentation for what these parameters
                         mean.
                         """
                     )
                 ],
                 include_in_argparse=False,
                 show_default_in_yaml=False,
+                place_default_in_yaml=True,
             )
         )
 
         ###########################################################
         # Stable Diffusion Settings
 
         self.stable_diffusion_settings = oesp.ConfigSettingGroup("Stable Diffusion")
@@ -450,41 +554,63 @@
                         See Stable Diffusion's documentation for what these parameters
                         mean.
                         """
                     )
                 ],
                 include_in_argparse=False,
                 show_default_in_yaml=False,
+                place_default_in_yaml=True,
+            )
+        )
+        self.stable_diffusion_settings.add_setting(
+            oesp.ConfigSetting[bool](
+                name="use_ai_generated_keywords",
+                default=False,
+                description_lines=[
+                    textwrap.dedent(
+                        """
+                        FEATURE PREVIEW: If set, the bot will ask Oobabooga to generate
+                        image keywords from a user's message.  It will then pass the
+                        keywords that Oobabooga produces to Stable Diffusion to finally
+                        generate an image.
+                        Otherwise, the bot will simply extract keywords directly
+                        from the user's message using a simple regex.
+                        """
+                    )
+                ],
             )
         )
 
         ###########################################################
         # Template Settings
 
         self.template_settings = oesp.ConfigSettingGroup(
             "Template",
             description="UI and AI request templates",
             include_in_argparse=False,
-            # todo: turn back on in later release
-            include_in_yaml=False,
         )
         self.setting_groups.append(self.template_settings)
 
         for template, tokens_desc_tuple in templates.TemplateStore.TEMPLATES.items():
+            _, _, is_ai_prompt = tokens_desc_tuple
+
             self.template_settings.add_setting(
                 oesp.ConfigSetting[str](
                     name=str(template),
                     default=templates.TemplateStore.DEFAULT_TEMPLATES[template],
-                    description_lines=make_template_comment(
+                    description_lines=_make_template_comment(
                         str(template), tokens_desc_tuple
                     ),
-                    show_default_in_yaml=False,
+                    include_in_yaml=is_ai_prompt,
                 )
             )
 
+        self._add_deprecated_settings()
+
+    def _add_deprecated_settings(self) -> None:
         ###########################################################
         # Deprecated Settings
         # These used to be part of the Stable Diffusion section,
         # but now are covered in the stable_diffusion->request_params
         # section of the config.yml file.
         #
         # These are still here for backwards compatibility, but
@@ -619,62 +745,93 @@
             #
             #  e.g. oobabot --generate-config > config.yml
             #       oobabot
             """
         )
     )
 
-    def write_sample_config(self, out_stream) -> None:
-        oesp.write_sample_config(self.setting_groups, out_stream)
+    def write_to_stream(self, out_stream) -> None:
+        oesp.write_to_stream(self.setting_groups, out_stream)
         if sys.stdout.isatty():
             print(self.META_INSTRUCTION, file=sys.stderr)
         else:
             print("# oobabot: config.yml output successfully", file=sys.stderr)
 
-    def load(self, args) -> None:
+    def write_to_file(self, filename: str) -> None:
+        oesp.write_to_file(self.setting_groups, filename)
+
+    def _filename_from_args(self, args: typing.List[str]) -> str:
+        """
+        Get the configuration filename from the command line arguments.
+        If none is supplied, return the default.
+        """
+
         # we need to hack this in here because we want to know the filename
         # before we parse the args, so that we can load the config file
-        # first and then have the arguments ovewrite the config file.
+        # first and then have the arguments overwrite the config file.
         config_setting = self.general_settings.get_setting("config")
-        config_filename = config_setting.default
         if args is not None:
             for config_flag in config_setting.cli_args:
                 # find the element after config_flag in args
                 try:
-                    config_filename = args[args.index(config_flag) + 1]
-                    break
-                except ValueError:
+                    return args[args.index(config_flag) + 1]
+                except (ValueError, IndexError):
                     continue
+        return config_setting.default
 
-        argparser = oesp.load(
-            args=args,
+    def load(
+        self,
+        cli_args: typing.List[str],
+        config_file: typing.Optional[str] = None,
+    ) -> None:
+        """
+        Load the config from the command line arguments and config file.
+
+        params:
+            cli_args: list of command line arguments to parse
+            config_file: path to the config file to load
+
+        cli_args is intended to be used when running from a standalone
+        application, while config_file is intended to be used when
+        running from inside another process.
+        """
+
+        if config_file is None:
+            config_file = self._filename_from_args(cli_args)
+
+        self.arg_parser = oesp.load(
+            cli_args=cli_args,
             setting_groups=self.setting_groups,
-            filename=config_filename,
+            config_file=config_file,
         )
 
-        if self.general_settings.get("help"):
-            helpstr = argparser.format_help()
-            print(helpstr)
+    def print_help(self):
+        """
+        Prints CLI usage information to STDOUT.
+        """
+        if self.arg_parser is None:
+            raise ValueError("display_help called before load")
+
+        help_str = self.arg_parser.format_help()
+        print(help_str)
+
+        print(
+            "\n"
+            + _console_wrapped(
+                (
+                    "Additional settings can be set in config.yml.  "
+                    "Use the --generate-config option to print a new "
+                    "copy of this file to STDOUT."
+                )
+            )
+        )
 
+        if "" == self.discord_settings.get("discord_token"):
             print(
                 "\n"
-                + console_wrapped(
+                + _console_wrapped(
                     (
-                        "Additional settings can be set in config.yml.  "
-                        "Use the --generate-config option to print a new "
-                        "copy of this file to STDOUT."
+                        f"Please set the '{self.DISCORD_TOKEN_ENV_VAR}' "
+                        "environment variable to your bot's discord token."
                     )
                 )
             )
-
-            if "" == self.discord_settings.get("discord_token"):
-                print(
-                    "\n"
-                    + console_wrapped(
-                        (
-                            f"Please set the '{self.DISCORD_TOKEN_ENV_VAR}' "
-                            "environment variable to your bot's discord token."
-                        )
-                    )
-                )
-
-            sys.exit(0)
```

### Comparing `oobabot-0.1.7/src/oobabot/templates.py` & `oobabot-0.1.8/src/oobabot/templates.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,118 +1,163 @@
 # -*- coding: utf-8 -*-
+"""
+Templates for text generated by the bot.  There are two types:
+ - templates used to generate prompts for the AI
+ - templates used to generate UI messages for the user
+"""
+
 import enum
 import functools
 import textwrap
 import typing
 
 
 @functools.total_ordering
 class Templates(enum.Enum):
+    """
+    Enumeration of all different templates.
+    """
+
     COMMAND_LOBOTOMIZE_RESPONSE = "command_lobotomize_response"
 
     IMAGE_DETACH = "image_detach"
     IMAGE_CONFIRMATION = "image_confirmation"
     IMAGE_GENERATION_ERROR = "image_generation_error"
     IMAGE_UNAUTHORIZED = "image_unauthorized"
 
+    # prompts to the AI to generate text responses
     PROMPT = "prompt"
     PROMPT_HISTORY_LINE = "prompt_history_line"
     PROMPT_IMAGE_COMING = "prompt_image_coming"
 
+    # prompts to the AI to generate image keywords
+    PROMPT_IMAGE_KEYWORDS = "prompt_image_keywords"
+
     def __str__(self) -> str:
         return self.value
 
     def __lt__(self, other: "Templates") -> bool:
         return str(self.value) < str(other.value)
 
 
 class TemplateToken(str, enum.Enum):
+    """
+    Enumeration of all tokens used in templates.
+    Tokens are variable substitutions into the templates.
+    """
+
     AI_NAME = "AI_NAME"
     PERSONA = "PERSONA"
     IMAGE_COMING = "IMAGE_COMING"
     IMAGE_PROMPT = "IMAGE_PROMPT"
     MESSAGE_HISTORY = "MESSAGE_HISTORY"
     USER_MESSAGE = "USER_MESSAGE"
     USER_NAME = "USER_NAME"
 
     def __str__(self):
         return "{" + self.value + "}"
 
 
 class TemplateStore:
-    # Purpose: store templates and format messages using them
+    """
+    Data object storing all template definitions and default values.
+    """
 
     # mapping of template names to tokens allowed in that template
-    TEMPLATES: typing.Dict[Templates, typing.Tuple[typing.List[TemplateToken], str]] = {
+    #  key: template name
+    #  value: tuple of (list of tokens, description, is_an_ai_prompt)
+    TEMPLATES: typing.Dict[
+        Templates, typing.Tuple[typing.List[TemplateToken], str, bool]
+    ] = {
         Templates.COMMAND_LOBOTOMIZE_RESPONSE: (
             [
                 TemplateToken.AI_NAME,
                 TemplateToken.USER_NAME,
             ],
             "Displayed in Discord after a successful /lobotomize command.  "
             + "Both the discord users and the bot AI will see this message.",
+            False,
         ),
         Templates.PROMPT: (
             [
                 TemplateToken.AI_NAME,
                 TemplateToken.IMAGE_COMING,
                 TemplateToken.MESSAGE_HISTORY,
                 TemplateToken.PERSONA,
             ],
-            "The main prompt sent to Oobabooga to generate a resonse from "
+            "The main prompt sent to Oobabooga to generate a response from "
             + "the bot AI.  The AI's reply to this prompt will be sent to "
             + "discord as the bot's response.",
+            True,
         ),
         Templates.PROMPT_HISTORY_LINE: (
             [
                 TemplateToken.USER_MESSAGE,
                 TemplateToken.USER_NAME,
             ],
             "Part of the AI response-generation prompt, this is used to "
             + "render a single line of chat history.  A list of these, "
             + "one for each past chat message, will become {MESSAGE_HISTORY} "
             + "and inserted into the main prompt",
+            True,
         ),
         Templates.PROMPT_IMAGE_COMING: (
             [
                 TemplateToken.AI_NAME,
             ],
             "Part of the AI response-generation prompt, this is used to "
             + "inform the AI that it is in the process of generating an "
             + "image.",
+            True,
+        ),
+        Templates.PROMPT_IMAGE_KEYWORDS: (
+            [
+                TemplateToken.AI_NAME,
+                TemplateToken.USER_MESSAGE,
+            ],
+            """
+            Sent to Oobabooga, along with the user's image request, to generate
+            image keywords.  The AI's response to this prompt will then be sent
+            to Stable Diffusion to generate an image.
+            """,
+            True,
         ),
         Templates.IMAGE_DETACH: (
             [
                 TemplateToken.IMAGE_PROMPT,
                 TemplateToken.USER_NAME,
             ],
             "Shown in Discord when the user selects to discard an image "
             + "that Stable Diffusion had generated.",
+            False,
         ),
         Templates.IMAGE_CONFIRMATION: (
             [
                 TemplateToken.IMAGE_PROMPT,
                 TemplateToken.USER_NAME,
             ],
             "Shown in Discord when an image is first generated from "
             + "Stable Diffusion.  This should prompt the user to either "
             + "save or discard the image.",
+            False,
         ),
         Templates.IMAGE_GENERATION_ERROR: (
             [
                 TemplateToken.IMAGE_PROMPT,
                 TemplateToken.USER_NAME,
             ],
             "Shown in Discord when the we could not contact Stable Diffusion "
             + "to generate an image.",
+            False,
         ),
         Templates.IMAGE_UNAUTHORIZED: (
             [TemplateToken.USER_NAME],
             "Shown in Discord privately to a user if they try to regenerate "
             "an image that was requested by someone else.",
+            False,
         ),
     }
 
     DEFAULT_TEMPLATES: typing.Dict[Templates, str] = {
         Templates.PROMPT: textwrap.dedent(
             """
             You are in a chat room with multiple participants.
@@ -138,25 +183,41 @@
             """
         ),
         Templates.PROMPT_IMAGE_COMING: textwrap.dedent(
             """
             {AI_NAME}: is currently generating an image, as requested.
             """
         ),
+        Templates.PROMPT_IMAGE_KEYWORDS: textwrap.dedent(
+            """
+            Below is an instruction that describes a task, paired with an input
+            that provides further context. Write a response that appropriately
+            completes the request.
+
+            ### Instruction:
+            The input text asks for an image to be created.  Please create a list
+            of keywords to describe that image.
+
+            ### Input:
+            {USER_MESSAGE}
+
+            ### Response:
+            """
+        ),
         Templates.IMAGE_DETACH: textwrap.dedent(
             """
             {USER_NAME} asked for an image with the prompt:
                 '{IMAGE_PROMPT}'
             ...but couldn't find a suitable one.
             """
         ),
         Templates.IMAGE_CONFIRMATION: textwrap.dedent(
             """
             {USER_NAME}, is this what you wanted?
-            If no choice is made, this message will 💣 self-destuct 💣 in 3 minutes.
+            If no choice is made, this message will 💣 self-destruct 💣 in 3 minutes.
             """
         ),
         Templates.IMAGE_GENERATION_ERROR: textwrap.dedent(
             """
             Something went wrong generating your image.  Sorry about that!
             """
         ),
@@ -170,73 +231,80 @@
             Ummmm... what were we talking about?
             """
         ),
     }
 
     def __init__(self, settings: dict):
         self.templates: typing.Dict[Templates, TemplateMessageFormatter] = {}
-        for template, (tokens, purpose) in self.TEMPLATES.items():
+        for template, (tokens, purpose, is_ai_prompt) in self.TEMPLATES.items():
             template_name = str(template)
             template_fmt = settings[template_name]
             if template_fmt is None:
                 raise ValueError(f"Template {template_name} has no default format")
-            self.add_template(template, template_fmt, tokens, purpose)
+            self.add_template(template, template_fmt, tokens, purpose, is_ai_prompt)
 
     def add_template(
         self,
         template_name: Templates,
         format_str: str,
         allowed_tokens: typing.List[TemplateToken],
         purpose: str,
+        is_ai_prompt: bool,
     ):
         self.templates[template_name] = TemplateMessageFormatter(
             template_name,
             format_str,
             allowed_tokens,
             purpose,
+            is_ai_prompt,
         )
 
     def format(
         self, template_name: Templates, format_args: typing.Dict[TemplateToken, str]
     ) -> str:
         return self.templates[template_name].format(format_args)
 
 
 class TemplateMessageFormatter:
-    # Purpose: format messages using a template string
+    """
+    Validates that templates are safe to run string.format() on, and
+    runs string.format()
+    """
 
     def __init__(
         self,
         template_name: Templates,
         template: str,
         allowed_tokens: typing.List[TemplateToken],
         purpose: str,
+        is_ai_prompt: bool,
     ):
         self._validate_format_string(template_name, template, allowed_tokens)
         self.template_name = template_name
         self.template = template
         self.allowed_tokens = allowed_tokens
         self.purpose = purpose
+        self.is_ai_prompt = is_ai_prompt
 
     def __str__(self):
         return self.template
 
     def format(self, format_args: typing.Dict[TemplateToken, str]) -> str:
         return self.template.format(**format_args)
 
     @staticmethod
     def _validate_format_string(
         template_name: Templates,
         format_str: str,
         allowed_args: typing.List[TemplateToken],
     ):
-        def find_all_ch(s: str, ch: str) -> typing.Generator[int, None, None]:
+        def find_all_ch(string: str, char: str) -> typing.Generator[int, None, None]:
             # find all indices of ch in s
-            for i, ltr in enumerate(s):
-                if ltr == ch:
+            for i, letter in enumerate(string):
+                if letter == char:
                     yield i
 
         # raises if fmt_string contains any args not in allowed_args
         allowed_close_brace_indices: typing.Set[int] = set()
 
         for open_brace_idx in find_all_ch(format_str, "{"):
             for allowed_arg in allowed_args:
```

### Comparing `oobabot-0.1.7/PKG-INFO` & `oobabot-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oobabot
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Discord bot which talks to Large Language Model AIs running on oobabooga's text-generation-webui
 Home-page: https://github.com/chrisrude/oobabot
 License: MIT
 Author: Christopher Rude
 Author-email: chris@rudesoftware.net
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -90,86 +90,102 @@
 
 ~: oobabot --base-url ws://oobabooga-hostname:5005/ --ai-name YourBotsName --persona "You are a cat named YourBotsName"
 ```
 
 You should now be able to run oobabot from wherever pip installed it.
 
 ```none
-usage: oobabot [-h] [-c CONFIG] [--generate-config] [--ai-name AI_NAME] [--persona PERSONA]
-               [--wakewords [WAKEWORDS ...]] [--discord-token DISCORD_TOKEN]
-               [--dont-split-responses] [--history-lines HISTORY_LINES] [--ignore-dms]
-               [--reply-in-thread] [--stream-responses] [--base-url BASE_URL]
-               [--log-all-the-things] [--image-words [IMAGE_WORDS ...]]
+  ³ oobabot  ~/oobabot        oobabot --help         383ms  Tue May 23 18:56:42 2023
+usage: oobabot [-h] [-c CONFIG] [--generate-config] [--invite-url] [--ai-name AI_NAME]
+               [--persona PERSONA] [--wakewords [WAKEWORDS ...]]
+               [--discord-token DISCORD_TOKEN] [--dont-split-responses]
+               [--history-lines HISTORY_LINES] [--ignore-dms] [--reply-in-thread]
+               [--stream-responses] [--base-url BASE_URL] [--log-all-the-things]
+               [--message-regex MESSAGE_REGEX] [--image-words [IMAGE_WORDS ...]]
                [--stable-diffusion-url STABLE_DIFFUSION_URL]
-               [--extra-prompt-text EXTRA_PROMPT_TEXT]
+               [--extra-prompt-text EXTRA_PROMPT_TEXT] [--use-ai-generated-keywords]
 
-oobabot v0.1.7: Discord bot for oobabooga's text-generation-webui
+oobabot v0.1.8: Discord bot for oobabooga's text-generation-webui
 
 General Settings:
 
   -h, --help
   -c CONFIG, --config CONFIG
                         Path to a config file to read settings from. Command line settings
                         will override settings in this file. (default: config.yml)
   --generate-config     If set, oobabot will print its configuration as a .yml file, then
                         exit. Any command-line settings also passed will be reflected in
                         this file. (default: False)
+  --invite-url          Print a URL which can be used to invite the bot to a Discord
+                        server. Requires that the Discord token is set. (default: False)
 
 Persona:
 
   --ai-name AI_NAME     Name the AI will use to refer to itself (default: oobabot)
   --persona PERSONA     This prefix will be added in front of every user-supplied request.
                         This is useful for setting up a 'character' for the bot to play.
                         Alternatively, this can be set with the OOBABOT_PERSONA environment
                         variable. (default: )
   --wakewords [WAKEWORDS ...]
                         One or more words that the bot will listen for. The bot will listen
-                        in all discord channels can access for one of these words to be
+                        in all discord channels it can access for one of these words to be
                         mentioned, then reply to any messages it sees with a matching word.
                         The bot will always reply to @-mentions and direct messages, even
                         if no wakewords are supplied. (default: ['oobabot'])
 
 Discord:
 
   --discord-token DISCORD_TOKEN
                         Token to log into Discord with. For security purposes it's strongly
                         recommended that you set this via the DISCORD_TOKEN environment
                         variable instead, if possible. (default: )
   --dont-split-responses
                         Post the entire response as a single message, rather than splitting
-                        it into seperate messages by sentence. (default: False)
+                        it into separate messages by sentence. (default: False)
   --history-lines HISTORY_LINES
                         Number of lines of chat history the AI will see when generating a
                         response. (default: 7)
   --ignore-dms          If set, the bot will not respond to direct messages. (default:
                         False)
   --reply-in-thread     If set, the bot will generate a thread to respond in if it is not
                         already in one. (default: False)
-  --stream-responses    Stream responses into a single message as they are generated.
-                        (default: False)
+  --stream-responses    FEATURE PREVIEW: Stream responses into a single message as they are
+                        generated. Note: may be janky (default: False)
 
 Oobabooga:
 
   --base-url BASE_URL   Base URL for the oobabooga instance. This should be
                         ws://hostname[:port] for plain websocket connections, or
                         wss://hostname[:port] for websocket connections over TLS. (default:
                         ws://localhost:5005)
   --log-all-the-things  Print all AI input and output to STDOUT. (default: False)
+  --message-regex MESSAGE_REGEX
+                        A regex that will be used to extract message lines from the AI's
+                        output. The first capture group will be used as the message. If
+                        this is not set, the entire output will be used as the message.
+                        (default: )
 
 Stable Diffusion:
 
   --image-words [IMAGE_WORDS ...]
                         When one of these words is used in a message, the bot will generate
-                        an image. (default: ['drawing', 'photo', 'pic', 'picture', 'image',
-                        'sketch'])
+                        an image. (default: ['draw me', 'drawing', 'photo', 'pic',
+                        'picture', 'image', 'sketch'])
   --stable-diffusion-url STABLE_DIFFUSION_URL
                         URL for an AUTOMATIC1111 Stable Diffusion server. (default: )
   --extra-prompt-text EXTRA_PROMPT_TEXT
                         This will be appended to every image generation prompt sent to
                         Stable Diffusion. (default: )
+  --use-ai-generated-keywords
+                        FEATURE PREVIEW: If set, the bot will ask Oobabooga to generate
+                        image keywords from a user's message. It will then pass the
+                        keywords that Oobabooga produces to Stable Diffusion to finally
+                        generate an image. Otherwise, the bot will simply extract keywords
+                        directly from the user's message using a simple regex. (default:
+                        False)
 
 
 Additional settings can be set in config.yml.  Use the --generate-config option to print a
 new copy of this file to STDOUT.
 
 Please set the 'DISCORD_TOKEN' environment variable to your bot's discord token.
 ```
```

