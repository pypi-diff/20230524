# Comparing `tmp/whatsapp-api-client-python-0.0.34.tar.gz` & `tmp/whatsapp-api-client-python-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-api-client-python-0.0.34.tar", last modified: Mon Mar 27 06:38:55 2023, max compression
+gzip compressed data, was "whatsapp-api-client-python-0.0.35.tar", last modified: Wed May 24 07:21:08 2023, max compression
```

## Comparing `whatsapp-api-client-python-0.0.34.tar` & `whatsapp-api-client-python-0.0.35.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:38:55.808400 whatsapp-api-client-python-0.0.34/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-27 06:38:35.000000 whatsapp-api-client-python-0.0.34/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24966 2023-03-27 06:38:55.808400 whatsapp-api-client-python-0.0.34/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24417 2023-03-27 06:38:35.000000 whatsapp-api-client-python-0.0.34/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 06:38:55.808400 whatsapp-api-client-python-0.0.34/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-03-27 06:38:35.000000 whatsapp-api-client-python-0.0.34/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:38:55.804400 whatsapp-api-client-python-0.0.34/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-03-27 06:38:35.000000 whatsapp-api-client-python-0.0.34/tests/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:38:55.808400 whatsapp-api-client-python-0.0.34/whatsapp_api_client_python/
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-03-27 06:38:35.000000 whatsapp-api-client-python-0.0.34/whatsapp_api_client_python/API.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 06:38:35.000000 whatsapp-api-client-python-0.0.34/whatsapp_api_client_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-27 06:38:35.000000 whatsapp-api-client-python-0.0.34/whatsapp_api_client_python/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:38:55.808400 whatsapp-api-client-python-0.0.34/whatsapp_api_client_python/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 06:38:35.000000 whatsapp-api-client-python-0.0.34/whatsapp_api_client_python/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-03-27 06:38:35.000000 whatsapp-api-client-python-0.0.34/whatsapp_api_client_python/tools/account.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-27 06:38:35.000000 whatsapp-api-client-python-0.0.34/whatsapp_api_client_python/tools/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-03-27 06:38:35.000000 whatsapp-api-client-python-0.0.34/whatsapp_api_client_python/tools/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-03-27 06:38:35.000000 whatsapp-api-client-python-0.0.34/whatsapp_api_client_python/tools/journals.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-27 06:38:35.000000 whatsapp-api-client-python-0.0.34/whatsapp_api_client_python/tools/marking.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-03-27 06:38:35.000000 whatsapp-api-client-python-0.0.34/whatsapp_api_client_python/tools/queues.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-03-27 06:38:35.000000 whatsapp-api-client-python-0.0.34/whatsapp_api_client_python/tools/receiving.py
--rw-r--r--   0 runner    (1001) docker     (123)    13455 2023-03-27 06:38:35.000000 whatsapp-api-client-python-0.0.34/whatsapp_api_client_python/tools/sending.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-03-27 06:38:35.000000 whatsapp-api-client-python-0.0.34/whatsapp_api_client_python/tools/serviceMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-03-27 06:38:35.000000 whatsapp-api-client-python-0.0.34/whatsapp_api_client_python/tools/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:38:55.808400 whatsapp-api-client-python-0.0.34/whatsapp_api_client_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24966 2023-03-27 06:38:55.000000 whatsapp-api-client-python-0.0.34/whatsapp_api_client_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-27 06:38:55.000000 whatsapp-api-client-python-0.0.34/whatsapp_api_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 06:38:55.000000 whatsapp-api-client-python-0.0.34/whatsapp_api_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-27 06:38:55.000000 whatsapp-api-client-python-0.0.34/whatsapp_api_client_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-27 06:38:55.000000 whatsapp-api-client-python-0.0.34/whatsapp_api_client_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 07:21:08.785300 whatsapp-api-client-python-0.0.35/
+-rw-rw-rw-   0        0        0    18130 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/LICENSE
+-rw-rw-rw-   0        0        0    20699 2023-05-24 07:21:08.784297 whatsapp-api-client-python-0.0.35/PKG-INFO
+-rw-rw-rw-   0        0        0    19661 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-24 07:21:08.785300 whatsapp-api-client-python-0.0.35/setup.cfg
+-rw-rw-rw-   0        0        0     1410 2023-05-24 07:14:52.000000 whatsapp-api-client-python-0.0.35/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:21:08.768264 whatsapp-api-client-python-0.0.35/tests/
+-rw-rw-rw-   0        0        0      960 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:21:08.770323 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/
+-rw-rw-rw-   0        0        0     2818 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/API.py
+-rw-rw-rw-   0        0        0        0 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/__init__.py
+-rw-rw-rw-   0        0        0      336 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/response.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:21:08.783295 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/
+-rw-rw-rw-   0        0        0        0 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/__init__.py
+-rw-rw-rw-   0        0        0     2814 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/account.py
+-rw-rw-rw-   0        0        0      517 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/device.py
+-rw-rw-rw-   0        0        0     4680 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/groups.py
+-rw-rw-rw-   0        0        0     2174 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/journals.py
+-rw-rw-rw-   0        0        0      598 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/marking.py
+-rw-rw-rw-   0        0        0      865 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/queues.py
+-rw-rw-rw-   0        0        0     3354 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/receiving.py
+-rw-rw-rw-   0        0        0     7412 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/sending.py
+-rw-rw-rw-   0        0        0     4254 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/serviceMethods.py
+-rw-rw-rw-   0        0        0     1265 2023-05-20 05:19:15.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/webhooks.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:21:08.775274 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python.egg-info/
+-rw-rw-rw-   0        0        0    20699 2023-05-24 07:21:08.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      899 2023-05-24 07:21:08.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 07:21:08.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-24 07:21:08.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-05-24 07:21:08.000000 whatsapp-api-client-python-0.0.35/whatsapp_api_client_python.egg-info/top_level.txt
```

### Comparing `whatsapp-api-client-python-0.0.34/PKG-INFO` & `whatsapp-api-client-python-0.0.35/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,199 +1,216 @@
-Metadata-Version: 2.1
-Name: whatsapp-api-client-python
-Version: 0.0.34
-Summary: This library helps you easily create a python '        'application to connect the WhatsApp API using service green-api.com
-Home-page: https://github.com/green-api/whatsapp-api-client-python
-Author: Ivan Sadovy
-Author-email: sadiv@bk.ru
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-﻿# whatsapp-api-client-python
-
-[![Python application](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-app.yml/badge.svg)](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-app.yml)
-[![Upload Python Package](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-publish.yml/badge.svg)](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-publish.yml)
-
-- [Документация на русском языке](README_RUS.md)
-
-Python library for intagration with WhatsAPP messanger via API of [green-api.com](https://green-api.com) service. To use the library you have to get a registration token and an account id in the [personal area](https://console.green-api.com). There is a free developer account tariff plan.
-
-## API
-
-You can find REST API documentation by [url](https://green-api.com/docs/api/). The library is a wrapper for REST API, so the documentation at the above url applies to the library as well.
-
-## Installation
-
-```shell
-pip install whatsapp-api-client-python
-```
-
-## Import 
-
-```
-from whatsapp_api_client_python import API
-```
-## Authorization
-
-To send a message or to exacute some other Green-API method, you have to have the WhatsApp account in the phone application to be authorized. To authorize your account please go to the [personal area](https://console.green-api.com) and scan a QR-code using the WhatsApp application.
-
-## Examples
-
-### How to initialize an object
-
-```python
-greenAPI = API.GreenApi(ID_INSTANCE, API_TOKEN_INSTANCE)
-```
-
-### Sending a text message to a WhatsApp number
-
-```python
-result = greenAPI.sending.sendMessage('79001234567@g.us', 'Message text')
-```
-
-Example url: [sendTextMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendTextMessage.py)
-
-Please note that keys can be obtained from environment variables:
-```python
-from os import environ
-
-ID_INSTANCE = environ['ID_INSTANCE']
-API_TOKEN_INSTANCE = environ['API_TOKEN_INSTANCE']
-```
-
-### Sending an image via URL
-
-```python
-result = greenAPI.sending.sendFileByUrl('120363025955348359@g.us', 
-        'https://www.google.ru/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png', 
-        'googlelogo_color_272x92dp.png', 'Google logo')
-```
-
-Example url: [sendPictureByLink.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByLink.py)
-
-### Sending an image by uploading from the disk
-
-```python
-result = greenAPI.sending.sendFileByUpload('120363025955348359@g.us', 
-        'C:\Games\PicFromDisk.png', 
-        'PicFromDisk.png', 'Picture from disk')
-```
-
-Example url: [sendPictureByUpload.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByUpload.py)
-
-### Group creation and sending a message to the group
-
-```python
-chatIds = [
-    "79001234567@c.us"
-]
-resultCreate = greenAPI.groups.createGroup('GroupName', 
-    chatIds)
-
-if resultCreate.code == 200:
-    resultSend = greenAPI.sending.sendMessage(resultCreate.data['chatId'], 
-        'Message text')
-```
-
-IMPORTANT: If one tries to create a group with a non-existent number, WhatsApp 
-may block the sender's number. The number in the example is non-existent.
-
-Example url: [createGroupAndSendMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/createGroupAndSendMessage.py)
-
-### Receive incoming messages by HTTP API
-
-The general concept of receiving data in the Green API is described [here](https://green-api.com/en/docs/api/receiving/)
-To start receiving messages by the HTTP API you need to execute the library method:
-
-```python
-greenAPI.webhooks.startReceivingNotifications(onEvent)
-```
-
-onEvent - your method which should contain parameters:
-Parameter | Description
------ | -----
-typewebhook | received message type (string)
-body | message body (json)
-
-Message body types and formats [here](https://green-api.com/en/docs/api/receiving/notifications-format/)
-
-This method will be called when an incoming message is received. Next, process messages according to the business logic of your system.
-
-## Examples list
-
-Description |  Module
------ | ----- 
-Example of sending text | [sendTextMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendTextMessage.py)
-Example of sending a picture by URL | [sendPictureByLink.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByLink.py)
-Example of sending a picture by uploading from the disk | [sendPictureByUpload.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByUpload.py)
-Example of a group creation and sending a message to the group | [createGroupAndSendMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/createGroupAndSendMessage.py)
-Example of incoming webhooks receiving | [receiveNotification.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/receiveNotification.py)
-
-
-## The full list of the library methods
-
-| Method                                 | Description                                                                                                                                                                                         | Documentation                                                                                                                            |
-|----------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------|
-| `account.getSettings`                  | The method is aimed for getting the current settings of the account                                                                                                                                 | [GetSettings.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/GetSettings.md)                                       |
-| `account.getStateInstance`             | The method is aimed for getting the account state                                                                                                                                                   | [GetStateInstance.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/GetStateInstance.md)                             |
-| `account.getStatusInstance`            | The method is aimed for getting the status of the account instance socket connection with WhatsApp                                                                                                  | [GetStatusInstance.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/GetStatusInstance.md)                           |
-| `account.logout`                       | The method is aimed for logging out an account                                                                                                                                                      | [Logout.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/Logout.md)                                                 |
-| `account.qr`                           | The method is aimed for getting QR code                                                                                                                                                             | [QR.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/QR.md)                                                         |
-| `account.reboot`                       | The method is aimed for rebooting an account                                                                                                                                                        | [Reboot.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/Reboot.md)                                                 |
-| `account.setProfilePicture`            | The method is aimed for setting an account picture                                                                                                                                                  | [SetProfilePicture.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/SetProfilePicture.md)                           |
-| `account.setSettings`                  | The method is aimed for setting an account settings                                                                                                                                                 | [SetSettings.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/SetSettings.md)                                       |
-| `account.setSystemProxy`               | The method is aimed for setting a system proxy. Use the method when you need to reset custom proxy settings to system ones                                                                          | [SetSystemProxy.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/SetSystemProxy.md)                                 |
-| `groups.addGroupParticipant`           | Метод добавляет участника в групповой чат                                                                                                                                                           | [AddGroupParticipant.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/AddGroupParticipant.md)                        |
-| `groups.createGroup`                   | The method adds a participant to a group chat. IMPORTANT: If one tries to create a group with a non-existent number, WhatsApp may block the sender's number.                                        | [CreateGroup.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/CreateGroup.md)                                        |
-| `groups.getGroupData`                  | The method gets group chat data                                                                                                                                                                     | [GetGroupData.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/GetGroupData.md)                                     |
-| `groups.leaveGroup`                    | The method makes the current account user leave the group chat                                                                                                                                      | [LeaveGroup.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/LeaveGroup.md)                                          |
-| `groups.removeAdmin`                   | he method removes a participant from group chat administration rights                                                                                                                               | [RemoveAdmin.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/RemoveAdmin.md)                                        |
-| `groups.removeGroupParticipant`        | The method removes a participant from a group chat                                                                                                                                                  | [RemoveGroupParticipant.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/RemoveGroupParticipant.md)                  |
-| `groups.setGroupAdmin`                 | The method sets a group chat participant as an administrator                                                                                                                                        | [SetGroupAdmin.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/SetGroupAdmin.md)                                    |
-| `groups.setGroupPicture`               | The method sets a group picture                                                                                                                                                                     | [SetGroupPicture.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/SetGroupPicture.md)                                |
-| `groups.updateGroupName`               | The method changes a group chat name                                                                                                                                                                | [UpdateGroupName.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/UpdateGroupName.md)                                |
-| `journals.getChatHistory`              | The method returns the chat message history                                                                                                                                                         | [GetChatHistory.md](https://github.com/green-api/docs/blob/master/ru/docs/api/journals/GetChatHistory.md)                                |
-| `journals.lastIncomingMessages`        | The method returns the last incoming messages of the account. In the default mode the incoming messages for 24 hours are returned                                                                   | [GetChatHistory.md](https://github.com/green-api/docs/blob/master/ru/docs/api/journals/LastIncomingMessages.md)                          |
-| `journals.lastOutgoingMessages`        | The method returns the last outgoing messages of the account. In the default mode the last messages for 24 hours are returned                                                                       | [LastOutgoingMessages.md](https://github.com/green-api/docs/blob/master/ru/docs/api/journals/LastOutgoingMessages.md)                    |
-| `marking.readChat`                     | The method is aimed for marking messages in a chat as read. Either all messages or a specified message in a chat can be marked as read                                                              | [ReadChat.md](https://github.com/green-api/docs/blob/master/ru/docs/api/marks/ReadChat.md)                                               |
-| `device.getDeviceInfo`                 | The method is aimed for getting information about the device (phone) running WhatsApp Business application                                                                                          | [GetDeviceInfo.md](https://github.com/green-api/docs/blob/master/ru/docs/api/phone/GetDeviceInfo.md)                                     |
-| `queues.clearMessagesQueue`            | The method is aimed for clearing the queue of messages to be sent                                                                                                                                   | [ClearMessagesQueue.md](https://github.com/green-api/docs/blob/master/ru/docs/api/queues/ClearMessagesQueue.md)                          |
-| `queues.showMessagesQueue`             | The method is aimed for getting a list of messages in the queue to be sent                                                                                                                          | [ShowMessagesQueue.md](https://github.com/green-api/docs/blob/master/ru/docs/api/queues/ShowMessagesQueue.md)                            |
-| `receiving.deleteNotification`         | The method is aimed for deleting an incoming notification from the notification queue                                                                                                               | [DeleteNotification.md](https://github.com/green-api/docs/blob/master/ru/docs/api/receiving/technology-http-api/DeleteNotification.md)   |
-| `receiving.receiveNotification`        | The method is aimed for receiving one incoming notification from the notifications queue                                                                                                            | [ReceiveNotification.md](https://github.com/green-api/docs/blob/master/ru/docs/api/receiving/technology-http-api/ReceiveNotification.md) |
-| `sending.sendButtons`                  | The method is aimed for sending a button message to a personal or a group chat                                                                                                                      | [SendButtons.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendButtons.md)                                       |
-| `sending.sendContact`                  | The method is aimed for sending a contact message                                                                                                                                                   | [SendContact.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendContact.md)                                       |
-| `sending.sendFileByUpload`             | The method is aimed for sending a file uploaded by form                                                                                                                                             | [SendFileByUpload.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendFileByUpload.md)                             |
-| `sending.sendFileByUrl`                | The method is aimed for sending a file uploaded by Url                                                                                                                                              | [SendFileByUrl.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendFileByUrl.md)                                   |
-| `sending.sendLink`                     | The method is aimed for sending a message with a link, by which an image preview, title and description will be added                                                                               | [SendLink.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendLink.md)                                             |
-| `sending.sendListMessage`              | The method is aimed for sending a message with a select button from a list of values to a personal or a group chat                                                                                  | [SendListMessage.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendListMessage.md)                               |
-| `sending.sendLocation`                 | The method is aimed for sending a location message                                                                                                                                                  | [SendLocation.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendLocation.md)                                     |
-| `sending.sendMessage`                  | The method is aimed for sending a text message to a personal or a group chat                                                                                                                        | [SendMessage.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendMessage.md)                                       |
-| `sending.sendTemplateButtons`          | The method is aimed for sending a message with template list interactive buttons to a personal or a group chat                                                                                      | [SendTemplateButtons.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendTemplateButtons.md)                       |
-| `sending.forwardMessages`              | The method is intended for forwarding messages to a personal or group chat                                                                                                                          | [ForwardMessages.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/ForwardMessages.md)                               |
-| `serviceMethods.checkWhatsapp`         | The method checks WhatsApp account availability on a phone number                                                                                                                                   | [CheckWhatsapp.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/CheckWhatsapp.md)                                   |
-| `serviceMethods.getAvatar`             | The method returns a user or a group chat avatar                                                                                                                                                    | [GetAvatar.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/GetAvatar.md)                                           |
-| `serviceMethods.getContactInfo`        | The method is aimed for getting information on a contact                                                                                                                                            | [GetContactInfo.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/GetContactInfo.md)                                 |
-| `serviceMethods.getContacts`           | The method is aimed for getting a list of the current account contacts                                                                                                                              | [GetContacts.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/GetContacts.md)                                       |
-| `serviceMethods.setDisappearingChat`   | The method is aimed for changing settings of disappearing messages in chats. The standard settings of the application are to be used: 0 (off), 86400 (24 hours), 604800 (7 days), 7776000 (90 days) | [SetDisappearingChat.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/SetDisappearingChat.md)                       |
-| `serviceMethods.archiveChat`           | The method archives a chat. One can archive chats that have at least one incoming message                                                                                                           | [ArchiveChat.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/ArchiveChat.md)                                       |
-| `serviceMethods.deleteMessage`         | The method deletes a message from a chat                                                                                                                                                            | [DeleteMessage.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/deleteMessage.md)                                   |
-| `serviceMethods.unarchiveChat`         | The method unarchives a chat                                                                                                                                                                        | [UnarchiveChat.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/UnarchiveChat.md)                                   |
-| `serviceMethods.setDisappearingChat`   | The method is aimed for changing settings of disappearing messages in chats                                                                                                                         | [SetDisappearingChat.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/SetDisappearingChat.md)                       |
-| `webhooks.startReceivingNotifications` | The method is aimed for starting to receive webhooks                                                                                                                                                | <library method>                                                                                                                         |
-| `webhooks.stopReceivingNotifications`  | The method is aimed for stopping to receive webhooks                                                                                                                                                | <library method>                                                                                                                         |
-
-## Service methods documentation
-
-[https://green-api.com/en/docs/api/](https://green-api.com/en/docs/api/)
-
-## External products
-
-* [requests](https://requests.readthedocs.io) - for http requests
-
-## License
-
-Licensed under MIT terms. Please see file [LICENSE](LICENSE)
+Metadata-Version: 2.1
+Name: whatsapp-api-client-python
+Version: 0.0.35
+Summary: This library helps you easily create a Python application with WhatsApp API.
+Home-page: https://github.com/green-api/whatsapp-api-client-python
+Author: GREEN API
+Author-email: support@green-api.com
+License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+﻿# whatsapp-api-client-python
+
+[![Python application](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-app.yml/badge.svg)](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-app.yml)
+[![Upload Python Package](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-publish.yml/badge.svg)](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-publish.yml)
+
+- [Документация на русском языке](README_RUS.md)
+
+Python library for intagration with WhatsAPP messanger via API of [green-api.com](https://green-api.com/en/) service. To use the library you have to get a registration token and an account id in the [personal area](https://console.green-api.com). There is a free developer account tariff plan.
+
+## API
+
+You can find REST API documentation by [url](https://green-api.com/en/docs/api/). The library is a wrapper for REST API, so the documentation at the above url applies to the library as well.
+
+## Installation
+
+```shell
+pip install whatsapp-api-client-python
+```
+
+## Import 
+
+```
+from whatsapp_api_client_python import API
+```
+## Authorization
+
+To send a message or to exacute some other Green-API method, you have to have the WhatsApp account in the phone application to be authorized. To authorize your account please go to the [personal area](https://console.green-api.com) and scan a QR-code using the WhatsApp application.
+
+## Examples
+
+### How to initialize an object
+
+```python
+greenAPI = API.GreenApi(ID_INSTANCE, API_TOKEN_INSTANCE)
+```
+
+### Sending a text message to a WhatsApp number
+
+```python
+result = greenAPI.sending.sendMessage('79001234567@g.us', 'Message text')
+```
+
+Example url: [sendTextMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendTextMessage.py)
+
+Please note that keys can be obtained from environment variables:
+```python
+from os import environ
+
+ID_INSTANCE = environ['ID_INSTANCE']
+API_TOKEN_INSTANCE = environ['API_TOKEN_INSTANCE']
+```
+
+### Sending an image via URL
+
+```python
+result = greenAPI.sending.sendFileByUrl('120363025955348359@g.us', 
+        'https://www.google.ru/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png', 
+        'googlelogo_color_272x92dp.png', 'Google logo')
+```
+
+Example url: [sendPictureByLink.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByLink.py)
+
+### Sending an image by uploading from the disk
+
+```python
+result = greenAPI.sending.sendFileByUpload('120363025955348359@g.us', 
+        'C:\Games\PicFromDisk.png', 
+        'PicFromDisk.png', 'Picture from disk')
+```
+
+Example url: [sendPictureByUpload.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByUpload.py)
+
+### Group creation and sending a message to the group
+
+```python
+chatIds = [
+    "79001234567@c.us"
+]
+resultCreate = greenAPI.groups.createGroup('GroupName', 
+    chatIds)
+
+if resultCreate.code == 200:
+    resultSend = greenAPI.sending.sendMessage(resultCreate.data['chatId'], 
+        'Message text')
+```
+
+IMPORTANT: If one tries to create a group with a non-existent number, WhatsApp 
+may block the sender's number. The number in the example is non-existent.
+
+Example url: [createGroupAndSendMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/createGroupAndSendMessage.py)
+
+### Receive incoming messages by HTTP API
+
+The general concept of receiving data in the Green API is described [here](https://green-api.com/en/docs/api/receiving/)
+To start receiving messages by the HTTP API you need to execute the library method:
+
+```python
+greenAPI.webhooks.startReceivingNotifications(onEvent)
+```
+
+onEvent - your method which should contain parameters:
+Parameter | Description
+----- | -----
+typewebhook | received message type (string)
+body | message body (json)
+
+Message body types and formats [here](https://green-api.com/en/docs/api/receiving/notifications-format/)
+
+This method will be called when an incoming message is received. Next, process messages according to the business logic of your system.
+
+## Examples list
+
+Description |  Module
+----- | ----- 
+Example of sending text | [sendTextMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendTextMessage.py)
+Example of sending a picture by URL | [sendPictureByLink.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByLink.py)
+Example of sending a picture by uploading from the disk | [sendPictureByUpload.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByUpload.py)
+Example of a group creation and sending a message to the group | [createGroupAndSendMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/createGroupAndSendMessage.py)
+Example of incoming webhooks receiving | [receiveNotification.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/receiveNotification.py)
+
+
+## The full list of the library methods
+
+| API method                             | Description                                                                                                              | Documentation link                                                                                          |
+|----------------------------------------|--------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|
+| `account.getSettings`                  | The method is designed to get the current settings of the account                                                        | [GetSettings](https://green-api.com/en/docs/api/account/GetSettings/)                                       |
+| `account.setSettings`                  | The method is designed to set the account settings                                                                       | [SetSettings](https://green-api.com/en/docs/api/account/SetSettings/)                                       |
+| `account.getStateInstance`             | The method is designed to get the state of the account                                                                   | [GetStateInstance](https://green-api.com/en/docs/api/account/GetStateInstance/)                             |
+| `account.getStatusInstance`            | The method is designed to get the socket connection state of the account instance with WhatsApp                          | [GetStatusInstance](https://green-api.com/en/docs/api/account/GetStatusInstance/)                           |
+| `account.reboot`                       | The method is designed to restart the account                                                                            | [Reboot](https://green-api.com/en/docs/api/account/Reboot/)                                                 |
+| `account.logout`                       | The method is designed to unlogin the account                                                                            | [Logout](https://green-api.com/en/docs/api/account/Logout/)                                                 |
+| `account.qr`                           | The method is designed to get a QR code                                                                                  | [QR](https://green-api.com/en/docs/api/account/QR/)                                                         |
+| `account.setProfilePicture`            | The method is designed to set the avatar of the account                                                                  | [SetProfilePicture](https://green-api.com/en/docs/api/account/SetProfilePicture/)                           |
+| `device.getDeviceInfo`                 | The method is designed to get information about the device (phone) on which the WhatsApp Business application is running | [GetDeviceInfo](https://green-api.com/en/docs/api/phone/GetDeviceInfo/)                                     |
+| `groups.createGroup`                   | The method is designed to create a group chat                                                                            | [CreateGroup](https://green-api.com/en/docs/api/groups/CreateGroup/)                                        |
+| `groups.updateGroupName`               | The method changes the name of the group chat                                                                            | [UpdateGroupName](https://green-api.com/en/docs/api/groups/UpdateGroupName/)                                |
+| `groups.getGroupData`                  | The method gets group chat data                                                                                          | [GetGroupData](https://green-api.com/en/docs/api/groups/GetGroupData/)                                      |
+| `groups.addGroupParticipant`           | The method adds a participant to the group chat                                                                          | [AddGroupParticipant](https://green-api.com/en/docs/api/groups/AddGroupParticipant/)                        |
+| `groups.removeGroupParticipant`        | The method removes the participant from the group chat                                                                   | [RemoveGroupParticipant](https://green-api.com/en/docs/api/groups/RemoveGroupParticipant/)                  |
+| `groups.setGroupAdmin`                 | The method designates a member of a group chat as an administrator                                                       | [SetGroupAdmin](https://green-api.com/en/docs/api/groups/SetGroupAdmin/)                                    |
+| `groups.removeAdmin`                   | The method deprives the participant of group chat administration rights                                                  | [RemoveAdmin](https://green-api.com/en/docs/api/groups/RemoveAdmin/)                                        |
+| `groups.setGroupPicture`               | The method sets the avatar of the group                                                                                  | [SetGroupPicture](https://green-api.com/en/docs/api/groups/SetGroupPicture/)                                |
+| `groups.leaveGroup`                    | The method logs the user of the current account out of the group chat                                                    | [LeaveGroup](https://green-api.com/en/docs/api/groups/LeaveGroup/)                                          |
+| `journals.getChatHistory`              | The method returns the chat message history                                                                              | [GetChatHistory](https://green-api.com/en/docs/api/journals/GetChatHistory/)                                |
+| `journals.getMessage`                  | The method returns a chat message                                                                                        | [GetMessage](https://green-api.com/en/docs/api/journals/GetMessage/)                                        |
+| `journals.lastIncomingMessages`        | The method returns the most recent incoming messages of the account                                                      | [LastIncomingMessages](https://green-api.com/en/docs/api/journals/LastIncomingMessages/)                    |
+| `journals.lastOutgoingMessages`        | The method returns the last sent messages of the account                                                                 | [LastOutgoingMessages](https://green-api.com/en/docs/api/journals/LastOutgoingMessages/)                    |
+| `queues.showMessagesQueue`             | The method is designed to get the list of messages that are in the queue to be sent                                      | [ShowMessagesQueue](https://green-api.com/en/docs/api/queues/ShowMessagesQueue/)                            |
+| `queues.clearMessagesQueue`            | The method is designed to clear the queue of messages to be sent                                                         | [ClearMessagesQueue](https://green-api.com/en/docs/api/queues/ClearMessagesQueue/)                          |
+| `marking.readChat`                     | The method is designed to mark chat messages as read                                                                     | [ReadChat](https://green-api.com/en/docs/api/marks/ReadChat/)                                               |
+| `receiving.receiveNotification`        | The method is designed to receive a single incoming notification from the notification queue                             | [ReceiveNotification](https://green-api.com/en/docs/api/receiving/technology-http-api/ReceiveNotification/) |
+| `receiving.deleteNotification`         | The method is designed to remove an incoming notification from the notification queue                                    | [DeleteNotification](https://green-api.com/en/docs/api/receiving/technology-http-api/DeleteNotification/)   |
+| `receiving.downloadFile`               | The method is for downloading received and sent files                                                                    | [DownloadFile](https://green-api.com/en/docs/api/receiving/files/DownloadFile/)                             |
+| `sending.sendMessage`                  | The method is designed to send a text message to a personal or group chat                                                | [SendMessage](https://green-api.com/en/docs/api/sending/SendMessage/)                                       |
+| `sending.sendButtons`                  | The method is designed to send a message with buttons to a personal or group chat                                        | [SendButtons](https://green-api.com/en/docs/api/sending/SendButtons/)                                       |
+| `sending.sendTemplateButtons`          | The method is designed to send a message with interactive buttons from the list of templates in a personal or group chat | [SendTemplateButtons](https://green-api.com/en/docs/api/sending/SendTemplateButtons/)                       |
+| `sending.sendListMessage`              | The method is designed to send a message with a selection button from a list of values to a personal or group chat       | [SendListMessage](https://green-api.com/en/docs/api/sending/SendListMessage/)                               |
+| `sending.sendFileByUpload`             | The method is designed to send a file loaded through a form (form-data)                                                  | [SendFileByUpload](https://green-api.com/en/docs/api/sending/SendFileByUpload/)                             |
+| `sending.sendFileByUrl`                | The method is designed to send a file downloaded via a link                                                              | [SendFileByUrl](https://green-api.com/en/docs/api/sending/SendFileByUrl/)                                   |
+| `sending.sendLocation`                 | The method is designed to send a geolocation message                                                                     | [SendLocation](https://green-api.com/en/docs/api/sending/SendLocation/)                                     |
+| `sending.sendContact`                  | The method is for sending a message with a contact                                                                       | [SendContact](https://green-api.com/en/docs/api/sending/SendContact/)                                       |
+| `sending.sendLink`                     | The method is designed to send a message with a link that will add an image preview, title and description               | [SendLink](https://green-api.com/en/docs/api/sending/SendLink/)                                             |
+| `sending.forwardMessages`              | The method is designed for forwarding messages to a personal or group chat                                               | [ForwardMessages](https://green-api.com/en/docs/api/sending/ForwardMessages/)                               |
+| `serviceMethods.checkWhatsapp`         | The method checks if there is a WhatsApp account on the phone number                                                     | [CheckWhatsapp](https://green-api.com/en/docs/api/service/CheckWhatsapp/)                                   |
+| `serviceMethods.getAvatar`             | The method returns the avatar of the correspondent or group chat                                                         | [GetAvatar](https://green-api.com/en/docs/api/service/GetAvatar/)                                           |
+| `serviceMethods.getContacts`           | The method is designed to get a list of contacts of the current account                                                  | [GetContacts](https://green-api.com/en/docs/api/service/GetContacts/)                                       |
+| `serviceMethods.getContactInfo`        | The method is designed to obtain information about the contact                                                           | [GetContactInfo](https://green-api.com/en/docs/api/service/GetContactInfo/)                                 |
+| `serviceMethods.deleteMessage`         | The method deletes the message from chat                                                                                 | [DeleteMessage](https://green-api.com/en/docs/api/service/deleteMessage/)                                   |
+| `serviceMethods.archiveChat`           | The method archives the chat                                                                                             | [ArchiveChat](https://green-api.com/en/docs/api/service/archiveChat/)                                       |
+| `serviceMethods.unarchiveChat`         | The method unarchives the chat                                                                                           | [UnarchiveChat](https://green-api.com/en/docs/api/service/unarchiveChat/)                                   |
+| `serviceMethods.setDisappearingChat`   | The method is designed to change the settings of disappearing messages in chats                                          | [SetDisappearingChat](https://green-api.com/en/docs/api/service/SetDisappearingChat/)                       |
+| `webhooks.startReceivingNotifications` | The method is designed to start receiving new notifications                                                              |                                                                                                             |
+| `webhooks.stopReceivingNotifications`  | The method is designed to stop receiving new notifications                                                               |                                                                                                             |
+
+## Service methods documentation
+
+[https://green-api.com/en/docs/api/](https://green-api.com/en/docs/api/)
+
+## External products
+
+* [requests](https://requests.readthedocs.io) - for http requests
+
+## License
+
+[![CC BY-ND 4.0][cc-by-nd-shield]][cc-by-nd]
+
+This work is licensed under a
+[Creative Commons Attribution-NoDerivatives 4.0 International License][cc-by-nd].
+
+[cc-by-nd]: https://creativecommons.org/licenses/by-nd/4.0/
+[cc-by-nd-shield]: https://img.shields.io/badge/License-CC%20BY--ND%204.0-lightgrey.svg
+
+Please see file [LICENSE](LICENSE)
```

### Comparing `whatsapp-api-client-python-0.0.34/README.md` & `whatsapp-api-client-python-0.0.35/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,185 +1,193 @@
-﻿# whatsapp-api-client-python
-
-[![Python application](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-app.yml/badge.svg)](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-app.yml)
-[![Upload Python Package](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-publish.yml/badge.svg)](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-publish.yml)
-
-- [Документация на русском языке](README_RUS.md)
-
-Python library for intagration with WhatsAPP messanger via API of [green-api.com](https://green-api.com) service. To use the library you have to get a registration token and an account id in the [personal area](https://console.green-api.com). There is a free developer account tariff plan.
-
-## API
-
-You can find REST API documentation by [url](https://green-api.com/docs/api/). The library is a wrapper for REST API, so the documentation at the above url applies to the library as well.
-
-## Installation
-
-```shell
-pip install whatsapp-api-client-python
-```
-
-## Import 
-
-```
-from whatsapp_api_client_python import API
-```
-## Authorization
-
-To send a message or to exacute some other Green-API method, you have to have the WhatsApp account in the phone application to be authorized. To authorize your account please go to the [personal area](https://console.green-api.com) and scan a QR-code using the WhatsApp application.
-
-## Examples
-
-### How to initialize an object
-
-```python
-greenAPI = API.GreenApi(ID_INSTANCE, API_TOKEN_INSTANCE)
-```
-
-### Sending a text message to a WhatsApp number
-
-```python
-result = greenAPI.sending.sendMessage('79001234567@g.us', 'Message text')
-```
-
-Example url: [sendTextMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendTextMessage.py)
-
-Please note that keys can be obtained from environment variables:
-```python
-from os import environ
-
-ID_INSTANCE = environ['ID_INSTANCE']
-API_TOKEN_INSTANCE = environ['API_TOKEN_INSTANCE']
-```
-
-### Sending an image via URL
-
-```python
-result = greenAPI.sending.sendFileByUrl('120363025955348359@g.us', 
-        'https://www.google.ru/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png', 
-        'googlelogo_color_272x92dp.png', 'Google logo')
-```
-
-Example url: [sendPictureByLink.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByLink.py)
-
-### Sending an image by uploading from the disk
-
-```python
-result = greenAPI.sending.sendFileByUpload('120363025955348359@g.us', 
-        'C:\Games\PicFromDisk.png', 
-        'PicFromDisk.png', 'Picture from disk')
-```
-
-Example url: [sendPictureByUpload.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByUpload.py)
-
-### Group creation and sending a message to the group
-
-```python
-chatIds = [
-    "79001234567@c.us"
-]
-resultCreate = greenAPI.groups.createGroup('GroupName', 
-    chatIds)
-
-if resultCreate.code == 200:
-    resultSend = greenAPI.sending.sendMessage(resultCreate.data['chatId'], 
-        'Message text')
-```
-
-IMPORTANT: If one tries to create a group with a non-existent number, WhatsApp 
-may block the sender's number. The number in the example is non-existent.
-
-Example url: [createGroupAndSendMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/createGroupAndSendMessage.py)
-
-### Receive incoming messages by HTTP API
-
-The general concept of receiving data in the Green API is described [here](https://green-api.com/en/docs/api/receiving/)
-To start receiving messages by the HTTP API you need to execute the library method:
-
-```python
-greenAPI.webhooks.startReceivingNotifications(onEvent)
-```
-
-onEvent - your method which should contain parameters:
-Parameter | Description
------ | -----
-typewebhook | received message type (string)
-body | message body (json)
-
-Message body types and formats [here](https://green-api.com/en/docs/api/receiving/notifications-format/)
-
-This method will be called when an incoming message is received. Next, process messages according to the business logic of your system.
-
-## Examples list
-
-Description |  Module
------ | ----- 
-Example of sending text | [sendTextMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendTextMessage.py)
-Example of sending a picture by URL | [sendPictureByLink.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByLink.py)
-Example of sending a picture by uploading from the disk | [sendPictureByUpload.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByUpload.py)
-Example of a group creation and sending a message to the group | [createGroupAndSendMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/createGroupAndSendMessage.py)
-Example of incoming webhooks receiving | [receiveNotification.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/receiveNotification.py)
-
-
-## The full list of the library methods
-
-| Method                                 | Description                                                                                                                                                                                         | Documentation                                                                                                                            |
-|----------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------|
-| `account.getSettings`                  | The method is aimed for getting the current settings of the account                                                                                                                                 | [GetSettings.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/GetSettings.md)                                       |
-| `account.getStateInstance`             | The method is aimed for getting the account state                                                                                                                                                   | [GetStateInstance.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/GetStateInstance.md)                             |
-| `account.getStatusInstance`            | The method is aimed for getting the status of the account instance socket connection with WhatsApp                                                                                                  | [GetStatusInstance.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/GetStatusInstance.md)                           |
-| `account.logout`                       | The method is aimed for logging out an account                                                                                                                                                      | [Logout.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/Logout.md)                                                 |
-| `account.qr`                           | The method is aimed for getting QR code                                                                                                                                                             | [QR.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/QR.md)                                                         |
-| `account.reboot`                       | The method is aimed for rebooting an account                                                                                                                                                        | [Reboot.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/Reboot.md)                                                 |
-| `account.setProfilePicture`            | The method is aimed for setting an account picture                                                                                                                                                  | [SetProfilePicture.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/SetProfilePicture.md)                           |
-| `account.setSettings`                  | The method is aimed for setting an account settings                                                                                                                                                 | [SetSettings.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/SetSettings.md)                                       |
-| `account.setSystemProxy`               | The method is aimed for setting a system proxy. Use the method when you need to reset custom proxy settings to system ones                                                                          | [SetSystemProxy.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/SetSystemProxy.md)                                 |
-| `groups.addGroupParticipant`           | Метод добавляет участника в групповой чат                                                                                                                                                           | [AddGroupParticipant.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/AddGroupParticipant.md)                        |
-| `groups.createGroup`                   | The method adds a participant to a group chat. IMPORTANT: If one tries to create a group with a non-existent number, WhatsApp may block the sender's number.                                        | [CreateGroup.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/CreateGroup.md)                                        |
-| `groups.getGroupData`                  | The method gets group chat data                                                                                                                                                                     | [GetGroupData.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/GetGroupData.md)                                     |
-| `groups.leaveGroup`                    | The method makes the current account user leave the group chat                                                                                                                                      | [LeaveGroup.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/LeaveGroup.md)                                          |
-| `groups.removeAdmin`                   | he method removes a participant from group chat administration rights                                                                                                                               | [RemoveAdmin.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/RemoveAdmin.md)                                        |
-| `groups.removeGroupParticipant`        | The method removes a participant from a group chat                                                                                                                                                  | [RemoveGroupParticipant.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/RemoveGroupParticipant.md)                  |
-| `groups.setGroupAdmin`                 | The method sets a group chat participant as an administrator                                                                                                                                        | [SetGroupAdmin.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/SetGroupAdmin.md)                                    |
-| `groups.setGroupPicture`               | The method sets a group picture                                                                                                                                                                     | [SetGroupPicture.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/SetGroupPicture.md)                                |
-| `groups.updateGroupName`               | The method changes a group chat name                                                                                                                                                                | [UpdateGroupName.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/UpdateGroupName.md)                                |
-| `journals.getChatHistory`              | The method returns the chat message history                                                                                                                                                         | [GetChatHistory.md](https://github.com/green-api/docs/blob/master/ru/docs/api/journals/GetChatHistory.md)                                |
-| `journals.lastIncomingMessages`        | The method returns the last incoming messages of the account. In the default mode the incoming messages for 24 hours are returned                                                                   | [GetChatHistory.md](https://github.com/green-api/docs/blob/master/ru/docs/api/journals/LastIncomingMessages.md)                          |
-| `journals.lastOutgoingMessages`        | The method returns the last outgoing messages of the account. In the default mode the last messages for 24 hours are returned                                                                       | [LastOutgoingMessages.md](https://github.com/green-api/docs/blob/master/ru/docs/api/journals/LastOutgoingMessages.md)                    |
-| `marking.readChat`                     | The method is aimed for marking messages in a chat as read. Either all messages or a specified message in a chat can be marked as read                                                              | [ReadChat.md](https://github.com/green-api/docs/blob/master/ru/docs/api/marks/ReadChat.md)                                               |
-| `device.getDeviceInfo`                 | The method is aimed for getting information about the device (phone) running WhatsApp Business application                                                                                          | [GetDeviceInfo.md](https://github.com/green-api/docs/blob/master/ru/docs/api/phone/GetDeviceInfo.md)                                     |
-| `queues.clearMessagesQueue`            | The method is aimed for clearing the queue of messages to be sent                                                                                                                                   | [ClearMessagesQueue.md](https://github.com/green-api/docs/blob/master/ru/docs/api/queues/ClearMessagesQueue.md)                          |
-| `queues.showMessagesQueue`             | The method is aimed for getting a list of messages in the queue to be sent                                                                                                                          | [ShowMessagesQueue.md](https://github.com/green-api/docs/blob/master/ru/docs/api/queues/ShowMessagesQueue.md)                            |
-| `receiving.deleteNotification`         | The method is aimed for deleting an incoming notification from the notification queue                                                                                                               | [DeleteNotification.md](https://github.com/green-api/docs/blob/master/ru/docs/api/receiving/technology-http-api/DeleteNotification.md)   |
-| `receiving.receiveNotification`        | The method is aimed for receiving one incoming notification from the notifications queue                                                                                                            | [ReceiveNotification.md](https://github.com/green-api/docs/blob/master/ru/docs/api/receiving/technology-http-api/ReceiveNotification.md) |
-| `sending.sendButtons`                  | The method is aimed for sending a button message to a personal or a group chat                                                                                                                      | [SendButtons.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendButtons.md)                                       |
-| `sending.sendContact`                  | The method is aimed for sending a contact message                                                                                                                                                   | [SendContact.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendContact.md)                                       |
-| `sending.sendFileByUpload`             | The method is aimed for sending a file uploaded by form                                                                                                                                             | [SendFileByUpload.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendFileByUpload.md)                             |
-| `sending.sendFileByUrl`                | The method is aimed for sending a file uploaded by Url                                                                                                                                              | [SendFileByUrl.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendFileByUrl.md)                                   |
-| `sending.sendLink`                     | The method is aimed for sending a message with a link, by which an image preview, title and description will be added                                                                               | [SendLink.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendLink.md)                                             |
-| `sending.sendListMessage`              | The method is aimed for sending a message with a select button from a list of values to a personal or a group chat                                                                                  | [SendListMessage.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendListMessage.md)                               |
-| `sending.sendLocation`                 | The method is aimed for sending a location message                                                                                                                                                  | [SendLocation.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendLocation.md)                                     |
-| `sending.sendMessage`                  | The method is aimed for sending a text message to a personal or a group chat                                                                                                                        | [SendMessage.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendMessage.md)                                       |
-| `sending.sendTemplateButtons`          | The method is aimed for sending a message with template list interactive buttons to a personal or a group chat                                                                                      | [SendTemplateButtons.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendTemplateButtons.md)                       |
-| `sending.forwardMessages`              | The method is intended for forwarding messages to a personal or group chat                                                                                                                          | [ForwardMessages.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/ForwardMessages.md)                               |
-| `serviceMethods.checkWhatsapp`         | The method checks WhatsApp account availability on a phone number                                                                                                                                   | [CheckWhatsapp.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/CheckWhatsapp.md)                                   |
-| `serviceMethods.getAvatar`             | The method returns a user or a group chat avatar                                                                                                                                                    | [GetAvatar.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/GetAvatar.md)                                           |
-| `serviceMethods.getContactInfo`        | The method is aimed for getting information on a contact                                                                                                                                            | [GetContactInfo.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/GetContactInfo.md)                                 |
-| `serviceMethods.getContacts`           | The method is aimed for getting a list of the current account contacts                                                                                                                              | [GetContacts.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/GetContacts.md)                                       |
-| `serviceMethods.setDisappearingChat`   | The method is aimed for changing settings of disappearing messages in chats. The standard settings of the application are to be used: 0 (off), 86400 (24 hours), 604800 (7 days), 7776000 (90 days) | [SetDisappearingChat.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/SetDisappearingChat.md)                       |
-| `serviceMethods.archiveChat`           | The method archives a chat. One can archive chats that have at least one incoming message                                                                                                           | [ArchiveChat.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/ArchiveChat.md)                                       |
-| `serviceMethods.deleteMessage`         | The method deletes a message from a chat                                                                                                                                                            | [DeleteMessage.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/deleteMessage.md)                                   |
-| `serviceMethods.unarchiveChat`         | The method unarchives a chat                                                                                                                                                                        | [UnarchiveChat.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/UnarchiveChat.md)                                   |
-| `serviceMethods.setDisappearingChat`   | The method is aimed for changing settings of disappearing messages in chats                                                                                                                         | [SetDisappearingChat.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/SetDisappearingChat.md)                       |
-| `webhooks.startReceivingNotifications` | The method is aimed for starting to receive webhooks                                                                                                                                                | <library method>                                                                                                                         |
-| `webhooks.stopReceivingNotifications`  | The method is aimed for stopping to receive webhooks                                                                                                                                                | <library method>                                                                                                                         |
-
-## Service methods documentation
-
-[https://green-api.com/en/docs/api/](https://green-api.com/en/docs/api/)
-
-## External products
-
-* [requests](https://requests.readthedocs.io) - for http requests
-
-## License
-
-Licensed under MIT terms. Please see file [LICENSE](LICENSE)
+﻿# whatsapp-api-client-python
+
+[![Python application](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-app.yml/badge.svg)](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-app.yml)
+[![Upload Python Package](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-publish.yml/badge.svg)](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-publish.yml)
+
+- [Документация на русском языке](README_RUS.md)
+
+Python library for intagration with WhatsAPP messanger via API of [green-api.com](https://green-api.com/en/) service. To use the library you have to get a registration token and an account id in the [personal area](https://console.green-api.com). There is a free developer account tariff plan.
+
+## API
+
+You can find REST API documentation by [url](https://green-api.com/en/docs/api/). The library is a wrapper for REST API, so the documentation at the above url applies to the library as well.
+
+## Installation
+
+```shell
+pip install whatsapp-api-client-python
+```
+
+## Import 
+
+```
+from whatsapp_api_client_python import API
+```
+## Authorization
+
+To send a message or to exacute some other Green-API method, you have to have the WhatsApp account in the phone application to be authorized. To authorize your account please go to the [personal area](https://console.green-api.com) and scan a QR-code using the WhatsApp application.
+
+## Examples
+
+### How to initialize an object
+
+```python
+greenAPI = API.GreenApi(ID_INSTANCE, API_TOKEN_INSTANCE)
+```
+
+### Sending a text message to a WhatsApp number
+
+```python
+result = greenAPI.sending.sendMessage('79001234567@g.us', 'Message text')
+```
+
+Example url: [sendTextMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendTextMessage.py)
+
+Please note that keys can be obtained from environment variables:
+```python
+from os import environ
+
+ID_INSTANCE = environ['ID_INSTANCE']
+API_TOKEN_INSTANCE = environ['API_TOKEN_INSTANCE']
+```
+
+### Sending an image via URL
+
+```python
+result = greenAPI.sending.sendFileByUrl('120363025955348359@g.us', 
+        'https://www.google.ru/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png', 
+        'googlelogo_color_272x92dp.png', 'Google logo')
+```
+
+Example url: [sendPictureByLink.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByLink.py)
+
+### Sending an image by uploading from the disk
+
+```python
+result = greenAPI.sending.sendFileByUpload('120363025955348359@g.us', 
+        'C:\Games\PicFromDisk.png', 
+        'PicFromDisk.png', 'Picture from disk')
+```
+
+Example url: [sendPictureByUpload.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByUpload.py)
+
+### Group creation and sending a message to the group
+
+```python
+chatIds = [
+    "79001234567@c.us"
+]
+resultCreate = greenAPI.groups.createGroup('GroupName', 
+    chatIds)
+
+if resultCreate.code == 200:
+    resultSend = greenAPI.sending.sendMessage(resultCreate.data['chatId'], 
+        'Message text')
+```
+
+IMPORTANT: If one tries to create a group with a non-existent number, WhatsApp 
+may block the sender's number. The number in the example is non-existent.
+
+Example url: [createGroupAndSendMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/createGroupAndSendMessage.py)
+
+### Receive incoming messages by HTTP API
+
+The general concept of receiving data in the Green API is described [here](https://green-api.com/en/docs/api/receiving/)
+To start receiving messages by the HTTP API you need to execute the library method:
+
+```python
+greenAPI.webhooks.startReceivingNotifications(onEvent)
+```
+
+onEvent - your method which should contain parameters:
+Parameter | Description
+----- | -----
+typewebhook | received message type (string)
+body | message body (json)
+
+Message body types and formats [here](https://green-api.com/en/docs/api/receiving/notifications-format/)
+
+This method will be called when an incoming message is received. Next, process messages according to the business logic of your system.
+
+## Examples list
+
+Description |  Module
+----- | ----- 
+Example of sending text | [sendTextMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendTextMessage.py)
+Example of sending a picture by URL | [sendPictureByLink.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByLink.py)
+Example of sending a picture by uploading from the disk | [sendPictureByUpload.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByUpload.py)
+Example of a group creation and sending a message to the group | [createGroupAndSendMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/createGroupAndSendMessage.py)
+Example of incoming webhooks receiving | [receiveNotification.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/receiveNotification.py)
+
+
+## The full list of the library methods
+
+| API method                             | Description                                                                                                              | Documentation link                                                                                          |
+|----------------------------------------|--------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|
+| `account.getSettings`                  | The method is designed to get the current settings of the account                                                        | [GetSettings](https://green-api.com/en/docs/api/account/GetSettings/)                                       |
+| `account.setSettings`                  | The method is designed to set the account settings                                                                       | [SetSettings](https://green-api.com/en/docs/api/account/SetSettings/)                                       |
+| `account.getStateInstance`             | The method is designed to get the state of the account                                                                   | [GetStateInstance](https://green-api.com/en/docs/api/account/GetStateInstance/)                             |
+| `account.getStatusInstance`            | The method is designed to get the socket connection state of the account instance with WhatsApp                          | [GetStatusInstance](https://green-api.com/en/docs/api/account/GetStatusInstance/)                           |
+| `account.reboot`                       | The method is designed to restart the account                                                                            | [Reboot](https://green-api.com/en/docs/api/account/Reboot/)                                                 |
+| `account.logout`                       | The method is designed to unlogin the account                                                                            | [Logout](https://green-api.com/en/docs/api/account/Logout/)                                                 |
+| `account.qr`                           | The method is designed to get a QR code                                                                                  | [QR](https://green-api.com/en/docs/api/account/QR/)                                                         |
+| `account.setProfilePicture`            | The method is designed to set the avatar of the account                                                                  | [SetProfilePicture](https://green-api.com/en/docs/api/account/SetProfilePicture/)                           |
+| `device.getDeviceInfo`                 | The method is designed to get information about the device (phone) on which the WhatsApp Business application is running | [GetDeviceInfo](https://green-api.com/en/docs/api/phone/GetDeviceInfo/)                                     |
+| `groups.createGroup`                   | The method is designed to create a group chat                                                                            | [CreateGroup](https://green-api.com/en/docs/api/groups/CreateGroup/)                                        |
+| `groups.updateGroupName`               | The method changes the name of the group chat                                                                            | [UpdateGroupName](https://green-api.com/en/docs/api/groups/UpdateGroupName/)                                |
+| `groups.getGroupData`                  | The method gets group chat data                                                                                          | [GetGroupData](https://green-api.com/en/docs/api/groups/GetGroupData/)                                      |
+| `groups.addGroupParticipant`           | The method adds a participant to the group chat                                                                          | [AddGroupParticipant](https://green-api.com/en/docs/api/groups/AddGroupParticipant/)                        |
+| `groups.removeGroupParticipant`        | The method removes the participant from the group chat                                                                   | [RemoveGroupParticipant](https://green-api.com/en/docs/api/groups/RemoveGroupParticipant/)                  |
+| `groups.setGroupAdmin`                 | The method designates a member of a group chat as an administrator                                                       | [SetGroupAdmin](https://green-api.com/en/docs/api/groups/SetGroupAdmin/)                                    |
+| `groups.removeAdmin`                   | The method deprives the participant of group chat administration rights                                                  | [RemoveAdmin](https://green-api.com/en/docs/api/groups/RemoveAdmin/)                                        |
+| `groups.setGroupPicture`               | The method sets the avatar of the group                                                                                  | [SetGroupPicture](https://green-api.com/en/docs/api/groups/SetGroupPicture/)                                |
+| `groups.leaveGroup`                    | The method logs the user of the current account out of the group chat                                                    | [LeaveGroup](https://green-api.com/en/docs/api/groups/LeaveGroup/)                                          |
+| `journals.getChatHistory`              | The method returns the chat message history                                                                              | [GetChatHistory](https://green-api.com/en/docs/api/journals/GetChatHistory/)                                |
+| `journals.getMessage`                  | The method returns a chat message                                                                                        | [GetMessage](https://green-api.com/en/docs/api/journals/GetMessage/)                                        |
+| `journals.lastIncomingMessages`        | The method returns the most recent incoming messages of the account                                                      | [LastIncomingMessages](https://green-api.com/en/docs/api/journals/LastIncomingMessages/)                    |
+| `journals.lastOutgoingMessages`        | The method returns the last sent messages of the account                                                                 | [LastOutgoingMessages](https://green-api.com/en/docs/api/journals/LastOutgoingMessages/)                    |
+| `queues.showMessagesQueue`             | The method is designed to get the list of messages that are in the queue to be sent                                      | [ShowMessagesQueue](https://green-api.com/en/docs/api/queues/ShowMessagesQueue/)                            |
+| `queues.clearMessagesQueue`            | The method is designed to clear the queue of messages to be sent                                                         | [ClearMessagesQueue](https://green-api.com/en/docs/api/queues/ClearMessagesQueue/)                          |
+| `marking.readChat`                     | The method is designed to mark chat messages as read                                                                     | [ReadChat](https://green-api.com/en/docs/api/marks/ReadChat/)                                               |
+| `receiving.receiveNotification`        | The method is designed to receive a single incoming notification from the notification queue                             | [ReceiveNotification](https://green-api.com/en/docs/api/receiving/technology-http-api/ReceiveNotification/) |
+| `receiving.deleteNotification`         | The method is designed to remove an incoming notification from the notification queue                                    | [DeleteNotification](https://green-api.com/en/docs/api/receiving/technology-http-api/DeleteNotification/)   |
+| `receiving.downloadFile`               | The method is for downloading received and sent files                                                                    | [DownloadFile](https://green-api.com/en/docs/api/receiving/files/DownloadFile/)                             |
+| `sending.sendMessage`                  | The method is designed to send a text message to a personal or group chat                                                | [SendMessage](https://green-api.com/en/docs/api/sending/SendMessage/)                                       |
+| `sending.sendButtons`                  | The method is designed to send a message with buttons to a personal or group chat                                        | [SendButtons](https://green-api.com/en/docs/api/sending/SendButtons/)                                       |
+| `sending.sendTemplateButtons`          | The method is designed to send a message with interactive buttons from the list of templates in a personal or group chat | [SendTemplateButtons](https://green-api.com/en/docs/api/sending/SendTemplateButtons/)                       |
+| `sending.sendListMessage`              | The method is designed to send a message with a selection button from a list of values to a personal or group chat       | [SendListMessage](https://green-api.com/en/docs/api/sending/SendListMessage/)                               |
+| `sending.sendFileByUpload`             | The method is designed to send a file loaded through a form (form-data)                                                  | [SendFileByUpload](https://green-api.com/en/docs/api/sending/SendFileByUpload/)                             |
+| `sending.sendFileByUrl`                | The method is designed to send a file downloaded via a link                                                              | [SendFileByUrl](https://green-api.com/en/docs/api/sending/SendFileByUrl/)                                   |
+| `sending.sendLocation`                 | The method is designed to send a geolocation message                                                                     | [SendLocation](https://green-api.com/en/docs/api/sending/SendLocation/)                                     |
+| `sending.sendContact`                  | The method is for sending a message with a contact                                                                       | [SendContact](https://green-api.com/en/docs/api/sending/SendContact/)                                       |
+| `sending.sendLink`                     | The method is designed to send a message with a link that will add an image preview, title and description               | [SendLink](https://green-api.com/en/docs/api/sending/SendLink/)                                             |
+| `sending.forwardMessages`              | The method is designed for forwarding messages to a personal or group chat                                               | [ForwardMessages](https://green-api.com/en/docs/api/sending/ForwardMessages/)                               |
+| `serviceMethods.checkWhatsapp`         | The method checks if there is a WhatsApp account on the phone number                                                     | [CheckWhatsapp](https://green-api.com/en/docs/api/service/CheckWhatsapp/)                                   |
+| `serviceMethods.getAvatar`             | The method returns the avatar of the correspondent or group chat                                                         | [GetAvatar](https://green-api.com/en/docs/api/service/GetAvatar/)                                           |
+| `serviceMethods.getContacts`           | The method is designed to get a list of contacts of the current account                                                  | [GetContacts](https://green-api.com/en/docs/api/service/GetContacts/)                                       |
+| `serviceMethods.getContactInfo`        | The method is designed to obtain information about the contact                                                           | [GetContactInfo](https://green-api.com/en/docs/api/service/GetContactInfo/)                                 |
+| `serviceMethods.deleteMessage`         | The method deletes the message from chat                                                                                 | [DeleteMessage](https://green-api.com/en/docs/api/service/deleteMessage/)                                   |
+| `serviceMethods.archiveChat`           | The method archives the chat                                                                                             | [ArchiveChat](https://green-api.com/en/docs/api/service/archiveChat/)                                       |
+| `serviceMethods.unarchiveChat`         | The method unarchives the chat                                                                                           | [UnarchiveChat](https://green-api.com/en/docs/api/service/unarchiveChat/)                                   |
+| `serviceMethods.setDisappearingChat`   | The method is designed to change the settings of disappearing messages in chats                                          | [SetDisappearingChat](https://green-api.com/en/docs/api/service/SetDisappearingChat/)                       |
+| `webhooks.startReceivingNotifications` | The method is designed to start receiving new notifications                                                              |                                                                                                             |
+| `webhooks.stopReceivingNotifications`  | The method is designed to stop receiving new notifications                                                               |                                                                                                             |
+
+## Service methods documentation
+
+[https://green-api.com/en/docs/api/](https://green-api.com/en/docs/api/)
+
+## External products
+
+* [requests](https://requests.readthedocs.io) - for http requests
+
+## License
+
+[![CC BY-ND 4.0][cc-by-nd-shield]][cc-by-nd]
+
+This work is licensed under a
+[Creative Commons Attribution-NoDerivatives 4.0 International License][cc-by-nd].
+
+[cc-by-nd]: https://creativecommons.org/licenses/by-nd/4.0/
+[cc-by-nd-shield]: https://img.shields.io/badge/License-CC%20BY--ND%204.0-lightgrey.svg
+
+Please see file [LICENSE](LICENSE)
```

### Comparing `whatsapp-api-client-python-0.0.34/tests/test_main.py` & `whatsapp-api-client-python-0.0.35/tests/test_main.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from os import environ
-
-from whatsapp_api_client_python import API as API
-
-
-ID_INSTANCE = environ['ID_INSTANCE']
-API_TOKEN_INSTANCE = environ['API_TOKEN_INSTANCE']
-
-greenAPI = API.GreenApi(ID_INSTANCE, API_TOKEN_INSTANCE)
-
-class TestClass: 
-        def test_getSettings(self):            
-                result = greenAPI.account.getSettings()
-                if result.code != 200:
-                        print(result.error)
-                assert isinstance(result, API.Response) and result.code == 200
-
-        def test_getStateInstance(self):            
-                result = greenAPI.account.getStateInstance()
-                if result.code != 200:
-                        print(result.error)
-                assert isinstance(result, API.Response) and result.code == 200
-
-def main():
-        TestClass.test_getSettings(TestClass)
-        TestClass.test_getStateInstance(TestClass)
-
-if __name__ == "__main__":
+from os import environ
+
+from whatsapp_api_client_python import API as API
+
+
+ID_INSTANCE = environ['ID_INSTANCE']
+API_TOKEN_INSTANCE = environ['API_TOKEN_INSTANCE']
+
+greenAPI = API.GreenApi(ID_INSTANCE, API_TOKEN_INSTANCE)
+
+class TestClass: 
+        def test_getSettings(self):            
+                result = greenAPI.account.getSettings()
+                if result.code != 200:
+                        print(result.error)
+                assert isinstance(result, API.Response) and result.code == 200
+
+        def test_getStateInstance(self):            
+                result = greenAPI.account.getStateInstance()
+                if result.code != 200:
+                        print(result.error)
+                assert isinstance(result, API.Response) and result.code == 200
+
+def main():
+        TestClass.test_getSettings(TestClass)
+        TestClass.test_getStateInstance(TestClass)
+
+if __name__ == "__main__":
     main()
```

### Comparing `whatsapp-api-client-python-0.0.34/whatsapp_api_client_python/API.py` & `whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/API.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-from array import array
-import requests
-import json
-from whatsapp_api_client_python.response import Response
-
-from whatsapp_api_client_python.tools.account import Account
-from whatsapp_api_client_python.tools.device import Device
-from whatsapp_api_client_python.tools.groups import Groups
-from whatsapp_api_client_python.tools.journals import Journals
-from whatsapp_api_client_python.tools.marking import Marking
-from whatsapp_api_client_python.tools.queues import Queues
-from whatsapp_api_client_python.tools.receiving import Receiving
-from whatsapp_api_client_python.tools.sending import Sending
-from whatsapp_api_client_python.tools.serviceMethods import ServiceMethods
-from whatsapp_api_client_python.tools.webhooks import Webhooks
-
-
-class GreenApi:
-    'REST API class'
-
-    host: str
-    idInstance: str
-    apiTokenInstance: str
-
-    def __init__(self, 
-                    idInstance: str, 
-                    apiTokenInstance: str,
-                    host: str = 'https://api.green-api.com') -> None:
-        self.host = host
-        self.idInstance = idInstance
-        self.apiTokenInstance = apiTokenInstance
-
-        self.account = Account(self)
-        self.device = Device(self)
-        self.groups = Groups(self)
-        self.journals = Journals(self)
-        self.marking = Marking(self)
-        self.queues = Queues(self)
-        self.receiving = Receiving(self)
-        self.sending = Sending(self)
-        self.serviceMethods = ServiceMethods(self)
-        self.webhooks = Webhooks(self)
-
-    def request(self, method: str, url: str, 
-                payload: any = None, files: array = None):
-        url = url.replace('{{host}}', self.host)
-        url = url.replace('{{idInstance}}', self.idInstance)
-        url = url.replace('{{apiTokenInstance}}', self.apiTokenInstance)
-        status_code = 0
-        text = ''
-        try:
-            headers = {}
-            payloadData = None
-            if payload != None:
-                if files == None:
-                    headers = {
-                        'Content-Type': 'application/json'
-                    }
-                    payloadData = json.dumps(payload)
-                else:
-                    payloadData = payload   
-            result = requests.request(method, url, headers = headers, 
-                                        data = payloadData, 
-                                        files = files)
-            status_code = result.status_code
-            text = result.text
-            result.raise_for_status()
-        except requests.HTTPError:
-            return Response(status_code, text)
-        except Exception as err:
-            status_code = 0
-            text = f'Other error occurred: {err}'
+from array import array
+import requests
+import json
+from whatsapp_api_client_python.response import Response
+
+from whatsapp_api_client_python.tools.account import Account
+from whatsapp_api_client_python.tools.device import Device
+from whatsapp_api_client_python.tools.groups import Groups
+from whatsapp_api_client_python.tools.journals import Journals
+from whatsapp_api_client_python.tools.marking import Marking
+from whatsapp_api_client_python.tools.queues import Queues
+from whatsapp_api_client_python.tools.receiving import Receiving
+from whatsapp_api_client_python.tools.sending import Sending
+from whatsapp_api_client_python.tools.serviceMethods import ServiceMethods
+from whatsapp_api_client_python.tools.webhooks import Webhooks
+
+
+class GreenApi:
+    'REST API class'
+
+    host: str
+    idInstance: str
+    apiTokenInstance: str
+
+    def __init__(self, 
+                    idInstance: str, 
+                    apiTokenInstance: str,
+                    host: str = 'https://api.green-api.com') -> None:
+        self.host = host
+        self.idInstance = idInstance
+        self.apiTokenInstance = apiTokenInstance
+
+        self.account = Account(self)
+        self.device = Device(self)
+        self.groups = Groups(self)
+        self.journals = Journals(self)
+        self.marking = Marking(self)
+        self.queues = Queues(self)
+        self.receiving = Receiving(self)
+        self.sending = Sending(self)
+        self.serviceMethods = ServiceMethods(self)
+        self.webhooks = Webhooks(self)
+
+    def request(self, method: str, url: str, 
+                payload: any = None, files: array = None):
+        url = url.replace('{{host}}', self.host)
+        url = url.replace('{{idInstance}}', self.idInstance)
+        url = url.replace('{{apiTokenInstance}}', self.apiTokenInstance)
+        status_code = 0
+        text = ''
+        try:
+            headers = {}
+            payloadData = None
+            if payload != None:
+                if files == None:
+                    headers = {
+                        'Content-Type': 'application/json'
+                    }
+                    payloadData = json.dumps(payload)
+                else:
+                    payloadData = payload   
+            result = requests.request(method, url, headers = headers, 
+                                        data = payloadData, 
+                                        files = files)
+            status_code = result.status_code
+            text = result.text
+            result.raise_for_status()
+        except requests.HTTPError:
+            return Response(status_code, text)
+        except Exception as err:
+            status_code = 0
+            text = f'Other error occurred: {err}'
         return Response(status_code, text)
```

### Comparing `whatsapp-api-client-python-0.0.34/whatsapp_api_client_python/tools/groups.py` & `whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/groups.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-from array import ArrayType, array
-import os.path
-from whatsapp_api_client_python.response import Response
-
-
-class Groups:
-    def __init__(self, greenApi) -> None:
-        self.greenApi = greenApi
-        
-    def addGroupParticipant(self, 
-            groupId: str, 
-            participantChatId: str) -> Response:
-            'The method adds a participant to a group chat.'
-
-            requestBody = {
-                'groupId': groupId,
-                'participantChatId': participantChatId,
-            }
-            
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/AddGroupParticipant/{{apiTokenInstance}}',
-                requestBody)
-
-    def createGroup(self, groupName: str, chatIds: array) -> Response:
-            'The method is aimed for creating a group chat.'
-            
-            requestBody = {
-                'groupName': groupName,
-                'chatIds': chatIds
-            }
-
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/CreateGroup/{{apiTokenInstance}}',
-                requestBody)
-
-    def getGroupData(self, groupId: str) -> Response:
-            'The method gets group chat data.'
-
-            requestBody = {
-                'groupId': groupId
-            }
-            
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/GetGroupData/{{apiTokenInstance}}',
-                requestBody)
-
-    def leaveGroup(self, groupId: str) -> Response:
-            'The method makes the current account user leave the group chat.'
-
-            requestBody = {
-                'groupId': groupId
-            }
-            
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/LeaveGroup/{{apiTokenInstance}}',
-                requestBody)
-
-    def removeAdmin(self, groupId: str, participantChatId: str) -> Response:
-            'The method removes a participant from group chat '\
-            'administartion rights.'
-
-            requestBody = {
-                'groupId': groupId,
-                'participantChatId': participantChatId
-            }
-            
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/RemoveAdmin/{{apiTokenInstance}}',
-                requestBody)
-
-    def removeGroupParticipant(self, 
-        groupId: str, 
-        participantChatId: str) -> Response:
-            'The method removes a participant from a group chat.'
-
-            requestBody = {
-                'groupId': groupId,
-                'participantChatId': participantChatId
-            }
-            
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/RemoveGroupParticipant/{{apiTokenInstance}}',
-                requestBody)
-
-    def setGroupAdmin(self, 
-        groupId: str, 
-        participantChatId: str) -> Response:
-            'The method sets a group chat participant as an administrator.'
-
-            requestBody = {
-                'groupId': groupId,
-                'participantChatId': participantChatId
-            }
-            
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/SetGroupAdmin/{{apiTokenInstance}}',
-                requestBody)
-
-    def setGroupPicture(self, 
-        groupId: str, 
-        path: str) -> Response:
-            'The method sets a group picture.'
-
-            requestBody = {
-                'groupId': groupId
-            }
-
-            pathParts = os.path.split(path)
-            file = pathParts[1]
-
-            files = [
-                ('file',(file, open(path,'rb'),'image/jpeg'))
-            ]
-            
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/SetGroupPicture/{{apiTokenInstance}}',
-                requestBody, files)
-
-    def updateGroupName(self, 
-        groupId: str, 
-        groupName: str) -> Response:
-            'The method changes a group chat name.'
-
-            requestBody = {
-                'groupId': groupId,
-                'groupName': groupName
-            }
-            
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/UpdateGroupName/{{apiTokenInstance}}',
+from array import ArrayType, array
+import os.path
+from whatsapp_api_client_python.response import Response
+
+
+class Groups:
+    def __init__(self, greenApi) -> None:
+        self.greenApi = greenApi
+        
+    def addGroupParticipant(self, 
+            groupId: str, 
+            participantChatId: str) -> Response:
+            'The method adds a participant to a group chat.'
+
+            requestBody = {
+                'groupId': groupId,
+                'participantChatId': participantChatId,
+            }
+            
+            return self.greenApi.request('POST', 
+                '{{host}}/waInstance{{idInstance}}'
+                '/AddGroupParticipant/{{apiTokenInstance}}',
+                requestBody)
+
+    def createGroup(self, groupName: str, chatIds: array) -> Response:
+            'The method is aimed for creating a group chat.'
+            
+            requestBody = {
+                'groupName': groupName,
+                'chatIds': chatIds
+            }
+
+            return self.greenApi.request('POST', 
+                '{{host}}/waInstance{{idInstance}}'
+                '/CreateGroup/{{apiTokenInstance}}',
+                requestBody)
+
+    def getGroupData(self, groupId: str) -> Response:
+            'The method gets group chat data.'
+
+            requestBody = {
+                'groupId': groupId
+            }
+            
+            return self.greenApi.request('POST', 
+                '{{host}}/waInstance{{idInstance}}'
+                '/GetGroupData/{{apiTokenInstance}}',
+                requestBody)
+
+    def leaveGroup(self, groupId: str) -> Response:
+            'The method makes the current account user leave the group chat.'
+
+            requestBody = {
+                'groupId': groupId
+            }
+            
+            return self.greenApi.request('POST', 
+                '{{host}}/waInstance{{idInstance}}'
+                '/LeaveGroup/{{apiTokenInstance}}',
+                requestBody)
+
+    def removeAdmin(self, groupId: str, participantChatId: str) -> Response:
+            'The method removes a participant from group chat '\
+            'administartion rights.'
+
+            requestBody = {
+                'groupId': groupId,
+                'participantChatId': participantChatId
+            }
+            
+            return self.greenApi.request('POST', 
+                '{{host}}/waInstance{{idInstance}}'
+                '/RemoveAdmin/{{apiTokenInstance}}',
+                requestBody)
+
+    def removeGroupParticipant(self, 
+        groupId: str, 
+        participantChatId: str) -> Response:
+            'The method removes a participant from a group chat.'
+
+            requestBody = {
+                'groupId': groupId,
+                'participantChatId': participantChatId
+            }
+            
+            return self.greenApi.request('POST', 
+                '{{host}}/waInstance{{idInstance}}'
+                '/RemoveGroupParticipant/{{apiTokenInstance}}',
+                requestBody)
+
+    def setGroupAdmin(self, 
+        groupId: str, 
+        participantChatId: str) -> Response:
+            'The method sets a group chat participant as an administrator.'
+
+            requestBody = {
+                'groupId': groupId,
+                'participantChatId': participantChatId
+            }
+            
+            return self.greenApi.request('POST', 
+                '{{host}}/waInstance{{idInstance}}'
+                '/SetGroupAdmin/{{apiTokenInstance}}',
+                requestBody)
+
+    def setGroupPicture(self, 
+        groupId: str, 
+        path: str) -> Response:
+            'The method sets a group picture.'
+
+            requestBody = {
+                'groupId': groupId
+            }
+
+            pathParts = os.path.split(path)
+            file = pathParts[1]
+
+            files = [
+                ('file',(file, open(path,'rb'),'image/jpeg'))
+            ]
+            
+            return self.greenApi.request('POST', 
+                '{{host}}/waInstance{{idInstance}}'
+                '/SetGroupPicture/{{apiTokenInstance}}',
+                requestBody, files)
+
+    def updateGroupName(self, 
+        groupId: str, 
+        groupName: str) -> Response:
+            'The method changes a group chat name.'
+
+            requestBody = {
+                'groupId': groupId,
+                'groupName': groupName
+            }
+            
+            return self.greenApi.request('POST', 
+                '{{host}}/waInstance{{idInstance}}'
+                '/UpdateGroupName/{{apiTokenInstance}}',
                 requestBody)
```

### Comparing `whatsapp-api-client-python-0.0.34/whatsapp_api_client_python/tools/marking.py` & `whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/marking.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from whatsapp_api_client_python.response import Response
-
-
-class Marking:
-    def __init__(self, greenApi) -> None:
-        self.greenApi = greenApi
-        
-    def readChat(self, chatId: str, idMessage: str) -> Response:
-            'The method returns the chat message history.'
-
-            requestBody = {
-                'chatId': chatId,
-                'idMessage': idMessage,
-            }
-
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/ReadChat/{{apiTokenInstance}}',
+from whatsapp_api_client_python.response import Response
+
+
+class Marking:
+    def __init__(self, greenApi) -> None:
+        self.greenApi = greenApi
+        
+    def readChat(self, chatId: str, idMessage: str) -> Response:
+            'The method returns the chat message history.'
+
+            requestBody = {
+                'chatId': chatId,
+                'idMessage': idMessage,
+            }
+
+            return self.greenApi.request('POST', 
+                '{{host}}/waInstance{{idInstance}}'
+                '/ReadChat/{{apiTokenInstance}}',
                 requestBody)
```

### Comparing `whatsapp-api-client-python-0.0.34/whatsapp_api_client_python/tools/queues.py` & `whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/queues.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from whatsapp_api_client_python.response import Response
-
-
-class Queues:
-    def __init__(self, greenApi) -> None:
-        self.greenApi = greenApi
-        
-    def clearMessagesQueue(self) -> Response:
-            'The method is aimed for clearing the queue of messages to be sent.'
-
-            return self.greenApi.request('GET', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/ClearMessagesQueue/{{apiTokenInstance}}')
-
-    def showMessagesQueue(self) -> Response:
-            'The method is aimed for getting a list of messages in the queue '\
-            'to be sent. Messages sending rate is managed by Messages sending '\
-            'delay parameter.'
-
-            return self.greenApi.request('GET', 
-                '{{host}}/waInstance{{idInstance}}'
+from whatsapp_api_client_python.response import Response
+
+
+class Queues:
+    def __init__(self, greenApi) -> None:
+        self.greenApi = greenApi
+        
+    def clearMessagesQueue(self) -> Response:
+            'The method is aimed for clearing the queue of messages to be sent.'
+
+            return self.greenApi.request('GET', 
+                '{{host}}/waInstance{{idInstance}}'
+                '/ClearMessagesQueue/{{apiTokenInstance}}')
+
+    def showMessagesQueue(self) -> Response:
+            'The method is aimed for getting a list of messages in the queue '\
+            'to be sent. Messages sending rate is managed by Messages sending '\
+            'delay parameter.'
+
+            return self.greenApi.request('GET', 
+                '{{host}}/waInstance{{idInstance}}'
                 '/ShowMessagesQueue/{{apiTokenInstance}}')
```

### Comparing `whatsapp-api-client-python-0.0.34/whatsapp_api_client_python/tools/receiving.py` & `whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/receiving.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from whatsapp_api_client_python.response import Response
-
-
-class Receiving:
-    def __init__(self, greenApi) -> None:
-        self.greenApi = greenApi
-        
-    def downloadFile(self, idMessage: str) -> Response:
-        'The method is aimed for downloading incoming and outgoing files. '\
-        'Links to incoming files are transmitted in Incoming messages, '\
-        'and you can also get them using LastIncomingMessages method. '\
-        'You can get links to outgoing files using '\
-        'LastOutgoingMessages method.'\
-        'Files storage period and, accordingly, the capability '\
-        'to download them is limited to 24 hours.'
-
-        requestBody = {
-            'idMessage': idMessage,
-        }
-
-        return self.greenApi.request('POST', 
-            '{{host}}/waInstance{{idInstance}}'
-            '/DownloadFile/{{apiTokenInstance}}',
-            requestBody)
-
-    def receiveNotification(self) -> Response:
-        'The method is aimed for receiving one incoming notification from '\
-        'the notifications queue. '\
-        'ReceiveNotification method waits for a notification receipt '\
-        'for 20 sec. The method call ends with an empty response if a timeout '\
-        'is reached. If a notification comes to the queue within 20 seconds, '\
-        'the method call is completed, and the method returns the received '\
-        'notification.'\
-        'After receiving and processing an incoming notification, you need '\
-        'to delete the notification from the queue. This requires you to run '\
-        'DeleteNotification method. After calling DeleteNotification method, '\
-        'the notification will be considered received and processed and '\
-        'will be permanently deleted from the queue. Therefore, the next call '\
-        'of ReceiveNotification method will return the next notification from '\
-        'the queue in the order in which notifications come to the queue.'\
-        'Incoming notifications are stored in the queue for 24 hours. '\
-        'Notifications are sent from the queue in FIFO order'
-
-        return self.greenApi.request('GET', 
-            '{{host}}/waInstance{{idInstance}}'
-            '/ReceiveNotification/{{apiTokenInstance}}')
-
-    def deleteNotification(self, receiptId: int) -> Response:
-        'The method is aimed for deleting an incoming notification from '\
-        'the notification queue. To specify what notification to delete, '\
-        'use receiptId parameter. After receiving and processing an incoming '\
-        'notification, you need to delete the notification from the queue. '\
-        'This requires you to run this method. After calling the method, '\
-        'the notification will be considered received and processed and '\
-        'will be permanently deleted from the queue. Therefore, the next call '\
-        'of ReceiveNotification method will return the next notification from '\
-        'the queue in the order in which notifications come to the queue.'\
-        'Incoming notifications are stored in the queue for 24 hours.'\
-        'Notifications are sent from the queue in FIFO order'
-
-        return self.greenApi.request('DELETE', 
-            '{{host}}/waInstance{{idInstance}}'
+from whatsapp_api_client_python.response import Response
+
+
+class Receiving:
+    def __init__(self, greenApi) -> None:
+        self.greenApi = greenApi
+        
+    def downloadFile(self, idMessage: str) -> Response:
+        'The method is aimed for downloading incoming and outgoing files. '\
+        'Links to incoming files are transmitted in Incoming messages, '\
+        'and you can also get them using LastIncomingMessages method. '\
+        'You can get links to outgoing files using '\
+        'LastOutgoingMessages method.'\
+        'Files storage period and, accordingly, the capability '\
+        'to download them is limited to 24 hours.'
+
+        requestBody = {
+            'idMessage': idMessage,
+        }
+
+        return self.greenApi.request('POST', 
+            '{{host}}/waInstance{{idInstance}}'
+            '/DownloadFile/{{apiTokenInstance}}',
+            requestBody)
+
+    def receiveNotification(self) -> Response:
+        'The method is aimed for receiving one incoming notification from '\
+        'the notifications queue. '\
+        'ReceiveNotification method waits for a notification receipt '\
+        'for 20 sec. The method call ends with an empty response if a timeout '\
+        'is reached. If a notification comes to the queue within 20 seconds, '\
+        'the method call is completed, and the method returns the received '\
+        'notification.'\
+        'After receiving and processing an incoming notification, you need '\
+        'to delete the notification from the queue. This requires you to run '\
+        'DeleteNotification method. After calling DeleteNotification method, '\
+        'the notification will be considered received and processed and '\
+        'will be permanently deleted from the queue. Therefore, the next call '\
+        'of ReceiveNotification method will return the next notification from '\
+        'the queue in the order in which notifications come to the queue.'\
+        'Incoming notifications are stored in the queue for 24 hours. '\
+        'Notifications are sent from the queue in FIFO order'
+
+        return self.greenApi.request('GET', 
+            '{{host}}/waInstance{{idInstance}}'
+            '/ReceiveNotification/{{apiTokenInstance}}')
+
+    def deleteNotification(self, receiptId: int) -> Response:
+        'The method is aimed for deleting an incoming notification from '\
+        'the notification queue. To specify what notification to delete, '\
+        'use receiptId parameter. After receiving and processing an incoming '\
+        'notification, you need to delete the notification from the queue. '\
+        'This requires you to run this method. After calling the method, '\
+        'the notification will be considered received and processed and '\
+        'will be permanently deleted from the queue. Therefore, the next call '\
+        'of ReceiveNotification method will return the next notification from '\
+        'the queue in the order in which notifications come to the queue.'\
+        'Incoming notifications are stored in the queue for 24 hours.'\
+        'Notifications are sent from the queue in FIFO order'
+
+        return self.greenApi.request('DELETE', 
+            '{{host}}/waInstance{{idInstance}}'
             '/DeleteNotification/{{apiTokenInstance}}/' + str(receiptId))
```

### Comparing `whatsapp-api-client-python-0.0.34/whatsapp_api_client_python/tools/serviceMethods.py` & `whatsapp-api-client-python-0.0.35/whatsapp_api_client_python/tools/serviceMethods.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-from whatsapp_api_client_python.response import Response
-
-
-class ServiceMethods:
-    def __init__(self, greenApi) -> None:
-        self.greenApi = greenApi
-        
-    def checkWhatsapp(self, phoneNumber: int) -> Response:
-            'The method checks WhatsApp account availability on a phone number.'
-
-            requestBody = {
-                'phoneNumber': phoneNumber
-            }
-
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/CheckWhatsapp/{{apiTokenInstance}}',
-                requestBody)
-
-    def getAvatar(self, chatId: str) -> Response:
-            'The method returns a user or a group chat avatar.'
-
-            requestBody = {
-                'chatId': chatId
-            }
-
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/GetAvatar/{{apiTokenInstance}}',
-                requestBody)
-
-    def getContactInfo(self, chatId: str) -> Response:
-            'The method is aimed for getting information on a contact.'
-
-            requestBody = {
-                'chatId': chatId
-            }
-
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/GetContactInfo/{{apiTokenInstance}}',
-                requestBody)
-
-    def getContacts(self) -> Response:
-            'The method is aimed for getting a list of the current account '\
-            'contacts. Sends contacts of all recipients whom the account '\
-            'connected with. Parameter "contact name" "name" takes on '\
-            'a value based on the below criteria: '\
-            'If the account is recorded in the phonebook, then we get the '\
-            'name from the book; '\
-            'If the account is not recorded in the phonebook, then we get '\
-            'the name from WhatsApp account;'\
-            'If the account is not recorded in the phone book and WhatsApp '\
-            'account name is not assigned, then we get an empty field.'
-
-            return self.greenApi.request('GET', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/GetContacts/{{apiTokenInstance}}')
-
-    def archiveChat(self, chatId: str) -> Response:
-            'The method archives a chat. You can archive chats that have at '\
-            'least one incoming message.'
-
-            requestBody = {
-                'chatId': chatId
-            }
-
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/ArchiveChat/{{apiTokenInstance}}',
-                requestBody)
-
-    def deleteMessage(self, chatId: str, idMessage: str) -> Response:
-            'The method deletes a message from a chat.'
-
-            requestBody = {
-                'chatId': chatId,
-                'idMessage': idMessage
-            }
-
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/DeleteMessage/{{apiTokenInstance}}',
-                requestBody)
-
-    def unarchiveChat(self, chatId: str) -> Response:
-            'The method deletes a message from a chat.'
-
-            requestBody = {
-                'chatId': chatId
-            }
-
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/UnarchiveChat/{{apiTokenInstance}}',
-                requestBody)
-
-    def setDisappearingChat(self, chatId: str, 
-                            ephemeralExpiration: int) -> Response:
-            'The method is aimed for changing settings of disappearing '\
-            'messages in chats. The standard settings of the application '\
-            'are used: 0 (off), 86400 (24 hours), '\
-            '604800 (7 days), 7776000 (90 days).'
-
-            requestBody = {
-                'chatId': chatId,
-                'ephemeralExpiration': ephemeralExpiration
-            }
-
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/SetDisappearingChat/{{apiTokenInstance}}',
+from whatsapp_api_client_python.response import Response
+
+
+class ServiceMethods:
+    def __init__(self, greenApi) -> None:
+        self.greenApi = greenApi
+        
+    def checkWhatsapp(self, phoneNumber: int) -> Response:
+            'The method checks WhatsApp account availability on a phone number.'
+
+            requestBody = {
+                'phoneNumber': phoneNumber
+            }
+
+            return self.greenApi.request('POST', 
+                '{{host}}/waInstance{{idInstance}}'
+                '/CheckWhatsapp/{{apiTokenInstance}}',
+                requestBody)
+
+    def getAvatar(self, chatId: str) -> Response:
+            'The method returns a user or a group chat avatar.'
+
+            requestBody = {
+                'chatId': chatId
+            }
+
+            return self.greenApi.request('POST', 
+                '{{host}}/waInstance{{idInstance}}'
+                '/GetAvatar/{{apiTokenInstance}}',
+                requestBody)
+
+    def getContactInfo(self, chatId: str) -> Response:
+            'The method is aimed for getting information on a contact.'
+
+            requestBody = {
+                'chatId': chatId
+            }
+
+            return self.greenApi.request('POST', 
+                '{{host}}/waInstance{{idInstance}}'
+                '/GetContactInfo/{{apiTokenInstance}}',
+                requestBody)
+
+    def getContacts(self) -> Response:
+            'The method is aimed for getting a list of the current account '\
+            'contacts. Sends contacts of all recipients whom the account '\
+            'connected with. Parameter "contact name" "name" takes on '\
+            'a value based on the below criteria: '\
+            'If the account is recorded in the phonebook, then we get the '\
+            'name from the book; '\
+            'If the account is not recorded in the phonebook, then we get '\
+            'the name from WhatsApp account;'\
+            'If the account is not recorded in the phone book and WhatsApp '\
+            'account name is not assigned, then we get an empty field.'
+
+            return self.greenApi.request('GET', 
+                '{{host}}/waInstance{{idInstance}}'
+                '/GetContacts/{{apiTokenInstance}}')
+
+    def archiveChat(self, chatId: str) -> Response:
+            'The method archives a chat. You can archive chats that have at '\
+            'least one incoming message.'
+
+            requestBody = {
+                'chatId': chatId
+            }
+
+            return self.greenApi.request('POST', 
+                '{{host}}/waInstance{{idInstance}}'
+                '/ArchiveChat/{{apiTokenInstance}}',
+                requestBody)
+
+    def deleteMessage(self, chatId: str, idMessage: str) -> Response:
+            'The method deletes a message from a chat.'
+
+            requestBody = {
+                'chatId': chatId,
+                'idMessage': idMessage
+            }
+
+            return self.greenApi.request('POST', 
+                '{{host}}/waInstance{{idInstance}}'
+                '/DeleteMessage/{{apiTokenInstance}}',
+                requestBody)
+
+    def unarchiveChat(self, chatId: str) -> Response:
+            'The method deletes a message from a chat.'
+
+            requestBody = {
+                'chatId': chatId
+            }
+
+            return self.greenApi.request('POST', 
+                '{{host}}/waInstance{{idInstance}}'
+                '/UnarchiveChat/{{apiTokenInstance}}',
+                requestBody)
+
+    def setDisappearingChat(self, chatId: str, 
+                            ephemeralExpiration: int) -> Response:
+            'The method is aimed for changing settings of disappearing '\
+            'messages in chats. The standard settings of the application '\
+            'are used: 0 (off), 86400 (24 hours), '\
+            '604800 (7 days), 7776000 (90 days).'
+
+            requestBody = {
+                'chatId': chatId,
+                'ephemeralExpiration': ephemeralExpiration
+            }
+
+            return self.greenApi.request('POST', 
+                '{{host}}/waInstance{{idInstance}}'
+                '/SetDisappearingChat/{{apiTokenInstance}}',
                 requestBody)
```

### Comparing `whatsapp-api-client-python-0.0.34/whatsapp_api_client_python.egg-info/PKG-INFO` & `whatsapp-api-client-python-0.0.35/whatsapp_api_client_python.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,199 +1,216 @@
-Metadata-Version: 2.1
-Name: whatsapp-api-client-python
-Version: 0.0.34
-Summary: This library helps you easily create a python '        'application to connect the WhatsApp API using service green-api.com
-Home-page: https://github.com/green-api/whatsapp-api-client-python
-Author: Ivan Sadovy
-Author-email: sadiv@bk.ru
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-﻿# whatsapp-api-client-python
-
-[![Python application](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-app.yml/badge.svg)](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-app.yml)
-[![Upload Python Package](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-publish.yml/badge.svg)](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-publish.yml)
-
-- [Документация на русском языке](README_RUS.md)
-
-Python library for intagration with WhatsAPP messanger via API of [green-api.com](https://green-api.com) service. To use the library you have to get a registration token and an account id in the [personal area](https://console.green-api.com). There is a free developer account tariff plan.
-
-## API
-
-You can find REST API documentation by [url](https://green-api.com/docs/api/). The library is a wrapper for REST API, so the documentation at the above url applies to the library as well.
-
-## Installation
-
-```shell
-pip install whatsapp-api-client-python
-```
-
-## Import 
-
-```
-from whatsapp_api_client_python import API
-```
-## Authorization
-
-To send a message or to exacute some other Green-API method, you have to have the WhatsApp account in the phone application to be authorized. To authorize your account please go to the [personal area](https://console.green-api.com) and scan a QR-code using the WhatsApp application.
-
-## Examples
-
-### How to initialize an object
-
-```python
-greenAPI = API.GreenApi(ID_INSTANCE, API_TOKEN_INSTANCE)
-```
-
-### Sending a text message to a WhatsApp number
-
-```python
-result = greenAPI.sending.sendMessage('79001234567@g.us', 'Message text')
-```
-
-Example url: [sendTextMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendTextMessage.py)
-
-Please note that keys can be obtained from environment variables:
-```python
-from os import environ
-
-ID_INSTANCE = environ['ID_INSTANCE']
-API_TOKEN_INSTANCE = environ['API_TOKEN_INSTANCE']
-```
-
-### Sending an image via URL
-
-```python
-result = greenAPI.sending.sendFileByUrl('120363025955348359@g.us', 
-        'https://www.google.ru/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png', 
-        'googlelogo_color_272x92dp.png', 'Google logo')
-```
-
-Example url: [sendPictureByLink.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByLink.py)
-
-### Sending an image by uploading from the disk
-
-```python
-result = greenAPI.sending.sendFileByUpload('120363025955348359@g.us', 
-        'C:\Games\PicFromDisk.png', 
-        'PicFromDisk.png', 'Picture from disk')
-```
-
-Example url: [sendPictureByUpload.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByUpload.py)
-
-### Group creation and sending a message to the group
-
-```python
-chatIds = [
-    "79001234567@c.us"
-]
-resultCreate = greenAPI.groups.createGroup('GroupName', 
-    chatIds)
-
-if resultCreate.code == 200:
-    resultSend = greenAPI.sending.sendMessage(resultCreate.data['chatId'], 
-        'Message text')
-```
-
-IMPORTANT: If one tries to create a group with a non-existent number, WhatsApp 
-may block the sender's number. The number in the example is non-existent.
-
-Example url: [createGroupAndSendMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/createGroupAndSendMessage.py)
-
-### Receive incoming messages by HTTP API
-
-The general concept of receiving data in the Green API is described [here](https://green-api.com/en/docs/api/receiving/)
-To start receiving messages by the HTTP API you need to execute the library method:
-
-```python
-greenAPI.webhooks.startReceivingNotifications(onEvent)
-```
-
-onEvent - your method which should contain parameters:
-Parameter | Description
------ | -----
-typewebhook | received message type (string)
-body | message body (json)
-
-Message body types and formats [here](https://green-api.com/en/docs/api/receiving/notifications-format/)
-
-This method will be called when an incoming message is received. Next, process messages according to the business logic of your system.
-
-## Examples list
-
-Description |  Module
------ | ----- 
-Example of sending text | [sendTextMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendTextMessage.py)
-Example of sending a picture by URL | [sendPictureByLink.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByLink.py)
-Example of sending a picture by uploading from the disk | [sendPictureByUpload.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByUpload.py)
-Example of a group creation and sending a message to the group | [createGroupAndSendMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/createGroupAndSendMessage.py)
-Example of incoming webhooks receiving | [receiveNotification.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/receiveNotification.py)
-
-
-## The full list of the library methods
-
-| Method                                 | Description                                                                                                                                                                                         | Documentation                                                                                                                            |
-|----------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------|
-| `account.getSettings`                  | The method is aimed for getting the current settings of the account                                                                                                                                 | [GetSettings.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/GetSettings.md)                                       |
-| `account.getStateInstance`             | The method is aimed for getting the account state                                                                                                                                                   | [GetStateInstance.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/GetStateInstance.md)                             |
-| `account.getStatusInstance`            | The method is aimed for getting the status of the account instance socket connection with WhatsApp                                                                                                  | [GetStatusInstance.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/GetStatusInstance.md)                           |
-| `account.logout`                       | The method is aimed for logging out an account                                                                                                                                                      | [Logout.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/Logout.md)                                                 |
-| `account.qr`                           | The method is aimed for getting QR code                                                                                                                                                             | [QR.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/QR.md)                                                         |
-| `account.reboot`                       | The method is aimed for rebooting an account                                                                                                                                                        | [Reboot.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/Reboot.md)                                                 |
-| `account.setProfilePicture`            | The method is aimed for setting an account picture                                                                                                                                                  | [SetProfilePicture.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/SetProfilePicture.md)                           |
-| `account.setSettings`                  | The method is aimed for setting an account settings                                                                                                                                                 | [SetSettings.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/SetSettings.md)                                       |
-| `account.setSystemProxy`               | The method is aimed for setting a system proxy. Use the method when you need to reset custom proxy settings to system ones                                                                          | [SetSystemProxy.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/SetSystemProxy.md)                                 |
-| `groups.addGroupParticipant`           | Метод добавляет участника в групповой чат                                                                                                                                                           | [AddGroupParticipant.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/AddGroupParticipant.md)                        |
-| `groups.createGroup`                   | The method adds a participant to a group chat. IMPORTANT: If one tries to create a group with a non-existent number, WhatsApp may block the sender's number.                                        | [CreateGroup.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/CreateGroup.md)                                        |
-| `groups.getGroupData`                  | The method gets group chat data                                                                                                                                                                     | [GetGroupData.md](https://github.com/green-api/docs/blob/master/ru/docs/api/account/GetGroupData.md)                                     |
-| `groups.leaveGroup`                    | The method makes the current account user leave the group chat                                                                                                                                      | [LeaveGroup.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/LeaveGroup.md)                                          |
-| `groups.removeAdmin`                   | he method removes a participant from group chat administration rights                                                                                                                               | [RemoveAdmin.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/RemoveAdmin.md)                                        |
-| `groups.removeGroupParticipant`        | The method removes a participant from a group chat                                                                                                                                                  | [RemoveGroupParticipant.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/RemoveGroupParticipant.md)                  |
-| `groups.setGroupAdmin`                 | The method sets a group chat participant as an administrator                                                                                                                                        | [SetGroupAdmin.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/SetGroupAdmin.md)                                    |
-| `groups.setGroupPicture`               | The method sets a group picture                                                                                                                                                                     | [SetGroupPicture.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/SetGroupPicture.md)                                |
-| `groups.updateGroupName`               | The method changes a group chat name                                                                                                                                                                | [UpdateGroupName.md](https://github.com/green-api/docs/blob/master/ru/docs/api/groups/UpdateGroupName.md)                                |
-| `journals.getChatHistory`              | The method returns the chat message history                                                                                                                                                         | [GetChatHistory.md](https://github.com/green-api/docs/blob/master/ru/docs/api/journals/GetChatHistory.md)                                |
-| `journals.lastIncomingMessages`        | The method returns the last incoming messages of the account. In the default mode the incoming messages for 24 hours are returned                                                                   | [GetChatHistory.md](https://github.com/green-api/docs/blob/master/ru/docs/api/journals/LastIncomingMessages.md)                          |
-| `journals.lastOutgoingMessages`        | The method returns the last outgoing messages of the account. In the default mode the last messages for 24 hours are returned                                                                       | [LastOutgoingMessages.md](https://github.com/green-api/docs/blob/master/ru/docs/api/journals/LastOutgoingMessages.md)                    |
-| `marking.readChat`                     | The method is aimed for marking messages in a chat as read. Either all messages or a specified message in a chat can be marked as read                                                              | [ReadChat.md](https://github.com/green-api/docs/blob/master/ru/docs/api/marks/ReadChat.md)                                               |
-| `device.getDeviceInfo`                 | The method is aimed for getting information about the device (phone) running WhatsApp Business application                                                                                          | [GetDeviceInfo.md](https://github.com/green-api/docs/blob/master/ru/docs/api/phone/GetDeviceInfo.md)                                     |
-| `queues.clearMessagesQueue`            | The method is aimed for clearing the queue of messages to be sent                                                                                                                                   | [ClearMessagesQueue.md](https://github.com/green-api/docs/blob/master/ru/docs/api/queues/ClearMessagesQueue.md)                          |
-| `queues.showMessagesQueue`             | The method is aimed for getting a list of messages in the queue to be sent                                                                                                                          | [ShowMessagesQueue.md](https://github.com/green-api/docs/blob/master/ru/docs/api/queues/ShowMessagesQueue.md)                            |
-| `receiving.deleteNotification`         | The method is aimed for deleting an incoming notification from the notification queue                                                                                                               | [DeleteNotification.md](https://github.com/green-api/docs/blob/master/ru/docs/api/receiving/technology-http-api/DeleteNotification.md)   |
-| `receiving.receiveNotification`        | The method is aimed for receiving one incoming notification from the notifications queue                                                                                                            | [ReceiveNotification.md](https://github.com/green-api/docs/blob/master/ru/docs/api/receiving/technology-http-api/ReceiveNotification.md) |
-| `sending.sendButtons`                  | The method is aimed for sending a button message to a personal or a group chat                                                                                                                      | [SendButtons.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendButtons.md)                                       |
-| `sending.sendContact`                  | The method is aimed for sending a contact message                                                                                                                                                   | [SendContact.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendContact.md)                                       |
-| `sending.sendFileByUpload`             | The method is aimed for sending a file uploaded by form                                                                                                                                             | [SendFileByUpload.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendFileByUpload.md)                             |
-| `sending.sendFileByUrl`                | The method is aimed for sending a file uploaded by Url                                                                                                                                              | [SendFileByUrl.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendFileByUrl.md)                                   |
-| `sending.sendLink`                     | The method is aimed for sending a message with a link, by which an image preview, title and description will be added                                                                               | [SendLink.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendLink.md)                                             |
-| `sending.sendListMessage`              | The method is aimed for sending a message with a select button from a list of values to a personal or a group chat                                                                                  | [SendListMessage.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendListMessage.md)                               |
-| `sending.sendLocation`                 | The method is aimed for sending a location message                                                                                                                                                  | [SendLocation.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendLocation.md)                                     |
-| `sending.sendMessage`                  | The method is aimed for sending a text message to a personal or a group chat                                                                                                                        | [SendMessage.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendMessage.md)                                       |
-| `sending.sendTemplateButtons`          | The method is aimed for sending a message with template list interactive buttons to a personal or a group chat                                                                                      | [SendTemplateButtons.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/SendTemplateButtons.md)                       |
-| `sending.forwardMessages`              | The method is intended for forwarding messages to a personal or group chat                                                                                                                          | [ForwardMessages.md](https://github.com/green-api/docs/blob/master/ru/docs/api/sending/ForwardMessages.md)                               |
-| `serviceMethods.checkWhatsapp`         | The method checks WhatsApp account availability on a phone number                                                                                                                                   | [CheckWhatsapp.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/CheckWhatsapp.md)                                   |
-| `serviceMethods.getAvatar`             | The method returns a user or a group chat avatar                                                                                                                                                    | [GetAvatar.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/GetAvatar.md)                                           |
-| `serviceMethods.getContactInfo`        | The method is aimed for getting information on a contact                                                                                                                                            | [GetContactInfo.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/GetContactInfo.md)                                 |
-| `serviceMethods.getContacts`           | The method is aimed for getting a list of the current account contacts                                                                                                                              | [GetContacts.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/GetContacts.md)                                       |
-| `serviceMethods.setDisappearingChat`   | The method is aimed for changing settings of disappearing messages in chats. The standard settings of the application are to be used: 0 (off), 86400 (24 hours), 604800 (7 days), 7776000 (90 days) | [SetDisappearingChat.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/SetDisappearingChat.md)                       |
-| `serviceMethods.archiveChat`           | The method archives a chat. One can archive chats that have at least one incoming message                                                                                                           | [ArchiveChat.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/ArchiveChat.md)                                       |
-| `serviceMethods.deleteMessage`         | The method deletes a message from a chat                                                                                                                                                            | [DeleteMessage.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/deleteMessage.md)                                   |
-| `serviceMethods.unarchiveChat`         | The method unarchives a chat                                                                                                                                                                        | [UnarchiveChat.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/UnarchiveChat.md)                                   |
-| `serviceMethods.setDisappearingChat`   | The method is aimed for changing settings of disappearing messages in chats                                                                                                                         | [SetDisappearingChat.md](https://github.com/green-api/docs/blob/master/ru/docs/api/service/SetDisappearingChat.md)                       |
-| `webhooks.startReceivingNotifications` | The method is aimed for starting to receive webhooks                                                                                                                                                | <library method>                                                                                                                         |
-| `webhooks.stopReceivingNotifications`  | The method is aimed for stopping to receive webhooks                                                                                                                                                | <library method>                                                                                                                         |
-
-## Service methods documentation
-
-[https://green-api.com/en/docs/api/](https://green-api.com/en/docs/api/)
-
-## External products
-
-* [requests](https://requests.readthedocs.io) - for http requests
-
-## License
-
-Licensed under MIT terms. Please see file [LICENSE](LICENSE)
+Metadata-Version: 2.1
+Name: whatsapp-api-client-python
+Version: 0.0.35
+Summary: This library helps you easily create a Python application with WhatsApp API.
+Home-page: https://github.com/green-api/whatsapp-api-client-python
+Author: GREEN API
+Author-email: support@green-api.com
+License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+﻿# whatsapp-api-client-python
+
+[![Python application](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-app.yml/badge.svg)](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-app.yml)
+[![Upload Python Package](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-publish.yml/badge.svg)](https://github.com/green-api/whatsapp-api-client-python/actions/workflows/python-publish.yml)
+
+- [Документация на русском языке](README_RUS.md)
+
+Python library for intagration with WhatsAPP messanger via API of [green-api.com](https://green-api.com/en/) service. To use the library you have to get a registration token and an account id in the [personal area](https://console.green-api.com). There is a free developer account tariff plan.
+
+## API
+
+You can find REST API documentation by [url](https://green-api.com/en/docs/api/). The library is a wrapper for REST API, so the documentation at the above url applies to the library as well.
+
+## Installation
+
+```shell
+pip install whatsapp-api-client-python
+```
+
+## Import 
+
+```
+from whatsapp_api_client_python import API
+```
+## Authorization
+
+To send a message or to exacute some other Green-API method, you have to have the WhatsApp account in the phone application to be authorized. To authorize your account please go to the [personal area](https://console.green-api.com) and scan a QR-code using the WhatsApp application.
+
+## Examples
+
+### How to initialize an object
+
+```python
+greenAPI = API.GreenApi(ID_INSTANCE, API_TOKEN_INSTANCE)
+```
+
+### Sending a text message to a WhatsApp number
+
+```python
+result = greenAPI.sending.sendMessage('79001234567@g.us', 'Message text')
+```
+
+Example url: [sendTextMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendTextMessage.py)
+
+Please note that keys can be obtained from environment variables:
+```python
+from os import environ
+
+ID_INSTANCE = environ['ID_INSTANCE']
+API_TOKEN_INSTANCE = environ['API_TOKEN_INSTANCE']
+```
+
+### Sending an image via URL
+
+```python
+result = greenAPI.sending.sendFileByUrl('120363025955348359@g.us', 
+        'https://www.google.ru/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png', 
+        'googlelogo_color_272x92dp.png', 'Google logo')
+```
+
+Example url: [sendPictureByLink.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByLink.py)
+
+### Sending an image by uploading from the disk
+
+```python
+result = greenAPI.sending.sendFileByUpload('120363025955348359@g.us', 
+        'C:\Games\PicFromDisk.png', 
+        'PicFromDisk.png', 'Picture from disk')
+```
+
+Example url: [sendPictureByUpload.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByUpload.py)
+
+### Group creation and sending a message to the group
+
+```python
+chatIds = [
+    "79001234567@c.us"
+]
+resultCreate = greenAPI.groups.createGroup('GroupName', 
+    chatIds)
+
+if resultCreate.code == 200:
+    resultSend = greenAPI.sending.sendMessage(resultCreate.data['chatId'], 
+        'Message text')
+```
+
+IMPORTANT: If one tries to create a group with a non-existent number, WhatsApp 
+may block the sender's number. The number in the example is non-existent.
+
+Example url: [createGroupAndSendMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/createGroupAndSendMessage.py)
+
+### Receive incoming messages by HTTP API
+
+The general concept of receiving data in the Green API is described [here](https://green-api.com/en/docs/api/receiving/)
+To start receiving messages by the HTTP API you need to execute the library method:
+
+```python
+greenAPI.webhooks.startReceivingNotifications(onEvent)
+```
+
+onEvent - your method which should contain parameters:
+Parameter | Description
+----- | -----
+typewebhook | received message type (string)
+body | message body (json)
+
+Message body types and formats [here](https://green-api.com/en/docs/api/receiving/notifications-format/)
+
+This method will be called when an incoming message is received. Next, process messages according to the business logic of your system.
+
+## Examples list
+
+Description |  Module
+----- | ----- 
+Example of sending text | [sendTextMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendTextMessage.py)
+Example of sending a picture by URL | [sendPictureByLink.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByLink.py)
+Example of sending a picture by uploading from the disk | [sendPictureByUpload.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/sendPictureByUpload.py)
+Example of a group creation and sending a message to the group | [createGroupAndSendMessage.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/createGroupAndSendMessage.py)
+Example of incoming webhooks receiving | [receiveNotification.py](https://github.com/green-api/whatsapp-api-client-python/blob/master/examples/receiveNotification.py)
+
+
+## The full list of the library methods
+
+| API method                             | Description                                                                                                              | Documentation link                                                                                          |
+|----------------------------------------|--------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|
+| `account.getSettings`                  | The method is designed to get the current settings of the account                                                        | [GetSettings](https://green-api.com/en/docs/api/account/GetSettings/)                                       |
+| `account.setSettings`                  | The method is designed to set the account settings                                                                       | [SetSettings](https://green-api.com/en/docs/api/account/SetSettings/)                                       |
+| `account.getStateInstance`             | The method is designed to get the state of the account                                                                   | [GetStateInstance](https://green-api.com/en/docs/api/account/GetStateInstance/)                             |
+| `account.getStatusInstance`            | The method is designed to get the socket connection state of the account instance with WhatsApp                          | [GetStatusInstance](https://green-api.com/en/docs/api/account/GetStatusInstance/)                           |
+| `account.reboot`                       | The method is designed to restart the account                                                                            | [Reboot](https://green-api.com/en/docs/api/account/Reboot/)                                                 |
+| `account.logout`                       | The method is designed to unlogin the account                                                                            | [Logout](https://green-api.com/en/docs/api/account/Logout/)                                                 |
+| `account.qr`                           | The method is designed to get a QR code                                                                                  | [QR](https://green-api.com/en/docs/api/account/QR/)                                                         |
+| `account.setProfilePicture`            | The method is designed to set the avatar of the account                                                                  | [SetProfilePicture](https://green-api.com/en/docs/api/account/SetProfilePicture/)                           |
+| `device.getDeviceInfo`                 | The method is designed to get information about the device (phone) on which the WhatsApp Business application is running | [GetDeviceInfo](https://green-api.com/en/docs/api/phone/GetDeviceInfo/)                                     |
+| `groups.createGroup`                   | The method is designed to create a group chat                                                                            | [CreateGroup](https://green-api.com/en/docs/api/groups/CreateGroup/)                                        |
+| `groups.updateGroupName`               | The method changes the name of the group chat                                                                            | [UpdateGroupName](https://green-api.com/en/docs/api/groups/UpdateGroupName/)                                |
+| `groups.getGroupData`                  | The method gets group chat data                                                                                          | [GetGroupData](https://green-api.com/en/docs/api/groups/GetGroupData/)                                      |
+| `groups.addGroupParticipant`           | The method adds a participant to the group chat                                                                          | [AddGroupParticipant](https://green-api.com/en/docs/api/groups/AddGroupParticipant/)                        |
+| `groups.removeGroupParticipant`        | The method removes the participant from the group chat                                                                   | [RemoveGroupParticipant](https://green-api.com/en/docs/api/groups/RemoveGroupParticipant/)                  |
+| `groups.setGroupAdmin`                 | The method designates a member of a group chat as an administrator                                                       | [SetGroupAdmin](https://green-api.com/en/docs/api/groups/SetGroupAdmin/)                                    |
+| `groups.removeAdmin`                   | The method deprives the participant of group chat administration rights                                                  | [RemoveAdmin](https://green-api.com/en/docs/api/groups/RemoveAdmin/)                                        |
+| `groups.setGroupPicture`               | The method sets the avatar of the group                                                                                  | [SetGroupPicture](https://green-api.com/en/docs/api/groups/SetGroupPicture/)                                |
+| `groups.leaveGroup`                    | The method logs the user of the current account out of the group chat                                                    | [LeaveGroup](https://green-api.com/en/docs/api/groups/LeaveGroup/)                                          |
+| `journals.getChatHistory`              | The method returns the chat message history                                                                              | [GetChatHistory](https://green-api.com/en/docs/api/journals/GetChatHistory/)                                |
+| `journals.getMessage`                  | The method returns a chat message                                                                                        | [GetMessage](https://green-api.com/en/docs/api/journals/GetMessage/)                                        |
+| `journals.lastIncomingMessages`        | The method returns the most recent incoming messages of the account                                                      | [LastIncomingMessages](https://green-api.com/en/docs/api/journals/LastIncomingMessages/)                    |
+| `journals.lastOutgoingMessages`        | The method returns the last sent messages of the account                                                                 | [LastOutgoingMessages](https://green-api.com/en/docs/api/journals/LastOutgoingMessages/)                    |
+| `queues.showMessagesQueue`             | The method is designed to get the list of messages that are in the queue to be sent                                      | [ShowMessagesQueue](https://green-api.com/en/docs/api/queues/ShowMessagesQueue/)                            |
+| `queues.clearMessagesQueue`            | The method is designed to clear the queue of messages to be sent                                                         | [ClearMessagesQueue](https://green-api.com/en/docs/api/queues/ClearMessagesQueue/)                          |
+| `marking.readChat`                     | The method is designed to mark chat messages as read                                                                     | [ReadChat](https://green-api.com/en/docs/api/marks/ReadChat/)                                               |
+| `receiving.receiveNotification`        | The method is designed to receive a single incoming notification from the notification queue                             | [ReceiveNotification](https://green-api.com/en/docs/api/receiving/technology-http-api/ReceiveNotification/) |
+| `receiving.deleteNotification`         | The method is designed to remove an incoming notification from the notification queue                                    | [DeleteNotification](https://green-api.com/en/docs/api/receiving/technology-http-api/DeleteNotification/)   |
+| `receiving.downloadFile`               | The method is for downloading received and sent files                                                                    | [DownloadFile](https://green-api.com/en/docs/api/receiving/files/DownloadFile/)                             |
+| `sending.sendMessage`                  | The method is designed to send a text message to a personal or group chat                                                | [SendMessage](https://green-api.com/en/docs/api/sending/SendMessage/)                                       |
+| `sending.sendButtons`                  | The method is designed to send a message with buttons to a personal or group chat                                        | [SendButtons](https://green-api.com/en/docs/api/sending/SendButtons/)                                       |
+| `sending.sendTemplateButtons`          | The method is designed to send a message with interactive buttons from the list of templates in a personal or group chat | [SendTemplateButtons](https://green-api.com/en/docs/api/sending/SendTemplateButtons/)                       |
+| `sending.sendListMessage`              | The method is designed to send a message with a selection button from a list of values to a personal or group chat       | [SendListMessage](https://green-api.com/en/docs/api/sending/SendListMessage/)                               |
+| `sending.sendFileByUpload`             | The method is designed to send a file loaded through a form (form-data)                                                  | [SendFileByUpload](https://green-api.com/en/docs/api/sending/SendFileByUpload/)                             |
+| `sending.sendFileByUrl`                | The method is designed to send a file downloaded via a link                                                              | [SendFileByUrl](https://green-api.com/en/docs/api/sending/SendFileByUrl/)                                   |
+| `sending.sendLocation`                 | The method is designed to send a geolocation message                                                                     | [SendLocation](https://green-api.com/en/docs/api/sending/SendLocation/)                                     |
+| `sending.sendContact`                  | The method is for sending a message with a contact                                                                       | [SendContact](https://green-api.com/en/docs/api/sending/SendContact/)                                       |
+| `sending.sendLink`                     | The method is designed to send a message with a link that will add an image preview, title and description               | [SendLink](https://green-api.com/en/docs/api/sending/SendLink/)                                             |
+| `sending.forwardMessages`              | The method is designed for forwarding messages to a personal or group chat                                               | [ForwardMessages](https://green-api.com/en/docs/api/sending/ForwardMessages/)                               |
+| `serviceMethods.checkWhatsapp`         | The method checks if there is a WhatsApp account on the phone number                                                     | [CheckWhatsapp](https://green-api.com/en/docs/api/service/CheckWhatsapp/)                                   |
+| `serviceMethods.getAvatar`             | The method returns the avatar of the correspondent or group chat                                                         | [GetAvatar](https://green-api.com/en/docs/api/service/GetAvatar/)                                           |
+| `serviceMethods.getContacts`           | The method is designed to get a list of contacts of the current account                                                  | [GetContacts](https://green-api.com/en/docs/api/service/GetContacts/)                                       |
+| `serviceMethods.getContactInfo`        | The method is designed to obtain information about the contact                                                           | [GetContactInfo](https://green-api.com/en/docs/api/service/GetContactInfo/)                                 |
+| `serviceMethods.deleteMessage`         | The method deletes the message from chat                                                                                 | [DeleteMessage](https://green-api.com/en/docs/api/service/deleteMessage/)                                   |
+| `serviceMethods.archiveChat`           | The method archives the chat                                                                                             | [ArchiveChat](https://green-api.com/en/docs/api/service/archiveChat/)                                       |
+| `serviceMethods.unarchiveChat`         | The method unarchives the chat                                                                                           | [UnarchiveChat](https://green-api.com/en/docs/api/service/unarchiveChat/)                                   |
+| `serviceMethods.setDisappearingChat`   | The method is designed to change the settings of disappearing messages in chats                                          | [SetDisappearingChat](https://green-api.com/en/docs/api/service/SetDisappearingChat/)                       |
+| `webhooks.startReceivingNotifications` | The method is designed to start receiving new notifications                                                              |                                                                                                             |
+| `webhooks.stopReceivingNotifications`  | The method is designed to stop receiving new notifications                                                               |                                                                                                             |
+
+## Service methods documentation
+
+[https://green-api.com/en/docs/api/](https://green-api.com/en/docs/api/)
+
+## External products
+
+* [requests](https://requests.readthedocs.io) - for http requests
+
+## License
+
+[![CC BY-ND 4.0][cc-by-nd-shield]][cc-by-nd]
+
+This work is licensed under a
+[Creative Commons Attribution-NoDerivatives 4.0 International License][cc-by-nd].
+
+[cc-by-nd]: https://creativecommons.org/licenses/by-nd/4.0/
+[cc-by-nd-shield]: https://img.shields.io/badge/License-CC%20BY--ND%204.0-lightgrey.svg
+
+Please see file [LICENSE](LICENSE)
```

### Comparing `whatsapp-api-client-python-0.0.34/whatsapp_api_client_python.egg-info/SOURCES.txt` & `whatsapp-api-client-python-0.0.35/whatsapp_api_client_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

