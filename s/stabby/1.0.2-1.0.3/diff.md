# Comparing `tmp/stabby-1.0.2.tar.gz` & `tmp/stabby-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stabby-1.0.2.tar", last modified: Tue May 23 09:01:54 2023, max compression
+gzip compressed data, was "stabby-1.0.3.tar", last modified: Wed May 24 03:01:48 2023, max compression
```

## Comparing `stabby-1.0.2.tar` & `stabby-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:01:54.580117 stabby-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-23 09:01:54.580117 stabby-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-23 09:01:40.000000 stabby-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 09:01:54.580117 stabby-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-23 09:01:40.000000 stabby-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:01:54.580117 stabby-1.0.2/simple_tabby/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:01:40.000000 stabby-1.0.2/simple_tabby/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-23 09:01:40.000000 stabby-1.0.2/simple_tabby/stabby.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:01:54.580117 stabby-1.0.2/stabby.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-23 09:01:54.000000 stabby-1.0.2/stabby.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-23 09:01:54.000000 stabby-1.0.2/stabby.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:01:54.000000 stabby-1.0.2/stabby.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 09:01:54.000000 stabby-1.0.2/stabby.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-23 09:01:54.000000 stabby-1.0.2/stabby.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 09:01:54.000000 stabby-1.0.2/stabby.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:01:48.968495 stabby-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-24 03:01:48.968495 stabby-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-24 03:01:37.000000 stabby-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 03:01:48.968495 stabby-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-24 03:01:37.000000 stabby-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:01:48.968495 stabby-1.0.3/simple_tabby/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 03:01:37.000000 stabby-1.0.3/simple_tabby/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-24 03:01:37.000000 stabby-1.0.3/simple_tabby/stabby.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:01:48.968495 stabby-1.0.3/stabby.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-24 03:01:48.000000 stabby-1.0.3/stabby.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-24 03:01:48.000000 stabby-1.0.3/stabby.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 03:01:48.000000 stabby-1.0.3/stabby.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-24 03:01:48.000000 stabby-1.0.3/stabby.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-24 03:01:48.000000 stabby-1.0.3/stabby.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-24 03:01:48.000000 stabby-1.0.3/stabby.egg-info/top_level.txt
```

### Comparing `stabby-1.0.2/PKG-INFO` & `stabby-1.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stabby
-Version: 1.0.2
+Version: 1.0.3
 Summary: A helper for ssh operate in terminal
 Home-page: https://github.com/Booooooger/simple_tabby
 Author: yombo
 Author-email: yombo@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -31,35 +31,54 @@
 ```
 
 # Usage
 
 ## add your first remote server config 
 run command `stabby add ` , follow promotes input server configuration , like below:
 ```shell
-
+usage: stabby add [-h] -s S -p P [-port PORT] [-u U] [-n N]                                                    
+                                                                                                        
+optional arguments:                                                                                            
+  -h, --help  show this help message and exit                                                                  
+  -s S        remote server host                                                                               
+  -p P        remote server password                                                                           
+  -port PORT  remote server ssh port                                                                           
+  -u U        remote server user name                                                                          
+  -n N        remote server name   
+```
+example :
+```shell
+stabby add -s 192.168.1.253 -p password123 -n dev
 ```
 
 ## connect to remote server
 
 run command `stabby` ,you can see as below:
 
+![image](./docs/1684896760610.jpg)
 
+you can select one remote server that you have added to connect by **KEY_UP** 、**KEY_DOWN** or **KEY_LEFT** 、**KEY_RIGHT** 
+
+as you also can open ssh tunnue with `-t` command arg ,for example:
+```shell
+# stabby -t localport:remoteport
+stabby -t 6041:5041
+```
 
 # How does it work
 
 It's so easy. Default , stabby(simple_tabby) loads config file under `$USER_HOME/.simple_tabby/default.json`, file content like below:
 
 ```json
 [
   {
-    "name": "name",
+    "title": "title for remote server",
     "host": "remote server ip or host",
     "port": 22,
-    "user": "remote user",
+    "user": "remote user ,default is root",
     "password": "remote password",
-    "privateKey": "ssh key path",
   }
 ]
 ```
 
-and the file need to create by yourself. you can use different json file to group your remote server information. if load file success, stabby will print as table like below:
-
+when stabby is running, it loads file as json objects,let user can see all server
+![](docs/1684896760610.jpg)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stabby-1.0.2/README.md` & `stabby-1.0.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -20,35 +20,54 @@
 ```
 
 # Usage
 
 ## add your first remote server config 
 run command `stabby add ` , follow promotes input server configuration , like below:
 ```shell
-
+usage: stabby add [-h] -s S -p P [-port PORT] [-u U] [-n N]                                                    
+                                                                                                        
+optional arguments:                                                                                            
+  -h, --help  show this help message and exit                                                                  
+  -s S        remote server host                                                                               
+  -p P        remote server password                                                                           
+  -port PORT  remote server ssh port                                                                           
+  -u U        remote server user name                                                                          
+  -n N        remote server name   
+```
+example :
+```shell
+stabby add -s 192.168.1.253 -p password123 -n dev
 ```
 
 ## connect to remote server
 
 run command `stabby` ,you can see as below:
 
+![image](./docs/1684896760610.jpg)
 
+you can select one remote server that you have added to connect by **KEY_UP** 、**KEY_DOWN** or **KEY_LEFT** 、**KEY_RIGHT** 
+
+as you also can open ssh tunnue with `-t` command arg ,for example:
+```shell
+# stabby -t localport:remoteport
+stabby -t 6041:5041
+```
 
 # How does it work
 
 It's so easy. Default , stabby(simple_tabby) loads config file under `$USER_HOME/.simple_tabby/default.json`, file content like below:
 
 ```json
 [
   {
-    "name": "name",
+    "title": "title for remote server",
     "host": "remote server ip or host",
     "port": 22,
-    "user": "remote user",
+    "user": "remote user ,default is root",
     "password": "remote password",
-    "privateKey": "ssh key path",
   }
 ]
 ```
 
-and the file need to create by yourself. you can use different json file to group your remote server information. if load file success, stabby will print as table like below:
-
+when stabby is running, it loads file as json objects,let user can see all server
+![](docs/1684896760610.jpg)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stabby-1.0.2/setup.py` & `stabby-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("README.md", "r") as fh:
 
     long_description = fh.read()
 
 setup(
     name='stabby',
-    version='1.0.2',
+    version='1.0.3',
     author="yombo",
     author_email="yombo@qq.com",
     url="https://github.com/Booooooger/simple_tabby",
     description="A helper for ssh operate in terminal",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

### Comparing `stabby-1.0.2/simple_tabby/stabby.py` & `stabby-1.0.3/simple_tabby/stabby.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,22 +24,30 @@
         print("trying to login server with ssh-key, if you has config password, the password has copied to clip, just pasted and enter!!")
 
     if (args.tunnet):
         ports = args.tunnet.split(":")
         command = f"ssh -L {ports[0]}:127.0.0.1:{ports[1]} -N -f {user}@{host}"
         print("-> run command :",command)
         i = os.system(command)
-
-    os.system(f"ssh {user}@{host} -p {port} -i {private_key}")
-
+    else:
+       command = f"ssh {user}@{host} -p {port} -i {private_key}"
+       print("-> run command :",command)
+       os.system(command)
+
+def pc(args):
+    if args is not None:
+        for config in SSH_SERVER_CONFIGS:
+            if config['title']==args :
+                return f"host:{config['host']} \nport:{config['port']}\nuser:{config['user']}\n"
+    return None
    
 def show_options():
     from simple_term_menu import TerminalMenu
     options = [SSH_SERVER_CONFIGS[i]['title'] for i in range(len(SSH_SERVER_CONFIGS))]
-    ternimal_menu = TerminalMenu(options,show_search_hint=True,quit_keys=["q"])
+    ternimal_menu = TerminalMenu(options,show_search_hint=True,quit_keys=["q"],preview_command=pc, preview_size=0.75)
     return ternimal_menu.show()
 
 def save_file():
     with open(os.path.join(DEFAULT_CONFIG_PATH,'default.json'),'w') as f:
         f.write(json.dumps(SSH_SERVER_CONFIGS,indent=4,sort_keys=True))
 
 
@@ -52,38 +60,38 @@
         SSH_SERVER_CONFIGS = SSH_SERVER_CONFIGS+configs
 
 def add(args):
     load_config()
     SSH_SERVER_CONFIGS.append({
         'title':args.n if args.n else args.s,
         'host':args.s,
-        'user':args.s,
-        'password':args.pwd,
+        'user':args.u,
+        'password':args.p,
         'port':args.port
     })
-    print(SSH_SERVER_CONFIGS)
-    # save_file()
+    save_file()
 
 def login(args):
     load_config()
     selected_idx = show_options()
-    selected_config = SSH_SERVER_CONFIGS[selected_idx]
-    connect(selected_config,args)
+    if(selected_idx is not None):
+        selected_config = SSH_SERVER_CONFIGS[selected_idx]
+        connect(selected_config,args)
     
 def main():
     parser = argparse.ArgumentParser(description="Mini tool login remote ssh server ", add_help=True)
     parser.add_argument('-t', '--tunnet', type=str, required=False,nargs='?',
                     help="open tunnet with ssh localport:remoteport")
     parser.set_defaults(func=login)
     
     subparsers = parser.add_subparsers(help='sub-command help')
     add_parser = subparsers.add_parser('add',help="add new server config")
     add_parser.add_argument('-s',type=str,required=True,help="remote server host")
-    add_parser.add_argument('-pwd',type=str,required=True,help="remote server password")
-    add_parser.add_argument('-p',type=int,default=22,help="remote server ssh port")
+    add_parser.add_argument('-p',type=str,required=True,help="remote server password")
+    add_parser.add_argument('-port',type=int,default=22,help="remote server ssh port")
     add_parser.add_argument('-u',type=str,default="root",help="remote server user name ")
     add_parser.add_argument('-n',type=str,default=None,help="remote server name ")
     add_parser.set_defaults(func=add)
     
     args = parser.parse_args()
     args.func(args)
```

### Comparing `stabby-1.0.2/stabby.egg-info/PKG-INFO` & `stabby-1.0.3/stabby.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stabby
-Version: 1.0.2
+Version: 1.0.3
 Summary: A helper for ssh operate in terminal
 Home-page: https://github.com/Booooooger/simple_tabby
 Author: yombo
 Author-email: yombo@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -31,35 +31,54 @@
 ```
 
 # Usage
 
 ## add your first remote server config 
 run command `stabby add ` , follow promotes input server configuration , like below:
 ```shell
-
+usage: stabby add [-h] -s S -p P [-port PORT] [-u U] [-n N]                                                    
+                                                                                                        
+optional arguments:                                                                                            
+  -h, --help  show this help message and exit                                                                  
+  -s S        remote server host                                                                               
+  -p P        remote server password                                                                           
+  -port PORT  remote server ssh port                                                                           
+  -u U        remote server user name                                                                          
+  -n N        remote server name   
+```
+example :
+```shell
+stabby add -s 192.168.1.253 -p password123 -n dev
 ```
 
 ## connect to remote server
 
 run command `stabby` ,you can see as below:
 
+![image](./docs/1684896760610.jpg)
 
+you can select one remote server that you have added to connect by **KEY_UP** 、**KEY_DOWN** or **KEY_LEFT** 、**KEY_RIGHT** 
+
+as you also can open ssh tunnue with `-t` command arg ,for example:
+```shell
+# stabby -t localport:remoteport
+stabby -t 6041:5041
+```
 
 # How does it work
 
 It's so easy. Default , stabby(simple_tabby) loads config file under `$USER_HOME/.simple_tabby/default.json`, file content like below:
 
 ```json
 [
   {
-    "name": "name",
+    "title": "title for remote server",
     "host": "remote server ip or host",
     "port": 22,
-    "user": "remote user",
+    "user": "remote user ,default is root",
     "password": "remote password",
-    "privateKey": "ssh key path",
   }
 ]
 ```
 
-and the file need to create by yourself. you can use different json file to group your remote server information. if load file success, stabby will print as table like below:
-
+when stabby is running, it loads file as json objects,let user can see all server
+![](docs/1684896760610.jpg)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

