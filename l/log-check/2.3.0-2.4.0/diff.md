# Comparing `tmp/log_check-2.3.0.tar.gz` & `tmp/log_check-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log_check-2.3.0.tar", last modified: Wed Nov  9 07:45:50 2022, max compression
+gzip compressed data, was "log_check-2.4.0.tar", last modified: Wed May 17 14:38:31 2023, max compression
```

## Comparing `log_check-2.3.0.tar` & `log_check-2.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2022-11-09 07:45:50.304355 log_check-2.3.0/
--rw-rw-rw-   0        0        0      259 2022-11-09 07:45:50.303375 log_check-2.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1771 2022-09-26 03:24:55.000000 log_check-2.3.0/README.md
-drwxrwxrwx   0        0        0        0 2022-11-09 07:45:50.303375 log_check-2.3.0/log_check.egg-info/
--rw-rw-rw-   0        0        0      259 2022-11-09 07:45:50.000000 log_check-2.3.0/log_check.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2022-11-09 07:45:50.000000 log_check-2.3.0/log_check.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-09 07:45:50.000000 log_check-2.3.0/log_check.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2022-11-09 07:45:50.000000 log_check-2.3.0/log_check.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-11-09 07:45:50.000000 log_check-2.3.0/log_check.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2022-11-09 07:45:50.000000 log_check-2.3.0/log_check.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6236 2022-11-09 03:03:40.000000 log_check-2.3.0/log_check.py
--rw-rw-rw-   0        0        0       42 2022-11-09 07:45:50.304355 log_check-2.3.0/setup.cfg
--rw-rw-rw-   0        0        0      486 2022-11-09 07:43:41.000000 log_check-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:38:31.422578 log_check-2.4.0/
+-rw-rw-rw-   0        0        0      259 2023-05-17 14:38:31.422578 log_check-2.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1850 2023-05-17 14:21:53.000000 log_check-2.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 14:38:31.421612 log_check-2.4.0/log_check.egg-info/
+-rw-rw-rw-   0        0        0      259 2023-05-17 14:38:31.000000 log_check-2.4.0/log_check.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-05-17 14:38:31.000000 log_check-2.4.0/log_check.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 14:38:31.000000 log_check-2.4.0/log_check.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-05-17 14:38:31.000000 log_check-2.4.0/log_check.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 14:37:55.000000 log_check-2.4.0/log_check.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-05-17 14:38:31.000000 log_check-2.4.0/log_check.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6082 2023-05-17 14:35:46.000000 log_check-2.4.0/log_check.py
+-rw-rw-rw-   0        0        0       42 2023-05-17 14:38:31.422578 log_check-2.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      507 2023-05-17 14:38:15.000000 log_check-2.4.0/setup.py
```

### Comparing `log_check-2.3.0/log_check.py` & `log_check-2.4.0/log_check.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,198 +1,182 @@
-# -*- coding: UTF-8 -*-
-
-import sys, re, os
-from colorama import Fore
-from colorama import Style
-
-help = """
-Usage:
-    logc [option] [paths|files]
-
-Option:
-    -S, -show_ok                show ok file.
-    -H, -hide_ok                hide ok file, progress bar instead.
-    -h, -help                   just show this.
-
-Example:
-    logc                        check all .cpp, .h, .hpp, .mm in `./`
-    logc ../crcp                check all .cpp, .h, .hpp, .mm in `../crcp`
-    logc main.cpp               check main.cpp
-"""
-
-g_unknow_logs = []
-
-class Progress:
-    def __init__(self, max = 100, width = 60):
-        self.max = max
-        self.width = width
-        self.i = 0
-
-    def next(self, info=None):
-        self.i = self.i+1
-        finished = int(self.i / self.max * self.width + 0.5) # 四舍五入
-        rest = self.width - finished
-        if info==None:
-            bar = '|{}{}|{}/{}'.format('#'*finished, ' '*rest, self.i, self.max)
-        else:
-            bar = '|{}{}|{}/{}`{}`'.format('#'*finished, ' '*rest, self.i, self.max, info)
-        print('\b'*len(bar), end='')
-        print(bar, end='')
-
-
-def getfiles(current_dir, types, files = []):
-    try:
-        dir_list = os.listdir(current_dir)
-    except PermissionError:
-        return None
-    for dir in dir_list:
-        path = os.path.join(current_dir, dir)
-        if os.path.isdir(path):
-            getfiles(path, types, files)
-        else:
-            obs_path = current_dir + '/' + dir
-            for type in types:
-                if obs_path.endswith(type):
-                    files.append(obs_path.replace('\\', '/'))
-    return files
-
-
-def parse(text, start_pos):
-    first_quote_idx = text.find('\"', start_pos)
-    in_dou_quote = False
-    fmt_end_pos = None
-    for i in range(first_quote_idx, len(text)):
-        c = text[i] 
-        if c == '\"':
-            in_dou_quote = not in_dou_quote
-        if not in_dou_quote and (c==',' or c==')'):
-            fmt_end_pos = i
-            break
-    if fmt_end_pos == None:
-        raise Exception('fmt_end_pos is None')
-    place_hoder_num = len( re.findall(r'({.*?})', text[start_pos:fmt_end_pos]) )
-
-    i = fmt_end_pos
-    arg_num = 0
-    left_braces = {'(', '[', '{'}
-    right_braces = {')', ']', '}'}
-    in_dou_quote = False
-    in_sin_quote = False
-    deep = 1
-    while deep!=0 and i<len(text):
-        c = text[i]
-        if c == '"':
-            in_dou_quote = not in_dou_quote
-        if c == "'":
-            in_sin_quote = not in_sin_quote
-        if not in_dou_quote and not in_sin_quote:
-            if c in left_braces:
-                deep = deep+1
-            if c in right_braces:
-                deep = deep-1
-        if c == ',' and deep == 1 and not in_dou_quote and not in_sin_quote:
-            arg_num = arg_num+1
-        i = i+1
-    end_pos = i
-    if deep != 0:
-        raise Exception('deep({}) error'.format(deep))
-
-    statement = text[start_pos:end_pos]
-    return ((place_hoder_num, arg_num, statement))
-
-bad_log_fmt = """
-{} [line {}] : {{}} = {}, argc = {}
-"""+Fore.RED+"""{}
-"""+Style.RESET_ALL
-
-def check(files, show_ok):
-    if len(files) == 0:
-        return
-    max_file_name_len = max([len(file_name) for file_name in files])
-
-    bad_files = []
-
-    if show_ok == None:
-        show_ok = len(files) <= 128
-
-    progress = Progress(max=len(files))
-
-    for source_file in files:
-        try:
-            text = open(source_file, encoding='utf-8').read().replace('\\\"', '').replace('\\\'', '')
-        except UnicodeDecodeError:
-            print('\n can not read file `{}`'.format(source_file))
-            continue
-        iter = re.finditer('(LOG[T|D|I|W|E|C]\(|fmt::format\()', text, re.MULTILINE)
-
-        bad_fmt = []
-        log_len = 0
-        for item in iter:
-            log_len = log_len+1
-            key_word = item.group()
-            location = len(re.findall('\n', text[:item.start()])) + 1
-            try:
-                place_hoder_num, arg_num, statement = parse(text, item.start())
-            except Exception as e:
-                g_unknow_logs.append({'file':source_file, 'line':location, 'exception': e, 'key_word':key_word})
-                continue
-                
-            if place_hoder_num != arg_num:
-                print(bad_log_fmt.format(source_file, location, place_hoder_num, arg_num, statement))
-                bad_fmt.append((key_word, place_hoder_num, arg_num))
-            
-        space_num = max_file_name_len-len(source_file)
-        if len(bad_fmt) == 0:
-            if show_ok:
-                space_num = max_file_name_len-len(source_file)
-                print((Fore.GREEN+'{}{} all {:2} `Fmt` ok'+Style.RESET_ALL).format(source_file, ' '*space_num, log_len))
-        else:
-            print('{}{} {:2} bad `Fmt` total in {} `Fmt`\n'.format(source_file, ' '*space_num, len(bad_fmt), log_len))
-            bad_files.append({'source_file':source_file, 'bad_fmt': bad_fmt})
-        
-        if not show_ok:
-            progress.next()
-
-    print()
-    print()
-    print('({}/{})(badfile/total) {:3} bad `Fmt` total'.format(len(bad_files), len(files), sum([len(bad_file['bad_fmt']) for bad_file in bad_files])))
-    print()
-    print()
-    print()
-    print('{} unknown `Fmt`:'.format(len(g_unknow_logs)))
-    for log in g_unknow_logs:
-        print(log)
-
-def main():
-    if '-help' in sys.argv or '-h' in sys.argv:
-        print(help)
-        exit()
-
-    default_types = ['.cpp', '.h', '.hpp', '.mm']
-    show_ok = None
-    show_ok_res = {
-       '-S'       : True,
-       '-show_ok' : True,
-       '-H'       : False,
-       '-hide_ok' : False,
-    }
-    for arg in show_ok_res:
-        if arg in sys.argv:
-            sys.argv.remove(arg)
-            show_ok = show_ok_res[arg]
-        
-    if len(sys.argv) > 1:
-        files = []
-        for arg in sys.argv[1:]:
-            if os.path.isdir(arg):
-                files = files + getfiles(arg, default_types)
-            elif os.path.isfile(arg):
-                files.append(arg)
-                print('{} is file'.format(arg))
-            else:
-                print('`{}` is not file or dir!!!'.format(arg))
-        check(files, show_ok)
-    else:
-        check(getfiles('./', default_types), show_ok)
-
-if __name__ == "__main__":
-    main()
+# -*- coding: UTF-8 -*-
+
+import sys, re, os
+from colorama import Fore
+from colorama import Style
+from rich.progress import Progress
+
+help = """
+Usage:
+    logc [option] [paths|files]
+
+Option:
+    -S, -show_ok                show ok file.
+    -H, -hide_ok                hide ok file, progress bar instead.
+    -h, -help                   just show this.
+
+Example:
+    logc                        check all .cpp, .h, .hpp, .mm in `./`
+    logc ../crcp                check all .cpp, .h, .hpp, .mm in `../crcp`
+    logc main.cpp               check main.cpp
+"""
+
+g_unknow_logs = []
+
+def getfiles(current_dir, types, files = []):
+    try:
+        dir_list = os.listdir(current_dir)
+    except PermissionError:
+        return None
+    for dir in dir_list:
+        path = os.path.join(current_dir, dir)
+        if os.path.isdir(path):
+            getfiles(path, types, files)
+        else:
+            obs_path = current_dir + '/' + dir
+            for type in types:
+                if obs_path.endswith(type):
+                    files.append(obs_path.replace('\\', '/'))
+    return files
+
+
+def parse(text, start_pos):
+    first_quote_idx = text.find('\"', start_pos)
+    in_dou_quote = False
+    fmt_end_pos = None
+    for i in range(first_quote_idx, len(text)):
+        c = text[i] 
+        if c == '\"':
+            in_dou_quote = not in_dou_quote
+        if not in_dou_quote and (c==',' or c==')'):
+            fmt_end_pos = i
+            break
+    if fmt_end_pos == None:
+        raise Exception('fmt_end_pos is None')
+    place_hoder_num = len( re.findall(r'({.*?})', text[start_pos:fmt_end_pos]) )
+
+    i = fmt_end_pos
+    arg_num = 0
+    left_braces = {'(', '[', '{'}
+    right_braces = {')', ']', '}'}
+    in_dou_quote = False
+    in_sin_quote = False
+    deep = 1
+    while deep!=0 and i<len(text):
+        c = text[i]
+        if c == '"':
+            in_dou_quote = not in_dou_quote
+        if c == "'":
+            in_sin_quote = not in_sin_quote
+        if not in_dou_quote and not in_sin_quote:
+            if c in left_braces:
+                deep = deep+1
+            if c in right_braces:
+                deep = deep-1
+        if c == ',' and deep == 1 and not in_dou_quote and not in_sin_quote:
+            arg_num = arg_num+1
+        i = i+1
+    end_pos = i
+    if deep != 0:
+        raise Exception('deep({}) error'.format(deep))
+
+    statement = text[start_pos:end_pos]
+    return ((place_hoder_num, arg_num, statement))
+
+bad_log_fmt = """
+{} [line {}] : {{}} = {}, argc = {}
+"""+Fore.RED+"""{}
+"""+Style.RESET_ALL
+
+def check(files, show_ok):
+    if len(files) == 0:
+        return
+    max_file_name_len = max([len(file_name) for file_name in files])
+
+    bad_files = []
+
+    if show_ok == None:
+        show_ok = len(files) <= 128
+
+    with Progress() as progress:
+        task = progress.add_task("[red]checking...", total=len(files))
+
+        for source_file in files:
+            try:
+                text = open(source_file, encoding='utf-8').read().replace('\\\"', '').replace('\\\'', '')
+            except UnicodeDecodeError:
+                print('\n can not read file `{}`'.format(source_file))
+                continue
+            iter = re.finditer('(LOG[T|D|I|W|E|C]\(|fmt::format\()', text, re.MULTILINE)
+
+            bad_fmt = []
+            log_len = 0
+            for item in iter:
+                log_len = log_len+1
+                key_word = item.group()
+                location = len(re.findall('\n', text[:item.start()])) + 1
+                try:
+                    place_hoder_num, arg_num, statement = parse(text, item.start())
+                except Exception as e:
+                    g_unknow_logs.append({'file':source_file, 'line':location, 'exception': e, 'key_word':key_word})
+                    continue
+                    
+                if place_hoder_num != arg_num:
+                    print(bad_log_fmt.format(source_file, location, place_hoder_num, arg_num, statement))
+                    bad_fmt.append((key_word, place_hoder_num, arg_num))
+                
+            space_num = max_file_name_len-len(source_file)
+            if len(bad_fmt) == 0:
+                if show_ok:
+                    space_num = max_file_name_len-len(source_file)
+                    print((Fore.GREEN+'{}{} all {:2} `Fmt` ok'+Style.RESET_ALL).format(source_file, ' '*space_num, log_len))
+            else:
+                print('{}{} {:2} bad `Fmt` total in {} `Fmt`\n'.format(source_file, ' '*space_num, len(bad_fmt), log_len))
+                bad_files.append({'source_file':source_file, 'bad_fmt': bad_fmt})
+            
+            if not show_ok:
+                progress.advance(task)
+
+    print()
+    print()
+    print('({}/{})(badfile/total) {:3} bad `Fmt` total'.format(len(bad_files), len(files), sum([len(bad_file['bad_fmt']) for bad_file in bad_files])))
+    print()
+    print()
+    print()
+    print('{} unknown `Fmt`:'.format(len(g_unknow_logs)))
+    for log in g_unknow_logs:
+        print(log)
+
+def main():
+    if '-help' in sys.argv or '-h' in sys.argv:
+        print(help)
+        exit()
+
+    default_types = ['.cpp', '.h', '.hpp', '.mm']
+    show_ok = None
+    show_ok_res = {
+       '-S'       : True,
+       '-show_ok' : True,
+       '-H'       : False,
+       '-hide_ok' : False,
+    }
+    for arg in show_ok_res:
+        if arg in sys.argv:
+            sys.argv.remove(arg)
+            show_ok = show_ok_res[arg]
+        
+    if len(sys.argv) > 1:
+        files = []
+        for arg in sys.argv[1:]:
+            if os.path.isdir(arg):
+                files = files + getfiles(arg, default_types)
+            elif os.path.isfile(arg):
+                files.append(arg)
+                print('{} is file'.format(arg))
+            else:
+                print('`{}` is not file or dir!!!'.format(arg))
+        check(files, show_ok)
+    else:
+        check(getfiles('./', default_types), show_ok)
+
+if __name__ == "__main__":
+    main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

