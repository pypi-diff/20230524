# Comparing `tmp/soil-1.0.0rc8.tar.gz` & `tmp/soil-1.0.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soil-1.0.0rc8.tar", last modified: Mon May 22 16:31:11 2023, max compression
+gzip compressed data, was "soil-1.0.0rc9.tar", last modified: Mon May 22 18:25:57 2023, max compression
```

## Comparing `soil-1.0.0rc8.tar` & `soil-1.0.0rc9.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 16:31:11.080400 soil-1.0.0rc8/
--rw-r--r--   0 j         (1000) j         (1000)    11412 2018-12-07 19:26:39.000000 soil-1.0.0rc8/LICENSE
--rw-r--r--   0 j         (1000) j         (1000)      163 2020-03-11 15:11:50.000000 soil-1.0.0rc8/MANIFEST.in
--rw-rw-r--   0 j         (1000) j         (1000)     5739 2023-05-22 16:31:11.080400 soil-1.0.0rc8/PKG-INFO
--rw-rw-r--   0 j         (1000) j         (1000)     4655 2023-04-24 16:43:50.000000 soil-1.0.0rc8/README.md
--rw-rw-r--   0 j         (1000) j         (1000)      152 2023-05-16 09:54:11.000000 soil-1.0.0rc8/requirements.txt
--rw-rw-r--   0 j         (1000) j         (1000)      191 2023-05-22 16:31:11.080400 soil-1.0.0rc8/setup.cfg
--rw-rw-r--   0 j         (1000) j         (1000)     2211 2023-04-24 16:05:52.000000 soil-1.0.0rc8/setup.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 16:31:11.072400 soil-1.0.0rc8/soil/
--rw-rw-r--   0 j         (1000) j         (1000)      840 2023-05-22 07:43:59.000000 soil-1.0.0rc8/soil/.VERSION.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)      139 2023-04-14 19:48:55.000000 soil-1.0.0rc8/soil/.__init__.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    13297 2023-03-23 13:34:51.000000 soil-1.0.0rc8/soil/.analysis.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)     3720 2023-04-26 07:50:45.000000 soil-1.0.0rc8/soil/.datacollection.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)   102403 2023-05-18 08:01:44.000000 soil-1.0.0rc8/soil/.decorators.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)     2450 2023-05-17 21:10:06.000000 soil-1.0.0rc8/soil/.environment.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    13143 2023-04-25 22:09:53.000000 soil-1.0.0rc8/soil/.events.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)     2588 2023-04-14 20:43:29.000000 soil-1.0.0rc8/soil/.exporters.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)     1110 2023-04-14 21:29:51.000000 soil-1.0.0rc8/soil/.serialization.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    15937 2023-04-16 19:59:22.000000 soil-1.0.0rc8/soil/.simulation.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)     5011 2023-03-23 13:48:01.000000 soil-1.0.0rc8/soil/.stats.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    11233 2023-05-18 11:05:12.000000 soil-1.0.0rc8/soil/.time.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    32688 2023-04-21 14:21:10.000000 soil-1.0.0rc8/soil/.utils.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)      139 2023-04-04 13:46:42.000000 soil-1.0.0rc8/soil/.visualization.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)        8 2023-05-22 07:43:59.000000 soil-1.0.0rc8/soil/VERSION
--rw-rw-r--   0 j         (1000) j         (1000)     7865 2023-05-18 15:20:16.000000 soil-1.0.0rc8/soil/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)      107 2023-04-21 12:27:50.000000 soil-1.0.0rc8/soil/__main__.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 16:31:11.072400 soil-1.0.0rc8/soil/agents/
--rw-rw-r--   0 j         (1000) j         (1000)     7016 2023-05-22 07:37:15.000000 soil-1.0.0rc8/soil/agents/.__init__.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    59903 2023-04-25 23:21:25.000000 soil-1.0.0rc8/soil/agents/.evented.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)     6689 2023-05-18 07:39:51.000000 soil-1.0.0rc8/soil/agents/.fsm.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    21543 2023-05-18 10:56:12.000000 soil-1.0.0rc8/soil/agents/.meta.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)     5801 2023-04-25 03:00:06.000000 soil-1.0.0rc8/soil/agents/.network_agents.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)      734 2023-04-21 12:27:50.000000 soil-1.0.0rc8/soil/agents/BassModel.py
--rw-rw-r--   0 j         (1000) j         (1000)     1171 2023-04-21 12:27:50.000000 soil-1.0.0rc8/soil/agents/CounterModel.py
--rw-rw-r--   0 j         (1000) j         (1000)      766 2023-04-21 12:27:50.000000 soil-1.0.0rc8/soil/agents/IndependentCascadeModel.py
--rw-rw-r--   0 j         (1000) j         (1000)     3385 2023-04-21 12:27:50.000000 soil-1.0.0rc8/soil/agents/SISaModel.py
--rw-rw-r--   0 j         (1000) j         (1000)     6528 2023-05-22 09:39:27.000000 soil-1.0.0rc8/soil/agents/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)     1051 2023-05-19 08:38:34.000000 soil-1.0.0rc8/soil/agents/evented.py
--rw-rw-r--   0 j         (1000) j         (1000)     5815 2023-05-22 07:47:10.000000 soil-1.0.0rc8/soil/agents/fsm.py
--rw-rw-r--   0 j         (1000) j         (1000)      731 2023-04-29 09:53:33.000000 soil-1.0.0rc8/soil/agents/geo.py
--rw-rw-r--   0 j         (1000) j         (1000)     2121 2023-05-18 12:44:14.000000 soil-1.0.0rc8/soil/agents/meta.py
--rw-rw-r--   0 j         (1000) j         (1000)     3585 2023-05-10 16:19:55.000000 soil-1.0.0rc8/soil/agents/network_agents.py
--rw-rw-r--   0 j         (1000) j         (1000)     3751 2023-05-18 12:38:35.000000 soil-1.0.0rc8/soil/agents/view.py
--rw-rw-r--   0 j         (1000) j         (1000)     2205 2023-05-18 10:58:30.000000 soil-1.0.0rc8/soil/analysis.py
--rw-rw-r--   0 j         (1000) j         (1000)       36 2023-04-21 12:27:50.000000 soil-1.0.0rc8/soil/config.py
--rw-rw-r--   0 j         (1000) j         (1000)      853 2023-04-26 07:50:45.000000 soil-1.0.0rc8/soil/datacollection.py
--rw-rw-r--   0 j         (1000) j         (1000)     7217 2023-04-21 12:27:50.000000 soil-1.0.0rc8/soil/debugging.py
--rw-rw-r--   0 j         (1000) j         (1000)      989 2023-05-18 12:42:23.000000 soil-1.0.0rc8/soil/decorators.py
--rw-rw-r--   0 j         (1000) j         (1000)    19631 2023-05-19 14:04:51.000000 soil-1.0.0rc8/soil/environment.py
--rw-rw-r--   0 j         (1000) j         (1000)      626 2023-05-10 15:48:22.000000 soil-1.0.0rc8/soil/events.py
--rw-rw-r--   0 j         (1000) j         (1000)     9555 2023-05-18 14:06:19.000000 soil-1.0.0rc8/soil/exporters.py
--rw-rw-r--   0 j         (1000) j         (1000)     2149 2023-04-21 12:27:50.000000 soil-1.0.0rc8/soil/network.py
--rw-rw-r--   0 j         (1000) j         (1000)      739 2023-04-21 12:27:50.000000 soil-1.0.0rc8/soil/parameters.py
--rw-rw-r--   0 j         (1000) j         (1000)     8070 2023-04-29 09:32:04.000000 soil-1.0.0rc8/soil/serialization.py
--rw-r--r--   0 j         (1000) j         (1000)       24 2018-12-07 19:26:39.000000 soil-1.0.0rc8/soil/settings.py
--rw-rw-r--   0 j         (1000) j         (1000)    13135 2023-05-18 15:20:04.000000 soil-1.0.0rc8/soil/simulation.py
--rw-rw-r--   0 j         (1000) j         (1000)     8089 2023-05-18 16:17:24.000000 soil-1.0.0rc8/soil/time.py
--rw-rw-r--   0 j         (1000) j         (1000)     4783 2023-05-18 10:58:56.000000 soil-1.0.0rc8/soil/utils.py
--rw-rw-r--   0 j         (1000) j         (1000)      476 2023-04-21 12:27:50.000000 soil-1.0.0rc8/soil/version.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 16:31:11.076400 soil-1.0.0rc8/soil/web/
--rw-r--r--   0 j         (1000) j         (1000)       41 2018-12-08 17:08:24.000000 soil-1.0.0rc8/soil/web/.gitignore
--rw-r--r--   0 j         (1000) j         (1000)     2984 2018-12-08 17:08:24.000000 soil-1.0.0rc8/soil/web/README.md
--rw-rw-r--   0 j         (1000) j         (1000)    11272 2023-04-21 12:27:50.000000 soil-1.0.0rc8/soil/web/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)       59 2023-04-21 12:27:50.000000 soil-1.0.0rc8/soil/web/__main__.py
--rw-rw-r--   0 j         (1000) j         (1000)      575 2023-04-21 12:27:50.000000 soil-1.0.0rc8/soil/web/config.yml
--rw-rw-r--   0 j         (1000) j         (1000)     1073 2023-04-21 12:27:50.000000 soil-1.0.0rc8/soil/web/run.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 16:31:11.060401 soil-1.0.0rc8/soil/web/static/
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 16:31:11.076400 soil-1.0.0rc8/soil/web/static/css/
--rw-r--r--   0 j         (1000) j         (1000)     7157 2018-12-08 17:08:24.000000 soil-1.0.0rc8/soil/web/static/css/main.css
--rw-r--r--   0 j         (1000) j         (1000)     1107 2018-12-08 17:08:24.000000 soil-1.0.0rc8/soil/web/static/css/timeline.css
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 16:31:11.076400 soil-1.0.0rc8/soil/web/static/img/
--rw-r--r--   0 j         (1000) j         (1000)    18053 2018-12-08 17:08:25.000000 soil-1.0.0rc8/soil/web/static/img/logo_gsi.svg
--rw-r--r--   0 j         (1000) j         (1000)   103744 2018-12-08 17:08:25.000000 soil-1.0.0rc8/soil/web/static/img/logo_soil.png
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 16:31:11.076400 soil-1.0.0rc8/soil/web/static/img/svg/
--rw-r--r--   0 j         (1000) j         (1000)      462 2018-12-08 17:08:25.000000 soil-1.0.0rc8/soil/web/static/img/svg/home.svg
--rw-r--r--   0 j         (1000) j         (1000)      812 2018-12-08 17:08:25.000000 soil-1.0.0rc8/soil/web/static/img/svg/person.svg
--rw-r--r--   0 j         (1000) j         (1000)      697 2018-12-08 17:08:25.000000 soil-1.0.0rc8/soil/web/static/img/svg/plus.svg
--rw-r--r--   0 j         (1000) j         (1000)      992 2018-12-08 17:08:25.000000 soil-1.0.0rc8/soil/web/static/img/svg/target.svg
--rw-r--r--   0 j         (1000) j         (1000)     1561 2018-12-08 17:08:25.000000 soil-1.0.0rc8/soil/web/static/img/svg/time.svg
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 16:31:11.076400 soil-1.0.0rc8/soil/web/static/js/
--rwxr-xr-x   0 j         (1000) j         (1000)    16528 2018-12-08 17:08:25.000000 soil-1.0.0rc8/soil/web/static/js/socket.js
--rw-r--r--   0 j         (1000) j         (1000)     5040 2018-12-08 17:08:25.000000 soil-1.0.0rc8/soil/web/static/js/template.js
--rw-r--r--   0 j         (1000) j         (1000)    12269 2018-12-08 17:08:25.000000 soil-1.0.0rc8/soil/web/static/js/timeline.js
--rw-r--r--   0 j         (1000) j         (1000)    21818 2018-12-08 17:08:25.000000 soil-1.0.0rc8/soil/web/static/js/visualization.js
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 16:31:11.076400 soil-1.0.0rc8/soil/web/templates/
--rw-r--r--   0 j         (1000) j         (1000)    16450 2018-12-08 17:08:25.000000 soil-1.0.0rc8/soil/web/templates/index.html
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 16:31:11.072400 soil-1.0.0rc8/soil.egg-info/
--rw-r--r--   0 j         (1000) j         (1000)     5739 2023-05-22 16:31:11.000000 soil-1.0.0rc8/soil.egg-info/PKG-INFO
--rw-r--r--   0 j         (1000) j         (1000)     2228 2023-05-22 16:31:11.000000 soil-1.0.0rc8/soil.egg-info/SOURCES.txt
--rw-r--r--   0 j         (1000) j         (1000)        1 2023-05-22 16:31:11.000000 soil-1.0.0rc8/soil.egg-info/dependency_links.txt
--rw-r--r--   0 j         (1000) j         (1000)       78 2023-05-22 16:31:11.000000 soil-1.0.0rc8/soil.egg-info/entry_points.txt
--rw-r--r--   0 j         (1000) j         (1000)      278 2023-05-22 16:31:11.000000 soil-1.0.0rc8/soil.egg-info/requires.txt
--rw-r--r--   0 j         (1000) j         (1000)        5 2023-05-22 16:31:11.000000 soil-1.0.0rc8/soil.egg-info/top_level.txt
--rw-rw-r--   0 j         (1000) j         (1000)       90 2023-04-24 17:04:44.000000 soil-1.0.0rc8/test-requirements.txt
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 16:31:11.080400 soil-1.0.0rc8/tests/
--rw-rw-r--   0 j         (1000) j         (1000)    16405 2023-05-19 14:08:32.000000 soil-1.0.0rc8/tests/test_agents.py
--rw-rw-r--   0 j         (1000) j         (1000)     2231 2023-04-25 13:22:59.000000 soil-1.0.0rc8/tests/test_config.py
--rw-rw-r--   0 j         (1000) j         (1000)     2450 2023-04-21 12:27:50.000000 soil-1.0.0rc8/tests/test_examples.py
--rw-rw-r--   0 j         (1000) j         (1000)     3792 2023-05-04 14:58:41.000000 soil-1.0.0rc8/tests/test_exporters.py
--rw-rw-r--   0 j         (1000) j         (1000)      636 2023-04-24 16:55:59.000000 soil-1.0.0rc8/tests/test_ipython.py
--rw-rw-r--   0 j         (1000) j         (1000)     9540 2023-05-18 12:37:14.000000 soil-1.0.0rc8/tests/test_main.py
--rw-rw-r--   0 j         (1000) j         (1000)     1940 2023-04-21 12:27:50.000000 soil-1.0.0rc8/tests/test_mesa.py
--rw-rw-r--   0 j         (1000) j         (1000)     3133 2023-04-21 12:27:50.000000 soil-1.0.0rc8/tests/test_network.py
--rw-rw-r--   0 j         (1000) j         (1000)     1549 2023-05-02 15:39:46.000000 soil-1.0.0rc8/tests/test_time.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 18:25:57.350873 soil-1.0.0rc9/
+-rw-r--r--   0 j         (1000) j         (1000)    11412 2018-12-07 19:26:39.000000 soil-1.0.0rc9/LICENSE
+-rw-r--r--   0 j         (1000) j         (1000)      163 2020-03-11 15:11:50.000000 soil-1.0.0rc9/MANIFEST.in
+-rw-rw-r--   0 j         (1000) j         (1000)     5739 2023-05-22 18:25:57.350873 soil-1.0.0rc9/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)     4655 2023-04-24 16:43:50.000000 soil-1.0.0rc9/README.md
+-rw-rw-r--   0 j         (1000) j         (1000)      152 2023-05-16 09:54:11.000000 soil-1.0.0rc9/requirements.txt
+-rw-rw-r--   0 j         (1000) j         (1000)      191 2023-05-22 18:25:57.354873 soil-1.0.0rc9/setup.cfg
+-rw-rw-r--   0 j         (1000) j         (1000)     2211 2023-04-24 16:05:52.000000 soil-1.0.0rc9/setup.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 18:25:57.346873 soil-1.0.0rc9/soil/
+-rw-rw-r--   0 j         (1000) j         (1000)      840 2023-05-22 07:43:59.000000 soil-1.0.0rc9/soil/.VERSION.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)      139 2023-04-14 19:48:55.000000 soil-1.0.0rc9/soil/.__init__.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    13297 2023-03-23 13:34:51.000000 soil-1.0.0rc9/soil/.analysis.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     3720 2023-04-26 07:50:45.000000 soil-1.0.0rc9/soil/.datacollection.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)   102403 2023-05-18 08:01:44.000000 soil-1.0.0rc9/soil/.decorators.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     2450 2023-05-17 21:10:06.000000 soil-1.0.0rc9/soil/.environment.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    13143 2023-04-25 22:09:53.000000 soil-1.0.0rc9/soil/.events.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     2588 2023-04-14 20:43:29.000000 soil-1.0.0rc9/soil/.exporters.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     1110 2023-04-14 21:29:51.000000 soil-1.0.0rc9/soil/.serialization.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    15937 2023-04-16 19:59:22.000000 soil-1.0.0rc9/soil/.simulation.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     5011 2023-03-23 13:48:01.000000 soil-1.0.0rc9/soil/.stats.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    11233 2023-05-18 11:05:12.000000 soil-1.0.0rc9/soil/.time.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    32688 2023-04-21 14:21:10.000000 soil-1.0.0rc9/soil/.utils.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)      139 2023-04-04 13:46:42.000000 soil-1.0.0rc9/soil/.visualization.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)        8 2023-05-22 17:43:46.000000 soil-1.0.0rc9/soil/VERSION
+-rw-rw-r--   0 j         (1000) j         (1000)     7865 2023-05-18 15:20:16.000000 soil-1.0.0rc9/soil/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)      107 2023-04-21 12:27:50.000000 soil-1.0.0rc9/soil/__main__.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 18:25:57.346873 soil-1.0.0rc9/soil/agents/
+-rw-rw-r--   0 j         (1000) j         (1000)     7016 2023-05-22 07:37:15.000000 soil-1.0.0rc9/soil/agents/.__init__.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    59903 2023-04-25 23:21:25.000000 soil-1.0.0rc9/soil/agents/.evented.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     6689 2023-05-18 07:39:51.000000 soil-1.0.0rc9/soil/agents/.fsm.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    21543 2023-05-18 10:56:12.000000 soil-1.0.0rc9/soil/agents/.meta.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     5801 2023-04-25 03:00:06.000000 soil-1.0.0rc9/soil/agents/.network_agents.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)      734 2023-04-21 12:27:50.000000 soil-1.0.0rc9/soil/agents/BassModel.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1171 2023-04-21 12:27:50.000000 soil-1.0.0rc9/soil/agents/CounterModel.py
+-rw-rw-r--   0 j         (1000) j         (1000)      766 2023-04-21 12:27:50.000000 soil-1.0.0rc9/soil/agents/IndependentCascadeModel.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3385 2023-04-21 12:27:50.000000 soil-1.0.0rc9/soil/agents/SISaModel.py
+-rw-rw-r--   0 j         (1000) j         (1000)     6528 2023-05-22 09:39:27.000000 soil-1.0.0rc9/soil/agents/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1051 2023-05-19 08:38:34.000000 soil-1.0.0rc9/soil/agents/evented.py
+-rw-rw-r--   0 j         (1000) j         (1000)     5815 2023-05-22 07:47:10.000000 soil-1.0.0rc9/soil/agents/fsm.py
+-rw-rw-r--   0 j         (1000) j         (1000)      731 2023-04-29 09:53:33.000000 soil-1.0.0rc9/soil/agents/geo.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2121 2023-05-18 12:44:14.000000 soil-1.0.0rc9/soil/agents/meta.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3585 2023-05-10 16:19:55.000000 soil-1.0.0rc9/soil/agents/network_agents.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3751 2023-05-18 12:38:35.000000 soil-1.0.0rc9/soil/agents/view.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2205 2023-05-18 10:58:30.000000 soil-1.0.0rc9/soil/analysis.py
+-rw-rw-r--   0 j         (1000) j         (1000)       36 2023-04-21 12:27:50.000000 soil-1.0.0rc9/soil/config.py
+-rw-rw-r--   0 j         (1000) j         (1000)      853 2023-04-26 07:50:45.000000 soil-1.0.0rc9/soil/datacollection.py
+-rw-rw-r--   0 j         (1000) j         (1000)     7217 2023-04-21 12:27:50.000000 soil-1.0.0rc9/soil/debugging.py
+-rw-rw-r--   0 j         (1000) j         (1000)      989 2023-05-18 12:42:23.000000 soil-1.0.0rc9/soil/decorators.py
+-rw-rw-r--   0 j         (1000) j         (1000)    20191 2023-05-22 18:22:18.000000 soil-1.0.0rc9/soil/environment.py
+-rw-rw-r--   0 j         (1000) j         (1000)      626 2023-05-10 15:48:22.000000 soil-1.0.0rc9/soil/events.py
+-rw-rw-r--   0 j         (1000) j         (1000)     9555 2023-05-18 14:06:19.000000 soil-1.0.0rc9/soil/exporters.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2149 2023-04-21 12:27:50.000000 soil-1.0.0rc9/soil/network.py
+-rw-rw-r--   0 j         (1000) j         (1000)      739 2023-04-21 12:27:50.000000 soil-1.0.0rc9/soil/parameters.py
+-rw-rw-r--   0 j         (1000) j         (1000)     8070 2023-04-29 09:32:04.000000 soil-1.0.0rc9/soil/serialization.py
+-rw-r--r--   0 j         (1000) j         (1000)       24 2018-12-07 19:26:39.000000 soil-1.0.0rc9/soil/settings.py
+-rw-rw-r--   0 j         (1000) j         (1000)    13135 2023-05-18 15:20:04.000000 soil-1.0.0rc9/soil/simulation.py
+-rw-rw-r--   0 j         (1000) j         (1000)     8130 2023-05-22 17:40:58.000000 soil-1.0.0rc9/soil/time.py
+-rw-rw-r--   0 j         (1000) j         (1000)     4783 2023-05-18 10:58:56.000000 soil-1.0.0rc9/soil/utils.py
+-rw-rw-r--   0 j         (1000) j         (1000)      476 2023-04-21 12:27:50.000000 soil-1.0.0rc9/soil/version.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 18:25:57.350873 soil-1.0.0rc9/soil/web/
+-rw-r--r--   0 j         (1000) j         (1000)       41 2018-12-08 17:08:24.000000 soil-1.0.0rc9/soil/web/.gitignore
+-rw-r--r--   0 j         (1000) j         (1000)     2984 2018-12-08 17:08:24.000000 soil-1.0.0rc9/soil/web/README.md
+-rw-rw-r--   0 j         (1000) j         (1000)    11272 2023-04-21 12:27:50.000000 soil-1.0.0rc9/soil/web/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)       59 2023-04-21 12:27:50.000000 soil-1.0.0rc9/soil/web/__main__.py
+-rw-rw-r--   0 j         (1000) j         (1000)      575 2023-04-21 12:27:50.000000 soil-1.0.0rc9/soil/web/config.yml
+-rw-rw-r--   0 j         (1000) j         (1000)     1073 2023-04-21 12:27:50.000000 soil-1.0.0rc9/soil/web/run.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 18:25:57.338873 soil-1.0.0rc9/soil/web/static/
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 18:25:57.350873 soil-1.0.0rc9/soil/web/static/css/
+-rw-r--r--   0 j         (1000) j         (1000)     7157 2018-12-08 17:08:24.000000 soil-1.0.0rc9/soil/web/static/css/main.css
+-rw-r--r--   0 j         (1000) j         (1000)     1107 2018-12-08 17:08:24.000000 soil-1.0.0rc9/soil/web/static/css/timeline.css
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 18:25:57.350873 soil-1.0.0rc9/soil/web/static/img/
+-rw-r--r--   0 j         (1000) j         (1000)    18053 2018-12-08 17:08:25.000000 soil-1.0.0rc9/soil/web/static/img/logo_gsi.svg
+-rw-r--r--   0 j         (1000) j         (1000)   103744 2018-12-08 17:08:25.000000 soil-1.0.0rc9/soil/web/static/img/logo_soil.png
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 18:25:57.350873 soil-1.0.0rc9/soil/web/static/img/svg/
+-rw-r--r--   0 j         (1000) j         (1000)      462 2018-12-08 17:08:25.000000 soil-1.0.0rc9/soil/web/static/img/svg/home.svg
+-rw-r--r--   0 j         (1000) j         (1000)      812 2018-12-08 17:08:25.000000 soil-1.0.0rc9/soil/web/static/img/svg/person.svg
+-rw-r--r--   0 j         (1000) j         (1000)      697 2018-12-08 17:08:25.000000 soil-1.0.0rc9/soil/web/static/img/svg/plus.svg
+-rw-r--r--   0 j         (1000) j         (1000)      992 2018-12-08 17:08:25.000000 soil-1.0.0rc9/soil/web/static/img/svg/target.svg
+-rw-r--r--   0 j         (1000) j         (1000)     1561 2018-12-08 17:08:25.000000 soil-1.0.0rc9/soil/web/static/img/svg/time.svg
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 18:25:57.350873 soil-1.0.0rc9/soil/web/static/js/
+-rwxr-xr-x   0 j         (1000) j         (1000)    16528 2018-12-08 17:08:25.000000 soil-1.0.0rc9/soil/web/static/js/socket.js
+-rw-r--r--   0 j         (1000) j         (1000)     5040 2018-12-08 17:08:25.000000 soil-1.0.0rc9/soil/web/static/js/template.js
+-rw-r--r--   0 j         (1000) j         (1000)    12269 2018-12-08 17:08:25.000000 soil-1.0.0rc9/soil/web/static/js/timeline.js
+-rw-r--r--   0 j         (1000) j         (1000)    21818 2018-12-08 17:08:25.000000 soil-1.0.0rc9/soil/web/static/js/visualization.js
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 18:25:57.350873 soil-1.0.0rc9/soil/web/templates/
+-rw-r--r--   0 j         (1000) j         (1000)    16450 2018-12-08 17:08:25.000000 soil-1.0.0rc9/soil/web/templates/index.html
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 18:25:57.346873 soil-1.0.0rc9/soil.egg-info/
+-rw-r--r--   0 j         (1000) j         (1000)     5739 2023-05-22 18:25:57.000000 soil-1.0.0rc9/soil.egg-info/PKG-INFO
+-rw-r--r--   0 j         (1000) j         (1000)     2228 2023-05-22 18:25:57.000000 soil-1.0.0rc9/soil.egg-info/SOURCES.txt
+-rw-r--r--   0 j         (1000) j         (1000)        1 2023-05-22 18:25:57.000000 soil-1.0.0rc9/soil.egg-info/dependency_links.txt
+-rw-r--r--   0 j         (1000) j         (1000)       78 2023-05-22 18:25:57.000000 soil-1.0.0rc9/soil.egg-info/entry_points.txt
+-rw-r--r--   0 j         (1000) j         (1000)      278 2023-05-22 18:25:57.000000 soil-1.0.0rc9/soil.egg-info/requires.txt
+-rw-r--r--   0 j         (1000) j         (1000)        5 2023-05-22 18:25:57.000000 soil-1.0.0rc9/soil.egg-info/top_level.txt
+-rw-rw-r--   0 j         (1000) j         (1000)       90 2023-04-24 17:04:44.000000 soil-1.0.0rc9/test-requirements.txt
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-22 18:25:57.350873 soil-1.0.0rc9/tests/
+-rw-rw-r--   0 j         (1000) j         (1000)    16405 2023-05-19 14:08:32.000000 soil-1.0.0rc9/tests/test_agents.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2231 2023-04-25 13:22:59.000000 soil-1.0.0rc9/tests/test_config.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2450 2023-04-21 12:27:50.000000 soil-1.0.0rc9/tests/test_examples.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3792 2023-05-04 14:58:41.000000 soil-1.0.0rc9/tests/test_exporters.py
+-rw-rw-r--   0 j         (1000) j         (1000)      636 2023-04-24 16:55:59.000000 soil-1.0.0rc9/tests/test_ipython.py
+-rw-rw-r--   0 j         (1000) j         (1000)     9540 2023-05-18 12:37:14.000000 soil-1.0.0rc9/tests/test_main.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1940 2023-04-21 12:27:50.000000 soil-1.0.0rc9/tests/test_mesa.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3133 2023-04-21 12:27:50.000000 soil-1.0.0rc9/tests/test_network.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1549 2023-05-02 15:39:46.000000 soil-1.0.0rc9/tests/test_time.py
```

### Comparing `soil-1.0.0rc8/LICENSE` & `soil-1.0.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/PKG-INFO` & `soil-1.0.0rc9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: soil
-Version: 1.0.0rc8
+Version: 1.0.0rc9
 Summary: An Agent-Based Social Simulator for Social Networks
 Home-page: https://github.com/gsi-upm/soil
-Download-URL: https://github.com/gsi-upm/soil/archive/1.0.0rc8.tar.gz
+Download-URL: https://github.com/gsi-upm/soil/archive/1.0.0rc9.tar.gz
 Author: J. Fernando Sanchez
 Author-email: jf.sanchez@upm.es
 Keywords: agent,social,simulator
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `soil-1.0.0rc8/README.md` & `soil-1.0.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/setup.py` & `soil-1.0.0rc9/setup.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/.VERSION.~undo-tree~` & `soil-1.0.0rc9/soil/.VERSION.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/.analysis.py.~undo-tree~` & `soil-1.0.0rc9/soil/.analysis.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/.datacollection.py.~undo-tree~` & `soil-1.0.0rc9/soil/.datacollection.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/.decorators.py.~undo-tree~` & `soil-1.0.0rc9/soil/.decorators.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/.environment.py.~undo-tree~` & `soil-1.0.0rc9/soil/.environment.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/.events.py.~undo-tree~` & `soil-1.0.0rc9/soil/.events.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/.exporters.py.~undo-tree~` & `soil-1.0.0rc9/soil/.exporters.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/.serialization.py.~undo-tree~` & `soil-1.0.0rc9/soil/.serialization.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/.simulation.py.~undo-tree~` & `soil-1.0.0rc9/soil/.simulation.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/.stats.py.~undo-tree~` & `soil-1.0.0rc9/soil/.stats.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/.time.py.~undo-tree~` & `soil-1.0.0rc9/soil/.time.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/.utils.py.~undo-tree~` & `soil-1.0.0rc9/soil/.utils.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/__init__.py` & `soil-1.0.0rc9/soil/__init__.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/agents/.__init__.py.~undo-tree~` & `soil-1.0.0rc9/soil/agents/.__init__.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/agents/.evented.py.~undo-tree~` & `soil-1.0.0rc9/soil/agents/.evented.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/agents/.fsm.py.~undo-tree~` & `soil-1.0.0rc9/soil/agents/.fsm.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/agents/.meta.py.~undo-tree~` & `soil-1.0.0rc9/soil/agents/.meta.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/agents/.network_agents.py.~undo-tree~` & `soil-1.0.0rc9/soil/agents/.network_agents.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/agents/BassModel.py` & `soil-1.0.0rc9/soil/agents/BassModel.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/agents/CounterModel.py` & `soil-1.0.0rc9/soil/agents/CounterModel.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/agents/IndependentCascadeModel.py` & `soil-1.0.0rc9/soil/agents/IndependentCascadeModel.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/agents/SISaModel.py` & `soil-1.0.0rc9/soil/agents/SISaModel.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/agents/__init__.py` & `soil-1.0.0rc9/soil/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/agents/evented.py` & `soil-1.0.0rc9/soil/agents/evented.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/agents/fsm.py` & `soil-1.0.0rc9/soil/agents/fsm.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/agents/geo.py` & `soil-1.0.0rc9/soil/agents/geo.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/agents/meta.py` & `soil-1.0.0rc9/soil/agents/meta.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/agents/network_agents.py` & `soil-1.0.0rc9/soil/agents/network_agents.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/agents/view.py` & `soil-1.0.0rc9/soil/agents/view.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/analysis.py` & `soil-1.0.0rc9/soil/analysis.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/datacollection.py` & `soil-1.0.0rc9/soil/datacollection.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/debugging.py` & `soil-1.0.0rc9/soil/debugging.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/decorators.py` & `soil-1.0.0rc9/soil/decorators.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/environment.py` & `soil-1.0.0rc9/soil/environment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import os
 import sys
 import logging
+from datetime import datetime
 
 from typing import Any, Callable, Dict, Optional, Union, List, Type
 from types import coroutine
 
 import networkx as nx
 
 
@@ -29,14 +30,16 @@
     The environment parameters and the state of every agent can be accessed
     both by using the environment as a dictionary and with the environment's
     :meth:`soil.environment.Environment.get` method.
     """
 
     collector_class = datacollection.SoilCollector
     schedule_class = time.TimedActivation
+    start_time = 0
+    time_format = "%Y-%m-%d %H:%M:%S"
 
     def __new__(cls,
                 *args: Any,
                 seed="default",
                 dir_path=None,
                 collector_class: type = None,
                 agent_reporters: Optional[Any] = None,
@@ -71,14 +74,16 @@
         schedule=None,
         schedule_class=None,
         logger = None,
         agents: Optional[Dict] = None,
         collector_class: type = datacollection.SoilCollector,
         agent_reporters: Optional[Any] = None,
         model_reporters: Optional[Any] = None,
+        start_time=None,
+        time_format=None,
         tables: Optional[Any] = None,
         init: bool = True,
         **env_params,
     ):
 
         super().__init__()
 
@@ -87,20 +92,29 @@
 
         self.id = id
 
         if logger:
             self.logger = logger
         else:
             self.logger = utils.logger.getChild(self.id)
+        if start_time is not None:
+            self.start_time = start_time
+        if time_format is not None:
+            self.time_format = time_format
+
+        if isinstance(self.start_time, str):
+            self.start_time = datetime.strptime(self.start_time, self.time_format)
+        if isinstance(self.start_time, datetime):
+            self.start_time = datetime.timestamp(self.start_time)
 
         self.schedule = schedule
         if schedule is None:
             if schedule_class is None:
                 schedule_class = self.schedule_class
-            self.schedule = schedule_class(self)
+            self.schedule = schedule_class(self, time=self.start_time)
 
         for (k, v) in env_params.items():
             self[k] = v
 
         if agents:
             self.add_agents(**agents)
         if init:
```

### Comparing `soil-1.0.0rc8/soil/events.py` & `soil-1.0.0rc9/soil/events.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/exporters.py` & `soil-1.0.0rc9/soil/exporters.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/network.py` & `soil-1.0.0rc9/soil/network.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/parameters.py` & `soil-1.0.0rc9/soil/parameters.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/serialization.py` & `soil-1.0.0rc9/soil/serialization.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/simulation.py` & `soil-1.0.0rc9/soil/simulation.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/time.py` & `soil-1.0.0rc9/soil/time.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,18 +58,18 @@
 
 class PQueueSchedule:
     """
     A scheduler which activates each function with a delay returned by the function at each step.
     If no delay is returned, a default of 1 is used.
     """
 
-    def __init__(self, shuffle=True, seed=None, **kwargs):
+    def __init__(self, shuffle=True, seed=None, time=0, **kwargs):
         self._queue = []
         self._shuffle = shuffle
-        self.time = 0
+        self.time = time
         self.steps = 0
         self.random = random_std.Random(seed)
         self.next_time = self.time
 
     def insert(self, when, callback, replace=False):
         if when is None:
             when = self.time
@@ -130,18 +130,18 @@
 
         if next_time == INFINITY:
             self.time = INFINITY
             return
 
 
 class Schedule:
-    def __init__(self, shuffle=True, seed=None, **kwargs):
+    def __init__(self, shuffle=True, seed=None, time=0, **kwargs):
         self._queue = deque()
         self._shuffle = shuffle
-        self.time = 0
+        self.time = time
         self.steps = 0
         self.random = random_std.Random(seed)
         self.next_time = self.time
 
     def _find_loc(self, when=None):
         if when is None:
             when = self.time
@@ -222,20 +222,20 @@
         else:
             self.time = INFINITY
 
 
 class InnerActivation(BaseScheduler):
     inner_class = Schedule
 
-    def __init__(self, model, shuffle=True, **kwargs):
+    def __init__(self, model, shuffle=True, time=0, **kwargs):
         self.model = model
         self.logger = getattr(self.model, "logger", logger).getChild(f"time_{ self.model }")
         self._agents = {}
         self.agents_by_type = defaultdict(dict)
-        self.inner = self.inner_class(shuffle=shuffle, seed=self.model._seed)
+        self.inner = self.inner_class(shuffle=shuffle, seed=self.model._seed, time=time)
 
     @property
     def steps(self):
         return self.inner.steps
 
     @property
     def time(self):
```

### Comparing `soil-1.0.0rc8/soil/utils.py` & `soil-1.0.0rc9/soil/utils.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/web/README.md` & `soil-1.0.0rc9/soil/web/README.md`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/web/__init__.py` & `soil-1.0.0rc9/soil/web/__init__.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/web/config.yml` & `soil-1.0.0rc9/soil/web/config.yml`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/web/run.py` & `soil-1.0.0rc9/soil/web/run.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/web/static/css/main.css` & `soil-1.0.0rc9/soil/web/static/css/main.css`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/web/static/css/timeline.css` & `soil-1.0.0rc9/soil/web/static/css/timeline.css`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/web/static/img/logo_gsi.svg` & `soil-1.0.0rc9/soil/web/static/img/logo_gsi.svg`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/web/static/img/logo_soil.png` & `soil-1.0.0rc9/soil/web/static/img/logo_soil.png`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/web/static/img/svg/person.svg` & `soil-1.0.0rc9/soil/web/static/img/svg/person.svg`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/web/static/img/svg/plus.svg` & `soil-1.0.0rc9/soil/web/static/img/svg/plus.svg`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/web/static/img/svg/target.svg` & `soil-1.0.0rc9/soil/web/static/img/svg/target.svg`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/web/static/img/svg/time.svg` & `soil-1.0.0rc9/soil/web/static/img/svg/time.svg`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/web/static/js/socket.js` & `soil-1.0.0rc9/soil/web/static/js/socket.js`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/web/static/js/template.js` & `soil-1.0.0rc9/soil/web/static/js/template.js`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/web/static/js/timeline.js` & `soil-1.0.0rc9/soil/web/static/js/timeline.js`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/web/static/js/visualization.js` & `soil-1.0.0rc9/soil/web/static/js/visualization.js`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil/web/templates/index.html` & `soil-1.0.0rc9/soil/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/soil.egg-info/PKG-INFO` & `soil-1.0.0rc9/soil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: soil
-Version: 1.0.0rc8
+Version: 1.0.0rc9
 Summary: An Agent-Based Social Simulator for Social Networks
 Home-page: https://github.com/gsi-upm/soil
-Download-URL: https://github.com/gsi-upm/soil/archive/1.0.0rc8.tar.gz
+Download-URL: https://github.com/gsi-upm/soil/archive/1.0.0rc9.tar.gz
 Author: J. Fernando Sanchez
 Author-email: jf.sanchez@upm.es
 Keywords: agent,social,simulator
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `soil-1.0.0rc8/soil.egg-info/SOURCES.txt` & `soil-1.0.0rc9/soil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/tests/test_agents.py` & `soil-1.0.0rc9/tests/test_agents.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/tests/test_config.py` & `soil-1.0.0rc9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/tests/test_examples.py` & `soil-1.0.0rc9/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/tests/test_exporters.py` & `soil-1.0.0rc9/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/tests/test_ipython.py` & `soil-1.0.0rc9/tests/test_ipython.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/tests/test_main.py` & `soil-1.0.0rc9/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/tests/test_mesa.py` & `soil-1.0.0rc9/tests/test_mesa.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/tests/test_network.py` & `soil-1.0.0rc9/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc8/tests/test_time.py` & `soil-1.0.0rc9/tests/test_time.py`

 * *Files identical despite different names*

