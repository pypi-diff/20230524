# Comparing `tmp/socservthread-1.1.3.tar.gz` & `tmp/socservthread-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socservthread-1.1.3.tar", last modified: Mon May 22 16:23:43 2023, max compression
+gzip compressed data, was "socservthread-1.1.4.tar", last modified: Wed May 24 14:18:36 2023, max compression
```

## Comparing `socservthread-1.1.3.tar` & `socservthread-1.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 16:23:43.997983 socservthread-1.1.3/
--rw-rw-rw-   0        0        0     1094 2021-02-10 19:27:17.000000 socservthread-1.1.3/LICENCE
--rw-rw-rw-   0        0        0      509 2023-05-22 16:23:43.997983 socservthread-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-05-22 14:50:28.000000 socservthread-1.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 16:23:43.997983 socservthread-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      733 2023-05-22 16:23:09.000000 socservthread-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:23:43.985474 socservthread-1.1.3/socservthread/
--rw-rw-rw-   0        0        0        2 2021-02-10 19:41:50.000000 socservthread-1.1.3/socservthread/__init__.py
--rw-rw-rw-   0        0        0     5194 2023-05-22 16:22:09.000000 socservthread-1.1.3/socservthread/socservthread.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:23:43.997983 socservthread-1.1.3/socservthread.egg-info/
--rw-rw-rw-   0        0        0      509 2023-05-22 16:23:43.000000 socservthread-1.1.3/socservthread.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-05-22 16:23:43.000000 socservthread-1.1.3/socservthread.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 16:23:43.000000 socservthread-1.1.3/socservthread.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-22 16:23:43.000000 socservthread-1.1.3/socservthread.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 14:18:36.704614 socservthread-1.1.4/
+-rw-rw-rw-   0        0        0     1094 2021-02-10 19:27:17.000000 socservthread-1.1.4/LICENCE
+-rw-rw-rw-   0        0        0      509 2023-05-24 14:18:36.704614 socservthread-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      116 2023-05-22 14:50:28.000000 socservthread-1.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-24 14:18:36.704614 socservthread-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      733 2023-05-24 14:12:54.000000 socservthread-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 14:18:36.692512 socservthread-1.1.4/socservthread/
+-rw-rw-rw-   0        0        0        2 2021-02-10 19:41:50.000000 socservthread-1.1.4/socservthread/__init__.py
+-rw-rw-rw-   0        0        0     5201 2023-05-24 14:17:10.000000 socservthread-1.1.4/socservthread/socservthread.py
+drwxrwxrwx   0        0        0        0 2023-05-24 14:18:36.699356 socservthread-1.1.4/socservthread.egg-info/
+-rw-rw-rw-   0        0        0      509 2023-05-24 14:18:36.000000 socservthread-1.1.4/socservthread.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-05-24 14:18:36.000000 socservthread-1.1.4/socservthread.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 14:18:36.000000 socservthread-1.1.4/socservthread.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-24 14:18:36.000000 socservthread-1.1.4/socservthread.egg-info/top_level.txt
```

### Comparing `socservthread-1.1.3/LICENCE` & `socservthread-1.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `socservthread-1.1.3/setup.py` & `socservthread-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="socservthread", # Replace with your own username
-    version="1.1.3",
+    version="1.1.4",
     author="Didier Orlandi",
     author_email="didier.orlandi@wanadoo.fr",
     description="Serveur TCP socket",
     long_description=long_description,
     long_description_content_type="text/markdown",
     #url="https://github.com/",
     packages=setuptools.find_packages(),
```

### Comparing `socservthread-1.1.3/socservthread/socservthread.py` & `socservthread-1.1.4/socservthread/socservthread.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,25 +38,25 @@
                             #print("queue size : ")
                             #qa = self.queue.qsize()
                             #print(qa)                    
                             #print("réception & entré 1er sorti :")
 
             except:
                 #pass
-                print("exception pour TCP server  ....")
+                print("exception pour TCP Client  ....")
             finally:
                 if self.exit_event.is_set():# si événement d'arrêt du thread est envoyé on arrête le thread
-                    print("on a arrêté le thread tcp server  ! ")   
+                    print("on a arrêté le thread tcp client  ! ")   
                     self.close()
                     break
 
     def close(self):
         self.clientsocket.shutdown(socket.SHUT_RDWR)
         self.clientsocket.close()
-        print ("server TCP closed")
+        print ("server TCP client closed")
 
 #-----------------------------------------------------
 class tcp_server(threading.Thread):
     
     def __init__(self, hostServer, portServer, _SizeStruc=["<ff",8]):      # arguments du de la classe
         threading.Thread.__init__(self)  # ne pas oublier cette ligne
         # (appel au constructeur de la classe mère)
@@ -92,12 +92,12 @@
                 #pass
                 print("exception pour TCP server ....")
             finally:
                 if self.exit_event.is_set():# si événement d'arrêt du thread est envoyé on arrête le thread
                     print("on a arrêté le thread TCP server ! ")
                     if newClient != None:
                         print("on ferme le socket")
-                        #newClient.exit_event.set()# on envoie l'événement d'arrêt au thread client
-                        newClient.close()
+                        newClient.exit_event.set()# on envoie l'événement d'arrêt au thread client
+                        #newClient.close()
                     break
 
 #-----------------------------------------------------
```

