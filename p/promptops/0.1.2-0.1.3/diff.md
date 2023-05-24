# Comparing `tmp/promptops-0.1.2.tar.gz` & `tmp/promptops-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptops-0.1.2.tar", last modified: Wed May 24 14:28:54 2023, max compression
+gzip compressed data, was "promptops-0.1.3.tar", last modified: Wed May 24 14:43:53 2023, max compression
```

## Comparing `promptops-0.1.2.tar` & `promptops-0.1.3.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:28:54.540195 promptops-0.1.2/
--rw-r--r--   0 vasily     (501) staff       (20)      595 2023-05-24 14:28:54.539786 promptops-0.1.2/PKG-INFO
--rw-r--r--   0 vasily     (501) staff       (20)     1198 2023-05-24 13:48:37.000000 promptops-0.1.2/README.md
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:28:54.514498 promptops-0.1.2/local_runner/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.2/local_runner/__init__.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:28:54.516293 promptops-0.1.2/local_runner/comms/
--rw-r--r--   0 vasily     (501) staff       (20)      133 2023-05-24 13:48:37.000000 promptops-0.1.2/local_runner/comms/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      432 2023-05-24 13:48:37.000000 promptops-0.1.2/local_runner/comms/base.py
--rw-r--r--   0 vasily     (501) staff       (20)     2890 2023-05-24 13:48:37.000000 promptops-0.1.2/local_runner/comms/dtos.py
--rw-r--r--   0 vasily     (501) staff       (20)     1536 2023-05-24 13:48:37.000000 promptops-0.1.2/local_runner/comms/http_reporter.py
--rw-r--r--   0 vasily     (501) staff       (20)     1368 2023-05-24 13:48:37.000000 promptops-0.1.2/local_runner/comms/ws.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:28:54.516790 promptops-0.1.2/local_runner/config/
--rw-r--r--   0 vasily     (501) staff       (20)       48 2023-05-24 13:48:37.000000 promptops-0.1.2/local_runner/config/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     1720 2023-05-24 13:48:37.000000 promptops-0.1.2/local_runner/config/config.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:28:54.517340 promptops-0.1.2/local_runner/creds/
--rw-r--r--   0 vasily     (501) staff       (20)       77 2023-05-24 13:48:37.000000 promptops-0.1.2/local_runner/creds/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     1458 2023-05-24 13:48:37.000000 promptops-0.1.2/local_runner/creds/creds.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:28:54.517957 promptops-0.1.2/local_runner/exec/
--rw-r--r--   0 vasily     (501) staff       (20)       54 2023-05-24 13:48:37.000000 promptops-0.1.2/local_runner/exec/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2317 2023-05-24 13:48:37.000000 promptops-0.1.2/local_runner/exec/manager.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:28:54.518662 promptops-0.1.2/local_runner/handler/
--rw-r--r--   0 vasily     (501) staff       (20)       29 2023-05-24 13:48:37.000000 promptops-0.1.2/local_runner/handler/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      471 2023-05-24 13:48:37.000000 promptops-0.1.2/local_runner/handler/censor.py
--rw-r--r--   0 vasily     (501) staff       (20)     3115 2023-05-24 13:48:37.000000 promptops-0.1.2/local_runner/handler/handler.py
--rw-r--r--   0 vasily     (501) staff       (20)     1233 2023-05-24 13:48:37.000000 promptops-0.1.2/local_runner/main.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:28:54.519306 promptops-0.1.2/local_runner/registration/
--rw-r--r--   0 vasily     (501) staff       (20)       56 2023-05-24 13:48:37.000000 promptops-0.1.2/local_runner/registration/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2523 2023-05-24 13:48:37.000000 promptops-0.1.2/local_runner/registration/registration.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:28:54.519806 promptops-0.1.2/local_runner/tokens/
--rw-r--r--   0 vasily     (501) staff       (20)       27 2023-05-24 13:48:37.000000 promptops-0.1.2/local_runner/tokens/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2235 2023-05-24 13:48:37.000000 promptops-0.1.2/local_runner/tokens/issuer.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:28:54.527286 promptops-0.1.2/promptops/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      942 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/cancellable.py
--rw-r--r--   0 vasily     (501) staff       (20)     1850 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/corrections.py
--rw-r--r--   0 vasily     (501) staff       (20)      394 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/feedback.py
--rw-r--r--   0 vasily     (501) staff       (20)     3609 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/history.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:28:54.531898 promptops-0.1.2/promptops/loading/
--rw-r--r--   0 vasily     (501) staff       (20)      131 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/loading/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      677 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/loading/base.py
--rw-r--r--   0 vasily     (501) staff       (20)      481 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/loading/context.py
--rw-r--r--   0 vasily     (501) staff       (20)     1279 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/loading/pong.py
--rw-r--r--   0 vasily     (501) staff       (20)     1344 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/loading/progress.py
--rw-r--r--   0 vasily     (501) staff       (20)     1077 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/loading/promptops.py
--rw-r--r--   0 vasily     (501) staff       (20)     1025 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/loading/simple.py
--rw-r--r--   0 vasily     (501) staff       (20)     6279 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/main.py
--rw-r--r--   0 vasily     (501) staff       (20)       28 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/nux.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:28:54.533773 promptops-0.1.2/promptops/query/
--rw-r--r--   0 vasily     (501) staff       (20)       30 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/query/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      434 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/query/dtos.py
--rw-r--r--   0 vasily     (501) staff       (20)     3908 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/query/explanation.py
--rw-r--r--   0 vasily     (501) staff       (20)     1222 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/query/messages.py
--rw-r--r--   0 vasily     (501) staff       (20)    16290 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/query/query.py
--rw-r--r--   0 vasily     (501) staff       (20)     1126 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/query.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:28:54.534403 promptops-0.1.2/promptops/recipes/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/recipes/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     6435 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/recipes/creation.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:28:54.535178 promptops-0.1.2/promptops/scrub_secrets/
--rw-r--r--   0 vasily     (501) staff       (20)       55 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/scrub_secrets/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/scrub_secrets/scrub.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:28:54.535936 promptops-0.1.2/promptops/secrets/
--rw-r--r--   0 vasily     (501) staff       (20)       55 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/secrets/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/secrets/scrub.py
--rw-r--r--   0 vasily     (501) staff       (20)      326 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/settings.py
--rw-r--r--   0 vasily     (501) staff       (20)     2292 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/settings_store.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:28:54.538256 promptops-0.1.2/promptops/shells/
--rw-r--r--   0 vasily     (501) staff       (20)       30 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/shells/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     3332 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/shells/base.py
--rw-r--r--   0 vasily     (501) staff       (20)     1245 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/shells/bash.py
--rw-r--r--   0 vasily     (501) staff       (20)     1097 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/shells/common.py
--rw-r--r--   0 vasily     (501) staff       (20)     1635 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/shells/fish.py
--rw-r--r--   0 vasily     (501) staff       (20)     1789 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/shells/zsh.py
--rw-r--r--   0 vasily     (501) staff       (20)     2543 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/similarity.py
--rw-r--r--   0 vasily     (501) staff       (20)       42 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/trace.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:28:54.539277 promptops-0.1.2/promptops/ui/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/ui/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     3070 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/ui/prompts.py
--rw-r--r--   0 vasily     (501) staff       (20)     7026 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/ui/selections.py
--rw-r--r--   0 vasily     (501) staff       (20)     1099 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/ui.py
--rw-r--r--   0 vasily     (501) staff       (20)     3990 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/user.py
--rw-r--r--   0 vasily     (501) staff       (20)       22 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/version.py
--rw-r--r--   0 vasily     (501) staff       (20)     1632 2023-05-24 13:48:37.000000 promptops-0.1.2/promptops/version_check.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:28:54.529417 promptops-0.1.2/promptops.egg-info/
--rw-r--r--   0 vasily     (501) staff       (20)      595 2023-05-24 14:28:54.000000 promptops-0.1.2/promptops.egg-info/PKG-INFO
--rw-r--r--   0 vasily     (501) staff       (20)     1940 2023-05-24 14:28:54.000000 promptops-0.1.2/promptops.egg-info/SOURCES.txt
--rw-r--r--   0 vasily     (501) staff       (20)        1 2023-05-24 14:28:54.000000 promptops-0.1.2/promptops.egg-info/dependency_links.txt
--rw-r--r--   0 vasily     (501) staff       (20)      120 2023-05-24 14:28:54.000000 promptops-0.1.2/promptops.egg-info/entry_points.txt
--rw-r--r--   0 vasily     (501) staff       (20)      209 2023-05-24 14:28:54.000000 promptops-0.1.2/promptops.egg-info/requires.txt
--rw-r--r--   0 vasily     (501) staff       (20)       23 2023-05-24 14:28:54.000000 promptops-0.1.2/promptops.egg-info/top_level.txt
--rw-r--r--   0 vasily     (501) staff       (20)       87 2023-05-24 14:19:51.000000 promptops-0.1.2/pyproject.toml
--rw-r--r--   0 vasily     (501) staff       (20)       38 2023-05-24 14:28:54.540336 promptops-0.1.2/setup.cfg
--rw-r--r--   0 vasily     (501) staff       (20)     1894 2023-05-24 14:28:11.000000 promptops-0.1.2/setup.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:43:53.797190 promptops-0.1.3/
+-rw-r--r--   0 vasily     (501) staff       (20)     1809 2023-05-24 14:43:53.796769 promptops-0.1.3/PKG-INFO
+-rw-r--r--   0 vasily     (501) staff       (20)     1198 2023-05-24 13:48:37.000000 promptops-0.1.3/README.md
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:43:53.770280 promptops-0.1.3/local_runner/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.3/local_runner/__init__.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:43:53.772107 promptops-0.1.3/local_runner/comms/
+-rw-r--r--   0 vasily     (501) staff       (20)      133 2023-05-24 13:48:37.000000 promptops-0.1.3/local_runner/comms/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      432 2023-05-24 13:48:37.000000 promptops-0.1.3/local_runner/comms/base.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2890 2023-05-24 13:48:37.000000 promptops-0.1.3/local_runner/comms/dtos.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1536 2023-05-24 13:48:37.000000 promptops-0.1.3/local_runner/comms/http_reporter.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1368 2023-05-24 13:48:37.000000 promptops-0.1.3/local_runner/comms/ws.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:43:53.772782 promptops-0.1.3/local_runner/config/
+-rw-r--r--   0 vasily     (501) staff       (20)       48 2023-05-24 13:48:37.000000 promptops-0.1.3/local_runner/config/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1720 2023-05-24 13:48:37.000000 promptops-0.1.3/local_runner/config/config.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:43:53.773273 promptops-0.1.3/local_runner/creds/
+-rw-r--r--   0 vasily     (501) staff       (20)       77 2023-05-24 13:48:37.000000 promptops-0.1.3/local_runner/creds/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1458 2023-05-24 13:48:37.000000 promptops-0.1.3/local_runner/creds/creds.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:43:53.774066 promptops-0.1.3/local_runner/exec/
+-rw-r--r--   0 vasily     (501) staff       (20)       54 2023-05-24 13:48:37.000000 promptops-0.1.3/local_runner/exec/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2317 2023-05-24 13:48:37.000000 promptops-0.1.3/local_runner/exec/manager.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:43:53.775042 promptops-0.1.3/local_runner/handler/
+-rw-r--r--   0 vasily     (501) staff       (20)       29 2023-05-24 13:48:37.000000 promptops-0.1.3/local_runner/handler/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      471 2023-05-24 13:48:37.000000 promptops-0.1.3/local_runner/handler/censor.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3115 2023-05-24 13:48:37.000000 promptops-0.1.3/local_runner/handler/handler.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1233 2023-05-24 13:48:37.000000 promptops-0.1.3/local_runner/main.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:43:53.775710 promptops-0.1.3/local_runner/registration/
+-rw-r--r--   0 vasily     (501) staff       (20)       56 2023-05-24 13:48:37.000000 promptops-0.1.3/local_runner/registration/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2523 2023-05-24 13:48:37.000000 promptops-0.1.3/local_runner/registration/registration.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:43:53.776585 promptops-0.1.3/local_runner/tokens/
+-rw-r--r--   0 vasily     (501) staff       (20)       27 2023-05-24 13:48:37.000000 promptops-0.1.3/local_runner/tokens/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2235 2023-05-24 13:48:37.000000 promptops-0.1.3/local_runner/tokens/issuer.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:43:53.782384 promptops-0.1.3/promptops/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      942 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/cancellable.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1850 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/corrections.py
+-rw-r--r--   0 vasily     (501) staff       (20)      394 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/feedback.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3609 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/history.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:43:53.787987 promptops-0.1.3/promptops/loading/
+-rw-r--r--   0 vasily     (501) staff       (20)      131 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/loading/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      677 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/loading/base.py
+-rw-r--r--   0 vasily     (501) staff       (20)      481 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/loading/context.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1279 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/loading/pong.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1344 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/loading/progress.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1077 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/loading/promptops.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1025 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/loading/simple.py
+-rw-r--r--   0 vasily     (501) staff       (20)     6279 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/main.py
+-rw-r--r--   0 vasily     (501) staff       (20)       28 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/nux.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:43:53.789994 promptops-0.1.3/promptops/query/
+-rw-r--r--   0 vasily     (501) staff       (20)       30 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/query/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      434 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/query/dtos.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3908 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/query/explanation.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1222 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/query/messages.py
+-rw-r--r--   0 vasily     (501) staff       (20)    16290 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/query/query.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1126 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/query.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:43:53.790685 promptops-0.1.3/promptops/recipes/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/recipes/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     6435 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/recipes/creation.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:43:53.791460 promptops-0.1.3/promptops/scrub_secrets/
+-rw-r--r--   0 vasily     (501) staff       (20)       55 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/scrub_secrets/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/scrub_secrets/scrub.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:43:53.792222 promptops-0.1.3/promptops/secrets/
+-rw-r--r--   0 vasily     (501) staff       (20)       55 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/secrets/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/secrets/scrub.py
+-rw-r--r--   0 vasily     (501) staff       (20)      326 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/settings.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2292 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/settings_store.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:43:53.795018 promptops-0.1.3/promptops/shells/
+-rw-r--r--   0 vasily     (501) staff       (20)       30 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/shells/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3332 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/shells/base.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1245 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/shells/bash.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1097 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/shells/common.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1635 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/shells/fish.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1789 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/shells/zsh.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2543 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/similarity.py
+-rw-r--r--   0 vasily     (501) staff       (20)       42 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/trace.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:43:53.796214 promptops-0.1.3/promptops/ui/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/ui/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3070 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/ui/prompts.py
+-rw-r--r--   0 vasily     (501) staff       (20)     7026 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/ui/selections.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1099 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/ui.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3990 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/user.py
+-rw-r--r--   0 vasily     (501) staff       (20)       22 2023-05-24 14:43:20.000000 promptops-0.1.3/promptops/version.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1632 2023-05-24 13:48:37.000000 promptops-0.1.3/promptops/version_check.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 14:43:53.785013 promptops-0.1.3/promptops.egg-info/
+-rw-r--r--   0 vasily     (501) staff       (20)     1809 2023-05-24 14:43:53.000000 promptops-0.1.3/promptops.egg-info/PKG-INFO
+-rw-r--r--   0 vasily     (501) staff       (20)     1940 2023-05-24 14:43:53.000000 promptops-0.1.3/promptops.egg-info/SOURCES.txt
+-rw-r--r--   0 vasily     (501) staff       (20)        1 2023-05-24 14:43:53.000000 promptops-0.1.3/promptops.egg-info/dependency_links.txt
+-rw-r--r--   0 vasily     (501) staff       (20)      120 2023-05-24 14:43:53.000000 promptops-0.1.3/promptops.egg-info/entry_points.txt
+-rw-r--r--   0 vasily     (501) staff       (20)      209 2023-05-24 14:43:53.000000 promptops-0.1.3/promptops.egg-info/requires.txt
+-rw-r--r--   0 vasily     (501) staff       (20)       23 2023-05-24 14:43:53.000000 promptops-0.1.3/promptops.egg-info/top_level.txt
+-rw-r--r--   0 vasily     (501) staff       (20)       87 2023-05-24 14:19:51.000000 promptops-0.1.3/pyproject.toml
+-rw-r--r--   0 vasily     (501) staff       (20)       38 2023-05-24 14:43:53.797369 promptops-0.1.3/setup.cfg
+-rw-r--r--   0 vasily     (501) staff       (20)     1967 2023-05-24 14:41:57.000000 promptops-0.1.3/setup.py
```

### Comparing `promptops-0.1.2/README.md` & `promptops-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/local_runner/comms/dtos.py` & `promptops-0.1.3/local_runner/comms/dtos.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/local_runner/comms/http_reporter.py` & `promptops-0.1.3/local_runner/comms/http_reporter.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/local_runner/comms/ws.py` & `promptops-0.1.3/local_runner/comms/ws.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/local_runner/config/config.py` & `promptops-0.1.3/local_runner/config/config.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/local_runner/creds/creds.py` & `promptops-0.1.3/local_runner/creds/creds.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/local_runner/exec/manager.py` & `promptops-0.1.3/local_runner/exec/manager.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/local_runner/handler/handler.py` & `promptops-0.1.3/local_runner/handler/handler.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/local_runner/main.py` & `promptops-0.1.3/local_runner/main.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/local_runner/registration/registration.py` & `promptops-0.1.3/local_runner/registration/registration.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/local_runner/tokens/issuer.py` & `promptops-0.1.3/local_runner/tokens/issuer.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/cancellable.py` & `promptops-0.1.3/promptops/cancellable.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/corrections.py` & `promptops-0.1.3/promptops/corrections.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/history.py` & `promptops-0.1.3/promptops/history.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/loading/base.py` & `promptops-0.1.3/promptops/loading/base.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/loading/pong.py` & `promptops-0.1.3/promptops/loading/pong.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/loading/progress.py` & `promptops-0.1.3/promptops/loading/progress.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/loading/promptops.py` & `promptops-0.1.3/promptops/loading/promptops.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/loading/simple.py` & `promptops-0.1.3/promptops/loading/simple.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/main.py` & `promptops-0.1.3/promptops/main.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/query/explanation.py` & `promptops-0.1.3/promptops/query/explanation.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/query/messages.py` & `promptops-0.1.3/promptops/query/messages.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/query/query.py` & `promptops-0.1.3/promptops/query/query.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/query.py` & `promptops-0.1.3/promptops/query.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/recipes/creation.py` & `promptops-0.1.3/promptops/recipes/creation.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/scrub_secrets/scrub.py` & `promptops-0.1.3/promptops/scrub_secrets/scrub.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/secrets/scrub.py` & `promptops-0.1.3/promptops/secrets/scrub.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/settings_store.py` & `promptops-0.1.3/promptops/settings_store.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/shells/base.py` & `promptops-0.1.3/promptops/shells/base.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/shells/bash.py` & `promptops-0.1.3/promptops/shells/bash.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/shells/common.py` & `promptops-0.1.3/promptops/shells/common.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/shells/fish.py` & `promptops-0.1.3/promptops/shells/fish.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/shells/zsh.py` & `promptops-0.1.3/promptops/shells/zsh.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/similarity.py` & `promptops-0.1.3/promptops/similarity.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/ui/prompts.py` & `promptops-0.1.3/promptops/ui/prompts.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/ui/selections.py` & `promptops-0.1.3/promptops/ui/selections.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/ui.py` & `promptops-0.1.3/promptops/ui.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/user.py` & `promptops-0.1.3/promptops/user.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops/version_check.py` & `promptops-0.1.3/promptops/version_check.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/promptops.egg-info/SOURCES.txt` & `promptops-0.1.3/promptops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `promptops-0.1.2/setup.py` & `promptops-0.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pathlib import Path
 from setuptools import setup, find_packages
 import os
 
 
 def get_long_description():
     # fmt: off
     """#PromptOps
@@ -18,23 +19,24 @@
     return g["__version__"]
 
 
 setup(
     name="promptops",
     version=get_version(),
     description="Your CLI assistant. Ask questions, get shell commands.",
-    long_description=get_long_description(),
+    long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type="text/markdown",
     author="CtrlStack inc.",
     url="https://promptops.com/",
     project_urls={
         "Documentation": "https://docs.promptops.com/cli",
         "Changelog": "https://docs.promptops.com/en/stable/changelog.html",
         "Live demo": "https://promptops.com/",
     },
+    license='GPLv3',
     packages=find_packages(exclude=("tests", "tests.*")),
     include_package_data=False,
     python_requires=">=3.9",
     install_requires=[
         "colorama~=0.4.6",
         "urllib3>=1.26,<2",  # kubernetes uses google-auth which has urllib3<2
         "requests~=2.29.0",
```

