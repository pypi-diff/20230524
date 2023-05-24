# Comparing `tmp/neon_speech-3.3.2a4-py3-none-any.whl.zip` & `tmp/neon_speech-3.3.2a5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 23741 bytes, number of entries: 14
--rw-r--r--  2.0 unx     1831 b- defN 23-May-18 05:37 neon_speech/__init__.py
--rw-r--r--  2.0 unx     2915 b- defN 23-May-18 05:37 neon_speech/__main__.py
--rw-r--r--  2.0 unx     5085 b- defN 23-May-18 05:37 neon_speech/cli.py
--rw-r--r--  2.0 unx     9921 b- defN 23-May-18 05:37 neon_speech/listener.py
--rw-r--r--  2.0 unx     5107 b- defN 23-May-18 05:37 neon_speech/mic.py
--rw-r--r--  2.0 unx    21918 b- defN 23-May-18 05:37 neon_speech/service.py
--rw-r--r--  2.0 unx     4478 b- defN 23-May-18 05:37 neon_speech/stt.py
--rw-r--r--  2.0 unx     4285 b- defN 23-May-18 05:37 neon_speech/utils.py
--rw-r--r--  2.0 unx     1634 b- defN 23-May-18 05:37 neon_speech-3.3.2a4.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2587 b- defN 23-May-18 05:37 neon_speech-3.3.2a4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-18 05:37 neon_speech-3.3.2a4.dist-info/WHEEL
--rw-r--r--  2.0 unx      111 b- defN 23-May-18 05:37 neon_speech-3.3.2a4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-May-18 05:37 neon_speech-3.3.2a4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1143 b- defN 23-May-18 05:37 neon_speech-3.3.2a4.dist-info/RECORD
-14 files, 61119 bytes uncompressed, 21849 bytes compressed:  64.3%
+Zip file size: 23742 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     1831 b- defN 23-May-24 19:42 neon_speech/__init__.py
+-rw-r--r--  2.0 unx     2914 b- defN 23-May-24 19:42 neon_speech/__main__.py
+-rw-r--r--  2.0 unx     5085 b- defN 23-May-24 19:42 neon_speech/cli.py
+-rw-r--r--  2.0 unx     9921 b- defN 23-May-24 19:42 neon_speech/listener.py
+-rw-r--r--  2.0 unx     5107 b- defN 23-May-24 19:42 neon_speech/mic.py
+-rw-r--r--  2.0 unx    21917 b- defN 23-May-24 19:42 neon_speech/service.py
+-rw-r--r--  2.0 unx     4478 b- defN 23-May-24 19:42 neon_speech/stt.py
+-rw-r--r--  2.0 unx     4285 b- defN 23-May-24 19:42 neon_speech/utils.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-May-24 19:42 neon_speech-3.3.2a5.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2587 b- defN 23-May-24 19:42 neon_speech-3.3.2a5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-24 19:42 neon_speech-3.3.2a5.dist-info/WHEEL
+-rw-r--r--  2.0 unx      111 b- defN 23-May-24 19:42 neon_speech-3.3.2a5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-May-24 19:42 neon_speech-3.3.2a5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1143 b- defN 23-May-24 19:42 neon_speech-3.3.2a5.dist-info/RECORD
+14 files, 61117 bytes uncompressed, 21850 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: neon_speech/stt.py
 Comment: 
 
 Filename: neon_speech/utils.py
 Comment: 
 
-Filename: neon_speech-3.3.2a4.dist-info/LICENSE.md
+Filename: neon_speech-3.3.2a5.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_speech-3.3.2a4.dist-info/METADATA
+Filename: neon_speech-3.3.2a5.dist-info/METADATA
 Comment: 
 
-Filename: neon_speech-3.3.2a4.dist-info/WHEEL
+Filename: neon_speech-3.3.2a5.dist-info/WHEEL
 Comment: 
 
-Filename: neon_speech-3.3.2a4.dist-info/entry_points.txt
+Filename: neon_speech-3.3.2a5.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_speech-3.3.2a4.dist-info/top_level.txt
+Filename: neon_speech-3.3.2a5.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_speech-3.3.2a4.dist-info/RECORD
+Filename: neon_speech-3.3.2a5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_speech/__main__.py

```diff
@@ -41,15 +41,15 @@
     if kwargs.get("config"):
         LOG.warning("Found config kwarg, updating to 'speech_config'")
         kwargs["speech_config"] = kwargs.pop("config")
 
     from ovos_utils.process_utils import reset_sigint_handler
     from neon_speech.service import NeonSpeechClient
     reset_sigint_handler()
-    Lock("speech")
+    Lock("voice")
     malloc_running = start_malloc(stack_depth=4)
     service = NeonSpeechClient(*args, **kwargs)
     service.start()
     wait_for_exit_signal()
     if malloc_running:
         try:
             print_malloc(snapshot_malloc())
```

## neon_speech/service.py

```diff
@@ -108,15 +108,15 @@
         self.config = Configuration()
         self.lock = Lock()
 
         callbacks = StatusCallbackMap(on_ready=ready_hook, on_error=error_hook,
                                       on_stopping=stopping_hook,
                                       on_alive=alive_hook,
                                       on_started=started_hook)
-        self.status = ProcessStatus('speech', self.bus, callbacks)
+        self.status = ProcessStatus('voice', self.bus, callbacks)
         self.status.set_started()
         self.status.bind(self.bus)
         self.loop = NeonRecognizerLoop(self.bus, watchdog)
         self.connect_loop_events()
         self.connect_bus_events()
         if self.config.get('listener', {}).get('enable_stt_api', True):
             self.api_stt = STTFactory.create(config=self.config,
```

## Comparing `neon_speech-3.3.2a4.dist-info/LICENSE.md` & `neon_speech-3.3.2a5.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_speech-3.3.2a4.dist-info/METADATA` & `neon_speech-3.3.2a5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-speech
-Version: 3.3.2a4
+Version: 3.3.2a5
 Summary: Neon Speech Module
 Home-page: https://github.com/NeonGeckoCom/neon_speech
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

## Comparing `neon_speech-3.3.2a4.dist-info/RECORD` & `neon_speech-3.3.2a5.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 neon_speech/__init__.py,sha256=UDwbScPcnqA05m_zQmXnY6YeoL5j6NS_TaLj0mQdU_8,1831
-neon_speech/__main__.py,sha256=GEiV1L4ZngcJZ1m9LkEnBkqYJKsF_8hz7BVsYGQgUCo,2915
+neon_speech/__main__.py,sha256=nupeYDuAIkFPZQ1Y39CC_1JXccrrkAzdvb6QVVzIl-c,2914
 neon_speech/cli.py,sha256=2BiU-fTcmOyT3CJ6gmoCtUsP7bAUcDOt8-MkPEfMJX0,5085
 neon_speech/listener.py,sha256=Abwh5UxXYtnRlty4wA8dW0fW69YxbYRg6Gd0SJE8cGo,9921
 neon_speech/mic.py,sha256=uA_yi3hX_2yYx0G1ZkiCUu-IKZk37sCJUBERjGm3WhQ,5107
-neon_speech/service.py,sha256=RsbXxys1OqUDMwzMATndDqoTKnJXVhoWXWuYeYFTGUw,21918
+neon_speech/service.py,sha256=Q_e6HAqWhATdlU5Gcj86S1sN6CVhMS8Xpi8iPeXwvLI,21917
 neon_speech/stt.py,sha256=K6z7Wvbl1uT-h1bxI6jCnuQHfijfDeNULlifF8LVh2A,4478
 neon_speech/utils.py,sha256=6axY_oHDqmIKIBvYhnuUIJoRZTwKyYif-isfc2wKPcI,4285
-neon_speech-3.3.2a4.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-neon_speech-3.3.2a4.dist-info/METADATA,sha256=CwY7xuYXjkNEgrH2eSXdkrrUZeQErv0S6Y3wEZZ9vh8,2587
-neon_speech-3.3.2a4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neon_speech-3.3.2a4.dist-info/entry_points.txt,sha256=Y5nCn6RrdZVozA3UnFkIX_43MJ5TF-bmlqsz3LA_9rM,111
-neon_speech-3.3.2a4.dist-info/top_level.txt,sha256=fXNizEfCNvNDWenv5znkv_2KPpvzwwsRM7S3sG7bllw,12
-neon_speech-3.3.2a4.dist-info/RECORD,,
+neon_speech-3.3.2a5.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+neon_speech-3.3.2a5.dist-info/METADATA,sha256=CAYvMP97ZJiuViSLB-JR3Z1ZFgsMKKYcYbuXxGUdWKg,2587
+neon_speech-3.3.2a5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_speech-3.3.2a5.dist-info/entry_points.txt,sha256=Y5nCn6RrdZVozA3UnFkIX_43MJ5TF-bmlqsz3LA_9rM,111
+neon_speech-3.3.2a5.dist-info/top_level.txt,sha256=fXNizEfCNvNDWenv5znkv_2KPpvzwwsRM7S3sG7bllw,12
+neon_speech-3.3.2a5.dist-info/RECORD,,
```

