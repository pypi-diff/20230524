# Comparing `tmp/audio-journal-0.0.4.tar.gz` & `tmp/audio-journal-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio-journal-0.0.4.tar", last modified: Tue May 23 21:17:12 2023, max compression
+gzip compressed data, was "audio-journal-0.0.5.tar", last modified: Tue May 23 21:38:52 2023, max compression
```

## Comparing `audio-journal-0.0.4.tar` & `audio-journal-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-05-23 21:17:12.542332 audio-journal-0.0.4/
--rw-r--r--   0 kyle       (501) staff       (20)    11337 2023-05-18 23:36:04.000000 audio-journal-0.0.4/LICENSE
--rw-r--r--   0 kyle       (501) staff       (20)      155 2023-05-23 21:17:06.000000 audio-journal-0.0.4/MANIFEST.in
--rw-r--r--   0 kyle       (501) staff       (20)      926 2023-05-23 21:17:12.542126 audio-journal-0.0.4/PKG-INFO
--rw-r--r--   0 kyle       (501) staff       (20)      104 2023-05-20 00:13:01.000000 audio-journal-0.0.4/README.md
-drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-05-23 21:17:12.539747 audio-journal-0.0.4/audio_journal/
--rw-r--r--   0 kyle       (501) staff       (20)       22 2023-05-23 19:48:37.000000 audio-journal-0.0.4/audio_journal/__init__.py
--rw-r--r--   0 kyle       (501) staff       (20)     2324 2023-05-23 19:48:37.000000 audio-journal-0.0.4/audio_journal/_modidx.py
-drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-05-23 21:17:12.541359 audio-journal-0.0.4/audio_journal/beeps/
--rw-r--r--   0 kyle       (501) staff       (20)   116188 2023-05-20 00:32:57.000000 audio-journal-0.0.4/audio_journal/beeps/error.wav
--rw-r--r--   0 kyle       (501) staff       (20)    24274 2023-05-20 00:32:57.000000 audio-journal-0.0.4/audio_journal/beeps/start.wav
--rw-r--r--   0 kyle       (501) staff       (20)    30708 2023-05-20 00:32:57.000000 audio-journal-0.0.4/audio_journal/beeps/stop.wav
--rw-r--r--   0 kyle       (501) staff       (20)  1186954 2023-05-20 00:32:57.000000 audio-journal-0.0.4/audio_journal/beeps/success.wav
--rw-r--r--   0 kyle       (501) staff       (20)     1200 2023-05-23 19:48:37.000000 audio-journal-0.0.4/audio_journal/config.py
--rw-r--r--   0 kyle       (501) staff       (20)      807 2023-05-23 19:48:37.000000 audio-journal-0.0.4/audio_journal/main.py
--rw-r--r--   0 kyle       (501) staff       (20)     1786 2023-05-23 19:48:37.000000 audio-journal-0.0.4/audio_journal/notion.py
--rw-r--r--   0 kyle       (501) staff       (20)     1923 2023-05-23 19:48:37.000000 audio-journal-0.0.4/audio_journal/record.py
--rw-r--r--   0 kyle       (501) staff       (20)      956 2023-05-23 19:48:37.000000 audio-journal-0.0.4/audio_journal/sounds.py
--rw-r--r--   0 kyle       (501) staff       (20)     1393 2023-05-23 19:48:37.000000 audio-journal-0.0.4/audio_journal/transcribe.py
-drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-05-23 21:17:12.540715 audio-journal-0.0.4/audio_journal.egg-info/
--rw-r--r--   0 kyle       (501) staff       (20)      926 2023-05-23 21:17:12.000000 audio-journal-0.0.4/audio_journal.egg-info/PKG-INFO
--rw-r--r--   0 kyle       (501) staff       (20)      629 2023-05-23 21:17:12.000000 audio-journal-0.0.4/audio_journal.egg-info/SOURCES.txt
--rw-r--r--   0 kyle       (501) staff       (20)        1 2023-05-23 21:17:12.000000 audio-journal-0.0.4/audio_journal.egg-info/dependency_links.txt
--rw-r--r--   0 kyle       (501) staff       (20)      115 2023-05-23 21:17:12.000000 audio-journal-0.0.4/audio_journal.egg-info/entry_points.txt
--rw-r--r--   0 kyle       (501) staff       (20)        1 2023-05-18 23:47:02.000000 audio-journal-0.0.4/audio_journal.egg-info/not-zip-safe
--rw-r--r--   0 kyle       (501) staff       (20)       76 2023-05-23 21:17:12.000000 audio-journal-0.0.4/audio_journal.egg-info/requires.txt
--rw-r--r--   0 kyle       (501) staff       (20)       14 2023-05-23 21:17:12.000000 audio-journal-0.0.4/audio_journal.egg-info/top_level.txt
--rw-r--r--   0 kyle       (501) staff       (20)     1077 2023-05-23 21:16:51.000000 audio-journal-0.0.4/settings.ini
--rw-r--r--   0 kyle       (501) staff       (20)       38 2023-05-23 21:17:12.542373 audio-journal-0.0.4/setup.cfg
--rw-r--r--   0 kyle       (501) staff       (20)     2596 2023-05-18 23:36:04.000000 audio-journal-0.0.4/setup.py
+drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-05-23 21:38:52.322024 audio-journal-0.0.5/
+-rw-r--r--   0 kyle       (501) staff       (20)    11337 2023-05-18 23:36:04.000000 audio-journal-0.0.5/LICENSE
+-rw-r--r--   0 kyle       (501) staff       (20)      155 2023-05-23 21:23:16.000000 audio-journal-0.0.5/MANIFEST.in
+-rw-r--r--   0 kyle       (501) staff       (20)     3127 2023-05-23 21:38:52.321816 audio-journal-0.0.5/PKG-INFO
+-rw-r--r--   0 kyle       (501) staff       (20)     2305 2023-05-23 21:38:10.000000 audio-journal-0.0.5/README.md
+drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-05-23 21:38:52.319717 audio-journal-0.0.5/audio_journal/
+-rw-r--r--   0 kyle       (501) staff       (20)       22 2023-05-23 21:38:08.000000 audio-journal-0.0.5/audio_journal/__init__.py
+-rw-r--r--   0 kyle       (501) staff       (20)     2324 2023-05-23 21:38:08.000000 audio-journal-0.0.5/audio_journal/_modidx.py
+drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-05-23 21:38:52.321047 audio-journal-0.0.5/audio_journal/beeps/
+-rw-r--r--   0 kyle       (501) staff       (20)   116188 2023-05-20 00:32:57.000000 audio-journal-0.0.5/audio_journal/beeps/error.wav
+-rw-r--r--   0 kyle       (501) staff       (20)    24274 2023-05-20 00:32:57.000000 audio-journal-0.0.5/audio_journal/beeps/start.wav
+-rw-r--r--   0 kyle       (501) staff       (20)    30708 2023-05-20 00:32:57.000000 audio-journal-0.0.5/audio_journal/beeps/stop.wav
+-rw-r--r--   0 kyle       (501) staff       (20)  1186954 2023-05-20 00:32:57.000000 audio-journal-0.0.5/audio_journal/beeps/success.wav
+-rw-r--r--   0 kyle       (501) staff       (20)     1200 2023-05-23 21:38:08.000000 audio-journal-0.0.5/audio_journal/config.py
+-rw-r--r--   0 kyle       (501) staff       (20)      807 2023-05-23 21:38:08.000000 audio-journal-0.0.5/audio_journal/main.py
+-rw-r--r--   0 kyle       (501) staff       (20)     1786 2023-05-23 21:38:08.000000 audio-journal-0.0.5/audio_journal/notion.py
+-rw-r--r--   0 kyle       (501) staff       (20)     1848 2023-05-23 21:38:08.000000 audio-journal-0.0.5/audio_journal/record.py
+-rw-r--r--   0 kyle       (501) staff       (20)      956 2023-05-23 21:38:08.000000 audio-journal-0.0.5/audio_journal/sounds.py
+-rw-r--r--   0 kyle       (501) staff       (20)     1393 2023-05-23 21:38:08.000000 audio-journal-0.0.5/audio_journal/transcribe.py
+drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-05-23 21:38:52.320463 audio-journal-0.0.5/audio_journal.egg-info/
+-rw-r--r--   0 kyle       (501) staff       (20)     3127 2023-05-23 21:38:52.000000 audio-journal-0.0.5/audio_journal.egg-info/PKG-INFO
+-rw-r--r--   0 kyle       (501) staff       (20)      629 2023-05-23 21:38:52.000000 audio-journal-0.0.5/audio_journal.egg-info/SOURCES.txt
+-rw-r--r--   0 kyle       (501) staff       (20)        1 2023-05-23 21:38:52.000000 audio-journal-0.0.5/audio_journal.egg-info/dependency_links.txt
+-rw-r--r--   0 kyle       (501) staff       (20)      115 2023-05-23 21:38:52.000000 audio-journal-0.0.5/audio_journal.egg-info/entry_points.txt
+-rw-r--r--   0 kyle       (501) staff       (20)        1 2023-05-18 23:47:02.000000 audio-journal-0.0.5/audio_journal.egg-info/not-zip-safe
+-rw-r--r--   0 kyle       (501) staff       (20)       76 2023-05-23 21:38:52.000000 audio-journal-0.0.5/audio_journal.egg-info/requires.txt
+-rw-r--r--   0 kyle       (501) staff       (20)       14 2023-05-23 21:38:52.000000 audio-journal-0.0.5/audio_journal.egg-info/top_level.txt
+-rw-r--r--   0 kyle       (501) staff       (20)     1077 2023-05-23 21:38:41.000000 audio-journal-0.0.5/settings.ini
+-rw-r--r--   0 kyle       (501) staff       (20)       38 2023-05-23 21:38:52.322064 audio-journal-0.0.5/setup.cfg
+-rw-r--r--   0 kyle       (501) staff       (20)     2596 2023-05-18 23:36:04.000000 audio-journal-0.0.5/setup.py
```

### Comparing `audio-journal-0.0.4/LICENSE` & `audio-journal-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `audio-journal-0.0.4/audio_journal/_modidx.py` & `audio-journal-0.0.5/audio_journal/_modidx.py`

 * *Files identical despite different names*

### Comparing `audio-journal-0.0.4/audio_journal/beeps/error.wav` & `audio-journal-0.0.5/audio_journal/beeps/error.wav`

 * *Files identical despite different names*

### Comparing `audio-journal-0.0.4/audio_journal/beeps/start.wav` & `audio-journal-0.0.5/audio_journal/beeps/start.wav`

 * *Files identical despite different names*

### Comparing `audio-journal-0.0.4/audio_journal/beeps/stop.wav` & `audio-journal-0.0.5/audio_journal/beeps/stop.wav`

 * *Files identical despite different names*

### Comparing `audio-journal-0.0.4/audio_journal/beeps/success.wav` & `audio-journal-0.0.5/audio_journal/beeps/success.wav`

 * *Files identical despite different names*

### Comparing `audio-journal-0.0.4/audio_journal/config.py` & `audio-journal-0.0.5/audio_journal/config.py`

 * *Files identical despite different names*

### Comparing `audio-journal-0.0.4/audio_journal/main.py` & `audio-journal-0.0.5/audio_journal/main.py`

 * *Files identical despite different names*

### Comparing `audio-journal-0.0.4/audio_journal/notion.py` & `audio-journal-0.0.5/audio_journal/notion.py`

 * *Files identical despite different names*

### Comparing `audio-journal-0.0.4/audio_journal/record.py` & `audio-journal-0.0.5/audio_journal/record.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,31 +25,30 @@
             print(status, file=sys.stderr)
         q.put(indata.copy())
 
     try:
         with sf.SoundFile(filename, mode='x', samplerate=sample_rate,
                           channels=channels, subtype='PCM_24') as file:
             with sd.InputStream(samplerate=sample_rate, channels=channels, callback=audio_callback):
-                print("Waiting for keyboard input now...")
                 input()
                 sd.stop()
                 while not q.empty():
                     file.write(q.get())
     except Exception as e:
         print(f"Error while recording audio: {e}")
 
 # %% ../nbs/03_record.ipynb 3
 def recording_process():
     os.makedirs("temp_recordings", exist_ok=True)
     os.makedirs("completed_recordings", exist_ok=True)
     while True:
-        print("Press the space key to start recording...")
+        print("Press Enter to start recording...")
         input()
         play_start_sound()
-        print("Recording... Press the space key to stop recording.")
+        print("Recording... Press Enter to stop recording.")
         current_date_time = datetime.datetime.now().strftime("%B %d, %Y %H-%M-%S")
         temp_audio_filename = f"temp_recordings/audio_{current_date_time}.wav"
         completed_audio_filename = f"completed_recordings/audio_{current_date_time}.wav"
         record_audio(temp_audio_filename)
         play_stop_sound()
         shutil.move(temp_audio_filename, completed_audio_filename)
         print(f"Audio recorded and saved to {completed_audio_filename}")
```

### Comparing `audio-journal-0.0.4/audio_journal/sounds.py` & `audio-journal-0.0.5/audio_journal/sounds.py`

 * *Files identical despite different names*

### Comparing `audio-journal-0.0.4/audio_journal/transcribe.py` & `audio-journal-0.0.5/audio_journal/transcribe.py`

 * *Files identical despite different names*

### Comparing `audio-journal-0.0.4/audio_journal.egg-info/SOURCES.txt` & `audio-journal-0.0.5/audio_journal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audio-journal-0.0.4/settings.ini` & `audio-journal-0.0.5/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = audio-journal
 lib_name = %(repo)s
-version = 0.0.4
+version = 0.0.5
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = audio_journal
```

### Comparing `audio-journal-0.0.4/setup.py` & `audio-journal-0.0.5/setup.py`

 * *Files identical despite different names*

