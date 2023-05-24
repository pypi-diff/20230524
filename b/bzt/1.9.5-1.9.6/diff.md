# Comparing `tmp/bzt-1.9.5.tar.gz` & `tmp/bzt-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bzt-1.9.5.tar", last modified: Fri Aug 11 10:11:59 2017, max compression
+gzip compressed data, was "dist/bzt-1.9.6.tar", last modified: Wed Sep 27 10:37:08 2017, max compression
```

## Comparing `bzt-1.9.5.tar` & `bzt-1.9.6.tar`

### file list

```diff
@@ -1,90 +1,97 @@
-drwxrwxr-x   0 undera    (1000) undera    (1000)        0 2017-08-11 10:11:59.000000 bzt-1.9.5/
-drwxrwxr-x   0 undera    (1000) undera    (1000)        0 2017-08-11 10:11:59.000000 bzt-1.9.5/bzt.egg-info/
--rw-rw-r--   0 undera    (1000) undera    (1000)        1 2017-08-11 10:11:59.000000 bzt-1.9.5/bzt.egg-info/dependency_links.txt
--rw-rw-r--   0 undera    (1000) undera    (1000)      102 2017-08-11 10:11:59.000000 bzt-1.9.5/bzt.egg-info/entry_points.txt
--rw-rw-r--   0 undera    (1000) undera    (1000)      320 2017-08-11 10:11:59.000000 bzt-1.9.5/bzt.egg-info/PKG-INFO
--rw-rw-r--   0 undera    (1000) undera    (1000)      171 2017-08-11 10:11:59.000000 bzt-1.9.5/bzt.egg-info/requires.txt
--rw-rw-r--   0 undera    (1000) undera    (1000)        4 2017-08-11 10:11:59.000000 bzt-1.9.5/bzt.egg-info/top_level.txt
--rw-rw-r--   0 undera    (1000) undera    (1000)     2067 2017-08-11 10:11:59.000000 bzt-1.9.5/bzt.egg-info/SOURCES.txt
--rw-rw-r--   0 undera    (1000) undera    (1000)       65 2017-08-03 14:08:13.000000 bzt-1.9.5/MANIFEST.in
--rw-rw-r--   0 undera    (1000) undera    (1000)     2517 2017-08-02 10:13:24.000000 bzt-1.9.5/setup.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    11358 2016-04-17 13:41:52.000000 bzt-1.9.5/LICENSE
--rw-rw-r--   0 undera    (1000) undera    (1000)      320 2017-08-11 10:11:59.000000 bzt-1.9.5/PKG-INFO
--rw-rw-r--   0 undera    (1000) undera    (1000)      572 2016-04-17 13:41:52.000000 bzt-1.9.5/NOTICE
-drwxrwxr-x   0 undera    (1000) undera    (1000)        0 2017-08-11 10:11:59.000000 bzt-1.9.5/bzt/
-drwxrwxr-x   0 undera    (1000) undera    (1000)        0 2017-08-11 10:11:59.000000 bzt-1.9.5/bzt/modules/
--rw-rw-r--   0 undera    (1000) undera    (1000)     7095 2017-07-05 05:18:34.000000 bzt-1.9.5/bzt/modules/javascript.py
--rw-rw-r--   0 undera    (1000) undera    (1000)     7345 2017-07-16 12:51:47.000000 bzt-1.9.5/bzt/modules/functional.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    26362 2017-08-10 19:18:25.000000 bzt-1.9.5/bzt/modules/aggregator.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    21037 2017-08-10 15:03:00.000000 bzt-1.9.5/bzt/modules/reporting.py
--rw-rw-r--   0 undera    (1000) undera    (1000)     9441 2017-07-12 10:52:09.000000 bzt-1.9.5/bzt/modules/proxy2jmx.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    72755 2017-08-02 10:00:40.000000 bzt-1.9.5/bzt/modules/blazemeter.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    17762 2017-04-18 20:08:04.000000 bzt-1.9.5/bzt/modules/monitoring.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    18648 2017-03-06 13:26:54.000000 bzt-1.9.5/bzt/modules/chrome.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    24669 2017-08-10 19:35:56.000000 bzt-1.9.5/bzt/modules/grinder.py
--rw-rw-r--   0 undera    (1000) undera    (1000)     8560 2017-08-10 07:40:02.000000 bzt-1.9.5/bzt/modules/ab.py
--rw-rw-r--   0 undera    (1000) undera    (1000)     4237 2017-07-05 05:18:34.000000 bzt-1.9.5/bzt/modules/ruby.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    16092 2017-08-10 07:40:02.000000 bzt-1.9.5/bzt/modules/selenium.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    62651 2017-08-10 07:40:02.000000 bzt-1.9.5/bzt/modules/jmeter.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    29836 2017-08-10 07:40:02.000000 bzt-1.9.5/bzt/modules/pbench.py
--rw-rw-r--   0 undera    (1000) undera    (1000)     5071 2017-08-10 07:40:02.000000 bzt-1.9.5/bzt/modules/__init__.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    12770 2017-07-19 13:25:34.000000 bzt-1.9.5/bzt/modules/services.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    37464 2017-06-02 21:01:58.000000 bzt-1.9.5/bzt/modules/console.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    48197 2017-07-16 12:51:47.000000 bzt-1.9.5/bzt/modules/python.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    19450 2017-07-25 07:07:52.000000 bzt-1.9.5/bzt/modules/java.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    28089 2017-08-10 07:40:02.000000 bzt-1.9.5/bzt/modules/gatling.py
--rw-rw-r--   0 undera    (1000) undera    (1000)     9734 2017-08-10 07:40:02.000000 bzt-1.9.5/bzt/modules/siege.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    19415 2017-02-22 17:26:27.000000 bzt-1.9.5/bzt/modules/soapui.py
--rw-rw-r--   0 undera    (1000) undera    (1000)     3211 2017-08-10 07:40:02.000000 bzt-1.9.5/bzt/modules/csharp.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    17766 2017-08-10 07:40:02.000000 bzt-1.9.5/bzt/modules/locustio.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    19118 2017-08-10 07:40:02.000000 bzt-1.9.5/bzt/modules/tsung.py
--rw-rw-r--   0 undera    (1000) undera    (1000)     6452 2017-08-07 08:49:45.000000 bzt-1.9.5/bzt/modules/provisioning.py
--rw-rw-r--   0 undera    (1000) undera    (1000)     5404 2016-07-07 07:57:56.000000 bzt-1.9.5/bzt/modules/screen.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    16632 2017-08-05 06:34:38.000000 bzt-1.9.5/bzt/modules/passfail.py
--rw-rw-r--   0 undera    (1000) undera    (1000)     6923 2016-10-04 14:14:52.000000 bzt-1.9.5/bzt/modules/shellexec.py
-drwxrwxr-x   0 undera    (1000) undera    (1000)        0 2017-08-11 10:11:59.000000 bzt-1.9.5/bzt/six/
--rw-rw-r--   0 undera    (1000) undera    (1000)     2234 2017-04-18 20:08:04.000000 bzt-1.9.5/bzt/six/py2.py
--rw-rw-r--   0 undera    (1000) undera    (1000)      966 2016-04-17 13:41:52.000000 bzt-1.9.5/bzt/six/__init__.py
--rw-rw-r--   0 undera    (1000) undera    (1000)     2096 2017-04-18 20:08:04.000000 bzt-1.9.5/bzt/six/py3.py
-drwxrwxr-x   0 undera    (1000) undera    (1000)        0 2017-08-11 10:11:59.000000 bzt-1.9.5/bzt/resources/
--rw-rw-r--   0 undera    (1000) undera    (1000)     5960 2017-06-02 21:01:58.000000 bzt-1.9.5/bzt/resources/grinder-logger-1.0.jar
--rw-rw-r--   0 undera    (1000) undera    (1000)     3978 2017-07-05 05:18:34.000000 bzt-1.9.5/bzt/resources/rspec_taurus_plugin.rb
--rw-rw-r--   0 undera    (1000) undera    (1000)     7132 2017-08-10 15:03:00.000000 bzt-1.9.5/bzt/resources/nose_plugin.py
--rw-rw-r--   0 undera    (1000) undera    (1000)     6561 2017-07-19 07:08:51.000000 bzt-1.9.5/bzt/resources/mocha-taurus-plugin.js
--rw-rw-r--   0 undera    (1000) undera    (1000)      140 2016-08-12 08:10:12.000000 bzt-1.9.5/bzt/resources/__init__.pyc
--rw-rw-r--   0 undera    (1000) undera    (1000)     2487 2017-06-02 21:01:58.000000 bzt-1.9.5/bzt/resources/base-bzt-rc.yml
--rw-rw-r--   0 undera    (1000) undera    (1000)    11692 2016-09-04 11:23:08.000000 bzt-1.9.5/bzt/resources/taurus-junit-1.0.jar
--rw-rw-r--   0 undera    (1000) undera    (1000)        0 2016-04-17 13:41:52.000000 bzt-1.9.5/bzt/resources/__init__.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    11460 2017-06-19 23:24:05.000000 bzt-1.9.5/bzt/resources/taurus-testng-1.0.jar
--rwxrwxr-x   0 undera    (1000) undera    (1000)      134 2017-08-03 12:35:33.000000 bzt-1.9.5/bzt/resources/chrome_launcher.sh
--rwxrwxr-x   0 undera    (1000) undera    (1000)     3687 2017-07-10 12:33:22.000000 bzt-1.9.5/bzt/resources/locustio-taurus-wrapper.py
--rw-rw-r--   0 undera    (1000) undera    (1000)     4147 2017-08-03 14:08:13.000000 bzt-1.9.5/bzt/resources/base-config.yml
-drwxrwxr-x   0 undera    (1000) undera    (1000)        0 2017-08-11 10:11:59.000000 bzt-1.9.5/bzt/resources/NUnitRunner/
--rwxrw-r--   0 undera    (1000) undera    (1000)   333312 2017-08-11 10:11:58.000000 bzt-1.9.5/bzt/resources/NUnitRunner/nunit.framework.dll
--rw-rw-r--   0 undera    (1000) undera    (1000)    70656 2017-08-11 10:11:58.000000 bzt-1.9.5/bzt/resources/NUnitRunner/nunit-agent-x86.exe
--rw-rw-r--   0 undera    (1000) undera    (1000)   116224 2017-08-11 10:11:58.000000 bzt-1.9.5/bzt/resources/NUnitRunner/nunit.engine.dll
--rw-rw-r--   0 undera    (1000) undera    (1000)    18944 2017-08-11 10:11:58.000000 bzt-1.9.5/bzt/resources/NUnitRunner/nunit.engine.api.dll
--rw-rw-r--   0 undera    (1000) undera    (1000)    35328 2017-08-11 10:11:58.000000 bzt-1.9.5/bzt/resources/NUnitRunner/Mono.Options.dll
--rw-rw-r--   0 undera    (1000) undera    (1000)        0 2017-08-03 14:08:13.000000 bzt-1.9.5/bzt/resources/NUnitRunner/.gitkeep
--rw-rw-r--   0 undera    (1000) undera    (1000)   280576 2017-08-11 10:11:58.000000 bzt-1.9.5/bzt/resources/NUnitRunner/Mono.Cecil.dll
--rwxrwxr-x   0 undera    (1000) undera    (1000)    10240 2017-08-11 10:11:58.000000 bzt-1.9.5/bzt/resources/NUnitRunner/NUnitRunner.exe
--rw-rw-r--   0 undera    (1000) undera    (1000)    70656 2017-08-11 10:11:58.000000 bzt-1.9.5/bzt/resources/NUnitRunner/nunit-agent.exe
--rwxrw-r--   0 undera    (1000) undera    (1000)   653824 2017-08-11 10:11:58.000000 bzt-1.9.5/bzt/resources/NUnitRunner/Newtonsoft.Json.dll
--rw-rw-r--   0 undera    (1000) undera    (1000)      569 2017-04-18 20:08:04.000000 bzt-1.9.5/bzt/resources/logback-worker.xml
--rw-rw-r--   0 undera    (1000) undera    (1000)     1247 2017-06-02 21:01:58.000000 bzt-1.9.5/bzt/resources/gatling_script.tpl
--rw-rw-r--   0 undera    (1000) undera    (1000)     5127 2017-06-02 21:01:58.000000 bzt-1.9.5/bzt/resources/chrome-loader.c
--rw-rw-r--   0 undera    (1000) undera    (1000)     1913 2016-04-17 13:41:52.000000 bzt-1.9.5/bzt/resources/pbench.conf
--rw-rw-r--   0 undera    (1000) undera    (1000)     2419 2017-08-11 10:05:23.000000 bzt-1.9.5/bzt/__init__.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    12720 2017-06-02 21:01:58.000000 bzt-1.9.5/bzt/requests_model.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    25150 2017-08-02 10:13:24.000000 bzt-1.9.5/bzt/bza.py
--rw-rw-r--   0 undera    (1000) undera    (1000)       63 2017-08-10 07:40:02.000000 bzt-1.9.5/bzt/__main__.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    38348 2017-08-10 07:40:02.000000 bzt-1.9.5/bzt/utils.py
-drwxrwxr-x   0 undera    (1000) undera    (1000)        0 2017-08-11 10:11:59.000000 bzt-1.9.5/bzt/jmx/
--rw-rw-r--   0 undera    (1000) undera    (1000)      715 2017-08-01 15:42:52.000000 bzt-1.9.5/bzt/jmx/__init__.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    42954 2017-08-10 07:40:02.000000 bzt-1.9.5/bzt/jmx/base.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    29827 2017-08-10 07:40:02.000000 bzt-1.9.5/bzt/jmx/tools.py
--rw-rw-r--   0 undera    (1000) undera    (1000)    40974 2017-08-10 07:40:02.000000 bzt-1.9.5/bzt/engine.py
--rwxrwxr-x   0 undera    (1000) undera    (1000)    19553 2017-08-10 07:37:27.000000 bzt-1.9.5/bzt/cli.py
--rw-rw-r--   0 undera    (1000) undera    (1000)     4158 2017-06-02 21:01:58.000000 bzt-1.9.5/bzt/soapui2yaml.py
--rwxrwxr-x   0 undera    (1000) undera    (1000)    65855 2017-06-02 21:01:58.000000 bzt-1.9.5/bzt/jmx2yaml.py
--rw-rw-r--   0 undera    (1000) undera    (1000)       38 2017-08-11 10:11:59.000000 bzt-1.9.5/setup.cfg
+drwxrwxr-x   0 undera    (1000) undera    (1000)        0 2017-09-27 10:37:08.000000 bzt-1.9.6/
+-rw-rw-r--   0 undera    (1000) undera    (1000)    11358 2016-04-17 13:41:52.000000 bzt-1.9.6/LICENSE
+-rw-rw-r--   0 undera    (1000) undera    (1000)      572 2016-04-17 13:41:52.000000 bzt-1.9.6/NOTICE
+drwxrwxr-x   0 undera    (1000) undera    (1000)        0 2017-09-27 10:37:08.000000 bzt-1.9.6/bzt.egg-info/
+-rw-rw-r--   0 undera    (1000) undera    (1000)     2227 2017-09-27 10:37:08.000000 bzt-1.9.6/bzt.egg-info/SOURCES.txt
+-rw-rw-r--   0 undera    (1000) undera    (1000)      102 2017-09-27 10:37:08.000000 bzt-1.9.6/bzt.egg-info/entry_points.txt
+-rw-rw-r--   0 undera    (1000) undera    (1000)        1 2017-09-27 10:37:08.000000 bzt-1.9.6/bzt.egg-info/dependency_links.txt
+-rw-rw-r--   0 undera    (1000) undera    (1000)      178 2017-09-27 10:37:08.000000 bzt-1.9.6/bzt.egg-info/requires.txt
+-rw-rw-r--   0 undera    (1000) undera    (1000)      354 2017-09-27 10:37:08.000000 bzt-1.9.6/bzt.egg-info/PKG-INFO
+-rw-rw-r--   0 undera    (1000) undera    (1000)        4 2017-09-27 10:37:08.000000 bzt-1.9.6/bzt.egg-info/top_level.txt
+-rw-rw-r--   0 undera    (1000) undera    (1000)     2551 2017-09-27 09:34:12.000000 bzt-1.9.6/setup.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)     1613 2017-03-10 15:20:23.000000 bzt-1.9.6/README.md
+-rw-rw-r--   0 undera    (1000) undera    (1000)      354 2017-09-27 10:37:08.000000 bzt-1.9.6/PKG-INFO
+-rw-rw-r--   0 undera    (1000) undera    (1000)       90 2017-09-10 08:49:13.000000 bzt-1.9.6/MANIFEST.in
+-rw-rw-r--   0 undera    (1000) undera    (1000)       38 2017-09-27 10:37:08.000000 bzt-1.9.6/setup.cfg
+drwxrwxr-x   0 undera    (1000) undera    (1000)        0 2017-09-27 10:37:08.000000 bzt-1.9.6/bzt/
+-rw-rw-r--   0 undera    (1000) undera    (1000)     2419 2017-09-27 09:34:33.000000 bzt-1.9.6/bzt/__init__.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)       63 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/__main__.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    12720 2017-05-29 15:07:32.000000 bzt-1.9.6/bzt/requests_model.py
+-rwxrwxr-x   0 undera    (1000) undera    (1000)    19553 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/cli.py
+drwxrwxr-x   0 undera    (1000) undera    (1000)        0 2017-09-27 10:37:08.000000 bzt-1.9.6/bzt/modules/
+-rw-rw-r--   0 undera    (1000) undera    (1000)     5071 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/modules/__init__.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)     3211 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/modules/csharp.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)     6452 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/modules/provisioning.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    76396 2017-09-26 14:23:54.000000 bzt-1.9.6/bzt/modules/blazemeter.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    28515 2017-09-11 10:51:02.000000 bzt-1.9.6/bzt/modules/gatling.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    68863 2017-09-25 08:26:22.000000 bzt-1.9.6/bzt/modules/jmeter.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)     8151 2017-09-27 10:26:13.000000 bzt-1.9.6/bzt/modules/molotov.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    29836 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/modules/pbench.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    19415 2017-03-10 15:20:23.000000 bzt-1.9.6/bzt/modules/soapui.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)     5374 2017-09-25 07:01:58.000000 bzt-1.9.6/bzt/modules/screen.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    24901 2017-09-21 08:07:54.000000 bzt-1.9.6/bzt/modules/grinder.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    50996 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/modules/python.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    16633 2017-09-17 14:58:47.000000 bzt-1.9.6/bzt/modules/passfail.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)     7095 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/modules/javascript.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    21499 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/modules/reporting.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)     4237 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/modules/ruby.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)     9441 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/modules/proxy2jmx.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    37464 2017-05-12 09:18:00.000000 bzt-1.9.6/bzt/modules/console.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    17766 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/modules/locustio.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    12785 2017-09-11 10:51:02.000000 bzt-1.9.6/bzt/modules/services.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)     7345 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/modules/functional.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    16102 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/modules/selenium.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)     8560 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/modules/ab.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    26362 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/modules/aggregator.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)     6923 2017-04-15 14:25:25.000000 bzt-1.9.6/bzt/modules/shellexec.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    18648 2017-04-15 14:25:25.000000 bzt-1.9.6/bzt/modules/chrome.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    19118 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/modules/tsung.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)     9734 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/modules/siege.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    19450 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/modules/java.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    18209 2017-09-13 09:36:13.000000 bzt-1.9.6/bzt/modules/monitoring.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    25787 2017-09-26 09:52:08.000000 bzt-1.9.6/bzt/bza.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)     4158 2017-05-10 15:38:53.000000 bzt-1.9.6/bzt/soapui2yaml.py
+-rwxrwxr-x   0 undera    (1000) undera    (1000)    65855 2017-05-22 10:55:12.000000 bzt-1.9.6/bzt/jmx2yaml.py
+drwxrwxr-x   0 undera    (1000) undera    (1000)        0 2017-09-27 10:37:08.000000 bzt-1.9.6/bzt/six/
+-rw-rw-r--   0 undera    (1000) undera    (1000)      966 2016-04-17 13:41:52.000000 bzt-1.9.6/bzt/six/__init__.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)     2290 2017-09-11 10:51:02.000000 bzt-1.9.6/bzt/six/py3.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)     2289 2017-09-11 10:51:02.000000 bzt-1.9.6/bzt/six/py2.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    38351 2017-09-11 10:51:02.000000 bzt-1.9.6/bzt/utils.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    40939 2017-09-11 10:51:02.000000 bzt-1.9.6/bzt/engine.py
+drwxrwxr-x   0 undera    (1000) undera    (1000)        0 2017-09-27 10:37:08.000000 bzt-1.9.6/bzt/jmx/
+-rw-rw-r--   0 undera    (1000) undera    (1000)      715 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/jmx/__init__.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    43917 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/jmx/base.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)    30155 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/jmx/tools.py
+drwxrwxr-x   0 undera    (1000) undera    (1000)        0 2017-09-27 10:37:08.000000 bzt-1.9.6/bzt/resources/
+-rw-rw-r--   0 undera    (1000) undera    (1000)     1913 2016-04-17 13:41:52.000000 bzt-1.9.6/bzt/resources/pbench.conf
+-rw-rw-r--   0 undera    (1000) undera    (1000)     2487 2017-05-29 16:37:26.000000 bzt-1.9.6/bzt/resources/base-bzt-rc.yml
+-rw-rw-r--   0 undera    (1000) undera    (1000)        0 2016-04-17 13:41:52.000000 bzt-1.9.6/bzt/resources/__init__.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)     1247 2017-06-02 14:26:38.000000 bzt-1.9.6/bzt/resources/gatling_script.tpl
+-rw-rw-r--   0 undera    (1000) undera    (1000)      569 2017-04-15 10:17:22.000000 bzt-1.9.6/bzt/resources/logback-worker.xml
+-rw-rw-r--   0 undera    (1000) undera    (1000)      140 2017-02-06 09:53:06.000000 bzt-1.9.6/bzt/resources/__init__.pyc
+drwxrwxr-x   0 undera    (1000) undera    (1000)        0 2017-09-27 10:37:08.000000 bzt-1.9.6/bzt/resources/__pycache__/
+-rw-rw-r--   0 undera    (1000) undera    (1000)      136 2017-03-31 08:11:13.000000 bzt-1.9.6/bzt/resources/__pycache__/__init__.cpython-35.pyc
+-rw-rw-r--   0 undera    (1000) undera    (1000)     5525 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/resources/pytest_runner.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)     7433 2017-09-27 10:32:06.000000 bzt-1.9.6/bzt/resources/grinder-logger-1.0.jar
+-rw-rw-r--   0 undera    (1000) undera    (1000)     4260 2017-09-26 14:08:21.000000 bzt-1.9.6/bzt/resources/base-config.yml
+-rwxrwxr-x   0 undera    (1000) undera    (1000)      134 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/resources/chrome_launcher.sh
+-rwxrwxr-x   0 undera    (1000) undera    (1000)     3687 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/resources/locustio-taurus-wrapper.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)     3978 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/resources/rspec_taurus_plugin.rb
+-rw-rw-r--   0 undera    (1000) undera    (1000)     5127 2017-05-29 15:07:32.000000 bzt-1.9.6/bzt/resources/chrome-loader.c
+-rw-rw-r--   0 undera    (1000) undera    (1000)    11462 2017-09-27 10:34:25.000000 bzt-1.9.6/bzt/resources/taurus-testng-1.0.jar
+-rw-rw-r--   0 undera    (1000) undera    (1000)     6561 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/resources/mocha-taurus-plugin.js
+-rw-rw-r--   0 undera    (1000) undera    (1000)     3519 2017-09-26 14:08:21.000000 bzt-1.9.6/bzt/resources/molotov_ext.py
+drwxrwxr-x   0 undera    (1000) undera    (1000)        0 2017-09-27 10:37:08.000000 bzt-1.9.6/bzt/resources/NUnitRunner/
+-rw-r--r--   0 undera    (1000) undera    (1000)    35328 2017-09-27 10:34:26.000000 bzt-1.9.6/bzt/resources/NUnitRunner/Mono.Options.dll
+-rw-r--r--   0 undera    (1000) undera    (1000)    70656 2017-09-27 10:34:26.000000 bzt-1.9.6/bzt/resources/NUnitRunner/nunit-agent-x86.exe
+-rw-r--r--   0 undera    (1000) undera    (1000)    11264 2017-09-27 10:34:26.000000 bzt-1.9.6/bzt/resources/NUnitRunner/NUnitRunner.exe
+-rw-r--r--   0 undera    (1000) undera    (1000)    70656 2017-09-27 10:34:26.000000 bzt-1.9.6/bzt/resources/NUnitRunner/nunit-agent.exe
+-rw-r--r--   0 undera    (1000) undera    (1000)   116224 2017-09-27 10:34:26.000000 bzt-1.9.6/bzt/resources/NUnitRunner/nunit.engine.dll
+-rw-r--r--   0 undera    (1000) undera    (1000)    18944 2017-09-27 10:34:26.000000 bzt-1.9.6/bzt/resources/NUnitRunner/nunit.engine.api.dll
+-rw-rw-r--   0 undera    (1000) undera    (1000)        0 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/resources/NUnitRunner/.gitkeep
+-rw-r--r--   0 undera    (1000) undera    (1000)   280576 2017-09-27 10:34:26.000000 bzt-1.9.6/bzt/resources/NUnitRunner/Mono.Cecil.dll
+-rwxr--r--   0 undera    (1000) undera    (1000)   653824 2017-09-27 10:34:26.000000 bzt-1.9.6/bzt/resources/NUnitRunner/Newtonsoft.Json.dll
+-rwxr--r--   0 undera    (1000) undera    (1000)   333312 2017-09-27 10:34:26.000000 bzt-1.9.6/bzt/resources/NUnitRunner/nunit.framework.dll
+-rw-rw-r--   0 undera    (1000) undera    (1000)    11389 2017-09-27 10:32:14.000000 bzt-1.9.6/bzt/resources/taurus-junit-1.0.jar
+-rw-rw-r--   0 undera    (1000) undera    (1000)     7132 2017-09-10 08:49:13.000000 bzt-1.9.6/bzt/resources/nose_plugin.py
+-rw-rw-r--   0 undera    (1000) undera    (1000)      256 2017-09-11 10:51:02.000000 bzt-1.9.6/requirements.txt
```

### Comparing `bzt-1.9.5/bzt.egg-info/SOURCES.txt` & `bzt-1.9.6/bzt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 LICENSE
 MANIFEST.in
 NOTICE
+README.md
+requirements.txt
 setup.py
 bzt/__init__.py
 bzt/__main__.py
 bzt/bza.py
 bzt/cli.py
 bzt/engine.py
 bzt/jmx2yaml.py
@@ -30,14 +32,15 @@
 bzt/modules/functional.py
 bzt/modules/gatling.py
 bzt/modules/grinder.py
 bzt/modules/java.py
 bzt/modules/javascript.py
 bzt/modules/jmeter.py
 bzt/modules/locustio.py
+bzt/modules/molotov.py
 bzt/modules/monitoring.py
 bzt/modules/passfail.py
 bzt/modules/pbench.py
 bzt/modules/provisioning.py
 bzt/modules/proxy2jmx.py
 bzt/modules/python.py
 bzt/modules/reporting.py
@@ -56,25 +59,28 @@
 bzt/resources/chrome-loader.c
 bzt/resources/chrome_launcher.sh
 bzt/resources/gatling_script.tpl
 bzt/resources/grinder-logger-1.0.jar
 bzt/resources/locustio-taurus-wrapper.py
 bzt/resources/logback-worker.xml
 bzt/resources/mocha-taurus-plugin.js
+bzt/resources/molotov_ext.py
 bzt/resources/nose_plugin.py
 bzt/resources/pbench.conf
+bzt/resources/pytest_runner.py
 bzt/resources/rspec_taurus_plugin.rb
 bzt/resources/taurus-junit-1.0.jar
 bzt/resources/taurus-testng-1.0.jar
 bzt/resources/NUnitRunner/.gitkeep
 bzt/resources/NUnitRunner/Mono.Cecil.dll
 bzt/resources/NUnitRunner/Mono.Options.dll
 bzt/resources/NUnitRunner/NUnitRunner.exe
 bzt/resources/NUnitRunner/Newtonsoft.Json.dll
 bzt/resources/NUnitRunner/nunit-agent-x86.exe
 bzt/resources/NUnitRunner/nunit-agent.exe
 bzt/resources/NUnitRunner/nunit.engine.api.dll
 bzt/resources/NUnitRunner/nunit.engine.dll
 bzt/resources/NUnitRunner/nunit.framework.dll
+bzt/resources/__pycache__/__init__.cpython-35.pyc
 bzt/six/__init__.py
 bzt/six/py2.py
 bzt/six/py3.py
```

### Comparing `bzt-1.9.5/setup.py` & `bzt-1.9.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-import platform
+import os
 import sys
+from setuptools import setup
 from setuptools.command.install import install
 
-import os
-from setuptools import setup
+# noinspection PyPackageRequirements
+import pip
 
 import bzt
 
 
 class InstallWithHook(install, object):
     """
     Command adding post-install hook to setup
@@ -41,34 +42,34 @@
             sys.stdout.write("[%s] Found %s\n" % (bzt.VERSION, dirname))
             src = os.path.join(dirname, "10-base.json")
             if os.path.exists(src):
                 sys.stdout.write("Removing outdated %s\n" % src)
                 os.remove(src)
 
 
-requires = ['pyyaml', 'psutil > 3, != 5.1.1', 'colorlog', 'colorama',
-            'cssselect', 'urwid', 'six', 'nose',
-            'selenium', 'progressbar33', 'pyvirtualdisplay', 'requests>=2.11.1', "apiritif>=0.3",
-            'astunparse', 'lxml >= 3.8.0']
+# thanks to pip there are two incompatible ways to parse requirements.txt
+if pip.__version__ < '7':
+    requirements = pip.req.parse_requirements('requirements.txt')
+else:
+    # new versions of pip requires a session
+    requirements = pip.req.parse_requirements('requirements.txt', session=pip.download.PipSession())
 
-if sys.version_info.major < 3:
-    requires += ['ipaddress']  # backport of 'ipaddress' module to Python 2
+requires = [str(item.req) for item in requirements]
 
 setup(
     name="bzt",
     version=bzt.VERSION,
     description='Taurus Tool for Continuous Testing',
     author='Andrey Pokhilko',
     author_email='andrey@blazemeter.com',
     url='http://gettaurus.org/',
     download_url='http://gettaurus.org/docs/DeveloperGuide/#Python-Egg-Snapshots',
     license='Apache 2.0',
     platform='any',
     docs_url='http://gettaurus.org/docs/',
-
     install_requires=requires,
     packages=['bzt', 'bzt.six', 'bzt.jmx', 'bzt.modules', 'bzt.resources'],
     entry_points={
         'console_scripts': [
             'bzt=bzt.cli:main',
             'jmx2yaml=bzt.jmx2yaml:main',
             'soapui2yaml=bzt.soapui2yaml:main',
```

### Comparing `bzt-1.9.5/LICENSE` & `bzt-1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/NOTICE` & `bzt-1.9.6/NOTICE`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/modules/javascript.py` & `bzt-1.9.6/bzt/modules/javascript.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/modules/functional.py` & `bzt-1.9.6/bzt/modules/functional.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/modules/aggregator.py` & `bzt-1.9.6/bzt/modules/aggregator.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/modules/reporting.py` & `bzt-1.9.6/bzt/modules/reporting.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,16 +37,18 @@
     A reporter that prints short statistics on test end
     """
 
     def __init__(self):
         super(FinalStatus, self).__init__()
         self.last_sec = None
         self.cumulative_results = None
-        self.start_time = time.time()
+        self.start_time = None
         self.end_time = None
+        self.first_ts = float("inf")
+        self.last_ts = 0
 
     def startup(self):
         self.start_time = time.time()
 
     def prepare(self):
         super(FinalStatus, self).prepare()
         if isinstance(self.engine.aggregator, ResultsProvider):
@@ -56,33 +58,36 @@
 
     def aggregated_second(self, data):
         """
         Just store the latest info
 
         :type data: bzt.modules.aggregator.DataPoint
         """
+        self.first_ts = min(self.first_ts, data[DataPoint.TIMESTAMP])
+        self.last_ts = max(self.last_ts, data[DataPoint.TIMESTAMP])
         self.last_sec = data
 
     def aggregated_results(self, results, cumulative_results):
         """
         Just store the latest info
 
         :type cumulative_results: bzt.modules.functional.ResultsTree
         :type results: bzt.modules.functional.ResultsTree
         """
         self.cumulative_results = cumulative_results
 
+    def shutdown(self):
+        self.end_time = time.time()
+
     def post_process(self):
         """
         Log basic stats
         """
         super(FinalStatus, self).post_process()
 
-        self.end_time = time.time()
-
         if self.parameters.get("test-duration", True):
             self.__report_duration()
 
         if self.last_sec:
             summary_kpi = self.last_sec[DataPoint.CUMULATIVE][""]
 
             if self.parameters.get("summary", True):
@@ -177,14 +182,20 @@
         date_start = datetime.fromtimestamp(int(self.start_time))
         date_end = datetime.fromtimestamp(int(self.end_time))
         self.log.info("Test duration: %s", date_end - date_start)
 
     def __dump_xml(self, filename):
         self.log.info("Dumping final status as XML: %s", filename)
         root = etree.Element("FinalStatus")
+
+        if self.first_ts < float("inf") and self.last_ts > 0:
+            duration_elem = etree.Element("TestDuration")
+            duration_elem.text = str(round(float(self.last_ts - self.first_ts), 3))
+            root.append(duration_elem)
+
         report_info = get_bza_report_info(self.engine, self.log)
         if report_info:
             link, _ = report_info[0]
             report_element = etree.Element("ReportURL")
             report_element.text = link
             root.append(report_element)
         if self.last_sec:
```

### Comparing `bzt-1.9.5/bzt/modules/proxy2jmx.py` & `bzt-1.9.6/bzt/modules/proxy2jmx.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/modules/blazemeter.py` & `bzt-1.9.6/bzt/modules/blazemeter.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,21 @@
 from ssl import SSLError
 
 import yaml
 from requests.exceptions import ReadTimeout
 from urwid import Pile, Text
 
 from bzt import TaurusInternalException, TaurusConfigError, TaurusException, TaurusNetworkError, NormalShutdown
+from bzt import AutomatedShutdown
 from bzt.bza import User, Session, Test
 from bzt.engine import Reporter, Provisioning, ScenarioExecutor, Configuration, Service, Singletone
 from bzt.modules.aggregator import DataPoint, KPISet, ConsolidatingAggregator, ResultsProvider, AggregatorListener
 from bzt.modules.chrome import ChromeProfiler
 from bzt.modules.console import WidgetProvider, PrioritizedWidget
+from bzt.modules.functional import FunctionalResultsReader, FunctionalAggregator, FunctionalSample
 from bzt.modules.monitoring import Monitoring, MonitoringListener
 from bzt.modules.services import Unpacker
 from bzt.six import BytesIO, iteritems, HTTPError, r_input, URLError, b
 from bzt.utils import open_browser, get_full_path, get_files_recursive, replace_in_config, humanize_bytes, \
     ExceptionalDownloader, ProgressBarContext
 from bzt.utils import to_json, dehumanize_time, BetterDict, ensure_is_dict
 
@@ -379,15 +381,17 @@
                 time.sleep(self.send_interval)
                 tries -= 1
 
             self._postproc_phase3()
 
     def _postproc_phase3(self):
         try:
-            self.end_online()
+            if self.send_data:
+                self.end_online()
+
             if self._user.token and self.engine.stopping_reason:
                 exc_class = self.engine.stopping_reason.__class__.__name__
                 note = "%s: %s" % (exc_class, str(self.engine.stopping_reason))
                 self.append_note_to_session(note)
                 if self._master:
                     self.append_note_to_master(note)
 
@@ -866,14 +870,15 @@
         super(ProjectFinder, self).__init__()
         self.default_test_name = "Taurus Test"
         self.parameters = parameters
         self.settings = settings
         self.log = parent_log.getChild(self.__class__.__name__)
         self.user = user
         self.workspaces = workspaces
+        self.is_functional = False
 
     def _find_project(self, proj_name):
         """
         :rtype: bzt.bza.Project
         """
         if isinstance(proj_name, (int, float)):  # TODO: what if it's string "123"?
             proj_id = int(proj_name)
@@ -945,14 +950,15 @@
                 test_class = CloudCollectionTest
 
         assert test_class is not None
         router = test_class(self.user, test, project, test_name, default_location, self.log)
         router._workspaces = self.workspaces
         router.cloud_mode = self.settings.get("cloud-mode", None)
         router.dedicated_ips = self.settings.get("dedicated-ips", False)
+        router.is_functional = self.is_functional
         return router
 
     def _default_or_create_project(self, proj_name):
         if proj_name:
             return self.workspaces.first().create_project(proj_name)
         else:
             info = self.user.fetch()
@@ -982,14 +988,15 @@
         self._user = user
         self._project = project
         self._test = test
         self.master = None
         self._workspaces = None
         self.cloud_mode = None
         self.dedicated_ips = False
+        self.is_functional = False
 
     @abstractmethod
     def prepare_locations(self, executors, engine_config):
         pass
 
     def prepare_cloud_config(self, engine_config):
         config = copy.deepcopy(engine_config)
@@ -1128,18 +1135,21 @@
 
         if delete_old_files:
             self._test.delete_files()
 
         taurus_config = yaml.dump(taurus_config, default_flow_style=False, explicit_start=True, canonical=False)
         self._test.upload_files(taurus_config, rfiles)
         self._test.update_props({'configuration': {'executionType': self.cloud_mode}})
+        self._test.update_props({
+            'configuration': {'plugins': {'functionalExecution': {'enabled': self.is_functional}}}
+        })
 
     def launch_test(self):
         self.log.info("Initiating cloud test with %s ...", self._test.address)
-        self.master = self._test.start()
+        self.master = self._test.start(as_functional=self.is_functional)
         return self.master.address + '/app/#/masters/%s' % self.master['id']
 
     def start_if_ready(self):
         self._started = True
 
     def stop_test(self):
         if self.master:
@@ -1430,14 +1440,15 @@
         self.detach = self.settings.get("detach", self.detach)
         self.check_interval = dehumanize_time(self.settings.get("check-interval", self.check_interval))
         self.public_report = self.settings.get("public-report", self.public_report)
         self._filter_reporting()
 
         finder = ProjectFinder(self.parameters, self.settings, self.user, self._workspaces, self.log)
         finder.default_test_name = "Taurus Cloud Test"
+        finder.is_functional = self.engine.is_functional_mode()
         self.router = finder.resolve_test_type()
         self.router.prepare_locations(self.executors, self.engine.config)
 
         res_files = self.get_rfiles()
         files_for_cloud = self._fix_filenames(res_files)
         config_for_cloud = self.router.prepare_cloud_config(self.engine.config)
         config_for_cloud.dump(self.engine.create_artifact("cloud", ""))
@@ -1450,14 +1461,17 @@
 
         self.widget = self.get_widget()
 
         if isinstance(self.engine.aggregator, ConsolidatingAggregator):
             self.results_reader = ResultsFromBZA()
             self.results_reader.log = self.log
             self.engine.aggregator.add_underling(self.results_reader)
+        elif isinstance(self.engine.aggregator, FunctionalAggregator):
+            self.results_reader = FunctionalBZAReader(self.log)
+            self.engine.aggregator.add_underling(self.results_reader)
 
     def __dump_locations_if_needed(self):
         if self.settings.get("dump-locations", False):
             self.log.warning("Dumping available locations instead of running the test")
             use_deprecated = self.settings.get("use-deprecated-api", True)
             is_taurus3 = self.settings.get("cloud-mode", None) == 'taurusCloud'
             locations = {}
@@ -1578,14 +1592,20 @@
                 mod = service.get('module', TaurusConfigError("No 'module' specified for service"))
                 assert isinstance(mod, str)
                 module = self.engine.instantiate_module(mod)
                 if isinstance(module, ServiceStubCaptureHAR):
                     self._download_logs()
                     break
 
+            if "functionalSummary" in full:
+                summary = full["functionalSummary"]
+                is_failed = summary.get("isFailed", False)
+                if is_failed:
+                    raise AutomatedShutdown("Cloud tests failed")
+
     def _download_logs(self):
         for session in self.router.master.sessions():
             assert isinstance(session, Session)
             for log in session.get_logs():
                 self.log.info("Downloading %s from the cloud", log['filename'])
                 cloud_dir = os.path.join(self.engine.artifacts_dir, 'cloud-artifacts')
                 if not os.path.exists(cloud_dir):
@@ -1773,14 +1793,78 @@
             time.sleep(self.master.timeout)
             aggr = self.master.get_aggregate_report()
             self.log.info("Succeeded with retry")
 
         return data, aggr
 
 
+class FunctionalBZAReader(FunctionalResultsReader):
+    def __init__(self, parent_log, master=None):
+        super(FunctionalBZAReader, self).__init__()
+        self.master = master
+        self.log = parent_log.getChild(self.__class__.__name__)
+
+    @staticmethod
+    def extract_samples_from_group(group, group_summary):
+        group_name = group_summary.get("name") or "Tests"
+        for sample in group["samples"]:
+            status = "PASSED"
+            if sample["error"]:
+                status = "FAILED"
+            error_msg = ""
+            error_trace = ""
+            assertions = sample.get("assertions")
+            if assertions:
+                for assertion in assertions:
+                    if assertion.get("isFailed"):
+                        error_msg = assertion.get("errorMessage")
+                        status = "BROKEN"
+
+            rtm = sample.get("responseTime") or 0.0
+            yield FunctionalSample(
+                test_case=sample["label"],
+                test_suite=group_name,
+                status=status,
+                start_time=int(sample["created"]),
+                duration=rtm / 1000.0,
+                error_msg=error_msg,
+                error_trace=error_trace,
+                extras={},
+                subsamples=[],
+            )
+
+    def read(self, last_pass=False):
+        if self.master is None:
+            return
+
+        if last_pass:
+            try:
+                groups = self.master.get_functional_report_groups()
+            except (URLError, TaurusNetworkError):
+                self.log.warning("Failed to get test groups, will retry in %s seconds...", self.master.timeout)
+                self.log.debug("Full exception: %s", traceback.format_exc())
+                time.sleep(self.master.timeout)
+                groups = self.master.get_functional_report_groups()
+                self.log.info("Succeeded with retry")
+
+            for group_summary in groups:
+                group_id = group_summary['groupId']
+                try:
+                    group = self.master.get_functional_report_group(group_id)
+                except (URLError, TaurusNetworkError):
+                    self.log.warning("Failed to get test group, will retry in %s seconds...", self.master.timeout)
+                    self.log.debug("Full exception: %s", traceback.format_exc())
+                    time.sleep(self.master.timeout)
+                    group = self.master.get_functional_report_group(group_id)
+                    self.log.info("Succeeded with retry")
+
+                for sample in self.extract_samples_from_group(group, group_summary):
+                    yield sample
+
+
 class CloudProvWidget(Pile, PrioritizedWidget):
     def __init__(self, test):
         """
         :type test: BaseCloudTest
         """
         self.test = test
         self.text = Text("")
```

### Comparing `bzt-1.9.5/bzt/modules/monitoring.py` & `bzt-1.9.6/bzt/modules/monitoring.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import psutil
 from bzt import TaurusNetworkError, TaurusInternalException, TaurusConfigError
 from urwid import Pile, Text
 
 from bzt.engine import Service, Singletone
 from bzt.modules.console import WidgetProvider, PrioritizedWidget
 from bzt.modules.passfail import FailCriterion
-from bzt.six import iteritems, urlopen, urlencode
+from bzt.six import iteritems, urlopen, urlencode, b
 from bzt.utils import dehumanize_time
 
 
 class Monitoring(Service, WidgetProvider, Singletone):
     """
     :type clients: list[ServerAgentClient]
     :type listeners: list[MonitoringListener]
@@ -231,22 +231,30 @@
             mem_usage = None
             if not self.__informed_on_mem_issue:
                 self.log.debug("Failed to get memory usage: %s", traceback.format_exc())
                 self.log.warning("Failed to get memory usage, use -v to get more detailed error info")
                 self.__informed_on_mem_issue = True
 
         net = psutil.net_io_counters()
-        tx_bytes = (net.bytes_sent - self.__net_counters.bytes_sent) / interval
-        rx_bytes = (net.bytes_recv - self.__net_counters.bytes_recv) / interval
-        self.__net_counters = net
+        if net is not None:
+            tx_bytes = (net.bytes_sent - self.__net_counters.bytes_sent) / interval
+            rx_bytes = (net.bytes_recv - self.__net_counters.bytes_recv) / interval
+            self.__net_counters = net
+        else:
+            rx_bytes = 0.0
+            tx_bytes = 0.0
 
         disk = self.__get_disk_counters()
-        dru = (disk.read_bytes - self.__disk_counters.read_bytes) / interval
-        dwu = (disk.write_bytes - self.__disk_counters.write_bytes) / interval
-        self.__disk_counters = disk
+        if disk is not None:
+            dru = (disk.read_bytes - self.__disk_counters.read_bytes) / interval
+            dwu = (disk.write_bytes - self.__disk_counters.write_bytes) / interval
+            self.__disk_counters = disk
+        else:
+            dru = 0.0
+            dwu = 0.0
 
         if self.engine:
             engine_loop = self.engine.engine_loop_utilization
             disk_usage = psutil.disk_usage(self.engine.artifacts_dir).percent
         else:
             engine_loop = None
             disk_usage = None
@@ -263,21 +271,23 @@
             disk_usage=disk_usage,
             mem_usage=mem_usage,
             rx=rx_bytes, tx=tx_bytes, dru=dru, dwu=dwu,
             engine_loop=engine_loop, conn_all=len(connections)
         )
 
     def __get_disk_counters(self):
+        counters = None
         try:
-            return psutil.disk_io_counters()
+            counters = psutil.disk_io_counters()
         except RuntimeError as exc:
             self.log.debug("Failed to get disk metrics: %s", exc)
+        if counters is None:
+            counters = psutil._common.sdiskio(0, 0, 0, 0, 0, 0)  # pylint: disable=protected-access
             # noinspection PyProtectedMember
-            return psutil._common.sdiskio(0, 0, 0, 0, 0, 0)  # pylint: disable=protected-access
-
+        return counters
 
 class GraphiteClient(MonitoringClient):
     def __init__(self, parent_logger, label, config):
         super(GraphiteClient, self).__init__()
         self.log = parent_logger.getChild(self.__class__.__name__)
         self.config = config
         exc = TaurusConfigError('Graphite client requires address parameter')
@@ -380,36 +390,37 @@
         self.socket = socket.socket()
         self.select = select.select
         self.interval = int(dehumanize_time(config.get("interval", 1)))
 
     def connect(self):
         try:
             self.socket.connect((self.address, self.port))
-            self.socket.send("test\n")
+            self.socket.send(b("test\n"))
             resp = self.socket.recv(4)
-            assert resp == "Yep\n"
+            assert resp == b("Yep\n")
             self.log.debug("Connected to serverAgent at %s:%s successfully", self.address, self.port)
-        except:
+        except BaseException as exc:
+            self.log.warning("Error during connecting to agent at %s:%s: %s", self.address, self.port, exc)
             msg = "Failed to connect to serverAgent at %s:%s" % (self.address, self.port)
             raise TaurusNetworkError(msg)
 
     def disconnect(self):
         self.log.debug("Closing connection with agent at %s:%s...", self.address, self.port)
         try:
-            self.socket.send("exit\n")
+            self.socket.send(b("exit\n"))
         except BaseException as exc:
             self.log.warning("Error during disconnecting from agent at %s:%s: %s", self.address, self.port, exc)
         finally:
             self.socket.close()
 
     def start(self):
-        self.socket.send("interval:%s\n" % self.interval if self.interval > 0 else 1)
+        self.socket.send(b("interval:%s\n" % self.interval if self.interval > 0 else 1))
         command = "metrics:%s\n" % self._metrics_command
         self.log.debug("Sending metrics command: %s", command)
-        self.socket.send(command)
+        self.socket.send(b(command))
         self.socket.setblocking(False)
 
     def get_data(self):
         """
         :rtype: list[dict]
         """
         readable, writable, errored = self.select([self.socket], [self.socket], [self.socket], 0)
@@ -417,15 +428,15 @@
         for _ in errored:
             self.log.warning("Failed to get monitoring data from agent at %s:%s", self.address, self.port)
 
         source = self.host_label if self.host_label else '%s:%s' % (self.address, self.port)
 
         res = []
         for _sock in readable:
-            self._partial_buffer += _sock.recv(1024)
+            self._partial_buffer += _sock.recv(1024).decode()
             while "\n" in self._partial_buffer:
                 line = self._partial_buffer[:self._partial_buffer.index("\n")]
                 self._partial_buffer = self._partial_buffer[self._partial_buffer.index("\n") + 1:]
                 self.log.debug("Data line: %s", line)
                 values = line.split("\t")
                 item = {x: float(values.pop(0)) for x in self._result_fields}
                 item['ts'] = int(time.time())
```

### Comparing `bzt-1.9.5/bzt/modules/chrome.py` & `bzt-1.9.6/bzt/modules/chrome.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/modules/grinder.py` & `bzt-1.9.6/bzt/modules/grinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,26 +11,25 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
+import os
 import re
 import subprocess
 import time
 
-import os
 from bzt import TaurusConfigError, ToolError
-from bzt.six import iteritems
-
 from bzt.engine import ScenarioExecutor, Scenario, FileLister, HavingInstallableTools, SelfDiagnosable
 from bzt.modules.aggregator import ConsolidatingAggregator, ResultsReader
 from bzt.modules.console import WidgetProvider, ExecutorWidget
 from bzt.requests_model import HTTPRequest
+from bzt.six import iteritems
 from bzt.utils import shell_exec, MirrorsManager, dehumanize_time, get_full_path, PythonGenerator
 from bzt.utils import unzip, RequiredTool, JavaVM, shutdown_process, TclLibrary
 
 
 class GrinderExecutor(ScenarioExecutor, WidgetProvider, FileLister, HavingInstallableTools, SelfDiagnosable):
     """
     Grinder executor module
@@ -349,30 +348,35 @@
             if thread_id not in self.known_threads:
                 self.known_threads.add(thread_id)
                 self.concurrency += 1
 
             url, error_msg = self.__parse_prev_line(worker_id, lines, lnum, r_code, bytes_count)
             if int(data_fields[self.idx["Errors"]]) > 0 or int(data_fields[self.idx['HTTP response errors']]) > 0:
                 if not error_msg:
-                    error_msg = "HTTP %s" % r_code
+                    if r_code != '0':
+                        error_msg = "HTTP %s" % r_code
+                    else:
+                        error_msg = "Java exception calling TestRunner"
             else:
                 error_msg = None  # suppress errors
 
             if self.report_by_url:
                 label = url
             elif test_id in self.test_names:
                 label = self.test_names[test_id]
             else:
                 label = "Test #%s" % test_id
 
             source_id = ''  # maybe use worker_id somehow?
             yield int(t_stamp), label, self.concurrency, r_time, con_time, \
                   latency, r_code, error_msg, source_id, bytes_count
-        end = time.time()
-        self.log.debug("Log reading speed: %s lines/s", len(lines) / (end - start))
+        if cnt > 0:
+            duration = time.time() - start
+            duration = duration if duration > 0.01 else 1
+            self.log.debug("Log reading speed: %s lines/s", len(lines) / duration)
 
     def __split(self, line):
         if not line.endswith("\n"):
             self.partial_buffer += line
             return None, None
 
         line = "%s%s" % (self.partial_buffer, line)
@@ -405,15 +409,15 @@
             return None, None
 
         return data_fields, worker_id
 
     def __parse_prev_line(self, worker_id, lines, lnum, r_code, bytes_count):
         url = ''
         error_msg = None
-        for lineNo in reversed(xrange(max(lnum - 100, 0), lnum)):  # looking max 100 lines back. TODO: parameterize?
+        for lineNo in reversed(range(max(lnum - 100, 0), lnum)):  # looking max 100 lines back. TODO: parameterize?
             line = lines[lineNo].strip()
             matched = self.DETAILS_REGEX.match(line)
             if not matched:
                 continue
 
             if worker_id == matched.group(1) and r_code == matched.group(3) and str(bytes_count) == matched.group(5):
                 return matched.group(2), matched.group(4)
```

### Comparing `bzt-1.9.5/bzt/modules/ab.py` & `bzt-1.9.6/bzt/modules/ab.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/modules/ruby.py` & `bzt-1.9.6/bzt/modules/ruby.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/modules/selenium.py` & `bzt-1.9.6/bzt/modules/selenium.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 class SeleniumExecutor(AbstractSeleniumExecutor, WidgetProvider, FileLister, HavingInstallableTools, SelfDiagnosable):
     """
     Selenium executor
     :type runner: bzt.modules.SubprocessedExecutor
     :type virtual_display_service: VirtualDisplay
     """
 
-    SUPPORTED_RUNNERS = ["nose", "junit", "testng", "rspec", "mocha", "nunit"]
+    SUPPORTED_RUNNERS = ["nose", "junit", "testng", "rspec", "mocha", "nunit", "pytest"]
 
     CHROMEDRIVER_DOWNLOAD_LINK = "https://chromedriver.storage.googleapis.com/{version}/chromedriver_{arch}.zip"
     CHROMEDRIVER_VERSION = "2.29"
 
     GECKODRIVER_DOWNLOAD_LINK = "https://github.com/mozilla/geckodriver/releases/download/v{version}/" \
                                 "geckodriver-v{version}-{arch}.{ext}"
     GECKODRIVER_VERSION = "0.17.0"
```

### Comparing `bzt-1.9.5/bzt/modules/jmeter.py` & `bzt-1.9.6/bzt/modules/jmeter.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,24 +28,25 @@
 from collections import Counter, namedtuple
 from distutils.version import LooseVersion
 from itertools import dropwhile
 
 from cssselect import GenericTranslator
 
 from bzt import TaurusConfigError, ToolError, TaurusInternalException, TaurusNetworkError
-from bzt.engine import ScenarioExecutor, Scenario, FileLister, HavingInstallableTools, SelfDiagnosable
+from bzt.engine import ScenarioExecutor, Scenario, FileLister, HavingInstallableTools, SelfDiagnosable, Provisioning
 from bzt.modules.aggregator import ConsolidatingAggregator, ResultsReader, DataPoint, KPISet
 from bzt.modules.console import WidgetProvider, ExecutorWidget
 from bzt.modules.functional import FunctionalAggregator, FunctionalResultsReader, FunctionalSample
 from bzt.modules.provisioning import Local
 from bzt.modules.soapui import SoapUIScriptConverter
 from bzt.requests_model import ResourceFilesCollector
-from bzt.six import iteritems, string_types, StringIO, etree, binary_type, parse, unicode_decode
+from bzt.six import communicate
+from bzt.six import iteritems, string_types, StringIO, etree, parse, unicode_decode, numeric_types
 from bzt.utils import get_full_path, EXE_SUFFIX, MirrorsManager, ExceptionalDownloader, get_uniq_name
-from bzt.utils import shell_exec, BetterDict, guess_csv_dialect
+from bzt.utils import shell_exec, BetterDict, guess_csv_dialect, ensure_is_dict, dehumanize_time
 from bzt.utils import unzip, RequiredTool, JavaVM, shutdown_process, ProgressBarContext, TclLibrary
 from bzt.jmx import JMX, JMeterScenarioBuilder, LoadSettingsProcessor
 
 
 class JMeterExecutor(ScenarioExecutor, WidgetProvider, FileLister, HavingInstallableTools, SelfDiagnosable):
     """
     JMeter executor module
@@ -53,18 +54,19 @@
     :type modified_jmx: str
     :type jmeter_log: str
     :type properties_file: str
     :type sys_properties_file: str
     """
     MIRRORS_SOURCE = "https://jmeter.apache.org/download_jmeter.cgi"
     JMETER_DOWNLOAD_LINK = "https://archive.apache.org/dist/jmeter/binaries/apache-jmeter-{version}.zip"
-    PLUGINS_MANAGER = 'https://search.maven.org/remotecontent?filepath=' \
-                      'kg/apc/jmeter-plugins-manager/0.15/jmeter-plugins-manager-0.15.jar'
+    PLUGINS_MANAGER_VERSION = "0.16"
+    PLUGINS_MANAGER = 'https://search.maven.org/remotecontent?filepath=kg/apc/jmeter-plugins-manager/'\
+            '{ver}/jmeter-plugins-manager-{ver}.jar'.format(ver=PLUGINS_MANAGER_VERSION)
     CMDRUNNER = 'https://search.maven.org/remotecontent?filepath=kg/apc/cmdrunner/2.0/cmdrunner-2.0.jar'
-    JMETER_VER = "3.2"
+    JMETER_VER = "3.3"
     UDP_PORT_NUMBER = None
 
     def __init__(self):
         super(JMeterExecutor, self).__init__()
         self.original_jmx = None
         self.modified_jmx = None
         self.jmeter_log = None
@@ -79,14 +81,123 @@
         self.management_port = None
         self._env = {}
         self.resource_files_collector = None
         self.stdout_file = None
         self.stderr_file = None
         self.tool = None
 
+    def get_load(self):
+        """
+        Helper method to read load specification
+        """
+        load = self.get_specific_load()
+
+        throughput = load.throughput
+        concurrency = load.concurrency
+        iterations = load.iterations
+        steps = load.steps
+        hold = load.hold
+        ramp_up = load.ramp_up
+
+        hold = self._try_convert(hold, dehumanize_time, 0)
+        duration = hold
+
+        if ramp_up is not None:
+            ramp_up = self._try_convert(ramp_up, dehumanize_time, 0)
+            duration += ramp_up
+
+        msg = ''
+        if not isinstance(concurrency, numeric_types + (type(None),)):
+            msg += "\nNon-integer concurrency value [%s]: %s " % (type(concurrency).__name__, concurrency)
+        if not isinstance(throughput, numeric_types + (type(None),)):
+            msg += "\nNon-integer throughput value [%s]: %s " % (type(throughput).__name__, throughput)
+        if not isinstance(steps, numeric_types + (type(None),)):
+            msg += "\nNon-integer steps value [%s]: %s " % (type(steps).__name__, steps)
+        if not isinstance(iterations, numeric_types + (type(None),)):
+            msg += "\nNon-integer iterations value [%s]: %s " % (type(iterations).__name__, iterations)
+
+        if msg:
+            self.log.warning(msg)
+
+        throughput = self._try_convert(throughput, float, 0)
+        concurrency = self._try_convert(concurrency, int, 0)
+        iterations = self._try_convert(iterations, int, 0)
+        steps = self._try_convert(steps, int, 0)
+
+        if duration and not iterations:
+            iterations = 0  # which means infinite
+
+        return self.LOAD_FMT(concurrency=concurrency, ramp_up=ramp_up, throughput=throughput, hold=hold,
+                             iterations=iterations, duration=duration, steps=steps)
+
+    @staticmethod
+    def _get_prop_default(val):
+        comma_ind = val.find(",")
+        if val.startswith("${") and val.endswith(")}") and comma_ind > -1:
+            return val[comma_ind + 1: -2]
+        else:
+            return None
+
+    @staticmethod
+    def _try_convert(val, func, default=None):
+        if val is None:
+            res = val
+        elif isinstance(val, string_types) and val.startswith('$'):   # it's property...
+            if default is not None:
+                val = JMeterExecutor._get_prop_default(val) or default
+                res = func(val)
+            else:
+                res = val
+        else:
+            res = func(val)
+
+        return res
+
+    def get_specific_load(self):
+        """
+        Helper method to read load specification
+        """
+        prov_type = self.engine.config.get(Provisioning.PROV)
+
+        ensure_is_dict(self.execution, ScenarioExecutor.THRPT, prov_type)
+        throughput = self.execution[ScenarioExecutor.THRPT].get(prov_type, 0)
+
+        ensure_is_dict(self.execution, ScenarioExecutor.CONCURR, prov_type)
+        concurrency = self.execution[ScenarioExecutor.CONCURR].get(prov_type, 0)
+
+        iterations = self.execution.get("iterations", None)
+
+        steps = self.execution.get(ScenarioExecutor.STEPS, None)
+
+        hold = self.execution.get(ScenarioExecutor.HOLD_FOR, 0)
+        hold = self._try_convert(hold, dehumanize_time)
+
+        ramp_up = self.execution.get(ScenarioExecutor.RAMP_UP, None)
+        ramp_up = self._try_convert(ramp_up, dehumanize_time)
+
+        if not hold:
+            duration = ramp_up
+        elif not ramp_up:
+            duration = hold
+        elif isinstance(ramp_up, numeric_types) and isinstance(hold, numeric_types):
+            duration = hold + ramp_up
+        else:
+            duration = 1        # dehumanize_time(<sum_of_props>) can be unpredictable so we use default there
+
+        throughput = self._try_convert(throughput, float)
+        concurrency = self._try_convert(concurrency, int)
+        iterations = self._try_convert(iterations, int)
+        steps = self._try_convert(steps, int)
+
+        if duration and not iterations:
+            iterations = 0  # which means infinite
+
+        return self.LOAD_FMT(concurrency=concurrency, ramp_up=ramp_up, throughput=throughput, hold=hold,
+                             iterations=iterations, duration=duration, steps=steps)
+
     def get_scenario(self, name=None, cache_scenario=True):
         scenario_obj = super(JMeterExecutor, self).get_scenario(name=name, cache_scenario=False)
 
         if not isinstance(self.engine.provisioning, Local):
             return scenario_obj
 
         if Scenario.SCRIPT in scenario_obj and scenario_obj[Scenario.SCRIPT] is not None:
@@ -124,52 +235,71 @@
         merged_scenario.merge(base_scenario.data)
         for field in [Scenario.SCRIPT, "test-case"]:
             if field in merged_scenario:
                 merged_scenario.pop(field)
 
         return scenario_name, merged_scenario
 
+    @staticmethod
+    def _get_tool_version(jmx_file):
+        jmx = JMX(jmx_file)
+        selector = 'jmeterTestPlan'
+        test_plan = jmx.get(selector)[0]
+        ver = test_plan.get('jmeter')
+        if isinstance(ver, string_types):
+            index = ver.find(" ")
+            if index != -1:
+                return ver[:index]
+
+        return JMeterExecutor.JMETER_VER
+
     def prepare(self):
         """
         Preparation for JMeter involves either getting existing JMX
         and modifying it, or generating new JMX from input data. Then,
         original JMX is modified to contain JTL writing classes with
         required settings and have workload as suggested by Provisioning
 
         :raise TaurusConfigError:
         """
         scenario = self.get_scenario()
 
         self.jmeter_log = self.engine.create_artifact("jmeter", ".log")
         self._set_remote_port()
-        self.install_required_tools()
         self.distributed_servers = self.execution.get('distributed', self.distributed_servers)
 
         is_jmx_generated = False
 
         self.original_jmx = self.get_script_path()
+        if self.settings.get("version", self.JMETER_VER) == "auto":
+            self.settings["version"] = self._get_tool_version(self.original_jmx)
+        self.install_required_tools()
+
         if not self.original_jmx:
             if scenario.get("requests"):
                 self.original_jmx = self.__jmx_from_requests()
                 is_jmx_generated = True
             else:
                 raise TaurusConfigError("You must specify either a JMX file or list of requests to run JMeter")
 
+        # check for necessary plugins and install them if needed
+        if self.settings.get("detect-plugins", True):
+            self.tool.install_for_jmx(self.original_jmx)
+
         if self.engine.aggregator.is_functional:
             flags = {"connectTime": True}
-            version = str(self.settings.get("version", self.JMETER_VER))
-            if version.startswith("2"):
+            version = LooseVersion(str(self.settings.get("version", self.JMETER_VER)))
+            major = version.version[0]
+            if major == 2:
                 flags["bytes"] = True
             else:
                 flags["sentBytes"] = True
             self.settings.merge({"xml-jtl-flags": flags})
 
-        load = self.get_load()
-
-        modified = self.__get_modified_jmx(self.original_jmx, load, is_jmx_generated)
+        modified = self.__get_modified_jmx(self.original_jmx, is_jmx_generated)
         self.modified_jmx = self.__save_modified_jmx(modified, self.original_jmx, is_jmx_generated)
 
         self.__set_jmeter_properties(scenario)
         self.__set_system_properties()
         self.__set_jvm_properties()
 
         out = self.engine.create_artifact("jmeter", ".out")
@@ -256,14 +386,16 @@
             cmdline += ["-S", os.path.abspath(self.sys_properties_file)]
         if self.distributed_servers and not self.settings.get("gui", False):
             cmdline += ['-R%s' % ','.join(self.distributed_servers)]
 
         self.start_time = time.time()
         try:
             self.process = self.execute(cmdline, stdout=self.stdout_file, stderr=self.stderr_file, env=self._env)
+        except KeyboardInterrupt:
+            raise
         except BaseException as exc:
             ToolError("%s\nFailed to start JMeter: %s" % (cmdline, exc))
 
     def check(self):
         """
         Checks if JMeter is still running. Also checks if resulting JTL contains
         any data and throws exception otherwise.
@@ -445,22 +577,22 @@
 
     def __force_tran_parent_sample(self, jmx):
         scenario = self.get_scenario()
         if scenario.get("force-parent-sample", True):
             self.log.debug("Enforcing parent sample for transaction controller")
             jmx.set_text('TransactionController > boolProp[name="TransactionController.parent"]', 'true')
 
-    def __get_modified_jmx(self, original, load, is_jmx_generated):
+    def __get_modified_jmx(self, original, is_jmx_generated):
         """
         add two listeners to test plan:
             - to collect basic stats for KPIs
             - to collect detailed errors/trace info
         :return: path to artifact
         """
-        self.log.debug("Load: %s", load)
+        self.log.debug("Load: %s", self.get_specific_load())
         jmx = JMX(original)
 
         if self.get_scenario().get("disable-listeners", not self.settings.get("gui", False)):
             JMeterExecutor.__disable_listeners(jmx)
 
         user_def_vars = self.get_scenario().get("variables")
         if user_def_vars:
@@ -473,15 +605,16 @@
             jmx.append(JMeterScenarioBuilder.TEST_PLAN_SEL, etree.Element("hashTree"))
 
         self.__apply_test_mode(jmx)
         LoadSettingsProcessor(self).modify(jmx)
         self.__add_result_listeners(jmx)
         if not is_jmx_generated:
             self.__force_tran_parent_sample(jmx)
-            if self.settings.get('version', self.JMETER_VER) >= '3.2':
+            version = LooseVersion(str(self.settings.get('version', self.JMETER_VER)))
+            if version >= LooseVersion("3.2"):
                 self.__force_hc4_cookie_handler(jmx)
         self.__fill_empty_delimiters(jmx)
 
         self.__apply_modifications(jmx)
 
         return jmx
 
@@ -1372,31 +1505,50 @@
         self.tool_path = self.tool_path.format(version=self.version)
 
     def check_if_installed(self):
         self.log.debug("Trying jmeter: %s", self.tool_path)
         try:
             with tempfile.NamedTemporaryFile(prefix="jmeter", suffix="log", delete=False) as jmlog:
                 jm_proc = shell_exec([self.tool_path, '-j', jmlog.name, '--version'], stderr=subprocess.STDOUT)
-                jmout, jmerr = jm_proc.communicate()
+                jmout, jmerr = communicate(jm_proc)
                 self.log.debug("JMeter check: %s / %s", jmout, jmerr)
 
             os.remove(jmlog.name)
 
-            if isinstance(jmout, binary_type):
-                jmout = jmout.decode()
-
             if "is too low to run JMeter" in jmout:
                 raise ToolError("Java version is too low to run JMeter")
 
             return True
 
         except OSError:
             self.log.debug("JMeter check failed.")
             return False
 
+    def _pmgr_call(self, params):
+        cmd = [self._pmgr_path()] + params
+        proc = shell_exec(cmd)
+        return communicate(proc)
+
+    def install_for_jmx(self, jmx_file):
+        if not os.path.isfile(jmx_file):
+            self.log.warning("Script %s not found" % jmx_file)
+            return
+
+        try:
+            out, err = self._pmgr_call(["install-for-jmx", jmx_file])
+            self.log.debug("Try to detect plugins for %s\n%s\n%s", jmx_file, out, err)
+        except KeyboardInterrupt:
+            raise
+        except BaseException as exc:
+            self.log.warning("Failed to detect plugins for %s: %s", jmx_file, exc)
+            return
+
+        if err and "Wrong command: install-for-jmx" in err:     # old manager
+            self.log.debug("pmgr can't discover jmx for plugins")
+
     def __install_jmeter(self, dest):
         if self.download_link:
             jmeter_dist = self._download(use_link=True)
         else:
             jmeter_dist = self._download()
 
         try:
@@ -1417,25 +1569,29 @@
         with ProgressBarContext() as pbar:
             for tool in tools:
                 url = tool[0]
                 _file = os.path.basename(url)
                 self.log.info("Downloading %s from %s", _file, url)
                 try:
                     downloader.get(url, tool[1], reporthook=pbar.download_callback)
+                except KeyboardInterrupt:
+                    raise
                 except BaseException as exc:
                     raise TaurusNetworkError("Error while downloading %s: %s" % (_file, exc))
 
     def __install_plugins_manager(self, plugins_manager_path):
         installer = "org.jmeterplugins.repository.PluginManagerCMDInstaller"
         cmd = ["java", "-cp", plugins_manager_path, installer]
         self.log.debug("Trying: %s", cmd)
         try:
             proc = shell_exec(cmd)
-            out, err = proc.communicate()
+            out, err = communicate(proc)
             self.log.debug("Install PluginsManager: %s / %s", out, err)
+        except KeyboardInterrupt:
+            raise
         except BaseException as exc:
             raise ToolError("Failed to install PluginsManager: %s" % exc)
 
     def __install_plugins(self, plugins_manager_cmd):
         plugin_str = ",".join(self.plugins)
         self.log.info("Installing JMeter plugins: %s", plugin_str)
         cmd = [plugins_manager_cmd, 'install', plugin_str]
@@ -1464,30 +1620,36 @@
                     # property names correspond to
                     # https://github.com/apache/jmeter/blob/trunk/src/core/org/apache/jmeter/JMeter.java#L110
                     jvm_args += ' -Dhttp.proxyUser="%s" -Dhttp.proxyPass="%s"' % (username, password)
 
                 env['JVM_ARGS'] = jvm_args
 
             proc = shell_exec(cmd)
-            out, err = proc.communicate()
+            out, err = communicate(proc)
             self.log.debug("Install plugins: %s / %s", out, err)
+        except KeyboardInterrupt:
+            raise
         except BaseException as exc:
             raise ToolError("Failed to install plugins %s: %s" % (plugin_str, exc))
 
+    def _pmgr_path(self):
+        dest = get_full_path(self.tool_path, step_up=2)
+        return os.path.join(dest, 'bin', 'PluginsManagerCMD' + EXE_SUFFIX)
+
     def install(self):
         dest = get_full_path(self.tool_path, step_up=2)
         self.log.info("Will install %s into %s", self.tool_name, dest)
         plugins_manager_name = os.path.basename(JMeterExecutor.PLUGINS_MANAGER)
         cmdrunner_name = os.path.basename(JMeterExecutor.CMDRUNNER)
         plugins_manager_path = os.path.join(dest, 'lib', 'ext', plugins_manager_name)
         cmdrunner_path = os.path.join(dest, 'lib', cmdrunner_name)
         direct_install_tools = [  # source link and destination
             [JMeterExecutor.PLUGINS_MANAGER, plugins_manager_path],
             [JMeterExecutor.CMDRUNNER, cmdrunner_path]]
-        plugins_manager_cmd = os.path.join(dest, 'bin', 'PluginsManagerCMD' + EXE_SUFFIX)
+        plugins_manager_cmd = self._pmgr_path()
 
         self.__install_jmeter(dest)
         self.__download_additions(direct_install_tools)
         self.__install_plugins_manager(plugins_manager_path)
         self.__install_plugins(plugins_manager_cmd)
 
         cleaner = JarCleaner(self.log)
```

### Comparing `bzt-1.9.5/bzt/modules/pbench.py` & `bzt-1.9.6/bzt/modules/pbench.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/modules/__init__.py` & `bzt-1.9.6/bzt/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/modules/services.py` & `bzt-1.9.6/bzt/modules/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,21 +18,22 @@
 
 import copy
 import os
 import subprocess
 import time
 import zipfile
 import json
+from bzt.six import communicate
 
 try:
     from pyvirtualdisplay.smartdisplay import SmartDisplay as Display
 except ImportError:
     from pyvirtualdisplay import Display
 
-from bzt import NormalShutdown, ToolError, TaurusConfigError, TaurusInternalException, ManualShutdown
+from bzt import NormalShutdown, ToolError, TaurusConfigError, TaurusInternalException
 from bzt.engine import Service, HavingInstallableTools, Singletone
 from bzt.six import get_stacktrace, urlopen, URLError
 from bzt.utils import get_full_path, shutdown_process, shell_exec, RequiredTool, is_windows
 from bzt.utils import replace_in_config, JavaVM, Node
 
 
 class Unpacker(Service):
@@ -141,15 +142,15 @@
         if not os.path.isfile(adb_path):
             self.log.debug('adb is not found in sdk, trying to use an external one..')
             adb_path = 'adb'
         cmd = [adb_path, "shell", "getprop", "sys.boot_completed"]
         self.log.debug("Trying: %s", cmd)
         try:
             proc = shell_exec(cmd)
-            out, _ = proc.communicate()
+            out, _ = communicate(proc)
             return out.strip() == '1'
         except BaseException as exc:
             raise ToolError('Checking if android emulator starts is impossible: %s', exc)
 
     def shutdown(self):
         if self.emulator_process:
             self.log.debug('Stopping android emulator...')
```

### Comparing `bzt-1.9.5/bzt/modules/console.py` & `bzt-1.9.6/bzt/modules/console.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/modules/python.py` & `bzt-1.9.6/bzt/modules/python.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import ast
 import copy
 import os
 import re
+import shlex
 import sys
 from abc import abstractmethod
 from collections import OrderedDict
 
 import apiritif
 import astunparse
 
@@ -1179,7 +1180,91 @@
             self.log.debug("Translating function %s with arguments %s", varname, arguments)
             func = functions[varname](self)
             result = func.to_python(args)
             if result is None:
                 result = ast.Name(id=varname, ctx=ast.Load())
         self.log.debug("Compile: %r -> %r", expr, result)
         return result
+
+
+class PyTestExecutor(SubprocessedExecutor, HavingInstallableTools):
+    def __init__(self):
+        super(PyTestExecutor, self).__init__()
+        self.runner_path = os.path.join(get_full_path(__file__, step_up=2), "resources", "pytest_runner.py")
+        self._tailer = NoneTailer()
+        self._additional_args = []
+
+    def prepare(self):
+        self.install_required_tools()
+        self.script = self.get_script_path()
+        if not self.script:
+            raise TaurusConfigError("'script' should be present for pytest executor")
+
+        scenario = self.get_scenario()
+        if "additional-args" in scenario:
+            argv = scenario.get("additional-args")
+            self._additional_args = shlex.split(argv)
+
+        self.reporting_setup(suffix=".ldjson")
+
+    def __is_verbose(self):
+        engine_verbose = self.engine.config.get(SETTINGS).get("verbose", False)
+        executor_verbose = self.settings.get("verbose", engine_verbose)
+        return executor_verbose
+
+    def install_required_tools(self):
+        """
+        we need installed nose plugin
+        """
+        if sys.version >= '3':
+            self.log.warning("You are using Python 3, make sure that your scripts are able to run in Python 3")
+
+        self._check_tools([TaurusPytestRunner(self.runner_path, "")])
+
+    def startup(self):
+        """
+        run python tests
+        """
+        executable = self.settings.get("interpreter", sys.executable)
+
+        self.env.update({"PYTHONPATH": os.getenv("PYTHONPATH", "") + os.pathsep + get_full_path(__file__, step_up=3)})
+
+        cmdline = [executable, self.runner_path, '--report-file', self.report_file]
+        cmdline += self._additional_args
+
+        load = self.get_load()
+        if load.iterations:
+            cmdline += ['-i', str(load.iterations)]
+
+        if load.hold:
+            cmdline += ['-d', str(load.hold)]
+
+        cmdline += [self.script]
+        self._start_subprocess(cmdline)
+
+        if self.__is_verbose():
+            self._tailer = FileTailer(self.stdout_file)
+
+    def check(self):
+        self.__log_lines()
+        return super(PyTestExecutor, self).check()
+
+    def post_process(self):
+        super(PyTestExecutor, self).post_process()
+        self.__log_lines()
+
+    def __log_lines(self):
+        lines = []
+        for line in self._tailer.get_lines():
+            if not IGNORED_LINE.match(line):
+                lines.append(line)
+
+        if lines:
+            self.log.info("\n".join(lines))
+
+
+class TaurusPytestRunner(RequiredTool):
+    def __init__(self, tool_path, download_link):
+        super(TaurusPytestRunner, self).__init__("TaurusPytestRunner", tool_path, download_link)
+
+    def install(self):
+        raise ToolError("Automatic installation of Taurus pytest runner isn't implemented")
```

### Comparing `bzt-1.9.5/bzt/modules/java.py` & `bzt-1.9.6/bzt/modules/java.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/modules/gatling.py` & `bzt-1.9.6/bzt/modules/gatling.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
 
 class GatlingExecutor(ScenarioExecutor, WidgetProvider, FileLister, HavingInstallableTools, SelfDiagnosable):
     """
     Gatling executor module
     """
     DOWNLOAD_LINK = "https://repo1.maven.org/maven2/io/gatling/highcharts/gatling-charts-highcharts-bundle" \
                     "/{version}/gatling-charts-highcharts-bundle-{version}-bundle.zip"
-    VERSION = "2.1.7"
+    VERSION = "2.3.0"
 
     def __init__(self):
         super(GatlingExecutor, self).__init__()
         self.script = None
         self.process = None
         self.end_time = None
         self.retcode = None
@@ -388,19 +388,25 @@
         load = self.get_load()
         scenario = self.get_scenario()
 
         timeout = scenario.get('timeout', None)
         if timeout is not None:
             params_for_scala['gatling.http.ahc.requestTimeout'] = int(dehumanize_time(timeout) * 1000)
         if scenario.get('keepalive', True):
+            # gatling <= 2.2.0
             params_for_scala['gatling.http.ahc.allowPoolingConnections'] = 'true'
             params_for_scala['gatling.http.ahc.allowPoolingSslConnections'] = 'true'
+            # gatling > 2.2.0
+            params_for_scala['gatling.http.ahc.keepAlive'] = 'true'
         else:
+            # gatling <= 2.2.0
             params_for_scala['gatling.http.ahc.allowPoolingConnections'] = 'false'
             params_for_scala['gatling.http.ahc.allowPoolingSslConnections'] = 'false'
+            # gatling > 2.2.0
+            params_for_scala['gatling.http.ahc.keepAlive'] = 'false'
         if load.concurrency is not None:
             params_for_scala['concurrency'] = load.concurrency
         if load.ramp_up is not None:
             params_for_scala['ramp-up'] = int(load.ramp_up)
         if load.hold is not None:
             params_for_scala['hold-for'] = int(load.hold)
         if load.iterations is not None and load.iterations != 0:
@@ -465,19 +471,21 @@
         Save data log as artifact
         """
         if self.reader and self.reader.filename:
             self.engine.existing_artifact(self.reader.filename)
 
     def install_required_tools(self):
         required_tools = [TclLibrary(self.log), JavaVM(self.log)]
-        gatling_path = self.settings.get("path", "~/.bzt/gatling-taurus/bin/gatling" + EXE_SUFFIX)
+        gatling_version = self.settings.get("version", GatlingExecutor.VERSION)
+        def_path = "~/.bzt/gatling-taurus/{version}/bin/gatling{suffix}".format(version=gatling_version,
+                                                                                suffix=EXE_SUFFIX)
+        gatling_path = self.settings.get("path", def_path)
         gatling_path = os.path.abspath(os.path.expanduser(gatling_path))
         self.settings["path"] = gatling_path
         download_link = self.settings.get("download-link", GatlingExecutor.DOWNLOAD_LINK)
-        gatling_version = self.settings.get("version", GatlingExecutor.VERSION)
         required_tools.append(Gatling(gatling_path, self.log, download_link, gatling_version))
 
         for tool in required_tools:
             if not tool.check_if_installed():
                 tool.install()
 
     def get_widget(self):
@@ -623,29 +631,29 @@
             error = fields[8]
         else:
             error = None
         return int(t_stamp), label, r_time, con_time, latency, r_code, error
 
     def _guess_gatling_version(self, fields):
         if fields[0].strip() in ["USER", "REQUEST", "RUN"]:
-            self.log.debug("Parsing Gatling 2.2 stats")
-            return "2.2"
+            self.log.debug("Parsing Gatling 2.2+ stats")
+            return "2.2+"
         elif fields[2].strip() in ["USER", "REQUEST", "RUN"]:
             self.log.debug("Parsing Gatling 2.1 stats")
             return "2.1"
         else:
             return None
 
     def _extract_log_data(self, fields):
         if self.guessed_gatling_version is None:
             self.guessed_gatling_version = self._guess_gatling_version(fields)
 
         if self.guessed_gatling_version == "2.1":
             return self._extract_log_gatling_21(fields)
-        elif self.guessed_gatling_version == "2.2":
+        elif self.guessed_gatling_version == "2.2+":
             return self._extract_log_gatling_22(fields)
         else:
             return None
 
     def _read(self, last_pass=False):
         """
         Generator method that returns next portion of data
```

### Comparing `bzt-1.9.5/bzt/modules/siege.py` & `bzt-1.9.6/bzt/modules/siege.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/modules/soapui.py` & `bzt-1.9.6/bzt/modules/soapui.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/modules/csharp.py` & `bzt-1.9.6/bzt/modules/csharp.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/modules/locustio.py` & `bzt-1.9.6/bzt/modules/locustio.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/modules/tsung.py` & `bzt-1.9.6/bzt/modules/tsung.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/modules/provisioning.py` & `bzt-1.9.6/bzt/modules/provisioning.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/modules/screen.py` & `bzt-1.9.6/bzt/modules/screen.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,18 +130,17 @@
         self.text.config(state=tkinter.NORMAL)
         self.text.delete("1.0", tkinter.END)
 
         for idx, row in enumerate(canvas.content()):
             pos = 0
             for part in row:
                 txt = part[2]
-                if isinstance(txt, text_type):
-                    strlen = len(txt)
-                else:
-                    strlen = len(txt.decode('utf8'))
+                if not isinstance(txt, text_type):
+                    txt = txt.decode('utf8')
+                strlen = len(txt)
                 self.text.insert(tkinter.END, txt)
                 if part[0] is not None:
                     self.text.tag_add(part[0], "%s.%s" % (idx + 1, pos), "%s.%s" % (idx + 1, pos + strlen))
                 pos += strlen
 
             self.text.insert(tkinter.END, "\n")
```

### Comparing `bzt-1.9.5/bzt/modules/passfail.py` & `bzt-1.9.6/bzt/modules/passfail.py`

 * *Files 0% similar despite different names*

```diff
@@ -375,15 +375,15 @@
         if ',' in crit_config:
             crit_str = crit_config[:crit_config.index(',')].strip()
             action_str = crit_config[crit_config.index(',') + 1:].strip()
         else:
             crit_str = crit_config
             action_str = ""
 
-        crit_pat = re.compile(r"([\w\?-]+)(\s*of\s*([\S ]+))?\s*([<>=]+)\s*(\S+)(\s+(for|within|over)\s+(\S+))?")
+        crit_pat = re.compile(r"([\w?*.-]+)(\s*of\s*([\S ]+))?\s*([<>=]+)\s*(\S+)(\s+(for|within|over)\s+(\S+))?")
         crit_match = crit_pat.match(crit_str.strip())
         if not crit_match:
             raise TaurusConfigError("Criteria string is mailformed in its condition part: %s" % crit_str)
         crit_groups = crit_match.groups()
         res["subject"] = crit_groups[0]
         res["condition"] = crit_groups[3]
         res["threshold"] = crit_groups[4]
```

### Comparing `bzt-1.9.5/bzt/modules/shellexec.py` & `bzt-1.9.6/bzt/modules/shellexec.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/six/py2.py` & `bzt-1.9.6/bzt/six/py2.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,7 +87,11 @@
 
 
 def unicode_decode(string):
     if not isinstance(string, unicode):
         return string.decode('utf-8')
     else:
         return string
+
+
+def communicate(proc):
+    return proc.communicate()
```

### Comparing `bzt-1.9.5/bzt/six/__init__.py` & `bzt-1.9.6/bzt/six/__init__.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/six/py3.py` & `bzt-1.9.6/bzt/six/py3.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,36 +12,33 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 # pylint: skip-file
-
 import io
+import sys
 import operator
 import collections
 import traceback
 import urllib
-from io import IOBase
-
-import urllib.error
-import urllib.request
-import urllib.parse
+import socketserver
 import configparser
+
 from http import server, cookiejar
-import socketserver
+
 
 string_types = str,
 integer_types = int,
 numeric_types=(int, float, complex)
 class_types = type,
 text_type = str
 binary_type = bytes
-file_type = IOBase
+file_type = io.IOBase
 
 configparser = configparser
 UserDict = collections.UserDict
 
 StringIO = io.StringIO
 BytesIO = io.BytesIO
 
@@ -85,7 +82,15 @@
     exc = _type(message)
     exc.__traceback__ = stacktrace
     raise exc
 
 
 def unicode_decode(string):
     return string
+
+
+def communicate(proc):
+    stdout, stderr = proc.communicate()
+    if stderr:
+        stderr = str(stderr, sys.stderr.encoding or sys.getfilesystemencoding())
+    stdout = str(stdout, sys.stdout.encoding or sys.getfilesystemencoding())
+    return stdout, stderr
```

### Comparing `bzt-1.9.5/bzt/resources/rspec_taurus_plugin.rb` & `bzt-1.9.6/bzt/resources/rspec_taurus_plugin.rb`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/resources/nose_plugin.py` & `bzt-1.9.6/bzt/resources/nose_plugin.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/resources/mocha-taurus-plugin.js` & `bzt-1.9.6/bzt/resources/mocha-taurus-plugin.js`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/resources/base-bzt-rc.yml` & `bzt-1.9.6/bzt/resources/base-bzt-rc.yml`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/resources/taurus-junit-1.0.jar` & `bzt-1.9.6/bzt/resources/taurus-junit-1.0.jar`

 * *Files 14% similar despite different names*

#### zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 11692 bytes, number of entries: 13
-drwxr-xr-x  2.0 unx        0 b- stor 16-Aug-31 12:10 META-INF/
--rw-r--r--  2.0 unx      125 b- defN 16-Aug-31 12:10 META-INF/MANIFEST.MF
-drwxr-xr-x  2.0 unx        0 b- stor 16-Aug-29 18:28 taurusjunit/
--rw-r--r--  2.0 unx     3261 b- defN 16-Aug-30 17:50 taurusjunit/Sample.class
--rw-r--r--  2.0 unx     2715 b- defN 16-Aug-31 12:10 taurusjunit/TaurusReporter.class
--rw-r--r--  2.0 unx      830 b- defN 16-Aug-29 18:28 taurusjunit/Utils.class
--rw-r--r--  2.0 unx     7328 b- defN 16-Aug-29 18:28 taurusjunit/CustomRunner.class
--rw-r--r--  2.0 unx     4349 b- defN 16-Aug-31 12:10 taurusjunit/CustomListener.class
-drwxr-xr-x  2.0 unx        0 b- stor 16-Aug-31 12:10 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 16-Aug-31 12:10 META-INF/maven/org.blazemeter.taurus/
-drwxr-xr-x  2.0 unx        0 b- stor 16-Aug-31 12:10 META-INF/maven/org.blazemeter.taurus/taurus-junit/
--rw-r--r--  2.0 unx     2759 b- defN 16-Aug-29 18:28 META-INF/maven/org.blazemeter.taurus/taurus-junit/pom.xml
--rw-r--r--  2.0 unx      116 b- defN 16-Aug-30 17:50 META-INF/maven/org.blazemeter.taurus/taurus-junit/pom.properties
-13 files, 21483 bytes uncompressed, 9872 bytes compressed:  54.0%
+Zip file size: 11389 bytes, number of entries: 13
+drwxr-xr-x  2.0 unx        0 b- stor 17-Sep-27 13:32 META-INF/
+-rw-r--r--  2.0 unx      132 b- defN 17-Sep-27 13:32 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 17-Sep-27 13:32 taurusjunit/
+-rw-rw-r--  2.0 unx     3261 b- defN 17-Sep-27 13:32 taurusjunit/Sample.class
+-rw-rw-r--  2.0 unx     4349 b- defN 17-Sep-27 13:32 taurusjunit/CustomListener.class
+-rw-rw-r--  2.0 unx      830 b- defN 17-Sep-27 13:32 taurusjunit/Utils.class
+-rw-rw-r--  2.0 unx     7328 b- defN 17-Sep-27 13:32 taurusjunit/CustomRunner.class
+-rw-rw-r--  2.0 unx     2715 b- defN 17-Sep-27 13:32 taurusjunit/TaurusReporter.class
+?rwsrwsrwt  2.0 unx        0 b- stor 17-Sep-27 13:32 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 17-Sep-27 13:32 META-INF/maven/org.blazemeter.taurus/
+?rwsrwsrwt  2.0 unx        0 b- stor 17-Sep-27 13:32 META-INF/maven/org.blazemeter.taurus/taurus-junit/
+-rw-rw-r--  2.0 unx     1329 b- defN 16-Aug-28 21:55 META-INF/maven/org.blazemeter.taurus/taurus-junit/pom.xml
+-rw-rw-r--  2.0 unx      116 b- defN 17-Sep-27 13:32 META-INF/maven/org.blazemeter.taurus/taurus-junit/pom.properties
+13 files, 20060 bytes uncompressed, 9569 bytes compressed:  52.3%
```

#### zipnote «TEMP»/diffoscope_6eep_6th_/tmpb0p1tpew_.zip

```diff
@@ -6,24 +6,24 @@
 
 Filename: taurusjunit/
 Comment: 
 
 Filename: taurusjunit/Sample.class
 Comment: 
 
-Filename: taurusjunit/TaurusReporter.class
+Filename: taurusjunit/CustomListener.class
 Comment: 
 
 Filename: taurusjunit/Utils.class
 Comment: 
 
 Filename: taurusjunit/CustomRunner.class
 Comment: 
 
-Filename: taurusjunit/CustomListener.class
+Filename: taurusjunit/TaurusReporter.class
 Comment: 
 
 Filename: META-INF/maven/
 Comment: 
 
 Filename: META-INF/maven/org.blazemeter.taurus/
 Comment:
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Archiver-Version: Plexus Archiver
-Created-By: Apache Maven
-Built-By: dmand
-Build-Jdk: 1.8.0_101
+Built-By: undera
+Created-By: Apache Maven 3.3.9
+Build-Jdk: 1.8.0_144
```

#### META-INF/maven/org.blazemeter.taurus/taurus-junit/pom.xml

##### META-INF/maven/org.blazemeter.taurus/taurus-junit/pom.xml

```diff
@@ -1,17 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <groupId>org.blazemeter.taurus</groupId>
   <artifactId>taurus-junit</artifactId>
   <version>1.0</version>
-  <properties>
-    <aspectj.version>1.8.5</aspectj.version>
-    <allure.version>1.4.11</allure.version>
-  </properties>
   <dependencies>
     <dependency>
       <groupId>junit</groupId>
       <artifactId>junit</artifactId>
       <version>4.12</version>
     </dependency>
     <dependency>
@@ -21,47 +17,20 @@
       <scope>test</scope>
     </dependency>
     <dependency>
       <groupId>org.json</groupId>
       <artifactId>json</artifactId>
       <version>20160810</version>
     </dependency>
-    <dependency>
-      <groupId>ru.yandex.qatools.allure</groupId>
-      <artifactId>allure-junit-adaptor</artifactId>
-      <version>${allure.version}</version>
-    </dependency>
   </dependencies>
   <build>
     <plugins>
       <plugin>
         <artifactId>maven-compiler-plugin</artifactId>
         <configuration>
           <source>1.7</source>
           <target>1.7</target>
         </configuration>
       </plugin>
-      <plugin>
-        <groupId>org.apache.maven.plugins</groupId>
-        <artifactId>maven-surefire-plugin</artifactId>
-        <version>2.14</version>
-        <configuration>
-          <testFailureIgnore>false</testFailureIgnore>
-          <argLine>-javaagent:${settings.localRepository}/org/aspectj/aspectjweaver/${aspectj.version}/aspectjweaver-${aspectj.version}.jar</argLine>
-          <properties>
-            <property>
-              <name>listener</name>
-              <value>ru.yandex.qatools.allure.junit.AllureRunListener</value>
-            </property>
-          </properties>
-        </configuration>
-        <dependencies>
-          <dependency>
-            <groupId>org.aspectj</groupId>
-            <artifactId>aspectjweaver</artifactId>
-            <version>${aspectj.version}</version>
-          </dependency>
-        </dependencies>
-      </plugin>
     </plugins>
   </build>
 </project>
```

#### META-INF/maven/org.blazemeter.taurus/taurus-junit/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Tue Aug 30 17:50:16 MSK 2016
+#Wed Sep 27 13:32:14 MSK 2017
 version=1.0
 groupId=org.blazemeter.taurus
 artifactId=taurus-junit
```

### Comparing `bzt-1.9.5/bzt/resources/taurus-testng-1.0.jar` & `bzt-1.9.6/bzt/resources/taurus-testng-1.0.jar`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 11460 bytes, number of entries: 13
-drwxr-xr-x  2.0 unx        0 b- stor 17-Jun-13 14:35 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 17-Jun-13 14:35 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 17-Jun-13 14:35 taurustestng/
--rw-rw-r--  2.0 unx      832 b- defN 17-Jun-13 14:35 taurustestng/Utils.class
--rw-rw-r--  2.0 unx     7027 b- defN 17-Jun-13 14:35 taurustestng/TestNGRunner.class
--rw-rw-r--  2.0 unx     3294 b- defN 17-Jun-13 14:35 taurustestng/Sample.class
--rw-rw-r--  2.0 unx     2711 b- defN 17-Jun-13 14:35 taurustestng/TaurusReporter.class
--rw-rw-r--  2.0 unx     4842 b- defN 17-Jun-13 14:35 taurustestng/TestListener.class
-?rwsrwsrwt  2.0 unx        0 b- stor 17-Jun-13 14:35 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 17-Jun-13 14:35 META-INF/maven/org.blazemeter.taurus/
-?rwsrwsrwt  2.0 unx        0 b- stor 17-Jun-13 14:35 META-INF/maven/org.blazemeter.taurus/taurus-testng/
--rw-rw-r--  2.0 unx     1338 b- defN 16-Nov-11 12:18 META-INF/maven/org.blazemeter.taurus/taurus-testng/pom.xml
--rw-rw-r--  2.0 unx      117 b- defN 17-May-10 12:39 META-INF/maven/org.blazemeter.taurus/taurus-testng/pom.properties
-13 files, 20291 bytes uncompressed, 9626 bytes compressed:  52.6%
+Zip file size: 11462 bytes, number of entries: 13
+drwxr-xr-x  2.0 unx        0 b- stor 17-Sep-27 13:34 META-INF/
+-rw-r--r--  2.0 unx      132 b- defN 17-Sep-27 13:34 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 17-Sep-27 13:32 taurustestng/
+-rw-rw-r--  2.0 unx     3294 b- defN 17-Sep-27 13:32 taurustestng/Sample.class
+-rw-rw-r--  2.0 unx     7027 b- defN 17-Sep-27 13:32 taurustestng/TestNGRunner.class
+-rw-rw-r--  2.0 unx      832 b- defN 17-Sep-27 13:32 taurustestng/Utils.class
+-rw-rw-r--  2.0 unx     4842 b- defN 17-Sep-27 13:32 taurustestng/TestListener.class
+-rw-rw-r--  2.0 unx     2711 b- defN 17-Sep-27 13:32 taurustestng/TaurusReporter.class
+?rwsrwsrwt  2.0 unx        0 b- stor 17-Sep-27 13:34 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 17-Sep-27 13:34 META-INF/maven/org.blazemeter.taurus/
+?rwsrwsrwt  2.0 unx        0 b- stor 17-Sep-27 13:34 META-INF/maven/org.blazemeter.taurus/taurus-testng/
+-rw-rw-r--  2.0 unx     1338 b- defN 16-Nov-06 13:22 META-INF/maven/org.blazemeter.taurus/taurus-testng/pom.xml
+-rw-rw-r--  2.0 unx      117 b- defN 17-Sep-27 13:34 META-INF/maven/org.blazemeter.taurus/taurus-testng/pom.properties
+13 files, 20293 bytes uncompressed, 9628 bytes compressed:  52.6%
```

#### zipnote «TEMP»/diffoscope_6eep_6th_/tmp5df616j1_.zip

```diff
@@ -3,27 +3,27 @@
 
 Filename: META-INF/MANIFEST.MF
 Comment: 
 
 Filename: taurustestng/
 Comment: 
 
-Filename: taurustestng/Utils.class
+Filename: taurustestng/Sample.class
 Comment: 
 
 Filename: taurustestng/TestNGRunner.class
 Comment: 
 
-Filename: taurustestng/Sample.class
+Filename: taurustestng/Utils.class
 Comment: 
 
-Filename: taurustestng/TaurusReporter.class
+Filename: taurustestng/TestListener.class
 Comment: 
 
-Filename: taurustestng/TestListener.class
+Filename: taurustestng/TaurusReporter.class
 Comment: 
 
 Filename: META-INF/maven/
 Comment: 
 
 Filename: META-INF/maven/org.blazemeter.taurus/
 Comment:
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Archiver-Version: Plexus Archiver
-Built-By: dmand
+Built-By: undera
 Created-By: Apache Maven 3.3.9
-Build-Jdk: 1.8.0_91
+Build-Jdk: 1.8.0_144
```

#### META-INF/maven/org.blazemeter.taurus/taurus-testng/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Wed May 10 12:39:44 MSK 2017
+#Wed Sep 27 13:34:25 MSK 2017
 version=1.0
 groupId=org.blazemeter.taurus
 artifactId=taurus-testng
```

### Comparing `bzt-1.9.5/bzt/resources/locustio-taurus-wrapper.py` & `bzt-1.9.6/bzt/resources/locustio-taurus-wrapper.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/resources/base-config.yml` & `bzt-1.9.6/bzt/resources/base-config.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     class: bzt.modules.gatling.GatlingExecutor
   grinder:
     class: bzt.modules.grinder.GrinderExecutor
   jmeter:
     class: bzt.modules.jmeter.JMeterExecutor
   locust:
     class: bzt.modules.locustio.LocustIOExecutor
+  molotov:
+    class: bzt.modules.molotov.MolotovExecutor
   pbench:
     class: bzt.modules.pbench.PBenchExecutor
   siege:
     class: bzt.modules.siege.SiegeExecutor
   tsung:
     class: bzt.modules.tsung.TsungExecutor
 
@@ -30,14 +32,16 @@
     class: bzt.modules.java.TestNGTester
   rspec:
     class: bzt.modules.ruby.RSpecTester
   mocha:
     class: bzt.modules.javascript.MochaTester
   nunit:
     class: bzt.modules.csharp.NUnitExecutor
+  pytest:
+    class: bzt.modules.python.PyTestExecutor
 
   # service & infra modules
   local:
     class: bzt.modules.provisioning.Local
   monitoring:
     class: bzt.modules.monitoring.Monitoring
   passfail:
```

### Comparing `bzt-1.9.5/bzt/resources/NUnitRunner/nunit.framework.dll` & `bzt-1.9.6/bzt/resources/NUnitRunner/nunit.framework.dll`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/resources/NUnitRunner/nunit-agent-x86.exe` & `bzt-1.9.6/bzt/resources/NUnitRunner/nunit-agent-x86.exe`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/resources/NUnitRunner/nunit.engine.dll` & `bzt-1.9.6/bzt/resources/NUnitRunner/nunit.engine.dll`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/resources/NUnitRunner/nunit.engine.api.dll` & `bzt-1.9.6/bzt/resources/NUnitRunner/nunit.engine.api.dll`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/resources/NUnitRunner/Mono.Options.dll` & `bzt-1.9.6/bzt/resources/NUnitRunner/Mono.Options.dll`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/resources/NUnitRunner/Mono.Cecil.dll` & `bzt-1.9.6/bzt/resources/NUnitRunner/Mono.Cecil.dll`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/resources/NUnitRunner/NUnitRunner.exe` & `bzt-1.9.6/bzt/resources/NUnitRunner/NUnitRunner.exe`

 * *Files 16% similar despite different names*

#### pedump {}

```diff
@@ -1,107 +1,107 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0x00000000
+	             Time stamp: 0x59c8c1f9
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x0102
 
 PE Header:
 	         Magic (0x010b): 0x010b
-	             LMajor (6): 0x08
+	             LMajor (6): 0x30
 	             LMinor (0): 0x00
-	              Code Size: 0x00002000
-	  Initialized Data Size: 0x00000600
+	              Code Size: 0x00002200
+	  Initialized Data Size: 0x00000800
 	Uninitialized Data Size: 0x00000000
-	        Entry Point RVA: 0x00003fae
+	        Entry Point RVA: 0x000040ea
 	 	  Code Base RVA: 0x00002000
-		  Data Base RVA: 0x00004000
+		  Data Base RVA: 0x00006000
 
 
 NT Header:
 	   Image Base (0x400000): 0x00400000
 	Section Alignment (8192): 0x00002000
 	   File Align (512/4096): 0x00000200
 	            OS Major (4): 0x0004
 	            OS Minor (0): 0x0000
 	  	  User Major (0): 0x0000
 	  	  User Minor (0): 0x0000
 	  	Subsys major (4): 0x0004
 	  	Subsys minor (0): 0x0000
 	 	       Reserverd: 0x00000000
-	 	      Image Size: 0x00008000
+	 	      Image Size: 0x0000a000
 	 	     Header Size: 0x00000200
 	            Checksum (0): 0x00000000
 	               Subsystem: 0x0003
 	           DLL Flags (0): 0x8540
 	 Stack Reserve Size (1M): 0x00100000
 	Stack commit Size (4096): 0x00001000
 	  Heap Reserve Size (1M): 0x00100000
 	 Heap Commit Size (4096): 0x00001000
 	      Loader flags (0x1): 0x00000000
 	   Data Directories (16): 0x00000010
 
 Data directories:
 	     Export Table: 0x00000000 [0x00000000]
-	     Import Table: 0x00003f60 [0x0000004b]
-	   Resource Table: 0x00004000 [0x00000338]
+	     Import Table: 0x00004098 [0x0000004f]
+	   Resource Table: 0x00006000 [0x000005dc]
 	  Exception Table: 0x00000000 [0x00000000]
 	Certificate Table: 0x00000000 [0x00000000]
-	      Reloc Table: 0x00006000 [0x0000000c]
-	            Debug: 0x00000000 [0x00000000]
+	      Reloc Table: 0x00008000 [0x0000000c]
+	            Debug: 0x00003f60 [0x0000001c]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x00001fb4
+	   Virtual Size: 0x000020f0
 	Virtual Address: 0x00002000
-	  Raw Data Size: 0x00002000
+	  Raw Data Size: 0x00002200
 	   Raw Data Ptr: 0x00000200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: code, exec, read, 
 
 	Name: .rsrc
-	   Virtual Size: 0x00000338
-	Virtual Address: 0x00004000
-	  Raw Data Size: 0x00000400
-	   Raw Data Ptr: 0x00002200
+	   Virtual Size: 0x000005dc
+	Virtual Address: 0x00006000
+	  Raw Data Size: 0x00000600
+	   Raw Data Ptr: 0x00002400
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, read, 
 
 	Name: .reloc
 	   Virtual Size: 0x0000000c
-	Virtual Address: 0x00006000
+	Virtual Address: 0x00008000
 	  Raw Data Size: 0x00000200
-	   Raw Data Ptr: 0x00002600
+	   Raw Data Ptr: 0x00002a00
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, discard, read, 
 
           CLI header size: 72
          Runtime required: 2.5
                     Flags: ilonly, 32bits, no-trackdebug, notsigned
-	         Metadata: 0x00002780 [0x000017e0]
-	Entry Point Token: 0x06000004
+	         Metadata: 0x000026f8 [0x00001868]
+	Entry Point Token: 0x06000003
 	     Resources at: 0x00000000 [0x00000000]
 	   Strong Name at: 0x00000000 [0x00000000]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
 Strong name: none
@@ -109,32 +109,32 @@
 Public key: none
 
 Metadata header:
            Version: 1.1
     Version string: v4.0.30319
 
 Metadata pointers:
-	Tables (#~): 0x0000006c - 0x00000690 [1572 == 0x00000624]
-	    Strings: 0x00000690 - 0x00000d7c [1772 == 0x000006ec]
-	       Blob: 0x000015f4 - 0x000017e0 [492 == 0x000001ec]
-	User string: 0x00000d7c - 0x000015e4 [2152 == 0x00000868]
-	       GUID: 0x000015e4 - 0x000015f4 [16 == 0x00000010]
+	Tables (#~): 0x0000006c - 0x000006ac [1600 == 0x00000640]
+	    Strings: 0x000006ac - 0x00000dd8 [1836 == 0x0000072c]
+	       Blob: 0x00001654 - 0x00001868 [532 == 0x00000214]
+	User string: 0x00000dd8 - 0x00001644 [2156 == 0x0000086c]
+	       GUID: 0x00001644 - 0x00001654 [16 == 0x00000010]
 Rows:
-Table Module: 1 records (10 bytes, at a4c)
-Table TypeRef: 46 records (6 bytes, at a56)
-Table TypeDef: 7 records (14 bytes, at b6a)
-Table Field: 16 records (6 bytes, at bcc)
-Table Method: 20 records (14 bytes, at c2c)
-Table Param: 11 records (6 bytes, at d44)
-Table InterfaceImpl: 1 records (4 bytes, at d86)
-Table MemberRef: 59 records (6 bytes, at d8a)
-Table CustomAttribute: 15 records (6 bytes, at eec)
-Table StandaloneSig: 5 records (2 bytes, at f46)
-Table PropertyMap: 1 records (4 bytes, at f50)
-Table Property: 1 records (6 bytes, at f54)
-Table MethodSemantics: 2 records (6 bytes, at f5a)
-Table TypeSpec: 3 records (2 bytes, at f66)
-Table Assembly: 1 records (22 bytes, at f6c)
-Table AssemblyRef: 6 records (20 bytes, at f82)
-Table NestedClass: 4 records (4 bytes, at ffa)
-Table MethodSpec: 1 records (4 bytes, at 100a)
-RVA for Entry Point: 0x00002254
+Table Module: 1 records (10 bytes, at 9c4)
+Table TypeRef: 48 records (6 bytes, at 9ce)
+Table TypeDef: 7 records (14 bytes, at aee)
+Table Field: 16 records (6 bytes, at b50)
+Table Method: 20 records (14 bytes, at bb0)
+Table Param: 11 records (6 bytes, at cc8)
+Table InterfaceImpl: 1 records (4 bytes, at d0a)
+Table MemberRef: 60 records (6 bytes, at d0e)
+Table CustomAttribute: 17 records (6 bytes, at e76)
+Table StandaloneSig: 4 records (2 bytes, at edc)
+Table PropertyMap: 1 records (4 bytes, at ee4)
+Table Property: 1 records (6 bytes, at ee8)
+Table MethodSemantics: 2 records (6 bytes, at eee)
+Table TypeSpec: 3 records (2 bytes, at efa)
+Table Assembly: 1 records (22 bytes, at f00)
+Table AssemblyRef: 6 records (20 bytes, at f16)
+Table NestedClass: 4 records (4 bytes, at f8e)
+Table MethodSpec: 1 records (4 bytes, at f9e)
+RVA for Entry Point: 0x00002238
```

### Comparing `bzt-1.9.5/bzt/resources/NUnitRunner/nunit-agent.exe` & `bzt-1.9.6/bzt/resources/NUnitRunner/nunit-agent.exe`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/resources/NUnitRunner/Newtonsoft.Json.dll` & `bzt-1.9.6/bzt/resources/NUnitRunner/Newtonsoft.Json.dll`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/resources/logback-worker.xml` & `bzt-1.9.6/bzt/resources/logback-worker.xml`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/resources/gatling_script.tpl` & `bzt-1.9.6/bzt/resources/gatling_script.tpl`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/resources/chrome-loader.c` & `bzt-1.9.6/bzt/resources/chrome-loader.c`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/resources/pbench.conf` & `bzt-1.9.6/bzt/resources/pbench.conf`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/__init__.py` & `bzt-1.9.6/bzt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import sys, platform
 from abc import abstractmethod
 
-VERSION = "1.9.5"
+VERSION = "1.9.6"
 
 
 class RCProvider(object):
     """
     Abstract return code provider
     """
```

### Comparing `bzt-1.9.5/bzt/requests_model.py` & `bzt-1.9.6/bzt/requests_model.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/bza.py` & `bzt-1.9.6/bzt/bza.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,20 +88,22 @@
         response = self.http_request(method=log_method, url=url, data=data, headers=headers, cookies=self._cookies,
                                      timeout=self.timeout)
 
         resp = response.content
         if not isinstance(resp, str):
             resp = resp.decode()
 
-        self.log.debug("Response: %s", resp[:self.logger_limit] if resp else None)
+        self.log.debug("Response [%s]: %s", response.status_code, resp[:self.logger_limit] if resp else None)
         if response.status_code >= 400:
             try:
                 result = json.loads(resp) if len(resp) else {}
                 if 'error' in result and result['error']:
                     raise TaurusNetworkError("API call error %s: %s" % (url, result['error']))
+                else:
+                    raise TaurusNetworkError("API call error %s on %s: %s" % (response.status_code, url, result))
             except ValueError:
                 raise TaurusNetworkError("API call error %s: %s %s" % (url, response.status_code, response.reason))
 
         if raw_result:
             return resp
 
         try:
@@ -401,16 +403,18 @@
         query = "cmd=rm&" + "&".join("targets[]=%s" % fname['hash'] for fname in files)
         url = self.address + path + '?' + query
         response = self._request(url)
         if len(response['removed']) == len(files):
             self.log.debug("Successfully deleted %d test files", len(response['removed']))
         return response['removed']
 
-    def start(self):
+    def start(self, as_functional=False):
         url = self.address + "/api/v4/tests/%s/start" % self['id']
+        if as_functional:
+            url += "?functionalExecution=true"
         resp = self._request(url, method='POST')
         master = Master(self, resp['result'])
         return master
 
     def upload_files(self, taurus_config, resource_files):
         self.log.debug("Uploading files into the test: %s", resource_files)
         url = '%s/api/v4/tests/%s/files' % (self.address, self['id'])
@@ -538,14 +542,22 @@
         url = self.address + "/api/v4/masters/%s/stop"
         self._request(url % self['id'], method='POST')
 
     def get_full(self):
         url = self.address + "/api/v4/masters/%s/full" % self['id']
         return self._request(url)['result']
 
+    def get_functional_report_groups(self):
+        url = self.address + "/api/v4/masters/%s/reports/functional/groups" % self['id']
+        return self._request(url)['result']
+
+    def get_functional_report_group(self, group_id):
+        url = self.address + "/api/v4/masters/%s/reports/functional/groups/%s" % (self['id'], group_id)
+        return self._request(url)['result']
+
 
 class Session(BZAObject):
     def __init__(self, proto=None, data=None):
         super(Session, self).__init__(proto, data)
         self.data_signature = None
         self.kpi_target = 'labels_bulk'
         self.monitoring_upload_notified = False
```

### Comparing `bzt-1.9.5/bzt/utils.py` & `bzt-1.9.6/bzt/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,15 +289,15 @@
             else:
                 if isinstance(rules.get(key), dict) and isinstance(self.get(key), BetterDict):
                     self.get(key).filter(rules[key])
                     if not self.get(key):  # clear empty
                         del self[key]
 
 
-def get_uniq_name(directory, prefix, suffix, forbidden_names=()):
+def get_uniq_name(directory, prefix, suffix="", forbidden_names=()):
     base = os.path.join(directory, prefix)
     diff = ""
     num = 0
     while os.path.exists(base + diff + suffix) or base + diff + suffix in forbidden_names:
         num += 1
         diff = "-%s" % num
```

### Comparing `bzt-1.9.5/bzt/jmx/__init__.py` & `bzt-1.9.6/bzt/jmx/__init__.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/jmx/base.py` & `bzt-1.9.6/bzt/jmx/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             self.load(original)
         else:
             root = etree.Element("jmeterTestPlan")
             self.tree = etree.ElementTree(root)
 
             test_plan = etree.Element("TestPlan", guiclass="TestPlanGui",
                                       testname=test_plan_name,
-                                      testclass="TestPlan")
+                                      testclass="TestPlan", enabled="true")
 
             htree = etree.Element("hashTree")
             htree.append(test_plan)
             htree.append(etree.Element("hashTree"))
             self.append("jmeterTestPlan", htree)
 
             element_prop = self._get_arguments_panel("TestPlan.user_defined_variables")
@@ -463,38 +463,45 @@
 
     @staticmethod
     def get_thread_group(concurrency=None, rampup=0, hold=0, iterations=None,
                          testname="ThreadGroup", on_error="continue"):
         """
         Generates ThreadGroup
 
-        :param concurrency:
-        :param rampup:
-        :param hold:
-        :param iterations:
-        :param testname:
-        :param on_error:
-        :return:
-        """
-        if not rampup:
-            rampup = 0
+        Expected values (by JMeter):
+            ThreadGroup.num_threads (concurrency): int
+            ThreadGroup.ramp_time (rampup): int
+            ThreadGroup.scheduler (need to hold): boolean
+            ThreadGroup.duration (rampup + hold): int
+            LoopController.loops (iterations): int
 
-        rampup = cond_int(rampup)
-        hold = cond_int(hold)
+        :return: etree element, ThreadGroup
+        """
+        rampup = cond_int(rampup or 0)
+        hold = cond_int(hold or 0)
 
         if not concurrency:
             concurrency = 1
 
         if not iterations:
             iterations = -1
 
         scheduler = False
         if hold or (rampup and not iterations):
             scheduler = True
 
+        if not hold:
+            duration = rampup
+        elif not rampup:
+            duration = hold
+        elif isinstance(rampup, numeric_types) and isinstance(hold, numeric_types):
+            duration = hold + rampup
+        else:
+            duration = "${__intSum(%s,%s)}" % (rampup, hold)
+
         trg = etree.Element("ThreadGroup", guiclass="ThreadGroupGui",
                             testclass="ThreadGroup", testname=testname)
         if on_error is not None:
             trg.append(JMX._string_prop("ThreadGroup.on_sample_error", on_error))
         loop = etree.Element("elementProp",
                              name="ThreadGroup.main_controller",
                              elementType="LoopController",
@@ -505,15 +512,15 @@
         trg.append(loop)
 
         trg.append(JMX._string_prop("ThreadGroup.num_threads", concurrency))
         trg.append(JMX._string_prop("ThreadGroup.ramp_time", rampup))
         trg.append(JMX._string_prop("ThreadGroup.start_time", ""))
         trg.append(JMX._string_prop("ThreadGroup.end_time", ""))
         trg.append(JMX._bool_prop("ThreadGroup.scheduler", scheduler))
-        trg.append(JMX._string_prop("ThreadGroup.duration", rampup + hold))
+        trg.append(JMX._string_prop("ThreadGroup.duration", duration))
 
         return trg
 
     def get_rps_shaper(self):
         """
 
         :return: etree.Element
@@ -528,19 +535,19 @@
         throughput_timer_element.append(shaper_load_prof)
 
         return throughput_timer_element
 
     def add_rps_shaper_schedule(self, shaper_etree, start_rps, end_rps, duration):
         """
         Adds schedule to rps shaper
-        :param shaper_etree:
-        :param start_rps:
-        :param end_rps:
-        :param duration:
-        :return:
+
+        Expected values (by JMeter):
+            <first> ('start_rps'): float
+            <second> ('end_rps'): float
+            <third> ('duration'): int
         """
         shaper_collection = shaper_etree.find(".//collectionProp[@name='load_profile']")
         coll_prop = self._collection_prop("1817389797")
         start_rps_prop = self._string_prop("49", cond_int(start_rps))
         end_rps_prop = self._string_prop("1567", cond_int(end_rps))
         duration_prop = self._string_prop("53", cond_int(duration))
         coll_prop.append(start_rps_prop)
@@ -575,14 +582,22 @@
         udv_element.append(udv_collection_prop)
         return udv_element
 
     @staticmethod
     def get_concurrency_thread_group(
             concurrency=None, rampup=0, hold=0, steps=None, on_error="continue", testname="ConcurrencyThreadGroup"):
         """
+        Generates ConcurrencyThreadGroup
+
+        Expected values (by JMeter):
+            Targetlevel (concurrency): int
+            RampUp (rampup): float
+            Steps (steps): boolean
+            Hold (hold): float
+
         :return: etree element, Concurrency Thread Group
         """
         if not rampup:
             rampup = 0
 
         if not concurrency:
             concurrency = 1
@@ -1039,14 +1054,23 @@
         controller = etree.Element("IfController", guiclass="IfControllerPanel", testclass="IfController",
                                    testname="If Controller")
         controller.append(JMX._string_prop("IfController.condition", condition))
         return controller
 
     @staticmethod
     def _get_loop_controller(loops):
+        """
+        Generates Loop Controller
+
+        Expected values(by JMeter):
+            LoopController.loops(iterations): int
+            LoopController.continue_forever: boolean
+
+        :return: etree element, LoopController
+        """
         if loops == 'forever':
             iterations = -1
         else:
             iterations = loops
         controller = etree.Element("LoopController", guiclass="LoopControlPanel", testclass="LoopController",
                                    testname="Loop Controller")
         controller.append(JMX._bool_prop("LoopController.continue_forever", False))  # always false except of root LC
```

### Comparing `bzt-1.9.5/bzt/jmx/tools.py` & `bzt-1.9.6/bzt/jmx/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import re
 import traceback
 
 from bzt import TaurusInternalException, TaurusConfigError
 from bzt.engine import Scenario
 from bzt.jmx import JMX
 from bzt.requests_model import RequestVisitor
-from bzt.six import etree, iteritems
+from bzt.six import etree, iteritems, numeric_types
 from bzt.utils import BetterDict, dehumanize_time, ensure_is_dict, get_host_ips, get_full_path, guess_csv_dialect
 
 
 class RequestCompiler(RequestVisitor):
     def __init__(self, jmx_builder):
         super(RequestCompiler, self).__init__()
         self.jmx_builder = jmx_builder
@@ -204,15 +204,15 @@
 
 class LoadSettingsProcessor(object):
     TG = ThreadGroup.__name__
     CTG = ConcurrencyThreadGroup.__name__
 
     def __init__(self, executor):
         self.log = executor.log.getChild(self.__class__.__name__)
-        self.load = executor.get_load()
+        self.load = executor.get_specific_load()
         self.tg = self._detect_thread_group(executor)
         self.tg_handler = ThreadGroupHandler(self.log)
 
     def _detect_thread_group(self, executor):
         """
         Detect preferred thread group
         :param executor:
@@ -241,18 +241,23 @@
     def modify(self, jmx):
         if not (self.load.iterations or self.load.concurrency or self.load.duration):
             self.log.debug('No iterations/concurrency/duration found, thread group modification is skipped')
             return
 
         # IMPORTANT: fix groups order as changing of element type changes order of getting of groups
         groups = list(self.tg_handler.groups(jmx))
-        target_list = zip(groups, self._get_concurrencies(groups))
 
-        for group, concurrency in target_list:
-            self.tg_handler.convert(group=group, target=self.tg, load=self.load, concurrency=concurrency)
+        if self.load.concurrency and not isinstance(self.load.concurrency, numeric_types):  # property found
+            for group in groups:
+                self.tg_handler.convert(group=group, target=self.tg, load=self.load, concurrency=self.load.concurrency)
+        else:
+            target_list = zip(groups, self._get_concurrencies(groups))
+
+            for group, concurrency in target_list:
+                self.tg_handler.convert(group=group, target=self.tg, load=self.load, concurrency=concurrency)
 
         if self.load.throughput:
             self._add_shaper(jmx)
 
         if self.load.steps and self.tg == self.TG:
             self.log.warning("Stepping ramp-up isn't supported for regular ThreadGroup")
 
@@ -699,22 +704,22 @@
         if not isinstance(sources, list):
             raise TaurusConfigError("data-sources '%s' is not a list" % sources)
         elements = []
         for idx, source in enumerate(sources):
             source = ensure_is_dict(sources, idx, "path")
             source_path = source["path"]
 
-            jmeter_var_pattern = re.compile("^\$\{.*\}$")
+            jmeter_var_pattern = re.compile("\${.+\}")
             delimiter = source.get('delimiter', None)
 
-            if jmeter_var_pattern.match(source_path):
-                self.log.warning('JMeter variable "%s" found, check of file existence is impossible', source_path)
+            if jmeter_var_pattern.search(source_path):
+                self.log.warning("Path to CSV contains JMeter variable/function, can't check for file existence: %s", source_path)
                 if not delimiter:
-                    self.log.warning('CSV dialect detection impossible, default delimiter selected (",")')
                     delimiter = ','
+                    self.log.warning("Can't detect CSV dialect, default delimiter will be '%s'", delimiter)
             else:
                 modified_path = self.executor.engine.find_file(source_path)
                 if not os.path.isfile(modified_path):
                     raise TaurusConfigError("data-sources path not found: %s" % modified_path)
                 if not delimiter:
                     delimiter = self.__guess_delimiter(modified_path)
                 source_path = get_full_path(modified_path)
```

### Comparing `bzt-1.9.5/bzt/engine.py` & `bzt-1.9.6/bzt/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 
     :type reporters: list[Reporter]
     :type services: list[Service]
     :type log: logging.Logger
     :type aggregator: bzt.modules.aggregator.ConsolidatingAggregator
     :type stopping_reason: BaseException
     """
+    ARTIFACTS_DIR = "%Y-%m-%d_%H-%M-%S.%f"
 
     def __init__(self, parent_logger):
         """
 
         :type parent_logger: logging.Logger
         """
         self.file_search_paths = []
@@ -329,16 +330,15 @@
             shutil.copy(filename, new_name)
 
     def create_artifacts_dir(self, existing_artifacts=(), merged_config=None):
         """
         Create directory for artifacts, directory name based on datetime.now()
         """
         if not self.artifacts_dir:
-            default = "%Y-%m-%d_%H-%M-%S.%f"
-            artifacts_dir = self.config.get(SETTINGS).get("artifacts-dir", default)
+            artifacts_dir = self.config.get(SETTINGS).get("artifacts-dir", self.ARTIFACTS_DIR)
             self.artifacts_dir = datetime.datetime.now().strftime(artifacts_dir)
 
         self.artifacts_dir = get_full_path(self.artifacts_dir)
 
         self.log.info("Artifacts dir: %s", self.artifacts_dir)
 
         if not os.path.isdir(self.artifacts_dir):
@@ -863,14 +863,15 @@
 
     RAMP_UP = "ramp-up"
     HOLD_FOR = "hold-for"
     CONCURR = "concurrency"
     THRPT = "throughput"
     EXEC = "execution"
     STEPS = "steps"
+    LOAD_FMT = namedtuple("LoadSpec", "concurrency throughput ramp_up hold iterations duration steps")
 
     def __init__(self):
         super(ScenarioExecutor, self).__init__()
         self.provisioning = None
         self.execution = BetterDict()
         self.__scenario = None
         self.label = None
@@ -982,20 +983,16 @@
             msg += "Invalid throughput value[%s]: %s " % (type(steps).__name__, steps)
         if not isinstance(iterations, numeric_types + (type(None),)):
             msg += "Invalid throughput value[%s]: %s " % (type(iterations).__name__, iterations)
 
         if msg:
             raise TaurusConfigError(msg)
 
-        res = namedtuple("LoadSpec",
-                         ('concurrency', "throughput", 'ramp_up', 'hold', 'iterations', 'duration', 'steps'))
-
-        return res(concurrency=concurrency, ramp_up=ramp_up,
-                   throughput=throughput, hold=hold, iterations=iterations,
-                   duration=duration, steps=steps)
+        return self.LOAD_FMT(concurrency=concurrency, ramp_up=ramp_up, throughput=throughput, hold=hold,
+                             iterations=iterations, duration=duration, steps=steps)
 
     def get_resource_files(self):
         files_list = []
         if isinstance(self, FileLister):
             files_list.extend(self.resource_files())
         files_list.extend(self.execution.get("files", []))
         return files_list
```

### Comparing `bzt-1.9.5/bzt/cli.py` & `bzt-1.9.6/bzt/cli.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/soapui2yaml.py` & `bzt-1.9.6/bzt/soapui2yaml.py`

 * *Files identical despite different names*

### Comparing `bzt-1.9.5/bzt/jmx2yaml.py` & `bzt-1.9.6/bzt/jmx2yaml.py`

 * *Files identical despite different names*

