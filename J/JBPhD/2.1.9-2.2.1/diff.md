# Comparing `tmp/JBPhD-2.1.9.tar.gz` & `tmp/JBPhD-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JBPhD-2.1.9.tar", last modified: Wed May 24 10:24:24 2023, max compression
+gzip compressed data, was "JBPhD-2.2.1.tar", last modified: Wed May 24 10:33:07 2023, max compression
```

## Comparing `JBPhD-2.1.9.tar` & `JBPhD-2.2.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 10:24:20.000000 JBPhD-2.1.9/
-drwxrwxrwx   0        0        0        0 2023-05-24 10:24:20.000000 JBPhD-2.1.9/JBPhD.egg-info/
--rw-rw-rw-   0        0        0      201 2023-05-24 10:24:20.000000 JBPhD-2.1.9/JBPhD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1716 2023-05-24 10:24:20.000000 JBPhD-2.1.9/JBPhD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 10:24:20.000000 JBPhD-2.1.9/JBPhD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-24 10:24:20.000000 JBPhD-2.1.9/JBPhD.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      147 2023-05-24 10:24:20.000000 JBPhD-2.1.9/JBPhD.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-24 10:24:20.000000 JBPhD-2.1.9/JBPhD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       26 2023-05-07 16:04:18.000000 JBPhD-2.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0      201 2023-05-24 10:24:24.000000 JBPhD-2.1.9/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-05-07 16:42:22.000000 JBPhD-2.1.9/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 10:24:20.000000 JBPhD-2.1.9/Task/
--rw-rw-rw-   0        0        0     2489 2023-05-18 22:38:28.000000 JBPhD-2.1.9/Task/Analysis.py
--rw-rw-rw-   0        0        0     2336 2023-04-20 18:29:48.000000 JBPhD-2.1.9/Task/Api.json
--rw-rw-rw-   0        0        0     2332 2023-04-30 20:14:46.000000 JBPhD-2.1.9/Task/Api2.json
--rw-rw-rw-   0        0        0   256511 2023-05-07 17:28:42.000000 JBPhD-2.1.9/Task/Back_Right.PNG
--rw-rw-rw-   0        0        0    60437 2023-02-02 09:16:10.000000 JBPhD-2.1.9/Task/Consent Form.docx
--rw-rw-rw-   0        0        0       18 2023-05-15 21:31:52.000000 JBPhD-2.1.9/Task/Consent Form.txt
--rw-rw-rw-   0        0        0      911 2023-05-18 15:51:28.000000 JBPhD-2.1.9/Task/Dependencies.py
--rw-rw-rw-   0        0        0    12338 2023-05-18 15:51:04.000000 JBPhD-2.1.9/Task/Dependency Installation.py
--rw-rw-rw-   0        0        0      552 2023-05-06 17:47:44.000000 JBPhD-2.1.9/Task/Email Output.py
--rw-rw-rw-   0        0        0      202 2023-05-07 16:32:10.000000 JBPhD-2.1.9/Task/Experimental Run Trial.py
--rw-rw-rw-   0        0        0     4074 2023-05-18 15:48:40.000000 JBPhD-2.1.9/Task/Export.py
--rw-rw-rw-   0        0        0   249107 2023-05-07 17:28:42.000000 JBPhD-2.1.9/Task/Front_Left.PNG
--rw-rw-rw-   0        0        0   249006 2023-05-07 17:28:42.000000 JBPhD-2.1.9/Task/Front_Right.PNG
--rw-rw-rw-   0        0        0     1184 2023-05-15 13:38:26.000000 JBPhD-2.1.9/Task/Gradient Background.py
--rw-rw-rw-   0        0        0      883 2023-04-14 22:45:36.000000 JBPhD-2.1.9/Task/Graph.py
--rw-rw-rw-   0        0        0   281708 2023-04-07 13:54:00.000000 JBPhD-2.1.9/Task/ImageSample.PNG
--rw-rw-rw-   0        0        0   256274 2023-05-07 17:28:42.000000 JBPhD-2.1.9/Task/Inverse_Back_Left.PNG
--rw-rw-rw-   0        0        0      384 2023-04-24 19:08:56.000000 JBPhD-2.1.9/Task/Location.py
--rw-rw-rw-   0        0        0       54 2023-05-07 14:35:12.000000 JBPhD-2.1.9/Task/MANIFEST.in.txt
--rw-rw-rw-   0        0        0    14031 2023-04-07 13:54:00.000000 JBPhD-2.1.9/Task/Manikin Back Down Left.png
--rw-rw-rw-   0        0        0    13918 2023-04-07 13:54:00.000000 JBPhD-2.1.9/Task/Manikin Back Up Right.png
--rw-rw-rw-   0        0        0    16784 2023-04-07 13:54:00.000000 JBPhD-2.1.9/Task/Manikin front Down Right.png
--rw-rw-rw-   0        0        0    20357 2023-04-07 13:54:00.000000 JBPhD-2.1.9/Task/Manikin front Up Right.png
--rw-rw-rw-   0        0        0     3101 2023-05-18 16:38:38.000000 JBPhD-2.1.9/Task/N-Back Revision.py
--rw-rw-rw-   0        0        0        2 2023-05-18 19:20:22.000000 JBPhD-2.1.9/Task/N-Back count.txt
--rw-rw-rw-   0        0        0    19276 2023-05-18 19:25:40.000000 JBPhD-2.1.9/Task/N-Back.py
-drwxrwxrwx   0        0        0        0 2023-05-24 10:24:20.000000 JBPhD-2.1.9/Task/Participant 90210/
--rw-rw-rw-   0        0        0     3063 2023-05-18 22:28:16.000000 JBPhD-2.1.9/Task/Participant 90210/90210 - Combined Reaction Times.csv
--rw-rw-rw-   0        0        0     2640 2023-05-18 22:09:26.000000 JBPhD-2.1.9/Task/Participant 90210/90210 - Combined Scores.csv
--rw-rw-rw-   0        0        0     4421 2023-05-18 19:19:36.000000 JBPhD-2.1.9/Task/Participant 90210/90210 - N-Back Reaction Times.csv
--rw-rw-rw-   0        0        0     2650 2023-05-18 19:19:36.000000 JBPhD-2.1.9/Task/Participant 90210/90210 - N-Back Score.csv
--rwxrwxrwx   0        0        0      680 2023-04-23 19:01:06.000000 JBPhD-2.1.9/Task/Python Install.bat
--rw-rw-rw-   0        0        0       20 2023-05-07 14:41:38.000000 JBPhD-2.1.9/Task/README.txt.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 22:01:58.000000 JBPhD-2.1.9/Task/RT count.txt
--rw-rw-rw-   0        0        0    17877 2023-05-18 15:42:10.000000 JBPhD-2.1.9/Task/Reaction Time Task - Copy.py
--rwxrwxrwx   0        0        0      448 2023-05-07 14:17:02.000000 JBPhD-2.1.9/Task/Suffix.bat
--rw-rw-rw-   0        0        0        4 2023-05-15 11:59:06.000000 JBPhD-2.1.9/Task/Switch Count.txt
--rw-rw-rw-   0        0        0    24157 2023-05-15 10:24:58.000000 JBPhD-2.1.9/Task/Switching.py
--rw-rw-rw-   0        0        0    13650 2023-05-18 15:49:20.000000 JBPhD-2.1.9/Task/Task.py
--rw-rw-rw-   0        0        0     6625 2023-05-18 22:04:18.000000 JBPhD-2.1.9/Task/Trial.py
-drwxrwxrwx   0        0        0        0 2023-05-24 10:24:20.000000 JBPhD-2.1.9/Task/__pycache__/
--rw-rw-rw-   0        0        0     5027 2023-05-07 22:15:14.000000 JBPhD-2.1.9/Task/__pycache__/Dependencies.cpython-311.pyc
--rw-rw-rw-   0        0        0     6694 2023-05-06 18:08:18.000000 JBPhD-2.1.9/Task/__pycache__/Export.cpython-311.pyc
--rw-rw-rw-   0        0        0      696 2023-05-04 10:46:06.000000 JBPhD-2.1.9/Task/__pycache__/Location.cpython-311.pyc
--rw-rw-rw-   0        0        0    18767 2023-05-07 22:15:14.000000 JBPhD-2.1.9/Task/__pycache__/Task.cpython-311.pyc
--rw-rw-rw-   0        0        0      931 2023-05-05 14:18:56.000000 JBPhD-2.1.9/Task/__pycache__/spwf.cpython-311.pyc
--rw-rw-rw-   0        0        0     3162 2023-04-07 13:54:00.000000 JBPhD-2.1.9/Task/asterisk.png
--rw-rw-rw-   0        0        0    47189 2023-04-07 13:54:00.000000 JBPhD-2.1.9/Task/circle.jpg
--rw-rw-rw-   0        0        0    12363 2023-04-07 13:54:00.000000 JBPhD-2.1.9/Task/greendot.png
--rw-rw-rw-   0        0        0    38788 2023-04-07 13:54:00.000000 JBPhD-2.1.9/Task/greentick.png
--rw-rw-rw-   0        0        0       54 2023-05-07 14:31:32.000000 JBPhD-2.1.9/Task/help.txt
--rw-rw-rw-   0        0        0        5 2023-05-18 15:38:22.000000 JBPhD-2.1.9/Task/participant number.txt
--rw-rw-rw-   0        0        0      491 2023-05-14 16:12:16.000000 JBPhD-2.1.9/Task/pins.csv
--rw-rw-rw-   0        0        0    24503 2023-04-07 13:54:00.000000 JBPhD-2.1.9/Task/redcross.png
--rw-rw-rw-   0        0        0    98588 2023-04-07 13:54:00.000000 JBPhD-2.1.9/Task/reddot.png
--rw-rw-rw-   0        0        0      566 2023-05-07 14:26:16.000000 JBPhD-2.1.9/Task/setup.py
--rw-rw-rw-   0        0        0      472 2023-05-05 14:17:12.000000 JBPhD-2.1.9/Task/spwf.py
--rw-rw-rw-   0        0        0       44 2023-04-24 16:27:34.000000 JBPhD-2.1.9/Task/spwfoutput.txt
--rw-rw-rw-   0        0        0      100 2023-04-24 16:27:34.000000 JBPhD-2.1.9/Task/spwfvalue.txt
--rw-rw-rw-   0        0        0       14 2023-05-15 13:41:08.000000 JBPhD-2.1.9/Task/suffix.txt
--rw-rw-rw-   0        0        0   161693 2023-04-07 13:54:00.000000 JBPhD-2.1.9/Task/trial.jpeg
--rw-rw-rw-   0        0        0   432254 2023-05-04 10:35:10.000000 JBPhD-2.1.9/Task/uop.ico
--rw-rw-rw-   0        0        0     3908 2023-05-04 10:32:40.000000 JBPhD-2.1.9/Task/uop.jpeg
--rw-rw-rw-   0        0        0     7038 2023-04-16 20:40:14.000000 JBPhD-2.1.9/Task/uop.png
--rw-rw-rw-   0        0        0       42 2023-05-24 10:24:24.000000 JBPhD-2.1.9/setup.cfg
--rw-rw-rw-   0        0        0      855 2023-05-24 10:23:56.000000 JBPhD-2.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:33:06.000000 JBPhD-2.2.1/
+drwxrwxrwx   0        0        0        0 2023-05-24 10:33:06.000000 JBPhD-2.2.1/JBPhD.egg-info/
+-rw-rw-rw-   0        0        0      257 2023-05-24 10:33:06.000000 JBPhD-2.2.1/JBPhD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1716 2023-05-24 10:33:06.000000 JBPhD-2.2.1/JBPhD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 10:33:06.000000 JBPhD-2.2.1/JBPhD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-24 10:33:06.000000 JBPhD-2.2.1/JBPhD.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      147 2023-05-24 10:33:06.000000 JBPhD-2.2.1/JBPhD.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-24 10:33:06.000000 JBPhD-2.2.1/JBPhD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       26 2023-05-07 16:04:18.000000 JBPhD-2.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      257 2023-05-24 10:33:08.000000 JBPhD-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-05-07 16:42:22.000000 JBPhD-2.2.1/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 10:33:06.000000 JBPhD-2.2.1/Task/
+-rw-rw-rw-   0        0        0     2489 2023-05-18 22:38:28.000000 JBPhD-2.2.1/Task/Analysis.py
+-rw-rw-rw-   0        0        0     2336 2023-04-20 18:29:48.000000 JBPhD-2.2.1/Task/Api.json
+-rw-rw-rw-   0        0        0     2332 2023-04-30 20:14:46.000000 JBPhD-2.2.1/Task/Api2.json
+-rw-rw-rw-   0        0        0   256511 2023-05-07 17:28:42.000000 JBPhD-2.2.1/Task/Back_Right.PNG
+-rw-rw-rw-   0        0        0    60437 2023-02-02 09:16:10.000000 JBPhD-2.2.1/Task/Consent Form.docx
+-rw-rw-rw-   0        0        0       18 2023-05-15 21:31:52.000000 JBPhD-2.2.1/Task/Consent Form.txt
+-rw-rw-rw-   0        0        0      911 2023-05-18 15:51:28.000000 JBPhD-2.2.1/Task/Dependencies.py
+-rw-rw-rw-   0        0        0    12338 2023-05-18 15:51:04.000000 JBPhD-2.2.1/Task/Dependency Installation.py
+-rw-rw-rw-   0        0        0      552 2023-05-06 17:47:44.000000 JBPhD-2.2.1/Task/Email Output.py
+-rw-rw-rw-   0        0        0      202 2023-05-07 16:32:10.000000 JBPhD-2.2.1/Task/Experimental Run Trial.py
+-rw-rw-rw-   0        0        0     4074 2023-05-18 15:48:40.000000 JBPhD-2.2.1/Task/Export.py
+-rw-rw-rw-   0        0        0   249107 2023-05-07 17:28:42.000000 JBPhD-2.2.1/Task/Front_Left.PNG
+-rw-rw-rw-   0        0        0   249006 2023-05-07 17:28:42.000000 JBPhD-2.2.1/Task/Front_Right.PNG
+-rw-rw-rw-   0        0        0     1184 2023-05-15 13:38:26.000000 JBPhD-2.2.1/Task/Gradient Background.py
+-rw-rw-rw-   0        0        0      883 2023-04-14 22:45:36.000000 JBPhD-2.2.1/Task/Graph.py
+-rw-rw-rw-   0        0        0   281708 2023-04-07 13:54:00.000000 JBPhD-2.2.1/Task/ImageSample.PNG
+-rw-rw-rw-   0        0        0   256274 2023-05-07 17:28:42.000000 JBPhD-2.2.1/Task/Inverse_Back_Left.PNG
+-rw-rw-rw-   0        0        0      384 2023-04-24 19:08:56.000000 JBPhD-2.2.1/Task/Location.py
+-rw-rw-rw-   0        0        0       54 2023-05-07 14:35:12.000000 JBPhD-2.2.1/Task/MANIFEST.in.txt
+-rw-rw-rw-   0        0        0    14031 2023-04-07 13:54:00.000000 JBPhD-2.2.1/Task/Manikin Back Down Left.png
+-rw-rw-rw-   0        0        0    13918 2023-04-07 13:54:00.000000 JBPhD-2.2.1/Task/Manikin Back Up Right.png
+-rw-rw-rw-   0        0        0    16784 2023-04-07 13:54:00.000000 JBPhD-2.2.1/Task/Manikin front Down Right.png
+-rw-rw-rw-   0        0        0    20357 2023-04-07 13:54:00.000000 JBPhD-2.2.1/Task/Manikin front Up Right.png
+-rw-rw-rw-   0        0        0     3101 2023-05-18 16:38:38.000000 JBPhD-2.2.1/Task/N-Back Revision.py
+-rw-rw-rw-   0        0        0        2 2023-05-18 19:20:22.000000 JBPhD-2.2.1/Task/N-Back count.txt
+-rw-rw-rw-   0        0        0    19276 2023-05-18 19:25:40.000000 JBPhD-2.2.1/Task/N-Back.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:33:06.000000 JBPhD-2.2.1/Task/Participant 90210/
+-rw-rw-rw-   0        0        0     3063 2023-05-18 22:28:16.000000 JBPhD-2.2.1/Task/Participant 90210/90210 - Combined Reaction Times.csv
+-rw-rw-rw-   0        0        0     2640 2023-05-18 22:09:26.000000 JBPhD-2.2.1/Task/Participant 90210/90210 - Combined Scores.csv
+-rw-rw-rw-   0        0        0     4421 2023-05-18 19:19:36.000000 JBPhD-2.2.1/Task/Participant 90210/90210 - N-Back Reaction Times.csv
+-rw-rw-rw-   0        0        0     2650 2023-05-18 19:19:36.000000 JBPhD-2.2.1/Task/Participant 90210/90210 - N-Back Score.csv
+-rwxrwxrwx   0        0        0      680 2023-04-23 19:01:06.000000 JBPhD-2.2.1/Task/Python Install.bat
+-rw-rw-rw-   0        0        0       20 2023-05-07 14:41:38.000000 JBPhD-2.2.1/Task/README.txt.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 22:01:58.000000 JBPhD-2.2.1/Task/RT count.txt
+-rw-rw-rw-   0        0        0    17877 2023-05-18 15:42:10.000000 JBPhD-2.2.1/Task/Reaction Time Task - Copy.py
+-rwxrwxrwx   0        0        0      448 2023-05-07 14:17:02.000000 JBPhD-2.2.1/Task/Suffix.bat
+-rw-rw-rw-   0        0        0        4 2023-05-15 11:59:06.000000 JBPhD-2.2.1/Task/Switch Count.txt
+-rw-rw-rw-   0        0        0    24157 2023-05-15 10:24:58.000000 JBPhD-2.2.1/Task/Switching.py
+-rw-rw-rw-   0        0        0    13650 2023-05-18 15:49:20.000000 JBPhD-2.2.1/Task/Task.py
+-rw-rw-rw-   0        0        0     6625 2023-05-18 22:04:18.000000 JBPhD-2.2.1/Task/Trial.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:33:06.000000 JBPhD-2.2.1/Task/__pycache__/
+-rw-rw-rw-   0        0        0     5027 2023-05-07 22:15:14.000000 JBPhD-2.2.1/Task/__pycache__/Dependencies.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6694 2023-05-06 18:08:18.000000 JBPhD-2.2.1/Task/__pycache__/Export.cpython-311.pyc
+-rw-rw-rw-   0        0        0      696 2023-05-04 10:46:06.000000 JBPhD-2.2.1/Task/__pycache__/Location.cpython-311.pyc
+-rw-rw-rw-   0        0        0    18767 2023-05-07 22:15:14.000000 JBPhD-2.2.1/Task/__pycache__/Task.cpython-311.pyc
+-rw-rw-rw-   0        0        0      931 2023-05-05 14:18:56.000000 JBPhD-2.2.1/Task/__pycache__/spwf.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3162 2023-04-07 13:54:00.000000 JBPhD-2.2.1/Task/asterisk.png
+-rw-rw-rw-   0        0        0    47189 2023-04-07 13:54:00.000000 JBPhD-2.2.1/Task/circle.jpg
+-rw-rw-rw-   0        0        0    12363 2023-04-07 13:54:00.000000 JBPhD-2.2.1/Task/greendot.png
+-rw-rw-rw-   0        0        0    38788 2023-04-07 13:54:00.000000 JBPhD-2.2.1/Task/greentick.png
+-rw-rw-rw-   0        0        0       54 2023-05-07 14:31:32.000000 JBPhD-2.2.1/Task/help.txt
+-rw-rw-rw-   0        0        0        5 2023-05-18 15:38:22.000000 JBPhD-2.2.1/Task/participant number.txt
+-rw-rw-rw-   0        0        0      491 2023-05-14 16:12:16.000000 JBPhD-2.2.1/Task/pins.csv
+-rw-rw-rw-   0        0        0    24503 2023-04-07 13:54:00.000000 JBPhD-2.2.1/Task/redcross.png
+-rw-rw-rw-   0        0        0    98588 2023-04-07 13:54:00.000000 JBPhD-2.2.1/Task/reddot.png
+-rw-rw-rw-   0        0        0      566 2023-05-07 14:26:16.000000 JBPhD-2.2.1/Task/setup.py
+-rw-rw-rw-   0        0        0      472 2023-05-05 14:17:12.000000 JBPhD-2.2.1/Task/spwf.py
+-rw-rw-rw-   0        0        0       44 2023-04-24 16:27:34.000000 JBPhD-2.2.1/Task/spwfoutput.txt
+-rw-rw-rw-   0        0        0      100 2023-04-24 16:27:34.000000 JBPhD-2.2.1/Task/spwfvalue.txt
+-rw-rw-rw-   0        0        0       14 2023-05-15 13:41:08.000000 JBPhD-2.2.1/Task/suffix.txt
+-rw-rw-rw-   0        0        0   161693 2023-04-07 13:54:00.000000 JBPhD-2.2.1/Task/trial.jpeg
+-rw-rw-rw-   0        0        0   432254 2023-05-04 10:35:10.000000 JBPhD-2.2.1/Task/uop.ico
+-rw-rw-rw-   0        0        0     3908 2023-05-04 10:32:40.000000 JBPhD-2.2.1/Task/uop.jpeg
+-rw-rw-rw-   0        0        0     7038 2023-04-16 20:40:14.000000 JBPhD-2.2.1/Task/uop.png
+-rw-rw-rw-   0        0        0       42 2023-05-24 10:33:08.000000 JBPhD-2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      890 2023-05-24 10:30:38.000000 JBPhD-2.2.1/setup.py
```

### Comparing `JBPhD-2.1.9/JBPhD.egg-info/SOURCES.txt` & `JBPhD-2.2.1/JBPhD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Analysis.py` & `JBPhD-2.2.1/Task/Analysis.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Api.json` & `JBPhD-2.2.1/Task/Api.json`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Api2.json` & `JBPhD-2.2.1/Task/Api2.json`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Back_Right.PNG` & `JBPhD-2.2.1/Task/Back_Right.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Consent Form.docx` & `JBPhD-2.2.1/Task/Consent Form.docx`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Dependencies.py` & `JBPhD-2.2.1/Task/Dependencies.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Dependency Installation.py` & `JBPhD-2.2.1/Task/Dependency Installation.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Email Output.py` & `JBPhD-2.2.1/Task/Email Output.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Export.py` & `JBPhD-2.2.1/Task/Export.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Front_Left.PNG` & `JBPhD-2.2.1/Task/Front_Left.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Front_Right.PNG` & `JBPhD-2.2.1/Task/Front_Right.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Gradient Background.py` & `JBPhD-2.2.1/Task/Gradient Background.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Graph.py` & `JBPhD-2.2.1/Task/Graph.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/ImageSample.PNG` & `JBPhD-2.2.1/Task/ImageSample.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Inverse_Back_Left.PNG` & `JBPhD-2.2.1/Task/Inverse_Back_Left.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Manikin Back Down Left.png` & `JBPhD-2.2.1/Task/Manikin Back Down Left.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Manikin Back Up Right.png` & `JBPhD-2.2.1/Task/Manikin Back Up Right.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Manikin front Down Right.png` & `JBPhD-2.2.1/Task/Manikin front Down Right.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Manikin front Up Right.png` & `JBPhD-2.2.1/Task/Manikin front Up Right.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/N-Back Revision.py` & `JBPhD-2.2.1/Task/N-Back Revision.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/N-Back.py` & `JBPhD-2.2.1/Task/N-Back.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Participant 90210/90210 - Combined Reaction Times.csv` & `JBPhD-2.2.1/Task/Participant 90210/90210 - Combined Reaction Times.csv`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Participant 90210/90210 - Combined Scores.csv` & `JBPhD-2.2.1/Task/Participant 90210/90210 - Combined Scores.csv`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Participant 90210/90210 - N-Back Reaction Times.csv` & `JBPhD-2.2.1/Task/Participant 90210/90210 - N-Back Reaction Times.csv`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Participant 90210/90210 - N-Back Score.csv` & `JBPhD-2.2.1/Task/Participant 90210/90210 - N-Back Score.csv`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Python Install.bat` & `JBPhD-2.2.1/Task/Python Install.bat`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Reaction Time Task - Copy.py` & `JBPhD-2.2.1/Task/Reaction Time Task - Copy.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Switching.py` & `JBPhD-2.2.1/Task/Switching.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Task.py` & `JBPhD-2.2.1/Task/Task.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/Trial.py` & `JBPhD-2.2.1/Task/Trial.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/__pycache__/Dependencies.cpython-311.pyc` & `JBPhD-2.2.1/Task/__pycache__/Dependencies.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/__pycache__/Export.cpython-311.pyc` & `JBPhD-2.2.1/Task/__pycache__/Export.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/__pycache__/Location.cpython-311.pyc` & `JBPhD-2.2.1/Task/__pycache__/Location.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/__pycache__/Task.cpython-311.pyc` & `JBPhD-2.2.1/Task/__pycache__/Task.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/__pycache__/spwf.cpython-311.pyc` & `JBPhD-2.2.1/Task/__pycache__/spwf.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/asterisk.png` & `JBPhD-2.2.1/Task/asterisk.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/circle.jpg` & `JBPhD-2.2.1/Task/circle.jpg`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/greendot.png` & `JBPhD-2.2.1/Task/greendot.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/greentick.png` & `JBPhD-2.2.1/Task/greentick.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/redcross.png` & `JBPhD-2.2.1/Task/redcross.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/reddot.png` & `JBPhD-2.2.1/Task/reddot.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/setup.py` & `JBPhD-2.2.1/Task/setup.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/trial.jpeg` & `JBPhD-2.2.1/Task/trial.jpeg`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/uop.ico` & `JBPhD-2.2.1/Task/uop.ico`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/uop.jpeg` & `JBPhD-2.2.1/Task/uop.jpeg`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/Task/uop.png` & `JBPhD-2.2.1/Task/uop.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.9/setup.py` & `JBPhD-2.2.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 packagereqs = ['sendgrid', 'psutil', 'plyer', 'cryptography', 'pygame', 'pandas', 'google-auth', 'google-auth-oauthlib', 'google-auth-httplib2', 'google-api-python-client', 'Pillow', 'Scipy', 'Numpy']
 
 with open('README.txt', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='JBPhD',
-    version='2.1.9',
+    version='2.2.1',
     packages=find_namespace_packages(include=['Task']),
     install_requires=packagereqs,
     entry_points={
         'console_scripts': [
             'myproject = myproject.main:main'
         ]
     },
+    description=long_description,
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     include_package_data=True,
     data_files=[('.', ['README.txt', 'MANIFEST.in'])],
```

