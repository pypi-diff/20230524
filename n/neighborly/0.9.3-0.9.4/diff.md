# Comparing `tmp/neighborly-0.9.3.tar.gz` & `tmp/neighborly-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neighborly-0.9.3.tar", last modified: Mon Aug 15 04:29:08 2022, max compression
+gzip compressed data, was "neighborly-0.9.4.tar", last modified: Tue Nov 15 23:46:57 2022, max compression
```

## Comparing `neighborly-0.9.3.tar` & `neighborly-0.9.4.tar`

### file list

```diff
@@ -1,82 +1,86 @@
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2022-08-15 04:29:08.017412 neighborly-0.9.3/
--rw-r--r--   0 shijbey    (501) staff       (20)     5218 2022-04-29 01:20:53.000000 neighborly-0.9.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 shijbey    (501) staff       (20)     1074 2022-01-28 18:12:02.000000 neighborly-0.9.3/LICENSE
--rw-r--r--   0 shijbey    (501) staff       (20)      106 2022-08-09 16:37:17.000000 neighborly-0.9.3/MANIFEST.in
--rw-r--r--   0 shijbey    (501) staff       (20)     7921 2022-08-15 04:29:08.017511 neighborly-0.9.3/PKG-INFO
--rw-r--r--   0 shijbey    (501) staff       (20)     6891 2022-08-09 17:19:21.000000 neighborly-0.9.3/README.md
--rw-r--r--   0 shijbey    (501) staff       (20)      104 2022-08-08 21:08:07.000000 neighborly-0.9.3/pyproject.toml
--rw-r--r--   0 shijbey    (501) staff       (20)     1493 2022-08-15 04:29:08.017987 neighborly-0.9.3/setup.cfg
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2022-08-15 04:29:07.999422 neighborly-0.9.3/src/
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2022-08-15 04:29:08.002935 neighborly-0.9.3/src/neighborly/
--rw-r--r--   0 shijbey    (501) staff       (20)       22 2022-08-09 16:40:01.000000 neighborly-0.9.3/src/neighborly/__init__.py
--rw-r--r--   0 shijbey    (501) staff       (20)     7703 2022-08-12 17:55:24.000000 neighborly-0.9.3/src/neighborly/__main__.py
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2022-08-15 04:29:08.005605 neighborly-0.9.3/src/neighborly/builtin/
--rw-r--r--   0 shijbey    (501) staff       (20)        0 2022-08-08 21:08:07.000000 neighborly-0.9.3/src/neighborly/builtin/__init__.py
--rw-r--r--   0 shijbey    (501) staff       (20)    19050 2022-08-11 22:39:03.000000 neighborly-0.9.3/src/neighborly/builtin/events.py
--rw-r--r--   0 shijbey    (501) staff       (20)    10920 2022-08-10 16:47:06.000000 neighborly-0.9.3/src/neighborly/builtin/helpers.py
--rw-r--r--   0 shijbey    (501) staff       (20)     4768 2022-08-09 15:58:59.000000 neighborly-0.9.3/src/neighborly/builtin/role_filters.py
--rw-r--r--   0 shijbey    (501) staff       (20)     5746 2022-08-09 17:50:58.000000 neighborly-0.9.3/src/neighborly/builtin/statuses.py
--rw-r--r--   0 shijbey    (501) staff       (20)    44167 2022-08-10 17:23:22.000000 neighborly-0.9.3/src/neighborly/builtin/systems.py
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2022-08-15 04:29:08.010652 neighborly-0.9.3/src/neighborly/core/
--rw-r--r--   0 shijbey    (501) staff       (20)        0 2022-02-18 17:28:10.000000 neighborly-0.9.3/src/neighborly/core/__init__.py
--rw-r--r--   0 shijbey    (501) staff       (20)     2141 2022-08-09 14:17:42.000000 neighborly-0.9.3/src/neighborly/core/activity.py
--rw-r--r--   0 shijbey    (501) staff       (20)     7075 2022-08-11 21:03:13.000000 neighborly-0.9.3/src/neighborly/core/archetypes.py
--rw-r--r--   0 shijbey    (501) staff       (20)     1479 2022-08-08 21:08:07.000000 neighborly-0.9.3/src/neighborly/core/behavior_tree.py
--rw-r--r--   0 shijbey    (501) staff       (20)    17737 2022-08-12 00:21:53.000000 neighborly-0.9.3/src/neighborly/core/business.py
--rw-r--r--   0 shijbey    (501) staff       (20)     5737 2022-08-10 15:30:26.000000 neighborly-0.9.3/src/neighborly/core/character.py
--rw-r--r--   0 shijbey    (501) staff       (20)    13418 2022-08-08 21:08:07.000000 neighborly-0.9.3/src/neighborly/core/ecs.py
--rw-r--r--   0 shijbey    (501) staff       (20)     1523 2022-08-10 15:35:58.000000 neighborly-0.9.3/src/neighborly/core/engine.py
--rw-r--r--   0 shijbey    (501) staff       (20)    12973 2022-08-11 22:36:26.000000 neighborly-0.9.3/src/neighborly/core/life_event.py
--rw-r--r--   0 shijbey    (501) staff       (20)     2429 2022-08-08 21:08:07.000000 neighborly-0.9.3/src/neighborly/core/location.py
--rw-r--r--   0 shijbey    (501) staff       (20)     2061 2022-08-08 21:08:07.000000 neighborly-0.9.3/src/neighborly/core/name_generation.py
--rwxr-xr-x   0 shijbey    (501) staff       (20)     4281 2022-08-10 13:57:07.000000 neighborly-0.9.3/src/neighborly/core/personal_values.py
--rw-r--r--   0 shijbey    (501) staff       (20)      573 2022-08-08 21:08:07.000000 neighborly-0.9.3/src/neighborly/core/position.py
--rw-r--r--   0 shijbey    (501) staff       (20)    10665 2022-08-08 21:08:07.000000 neighborly-0.9.3/src/neighborly/core/relationship.py
--rw-r--r--   0 shijbey    (501) staff       (20)     2808 2022-08-10 15:31:44.000000 neighborly-0.9.3/src/neighborly/core/residence.py
--rw-r--r--   0 shijbey    (501) staff       (20)     3253 2022-08-08 21:08:07.000000 neighborly-0.9.3/src/neighborly/core/rng.py
--rw-r--r--   0 shijbey    (501) staff       (20)     7459 2022-08-11 22:48:17.000000 neighborly-0.9.3/src/neighborly/core/routine.py
--rw-r--r--   0 shijbey    (501) staff       (20)      516 2022-06-30 12:38:50.000000 neighborly-0.9.3/src/neighborly/core/status.py
--rw-r--r--   0 shijbey    (501) staff       (20)     8642 2022-08-08 21:08:07.000000 neighborly-0.9.3/src/neighborly/core/time.py
--rw-r--r--   0 shijbey    (501) staff       (20)     6118 2022-08-10 15:42:53.000000 neighborly-0.9.3/src/neighborly/core/town.py
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2022-08-15 04:29:08.011216 neighborly-0.9.3/src/neighborly/core/utils/
--rw-r--r--   0 shijbey    (501) staff       (20)        0 2022-04-29 01:21:04.000000 neighborly-0.9.3/src/neighborly/core/utils/__init__.py
--rw-r--r--   0 shijbey    (501) staff       (20)     3787 2022-08-08 21:08:07.000000 neighborly-0.9.3/src/neighborly/core/utils/graph.py
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2022-08-15 04:29:08.011546 neighborly-0.9.3/src/neighborly/core/utils/tracery/
--rw-r--r--   0 shijbey    (501) staff       (20)    12353 2022-08-08 21:08:07.000000 neighborly-0.9.3/src/neighborly/core/utils/tracery/__init__.py
--rw-r--r--   0 shijbey    (501) staff       (20)     1402 2022-04-29 01:21:04.000000 neighborly-0.9.3/src/neighborly/core/utils/tracery/modifiers.py
--rw-r--r--   0 shijbey    (501) staff       (20)     1629 2022-08-08 21:08:07.000000 neighborly-0.9.3/src/neighborly/core/utils/utilities.py
--rw-r--r--   0 shijbey    (501) staff       (20)     1038 2022-08-09 13:22:34.000000 neighborly-0.9.3/src/neighborly/exporter.py
--rw-r--r--   0 shijbey    (501) staff       (20)     1782 2022-08-08 21:08:07.000000 neighborly-0.9.3/src/neighborly/inspection_tools.py
--rw-r--r--   0 shijbey    (501) staff       (20)     3594 2022-08-10 15:31:45.000000 neighborly-0.9.3/src/neighborly/loaders.py
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2022-08-15 04:29:08.012063 neighborly-0.9.3/src/neighborly/plugins/
--rw-r--r--   0 shijbey    (501) staff       (20)        0 2022-08-08 21:08:07.000000 neighborly-0.9.3/src/neighborly/plugins/__init__.py
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2022-08-15 04:29:08.012356 neighborly-0.9.3/src/neighborly/plugins/default_plugin/
--rw-r--r--   0 shijbey    (501) staff       (20)     3021 2022-08-11 21:21:23.000000 neighborly-0.9.3/src/neighborly/plugins/default_plugin/__init__.py
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2022-08-15 04:29:08.012760 neighborly-0.9.3/src/neighborly/plugins/default_plugin/data/
--rw-r--r--   0 shijbey    (501) staff       (20)     1267 2022-08-09 14:18:08.000000 neighborly-0.9.3/src/neighborly/plugins/default_plugin/data/data.yaml
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2022-08-15 04:29:08.014814 neighborly-0.9.3/src/neighborly/plugins/default_plugin/data/names/
--rw-r--r--   0 shijbey    (501) staff       (20)    19702 2022-02-18 17:28:10.000000 neighborly-0.9.3/src/neighborly/plugins/default_plugin/data/names/US_settlement_names.txt
--rw-r--r--   0 shijbey    (501) staff       (20)     5884 2022-02-18 17:28:10.000000 neighborly-0.9.3/src/neighborly/plugins/default_plugin/data/names/bar_names.txt
--rw-r--r--   0 shijbey    (501) staff       (20)    35576 2022-02-18 17:28:10.000000 neighborly-0.9.3/src/neighborly/plugins/default_plugin/data/names/feminine_names.txt
--rw-r--r--   0 shijbey    (501) staff       (20)    20293 2022-02-18 17:28:10.000000 neighborly-0.9.3/src/neighborly/plugins/default_plugin/data/names/masculine_names.txt
--rw-r--r--   0 shijbey    (501) staff       (20)      627 2022-02-18 17:28:10.000000 neighborly-0.9.3/src/neighborly/plugins/default_plugin/data/names/neutral_names.txt
--rw-r--r--   0 shijbey    (501) staff       (20)    17714 2022-02-18 17:28:10.000000 neighborly-0.9.3/src/neighborly/plugins/default_plugin/data/names/restaurant_names.txt
--rw-r--r--   0 shijbey    (501) staff       (20)   106910 2022-02-18 17:28:10.000000 neighborly-0.9.3/src/neighborly/plugins/default_plugin/data/names/surnames.txt
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2022-08-15 04:29:08.017101 neighborly-0.9.3/src/neighborly/plugins/talktown/
--rw-r--r--   0 shijbey    (501) staff       (20)    11165 2022-08-12 17:57:54.000000 neighborly-0.9.3/src/neighborly/plugins/talktown/__init__.py
--rw-r--r--   0 shijbey    (501) staff       (20)     9487 2022-08-10 15:31:44.000000 neighborly-0.9.3/src/neighborly/plugins/talktown/business_archetypes.py
--rw-r--r--   0 shijbey    (501) staff       (20)      290 2022-08-08 21:08:07.000000 neighborly-0.9.3/src/neighborly/plugins/talktown/components.py
--rw-r--r--   0 shijbey    (501) staff       (20)    11662 2022-08-09 15:51:08.000000 neighborly-0.9.3/src/neighborly/plugins/talktown/occupation_types.py
--rw-r--r--   0 shijbey    (501) staff       (20)     2611 2022-08-08 21:08:07.000000 neighborly-0.9.3/src/neighborly/plugins/talktown/personality.py
--rw-r--r--   0 shijbey    (501) staff       (20)     2269 2022-08-08 21:08:07.000000 neighborly-0.9.3/src/neighborly/plugins/talktown/school.py
--rw-r--r--   0 shijbey    (501) staff       (20)     3115 2022-08-08 21:08:07.000000 neighborly-0.9.3/src/neighborly/plugins/talktown/utils.py
--rw-r--r--   0 shijbey    (501) staff       (20)     2107 2022-08-12 17:57:23.000000 neighborly-0.9.3/src/neighborly/plugins/weather_plugin.py
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2022-08-15 04:29:08.017265 neighborly-0.9.3/src/neighborly/server/
--rw-r--r--   0 shijbey    (501) staff       (20)     1690 2022-08-08 21:08:07.000000 neighborly-0.9.3/src/neighborly/server/__init__.py
--rw-r--r--   0 shijbey    (501) staff       (20)     7791 2022-08-12 17:57:07.000000 neighborly-0.9.3/src/neighborly/simulation.py
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2022-08-15 04:29:08.003937 neighborly-0.9.3/src/neighborly.egg-info/
--rw-r--r--   0 shijbey    (501) staff       (20)     7921 2022-08-15 04:29:07.000000 neighborly-0.9.3/src/neighborly.egg-info/PKG-INFO
--rw-r--r--   0 shijbey    (501) staff       (20)     2506 2022-08-15 04:29:07.000000 neighborly-0.9.3/src/neighborly.egg-info/SOURCES.txt
--rw-r--r--   0 shijbey    (501) staff       (20)        1 2022-08-15 04:29:07.000000 neighborly-0.9.3/src/neighborly.egg-info/dependency_links.txt
--rw-r--r--   0 shijbey    (501) staff       (20)      165 2022-08-15 04:29:07.000000 neighborly-0.9.3/src/neighborly.egg-info/requires.txt
--rw-r--r--   0 shijbey    (501) staff       (20)       11 2022-08-15 04:29:07.000000 neighborly-0.9.3/src/neighborly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-11-15 23:46:57.534600 neighborly-0.9.4/
+-rw-rw-rw-   0        0        0     1802 2022-11-15 23:44:51.000000 neighborly-0.9.4/CHANGELOG.md
+-rw-rw-rw-   0        0        0     5352 2022-09-27 19:23:48.000000 neighborly-0.9.4/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0     1080 2022-01-20 04:47:06.000000 neighborly-0.9.4/LICENSE
+-rw-rw-rw-   0        0        0      125 2022-11-14 14:29:43.000000 neighborly-0.9.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     9899 2022-11-15 23:46:57.534600 neighborly-0.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8646 2022-11-14 14:29:43.000000 neighborly-0.9.4/README.md
+-rw-rw-rw-   0        0        0      296 2022-11-14 14:29:43.000000 neighborly-0.9.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1560 2022-11-15 23:46:57.543159 neighborly-0.9.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-11-15 23:46:57.154513 neighborly-0.9.4/src/
+drwxrwxrwx   0        0        0        0 2022-11-15 23:46:57.200734 neighborly-0.9.4/src/neighborly/
+-rw-rw-rw-   0        0        0      350 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/__init__.py
+-rw-rw-rw-   0        0        0     7989 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/__main__.py
+drwxrwxrwx   0        0        0        0 2022-11-15 23:46:57.275369 neighborly-0.9.4/src/neighborly/builtin/
+-rw-rw-rw-   0        0        0        0 2022-09-27 19:23:48.000000 neighborly-0.9.4/src/neighborly/builtin/__init__.py
+-rw-rw-rw-   0        0        0     1988 2022-11-14 19:58:02.000000 neighborly-0.9.4/src/neighborly/builtin/ai.py
+-rw-rw-rw-   0        0        0     6260 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/builtin/archetypes.py
+-rw-rw-rw-   0        0        0     7422 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/builtin/components.py
+-rw-rw-rw-   0        0        0    21337 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/builtin/events.py
+-rw-rw-rw-   0        0        0    16976 2022-11-14 21:35:59.000000 neighborly-0.9.4/src/neighborly/builtin/helpers.py
+-rw-rw-rw-   0        0        0     7135 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/builtin/role_filters.py
+-rw-rw-rw-   0        0        0    40118 2022-11-15 18:09:14.000000 neighborly-0.9.4/src/neighborly/builtin/systems.py
+drwxrwxrwx   0        0        0        0 2022-11-15 23:46:57.398997 neighborly-0.9.4/src/neighborly/core/
+-rw-rw-rw-   0        0        0        0 2022-04-19 16:58:40.000000 neighborly-0.9.4/src/neighborly/core/__init__.py
+-rw-rw-rw-   0        0        0     1510 2022-11-14 21:48:49.000000 neighborly-0.9.4/src/neighborly/core/action.py
+-rw-rw-rw-   0        0        0     4329 2022-11-14 15:56:12.000000 neighborly-0.9.4/src/neighborly/core/ai.py
+-rw-rw-rw-   0        0        0    12396 2022-11-14 16:12:59.000000 neighborly-0.9.4/src/neighborly/core/archetypes.py
+-rw-rw-rw-   0        0        0      731 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/core/building.py
+-rw-rw-rw-   0        0        0    24421 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/core/business.py
+-rw-rw-rw-   0        0        0     1353 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/core/character.py
+-rw-rw-rw-   0        0        0      258 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/core/constants.py
+-rw-rw-rw-   0        0        0    13240 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/core/ecs.py
+-rw-rw-rw-   0        0        0     1503 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/core/engine.py
+-rw-rw-rw-   0        0        0     8383 2022-11-14 21:27:47.000000 neighborly-0.9.4/src/neighborly/core/event.py
+-rw-rw-rw-   0        0        0     9501 2022-11-15 17:01:52.000000 neighborly-0.9.4/src/neighborly/core/life_event.py
+-rw-rw-rw-   0        0        0      957 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/core/location.py
+-rw-rw-rw-   0        0        0     1496 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/core/name_generation.py
+-rw-rw-rw-   0        0        0     4706 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/core/personal_values.py
+-rw-rw-rw-   0        0        0      506 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/core/position.py
+-rw-rw-rw-   0        0        0    13580 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/core/query.py
+-rw-rw-rw-   0        0        0     7174 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/core/relationship.py
+-rw-rw-rw-   0        0        0     2225 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/core/residence.py
+-rw-rw-rw-   0        0        0     1559 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/core/role.py
+-rw-rw-rw-   0        0        0    10114 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/core/routine.py
+-rw-rw-rw-   0        0        0      332 2022-09-27 19:23:48.000000 neighborly-0.9.4/src/neighborly/core/serializable.py
+-rw-rw-rw-   0        0        0     1632 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/core/system.py
+-rw-rw-rw-   0        0        0    10668 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/core/time.py
+-rw-rw-rw-   0        0        0     3622 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/core/town.py
+drwxrwxrwx   0        0        0        0 2022-11-15 23:46:57.429044 neighborly-0.9.4/src/neighborly/core/utils/
+-rw-rw-rw-   0        0        0        0 2022-05-02 18:47:44.000000 neighborly-0.9.4/src/neighborly/core/utils/__init__.py
+-rw-rw-rw-   0        0        0     3959 2022-09-27 19:23:48.000000 neighborly-0.9.4/src/neighborly/core/utils/graph.py
+-rw-rw-rw-   0        0        0     3142 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/core/utils/grid.py
+-rw-rw-rw-   0        0        0     1230 2022-09-27 19:23:48.000000 neighborly-0.9.4/src/neighborly/core/utils/utilities.py
+-rw-rw-rw-   0        0        0      790 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/exporter.py
+-rw-rw-rw-   0        0        0     4960 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/loaders.py
+drwxrwxrwx   0        0        0        0 2022-11-15 23:46:57.439554 neighborly-0.9.4/src/neighborly/plugins/
+-rw-rw-rw-   0        0        0        0 2022-05-02 18:47:39.000000 neighborly-0.9.4/src/neighborly/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-15 23:46:57.441546 neighborly-0.9.4/src/neighborly/plugins/defaults/
+-rw-rw-rw-   0        0        0     7449 2022-11-14 16:02:57.000000 neighborly-0.9.4/src/neighborly/plugins/defaults/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-15 23:46:57.449584 neighborly-0.9.4/src/neighborly/plugins/defaults/data/
+-rw-rw-rw-   0        0        0     1341 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/plugins/defaults/data/data.yaml
+drwxrwxrwx   0        0        0        0 2022-11-15 23:46:57.463546 neighborly-0.9.4/src/neighborly/plugins/defaults/data/names/
+-rw-rw-rw-   0        0        0    21769 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/plugins/defaults/data/names/US_settlement_names.txt
+-rw-rw-rw-   0        0        0     6194 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/plugins/defaults/data/names/bar_names.txt
+-rw-rw-rw-   0        0        0    40577 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/plugins/defaults/data/names/feminine_names.txt
+-rw-rw-rw-   0        0        0    23236 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/plugins/defaults/data/names/masculine_names.txt
+-rw-rw-rw-   0        0        0      723 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/plugins/defaults/data/names/neutral_names.txt
+-rw-rw-rw-   0        0        0    19159 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/plugins/defaults/data/names/restaurant_names.txt
+-rw-rw-rw-   0        0        0   121266 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/plugins/defaults/data/names/surnames.txt
+drwxrwxrwx   0        0        0        0 2022-11-15 23:46:57.532596 neighborly-0.9.4/src/neighborly/plugins/talktown/
+-rw-rw-rw-   0        0        0     9625 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/plugins/talktown/__init__.py
+-rw-rw-rw-   0        0        0    12461 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/plugins/talktown/business_archetypes.py
+-rw-rw-rw-   0        0        0     5158 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/plugins/talktown/business_components.py
+-rw-rw-rw-   0        0        0     7102 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/plugins/talktown/occupation_types.py
+-rw-rw-rw-   0        0        0     2469 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/plugins/talktown/personality.py
+-rw-rw-rw-   0        0        0     1760 2022-11-14 21:37:34.000000 neighborly-0.9.4/src/neighborly/plugins/talktown/school.py
+-rw-rw-rw-   0        0        0     3243 2022-09-27 19:23:48.000000 neighborly-0.9.4/src/neighborly/plugins/talktown/utils.py
+-rw-rw-rw-   0        0        0     2276 2022-11-14 14:29:43.000000 neighborly-0.9.4/src/neighborly/plugins/weather.py
+-rw-rw-rw-   0        0        0     8301 2022-11-15 16:56:31.000000 neighborly-0.9.4/src/neighborly/simulation.py
+drwxrwxrwx   0        0        0        0 2022-11-15 23:46:57.237254 neighborly-0.9.4/src/neighborly.egg-info/
+-rw-rw-rw-   0        0        0     9899 2022-11-15 23:46:57.000000 neighborly-0.9.4/src/neighborly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2595 2022-11-15 23:46:57.000000 neighborly-0.9.4/src/neighborly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-15 23:46:57.000000 neighborly-0.9.4/src/neighborly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2022-11-15 23:46:57.000000 neighborly-0.9.4/src/neighborly.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       89 2022-11-15 23:46:57.000000 neighborly-0.9.4/src/neighborly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2022-11-15 23:46:57.000000 neighborly-0.9.4/src/neighborly.egg-info/top_level.txt
```

### Comparing `neighborly-0.9.3/CODE_OF_CONDUCT.md` & `neighborly-0.9.4/CODE_OF_CONDUCT.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-# Contributor Covenant Code of Conduct
-
-## Our Pledge
-
-We as members, contributors, and leaders pledge to make participation in our
-community a harassment-free experience for everyone, regardless of age, body
-size, visible or invisible disability, ethnicity, sex characteristics, gender
-identity and expression, level of experience, education, socio-economic status,
-nationality, personal appearance, race, religion, or sexual identity
-and orientation.
-
-We pledge to act and interact in ways that contribute to an open, welcoming,
-diverse, inclusive, and healthy community.
-
-## Our Standards
-
-Examples of behavior that contributes to a positive environment for our
-community include:
-
-* Demonstrating empathy and kindness toward other people
-* Being respectful of differing opinions, viewpoints, and experiences
-* Giving and gracefully accepting constructive feedback
-* Accepting responsibility and apologizing to those affected by our mistakes,
-  and learning from the experience
-* Focusing on what is best not just for us as individuals, but for the
-  overall community
-
-Examples of unacceptable behavior include:
-
-* The use of sexualized language or imagery, and sexual attention or
-  advances of any kind
-* Trolling, insulting or derogatory comments, and personal or political attacks
-* Public or private harassment
-* Publishing others' private information, such as a physical or email
-  address, without their explicit permission
-* Other conduct which could reasonably be considered inappropriate in a
-  professional setting
-
-## Enforcement Responsibilities
-
-Community leaders are responsible for clarifying and enforcing our standards of
-acceptable behavior and will take appropriate and fair corrective action in
-response to any behavior that they deem inappropriate, threatening, offensive,
-or harmful.
-
-Community leaders have the right and responsibility to remove, edit, or reject
-comments, commits, code, wiki edits, issues, and other contributions that are
-not aligned to this Code of Conduct, and will communicate reasons for moderation
-decisions when appropriate.
-
-## Scope
-
-This Code of Conduct applies within all community spaces, and also applies when
-an individual is officially representing the community in public spaces.
-Examples of representing our community include using an official e-mail address,
-posting via an official social media account, or acting as an appointed
-representative at an online or offline event.
-
-## Enforcement
-
-Instances of abusive, harassing, or otherwise unacceptable behavior may be
-reported to the community leaders responsible for enforcement at
-shijbey@ucsc.edu.
-All complaints will be reviewed and investigated promptly and fairly.
-
-All community leaders are obligated to respect the privacy and security of the
-reporter of any incident.
-
-## Enforcement Guidelines
-
-Community leaders will follow these Community Impact Guidelines in determining
-the consequences for any action they deem in violation of this Code of Conduct:
-
-### 1. Correction
-
-**Community Impact**: Use of inappropriate language or other behavior deemed
-unprofessional or unwelcome in the community.
-
-**Consequence**: A private, written warning from community leaders, providing
-clarity around the nature of the violation and an explanation of why the
-behavior was inappropriate. A public apology may be requested.
-
-### 2. Warning
-
-**Community Impact**: A violation through a single incident or series
-of actions.
-
-**Consequence**: A warning with consequences for continued behavior. No
-interaction with the people involved, including unsolicited interaction with
-those enforcing the Code of Conduct, for a specified period of time. This
-includes avoiding interactions in community spaces as well as external channels
-like social media. Violating these terms may lead to a temporary or
-permanent ban.
-
-### 3. Temporary Ban
-
-**Community Impact**: A serious violation of community standards, including
-sustained inappropriate behavior.
-
-**Consequence**: A temporary ban from any sort of interaction or public
-communication with the community for a specified period of time. No public or
-private interaction with the people involved, including unsolicited interaction
-with those enforcing the Code of Conduct, is allowed during this period.
-Violating these terms may lead to a permanent ban.
-
-### 4. Permanent Ban
-
-**Community Impact**: Demonstrating a pattern of violation of community
-standards, including sustained inappropriate behavior,  harassment of an
-individual, or aggression toward or disparagement of classes of individuals.
-
-**Consequence**: A permanent ban from any sort of public interaction within
-the community.
-
-## Attribution
-
-This Code of Conduct is adapted from the [Contributor Covenant][homepage],
-version 2.0, available at
-https://www.contributor-covenant.org/version/2/0/code_of_conduct.html.
-
-Community Impact Guidelines were inspired by [Mozilla's code of conduct
-enforcement ladder](https://github.com/mozilla/diversity).
-
-[homepage]: https://www.contributor-covenant.org
-
-For answers to common questions about this code of conduct, see the FAQ at
-https://www.contributor-covenant.org/faq. Translations are available at
-https://www.contributor-covenant.org/translations.
+# Contributor Covenant Code of Conduct
+
+## Our Pledge
+
+We as members, contributors, and leaders pledge to make participation in our
+community a harassment-free experience for everyone, regardless of age, body
+size, visible or invisible disability, ethnicity, sex characteristics, gender
+identity and expression, level of experience, education, socio-economic status,
+nationality, personal appearance, race, religion, or sexual identity
+and orientation.
+
+We pledge to act and interact in ways that contribute to an open, welcoming,
+diverse, inclusive, and healthy community.
+
+## Our Standards
+
+Examples of behavior that contributes to a positive environment for our
+community include:
+
+* Demonstrating empathy and kindness toward other people
+* Being respectful of differing opinions, viewpoints, and experiences
+* Giving and gracefully accepting constructive feedback
+* Accepting responsibility and apologizing to those affected by our mistakes,
+  and learning from the experience
+* Focusing on what is best not just for us as individuals, but for the
+  overall community
+
+Examples of unacceptable behavior include:
+
+* The use of sexualized language or imagery, and sexual attention or
+  advances of any kind
+* Trolling, insulting or derogatory comments, and personal or political attacks
+* Public or private harassment
+* Publishing others' private information, such as a physical or email
+  address, without their explicit permission
+* Other conduct which could reasonably be considered inappropriate in a
+  professional setting
+
+## Enforcement Responsibilities
+
+Community leaders are responsible for clarifying and enforcing our standards of
+acceptable behavior and will take appropriate and fair corrective action in
+response to any behavior that they deem inappropriate, threatening, offensive,
+or harmful.
+
+Community leaders have the right and responsibility to remove, edit, or reject
+comments, commits, code, wiki edits, issues, and other contributions that are
+not aligned to this Code of Conduct, and will communicate reasons for moderation
+decisions when appropriate.
+
+## Scope
+
+This Code of Conduct applies within all community spaces, and also applies when
+an individual is officially representing the community in public spaces.
+Examples of representing our community include using an official e-mail address,
+posting via an official social media account, or acting as an appointed
+representative at an online or offline event.
+
+## Enforcement
+
+Instances of abusive, harassing, or otherwise unacceptable behavior may be
+reported to the community leaders responsible for enforcement at
+shijbey@ucsc.edu.
+All complaints will be reviewed and investigated promptly and fairly.
+
+All community leaders are obligated to respect the privacy and security of the
+reporter of any incident.
+
+## Enforcement Guidelines
+
+Community leaders will follow these Community Impact Guidelines in determining
+the consequences for any action they deem in violation of this Code of Conduct:
+
+### 1. Correction
+
+**Community Impact**: Use of inappropriate language or other behavior deemed
+unprofessional or unwelcome in the community.
+
+**Consequence**: A private, written warning from community leaders, providing
+clarity around the nature of the violation and an explanation of why the
+behavior was inappropriate. A public apology may be requested.
+
+### 2. Warning
+
+**Community Impact**: A violation through a single incident or series
+of actions.
+
+**Consequence**: A warning with consequences for continued behavior. No
+interaction with the people involved, including unsolicited interaction with
+those enforcing the Code of Conduct, for a specified period of time. This
+includes avoiding interactions in community spaces as well as external channels
+like social media. Violating these terms may lead to a temporary or
+permanent ban.
+
+### 3. Temporary Ban
+
+**Community Impact**: A serious violation of community standards, including
+sustained inappropriate behavior.
+
+**Consequence**: A temporary ban from any sort of interaction or public
+communication with the community for a specified period of time. No public or
+private interaction with the people involved, including unsolicited interaction
+with those enforcing the Code of Conduct, is allowed during this period.
+Violating these terms may lead to a permanent ban.
+
+### 4. Permanent Ban
+
+**Community Impact**: Demonstrating a pattern of violation of community
+standards, including sustained inappropriate behavior,  harassment of an
+individual, or aggression toward or disparagement of classes of individuals.
+
+**Consequence**: A permanent ban from any sort of public interaction within
+the community.
+
+## Attribution
+
+This Code of Conduct is adapted from the [Contributor Covenant][homepage],
+version 2.0, available at
+<https://www.contributor-covenant.org/version/2/0/code_of_conduct.html>.
+
+Community Impact Guidelines were inspired by [Mozilla's code of conduct
+enforcement ladder](https://github.com/mozilla/diversity).
+
+[homepage]: https://www.contributor-covenant.org
+
+For answers to common questions about this code of conduct, see the FAQ at
+<https://www.contributor-covenant.org/faq>. Translations are available at
+<https://www.contributor-covenant.org/translations>.
```

### Comparing `neighborly-0.9.3/LICENSE` & `neighborly-0.9.4/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2022 Shi Johnson-Bey <shijbey@gmail.com>
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright 2022 Shi Johnson-Bey <shijbey@gmail.com>
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `neighborly-0.9.3/PKG-INFO` & `neighborly-0.9.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,198 +1,247 @@
-Metadata-Version: 2.1
-Name: neighborly
-Version: 0.9.3
-Summary: An extensible social simulation engine for generating towns of characters
-Home-page: https://github.com/ShiJbey/neighborly
-Author: Shi Johnson-Bey
-Author-email: shijbey@ucsc.edu
-License: MIT
-Project-URL: Bug Tracker, https://github.com/ShiJbey/neighborly/issues
-Keywords: social simulation,emergent narrative,life simulator framework,multi-agent
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Games/Entertainment :: Simulation
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Artificial Life
-Classifier: Topic :: Sociology
-Classifier: Typing :: Typed
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: samples
-License-File: LICENSE
-
-<h1 align="center">
-  <img
-    width="300"
-    height="300"
-    src="https://user-images.githubusercontent.com/11076525/165836171-9ffdea6e-1633-440c-be06-b46e1e3e4e04.png"
-  >
-  <br>
-  Neighborly
-</h1>
-
-<h3 align="center"><b>Social simulation engine for procedurally generating towns of characters</b></h2>
-
-<p align="center">
-  <img src="https://img.shields.io/pypi/dm/neighborly">
-  <img src="https://img.shields.io/pypi/l/neighborly">
-  <img src="https://img.shields.io/pypi/v/neighborly">
-  <img src="https://img.shields.io/pypi/pyversions/neighborly">
-</p>
-
-# Overview
-
-Neighborly is a social simulation engine for procedurally generating towns of characters. It simulates
-the lives of each character, their jobs, routines, relationships, and life events. Neighborly utilizes
-an entity-component system architecture, and enables users to specify custom character types, businesses,
-occupations, life events, and AI components and simulation systems.
-
-Neighborly takes lessons learned from working with
-[_Talk of the Town_](https://github.com/james-owen-ryan/talktown)
-and aims to give people better documentation, simpler interfaces, and more opportunities for extension and content authoring.
-
-<b>Neighborly is not fully functional yet. I am actively working toward a working release.</b>
-
-# Core Features
-
-* Create custom Character Archetypes and have them all interact within the same simulation
-* Create custom Business and Occupation definitions
-* Configure simulation data using YAML or in code with Python
-* Plugin architecture allows users to modularize and share their custom content
-* Low fidelity simulation simulates the macro events in character's lives (relationship milestones, job changes, victories, tragic events)
-* Export simulation state to JSON for further data processing
-
-# Tutorials and How-to Guides
-
-I plan to add these after I have finished implementing Neighborly's core
-functionality. I will try to align them with the sample projects, but we
-will see how the first pre-release looks. For now, loosely refer to the
-samples. Although, they too lag behind breaking changes to the core codebase.
-
-# Installing from PyPI
-
-Neighborly is available to install via pip.
-
-```bash
-pip install neighborly
-```
-
-# Installing for local development
-
-If you wish to download a Neighborly for local development, follow the these instructions.
-
-```bash
-# Step One: Clone Repository
-git clone https://github.com/ShiJbey/neighborly.git
-
-# Step Two (Optional): Create and activate python virtual environment
-cd neighborly
-
-# For Linux and MacOS
-python3 -m venv venv
-source ./venv/bin/activate
-
-# For Windows
-python -m venv venv
-./venv/Scripts/Activate
-
-# Step Three: Install local build and dependencies
-python -m pip install -e "."
-```
-
-# Running the Tests
-
-The tests are currently out-of-date and may refer to systems
-and logic that no longer exists in Neighborly. The codebase
-changes so frequently that it hasn't been worth the time. 
-As modules  become more established, I will add proper tests for them. 
-Feel free to contribute tests by forking the repo, adding your test(s), and
-submitting a pull request with a description of your test cases. Your commits
-should only contain changes to files within the `tests` directory. If you
-change any files in other parts of the project, your PR will be rejected.
-
-Please follow the steps below to run Neighborly's test suite. Neighborly uses
-[PyTest](https://docs.pytest.org/en/7.1.x/) to handle unit testing.
-
-```bash
-# Step 1: Install dependencies for tests
-python -m pip install -e ".[tests]"
-
-# Step 2: Run Pytest
-pytest
-```
-
-# Running the Samples
-
-Please follow the steps below to run the sample simulations.
-We also have examples for using Neighborly in a IPython
-notebook and with PyGame.
-
-```bash
-# Step 1: Install dependencies for samples
-python -m pip install -e ".[samples]"
-
-# Step 2: Run desired sample
-python ./samples/<sample_name>.py
-```
-
-# Documentation
-
-Neighborly uses [Numpy-style](https://numpydoc.readthedocs.io/en/latest/format.html) docstrings in code and full documentation can be found in the [Wiki](https://github.com/ShiJbey/neighborly/wiki).
-
-When adding docstrings for existing or new bits of code please use the following
-references for how to format your contributions:
-
-* [Sphinx Napoleon Plugin for processing Numpy Docstrings](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html)
-* [Example Numpy Style Docstrings](https://www.sphinx-doc.org/en/master/usage/extensions/example_numpy.html#example-numpy)
-
-
-# Contributing
-
-If you are interested in contributing to Neighborly, feel free to fork this repository, make your changes, and submit a pull-request. Please keep in mind that this project is a tool for creativity and learning. We have a [code of conduct](./CODE_OF_CONDUCT.md) to encourage healthy collaboration, and will enforce it if we need to.
-
-**WARNING::** This repository's structure in high flux. Parts of the code get shifted to make the APIs cleaner for use.
-
-Here are some ways that people can contribute to Neighborly:
-
-1. Proposing/Implementing new features
-2. Fixing bugs
-3. Providing optimizations
-4. Fixing typos
-5. Filing issues
-6. Contributing tutorials/how-tos to the wiki
-7. Fixing grammar and spelling in the wiki
-8. Creating new samples
-
-## Code Style
-
-Neighborly does not have a set-in-stone code style yet, but I have started integrating
-isort, black, and flake8 into the development workflow in VSCode.
-
-You can follow [these instructions](https://black.readthedocs.io/en/stable/integrations/editors.html) for setting up both black and isort. And I found this gist helpful for getting [flake8 working in PyCharm](https://gist.github.com/tossmilestone/23139d870841a3d5cba2aea28da1a895).
-
-# Notes
-
-## Non-Deterministic Behavior
-
-The goal of having a seeded pseudo random simulation is so that users experience deterministic behavior when using the
-same starting seed. We try to remove all forms of non-determinism, but some slip through. The known areas are listed
-below. If you find any, please make a new issue with details of the behavior.
-
-* Names may not be consistent when using the same seed. Currently, names are generated
-  using [Tracery](https://github.com/aparrish/pytracery). We would need to create a custom version that uses an RNG
-  instance instead of the global random module to generate names.
-
-## DMCA Statement
-
-Upon receipt of a notice alleging copyright infringement, I will take whatever action it deems
-appropriate within its sole discretion, including removal of the allegedly infringing materials.
-
-The repo image is something fun that I made. I love _The Simpsons_, and I couldn't think of anything more neighborly
-than Ned Flanders. If the copyright owner for _The Simpsons_ would like me to take it down,
-please contact me.
-
-The same takedown policy applies to any code samples inspired by TV shows, movies, and games.
+Metadata-Version: 2.1
+Name: neighborly
+Version: 0.9.4
+Summary: An extensible social simulation framework for generating towns of characters
+Home-page: https://github.com/ShiJbey/neighborly
+Author: Shi Johnson-Bey
+Author-email: shijbey@ucsc.edu
+License: MIT
+Project-URL: Bug Tracker, https://github.com/ShiJbey/neighborly/issues
+Project-URL: Documentation, https://github.com/ShiJbey/neighborly/wiki
+Project-URL: Changelog, https://github.com/ShiJbey/neighborly/blob/main/CHANGELOG.md
+Keywords: social simulation,emergent narrative,life simulator,multi-agent framework
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Games/Entertainment :: Simulation
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Artificial Life
+Classifier: Topic :: Sociology
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+License-File: LICENSE
+
+<h1 align="center">
+  <img
+    width="150"
+    height="150"
+    src="https://user-images.githubusercontent.com/11076525/165836171-9ffdea6e-1633-440c-be06-b46e1e3e4e04.png"
+  >
+  <br>
+  Neighborly
+</h1>
+
+<p align="center">
+  <img src="https://img.shields.io/badge/status-unstable-critical?style=flat">
+  <img src="https://img.shields.io/pypi/v/neighborly">
+  <img src="https://img.shields.io/pypi/pyversions/neighborly">
+  <img src="https://img.shields.io/pypi/l/neighborly">
+  <img src="https://img.shields.io/pypi/dm/neighborly">
+  <img src="https://img.shields.io/badge/code%20style-black-black">
+  <img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336">
+</p>
+
+# Overview
+
+Neighborly is a Python framework for generating and forward simulating towns of
+characters over large periods of time (decades to centuries). It uses a character-driven
+social simulation that forward-simulates the lives of each character, their jobs,
+routines, relationships, and life events. Users can specify custom characters,
+residential/commercial buildings, occupations, life events, social actions, and more.
+
+Currently, _Neighborly_ works best as narrative data generator. When the simulation
+ends, users can save the history of events, characters, relationships, and other stuff.
+
+Neighborly was inspired by lessons learned from working with
+[_Talk of the Town_](https://github.com/james-owen-ryan/talktown)
+and aims to give people better documentation, simpler interfaces, and more opportunities
+for extension and content authoring.
+
+## Core Features
+
+* Create custom character, buildings, life events, and social actions
+* Commandline interface (CLI) tool
+* Configure the CLI using YAML text files
+* Plugin architecture allows users to modularize and share their custom content
+* Export simulation state to JSON for further data processing
+
+# How to use
+
+Below are instructions for installing Neighborly and the options one has for using it
+in their projects. If you want examples of how to use Neighborly and how to extend it
+with custom content, please refer to
+[Neighborly's wiki](https://github.com/ShiJbey/neighborly/wiki) and the sample scripts
+in the [_samples_ directory](https://github.com/ShiJbey/neighborly/tree/main/samples).
+
+## Installation
+
+Neighborly is available to install from PyPI.
+
+```bash
+pip install neighborly
+```
+
+Or you can install it by cloning the main branch of this repo and installing that.
+
+```bash
+git clone https://github.com/ShiJbey/neighborly.git
+
+cd neighborly
+
+python -m pip install .
+```
+
+## Using as a library
+
+Neighborly can be used as a library within a Python script or package.
+The `samples` directory contains python scripts that use Neighborly this
+way. Please refer to them when creating new Plugins and other content.
+
+## Running the CLI
+
+Neighborly can be run as a module `$ python -m neighborly` or commandline `$ neighborly`
+script. If you require additional help while running, please use
+`python -m neighborly --help` or `neighborly --help`.
+
+By default, Neighborly runs a builtin version of **Talk of the Town**. However, you can
+configure the simulation settings by creating a `neighborlyconfig.yaml` file in
+the same directory where you're running the CLI. Please refer to the
+[wiki](https://github.com/ShiJbey/neighborly/wiki/Neighborly-CLI) for a list of
+valid configuration settings.
+
+When world generation concludes, Neighborly can write the final simulation data
+to a JSON file with the name of the town and the seed used for random number
+generation.
+
+## Running the Samples
+
+Neighborly provides sample simulations to show users how to customize
+it to create new story world themes.
+
+```bash
+# Make sure that you've activated your python virtual environment
+# Replace <sample_name>.py with the name of the
+# sample you want to run
+python ./samples/<sample_name>.py
+```
+
+## Installing for local development
+
+If you wish to download a Neighborly for local development, you need to clone/fork this
+repository and install using the _editable_ flag (-e). Please see the instructions
+below.
+
+```bash
+# Step One: Clone Repository
+git clone https://github.com/ShiJbey/neighborly.git
+
+# Step Two (Optional): Create and activate python virtual environment
+cd neighborly
+
+# For Linux and MacOS
+python3 -m venv venv
+source ./venv/bin/activate
+
+# For Windows
+python -m venv venv
+./venv/Scripts/Activate
+
+# Step Three: Install local build and dependencies
+python -m pip install -e "."
+```
+
+## Running the Tests
+
+The tests are currently out-of-date and may refer to systems
+and logic that no longer exists in Neighborly. The codebase
+changes so frequently that it hasn't been worth the time.
+As modules  become more established, I will add proper tests for them.
+Feel free to contribute tests by forking the repo, adding your test(s), and
+submitting a pull request with a description of your test cases. Your commits
+should only contain changes to files within the `tests` directory. If you
+change any files in other parts of the project, your PR will be rejected.
+
+Please follow the steps below to run Neighborly's test suite. Neighborly uses
+[PyTest](https://docs.pytest.org/en/7.1.x/) to handle unit testing.
+
+```bash
+# Step 1: Install dependencies for tests
+python -m pip install -e ".[tests]"
+
+# Step 2: Run Pytest
+pytest
+
+# Step3 : (Optional) Generate a test coverage report
+pytest --cov=neighborly tests/
+```
+
+# Documentation
+
+Neighborly uses [Numpy-style](https://numpydoc.readthedocs.io/en/latest/format.html)
+docstrings in code and full documentation can be found in the
+[Wiki](https://github.com/ShiJbey/neighborly/wiki).
+
+When adding docstrings for existing or new bits of code please use the following
+references for how to format your contributions:
+
+* [Sphinx Napoleon Plugin for processing Numpy Docstrings](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html)
+* [Example Numpy Style Docstrings](https://www.sphinx-doc.org/en/master/usage/extensions/example_numpy.html#example-numpy)
+
+# Contributing
+
+Here are some ways that people can contribute to Neighborly:
+
+1. Proposing/Implementing new features
+2. Fixing bugs
+3. Providing optimizations
+4. Fixing typos
+5. Filing issues
+6. Contributing tutorials/how-tos to the wiki
+7. Fixing grammar and spelling in the wiki
+8. Creating new samples/plugins
+
+If you are interested in contributing to Neighborly, there are multiple ways to get
+involved, and not all of them require you to be proficient with GitHub. Interested
+parties can contribute to the core code base of Neighborly and/or create nre content
+in the way of plugins. I love feedback, and if you have any questions, create a new
+issue, and I will do my best to answer. If you want to contribute to the core code,
+free to fork this repository, make your changes, and submit a pull-request with a
+description of your contribution. Please keep in mind that this project is a
+tool for creativity and learning. I have a [code of conduct](./CODE_OF_CONDUCT.md) to
+encourage healthy collaboration, and will enforce it if I need to.
+
+## Code Style
+
+Neighborly uses [_Black_](https://black.readthedocs.io/en/stable/) to handle code style
+and sorts imports using [_isort_](https://pycqa.github.io/isort/). You can follow
+[these instructions](https://black.readthedocs.io/en/stable/integrations/editors.html)
+for setting up both black and isort.
+
+# Notes
+
+## Non-Deterministic Behavior
+
+The goal of having a seeded pseudo random simulation is so that users experience
+deterministic behavior when using the same starting seed. I try to remove all forms of
+non-determinism, but some slip through. The known areas are listed below. If you find
+any, please make a new issue with details of the behavior.
+
+* Neighborly uses [Tracery](https://github.com/aparrish/pytracery) to generate names for
+characters and locations, and these names may not be consistent despite using the same
+rng seed value.
+
+## DMCA Statement
+
+Upon receipt of a notice alleging copyright infringement, I will take whatever action it
+deems appropriate within its sole discretion, including removal of the allegedly
+infringing materials.
+
+The repo image is something fun that I made. I love _The Simpsons_, and I couldn't think
+of anyone more neighborly than Ned Flanders. If the copyright owner for _The Simpsons_
+would like me to take it down, please contact me. The same takedown policy applies to
+any code samples inspired by TV shows, movies, and games.
```

### Comparing `neighborly-0.9.3/README.md` & `neighborly-0.9.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,172 +1,219 @@
-<h1 align="center">
-  <img
-    width="300"
-    height="300"
-    src="https://user-images.githubusercontent.com/11076525/165836171-9ffdea6e-1633-440c-be06-b46e1e3e4e04.png"
-  >
-  <br>
-  Neighborly
-</h1>
-
-<h3 align="center"><b>Social simulation engine for procedurally generating towns of characters</b></h2>
-
-<p align="center">
-  <img src="https://img.shields.io/pypi/dm/neighborly">
-  <img src="https://img.shields.io/pypi/l/neighborly">
-  <img src="https://img.shields.io/pypi/v/neighborly">
-  <img src="https://img.shields.io/pypi/pyversions/neighborly">
-</p>
-
-# Overview
-
-Neighborly is a social simulation engine for procedurally generating towns of characters. It simulates
-the lives of each character, their jobs, routines, relationships, and life events. Neighborly utilizes
-an entity-component system architecture, and enables users to specify custom character types, businesses,
-occupations, life events, and AI components and simulation systems.
-
-Neighborly takes lessons learned from working with
-[_Talk of the Town_](https://github.com/james-owen-ryan/talktown)
-and aims to give people better documentation, simpler interfaces, and more opportunities for extension and content authoring.
-
-<b>Neighborly is not fully functional yet. I am actively working toward a working release.</b>
-
-# Core Features
-
-* Create custom Character Archetypes and have them all interact within the same simulation
-* Create custom Business and Occupation definitions
-* Configure simulation data using YAML or in code with Python
-* Plugin architecture allows users to modularize and share their custom content
-* Low fidelity simulation simulates the macro events in character's lives (relationship milestones, job changes, victories, tragic events)
-* Export simulation state to JSON for further data processing
-
-# Tutorials and How-to Guides
-
-I plan to add these after I have finished implementing Neighborly's core
-functionality. I will try to align them with the sample projects, but we
-will see how the first pre-release looks. For now, loosely refer to the
-samples. Although, they too lag behind breaking changes to the core codebase.
-
-# Installing from PyPI
-
-Neighborly is available to install via pip.
-
-```bash
-pip install neighborly
-```
-
-# Installing for local development
-
-If you wish to download a Neighborly for local development, follow the these instructions.
-
-```bash
-# Step One: Clone Repository
-git clone https://github.com/ShiJbey/neighborly.git
-
-# Step Two (Optional): Create and activate python virtual environment
-cd neighborly
-
-# For Linux and MacOS
-python3 -m venv venv
-source ./venv/bin/activate
-
-# For Windows
-python -m venv venv
-./venv/Scripts/Activate
-
-# Step Three: Install local build and dependencies
-python -m pip install -e "."
-```
-
-# Running the Tests
-
-The tests are currently out-of-date and may refer to systems
-and logic that no longer exists in Neighborly. The codebase
-changes so frequently that it hasn't been worth the time. 
-As modules  become more established, I will add proper tests for them. 
-Feel free to contribute tests by forking the repo, adding your test(s), and
-submitting a pull request with a description of your test cases. Your commits
-should only contain changes to files within the `tests` directory. If you
-change any files in other parts of the project, your PR will be rejected.
-
-Please follow the steps below to run Neighborly's test suite. Neighborly uses
-[PyTest](https://docs.pytest.org/en/7.1.x/) to handle unit testing.
-
-```bash
-# Step 1: Install dependencies for tests
-python -m pip install -e ".[tests]"
-
-# Step 2: Run Pytest
-pytest
-```
-
-# Running the Samples
-
-Please follow the steps below to run the sample simulations.
-We also have examples for using Neighborly in a IPython
-notebook and with PyGame.
-
-```bash
-# Step 1: Install dependencies for samples
-python -m pip install -e ".[samples]"
-
-# Step 2: Run desired sample
-python ./samples/<sample_name>.py
-```
-
-# Documentation
-
-Neighborly uses [Numpy-style](https://numpydoc.readthedocs.io/en/latest/format.html) docstrings in code and full documentation can be found in the [Wiki](https://github.com/ShiJbey/neighborly/wiki).
-
-When adding docstrings for existing or new bits of code please use the following
-references for how to format your contributions:
-
-* [Sphinx Napoleon Plugin for processing Numpy Docstrings](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html)
-* [Example Numpy Style Docstrings](https://www.sphinx-doc.org/en/master/usage/extensions/example_numpy.html#example-numpy)
-
-
-# Contributing
-
-If you are interested in contributing to Neighborly, feel free to fork this repository, make your changes, and submit a pull-request. Please keep in mind that this project is a tool for creativity and learning. We have a [code of conduct](./CODE_OF_CONDUCT.md) to encourage healthy collaboration, and will enforce it if we need to.
-
-**WARNING::** This repository's structure in high flux. Parts of the code get shifted to make the APIs cleaner for use.
-
-Here are some ways that people can contribute to Neighborly:
-
-1. Proposing/Implementing new features
-2. Fixing bugs
-3. Providing optimizations
-4. Fixing typos
-5. Filing issues
-6. Contributing tutorials/how-tos to the wiki
-7. Fixing grammar and spelling in the wiki
-8. Creating new samples
-
-## Code Style
-
-Neighborly does not have a set-in-stone code style yet, but I have started integrating
-isort, black, and flake8 into the development workflow in VSCode.
-
-You can follow [these instructions](https://black.readthedocs.io/en/stable/integrations/editors.html) for setting up both black and isort. And I found this gist helpful for getting [flake8 working in PyCharm](https://gist.github.com/tossmilestone/23139d870841a3d5cba2aea28da1a895).
-
-# Notes
-
-## Non-Deterministic Behavior
-
-The goal of having a seeded pseudo random simulation is so that users experience deterministic behavior when using the
-same starting seed. We try to remove all forms of non-determinism, but some slip through. The known areas are listed
-below. If you find any, please make a new issue with details of the behavior.
-
-* Names may not be consistent when using the same seed. Currently, names are generated
-  using [Tracery](https://github.com/aparrish/pytracery). We would need to create a custom version that uses an RNG
-  instance instead of the global random module to generate names.
-
-## DMCA Statement
-
-Upon receipt of a notice alleging copyright infringement, I will take whatever action it deems
-appropriate within its sole discretion, including removal of the allegedly infringing materials.
-
-The repo image is something fun that I made. I love _The Simpsons_, and I couldn't think of anything more neighborly
-than Ned Flanders. If the copyright owner for _The Simpsons_ would like me to take it down,
-please contact me.
-
-The same takedown policy applies to any code samples inspired by TV shows, movies, and games.
+<h1 align="center">
+  <img
+    width="150"
+    height="150"
+    src="https://user-images.githubusercontent.com/11076525/165836171-9ffdea6e-1633-440c-be06-b46e1e3e4e04.png"
+  >
+  <br>
+  Neighborly
+</h1>
+
+<p align="center">
+  <img src="https://img.shields.io/badge/status-unstable-critical?style=flat">
+  <img src="https://img.shields.io/pypi/v/neighborly">
+  <img src="https://img.shields.io/pypi/pyversions/neighborly">
+  <img src="https://img.shields.io/pypi/l/neighborly">
+  <img src="https://img.shields.io/pypi/dm/neighborly">
+  <img src="https://img.shields.io/badge/code%20style-black-black">
+  <img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336">
+</p>
+
+# Overview
+
+Neighborly is a Python framework for generating and forward simulating towns of
+characters over large periods of time (decades to centuries). It uses a character-driven
+social simulation that forward-simulates the lives of each character, their jobs,
+routines, relationships, and life events. Users can specify custom characters,
+residential/commercial buildings, occupations, life events, social actions, and more.
+
+Currently, _Neighborly_ works best as narrative data generator. When the simulation
+ends, users can save the history of events, characters, relationships, and other stuff.
+
+Neighborly was inspired by lessons learned from working with
+[_Talk of the Town_](https://github.com/james-owen-ryan/talktown)
+and aims to give people better documentation, simpler interfaces, and more opportunities
+for extension and content authoring.
+
+## Core Features
+
+* Create custom character, buildings, life events, and social actions
+* Commandline interface (CLI) tool
+* Configure the CLI using YAML text files
+* Plugin architecture allows users to modularize and share their custom content
+* Export simulation state to JSON for further data processing
+
+# How to use
+
+Below are instructions for installing Neighborly and the options one has for using it
+in their projects. If you want examples of how to use Neighborly and how to extend it
+with custom content, please refer to
+[Neighborly's wiki](https://github.com/ShiJbey/neighborly/wiki) and the sample scripts
+in the [_samples_ directory](https://github.com/ShiJbey/neighborly/tree/main/samples).
+
+## Installation
+
+Neighborly is available to install from PyPI.
+
+```bash
+pip install neighborly
+```
+
+Or you can install it by cloning the main branch of this repo and installing that.
+
+```bash
+git clone https://github.com/ShiJbey/neighborly.git
+
+cd neighborly
+
+python -m pip install .
+```
+
+## Using as a library
+
+Neighborly can be used as a library within a Python script or package.
+The `samples` directory contains python scripts that use Neighborly this
+way. Please refer to them when creating new Plugins and other content.
+
+## Running the CLI
+
+Neighborly can be run as a module `$ python -m neighborly` or commandline `$ neighborly`
+script. If you require additional help while running, please use
+`python -m neighborly --help` or `neighborly --help`.
+
+By default, Neighborly runs a builtin version of **Talk of the Town**. However, you can
+configure the simulation settings by creating a `neighborlyconfig.yaml` file in
+the same directory where you're running the CLI. Please refer to the
+[wiki](https://github.com/ShiJbey/neighborly/wiki/Neighborly-CLI) for a list of
+valid configuration settings.
+
+When world generation concludes, Neighborly can write the final simulation data
+to a JSON file with the name of the town and the seed used for random number
+generation.
+
+## Running the Samples
+
+Neighborly provides sample simulations to show users how to customize
+it to create new story world themes.
+
+```bash
+# Make sure that you've activated your python virtual environment
+# Replace <sample_name>.py with the name of the
+# sample you want to run
+python ./samples/<sample_name>.py
+```
+
+## Installing for local development
+
+If you wish to download a Neighborly for local development, you need to clone/fork this
+repository and install using the _editable_ flag (-e). Please see the instructions
+below.
+
+```bash
+# Step One: Clone Repository
+git clone https://github.com/ShiJbey/neighborly.git
+
+# Step Two (Optional): Create and activate python virtual environment
+cd neighborly
+
+# For Linux and MacOS
+python3 -m venv venv
+source ./venv/bin/activate
+
+# For Windows
+python -m venv venv
+./venv/Scripts/Activate
+
+# Step Three: Install local build and dependencies
+python -m pip install -e "."
+```
+
+## Running the Tests
+
+The tests are currently out-of-date and may refer to systems
+and logic that no longer exists in Neighborly. The codebase
+changes so frequently that it hasn't been worth the time.
+As modules  become more established, I will add proper tests for them.
+Feel free to contribute tests by forking the repo, adding your test(s), and
+submitting a pull request with a description of your test cases. Your commits
+should only contain changes to files within the `tests` directory. If you
+change any files in other parts of the project, your PR will be rejected.
+
+Please follow the steps below to run Neighborly's test suite. Neighborly uses
+[PyTest](https://docs.pytest.org/en/7.1.x/) to handle unit testing.
+
+```bash
+# Step 1: Install dependencies for tests
+python -m pip install -e ".[tests]"
+
+# Step 2: Run Pytest
+pytest
+
+# Step3 : (Optional) Generate a test coverage report
+pytest --cov=neighborly tests/
+```
+
+# Documentation
+
+Neighborly uses [Numpy-style](https://numpydoc.readthedocs.io/en/latest/format.html)
+docstrings in code and full documentation can be found in the
+[Wiki](https://github.com/ShiJbey/neighborly/wiki).
+
+When adding docstrings for existing or new bits of code please use the following
+references for how to format your contributions:
+
+* [Sphinx Napoleon Plugin for processing Numpy Docstrings](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html)
+* [Example Numpy Style Docstrings](https://www.sphinx-doc.org/en/master/usage/extensions/example_numpy.html#example-numpy)
+
+# Contributing
+
+Here are some ways that people can contribute to Neighborly:
+
+1. Proposing/Implementing new features
+2. Fixing bugs
+3. Providing optimizations
+4. Fixing typos
+5. Filing issues
+6. Contributing tutorials/how-tos to the wiki
+7. Fixing grammar and spelling in the wiki
+8. Creating new samples/plugins
+
+If you are interested in contributing to Neighborly, there are multiple ways to get
+involved, and not all of them require you to be proficient with GitHub. Interested
+parties can contribute to the core code base of Neighborly and/or create nre content
+in the way of plugins. I love feedback, and if you have any questions, create a new
+issue, and I will do my best to answer. If you want to contribute to the core code,
+free to fork this repository, make your changes, and submit a pull-request with a
+description of your contribution. Please keep in mind that this project is a
+tool for creativity and learning. I have a [code of conduct](./CODE_OF_CONDUCT.md) to
+encourage healthy collaboration, and will enforce it if I need to.
+
+## Code Style
+
+Neighborly uses [_Black_](https://black.readthedocs.io/en/stable/) to handle code style
+and sorts imports using [_isort_](https://pycqa.github.io/isort/). You can follow
+[these instructions](https://black.readthedocs.io/en/stable/integrations/editors.html)
+for setting up both black and isort.
+
+# Notes
+
+## Non-Deterministic Behavior
+
+The goal of having a seeded pseudo random simulation is so that users experience
+deterministic behavior when using the same starting seed. I try to remove all forms of
+non-determinism, but some slip through. The known areas are listed below. If you find
+any, please make a new issue with details of the behavior.
+
+* Neighborly uses [Tracery](https://github.com/aparrish/pytracery) to generate names for
+characters and locations, and these names may not be consistent despite using the same
+rng seed value.
+
+## DMCA Statement
+
+Upon receipt of a notice alleging copyright infringement, I will take whatever action it
+deems appropriate within its sole discretion, including removal of the allegedly
+infringing materials.
+
+The repo image is something fun that I made. I love _The Simpsons_, and I couldn't think
+of anyone more neighborly than Ned Flanders. If the copyright owner for _The Simpsons_
+would like me to take it down, please contact me. The same takedown policy applies to
+any code samples inspired by TV shows, movies, and games.
```

### Comparing `neighborly-0.9.3/src/neighborly/__main__.py` & `neighborly-0.9.4/src/neighborly/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,269 +1,270 @@
-from __future__ import annotations
-
-import argparse
-import importlib
-import json
-import logging
-import os
-import pathlib
-import random
-import sys
-from typing import Any, Dict, List, Literal, Optional, Union
-
-import yaml
-from pydantic import BaseModel, Field
-
-import neighborly
-import neighborly.core.utils.utilities as utilities
-from neighborly.core.life_event import LifeEventLog
-from neighborly.exporter import NeighborlyJsonExporter
-from neighborly.server import NeighborlyServer
-from neighborly.simulation import Plugin, PluginSetupError, SimulationBuilder
-
-logger = logging.getLogger(__name__)
-
-
-class PluginConfig(BaseModel):
-    """
-    Settings for loading and constructing a plugin
-
-    Attributes
-    ----------
-    name: str
-        Name of the plugin to load
-    path: Optional[str]
-        The path where the plugin is located
-    options: Dict[str, Any]
-        Parameters to pass to the plugin when constructing
-        and loading it
-    """
-
-    name: str
-    path: Optional[str] = None
-    options: Dict[str, Any] = Field(default_factory=dict)
-
-
-class NeighborlyConfig(BaseModel):
-    """
-    Static configuration setting for the Neighborly
-
-    Attributes
-    ----------
-    simulation: SimulationConfig
-        Static configuration settings specifically for
-        the simulation instance
-    plugins: List[Union[str, PluginConfig]]
-        Names of plugins to load or names combined with
-        instantiation parameters
-    path: str
-        Path to the config file
-    """
-
-    quiet: bool = False
-    seed: int
-    hours_per_timestep: int
-    world_gen_start: str
-    world_gen_end: str
-    town_name: str
-    town_size: Literal["small", "medium", "large"]
-    plugins: List[Union[str, PluginConfig]] = Field(default_factory=list)
-    path: str = "."
-
-    @classmethod
-    def from_partial(
-        cls, data: Dict[str, Any], defaults: NeighborlyConfig
-    ) -> NeighborlyConfig:
-        """Construct new config from a default config and a partial set of parameters"""
-        return cls(**utilities.merge(data, defaults.dict()))
-
-
-def load_plugin(module_name: str, path: Optional[str] = None) -> Plugin:
-    """
-    Load a plugin
-
-    Parameters
-    ----------
-    module_name: str
-        Name of module to load
-    path: Optional[str]
-        Path where the Python module lives
-    """
-    path_prepended = False
-
-    if path:
-        path_prepended = True
-        plugin_abs_path = os.path.abspath(path)
-        sys.path.insert(0, plugin_abs_path)
-        logger.debug(f"Temporarily added plugin path '{plugin_abs_path}' to sys.path")
-
-    try:
-        plugin_module = importlib.import_module(module_name)
-        plugin: Plugin = plugin_module.__dict__["get_plugin"]()
-        return plugin
-    except KeyError:
-        raise PluginSetupError(
-            f"'get_plugin' function not found for plugin: {module_name}"
-        )
-    finally:
-        # Remove the given plugin path from the front
-        # of the system path to prevent module resolution bugs
-        if path_prepended:
-            sys.path.pop(0)
-
-
-def load_config_from_path(config_path: str) -> Dict[str, Any]:
-    """
-    This function loads the configuration file at the given path
-
-    Parameters
-    ----------
-    config_path: str
-        Path to a configuration file to load
-    """
-    path = pathlib.Path(os.path.abspath(config_path))
-
-    with open(path, "r") as f:
-        if path.suffix.lower() == ".json":
-            return json.load(f)
-        elif path.suffix.lower() == ".yaml":
-            return yaml.safe_load(f)
-        else:
-            raise ValueError(
-                f"Attempted to load config from incorrect file type: {path.suffix}."
-            )
-
-
-def try_load_local_config() -> Optional[Dict[str, Any]]:
-    """
-    Attempt to load a configuration file in the current working
-    directory.
-    """
-    config_load_precedence = [
-        os.path.join(os.getcwd(), "neighborlyconfig.yaml"),
-        os.path.join(os.getcwd(), "neighborlyconfig.yml"),
-        os.path.join(os.getcwd(), "neighborlyconfig.json"),
-    ]
-
-    for path in config_load_precedence:
-        if os.path.exists(path):
-            return load_config_from_path(path)
-
-    return None
-
-
-def get_arg_parser() -> argparse.ArgumentParser:
-    parser = argparse.ArgumentParser("Run Neighborly social simulation")
-    parser.add_argument(
-        "-v",
-        "--version",
-        action="store_true",
-        default=False,
-        help="Print the version of Neighborly",
-    )
-    parser.add_argument(
-        "-c",
-        "--config",
-        help="Path to the neighborlyconfig.yaml file to load for configuration",
-    )
-    parser.add_argument("-o", "--output", help="path to write final simulation state")
-    parser.add_argument(
-        "-d",
-        "--debug",
-        action="store_true",
-        default=False,
-        help="Print verbose debug output and save a log file",
-    )
-    parser.add_argument(
-        "--no-emit",
-        default=False,
-        action="store_true",
-        help="Disable creating an output file with the simulation's final state",
-    )
-    parser.add_argument(
-        "-q,",
-        "--quiet",
-        default=False,
-        action="store_true",
-        help="Disable all printing to stdout",
-    )
-    parser.add_argument(
-        "--server", default=False, action="store_true", help="Run web server UI"
-    )
-    return parser
-
-
-def main():
-    args = get_arg_parser().parse_args()
-
-    if args.version:
-        print(neighborly.__version__)
-        sys.exit(0)
-
-    if args.debug:
-        logging.basicConfig(
-            filename="neighborly.log", filemode="w", level=logging.DEBUG
-        )
-
-    config: NeighborlyConfig = NeighborlyConfig(
-        seed=random.randint(0, 999999),
-        hours_per_timestep=6,
-        world_gen_start="1839-08-19T00:00.000z",
-        world_gen_end="1979-08-19T00:00.000z",
-        town_size="medium",
-        town_name="#town_name#",
-        plugins=["neighborly.plugins.default_plugin", "neighborly.plugins.talktown"],
-    )
-
-    if args.config:
-        config = NeighborlyConfig.from_partial(
-            load_config_from_path(args.config), config
-        )
-        config.path = os.path.abspath(args.config)
-    else:
-        loaded_settings = try_load_local_config()
-        if loaded_settings:
-            logger.debug("Successfully loaded config from cwd.")
-            config = NeighborlyConfig.from_partial(loaded_settings, config)
-
-    sim_builder = SimulationBuilder(
-        seed=config.seed,
-        world_gen_start=config.world_gen_start,
-        world_gen_end=config.world_gen_end,
-        time_increment_hours=config.hours_per_timestep,
-    )
-
-    for plugin_entry in config.plugins:
-        if isinstance(plugin_entry, str):
-            plugin = load_plugin(plugin_entry)
-            sim_builder.add_plugin(plugin)
-        else:
-            plugin = load_plugin(plugin_entry.name, plugin_entry.path)
-            sim_builder.add_plugin(plugin, **plugin_entry.options)
-
-    sim = sim_builder.build()
-
-    config.quiet = args.quiet
-    if not config.quiet:
-        sim.world.get_resource(LifeEventLog).subscribe(lambda e: print(str(e)))
-
-    if args.server:
-        server = NeighborlyServer(sim)
-        server.run()
-    else:
-        sim.establish_setting()
-
-        if not args.no_emit:
-            output_path = (
-                args.output
-                if args.output
-                else f"{sim.seed}_{sim.town.name.replace(' ', '_')}.json"
-            )
-
-            with open(output_path, "w") as f:
-                data = NeighborlyJsonExporter().export(sim)
-                f.write(data)
-                logger.debug(f"Simulation data written to: '{output_path}'")
-
-
-if __name__ == "__main__":
-    main()
+from __future__ import annotations
+
+import argparse
+import importlib
+import json
+import logging
+import os
+import pathlib
+import random
+import sys
+from typing import Any, Dict, List, Literal, Optional, Union
+
+import yaml
+from pydantic import BaseModel, Field
+
+import neighborly
+import neighborly.core.utils.utilities as utilities
+from neighborly import SimDateTime
+from neighborly.exporter import NeighborlyJsonExporter
+from neighborly.simulation import Plugin, PluginSetupError, SimulationBuilder
+
+logger = logging.getLogger(__name__)
+
+
+class PluginConfig(BaseModel):
+    """
+    Settings for loading and constructing a plugin
+
+    Fields
+    ----------
+    name: str
+        Name of the plugin's python module
+    path: Optional[str]
+        The path where the plugin is located
+    options: Dict[str, Any]
+        Parameters to pass to the plugin when constructing
+        and loading it
+    """
+
+    name: str
+    path: Optional[str] = None
+    options: Dict[str, Any] = Field(default_factory=dict)
+
+
+class NeighborlyConfig(BaseModel):
+    """
+    Static configuration setting for the Neighborly
+
+    Fields
+    ----------
+    quiet: bool
+        Should the simulation not print to the console
+    seed: int
+        Seed used for random number generation
+    hours_per_timestep: str
+        How many hours elapse each simulation step
+    world_gen_start: str
+        Date when world generation starts (YYYY-MM-DD)
+    world_gen_end: str
+        Date when world generation ends (YYYY-MM-DD)
+    town_name: str
+        Name to give the generated town
+    town_size: Literal["small", "medium", "large"]
+        The size of th town to create
+    plugins: List[Union[str, PluginConfig]]
+        Names of plugins to load or names combined with
+        instantiation parameters
+    path: str
+        Path to the config file
+    """
+
+    quiet: bool = False
+    seed: Union[int, str]
+    hours_per_timestep: int
+    world_gen_start: str
+    world_gen_end: str
+    years_to_simulate: int
+    town_name: str
+    town_size: Literal["small", "medium", "large"]
+    plugins: List[Union[str, PluginConfig]] = Field(default_factory=list)
+    path: str = "."
+
+    @classmethod
+    def from_partial(
+        cls, data: Dict[str, Any], defaults: NeighborlyConfig
+    ) -> NeighborlyConfig:
+        """Construct new config from a default config and a partial set of parameters"""
+        return cls(**utilities.merge(data, defaults.dict()))
+
+
+def load_plugin(module_name: str, path: Optional[str] = None) -> Plugin:
+    """
+    Load a plugin
+
+    Parameters
+    ----------
+    module_name: str
+        Name of module to load
+    path: Optional[str]
+        Path where the Python module lives
+    """
+    path_prepended = False
+
+    if path:
+        path_prepended = True
+        plugin_abs_path = os.path.abspath(path)
+        sys.path.insert(0, plugin_abs_path)
+        logger.debug(f"Temporarily added plugin path '{plugin_abs_path}' to sys.path")
+
+    try:
+        plugin_module = importlib.import_module(module_name)
+        plugin: Plugin = getattr(plugin_module, "get_plugin")()
+        return plugin
+    except KeyError:
+        raise PluginSetupError(
+            f"'get_plugin' function not found for plugin: {module_name}"
+        )
+    finally:
+        # Remove the given plugin path from the front
+        # of the system path to prevent module resolution bugs
+        if path_prepended:
+            sys.path.pop(0)
+
+
+def load_config_from_path(config_path: str) -> Dict[str, Any]:
+    """
+    This function loads the configuration file at the given path
+
+    Parameters
+    ----------
+    config_path: str
+        Path to a configuration file to load
+    """
+    path = pathlib.Path(os.path.abspath(config_path))
+
+    with open(path, "r") as f:
+        if path.suffix.lower() == ".json":
+            return json.load(f)
+        elif path.suffix.lower() == ".yaml":
+            return yaml.safe_load(f)
+        else:
+            raise ValueError(
+                f"Attempted to load config from incorrect file type: {path.suffix}."
+            )
+
+
+def try_load_local_config() -> Optional[Dict[str, Any]]:
+    """
+    Attempt to load a configuration file in the current working
+    directory.
+    """
+    config_load_precedence = [
+        os.path.join(os.getcwd(), "neighborlyconfig.yaml"),
+        os.path.join(os.getcwd(), "neighborlyconfig.yml"),
+        os.path.join(os.getcwd(), "neighborlyconfig.json"),
+    ]
+
+    for path in config_load_precedence:
+        if os.path.exists(path):
+            return load_config_from_path(path)
+
+    return None
+
+
+def get_arg_parser() -> argparse.ArgumentParser:
+    parser = argparse.ArgumentParser("Run Neighborly social simulation")
+    parser.add_argument(
+        "-v",
+        "--version",
+        action="store_true",
+        default=False,
+        help="Print the version of Neighborly",
+    )
+    parser.add_argument(
+        "-c",
+        "--config",
+        help="Path to the neighborlyconfig.yaml file to load for configuration",
+    )
+    parser.add_argument("-o", "--output", help="path to write final simulation state")
+    parser.add_argument(
+        "-d",
+        "--debug",
+        action="store_true",
+        default=False,
+        help="Print verbose debug output and save a log file",
+    )
+    parser.add_argument(
+        "--no-emit",
+        default=False,
+        action="store_true",
+        help="Disable creating an output file with the simulation's final state",
+    )
+    parser.add_argument(
+        "-q,",
+        "--quiet",
+        default=False,
+        action="store_true",
+        help="Disable all printing to stdout",
+    )
+    return parser
+
+
+def main():
+    args = get_arg_parser().parse_args()
+
+    if args.version:
+        print(neighborly.__version__)
+        sys.exit(0)
+
+    if args.debug:
+        logging.basicConfig(
+            filename="neighborly.log", filemode="w", level=logging.DEBUG
+        )
+
+    config: NeighborlyConfig = NeighborlyConfig(
+        seed=random.randint(0, 999999),
+        hours_per_timestep=6,
+        world_gen_start="1839-08-19",
+        world_gen_end="1979-08-19",
+        years_to_simulate=100,
+        town_size="medium",
+        town_name="#town_name#",
+        plugins=["neighborly.plugins.defaults", "neighborly.plugins.talktown"],
+    )
+
+    if args.config:
+        config = NeighborlyConfig.from_partial(
+            load_config_from_path(args.config), config
+        )
+        config.path = os.path.abspath(args.config)
+    else:
+        loaded_settings = try_load_local_config()
+        if loaded_settings:
+            logger.debug("Successfully loaded config from cwd.")
+            config = NeighborlyConfig.from_partial(loaded_settings, config)
+
+    sim_builder = SimulationBuilder(
+        seed=config.seed,
+        starting_date=config.world_gen_start,
+        time_increment_hours=config.hours_per_timestep,
+        print_events=not args.quiet,
+    )
+
+    for plugin_entry in config.plugins:
+        if isinstance(plugin_entry, str):
+            plugin = load_plugin(plugin_entry)
+            sim_builder.add_plugin(plugin)
+        else:
+            plugin = load_plugin(plugin_entry.name, plugin_entry.path)
+            sim_builder.add_plugin(plugin, **plugin_entry.options)
+
+    sim = sim_builder.build()
+
+    sim.run_until(SimDateTime.from_str(config.world_gen_end))
+
+    if not args.no_emit:
+        output_path = (
+            args.output
+            if args.output
+            else f"{sim.seed}_{sim.town.name.replace(' ', '_')}.json"
+        )
+
+        with open(output_path, "w") as f:
+            data = NeighborlyJsonExporter().export(sim)
+            f.write(data)
+            logger.debug(f"Simulation data written to: '{output_path}'")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `neighborly-0.9.3/src/neighborly/core/business.py` & `neighborly-0.9.4/src/neighborly/core/business.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,563 +1,785 @@
-from __future__ import annotations
-
-import functools
-import logging
-import math
-from dataclasses import dataclass
-from enum import Enum, IntFlag
-from typing import Any, ClassVar, Dict, List, Optional, Protocol, Tuple
-
-from neighborly.core.character import GameCharacter
-from neighborly.core.ecs import Component, GameObject, World
-from neighborly.core.engine import NeighborlyEngine
-from neighborly.core.life_event import LifeEvent
-from neighborly.core.residence import Resident
-from neighborly.core.routine import RoutineEntry, RoutinePriority
-from neighborly.core.time import SimDateTime
-
-logger = logging.getLogger(__name__)
-
-
-class IOccupationPreconditionFn(Protocol):
-    """
-    A function that must evaluate to True for a character to
-    be eligible to hold the occupation.
-
-    Notes
-    -----
-    This was implemented using a Protocol because the
-    implementation of Callable from the typing module
-    does not have proper support for **kwargs
-    """
-
-    def __call__(self, world: World, gameobject: GameObject, **kwargs: Any) -> bool:
-        """
-        A function that must evaluate to True for a character to
-        be eligible to hold the occupation.
-
-        Arguments
-        ---------
-        world: World
-            The simulation's world instance
-        gameobject: GameObject
-            The GameObject to evaluate for the position
-
-        Returns
-        -------
-        bool: True if the character is eligible for the occupation
-            False otherwise
-        """
-        raise NotImplementedError()
-
-
-def join_preconditions(
-    *preconditions: IOccupationPreconditionFn,
-) -> IOccupationPreconditionFn:
-    """Join multiple occupation precondition functions into a single function"""
-
-    def wrapper(world: World, gameobject: GameObject, **kwargs: Any) -> bool:
-        return all([p(world, gameobject, **kwargs) for p in preconditions])
-
-    return wrapper
-
-
-def or_preconditions(
-    *preconditions: IOccupationPreconditionFn,
-) -> IOccupationPreconditionFn:
-    """Only one of the given preconditions has to pass to return True"""
-
-    def wrapper(world: World, gameobject: GameObject, **kwargs: Any) -> bool:
-        for p in preconditions:
-            if p(world, gameobject, **kwargs):
-                return True
-        return False
-
-    return wrapper
-
-
-@dataclass
-class OccupationType:
-    """
-    Shared information about all occupations with this type
-
-    Attributes
-    ----------
-    name: str
-        Name of the position
-    level: int
-        Prestige or socioeconomic status associated with the position
-    precondition: Optional[IOccupationPreconditionFn]
-        Function that determines of a candidate gameobject meets th requirements
-        of the occupation
-    """
-
-    name: str
-    level: int = 1
-    precondition: Optional[IOccupationPreconditionFn] = None
-
-    def fill_role(self, world: World, business: Business) -> Optional[Occupation]:
-        """
-        Attempt to find a component character that meets the preconditions
-        for this occupation
-        """
-        candidate_list: List[GameObject] = list(
-            filter(
-                lambda g: self.precondition(world, g) if self.precondition else True,
-                map(
-                    lambda res: world.get_gameobject(res[0]),
-                    world.get_components(GameCharacter, Resident),
-                ),
-            )
-        )
-
-        if any(candidate_list):
-            chosen_candidate = world.get_resource(NeighborlyEngine).rng.choice(
-                candidate_list
-            )
-            occupation = Occupation(self, business.id)
-            chosen_candidate.add_component(occupation)
-            return occupation
-        return None
-
-
-class OccupationTypeLibrary:
-    """Stores OccupationType instances mapped to strings for lookup at runtime"""
-
-    _registry: ClassVar[Dict[str, OccupationType]] = {}
-
-    @classmethod
-    def add(
-        cls,
-        occupation_type: OccupationType,
-        name: str = None,
-        overwrite_ok: bool = False,
-    ) -> None:
-        entry_key = name if name else occupation_type.name
-        # if entry_key in cls._registry and not overwrite_ok:
-        #     logger.warning(f"Attempted to overwrite OcuppationType: ({entry_key})")
-        #     return
-        cls._registry[entry_key] = occupation_type
-
-    @classmethod
-    def get(cls, name: str) -> OccupationType:
-        return cls._registry[name]
-
-
-class Occupation(Component):
-    """
-    Employment Information about a character
-    """
-
-    __slots__ = "_occupation_def", "_years_held", "_business"
-
-    _definition_registry: Dict[str, OccupationType] = {}
-
-    def __init__(
-        self,
-        occupation_type: OccupationType,
-        business: int,
-    ) -> None:
-        super().__init__()
-        self._occupation_def: OccupationType = occupation_type
-        self._business: int = business
-        self._years_held: float = 0.0
-
-    def to_dict(self) -> Dict[str, Any]:
-        return {
-            **super().to_dict(),
-            "occupation_def": self._occupation_def.name,
-            "business": self._business,
-            "years_held": self.get_years_held(),
-        }
-
-    def get_type(self) -> OccupationType:
-        return self._occupation_def
-
-    def get_business(self) -> int:
-        return self._business
-
-    def get_years_held(self) -> int:
-        return math.floor(self._years_held)
-
-    def increment_years_held(self, years: float) -> None:
-        self._years_held += years
-
-    @classmethod
-    def create(cls, world, business: int = -1, **kwargs) -> Occupation:
-        type_name = kwargs["name"]
-        level = kwargs.get("level", 1)
-        preconditions = kwargs.get("preconditions", [])
-        return Occupation(
-            cls.get_occupation_definition(type_name, level, preconditions),
-            business=business,
-        )
-
-    @classmethod
-    def get_occupation_definition(
-        cls, name: str, level: int, precondition: IOccupationPreconditionFn
-    ) -> OccupationType:
-        if name not in cls._definition_registry:
-            cls._definition_registry[name] = OccupationType(
-                name=name, level=level, precondition=precondition
-            )
-        return cls._definition_registry[name]
-
-    def on_remove(self) -> None:
-        """Run when the component is removed from the GameObject"""
-        world = self.gameobject.world
-        workplace = world.get_gameobject(self._business).get_component(Business)
-        if workplace.owner != self.gameobject.id:
-            workplace.remove_employee(self.gameobject.id)
-        else:
-            workplace.owner = None
-
-    def on_archive(self) -> None:
-        self.gameobject.remove_component(type(self))
-
-
-@dataclass
-class WorkHistoryEntry:
-    """Record of a job held by a character"""
-
-    occupation_type: str
-    business: int
-    start_date: SimDateTime
-    end_date: SimDateTime
-    reason_for_leaving: Optional[LifeEvent] = None
-
-    @property
-    def years_held(self) -> int:
-        return (self.start_date - self.end_date).years
-
-    def to_dict(self) -> Dict[str, Any]:
-        """Return dictionary representation for serialization"""
-
-        ret = {
-            "occupation_type": self.occupation_type,
-            "business": self.business,
-            "start_date": self.start_date.to_iso_str(),
-            "end_date": self.end_date.to_iso_str(),
-        }
-
-        if self.reason_for_leaving:
-            # This should probably point to a unique ID for the
-            # event, but we will leave it as the name of the event for now
-            ret["reason_for_leaving"] = self.reason_for_leaving.name
-
-        return ret
-
-
-class WorkHistory(Component):
-    """
-    Stores information about all the jobs that a character
-    has held
-
-    Attributes
-    ----------
-    _chronological_history: List[WorkHistoryEntry]
-        List of previous job in order from oldest to most recent
-    """
-
-    __slots__ = "_chronological_history", "_categorical_history"
-
-    def __init__(self) -> None:
-        super().__init__()
-        self._chronological_history: List[WorkHistoryEntry] = []
-        self._categorical_history: Dict[str, List[WorkHistoryEntry]] = {}
-
-    def add_entry(
-        self,
-        occupation_type: str,
-        business: int,
-        start_date: SimDateTime,
-        end_date: SimDateTime,
-        reason_for_leaving: Optional[LifeEvent] = None,
-    ) -> None:
-        """Add an entry to the work history"""
-        entry = WorkHistoryEntry(
-            occupation_type=occupation_type,
-            business=business,
-            start_date=start_date,
-            end_date=end_date,
-            reason_for_leaving=reason_for_leaving,
-        )
-
-        self._chronological_history.append(entry)
-
-        if occupation_type not in self._categorical_history:
-            self._categorical_history[occupation_type] = []
-
-        self._categorical_history[occupation_type].append(entry)
-
-    def has_experience_as_a(self, occupation_type: str) -> bool:
-        """Return True if the work history has an entry for a given occupation type"""
-        return occupation_type in self._categorical_history
-
-    def total_experience_as_a(self, occupation_type: str) -> int:
-        """Return the total years of experience someone has as a given occupation type"""
-        return functools.reduce(
-            lambda _sum, _entry: _sum + _entry.years_held,
-            self._categorical_history.get(occupation_type, []),
-            0,
-        )
-
-    def to_dict(self) -> Dict[str, Any]:
-        return {
-            **super().to_dict(),
-            "history": [entry.to_dict() for entry in self._chronological_history],
-        }
-
-    def __len__(self) -> int:
-        return len(self._chronological_history)
-
-
-class BusinessService(IntFlag):
-    NONE = 0
-    DRINKING = 1 << 0
-    BANKING = 1 << 1
-    COLLEGE_EDUCATION = 1 << 2
-    CONSTRUCTION = 1 << 3
-    COSMETICS = 1 << 4
-    CLOTHING = 1 << 5
-    FIRE_EMERGENCY = 1 << 6
-    FOOD = 1 << 7
-    HARDWARE = 1 << 8
-    HOME_IMPROVEMENT = 1 << 9
-    HOUSING = 1 << 10
-    LEGAL = 1 << 11
-    MEDICAL_EMERGENCY = 1 << 12
-    MORTICIAN = 1 << 13
-    RECREATION = 1 << 14
-    PUBLIC_SERVICE = 1 << 15
-    PRIMARY_EDUCATION = 1 << 16
-    REALTY = 1 << 17
-    SECONDARY_EDUCATION = 1 << 18
-    SHOPPING = 1 << 19
-    SOCIALIZING = 1 << 20
-    ERRANDS = 1 << 21
-
-
-class BusinessStatus(Enum):
-    PendingOpening = 0
-    OpenForBusiness = 1
-    ClosedForBusiness = 2
-
-
-class Business(Component):
-    __slots__ = (
-        "business_type",
-        "name",
-        "_years_in_business",
-        "operating_hours",
-        "_employees",
-        "_open_positions",
-        "owner",
-        "owner_type",
-        "status",
-        "services",
-    )
-
-    def __init__(
-        self,
-        business_type: str,
-        name: str,
-        owner_type: str = None,
-        owner: int = None,
-        open_positions: Dict[str, int] = None,
-        operating_hours: Dict[str, List[RoutineEntry]] = None,
-        services: BusinessService = BusinessService.NONE,
-    ) -> None:
-        super().__init__()
-        self.business_type: str = business_type
-        self.owner_type: Optional[str] = owner_type
-        self.name: str = name
-        # self._operating_hours: Dict[str, List[RoutineEntry]] = self._create_routines(
-        #     parse_schedule_str(business_def.hours)
-        # )
-        self.operating_hours: Dict[str, List[RoutineEntry]] = (
-            operating_hours if operating_hours else {}
-        )
-        self._open_positions: Dict[str, int] = open_positions if open_positions else {}
-        self._employees: Dict[int, str] = {}
-        self.owner: Optional[int] = owner
-        self.status: BusinessStatus = BusinessStatus.PendingOpening
-        self._years_in_business: float = 0.0
-        self.services: BusinessService = services
-
-    @property
-    def years_in_business(self) -> int:
-        return math.floor(self._years_in_business)
-
-    def to_dict(self) -> Dict[str, Any]:
-        return {
-            **super().to_dict(),
-            "business_type": self.business_type,
-            "name": self.name,
-            "operating_hours": self.operating_hours,
-            "open_positions": self.operating_hours,
-            "employees": self.get_employees(),
-            "owner": self.owner if self.owner is not None else -1,
-        }
-
-    def needs_owner(self) -> bool:
-        return self.owner is None and self.owner_type is not None
-
-    def get_open_positions(self) -> List[str]:
-        return [title for title, n in self._open_positions.items() if n > 0]
-
-    def get_employees(self) -> List[int]:
-        """Return a list of IDs for current employees"""
-        return list(self._employees.keys())
-
-    def add_employee(self, character: int, position: str) -> None:
-        """Add character to employees and remove a vacant position"""
-        self._employees[character] = position
-        self._open_positions[position] -= 1
-
-    def remove_employee(self, character: int) -> None:
-        """Remove a character as an employee and add a vacant position"""
-        position = self._employees[character]
-        del self._employees[character]
-        self._open_positions[position] += 1
-
-    def set_business_status(self, status: BusinessStatus) -> None:
-        self.status = status
-
-    def increment_years_in_business(self, years: float) -> None:
-        self._years_in_business += years
-
-    def __repr__(self) -> str:
-        """Return printable representation"""
-        return "Business(type='{}', name='{}', owner={}, employees={}, openings={})".format(
-            self.business_type,
-            self.name,
-            self.owner,
-            self._employees,
-            self._open_positions,
-        )
-
-    @classmethod
-    def create(cls, world: World, **kwargs) -> Business:
-        engine = world.get_resource(NeighborlyEngine)
-
-        business_type: str = kwargs["business_type"]
-        business_name: str = engine.name_generator.get_name(
-            kwargs.get("name_format", business_type)
-        )
-        owner_type: Optional[str] = kwargs.get("owner_type")
-        employee_types: Dict[str, int] = kwargs.get("employee_types", {})
-        services: BusinessService = kwargs.get("services", BusinessService.NONE)
-        operating_hours: Dict[str, List[RoutineEntry]] = to_operating_hours(
-            kwargs.get("hours", [])
-        )
-
-        return Business(
-            business_type=business_type,
-            name=business_name,
-            open_positions=employee_types,
-            services=services,
-            owner_type=owner_type,
-            operating_hours=operating_hours,
-        )
-
-    @staticmethod
-    def _create_routines(
-        times: Dict[str, Tuple[int, int]]
-    ) -> Dict[str, List[RoutineEntry]]:
-        """Create routine entries given tuples of time intervals mapped to days of the week"""
-        schedules: Dict[str, list[RoutineEntry]] = {}
-
-        for day, (opens, closes) in times.items():
-            routine_entries: List[RoutineEntry] = []
-
-            if opens > closes:
-                # Night shift business have their schedules
-                # split between two entries
-                routine_entries.append(
-                    RoutineEntry(
-                        start=opens,
-                        end=24,
-                        activity="working",
-                        location="work",
-                        priority=RoutinePriority.HIGH,
-                    )
-                )
-
-                routine_entries.append(
-                    RoutineEntry(
-                        start=0,
-                        end=closes,
-                        activity="working",
-                        location="work",
-                        priority=RoutinePriority.HIGH,
-                    )
-                )
-            elif opens < closes:
-                # Day shift business
-                routine_entries.append(
-                    RoutineEntry(
-                        start=opens,
-                        end=closes,
-                        activity="working",
-                        location="work",
-                        priority=RoutinePriority.HIGH,
-                    )
-                )
-            else:
-                raise ValueError("Opening and closing times must be different")
-
-            schedules[day] = routine_entries
-
-        return schedules
-
-
-def to_operating_hours(str_hours: List[str]) -> Dict[str, List[RoutineEntry]]:
-    """
-    Convert a list of string with times of day and convert
-    them to a list of RoutineEntries for when employees
-    should report to work and when a business is open to the
-    public.
-
-    Parameters
-    ----------
-    str_hours: List[str]
-        The times of day that this business is open
-
-    Returns
-    -------
-    List[RoutineEntry]
-        Routine entries for when this business is operational
-    """
-    times_to_intervals = {
-        "morning": (5, 12),
-        "late-morning": (11, 12),
-        "early-morning": (5, 8),
-        "day": (8, 11),
-        "afternoon": (12, 17),
-        "evening": (17, 21),
-        "night": (21, 23),
-    }
-
-    operating_hours: Dict[str, List[RoutineEntry]] = {
-        "monday": [],
-        "tuesday": [],
-        "wednesday": [],
-        "thursday": [],
-        "friday": [],
-        "saturday": [],
-        "sunday": [],
-    }
-
-    routines: List[RoutineEntry] = []
-
-    for time_of_day in str_hours:
-        try:
-            start, end = times_to_intervals[time_of_day]
-            routines.append(RoutineEntry(start, end, location="work", activity="work"))
-        except KeyError:
-            raise ValueError(f"{time_of_day} is not a valid time of day.")
-
-    for key in operating_hours:
-        operating_hours[key].extend(routines)
-
-    return operating_hours
+from __future__ import annotations
+
+import logging
+import math
+import re
+from abc import ABC
+from dataclasses import dataclass
+from typing import Any, Dict, List, Optional, Protocol, Set, Tuple
+
+from neighborly.builtin.components import Active
+from neighborly.core.character import GameCharacter
+from neighborly.core.ecs import Component, GameObject, World, component_info
+from neighborly.core.engine import NeighborlyEngine
+from neighborly.core.event import Event
+from neighborly.core.routine import (
+    Routine,
+    RoutineEntry,
+    RoutinePriority,
+    time_str_to_int,
+)
+from neighborly.core.time import SimDateTime, Weekday
+
+logger = logging.getLogger(__name__)
+
+
+@dataclass
+class BusinessInfo:
+    min_population: int
+    max_instances: int
+    demise: int
+
+
+__business_info_registry: Dict[str, BusinessInfo] = {}
+
+
+class IOccupationPreconditionFn(Protocol):
+    """
+    A function that must evaluate to True for an entity to
+    be eligible to hold the occupation.
+
+    Notes
+    -----
+    This was implemented using a Protocol because the
+    implementation of Callable from the typing module
+    does not have proper support for **kwargs
+    """
+
+    def __call__(self, world: World, gameobject: GameObject, **kwargs: Any) -> bool:
+        """
+        A function that must evaluate to True for an entity to
+        be eligible to hold the occupation.
+
+        Arguments
+        ---------
+        world: World
+            The simulation's world instance
+        gameobject: GameObject
+            The GameObject to evaluate for the position
+
+        Returns
+        -------
+        bool: True if the entity is eligible for the occupation
+            False otherwise
+        """
+        raise NotImplementedError()
+
+
+def join_preconditions(
+    *preconditions: IOccupationPreconditionFn,
+) -> IOccupationPreconditionFn:
+    """Join multiple occupation precondition functions into a single function"""
+
+    def wrapper(world: World, gameobject: GameObject, **kwargs: Any) -> bool:
+        return all([p(world, gameobject, **kwargs) for p in preconditions])
+
+    return wrapper
+
+
+def or_preconditions(
+    *preconditions: IOccupationPreconditionFn,
+) -> IOccupationPreconditionFn:
+    """Only one of the given preconditions has to pass to return True"""
+
+    def wrapper(world: World, gameobject: GameObject, **kwargs: Any) -> bool:
+        for p in preconditions:
+            if p(world, gameobject, **kwargs):
+                return True
+        return False
+
+    return wrapper
+
+
+@dataclass
+class OccupationType:
+    """
+    Shared information about all occupations with this type
+
+    Attributes
+    ----------
+    name: str
+        Name of the position
+    level: int
+        Prestige or socioeconomic status associated with the position
+    precondition: Optional[IOccupationPreconditionFn]
+        Function that determines of a candidate gameobject meets th requirements
+        of the occupation
+    """
+
+    name: str
+    level: int = 1
+    description: str = ""
+    precondition: Optional[IOccupationPreconditionFn] = None
+
+    def fill_role(
+        self, world: World, business: Business
+    ) -> Optional[Tuple[GameObject, Occupation]]:
+        """
+        Attempt to find a component entity that meets the preconditions
+        for this occupation
+        """
+        candidate_list: List[GameObject] = list(
+            filter(
+                lambda g: self.precondition(world, g) if self.precondition else True,
+                map(
+                    lambda res: world.get_gameobject(res[0]),
+                    world.get_components(GameCharacter, Unemployed, Active),
+                ),
+            )
+        )
+
+        if any(candidate_list):
+            chosen_candidate = world.get_resource(NeighborlyEngine).rng.choice(
+                candidate_list
+            )
+            return chosen_candidate, Occupation(
+                occupation_type=self.name,
+                business=business.gameobject.id,
+                level=self.level,
+                start_date=world.get_resource(SimDateTime).copy(),
+            )
+        return None
+
+    def fill_role_with(
+        self, world: World, business: Business, candidate: GameObject
+    ) -> Optional[Occupation]:
+        if self.precondition:
+            if self.precondition(world, candidate):
+                return Occupation(
+                    occupation_type=self.name,
+                    business=business.gameobject.id,
+                    level=self.level,
+                    start_date=world.get_resource(SimDateTime).copy(),
+                )
+            else:
+                return None
+        else:
+            return Occupation(
+                occupation_type=self.name,
+                business=business.gameobject.id,
+                level=self.level,
+                start_date=world.get_resource(SimDateTime).copy(),
+            )
+
+    def __repr__(self) -> str:
+        return f"OccupationType(name={self.name}, level={self.level})"
+
+
+class OccupationTypes:
+    """Stores OccupationType instances mapped to strings for lookup at runtime"""
+
+    _registry: Dict[str, OccupationType] = {}
+
+    @classmethod
+    def add(
+        cls,
+        occupation_type: OccupationType,
+        name: Optional[str] = None,
+    ) -> None:
+        entry_key = name if name else occupation_type.name
+        if entry_key in cls._registry:
+            logger.debug(f"Overwriting OccupationType: ({entry_key})")
+        cls._registry[entry_key] = occupation_type
+
+    @classmethod
+    def get(cls, name: str) -> OccupationType:
+        """
+        Get an OccupationType by name
+
+        Parameters
+        ----------
+        name: str
+            The registered name of the OccupationType
+
+        Returns
+        -------
+        OccupationType
+
+        Raises
+        ------
+        KeyError
+            When there is not an OccupationType
+            registered to that name
+        """
+        return cls._registry[name]
+
+
+class Occupation(Component):
+    """
+    Employment Information about an entity
+    """
+
+    __slots__ = "_occupation_type", "_years_held", "_business", "_level", "_start_date"
+
+    def __init__(
+        self,
+        occupation_type: str,
+        business: int,
+        level: int,
+        start_date: SimDateTime,
+    ) -> None:
+        super().__init__()
+        self._occupation_type: str = occupation_type
+        self._business: int = business
+        self._level: int = level
+        self._years_held: float = 0.0
+        self._start_date: SimDateTime = start_date
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            **super().to_dict(),
+            "occupation_type": self._occupation_type,
+            "level": self._level,
+            "business": self._business,
+            "years_held": self._years_held,
+        }
+
+    @property
+    def business(self) -> int:
+        return self._business
+
+    @property
+    def years_held(self) -> int:
+        return math.floor(self._years_held)
+
+    @property
+    def level(self) -> int:
+        return self._level
+
+    @property
+    def occupation_type(self) -> str:
+        return self._occupation_type
+
+    @property
+    def start_date(self) -> SimDateTime:
+        return self._start_date
+
+    def increment_years_held(self, years: float) -> None:
+        self._years_held += years
+
+    def __repr__(self) -> str:
+        return "Occupation(occupation_type={}, business={}, level={}, years_held={})".format(
+            self.occupation_type, self.business, self.level, self.years_held
+        )
+
+
+@dataclass
+class WorkHistoryEntry:
+    """Record of a job held by an entity"""
+
+    occupation_type: str
+    business: int
+    start_date: SimDateTime
+    end_date: SimDateTime
+    reason_for_leaving: Optional[Event] = None
+
+    @property
+    def years_held(self) -> int:
+        return (self.start_date - self.end_date).years
+
+    def to_dict(self) -> Dict[str, Any]:
+        """Return dictionary representation for serialization"""
+
+        ret = {
+            "occupation_type": self.occupation_type,
+            "business": self.business,
+            "start_date": self.start_date.to_iso_str(),
+            "end_date": self.end_date.to_iso_str(),
+        }
+
+        if self.reason_for_leaving:
+            # This should probably point to a unique ID for the
+            # event, but we will leave it as the name of the event for now
+            ret["reason_for_leaving"] = self.reason_for_leaving.name
+
+        return ret
+
+    def __repr__(self) -> str:
+        return (
+            "WorkHistoryEntry(type={}, business={}, start_date={}, end_date={})".format(
+                self.occupation_type,
+                self.business,
+                self.start_date.to_iso_str(),
+                self.end_date.to_iso_str() if self.end_date else "N/A",
+            )
+        )
+
+
+class WorkHistory(Component):
+    """
+    Stores information about all the jobs that an entity
+    has held
+
+    Attributes
+    ----------
+    _chronological_history: List[WorkHistoryEntry]
+        List of previous job in order from oldest to most recent
+    """
+
+    __slots__ = "_chronological_history", "_categorical_history"
+
+    def __init__(self) -> None:
+        super().__init__()
+        self._chronological_history: List[WorkHistoryEntry] = []
+        self._categorical_history: Dict[str, List[WorkHistoryEntry]] = {}
+
+    @property
+    def entries(self) -> List[WorkHistoryEntry]:
+        return self._chronological_history
+
+    def add_entry(
+        self,
+        occupation_type: str,
+        business: int,
+        start_date: SimDateTime,
+        end_date: SimDateTime,
+        reason_for_leaving: Optional[Event] = None,
+    ) -> None:
+        """Add an entry to the work history"""
+        entry = WorkHistoryEntry(
+            occupation_type=occupation_type,
+            business=business,
+            start_date=start_date,
+            end_date=end_date,
+            reason_for_leaving=reason_for_leaving,
+        )
+
+        self._chronological_history.append(entry)
+
+        if occupation_type not in self._categorical_history:
+            self._categorical_history[occupation_type] = []
+
+        self._categorical_history[occupation_type].append(entry)
+
+    def get_last_entry(self) -> Optional[WorkHistoryEntry]:
+        """Get the latest entry to WorkHistory"""
+        if self._chronological_history:
+            return self._chronological_history[-1]
+        return None
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            **super().to_dict(),
+            "history": [entry.to_dict() for entry in self._chronological_history],
+        }
+
+    def __len__(self) -> int:
+        return len(self._chronological_history)
+
+    def __repr__(self) -> str:
+        return "WorkHistory({})".format(
+            [e.__repr__() for e in self._chronological_history]
+        )
+
+
+class ServiceType:
+    """A service that can be offered by a business establishment"""
+
+    __slots__ = "_uid", "_name"
+
+    def __init__(self, uid: int, name: str) -> None:
+        self._uid = uid
+        self._name = name
+
+    @property
+    def uid(self) -> int:
+        return self._uid
+
+    @property
+    def name(self) -> str:
+        return self._name
+
+    def __hash__(self) -> int:
+        return self._uid
+
+    def __eq__(self, other: ServiceType) -> bool:
+        return self.uid == other.uid
+
+
+class ServiceTypes:
+    """
+    Repository of various services offered
+    """
+
+    _next_id: int = 1
+    _name_to_service: Dict[str, ServiceType] = {}
+    _id_to_name: Dict[int, str] = {}
+
+    @classmethod
+    def __contains__(cls, service_name: str) -> bool:
+        """Return True if a service type exists with the given name"""
+        return service_name.lower() in cls._name_to_service
+
+    @classmethod
+    def get(cls, service_name: str) -> ServiceType:
+        lc_service_name = service_name.lower()
+
+        if lc_service_name in cls._name_to_service:
+            return cls._name_to_service[lc_service_name]
+
+        uid = cls._next_id
+        cls._next_id = cls._next_id + 1
+        service_type = ServiceType(uid, lc_service_name)
+        cls._name_to_service[lc_service_name] = service_type
+        cls._id_to_name[uid] = lc_service_name
+
+
+class Services(Component):
+
+    __slots__ = "_services"
+
+    def __init__(self, services: Set[ServiceType]) -> None:
+        super().__init__()
+        self._services: Set[ServiceType] = services
+
+    def __contains__(self, service_name: str) -> bool:
+        return ServiceTypes.get(service_name) in self._services
+
+    def has_service(self, service: ServiceType) -> bool:
+        return service in self._services
+
+
+@component_info(
+    "Closed For Business",
+    "This business is no longer open and nobody works here.",
+)
+class ClosedForBusiness(Component):
+    pass
+
+
+@component_info(
+    "Open For Business",
+    "This business open for business and people can travel here.",
+)
+class OpenForBusiness(Component):
+
+    __slots__ = "duration"
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.duration: float = 0.0
+
+
+@component_info(
+    "Pending Opening",
+    "This business is built, but has no owner.",
+)
+class PendingOpening(Component):
+
+    __slots__ = "duration"
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.duration: float = 0.0
+
+
+class IBusinessType(Component, ABC):
+    """Empty interface for creating types of businesses like Restaurants, ETC"""
+
+    pass
+
+
+class Business(Component):
+    __slots__ = (
+        "operating_hours",
+        "_employees",
+        "_open_positions",
+        "owner",
+        "owner_type",
+    )
+
+    def __init__(
+        self,
+        owner_type: Optional[str] = None,
+        owner: Optional[int] = None,
+        open_positions: Optional[Dict[str, int]] = None,
+        operating_hours: Optional[Dict[Weekday, Tuple[int, int]]] = None,
+    ) -> None:
+        super().__init__()
+        self.owner_type: Optional[str] = owner_type
+        self.operating_hours: Dict[Weekday, Tuple[int, int]] = (
+            operating_hours if operating_hours else {}
+        )
+        self._open_positions: Dict[str, int] = open_positions if open_positions else {}
+        self._employees: Dict[int, str] = {}
+        self.owner: Optional[int] = owner
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            **super().to_dict(),
+            "operating_hours": self.operating_hours,
+            "open_positions": self._open_positions,
+            "employees": self.get_employees(),
+            "owner": self.owner if self.owner is not None else -1,
+            "owner_type": self.owner_type if self.owner_type is not None else "",
+        }
+
+    def needs_owner(self) -> bool:
+        return self.owner is None and self.owner_type is not None
+
+    def get_open_positions(self) -> List[str]:
+        return [title for title, n in self._open_positions.items() if n > 0]
+
+    def get_employees(self) -> List[int]:
+        """Return a list of IDs for current employees"""
+        return list(self._employees.keys())
+
+    def set_owner(self, owner: Optional[int]) -> None:
+        """Set the ID for the owner of the business"""
+        self.owner = owner
+
+    def add_employee(self, character: int, position: str) -> None:
+        """Add entity to employees and remove a vacant position"""
+        self._employees[character] = position
+        self._open_positions[position] -= 1
+
+    def remove_employee(self, character: int) -> None:
+        """Remove an entity as an employee and add a vacant position"""
+        position = self._employees[character]
+        del self._employees[character]
+        self._open_positions[position] += 1
+
+    def __repr__(self) -> str:
+        """Return printable representation"""
+        return "Business(owner={}, employees={}, openings={})".format(
+            self.owner,
+            self._employees,
+            self._open_positions,
+        )
+
+    @classmethod
+    def create(cls, world: World, **kwargs) -> Business:
+
+        owner_type: Optional[str] = kwargs.get("owner_type")
+        employee_types: Dict[str, int] = kwargs.get("employee_types", {})
+        operating_hours: Dict[Weekday, Tuple[int, int]] = parse_operating_hour_str(
+            kwargs.get("hours", "day")
+        )
+
+        return Business(
+            open_positions=employee_types,
+            owner_type=owner_type,
+            operating_hours=operating_hours,
+        )
+
+    def create_routines(self) -> Dict[Weekday, RoutineEntry]:
+        """Create routine entries given tuples of time intervals mapped to days of the week"""
+        routine_entries: Dict[Weekday, RoutineEntry] = {}
+
+        for day, (opens, closes) in self.operating_hours.items():
+            routine_entries[day] = RoutineEntry(
+                start=opens,
+                end=closes,
+                location=self.gameobject.id,
+                priority=RoutinePriority.HIGH,
+                tags=["work"],
+            )
+
+        return routine_entries
+
+
+@component_info(
+    "Unemployed",
+    "Character doesn't have a job",
+)
+class Unemployed(Component):
+    __slots__ = "duration_days"
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.duration_days: float = 0
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {**super().to_dict(), "duration_days": self.duration_days}
+
+
+@component_info(
+    "In the Workforce",
+    "This Character is eligible for employment opportunities.",
+)
+class InTheWorkforce(Component):
+    pass
+
+
+def start_job(
+    business: Business,
+    character: GameCharacter,
+    occupation: Occupation,
+    is_owner: bool = False,
+) -> None:
+    if is_owner:
+        business.owner = character.gameobject.id
+    else:
+        business.add_employee(character.gameobject.id, occupation.occupation_type)
+
+    character.gameobject.add_component(occupation)
+
+    if character.gameobject.has_component(Unemployed):
+        character.gameobject.remove_component(Unemployed)
+
+    character_routine = character.gameobject.get_component(Routine)
+    for day, interval in business.operating_hours.items():
+        character_routine.add_entries(
+            f"work_@_{business.gameobject.id}",
+            [day],
+            RoutineEntry(
+                start=interval[0],
+                end=interval[1],
+                location=business.gameobject.id,
+                priority=RoutinePriority.MED,
+            ),
+        )
+
+
+def end_job(business: Business, character: GameObject, occupation: Occupation) -> None:
+    world = character.world
+
+    if business.owner_type is not None and business.owner == character.id:
+        business.set_owner(None)
+    else:
+        business.remove_employee(character.id)
+
+    if not character.has_component(WorkHistory):
+        character.add_component(WorkHistory())
+
+    character.remove_component(Occupation)
+
+    character.get_component(WorkHistory).add_entry(
+        occupation_type=occupation.occupation_type,
+        business=business.gameobject.id,
+        start_date=occupation.start_date,
+        end_date=world.get_resource(SimDateTime).copy(),
+    )
+
+    # Remove routine entries
+    character_routine = character.get_component(Routine)
+    for day, _ in business.operating_hours.items():
+        character_routine.remove_entries(
+            [day],
+            f"work_@_{business.gameobject.id}",
+        )
+
+
+def parse_operating_hour_str(
+    operating_hours_str: str,
+) -> Dict[Weekday, Tuple[int, int]]:
+    """
+    Convert a string representing the hours of operation
+    for a business to a dictionary representing the days
+    of the week mapped to tuple time intervals for when
+    the business is open.
+
+    Parameters
+    ----------
+    operating_hours_str: str
+        String indicating the operating hours
+
+    Notes
+    -----
+    The following a re valid formats for the operating hours string
+    (1a interval 24HR) ## - ##
+        Opening hour - closing hour
+        Assumes that the business is open all days of the week
+    (1b interval 12HR AM/PM) ## AM - ## PM
+        Twelve-hour time interval
+    (2 interval-alias) "morning", "day", "night", or ...
+        Single string that maps to a preset time interval
+        Assumes that the business is open all days of the week
+    (3 days + interval) MTWRFSU: ## - ##
+        Specify the time interval and the specific days of the
+        week that the business is open
+    (4 days + interval-alias) MTWRFSU: "morning", or ...
+        Specify the days of the week and a time interval for
+        when the business will be open
+
+    Returns
+    -------
+    Dict[str, Tuple[int, int]]
+        Days of the week mapped to lists of time intervals
+    """
+
+    interval_aliases = {
+        "morning": (5, 12),
+        "late-morning": (11, 12),
+        "early-morning": (5, 8),
+        "day": (8, 11),
+        "afternoon": (12, 17),
+        "evening": (17, 21),
+        "night": (21, 23),
+    }
+
+    # time_alias = {
+    #     "early-morning": "02:00",
+    #     "dawn": "06:00",
+    #     "morning": "08:00",
+    #     "late-morning": "10:00",
+    #     "noon": "12:00",
+    #     "afternoon": "14:00",
+    #     "evening": "17:00",
+    #     "night": "21:00",
+    #     "midnight": "23:00",
+    # }
+
+    operating_hours_str = operating_hours_str.strip()
+
+    # Check for number interval
+    if match := re.fullmatch(
+        r"[0-2]?[0-9]\s*(PM|AM)?\s*-\s*[0-2]?[0-9]\s*(PM|AM)?", operating_hours_str
+    ):
+        interval_strs: List[str] = list(
+            map(lambda s: s.strip(), match.group(0).split("-"))
+        )
+
+        interval: Tuple[int, int] = (
+            time_str_to_int(interval_strs[0]),
+            time_str_to_int(interval_strs[1]),
+        )
+
+        if 23 < interval[0] < 0:
+            raise ValueError(f"Interval start not within bounds [0,23]: {interval}")
+        if 23 < interval[1] < 0:
+            raise ValueError(f"Interval end not within bounds [0,23]: {interval}")
+
+        return {d: interval for d in list(Weekday)}
+
+    # Check for interval alias
+    elif match := re.fullmatch(r"[a-zA-Z]+", operating_hours_str):
+        alias = match.group(0)
+        if alias in interval_aliases:
+            interval = interval_aliases[alias]
+            return {d: interval for d in list(Weekday)}
+        else:
+            raise ValueError(f"Invalid interval alias in: '{operating_hours_str}'")
+
+    # Check for days with number interval
+    elif match := re.fullmatch(
+        r"[MTWRFSU]+\s*:\s*[0-2]?[0-9]\s*-\s*[0-2]?[0-9]", operating_hours_str
+    ):
+        days_section, interval_section = tuple(match.group(0).split(":"))
+        days_section = days_section.strip()
+        interval_strs: List[str] = list(
+            map(lambda s: s.strip(), interval_section.strip().split("-"))
+        )
+        interval: Tuple[int, int] = (int(interval_strs[0]), int(interval_strs[1]))
+
+        if 23 < interval[0] < 0:
+            raise ValueError(f"Interval start not within bounds [0,23]: {interval}")
+        if 23 < interval[1] < 0:
+            raise ValueError(f"Interval end not within bounds [0,23]: {interval}")
+
+        return {Weekday.from_abbr(d): interval for d in days_section.strip()}
+
+    # Check for days with alias interval
+    elif match := re.fullmatch(r"[MTWRFSU]+\s*:\s*[a-zA-Z]+", operating_hours_str):
+        days_section, alias = tuple(match.group(0).split(":"))
+        days_section = days_section.strip()
+        alias = alias.strip()
+        if alias in interval_aliases:
+            interval = interval_aliases[alias]
+            return {Weekday.from_abbr(d): interval for d in days_section.strip()}
+        else:
+            raise ValueError(
+                f"Invalid interval alias ({alias}) in: '{operating_hours_str}'"
+            )
+
+    raise ValueError(f"Invalid operating hours string: '{operating_hours_str}'")
```

### Comparing `neighborly-0.9.3/src/neighborly/core/ecs.py` & `neighborly-0.9.4/src/neighborly/core/ecs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,421 +1,398 @@
-"""
-Custom Entity-Component implementation that blends
-the Unity-style GameObjects with the ECS logic from the
-Python esper library and the Bevy Game Engine.
-
-Sources:
-https://docs.unity3d.com/ScriptReference/GameObject.html
-https://github.com/benmoran56/esper
-https://github.com/bevyengine/bevy
-"""
-from __future__ import annotations
-
-import hashlib
-import logging
-from abc import ABC
-from typing import Any, Dict, Iterable, List, Optional, Tuple, Type, TypeVar
-from uuid import uuid1
-
-import esper
-
-logger = logging.getLogger(__name__)
-
-_CT = TypeVar("_CT", bound="Component")
-_RT = TypeVar("_RT", bound="Any")
-
-
-class GameObject:
-    """
-    Collections of components that share are unique identifier
-    and represent entities within the game world
-
-    Attributes
-    ----------
-    id: int
-        unique identifier
-    name: str
-        name of the GameObject
-    world: World
-        the World instance this GameObject belongs to
-    components: List[Components]
-        Components attached to this GameObject
-    """
-
-    __slots__ = (
-        "_id",
-        "_name",
-        "_components",
-        "_world",
-        "_archetype",
-    )
-
-    def __init__(
-        self,
-        unique_id: Optional[int] = None,
-        name: str = "GameObject",
-        components: Iterable[Component] = (),
-        world: Optional[World] = None,
-        archetype: Optional[EntityArchetype] = None,
-    ) -> None:
-        self._name: str = name
-        self._id: int = unique_id if unique_id else self.generate_id()
-        self._world: Optional[World] = world
-        self._components: Dict[Type[_CT], Component] = {}
-        self._archetype: Optional[EntityArchetype] = archetype
-
-        if components:
-            for component in components:
-                self.add_component(component)
-
-    @property
-    def id(self) -> int:
-        """Return GameObject's ID"""
-        return self._id
-
-    @property
-    def name(self) -> str:
-        """Get the name of the GameObject"""
-        return self._name
-
-    @property
-    def archetype(self) -> Optional[EntityArchetype]:
-        """Return the name of the archetype for creating this GameObject"""
-        return self._archetype
-
-    @property
-    def world(self) -> World:
-        """Return the world that this GameObject belongs to"""
-        if self._world:
-            return self._world
-        raise TypeError("World is None for GameObject")
-
-    @property
-    def components(self) -> List[Component]:
-        return list(self._components.values())
-
-    def set_world(self, world: Optional[World]) -> None:
-        """set the world instance"""
-        self._world = world
-
-    def add_component(self, component: Component) -> GameObject:
-        """Add a component to this GameObject"""
-        component.set_gameobject(self)
-        self._components[type(component)] = component
-        self.world.ecs.add_component(self.id, component)
-        component.on_add()
-        return self
-
-    def remove_component(self, component_type: Type[_CT]) -> None:
-        """Add a component to this GameObject"""
-        component = self._components[component_type]
-        component.on_remove()
-        self.world.ecs.remove_component(self.id, component_type)
-        del self._components[component_type]
-
-    def get_component(self, component_type: Type[_CT]) -> _CT:
-        return self._components[component_type]
-
-    def has_component(self, *component_type: Type[_CT]) -> bool:
-        return all([ct in self._components for ct in component_type])
-
-    def try_component(self, component_type: Type[_CT]) -> Optional[_CT]:
-        return self._components.get(component_type)
-
-    def archive(self) -> None:
-        """
-        Deactivates the GameObject by removing excess components.
-
-        The GameObject stays in the ECS though.
-        """
-        for component in self.components:
-            component.on_archive()
-
-    def to_dict(self) -> Dict[str, Any]:
-        return {
-            "id": self.id,
-            "name": self.name,
-            "components": [c.to_dict() for c in self._components.values()],
-            "archetype": self.archetype.name if self.archetype else "",
-        }
-
-    def __hash__(self) -> int:
-        return self._id
-
-    @staticmethod
-    def generate_id() -> int:
-        """Create a new unique int ID"""
-        return int.from_bytes(hashlib.sha256(uuid1().bytes).digest()[:8], "little")
-
-
-class Component(ABC):
-    """
-    Components are collections of related data attached to GameObjects.
-
-    Attributes
-    ----------
-    _gameobject: Optional[GameObject]
-        Reference to the gameobject this component is attached to
-    """
-
-    __slots__ = "_gameobject"
-
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__()
-        self._gameobject: Optional[GameObject] = None
-
-    @property
-    def gameobject(self) -> GameObject:
-        """Returns the GameObject this component is attached to"""
-        if self._gameobject is None:
-            raise TypeError("Component's GameObject is None")
-        return self._gameobject
-
-    def set_gameobject(self, gameobject: Optional[GameObject]) -> None:
-        """set the gameobject instance for this component"""
-        self._gameobject = gameobject
-
-    def on_add(self) -> None:
-        """Run when the component is added to the GameObject"""
-        return
-
-    def on_remove(self) -> None:
-        """Run when the component is removed from the GameObject"""
-        return
-
-    def on_archive(self) -> None:
-        """Run when the GameObject this is connected to is archived"""
-        return
-
-    @classmethod
-    def create(cls, world: World, **kwargs) -> Component:
-        """Create an instance of the component using a reference to the World object and additional parameters"""
-        return cls(**kwargs)
-
-    def to_dict(self) -> Dict[str, Any]:
-        """Serialize the component to a dict"""
-        return {"type": self.__class__.__name__}
-
-
-class ISystem(ABC, esper.Processor):
-    world: World
-
-    def __init__(self):
-        super().__init__()
-
-
-class World:
-    """
-    Manages Gameobjects, Systems, and resources for the simulation
-
-    Attributes
-    ----------
-    _ecs: esper.World
-        Esper ECS instance used for efficiency
-    _gameobjects: Dict[int, GameObject]
-        Mapping of GameObjects to unique identifiers
-    _dead_gameobjects: List[int]
-        List of identifiers for GameObject to remove after
-        the latest time step
-    _resources: Dict[Type, Any]
-        Global resources shared by systems in the ECS
-    """
-
-    __slots__ = (
-        "_ecs",
-        "_gameobjects",
-        "_dead_gameobjects",
-        "_resources",
-    )
-
-    def __init__(self) -> None:
-        self._ecs: esper.World = esper.World()
-        self._gameobjects: Dict[int, GameObject] = {}
-        self._dead_gameobjects: List[int] = []
-        self._resources: Dict[str, Any] = {}
-
-    @property
-    def ecs(self) -> esper.World:
-        return self._ecs
-
-    def spawn_gameobject(
-        self, *components: Component, name: Optional[str] = None
-    ) -> GameObject:
-        """Create a new gameobject and attach any given component instances"""
-        entity_id = self._ecs.create_entity(*components)
-        gameobject = GameObject(
-            unique_id=entity_id,
-            components=components,
-            world=self,
-            name=(name if name else f"GameObject({entity_id})"),
-        )
-        self._gameobjects[gameobject.id] = gameobject
-        return gameobject
-
-    def spawn_archetype(self, archetype: EntityArchetype) -> GameObject:
-        component_instances: List[Component] = []
-        for component_type, options in archetype.components.items():
-            component_instances.append(component_type.create(self, **options))
-
-        entity_id = self._ecs.create_entity(*component_instances)
-        gameobject = GameObject(
-            unique_id=entity_id,
-            components=component_instances,
-            world=self,
-            name=f"{archetype.name}({entity_id})",
-            archetype=archetype,
-        )
-
-        archetype.increment_instances()
-
-        self._gameobjects[gameobject.id] = gameobject
-
-        return gameobject
-
-    def get_gameobject(self, gid: int) -> GameObject:
-        """Retrieve the GameObject with the given id"""
-        return self._gameobjects[gid]
-
-    def get_gameobjects(self) -> List[GameObject]:
-        """Get all gameobjects"""
-        return list(self._gameobjects.values())
-
-    def has_gameobject(self, gid: int) -> bool:
-        """Check that a GameObject with the given id exists"""
-        return gid in self._gameobjects
-
-    def try_gameobject(self, gid: int) -> Optional[GameObject]:
-        """Retrieve the GameObject with the given id"""
-        return self._gameobjects.get(gid)
-
-    def delete_gameobject(self, gid: int) -> None:
-        """Remove gameobject from world"""
-        self._ecs.delete_entity(gid)
-        self._dead_gameobjects.append(gid)
-
-    def get_component(self, component_type: Type[_CT]) -> List[Tuple[int, _CT]]:
-        """Get all the gameobjects that have a given component type"""
-        return self._ecs.get_component(component_type)
-
-    def get_components(
-        self, *component_types: Type[_CT]
-    ) -> List[Tuple[int, List[_CT, ...]]]:
-        """Get all game objects with the given components"""
-        return self._ecs.get_components(*component_types)
-
-    def try_components(
-        self, entity: int, *component_types: Type[_CT]
-    ) -> Optional[List[List[_CT]]]:
-        """Try to get a multiple component types for a GameObject."""
-        return self._ecs.try_components(entity, *component_types)
-
-    def _clear_dead_gameobjects(self) -> None:
-        """Delete gameobjects that were removed from the world"""
-        for gameobject_id in self._dead_gameobjects:
-            gameobject = self._gameobjects[gameobject_id]
-            for component in gameobject.components:
-                component.on_remove()
-            if gameobject.archetype:
-                gameobject.archetype.decrement_instances()
-            gameobject.set_world(None)
-            del self._gameobjects[gameobject_id]
-
-        self._dead_gameobjects.clear()
-
-    def add_system(self, system: ISystem, priority: int = 0) -> None:
-        """Add a System instance to the World"""
-        self._ecs.add_processor(system, priority=priority)
-        system.world = self
-
-    def remove_system(self, system: Type[ISystem]) -> None:
-        """Remove a System from the World"""
-        self._ecs.remove_processor(system)
-        system.world = None
-
-    def step(self, **kwargs) -> None:
-        """Call the process method on all systems"""
-        self._clear_dead_gameobjects()
-        self._ecs.process(**kwargs)
-
-    def add_resource(self, resource: Any) -> None:
-        """Add a global resource to the world"""
-        resource_type = type(resource)
-        if resource_type in self._resources:
-            logger.warning(f"Replacing existing resource of type: {resource_type}")
-        self._resources[resource_type] = resource
-
-    def remove_resource(self, resource_type: Any) -> None:
-        """remove a global resource to the world"""
-        del self._resources[resource_type]
-
-    def get_resource(self, resource_type: Type[_RT]) -> _RT:
-        """Add a global resource to the world"""
-        return self._resources[resource_type]
-
-    def has_resource(self, resource_type: Any) -> bool:
-        """Return true if the world has the given resource"""
-        return resource_type in self._resources
-
-    def __repr__(self) -> str:
-        return "World(gameobjects={}, resources={})".format(
-            len(self._gameobjects),
-            list(self._resources.values()),
-        )
-
-
-class EntityArchetype:
-    """
-    Organizes information for constructing components that compose GameObjects.
-
-    Attributes
-    ----------
-    _name: str
-        (Read-only) The name of the entity archetype
-    _components: Dict[Type[Component], Dict[str, Any]]
-        Dict of components used to construct this archetype
-    """
-
-    __slots__ = "_name", "_components", "_instances"
-
-    def __init__(self, name: str) -> None:
-        self._name: str = name
-        self._components: Dict[Type[Component], Dict[str, Any]] = {}
-        self._instances: int = 0
-
-    @property
-    def name(self) -> str:
-        """Returns the name of this archetype"""
-        return self._name
-
-    @property
-    def components(self) -> Dict[Type[Component], Dict[str, Any]]:
-        """Returns a list of components in this archetype"""
-        return {**self._components}
-
-    @property
-    def instances(self) -> int:
-        return self._instances
-
-    def add(self, component_type: Type[Component], **kwargs: Any) -> EntityArchetype:
-        """
-        Add a component to this archetype
-
-        Parameters
-        ----------
-        component_type: subclass of neighborly.core.ecs.Component
-            The component type to add to the entity archetype
-        **kwargs: Dict[str, Any]
-            Attribute overrides to pass to the component
-        """
-        self._components[component_type] = {**kwargs}
-        return self
-
-    def increment_instances(self) -> None:
-        self._instances += 1
-
-    def decrement_instances(self) -> None:
-        self._instances -= 1
-
-    def __repr__(self) -> str:
-        return "{}(name={}, components={})".format(
-            self.__class__.__name__, self._name, self._components
-        )
+"""
+Custom Entity-Component implementation that blends
+the Unity-style GameObjects with the ECS logic from the
+Python esper library and the Bevy Game Engine.
+
+Sources:
+https://docs.unity3d.com/ScriptReference/GameObject.html
+https://github.com/benmoran56/esper
+https://github.com/bevyengine/bevy
+"""
+from __future__ import annotations
+
+import logging
+from abc import ABC
+from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Type, TypeVar
+
+import esper
+
+logger = logging.getLogger(__name__)
+
+
+# Store string names of components for lookup later
+_component_names: Dict[Type[Component], str] = {}
+
+
+# Text descriptions of components (mostly used by GUI applications)
+_component_descriptions: Dict[Type[Component], str] = {}
+
+
+_CT = TypeVar("_CT", bound="Component")
+_RT = TypeVar("_RT", bound="Any")
+_ST = TypeVar("_ST", bound="ISystem")
+
+
+class ResourceNotFoundError(Exception):
+    def __init__(self, resource_type: Type[Any]) -> None:
+        super().__init__()
+        self.resource_type: Type = resource_type
+        self.message = f"Could not find resource with type: {resource_type.__name__}"
+
+    def __str__(self) -> str:
+        return self.message
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}({self.resource_type})"
+
+
+class GameObjectNotFoundError(Exception):
+    def __init__(self, gid: int) -> None:
+        super().__init__()
+        self.gid: int = gid
+        self.message = f"Could not find GameObject with id: {gid}."
+
+    def __str__(self) -> str:
+        return self.message
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}({self.gid})"
+
+
+class ComponentNotFoundError(Exception):
+    def __init__(self, component_type: Type[Component]) -> None:
+        super().__init__()
+        self.component_type: Type[Component] = component_type
+        self.message = f"Could not find Component with type: {component_type.__name__}."
+
+    def __str__(self) -> str:
+        return self.message
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}({self.component_type})"
+
+
+class GameObject:
+    """
+    Collections of components that share are unique identifier
+    and represent entities within the game world
+
+    Attributes
+    ----------
+    id: int
+      unique identifier
+    _name: str
+        name of the GameObject
+    _world: World
+        the World instance this GameObject belongs to
+    _components: List[Components]
+        Components attached to this GameObject
+    """
+
+    __slots__ = "_id", "_name", "_components", "_world"
+
+    def __init__(
+        self,
+        unique_id: int,
+        world: World,
+        name: Optional[str] = None,
+        components: Optional[Iterable[Component]] = None,
+    ) -> None:
+        self._name: str = name if name else f"GameObject ({unique_id})"
+        self._id: int = unique_id
+        self._world: World = world
+        self._components: Dict[Type[Component], Component] = {}
+
+        if components:
+            for component in components:
+                self.add_component(component)
+
+    @property
+    def id(self) -> int:
+        """Return GameObject's ID"""
+        return self._id
+
+    @property
+    def name(self) -> str:
+        """Get the name of the GameObject"""
+        return self._name
+
+    @property
+    def world(self) -> World:
+        """Return the world that this GameObject belongs to"""
+        return self._world
+
+    @property
+    def components(self) -> List[Component]:
+        """Returns the component instances associated with this GameObject"""
+        return list(self._components.values())
+
+    def get_component_types(self) -> List[Type[Component]]:
+        """Returns the types of components attached to this character"""
+        return list(self._components.keys())
+
+    def add_component(self, component: Component) -> GameObject:
+        """Add a component to this GameObject"""
+        component.set_gameobject(self)
+        self._components[type(component)] = component
+        self.world.ecs.add_component(self.id, component)
+        return self
+
+    def remove_component(self, component_type: Type[Component]) -> None:
+        """Add a component to this GameObject"""
+        if not self.has_component(component_type):
+            return
+        del self._components[component_type]
+        self.world.ecs.remove_component(self.id, component_type)
+
+    def get_component(self, component_type: Type[_CT]) -> _CT:
+        try:
+            return self._components[component_type]  # type: ignore
+        except KeyError:
+            raise ComponentNotFoundError(component_type)
+
+    def has_component(self, *component_type: Type[Component]) -> bool:
+        return all([ct in self._components for ct in component_type])
+
+    def try_component(self, component_type: Type[_CT]) -> Optional[_CT]:
+        return self._components.get(component_type)  # type: ignore
+
+    def to_dict(self) -> Dict[str, Any]:
+        ret = {
+            "id": self.id,
+            "name": self.name,
+            "components": [c.to_dict() for c in self._components.values()],
+        }
+
+        return ret
+
+    def pprint(self) -> None:
+        print(f"== GameObject({self.id}) ==\n")
+        for c in self.components:
+            c.pprint()
+
+    def __hash__(self) -> int:
+        return self._id
+
+    def __str__(self) -> str:
+        return f"GameObject(id={self.id})"
+
+    def __repr__(self) -> str:
+        return f"GameObject(id={self.id})"
+
+
+class Component(ABC):
+    """
+    Components are collections of related data attached to GameObjects.
+
+    Attributes
+    ----------
+    _gameobject: Optional[GameObject]
+        Reference to the gameobject this component is attached to
+    """
+
+    __slots__ = "_gameobject"
+
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__()
+        self._gameobject: Optional[GameObject] = None
+
+    @property
+    def gameobject(self) -> GameObject:
+        """Returns the GameObject this component is attached to"""
+        if self._gameobject is None:
+            raise TypeError("Component's GameObject is None")
+        return self._gameobject
+
+    def set_gameobject(self, gameobject: Optional[GameObject]) -> None:
+        """set the gameobject instance for this component"""
+        self._gameobject = gameobject
+
+    def pprint(self) -> None:
+        print(f"{self.__class__.__name__}:\n")
+
+    @classmethod
+    def create(cls, world: World, **kwargs) -> Component:
+        """Create an instance of the component using a reference to the World object and additional parameters"""
+        return cls(**kwargs)
+
+    def to_dict(self) -> Dict[str, Any]:
+        """Serialize the component to a dict"""
+        return {"type": self.__class__.__name__}
+
+    def __repr__(self) -> str:
+        return "{}".format(self.__class__.__name__)
+
+
+def component_info(
+    name: Optional[str] = None,
+    description: Optional[str] = None,
+) -> Callable[[Type[_CT]], Type[_CT]]:
+    """Decorator that registers a name for this component"""
+
+    def decorator(cls: Type[_CT]) -> Type[_CT]:
+        if name is not None:
+            _component_names[cls] = name
+        if description is not None:
+            _component_descriptions[cls] = description
+        return cls
+
+    return decorator
+
+
+class ISystem(ABC, esper.Processor):
+    world: World
+
+    def __init__(self):
+        super().__init__()
+
+
+class World:
+    """
+    Manages Gameobjects, Systems, and resources for the simulation
+
+    Attributes
+    ----------
+    _ecs: esper.World
+        Esper ECS instance used for efficiency
+    _gameobjects: Dict[int, GameObject]
+        Mapping of GameObjects to unique identifiers
+    _dead_gameobjects: List[int]
+        List of identifiers for GameObject to remove after
+        the latest time step
+    _resources: Dict[Type, Any]
+        Global resources shared by systems in the ECS
+    """
+
+    __slots__ = (
+        "_ecs",
+        "_gameobjects",
+        "_dead_gameobjects",
+        "_resources",
+    )
+
+    def __init__(self) -> None:
+        self._ecs: esper.World = esper.World()
+        self._gameobjects: Dict[int, GameObject] = {}
+        self._dead_gameobjects: List[int] = []
+        self._resources: Dict[Type[Any], Any] = {}
+
+    @property
+    def ecs(self) -> esper.World:
+        return self._ecs
+
+    def spawn_gameobject(
+        self, components: Optional[List[Component]] = None, name: Optional[str] = None
+    ) -> GameObject:
+        """Create a new gameobject and attach any given component instances"""
+        entity_id = self._ecs.create_entity(*components if components else [])
+        gameobject = GameObject(
+            unique_id=entity_id,
+            components=components,
+            world=self,
+            name=(name if name else f"GameObject({entity_id})"),
+        )
+        self._gameobjects[gameobject.id] = gameobject
+        return gameobject
+
+    def get_gameobject(self, gid: int) -> GameObject:
+        """Retrieve the GameObject with the given id"""
+        try:
+            return self._gameobjects[gid]
+        except KeyError:
+            raise GameObjectNotFoundError(gid)
+
+    def get_gameobjects(self) -> List[GameObject]:
+        """Get all gameobjects"""
+        return list(self._gameobjects.values())
+
+    def has_gameobject(self, gid: int) -> bool:
+        """Check that a GameObject with the given id exists"""
+        return gid in self._gameobjects
+
+    def try_gameobject(self, gid: int) -> Optional[GameObject]:
+        """Retrieve the GameObject with the given id"""
+        return self._gameobjects.get(gid)
+
+    def delete_gameobject(self, gid: int) -> None:
+        """Remove gameobject from world"""
+        self._dead_gameobjects.append(gid)
+
+    def get_component(self, component_type: Type[_CT]) -> List[Tuple[int, _CT]]:
+        """Get all the gameobjects that have a given component type"""
+        return self._ecs.get_component(component_type)
+
+    def get_components(
+        self, *component_types: Type[_CT]
+    ) -> List[Tuple[int, List[_CT]]]:
+        """Get all game objects with the given components"""
+        return self._ecs.get_components(*component_types)
+
+    def _clear_dead_gameobjects(self) -> None:
+        """Delete gameobjects that were removed from the world"""
+        for gameobject_id in self._dead_gameobjects:
+            gameobject = self._gameobjects[gameobject_id]
+            del self._gameobjects[gameobject_id]
+
+            # You need to check if the gameobject has any components
+            # If it doesn't then esper will not have it stored
+            if gameobject.components:
+                self._ecs.delete_entity(gameobject_id, True)
+
+        self._dead_gameobjects.clear()
+
+    def add_system(self, system: ISystem, priority: int = 0) -> None:
+        """Add a System instance to the World"""
+        self._ecs.add_processor(system, priority=priority)
+        system.world = self
+
+    def get_system(self, system_type: Type[_ST]) -> Optional[_ST]:
+        """Get a System of the given type"""
+        return self._ecs.get_processor(system_type)
+
+    def remove_system(self, system: Type[ISystem]) -> None:
+        """Remove a System from the World"""
+        self._ecs.remove_processor(system)
+
+    def step(self, **kwargs) -> None:
+        """Call the process method on all systems"""
+        self._clear_dead_gameobjects()
+        self._ecs.process(**kwargs)
+
+    def add_resource(self, resource: Any) -> None:
+        """Add a global resource to the world"""
+        resource_type = type(resource)
+        if resource_type in self._resources:
+            logger.warning(f"Replacing existing resource of type: {resource_type}")
+        self._resources[resource_type] = resource
+
+    def remove_resource(self, resource_type: Any) -> None:
+        """remove a global resource to the world"""
+        try:
+            del self._resources[resource_type]
+        except KeyError:
+            raise ResourceNotFoundError(resource_type)
+
+    def get_resource(self, resource_type: Type[_RT]) -> _RT:
+        """Add a global resource to the world"""
+        try:
+            return self._resources[resource_type]
+        except KeyError:
+            raise ResourceNotFoundError(resource_type)
+
+    def has_resource(self, resource_type: Any) -> bool:
+        """Return true if the world has the given resource"""
+        return resource_type in self._resources
+
+    def try_resource(self, resource_type: Type[_RT]) -> Optional[_RT]:
+        """Attempt to get resource with type. Return None if not found"""
+        return self._resources.get(resource_type)
+
+    def get_all_resources(self) -> List[Any]:
+        """Get all resources attached to this World instance"""
+        return list(self._resources.values())
+
+    def __repr__(self) -> str:
+        return "World(gameobjects={}, resources={})".format(
+            len(self._gameobjects),
+            list(self._resources.values()),
+        )
```

### Comparing `neighborly-0.9.3/src/neighborly/core/engine.py` & `neighborly-0.9.4/src/neighborly/core/engine.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,45 @@
-from __future__ import annotations
-
-import random
-from typing import Dict, Optional, Type
-
-import neighborly.core.utils.tracery as tracery
-from neighborly.core.ecs import Component
-from neighborly.core.name_generation import TraceryNameFactory
-
-
-class NeighborlyEngine:
-    """
-    An engine stores and instantiates entity archetypes for characters, businesses,
-    residences, and other places.
-
-    There should only be one NeighborlyEngine instance per simulation. It is designed
-    to handle the internal logic of determining when to create certain entities. For
-    example, the engine creates characters entities using spawn multipliers associated
-    with each archetype.
-    """
-
-    __slots__ = (
-        "_rng",
-        "_name_generator",
-        "_component_types",
-    )
-
-    def __init__(self, seed: Optional[int] = None) -> None:
-        self._rng: random.Random = random.Random(seed)
-        self._name_generator: TraceryNameFactory = TraceryNameFactory()
-        tracery.set_grammar_rng(self._rng)
-        self._component_types: Dict[str, Type[Component]] = {}
-
-    @property
-    def rng(self) -> random.Random:
-        return self._rng
-
-    @property
-    def name_generator(self) -> TraceryNameFactory:
-        return self._name_generator
-
-    def get_component(self, component_name: str) -> Type[Component]:
-        return self._component_types[component_name]
-
-    def add_component(self, component_type: Type[Component]) -> None:
-        self._component_types[component_type.__name__] = component_type
+from __future__ import annotations
+
+import random
+from typing import Dict, Optional, Type
+
+from neighborly.core.ecs import Component
+from neighborly.core.name_generation import TraceryNameFactory
+
+
+class NeighborlyEngine:
+    """
+    An engine stores and instantiates entity archetypes for characters, businesses,
+    residences, and other places.
+
+    There should only be one NeighborlyEngine instance per simulation. It is designed
+    to handle the internal logic of determining when to create certain entities. For
+    example, the engine creates characters entities using spawn multipliers associated
+    with each archetype.
+    """
+
+    __slots__ = (
+        "_rng",
+        "_name_generator",
+        "_component_types",
+    )
+
+    def __init__(self, seed: Optional[int] = None) -> None:
+        random.seed(seed)
+        self._rng: random.Random = random.Random(seed)
+        self._name_generator: TraceryNameFactory = TraceryNameFactory()
+        self._component_types: Dict[str, Type[Component]] = {}
+
+    @property
+    def rng(self) -> random.Random:
+        return self._rng
+
+    @property
+    def name_generator(self) -> TraceryNameFactory:
+        return self._name_generator
+
+    def get_component(self, component_name: str) -> Type[Component]:
+        return self._component_types[component_name]
+
+    def add_component(self, component_type: Type[Component]) -> None:
+        self._component_types[component_type.__name__] = component_type
```

### Comparing `neighborly-0.9.3/src/neighborly/core/personal_values.py` & `neighborly-0.9.4/src/neighborly/core/personal_values.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,141 +1,150 @@
-from __future__ import annotations
-
-from enum import Enum
-from typing import Dict, List, Optional
-
-import numpy as np
-import numpy.typing as npt
-
-from neighborly.core.ecs import Component, World
-from neighborly.core.engine import NeighborlyEngine
-
-TRAIT_MAX = 50
-TRAIT_MIN = -50
-
-
-class ValueTrait(Enum):
-    ADVENTURE = "adventure"
-    AMBITION = "ambition"
-    EXCITEMENT = "excitement"
-    COMMERCE = "commerce"
-    CONFIDENCE = "confidence"
-    CURIOSITY = "curiosity"
-    FAMILY = "family"
-    FRIENDSHIP = "friendship"
-    WEALTH = "wealth"
-    HEALTH = "health"
-    INDEPENDENCE = "independence"
-    KNOWLEDGE = "knowledge"
-    LEISURE_TIME = "leisure-time"
-    LOYALTY = "loyalty"
-    LUST = "lust"
-    MATERIAL_THINGS = "material things"
-    NATURE = "nature"
-    PEACE = "peace"
-    POWER = "power"
-    RELIABILITY = "reliability"
-    ROMANCE = "romance"
-    SINGLE_MINDEDNESS = "single mindedness"
-    SOCIAL = "social"
-    SELF_CONTROL = "self-control"
-    TRADITION = "tradition"
-    TRANQUILITY = "tranquility"
-
-
-_VALUE_INDICES: Dict[str, int] = {
-    str(value_trait.value): index for index, value_trait in enumerate(ValueTrait)
-}
-
-
-class PersonalValues(Component):
-    """
-    Values are what a character believes in. They are used
-    for decision-making and relationship compatibility among
-    other things.
-
-    Individual values are integers on the range [-50,50], inclusive.
-
-    This model of character values is borrowed from Dwarf Fortress'
-    model of character beliefs/values outlined at the following link
-    https://dwarffortresswiki.org/index.php/DF2014:Personality_trait
-    """
-
-    __slots__ = "_traits"
-
-    def __init__(
-        self, overrides: Optional[Dict[str, int]] = None, default: int = 0
-    ) -> None:
-        super().__init__()
-        self._traits: npt.NDArray[np.int32] = np.array(
-            [default] * len(_VALUE_INDICES.keys()), dtype=np.int32
-        )
-
-        if overrides:
-            for trait, value in overrides.items():
-                self._traits[_VALUE_INDICES[trait]] = max(
-                    TRAIT_MIN, min(TRAIT_MAX, value)
-                )
-
-    @property
-    def traits(self) -> npt.NDArray[np.int32]:
-        return self._traits
-
-    @staticmethod
-    def compatibility(
-        character_a: PersonalValues, character_b: PersonalValues
-    ) -> float:
-        # Cosine similarity is a value between -1 and 1
-        cos_sim: float = np.dot(character_a.traits, character_b.traits) / (
-            np.linalg.norm(character_a.traits) * np.linalg.norm(character_b.traits)
-        )
-
-        return cos_sim
-
-    def get_high_values(self, n=3) -> List[str]:
-        """Return the value names associated with the n values"""
-        # This code is adapted from https://stackoverflow.com/a/23734295
-
-        ind = np.argpartition(self.traits, -n)[-n:]
-
-        value_names = list(_VALUE_INDICES.keys())
-
-        return [value_names[i] for i in ind]
-
-    def __getitem__(self, trait: str) -> int:
-        return self._traits[_VALUE_INDICES[trait]]
-
-    def __setitem__(self, trait: str, value: int) -> None:
-        self._traits[_VALUE_INDICES[trait]] = max(TRAIT_MIN, min(TRAIT_MAX, value))
-
-    def __str__(self) -> str:
-        return f"Values Most: {self.get_high_values()}"
-
-    def __repr__(self) -> str:
-        return "{}({})".format(self.__class__.__name__, self._traits.__repr__())
-
-    @classmethod
-    def create(cls, world: World, **kwargs) -> Component:
-        engine = world.get_resource(NeighborlyEngine)
-        n_likes: int = kwargs.get("n_likes", 3)
-        n_dislikes: int = kwargs.get("n_dislikes", 3)
-
-        traits = [
-            str(trait.value)
-            for trait in engine.rng.sample(list(ValueTrait), n_likes + n_dislikes)
-        ]
-
-        # select likes and dislikes
-        high_values = engine.rng.sample(traits, n_likes)
-
-        low_values = list(filter(lambda t: t not in high_values, traits))
-
-        # Generate values for each ([30,50] for high values, [-50,-30] for dislikes)
-        values_overrides: Dict[str, int] = {}
-
-        for trait in high_values:
-            values_overrides[trait] = engine.rng.randint(30, 50)
-
-        for trait in low_values:
-            values_overrides[trait] = engine.rng.randint(-50, -30)
-
-        return PersonalValues(values_overrides)
+from __future__ import annotations
+
+from enum import Enum
+from typing import Any, Dict, List, Optional
+
+import numpy as np
+import numpy.typing as npt
+
+from neighborly.core.ecs import Component, World
+from neighborly.core.engine import NeighborlyEngine
+
+TRAIT_MAX = 50
+TRAIT_MIN = -50
+
+
+class ValueTrait(Enum):
+    ADVENTURE = "adventure"
+    AMBITION = "ambition"
+    EXCITEMENT = "excitement"
+    COMMERCE = "commerce"
+    CONFIDENCE = "confidence"
+    CURIOSITY = "curiosity"
+    FAMILY = "family"
+    FRIENDSHIP = "friendship"
+    WEALTH = "wealth"
+    HEALTH = "health"
+    INDEPENDENCE = "independence"
+    KNOWLEDGE = "knowledge"
+    LEISURE_TIME = "leisure-time"
+    LOYALTY = "loyalty"
+    LUST = "lust"
+    MATERIAL_THINGS = "material things"
+    NATURE = "nature"
+    PEACE = "peace"
+    POWER = "power"
+    RELIABILITY = "reliability"
+    ROMANCE = "romance"
+    SINGLE_MINDEDNESS = "single mindedness"
+    SOCIAL = "social"
+    SELF_CONTROL = "self-control"
+    TRADITION = "tradition"
+    TRANQUILITY = "tranquility"
+
+
+_VALUE_INDICES: Dict[str, int] = {
+    str(value_trait.value): index for index, value_trait in enumerate(ValueTrait)
+}
+
+
+class PersonalValues(Component):
+    """
+    Values are what an entity believes in. They are used
+    for decision-making and relationship compatibility among
+    other things.
+
+    Individual values are integers on the range [-50,50], inclusive.
+
+    This model of entity values is borrowed from Dwarf Fortress'
+    model of entity beliefs/values outlined at the following link
+    https://dwarffortresswiki.org/index.php/DF2014:Personality_trait
+    """
+
+    __slots__ = "_traits"
+
+    def __init__(
+        self, overrides: Optional[Dict[str, int]] = None, default: int = 0
+    ) -> None:
+        super().__init__()
+        self._traits: npt.NDArray[np.int32] = np.array(
+            [default] * len(_VALUE_INDICES.keys()), dtype=np.int32
+        )
+
+        if overrides:
+            for trait, value in overrides.items():
+                self._traits[_VALUE_INDICES[trait]] = max(
+                    TRAIT_MIN, min(TRAIT_MAX, value)
+                )
+
+    @property
+    def traits(self) -> npt.NDArray[np.int32]:
+        return self._traits
+
+    @staticmethod
+    def compatibility(
+        character_a: PersonalValues, character_b: PersonalValues
+    ) -> float:
+        # Cosine similarity is a value between -1 and 1
+        cos_sim: float = np.dot(character_a.traits, character_b.traits) / (
+            np.linalg.norm(character_a.traits) * np.linalg.norm(character_b.traits)
+        )
+
+        return cos_sim
+
+    def get_high_values(self, n=3) -> List[str]:
+        """Return the value names associated with the n values"""
+        # This code is adapted from https://stackoverflow.com/a/23734295
+
+        ind = np.argpartition(self.traits, -n)[-n:]
+
+        value_names = list(_VALUE_INDICES.keys())
+
+        return [value_names[i] for i in ind]
+
+    def __getitem__(self, trait: str) -> int:
+        return self._traits[_VALUE_INDICES[trait]]
+
+    def __setitem__(self, trait: str, value: int) -> None:
+        self._traits[_VALUE_INDICES[trait]] = max(TRAIT_MIN, min(TRAIT_MAX, value))
+
+    def __str__(self) -> str:
+        return f"Values Most: {self.get_high_values()}"
+
+    def __repr__(self) -> str:
+        return "{}({})".format(self.__class__.__name__, self._traits.__repr__())
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            **super().to_dict(),
+            "traits": {
+                str(p_value.value): self._traits[_VALUE_INDICES[str(p_value.value)]]
+                for p_value in list(PersonalValues)
+            },
+        }
+
+    @classmethod
+    def create(cls, world: World, **kwargs) -> Component:
+        engine = world.get_resource(NeighborlyEngine)
+        n_likes: int = kwargs.get("n_likes", 3)
+        n_dislikes: int = kwargs.get("n_dislikes", 3)
+
+        traits = [
+            str(trait.value)
+            for trait in engine.rng.sample(list(ValueTrait), n_likes + n_dislikes)
+        ]
+
+        # select likes and dislikes
+        high_values = engine.rng.sample(traits, n_likes)
+
+        low_values = list(filter(lambda t: t not in high_values, traits))
+
+        # Generate values for each ([30,50] for high values, [-50,-30] for dislikes)
+        values_overrides: Dict[str, int] = {}
+
+        for trait in high_values:
+            values_overrides[trait] = engine.rng.randint(30, 50)
+
+        for trait in low_values:
+            values_overrides[trait] = engine.rng.randint(-50, -30)
+
+        return PersonalValues(values_overrides)
```

### Comparing `neighborly-0.9.3/src/neighborly/core/residence.py` & `neighborly-0.9.4/src/neighborly/core/residence.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,85 +1,67 @@
-from __future__ import annotations
-
-from typing import Any, Dict
-
-from ordered_set import OrderedSet
-
-from neighborly.core.ecs import Component
-
-
-class Residence(Component):
-    """Residence is a place where characters live"""
-
-    __slots__ = "owners", "former_owners", "residents", "former_residents", "_vacant"
-
-    def __init__(self) -> None:
-        super().__init__()
-        self.owners: OrderedSet[int] = OrderedSet([])
-        self.former_owners: OrderedSet[int] = OrderedSet([])
-        self.residents: OrderedSet[int] = OrderedSet([])
-        self.former_residents: OrderedSet[int] = OrderedSet([])
-        self._vacant: bool = True
-
-    def on_archive(self) -> None:
-        self.gameobject.remove_component(type(self))
-
-    def to_dict(self) -> Dict[str, Any]:
-        return {
-            **super().to_dict(),
-            "owners": list(self.owners),
-            "former_owners": list(self.former_owners),
-            "residents": list(self.residents),
-            "former_residents": list(self.former_residents),
-            "vacant": self._vacant,
-        }
-
-    def add_owner(self, owner: int) -> None:
-        """Add owner to the residence"""
-        self.owners.add(owner)
-
-    def remove_owner(self, owner: int) -> None:
-        """Remove owner from residence"""
-        self.owners.remove(owner)
-
-    def is_owner(self, character: int) -> bool:
-        """Return True if the character is an owner of this residence"""
-        return character in self.owners
-
-    def add_resident(self, resident: int) -> None:
-        """Add a tenant to this residence"""
-        self.residents.add(resident)
-        self._vacant = False
-
-    def remove_resident(self, resident: int) -> None:
-        """Remove a tenant rom this residence"""
-        self.residents.remove(resident)
-        self.former_residents.add(resident)
-        self._vacant = len(self.residents) == 0
-
-    def is_resident(self, character: int) -> bool:
-        """Return True if the given character is a resident"""
-        return character in self.residents
-
-    def is_vacant(self) -> bool:
-        """Return True if the residence is vacant"""
-        return self._vacant
-
-
-class Resident(Component):
-    """Component attached to characters indicating that they live in the town"""
-
-    __slots__ = "residence"
-
-    def __init__(self, residence: int) -> None:
-        super().__init__()
-        self.residence: int = residence
-
-    def on_remove(self) -> None:
-        world = self.gameobject.world
-        residence = world.get_gameobject(self.residence).get_component(Residence)
-        residence.remove_resident(self.gameobject.id)
-        if residence.is_owner(self.gameobject.id):
-            residence.remove_owner(self.gameobject.id)
-
-    def on_archive(self) -> None:
-        self.gameobject.remove_component(type(self))
+from __future__ import annotations
+
+from typing import Any, Dict
+
+from ordered_set import OrderedSet
+
+from neighborly.core.ecs import Component
+
+
+class Residence(Component):
+    """Residence is a place where characters live"""
+
+    __slots__ = "owners", "former_owners", "residents", "former_residents", "_vacant"
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.owners: OrderedSet[int] = OrderedSet([])
+        self.former_owners: OrderedSet[int] = OrderedSet([])
+        self.residents: OrderedSet[int] = OrderedSet([])
+        self.former_residents: OrderedSet[int] = OrderedSet([])
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            **super().to_dict(),
+            "owners": list(self.owners),
+            "former_owners": list(self.former_owners),
+            "residents": list(self.residents),
+            "former_residents": list(self.former_residents),
+        }
+
+    def add_owner(self, owner: int) -> None:
+        """Add owner to the residence"""
+        self.owners.add(owner)
+
+    def remove_owner(self, owner: int) -> None:
+        """Remove owner from residence"""
+        self.owners.remove(owner)
+
+    def is_owner(self, character: int) -> bool:
+        """Return True if the entity is an owner of this residence"""
+        return character in self.owners
+
+    def add_resident(self, resident: int) -> None:
+        """Add a tenant to this residence"""
+        self.residents.add(resident)
+
+    def remove_resident(self, resident: int) -> None:
+        """Remove a tenant rom this residence"""
+        self.residents.remove(resident)
+        self.former_residents.add(resident)
+
+    def is_resident(self, character: int) -> bool:
+        """Return True if the given entity is a resident"""
+        return character in self.residents
+
+
+class Resident(Component):
+    """Component attached to characters indicating that they live in the town"""
+
+    __slots__ = "residence"
+
+    def __init__(self, residence: int) -> None:
+        super().__init__()
+        self.residence: int = residence
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {**super().to_dict(), "residence": self.residence}
```

### Comparing `neighborly-0.9.3/src/neighborly/core/time.py` & `neighborly-0.9.4/src/neighborly/core/time.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,281 +1,340 @@
-from __future__ import annotations
-
-from dataclasses import dataclass
-from typing import List
-
-HOURS_PER_DAY = 24
-DAYS_PER_WEEK = 7
-DAYS_PER_MONTH = 28
-WEEKS_PER_MONTH = 4
-MONTHS_PER_YEAR = 12
-HOURS_PER_YEAR = HOURS_PER_DAY * DAYS_PER_MONTH * MONTHS_PER_YEAR
-DAYS_PER_YEAR = DAYS_PER_MONTH * MONTHS_PER_YEAR
-
-_TIME_OF_DAY: List[str] = [
-    *(["night"] * 6),  # (00:00-05:59)
-    *(["morning"] * 1),  # (06:00-06:59)
-    *(["day"] * 11),  # (07:00-17:59)
-    *(["evening"] * 1),  # (18:00-18:59)
-    *(["night"] * 5),  # (19:00-23:59)
-]
-
-_DAYS_OF_WEEK: List[str] = [
-    "Sunday",
-    "Monday",
-    "Tuesday",
-    "Wednesday",
-    "Thursday",
-    "Friday",
-    "Saturday",
-]
-
-
-def get_time_of_day(hour: int) -> str:
-    """Return a string corresponding to the time of day for the given hour"""
-    return _TIME_OF_DAY[hour]
-
-
-@dataclass(frozen=True)
-class TimeDelta:
-    """Represents a difference in time from one SimDateTime to Another"""
-
-    years: int = 0
-    months: int = 0
-    days: int = 0
-    hours: int = 0
-
-    @property
-    def total_days(self) -> int:
-        """get the total number of days that this delta represents"""
-        return (
-            self.days
-            + (self.months * DAYS_PER_MONTH)
-            + (self.years * MONTHS_PER_YEAR * DAYS_PER_MONTH)
-        )
-
-    @property
-    def total_hours(self) -> int:
-        """get the total number of days that this delta represents"""
-        return (
-            self.hours
-            + (self.days * HOURS_PER_DAY)
-            + (self.months * DAYS_PER_MONTH * HOURS_PER_DAY)
-            + (self.years * MONTHS_PER_YEAR * DAYS_PER_MONTH * HOURS_PER_DAY)
-        )
-
-
-class SimDateTime:
-    """
-    Implementation of time in the simulated town
-    using 7-day weeks, 4-week months, and 12-month years
-    """
-
-    __slots__ = "_hour", "_day", "_month", "_year", "_weekday", "_delta_time"
-
-    def __init__(
-        self,
-        year: int = 0,
-        month: int = 0,
-        day: int = 0,
-        hour: int = 0,
-    ) -> None:
-        if 0 <= hour < HOURS_PER_DAY:
-            self._hour: int = hour
-        else:
-            raise ValueError(
-                f"Parameter 'hours' must be between 0 and {HOURS_PER_DAY - 1}"
-            )
-
-        if 0 <= day < DAYS_PER_MONTH:
-            self._day: int = day
-            self._weekday: int = day % 7
-        else:
-            raise ValueError(
-                f"Parameter 'day' must be between 0 and {DAYS_PER_MONTH - 1}"
-            )
-
-        if 0 <= month < MONTHS_PER_YEAR:
-            self._month: int = month
-        else:
-            raise ValueError(
-                f"Parameter 'month' must be between 0 and {MONTHS_PER_YEAR - 1}"
-            )
-
-        self._year: int = year
-        self._delta_time: int = 0
-
-    def increment(
-        self, hours: int = 0, days: int = 0, months: int = 0, years: int = 0
-    ) -> None:
-        """Advance time by a given amount"""
-
-        if hours < 0:
-            raise ValueError("Parameter 'hours' may not be negative")
-        if days < 0:
-            raise ValueError("Parameter 'days' may not be negative")
-        if months < 0:
-            raise ValueError("Parameter 'months' may not be negative")
-        if years < 0:
-            raise ValueError("Parameter 'years' may not be negative")
-
-        total_hours: int = self._hour + hours
-        carry_days: int = int(total_hours / 24)
-
-        self._hour = total_hours % 24
-
-        self._weekday = (self._weekday + days + carry_days) % 7
-
-        total_days: int = self.day + days + carry_days
-        carry_months: int = int(total_days / 28)  # 28 days per month
-        self._day = total_days % 28
-
-        total_months: int = self._month + months + carry_months
-        carry_years: int = int(total_months / 12)
-        self._month = total_months % 12
-
-        self._year = self._year + years + carry_years
-
-        self._delta_time = (
-            hours
-            + days * HOURS_PER_DAY
-            + months * DAYS_PER_MONTH * HOURS_PER_DAY
-            + years * MONTHS_PER_YEAR * DAYS_PER_MONTH * HOURS_PER_DAY
-        )
-
-    @property
-    def hour(self) -> int:
-        return self._hour
-
-    @property
-    def day(self) -> int:
-        return self._day
-
-    @property
-    def weekday(self) -> int:
-        return self._weekday
-
-    @property
-    def month(self) -> int:
-        return self._month
-
-    @property
-    def year(self) -> int:
-        return self._year
-
-    @property
-    def delta_time(self) -> int:
-        return self._delta_time
-
-    @property
-    def weekday_str(self) -> str:
-        return _DAYS_OF_WEEK[self._weekday]
-
-    def copy(self) -> SimDateTime:
-        return SimDateTime(
-            hour=self._hour,
-            day=self._day,
-            month=self._month,
-            year=self._year,
-        )
-
-    def __repr__(self) -> str:
-        return "{}(hour={}, day={}, month={}, year={}, weekday={})".format(
-            self.__class__.__name__,
-            self.hour,
-            self.day,
-            self.month,
-            self.year,
-            self.weekday_str,
-        )
-
-    def __str__(self) -> str:
-        return "{}-{}-{}-{}".format(self.year, self.month, self.day, self.hour)
-
-    def __sub__(self, other: SimDateTime) -> TimeDelta:
-        """Subtract a SimDateTime from another and return the difference"""
-        diff_hours = self.to_hours() - other.to_hours()
-
-        # Convert hours back to date components
-        remainder: int = diff_hours
-        years = remainder // (MONTHS_PER_YEAR * DAYS_PER_MONTH * HOURS_PER_DAY)
-        remainder = remainder % (MONTHS_PER_YEAR * DAYS_PER_MONTH * HOURS_PER_DAY)
-        months = remainder // (DAYS_PER_MONTH * HOURS_PER_DAY)
-        remainder = remainder % (DAYS_PER_MONTH * HOURS_PER_DAY)
-        days = remainder // HOURS_PER_DAY
-        hours = remainder % HOURS_PER_DAY
-
-        return TimeDelta(years=years, months=months, days=days, hours=hours)
-
-    def __add__(self, other: TimeDelta) -> SimDateTime:
-        """Add a TimeDelta to this data"""
-        if not isinstance(other, TimeDelta):
-            raise TypeError(f"expected TimeDelta object but was {type(other)}")
-        self.increment(
-            hours=other.hours, days=other.days, months=other.months, years=other.years
-        )
-        return self
-
-    def __le__(self, other: SimDateTime) -> bool:
-        if not isinstance(other, SimDateTime):
-            raise TypeError(f"expected TimeDelta object but was {type(other)}")
-        return self.to_iso_str() < other.to_iso_str()
-
-    def __gt__(self, other) -> bool:
-        if not isinstance(other, SimDateTime):
-            raise TypeError(f"expected TimeDelta object but was {type(other)}")
-        return self.to_iso_str() > other.to_iso_str()
-
-    def to_date_str(self) -> str:
-        return "{}, {:02d}/{:02d}/{:04d} @ {:02d}:00".format(
-            self.weekday_str[:3], self.day, self.month, self.year, self.hour
-        )
-
-    def to_iso_str(self) -> str:
-        """Return ISO string format"""
-        return "{:04d}-{:02d}-{:02d}T{:02d}:00.000z".format(
-            self.year, self.month, self.day, self.hour
-        )
-
-    def to_hours(self) -> int:
-        """Return the number of hours that have elapsed since 00-00-0000"""
-        return (
-            self.hour
-            + (self.day * HOURS_PER_DAY)
-            + (self.month * DAYS_PER_MONTH * HOURS_PER_DAY)
-            + (self.year * MONTHS_PER_YEAR * DAYS_PER_MONTH * HOURS_PER_DAY)
-        )
-
-    def to_ordinal(self) -> int:
-        """Returns the number of elapsed days since 00-00-0000"""
-        return (
-            +self.day
-            + (self.month * DAYS_PER_MONTH)
-            + (self.year * MONTHS_PER_YEAR * DAYS_PER_MONTH)
-        )
-
-    @classmethod
-    def from_ordinal(cls, ordinal_date: int) -> SimDateTime:
-        date = cls()
-        date.increment(days=ordinal_date)
-        return date
-
-    @classmethod
-    def from_iso_str(cls, iso_date: str) -> SimDateTime:
-        """Return a SimDateTime object given an ISO format string"""
-        date_time = iso_date.strip().split("T")
-        date = date_time[0]
-        time = date_time[1] if len(date_time) == 2 else "00:00.000z"
-        year, month, day = tuple(map(lambda s: int(s.strip()), date.split("-")))
-        hour = int(time.split(":")[0])
-        return cls(year=year, month=month, day=day, hour=hour)
-
-    @classmethod
-    def from_str(cls, time_str: str) -> SimDateTime:
-        time = cls()
-        year, month, day, hour = tuple(time_str.split("-"))
-        time._year = int(year)
-        time._month = int(month)
-        time._weekday = int(day) % 7
-        time._day = int(day)
-        time._hour = int(hour)
-        return time
+from __future__ import annotations
+
+from dataclasses import dataclass
+from enum import IntEnum
+from typing import List
+
+HOURS_PER_DAY = 24
+DAYS_PER_WEEK = 7
+DAYS_PER_MONTH = 28
+WEEKS_PER_MONTH = 4
+MONTHS_PER_YEAR = 12
+HOURS_PER_YEAR = HOURS_PER_DAY * DAYS_PER_MONTH * MONTHS_PER_YEAR
+DAYS_PER_YEAR = DAYS_PER_MONTH * MONTHS_PER_YEAR
+
+_TIME_OF_DAY: List[str] = [
+    *(["night"] * 6),  # (00:00-05:59)
+    *(["morning"] * 1),  # (06:00-06:59)
+    *(["day"] * 11),  # (07:00-17:59)
+    *(["evening"] * 1),  # (18:00-18:59)
+    *(["night"] * 5),  # (19:00-23:59)
+]
+
+
+class Weekday(IntEnum):
+    Sunday = 0
+    Monday = 1
+    Tuesday = 2
+    Wednesday = 3
+    Thursday = 4
+    Friday = 5
+    Saturday = 6
+
+    def __str__(self) -> str:
+        return self.name
+
+    def abbr(self) -> str:
+        abbreviations = [
+            "M",
+            "T",
+            "W",
+            "R",
+            "F",
+            "S",
+            "U",
+        ]
+        return abbreviations[self.value()]
+
+    @classmethod
+    def from_abbr(cls, value: str) -> Weekday:
+        abbreviations = {
+            "M": Weekday.Monday,
+            "T": Weekday.Tuesday,
+            "W": Weekday.Wednesday,
+            "R": Weekday.Thursday,
+            "F": Weekday.Friday,
+            "S": Weekday.Saturday,
+            "U": Weekday.Sunday,
+        }
+        return abbreviations[value]
+
+
+@dataclass(frozen=True)
+class TimeDelta:
+    """Represents a difference in time from one SimDateTime to Another"""
+
+    years: int = 0
+    months: int = 0
+    days: int = 0
+    hours: int = 0
+
+    @property
+    def total_days(self) -> int:
+        """get the total number of days that this delta represents"""
+        return (
+            self.days
+            + (self.months * DAYS_PER_MONTH)
+            + (self.years * MONTHS_PER_YEAR * DAYS_PER_MONTH)
+        )
+
+    @property
+    def total_hours(self) -> int:
+        """get the total number of days that this delta represents"""
+        return (
+            self.hours
+            + (self.days * HOURS_PER_DAY)
+            + (self.months * DAYS_PER_MONTH * HOURS_PER_DAY)
+            + (self.years * MONTHS_PER_YEAR * DAYS_PER_MONTH * HOURS_PER_DAY)
+        )
+
+
+class SimDateTime:
+    """
+    Implementation of time in the simulated town
+    using 7-day weeks, 4-week months, and 12-month years
+    """
+
+    __slots__ = "_hour", "_day", "_month", "_year", "_weekday", "_delta_time"
+
+    def __init__(
+        self,
+        year: int = 0,
+        month: int = 0,
+        day: int = 0,
+        hour: int = 0,
+    ) -> None:
+        if 0 <= hour < HOURS_PER_DAY:
+            self._hour: int = hour
+        else:
+            raise ValueError(
+                f"Parameter 'hours' must be between 0 and {HOURS_PER_DAY - 1}"
+            )
+
+        if 0 <= day < DAYS_PER_MONTH:
+            self._day: int = day
+            self._weekday: int = day % 7
+        else:
+            raise ValueError(
+                f"Parameter 'day' must be between 0 and {DAYS_PER_MONTH - 1}"
+            )
+
+        if 0 <= month < MONTHS_PER_YEAR:
+            self._month: int = month
+        else:
+            raise ValueError(
+                f"Parameter 'month' must be between 0 and {MONTHS_PER_YEAR - 1}"
+            )
+
+        self._year: int = year
+        self._delta_time: int = 0
+
+    def increment(
+        self, hours: int = 0, days: int = 0, months: int = 0, years: int = 0
+    ) -> None:
+        """Advance time by a given amount"""
+
+        if hours < 0:
+            raise ValueError("Parameter 'hours' may not be negative")
+        if days < 0:
+            raise ValueError("Parameter 'days' may not be negative")
+        if months < 0:
+            raise ValueError("Parameter 'months' may not be negative")
+        if years < 0:
+            raise ValueError("Parameter 'years' may not be negative")
+
+        total_hours: int = self._hour + hours
+        carry_days: int = int(total_hours / 24)
+
+        self._hour = total_hours % 24
+
+        self._weekday = (self._weekday + days + carry_days) % 7
+
+        total_days: int = self.day + days + carry_days
+        carry_months: int = int(total_days / 28)  # 28 days per month
+        self._day = total_days % 28
+
+        total_months: int = self._month + months + carry_months
+        carry_years: int = int(total_months / 12)
+        self._month = total_months % 12
+
+        self._year = self._year + years + carry_years
+
+        self._delta_time = (
+            hours
+            + days * HOURS_PER_DAY
+            + months * DAYS_PER_MONTH * HOURS_PER_DAY
+            + years * MONTHS_PER_YEAR * DAYS_PER_MONTH * HOURS_PER_DAY
+        )
+
+    @property
+    def hour(self) -> int:
+        return self._hour
+
+    @property
+    def day(self) -> int:
+        return self._day
+
+    @property
+    def weekday(self) -> int:
+        return self._weekday
+
+    @property
+    def month(self) -> int:
+        return self._month
+
+    @property
+    def year(self) -> int:
+        return self._year
+
+    @property
+    def delta_time(self) -> int:
+        return self._delta_time
+
+    @property
+    def weekday_str(self) -> str:
+        return str(Weekday(self._weekday))
+
+    def copy(self) -> SimDateTime:
+        return SimDateTime(
+            hour=self._hour,
+            day=self._day,
+            month=self._month,
+            year=self._year,
+        )
+
+    def __repr__(self) -> str:
+        return "{}(hour={}, day={}, month={}, year={}, weekday={})".format(
+            self.__class__.__name__,
+            self.hour,
+            self.day,
+            self.month,
+            self.year,
+            self.weekday_str,
+        )
+
+    def __str__(self) -> str:
+        return "{}-{}-{}-{}".format(self.year, self.month, self.day, self.hour)
+
+    def __sub__(self, other: SimDateTime) -> TimeDelta:
+        """Subtract a SimDateTime from another and return the difference"""
+        diff_hours = self.to_hours() - other.to_hours()
+
+        # Convert hours back to date components
+        remainder: int = diff_hours
+        years = remainder // (MONTHS_PER_YEAR * DAYS_PER_MONTH * HOURS_PER_DAY)
+        remainder = remainder % (MONTHS_PER_YEAR * DAYS_PER_MONTH * HOURS_PER_DAY)
+        months = remainder // (DAYS_PER_MONTH * HOURS_PER_DAY)
+        remainder = remainder % (DAYS_PER_MONTH * HOURS_PER_DAY)
+        days = remainder // HOURS_PER_DAY
+        hours = remainder % HOURS_PER_DAY
+
+        return TimeDelta(years=years, months=months, days=days, hours=hours)
+
+    def __add__(self, other: TimeDelta) -> SimDateTime:
+        """Add a TimeDelta to this data"""
+        if not isinstance(other, TimeDelta):
+            raise TypeError(f"expected TimeDelta object but was {type(other)}")
+        date_copy = self.copy()
+        date_copy.increment(
+            hours=other.hours, days=other.days, months=other.months, years=other.years
+        )
+        return date_copy
+
+    def __iadd__(self, other: TimeDelta) -> SimDateTime:
+        self.increment(
+            hours=other.hours, days=other.days, months=other.months, years=other.years
+        )
+        return self
+
+    def __le__(self, other: SimDateTime) -> bool:
+        return self.to_iso_str() <= other.to_iso_str()
+
+    def __lt__(self, other: SimDateTime) -> bool:
+        return self.to_iso_str() < other.to_iso_str()
+
+    def __ge__(self, other: SimDateTime) -> bool:
+        if not isinstance(other, SimDateTime):
+            raise TypeError(f"expected TimeDelta object but was {type(other)}")
+        return self.to_iso_str() >= other.to_iso_str()
+
+    def __gt__(self, other: SimDateTime) -> bool:
+        if not isinstance(other, SimDateTime):
+            raise TypeError(f"expected TimeDelta object but was {type(other)}")
+        return self.to_iso_str() > other.to_iso_str()
+
+    def __eq__(self, other: SimDateTime) -> bool:
+        return self.to_hours() == other.to_hours()
+
+    def to_date_str(self) -> str:
+        return "{}, {:02d}/{:02d}/{:04d} @ {:02d}:00".format(
+            self.weekday_str[:3], self.day, self.month, self.year, self.hour
+        )
+
+    def to_iso_str(self) -> str:
+        """Return ISO string format"""
+        return "{:04d}-{:02d}-{:02d}T{:02d}:00.000z".format(
+            self.year, self.month, self.day, self.hour
+        )
+
+    def to_hours(self) -> int:
+        """Return the number of hours that have elapsed since 00-00-0000"""
+        return (
+            self.hour
+            + (self.day * HOURS_PER_DAY)
+            + (self.month * DAYS_PER_MONTH * HOURS_PER_DAY)
+            + (self.year * MONTHS_PER_YEAR * DAYS_PER_MONTH * HOURS_PER_DAY)
+        )
+
+    def to_ordinal(self) -> int:
+        """Returns the number of elapsed days since 00-00-0000"""
+        return (
+            +self.day
+            + (self.month * DAYS_PER_MONTH)
+            + (self.year * MONTHS_PER_YEAR * DAYS_PER_MONTH)
+        )
+
+    def get_time_of_day(self) -> str:
+        """Return a string corresponding to the time of day for the given hour"""
+        return _TIME_OF_DAY[self.hour]
+
+    @classmethod
+    def from_ordinal(cls, ordinal_date: int) -> SimDateTime:
+        date = cls()
+        date.increment(days=ordinal_date)
+        return date
+
+    @classmethod
+    def from_iso_str(cls, iso_date: str) -> SimDateTime:
+        """Return a SimDateTime object given an ISO format string"""
+        date_time = iso_date.strip().split("T")
+        date = date_time[0]
+        time = date_time[1] if len(date_time) == 2 else "00:00.000z"
+        year, month, day = tuple(map(lambda s: int(s.strip()), date.split("-")))
+        hour = int(time.split(":")[0])
+        return cls(year=year, month=month, day=day, hour=hour)
+
+    @classmethod
+    def from_str(cls, time_str: str) -> SimDateTime:
+        time = cls()
+        items = tuple(time_str.split("-"))
+
+        if len(items) == 4:
+            year, month, day, hour = items
+            time._year = int(year)
+            time._month = int(month)
+            time._weekday = int(day) % 7
+            time._day = int(day)
+            time._hour = int(hour)
+            return time
+
+        elif len(items) == 3:
+            year, month, day = items
+            time._year = int(year)
+            time._month = int(month)
+            time._weekday = int(day) % 7
+            time._day = int(day)
+            time._hour = 0
+            return time
+
+        else:
+            raise ValueError(f"Invalid date string: {time_str}")
```

### Comparing `neighborly-0.9.3/src/neighborly/core/utils/graph.py` & `neighborly-0.9.4/src/neighborly/core/utils/graph.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,105 +1,108 @@
-from collections import defaultdict
-from typing import TypeVar, NamedTuple, Generic, DefaultDict, Dict, Tuple, cast
-
-from ordered_set import OrderedSet
-
-_T = TypeVar("_T")
-
-
-class BDGraphNode(NamedTuple):
-    incoming: OrderedSet[int]
-    outgoing: OrderedSet[int]
-
-
-class DirectedGraph(Generic[_T]):
-    """Directed graph that represents information that connects characters"""
-
-    __slots__ = "_nodes", "_edges"
-
-    def __init__(self) -> None:
-        self._nodes: DefaultDict[int, BDGraphNode] = defaultdict(
-            lambda: BDGraphNode(OrderedSet([]), OrderedSet([]))
-        )
-        self._edges: Dict[Tuple[int, int], _T] = {}
-
-    def add_connection(self, owner: int, target: int, data: _T) -> None:
-        """Insert a new connection between characters"""
-        self._nodes[owner].outgoing.add(target)
-        self._nodes[target].incoming.add(owner)
-        self._edges[(owner, target)] = data
-
-    def has_connection(self, owner: int, target: int) -> bool:
-        """Return true if a connection exists from the owner to the target"""
-        return (owner, target) in self._edges
-
-    def get_connection(self, owner: int, target: int) -> _T:
-        """Get a connection between two characters if one exists"""
-        return self._edges[(owner, target)]
-
-    def remove_node(self, node: int) -> None:
-        """Remove a node and delete incoming and outgoing connections"""
-        node_to_remove = self._nodes[node]
-
-        # Delete all the outgoing connections
-        for other_node in [*node_to_remove.outgoing]:
-            self.remove_connection(node, other_node)
-
-        # Delete incoming connections
-        for other_node in [*node_to_remove.incoming]:
-            self.remove_connection(other_node, node)
-
-        del self._nodes[node]
-
-    def remove_connection(self, owner: int, target: int) -> None:
-        """Remove a connection from the social graph"""
-        self._nodes[owner].outgoing.remove(target)
-        self._nodes[target].incoming.remove(owner)
-        del self._edges[owner, target]
-
-
-class UndirectedGraph(Generic[_T]):
-    """Manages information about characters shared feeling towards each other
-
-    This class is for modeling symmetric social connections
-    """
-
-    def __init__(self) -> None:
-        self._nodes: Dict[int, OrderedSet[int]] = {}
-        self._edges: Dict[Tuple[int, int], _T] = {}
-
-    def add_connection(self, node_a: int, node_b: int, data: _T) -> None:
-        """Insert a new connection between characters"""
-
-        if node_a not in self._nodes:
-            self._nodes[node_a] = OrderedSet([])
-
-        if node_b not in self._nodes:
-            self._nodes[node_b] = OrderedSet([])
-
-        self._nodes[node_a].add(node_b)
-        self._nodes[node_b].add(node_a)
-
-        nodes = cast(Tuple[int, int], tuple(sorted((node_a, node_b))))
-        self._edges[nodes] = data
-
-    def has_connection(self, node_a: int, node_b: int) -> bool:
-        """Return true if a connection exists from the owner to the target"""
-        nodes = tuple(sorted((node_a, node_b)))
-        return nodes in self._edges
-
-    def get_connection(self, node_a: int, node_b: int) -> _T:
-        """Get a connection between two characters if one exists"""
-        nodes = cast(Tuple[int, int], tuple(sorted((node_a, node_b))))
-        return self._edges[nodes]
-
-    def remove_node(self, node: int) -> None:
-        """Remove a node and delete incoming and outgoing connections"""
-        for other_node in self._nodes[node]:
-            self.remove_connection(node, other_node)
-
-        del self._nodes[node]
-
-    def remove_connection(self, node_a: int, node_b: int) -> None:
-        """Remove a connection from the social graph"""
-        nodes = cast(Tuple[int, int], tuple(sorted((node_a, node_b))))
-        del self._edges[nodes]
+from collections import defaultdict
+from typing import DefaultDict, Dict, Generic, NamedTuple, Tuple, TypeVar, cast
+
+from ordered_set import OrderedSet
+
+_T = TypeVar("_T")
+
+
+class BDGraphNode(NamedTuple):
+    incoming: OrderedSet[int]
+    outgoing: OrderedSet[int]
+
+
+class DirectedGraph(Generic[_T]):
+    """Directed graph that represents information that connects characters"""
+
+    __slots__ = "_nodes", "_edges"
+
+    def __init__(self) -> None:
+        self._nodes: DefaultDict[int, BDGraphNode] = defaultdict(
+            lambda: BDGraphNode(OrderedSet([]), OrderedSet([]))
+        )
+        self._edges: Dict[Tuple[int, int], _T] = {}
+
+    def add_connection(self, owner: int, target: int, data: _T) -> None:
+        """Insert a new connection between characters"""
+        self._nodes[owner].outgoing.add(target)
+        self._nodes[target].incoming.add(owner)
+        self._edges[(owner, target)] = data
+
+    def has_connection(self, owner: int, target: int) -> bool:
+        """Return true if a connection exists from the owner to the target"""
+        return (owner, target) in self._edges
+
+    def get_connection(self, owner: int, target: int) -> _T:
+        """Get a connection between two characters if one exists"""
+        return self._edges[(owner, target)]
+
+    def remove_node(self, node: int) -> None:
+        """Remove a node and delete incoming and outgoing connections"""
+        if node not in self._nodes:
+            raise KeyError
+
+        node_to_remove = self._nodes[node]
+
+        # Delete all the outgoing connections
+        for other_node in [*node_to_remove.outgoing]:
+            self.remove_connection(node, other_node)
+
+        # Delete incoming connections
+        for other_node in [*node_to_remove.incoming]:
+            self.remove_connection(other_node, node)
+
+        del self._nodes[node]
+
+    def remove_connection(self, owner: int, target: int) -> None:
+        """Remove a connection from the social graph"""
+        self._nodes[owner].outgoing.remove(target)
+        self._nodes[target].incoming.remove(owner)
+        del self._edges[owner, target]
+
+
+class UndirectedGraph(Generic[_T]):
+    """Manages information about characters shared feeling towards each other
+
+    This class is for modeling symmetric social connections
+    """
+
+    def __init__(self) -> None:
+        self._nodes: Dict[int, OrderedSet[int]] = {}
+        self._edges: Dict[Tuple[int, int], _T] = {}
+
+    def add_connection(self, node_a: int, node_b: int, data: _T) -> None:
+        """Insert a new connection between characters"""
+
+        if node_a not in self._nodes:
+            self._nodes[node_a] = OrderedSet([])
+
+        if node_b not in self._nodes:
+            self._nodes[node_b] = OrderedSet([])
+
+        self._nodes[node_a].add(node_b)
+        self._nodes[node_b].add(node_a)
+
+        nodes = cast(Tuple[int, int], tuple(sorted((node_a, node_b))))
+        self._edges[nodes] = data
+
+    def has_connection(self, node_a: int, node_b: int) -> bool:
+        """Return true if a connection exists from the owner to the target"""
+        nodes = tuple(sorted((node_a, node_b)))
+        return nodes in self._edges
+
+    def get_connection(self, node_a: int, node_b: int) -> _T:
+        """Get a connection between two characters if one exists"""
+        nodes = cast(Tuple[int, int], tuple(sorted((node_a, node_b))))
+        return self._edges[nodes]
+
+    def remove_node(self, node: int) -> None:
+        """Remove a node and delete incoming and outgoing connections"""
+        for other_node in self._nodes[node]:
+            self.remove_connection(node, other_node)
+
+        del self._nodes[node]
+
+    def remove_connection(self, node_a: int, node_b: int) -> None:
+        """Remove a connection from the social graph"""
+        nodes = cast(Tuple[int, int], tuple(sorted((node_a, node_b))))
+        del self._edges[nodes]
```

### Comparing `neighborly-0.9.3/src/neighborly/exporter.py` & `neighborly-0.9.4/src/neighborly/exporter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,23 @@
-import json
-
-from neighborly.core.life_event import LifeEventLog
-from neighborly.core.relationship import RelationshipGraph
-from neighborly.core.time import SimDateTime
-from neighborly.core.town import LandGrid, Town
-from neighborly.simulation import Simulation
-
-
-class NeighborlyJsonExporter:
-    """Serializes the simulation to a JSON string"""
-
-    def export(self, sim: Simulation) -> str:
-        return json.dumps(
-            {
-                "seed": sim.seed,
-                "date": sim.world.get_resource(SimDateTime).to_iso_str(),
-                "gameobjects": {g.id: g.to_dict() for g in sim.world.get_gameobjects()},
-                "events": [
-                    f.to_dict()
-                    for f in sim.world.get_resource(LifeEventLog).event_history
-                ],
-                "relationships": sim.world.get_resource(RelationshipGraph).to_dict(),
-                "town": sim.world.get_resource(Town).to_dict(),
-                "land": sim.world.get_resource(LandGrid).grid.to_dict(),
-            }
-        )
+import json
+
+from neighborly.core.serializable import ISerializable
+from neighborly.core.time import SimDateTime
+from neighborly.simulation import Simulation
+
+
+class NeighborlyJsonExporter:
+    """Serializes the simulation to a JSON string"""
+
+    def export(self, sim: Simulation) -> str:
+        return json.dumps(
+            {
+                "seed": sim.seed,
+                "date": sim.world.get_resource(SimDateTime).to_iso_str(),
+                "gameobjects": {g.id: g.to_dict() for g in sim.world.get_gameobjects()},
+                "resources": {
+                    r.__class__.__name__: r.to_dict()
+                    for r in sim.world.get_all_resources()
+                    if isinstance(r, ISerializable)
+                },
+            }
+        )
```

### Comparing `neighborly-0.9.3/src/neighborly/plugins/default_plugin/data/data.yaml` & `neighborly-0.9.4/src/neighborly/plugins/defaults/data/data.yaml`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-Characters:
-  - name: Person
-    name_format: "#first_name# #family_name#"
-    lifespan: 85
-    life_stages:
-      child: 0
-      teen: 13
-      young_adult: 18
-      adult: 30
-      elder: 65
-Residences:
-  - name: House
-Businesses:
-  - name: Park
-    min_population: 20
-    max_instances: 5
-  - name: Library
-    employee_types:
-      librarian: 2
-    min_population: 50
-    max_instances: 1
-Activities:
-  - name: Rest
-    traits:
-      - leisure-time
-  - name: Gambling
-    traits:
-      - wealth
-      - excitement
-      - adventure
-      - lust
-  - name: Shopping
-    traits:
-      - material things
-      - excitement
-      - leisure-time
-  - name: Recreation
-    traits:
-      - health
-      - excitement
-  - name: Studying
-    traits:
-      - knowledge
-      - power
-      - ambition
-  - name: Reading
-    traits:
-      - knowledge
-      - power
-      - leisure-time
-  - name: Errands
-    traits:
-      - reliability
-      - health
-      - family
-  - name: Eating
-    traits:
-      - social
-      - health
-      - family
-  - name: Socializing
-    traits:
-      - social
-      - excitement
-      - friendship
-  - name: Drinking
-    traits:
-      - social
-      - friendship
-  - name: Relaxing
-    traits:
-      - health
-      - tranquility
-      - leisure-time
+Characters:
+  - name: Person
+    name_format: "#first_name# #family_name#"
+    lifespan: 85
+    life_stages:
+      child: 0
+      teen: 13
+      young_adult: 18
+      adult: 30
+      elder: 65
+Residences:
+  - name: House
+Businesses:
+  - name: Park
+    min_population: 20
+    max_instances: 5
+  - name: Library
+    employee_types:
+      librarian: 2
+    min_population: 50
+    max_instances: 1
+Activities:
+  - name: Rest
+    traits:
+      - leisure-time
+  - name: Gambling
+    traits:
+      - wealth
+      - excitement
+      - adventure
+      - lust
+  - name: Shopping
+    traits:
+      - material things
+      - excitement
+      - leisure-time
+  - name: Recreation
+    traits:
+      - health
+      - excitement
+  - name: Studying
+    traits:
+      - knowledge
+      - power
+      - ambition
+  - name: Reading
+    traits:
+      - knowledge
+      - power
+      - leisure-time
+  - name: Errands
+    traits:
+      - reliability
+      - health
+      - family
+  - name: Eating
+    traits:
+      - social
+      - health
+      - family
+  - name: Socializing
+    traits:
+      - social
+      - excitement
+      - friendship
+  - name: Drinking
+    traits:
+      - social
+      - friendship
+  - name: Relaxing
+    traits:
+      - health
+      - tranquility
+      - leisure-time
```

### Comparing `neighborly-0.9.3/src/neighborly/plugins/talktown/__init__.py` & `neighborly-0.9.4/src/neighborly/plugins/talktown/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,228 +1,183 @@
-import logging
-import os
-import pathlib
-
-import neighborly.plugins.talktown.business_archetypes as tot_businesses
-import neighborly.plugins.talktown.occupation_types as tot_occupations
-from neighborly.core.archetypes import (
-    BusinessArchetypeLibrary,
-    CharacterArchetype,
-    CharacterArchetypeLibrary,
-    ResidenceArchetype,
-    ResidenceArchetypeLibrary,
-)
-from neighborly.core.business import OccupationTypeLibrary
-from neighborly.core.ecs import World
-from neighborly.core.rng import DefaultRNG
-from neighborly.core.town import LandGrid
-from neighborly.plugins.talktown.school import SchoolSystem
-from neighborly.simulation import Plugin, Simulation
-
-logger = logging.getLogger(__name__)
-
-_RESOURCES_DIR = pathlib.Path(os.path.abspath(__file__)).parent
-
-
-def establish_town(world: World, **kwargs) -> None:
-    """
-    Adds an initial set of families and businesses
-    to the start of the town.
-
-    This system runs once, then removes itself from
-    the ECS to free resources.
-
-    Parameters
-    ----------
-    world : World
-        The world instance of the simulation
-
-    Notes
-    -----
-    This function is based on the original Simulation.establish_setting
-    method in talktown.
-    """
-    vacant_lots = town.get_component(LandGrid).layout.get_vacancies()
-    # Each family requires 2 lots (1 for a house, 1 for a business)
-    # Save two lots for either a coalmine, quarry, or farm
-    n_families_to_add = (len(vacant_lots) // 2) - 1
-
-    for _ in range(n_families_to_add - 1):
-        # create residents
-        # create Farm
-        farm = world.spawn_archetype(BusinessArchetypeLibrary.get("Farm"))
-        # trigger hiring event
-        # trigger home move event
-
-    random_num = world.get_resource(DefaultRNG).random()
-    if random_num < 0.2:
-        # Create a Coalmine 20% of the time
-        coal_mine = world.spawn_archetype(BusinessArchetypeLibrary.get("Coal Mine"))
-    elif 0.2 <= random_num < 0.35:
-        # Create a Quarry 15% of the time
-        quarry = world.spawn_archetype(BusinessArchetypeLibrary.get("Quarry"))
-    else:
-        # Create Farm 65% of the time
-        farm = world.spawn_archetype(BusinessArchetypeLibrary.get("Farm"))
-
-    logger.debug("Town established. 'establish_town' function removed from systems")
-
-
-class TalkOfTheTownPlugin(Plugin):
-    def setup(self, sim: Simulation, **kwargs) -> None:
-        sim.world.add_system(SchoolSystem())
-
-        # Talk of the town only has one residence archetype
-        ResidenceArchetypeLibrary.add(ResidenceArchetype(name="House"))
-
-        # Talk of the town only has one character archetype
-        CharacterArchetypeLibrary.add(
-            CharacterArchetype(
-                name="Person",
-                name_format="#first_name# #family_name#",
-                lifespan=85,
-                life_stages={
-                    "child": 0,
-                    "teen": 13,
-                    "young_adult": 18,
-                    "adult": 30,
-                    "elder": 65,
-                },
-            )
-        )
-
-        # Register OccupationTypes
-        OccupationTypeLibrary.add(tot_occupations.apprentice)
-        OccupationTypeLibrary.add(tot_occupations.architect)
-        OccupationTypeLibrary.add(tot_occupations.baker)
-        OccupationTypeLibrary.add(tot_occupations.banker)
-        OccupationTypeLibrary.add(tot_occupations.bank_teller)
-        OccupationTypeLibrary.add(tot_occupations.barber)
-        OccupationTypeLibrary.add(tot_occupations.barkeeper)
-        OccupationTypeLibrary.add(tot_occupations.bartender)
-        OccupationTypeLibrary.add(tot_occupations.bottler)
-        OccupationTypeLibrary.add(tot_occupations.blacksmith)
-        OccupationTypeLibrary.add(tot_occupations.brewer)
-        OccupationTypeLibrary.add(tot_occupations.bricklayer)
-        OccupationTypeLibrary.add(tot_occupations.builder)
-        OccupationTypeLibrary.add(tot_occupations.busboy)
-        OccupationTypeLibrary.add(tot_occupations.bus_driver)
-        OccupationTypeLibrary.add(tot_occupations.butcher)
-        OccupationTypeLibrary.add(tot_occupations.carpenter)
-        OccupationTypeLibrary.add(tot_occupations.cashier)
-        OccupationTypeLibrary.add(tot_occupations.clothier)
-        OccupationTypeLibrary.add(tot_occupations.concierge)
-        OccupationTypeLibrary.add(tot_occupations.cook)
-        OccupationTypeLibrary.add(tot_occupations.cooper)
-        OccupationTypeLibrary.add(tot_occupations.daycare_provider)
-        OccupationTypeLibrary.add(tot_occupations.dentist)
-        OccupationTypeLibrary.add(tot_occupations.dishwasher)
-        OccupationTypeLibrary.add(tot_occupations.distiller)
-        OccupationTypeLibrary.add(tot_occupations.doctor)
-        OccupationTypeLibrary.add(tot_occupations.dressmaker)
-        OccupationTypeLibrary.add(tot_occupations.druggist)
-        OccupationTypeLibrary.add(tot_occupations.engineer)
-        OccupationTypeLibrary.add(tot_occupations.farmer)
-        OccupationTypeLibrary.add(tot_occupations.farmhand)
-        OccupationTypeLibrary.add(tot_occupations.fire_chief)
-        OccupationTypeLibrary.add(tot_occupations.fire_fighter)
-        OccupationTypeLibrary.add(tot_occupations.grocer)
-        OccupationTypeLibrary.add(tot_occupations.groundskeeper)
-        OccupationTypeLibrary.add(tot_occupations.hotel_maid)
-        OccupationTypeLibrary.add(tot_occupations.inn_keeper)
-        OccupationTypeLibrary.add(tot_occupations.insurance_agent)
-        OccupationTypeLibrary.add(tot_occupations.janitor)
-        OccupationTypeLibrary.add(tot_occupations.jeweler)
-        OccupationTypeLibrary.add(tot_occupations.joiner)
-        OccupationTypeLibrary.add(tot_occupations.laborer)
-        OccupationTypeLibrary.add(tot_occupations.landlord)
-        OccupationTypeLibrary.add(tot_occupations.lawyer)
-        OccupationTypeLibrary.add(tot_occupations.manager)
-        OccupationTypeLibrary.add(tot_occupations.miner)
-        OccupationTypeLibrary.add(tot_occupations.milkman)
-        OccupationTypeLibrary.add(tot_occupations.mayor)
-        OccupationTypeLibrary.add(tot_occupations.molder)
-        OccupationTypeLibrary.add(tot_occupations.mortician)
-        OccupationTypeLibrary.add(tot_occupations.nurse)
-        OccupationTypeLibrary.add(tot_occupations.optometrist)
-        OccupationTypeLibrary.add(tot_occupations.owner)
-        OccupationTypeLibrary.add(tot_occupations.painter)
-        OccupationTypeLibrary.add(tot_occupations.pharmacist)
-        OccupationTypeLibrary.add(tot_occupations.plasterer)
-        OccupationTypeLibrary.add(tot_occupations.plastic_surgeon)
-        OccupationTypeLibrary.add(tot_occupations.plumber)
-        OccupationTypeLibrary.add(tot_occupations.police_chief)
-        OccupationTypeLibrary.add(tot_occupations.principal)
-        OccupationTypeLibrary.add(tot_occupations.professor)
-        OccupationTypeLibrary.add(tot_occupations.proprietor)
-        OccupationTypeLibrary.add(tot_occupations.puddler)
-        OccupationTypeLibrary.add(tot_occupations.quarry_man)
-        OccupationTypeLibrary.add(tot_occupations.realtor)
-        OccupationTypeLibrary.add(tot_occupations.seamstress)
-        OccupationTypeLibrary.add(tot_occupations.secretary)
-        OccupationTypeLibrary.add(tot_occupations.stocker)
-        OccupationTypeLibrary.add(tot_occupations.shoemaker)
-        OccupationTypeLibrary.add(tot_occupations.stonecutter)
-        OccupationTypeLibrary.add(tot_occupations.tailor)
-        OccupationTypeLibrary.add(tot_occupations.tattoo_artist)
-        OccupationTypeLibrary.add(tot_occupations.taxi_driver)
-        OccupationTypeLibrary.add(tot_occupations.teacher)
-        OccupationTypeLibrary.add(tot_occupations.turner)
-        OccupationTypeLibrary.add(tot_occupations.waiter)
-        OccupationTypeLibrary.add(tot_occupations.whitewasher)
-        OccupationTypeLibrary.add(tot_occupations.woodworker)
-
-        # Register Business Archetypes
-        BusinessArchetypeLibrary.add(tot_businesses.apartment_complex)
-        BusinessArchetypeLibrary.add(tot_businesses.bakery)
-        BusinessArchetypeLibrary.add(tot_businesses.bank)
-        BusinessArchetypeLibrary.add(tot_businesses.bar)
-        BusinessArchetypeLibrary.add(tot_businesses.barbershop)
-        BusinessArchetypeLibrary.add(tot_businesses.bus_depot)
-        BusinessArchetypeLibrary.add(tot_businesses.carpentry_company)
-        BusinessArchetypeLibrary.add(tot_businesses.cemetery)
-        BusinessArchetypeLibrary.add(tot_businesses.city_hall)
-        BusinessArchetypeLibrary.add(tot_businesses.clothing_store)
-        BusinessArchetypeLibrary.add(tot_businesses.coal_mine)
-        BusinessArchetypeLibrary.add(tot_businesses.construction_firm)
-        BusinessArchetypeLibrary.add(tot_businesses.dairy)
-        BusinessArchetypeLibrary.add(tot_businesses.day_care)
-        BusinessArchetypeLibrary.add(tot_businesses.deli)
-        BusinessArchetypeLibrary.add(tot_businesses.dentist_office)
-        BusinessArchetypeLibrary.add(tot_businesses.department_store)
-        BusinessArchetypeLibrary.add(tot_businesses.diner)
-        BusinessArchetypeLibrary.add(tot_businesses.distillery)
-        BusinessArchetypeLibrary.add(tot_businesses.drug_store)
-        BusinessArchetypeLibrary.add(tot_businesses.farm)
-        BusinessArchetypeLibrary.add(tot_businesses.fire_station)
-        BusinessArchetypeLibrary.add(tot_businesses.foundry)
-        BusinessArchetypeLibrary.add(tot_businesses.furniture_store)
-        BusinessArchetypeLibrary.add(tot_businesses.general_store)
-        BusinessArchetypeLibrary.add(tot_businesses.grocery_store)
-        BusinessArchetypeLibrary.add(tot_businesses.hardware_store)
-        BusinessArchetypeLibrary.add(tot_businesses.hospital)
-        BusinessArchetypeLibrary.add(tot_businesses.hotel)
-        BusinessArchetypeLibrary.add(tot_businesses.inn)
-        BusinessArchetypeLibrary.add(tot_businesses.insurance_company)
-        BusinessArchetypeLibrary.add(tot_businesses.jewelry_shop)
-        BusinessArchetypeLibrary.add(tot_businesses.law_firm)
-        BusinessArchetypeLibrary.add(tot_businesses.optometry_clinic)
-        BusinessArchetypeLibrary.add(tot_businesses.painting_company)
-        BusinessArchetypeLibrary.add(tot_businesses.park)
-        BusinessArchetypeLibrary.add(tot_businesses.pharmacy)
-        BusinessArchetypeLibrary.add(tot_businesses.plastic_surgery_clinic)
-        BusinessArchetypeLibrary.add(tot_businesses.plumbing_company)
-        BusinessArchetypeLibrary.add(tot_businesses.police_station)
-        BusinessArchetypeLibrary.add(tot_businesses.quarry)
-        BusinessArchetypeLibrary.add(tot_businesses.realty_firm)
-        BusinessArchetypeLibrary.add(tot_businesses.restaurant)
-        BusinessArchetypeLibrary.add(tot_businesses.school)
-        BusinessArchetypeLibrary.add(tot_businesses.shoemaker_shop)
-        BusinessArchetypeLibrary.add(tot_businesses.supermarket)
-        BusinessArchetypeLibrary.add(tot_businesses.tailor_shop)
-        BusinessArchetypeLibrary.add(tot_businesses.tattoo_parlor)
-        BusinessArchetypeLibrary.add(tot_businesses.tavern)
-        BusinessArchetypeLibrary.add(tot_businesses.taxi_depot)
-
-
-def get_plugin() -> Plugin:
-    return TalkOfTheTownPlugin()
+import logging
+import os
+import pathlib
+
+import neighborly.plugins.talktown.business_archetypes as tot_businesses
+import neighborly.plugins.talktown.occupation_types as tot_occupations
+from neighborly.builtin.archetypes import HumanArchetype
+from neighborly.core.archetypes import (
+    BaseResidenceArchetype,
+    BusinessArchetypes,
+    CharacterArchetypes,
+    ResidenceArchetypes,
+)
+from neighborly.core.business import OccupationTypes
+from neighborly.plugins.talktown.school import SchoolSystem
+from neighborly.simulation import Plugin, Simulation
+
+logger = logging.getLogger(__name__)
+
+_RESOURCES_DIR = pathlib.Path(os.path.abspath(__file__)).parent
+
+
+class TalkOfTheTownPlugin(Plugin):
+    def setup(self, sim: Simulation, **kwargs) -> None:
+        sim.world.add_system(SchoolSystem())
+
+        # Talk of the town only has one residence archetype
+        ResidenceArchetypes.add("House", BaseResidenceArchetype())
+
+        # Talk of the town only has one entity archetype
+        CharacterArchetypes.add(
+            "Person",
+            HumanArchetype(
+                life_stage_ages={
+                    "child": 0,
+                    "teen": 13,
+                    "young_adult": 18,
+                    "adult": 30,
+                    "elder": 65,
+                },
+                chance_spawn_with_spouse=1.0,
+                max_children_at_spawn=3,
+            ),
+        )
+
+        # Register OccupationTypes
+        OccupationTypes.add(tot_occupations.apprentice)
+        OccupationTypes.add(tot_occupations.architect)
+        OccupationTypes.add(tot_occupations.baker)
+        OccupationTypes.add(tot_occupations.banker)
+        OccupationTypes.add(tot_occupations.bank_teller)
+        OccupationTypes.add(tot_occupations.barber)
+        OccupationTypes.add(tot_occupations.barkeeper)
+        OccupationTypes.add(tot_occupations.bartender)
+        OccupationTypes.add(tot_occupations.bottler)
+        OccupationTypes.add(tot_occupations.blacksmith)
+        OccupationTypes.add(tot_occupations.brewer)
+        OccupationTypes.add(tot_occupations.bricklayer)
+        OccupationTypes.add(tot_occupations.builder)
+        OccupationTypes.add(tot_occupations.busboy)
+        OccupationTypes.add(tot_occupations.bus_driver)
+        OccupationTypes.add(tot_occupations.butcher)
+        OccupationTypes.add(tot_occupations.carpenter)
+        OccupationTypes.add(tot_occupations.cashier)
+        OccupationTypes.add(tot_occupations.clothier)
+        OccupationTypes.add(tot_occupations.concierge)
+        OccupationTypes.add(tot_occupations.cook)
+        OccupationTypes.add(tot_occupations.cooper)
+        OccupationTypes.add(tot_occupations.daycare_provider)
+        OccupationTypes.add(tot_occupations.dentist)
+        OccupationTypes.add(tot_occupations.dishwasher)
+        OccupationTypes.add(tot_occupations.distiller)
+        OccupationTypes.add(tot_occupations.doctor)
+        OccupationTypes.add(tot_occupations.dressmaker)
+        OccupationTypes.add(tot_occupations.druggist)
+        OccupationTypes.add(tot_occupations.engineer)
+        OccupationTypes.add(tot_occupations.farmer)
+        OccupationTypes.add(tot_occupations.farmhand)
+        OccupationTypes.add(tot_occupations.fire_chief)
+        OccupationTypes.add(tot_occupations.fire_fighter)
+        OccupationTypes.add(tot_occupations.grocer)
+        OccupationTypes.add(tot_occupations.groundskeeper)
+        OccupationTypes.add(tot_occupations.hotel_maid)
+        OccupationTypes.add(tot_occupations.inn_keeper)
+        OccupationTypes.add(tot_occupations.insurance_agent)
+        OccupationTypes.add(tot_occupations.janitor)
+        OccupationTypes.add(tot_occupations.jeweler)
+        OccupationTypes.add(tot_occupations.joiner)
+        OccupationTypes.add(tot_occupations.laborer)
+        OccupationTypes.add(tot_occupations.landlord)
+        OccupationTypes.add(tot_occupations.lawyer)
+        OccupationTypes.add(tot_occupations.manager)
+        OccupationTypes.add(tot_occupations.miner)
+        OccupationTypes.add(tot_occupations.milkman)
+        OccupationTypes.add(tot_occupations.mayor)
+        OccupationTypes.add(tot_occupations.molder)
+        OccupationTypes.add(tot_occupations.mortician)
+        OccupationTypes.add(tot_occupations.nurse)
+        OccupationTypes.add(tot_occupations.optometrist)
+        OccupationTypes.add(tot_occupations.owner)
+        OccupationTypes.add(tot_occupations.painter)
+        OccupationTypes.add(tot_occupations.pharmacist)
+        OccupationTypes.add(tot_occupations.plasterer)
+        OccupationTypes.add(tot_occupations.plastic_surgeon)
+        OccupationTypes.add(tot_occupations.plumber)
+        OccupationTypes.add(tot_occupations.police_chief)
+        OccupationTypes.add(tot_occupations.police_officer)
+        OccupationTypes.add(tot_occupations.principal)
+        OccupationTypes.add(tot_occupations.professor)
+        OccupationTypes.add(tot_occupations.proprietor)
+        OccupationTypes.add(tot_occupations.puddler)
+        OccupationTypes.add(tot_occupations.quarry_man)
+        OccupationTypes.add(tot_occupations.realtor)
+        OccupationTypes.add(tot_occupations.seamstress)
+        OccupationTypes.add(tot_occupations.secretary)
+        OccupationTypes.add(tot_occupations.stocker)
+        OccupationTypes.add(tot_occupations.shoemaker)
+        OccupationTypes.add(tot_occupations.stonecutter)
+        OccupationTypes.add(tot_occupations.tailor)
+        OccupationTypes.add(tot_occupations.tattoo_artist)
+        OccupationTypes.add(tot_occupations.taxi_driver)
+        OccupationTypes.add(tot_occupations.teacher)
+        OccupationTypes.add(tot_occupations.turner)
+        OccupationTypes.add(tot_occupations.waiter)
+        OccupationTypes.add(tot_occupations.whitewasher)
+        OccupationTypes.add(tot_occupations.woodworker)
+
+        # Register Business Archetypes
+        BusinessArchetypes.add("Bakery", tot_businesses.bakery)
+        BusinessArchetypes.add("Bank", tot_businesses.bank)
+        BusinessArchetypes.add("Bar", tot_businesses.bar)
+        BusinessArchetypes.add("BarberShop", tot_businesses.barbershop)
+        BusinessArchetypes.add("BusDepot", tot_businesses.bus_depot)
+        BusinessArchetypes.add("CarpentryCompany", tot_businesses.carpentry_company)
+        BusinessArchetypes.add("Cemetery", tot_businesses.cemetery)
+        BusinessArchetypes.add("CityHall", tot_businesses.city_hall)
+        BusinessArchetypes.add("ClothingStore", tot_businesses.clothing_store)
+        BusinessArchetypes.add("CoalMine", tot_businesses.coal_mine)
+        BusinessArchetypes.add("ConstructionFirm", tot_businesses.construction_firm)
+        BusinessArchetypes.add("Dairy", tot_businesses.dairy)
+        BusinessArchetypes.add("DayCare", tot_businesses.day_care)
+        BusinessArchetypes.add("Deli", tot_businesses.deli)
+        BusinessArchetypes.add("DentistOffice", tot_businesses.dentist_office)
+        BusinessArchetypes.add("DepartmentStore", tot_businesses.department_store)
+        BusinessArchetypes.add("Dinner", tot_businesses.diner)
+        BusinessArchetypes.add("Distillery", tot_businesses.distillery)
+        BusinessArchetypes.add("DrugStore", tot_businesses.drug_store)
+        BusinessArchetypes.add("Farm", tot_businesses.farm)
+        BusinessArchetypes.add("FireStation", tot_businesses.fire_station)
+        BusinessArchetypes.add("Foundry", tot_businesses.foundry)
+        BusinessArchetypes.add("FurnitureStore", tot_businesses.furniture_store)
+        BusinessArchetypes.add("GeneralStore", tot_businesses.general_store)
+        BusinessArchetypes.add("GroceryStore", tot_businesses.grocery_store)
+        BusinessArchetypes.add("HardwareStore", tot_businesses.hardware_store)
+        BusinessArchetypes.add("Hospital", tot_businesses.hospital)
+        BusinessArchetypes.add("Hotel", tot_businesses.hotel)
+        BusinessArchetypes.add("Inn", tot_businesses.inn)
+        BusinessArchetypes.add("InsuranceCompany", tot_businesses.insurance_company)
+        BusinessArchetypes.add("JewelryShop", tot_businesses.jewelry_shop)
+        BusinessArchetypes.add("LawFirm", tot_businesses.law_firm)
+        BusinessArchetypes.add("OptometryClinic", tot_businesses.optometry_clinic)
+        BusinessArchetypes.add("PaintingCompany", tot_businesses.painting_company)
+        BusinessArchetypes.add("Park", tot_businesses.park)
+        BusinessArchetypes.add("Pharmacy", tot_businesses.pharmacy)
+        BusinessArchetypes.add(
+            "PlasticSurgeryClinic", tot_businesses.plastic_surgery_clinic
+        )
+        BusinessArchetypes.add("PlumbingCompany", tot_businesses.plumbing_company)
+        BusinessArchetypes.add("PoliceStation", tot_businesses.police_station)
+        BusinessArchetypes.add("Quarry", tot_businesses.quarry)
+        BusinessArchetypes.add("RealtyFirm", tot_businesses.realty_firm)
+        BusinessArchetypes.add("Restaurant", tot_businesses.restaurant)
+        BusinessArchetypes.add("School", tot_businesses.school)
+        BusinessArchetypes.add("ShoemakerShop", tot_businesses.shoemaker_shop)
+        BusinessArchetypes.add("SuperMarket", tot_businesses.supermarket)
+        BusinessArchetypes.add("TailorShop", tot_businesses.tailor_shop)
+        BusinessArchetypes.add("TattooParlor", tot_businesses.tattoo_parlor)
+        BusinessArchetypes.add("Tavern", tot_businesses.tavern)
+        BusinessArchetypes.add("TaxiDepot", tot_businesses.taxi_depot)
+
+
+def get_plugin() -> Plugin:
+    return TalkOfTheTownPlugin()
```

### Comparing `neighborly-0.9.3/src/neighborly/plugins/talktown/personality.py` & `neighborly-0.9.4/src/neighborly/plugins/talktown/personality.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-"""
-Talk of the Town uses a Big 5 personality model
-to make character decisions and determine
-compatibility in social interactions
-"""
-from __future__ import annotations
-
-from typing import Any, Dict
-
-from neighborly.core.ecs import Component, World
-from neighborly.core.engine import NeighborlyEngine
-
-BIG_FIVE_FLOOR = -1.0
-BIG_FIVE_CAP = 1.0
-
-
-class BigFivePersonality(Component):
-    """Relationship model"""
-
-    __slots__ = (
-        "openness",
-        "conscientiousness",
-        "extroversion",
-        "agreeableness",
-        "neuroticism",
-    )
-
-    def __init__(
-        self,
-        openness: float = 0,
-        conscientiousness: float = 0,
-        extroversion: float = 0,
-        agreeableness: float = 0,
-        neuroticism: float = 0,
-    ) -> None:
-        super().__init__()
-        self.openness: float = openness
-        self.conscientiousness: float = conscientiousness
-        self.extroversion: float = extroversion
-        self.agreeableness: float = agreeableness
-        self.neuroticism: float = neuroticism
-
-    def to_dict(self) -> Dict[str, Any]:
-        return {
-            **super().to_dict(),
-            "openness": self.openness,
-            "conscientiousness": self.conscientiousness,
-            "extroversion": self.extroversion,
-            "agreeableness": self.agreeableness,
-            "neuroticism": self.neuroticism,
-        }
-
-    @classmethod
-    def create(cls, world: World, **kwargs) -> BigFivePersonality:
-        """Create new instance given component spec"""
-        engine: NeighborlyEngine = kwargs["engine"]
-
-        openness: float = (
-                              engine.rng.random() * (BIG_FIVE_CAP - BIG_FIVE_FLOOR)
-                          ) + BIG_FIVE_FLOOR
-
-        conscientiousness: float = (
-                                       engine.rng.random() * (BIG_FIVE_CAP - BIG_FIVE_FLOOR)
-                                   ) + BIG_FIVE_FLOOR
-
-        extroversion: float = (
-                                  engine.rng.random() * (BIG_FIVE_CAP - BIG_FIVE_FLOOR)
-                              ) + BIG_FIVE_FLOOR
-
-        agreeableness: float = (
-                                   engine.rng.random() * (BIG_FIVE_CAP - BIG_FIVE_FLOOR)
-                               ) + BIG_FIVE_FLOOR
-
-        neuroticism: float = (
-                                 engine.rng.random() * (BIG_FIVE_CAP - BIG_FIVE_FLOOR)
-                             ) + BIG_FIVE_FLOOR
-
-        return cls(
-            openness, conscientiousness, extroversion, agreeableness, neuroticism
-        )
-
-    def __repr__(self) -> str:
-        return self.to_dict().__repr__()
+"""
+Talk of the Town uses a Big 5 personality model
+to make entity decisions and determine
+compatibility in social interactions
+"""
+from __future__ import annotations
+
+from typing import Any, Dict
+
+from neighborly.core.ecs import Component, World
+from neighborly.core.engine import NeighborlyEngine
+
+BIG_FIVE_FLOOR = -1.0
+BIG_FIVE_CAP = 1.0
+
+
+class BigFivePersonality(Component):
+    """Relationship model"""
+
+    __slots__ = (
+        "openness",
+        "conscientiousness",
+        "extroversion",
+        "agreeableness",
+        "neuroticism",
+    )
+
+    def __init__(
+        self,
+        openness: float = 0,
+        conscientiousness: float = 0,
+        extroversion: float = 0,
+        agreeableness: float = 0,
+        neuroticism: float = 0,
+    ) -> None:
+        super().__init__()
+        self.openness: float = openness
+        self.conscientiousness: float = conscientiousness
+        self.extroversion: float = extroversion
+        self.agreeableness: float = agreeableness
+        self.neuroticism: float = neuroticism
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            **super().to_dict(),
+            "openness": self.openness,
+            "conscientiousness": self.conscientiousness,
+            "extroversion": self.extroversion,
+            "agreeableness": self.agreeableness,
+            "neuroticism": self.neuroticism,
+        }
+
+    @classmethod
+    def create(cls, world: World, **kwargs) -> BigFivePersonality:
+        """Create new instance given component spec"""
+        engine: NeighborlyEngine = kwargs["engine"]
+
+        openness: float = (
+            engine.rng.random() * (BIG_FIVE_CAP - BIG_FIVE_FLOOR)
+        ) + BIG_FIVE_FLOOR
+
+        conscientiousness: float = (
+            engine.rng.random() * (BIG_FIVE_CAP - BIG_FIVE_FLOOR)
+        ) + BIG_FIVE_FLOOR
+
+        extroversion: float = (
+            engine.rng.random() * (BIG_FIVE_CAP - BIG_FIVE_FLOOR)
+        ) + BIG_FIVE_FLOOR
+
+        agreeableness: float = (
+            engine.rng.random() * (BIG_FIVE_CAP - BIG_FIVE_FLOOR)
+        ) + BIG_FIVE_FLOOR
+
+        neuroticism: float = (
+            engine.rng.random() * (BIG_FIVE_CAP - BIG_FIVE_FLOOR)
+        ) + BIG_FIVE_FLOOR
+
+        return cls(
+            openness, conscientiousness, extroversion, agreeableness, neuroticism
+        )
+
+    def __repr__(self) -> str:
+        return self.to_dict().__repr__()
```

### Comparing `neighborly-0.9.3/src/neighborly/plugins/talktown/utils.py` & `neighborly-0.9.4/src/neighborly/plugins/talktown/utils.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-from dataclasses import dataclass, field
-from heapq import heappush
-from typing import Generic, TypeVar, Union, List, Tuple
-
-_T = TypeVar("_T")
-
-
-def clamp(
-    value: Union[float, int], minimum: Union[float, int], maximum: Union[float, int]
-) -> Union[float, int]:
-    """
-    Clamp numerical value between a [min, max] interval
-
-    Parameters
-    ----------
-    value : Union[float, int]
-        Value to clamp
-    minimum : Union[float, int]
-        Minimum value to return
-    maximum : Union[float, int]
-        Maximum value that can be returned
-
-    Returns
-    -------
-    Union[float, int]
-    """
-    return max(minimum, min(value, maximum))
-
-
-def choose_from_scored_options(options: List[Tuple[_T, float]]) -> _T:
-    """Probabilistically chose one item from a list using their scores as weights"""
-    items, scores = tuple(zip(*options))
-    chosen_item: _T = random.choices(items, weights=scores, k=1)[0]  # type: ignore
-    return chosen_item
-
-
-def int_to_roman(num: int) -> str:
-    """Convert a given int to a Roman numeral string"""
-    # From https://www.w3resource.com/python-exercises/class-exercises/python-class-exercise-1.php
-    lookup = [
-        (1000, "M"),
-        (900, "CM"),
-        (500, "D"),
-        (400, "CD"),
-        (100, "C"),
-        (90, "XC"),
-        (50, "L"),
-        (40, "XL"),
-        (10, "X"),
-        (9, "IX"),
-        (5, "V"),
-        (4, "IV"),
-        (1, "I"),
-    ]
-    res = ""
-    for (n, roman) in lookup:
-        (d, num) = divmod(num, n)
-        res += roman * d
-    return res
-
-
-def roman_to_int(roman: str) -> int:
-    """Convert Roman numeral string to int"""
-    roman_lookup = {
-        "I": 1,
-        "IV": 4,
-        "V": 5,
-        "IX": 9,
-        "X": 10,
-        "XL": 40,
-        "L": 50,
-        "XC": 90,
-        "C": 100,
-        "CD": 400,
-        "D": 500,
-        "CM": 900,
-        "M": 1000,
-    }
-
-    i = 0
-    num = 0
-    while i < len(roman):
-        if i + 1 < len(roman) and roman[i: i + 2] in roman_lookup:
-            num += roman_lookup[roman[i: i + 2]]
-            i += 2
-        else:
-            # print(i)
-            num += roman_lookup[roman[i]]
-            i += 1
-    return num
-
-
-def int_to_ordinal(num: int) -> str:
-    """
-    Returns ordinal number string from int, e.g. 1, 2, 3 becomes 1st, 2nd, 3rd, etc.
-    """
-    n = int(num)
-    if 4 <= n <= 20:
-        return f"{n}th"
-    elif n == 1 or (n % 10) == 1:
-        return f"{n}st"
-    elif n == 2 or (n % 10) == 2:
-        return f"{n}nd"
-    elif n == 3 or (n % 10) == 3:
-        return f"{n}rd"
-    elif n < 100:
-        return f"{n}th"
-    return f"{n}th"
-
-
-@dataclass(order=True)
-class PrioritizedItem(Generic[_T]):
-    priority: float
-    item: _T = field(compare=False)
-
-
-class PriorityQueue(Generic[_T]):
-    def __init__(self) -> None:
-        self._queue: List[PrioritizedItem[_T]] = []
-
-    def push(self, priority: float, item: _T) -> None:
-        heappush(self._queue, PrioritizedItem[_T](priority, item))
-
-    def pop(self) -> _T:
-        return self._queue.pop(0).item
-
-    def __repr__(self) -> str:
-        return self._queue.__repr__()
+from dataclasses import dataclass, field
+from heapq import heappush
+from typing import Generic, TypeVar, Union, List, Tuple
+
+_T = TypeVar("_T")
+
+
+def clamp(
+    value: Union[float, int], minimum: Union[float, int], maximum: Union[float, int]
+) -> Union[float, int]:
+    """
+    Clamp numerical value between a [min, max] interval
+
+    Parameters
+    ----------
+    value : Union[float, int]
+        Value to clamp
+    minimum : Union[float, int]
+        Minimum value to return
+    maximum : Union[float, int]
+        Maximum value that can be returned
+
+    Returns
+    -------
+    Union[float, int]
+    """
+    return max(minimum, min(value, maximum))
+
+
+def choose_from_scored_options(options: List[Tuple[_T, float]]) -> _T:
+    """Probabilistically chose one item from a list using their scores as weights"""
+    items, scores = tuple(zip(*options))
+    chosen_item: _T = random.choices(items, weights=scores, k=1)[0]  # type: ignore
+    return chosen_item
+
+
+def int_to_roman(num: int) -> str:
+    """Convert a given int to a Roman numeral string"""
+    # From https://www.w3resource.com/python-exercises/class-exercises/python-class-exercise-1.php
+    lookup = [
+        (1000, "M"),
+        (900, "CM"),
+        (500, "D"),
+        (400, "CD"),
+        (100, "C"),
+        (90, "XC"),
+        (50, "L"),
+        (40, "XL"),
+        (10, "X"),
+        (9, "IX"),
+        (5, "V"),
+        (4, "IV"),
+        (1, "I"),
+    ]
+    res = ""
+    for (n, roman) in lookup:
+        (d, num) = divmod(num, n)
+        res += roman * d
+    return res
+
+
+def roman_to_int(roman: str) -> int:
+    """Convert Roman numeral string to int"""
+    roman_lookup = {
+        "I": 1,
+        "IV": 4,
+        "V": 5,
+        "IX": 9,
+        "X": 10,
+        "XL": 40,
+        "L": 50,
+        "XC": 90,
+        "C": 100,
+        "CD": 400,
+        "D": 500,
+        "CM": 900,
+        "M": 1000,
+    }
+
+    i = 0
+    num = 0
+    while i < len(roman):
+        if i + 1 < len(roman) and roman[i: i + 2] in roman_lookup:
+            num += roman_lookup[roman[i: i + 2]]
+            i += 2
+        else:
+            # print(i)
+            num += roman_lookup[roman[i]]
+            i += 1
+    return num
+
+
+def int_to_ordinal(num: int) -> str:
+    """
+    Returns ordinal number string from int, e.g. 1, 2, 3 becomes 1st, 2nd, 3rd, etc.
+    """
+    n = int(num)
+    if 4 <= n <= 20:
+        return f"{n}th"
+    elif n == 1 or (n % 10) == 1:
+        return f"{n}st"
+    elif n == 2 or (n % 10) == 2:
+        return f"{n}nd"
+    elif n == 3 or (n % 10) == 3:
+        return f"{n}rd"
+    elif n < 100:
+        return f"{n}th"
+    return f"{n}th"
+
+
+@dataclass(order=True)
+class PrioritizedItem(Generic[_T]):
+    priority: float
+    item: _T = field(compare=False)
+
+
+class PriorityQueue(Generic[_T]):
+    def __init__(self) -> None:
+        self._queue: List[PrioritizedItem[_T]] = []
+
+    def push(self, priority: float, item: _T) -> None:
+        heappush(self._queue, PrioritizedItem[_T](priority, item))
+
+    def pop(self) -> _T:
+        return self._queue.pop(0).item
+
+    def __repr__(self) -> str:
+        return self._queue.__repr__()
```

### Comparing `neighborly-0.9.3/src/neighborly/plugins/weather_plugin.py` & `neighborly-0.9.4/src/neighborly/plugins/weather.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,76 @@
-from enum import Enum
-
-from neighborly.core.ecs import ISystem
-from neighborly.core.engine import NeighborlyEngine
-from neighborly.core.time import SimDateTime
-from neighborly.simulation import Plugin, Simulation
-
-
-class Weather(Enum):
-    """Weather status"""
-
-    SUNNY = "sunny"
-    RAINING = "raining"
-    PARTIALLY_CLOUDY = "partially cloudy"
-    OVERCAST = "overcast"
-
-
-class WeatherManager:
-    """Manages the weather in the town
-
-    Attributes
-    ----------
-    current_weather : Weather
-        Current weather in the town
-    time_before_change : int
-        Number of hours before the weather
-        pattern changes
-    """
-
-    __slots__ = "current_weather", "time_before_change"
-
-    def __init__(self, default: Weather = Weather.SUNNY) -> None:
-        self.current_weather: Weather = default
-        self.time_before_change: int = 0
-
-
-class WeatherSystem(ISystem):
-    """Updates the current weather state
-
-    Attributes
-    ----------
-    avg_change_interval: int
-        Average number of hours that the current weather
-        state will last before being changed
-    """
-
-    def __init__(self, avg_change_interval: int = 24) -> None:
-        super().__init__()
-        self.avg_change_interval: int = avg_change_interval
-
-    def process(self, *args, **kwargs):
-        delta_time = self.world.get_resource(SimDateTime).delta_time
-        weather_manager = self.world.get_resource(WeatherManager)
-        engine = self.world.get_resource(NeighborlyEngine)
-
-        if weather_manager.time_before_change <= 0:
-            # Select the next weather pattern
-            weather_manager.current_weather = engine.rng.choice(list(Weather))
-            weather_manager.time_before_change = round(
-                engine.rng.normalvariate(mu=self.avg_change_interval, sigma=1)
-            )
-
-        weather_manager.time_before_change -= delta_time
-
-
-class WeatherPlugin(Plugin):
-    def setup(self, sim: Simulation, **kwargs) -> None:
-        sim.world.add_system(WeatherSystem(), 9)
-        sim.world.add_resource(WeatherManager())
-
-
-def get_plugin() -> Plugin:
-    return WeatherPlugin()
+from enum import Enum
+
+from neighborly.core.ecs import ISystem
+from neighborly.core.engine import NeighborlyEngine
+from neighborly.core.time import SimDateTime
+from neighborly.simulation import Plugin, Simulation
+
+
+class Weather(Enum):
+    """Weather status"""
+
+    SUNNY = "sunny"
+    RAINING = "raining"
+    PARTIALLY_CLOUDY = "partially cloudy"
+    OVERCAST = "overcast"
+
+
+class WeatherManager:
+    """Manages the weather in the town
+
+    Attributes
+    ----------
+    current_weather : Weather
+        Current weather in the town
+    time_before_change : int
+        Number of hours before the weather
+        pattern changes
+    """
+
+    __slots__ = "current_weather", "time_before_change"
+
+    def __init__(self, default: Weather = Weather.SUNNY) -> None:
+        self.current_weather: Weather = default
+        self.time_before_change: int = 0
+
+    def __repr__(self) -> str:
+        return f"Weather({str(self.current_weather.value)})"
+
+
+class WeatherSystem(ISystem):
+    """Updates the current weather state
+
+    Attributes
+    ----------
+    avg_change_interval: int
+        Average number of hours that the current weather
+        state will last before being changed
+    """
+
+    def __init__(self, avg_change_interval: int = 24) -> None:
+        super().__init__()
+        self.avg_change_interval: int = avg_change_interval
+
+    def process(self, *args, **kwargs):
+        delta_time = self.world.get_resource(SimDateTime).delta_time
+        weather_manager = self.world.get_resource(WeatherManager)
+        engine = self.world.get_resource(NeighborlyEngine)
+
+        if weather_manager.time_before_change <= 0:
+            # Select the next weather pattern
+            weather_manager.current_weather = engine.rng.choice(list(Weather))
+            weather_manager.time_before_change = round(
+                engine.rng.normalvariate(mu=self.avg_change_interval, sigma=1)
+            )
+
+        weather_manager.time_before_change -= delta_time
+
+
+class WeatherPlugin(Plugin):
+    def setup(self, sim: Simulation, **kwargs) -> None:
+        sim.world.add_system(WeatherSystem(), 9)
+        sim.world.add_resource(WeatherManager())
+
+
+def get_plugin() -> Plugin:
+    return WeatherPlugin()
```

### Comparing `neighborly-0.9.3/src/neighborly.egg-info/PKG-INFO` & `neighborly-0.9.4/src/neighborly.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,198 +1,247 @@
-Metadata-Version: 2.1
-Name: neighborly
-Version: 0.9.3
-Summary: An extensible social simulation engine for generating towns of characters
-Home-page: https://github.com/ShiJbey/neighborly
-Author: Shi Johnson-Bey
-Author-email: shijbey@ucsc.edu
-License: MIT
-Project-URL: Bug Tracker, https://github.com/ShiJbey/neighborly/issues
-Keywords: social simulation,emergent narrative,life simulator framework,multi-agent
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Games/Entertainment :: Simulation
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Artificial Life
-Classifier: Topic :: Sociology
-Classifier: Typing :: Typed
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: samples
-License-File: LICENSE
-
-<h1 align="center">
-  <img
-    width="300"
-    height="300"
-    src="https://user-images.githubusercontent.com/11076525/165836171-9ffdea6e-1633-440c-be06-b46e1e3e4e04.png"
-  >
-  <br>
-  Neighborly
-</h1>
-
-<h3 align="center"><b>Social simulation engine for procedurally generating towns of characters</b></h2>
-
-<p align="center">
-  <img src="https://img.shields.io/pypi/dm/neighborly">
-  <img src="https://img.shields.io/pypi/l/neighborly">
-  <img src="https://img.shields.io/pypi/v/neighborly">
-  <img src="https://img.shields.io/pypi/pyversions/neighborly">
-</p>
-
-# Overview
-
-Neighborly is a social simulation engine for procedurally generating towns of characters. It simulates
-the lives of each character, their jobs, routines, relationships, and life events. Neighborly utilizes
-an entity-component system architecture, and enables users to specify custom character types, businesses,
-occupations, life events, and AI components and simulation systems.
-
-Neighborly takes lessons learned from working with
-[_Talk of the Town_](https://github.com/james-owen-ryan/talktown)
-and aims to give people better documentation, simpler interfaces, and more opportunities for extension and content authoring.
-
-<b>Neighborly is not fully functional yet. I am actively working toward a working release.</b>
-
-# Core Features
-
-* Create custom Character Archetypes and have them all interact within the same simulation
-* Create custom Business and Occupation definitions
-* Configure simulation data using YAML or in code with Python
-* Plugin architecture allows users to modularize and share their custom content
-* Low fidelity simulation simulates the macro events in character's lives (relationship milestones, job changes, victories, tragic events)
-* Export simulation state to JSON for further data processing
-
-# Tutorials and How-to Guides
-
-I plan to add these after I have finished implementing Neighborly's core
-functionality. I will try to align them with the sample projects, but we
-will see how the first pre-release looks. For now, loosely refer to the
-samples. Although, they too lag behind breaking changes to the core codebase.
-
-# Installing from PyPI
-
-Neighborly is available to install via pip.
-
-```bash
-pip install neighborly
-```
-
-# Installing for local development
-
-If you wish to download a Neighborly for local development, follow the these instructions.
-
-```bash
-# Step One: Clone Repository
-git clone https://github.com/ShiJbey/neighborly.git
-
-# Step Two (Optional): Create and activate python virtual environment
-cd neighborly
-
-# For Linux and MacOS
-python3 -m venv venv
-source ./venv/bin/activate
-
-# For Windows
-python -m venv venv
-./venv/Scripts/Activate
-
-# Step Three: Install local build and dependencies
-python -m pip install -e "."
-```
-
-# Running the Tests
-
-The tests are currently out-of-date and may refer to systems
-and logic that no longer exists in Neighborly. The codebase
-changes so frequently that it hasn't been worth the time. 
-As modules  become more established, I will add proper tests for them. 
-Feel free to contribute tests by forking the repo, adding your test(s), and
-submitting a pull request with a description of your test cases. Your commits
-should only contain changes to files within the `tests` directory. If you
-change any files in other parts of the project, your PR will be rejected.
-
-Please follow the steps below to run Neighborly's test suite. Neighborly uses
-[PyTest](https://docs.pytest.org/en/7.1.x/) to handle unit testing.
-
-```bash
-# Step 1: Install dependencies for tests
-python -m pip install -e ".[tests]"
-
-# Step 2: Run Pytest
-pytest
-```
-
-# Running the Samples
-
-Please follow the steps below to run the sample simulations.
-We also have examples for using Neighborly in a IPython
-notebook and with PyGame.
-
-```bash
-# Step 1: Install dependencies for samples
-python -m pip install -e ".[samples]"
-
-# Step 2: Run desired sample
-python ./samples/<sample_name>.py
-```
-
-# Documentation
-
-Neighborly uses [Numpy-style](https://numpydoc.readthedocs.io/en/latest/format.html) docstrings in code and full documentation can be found in the [Wiki](https://github.com/ShiJbey/neighborly/wiki).
-
-When adding docstrings for existing or new bits of code please use the following
-references for how to format your contributions:
-
-* [Sphinx Napoleon Plugin for processing Numpy Docstrings](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html)
-* [Example Numpy Style Docstrings](https://www.sphinx-doc.org/en/master/usage/extensions/example_numpy.html#example-numpy)
-
-
-# Contributing
-
-If you are interested in contributing to Neighborly, feel free to fork this repository, make your changes, and submit a pull-request. Please keep in mind that this project is a tool for creativity and learning. We have a [code of conduct](./CODE_OF_CONDUCT.md) to encourage healthy collaboration, and will enforce it if we need to.
-
-**WARNING::** This repository's structure in high flux. Parts of the code get shifted to make the APIs cleaner for use.
-
-Here are some ways that people can contribute to Neighborly:
-
-1. Proposing/Implementing new features
-2. Fixing bugs
-3. Providing optimizations
-4. Fixing typos
-5. Filing issues
-6. Contributing tutorials/how-tos to the wiki
-7. Fixing grammar and spelling in the wiki
-8. Creating new samples
-
-## Code Style
-
-Neighborly does not have a set-in-stone code style yet, but I have started integrating
-isort, black, and flake8 into the development workflow in VSCode.
-
-You can follow [these instructions](https://black.readthedocs.io/en/stable/integrations/editors.html) for setting up both black and isort. And I found this gist helpful for getting [flake8 working in PyCharm](https://gist.github.com/tossmilestone/23139d870841a3d5cba2aea28da1a895).
-
-# Notes
-
-## Non-Deterministic Behavior
-
-The goal of having a seeded pseudo random simulation is so that users experience deterministic behavior when using the
-same starting seed. We try to remove all forms of non-determinism, but some slip through. The known areas are listed
-below. If you find any, please make a new issue with details of the behavior.
-
-* Names may not be consistent when using the same seed. Currently, names are generated
-  using [Tracery](https://github.com/aparrish/pytracery). We would need to create a custom version that uses an RNG
-  instance instead of the global random module to generate names.
-
-## DMCA Statement
-
-Upon receipt of a notice alleging copyright infringement, I will take whatever action it deems
-appropriate within its sole discretion, including removal of the allegedly infringing materials.
-
-The repo image is something fun that I made. I love _The Simpsons_, and I couldn't think of anything more neighborly
-than Ned Flanders. If the copyright owner for _The Simpsons_ would like me to take it down,
-please contact me.
-
-The same takedown policy applies to any code samples inspired by TV shows, movies, and games.
+Metadata-Version: 2.1
+Name: neighborly
+Version: 0.9.4
+Summary: An extensible social simulation framework for generating towns of characters
+Home-page: https://github.com/ShiJbey/neighborly
+Author: Shi Johnson-Bey
+Author-email: shijbey@ucsc.edu
+License: MIT
+Project-URL: Bug Tracker, https://github.com/ShiJbey/neighborly/issues
+Project-URL: Documentation, https://github.com/ShiJbey/neighborly/wiki
+Project-URL: Changelog, https://github.com/ShiJbey/neighborly/blob/main/CHANGELOG.md
+Keywords: social simulation,emergent narrative,life simulator,multi-agent framework
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Games/Entertainment :: Simulation
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Artificial Life
+Classifier: Topic :: Sociology
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+License-File: LICENSE
+
+<h1 align="center">
+  <img
+    width="150"
+    height="150"
+    src="https://user-images.githubusercontent.com/11076525/165836171-9ffdea6e-1633-440c-be06-b46e1e3e4e04.png"
+  >
+  <br>
+  Neighborly
+</h1>
+
+<p align="center">
+  <img src="https://img.shields.io/badge/status-unstable-critical?style=flat">
+  <img src="https://img.shields.io/pypi/v/neighborly">
+  <img src="https://img.shields.io/pypi/pyversions/neighborly">
+  <img src="https://img.shields.io/pypi/l/neighborly">
+  <img src="https://img.shields.io/pypi/dm/neighborly">
+  <img src="https://img.shields.io/badge/code%20style-black-black">
+  <img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336">
+</p>
+
+# Overview
+
+Neighborly is a Python framework for generating and forward simulating towns of
+characters over large periods of time (decades to centuries). It uses a character-driven
+social simulation that forward-simulates the lives of each character, their jobs,
+routines, relationships, and life events. Users can specify custom characters,
+residential/commercial buildings, occupations, life events, social actions, and more.
+
+Currently, _Neighborly_ works best as narrative data generator. When the simulation
+ends, users can save the history of events, characters, relationships, and other stuff.
+
+Neighborly was inspired by lessons learned from working with
+[_Talk of the Town_](https://github.com/james-owen-ryan/talktown)
+and aims to give people better documentation, simpler interfaces, and more opportunities
+for extension and content authoring.
+
+## Core Features
+
+* Create custom character, buildings, life events, and social actions
+* Commandline interface (CLI) tool
+* Configure the CLI using YAML text files
+* Plugin architecture allows users to modularize and share their custom content
+* Export simulation state to JSON for further data processing
+
+# How to use
+
+Below are instructions for installing Neighborly and the options one has for using it
+in their projects. If you want examples of how to use Neighborly and how to extend it
+with custom content, please refer to
+[Neighborly's wiki](https://github.com/ShiJbey/neighborly/wiki) and the sample scripts
+in the [_samples_ directory](https://github.com/ShiJbey/neighborly/tree/main/samples).
+
+## Installation
+
+Neighborly is available to install from PyPI.
+
+```bash
+pip install neighborly
+```
+
+Or you can install it by cloning the main branch of this repo and installing that.
+
+```bash
+git clone https://github.com/ShiJbey/neighborly.git
+
+cd neighborly
+
+python -m pip install .
+```
+
+## Using as a library
+
+Neighborly can be used as a library within a Python script or package.
+The `samples` directory contains python scripts that use Neighborly this
+way. Please refer to them when creating new Plugins and other content.
+
+## Running the CLI
+
+Neighborly can be run as a module `$ python -m neighborly` or commandline `$ neighborly`
+script. If you require additional help while running, please use
+`python -m neighborly --help` or `neighborly --help`.
+
+By default, Neighborly runs a builtin version of **Talk of the Town**. However, you can
+configure the simulation settings by creating a `neighborlyconfig.yaml` file in
+the same directory where you're running the CLI. Please refer to the
+[wiki](https://github.com/ShiJbey/neighborly/wiki/Neighborly-CLI) for a list of
+valid configuration settings.
+
+When world generation concludes, Neighborly can write the final simulation data
+to a JSON file with the name of the town and the seed used for random number
+generation.
+
+## Running the Samples
+
+Neighborly provides sample simulations to show users how to customize
+it to create new story world themes.
+
+```bash
+# Make sure that you've activated your python virtual environment
+# Replace <sample_name>.py with the name of the
+# sample you want to run
+python ./samples/<sample_name>.py
+```
+
+## Installing for local development
+
+If you wish to download a Neighborly for local development, you need to clone/fork this
+repository and install using the _editable_ flag (-e). Please see the instructions
+below.
+
+```bash
+# Step One: Clone Repository
+git clone https://github.com/ShiJbey/neighborly.git
+
+# Step Two (Optional): Create and activate python virtual environment
+cd neighborly
+
+# For Linux and MacOS
+python3 -m venv venv
+source ./venv/bin/activate
+
+# For Windows
+python -m venv venv
+./venv/Scripts/Activate
+
+# Step Three: Install local build and dependencies
+python -m pip install -e "."
+```
+
+## Running the Tests
+
+The tests are currently out-of-date and may refer to systems
+and logic that no longer exists in Neighborly. The codebase
+changes so frequently that it hasn't been worth the time.
+As modules  become more established, I will add proper tests for them.
+Feel free to contribute tests by forking the repo, adding your test(s), and
+submitting a pull request with a description of your test cases. Your commits
+should only contain changes to files within the `tests` directory. If you
+change any files in other parts of the project, your PR will be rejected.
+
+Please follow the steps below to run Neighborly's test suite. Neighborly uses
+[PyTest](https://docs.pytest.org/en/7.1.x/) to handle unit testing.
+
+```bash
+# Step 1: Install dependencies for tests
+python -m pip install -e ".[tests]"
+
+# Step 2: Run Pytest
+pytest
+
+# Step3 : (Optional) Generate a test coverage report
+pytest --cov=neighborly tests/
+```
+
+# Documentation
+
+Neighborly uses [Numpy-style](https://numpydoc.readthedocs.io/en/latest/format.html)
+docstrings in code and full documentation can be found in the
+[Wiki](https://github.com/ShiJbey/neighborly/wiki).
+
+When adding docstrings for existing or new bits of code please use the following
+references for how to format your contributions:
+
+* [Sphinx Napoleon Plugin for processing Numpy Docstrings](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html)
+* [Example Numpy Style Docstrings](https://www.sphinx-doc.org/en/master/usage/extensions/example_numpy.html#example-numpy)
+
+# Contributing
+
+Here are some ways that people can contribute to Neighborly:
+
+1. Proposing/Implementing new features
+2. Fixing bugs
+3. Providing optimizations
+4. Fixing typos
+5. Filing issues
+6. Contributing tutorials/how-tos to the wiki
+7. Fixing grammar and spelling in the wiki
+8. Creating new samples/plugins
+
+If you are interested in contributing to Neighborly, there are multiple ways to get
+involved, and not all of them require you to be proficient with GitHub. Interested
+parties can contribute to the core code base of Neighborly and/or create nre content
+in the way of plugins. I love feedback, and if you have any questions, create a new
+issue, and I will do my best to answer. If you want to contribute to the core code,
+free to fork this repository, make your changes, and submit a pull-request with a
+description of your contribution. Please keep in mind that this project is a
+tool for creativity and learning. I have a [code of conduct](./CODE_OF_CONDUCT.md) to
+encourage healthy collaboration, and will enforce it if I need to.
+
+## Code Style
+
+Neighborly uses [_Black_](https://black.readthedocs.io/en/stable/) to handle code style
+and sorts imports using [_isort_](https://pycqa.github.io/isort/). You can follow
+[these instructions](https://black.readthedocs.io/en/stable/integrations/editors.html)
+for setting up both black and isort.
+
+# Notes
+
+## Non-Deterministic Behavior
+
+The goal of having a seeded pseudo random simulation is so that users experience
+deterministic behavior when using the same starting seed. I try to remove all forms of
+non-determinism, but some slip through. The known areas are listed below. If you find
+any, please make a new issue with details of the behavior.
+
+* Neighborly uses [Tracery](https://github.com/aparrish/pytracery) to generate names for
+characters and locations, and these names may not be consistent despite using the same
+rng seed value.
+
+## DMCA Statement
+
+Upon receipt of a notice alleging copyright infringement, I will take whatever action it
+deems appropriate within its sole discretion, including removal of the allegedly
+infringing materials.
+
+The repo image is something fun that I made. I love _The Simpsons_, and I couldn't think
+of anyone more neighborly than Ned Flanders. If the copyright owner for _The Simpsons_
+would like me to take it down, please contact me. The same takedown policy applies to
+any code samples inspired by TV shows, movies, and games.
```

### Comparing `neighborly-0.9.3/src/neighborly.egg-info/SOURCES.txt` & `neighborly-0.9.4/src/neighborly.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,73 @@
+CHANGELOG.md
 CODE_OF_CONDUCT.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 src/neighborly/__init__.py
 src/neighborly/__main__.py
 src/neighborly/exporter.py
-src/neighborly/inspection_tools.py
 src/neighborly/loaders.py
 src/neighborly/simulation.py
 src/neighborly.egg-info/PKG-INFO
 src/neighborly.egg-info/SOURCES.txt
 src/neighborly.egg-info/dependency_links.txt
+src/neighborly.egg-info/entry_points.txt
 src/neighborly.egg-info/requires.txt
 src/neighborly.egg-info/top_level.txt
 src/neighborly/builtin/__init__.py
+src/neighborly/builtin/ai.py
+src/neighborly/builtin/archetypes.py
+src/neighborly/builtin/components.py
 src/neighborly/builtin/events.py
 src/neighborly/builtin/helpers.py
 src/neighborly/builtin/role_filters.py
-src/neighborly/builtin/statuses.py
 src/neighborly/builtin/systems.py
 src/neighborly/core/__init__.py
-src/neighborly/core/activity.py
+src/neighborly/core/action.py
+src/neighborly/core/ai.py
 src/neighborly/core/archetypes.py
-src/neighborly/core/behavior_tree.py
+src/neighborly/core/building.py
 src/neighborly/core/business.py
 src/neighborly/core/character.py
+src/neighborly/core/constants.py
 src/neighborly/core/ecs.py
 src/neighborly/core/engine.py
+src/neighborly/core/event.py
 src/neighborly/core/life_event.py
 src/neighborly/core/location.py
 src/neighborly/core/name_generation.py
 src/neighborly/core/personal_values.py
 src/neighborly/core/position.py
+src/neighborly/core/query.py
 src/neighborly/core/relationship.py
 src/neighborly/core/residence.py
-src/neighborly/core/rng.py
+src/neighborly/core/role.py
 src/neighborly/core/routine.py
-src/neighborly/core/status.py
+src/neighborly/core/serializable.py
+src/neighborly/core/system.py
 src/neighborly/core/time.py
 src/neighborly/core/town.py
 src/neighborly/core/utils/__init__.py
 src/neighborly/core/utils/graph.py
+src/neighborly/core/utils/grid.py
 src/neighborly/core/utils/utilities.py
-src/neighborly/core/utils/tracery/__init__.py
-src/neighborly/core/utils/tracery/modifiers.py
 src/neighborly/plugins/__init__.py
-src/neighborly/plugins/weather_plugin.py
-src/neighborly/plugins/default_plugin/__init__.py
-src/neighborly/plugins/default_plugin/data/data.yaml
-src/neighborly/plugins/default_plugin/data/names/US_settlement_names.txt
-src/neighborly/plugins/default_plugin/data/names/bar_names.txt
-src/neighborly/plugins/default_plugin/data/names/feminine_names.txt
-src/neighborly/plugins/default_plugin/data/names/masculine_names.txt
-src/neighborly/plugins/default_plugin/data/names/neutral_names.txt
-src/neighborly/plugins/default_plugin/data/names/restaurant_names.txt
-src/neighborly/plugins/default_plugin/data/names/surnames.txt
+src/neighborly/plugins/weather.py
+src/neighborly/plugins/defaults/__init__.py
+src/neighborly/plugins/defaults/data/data.yaml
+src/neighborly/plugins/defaults/data/names/US_settlement_names.txt
+src/neighborly/plugins/defaults/data/names/bar_names.txt
+src/neighborly/plugins/defaults/data/names/feminine_names.txt
+src/neighborly/plugins/defaults/data/names/masculine_names.txt
+src/neighborly/plugins/defaults/data/names/neutral_names.txt
+src/neighborly/plugins/defaults/data/names/restaurant_names.txt
+src/neighborly/plugins/defaults/data/names/surnames.txt
 src/neighborly/plugins/talktown/__init__.py
 src/neighborly/plugins/talktown/business_archetypes.py
-src/neighborly/plugins/talktown/components.py
+src/neighborly/plugins/talktown/business_components.py
 src/neighborly/plugins/talktown/occupation_types.py
 src/neighborly/plugins/talktown/personality.py
 src/neighborly/plugins/talktown/school.py
-src/neighborly/plugins/talktown/utils.py
-src/neighborly/server/__init__.py
+src/neighborly/plugins/talktown/utils.py
```

