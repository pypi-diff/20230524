# Comparing `tmp/elevenlabslib-0.8.0.tar.gz` & `tmp/elevenlabslib-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabslib-0.8.0.tar", last modified: Tue May 16 12:53:45 2023, max compression
+gzip compressed data, was "elevenlabslib-0.8.1.tar", last modified: Wed May 24 13:43:50 2023, max compression
```

## Comparing `elevenlabslib-0.8.0.tar` & `elevenlabslib-0.8.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 12:53:45.458269 elevenlabslib-0.8.0/
--rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.8.0/LICENSE
--rw-rw-rw-   0        0        0     2705 2023-05-16 12:53:45.457269 elevenlabslib-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     2050 2023-04-25 20:14:38.000000 elevenlabslib-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 12:53:45.437269 elevenlabslib-0.8.0/elevenlabslib/
--rw-rw-rw-   0        0        0     7678 2023-05-14 14:43:03.000000 elevenlabslib-0.8.0/elevenlabslib/ElevenLabsHistoryItem.py
--rw-rw-rw-   0        0        0     3025 2023-05-14 14:33:26.000000 elevenlabslib-0.8.0/elevenlabslib/ElevenLabsSample.py
--rw-rw-rw-   0        0        0    18927 2023-05-16 12:47:18.000000 elevenlabslib-0.8.0/elevenlabslib/ElevenLabsUser.py
--rw-rw-rw-   0        0        0    37163 2023-05-16 11:50:49.000000 elevenlabslib-0.8.0/elevenlabslib/ElevenLabsVoice.py
--rw-rw-rw-   0        0        0      533 2023-04-30 12:44:41.000000 elevenlabslib-0.8.0/elevenlabslib/__init__.py
--rw-rw-rw-   0        0        0     6285 2023-05-16 12:08:10.000000 elevenlabslib-0.8.0/elevenlabslib/helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:53:45.456268 elevenlabslib-0.8.0/elevenlabslib.egg-info/
--rw-rw-rw-   0        0        0     2705 2023-05-16 12:53:45.000000 elevenlabslib-0.8.0/elevenlabslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-05-16 12:53:45.000000 elevenlabslib-0.8.0/elevenlabslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 12:53:45.000000 elevenlabslib-0.8.0/elevenlabslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-16 12:53:45.000000 elevenlabslib-0.8.0/elevenlabslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-16 12:53:45.000000 elevenlabslib-0.8.0/elevenlabslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      855 2023-05-16 12:53:02.000000 elevenlabslib-0.8.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 12:53:45.458269 elevenlabslib-0.8.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 13:43:50.283703 elevenlabslib-0.8.1/
+-rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.8.1/LICENSE
+-rw-rw-rw-   0        0        0     3163 2023-05-24 13:43:50.282703 elevenlabslib-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2508 2023-05-21 23:44:11.000000 elevenlabslib-0.8.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 13:43:50.277704 elevenlabslib-0.8.1/elevenlabslib/
+-rw-rw-rw-   0        0        0     7678 2023-05-14 14:43:03.000000 elevenlabslib-0.8.1/elevenlabslib/ElevenLabsHistoryItem.py
+-rw-rw-rw-   0        0        0     3025 2023-05-14 14:33:26.000000 elevenlabslib-0.8.1/elevenlabslib/ElevenLabsSample.py
+-rw-rw-rw-   0        0        0    18927 2023-05-21 19:46:46.000000 elevenlabslib-0.8.1/elevenlabslib/ElevenLabsUser.py
+-rw-rw-rw-   0        0        0    37135 2023-05-24 13:39:53.000000 elevenlabslib-0.8.1/elevenlabslib/ElevenLabsVoice.py
+-rw-rw-rw-   0        0        0      533 2023-04-30 12:44:41.000000 elevenlabslib-0.8.1/elevenlabslib/__init__.py
+-rw-rw-rw-   0        0        0     6285 2023-05-21 19:46:46.000000 elevenlabslib-0.8.1/elevenlabslib/helpers.py
+-rw-rw-rw-   0        0        0     3738 2023-05-24 13:33:48.000000 elevenlabslib-0.8.1/elevenlabslib/linuxBugTest.py
+-rw-rw-rw-   0        0        0     2291 2023-05-23 14:40:59.000000 elevenlabslib-0.8.1/elevenlabslib/linuxtest2.py
+drwxrwxrwx   0        0        0        0 2023-05-24 13:43:50.281702 elevenlabslib-0.8.1/elevenlabslib.egg-info/
+-rw-rw-rw-   0        0        0     3163 2023-05-24 13:43:50.000000 elevenlabslib-0.8.1/elevenlabslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2023-05-24 13:43:50.000000 elevenlabslib-0.8.1/elevenlabslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 13:43:50.000000 elevenlabslib-0.8.1/elevenlabslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-24 13:43:50.000000 elevenlabslib-0.8.1/elevenlabslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-24 13:43:50.000000 elevenlabslib-0.8.1/elevenlabslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      855 2023-05-24 13:41:01.000000 elevenlabslib-0.8.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 13:43:50.283703 elevenlabslib-0.8.1/setup.cfg
```

### Comparing `elevenlabslib-0.8.0/LICENSE` & `elevenlabslib-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.8.0/PKG-INFO` & `elevenlabslib-0.8.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.8.0
+Version: 0.8.1
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,22 @@
 # elevenlabslib
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/elevenlabslib?color=%23009FFFFF&style=for-the-badge)
 ![PyPI](https://img.shields.io/pypi/v/elevenlabslib?color=%23FE6137&style=for-the-badge)
 ![GitHub last commit](https://img.shields.io/github/last-commit/lugia19/elevenlabslib?style=for-the-badge)
 
 Python wrapper for the full elevenlabs API.
 
+### NOTE: There's now an official wrapper, but this project will continue to be maintained.
+
+The main reason is the different approach to playback. By doing playback purely within python instead of piping to an external process, there are a couple of important extra things that can be done, such as:
+- Playback on a specific output device
+- Running functions exactly when the playback begins and ends
+- Controlling the playback from within python
+
+
 ### **Documentation now available at https://elevenlabslib.readthedocs.io/en/latest/**
 
 # Installation
 
 Just run `pip install elevenlabslib`, it's on [pypi](https://pypi.org/project/elevenlabslib/).
 
 Note: On Linux, you may need to install portaudio. On debian and derivatives, it's `sudo apt-get install libportaudio2`, and possibly also `sudo apt-get install python3-pyaudio`.
```

### Comparing `elevenlabslib-0.8.0/elevenlabslib/ElevenLabsHistoryItem.py` & `elevenlabslib-0.8.1/elevenlabslib/ElevenLabsHistoryItem.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.8.0/elevenlabslib/ElevenLabsSample.py` & `elevenlabslib-0.8.1/elevenlabslib/ElevenLabsSample.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.8.0/elevenlabslib/ElevenLabsUser.py` & `elevenlabslib-0.8.1/elevenlabslib/ElevenLabsUser.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.8.0/elevenlabslib/ElevenLabsVoice.py` & `elevenlabslib-0.8.1/elevenlabslib/ElevenLabsVoice.py`

 * *Files 2% similar despite different names*

```diff
@@ -586,30 +586,30 @@
                             if data != b"":
                                 logging.debug("Still some data left, writing it...")
                                 #logging.debug("Putting " + str(len(data)) +
                                 #              " bytes in queue.")
                                 self._q.put(data)
                             break
                         else:
-                            logging.critical("We're not at the end, yet we recieved less data than expected. THIS SHOULD NOT HAPPEN.")
+                            logging.error("We're not at the end, yet we recieved less data than expected. THIS SHOULD NOT HAPPEN.")
             logging.debug("While loop done.")
             self._events["playbackFinishedEvent"].wait()  # Wait until playback is finished
             self._onPlaybackEnd()
             logging.debug(stream.active)
         logging.debug("Stream done.")
         return
 
     def _stream_downloader_function(self, streamedResponse:requests.Response):
         # This is the function running in the download thread.
         streamedResponse.raise_for_status()
         totalLength = 0
         logging.debug("Starting iter...")
         for chunk in streamedResponse.iter_content(chunk_size=_downloadChunkSize):
-            if self._events["headerReadyEvent"].is_set():
-                logging.debug("HeaderReady is set, waiting for the soundfile...")
+            if self._events["headerReadyEvent"].is_set() and not self._events["soundFileReadyEvent"].is_set():
+                logging.debug("HeaderReady is set, but waiting for the soundfile...")
                 self._events["soundFileReadyEvent"].wait()  # Wait for the soundfile to be created.
                 if not self._events["headerReadyEvent"].is_set():
                     logging.debug("headerReady was cleared by the playback thread. Header data still missing, download more.")
                     self._events["soundFileReadyEvent"].clear()
 
             totalLength += len(chunk)
             if len(chunk) != _downloadChunkSize:
@@ -640,61 +640,61 @@
         return
 
     def _stream_playback_callback(self, outdata, frames, timeData, status):
         assert frames == _playbackBlockSize
 
         while True:
             try:
-                readData = self._q.get_nowait()
+                if self._events["downloadDoneEvent"].is_set():
+                    readData = self._q.get_nowait()
+                else:
+                    readData = self._q.get(timeout=5)    #Download isn't over so we may have to wait.
                 if len(readData) == 0 and not self._events["downloadDoneEvent"].is_set():
-                    logging.debug("An empty item got into the queue. Skip it.")
+                    logging.error("An empty item got into the queue. This shouldn't happen, but let's just skip it.")
                     continue
                 break
             except queue.Empty as e:
                 if self._events["downloadDoneEvent"].is_set():
                     logging.debug("Download (and playback) finished.")  # We're done.
                     raise sd.CallbackStop
                 else:
-                    # This should NEVER happen, as the getdownloaddata function handles waiting for new data to come in. ABORT.
-                    logging.debug("Missing data but download isn't over. What the fuck?")
+                    logging.critical("Could not get an item within the timeout. Abort.")
                     raise sd.CallbackAbort
         #We've read an item from the queue.
 
         if not self._events["playbackStartFired"].is_set(): #Ensure the callback only fires once.
             self._events["playbackStartFired"].set()
             logging.debug("Firing onPlaybackStart...")
             self._onPlaybackStart()
 
         # Last read chunk was smaller than it should've been. It's either EOF or that stupid soundFile bug.
         if 0 < len(readData) < len(outdata):
             logging.debug("Data read smaller than it should've been.")
-            logging.debug("Read " + str(len(readData)) + " bytes but expected " + str(len(outdata)) + ", padding...")
-
-            # I still don't really understand why this happens - seems to be related to the soundfile bug.
-            # Padding it like this means there ends up being a small portion of silence during the playback.
+            logging.debug(f"Read {len(readData)} bytes but expected {len(outdata)}, padding...")
 
             outdata[:len(readData)] = readData
             outdata[len(readData):] = b'\x00' * (len(outdata) - len(readData))
         elif len(readData) == 0:
             logging.debug("Callback got no data from the queue. Checking if playback is over...")
             with self._bytesLock:
                 oldPos = self._bytesFile.tell()
                 endPos = self._bytesFile.seek(0, os.SEEK_END)
                 if oldPos == endPos and self._events["downloadDoneEvent"].is_set():
                     logging.debug("EOF reached and download over! Stopping callback...")
                     raise sd.CallbackStop
                 else:
-                    logging.debug("...Read no data but the download isn't over, what the fuck? Panic. Just send silence.")
+                    logging.critical("...Read no data but the download isn't over? Panic. Just send silence.")
                     outdata[len(readData):] = b'\x00' * (len(outdata) - len(readData))
         else:
             outdata[:] = readData
     #THIS FUNCTION ASSUMES YOU'VE GIVEN THE THREAD THE LOCK.
     def _soundFile_read_and_fix(self, dataToRead:int=-1, dtype=_defaultDType):
         readData = self._bytesSoundFile.buffer_read(dataToRead, dtype=dtype)
-        logging.debug(f"Expected {dataToRead*self._frameSize} bytes, got back {len(readData)}")
+        if dataToRead * self._frameSize != len(readData):
+            logging.debug(f"Expected {dataToRead * self._frameSize} bytes, but got back {len(readData)}")
         if len(readData) < dataToRead * self._frameSize:
             logging.debug("Insufficient data read.")
             curPos = self._bytesFile.tell()
             endPos = self._bytesFile.seek(0, os.SEEK_END)
             if curPos != endPos:
                 logging.debug("We're not at the end of the file. Check if we're out of frames.")
                 logging.debug("Recreating soundfile...")
```

### Comparing `elevenlabslib-0.8.0/elevenlabslib/__init__.py` & `elevenlabslib-0.8.1/elevenlabslib/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.8.0/elevenlabslib/helpers.py` & `elevenlabslib-0.8.1/elevenlabslib/helpers.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.8.0/elevenlabslib.egg-info/PKG-INFO` & `elevenlabslib-0.8.1/elevenlabslib.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.8.0
+Version: 0.8.1
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,22 @@
 # elevenlabslib
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/elevenlabslib?color=%23009FFFFF&style=for-the-badge)
 ![PyPI](https://img.shields.io/pypi/v/elevenlabslib?color=%23FE6137&style=for-the-badge)
 ![GitHub last commit](https://img.shields.io/github/last-commit/lugia19/elevenlabslib?style=for-the-badge)
 
 Python wrapper for the full elevenlabs API.
 
+### NOTE: There's now an official wrapper, but this project will continue to be maintained.
+
+The main reason is the different approach to playback. By doing playback purely within python instead of piping to an external process, there are a couple of important extra things that can be done, such as:
+- Playback on a specific output device
+- Running functions exactly when the playback begins and ends
+- Controlling the playback from within python
+
+
 ### **Documentation now available at https://elevenlabslib.readthedocs.io/en/latest/**
 
 # Installation
 
 Just run `pip install elevenlabslib`, it's on [pypi](https://pypi.org/project/elevenlabslib/).
 
 Note: On Linux, you may need to install portaudio. On debian and derivatives, it's `sudo apt-get install libportaudio2`, and possibly also `sudo apt-get install python3-pyaudio`.
```

### Comparing `elevenlabslib-0.8.0/pyproject.toml` & `elevenlabslib-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0",
             "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elevenlabslib"
-version = "0.8.0"
+version = "0.8.1"
 authors = [
   { name="lugia19", email="lugia19@lugia19.com" },
 ]
 description = "Complete python wrapper for the elevenlabs API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies=[
```

