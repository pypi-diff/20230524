# Comparing `tmp/katello-host-tools-4.2.2.tar.gz` & `tmp/katello-host-tools-4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katello-host-tools-4.2.2.tar", last modified: Mon Nov  7 15:28:38 2022, max compression
+gzip compressed data, was "katello-host-tools-4.2.3.tar", last modified: Wed Dec  7 15:51:47 2022, max compression
```

## Comparing `katello-host-tools-4.2.2.tar` & `katello-host-tools-4.2.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:38.221391 katello-host-tools-4.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-11-07 15:28:38.221391 katello-host-tools-4.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1495 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:38.209391 katello-host-tools-4.2.2/apt_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/apt_plugins/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1045 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/apt_plugins/tracer_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:38.209391 katello-host-tools-4.2.2/dnf_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/dnf_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1634 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/dnf_plugins/tracer_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:38.213391 katello-host-tools-4.2.2/katello/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:38.213391 katello-host-tools-4.2.2/katello/agent/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:38.213391 katello-host-tools-4.2.2/katello/agent/goferd/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/agent/goferd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11456 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/agent/goferd/legacy_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     9845 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/agent/goferd/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:38.217391 katello-host-tools-4.2.2/katello/agent/pulp/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/agent/pulp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5118 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/agent/pulp/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     7218 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/agent/pulp/handler.py
--rw-r--r--   0 runner    (1001) docker     (121)    14218 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/agent/pulp/libdnf.py
--rw-r--r--   0 runner    (1001) docker     (121)    10943 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/agent/pulp/libyum.py
--rw-r--r--   0 runner    (1001) docker     (121)     5280 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/agent/pulp/report.py
--rw-r--r--   0 runner    (1001) docker     (121)     2450 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/agent/pulp/test.py
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:38.205391 katello-host-tools-4.2.2/katello/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:38.205391 katello-host-tools-4.2.2/katello/contrib/etc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:38.205391 katello-host-tools-4.2.2/katello/contrib/etc/gofer/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:38.209391 katello-host-tools-4.2.2/katello/contrib/etc/gofer/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)     1571 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/contrib/etc/gofer/plugins/katello.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:38.205391 katello-host-tools-4.2.2/katello/contrib/etc/rhsm/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:38.209391 katello-host-tools-4.2.2/katello/contrib/etc/rhsm/pluginconf.d/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/contrib/etc/rhsm/pluginconf.d/fqdn.FactsPlugin.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:38.205391 katello-host-tools-4.2.2/katello/contrib/etc/yum/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:38.209391 katello-host-tools-4.2.2/katello/contrib/etc/yum/pluginconf.d/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/contrib/etc/yum/pluginconf.d/enabled_repos_upload.conf
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/contrib/etc/yum/pluginconf.d/package_upload.conf
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/contrib/etc/yum/pluginconf.d/tracer_upload.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:38.209391 katello-host-tools-4.2.2/katello/contrib/extra/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/contrib/extra/81-tracer-upload-apt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/contrib/extra/katello-tracer-upload-dnf
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/contrib/extra/katello-tracer-upload.cron
--rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/deb_tracer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2198 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/enabled_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/packages.py
--rw-r--r--   0 runner    (1001) docker     (121)     3235 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/repos.py
--rw-r--r--   0 runner    (1001) docker     (121)     2251 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/scripts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1924 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/tracer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/uep.py
--rw-r--r--   0 runner    (1001) docker     (121)      873 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/katello/zypper_tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:38.217391 katello-host-tools-4.2.2/katello_host_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-11-07 15:28:38.000000 katello-host-tools-4.2.2/katello_host_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3762 2022-11-07 15:28:38.000000 katello-host-tools-4.2.2/katello_host_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 15:28:38.000000 katello-host-tools-4.2.2/katello_host_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-11-07 15:28:38.000000 katello-host-tools-4.2.2/katello_host_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-11-07 15:28:38.000000 katello-host-tools-4.2.2/katello_host_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-07 15:28:38.221391 katello-host-tools-4.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1699 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:38.217391 katello-host-tools-4.2.2/yum-plugins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/yum-plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      982 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/yum-plugins/enabled_repos_upload.py
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/yum-plugins/package_upload.py
--rw-r--r--   0 runner    (1001) docker     (121)     1225 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/yum-plugins/tracer_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:38.217391 katello-host-tools-4.2.2/zypper_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/zypper_plugins/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      992 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/zypper_plugins/enabled_repos_upload.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2276 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/zypper_plugins/package_upload.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1232 2022-11-07 15:28:36.000000 katello-host-tools-4.2.2/zypper_plugins/tracer_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:47.907148 katello-host-tools-4.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2022-12-07 15:51:47.907148 katello-host-tools-4.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:47.899148 katello-host-tools-4.2.3/apt_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/apt_plugins/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1045 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/apt_plugins/tracer_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:47.899148 katello-host-tools-4.2.3/dnf_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/dnf_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/dnf_plugins/tracer_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:47.899148 katello-host-tools-4.2.3/katello/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:47.899148 katello-host-tools-4.2.3/katello/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:47.903148 katello-host-tools-4.2.3/katello/agent/goferd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/agent/goferd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11456 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/agent/goferd/legacy_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9845 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/agent/goferd/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:47.903148 katello-host-tools-4.2.3/katello/agent/pulp/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/agent/pulp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/agent/pulp/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/agent/pulp/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14230 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/agent/pulp/libdnf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10943 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/agent/pulp/libyum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/agent/pulp/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/agent/pulp/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:47.895148 katello-host-tools-4.2.3/katello/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:47.895148 katello-host-tools-4.2.3/katello/contrib/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:47.895148 katello-host-tools-4.2.3/katello/contrib/etc/gofer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:47.899148 katello-host-tools-4.2.3/katello/contrib/etc/gofer/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/contrib/etc/gofer/plugins/katello.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:47.895148 katello-host-tools-4.2.3/katello/contrib/etc/rhsm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:47.899148 katello-host-tools-4.2.3/katello/contrib/etc/rhsm/pluginconf.d/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/contrib/etc/rhsm/pluginconf.d/fqdn.FactsPlugin.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:47.895148 katello-host-tools-4.2.3/katello/contrib/etc/yum/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:47.899148 katello-host-tools-4.2.3/katello/contrib/etc/yum/pluginconf.d/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/contrib/etc/yum/pluginconf.d/enabled_repos_upload.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/contrib/etc/yum/pluginconf.d/package_upload.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/contrib/etc/yum/pluginconf.d/tracer_upload.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:47.899148 katello-host-tools-4.2.3/katello/contrib/extra/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/contrib/extra/81-tracer-upload-apt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/contrib/extra/katello-tracer-upload-dnf
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/contrib/extra/katello-tracer-upload.cron
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/deb_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/enabled_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/uep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/katello/zypper_tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:47.903148 katello-host-tools-4.2.3/katello_host_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2022-12-07 15:51:47.000000 katello-host-tools-4.2.3/katello_host_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2022-12-07 15:51:47.000000 katello-host-tools-4.2.3/katello_host_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 15:51:47.000000 katello-host-tools-4.2.3/katello_host_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2022-12-07 15:51:47.000000 katello-host-tools-4.2.3/katello_host_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-07 15:51:47.000000 katello-host-tools-4.2.3/katello_host_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-07 15:51:47.907148 katello-host-tools-4.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:47.907148 katello-host-tools-4.2.3/yum-plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/yum-plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/yum-plugins/enabled_repos_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/yum-plugins/package_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/yum-plugins/tracer_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:47.907148 katello-host-tools-4.2.3/zypper_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/zypper_plugins/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      992 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/zypper_plugins/enabled_repos_upload.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2276 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/zypper_plugins/package_upload.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1232 2022-12-07 15:51:43.000000 katello-host-tools-4.2.3/zypper_plugins/tracer_upload.py
```

### Comparing `katello-host-tools-4.2.2/PKG-INFO` & `katello-host-tools-4.2.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katello-host-tools
-Version: 4.2.2
+Version: 4.2.3
 Summary: Libraries and command-line utilities for keeping Katello clients in sync and up to date
 Home-page: https://github.com/Katello/katello-host-tools
 Author: The Foreman Project
 Author-email: no-email@theforeman.org
 License: GPLv2+
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `katello-host-tools-4.2.2/README.md` & `katello-host-tools-4.2.3/README.md`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/apt_plugins/tracer_upload.py` & `katello-host-tools-4.2.3/apt_plugins/tracer_upload.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/dnf_plugins/tracer_upload.py` & `katello-host-tools-4.2.3/dnf_plugins/tracer_upload.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/katello/agent/goferd/legacy_plugin.py` & `katello-host-tools-4.2.3/katello/agent/goferd/legacy_plugin.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/katello/agent/goferd/plugin.py` & `katello-host-tools-4.2.3/katello/agent/goferd/plugin.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/katello/agent/pulp/dispatcher.py` & `katello-host-tools-4.2.3/katello/agent/pulp/dispatcher.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/katello/agent/pulp/handler.py` & `katello-host-tools-4.2.3/katello/agent/pulp/handler.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/katello/agent/pulp/libdnf.py` & `katello-host-tools-4.2.3/katello/agent/pulp/libdnf.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,15 +252,15 @@
             dict: A dictionary representation of a TransactionReport.
         """
         with LibDnf() as lib:
             patterns = set(str(p) for p in patterns)
             if advisories:
                 for ad, packages in lib.applicable_advisories(AdvisoryFilter(ids=advisories)):
                     for name, evr in packages:
-                        patterns.add(name)
+                        patterns.add(name + '-' + evr)
                 if patterns:
                    lib.upgrade(patterns)
             else:
                 lib.upgrade(patterns)
             if self.commit:
                 lib.do_transaction()
             report = UpdateTxReport(lib.transaction or ())
```

### Comparing `katello-host-tools-4.2.2/katello/agent/pulp/libyum.py` & `katello-host-tools-4.2.3/katello/agent/pulp/libyum.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/katello/agent/pulp/report.py` & `katello-host-tools-4.2.3/katello/agent/pulp/report.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/katello/agent/pulp/test.py` & `katello-host-tools-4.2.3/katello/agent/pulp/test.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/katello/constants.py` & `katello-host-tools-4.2.3/katello/constants.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/katello/contrib/etc/gofer/plugins/katello.conf` & `katello-host-tools-4.2.3/katello/contrib/etc/gofer/plugins/katello.conf`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/katello/deb_tracer.py` & `katello-host-tools-4.2.3/katello/deb_tracer.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/katello/enabled_report.py` & `katello-host-tools-4.2.3/katello/enabled_report.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/katello/packages.py` & `katello-host-tools-4.2.3/katello/packages.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/katello/repos.py` & `katello-host-tools-4.2.3/katello/repos.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/katello/scripts.py` & `katello-host-tools-4.2.3/katello/scripts.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/katello/tracer.py` & `katello-host-tools-4.2.3/katello/tracer.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/katello/uep.py` & `katello-host-tools-4.2.3/katello/uep.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/katello/utils.py` & `katello-host-tools-4.2.3/katello/utils.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/katello/zypper_tracer.py` & `katello-host-tools-4.2.3/katello/zypper_tracer.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/katello_host_tools.egg-info/PKG-INFO` & `katello-host-tools-4.2.3/katello_host_tools.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katello-host-tools
-Version: 4.2.2
+Version: 4.2.3
 Summary: Libraries and command-line utilities for keeping Katello clients in sync and up to date
 Home-page: https://github.com/Katello/katello-host-tools
 Author: The Foreman Project
 Author-email: no-email@theforeman.org
 License: GPLv2+
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `katello-host-tools-4.2.2/katello_host_tools.egg-info/SOURCES.txt` & `katello-host-tools-4.2.3/katello_host_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/setup.py` & `katello-host-tools-4.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Jeff Ortel <jortel@redhat.com>
 #
 
 from setuptools import setup, find_packages
 
 setup(
     name='katello-host-tools',
-    version='4.2.2',
+    version='4.2.3',
     description='Libraries and command-line utilities for keeping Katello clients in sync and up to date',
     author='The Foreman Project',
     author_email='no-email@theforeman.org',
     url='https://github.com/Katello/katello-host-tools',
     license='GPLv2+',
     packages=find_packages(),
     include_package_data=False,
```

### Comparing `katello-host-tools-4.2.2/yum-plugins/enabled_repos_upload.py` & `katello-host-tools-4.2.3/yum-plugins/enabled_repos_upload.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/yum-plugins/package_upload.py` & `katello-host-tools-4.2.3/yum-plugins/package_upload.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/yum-plugins/tracer_upload.py` & `katello-host-tools-4.2.3/yum-plugins/tracer_upload.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/zypper_plugins/enabled_repos_upload.py` & `katello-host-tools-4.2.3/zypper_plugins/enabled_repos_upload.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/zypper_plugins/package_upload.py` & `katello-host-tools-4.2.3/zypper_plugins/package_upload.py`

 * *Files identical despite different names*

### Comparing `katello-host-tools-4.2.2/zypper_plugins/tracer_upload.py` & `katello-host-tools-4.2.3/zypper_plugins/tracer_upload.py`

 * *Files identical despite different names*

