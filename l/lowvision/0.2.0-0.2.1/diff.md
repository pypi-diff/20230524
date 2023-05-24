# Comparing `tmp/lowvision-0.2.0.tar.gz` & `tmp/lowvision-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lowvision-0.2.0.tar", last modified: Tue May 23 05:15:04 2023, max compression
+gzip compressed data, was "lowvision-0.2.1.tar", last modified: Wed May 24 03:14:07 2023, max compression
```

## Comparing `lowvision-0.2.0.tar` & `lowvision-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-23 05:15:04.576752 lowvision-0.2.0/
--rw-r--r--   0 danielpcox   (502) staff       (20)     2174 2023-05-23 05:15:04.576610 lowvision-0.2.0/PKG-INFO
--rw-r--r--   0 danielpcox   (502) staff       (20)     1972 2023-05-23 02:26:52.000000 lowvision-0.2.0/README.md
-drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-23 05:15:04.575717 lowvision-0.2.0/lowvision/
--rw-r--r--   0 danielpcox   (502) staff       (20)        0 2023-05-22 22:04:23.000000 lowvision-0.2.0/lowvision/__init__.py
--rw-r--r--   0 danielpcox   (502) staff       (20)     4910 2023-05-23 04:56:18.000000 lowvision-0.2.0/lowvision/chat.py
--rwxr-xr-x   0 danielpcox   (502) staff       (20)     2735 2023-05-23 05:13:24.000000 lowvision-0.2.0/lowvision/shell.py
-drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-23 05:15:04.576449 lowvision-0.2.0/lowvision.egg-info/
--rw-r--r--   0 danielpcox   (502) staff       (20)     2174 2023-05-23 05:15:04.000000 lowvision-0.2.0/lowvision.egg-info/PKG-INFO
--rw-r--r--   0 danielpcox   (502) staff       (20)      256 2023-05-23 05:15:04.000000 lowvision-0.2.0/lowvision.egg-info/SOURCES.txt
--rw-r--r--   0 danielpcox   (502) staff       (20)        1 2023-05-23 05:15:04.000000 lowvision-0.2.0/lowvision.egg-info/dependency_links.txt
--rw-r--r--   0 danielpcox   (502) staff       (20)       18 2023-05-23 05:15:04.000000 lowvision-0.2.0/lowvision.egg-info/requires.txt
--rw-r--r--   0 danielpcox   (502) staff       (20)       16 2023-05-23 05:15:04.000000 lowvision-0.2.0/lowvision.egg-info/top_level.txt
--rw-r--r--   0 danielpcox   (502) staff       (20)      413 2023-05-23 05:13:53.000000 lowvision-0.2.0/pyproject.toml
--rw-r--r--   0 danielpcox   (502) staff       (20)       38 2023-05-23 05:15:04.576790 lowvision-0.2.0/setup.cfg
--rw-r--r--   0 danielpcox   (502) staff       (20)       38 2023-05-22 22:29:32.000000 lowvision-0.2.0/setup.py
+drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-24 03:14:07.481400 lowvision-0.2.1/
+-rw-r--r--   0 danielpcox   (502) staff       (20)     2174 2023-05-24 03:14:07.481261 lowvision-0.2.1/PKG-INFO
+-rw-r--r--   0 danielpcox   (502) staff       (20)     1972 2023-05-24 02:37:57.000000 lowvision-0.2.1/README.md
+drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-24 03:14:07.480052 lowvision-0.2.1/lowvision/
+-rw-r--r--   0 danielpcox   (502) staff       (20)        0 2023-05-22 22:04:23.000000 lowvision-0.2.1/lowvision/__init__.py
+-rw-r--r--   0 danielpcox   (502) staff       (20)     5119 2023-05-24 03:07:01.000000 lowvision-0.2.1/lowvision/chat.py
+-rwxr-xr-x   0 danielpcox   (502) staff       (20)     3466 2023-05-24 02:37:57.000000 lowvision-0.2.1/lowvision/shell.py
+drwxr-xr-x   0 danielpcox   (502) staff       (20)        0 2023-05-24 03:14:07.481068 lowvision-0.2.1/lowvision.egg-info/
+-rw-r--r--   0 danielpcox   (502) staff       (20)     2174 2023-05-24 03:14:07.000000 lowvision-0.2.1/lowvision.egg-info/PKG-INFO
+-rw-r--r--   0 danielpcox   (502) staff       (20)      256 2023-05-24 03:14:07.000000 lowvision-0.2.1/lowvision.egg-info/SOURCES.txt
+-rw-r--r--   0 danielpcox   (502) staff       (20)        1 2023-05-24 03:14:07.000000 lowvision-0.2.1/lowvision.egg-info/dependency_links.txt
+-rw-r--r--   0 danielpcox   (502) staff       (20)       18 2023-05-24 03:14:07.000000 lowvision-0.2.1/lowvision.egg-info/requires.txt
+-rw-r--r--   0 danielpcox   (502) staff       (20)       18 2023-05-24 03:14:07.000000 lowvision-0.2.1/lowvision.egg-info/top_level.txt
+-rw-r--r--   0 danielpcox   (502) staff       (20)      413 2023-05-24 02:54:37.000000 lowvision-0.2.1/pyproject.toml
+-rw-r--r--   0 danielpcox   (502) staff       (20)       38 2023-05-24 03:14:07.481441 lowvision-0.2.1/setup.cfg
+-rw-r--r--   0 danielpcox   (502) staff       (20)       38 2023-05-22 22:29:32.000000 lowvision-0.2.1/setup.py
```

### Comparing `lowvision-0.2.0/PKG-INFO` & `lowvision-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lowvision
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tools for low-vision coders
 Author-email: Daniel Cox <danielpcox@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Tools for low-vision coders
 
@@ -36,25 +36,25 @@
 
 ```bash
 python -m lowvision.shell -h
 ```
 
 Without arguments, it will
 - launch Bash
-- with a 1000 character scrollback buffer
+- with a 2000 character scrollback buffer
 - use `espeak` for text-to-speech
-- and `gpt-4` as the ChatGPT model
+- and `gpt-3.5-turbo` as the ChatGPT model
 
 Here's an example that changes all of those defaults:
 
 ```bash
 python -m lowvision.shell --shell /bin/sh \
                           --scrollback 5000 \
                           --tts 'say -v Daniel --rate 220' \
-                          --model gpt-3.5-turbo
+                          --model gpt-4
                           
 sh-3.2$ ping -c 3 google.com
 PING google.com (142.251.163.100): 56 data bytes
 64 bytes from 142.251.163.100: icmp_seq=0 ttl=106 time=18.316 ms
 ^C
 --- google.com ping statistics ---
 1 packets transmitted, 1 packets received, 0.0% packet loss
```

### Comparing `lowvision-0.2.0/README.md` & `lowvision-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -28,25 +28,25 @@
 
 ```bash
 python -m lowvision.shell -h
 ```
 
 Without arguments, it will
 - launch Bash
-- with a 1000 character scrollback buffer
+- with a 2000 character scrollback buffer
 - use `espeak` for text-to-speech
-- and `gpt-4` as the ChatGPT model
+- and `gpt-3.5-turbo` as the ChatGPT model
 
 Here's an example that changes all of those defaults:
 
 ```bash
 python -m lowvision.shell --shell /bin/sh \
                           --scrollback 5000 \
                           --tts 'say -v Daniel --rate 220' \
-                          --model gpt-3.5-turbo
+                          --model gpt-4
                           
 sh-3.2$ ping -c 3 google.com
 PING google.com (142.251.163.100): 56 data bytes
 64 bytes from 142.251.163.100: icmp_seq=0 ttl=106 time=18.316 ms
 ^C
 --- google.com ping statistics ---
 1 packets transmitted, 1 packets received, 0.0% packet loss
```

### Comparing `lowvision-0.2.0/lowvision/chat.py` & `lowvision-0.2.1/lowvision/chat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 import argparse
 import asyncio
-import io
 import pdb
-import subprocess
+import signal
 import sys
 import termios
 import textwrap
-import tty
 from datetime import datetime, timezone
 
 import openai
-from aioconsole import ainput
 
 
 class ChatLogger:
     def __init__(self, config: argparse.Namespace, old_term_settings: list):
         self.config = config
         self.old_settings = old_term_settings
         self.line_buffer = ''
         self.scrollback = ''
         self.max_chars = config.scrollback
         self.conversation = []
+        self.interrupt_response = False
 
     async def log(self, message: bytes):
         message = message.decode('utf-8', errors='ignore').replace('\r', '')
         self.line_buffer += message
         if '\n' in self.line_buffer:
             lines = self.line_buffer.split('\n')
             self.line_buffer = lines.pop()
@@ -48,33 +46,43 @@
         {self.scrollback}
         """)
         self.conversation = [
             {"role": "system", "content": system_prompt}
         ]
 
     async def chat_mode(self):
+
         # Put the terminal back in line-buffered mode for the chat
-        termios.tcsetattr(sys.stdin, termios.TCSADRAIN, self.old_settings)
+        termios.tcsetattr(sys.stdin.fileno(), termios.TCSAFLUSH, self.old_settings)
+
+        # Handle Ctrl-C differently in chat mode
+        def ctrl_C(signum, frame):
+            self.interrupt_response = True
+
+        signal.signal(signal.SIGINT, ctrl_C)
+
         print()
         self.reset_conversation()
         while True:
             try:
-                prompt = await ainput("?> ")
+                prompt = await asyncio.to_thread(input, "?> ")
             except EOFError:
                 break
             if prompt.strip() == "":
                 continue
             if prompt.strip() == "exit":
                 break
             if prompt.strip() == "pdb":
                 pdb.set_trace()
                 continue
             self.conversation.append({"role": "user", "content": prompt})
             q = asyncio.Queue()
+            await q.put(f'You asked: {prompt}... One moment.')
             asyncio.create_task(self.speak(q))
+            self.interrupt_response = False
             async for line in self.fetch_chat_completion(self.conversation):
                 self.conversation.append({"role": "assistant", "content": line})
                 # pdb.set_trace()
                 # subprocess.run(self.config.tts, shell=True, text=True, input=line, check=True)
                 await q.put(line)
             await q.put(None)  # terminate the speaking coroutine
             print()
@@ -91,15 +99,14 @@
             await proc.stdin.drain()
             proc.stdin.close()
             await proc.wait()
             q.task_done()
 
     # Asyncify the OpenAI API responses so we don't interrupt speech
     async def fetch_chat_completion(self, prompt):
-        loop = asyncio.get_running_loop()
         generator = self._fetch_chat_completion(prompt)
 
         def next_from_generator():
             try:
                 return next(generator)
             except StopIteration:
                 return None
@@ -113,30 +120,29 @@
 
     def _fetch_chat_completion(self, prompt):
         response = openai.ChatCompletion.create(
             model=self.config.model,
             messages=prompt,
             stream=True,
         )
-        line = []
+        line = ""
         for chunk in response:
+            if self.interrupt_response:
+                return
             delta = chunk['choices'][0]['delta']
             if 'content' in delta:
                 content = delta['content']
                 sys.stdout.write(content)
                 sys.stdout.flush()
-                if '\n' in content:
-                    segments = content.split('\n', 1)
-                    ending = "\n".join(segments[:-1])
-                    remainder = segments[-1]
-                    line.append(f'{ending}\n')
-                    yield "".join(line)
-                    line = [remainder]
+                if (sep := '\n') in content or (sep := '.') in content:
+                    left, rest = content.split(sep, 1)
+                    line += left
+                    yield line
+                    line = rest
                 else:
-                    line.append(content)
-
+                    line += content
         if line:
-            yield "".join(line)
+            yield line
 
 
 class ChatInterruption(Exception):
     pass
```

### Comparing `lowvision-0.2.0/lowvision/shell.py` & `lowvision-0.2.1/lowvision/shell.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,101 @@
 import argparse
 import asyncio
+import errno
+import fcntl
 import os
 import pty
-import select
 import signal
+import struct
 import sys
 import termios
-import tty
+from select import select
 
 import lowvision.chat as chat
 
 
-# Wraps bash to maintain a buffer of recent IO to discuss with ChatGPT
-async def main(config: argparse.Namespace):
-    terminal_size = os.get_terminal_size()
-    env = os.environ
-    print(terminal_size)
-    pid, fd = pty.fork()
-
-    def signal_handler(signum, frame):
-        os.write(fd, b'\x03')
-
-    signal.signal(signal.SIGINT, signal_handler)
-    signal.signal(signal.SIGTSTP, signal_handler)
-
-    if pid == 0:  # child process
-        env['LINES'] = str(terminal_size.lines)
-        env['COLUMNS'] = str(terminal_size.columns)
-        os.execve(config.shell, [config.shell], env)
-    else:  # parent process
-        old_settings = termios.tcgetattr(sys.stdin)
-        logger = chat.ChatLogger(config, old_settings)
-        tty.setcbreak(sys.stdin.fileno())
-
-        poller = select.poll()
-        poller.register(sys.stdin, select.POLLIN)
-        poller.register(fd, select.POLLIN | select.POLLHUP | select.POLLERR)
+def get_terminal_size():
+    size = struct.unpack('hh', fcntl.ioctl(sys.stdin.fileno(), termios.TIOCGWINSZ, '1234'))
+    return size
 
+
+def set_terminal_size(fd, size):
+    fcntl.ioctl(fd, termios.TIOCSWINSZ, struct.pack('hh', *size))
+
+
+async def main(config):
+    pid, master_fd = pty.fork()
+
+    if pid == 0:
+        # Child process
+        os.execv(config.shell, [config.shell])
+    else:
+        print(f"\nStarting chat-aware shell wrapper around {config.shell}. "
+              "Run `chat` to enter chat mode. Exit with `exit`. "
+              "Ctrl-C interrupts text-to-speech. "
+              "Exit and re-run with `-h` to see options. \n")
+        # Parent process
+        shell_pid = pid
+
+        def handle_signals(signal_number, frame):
+            os.kill(shell_pid, signal_number)
+
+        def handle_window_resize(signum, frame):
+            size = get_terminal_size()
+            set_terminal_size(master_fd, size)
+
+        signal.signal(signal.SIGWINCH, handle_window_resize)
+        signal.signal(signal.SIGINT, handle_signals)
+        signal.signal(signal.SIGTSTP, handle_signals)
+
+        set_terminal_size(master_fd, get_terminal_size())
+
+        old_term_settings = termios.tcgetattr(sys.stdin.fileno())
+
+        logger = chat.ChatLogger(config, old_term_settings)
         try:
+            new_term_settings = termios.tcgetattr(sys.stdin.fileno())
+            new_term_settings[3] = new_term_settings[3] & ~termios.ICANON & ~termios.ECHO
+            termios.tcsetattr(sys.stdin.fileno(), termios.TCSAFLUSH, new_term_settings)
+
             while True:
-                events = poller.poll()
-                for event_fd, event in events:
-                    if event_fd == sys.stdin.fileno() and event & select.POLLIN:
-                        data = os.read(sys.stdin.fileno(), 1024)
-                        os.write(fd, data)
-                    elif event_fd == fd:
-                        data = os.read(fd, 1024)
-                        if data:
-                            try:
-                                await logger.log(data)
-                                os.write(sys.stdout.fileno(), data)
-                            except chat.ChatInterruption:
-                                continue
-                            finally:
-                                tty.setcbreak(sys.stdin.fileno())
-                        else:
-                            poller.unregister(fd)
+                try:
+                    r_fd, _, _ = select([sys.stdin, master_fd], [], [])
+
+                    if sys.stdin in r_fd:
+                        input_data = os.read(sys.stdin.fileno(), 1024)
+                        if not input_data:
                             break
-                if not any(items[1] & (select.POLLIN | select.POLLHUP | select.POLLERR) for items in events):
-                    break
-        except OSError:
-            pass
+                        os.write(master_fd, input_data)
+
+                    if master_fd in r_fd:
+                        output_data = os.read(master_fd, 1024)
+                        if not output_data:
+                            break
+
+                        try:
+                            await logger.log(output_data)
+                            os.write(sys.stdout.fileno(), output_data)
+                        except chat.ChatInterruption:
+                            continue
+                        finally:
+                            termios.tcsetattr(sys.stdin.fileno(), termios.TCSAFLUSH, new_term_settings)
+                            signal.signal(signal.SIGINT, handle_signals)
+
+                except OSError as e:
+                    if e.errno == errno.EIO:
+                        break
+
         finally:
-            termios.tcsetattr(sys.stdin, termios.TCSADRAIN, old_settings)
-            os.close(fd)
+            termios.tcsetattr(sys.stdin.fileno(), termios.TCSAFLUSH, old_term_settings)
+            os.close(master_fd)
 
 
 if __name__ == "__main__":
     # argparse to get the shell and the size of the scrollback buffer (defaults to 1000 lines)
     parser = argparse.ArgumentParser()
     parser.add_argument('--shell', default='/bin/bash')
-    parser.add_argument('--scrollback', default=1000, type=int)
-    parser.add_argument('--model', default='gpt-4')
+    parser.add_argument('--scrollback', default=2000, type=int)
+    parser.add_argument('--model', default='gpt-3.5-turbo')
     parser.add_argument('--tts', default='espeak -v en-us -s 220')
     args = parser.parse_args()
     asyncio.run(main(args))
```

### Comparing `lowvision-0.2.0/lowvision.egg-info/PKG-INFO` & `lowvision-0.2.1/lowvision.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lowvision
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tools for low-vision coders
 Author-email: Daniel Cox <danielpcox@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Tools for low-vision coders
 
@@ -36,25 +36,25 @@
 
 ```bash
 python -m lowvision.shell -h
 ```
 
 Without arguments, it will
 - launch Bash
-- with a 1000 character scrollback buffer
+- with a 2000 character scrollback buffer
 - use `espeak` for text-to-speech
-- and `gpt-4` as the ChatGPT model
+- and `gpt-3.5-turbo` as the ChatGPT model
 
 Here's an example that changes all of those defaults:
 
 ```bash
 python -m lowvision.shell --shell /bin/sh \
                           --scrollback 5000 \
                           --tts 'say -v Daniel --rate 220' \
-                          --model gpt-3.5-turbo
+                          --model gpt-4
                           
 sh-3.2$ ping -c 3 google.com
 PING google.com (142.251.163.100): 56 data bytes
 64 bytes from 142.251.163.100: icmp_seq=0 ttl=106 time=18.316 ms
 ^C
 --- google.com ping statistics ---
 1 packets transmitted, 1 packets received, 0.0% packet loss
```

