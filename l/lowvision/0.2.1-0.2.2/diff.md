# Comparing `tmp/lowvision-0.2.1.tar.gz` & `tmp/lowvision-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lowvision-0.2.1.tar", last modified: Wed May 24 03:14:07 2023, max compression
+gzip compressed data, was "lowvision-0.2.2.tar", last modified: Wed May 24 03:32:15 2023, max compression
```

## Comparing `lowvision-0.2.1.tar` & `lowvision-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-24 03:14:07.481400 lowvision-0.2.1/
--rw-r--r--   0 danielpcox   (502) staff       (20)     2174 2023-05-24 03:14:07.481261 lowvision-0.2.1/PKG-INFO
--rw-r--r--   0 danielpcox   (502) staff       (20)     1972 2023-05-24 02:37:57.000000 lowvision-0.2.1/README.md
-drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-24 03:14:07.480052 lowvision-0.2.1/lowvision/
--rw-r--r--   0 danielpcox   (502) staff       (20)        0 2023-05-22 22:04:23.000000 lowvision-0.2.1/lowvision/__init__.py
--rw-r--r--   0 danielpcox   (502) staff       (20)     5119 2023-05-24 03:07:01.000000 lowvision-0.2.1/lowvision/chat.py
--rwxr-xr-x   0 danielpcox   (502) staff       (20)     3466 2023-05-24 02:37:57.000000 lowvision-0.2.1/lowvision/shell.py
-drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-24 03:14:07.481068 lowvision-0.2.1/lowvision.egg-info/
--rw-r--r--   0 danielpcox   (502) staff       (20)     2174 2023-05-24 03:14:07.000000 lowvision-0.2.1/lowvision.egg-info/PKG-INFO
--rw-r--r--   0 danielpcox   (502) staff       (20)      256 2023-05-24 03:14:07.000000 lowvision-0.2.1/lowvision.egg-info/SOURCES.txt
--rw-r--r--   0 danielpcox   (502) staff       (20)        1 2023-05-24 03:14:07.000000 lowvision-0.2.1/lowvision.egg-info/dependency_links.txt
--rw-r--r--   0 danielpcox   (502) staff       (20)       18 2023-05-24 03:14:07.000000 lowvision-0.2.1/lowvision.egg-info/requires.txt
--rw-r--r--   0 danielpcox   (502) staff       (20)       18 2023-05-24 03:14:07.000000 lowvision-0.2.1/lowvision.egg-info/top_level.txt
--rw-r--r--   0 danielpcox   (502) staff       (20)      413 2023-05-24 02:54:37.000000 lowvision-0.2.1/pyproject.toml
--rw-r--r--   0 danielpcox   (502) staff       (20)       38 2023-05-24 03:14:07.481441 lowvision-0.2.1/setup.cfg
--rw-r--r--   0 danielpcox   (502) staff       (20)       38 2023-05-22 22:29:32.000000 lowvision-0.2.1/setup.py
+drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-24 03:32:15.457956 lowvision-0.2.2/
+-rw-r--r--   0 danielpcox   (502) staff       (20)     2179 2023-05-24 03:32:15.457814 lowvision-0.2.2/PKG-INFO
+-rw-r--r--   0 danielpcox   (502) staff       (20)     1977 2023-05-24 03:19:37.000000 lowvision-0.2.2/README.md
+drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-24 03:32:15.456809 lowvision-0.2.2/lowvision/
+-rw-r--r--   0 danielpcox   (502) staff       (20)        0 2023-05-22 22:04:23.000000 lowvision-0.2.2/lowvision/__init__.py
+-rw-r--r--   0 danielpcox   (502) staff       (20)     5103 2023-05-24 03:30:09.000000 lowvision-0.2.2/lowvision/chat.py
+-rwxr-xr-x   0 danielpcox   (502) staff       (20)     3577 2023-05-24 03:28:34.000000 lowvision-0.2.2/lowvision/shell.py
+drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-24 03:32:15.457614 lowvision-0.2.2/lowvision.egg-info/
+-rw-r--r--   0 danielpcox   (502) staff       (20)     2179 2023-05-24 03:32:15.000000 lowvision-0.2.2/lowvision.egg-info/PKG-INFO
+-rw-r--r--   0 danielpcox   (502) staff       (20)      256 2023-05-24 03:32:15.000000 lowvision-0.2.2/lowvision.egg-info/SOURCES.txt
+-rw-r--r--   0 danielpcox   (502) staff       (20)        1 2023-05-24 03:32:15.000000 lowvision-0.2.2/lowvision.egg-info/dependency_links.txt
+-rw-r--r--   0 danielpcox   (502) staff       (20)       18 2023-05-24 03:32:15.000000 lowvision-0.2.2/lowvision.egg-info/requires.txt
+-rw-r--r--   0 danielpcox   (502) staff       (20)       18 2023-05-24 03:32:15.000000 lowvision-0.2.2/lowvision.egg-info/top_level.txt
+-rw-r--r--   0 danielpcox   (502) staff       (20)      413 2023-05-24 03:31:48.000000 lowvision-0.2.2/pyproject.toml
+-rw-r--r--   0 danielpcox   (502) staff       (20)       38 2023-05-24 03:32:15.457994 lowvision-0.2.2/setup.cfg
+-rw-r--r--   0 danielpcox   (502) staff       (20)       38 2023-05-22 22:29:32.000000 lowvision-0.2.2/setup.py
```

### Comparing `lowvision-0.2.1/PKG-INFO` & `lowvision-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lowvision
-Version: 0.2.1
+Version: 0.2.2
 Summary: Tools for low-vision coders
 Author-email: Daniel Cox <danielpcox@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Tools for low-vision coders
 
@@ -55,14 +55,14 @@
 sh-3.2$ ping -c 3 google.com
 PING google.com (142.251.163.100): 56 data bytes
 64 bytes from 142.251.163.100: icmp_seq=0 ttl=106 time=18.316 ms
 ^C
 --- google.com ping statistics ---
 1 packets transmitted, 1 packets received, 0.0% packet loss
 round-trip min/avg/max/stddev = 18.316/18.316/18.316/0.000 ms
-sh-3.2$ chat
+sh-3.2$ chat     
 ?> what happened?
 The user performed a ping test to google.com by sending 3 packets, and received a reply from one packet. The response shows the IP address of google.com and the round-trip time for the packet. The test was interrupted with ^C after receiving one response.
 ?> exit
 sh-3.2$
 ```
```

### Comparing `lowvision-0.2.1/README.md` & `lowvision-0.2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,14 @@
 sh-3.2$ ping -c 3 google.com
 PING google.com (142.251.163.100): 56 data bytes
 64 bytes from 142.251.163.100: icmp_seq=0 ttl=106 time=18.316 ms
 ^C
 --- google.com ping statistics ---
 1 packets transmitted, 1 packets received, 0.0% packet loss
 round-trip min/avg/max/stddev = 18.316/18.316/18.316/0.000 ms
-sh-3.2$ chat
+sh-3.2$ chat     
 ?> what happened?
 The user performed a ping test to google.com by sending 3 packets, and received a reply from one packet. The response shows the IP address of google.com and the round-trip time for the packet. The test was interrupted with ^C after receiving one response.
 ?> exit
 sh-3.2$
 ```
```

### Comparing `lowvision-0.2.1/lowvision/chat.py` & `lowvision-0.2.2/lowvision/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,22 +72,22 @@
             if prompt.strip() == "exit":
                 break
             if prompt.strip() == "pdb":
                 pdb.set_trace()
                 continue
             self.conversation.append({"role": "user", "content": prompt})
             q = asyncio.Queue()
-            await q.put(f'You asked: {prompt}... One moment.')
             asyncio.create_task(self.speak(q))
             self.interrupt_response = False
             async for line in self.fetch_chat_completion(self.conversation):
                 self.conversation.append({"role": "assistant", "content": line})
                 # pdb.set_trace()
                 # subprocess.run(self.config.tts, shell=True, text=True, input=line, check=True)
-                await q.put(line)
+                if not self.config.no_tts:
+                    await q.put(line)
             await q.put(None)  # terminate the speaking coroutine
             print()
 
         raise ChatInterruption
 
     async def speak(self, q: asyncio.Queue):
         while True:
```

### Comparing `lowvision-0.2.1/lowvision/shell.py` & `lowvision-0.2.2/lowvision/shell.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,15 +28,16 @@
     if pid == 0:
         # Child process
         os.execv(config.shell, [config.shell])
     else:
         print(f"\nStarting chat-aware shell wrapper around {config.shell}. "
               "Run `chat` to enter chat mode. Exit with `exit`. "
               "Ctrl-C interrupts text-to-speech. "
-              "Exit and re-run with `-h` to see options. \n")
+              "Exit and re-run with `-h` to see options.")
+        print("Option values: ", config.__dict__, "\n")
         # Parent process
         shell_pid = pid
 
         def handle_signals(signal_number, frame):
             os.kill(shell_pid, signal_number)
 
         def handle_window_resize(signum, frame):
@@ -93,9 +94,11 @@
 if __name__ == "__main__":
     # argparse to get the shell and the size of the scrollback buffer (defaults to 1000 lines)
     parser = argparse.ArgumentParser()
     parser.add_argument('--shell', default='/bin/bash')
     parser.add_argument('--scrollback', default=2000, type=int)
     parser.add_argument('--model', default='gpt-3.5-turbo')
     parser.add_argument('--tts', default='espeak -v en-us -s 220')
+    parser.add_argument('--no-tts', action='store_true')
+
     args = parser.parse_args()
     asyncio.run(main(args))
```

### Comparing `lowvision-0.2.1/lowvision.egg-info/PKG-INFO` & `lowvision-0.2.2/lowvision.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lowvision
-Version: 0.2.1
+Version: 0.2.2
 Summary: Tools for low-vision coders
 Author-email: Daniel Cox <danielpcox@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Tools for low-vision coders
 
@@ -55,14 +55,14 @@
 sh-3.2$ ping -c 3 google.com
 PING google.com (142.251.163.100): 56 data bytes
 64 bytes from 142.251.163.100: icmp_seq=0 ttl=106 time=18.316 ms
 ^C
 --- google.com ping statistics ---
 1 packets transmitted, 1 packets received, 0.0% packet loss
 round-trip min/avg/max/stddev = 18.316/18.316/18.316/0.000 ms
-sh-3.2$ chat
+sh-3.2$ chat     
 ?> what happened?
 The user performed a ping test to google.com by sending 3 packets, and received a reply from one packet. The response shows the IP address of google.com and the round-trip time for the packet. The test was interrupted with ^C after receiving one response.
 ?> exit
 sh-3.2$
 ```
```

