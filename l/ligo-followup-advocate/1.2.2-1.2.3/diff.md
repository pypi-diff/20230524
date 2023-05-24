# Comparing `tmp/ligo-followup-advocate-1.2.2.tar.gz` & `tmp/ligo-followup-advocate-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ligo-followup-advocate-1.2.2.tar", last modified: Wed May  3 17:51:18 2023, max compression
+gzip compressed data, was "ligo-followup-advocate-1.2.3.tar", last modified: Wed May 24 17:47:56 2023, max compression
```

## Comparing `ligo-followup-advocate-1.2.2.tar` & `ligo-followup-advocate-1.2.3.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.610091 ligo-followup-advocate-1.2.2/
--rw-rw-rw-   0 root         (0) root         (0)    17895 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/COPYING.md
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      880 2023-05-03 17:51:18.610091 ligo-followup-advocate-1.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2855 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.567091 ligo-followup-advocate-1.2.2/ligo/
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.611091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/
--rw-rw-rw-   0 root         (0) root         (0)    24975 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-05-03 17:51:18.611091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     1244 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/jinja.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.573091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2855 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/RAVEN_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      944 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/RAVEN_subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/authors.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/compare_skymaps.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1032 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/em_bright.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     2596 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/initial_body.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      425 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/initial_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1581 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/llama_alert_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/llama_subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     2303 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/llama_track_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     9941 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/macros.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1786 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1504 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/medium_latency_grb_subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/numbered_pipeline_citations.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      461 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/p_astro.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      419 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/retraction.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1122 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/skymap_info.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1350 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/update_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      223 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/userguide_conclusion.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.573091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.566091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.574091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1122/
--rw-rw-rw-   0 root         (0) root         (0)     1880 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1122/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.574091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1122/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1122/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1122/files/distances_x.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_x.json
--rw-rw-rw-   0 root         (0) root         (0)      987 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1122/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.575091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1133/
--rw-rw-rw-   0 root         (0) root         (0)     1877 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1133/event.json
--rw-rw-rw-   0 root         (0) root         (0)        4 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1133/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.575091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1134/
--rw-rw-rw-   0 root         (0) root         (0)     1904 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1134/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.576091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1134/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1134/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1134/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)      515 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1134/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.576091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/
--rw-rw-rw-   0 root         (0) root         (0)     1881 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.577091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/files/distances_x.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_x.json
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/files/initial.data
--rw-rw-rw-   0 root         (0) root         (0)     1086 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.577091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1235/
--rw-rw-rw-   0 root         (0) root         (0)     1876 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1235/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.578091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1235/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1235/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1235/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1235/files/initial.data
--rw-rw-rw-   0 root         (0) root         (0)      610 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1235/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.578091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E2244/
--rw-rw-rw-   0 root         (0) root         (0)     1904 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E2244/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.579091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E2244/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E2244/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E2244/files/distances_x.json
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_x.json
--rw-rw-rw-   0 root         (0) root         (0)      991 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E2244/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.580091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E5678/
--rw-rw-rw-   0 root         (0) root         (0)     1918 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E5678/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.580091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E5678/files/
--rw-rw-rw-   0 root         (0) root         (0)     5761 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E5678/files/initial.data
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E5678/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.580091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1122/
--rw-rw-rw-   0 root         (0) root         (0)     1936 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1122/event.json
--rw-rw-rw-   0 root         (0) root         (0)      633 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1122/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.581091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1234/
--rw-rw-rw-   0 root         (0) root         (0)     3958 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1234/event.json
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1234/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.581091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1235/
--rw-rw-rw-   0 root         (0) root         (0)     3982 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1235/event.json
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1235/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.581091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2468/
--rw-rw-rw-   0 root         (0) root         (0)     3956 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2468/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.582091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2468/files/
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2468/files/p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2468/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.582091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2469/
--rw-rw-rw-   0 root         (0) root         (0)     3979 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2469/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.582091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2469/files/
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2469/files/p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2469/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.583091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5566/
--rw-rw-rw-   0 root         (0) root         (0)     3958 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5566/event.json
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5566/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.583091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5678/
--rw-rw-rw-   0 root         (0) root         (0)     3955 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5678/event.json
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5678/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.583091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5679/
--rw-rw-rw-   0 root         (0) root         (0)     3979 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5679/event.json
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5679/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.584091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.590091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/
--rw-rw-rw-   0 root         (0) root         (0)     4609 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml
--rw-rw-rw-   0 root         (0) root         (0)     4599 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/S1234-2-Initial.xml
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/coincidence_far.json
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/em_bright.json
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)     1937 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files.json
--rw-rw-rw-   0 root         (0) root         (0)     7997 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/logs.json
--rw-rw-rw-   0 root         (0) root         (0)     5897 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/superevent.json
--rw-rw-rw-   0 root         (0) root         (0)     1612 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/voevents.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.591091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.593091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/files/
--rw-rw-rw-   0 root         (0) root         (0)     4476 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml
--rw-rw-rw-   0 root         (0) root         (0)  1065600 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)     4047 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/files/significance_subthreshold_lvc-i3.json
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/files.json
--rw-rw-rw-   0 root         (0) root         (0)     4911 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/logs.json
--rw-rw-rw-   0 root         (0) root         (0)     3397 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/superevent.json
--rw-rw-rw-   0 root         (0) root         (0)      966 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/voevents.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.594091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.608091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/
--rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0
--rw-rw-rw-   0 root         (0) root         (0)     6731 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml
--rw-rw-rw-   0 root         (0) root         (0)     6716 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/coincidence_far.json
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/em_bright.json
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/em_bright.json,0
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/p_astro.json,0
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files.json
--rw-rw-rw-   0 root         (0) root         (0)     7678 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/logs.json
--rw-rw-rw-   0 root         (0) root         (0)     5616 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/superevent.json
--rw-rw-rw-   0 root         (0) root         (0)     1585 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/voevents.json
--rw-rw-rw-   0 root         (0) root         (0)     5123 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/test_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     2576 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.609091 ligo-followup-advocate-1.2.2/ligo_followup_advocate.egg-info/
--rw-r--r--   0 root         (0) root         (0)      880 2023-05-03 17:51:18.000000 ligo-followup-advocate-1.2.2/ligo_followup_advocate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7102 2023-05-03 17:51:18.000000 ligo-followup-advocate-1.2.2/ligo_followup_advocate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 17:51:18.000000 ligo-followup-advocate-1.2.2/ligo_followup_advocate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2023-05-03 17:51:18.000000 ligo-followup-advocate-1.2.2/ligo_followup_advocate.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-05-03 17:51:18.000000 ligo-followup-advocate-1.2.2/ligo_followup_advocate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-03 17:51:18.000000 ligo-followup-advocate-1.2.2/ligo_followup_advocate.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1793 2023-05-03 17:51:18.611091 ligo-followup-advocate-1.2.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      539 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    68611 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.911851 ligo-followup-advocate-1.2.3/
+-rw-rw-rw-   0 root         (0) root         (0)    17895 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/COPYING.md
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      880 2023-05-24 17:47:56.912850 ligo-followup-advocate-1.2.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2855 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.779846 ligo-followup-advocate-1.2.3/ligo/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.914851 ligo-followup-advocate-1.2.3/ligo/followup_advocate/
+-rw-rw-rw-   0 root         (0) root         (0)    24955 2023-05-23 23:25:10.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-24 17:47:56.914851 ligo-followup-advocate-1.2.3/ligo/followup_advocate/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/jinja.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.788847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2973 2023-05-23 23:25:10.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/RAVEN_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      944 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/RAVEN_subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 17:47:46.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/authors.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/compare_skymaps.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/em_bright.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     2699 2023-05-23 23:25:10.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/initial_body.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      425 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/initial_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/llama_alert_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/llama_subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     2303 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/llama_track_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     9888 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/macros.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1786 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/medium_latency_grb_subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/numbered_pipeline_citations.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      461 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/p_astro.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      419 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/retraction.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1122 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/skymap_info.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1350 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/update_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      223 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/userguide_conclusion.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.788847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 17:47:46.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.777846 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.789847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1122/
+-rw-rw-rw-   0 root         (0) root         (0)     1880 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1122/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.790847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1122/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1122/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1122/files/distances_x.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_x.json
+-rw-rw-rw-   0 root         (0) root         (0)      987 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1122/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.791847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1133/
+-rw-rw-rw-   0 root         (0) root         (0)     1877 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1133/event.json
+-rw-rw-rw-   0 root         (0) root         (0)        4 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1133/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.792847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1134/
+-rw-rw-rw-   0 root         (0) root         (0)     1904 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1134/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.793847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1134/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1134/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1134/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)      515 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1134/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.793847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/
+-rw-rw-rw-   0 root         (0) root         (0)     1881 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.795847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/files/distances_x.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_x.json
+-rw-rw-rw-   0 root         (0) root         (0)      714 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/files/initial.data
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.795847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1235/
+-rw-rw-rw-   0 root         (0) root         (0)     1876 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1235/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.796847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1235/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1235/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1235/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)      714 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1235/files/initial.data
+-rw-rw-rw-   0 root         (0) root         (0)      610 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1235/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.797847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E2244/
+-rw-rw-rw-   0 root         (0) root         (0)     1904 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E2244/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.798847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E2244/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E2244/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E2244/files/distances_x.json
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_x.json
+-rw-rw-rw-   0 root         (0) root         (0)      991 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E2244/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.799847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E5678/
+-rw-rw-rw-   0 root         (0) root         (0)     1918 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E5678/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.799847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E5678/files/
+-rw-rw-rw-   0 root         (0) root         (0)     5761 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E5678/files/initial.data
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E5678/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.800847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1122/
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1122/event.json
+-rw-rw-rw-   0 root         (0) root         (0)      633 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1122/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.801847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1234/
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1234/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1234/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.801847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1235/
+-rw-rw-rw-   0 root         (0) root         (0)     3982 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1235/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1235/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.802847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2468/
+-rw-rw-rw-   0 root         (0) root         (0)     3956 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2468/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.802847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2468/files/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2468/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2468/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.803847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2469/
+-rw-rw-rw-   0 root         (0) root         (0)     3979 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2469/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.803847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2469/files/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2469/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2469/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.805847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5566/
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5566/event.json
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5566/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.805847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5678/
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5678/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5678/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.806847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5679/
+-rw-rw-rw-   0 root         (0) root         (0)     3979 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5679/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5679/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.807847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.831848 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/
+-rw-rw-rw-   0 root         (0) root         (0)     4609 2023-05-23 23:25:10.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml
+-rw-rw-rw-   0 root         (0) root         (0)     4607 2023-05-23 23:25:10.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/S1234-2-Initial.xml
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/coincidence_far.json
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/em_bright.json
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)     1832 2023-05-23 23:25:10.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files.json
+-rw-rw-rw-   0 root         (0) root         (0)     7997 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/logs.json
+-rw-rw-rw-   0 root         (0) root         (0)     5897 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/superevent.json
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/voevents.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.833848 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.840848 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/files/
+-rw-rw-rw-   0 root         (0) root         (0)     4476 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml
+-rw-rw-rw-   0 root         (0) root         (0)  1065600 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)     4047 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/files/significance_subthreshold_lvc-i3.json
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/files.json
+-rw-rw-rw-   0 root         (0) root         (0)     4911 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/logs.json
+-rw-rw-rw-   0 root         (0) root         (0)     3397 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/superevent.json
+-rw-rw-rw-   0 root         (0) root         (0)      966 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/voevents.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.842848 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.908851 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/
+-rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0
+-rw-rw-rw-   0 root         (0) root         (0)     6731 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml
+-rw-rw-rw-   0 root         (0) root         (0)     6716 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/coincidence_far.json
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/em_bright.json
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/em_bright.json,0
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/p_astro.json,0
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files.json
+-rw-rw-rw-   0 root         (0) root         (0)     7678 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/logs.json
+-rw-rw-rw-   0 root         (0) root         (0)     5616 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/superevent.json
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/voevents.json
+-rw-rw-rw-   0 root         (0) root         (0)     5123 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/test_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2576 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.911851 ligo-followup-advocate-1.2.3/ligo_followup_advocate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      880 2023-05-24 17:47:56.000000 ligo-followup-advocate-1.2.3/ligo_followup_advocate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7102 2023-05-24 17:47:56.000000 ligo-followup-advocate-1.2.3/ligo_followup_advocate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 17:47:56.000000 ligo-followup-advocate-1.2.3/ligo_followup_advocate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2023-05-24 17:47:56.000000 ligo-followup-advocate-1.2.3/ligo_followup_advocate.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-05-24 17:47:56.000000 ligo-followup-advocate-1.2.3/ligo_followup_advocate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-24 17:47:56.000000 ligo-followup-advocate-1.2.3/ligo_followup_advocate.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2023-05-24 17:47:56.914851 ligo-followup-advocate-1.2.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      539 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    68611 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/versioneer.py
```

### Comparing `ligo-followup-advocate-1.2.2/COPYING.md` & `ligo-followup-advocate-1.2.3/COPYING.md`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/PKG-INFO` & `ligo-followup-advocate-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ligo-followup-advocate
-Version: 1.2.2
+Version: 1.2.3
 Summary: LIGO/Virgo/KAGRA Follow-up Advocate Tools
 Home-page: https://git.ligo.org/emfollow/ligo-followup-advocate
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
 Maintainer: Brandon Piotrzkowski
 Maintainer-email: brandon.piotrzkowski@ligo.org
 License: GPL-2+
```

### Comparing `ligo-followup-advocate-1.2.2/README.md` & `ligo-followup-advocate-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/__init__.py` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,21 +120,21 @@
             early_warning_alert = True
         url = root.find('./What/Group/Param[@name="skymap_fits"]')
         if url is None:
             continue
         url = url.attrib['value']
         _, filename = os.path.split(url)
         skyloc_pipeline = guess_skyloc_pipeline(filename)
-        issued_time = astropy.time.Time(root.find('./Who/Date').text).datetime
+        issued_time = astropy.time.Time(root.find('./Who/Date').text).gps
         if filename not in skymaps:
             skymaps[filename] = dict(
                 alert_type=alert_type,
                 pipeline=skyloc_pipeline,
                 filename=filename,
-                latency=issued_time-event_time.datetime)
+                latency=issued_time-event_time.gps)
             if skyloc_pipeline.lower() not in citation_index:
                 citation_index[skyloc_pipeline.lower()] = \
                     max(citation_index.values()) + 1
     skymaps = list(skymaps.values())
 
     o = urllib.parse.urlparse(client.service_url)
 
@@ -630,20 +630,20 @@
                     event['labels'])
             url = root.find('./What/Group/Param[@name="joint_skymap_fits"]')
             if url is None:
                 continue
             url = url.attrib['value']
             _, filename = os.path.split(url)
             issued_time = astropy.time.Time(
-                              root.find('./Who/Date').text).datetime
+                              root.find('./Who/Date').text).gps
             if filename not in combined_skymaps:
                 combined_skymaps[filename] = dict(
                     alert_type=alert_type,
                     filename=filename,
-                    latency=issued_time-event_time.datetime)
+                    latency=issued_time-event_time.gps)
 
         if combined_skymaps:
             combined_skymaps = list(combined_skymaps.values())
             combined_skymap = combined_skymaps[-1]['filename']
             cl = 90
             include_ellipse, ra, dec, a, b, pa, area, greedy_area = \
                 uncertainty_ellipse(gracedb_id, combined_skymap, client, cl=cl)
```

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/jinja.py` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/jinja.py`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/RAVEN_circular.jinja2` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/RAVEN_circular.jinja2`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 A search performed by the RAVEN pipeline found a temporal coincidence between
 {{gracedb_id}} and a {% if snews %}SNEWS supernova{% elif grb %}{% if subthreshold %}sub-threshold {% endif %}{{grbmission(external_pipeline)}}{% endif %} {{propername(external_trigger)}} **CITE ORIGINAL GCN FOR THE EXTERNAL TRIGGER FROM https://gcn.gsfc.nasa.gov/gcn3_archive.html, e.g., (Bhalerao et al., GCN Circular XXXXX)**.
 The {% if snews %}neutrino{% elif grb %}GRB{% endif %} trigger time is {{latency}} seconds {{beforeafter}} the GW candidate event.
 {% if grb %}
 The estimated joint false alarm rate for the coincidence using just timing info is {{naturalfar(time_coinc_far)}}.
 {% if subthreshold_targeted %}The GRB candidate was found during a joint targeted search between the LIGO/Virgo/KAGRA collaboration and {{grbmission_targeted(external_pipeline)}}, and has a false alarm rate of {{naturalfar(far_grb)}}. {% endif %}
 {% if other_ext_pipelines %}RAVEN has also identified {% if other_ext_pipelines|length == 1 %}an additional detection{% elif other_ext_pipelines|length > 1%}additional detections{% endif %} from {{naturalotherexternalpipelines(other_ext_pipelines)}}.{% endif %}
-
 {% endif %}
+
 {% if combined_skymap %}
 {% if combined_skymaps|length == 1 %}A combined sky map is{% else %}Combined sky maps are{% endif %} also available:
 {% for skymap in combined_skymaps %}
- * {{skymap.filename}}, an {% if skymap.alert_type in ['preliminary','initial'] %}initial{% else %}updated{% endif %} localization, distributed via GCN notice about {{skymap.latency|naturaldelta}} after the candidate event time.
+ * {{skymap.filename}}, an {% if skymap.alert_type in ['preliminary','initial'] %}initial{% elif skymap.alert_type == 'earlywarning' %}early warning{% else %}updated{% endif %} localization, distributed via GCN notice about {{skymap.latency|abs|naturaldelta}} {% if skymap.latency < 0 %}before {% else %}after {% endif %}the candidate event time.
 {% endfor %}
 
 For the {{combined_skymap}} sky map, the {{cl}}% credible region is {{combined_skymap_greedy_area|round|int}} deg2.
 {% endif %}
 {% if external_pipeline|lower == 'swift'%}
 The joint localization is dominated by the {{grbmission(external_pipeline)}} candidate, which was identified with right ascension, declination of {{'%0.3f' % ext_ra|float}}, {{'%0.3f' % ext_dec|float}}{% if ext_error %} and 90% containment error radius of {{'%0.3f' % ext_error|float}} deg{% endif %}.
 {% endif %}
```

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/RAVEN_subject.jinja2` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/RAVEN_subject.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/authors.jinja2` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/authors.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/em_bright.jinja2` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/em_bright.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/initial_body.jinja2` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/initial_body.jinja2`

 * *Files 5% similar despite different names*

```diff
@@ -30,13 +30,13 @@
 {% if prob_has_ns is not none %}
 {%- include 'em_bright.jinja2' -%}
 {% endif %}
 {% if skymaps|length == 0 %}
 No{% else %}{{ skymaps|length|apnumber|capitalize }}{% endif %} {% if combined_skymap is not defined %}sky map{% else %}GW-only sky map{% endif %}{% if skymaps|length == 1 %} is{% else %}s are{% endif %} available at this time{% if skymaps|length > 0 %} and can be retrieved from the GraceDB event page:{% else %}.{% endif %}
 
 {% for skymap in skymaps %}
- * {{skymap.filename}}, an {% if skymap.alert_type in ['earlywarning','preliminary','initial'] %}initial{% else %}updated{% endif %} localization generated by {{citeskymap(skymap.pipeline, citation_index)}}, distributed via GCN notice about {{skymap.latency|naturaldelta}} after the candidate event time.
+ * {{skymap.filename}}, an {% if skymap.alert_type in ['preliminary','initial'] %}initial{% elif skymap.alert_type == 'earlywarning' %}early warning{% else %}updated{% endif %} localization generated by {{citeskymap(skymap.pipeline, citation_index)}}, distributed via GCN notice about {{skymap.latency|abs|naturaldelta}} {% if skymap.latency < 0 %}before {% else %}after {% endif %}the candidate event time.
 {% endfor %}
 
 {% if skymaps|length != 0 %}{%- include 'skymap_info.jinja2' -%}{% endif %}
 {% endif %}
 {% endfilter %}
```

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/llama_alert_circular.jinja2` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/llama_alert_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/llama_track_circular.jinja2` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/llama_track_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/macros.jinja2` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/macros.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -244,23 +244,23 @@
 {%- endmacro -%}
 
 
 Dictionary of common citations.
 
 {% set citations = {'pycbc': 'Dal Canton et al. ApJ 923, 254 (2021)',
                     'mbta': 'Aubin et al. CQG 38, 095004 (2021)',
-                    'gstlal': 'Tsukada et al. LIGO-DCC P2300116 (2023) and Ewing et al. LIGO-DCC P2300124 (2023)',
-                    'spiir': 'Qi Chu, PhD Thesis, The University of Western Australia (2017)',
+                    'gstlal': 'Tsukada et al. arXiv:2305.06286 (2023) and Ewing et al. arXiv:2305.05625 (2023)',
+                    'spiir': 'Chu et al. PRD 105, 024023 (2022)',
                     'pycbc_earlywarning': 'Nitz A. H., Schäfer M., Dal Canton T. ApJL 902, 2 (2020)',
                     'gstlal_earlywarning': 'Sachdev et al. ApJL 905, 2 (2020)',
                     'spiir_earlywarning': 'Kovalam et al. ApJL 927, 1 (2022)',
                     'cwb': 'Klimenko et al. PRD 93, 042004 (2016)',
                     'olib': 'Lynch et al. PRD 95, 104046 (2017)',
                     'mly': 'Skliris et al. arXiv:2009.14611 (2020)',
-                    'em_bright': 'Chatterjee et al. The Astrophysical Journal 896, 1 (2020)',
+                    'em_bright': 'Chatterjee et al. ApJ 896, 1 (2020)',
                     'pygrb': 'Williamson et al. PRD 90, 122004 (2014)',
                     'xpipeline': 'Was et al. PRD 86, 022003 (2012)',
                     'llama': 'Baret et al., Astroparticle Physics 35, 1 (2011)',
                     'llama_stat': 'Bartos et al. arXiv:1810.11467 (2018) and Countryman et al.\n arXiv:1901.05486 (2019)',
                     'bayestar': 'Singer & Price PRD 93, 024013 (2016)',
                     'bilby': 'Ashton et al. ApJS 241, 27 (2019)',
                     'lalinference': 'Veitch et al. PRD 91, 042003 (2015)',
```

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/skymap_info.jinja2` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/skymap_info.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/update_circular.jinja2` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/update_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1122/event.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1122/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1122/files.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1122/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1133/event.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1133/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1134/event.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1134/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1134/files.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1134/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/event.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/files/initial.data` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/files/initial.data`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/files.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1235/event.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1235/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1235/files/initial.data` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1235/files/initial.data`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1235/files.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1235/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E2244/event.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E2244/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E2244/files.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E2244/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E5678/event.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E5678/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E5678/files/initial.data` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E5678/files/initial.data`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1122/event.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1122/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1122/files.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1122/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1234/event.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1234/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1234/files.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1234/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1235/event.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1235/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1235/files.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1235/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2468/event.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2468/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2468/files.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2468/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2469/event.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2469/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2469/files.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2469/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5566/event.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5566/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5566/files.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5566/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5678/event.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5678/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5678/files.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5678/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5679/event.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5679/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5679/files.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5679/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml`

 * *Files 2% similar despite different names*

#### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <voe:VOEvent xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:voe="http://www.ivoa.net/xml/VOEvent/v2.0" xsi:schemaLocation="http://www.ivoa.net/xml/VOEvent/v2.0 http://www.ivoa.net/xml/VOEvent/VOEvent-v2.0.xsd" version="2.0" role="test" ivorn="ivo://gwnet/gcn_sender#S1234-1-EarlyWarning">
   <Who>
-    <Date>2018-06-28T13:36:02</Date>
+    <Date>2018-06-28T03:07:02</Date>
     <Author>
       <contactName>LIGO Scientific Collaboration and Virgo Collaboration</contactName>
     </Author>
   </Who>
   <What>
     <Param name="internal" dataType="int" value="1">
       <Description>Indicates whether this event should be distributed to LSC/Virgo members only</Description>
@@ -60,15 +60,15 @@
     <ObsDataLocation>
       <ObservatoryLocation id="LIGO Virgo"/>
       <ObservationLocation>
         <AstroCoordSystem id="UTC-FK5-GEO"/>
         <AstroCoords coord_system_id="UTC-FK5-GEO">
           <Time>
             <TimeInstant>
-              <ISOTime>2018-06-28T13:35:16.911085</ISOTime>
+              <ISOTime>2018-06-28T03:08:04.911085</ISOTime>
             </TimeInstant>
           </Time>
         </AstroCoords>
       </ObservationLocation>
     </ObsDataLocation>
   </WhereWhen>
   <How>
```

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/S1234-2-Initial.xml` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/S1234-2-Initial.xml`

 * *Files 2% similar despite different names*

#### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/S1234-2-Initial.xml` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/S1234-2-Initial.xml`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <voe:VOEvent xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:voe="http://www.ivoa.net/xml/VOEvent/v2.0" xsi:schemaLocation="http://www.ivoa.net/xml/VOEvent/v2.0 http://www.ivoa.net/xml/VOEvent/VOEvent-v2.0.xsd" version="2.0" role="test" ivorn="ivo://gwnet/gcn_sender#S1234-2-Initial">
   <Who>
-    <Date>2018-06-28T13:42:02</Date>
+    <Date>2018-06-28T03:20:02</Date>
     <Author>
       <contactName>LIGO Scientific Collaboration and Virgo Collaboration</contactName>
     </Author>
   </Who>
   <What>
     <Param name="internal" dataType="int" value="1">
       <Description>Indicates whether this event should be distributed to LSC/Virgo members only</Description>
@@ -47,28 +47,28 @@
     <Param name="Search" dataType="string" value="MDC" ucd="meta.code" unit="">
       <Description>Specific low-latency search</Description>
     </Param>
     <Param dataType="int" name="Significant" ucd="meta.number" value="1">
       <Description>Indicates that this event is a significant alert if 1, no if 0</Description>
     </Param>
     <Group type="GW_SKYMAP" name="BAYESTAR">
-      <Param name="skymap_fits" dataType="string" value="https://gracedb-playground.ligo.org/apibasic/superevents/S1234/files/bayestar.fits.gz" ucd="meta.ref.url" unit="">
+      <Param name="skymap_fits" dataType="string" value="https://gracedb-playground.ligo.org/apibasic/superevents/S1234/files/bayestar.multiorder.fits" ucd="meta.ref.url" unit="">
         <Description>Sky Map FITS</Description>
       </Param>
     </Group>
   </What>
   <WhereWhen>
     <ObsDataLocation>
       <ObservatoryLocation id="LIGO Virgo"/>
       <ObservationLocation>
         <AstroCoordSystem id="UTC-FK5-GEO"/>
         <AstroCoords coord_system_id="UTC-FK5-GEO">
           <Time>
             <TimeInstant>
-              <ISOTime>2018-06-28T13:35:16.911085</ISOTime>
+              <ISOTime>2018-06-28T03:08:04.911085</ISOTime>
             </TimeInstant>
           </Time>
         </AstroCoords>
       </ObservationLocation>
     </ObsDataLocation>
   </WhereWhen>
   <How>
```

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9473684210526315%*

 * *Differences: {"'bayestar.fits.gz,0'": "'https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar.fits.gz'",*

 * * "'bayestar.multiorder.fits,0'": "'https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar.multiorder.fits'"}*

```diff
@@ -1,16 +1,16 @@
 {
     "S1234-1-EarlyWarning.xml": "https://gracedb-dev1.ligo.org/api/events/S1234/files/S1234-1-EarlyWarning.xml",
     "S1234-2-Initial.xml": "https://gracedb-dev1.ligo.org/api/events/S1234/files/S1234-2-Initial.xml",
     "S1234-3-Update.xml": "https://gracedb-dev1.ligo.org/api/events/S1234/files/S1234-3-Update.xml",
     "bayestar-ext.fits.gz": "https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar-ext.fits.gz",
     "bayestar.fits.gz": "https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar.fits.gz",
-    "bayestar.fits.gz,0": "https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar.fits.gz,0",
+    "bayestar.fits.gz,0": "https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar.fits.gz",
     "bayestar.multiorder.fits": "https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar.multiorder.fits",
-    "bayestar.multiorder.fits,0": "https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar.multiorder.fits,0",
+    "bayestar.multiorder.fits,0": "https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar.multiorder.fits",
     "coinc.xml": "https://gracedb-dev1.ligo.org/api/events/S1234/files/coinc.xml",
     "coinc.xml,0": "https://gracedb-dev1.ligo.org/api/events/S1234/files/coinc.xml,0",
     "coincidence_far.json": "https://gracedb-dev1.ligo.org/api/events/S1234/files/coincidence_far.json",
     "em_bright.json": "https://gracedb-dev1.ligo.org/api/events/S1234/files/em_bright.json",
     "event.log": "https://gracedb-dev1.ligo.org/api/events/S1234/files/event.log",
     "event.log,0": "https://gracedb-dev1.ligo.org/api/events/S1234/files/event.log,0",
     "initial.data": "https://gracedb-dev1.ligo.org/api/events/S1234/files/initial.data",
```

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/logs.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/logs.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/superevent.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/superevent.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/voevents.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/voevents.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/files/significance_subthreshold_lvc-i3.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/files/significance_subthreshold_lvc-i3.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/files.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/logs.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/logs.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/superevent.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/superevent.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/voevents.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/voevents.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/logs.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/logs.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/superevent.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/superevent.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/voevents.json` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/voevents.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/test_tool.py` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/test_tool.py`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo/followup_advocate/tool.py` & `ligo-followup-advocate-1.2.3/ligo/followup_advocate/tool.py`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/ligo_followup_advocate.egg-info/PKG-INFO` & `ligo-followup-advocate-1.2.3/ligo_followup_advocate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ligo-followup-advocate
-Version: 1.2.2
+Version: 1.2.3
 Summary: LIGO/Virgo/KAGRA Follow-up Advocate Tools
 Home-page: https://git.ligo.org/emfollow/ligo-followup-advocate
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
 Maintainer: Brandon Piotrzkowski
 Maintainer-email: brandon.piotrzkowski@ligo.org
 License: GPL-2+
```

### Comparing `ligo-followup-advocate-1.2.2/ligo_followup_advocate.egg-info/SOURCES.txt` & `ligo-followup-advocate-1.2.3/ligo_followup_advocate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/setup.cfg` & `ligo-followup-advocate-1.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/setup.py` & `ligo-followup-advocate-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.2/versioneer.py` & `ligo-followup-advocate-1.2.3/versioneer.py`

 * *Files identical despite different names*

