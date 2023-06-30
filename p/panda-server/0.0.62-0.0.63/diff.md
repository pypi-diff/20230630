# Comparing `tmp/panda-server-0.0.62.tar.gz` & `tmp/panda-server-0.0.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda-server-0.0.62.tar", last modified: Fri Jun 30 04:36:09 2023, max compression
+gzip compressed data, was "panda-server-0.0.63.tar", last modified: Fri Jun 30 17:47:25 2023, max compression
```

## Comparing `panda-server-0.0.62.tar` & `panda-server-0.0.63.tar`

### file list

```diff
@@ -1,224 +1,224 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.492573 panda-server-0.0.62/
--rw-r--r--   0 runner    (1001) docker     (123)    81051 2023-06-30 04:35:59.000000 panda-server-0.0.62/ChangeLog.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-30 04:35:59.000000 panda-server-0.0.62/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-30 04:35:59.000000 panda-server-0.0.62/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-30 04:36:09.492573 panda-server-0.0.62/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 04:35:59.000000 panda-server-0.0.62/PandaPkgInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-30 04:35:59.000000 panda-server-0.0.62/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.468573 panda-server-0.0.62/panda_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-30 04:36:09.000000 panda-server-0.0.62/panda_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-06-30 04:36:09.000000 panda-server-0.0.62/panda_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 04:36:09.000000 panda-server-0.0.62/panda_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 04:36:09.000000 panda-server-0.0.62/panda_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-30 04:36:09.000000 panda-server-0.0.62/panda_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-30 04:36:09.000000 panda-server-0.0.62/panda_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.468573 panda-server-0.0.62/pandaserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.468573 panda-server-0.0.62/pandaserver/brokerage/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/brokerage/ErrorCode.py
--rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/brokerage/SiteMapper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/brokerage/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    80940 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/brokerage/broker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.468573 panda-server-0.0.62/pandaserver/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/config/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/config/daemon_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7167 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/config/panda_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.468573 panda-server-0.0.62/pandaserver/configurator/
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/configurator/Carbon.py
--rw-r--r--   0 runner    (1001) docker     (123)    35264 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/configurator/Configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/configurator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/configurator/aux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.468573 panda-server-0.0.62/pandaserver/daemons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/daemons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/daemons/master.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/daemons/master_systemd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.472573 panda-server-0.0.62/pandaserver/daemons/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/daemons/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/daemons/scripts/add_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/daemons/scripts/add_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/daemons/scripts/carbon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/daemons/scripts/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)    64166 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/daemons/scripts/copyArchive.py
--rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/daemons/scripts/datasetManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/daemons/scripts/dummy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/daemons/scripts/evpPD2P.py
--rw-r--r--   0 runner    (1001) docker     (123)    41977 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/daemons/scripts/metric_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/daemons/scripts/panda_activeusers_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/daemons/scripts/pilotStreaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/daemons/scripts/process_workflow_files_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/daemons/scripts/recover_lost_files_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)    15682 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/daemons/scripts/task_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/daemons/scripts/tmpwatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/daemons/scripts/worker_synchronization.py
--rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/daemons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.476573 panda-server-0.0.62/pandaserver/dataservice/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/Activator.py
--rw-r--r--   0 runner    (1001) docker     (123)    53929 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/AdderAtlasPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/AdderDummyPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    40284 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/AdderGen.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/AdderPluginBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/AdderResult.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/AdderSimplePlugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17541 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/Closer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/CloserAtlasPlugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27051 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/DDM.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1988 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/DDMHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/DataService.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/DataServiceUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    57671 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/DynDataDistributer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      412 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/ErrorCode.py
--rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/EventPicker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11067 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/Finisher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18450 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/Notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/ProcessLimiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/RecoverLostFilesCore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8488 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/Setupper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   113605 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/SetupperAtlasPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/SetupperDummyPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/SetupperPluginBase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/eventLookupClientEI.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2101 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/dataservice/forkSetupper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.476573 panda-server-0.0.62/pandaserver/jobdispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/jobdispatcher/DispatcherUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      263 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/jobdispatcher/ErrorCode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59465 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/jobdispatcher/JobDispatcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16269 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/jobdispatcher/Protocol.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8959 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/jobdispatcher/Watcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/jobdispatcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.476573 panda-server-0.0.62/pandaserver/proxycache/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2898 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/proxycache/DBMSql.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/proxycache/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/proxycache/panda_activeusers_query.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9479 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/proxycache/panda_proxy_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.476573 panda-server-0.0.62/pandaserver/server/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/server/.gacl
--rwxr-xr-x   0 runner    (1001) docker     (123)    22529 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/server/panda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.476573 panda-server-0.0.62/pandaserver/srvcore/
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/srvcore/CoreUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4037 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/srvcore/MailUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/srvcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/srvcore/oidc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/srvcore/srv_msg_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.484573 panda-server-0.0.62/pandaserver/taskbuffer/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/CloudSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/CloudTaskSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/ConBridge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2132 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/DBProxyPool.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3002 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/DatasetSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/DdmSpec.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4647 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/EiDBProxy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1799 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/ErrorCode.py
--rw-r--r--   0 runner    (1001) docker     (123)    11270 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/EventServiceUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7836 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/FileSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/GlobalShares.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/HarvesterMetricsSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/Initializer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25903 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/JobSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/JobUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/NucleusSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)  1235999 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/OraDBProxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/PanDAMsgProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/PandaDBSchemaInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/PrioUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/ProcessGroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/ResourceSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/SQLDumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/SiteSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/SupErrors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   138600 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/TaskBuffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/TaskBufferInterface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19209 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/WorkerSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)    17662 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/WrappedCursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/WrappedPickle.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/WrappedPostgresConn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/retryModule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/taskbuffer/workflow_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.488573 panda-server-0.0.62/pandaserver/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/SchemaChecker.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.488573 panda-server-0.0.62/pandaserver/test/alice/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/alice/titan_testScript_ec2_alice_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/alice/titan_testScript_ec2_alice_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/banUser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      623 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/boostPrio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/boostUser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      789 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/callbackDDM.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10377 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/finishJob.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/finishTaskJEDI.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/frontier_retagging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1314 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/getJobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1922 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/killJob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2952 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/killJobLowPrio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1625 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/killJobsInTask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/killProdJobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2417 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/killTask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      239 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/killTaskJEDI.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/killUser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.488573 panda-server-0.0.62/pandaserver/test/lsst/
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/lsst/lsstSubmit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/lsst/lsstSubmitMERGEtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/lsst/lsstSubmitPhosim332.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      339 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/reassignJobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/reassignSite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/reassignTask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/reassignWaiting.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/recoverLostFiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/reloadInputDS.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/sendCommandToJob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/setDebugMode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      806 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/setPriority.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1834 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/testEvgen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1808 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/testEvgen17.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2574 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/testG4sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/testG4sim17.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/testGetCriteriaForGlobalShares.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/testGlobalShares.py
--rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/testJobFlowATLAS.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3739 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/testReco.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/testSimulReco14.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/testSiteMap.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/testUpdateWorkerPilotStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/test/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.488573 panda-server-0.0.62/pandaserver/userinterface/
--rwxr-xr-x   0 runner    (1001) docker     (123)    81389 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/userinterface/Client.py
--rw-r--r--   0 runner    (1001) docker     (123)    89623 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/userinterface/UserIF.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/userinterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.488573 panda-server-0.0.62/pandaserver/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/workflow/pcwl_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/workflow/pcwl_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/workflow/psnakemake_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.488573 panda-server-0.0.62/pandaserver/workflow/snakeparser/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/workflow/snakeparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/workflow/snakeparser/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/workflow/snakeparser/log.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/workflow/snakeparser/names.py
--rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/workflow/snakeparser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/workflow/snakeparser/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    36076 2023-06-30 04:35:59.000000 panda-server-0.0.62/pandaserver/workflow/workflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-30 04:36:09.492573 panda-server-0.0.62/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)    12531 2023-06-30 04:35:59.000000 panda-server-0.0.62/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.488573 panda-server-0.0.62/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-30 04:35:59.000000 panda-server-0.0.62/templates/conda_meta.yaml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.488573 panda-server-0.0.62/templates/init.d/
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-30 04:35:59.000000 panda-server-0.0.62/templates/init.d/panda_daemon.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-06-30 04:35:59.000000 panda-server-0.0.62/templates/init.d/panda_httpd.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)     1547 2023-06-30 04:35:59.000000 panda-server-0.0.62/templates/init.d/panda_server.exe.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.488573 panda-server-0.0.62/templates/logrotate.d/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-30 04:35:59.000000 panda-server-0.0.62/templates/logrotate.d/panda_server.logrotate.template
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-06-30 04:35:59.000000 panda-server-0.0.62/templates/panda_server-httpd-FastCGI.conf.rpmnew.template
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-30 04:35:59.000000 panda-server-0.0.62/templates/panda_server-httpd.conf.rpmnew.template
--rwxr-xr-x   0 runner    (1001) docker     (123)    13906 2023-06-30 04:35:59.000000 panda-server-0.0.62/templates/panda_server-makeSlsXml.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      745 2023-06-30 04:35:59.000000 panda-server-0.0.62/templates/panda_server-vomsrenew.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-06-30 04:35:59.000000 panda-server-0.0.62/templates/panda_server.cfg.rpmnew.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.492573 panda-server-0.0.62/templates/sysconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-30 04:35:59.000000 panda-server-0.0.62/templates/sysconfig/panda_server.sysconfig.rpmnew.template
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-30 04:35:59.000000 panda-server-0.0.62/templates/sysconfig/panda_server_env.systemd.rpmnew.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:36:09.492573 panda-server-0.0.62/templates/systemd/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-30 04:35:59.000000 panda-server-0.0.62/templates/systemd/panda.service.template
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-30 04:35:59.000000 panda-server-0.0.62/templates/systemd/panda_daemon.service.template
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-30 04:35:59.000000 panda-server-0.0.62/templates/systemd/panda_httpd.service.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.533290 panda-server-0.0.63/
+-rw-r--r--   0 runner    (1001) docker     (123)    81051 2023-06-30 17:47:15.000000 panda-server-0.0.63/ChangeLog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-30 17:47:15.000000 panda-server-0.0.63/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-30 17:47:15.000000 panda-server-0.0.63/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-30 17:47:25.533290 panda-server-0.0.63/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 17:47:15.000000 panda-server-0.0.63/PandaPkgInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-30 17:47:15.000000 panda-server-0.0.63/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.505290 panda-server-0.0.63/panda_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-30 17:47:25.000000 panda-server-0.0.63/panda_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-06-30 17:47:25.000000 panda-server-0.0.63/panda_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:47:25.000000 panda-server-0.0.63/panda_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:47:25.000000 panda-server-0.0.63/panda_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-30 17:47:25.000000 panda-server-0.0.63/panda_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-30 17:47:25.000000 panda-server-0.0.63/panda_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.505290 panda-server-0.0.63/pandaserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.505290 panda-server-0.0.63/pandaserver/brokerage/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/brokerage/ErrorCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/brokerage/SiteMapper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/brokerage/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    80940 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/brokerage/broker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.505290 panda-server-0.0.63/pandaserver/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/config/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/config/daemon_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7167 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/config/panda_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.505290 panda-server-0.0.63/pandaserver/configurator/
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/configurator/Carbon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35264 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/configurator/Configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/configurator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/configurator/aux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.505290 panda-server-0.0.63/pandaserver/daemons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/daemons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/daemons/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/daemons/master_systemd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.509290 panda-server-0.0.63/pandaserver/daemons/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/daemons/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/daemons/scripts/add_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/daemons/scripts/add_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/daemons/scripts/carbon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/daemons/scripts/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64166 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/daemons/scripts/copyArchive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/daemons/scripts/datasetManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/daemons/scripts/dummy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/daemons/scripts/evpPD2P.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41977 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/daemons/scripts/metric_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/daemons/scripts/panda_activeusers_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/daemons/scripts/pilotStreaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-06-30 17:47:15.000000 panda-server-0.0.63/pandaserver/daemons/scripts/process_workflow_files_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/daemons/scripts/recover_lost_files_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15682 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/daemons/scripts/task_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/daemons/scripts/tmpwatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/daemons/scripts/worker_synchronization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/daemons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.513290 panda-server-0.0.63/pandaserver/dataservice/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/Activator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53929 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/AdderAtlasPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/AdderDummyPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40284 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/AdderGen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/AdderPluginBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/AdderResult.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/AdderSimplePlugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17541 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/Closer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/CloserAtlasPlugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27051 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/DDM.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1988 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/DDMHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/DataService.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/DataServiceUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57671 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/DynDataDistributer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      412 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/ErrorCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/EventPicker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11067 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/Finisher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18450 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/Notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/ProcessLimiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/RecoverLostFilesCore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8488 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/Setupper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   113605 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/SetupperAtlasPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/SetupperDummyPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/SetupperPluginBase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/eventLookupClientEI.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2101 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/dataservice/forkSetupper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.513290 panda-server-0.0.63/pandaserver/jobdispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/jobdispatcher/DispatcherUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      263 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/jobdispatcher/ErrorCode.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59465 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/jobdispatcher/JobDispatcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16269 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/jobdispatcher/Protocol.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8959 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/jobdispatcher/Watcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/jobdispatcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.513290 panda-server-0.0.63/pandaserver/proxycache/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2898 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/proxycache/DBMSql.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/proxycache/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/proxycache/panda_activeusers_query.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9479 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/proxycache/panda_proxy_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.513290 panda-server-0.0.63/pandaserver/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/server/.gacl
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22529 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/server/panda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.517290 panda-server-0.0.63/pandaserver/srvcore/
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/srvcore/CoreUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4037 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/srvcore/MailUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/srvcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/srvcore/oidc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/srvcore/srv_msg_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.521290 panda-server-0.0.63/pandaserver/taskbuffer/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/CloudSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/CloudTaskSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/ConBridge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2132 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/DBProxyPool.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3002 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/DatasetSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/DdmSpec.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4647 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/EiDBProxy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1799 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/ErrorCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11270 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/EventServiceUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7836 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/FileSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/GlobalShares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/HarvesterMetricsSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/Initializer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25903 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/JobSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/JobUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/NucleusSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1235999 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/OraDBProxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/PanDAMsgProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/PandaDBSchemaInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/PrioUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/ProcessGroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/ResourceSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/SQLDumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/SiteSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/SupErrors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   138600 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/TaskBuffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/TaskBufferInterface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19209 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/WorkerSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17742 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/WrappedCursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/WrappedPickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/WrappedPostgresConn.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/retryModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/taskbuffer/workflow_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.529290 panda-server-0.0.63/pandaserver/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/SchemaChecker.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.529290 panda-server-0.0.63/pandaserver/test/alice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/alice/titan_testScript_ec2_alice_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/alice/titan_testScript_ec2_alice_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/banUser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      623 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/boostPrio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/boostUser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      789 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/callbackDDM.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10377 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/finishJob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/finishTaskJEDI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/frontier_retagging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1314 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/getJobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1922 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/killJob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2952 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/killJobLowPrio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1625 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/killJobsInTask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/killProdJobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2417 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/killTask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      239 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/killTaskJEDI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/killUser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.529290 panda-server-0.0.63/pandaserver/test/lsst/
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/lsst/lsstSubmit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/lsst/lsstSubmitMERGEtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/lsst/lsstSubmitPhosim332.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      339 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/reassignJobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/reassignSite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/reassignTask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/reassignWaiting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/recoverLostFiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/reloadInputDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/sendCommandToJob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/setDebugMode.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      806 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/setPriority.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1834 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/testEvgen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1808 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/testEvgen17.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2574 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/testG4sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/testG4sim17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/testGetCriteriaForGlobalShares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/testGlobalShares.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/testJobFlowATLAS.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3739 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/testReco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/testSimulReco14.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/testSiteMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/testUpdateWorkerPilotStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/test/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.529290 panda-server-0.0.63/pandaserver/userinterface/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81389 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/userinterface/Client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89623 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/userinterface/UserIF.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/userinterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.529290 panda-server-0.0.63/pandaserver/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/workflow/pcwl_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/workflow/pcwl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/workflow/psnakemake_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.533290 panda-server-0.0.63/pandaserver/workflow/snakeparser/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/workflow/snakeparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/workflow/snakeparser/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/workflow/snakeparser/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/workflow/snakeparser/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/workflow/snakeparser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/workflow/snakeparser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36076 2023-06-30 17:47:16.000000 panda-server-0.0.63/pandaserver/workflow/workflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-30 17:47:25.533290 panda-server-0.0.63/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12531 2023-06-30 17:47:16.000000 panda-server-0.0.63/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.533290 panda-server-0.0.63/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-30 17:47:16.000000 panda-server-0.0.63/templates/conda_meta.yaml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.533290 panda-server-0.0.63/templates/init.d/
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-30 17:47:16.000000 panda-server-0.0.63/templates/init.d/panda_daemon.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-06-30 17:47:16.000000 panda-server-0.0.63/templates/init.d/panda_httpd.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1547 2023-06-30 17:47:16.000000 panda-server-0.0.63/templates/init.d/panda_server.exe.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.533290 panda-server-0.0.63/templates/logrotate.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-30 17:47:16.000000 panda-server-0.0.63/templates/logrotate.d/panda_server.logrotate.template
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-06-30 17:47:16.000000 panda-server-0.0.63/templates/panda_server-httpd-FastCGI.conf.rpmnew.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-30 17:47:16.000000 panda-server-0.0.63/templates/panda_server-httpd.conf.rpmnew.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13906 2023-06-30 17:47:16.000000 panda-server-0.0.63/templates/panda_server-makeSlsXml.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      745 2023-06-30 17:47:16.000000 panda-server-0.0.63/templates/panda_server-vomsrenew.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-06-30 17:47:16.000000 panda-server-0.0.63/templates/panda_server.cfg.rpmnew.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.533290 panda-server-0.0.63/templates/sysconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-30 17:47:16.000000 panda-server-0.0.63/templates/sysconfig/panda_server.sysconfig.rpmnew.template
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-30 17:47:16.000000 panda-server-0.0.63/templates/sysconfig/panda_server_env.systemd.rpmnew.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:47:25.533290 panda-server-0.0.63/templates/systemd/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-30 17:47:16.000000 panda-server-0.0.63/templates/systemd/panda.service.template
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-30 17:47:16.000000 panda-server-0.0.63/templates/systemd/panda_daemon.service.template
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-30 17:47:16.000000 panda-server-0.0.63/templates/systemd/panda_httpd.service.template
```

### Comparing `panda-server-0.0.62/ChangeLog.txt` & `panda-server-0.0.63/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/LICENSE.txt` & `panda-server-0.0.63/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/panda_server.egg-info/SOURCES.txt` & `panda-server-0.0.63/panda_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/brokerage/SiteMapper.py` & `panda-server-0.0.63/pandaserver/brokerage/SiteMapper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/brokerage/broker.py` & `panda-server-0.0.63/pandaserver/brokerage/broker.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/config/daemon_config.py` & `panda-server-0.0.63/pandaserver/config/daemon_config.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/config/panda_config.py` & `panda-server-0.0.63/pandaserver/config/panda_config.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/configurator/Carbon.py` & `panda-server-0.0.63/pandaserver/configurator/Carbon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/configurator/Configurator.py` & `panda-server-0.0.63/pandaserver/configurator/Configurator.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/configurator/aux.py` & `panda-server-0.0.63/pandaserver/configurator/aux.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/daemons/master.py` & `panda-server-0.0.63/pandaserver/daemons/master.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/daemons/master_systemd.py` & `panda-server-0.0.63/pandaserver/daemons/master_systemd.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/daemons/scripts/add_main.py` & `panda-server-0.0.63/pandaserver/daemons/scripts/add_main.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/daemons/scripts/add_sub.py` & `panda-server-0.0.63/pandaserver/daemons/scripts/add_sub.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/daemons/scripts/carbon.py` & `panda-server-0.0.63/pandaserver/daemons/scripts/carbon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/daemons/scripts/configurator.py` & `panda-server-0.0.63/pandaserver/daemons/scripts/configurator.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/daemons/scripts/copyArchive.py` & `panda-server-0.0.63/pandaserver/daemons/scripts/copyArchive.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/daemons/scripts/datasetManager.py` & `panda-server-0.0.63/pandaserver/daemons/scripts/datasetManager.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/daemons/scripts/dummy_test.py` & `panda-server-0.0.63/pandaserver/daemons/scripts/dummy_test.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/daemons/scripts/evpPD2P.py` & `panda-server-0.0.63/pandaserver/daemons/scripts/evpPD2P.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/daemons/scripts/metric_collector.py` & `panda-server-0.0.63/pandaserver/daemons/scripts/metric_collector.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/daemons/scripts/panda_activeusers_query.py` & `panda-server-0.0.63/pandaserver/daemons/scripts/panda_activeusers_query.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/daemons/scripts/pilotStreaming.py` & `panda-server-0.0.63/pandaserver/daemons/scripts/pilotStreaming.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/daemons/scripts/process_workflow_files_daemon.py` & `panda-server-0.0.63/pandaserver/daemons/scripts/process_workflow_files_daemon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/daemons/scripts/recover_lost_files_daemon.py` & `panda-server-0.0.63/pandaserver/daemons/scripts/recover_lost_files_daemon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/daemons/scripts/task_evaluator.py` & `panda-server-0.0.63/pandaserver/daemons/scripts/task_evaluator.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/daemons/scripts/tmpwatch.py` & `panda-server-0.0.63/pandaserver/daemons/scripts/tmpwatch.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/daemons/scripts/worker_synchronization.py` & `panda-server-0.0.63/pandaserver/daemons/scripts/worker_synchronization.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/daemons/utils.py` & `panda-server-0.0.63/pandaserver/daemons/utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/dataservice/Activator.py` & `panda-server-0.0.63/pandaserver/dataservice/Activator.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/dataservice/AdderAtlasPlugin.py` & `panda-server-0.0.63/pandaserver/dataservice/AdderAtlasPlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/dataservice/AdderGen.py` & `panda-server-0.0.63/pandaserver/dataservice/AdderGen.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/dataservice/AdderResult.py` & `panda-server-0.0.63/pandaserver/dataservice/AdderResult.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/dataservice/AdderSimplePlugin.py` & `panda-server-0.0.63/pandaserver/dataservice/AdderSimplePlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/dataservice/Closer.py` & `panda-server-0.0.63/pandaserver/dataservice/Closer.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/dataservice/CloserAtlasPlugin.py` & `panda-server-0.0.63/pandaserver/dataservice/CloserAtlasPlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/dataservice/DDM.py` & `panda-server-0.0.63/pandaserver/dataservice/DDM.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/dataservice/DDMHandler.py` & `panda-server-0.0.63/pandaserver/dataservice/DDMHandler.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/dataservice/DataService.py` & `panda-server-0.0.63/pandaserver/dataservice/DataService.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/dataservice/DataServiceUtils.py` & `panda-server-0.0.63/pandaserver/dataservice/DataServiceUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/dataservice/DynDataDistributer.py` & `panda-server-0.0.63/pandaserver/dataservice/DynDataDistributer.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/dataservice/EventPicker.py` & `panda-server-0.0.63/pandaserver/dataservice/EventPicker.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/dataservice/Finisher.py` & `panda-server-0.0.63/pandaserver/dataservice/Finisher.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/dataservice/Notifier.py` & `panda-server-0.0.63/pandaserver/dataservice/Notifier.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/dataservice/ProcessLimiter.py` & `panda-server-0.0.63/pandaserver/dataservice/ProcessLimiter.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/dataservice/RecoverLostFilesCore.py` & `panda-server-0.0.63/pandaserver/dataservice/RecoverLostFilesCore.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,14 +46,17 @@
     parser.add_argument('--dryRun',action='store_const',const=True,dest='dryRun',default=False,
                         help='dry run')
     parser.add_argument('--force', action='store_const', const=True, dest='force', default=False,
                         help='force retry even if no lost files')
     parser.add_argument('--reproduceParent', action='store_const', const=True, dest='reproduceParent',
                         default=False, help='reproduce the input files from which the lost files were produced. '
                         'Typically useful to recover merged files when unmerged files were already deleted')
+    parser.add_argument('--reproduceUptoNthGen', action='store', dest='reproduceUptoNthGen', type=int, default=0,
+                        help='reproduce files up to N-th upper generation. --reproduceUptoNthGen=1 corresponds '
+                             'to --reproduceParent. 0 by default so that any provenance files are not reproduced')
     # parse options
     if taskBuffer:
         if args_list:
             options = parser.parse_args(args_list)
         else:
             options, unknown = parser.parse_known_args()
     else:
@@ -79,14 +82,18 @@
             if k in keys:
                 setattr(options, k, exec_options[k])
         if 'jediTaskID' in exec_options:
             givenTaskID = exec_options['jediTaskID']
         if 'userName' in exec_options:
             dn = exec_options['userName']
 
+    if options.reproduceUptoNthGen > 0:
+        options.reproduceUptoNthGen -= 1
+        options.reproduceParent = True
+
     ds_files = {}
     if options.files is not None:
         files = options.files.split(',')
         ds_files[options.ds] = files
     else:
         # look for lost files
         if not givenTaskID:
@@ -162,19 +169,21 @@
                                                                               options.dryRun)
         msgStr = 'reset file status for {} in the DB: done with {} for jediTaskID={}'.format(tmpDS, ts, jediTaskID)
         if log_stream:
             log_stream.info(msgStr)
         else:
             print(msgStr)
         s |= ts
-        # recover parent
+        # recover provenance
         if options.reproduceParent:
             # reproduce input
             for lostDS in lostInputFiles:
                 com_args = ['--ds', lostDS, '--noChildRetry', '--resurrectDS']
+                if options.reproduceUptoNthGen > 0:
+                    com_args += ['--reproduceUptoNthGen', str(options.reproduceUptoNthGen)]
                 if options.dryRun:
                     com_args.append('--dryRun')
                 com_args += ['--files', ','.join(lostInputFiles[lostDS])]
             main(taskBuffer=taskBuffer, log_stream=log_stream, args_list=com_args)
 
     # go ahead
     if options.dryRun:
@@ -199,18 +208,18 @@
                         except Exception:
                             pass
         if not options.reproduceParent:
             msgStr = Client.retryTask(jediTaskID, noChildRetry=options.noChildRetry)[-1][-1]
         else:
             msgStr = Client.reloadInput(jediTaskID)[-1][-1]
         if log_stream:
-            log_stream.info("Retried task with {}".format(msgStr))
+            log_stream.info("Retried task {} with {}".format(jediTaskID, msgStr))
             log_stream.info("Done")
         else:
-            print("Retried task: done with {}".format(msgStr))
+            print("Retried task {}: done with {}".format(jediTaskID, msgStr))
         return True, msgStr
     else:
         msgStr = 'failed'
         if log_stream:
             log_stream.error(msgStr)
         else:
             print(msgStr)
```

### Comparing `panda-server-0.0.62/pandaserver/dataservice/Setupper.py` & `panda-server-0.0.63/pandaserver/dataservice/Setupper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/dataservice/SetupperAtlasPlugin.py` & `panda-server-0.0.63/pandaserver/dataservice/SetupperAtlasPlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/dataservice/SetupperDummyPlugin.py` & `panda-server-0.0.63/pandaserver/dataservice/SetupperDummyPlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/dataservice/SetupperPluginBase.py` & `panda-server-0.0.63/pandaserver/dataservice/SetupperPluginBase.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/dataservice/eventLookupClientEI.py` & `panda-server-0.0.63/pandaserver/dataservice/eventLookupClientEI.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/dataservice/forkSetupper.py` & `panda-server-0.0.63/pandaserver/dataservice/forkSetupper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/jobdispatcher/DispatcherUtils.py` & `panda-server-0.0.63/pandaserver/jobdispatcher/DispatcherUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/jobdispatcher/JobDispatcher.py` & `panda-server-0.0.63/pandaserver/jobdispatcher/JobDispatcher.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/jobdispatcher/Protocol.py` & `panda-server-0.0.63/pandaserver/jobdispatcher/Protocol.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/jobdispatcher/Watcher.py` & `panda-server-0.0.63/pandaserver/jobdispatcher/Watcher.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/proxycache/DBMSql.py` & `panda-server-0.0.63/pandaserver/proxycache/DBMSql.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/proxycache/panda_activeusers_query.py` & `panda-server-0.0.63/pandaserver/proxycache/panda_activeusers_query.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/proxycache/panda_proxy_cache.py` & `panda-server-0.0.63/pandaserver/proxycache/panda_proxy_cache.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/server/panda.py` & `panda-server-0.0.63/pandaserver/server/panda.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/srvcore/CoreUtils.py` & `panda-server-0.0.63/pandaserver/srvcore/CoreUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/srvcore/MailUtils.py` & `panda-server-0.0.63/pandaserver/srvcore/MailUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/srvcore/oidc_utils.py` & `panda-server-0.0.63/pandaserver/srvcore/oidc_utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/srvcore/srv_msg_utils.py` & `panda-server-0.0.63/pandaserver/srvcore/srv_msg_utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/CloudSpec.py` & `panda-server-0.0.63/pandaserver/taskbuffer/CloudSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/CloudTaskSpec.py` & `panda-server-0.0.63/pandaserver/taskbuffer/CloudTaskSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/ConBridge.py` & `panda-server-0.0.63/pandaserver/taskbuffer/ConBridge.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/DBProxyPool.py` & `panda-server-0.0.63/pandaserver/taskbuffer/DBProxyPool.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/DatasetSpec.py` & `panda-server-0.0.63/pandaserver/taskbuffer/DatasetSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/DdmSpec.py` & `panda-server-0.0.63/pandaserver/taskbuffer/DdmSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/EiDBProxy.py` & `panda-server-0.0.63/pandaserver/taskbuffer/EiDBProxy.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/ErrorCode.py` & `panda-server-0.0.63/pandaserver/taskbuffer/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/EventServiceUtils.py` & `panda-server-0.0.63/pandaserver/taskbuffer/EventServiceUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/FileSpec.py` & `panda-server-0.0.63/pandaserver/taskbuffer/FileSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/GlobalShares.py` & `panda-server-0.0.63/pandaserver/taskbuffer/GlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/HarvesterMetricsSpec.py` & `panda-server-0.0.63/pandaserver/taskbuffer/HarvesterMetricsSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/Initializer.py` & `panda-server-0.0.63/pandaserver/taskbuffer/Initializer.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/JobSpec.py` & `panda-server-0.0.63/pandaserver/taskbuffer/JobSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/JobUtils.py` & `panda-server-0.0.63/pandaserver/taskbuffer/JobUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/NucleusSpec.py` & `panda-server-0.0.63/pandaserver/taskbuffer/NucleusSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/OraDBProxy.py` & `panda-server-0.0.63/pandaserver/taskbuffer/OraDBProxy.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/PrioUtil.py` & `panda-server-0.0.63/pandaserver/taskbuffer/PrioUtil.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/ProcessGroups.py` & `panda-server-0.0.63/pandaserver/taskbuffer/ProcessGroups.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/ResourceSpec.py` & `panda-server-0.0.63/pandaserver/taskbuffer/ResourceSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/SQLDumper.py` & `panda-server-0.0.63/pandaserver/taskbuffer/SQLDumper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/SiteSpec.py` & `panda-server-0.0.63/pandaserver/taskbuffer/SiteSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/TaskBuffer.py` & `panda-server-0.0.63/pandaserver/taskbuffer/TaskBuffer.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/TaskBufferInterface.py` & `panda-server-0.0.63/pandaserver/taskbuffer/TaskBufferInterface.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/Utils.py` & `panda-server-0.0.63/pandaserver/taskbuffer/Utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/WorkerSpec.py` & `panda-server-0.0.63/pandaserver/taskbuffer/WorkerSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/WrappedCursor.py` & `panda-server-0.0.63/pandaserver/taskbuffer/WrappedCursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,16 @@
         sql = re.sub(r"NVL\(", r"COALESCE(", sql, flags=re.IGNORECASE)
         # random
         sql = re.sub(r"DBMS_RANDOM.value", r"RANDOM()", sql, flags=re.IGNORECASE)
         # GENERATE_SERIES
         sql = re.sub(r'\(SELECT\s+level\s+FROM\s+dual\s+CONNECT\s+BY\s+level\s*<=\s*(:[^ \)]+)\)*',
                      r'GENERATE_SERIES(1,\1)',
                      sql, flags=re.IGNORECASE)
+        # dual
+        sql = re.sub(r"FROM dual", "", sql, flags=re.IGNORECASE)
         # json
         if '/* use_json_type */' in sql:
             # remove \n to make regexp easier
             sql = re.sub(r'\n', r' ', sql)
             # collect table names
             table_names = set()
             for item in re.findall(r' FROM (.+?)(WHERE|$)', sql, flags=re.IGNORECASE):
```

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/WrappedPickle.py` & `panda-server-0.0.63/pandaserver/taskbuffer/WrappedPickle.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/retryModule.py` & `panda-server-0.0.63/pandaserver/taskbuffer/retryModule.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/taskbuffer/workflow_processor.py` & `panda-server-0.0.63/pandaserver/taskbuffer/workflow_processor.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/SchemaChecker.py` & `panda-server-0.0.63/pandaserver/test/SchemaChecker.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/alice/titan_testScript_ec2_alice_1.py` & `panda-server-0.0.63/pandaserver/test/alice/titan_testScript_ec2_alice_1.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/alice/titan_testScript_ec2_alice_2.py` & `panda-server-0.0.63/pandaserver/test/alice/titan_testScript_ec2_alice_2.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/banUser.py` & `panda-server-0.0.63/pandaserver/test/banUser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/boostPrio.py` & `panda-server-0.0.63/pandaserver/test/boostPrio.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/boostUser.py` & `panda-server-0.0.63/pandaserver/test/boostUser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/callbackDDM.py` & `panda-server-0.0.63/pandaserver/test/callbackDDM.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/finishJob.py` & `panda-server-0.0.63/pandaserver/test/finishJob.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/frontier_retagging.py` & `panda-server-0.0.63/pandaserver/test/frontier_retagging.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/getJobs.py` & `panda-server-0.0.63/pandaserver/test/getJobs.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/killJob.py` & `panda-server-0.0.63/pandaserver/test/killJob.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/killJobLowPrio.py` & `panda-server-0.0.63/pandaserver/test/killJobLowPrio.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/killJobsInTask.py` & `panda-server-0.0.63/pandaserver/test/killJobsInTask.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/killProdJobs.py` & `panda-server-0.0.63/pandaserver/test/killProdJobs.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/killTask.py` & `panda-server-0.0.63/pandaserver/test/killTask.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/killUser.py` & `panda-server-0.0.63/pandaserver/test/killUser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/lsst/lsstSubmit.py` & `panda-server-0.0.63/pandaserver/test/lsst/lsstSubmit.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/lsst/lsstSubmitMERGEtest.py` & `panda-server-0.0.63/pandaserver/test/lsst/lsstSubmitMERGEtest.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/lsst/lsstSubmitPhosim332.py` & `panda-server-0.0.63/pandaserver/test/lsst/lsstSubmitPhosim332.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/reassignSite.py` & `panda-server-0.0.63/pandaserver/test/reassignSite.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/reassignTask.py` & `panda-server-0.0.63/pandaserver/test/reassignTask.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/reassignWaiting.py` & `panda-server-0.0.63/pandaserver/test/reassignWaiting.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/reloadInputDS.py` & `panda-server-0.0.63/pandaserver/test/reloadInputDS.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/sendCommandToJob.py` & `panda-server-0.0.63/pandaserver/test/sendCommandToJob.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/setDebugMode.py` & `panda-server-0.0.63/pandaserver/test/setDebugMode.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/setPriority.py` & `panda-server-0.0.63/pandaserver/test/setPriority.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/testEvgen.py` & `panda-server-0.0.63/pandaserver/test/testEvgen.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/testEvgen17.py` & `panda-server-0.0.63/pandaserver/test/testEvgen17.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/testG4sim.py` & `panda-server-0.0.63/pandaserver/test/testG4sim.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/testG4sim17.py` & `panda-server-0.0.63/pandaserver/test/testG4sim17.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/testGetCriteriaForGlobalShares.py` & `panda-server-0.0.63/pandaserver/test/testGetCriteriaForGlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/testGlobalShares.py` & `panda-server-0.0.63/pandaserver/test/testGlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/testJobFlowATLAS.py` & `panda-server-0.0.63/pandaserver/test/testJobFlowATLAS.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/testReco.py` & `panda-server-0.0.63/pandaserver/test/testReco.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/testSimulReco14.py` & `panda-server-0.0.63/pandaserver/test/testSimulReco14.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/testSiteMap.py` & `panda-server-0.0.63/pandaserver/test/testSiteMap.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/test/testutils.py` & `panda-server-0.0.63/pandaserver/test/testutils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/userinterface/Client.py` & `panda-server-0.0.63/pandaserver/userinterface/Client.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/userinterface/UserIF.py` & `panda-server-0.0.63/pandaserver/userinterface/UserIF.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/workflow/pcwl_test.py` & `panda-server-0.0.63/pandaserver/workflow/pcwl_test.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/workflow/pcwl_utils.py` & `panda-server-0.0.63/pandaserver/workflow/pcwl_utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/workflow/psnakemake_test.py` & `panda-server-0.0.63/pandaserver/workflow/psnakemake_test.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/workflow/snakeparser/extensions.py` & `panda-server-0.0.63/pandaserver/workflow/snakeparser/extensions.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/workflow/snakeparser/log.py` & `panda-server-0.0.63/pandaserver/workflow/snakeparser/log.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/workflow/snakeparser/parser.py` & `panda-server-0.0.63/pandaserver/workflow/snakeparser/parser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/workflow/snakeparser/utils.py` & `panda-server-0.0.63/pandaserver/workflow/snakeparser/utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/pandaserver/workflow/workflow_utils.py` & `panda-server-0.0.63/pandaserver/workflow/workflow_utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/setup.py` & `panda-server-0.0.63/setup.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/templates/conda_meta.yaml.template` & `panda-server-0.0.63/templates/conda_meta.yaml.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/templates/init.d/panda_daemon.exe.template` & `panda-server-0.0.63/templates/init.d/panda_daemon.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/templates/init.d/panda_httpd.exe.template` & `panda-server-0.0.63/templates/init.d/panda_httpd.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/templates/init.d/panda_server.exe.template` & `panda-server-0.0.63/templates/init.d/panda_server.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/templates/logrotate.d/panda_server.logrotate.template` & `panda-server-0.0.63/templates/logrotate.d/panda_server.logrotate.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/templates/panda_server-httpd-FastCGI.conf.rpmnew.template` & `panda-server-0.0.63/templates/panda_server-httpd-FastCGI.conf.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/templates/panda_server-httpd.conf.rpmnew.template` & `panda-server-0.0.63/templates/panda_server-httpd.conf.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/templates/panda_server-makeSlsXml.exe.template` & `panda-server-0.0.63/templates/panda_server-makeSlsXml.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/templates/panda_server-vomsrenew.exe.template` & `panda-server-0.0.63/templates/panda_server-vomsrenew.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/templates/panda_server.cfg.rpmnew.template` & `panda-server-0.0.63/templates/panda_server.cfg.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/templates/sysconfig/panda_server.sysconfig.rpmnew.template` & `panda-server-0.0.63/templates/sysconfig/panda_server.sysconfig.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.62/templates/sysconfig/panda_server_env.systemd.rpmnew.template` & `panda-server-0.0.63/templates/sysconfig/panda_server_env.systemd.rpmnew.template`

 * *Files identical despite different names*

