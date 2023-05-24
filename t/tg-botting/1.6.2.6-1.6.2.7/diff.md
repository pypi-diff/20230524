# Comparing `tmp/tg-botting-1.6.2.6.tar.gz` & `tmp/tg-botting-1.6.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg-botting-1.6.2.6.tar", last modified: Mon May 22 16:44:22 2023, max compression
+gzip compressed data, was "tg-botting-1.6.2.7.tar", last modified: Wed May 24 15:31:24 2023, max compression
```

## Comparing `tg-botting-1.6.2.6.tar` & `tg-botting-1.6.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 16:44:22.235522 tg-botting-1.6.2.6/
--rw-rw-rw-   0        0        0      920 2023-05-22 16:44:22.235522 tg-botting-1.6.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      930 2022-12-06 14:18:03.000000 tg-botting-1.6.2.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 16:44:22.235522 tg-botting-1.6.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1447 2023-05-22 16:05:50.000000 tg-botting-1.6.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:44:22.229538 tg-botting-1.6.2.6/tg_botting/
--rw-rw-rw-   0        0        0    30372 2023-05-22 16:43:44.000000 tg-botting-1.6.2.6/tg_botting/bot.py
--rw-rw-rw-   0        0        0      976 2023-01-11 17:39:26.000000 tg-botting-1.6.2.6/tg_botting/cog.py
--rw-rw-rw-   0        0        0      995 2022-12-13 21:08:58.000000 tg-botting-1.6.2.6/tg_botting/generals.py
--rw-rw-rw-   0        0        0    15742 2023-05-13 19:27:53.000000 tg-botting-1.6.2.6/tg_botting/objects.py
--rw-rw-rw-   0        0        0       38 2022-12-13 21:06:01.000000 tg-botting-1.6.2.6/tg_botting/user_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:44:22.234525 tg-botting-1.6.2.6/tg_botting.egg-info/
--rw-rw-rw-   0        0        0      920 2023-05-22 16:44:22.000000 tg-botting-1.6.2.6/tg_botting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-05-22 16:44:22.000000 tg-botting-1.6.2.6/tg_botting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 16:44:22.000000 tg-botting-1.6.2.6/tg_botting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-22 16:44:22.000000 tg-botting-1.6.2.6/tg_botting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-22 16:44:22.000000 tg-botting-1.6.2.6/tg_botting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 15:31:24.241020 tg-botting-1.6.2.7/
+-rw-rw-rw-   0        0        0      920 2023-05-24 15:31:24.241020 tg-botting-1.6.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      930 2022-12-06 14:18:03.000000 tg-botting-1.6.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-24 15:31:24.242017 tg-botting-1.6.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1447 2023-05-24 15:31:06.000000 tg-botting-1.6.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:31:24.236033 tg-botting-1.6.2.7/tg_botting/
+-rw-rw-rw-   0        0        0    31783 2023-05-22 17:49:59.000000 tg-botting-1.6.2.7/tg_botting/bot.py
+-rw-rw-rw-   0        0        0      976 2023-01-11 17:39:26.000000 tg-botting-1.6.2.7/tg_botting/cog.py
+-rw-rw-rw-   0        0        0      995 2022-12-13 21:08:58.000000 tg-botting-1.6.2.7/tg_botting/generals.py
+-rw-rw-rw-   0        0        0    17322 2023-05-24 15:31:06.000000 tg-botting-1.6.2.7/tg_botting/objects.py
+-rw-rw-rw-   0        0        0       38 2022-12-13 21:06:01.000000 tg-botting-1.6.2.7/tg_botting/user_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:31:24.240023 tg-botting-1.6.2.7/tg_botting.egg-info/
+-rw-rw-rw-   0        0        0      920 2023-05-24 15:31:24.000000 tg-botting-1.6.2.7/tg_botting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-05-24 15:31:24.000000 tg-botting-1.6.2.7/tg_botting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 15:31:24.000000 tg-botting-1.6.2.7/tg_botting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-24 15:31:24.000000 tg-botting-1.6.2.7/tg_botting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-24 15:31:24.000000 tg-botting-1.6.2.7/tg_botting.egg-info/top_level.txt
```

### Comparing `tg-botting-1.6.2.6/PKG-INFO` & `tg-botting-1.6.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 1.6.2.6
+Version: 1.6.2.7
 Summary: python library for easy creation of a telegram bot.
 Home-page: https://github.com/2sweetheart2/tg_botting/tree/master
 Author: Sweetie (Roma Fomkin)
 Author-email: <2004sweetheart2004@gmail.com>
 Keywords: python,bot,tg,tg bot,telegram,telegram bot,botting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `tg-botting-1.6.2.6/README.md` & `tg-botting-1.6.2.7/README.md`

 * *Files identical despite different names*

### Comparing `tg-botting-1.6.2.6/setup.py` & `tg-botting-1.6.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.6.2.6'
+VERSION = '1.6.2.7'
 DESCRIPTION = 'python library for easy creation of a telegram bot.'
 LONG_DESCRIPTION = 'A package that allows you to create bots for telegram using its entire API.'
 
 setup(
     name="tg-botting",
     version=VERSION,
     url='https://github.com/2sweetheart2/tg_botting/tree/master',
```

### Comparing `tg-botting-1.6.2.6/tg_botting/bot.py` & `tg-botting-1.6.2.7/tg_botting/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -475,14 +475,27 @@
                     await _m(command, message)
 
         if command in self.actions_from_cog:
             await command.func(self.actions_from_cog.get(command), message,*args)
         else:
             await command.func(message,*args)
 
+    async def dispatch_command_(self, message, command):
+        if 'on_pre_command' in self.listeners_handle:
+            for _m in self.listeners_handle.get('on_pre_command'):
+                if _m in self.actions_from_cog:
+                    await _m(self.actions_from_cog.get(_m), command, message)
+                else:
+                    await _m(command, message)
+
+        if command in self.actions_from_cog:
+            await command.func(self.actions_from_cog.get(command), message)
+        else:
+            await command.func(message)
+
     async def dispatch_uknow_command(self, message):
         if self.listeners_handle.get("on_unknow_command"):
             for _m in self.listeners_handle.get('on_unknow_command'):
                 if _m in self.ignore_listener_filter or message.chat.id in self.chat_filter:
                     if _m in self.actions_from_cog:
                         await _m(self.actions_from_cog.get(_m), message)
                     else:
@@ -673,30 +686,43 @@
                                 if not isinstance(args[i],val.annotation):
                                     return await self.tupe_error(message,args[i],val.annotation)
                         except IndexError as e:
                             put_args.append(None)
                             continue
                         put_args.append(args[i])
                         ms.pop(0)
+                    message.text = ' '.join(ms)
+                    setattr(message, 'texts', ms)
+                    if len(self.chat_filter) > 0:
+                        if message.chat.id not in self.chat_filter and rs not in self.ignore_filter:
+                            return await self.dispatch_chat_filter_error(message)
+                    try:
+                        await self.dispatch_command(message, rs, put_args)
+                    except CallbackError as e:
+                        await message.reply(e.message)
+                        return await self.dispatch_error_command_invoke(message, rs, e)
+                    except Exception as e:
+                        await self.dispatch_error_command_invoke(message, rs, e)
+                        traceback.print_exc()
                 except:
                     print("ERROR2: ",na,'\n','put_args: ',put_args,'\nargs: ',args,rs)
+                    message.text = ' '.join(ms)
+                    setattr(message, 'texts', ms)
+                    if len(self.chat_filter) > 0:
+                        if message.chat.id not in self.chat_filter and rs not in self.ignore_filter:
+                            return await self.dispatch_chat_filter_error(message)
+                    try:
+                        await self.dispatch_command_(message, rs)
+                    except CallbackError as e:
+                        await message.reply(e.message)
+                        return await self.dispatch_error_command_invoke(message, rs, e)
+                    except Exception as e:
+                        await self.dispatch_error_command_invoke(message, rs, e)
+                        traceback.print_exc()
 
-                message.text = ' '.join(ms)
-                setattr(message, 'texts', ms)
-                if len(self.chat_filter) > 0:
-                    if message.chat.id not in self.chat_filter and rs not in self.ignore_filter:
-                        return await self.dispatch_chat_filter_error(message)
-                try:
-                    await self.dispatch_command(message, rs,put_args)
-                except CallbackError as e:
-                    await message.reply(e.message)
-                    return await self.dispatch_error_command_invoke(message, rs, e)
-                except Exception as e:
-                    await self.dispatch_error_command_invoke(message, rs, e)
-                    traceback.print_exc()
             else:
                 await self.dispatch_uknow_command(message)
         await self.dispatch_message(message)
         if message.successful_payment:
             await self.dispatch_payment(message)
         elif message.photo:
             await self.dispatch_photo(message)
```

### Comparing `tg-botting-1.6.2.6/tg_botting/cog.py` & `tg-botting-1.6.2.7/tg_botting/cog.py`

 * *Files identical despite different names*

### Comparing `tg-botting-1.6.2.6/tg_botting/generals.py` & `tg-botting-1.6.2.7/tg_botting/generals.py`

 * *Files identical despite different names*

### Comparing `tg-botting-1.6.2.6/tg_botting/objects.py` & `tg-botting-1.6.2.7/tg_botting/objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,41 +83,71 @@
             'one_time_keyboard': self.one_time,
             'selective': self.selective
         }
         return dic1
 
 
 class ChatPermission:
-    def __init__(self, can_send_messages=True, can_send_media_messages=True, can_send_polls=True,
+    def __init__(self, can_send_messages=True, can_send_media_messages=True, can_send_audios=True,
+                 can_send_documents=True,
+                 can_send_polls=True, can_send_photos=True, can_send_videos=True,
+                 can_send_video_notes=True, can_send_voice_notes=True,
                  can_send_other_messages=True, can_add_web_page_previews=True, can_change_info=False,
                  can_invite_users=False, can_pin_messages=False, can_manage_topics=False):
         self.can_send_messages = can_send_messages
         self.can_send_media_messages = can_send_media_messages
         self.can_send_polls = can_send_polls
+        self.can_send_photos = can_send_photos
+        self.can_send_voice_notes = can_send_voice_notes
+        self.can_send_video_notes = can_send_video_notes
+        self.can_send_videos = can_send_videos
+        self.can_send_documents = can_send_documents
+        self.can_send_audios = can_send_audios
         self.can_send_other_messages = can_send_other_messages
         self.can_add_web_page_previews = can_add_web_page_previews
         self.can_change_info = can_change_info
         self.can_invite_users = can_invite_users
         self.can_pin_messages = can_pin_messages
         self.can_manage_topics = can_manage_topics
 
     @property
     def to_dict(self):
         return {
             'can_send_messages': self.can_send_messages,
             'can_send_media_messages': self.can_send_media_messages,
+            'can_send_audios': self.can_send_audios,
+            'can_send_documents': self.can_send_documents,
+            'can_send_photos': self.can_send_photos,
+            'can_send_videos': self.can_send_videos,
+            'can_send_video_notes': self.can_send_video_notes,
+            'can_send_voice_notes': self.can_send_voice_notes,
             'can_send_polls': self.can_send_polls,
             'can_send_other_messages': self.can_send_other_messages,
             'can_add_web_page_previews': self.can_add_web_page_previews,
             'can_change_info': self.can_change_info,
             'can_invite_users': self.can_invite_users,
             'can_pin_messages': self.can_pin_messages,
             'can_manage_topics': self.can_manage_topics
         }
 
+    @classmethod
+    def create_from_payload(cls, payload):
+        d = ['can_send_messages', 'can_send_media_messages', 'can_send_audios', 'can_send_documents', 'can_send_photos',
+             'can_send_videos', 'can_send_video_notes', 'can_send_voice_notes', 'can_send_polls',
+             'can_send_other_messages',
+             'can_add_web_page_previews', 'can_change_info', 'can_invite_users', 'can_pin_messages',
+             'can_manage_topics']
+        p = []
+        for k, v in payload.items():
+            if k not in d:
+                p.append(False)
+            else:
+                p.append(v)
+        return cls(*p)
+
 
 class PromotePermission:
     def __init__(self, is_anonymous=False, can_manage_chat=False, can_post_messages=False, can_edit_messages=False,
                  can_delete_messages=False, can_manage_video_chats=False, can_restrict_members=False,
                  can_promote_members=False,
                  can_change_info=False, can_invite_users=False, can_pin_messages=False, can_manage_topics=False):
         self.is_anonymous = is_anonymous
@@ -195,16 +225,14 @@
 
     async def get_photos(self):
         if not self.photo:
             return None
         rs = (await self.bot.get_file(self.photo.file_id)).get('result')
         return rs.get('file_id')
 
-
-
     def get_event_user(self):
         if self.new_chat_member or self.new_chat_participant:
             return self.new_chat_member or self.new_chat_participant
         elif self.left_chat_participant or self.left_chat_member:
             return self.left_chat_participant or self.left_chat_member
         else:
             return self.user
@@ -274,16 +302,16 @@
             data['caption'] = text
             data.pop('chat_id')
             return await self.send_photo(photo, **data)
         text = str(text)
         if text is not None:
             if len(text) > 4096:
                 datas = []
-                for i in range(0,(len(text)//4094)+1):
-                    data['text'] = text[i*4096:(i+1)*4094]
+                for i in range(0, (len(text) // 4094) + 1):
+                    data['text'] = text[i * 4096:(i + 1) * 4094]
                     rs = await self.bot.tg_request('sendMessage', True, **data)
                     datas.append(rs)
                 return datas
         data['text'] = text
         rs = await self.bot.tg_request('sendMessage', True, **data)
         return rs.get('ok')
 
@@ -381,16 +409,18 @@
         self.id = payload.get('id')
         self.type = payload.get('type')
         if type == 'private':
             self.chatObj = UserChat(payload)
         elif type == 'group':
             self.chatObj = GroupChat(payload)
         self.invite_link = payload.get('invite_link') if 'invite_link' in payload else None
-        self.permissions = ChatPermission(payload.get('permissions')) if 'permissions' in payload else None
-        self.join_to_send_messages = payload.get('join_to_send_messages') if 'join_to_send_messages' in payload else False
+        self.permissions = ChatPermission.create_from_payload(
+            payload.get('permissions')) if 'permissions' in payload else ChatPermission()
+        self.join_to_send_messages = payload.get(
+            'join_to_send_messages') if 'join_to_send_messages' in payload else False
 
 
 class ChatActions(Enum):
     TYPING = "typing"
     UPLOAD_PHOTO = 'upload_photo'
     RECORD_VIDEO = 'record_video'
     UPLOAD_VIDEO = 'upload_video'
```

### Comparing `tg-botting-1.6.2.6/tg_botting.egg-info/PKG-INFO` & `tg-botting-1.6.2.7/tg_botting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 1.6.2.6
+Version: 1.6.2.7
 Summary: python library for easy creation of a telegram bot.
 Home-page: https://github.com/2sweetheart2/tg_botting/tree/master
 Author: Sweetie (Roma Fomkin)
 Author-email: <2004sweetheart2004@gmail.com>
 Keywords: python,bot,tg,tg bot,telegram,telegram bot,botting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

