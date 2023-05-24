# Comparing `tmp/pulumi_proxmoxve-4.1.1.tar.gz` & `tmp/pulumi_proxmoxve-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_proxmoxve-4.1.1.tar", last modified: Sun May 14 10:06:02 2023, max compression
+gzip compressed data, was "pulumi_proxmoxve-5.0.0.tar", last modified: Wed May 24 07:45:20 2023, max compression
```

## Comparing `pulumi_proxmoxve-4.1.1.tar` & `pulumi_proxmoxve-5.0.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:06:02.266315 pulumi_proxmoxve-4.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-05-14 10:06:02.266315 pulumi_proxmoxve-4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:06:02.258315 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/certifi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:06:02.258315 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/cluster/get_nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:06:02.262315 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:06:02.262315 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/ct/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/ct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/ct/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37407 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/ct/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    15863 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/ct/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/get_dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/get_hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/get_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/get_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/hosts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:06:02.262315 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/network/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/network/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/network/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/network/firewall_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/network/firewall_ip_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    29546 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/network/firewall_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/network/firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    15125 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/network/firewall_security_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/network/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:06:02.266315 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/get_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/get_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    22997 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10269 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:06:02.266315 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/storage/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17318 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/storage/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/storage/get_datastores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/storage/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:06:02.266315 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/vm/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34450 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/vm/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/vm/get_virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/vm/get_virtual_machines.py
--rw-r--r--   0 runner    (1001) docker     (123)    28465 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/vm/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    83159 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/vm/virtual_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:06:02.258315 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-05-14 10:06:02.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-14 10:06:02.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 10:06:02.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 10:06:02.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-14 10:06:02.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 10:06:02.000000 pulumi_proxmoxve-4.1.1/pulumi_proxmoxve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 10:06:02.266315 pulumi_proxmoxve-4.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-14 10:06:01.000000 pulumi_proxmoxve-4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:45:20.837174 pulumi_proxmoxve-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-05-24 07:45:20.837174 pulumi_proxmoxve-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:45:20.833174 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/certifi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:45:20.833174 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/cluster/get_nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:45:20.833174 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:45:20.833174 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/ct/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/ct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/ct/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37407 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/ct/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15863 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/ct/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/get_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/get_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/get_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/get_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/hosts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:45:20.833174 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/network/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/network/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/network/firewall_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/network/firewall_ip_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29546 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/network/firewall_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/network/firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15125 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/network/firewall_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/network/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:45:20.837174 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22997 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:45:20.837174 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/storage/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17318 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/storage/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/storage/get_datastores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/storage/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:45:20.837174 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/vm/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34450 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/vm/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/vm/get_virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/vm/get_virtual_machines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28465 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/vm/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83159 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/vm/virtual_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:45:20.833174 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/pulumi_proxmoxve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 07:45:20.837174 pulumi_proxmoxve-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-24 07:45:20.000000 pulumi_proxmoxve-5.0.0/setup.py
```

### Comparing `pulumi_proxmoxve-4.1.1/PKG-INFO` & `pulumi_proxmoxve-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_proxmoxve
-Version: 4.1.1
+Version: 5.0.0
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_proxmoxve-4.1.1/README.md` & `pulumi_proxmoxve-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/__init__.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/_inputs.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/get_version.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,103 +6,90 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'HostsEntryArgs',
-    'ProviderVirtualEnvironmentArgs',
+    'GetVersionResult',
+    'AwaitableGetVersionResult',
+    'get_version',
 ]
 
-@pulumi.input_type
-class HostsEntryArgs:
-    def __init__(__self__, *,
-                 address: pulumi.Input[str],
-                 hostnames: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(__self__, "address", address)
-        pulumi.set(__self__, "hostnames", hostnames)
-
-    @property
-    @pulumi.getter
-    def address(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "address")
-
-    @address.setter
-    def address(self, value: pulumi.Input[str]):
-        pulumi.set(self, "address", value)
-
-    @property
-    @pulumi.getter
-    def hostnames(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
-        return pulumi.get(self, "hostnames")
-
-    @hostnames.setter
-    def hostnames(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(self, "hostnames", value)
-
-
-@pulumi.input_type
-class ProviderVirtualEnvironmentArgs:
-    def __init__(__self__, *,
-                 endpoint: Optional[pulumi.Input[str]] = None,
-                 insecure: Optional[pulumi.Input[bool]] = None,
-                 otp: Optional[pulumi.Input[str]] = None,
-                 password: Optional[pulumi.Input[str]] = None,
-                 username: Optional[pulumi.Input[str]] = None):
-        if endpoint is not None:
-            pulumi.set(__self__, "endpoint", endpoint)
-        if insecure is not None:
-            pulumi.set(__self__, "insecure", insecure)
-        if otp is not None:
-            pulumi.set(__self__, "otp", otp)
-        if password is not None:
-            pulumi.set(__self__, "password", password)
-        if username is not None:
-            pulumi.set(__self__, "username", username)
-
-    @property
-    @pulumi.getter
-    def endpoint(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "endpoint")
-
-    @endpoint.setter
-    def endpoint(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "endpoint", value)
-
-    @property
-    @pulumi.getter
-    def insecure(self) -> Optional[pulumi.Input[bool]]:
-        return pulumi.get(self, "insecure")
-
-    @insecure.setter
-    def insecure(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "insecure", value)
-
-    @property
-    @pulumi.getter
-    def otp(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "otp")
-
-    @otp.setter
-    def otp(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "otp", value)
-
-    @property
-    @pulumi.getter
-    def password(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "password")
-
-    @password.setter
-    def password(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "password", value)
-
-    @property
-    @pulumi.getter
-    def username(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "username")
-
-    @username.setter
-    def username(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "username", value)
-
-
+@pulumi.output_type
+class GetVersionResult:
+    """
+    A collection of values returned by getVersion.
+    """
+    def __init__(__self__, id=None, keyboard_layout=None, release=None, repository_id=None, version=None):
+        if id and not isinstance(id, str):
+            raise TypeError("Expected argument 'id' to be a str")
+        pulumi.set(__self__, "id", id)
+        if keyboard_layout and not isinstance(keyboard_layout, str):
+            raise TypeError("Expected argument 'keyboard_layout' to be a str")
+        pulumi.set(__self__, "keyboard_layout", keyboard_layout)
+        if release and not isinstance(release, str):
+            raise TypeError("Expected argument 'release' to be a str")
+        pulumi.set(__self__, "release", release)
+        if repository_id and not isinstance(repository_id, str):
+            raise TypeError("Expected argument 'repository_id' to be a str")
+        pulumi.set(__self__, "repository_id", repository_id)
+        if version and not isinstance(version, str):
+            raise TypeError("Expected argument 'version' to be a str")
+        pulumi.set(__self__, "version", version)
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        The provider-assigned unique ID for this managed resource.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter(name="keyboardLayout")
+    def keyboard_layout(self) -> str:
+        return pulumi.get(self, "keyboard_layout")
+
+    @property
+    @pulumi.getter
+    def release(self) -> str:
+        return pulumi.get(self, "release")
+
+    @property
+    @pulumi.getter(name="repositoryId")
+    def repository_id(self) -> str:
+        return pulumi.get(self, "repository_id")
+
+    @property
+    @pulumi.getter
+    def version(self) -> str:
+        return pulumi.get(self, "version")
+
+
+class AwaitableGetVersionResult(GetVersionResult):
+    # pylint: disable=using-constant-test
+    def __await__(self):
+        if False:
+            yield self
+        return GetVersionResult(
+            id=self.id,
+            keyboard_layout=self.keyboard_layout,
+            release=self.release,
+            repository_id=self.repository_id,
+            version=self.version)
+
+
+def get_version(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVersionResult:
+    """
+    Use this data source to access information about an existing resource.
+    """
+    __args__ = dict()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
+    __ret__ = pulumi.runtime.invoke('proxmoxve:index/getVersion:getVersion', __args__, opts=opts, typ=GetVersionResult).value
+
+    return AwaitableGetVersionResult(
+        id=__ret__.id,
+        keyboard_layout=__ret__.keyboard_layout,
+        release=__ret__.release,
+        repository_id=__ret__.repository_id,
+        version=__ret__.version)
```

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/_utilities.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/certifi.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/certifi.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/cluster/get_nodes.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/cluster/get_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/config/outputs.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/config/vars.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,57 +4,61 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from . import outputs
 
-__all__ = [
-    'VirtualEnvironment',
-]
-
-@pulumi.output_type
-class VirtualEnvironment(dict):
-    def __init__(__self__, *,
-                 endpoint: Optional[str] = None,
-                 insecure: Optional[bool] = None,
-                 otp: Optional[str] = None,
-                 password: Optional[str] = None,
-                 username: Optional[str] = None):
-        if endpoint is not None:
-            pulumi.set(__self__, "endpoint", endpoint)
-        if insecure is not None:
-            pulumi.set(__self__, "insecure", insecure)
-        if otp is not None:
-            pulumi.set(__self__, "otp", otp)
-        if password is not None:
-            pulumi.set(__self__, "password", password)
-        if username is not None:
-            pulumi.set(__self__, "username", username)
+import types
 
+__config__ = pulumi.Config('proxmoxve')
+
+
+class _ExportableConfig(types.ModuleType):
     @property
-    @pulumi.getter
     def endpoint(self) -> Optional[str]:
-        return pulumi.get(self, "endpoint")
+        """
+        The endpoint for the Proxmox Virtual Environment API
+        """
+        return __config__.get('endpoint')
 
     @property
-    @pulumi.getter
     def insecure(self) -> Optional[bool]:
-        return pulumi.get(self, "insecure")
+        """
+        Whether to skip the TLS verification step
+        """
+        return __config__.get_bool('insecure')
 
     @property
-    @pulumi.getter
     def otp(self) -> Optional[str]:
-        return pulumi.get(self, "otp")
+        """
+        The one-time password for the Proxmox Virtual Environment API
+        """
+        return __config__.get('otp')
 
     @property
-    @pulumi.getter
     def password(self) -> Optional[str]:
-        return pulumi.get(self, "password")
+        """
+        The password for the Proxmox Virtual Environment API
+        """
+        return __config__.get('password')
+
+    @property
+    def ssh(self) -> Optional[str]:
+        """
+        The SSH connection configuration to a Proxmox node
+        """
+        return __config__.get('ssh')
 
     @property
-    @pulumi.getter
     def username(self) -> Optional[str]:
-        return pulumi.get(self, "username")
+        """
+        The username for the Proxmox Virtual Environment API
+        """
+        return __config__.get('username')
 
+    @property
+    def virtual_environment(self) -> Optional[str]:
+        return __config__.get('virtualEnvironment')
```

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/ct/_inputs.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/ct/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/ct/container.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/ct/container.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/ct/outputs.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/ct/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/dns.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/get_dns.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/get_dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/get_hosts.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/get_hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/get_time.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/get_time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/get_version.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/get_roles.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,93 +3,83 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from . import _utilities
+from .. import _utilities
 
 __all__ = [
-    'GetVersionResult',
-    'AwaitableGetVersionResult',
-    'get_version',
+    'GetRolesResult',
+    'AwaitableGetRolesResult',
+    'get_roles',
 ]
 
 @pulumi.output_type
-class GetVersionResult:
+class GetRolesResult:
     """
-    A collection of values returned by getVersion.
+    A collection of values returned by getRoles.
     """
-    def __init__(__self__, id=None, keyboard_layout=None, release=None, repository_id=None, version=None):
+    def __init__(__self__, id=None, privileges=None, role_ids=None, specials=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if keyboard_layout and not isinstance(keyboard_layout, str):
-            raise TypeError("Expected argument 'keyboard_layout' to be a str")
-        pulumi.set(__self__, "keyboard_layout", keyboard_layout)
-        if release and not isinstance(release, str):
-            raise TypeError("Expected argument 'release' to be a str")
-        pulumi.set(__self__, "release", release)
-        if repository_id and not isinstance(repository_id, str):
-            raise TypeError("Expected argument 'repository_id' to be a str")
-        pulumi.set(__self__, "repository_id", repository_id)
-        if version and not isinstance(version, str):
-            raise TypeError("Expected argument 'version' to be a str")
-        pulumi.set(__self__, "version", version)
+        if privileges and not isinstance(privileges, list):
+            raise TypeError("Expected argument 'privileges' to be a list")
+        pulumi.set(__self__, "privileges", privileges)
+        if role_ids and not isinstance(role_ids, list):
+            raise TypeError("Expected argument 'role_ids' to be a list")
+        pulumi.set(__self__, "role_ids", role_ids)
+        if specials and not isinstance(specials, list):
+            raise TypeError("Expected argument 'specials' to be a list")
+        pulumi.set(__self__, "specials", specials)
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="keyboardLayout")
-    def keyboard_layout(self) -> str:
-        return pulumi.get(self, "keyboard_layout")
-
-    @property
     @pulumi.getter
-    def release(self) -> str:
-        return pulumi.get(self, "release")
+    def privileges(self) -> Sequence[Sequence[str]]:
+        return pulumi.get(self, "privileges")
 
     @property
-    @pulumi.getter(name="repositoryId")
-    def repository_id(self) -> str:
-        return pulumi.get(self, "repository_id")
+    @pulumi.getter(name="roleIds")
+    def role_ids(self) -> Sequence[str]:
+        return pulumi.get(self, "role_ids")
 
     @property
     @pulumi.getter
-    def version(self) -> str:
-        return pulumi.get(self, "version")
+    def specials(self) -> Sequence[bool]:
+        return pulumi.get(self, "specials")
 
 
-class AwaitableGetVersionResult(GetVersionResult):
+class AwaitableGetRolesResult(GetRolesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetVersionResult(
+        return GetRolesResult(
             id=self.id,
-            keyboard_layout=self.keyboard_layout,
-            release=self.release,
-            repository_id=self.repository_id,
-            version=self.version)
+            privileges=self.privileges,
+            role_ids=self.role_ids,
+            specials=self.specials)
 
 
-def get_version(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVersionResult:
+def get_roles(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRolesResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('proxmoxve:index/getVersion:getVersion', __args__, opts=opts, typ=GetVersionResult).value
+    __ret__ = pulumi.runtime.invoke('proxmoxve:Permission/getRoles:getRoles', __args__, opts=opts, typ=GetRolesResult).value
 
-    return AwaitableGetVersionResult(
+    return AwaitableGetRolesResult(
         id=__ret__.id,
-        keyboard_layout=__ret__.keyboard_layout,
-        release=__ret__.release,
-        repository_id=__ret__.repository_id,
-        version=__ret__.version)
+        privileges=__ret__.privileges,
+        role_ids=__ret__.role_ids,
+        specials=__ret__.specials)
```

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/hosts.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/network/_inputs.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/network/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/network/firewall.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/network/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/network/firewall_alias.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/network/firewall_alias.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/network/firewall_ip_set.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/network/firewall_ip_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/network/firewall_options.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/network/firewall_options.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/network/firewall_rules.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/network/firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/network/firewall_security_group.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/network/firewall_security_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/network/outputs.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/network/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/outputs.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/__init__.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/_inputs.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/get_group.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/get_groups.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/get_pool.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/get_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/get_pools.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/get_pools.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/get_role.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/get_user.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/get_users.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/group.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/outputs.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/pool.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/role.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/permission/user.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/permission/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/provider.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,32 +15,36 @@
 @pulumi.input_type
 class ProviderArgs:
     def __init__(__self__, *,
                  endpoint: Optional[pulumi.Input[str]] = None,
                  insecure: Optional[pulumi.Input[bool]] = None,
                  otp: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
+                 ssh: Optional[pulumi.Input['ProviderSshArgs']] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  virtual_environment: Optional[pulumi.Input['ProviderVirtualEnvironmentArgs']] = None):
         """
         The set of arguments for constructing a Provider resource.
         :param pulumi.Input[str] endpoint: The endpoint for the Proxmox Virtual Environment API
         :param pulumi.Input[bool] insecure: Whether to skip the TLS verification step
         :param pulumi.Input[str] otp: The one-time password for the Proxmox Virtual Environment API
         :param pulumi.Input[str] password: The password for the Proxmox Virtual Environment API
+        :param pulumi.Input['ProviderSshArgs'] ssh: The SSH connection configuration to a Proxmox node
         :param pulumi.Input[str] username: The username for the Proxmox Virtual Environment API
         """
         if endpoint is not None:
             pulumi.set(__self__, "endpoint", endpoint)
         if insecure is not None:
             pulumi.set(__self__, "insecure", insecure)
         if otp is not None:
             pulumi.set(__self__, "otp", otp)
         if password is not None:
             pulumi.set(__self__, "password", password)
+        if ssh is not None:
+            pulumi.set(__self__, "ssh", ssh)
         if username is not None:
             pulumi.set(__self__, "username", username)
         if virtual_environment is not None:
             warnings.warn("""Move attributes out of virtual_environment block""", DeprecationWarning)
             pulumi.log.warn("""virtual_environment is deprecated: Move attributes out of virtual_environment block""")
         if virtual_environment is not None:
             pulumi.set(__self__, "virtual_environment", virtual_environment)
@@ -91,14 +95,26 @@
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
     @property
     @pulumi.getter
+    def ssh(self) -> Optional[pulumi.Input['ProviderSshArgs']]:
+        """
+        The SSH connection configuration to a Proxmox node
+        """
+        return pulumi.get(self, "ssh")
+
+    @ssh.setter
+    def ssh(self, value: Optional[pulumi.Input['ProviderSshArgs']]):
+        pulumi.set(self, "ssh", value)
+
+    @property
+    @pulumi.getter
     def username(self) -> Optional[pulumi.Input[str]]:
         """
         The username for the Proxmox Virtual Environment API
         """
         return pulumi.get(self, "username")
 
     @username.setter
@@ -120,14 +136,15 @@
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  endpoint: Optional[pulumi.Input[str]] = None,
                  insecure: Optional[pulumi.Input[bool]] = None,
                  otp: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
+                 ssh: Optional[pulumi.Input[pulumi.InputType['ProviderSshArgs']]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  virtual_environment: Optional[pulumi.Input[pulumi.InputType['ProviderVirtualEnvironmentArgs']]] = None,
                  __props__=None):
         """
         The provider type for the proxmoxve package. By default, resources use package-wide configuration
         settings, however an explicit `Provider` instance may be created and passed during resource
         construction to achieve fine-grained programmatic control over provider settings. See the
@@ -135,14 +152,15 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] endpoint: The endpoint for the Proxmox Virtual Environment API
         :param pulumi.Input[bool] insecure: Whether to skip the TLS verification step
         :param pulumi.Input[str] otp: The one-time password for the Proxmox Virtual Environment API
         :param pulumi.Input[str] password: The password for the Proxmox Virtual Environment API
+        :param pulumi.Input[pulumi.InputType['ProviderSshArgs']] ssh: The SSH connection configuration to a Proxmox node
         :param pulumi.Input[str] username: The username for the Proxmox Virtual Environment API
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ProviderArgs] = None,
@@ -168,14 +186,15 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  endpoint: Optional[pulumi.Input[str]] = None,
                  insecure: Optional[pulumi.Input[bool]] = None,
                  otp: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
+                 ssh: Optional[pulumi.Input[pulumi.InputType['ProviderSshArgs']]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  virtual_environment: Optional[pulumi.Input[pulumi.InputType['ProviderVirtualEnvironmentArgs']]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
@@ -183,14 +202,15 @@
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
             __props__.__dict__["endpoint"] = endpoint
             __props__.__dict__["insecure"] = pulumi.Output.from_input(insecure).apply(pulumi.runtime.to_json) if insecure is not None else None
             __props__.__dict__["otp"] = otp
             __props__.__dict__["password"] = password
+            __props__.__dict__["ssh"] = pulumi.Output.from_input(ssh).apply(pulumi.runtime.to_json) if ssh is not None else None
             __props__.__dict__["username"] = username
             if virtual_environment is not None and not opts.urn:
                 warnings.warn("""Move attributes out of virtual_environment block""", DeprecationWarning)
                 pulumi.log.warn("""virtual_environment is deprecated: Move attributes out of virtual_environment block""")
             __props__.__dict__["virtual_environment"] = pulumi.Output.from_input(virtual_environment).apply(pulumi.runtime.to_json) if virtual_environment is not None else None
         super(Provider, __self__).__init__(
             'proxmoxve',
```

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/storage/_inputs.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/storage/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/storage/file.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/storage/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/storage/get_datastores.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/storage/get_datastores.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/storage/outputs.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/storage/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/time.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/vm/_inputs.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/vm/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/vm/get_virtual_machine.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/vm/get_virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/vm/get_virtual_machines.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/vm/get_virtual_machines.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/vm/outputs.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/vm/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve/vm/virtual_machine.py` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve/vm/virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve.egg-info/PKG-INFO` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-proxmoxve
-Version: 4.1.1
+Version: 5.0.0
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_proxmoxve-4.1.1/pulumi_proxmoxve.egg-info/SOURCES.txt` & `pulumi_proxmoxve-5.0.0/pulumi_proxmoxve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-4.1.1/setup.py` & `pulumi_proxmoxve-5.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.1.1"
-PLUGIN_VERSION = "4.1.1"
+VERSION = "5.0.0"
+PLUGIN_VERSION = "5.0.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'proxmoxve', PLUGIN_VERSION, '--server', 'github://api.github.com/muhlba91/pulumi-proxmoxve'])
         except OSError as error:
```

