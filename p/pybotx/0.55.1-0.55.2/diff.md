# Comparing `tmp/pybotx-0.55.1.tar.gz` & `tmp/pybotx-0.55.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybotx-0.55.1.tar", max compression
+gzip compressed data, was "pybotx-0.55.2.tar", max compression
```

## Comparing `pybotx-0.55.1.tar` & `pybotx-0.55.2.tar`

### file list

```diff
@@ -1,131 +1,131 @@
--rw-r--r--   0        0        0     6078 2023-04-05 08:02:13.418536 pybotx-0.55.1/LICENSE
--rw-r--r--   0        0        0    21491 2023-04-05 08:02:13.418536 pybotx-0.55.1/README.md
--rw-r--r--   0        0        0     6519 2023-04-05 08:02:13.418536 pybotx-0.55.1/pybotx/__init__.py
--rw-r--r--   0        0        0      976 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/async_buffer.py
--rw-r--r--   0        0        0        0 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/bot/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/bot/api/__init__.py
--rw-r--r--   0        0        0      560 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/bot/api/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/bot/api/responses/__init__.py
--rw-r--r--   0        0        0     1048 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/bot/api/responses/bot_disabled.py
--rw-r--r--   0        0        0      275 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/bot/api/responses/command_accepted.py
--rw-r--r--   0        0        0    54140 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/bot/bot.py
--rw-r--r--   0        0        0     1558 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/bot/bot_accounts_storage.py
--rw-r--r--   0        0        0        0 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/bot/callbacks/__init__.py
--rw-r--r--   0        0        0     3101 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/bot/callbacks/callback_manager.py
--rw-r--r--   0        0        0     2176 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/bot/callbacks/callback_memory_repo.py
--rw-r--r--   0        0        0      983 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/bot/callbacks/callback_repo_proto.py
--rw-r--r--   0        0        0      330 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/bot/contextvars.py
--rw-r--r--   0        0        0      966 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/bot/exceptions.py
--rw-r--r--   0        0        0     2701 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/bot/handler.py
--rw-r--r--   0        0        0    14503 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/bot/handler_collector.py
--rw-r--r--   0        0        0        0 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/bot/middlewares/__init__.py
--rw-r--r--   0        0        0     1749 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/bot/middlewares/exception_middleware.py
--rw-r--r--   0        0        0      293 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/bot/testing.py
--rw-r--r--   0        0        0        0 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/__init__.py
--rw-r--r--   0        0        0     1617 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/authorized_botx_method.py
--rw-r--r--   0        0        0        0 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/bots_api/__init__.py
--rw-r--r--   0        0        0     1235 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/bots_api/get_token.py
--rw-r--r--   0        0        0     6815 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/botx_method.py
--rw-r--r--   0        0        0        0 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/chats_api/__init__.py
--rw-r--r--   0        0        0     2201 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/chats_api/add_admin.py
--rw-r--r--   0        0        0     1443 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/chats_api/add_user.py
--rw-r--r--   0        0        0     2975 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/chats_api/chat_info.py
--rw-r--r--   0        0        0     2177 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/chats_api/create_chat.py
--rw-r--r--   0        0        0     1415 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/chats_api/disable_stealth.py
--rw-r--r--   0        0        0     2004 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/chats_api/list_chats.py
--rw-r--r--   0        0        0     1398 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/chats_api/pin_message.py
--rw-r--r--   0        0        0     1430 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/chats_api/remove_user.py
--rw-r--r--   0        0        0     1699 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/chats_api/set_stealth.py
--rw-r--r--   0        0        0     1354 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/chats_api/unpin_message.py
--rw-r--r--   0        0        0        0 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/events_api/__init__.py
--rw-r--r--   0        0        0     3295 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/events_api/edit_event.py
--rw-r--r--   0        0        0     2324 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/events_api/message_status_event.py
--rw-r--r--   0        0        0     3770 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/events_api/reply_event.py
--rw-r--r--   0        0        0     1019 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/events_api/stop_typing_event.py
--rw-r--r--   0        0        0      955 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/events_api/typing_event.py
--rw-r--r--   0        0        0        0 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/exceptions/__init__.py
--rw-r--r--   0        0        0     1301 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/exceptions/base.py
--rw-r--r--   0        0        0      889 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/exceptions/callbacks.py
--rw-r--r--   0        0        0      424 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/exceptions/chats.py
--rw-r--r--   0        0        0      429 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/exceptions/common.py
--rw-r--r--   0        0        0      130 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/exceptions/event.py
--rw-r--r--   0        0        0      289 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/exceptions/files.py
--rw-r--r--   0        0        0      750 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/exceptions/http.py
--rw-r--r--   0        0        0      378 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/exceptions/notifications.py
--rw-r--r--   0        0        0      293 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/exceptions/users.py
--rw-r--r--   0        0        0        0 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/files_api/__init__.py
--rw-r--r--   0        0        0     2093 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/files_api/download_file.py
--rw-r--r--   0        0        0     2448 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/files_api/upload_file.py
--rw-r--r--   0        0        0      812 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/get_token.py
--rw-r--r--   0        0        0        0 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/notifications_api/__init__.py
--rw-r--r--   0        0        0     5567 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/notifications_api/direct_notification.py
--rw-r--r--   0        0        0     2925 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/notifications_api/internal_bot_notification.py
--rw-r--r--   0        0        0        0 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/openid_api/__init__.py
--rw-r--r--   0        0        0     1245 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/openid_api/refresh_access_token.py
--rw-r--r--   0        0        0        0 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/smartapps_api/__init__.py
--rw-r--r--   0        0        0     2259 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/smartapps_api/smartapp_event.py
--rw-r--r--   0        0        0     1836 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/smartapps_api/smartapp_notification.py
--rw-r--r--   0        0        0     2195 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/smartapps_api/smartapps_list.py
--rw-r--r--   0        0        0     1652 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/smartapps_api/upload_file.py
--rw-r--r--   0        0        0        0 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/stickers_api/__init__.py
--rw-r--r--   0        0        0     2883 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/stickers_api/add_sticker.py
--rw-r--r--   0        0        0     1689 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/stickers_api/create_sticker_pack.py
--rw-r--r--   0        0        0     1506 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/stickers_api/delete_sticker.py
--rw-r--r--   0        0        0     1426 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/stickers_api/delete_sticker_pack.py
--rw-r--r--   0        0        0     1793 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/stickers_api/edit_sticker_pack.py
--rw-r--r--   0        0        0      311 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/stickers_api/exceptions.py
--rw-r--r--   0        0        0     1984 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/stickers_api/get_sticker.py
--rw-r--r--   0        0        0     1397 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/stickers_api/get_sticker_pack.py
--rw-r--r--   0        0        0     2291 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/stickers_api/get_sticker_packs.py
--rw-r--r--   0        0        0     1321 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/stickers_api/sticker_pack.py
--rw-r--r--   0        0        0        0 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/users_api/__init__.py
--rw-r--r--   0        0        0     1231 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/users_api/search_user_by_email.py
--rw-r--r--   0        0        0     1257 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/users_api/search_user_by_huid.py
--rw-r--r--   0        0        0     1330 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/users_api/search_user_by_login.py
--rw-r--r--   0        0        0     1254 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/users_api/search_user_by_other_id.py
--rw-r--r--   0        0        0     2992 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/users_api/update_user_profile.py
--rw-r--r--   0        0        0     1737 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/users_api/user_from_csv.py
--rw-r--r--   0        0        0     1353 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/users_api/user_from_search.py
--rw-r--r--   0        0        0     1659 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/client/users_api/users_as_csv.py
--rw-r--r--   0        0        0      421 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/constants.py
--rw-r--r--   0        0        0      221 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/converters.py
--rw-r--r--   0        0        0      789 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/image_validators.py
--rw-r--r--   0        0        0     1341 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/logger.py
--rw-r--r--   0        0        0      409 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/missing.py
--rw-r--r--   0        0        0        0 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/models/__init__.py
--rw-r--r--   0        0        0     2079 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/models/api_base.py
--rw-r--r--   0        0        0     7256 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/models/async_files.py
--rw-r--r--   0        0        0    13052 2023-04-05 08:02:13.422536 pybotx-0.55.1/pybotx/models/attachments.py
--rw-r--r--   0        0        0     2480 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/base_command.py
--rw-r--r--   0        0        0      187 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/bot_account.py
--rw-r--r--   0        0        0      199 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/bot_sender.py
--rw-r--r--   0        0        0     1625 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/chats.py
--rw-r--r--   0        0        0     1595 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/commands.py
--rw-r--r--   0        0        0     8751 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/enums.py
--rw-r--r--   0        0        0        0 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/message/__init__.py
--rw-r--r--   0        0        0      670 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/message/edit_message.py
--rw-r--r--   0        0        0      524 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/message/forward.py
--rw-r--r--   0        0        0    10253 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/message/incoming_message.py
--rw-r--r--   0        0        0     4325 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/message/markup.py
--rw-r--r--   0        0        0     9106 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/message/mentions.py
--rw-r--r--   0        0        0      270 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/message/message_status.py
--rw-r--r--   0        0        0      882 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/message/outgoing_message.py
--rw-r--r--   0        0        0      696 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/message/reply.py
--rw-r--r--   0        0        0      825 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/message/reply_message.py
--rw-r--r--   0        0        0      538 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/method_callbacks.py
--rw-r--r--   0        0        0      547 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/smartapps.py
--rw-r--r--   0        0        0     2691 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/status.py
--rw-r--r--   0        0        0     1744 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/stickers.py
--rw-r--r--   0        0        0        0 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/system_events/__init__.py
--rw-r--r--   0        0        0     1591 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/system_events/added_to_chat.py
--rw-r--r--   0        0        0     2964 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/system_events/chat_created.py
--rw-r--r--   0        0        0     1267 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/system_events/cts_login.py
--rw-r--r--   0        0        0     1277 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/system_events/cts_logout.py
--rw-r--r--   0        0        0     1746 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/system_events/deleted_from_chat.py
--rw-r--r--   0        0        0     2144 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/system_events/internal_bot_notification.py
--rw-r--r--   0        0        0     1600 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/system_events/left_from_chat.py
--rw-r--r--   0        0        0     3744 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/system_events/smartapp_event.py
--rw-r--r--   0        0        0     1571 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/models/users.py
--rw-r--r--   0        0        0        0 2023-04-05 08:02:13.426536 pybotx-0.55.1/pybotx/py.typed
--rw-r--r--   0        0        0     1247 2023-04-05 08:02:13.426536 pybotx-0.55.1/pyproject.toml
--rw-r--r--   0        0        0    22397 1970-01-01 00:00:00.000000 pybotx-0.55.1/PKG-INFO
+-rw-r--r--   0        0        0     6078 2023-05-24 16:37:18.729078 pybotx-0.55.2/LICENSE
+-rw-r--r--   0        0        0    21491 2023-05-24 16:37:18.729078 pybotx-0.55.2/README.md
+-rw-r--r--   0        0        0     6519 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/__init__.py
+-rw-r--r--   0        0        0      976 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/async_buffer.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/bot/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/bot/api/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/bot/api/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/bot/api/responses/__init__.py
+-rw-r--r--   0        0        0     1048 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/bot/api/responses/bot_disabled.py
+-rw-r--r--   0        0        0      275 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/bot/api/responses/command_accepted.py
+-rw-r--r--   0        0        0    54140 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/bot/bot.py
+-rw-r--r--   0        0        0     1558 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/bot/bot_accounts_storage.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/bot/callbacks/__init__.py
+-rw-r--r--   0        0        0     3101 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/bot/callbacks/callback_manager.py
+-rw-r--r--   0        0        0     2176 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/bot/callbacks/callback_memory_repo.py
+-rw-r--r--   0        0        0      983 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/bot/callbacks/callback_repo_proto.py
+-rw-r--r--   0        0        0      330 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/bot/contextvars.py
+-rw-r--r--   0        0        0      966 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/bot/exceptions.py
+-rw-r--r--   0        0        0     2701 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/bot/handler.py
+-rw-r--r--   0        0        0    14503 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/bot/handler_collector.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/bot/middlewares/__init__.py
+-rw-r--r--   0        0        0     1749 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/bot/middlewares/exception_middleware.py
+-rw-r--r--   0        0        0      293 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/bot/testing.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/__init__.py
+-rw-r--r--   0        0        0     1617 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/authorized_botx_method.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/bots_api/__init__.py
+-rw-r--r--   0        0        0     1235 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/bots_api/get_token.py
+-rw-r--r--   0        0        0     6815 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/botx_method.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/chats_api/__init__.py
+-rw-r--r--   0        0        0     2201 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/chats_api/add_admin.py
+-rw-r--r--   0        0        0     1443 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/chats_api/add_user.py
+-rw-r--r--   0        0        0     2975 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/chats_api/chat_info.py
+-rw-r--r--   0        0        0     2177 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/chats_api/create_chat.py
+-rw-r--r--   0        0        0     1415 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/chats_api/disable_stealth.py
+-rw-r--r--   0        0        0     2004 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/chats_api/list_chats.py
+-rw-r--r--   0        0        0     1398 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/chats_api/pin_message.py
+-rw-r--r--   0        0        0     1430 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/chats_api/remove_user.py
+-rw-r--r--   0        0        0     1699 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/chats_api/set_stealth.py
+-rw-r--r--   0        0        0     1354 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/chats_api/unpin_message.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/events_api/__init__.py
+-rw-r--r--   0        0        0     3295 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/events_api/edit_event.py
+-rw-r--r--   0        0        0     2324 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/events_api/message_status_event.py
+-rw-r--r--   0        0        0     3770 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/events_api/reply_event.py
+-rw-r--r--   0        0        0     1019 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/events_api/stop_typing_event.py
+-rw-r--r--   0        0        0      955 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/events_api/typing_event.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/exceptions/__init__.py
+-rw-r--r--   0        0        0     1301 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/exceptions/base.py
+-rw-r--r--   0        0        0      889 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/exceptions/callbacks.py
+-rw-r--r--   0        0        0      424 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/exceptions/chats.py
+-rw-r--r--   0        0        0      429 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/exceptions/common.py
+-rw-r--r--   0        0        0      130 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/exceptions/event.py
+-rw-r--r--   0        0        0      289 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/exceptions/files.py
+-rw-r--r--   0        0        0      750 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/exceptions/http.py
+-rw-r--r--   0        0        0      378 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/exceptions/notifications.py
+-rw-r--r--   0        0        0      293 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/exceptions/users.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/files_api/__init__.py
+-rw-r--r--   0        0        0     2093 2023-05-24 16:37:18.729078 pybotx-0.55.2/pybotx/client/files_api/download_file.py
+-rw-r--r--   0        0        0     2448 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/files_api/upload_file.py
+-rw-r--r--   0        0        0      812 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/get_token.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/notifications_api/__init__.py
+-rw-r--r--   0        0        0     5567 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/notifications_api/direct_notification.py
+-rw-r--r--   0        0        0     2925 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/notifications_api/internal_bot_notification.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/openid_api/__init__.py
+-rw-r--r--   0        0        0     1245 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/openid_api/refresh_access_token.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/smartapps_api/__init__.py
+-rw-r--r--   0        0        0     2259 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/smartapps_api/smartapp_event.py
+-rw-r--r--   0        0        0     1836 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/smartapps_api/smartapp_notification.py
+-rw-r--r--   0        0        0     2195 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/smartapps_api/smartapps_list.py
+-rw-r--r--   0        0        0     1652 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/smartapps_api/upload_file.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/stickers_api/__init__.py
+-rw-r--r--   0        0        0     2883 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/stickers_api/add_sticker.py
+-rw-r--r--   0        0        0     1689 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/stickers_api/create_sticker_pack.py
+-rw-r--r--   0        0        0     1506 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/stickers_api/delete_sticker.py
+-rw-r--r--   0        0        0     1426 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/stickers_api/delete_sticker_pack.py
+-rw-r--r--   0        0        0     1793 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/stickers_api/edit_sticker_pack.py
+-rw-r--r--   0        0        0      311 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/stickers_api/exceptions.py
+-rw-r--r--   0        0        0     1984 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/stickers_api/get_sticker.py
+-rw-r--r--   0        0        0     1397 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/stickers_api/get_sticker_pack.py
+-rw-r--r--   0        0        0     2291 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/stickers_api/get_sticker_packs.py
+-rw-r--r--   0        0        0     1321 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/stickers_api/sticker_pack.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/users_api/__init__.py
+-rw-r--r--   0        0        0     1231 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/users_api/search_user_by_email.py
+-rw-r--r--   0        0        0     1257 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/users_api/search_user_by_huid.py
+-rw-r--r--   0        0        0     1330 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/users_api/search_user_by_login.py
+-rw-r--r--   0        0        0     1254 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/users_api/search_user_by_other_id.py
+-rw-r--r--   0        0        0     2992 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/users_api/update_user_profile.py
+-rw-r--r--   0        0        0     1737 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/users_api/user_from_csv.py
+-rw-r--r--   0        0        0     1353 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/users_api/user_from_search.py
+-rw-r--r--   0        0        0     1659 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/client/users_api/users_as_csv.py
+-rw-r--r--   0        0        0      421 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/constants.py
+-rw-r--r--   0        0        0      221 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/converters.py
+-rw-r--r--   0        0        0      789 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/image_validators.py
+-rw-r--r--   0        0        0     1341 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/logger.py
+-rw-r--r--   0        0        0      409 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/missing.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/__init__.py
+-rw-r--r--   0        0        0     2079 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/api_base.py
+-rw-r--r--   0        0        0     7256 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/async_files.py
+-rw-r--r--   0        0        0    13052 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/attachments.py
+-rw-r--r--   0        0        0     2480 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/base_command.py
+-rw-r--r--   0        0        0      187 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/bot_account.py
+-rw-r--r--   0        0        0      199 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/bot_sender.py
+-rw-r--r--   0        0        0     1625 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/chats.py
+-rw-r--r--   0        0        0     1595 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/commands.py
+-rw-r--r--   0        0        0     8751 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/enums.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/message/__init__.py
+-rw-r--r--   0        0        0      670 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/message/edit_message.py
+-rw-r--r--   0        0        0      524 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/message/forward.py
+-rw-r--r--   0        0        0    10253 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/message/incoming_message.py
+-rw-r--r--   0        0        0     4325 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/message/markup.py
+-rw-r--r--   0        0        0     9106 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/message/mentions.py
+-rw-r--r--   0        0        0      270 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/message/message_status.py
+-rw-r--r--   0        0        0      882 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/message/outgoing_message.py
+-rw-r--r--   0        0        0      696 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/message/reply.py
+-rw-r--r--   0        0        0      825 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/message/reply_message.py
+-rw-r--r--   0        0        0      538 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/method_callbacks.py
+-rw-r--r--   0        0        0      547 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/smartapps.py
+-rw-r--r--   0        0        0     2691 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/status.py
+-rw-r--r--   0        0        0     1744 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/stickers.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/system_events/__init__.py
+-rw-r--r--   0        0        0     1591 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/system_events/added_to_chat.py
+-rw-r--r--   0        0        0     2964 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/system_events/chat_created.py
+-rw-r--r--   0        0        0     1267 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/system_events/cts_login.py
+-rw-r--r--   0        0        0     1277 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/system_events/cts_logout.py
+-rw-r--r--   0        0        0     1746 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/system_events/deleted_from_chat.py
+-rw-r--r--   0        0        0     2144 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/system_events/internal_bot_notification.py
+-rw-r--r--   0        0        0     1600 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/system_events/left_from_chat.py
+-rw-r--r--   0        0        0     3744 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/system_events/smartapp_event.py
+-rw-r--r--   0        0        0     1571 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/models/users.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:37:18.733078 pybotx-0.55.2/pybotx/py.typed
+-rw-r--r--   0        0        0     1247 2023-05-24 16:37:18.733078 pybotx-0.55.2/pyproject.toml
+-rw-r--r--   0        0        0    22448 1970-01-01 00:00:00.000000 pybotx-0.55.2/PKG-INFO
```

### Comparing `pybotx-0.55.1/LICENSE` & `pybotx-0.55.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/README.md` & `pybotx-0.55.2/README.md`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/__init__.py` & `pybotx-0.55.2/pybotx/__init__.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/async_buffer.py` & `pybotx-0.55.2/pybotx/async_buffer.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/bot/api/exceptions.py` & `pybotx-0.55.2/pybotx/bot/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/bot/api/responses/bot_disabled.py` & `pybotx-0.55.2/pybotx/bot/api/responses/bot_disabled.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/bot/bot.py` & `pybotx-0.55.2/pybotx/bot/bot.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/bot/bot_accounts_storage.py` & `pybotx-0.55.2/pybotx/bot/bot_accounts_storage.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/bot/callbacks/callback_manager.py` & `pybotx-0.55.2/pybotx/bot/callbacks/callback_manager.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/bot/callbacks/callback_memory_repo.py` & `pybotx-0.55.2/pybotx/bot/callbacks/callback_memory_repo.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/bot/callbacks/callback_repo_proto.py` & `pybotx-0.55.2/pybotx/bot/callbacks/callback_repo_proto.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/bot/exceptions.py` & `pybotx-0.55.2/pybotx/bot/exceptions.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/bot/handler.py` & `pybotx-0.55.2/pybotx/bot/handler.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/bot/handler_collector.py` & `pybotx-0.55.2/pybotx/bot/handler_collector.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/bot/middlewares/exception_middleware.py` & `pybotx-0.55.2/pybotx/bot/middlewares/exception_middleware.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/authorized_botx_method.py` & `pybotx-0.55.2/pybotx/client/authorized_botx_method.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/bots_api/get_token.py` & `pybotx-0.55.2/pybotx/client/bots_api/get_token.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/botx_method.py` & `pybotx-0.55.2/pybotx/client/botx_method.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/chats_api/add_admin.py` & `pybotx-0.55.2/pybotx/client/chats_api/add_admin.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/chats_api/add_user.py` & `pybotx-0.55.2/pybotx/client/chats_api/add_user.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/chats_api/chat_info.py` & `pybotx-0.55.2/pybotx/client/chats_api/chat_info.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/chats_api/create_chat.py` & `pybotx-0.55.2/pybotx/client/chats_api/create_chat.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/chats_api/disable_stealth.py` & `pybotx-0.55.2/pybotx/client/chats_api/disable_stealth.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/chats_api/list_chats.py` & `pybotx-0.55.2/pybotx/client/chats_api/list_chats.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/chats_api/pin_message.py` & `pybotx-0.55.2/pybotx/client/chats_api/pin_message.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/chats_api/remove_user.py` & `pybotx-0.55.2/pybotx/client/chats_api/remove_user.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/chats_api/set_stealth.py` & `pybotx-0.55.2/pybotx/client/chats_api/set_stealth.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/chats_api/unpin_message.py` & `pybotx-0.55.2/pybotx/client/chats_api/unpin_message.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/events_api/edit_event.py` & `pybotx-0.55.2/pybotx/client/events_api/edit_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/events_api/message_status_event.py` & `pybotx-0.55.2/pybotx/client/events_api/message_status_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/events_api/reply_event.py` & `pybotx-0.55.2/pybotx/client/events_api/reply_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/events_api/stop_typing_event.py` & `pybotx-0.55.2/pybotx/client/events_api/stop_typing_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/events_api/typing_event.py` & `pybotx-0.55.2/pybotx/client/events_api/typing_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/exceptions/base.py` & `pybotx-0.55.2/pybotx/client/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/exceptions/callbacks.py` & `pybotx-0.55.2/pybotx/client/exceptions/callbacks.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/exceptions/http.py` & `pybotx-0.55.2/pybotx/client/exceptions/http.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/files_api/download_file.py` & `pybotx-0.55.2/pybotx/client/files_api/download_file.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/files_api/upload_file.py` & `pybotx-0.55.2/pybotx/client/files_api/upload_file.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/get_token.py` & `pybotx-0.55.2/pybotx/client/get_token.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/notifications_api/direct_notification.py` & `pybotx-0.55.2/pybotx/client/notifications_api/direct_notification.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/notifications_api/internal_bot_notification.py` & `pybotx-0.55.2/pybotx/client/notifications_api/internal_bot_notification.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/openid_api/refresh_access_token.py` & `pybotx-0.55.2/pybotx/client/openid_api/refresh_access_token.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/smartapps_api/smartapp_event.py` & `pybotx-0.55.2/pybotx/client/smartapps_api/smartapp_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/smartapps_api/smartapp_notification.py` & `pybotx-0.55.2/pybotx/client/smartapps_api/smartapp_notification.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/smartapps_api/smartapps_list.py` & `pybotx-0.55.2/pybotx/client/smartapps_api/smartapps_list.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/smartapps_api/upload_file.py` & `pybotx-0.55.2/pybotx/client/smartapps_api/upload_file.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/stickers_api/add_sticker.py` & `pybotx-0.55.2/pybotx/client/stickers_api/add_sticker.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/stickers_api/create_sticker_pack.py` & `pybotx-0.55.2/pybotx/client/stickers_api/create_sticker_pack.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/stickers_api/delete_sticker.py` & `pybotx-0.55.2/pybotx/client/stickers_api/delete_sticker.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/stickers_api/delete_sticker_pack.py` & `pybotx-0.55.2/pybotx/client/stickers_api/delete_sticker_pack.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/stickers_api/edit_sticker_pack.py` & `pybotx-0.55.2/pybotx/client/stickers_api/edit_sticker_pack.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/stickers_api/get_sticker.py` & `pybotx-0.55.2/pybotx/client/stickers_api/get_sticker.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/stickers_api/get_sticker_pack.py` & `pybotx-0.55.2/pybotx/client/stickers_api/get_sticker_pack.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/stickers_api/get_sticker_packs.py` & `pybotx-0.55.2/pybotx/client/stickers_api/get_sticker_packs.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/stickers_api/sticker_pack.py` & `pybotx-0.55.2/pybotx/client/stickers_api/sticker_pack.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/users_api/search_user_by_email.py` & `pybotx-0.55.2/pybotx/client/users_api/search_user_by_email.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/users_api/search_user_by_huid.py` & `pybotx-0.55.2/pybotx/client/users_api/search_user_by_huid.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/users_api/search_user_by_login.py` & `pybotx-0.55.2/pybotx/client/users_api/search_user_by_login.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/users_api/search_user_by_other_id.py` & `pybotx-0.55.2/pybotx/client/users_api/search_user_by_other_id.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/users_api/update_user_profile.py` & `pybotx-0.55.2/pybotx/client/users_api/update_user_profile.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/users_api/user_from_csv.py` & `pybotx-0.55.2/pybotx/client/users_api/user_from_csv.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/users_api/user_from_search.py` & `pybotx-0.55.2/pybotx/client/users_api/user_from_search.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/client/users_api/users_as_csv.py` & `pybotx-0.55.2/pybotx/client/users_api/users_as_csv.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/image_validators.py` & `pybotx-0.55.2/pybotx/image_validators.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/logger.py` & `pybotx-0.55.2/pybotx/logger.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/api_base.py` & `pybotx-0.55.2/pybotx/models/api_base.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/async_files.py` & `pybotx-0.55.2/pybotx/models/async_files.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/attachments.py` & `pybotx-0.55.2/pybotx/models/attachments.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/base_command.py` & `pybotx-0.55.2/pybotx/models/base_command.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/chats.py` & `pybotx-0.55.2/pybotx/models/chats.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/commands.py` & `pybotx-0.55.2/pybotx/models/commands.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/enums.py` & `pybotx-0.55.2/pybotx/models/enums.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/message/edit_message.py` & `pybotx-0.55.2/pybotx/models/message/edit_message.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/message/forward.py` & `pybotx-0.55.2/pybotx/models/message/forward.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/message/incoming_message.py` & `pybotx-0.55.2/pybotx/models/message/incoming_message.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/message/markup.py` & `pybotx-0.55.2/pybotx/models/message/markup.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/message/mentions.py` & `pybotx-0.55.2/pybotx/models/message/mentions.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/message/outgoing_message.py` & `pybotx-0.55.2/pybotx/models/message/outgoing_message.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/message/reply.py` & `pybotx-0.55.2/pybotx/models/message/reply.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/message/reply_message.py` & `pybotx-0.55.2/pybotx/models/message/reply_message.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/method_callbacks.py` & `pybotx-0.55.2/pybotx/models/method_callbacks.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/smartapps.py` & `pybotx-0.55.2/pybotx/models/smartapps.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/status.py` & `pybotx-0.55.2/pybotx/models/status.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/stickers.py` & `pybotx-0.55.2/pybotx/models/stickers.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/system_events/added_to_chat.py` & `pybotx-0.55.2/pybotx/models/system_events/added_to_chat.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/system_events/chat_created.py` & `pybotx-0.55.2/pybotx/models/system_events/chat_created.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/system_events/cts_login.py` & `pybotx-0.55.2/pybotx/models/system_events/cts_login.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/system_events/cts_logout.py` & `pybotx-0.55.2/pybotx/models/system_events/cts_logout.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/system_events/deleted_from_chat.py` & `pybotx-0.55.2/pybotx/models/system_events/deleted_from_chat.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/system_events/internal_bot_notification.py` & `pybotx-0.55.2/pybotx/models/system_events/internal_bot_notification.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/system_events/left_from_chat.py` & `pybotx-0.55.2/pybotx/models/system_events/left_from_chat.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/system_events/smartapp_event.py` & `pybotx-0.55.2/pybotx/models/system_events/smartapp_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pybotx/models/users.py` & `pybotx-0.55.2/pybotx/models/users.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.1/pyproject.toml` & `pybotx-0.55.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "pybotx"
-version = "0.55.1"
+version = "0.55.2"
 description = "A python library for interacting with eXpress BotX API"
 authors = [
     "Sidnev Nikolay <nsidnev@ccsteam.ru>",
     "Maxim Gorbachev <mgorbachev@ccsteam.ru>",
     "Alexander Samoylenko <alexandr.samojlenko@ccsteam.ru>",
     "Arseniy Zhiltsov <arseniy.zhiltsov@ccsteam.ru>"
 ]
 readme = "README.md"
 documentation = "https://expressapp.github.io/pybotx"
 repository = "https://github.com/ExpressApp/pybotx"
 
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<3.12"
 
 aiofiles = ">=0.7.0,<0.9.0"
 httpx = "0.23.0"
 loguru = ">=0.6.0,<0.7.0"
 mypy-extensions = ">=0.2.0,<0.5.0"
 pydantic = ">=1.6.0,<1.11.0"
 typing-extensions = ">=3.7.4,<5.0.0"
```

### Comparing `pybotx-0.55.1/PKG-INFO` & `pybotx-0.55.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pybotx
-Version: 0.55.1
+Version: 0.55.2
 Summary: A python library for interacting with eXpress BotX API
 Home-page: https://github.com/ExpressApp/pybotx
 Author: Sidnev Nikolay
 Author-email: nsidnev@ccsteam.ru
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiocsv (>=1.2.3,<1.3.0)
 Requires-Dist: aiofiles (>=0.7.0,<0.9.0)
 Requires-Dist: httpx (==0.23.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: mypy-extensions (>=0.2.0,<0.5.0)
 Requires-Dist: pydantic (>=1.6.0,<1.11.0)
 Requires-Dist: typing-extensions (>=3.7.4,<5.0.0)
```

