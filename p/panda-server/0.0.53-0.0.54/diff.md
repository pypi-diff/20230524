# Comparing `tmp/panda-server-0.0.53.tar.gz` & `tmp/panda-server-0.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda-server-0.0.53.tar", last modified: Tue Apr 25 06:52:21 2023, max compression
+gzip compressed data, was "panda-server-0.0.54.tar", last modified: Wed May 24 08:45:02 2023, max compression
```

## Comparing `panda-server-0.0.53.tar` & `panda-server-0.0.54.tar`

### file list

```diff
@@ -1,237 +1,224 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.168215 panda-server-0.0.53/
--rw-r--r--   0 runner    (1001) docker     (123)    81051 2023-04-25 06:52:10.000000 panda-server-0.0.53/ChangeLog.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-25 06:52:10.000000 panda-server-0.0.53/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-25 06:52:10.000000 panda-server-0.0.53/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-25 06:52:21.168215 panda-server-0.0.53/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-25 06:52:10.000000 panda-server-0.0.53/PandaPkgInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-25 06:52:10.000000 panda-server-0.0.53/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.128214 panda-server-0.0.53/panda_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-25 06:52:21.000000 panda-server-0.0.53/panda_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-04-25 06:52:21.000000 panda-server-0.0.53/panda_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 06:52:21.000000 panda-server-0.0.53/panda_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 06:52:20.000000 panda-server-0.0.53/panda_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-25 06:52:21.000000 panda-server-0.0.53/panda_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 06:52:21.000000 panda-server-0.0.53/panda_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.128214 panda-server-0.0.53/pandaserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.128214 panda-server-0.0.53/pandaserver/brokerage/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/brokerage/ErrorCode.py
--rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/brokerage/SiteMapper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/brokerage/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    80940 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/brokerage/broker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.128214 panda-server-0.0.53/pandaserver/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/config/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/config/daemon_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7052 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/config/panda_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.128214 panda-server-0.0.53/pandaserver/configurator/
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/configurator/Carbon.py
--rw-r--r--   0 runner    (1001) docker     (123)    35264 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/configurator/Configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/configurator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/configurator/aux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.128214 panda-server-0.0.53/pandaserver/daemons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/master.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.132214 panda-server-0.0.53/pandaserver/daemons/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/add_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/add_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/carbon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)    64166 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/copyArchive.py
--rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/datasetManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/dummy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/evpPD2P.py
--rw-r--r--   0 runner    (1001) docker     (123)    37494 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/metric_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/panda_activeusers_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/pilotStreaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/process_workflow_files_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/recover_lost_files_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)    15074 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/task_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/tmpwatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/scripts/worker_synchronization.py
--rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/daemons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.136214 panda-server-0.0.53/pandaserver/dataservice/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/Activator.py
--rw-r--r--   0 runner    (1001) docker     (123)    53929 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/AdderAtlasPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/AdderDummyPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    40218 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/AdderGen.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/AdderPluginBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/AdderResult.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/AdderSimplePlugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17541 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/Closer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/CloserAtlasPlugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27051 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/DDM.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1988 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/DDMHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/DataService.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/DataServiceUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    57671 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/DynDataDistributer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      412 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/ErrorCode.py
--rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/EventPicker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11067 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/Finisher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16870 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/Notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/ProcessLimiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/RecoverLostFilesCore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8488 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/Setupper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   113610 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/SetupperAtlasPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/SetupperDummyPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/SetupperPluginBase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/eventLookupClientEI.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2101 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/dataservice/forkSetupper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.140214 panda-server-0.0.53/pandaserver/jobdispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/jobdispatcher/DispatcherUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      263 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/jobdispatcher/ErrorCode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    58936 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/jobdispatcher/JobDispatcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16316 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/jobdispatcher/Protocol.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8959 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/jobdispatcher/Watcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/jobdispatcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.140214 panda-server-0.0.53/pandaserver/proxycache/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2898 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/proxycache/DBMSql.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/proxycache/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/proxycache/panda_activeusers_query.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9479 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/proxycache/panda_proxy_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.140214 panda-server-0.0.53/pandaserver/server/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/server/.gacl
--rwxr-xr-x   0 runner    (1001) docker     (123)    22396 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/server/panda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.140214 panda-server-0.0.53/pandaserver/srvcore/
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/srvcore/CoreUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4037 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/srvcore/MailUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/srvcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/srvcore/oidc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/srvcore/srv_msg_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.152214 panda-server-0.0.53/pandaserver/taskbuffer/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/CloudSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/CloudTaskSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/ConBridge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2132 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/DBProxyPool.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3002 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/DatasetSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/DdmSpec.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4647 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/EiDBProxy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1799 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/ErrorCode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/EventServiceUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7836 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/FileSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/GlobalShares.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/HarvesterMetricsSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/Initializer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25903 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/JobSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/JobUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/NucleusSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)  1229216 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/OraDBProxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/PanDAMsgProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/PandaDBSchemaInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/PrioUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/ProcessGroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/ResourceSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/SQLDumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/SiteSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/SupErrors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   137660 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/TaskBuffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/TaskBufferInterface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19209 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/WorkerSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)    17662 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/WrappedCursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/WrappedPickle.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/WrappedPostgresConn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/retryModule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/taskbuffer/workflow_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.160215 panda-server-0.0.53/pandaserver/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/SchemaChecker.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.160215 panda-server-0.0.53/pandaserver/test/alice/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/alice/titan_testScript_ec2_alice_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/alice/titan_testScript_ec2_alice_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/banUser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      623 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/boostPrio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/boostUser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      789 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/callbackDDM.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10377 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/finishJob.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/finishTaskJEDI.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/frontier_retagging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1314 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/getJobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/killJob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2952 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/killJobLowPrio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1625 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/killJobsInTask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/killProdJobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2417 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/killTask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      239 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/killTaskJEDI.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/killUser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.160215 panda-server-0.0.53/pandaserver/test/lsst/
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/lsst/lsstSubmit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/lsst/lsstSubmitMERGEtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/lsst/lsstSubmitPhosim332.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      339 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/reassignJobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/reassignSite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/reassignTask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/reassignWaiting.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/recoverLostFiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/reloadInputDS.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/sendCommandToJob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/setDebugMode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      806 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/setPriority.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1834 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testEvgen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1808 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testEvgen17.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2574 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testG4sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testG4sim17.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testGetCriteriaForGlobalShares.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testGlobalShares.py
--rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testJobFlowATLAS.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3739 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testReco.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testSimulReco14.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testSiteMap.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testUpdateWorkerPilotStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/test/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.160215 panda-server-0.0.53/pandaserver/userinterface/
--rwxr-xr-x   0 runner    (1001) docker     (123)    81389 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/userinterface/Client.py
--rw-r--r--   0 runner    (1001) docker     (123)    89144 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/userinterface/UserIF.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/userinterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.160215 panda-server-0.0.53/pandaserver/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/workflow/pcwl_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/workflow/pcwl_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/workflow/psnakemake_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.164214 panda-server-0.0.53/pandaserver/workflow/snakeparser/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/workflow/snakeparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/workflow/snakeparser/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/workflow/snakeparser/log.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/workflow/snakeparser/names.py
--rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/workflow/snakeparser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/workflow/snakeparser/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35878 2023-04-25 06:52:10.000000 panda-server-0.0.53/pandaserver/workflow/workflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-25 06:52:21.168215 panda-server-0.0.53/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)    13632 2023-04-25 06:52:10.000000 panda-server-0.0.53/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.168215 panda-server-0.0.53/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/conda_meta.yaml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.168215 panda-server-0.0.53/templates/init.d/
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/init.d/panda_daemon.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/init.d/panda_httpd.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)     1547 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/init.d/panda_server.exe.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.168215 panda-server-0.0.53/templates/logrotate.d/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/logrotate.d/panda_server.logrotate.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      164 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-add_main.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-add_sub.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-backupJobArch.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      164 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-boostUser.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      168 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-callback.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      168 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-configurator.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-copyArchive.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-datasetManager.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-esPreemption.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      317 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-evpPD2P.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-frontier_retagging.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-httpd-FastCGI.conf.rpmnew.template
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-httpd.conf.rpmnew.template
--rwxr-xr-x   0 runner    (1001) docker     (123)    13906 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-makeSlsXml.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-network_configurator.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-pilot_streaming.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      158 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-priority.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-proxyCache.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-schedconfig_json.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-sw_tags.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-tmpwatch.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      745 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server-vomsrenew.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/panda_server.cfg.rpmnew.template
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/pandasrv.cron.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:52:21.168215 panda-server-0.0.53/templates/sysconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-25 06:52:10.000000 panda-server-0.0.53/templates/sysconfig/panda_server.sysconfig.rpmnew.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.218685 panda-server-0.0.54/
+-rw-r--r--   0 runner    (1001) docker     (123)    81051 2023-05-24 08:44:50.000000 panda-server-0.0.54/ChangeLog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-24 08:44:50.000000 panda-server-0.0.54/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-24 08:44:50.000000 panda-server-0.0.54/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-24 08:45:02.218685 panda-server-0.0.54/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-24 08:44:50.000000 panda-server-0.0.54/PandaPkgInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-24 08:44:50.000000 panda-server-0.0.54/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.162684 panda-server-0.0.54/panda_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-24 08:45:02.000000 panda-server-0.0.54/panda_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-05-24 08:45:02.000000 panda-server-0.0.54/panda_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 08:45:02.000000 panda-server-0.0.54/panda_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 08:45:01.000000 panda-server-0.0.54/panda_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-24 08:45:02.000000 panda-server-0.0.54/panda_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 08:45:02.000000 panda-server-0.0.54/panda_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.162684 panda-server-0.0.54/pandaserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.162684 panda-server-0.0.54/pandaserver/brokerage/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/brokerage/ErrorCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/brokerage/SiteMapper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/brokerage/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    80940 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/brokerage/broker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.166684 panda-server-0.0.54/pandaserver/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/config/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/config/daemon_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7167 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/config/panda_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.166684 panda-server-0.0.54/pandaserver/configurator/
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/configurator/Carbon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35264 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/configurator/Configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/configurator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/configurator/aux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.166684 panda-server-0.0.54/pandaserver/daemons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/daemons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/daemons/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/daemons/master_systemd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.182684 panda-server-0.0.54/pandaserver/daemons/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/daemons/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/daemons/scripts/add_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/daemons/scripts/add_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/daemons/scripts/carbon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/daemons/scripts/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64166 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/daemons/scripts/copyArchive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/daemons/scripts/datasetManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/daemons/scripts/dummy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/daemons/scripts/evpPD2P.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41977 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/daemons/scripts/metric_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/daemons/scripts/panda_activeusers_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/daemons/scripts/pilotStreaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/daemons/scripts/process_workflow_files_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/daemons/scripts/recover_lost_files_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15074 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/daemons/scripts/task_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/daemons/scripts/tmpwatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/daemons/scripts/worker_synchronization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/daemons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.186684 panda-server-0.0.54/pandaserver/dataservice/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/Activator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53929 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/AdderAtlasPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/AdderDummyPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40601 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/AdderGen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/AdderPluginBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/AdderResult.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/AdderSimplePlugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17541 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/Closer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/CloserAtlasPlugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27051 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/DDM.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1988 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/DDMHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/DataService.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/DataServiceUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57671 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/DynDataDistributer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      412 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/ErrorCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/EventPicker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11067 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/Finisher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18450 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/Notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/ProcessLimiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/RecoverLostFilesCore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8488 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/Setupper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   113605 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/SetupperAtlasPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/SetupperDummyPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/SetupperPluginBase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/eventLookupClientEI.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2101 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/dataservice/forkSetupper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.190684 panda-server-0.0.54/pandaserver/jobdispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/jobdispatcher/DispatcherUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      263 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/jobdispatcher/ErrorCode.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    58936 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/jobdispatcher/JobDispatcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16316 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/jobdispatcher/Protocol.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8959 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/jobdispatcher/Watcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/jobdispatcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.190684 panda-server-0.0.54/pandaserver/proxycache/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2898 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/proxycache/DBMSql.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/proxycache/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/proxycache/panda_activeusers_query.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9479 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/proxycache/panda_proxy_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.190684 panda-server-0.0.54/pandaserver/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/server/.gacl
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22444 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/server/panda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.190684 panda-server-0.0.54/pandaserver/srvcore/
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/srvcore/CoreUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4037 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/srvcore/MailUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/srvcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/srvcore/oidc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/srvcore/srv_msg_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.202684 panda-server-0.0.54/pandaserver/taskbuffer/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/CloudSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/CloudTaskSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/ConBridge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2132 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/DBProxyPool.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3002 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/DatasetSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/DdmSpec.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4647 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/EiDBProxy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1799 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/ErrorCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/EventServiceUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7836 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/FileSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/GlobalShares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/HarvesterMetricsSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/Initializer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25903 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/JobSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/JobUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/NucleusSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1232253 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/OraDBProxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/PanDAMsgProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/PandaDBSchemaInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/PrioUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/ProcessGroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/ResourceSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/SQLDumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/SiteSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/SupErrors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   138224 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/TaskBuffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/TaskBufferInterface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19209 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/WorkerSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17662 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/WrappedCursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/WrappedPickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/WrappedPostgresConn.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/retryModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/taskbuffer/workflow_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.210684 panda-server-0.0.54/pandaserver/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/SchemaChecker.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.210684 panda-server-0.0.54/pandaserver/test/alice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/alice/titan_testScript_ec2_alice_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/alice/titan_testScript_ec2_alice_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/banUser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      623 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/boostPrio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/boostUser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      789 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/callbackDDM.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10377 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/finishJob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/finishTaskJEDI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/frontier_retagging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1314 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/getJobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/killJob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2952 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/killJobLowPrio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1625 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/killJobsInTask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/killProdJobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2417 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/killTask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      239 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/killTaskJEDI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/killUser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.210684 panda-server-0.0.54/pandaserver/test/lsst/
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/lsst/lsstSubmit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/lsst/lsstSubmitMERGEtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/lsst/lsstSubmitPhosim332.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      339 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/reassignJobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/reassignSite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/reassignTask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/reassignWaiting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/recoverLostFiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/reloadInputDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/sendCommandToJob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/setDebugMode.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      806 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/setPriority.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1834 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/testEvgen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1808 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/testEvgen17.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2574 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/testG4sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/testG4sim17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/testGetCriteriaForGlobalShares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/testGlobalShares.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/testJobFlowATLAS.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3739 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/testReco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/testSimulReco14.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/testSiteMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/testUpdateWorkerPilotStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/test/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.210684 panda-server-0.0.54/pandaserver/userinterface/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81389 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/userinterface/Client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89624 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/userinterface/UserIF.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/userinterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.214684 panda-server-0.0.54/pandaserver/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/workflow/pcwl_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/workflow/pcwl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/workflow/psnakemake_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.214684 panda-server-0.0.54/pandaserver/workflow/snakeparser/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/workflow/snakeparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/workflow/snakeparser/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/workflow/snakeparser/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/workflow/snakeparser/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/workflow/snakeparser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/workflow/snakeparser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35878 2023-05-24 08:44:50.000000 panda-server-0.0.54/pandaserver/workflow/workflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-24 08:45:02.218685 panda-server-0.0.54/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12523 2023-05-24 08:44:50.000000 panda-server-0.0.54/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.214684 panda-server-0.0.54/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-24 08:44:50.000000 panda-server-0.0.54/templates/conda_meta.yaml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.218685 panda-server-0.0.54/templates/init.d/
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-24 08:44:50.000000 panda-server-0.0.54/templates/init.d/panda_daemon.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-05-24 08:44:50.000000 panda-server-0.0.54/templates/init.d/panda_httpd.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1547 2023-05-24 08:44:50.000000 panda-server-0.0.54/templates/init.d/panda_server.exe.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.218685 panda-server-0.0.54/templates/logrotate.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-24 08:44:50.000000 panda-server-0.0.54/templates/logrotate.d/panda_server.logrotate.template
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-05-24 08:44:50.000000 panda-server-0.0.54/templates/panda_server-httpd-FastCGI.conf.rpmnew.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-24 08:44:50.000000 panda-server-0.0.54/templates/panda_server-httpd.conf.rpmnew.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13906 2023-05-24 08:44:50.000000 panda-server-0.0.54/templates/panda_server-makeSlsXml.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      745 2023-05-24 08:44:50.000000 panda-server-0.0.54/templates/panda_server-vomsrenew.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-24 08:44:50.000000 panda-server-0.0.54/templates/panda_server.cfg.rpmnew.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.218685 panda-server-0.0.54/templates/sysconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-24 08:44:50.000000 panda-server-0.0.54/templates/sysconfig/panda_server.sysconfig.rpmnew.template
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-24 08:44:50.000000 panda-server-0.0.54/templates/sysconfig/panda_server_env.systemd.rpmnew.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:45:02.218685 panda-server-0.0.54/templates/systemd/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-24 08:44:50.000000 panda-server-0.0.54/templates/systemd/panda.service.template
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-24 08:44:50.000000 panda-server-0.0.54/templates/systemd/panda_daemon.service.template
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-24 08:44:50.000000 panda-server-0.0.54/templates/systemd/panda_httpd.service.template
```

### Comparing `panda-server-0.0.53/ChangeLog.txt` & `panda-server-0.0.54/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/LICENSE.txt` & `panda-server-0.0.54/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/panda_server.egg-info/SOURCES.txt` & `panda-server-0.0.54/panda_server.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 pandaserver/config/panda_config.py
 pandaserver/configurator/Carbon.py
 pandaserver/configurator/Configurator.py
 pandaserver/configurator/__init__.py
 pandaserver/configurator/aux.py
 pandaserver/daemons/__init__.py
 pandaserver/daemons/master.py
+pandaserver/daemons/master_systemd.py
 pandaserver/daemons/utils.py
 pandaserver/daemons/scripts/__init__.py
 pandaserver/daemons/scripts/add_main.py
 pandaserver/daemons/scripts/add_sub.py
 pandaserver/daemons/scripts/carbon.py
 pandaserver/daemons/scripts/configurator.py
 pandaserver/daemons/scripts/copyArchive.py
@@ -177,36 +178,21 @@
 pandaserver/workflow/snakeparser/__init__.py
 pandaserver/workflow/snakeparser/extensions.py
 pandaserver/workflow/snakeparser/log.py
 pandaserver/workflow/snakeparser/names.py
 pandaserver/workflow/snakeparser/parser.py
 pandaserver/workflow/snakeparser/utils.py
 templates/conda_meta.yaml.template
-templates/panda_server-add_main.exe.template
-templates/panda_server-add_sub.exe.template
-templates/panda_server-backupJobArch.exe.template
-templates/panda_server-boostUser.exe.template
-templates/panda_server-callback.exe.template
-templates/panda_server-configurator.exe.template
-templates/panda_server-copyArchive.exe.template
-templates/panda_server-datasetManager.exe.template
-templates/panda_server-esPreemption.exe.template
-templates/panda_server-evpPD2P.exe.template
-templates/panda_server-frontier_retagging.exe.template
 templates/panda_server-httpd-FastCGI.conf.rpmnew.template
 templates/panda_server-httpd.conf.rpmnew.template
 templates/panda_server-makeSlsXml.exe.template
-templates/panda_server-network_configurator.exe.template
-templates/panda_server-pilot_streaming.exe.template
-templates/panda_server-priority.exe.template
-templates/panda_server-proxyCache.exe.template
-templates/panda_server-schedconfig_json.exe.template
-templates/panda_server-sw_tags.exe.template
-templates/panda_server-tmpwatch.exe.template
 templates/panda_server-vomsrenew.exe.template
 templates/panda_server.cfg.rpmnew.template
-templates/pandasrv.cron.template
 templates/init.d/panda_daemon.exe.template
 templates/init.d/panda_httpd.exe.template
 templates/init.d/panda_server.exe.template
 templates/logrotate.d/panda_server.logrotate.template
-templates/sysconfig/panda_server.sysconfig.rpmnew.template
+templates/sysconfig/panda_server.sysconfig.rpmnew.template
+templates/sysconfig/panda_server_env.systemd.rpmnew.template
+templates/systemd/panda.service.template
+templates/systemd/panda_daemon.service.template
+templates/systemd/panda_httpd.service.template
```

### Comparing `panda-server-0.0.53/pandaserver/brokerage/SiteMapper.py` & `panda-server-0.0.54/pandaserver/brokerage/SiteMapper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/brokerage/broker.py` & `panda-server-0.0.54/pandaserver/brokerage/broker.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/config/daemon_config.py` & `panda-server-0.0.54/pandaserver/config/daemon_config.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/config/panda_config.py` & `panda-server-0.0.54/pandaserver/config/panda_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,14 +137,18 @@
 except Exception:
     tmpSelf.__dict__['auth_config'] = {}
 
 # use cert in configurator
 if 'configurator_use_cert' not in tmpSelf.__dict__:
     tmpSelf.__dict__['configurator_use_cert'] = True
 
+# adder serialization
+if 'add_serialized' not in tmpSelf.__dict__:
+    tmpSelf.__dict__['add_serialized'] = False
+
 # dict for plugins
 g_pluginMap = {}    
 
 # parser for plugin setup
 def parsePluginConf(modConfigName):
     global tmpSelf
     global g_pluginMap
```

### Comparing `panda-server-0.0.53/pandaserver/configurator/Carbon.py` & `panda-server-0.0.54/pandaserver/configurator/Carbon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/configurator/Configurator.py` & `panda-server-0.0.54/pandaserver/configurator/Configurator.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/configurator/aux.py` & `panda-server-0.0.54/pandaserver/configurator/aux.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/daemons/master.py` & `panda-server-0.0.54/pandaserver/daemons/master.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/daemons/scripts/add_main.py` & `panda-server-0.0.54/pandaserver/daemons/scripts/add_main.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/daemons/scripts/add_sub.py` & `panda-server-0.0.54/pandaserver/daemons/scripts/add_sub.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/daemons/scripts/carbon.py` & `panda-server-0.0.54/pandaserver/daemons/scripts/carbon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/daemons/scripts/configurator.py` & `panda-server-0.0.54/pandaserver/daemons/scripts/configurator.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/daemons/scripts/copyArchive.py` & `panda-server-0.0.54/pandaserver/daemons/scripts/copyArchive.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/daemons/scripts/datasetManager.py` & `panda-server-0.0.54/pandaserver/daemons/scripts/datasetManager.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/daemons/scripts/dummy_test.py` & `panda-server-0.0.54/pandaserver/daemons/scripts/dummy_test.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/daemons/scripts/evpPD2P.py` & `panda-server-0.0.54/pandaserver/daemons/scripts/evpPD2P.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/daemons/scripts/metric_collector.py` & `panda-server-0.0.54/pandaserver/daemons/scripts/metric_collector.py`

 * *Files 18% similar despite different names*

```diff
@@ -114,14 +114,22 @@
         # end loop
         # tmp_log.debug('done')
         return True, return_map
     except Exception as e:
         tmp_log.error('Exception {0}: {1}'.format(e.__class__.__name__, e))
         return False, {}
 
+# get each share and its leaf share
+def fill_leaf_shares(key, val, the_list):
+    if val is None:
+        the_list.append(key)
+    else:
+        for k, v in val.items():
+            fill_leaf_shares(k, v, the_list)
+
 
 class MetricsDB(object):
     """
     Proxy to access the metrics table in DB
     """
 
     def __init__(self, tbuf):
@@ -463,28 +471,91 @@
 
     def gshare_preference(self):
         tmp_log = logger_utils.make_logger(main_logger, 'FetchData')
         try:
             # get share and hs info
             if self.gshare_status is None:
                 self.gshare_status = self.tbuf.getGShareStatus()
+            share_name_tree_dict = self.tbuf.get_tree_of_gshare_names()
             # initialize
             gshare_dict = dict()
+            total_hs = sum([ leaf['target'] for leaf in self.gshare_status ])
             # rank and data
             for idx, leaf in enumerate(self.gshare_status):
                 rank = idx + 1
                 gshare = leaf['name']
                 gshare_dict[gshare] = {
                     'gshare': gshare,
                     'rank': rank,
+                    'queuing_hs': leaf['queuing'],
                     'running_hs': leaf['running'],
                     'target_hs': leaf['target'],
                     'usage_perc': leaf['running']/leaf['target'] if leaf['target'] > 0 else 999999,
+                    'queue_perc': leaf['queuing']/leaf['target'] if leaf['target'] > 0 else 999999,
+                    'norm_usage_perc': leaf['running']/total_hs if total_hs > 0 else 999999,
+                    'norm_queue_perc': leaf['queuing']/total_hs if total_hs > 0 else 999999,
+                    'norm_target_perc': leaf['target']/total_hs if total_hs > 0 else 999999,
+                    'proj_target_hs': 0,
+                    'eqiv_target_hs': 0,
+                    'eqiv_usage_perc': 0,
                 }
-                tmp_log.debug('rank={rank}, gshare={gshare}, usage={usage_perc:.3%}'.format(**gshare_dict[gshare]))
+                tmp_log.debug('rank={rank}, gshare={gshare}, usage={usage_perc:.3%}, queue={queue_perc:.3%} '.format(**gshare_dict[gshare]))
+            # add L1 share
+            tmp_L1_leaves_map = {}
+            l1_share_dict = {}
+            for l1_share, val in share_name_tree_dict.items():
+                tmp_L1_leaves_map.setdefault(l1_share, [])
+                fill_leaf_shares(l1_share, val, tmp_L1_leaves_map[l1_share])
+            for l1_share, leaves_list in tmp_L1_leaves_map.items():
+                l1_share_name = 'L1 {}'.format(l1_share)
+                l1_share_dict.setdefault(l1_share_name, {
+                        'gshare': l1_share_name,
+                        'rank': -1,
+                        'queuing_hs': 0,
+                        'running_hs': 0,
+                        'target_hs': 0,
+                        'usage_perc': 0,
+                        'queue_perc': 0,
+                    })
+                val_dict = l1_share_dict[l1_share_name]
+                for leaf in leaves_list:
+                    if leaf in gshare_dict:
+                        for field in ['queuing_hs', 'running_hs', 'target_hs']:
+                            val_dict.setdefault(field, 0)
+                            val_dict[field] += gshare_dict[leaf].get(field, 0)
+                val_dict['usage_perc'] = val_dict['running_hs']/val_dict['target_hs'] if val_dict['target_hs'] > 0 else 999999
+                val_dict['queue_perc'] = val_dict['queuing_hs']/val_dict['target_hs'] if val_dict['target_hs'] > 0 else 999999
+                val_dict['norm_usage_perc'] = val_dict['running_hs']/total_hs if total_hs > 0 else 999999
+                val_dict['norm_queue_perc'] = val_dict['queuing_hs']/total_hs if total_hs > 0 else 999999
+                val_dict['norm_target_perc'] = val_dict['target_hs']/total_hs
+                val_dict['proj_target_hs'] = min(val_dict['target_hs'], max(val_dict['running_hs'], val_dict['queuing_hs']/2))
+            proj_total_hs = sum([ v['proj_target_hs'] for v in l1_share_dict.values() ])
+            idle_total_hs = total_hs - proj_total_hs
+            idle_l1_share_list = []
+            idle_threshold_perc = 0.85
+            for l1_share_name, val_dict in l1_share_dict.items():
+                if val_dict['usage_perc'] < idle_threshold_perc and val_dict['proj_target_hs'] < val_dict['target_hs']:
+                    # idle l1 shares
+                    idle_l1_share_list.append(l1_share_name)
+            busy_total_hs = sum([ v['target_hs'] for k, v in l1_share_dict.items() if k not in idle_l1_share_list ]) + 1
+            for l1_share_name, val_dict in l1_share_dict.items():
+                if l1_share_name in idle_l1_share_list:
+                    # idle l1 shares
+                    val_dict['eqiv_target_hs'] = val_dict['target_hs']
+                    val_dict['eqiv_usage_perc'] = val_dict['usage_perc']
+                else:
+                    # busy l1 shares
+                    val_dict['eqiv_target_hs'] = val_dict['target_hs'] + idle_total_hs*val_dict['target_hs']/busy_total_hs
+                    val_dict['eqiv_usage_perc'] = val_dict['running_hs']/val_dict['eqiv_target_hs']
+                tmp_log.debug(( 'share={gshare}, usage={usage_perc:.3%}, queue={queue_perc:.3%}, '
+                                'target_hs={target_hs:.0f}, eqiv_target_hs={eqiv_target_hs:.0f}, '
+                                'norm_target_perc={norm_target_perc:.3%}, eqiv_usage_perc={eqiv_usage_perc:.3%}, '
+                                'norm_usage={norm_usage_perc:.3%}, norm_queue={norm_queue_perc:.3%} '
+                                ).format(**val_dict))
+            gshare_dict.update(l1_share_dict)
             # return
             return gshare_dict
         except Exception:
             tmp_log.error(traceback.format_exc())
 
     def analy_site_eval(self):
         tmp_log = logger_utils.make_logger(main_logger, 'FetchData')
```

### Comparing `panda-server-0.0.53/pandaserver/daemons/scripts/panda_activeusers_query.py` & `panda-server-0.0.54/pandaserver/daemons/scripts/panda_activeusers_query.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/daemons/scripts/pilotStreaming.py` & `panda-server-0.0.54/pandaserver/daemons/scripts/pilotStreaming.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/daemons/scripts/process_workflow_files_daemon.py` & `panda-server-0.0.54/pandaserver/daemons/scripts/process_workflow_files_daemon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/daemons/scripts/recover_lost_files_daemon.py` & `panda-server-0.0.54/pandaserver/daemons/scripts/recover_lost_files_daemon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/daemons/scripts/task_evaluator.py` & `panda-server-0.0.54/pandaserver/daemons/scripts/task_evaluator.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/daemons/scripts/tmpwatch.py` & `panda-server-0.0.54/pandaserver/daemons/scripts/tmpwatch.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/daemons/scripts/worker_synchronization.py` & `panda-server-0.0.54/pandaserver/daemons/scripts/worker_synchronization.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/daemons/utils.py` & `panda-server-0.0.54/pandaserver/daemons/utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/dataservice/Activator.py` & `panda-server-0.0.54/pandaserver/dataservice/Activator.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/dataservice/AdderAtlasPlugin.py` & `panda-server-0.0.54/pandaserver/dataservice/AdderAtlasPlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/dataservice/AdderGen.py` & `panda-server-0.0.54/pandaserver/dataservice/AdderGen.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,15 +305,15 @@
                 if self.job.commandToPilot == 'tobekilled' and self.job.jobStatus == 'failed':
                     self.job.jobStatus = 'cancelled'
                 # update job
                 if oldJobStatus in ['cancelled', 'closed']:
                     pass
                 else:
                     db_lock = None
-                    if self.job.jediTaskID not in [0, None, 'NULL'] and self.lock_pool:
+                    if panda_config.add_serialized and self.job.jediTaskID not in [0, None, 'NULL'] and self.lock_pool:
                         db_lock = self.lock_pool.get(self.job.jediTaskID)
                         if db_lock:
                             db_lock.acquire()
                             self.logger.debug("got DB lock for jediTaskID={}".format(self.job.jediTaskID))
                         else:
                             self.logger.debug("couldn't get DB lock for jediTaskID={}".format(self.job.jediTaskID))
                     self.logger.debug("updating DB")
@@ -651,14 +651,21 @@
         if not tmpStat:
             self.logger.error("failed to copy files for variable number of outputs")
             return 2
         # check files
         lfns_set = set(lfns)
         fileList = []
         for file in self.job.Files:
+            if file.lfn.startswith('regex|'):
+                target = re.sub(r'^[^|]+\|', '', file.lfn)
+                for tmp_lfn in lfns_set:
+                    if re.search(target, tmp_lfn):
+                        file.lfn = tmp_lfn
+                        self.logger.debug(f'use new LFN {tmp_lfn} for {target}')
+                        break
             fileList.append(file.lfn)
             if file.type == 'input':
                 if file.lfn in lfns_set:
                     if self.job.prodSourceLabel in ['user','panda'] or self.job.is_on_site_merging():
                         # skipped file
                         file.status = 'skipped'
                         self.logger.debug(f'skipped input : {file.lfn}')
```

### Comparing `panda-server-0.0.53/pandaserver/dataservice/AdderResult.py` & `panda-server-0.0.54/pandaserver/dataservice/AdderResult.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/dataservice/AdderSimplePlugin.py` & `panda-server-0.0.54/pandaserver/dataservice/AdderSimplePlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/dataservice/Closer.py` & `panda-server-0.0.54/pandaserver/dataservice/Closer.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/dataservice/CloserAtlasPlugin.py` & `panda-server-0.0.54/pandaserver/dataservice/CloserAtlasPlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/dataservice/DDM.py` & `panda-server-0.0.54/pandaserver/dataservice/DDM.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/dataservice/DDMHandler.py` & `panda-server-0.0.54/pandaserver/dataservice/DDMHandler.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/dataservice/DataService.py` & `panda-server-0.0.54/pandaserver/dataservice/DataService.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/dataservice/DataServiceUtils.py` & `panda-server-0.0.54/pandaserver/dataservice/DataServiceUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/dataservice/DynDataDistributer.py` & `panda-server-0.0.54/pandaserver/dataservice/DynDataDistributer.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/dataservice/EventPicker.py` & `panda-server-0.0.54/pandaserver/dataservice/EventPicker.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/dataservice/Finisher.py` & `panda-server-0.0.54/pandaserver/dataservice/Finisher.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/dataservice/Notifier.py` & `panda-server-0.0.54/pandaserver/dataservice/Notifier.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 notifier
 
 '''
 
 import re
 import sys
 import uuid
-import urllib
-import smtplib
 import datetime
 import traceback
 import time
+import smtplib
+
+try:  # Python 2
+    from urllib import urlencode
+except ImportError:  # Python 3
+    from urllib.parse import urlencode
 
 from pandaserver.config import panda_config
 from pandaserver.taskbuffer.OraDBProxy import DBProxy
 from pandacommon.pandalogger.PandaLogger import PandaLogger
 from pandaserver.dataservice.DDM import rucioAPI
 import pandaserver.taskbuffer.ErrorCode
 
@@ -22,42 +26,44 @@
 _logger = PandaLogger().getLogger('Notifier')
 
 # ignored DN
 _ignoreList = [
     'Nurcan Ozturk',
     'Xin Zhao',
     'Dietrich Liko',
-    ]
+]
 
 # NG words in email address
-_ngWordsInMailAddr = ['support','system','stuff','service','secretariat','club','user','admin',
-                      'cvs','grid','librarian','svn','atlas','cms','lhcb','alice','alaelp']
+_ngWordsInMailAddr = ['support', 'system', 'stuff', 'service', 'secretariat', 'club', 'user', 'admin',
+                      'cvs', 'grid', 'librarian', 'svn', 'atlas', 'cms', 'lhcb', 'alice', 'alaelp']
 
 # port for SMTP server
-smtpPortList = [25,587]
+smtpPortList = [25, 587]
+
 
 def initLogger(pLogger):
     # redirect logging to parent as it doesn't work in nested threads
     global _logger
     _logger = pLogger
 
 
 # wrapper to patch smtplib.stderr to send debug info to logger
 class StderrLogger(object):
-    def __init__(self,token):
-        self.token  = token
-    def write(self,message):
+    def __init__(self, token):
+        self.token = token
+
+    def write(self, message):
         message = message.strip()
         if message != '':
-            _logger.debug('%s %s' % (self.token,message))
+            _logger.debug('%s %s' % (self.token, message))
 
 
 class Notifier:
     # constructor
-    def __init__(self,taskBuffer,job,datasets,summary={},mailFile=None,mailFileName=''):
+    def __init__(self, taskBuffer, job, datasets, summary={}, mailFile=None, mailFileName=''):
         self.job = job
         self.datasets = datasets
         self.taskBuffer = taskBuffer
         self.summary = summary
         self.mailFile = mailFile
         self.mailFileName = mailFileName
 
@@ -69,74 +75,75 @@
                 # check job type
                 if self.job.prodSourceLabel != 'user' and self.job.prodSourceLabel != 'panda':
                     _logger.error("Invalid job type : %s" % self.job.prodSourceLabel)
                     _logger.debug("%s end" % self.job.PandaID)
                     return
                 # ignore some DNs to avoid mail storm
                 for igName in _ignoreList:
-                    if re.search(igName,self.job.prodUserID) is not None:
+                    if re.search(igName, self.job.prodUserID) is not None:
                         _logger.debug("Ignore DN : %s" % self.job.prodUserID)
                         _logger.debug("%s end" % self.job.PandaID)
                         return
                 # get e-mail address
                 mailAddr = self.getEmail(self.job.prodUserID)
                 if mailAddr == '':
                     _logger.error("could not find email address for %s" % self.job.prodUserID)
                     _logger.debug("%s end" % self.job.PandaID)
                     return
                 # not send
-                if mailAddr in ['notsend','',None] or (mailAddr is not None and mailAddr.startswith('notsend')):
+                if mailAddr in ['notsend', '', None] or (mailAddr is not None and mailAddr.startswith('notsend')):
                     _logger.debug("not send to %s" % self.job.prodUserID)
                     _logger.debug("%s end" % self.job.PandaID)
                     return
                 # use all datasets
                 if self.summary != {}:
                     self.datasets = []
                     for tmpJobID in self.summary:
                         tmpDsList = self.summary[tmpJobID]
                         if tmpDsList == []:
                             continue
                         self.datasets += tmpDsList
                 # get full jobSpec including metadata
-                self.job = self.taskBuffer.peekJobs([self.job.PandaID],fromDefined=False,
-                                    fromActive=False,fromWaiting=False)[0]
+                self.job = self.taskBuffer.peekJobs([self.job.PandaID], fromDefined=False,
+                                                    fromActive=False, fromWaiting=False)[0]
                 if self.job is None:
                     _logger.error('%s : not found in DB' % self.job.PandaID)
                     _logger.debug("%s end" % self.job.PandaID)
                     return
                 # get IDs
                 ids = []
                 # from active tables
                 tmpIDs = self.taskBuffer.queryPandaIDwithDataset(self.datasets)
                 for tmpID in tmpIDs:
                     if tmpID not in ids:
                         ids.append(tmpID)
                 # from archived table
-                if self.job.jobsetID in [0,'NULL',None]:
-                    tmpIDs = self.taskBuffer.getPandIDsWithIdInArch(self.job.prodUserName,self.job.jobDefinitionID,False)
+                if self.job.jobsetID in [0, 'NULL', None]:
+                    tmpIDs = self.taskBuffer.getPandIDsWithIdInArch(self.job.prodUserName, self.job.jobDefinitionID,
+                                                                    False)
                 else:
-                    tmpIDs = self.taskBuffer.getPandIDsWithIdInArch(self.job.prodUserName,self.job.jobsetID,True)
+                    tmpIDs = self.taskBuffer.getPandIDsWithIdInArch(self.job.prodUserName, self.job.jobsetID, True)
                 for tmpID in tmpIDs:
                     if tmpID not in ids:
                         ids.append(tmpID)
-                _logger.debug("%s IDs: %s" % (self.job.PandaID,ids))
+                _logger.debug("%s IDs: %s" % (self.job.PandaID, ids))
                 if len(ids) != 0:
                     # get jobs
-                    jobs = self.taskBuffer.getFullJobStatus(ids,fromDefined=False,fromActive=False,
-                                                            fromWaiting=False,forAnal=False)
+                    jobs = self.taskBuffer.getFullJobStatus(ids, fromDefined=False, fromActive=False,
+                                                            fromWaiting=False, forAnal=False)
                     # statistics
-                    nTotal     = 0
+                    nTotal = 0
                     nSucceeded = 0
-                    nFailed    = 0
-                    nPartial   = 0
-                    nCancel    = 0
+                    nFailed = 0
+                    nPartial = 0
+                    nCancel = 0
                     # time info
                     creationTime = self.job.creationTime
-                    endTime      = self.job.modificationTime
-                    if isinstance(endTime,datetime.datetime):
+                    endTime = self.job.modificationTime
+                    if isinstance(endTime, datetime.datetime):
                         endTime = endTime.strftime('%Y-%m-%d %H:%M:%S')
                     # datasets
                     iDSList = []
                     oDSList = []
                     siteMap = {}
                     logDS = None
                     for tmpJob in jobs:
@@ -149,24 +156,24 @@
                             else:
                                 if file.dataset not in oDSList:
                                     oDSList.append(file.dataset)
                                 if file.type == 'log':
                                     logDS = file.dataset
                     # job/jobset IDs and site
                     if self.summary == {}:
-                        jobIDsite = "%s/%s" % (self.job.jobDefinitionID,self.job.computingSite)
+                        jobIDsite = "%s/%s" % (self.job.jobDefinitionID, self.job.computingSite)
                         jobsetID = self.job.jobDefinitionID
                         jobDefIDList = [self.job.jobDefinitionID]
                     else:
                         jobDefIDList = list(self.summary)
                         jobDefIDList.sort()
                         jobIDsite = ''
                         tmpIndent = "             "
                         for tmpJobID in jobDefIDList:
-                            jobIDsite += '%s/%s\n%s' % (tmpJobID,siteMap[tmpJobID],tmpIndent)
+                            jobIDsite += '%s/%s\n%s' % (tmpJobID, siteMap[tmpJobID], tmpIndent)
                         remCount = len(tmpIndent) + 1
                         jobIDsite = jobIDsite[:-remCount]
                         jobsetID = self.job.jobsetID
                     # count
                     for job in jobs:
                         if job is None:
                             continue
@@ -191,220 +198,212 @@
                             nFailed += 1
                         elif job.jobStatus == 'cancelled':
                             nCancel += 1
                     # make message
                     if nSucceeded == nTotal:
                         finalStatInSub = "(All Succeeded)"
                     else:
-                        finalStatInSub = "(%s/%s Succeeded)" % (nSucceeded,nTotal)
+                        finalStatInSub = "(%s/%s Succeeded)" % (nSucceeded, nTotal)
                     fromadd = panda_config.emailSender
-                    if self.job.jobsetID in [0,'NULL',None]:
+                    if self.job.jobsetID in [0, 'NULL', None]:
                         message = \
-"""Subject: PANDA notification for JobID : %s  %s
-From: %s
-To: %s
-
-Summary of JobID : %s
-
-Site : %s""" % (self.job.jobDefinitionID,finalStatInSub,fromadd,mailAddr,self.job.jobDefinitionID,self.job.computingSite)
+                            """Subject: PANDA notification for JobID : %s  %s
+                            From: %s
+                            To: %s
+                            
+                            Summary of JobID : %s
+                            
+                            Site : %s""" % (self.job.jobDefinitionID, finalStatInSub, fromadd, mailAddr, self.job.jobDefinitionID,
+                self.job.computingSite)
                     else:
                         message = \
-"""Subject: PANDA notification for JobsetID : %s  %s
-From: %s
-To: %s
-
-Summary of JobsetID : %s
-
-JobID/Site : %s""" % (jobsetID,finalStatInSub,fromadd,mailAddr,jobsetID,jobIDsite)
+                            """Subject: PANDA notification for JobsetID : %s  %s
+                            From: %s
+                            To: %s
+                            
+                            Summary of JobsetID : %s
+                            
+                            JobID/Site : %s""" % (jobsetID, finalStatInSub, fromadd, mailAddr, jobsetID, jobIDsite)
                     message += \
-"""
-
-Created : %s (UTC)
-Ended   : %s (UTC)
-
-Total Number of Jobs : %s
-           Succeeded : %s
-           Partial   : %s
-           Failed    : %s
-           Cancelled : %s
-""" % (creationTime,endTime,nTotal,nSucceeded,nPartial,nFailed,nCancel)
+                        """
+                        
+                        Created : %s (UTC)
+                        Ended   : %s (UTC)
+                        
+                        Total Number of Jobs : %s
+                                   Succeeded : %s
+                                   Partial   : %s
+                                   Failed    : %s
+                                   Cancelled : %s
+                        """ % (creationTime, endTime, nTotal, nSucceeded, nPartial, nFailed, nCancel)
                     # input datasets
                     for iDS in iDSList:
                         message += \
-"""
-In  : %s""" % iDS
+                            """
+                            In  : %s""" % iDS
                     # output datasets
                     for oDS in oDSList:
                         message += \
-"""
-Out : %s""" % oDS
+                            """
+                            Out : %s""" % oDS
                     # command
-                    if self.job.metadata not in ['','NULL',None]:
+                    if self.job.metadata not in ['', 'NULL', None]:
                         message += \
-"""
-
-Parameters : %s""" % self.job.metadata
+                            """
+                            
+                            Parameters : %s""" % self.job.metadata
                     # URLs to PandaMon
-                    if self.job.jobsetID in [0,'NULL',None]:
-                        for tmpIdx,tmpJobID in enumerate(jobDefIDList):
+                    if self.job.jobsetID in [0, 'NULL', None]:
+                        for tmpIdx, tmpJobID in enumerate(jobDefIDList):
                             urlData = {}
                             urlData['job'] = '*'
                             urlData['jobDefinitionID'] = tmpJobID
                             urlData['user'] = self.job.prodUserName
                             urlData['at'] = (str(creationTime)).split()[0]
                             if tmpIdx == 0:
                                 message += \
-"""
-
-PandaMonURL : http://panda.cern.ch/server/pandamon/query?%s""" % urllib.urlencode(urlData)
+                                    """
+                                    
+                                    PandaMonURL : http://panda.cern.ch/server/pandamon/query?%s""" % urlencode(urlData)
                             else:
                                 message += \
-"""
-              http://panda.cern.ch/server/pandamon/query?%s""" % urllib.urlencode(urlData)
+                                    """
+                                                  http://panda.cern.ch/server/pandamon/query?%s""" % urlencode(urlData)
                     else:
                         urlData = {}
                         urlData['job'] = '*'
                         urlData['jobsetID'] = self.job.jobsetID
                         urlData['user'] = self.job.prodUserName
                         urlData['at'] = (str(creationTime)).split()[0]
                         newUrlData = {}
                         newUrlData['jobtype'] = 'analysis'
                         newUrlData['jobsetID'] = self.job.jobsetID
                         newUrlData['prodUserName'] = self.job.prodUserName
                         newUrlData['hours'] = 71
                         message += \
-"""
-
-PandaMonURL : http://panda.cern.ch/server/pandamon/query?%s""" % urllib.urlencode(urlData)
+                            """
+                            
+                            PandaMonURL : http://panda.cern.ch/server/pandamon/query?%s""" % urlencode(urlData)
                         if logDS is not None:
                             message += \
-"""
-TaskMonitorURL : https://dashb-atlas-task.cern.ch/templates/task-analysis/#task=%s""" % logDS
+                                """
+                                TaskMonitorURL : https://dashb-atlas-task.cern.ch/templates/task-analysis/#task=%s""" % logDS
                         message += \
-"""
-NewPandaMonURL : https://pandamon.cern.ch/jobinfo?%s""" % urllib.urlencode(newUrlData)
+                            """
+                            NewPandaMonURL : https://pandamon.cern.ch/jobinfo?%s""" % urlencode(newUrlData)
 
                     # tailer
                     message += \
-"""
-
-
-Report Panda problems of any sort to
-
-  the eGroup for help request
-    hn-atlas-dist-analysis-help@cern.ch
-
-  the Panda JIRA for software bug
-    https://its.cern.ch/jira/browse/ATLASPANDA
-"""
+                        """
+                        
+                        
+                        Report Panda problems of any sort to
+                        
+                          the eGroup for help request
+                            hn-atlas-dist-analysis-help@cern.ch
+                        
+                          the Panda JIRA for software bug
+                            https://its.cern.ch/jira/browse/ATLASPANDA
+                        """
 
                     # send mail
-                    self.sendMail(self.job.PandaID,fromadd,mailAddr,message,1,True)
+                    self.sendMail(self.job.PandaID, fromadd, mailAddr, message, 1, True)
             except Exception:
-                errType,errValue = sys.exc_info()[:2]
-                _logger.error("%s %s %s" % (self.job.PandaID,errType,errValue))
+                errType, errValue = sys.exc_info()[:2]
+                _logger.error("%s %s %s" % (self.job.PandaID, errType, errValue))
             _logger.debug("%s end" % self.job.PandaID)
         else:
             try:
                 _logger.debug("start recovery for %s" % self.mailFileName)
                 # read from file
-                pandaID  = self.mailFile.readline()[:-1]
-                fromadd  = self.mailFile.readline()[:-1]
+                pandaID = self.mailFile.readline()[:-1]
+                fromadd = self.mailFile.readline()[:-1]
                 mailAddr = self.mailFile.readline()[:-1]
-                message  = self.mailFile.read()
+                message = self.mailFile.read()
                 _logger.debug("%s start recovery" % pandaID)
                 if message != '':
-                    self.sendMail(pandaID,fromadd,mailAddr,message,5,False)
+                    self.sendMail(pandaID, fromadd, mailAddr, message, 5, False)
             except Exception:
-                errType,errValue = sys.exc_info()[:2]
-                _logger.error("%s %s %s" % (self.mailFileName,errType,errValue))
+                errType, errValue = sys.exc_info()[:2]
+                _logger.error("%s %s %s" % (self.mailFileName, errType, errValue))
             _logger.debug("end recovery for %s" % self.mailFileName)
 
-
     # send mail
-    def sendMail(self,pandaID,fromadd,mailAddr,message,nTry,fileBackUp):
-        _logger.debug("%s send to %s\n%s" % (pandaID,mailAddr,message))
+    def sendMail(self, pandaID, fromadd, mailAddr, message, nTry, fileBackUp):
+        _logger.debug("%s send to %s\n%s" % (pandaID, mailAddr, message))
         for iTry in range(nTry):
             try:
-                org_smtpstderr = smtplib.stderr
-                smtplib.stderr = StderrLogger(pandaID)
                 smtpPort = smtpPortList[iTry % len(smtpPortList)]
-                server = smtplib.SMTP(panda_config.emailSMTPsrv,smtpPort)
+                server = smtplib.SMTP(panda_config.emailSMTPsrv, smtpPort)
                 server.set_debuglevel(1)
                 server.ehlo()
                 server.starttls()
-                #server.login(panda_config.emailLogin,panda_config.emailPass)
-                out = server.sendmail(fromadd,mailAddr,message)
-                _logger.debug('%s %s' % (pandaID,str(out)))
+                # server.login(panda_config.emailLogin,panda_config.emailPass)
+                out = server.sendmail(fromadd, mailAddr, message)
+                _logger.debug('%s %s' % (pandaID, str(out)))
                 server.quit()
                 break
             except Exception:
-                errType,errValue = sys.exc_info()[:2]
-                if iTry+1 < nTry:
+                errType, errValue = sys.exc_info()[:2]
+                if iTry + 1 < nTry:
                     # sleep for retry
-                    _logger.debug("%s sleep %s due to %s %s" % (pandaID,iTry,errType,errValue))
+                    _logger.debug("%s sleep %s due to %s %s" % (pandaID, iTry, errType, errValue))
                     time.sleep(30)
                 else:
-                    _logger.error("%s %s %s" % (pandaID,errType,errValue))
+                    _logger.error("%s %s %s" % (pandaID, errType, errValue))
                     if fileBackUp:
                         # write to file which is processed in add.py
-                        mailFile = '%s/mail_%s_%s' % (panda_config.logdir,self.job.PandaID,str(uuid.uuid4()))
-                        oMail = open(mailFile,"w")
-                        oMail.write(str(self.job.PandaID)+'\n'+fromadd+'\n'+mailAddr+'\n'+message)
+                        mailFile = '%s/mail_%s_%s' % (panda_config.logdir, self.job.PandaID, str(uuid.uuid4()))
+                        oMail = open(mailFile, "w")
+                        oMail.write(str(self.job.PandaID) + '\n' + fromadd + '\n' + mailAddr + '\n' + message)
                         oMail.close()
-        try:
-            smtplib.stderr = org_smtpstderr
-        except Exception:
-            pass
-
-
 
     # get email
     def getEmail(self, dn):
         # get DN
         _logger.debug("getDN for %s" % dn)
         dbProxy = DBProxy()
         distinguishedName = dbProxy.cleanUserID(dn)
         _logger.debug("DN = %s" % distinguishedName)
         if distinguishedName == "":
             _logger.error("cannot get DN for %s" % dn)
             return ""
         # get email from MetaDB
-        mailAddrInDB,dbUptime = self.taskBuffer.getEmailAddr(distinguishedName,withUpTime=True)
+        mailAddrInDB, dbUptime = self.taskBuffer.getEmailAddr(distinguishedName, withUpTime=True)
         _logger.debug("email in MetaDB : '%s'" % mailAddrInDB)
         notSendMail = False
-        if mailAddrInDB not in [None,'']:
+        if mailAddrInDB not in [None, '']:
             # email mortification is suppressed
             if mailAddrInDB.split(':')[0] == 'notsend':
                 notSendMail = True
         # avoid too frequently lookup
-        if dbUptime is not None and datetime.datetime.utcnow()-dbUptime < datetime.timedelta(hours=1):
+        if dbUptime is not None and datetime.datetime.utcnow() - dbUptime < datetime.timedelta(hours=1):
             _logger.debug("no lookup")
-            if notSendMail or mailAddrInDB in [None,'']:
+            if notSendMail or mailAddrInDB in [None, '']:
                 return 'notsend'
             else:
                 return mailAddrInDB.split(':')[-1]
         # get email from DQ2
         try:
-            tmpStatus,userInfo = rucioAPI.finger(dn)
+            tmpStatus, userInfo = rucioAPI.finger(dn)
             if tmpStatus:
                 mailAddr = userInfo['email']
                 _logger.debug("email from DDM : '%s'" % mailAddr)
             else:
                 mailAddr = None
                 _logger.error("failed to get email from DDM : {}".format(userInfo))
             if mailAddr is None:
                 mailAddr = ''
             # make email field to update DB
             mailAddrToDB = ''
             if notSendMail:
                 mailAddrToDB += 'notsend:'
             mailAddrToDB += mailAddr
             # update database
-            _logger.debug("update email for %s to %s" % (distinguishedName,mailAddrToDB))
-            self.taskBuffer.setEmailAddr(distinguishedName,mailAddrToDB)
+            _logger.debug("update email for %s to %s" % (distinguishedName, mailAddrToDB))
+            self.taskBuffer.setEmailAddr(distinguishedName, mailAddrToDB)
             if notSendMail:
                 return 'notsend'
             return mailAddr
         except Exception as e:
             _logger.error("getEmail failed with {} {}".format(str(e), traceback.format_exc()))
         return ""
```

### Comparing `panda-server-0.0.53/pandaserver/dataservice/ProcessLimiter.py` & `panda-server-0.0.54/pandaserver/dataservice/ProcessLimiter.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/dataservice/RecoverLostFilesCore.py` & `panda-server-0.0.54/pandaserver/dataservice/RecoverLostFilesCore.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/dataservice/Setupper.py` & `panda-server-0.0.54/pandaserver/dataservice/Setupper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/dataservice/SetupperAtlasPlugin.py` & `panda-server-0.0.54/pandaserver/dataservice/SetupperAtlasPlugin.py`

 * *Files identical despite different names*

```diff
@@ -217,15 +217,15 @@
         useZipToPinMap = dict()
         # extract prodDBlock
         for job in self.jobs:
             # ignore failed jobs
             if job.jobStatus in ['failed','cancelled'] or job.isCancelled():
                 continue
             # production datablock
-            if job.prodDBlock != 'NULL' and (not self.pandaDDM) and (job.prodSourceLabel not in ['user','panda']):
+            if job.prodDBlock != 'NULL' and job.prodDBlock and (job.prodSourceLabel not in ['user','panda']):
                 # get VUID and record prodDBlock into DB
                 if job.prodDBlock not in prodError:
                     self.logger.debug('listDatasets '+job.prodDBlock)
                     prodError[job.prodDBlock] = ''
                     for iDDMTry in range(3):
                         newOut,errMsg = rucioAPI.listDatasets(job.prodDBlock)
                         if newOut is None:
```

### Comparing `panda-server-0.0.53/pandaserver/dataservice/SetupperDummyPlugin.py` & `panda-server-0.0.54/pandaserver/dataservice/SetupperDummyPlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/dataservice/SetupperPluginBase.py` & `panda-server-0.0.54/pandaserver/dataservice/SetupperPluginBase.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/dataservice/eventLookupClientEI.py` & `panda-server-0.0.54/pandaserver/dataservice/eventLookupClientEI.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/dataservice/forkSetupper.py` & `panda-server-0.0.54/pandaserver/dataservice/forkSetupper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/jobdispatcher/DispatcherUtils.py` & `panda-server-0.0.54/pandaserver/jobdispatcher/DispatcherUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/jobdispatcher/JobDispatcher.py` & `panda-server-0.0.54/pandaserver/jobdispatcher/JobDispatcher.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/jobdispatcher/Protocol.py` & `panda-server-0.0.54/pandaserver/jobdispatcher/Protocol.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/jobdispatcher/Watcher.py` & `panda-server-0.0.54/pandaserver/jobdispatcher/Watcher.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/proxycache/DBMSql.py` & `panda-server-0.0.54/pandaserver/proxycache/DBMSql.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/proxycache/panda_activeusers_query.py` & `panda-server-0.0.54/pandaserver/proxycache/panda_activeusers_query.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/proxycache/panda_proxy_cache.py` & `panda-server-0.0.54/pandaserver/proxycache/panda_proxy_cache.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/server/panda.py` & `panda-server-0.0.54/pandaserver/server/panda.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
      pauseTask, resumeTask, increaseAttemptNrPanda, killUnfinishedJobs, changeTaskSplitRulePanda,\
      changeTaskModTimePanda, avalancheTask, getPandaIDsWithTaskID, reactivateTask, getTaskStatus, \
      reassignShare, listTasksInShare, getTaskParamsMap, updateWorkers, harvesterIsAlive,\
      reportWorkerStats, reportWorkerStats_jobtype, addHarvesterDialogs, \
      getJobStatisticsPerSiteResource, setNumSlotsForWP, reloadInput, enableJumboJobs, updateServiceMetrics, \
      getUserJobMetadata, getJumboJobDatasets, getGShareStatus,\
      sweepPQ,get_job_statistics_per_site_label_resource, relay_idds_command, send_command_to_job,\
-     execute_idds_workflow_command, set_user_secret, get_user_secrets, get_ban_users
+     execute_idds_workflow_command, set_user_secret, get_user_secrets, get_ban_users, get_files_in_datasets
 
 from pandaserver.userinterface import Client
 
 # import error
 import pandaserver.taskbuffer.ErrorCode
 
 
@@ -112,15 +112,15 @@
                    'getPandaIDsWithTaskID', 'reactivateTask', 'getTaskStatus',
                    'reassignShare', 'listTasksInShare', 'getTaskParamsMap', 'updateWorkers', 'harvesterIsAlive',
                    'reportWorkerStats', 'reportWorkerStats_jobtype', 'addHarvesterDialogs',
                    'getJobStatisticsPerSiteResource', 'setNumSlotsForWP', 'reloadInput', 'enableJumboJobs',
                    'updateServiceMetrics', 'getUserJobMetadata', 'getJumboJobDatasets',
                    'getGShareStatus', 'sweepPQ', 'get_job_statistics_per_site_label_resource', 'relay_idds_command',
                    'send_command_to_job','execute_idds_workflow_command', 'set_user_secret', 'get_user_secrets',
-                   'get_ban_users']
+                   'get_ban_users', 'get_files_in_datasets']
 
 
 # FastCGI/WSGI entry
 if panda_config.useFastCGI or panda_config.useWSGI:
 
     import os
     import cgi
```

### Comparing `panda-server-0.0.53/pandaserver/srvcore/CoreUtils.py` & `panda-server-0.0.54/pandaserver/srvcore/CoreUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/srvcore/MailUtils.py` & `panda-server-0.0.54/pandaserver/srvcore/MailUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/srvcore/oidc_utils.py` & `panda-server-0.0.54/pandaserver/srvcore/oidc_utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/srvcore/srv_msg_utils.py` & `panda-server-0.0.54/pandaserver/srvcore/srv_msg_utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/CloudSpec.py` & `panda-server-0.0.54/pandaserver/taskbuffer/CloudSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/CloudTaskSpec.py` & `panda-server-0.0.54/pandaserver/taskbuffer/CloudTaskSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/ConBridge.py` & `panda-server-0.0.54/pandaserver/taskbuffer/ConBridge.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/DBProxyPool.py` & `panda-server-0.0.54/pandaserver/taskbuffer/DBProxyPool.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/DatasetSpec.py` & `panda-server-0.0.54/pandaserver/taskbuffer/DatasetSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/DdmSpec.py` & `panda-server-0.0.54/pandaserver/taskbuffer/DdmSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/EiDBProxy.py` & `panda-server-0.0.54/pandaserver/taskbuffer/EiDBProxy.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/ErrorCode.py` & `panda-server-0.0.54/pandaserver/taskbuffer/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/EventServiceUtils.py` & `panda-server-0.0.54/pandaserver/taskbuffer/EventServiceUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/FileSpec.py` & `panda-server-0.0.54/pandaserver/taskbuffer/FileSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/GlobalShares.py` & `panda-server-0.0.54/pandaserver/taskbuffer/GlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/HarvesterMetricsSpec.py` & `panda-server-0.0.54/pandaserver/taskbuffer/HarvesterMetricsSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/Initializer.py` & `panda-server-0.0.54/pandaserver/taskbuffer/Initializer.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/JobSpec.py` & `panda-server-0.0.54/pandaserver/taskbuffer/JobSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/JobUtils.py` & `panda-server-0.0.54/pandaserver/taskbuffer/JobUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/NucleusSpec.py` & `panda-server-0.0.54/pandaserver/taskbuffer/NucleusSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/OraDBProxy.py` & `panda-server-0.0.54/pandaserver/taskbuffer/OraDBProxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -3842,15 +3842,15 @@
                 sqlRR += "WHERE jediTaskID=:jediTaskID AND datasetID=:datasetID AND fileID=:fileID AND status=:eventStatus "
                 # sql to read log backet IDs
                 sqlLBK  = "SELECT jobMetrics FROM ATLAS_PANDA.jobsArchived4 WHERE PandaID=:PandaID "
                 sqlLBK += "UNION "
                 sqlLBK += "SELECT jobMetrics FROM ATLAS_PANDAARCH.jobsArchived WHERE PandaID=:PandaID AND modificationTime>(CURRENT_DATE-30) "
                 # read files
                 sqlFile = "SELECT %s FROM ATLAS_PANDA.filesTable4 " % FileSpec.columnNames()
-                sqlFile+= "WHERE PandaID=:PandaID "
+                sqlFile+= "WHERE PandaID=:PandaID ORDER BY row_ID "
                 # read LFN and dataset name for output files
                 sqlFileOut = "SELECT lfn,dataset FROM ATLAS_PANDA.filesTable4 "
                 sqlFileOut+= "WHERE PandaID=:PandaID AND type=:type "
                 # read files from JEDI for jumbo jobs
                 sqlFileJEDI  = "SELECT lfn,GUID,fsize,checksum "
                 sqlFileJEDI += "FROM {0}.JEDI_Dataset_Contents ".format(panda_config.schemaJEDI)
                 sqlFileJEDI += "WHERE jediTaskID=:jediTaskID AND datasetID=:datasetID "
@@ -20682,14 +20682,33 @@
         Re-loads the shares, then returns the leaves sorted by under usage
         """
         self.__reload_shares()
         self.__reload_hs_distribution()
         return self.tree.sort_branch_by_current_hs_distribution(self.__hs_distribution)
 
 
+    def get_tree_of_gshare_names(self):
+        """
+        get nested dict of gshare names implying the tree structure
+        """
+        def get_nested_gshare(share):
+            val = None
+            if not share.children:
+                # leaf
+                pass
+            else:
+                # branch
+                val = {}
+                for child in share.children:
+                    val[child.name] = get_nested_gshare(child)
+            return val
+        ret_dict = get_nested_gshare(self.tree)
+        return ret_dict
+
+
     def __load_branch(self, share):
         """
         Recursively load a branch
         """
         node = GlobalShares.Share(share.name, share.value, share.parent, share.prodsourcelabel, share.workinggroup,
                                   share.campaign, share.processingtype, share.transpath, share.rtype, share.vo,
                                   share.queue_id, share.throttled)
@@ -23442,16 +23461,17 @@
         self.__reload_shares()
         self.__reload_hs_distribution()
         sorted_shares = self.tree.sort_branch_by_current_hs_distribution(self.__hs_distribution)
 
         sorted_shares_export = []
         for share in sorted_shares:
             sorted_shares_export.append({'name': share.name,
-                                         'running': self.__hs_distribution[share.name]['executing'],
-                                         'target': self.__hs_distribution[share.name]['pledged']})
+                                         'running': self.__hs_distribution[share.name]['executing'], 
+                                         'target': self.__hs_distribution[share.name]['pledged'], 
+                                         'queuing': self.__hs_distribution[share.name]['queued']})
         return sorted_shares_export
 
 
 
     # get output datasets
     def getOutputDatasetsJEDI(self, panda_id):
         comment = ' /* DBProxy.getOutputDatasetsJEDI */'
@@ -25322,7 +25342,61 @@
             n_remain, = self.cur.fetchone()
             tmpLog.debug("done={} release/remain={}/{}".format(n_done, n_release, n_remain))
             return n_done, n_remain
         except Exception:
             # error
             self.dumpErrorMessage(_logger, methodName)
             raise RuntimeError(methodName + ' failed')
+
+    # get LFNs in datasets
+    def get_files_in_datasets(self, task_id, dataset_types):
+        comment = ' /* DBProxy.get_lfns_in_datasets */'
+        method_name = comment.split(' ')[-2].split('.')[-1]
+        method_name += '< jediTaskID={0} >'.format(task_id)
+        tmp_log = LogWrapper(_logger, method_name)
+        tmp_log.debug("start")
+        try:
+            varMap = {}
+            varMap[':jediTaskID'] = task_id
+            sqlD = "SELECT datasetName,datasetID FROM {}.JEDI_Datasets "\
+                   "WHERE jediTaskID=:jediTaskID AND type IN (".format(panda_config.schemaJEDI)
+            for tmp_type in dataset_types.split(','):
+                sqlD += ':{},'.format(tmp_type)
+                varMap[':{}'.format(tmp_type)] = tmp_type
+            sqlD = sqlD[:-1]
+            sqlD += ') '
+            sqlS = "SELECT lfn,scope,fileID,status FROM {}.JEDI_Dataset_Contents ".format(panda_config.schemaJEDI)
+            sqlS += "WHERE jediTaskID=:jediTaskID AND datasetID=:datasetID ORDER BY fileID "
+            retVal = []
+            # start transaction
+            self.conn.begin()
+            self.cur.execute(sqlD + comment, varMap)
+            res = self.cur.fetchall()
+            for datasetName, datasetID in res:
+                datasetDict = {}
+                datasetDict['name'] = datasetName
+                datasetDict['id'] = datasetID
+                # read files
+                varMap = {}
+                varMap[':jediTaskID'] = task_id
+                varMap[':datasetID'] = datasetID
+                self.cur.execute(sqlS + comment, varMap)
+                resF = self.cur.fetchall()
+                fileList = []
+                for lfn, fileScope, fileID, status in resF:
+                    fileDict = {'lfn': lfn,
+                                'scope': fileScope,
+                                'id': fileID,
+                                'status': status}
+                    fileList.append(fileDict)
+                retVal.append({'dataset': datasetDict, 'files': fileList})
+            # commit
+            if not self._commit():
+                raise RuntimeError('Commit error')
+            tmp_log.debug("done")
+            return retVal
+        except Exception:
+            # roll back
+            self._rollback()
+            # error
+            self.dumpErrorMessage(_logger, method_name)
+            return None
```

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/PrioUtil.py` & `panda-server-0.0.54/pandaserver/taskbuffer/PrioUtil.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/ProcessGroups.py` & `panda-server-0.0.54/pandaserver/taskbuffer/ProcessGroups.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/ResourceSpec.py` & `panda-server-0.0.54/pandaserver/taskbuffer/ResourceSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/SQLDumper.py` & `panda-server-0.0.54/pandaserver/taskbuffer/SQLDumper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/SiteSpec.py` & `panda-server-0.0.54/pandaserver/taskbuffer/SiteSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/TaskBuffer.py` & `panda-server-0.0.54/pandaserver/taskbuffer/TaskBuffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -3330,14 +3330,26 @@
         res = proxy.getEventStat(jediTaskID, PandaID)
         # release DB proxy
         self.proxyPool.putProxy(proxy)
         # return
         return res
 
 
+    # get nested dict of gshare names implying the tree structure
+    def get_tree_of_gshare_names(self):
+        # get DB proxy
+        proxy = self.proxyPool.getProxy()
+        # exec
+        res = proxy.get_tree_of_gshare_names()
+        # release DB proxy
+        self.proxyPool.putProxy(proxy)
+        # return
+        return res
+
+
     # get the HS06 distribution for global shares
     def get_hs_distribution(self):
         # get DB proxy
         proxy = self.proxyPool.getProxy()
         # exec
         res = proxy.get_hs_distribution()
         # release DB proxy
@@ -4161,10 +4173,15 @@
 
     def carbon_aggregate_emissions(self):
         proxy = self.proxyPool.getProxy()
         ret = proxy.carbon_aggregate_emissions()
         self.proxyPool.putProxy(proxy)
         return ret
 
+    def get_files_in_datasets(self, task_id, dataset_types):
+        proxy = self.proxyPool.getProxy()
+        ret = proxy.get_files_in_datasets(task_id, dataset_types)
+        self.proxyPool.putProxy(proxy)
+        return ret
 
 # Singleton
 taskBuffer = TaskBuffer()
```

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/TaskBufferInterface.py` & `panda-server-0.0.54/pandaserver/taskbuffer/TaskBufferInterface.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/Utils.py` & `panda-server-0.0.54/pandaserver/taskbuffer/Utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/WorkerSpec.py` & `panda-server-0.0.54/pandaserver/taskbuffer/WorkerSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/WrappedCursor.py` & `panda-server-0.0.54/pandaserver/taskbuffer/WrappedCursor.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/WrappedPickle.py` & `panda-server-0.0.54/pandaserver/taskbuffer/WrappedPickle.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/retryModule.py` & `panda-server-0.0.54/pandaserver/taskbuffer/retryModule.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
     - limit the number of retries
     - increase the memory of a job if it failed because of insufficient memory
     """
     _logger.debug("Entered apply_retrial_rules for PandaID=%s, errors=%s, attemptNr=%s"
                   % (jobID, errors, attemptNr))
 
     retrial_rules = task_buffer.getRetrialRules()
-    _logger.debug("Back from getRetrialRules: %s" % retrial_rules)
+    _logger.debug("Back from getRetrialRules")
     if not retrial_rules:
         return
 
     try:
         job = task_buffer.peekJobs([jobID], fromDefined=False, fromArchived=True, fromWaiting=False)[0]
         acted_on_job = False
         for error in errors:
```

### Comparing `panda-server-0.0.53/pandaserver/taskbuffer/workflow_processor.py` & `panda-server-0.0.54/pandaserver/taskbuffer/workflow_processor.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/SchemaChecker.py` & `panda-server-0.0.54/pandaserver/test/SchemaChecker.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/alice/titan_testScript_ec2_alice_1.py` & `panda-server-0.0.54/pandaserver/test/alice/titan_testScript_ec2_alice_1.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/alice/titan_testScript_ec2_alice_2.py` & `panda-server-0.0.54/pandaserver/test/alice/titan_testScript_ec2_alice_2.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/banUser.py` & `panda-server-0.0.54/pandaserver/test/banUser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/boostPrio.py` & `panda-server-0.0.54/pandaserver/test/boostPrio.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/boostUser.py` & `panda-server-0.0.54/pandaserver/test/boostUser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/callbackDDM.py` & `panda-server-0.0.54/pandaserver/test/callbackDDM.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/finishJob.py` & `panda-server-0.0.54/pandaserver/test/finishJob.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/frontier_retagging.py` & `panda-server-0.0.54/pandaserver/test/frontier_retagging.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/getJobs.py` & `panda-server-0.0.54/pandaserver/test/getJobs.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/killJob.py` & `panda-server-0.0.54/pandaserver/test/killJob.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/killJobLowPrio.py` & `panda-server-0.0.54/pandaserver/test/killJobLowPrio.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/killJobsInTask.py` & `panda-server-0.0.54/pandaserver/test/killJobsInTask.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/killProdJobs.py` & `panda-server-0.0.54/pandaserver/test/killProdJobs.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/killTask.py` & `panda-server-0.0.54/pandaserver/test/killTask.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/killUser.py` & `panda-server-0.0.54/pandaserver/test/killUser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/lsst/lsstSubmit.py` & `panda-server-0.0.54/pandaserver/test/lsst/lsstSubmit.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/lsst/lsstSubmitMERGEtest.py` & `panda-server-0.0.54/pandaserver/test/lsst/lsstSubmitMERGEtest.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/lsst/lsstSubmitPhosim332.py` & `panda-server-0.0.54/pandaserver/test/lsst/lsstSubmitPhosim332.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/reassignSite.py` & `panda-server-0.0.54/pandaserver/test/reassignSite.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/reassignTask.py` & `panda-server-0.0.54/pandaserver/test/reassignTask.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/reassignWaiting.py` & `panda-server-0.0.54/pandaserver/test/reassignWaiting.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/reloadInputDS.py` & `panda-server-0.0.54/pandaserver/test/reloadInputDS.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/sendCommandToJob.py` & `panda-server-0.0.54/pandaserver/test/sendCommandToJob.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/setDebugMode.py` & `panda-server-0.0.54/pandaserver/test/setDebugMode.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/setPriority.py` & `panda-server-0.0.54/pandaserver/test/setPriority.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/testEvgen.py` & `panda-server-0.0.54/pandaserver/test/testEvgen.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/testEvgen17.py` & `panda-server-0.0.54/pandaserver/test/testEvgen17.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/testG4sim.py` & `panda-server-0.0.54/pandaserver/test/testG4sim.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/testG4sim17.py` & `panda-server-0.0.54/pandaserver/test/testG4sim17.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/testGetCriteriaForGlobalShares.py` & `panda-server-0.0.54/pandaserver/test/testGetCriteriaForGlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/testGlobalShares.py` & `panda-server-0.0.54/pandaserver/test/testGlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/testJobFlowATLAS.py` & `panda-server-0.0.54/pandaserver/test/testJobFlowATLAS.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/testReco.py` & `panda-server-0.0.54/pandaserver/test/testReco.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/testSimulReco14.py` & `panda-server-0.0.54/pandaserver/test/testSimulReco14.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/testSiteMap.py` & `panda-server-0.0.54/pandaserver/test/testSiteMap.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/test/testutils.py` & `panda-server-0.0.54/pandaserver/test/testutils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/userinterface/Client.py` & `panda-server-0.0.54/pandaserver/userinterface/Client.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/userinterface/UserIF.py` & `panda-server-0.0.54/pandaserver/userinterface/UserIF.py`

 * *Files 1% similar despite different names*

```diff
@@ -1025,14 +1025,19 @@
 
     # get user secrets
     def get_user_secrets(self, owner, keys, get_json):
         ret = self.taskBuffer.get_user_secrets(owner, keys, get_json)
         # return
         return ret
 
+    # get files in datasets
+    def get_files_in_datasets(self, task_id, dataset_types):
+        ret = self.taskBuffer.get_files_in_datasets(task_id, dataset_types)
+        # return
+        return ret
 
 # Singleton
 userIF = UserIF()
 del UserIF
 
 
 # get FQANs
@@ -2752,7 +2757,15 @@
         get_json = False
     if not dn:
         tmpMsg = 'SSL_CLIENT_S_DN is missing in HTTP request'
         tmpLog.error(tmpMsg)
         return json.dumps((False, tmpMsg))
     owner = clean_user_id(dn)
     return json.dumps(userIF.get_user_secrets(owner, keys, get_json))
+
+
+# get files in datasets
+def get_files_in_datasets(req, task_id, dataset_types='input,pseudo_input'):
+    # check security
+    if not isSecure(req):
+        return json.dumps((False,"SSL is required"))
+    return json.dumps(userIF.get_files_in_datasets(task_id, dataset_types))
```

### Comparing `panda-server-0.0.53/pandaserver/workflow/pcwl_test.py` & `panda-server-0.0.54/pandaserver/workflow/pcwl_test.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/workflow/pcwl_utils.py` & `panda-server-0.0.54/pandaserver/workflow/pcwl_utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/workflow/psnakemake_test.py` & `panda-server-0.0.54/pandaserver/workflow/psnakemake_test.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/workflow/snakeparser/extensions.py` & `panda-server-0.0.54/pandaserver/workflow/snakeparser/extensions.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/workflow/snakeparser/log.py` & `panda-server-0.0.54/pandaserver/workflow/snakeparser/log.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/workflow/snakeparser/parser.py` & `panda-server-0.0.54/pandaserver/workflow/snakeparser/parser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/workflow/snakeparser/utils.py` & `panda-server-0.0.54/pandaserver/workflow/snakeparser/utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/pandaserver/workflow/workflow_utils.py` & `panda-server-0.0.54/pandaserver/workflow/workflow_utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/setup.py` & `panda-server-0.0.54/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -235,15 +235,15 @@
     long_description='''This package contains PanDA Server Components''',
     license='GPL',
     author='Panda Team',
     author_email='atlas-adc-panda@cern.ch',
     url='https://twiki.cern.ch/twiki/bin/view/Atlas/PanDA',
     zip_safe=False,
     install_requires=['panda-common>=0.0.34',
-                      'panda-client',
+                      'panda-client-light',
                       'pyOpenSSL',
                       'python-daemon',
                       'mod_wsgi',
                       'six',
                       'sqlalchemy',
                       'stomp.py',
                       'pyyaml',
@@ -289,47 +289,32 @@
               ],
     package_data = {'pandaserver.server': ['.gacl']},
     data_files=[
                 # config files
                 ('etc/panda', ['templates/panda_server-httpd.conf.rpmnew.template',
                                'templates/panda_server-httpd-FastCGI.conf.rpmnew.template',
                                'templates/panda_server.cfg.rpmnew.template',
-                               'templates/pandasrv.cron.template',
                                'templates/logrotate.d/panda_server.logrotate.template',
-                               'templates/sysconfig/panda_server.sysconfig.rpmnew.template'
+                               'templates/sysconfig/panda_server.sysconfig.rpmnew.template',
+                               'templates/sysconfig/panda_server_env.systemd.rpmnew.template'
                                ]
                  ),
 
-                # init script
+                # init scripts for chkconfig -- these become obsolete in ALMA9
                 ('etc/rc.d/init.d', ['templates/init.d/panda_server.exe.template',
                                      'templates/init.d/panda_httpd.exe.template',
                                      'templates/init.d/panda_daemon.exe.template',
                                    ]
                  ),
-                # crons
-                ('usr/bin', ['templates/panda_server-add_main.exe.template',
-                             'templates/panda_server-add_sub.exe.template',
-                             'templates/panda_server-priority.exe.template',
-                             'templates/panda_server-copyArchive.exe.template',
-                             'templates/panda_server-vomsrenew.exe.template',
-                             'templates/panda_server-tmpwatch.exe.template',
-                             'templates/panda_server-datasetManager.exe.template',
-                             'templates/panda_server-evpPD2P.exe.template',
-                             'templates/panda_server-callback.exe.template',
-                             'templates/panda_server-makeSlsXml.exe.template',
-                             'templates/panda_server-boostUser.exe.template',
-                             'templates/panda_server-proxyCache.exe.template',
-                             'templates/panda_server-configurator.exe.template',
-                             'templates/panda_server-network_configurator.exe.template',
-                             'templates/panda_server-schedconfig_json.exe.template',
-                             'templates/panda_server-sw_tags.exe.template',
-                             'templates/panda_server-esPreemption.exe.template',
-                             'templates/panda_server-pilot_streaming.exe.template',
-                             'templates/panda_server-frontier_retagging.exe.template'
-                             ]
+
+                # service unit files for systemd -- these are to be used in ALMA9
+                ('etc/systemd/system', ['templates/systemd/panda.service.template',
+                                         'templates/init.d/panda_httpd.exe.template',
+                                         'templates/init.d/panda_daemon.exe.template',
+                                        ]
                  ),
 
                 # var dirs
                 #('var/log/panda', []),
                 #('var/cache/pandaserver', []),
                 ],
     cmdclass={'install': install_panda,
```

### Comparing `panda-server-0.0.53/templates/conda_meta.yaml.template` & `panda-server-0.0.54/templates/conda_meta.yaml.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/templates/init.d/panda_daemon.exe.template` & `panda-server-0.0.54/templates/init.d/panda_daemon.exe.template`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
   if [ -f $LOCKFILE ]; then
     echo "ERROR: PanDA Daemon is already running with lockfile:$LOCKFILE"
   else
     echo "start PanDA Daemon"
     for itry in `seq 1 5`
     do
       echo "trying $itry"
-      $PROGNAME --pid $PIDFILE >> $LOGSTDOUT 2>> $LOGSTDERR
+      $PROGNAME --pidfile $PIDFILE >> $LOGSTDOUT 2>> $LOGSTDERR
       touch $LOCKFILE
       sleep 5
       ps -p `cat $PIDFILE` > /dev/null
       ERROR=$?
       if [ $ERROR -eq 0 ]; then
     		echo "succeeded"
     		break
```

### Comparing `panda-server-0.0.53/templates/init.d/panda_httpd.exe.template` & `panda-server-0.0.54/templates/init.d/panda_httpd.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/templates/init.d/panda_server.exe.template` & `panda-server-0.0.54/templates/init.d/panda_server.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/templates/logrotate.d/panda_server.logrotate.template` & `panda-server-0.0.54/templates/logrotate.d/panda_server.logrotate.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/templates/panda_server-httpd-FastCGI.conf.rpmnew.template` & `panda-server-0.0.54/templates/panda_server-httpd-FastCGI.conf.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/templates/panda_server-httpd.conf.rpmnew.template` & `panda-server-0.0.54/templates/panda_server-httpd.conf.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/templates/panda_server-makeSlsXml.exe.template` & `panda-server-0.0.54/templates/panda_server-makeSlsXml.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/templates/panda_server-vomsrenew.exe.template` & `panda-server-0.0.54/templates/panda_server-vomsrenew.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/templates/panda_server.cfg.rpmnew.template` & `panda-server-0.0.54/templates/panda_server.cfg.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.53/templates/sysconfig/panda_server.sysconfig.rpmnew.template` & `panda-server-0.0.54/templates/sysconfig/panda_server.sysconfig.rpmnew.template`

 * *Files identical despite different names*

