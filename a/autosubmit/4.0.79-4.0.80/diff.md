# Comparing `tmp/autosubmit-4.0.79.tar.gz` & `tmp/autosubmit-4.0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosubmit-4.0.79.tar", last modified: Mon May  8 14:19:10 2023, max compression
+gzip compressed data, was "autosubmit-4.0.80.tar", last modified: Fri Jun 30 08:32:54 2023, max compression
```

## Comparing `autosubmit-4.0.79.tar` & `autosubmit-4.0.80.tar`

### file list

```diff
@@ -1,405 +1,407 @@
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.629279 autosubmit-4.0.79/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      226 2023-05-02 11:09:16.000000 autosubmit-4.0.79/.gitignore
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1361 2023-05-02 11:09:16.000000 autosubmit-4.0.79/.gitlab-ci.yml
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      629 2023-05-02 11:09:16.000000 autosubmit-4.0.79/.readthedocs.yaml
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.79/CHANGELOG
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      722 2023-05-02 11:09:16.000000 autosubmit-4.0.79/CONTRIBUTING.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    35147 2021-10-05 14:18:20.000000 autosubmit-4.0.79/LICENSE
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      119 2021-10-05 14:18:20.000000 autosubmit-4.0.79/MANIFEST.in
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3347 2023-05-08 14:19:10.629279 autosubmit-4.0.79/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5651 2023-05-02 11:09:16.000000 autosubmit-4.0.79/README.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2287 2023-05-02 11:09:16.000000 autosubmit-4.0.79/README_PIP.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        7 2023-05-08 14:19:05.000000 autosubmit-4.0.79/VERSION
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.593280 autosubmit-4.0.79/autosubmit/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.79/autosubmit/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   318723 2023-05-08 14:14:23.000000 autosubmit-4.0.79/autosubmit/autosubmit.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.597280 autosubmit-4.0.79/autosubmit/database/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.79/autosubmit/database/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.597280 autosubmit-4.0.79/autosubmit/database/data/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      258 2021-10-05 14:18:20.000000 autosubmit-4.0.79/autosubmit/database/data/autosubmit.sql
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19910 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/database/db_common.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7593 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/database/db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6065 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/database/db_structure.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.597280 autosubmit-4.0.79/autosubmit/experiment/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.79/autosubmit/experiment/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5280 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/experiment/experiment_common.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8450 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/experiment/statistics.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.597280 autosubmit-4.0.79/autosubmit/git/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.79/autosubmit/git/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13703 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/git/autosubmit_git.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.597280 autosubmit-4.0.79/autosubmit/helpers/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.79/autosubmit/helpers/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5776 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/helpers/autosubmit_helper.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      194 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/helpers/data_transfer.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1428 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/helpers/utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.597280 autosubmit-4.0.79/autosubmit/history/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.79/autosubmit/history/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.597280 autosubmit-4.0.79/autosubmit/history/data_classes/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.79/autosubmit/history/data_classes/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2432 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/history/data_classes/experiment_run.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10305 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/history/data_classes/job_data.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.597280 autosubmit-4.0.79/autosubmit/history/database_managers/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.79/autosubmit/history/database_managers/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5688 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/history/database_managers/database_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2409 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/history/database_managers/database_models.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19251 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/history/database_managers/experiment_history_db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6456 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/history/database_managers/experiment_status_db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    18844 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/history/experiment_history.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2382 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/history/experiment_status.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1952 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/history/internal_logging.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.597280 autosubmit-4.0.79/autosubmit/history/platform_monitor/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.79/autosubmit/history/platform_monitor/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.597280 autosubmit-4.0.79/autosubmit/history/platform_monitor/output_examples/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/history/platform_monitor/output_examples/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      185 2022-11-21 08:34:36.000000 autosubmit-4.0.79/autosubmit/history/platform_monitor/output_examples/pending.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      554 2022-11-21 08:34:36.000000 autosubmit-4.0.79/autosubmit/history/platform_monitor/output_examples/wrapper1.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      549 2022-11-21 08:34:36.000000 autosubmit-4.0.79/autosubmit/history/platform_monitor/output_examples/wrapper2.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6105 2022-11-21 08:34:36.000000 autosubmit-4.0.79/autosubmit/history/platform_monitor/output_examples/wrapper_big.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1025 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/history/platform_monitor/platform_monitor.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2298 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/history/platform_monitor/platform_utils.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2475 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/history/platform_monitor/slurm_monitor.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3454 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/history/platform_monitor/slurm_monitor_item.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10951 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/history/strategies.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2784 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/history/utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.601280 autosubmit-4.0.79/autosubmit/job/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.79/autosubmit/job/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    93132 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/job/job.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10907 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/job/job_common.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20050 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/job/job_dict.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13797 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/job/job_grouping.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   120598 2023-05-03 09:20:39.000000 autosubmit-4.0.79/autosubmit/job/job_list.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4609 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/job/job_list_persistence.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3565 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/job/job_package_persistence.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    62106 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/job/job_packager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    36449 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/job/job_packages.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11580 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/job/job_utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.601280 autosubmit-4.0.79/autosubmit/monitor/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.79/autosubmit/monitor/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10182 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/monitor/diagram.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    26910 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/monitor/monitor.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1414 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/monitor/utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.601280 autosubmit-4.0.79/autosubmit/notifications/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.79/autosubmit/notifications/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4049 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/notifications/mail_notifier.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1196 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/notifications/notifier.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.601280 autosubmit-4.0.79/autosubmit/platforms/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.79/autosubmit/platforms/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13279 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/platforms/ecplatform.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.601280 autosubmit-4.0.79/autosubmit/platforms/headers/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.79/autosubmit/platforms/headers/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5514 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/platforms/headers/ec_cca_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4100 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/platforms/headers/ec_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1826 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/platforms/headers/local_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7391 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/platforms/headers/lsf_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2972 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/platforms/headers/pbs10_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3497 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/platforms/headers/pbs11_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2963 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/platforms/headers/pbs12_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5750 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/platforms/headers/pjm_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2214 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/platforms/headers/ps_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3603 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/platforms/headers/sge_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7122 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/platforms/headers/slurm_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10469 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/platforms/locplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5557 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/platforms/lsfplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    53639 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/platforms/paramiko_platform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11370 2023-05-02 11:26:40.000000 autosubmit-4.0.79/autosubmit/platforms/paramiko_submitter.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5224 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/platforms/pbsplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20846 2023-05-08 14:14:23.000000 autosubmit-4.0.79/autosubmit/platforms/pjmplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    24463 2023-05-08 14:14:23.000000 autosubmit-4.0.79/autosubmit/platforms/platform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4184 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/platforms/psplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4617 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/platforms/sgeplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    31986 2023-05-08 14:14:23.000000 autosubmit-4.0.79/autosubmit/platforms/slurmplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1316 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/platforms/submitter.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.605280 autosubmit-4.0.79/autosubmit/platforms/wrappers/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.79/autosubmit/platforms/wrappers/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    38627 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/platforms/wrappers/wrapper_builder.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7581 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/platforms/wrappers/wrapper_factory.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.605280 autosubmit-4.0.79/autosubmit/statistics/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.79/autosubmit/statistics/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2869 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/statistics/jobs_stat.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6724 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/statistics/statistics.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1818 2023-02-02 09:02:16.000000 autosubmit-4.0.79/autosubmit/statistics/stats_summary.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1830 2023-05-02 11:09:16.000000 autosubmit-4.0.79/autosubmit/statistics/utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.593280 autosubmit-4.0.79/autosubmit.egg-info/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3347 2023-05-08 14:19:09.000000 autosubmit-4.0.79/autosubmit.egg-info/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12977 2023-05-08 14:19:10.000000 autosubmit-4.0.79/autosubmit.egg-info/SOURCES.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-05-08 14:19:09.000000 autosubmit-4.0.79/autosubmit.egg-info/dependency_links.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      452 2023-05-08 14:19:09.000000 autosubmit-4.0.79/autosubmit.egg-info/requires.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       20 2023-05-08 14:19:09.000000 autosubmit-4.0.79/autosubmit.egg-info/top_level.txt
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.605280 autosubmit-4.0.79/bin/
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     3086 2023-05-02 11:09:16.000000 autosubmit-4.0.79/bin/autosubmit
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.605280 autosubmit-4.0.79/docs/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7869 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/Makefile
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)  1513786 2021-10-05 14:18:20.000000 autosubmit-4.0.79/docs/autosubmit.pdf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.605280 autosubmit-4.0.79/docs/source/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.605280 autosubmit-4.0.79/docs/source/agui/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.605280 autosubmit-4.0.79/docs/source/agui/experiment/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.605280 autosubmit-4.0.79/docs/source/agui/experiment/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   112356 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/agui/experiment/fig/fig_experiment.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1430 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/agui/experiment/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.609280 autosubmit-4.0.79/docs/source/agui/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    25707 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/agui/fig/fig1_gui.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   140255 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/agui/fig/fig2_gui.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   184237 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/agui/fig/fig3_gui.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   114416 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/agui/fig/fig4_gui.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    44047 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/agui/fig/fig5_gui.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   248267 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/agui/fig/fig_ev_1.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   248251 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/agui/fig/fig_tree_1.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   241752 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/agui/fig/fig_tree_2.png
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.609280 autosubmit-4.0.79/docs/source/agui/graph/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.609280 autosubmit-4.0.79/docs/source/agui/graph/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   122929 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/agui/graph/fig/fig_graph_1.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   123449 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/agui/graph/fig/fig_graph_2.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   213843 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/agui/graph/fig/fig_graph_3.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    57438 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/agui/graph/fig/fig_graph_4.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6535 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/agui/graph/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4263 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/agui/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.609280 autosubmit-4.0.79/docs/source/agui/log/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.609280 autosubmit-4.0.79/docs/source/agui/log/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    25433 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/agui/log/fig/fig_log_1.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   117240 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/agui/log/fig/fig_log_2.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1125 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/agui/log/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.609280 autosubmit-4.0.79/docs/source/agui/performance/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.609280 autosubmit-4.0.79/docs/source/agui/performance/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   174233 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/agui/performance/fig/fig_performance_1.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      910 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/agui/performance/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.609280 autosubmit-4.0.79/docs/source/agui/statistics/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.609280 autosubmit-4.0.79/docs/source/agui/statistics/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    56486 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/agui/statistics/fig/fig_stat_1.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   101911 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/agui/statistics/fig/fig_stat_2.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      988 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/agui/statistics/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.609280 autosubmit-4.0.79/docs/source/agui/tree/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.609280 autosubmit-4.0.79/docs/source/agui/tree/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   114354 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/agui/tree/fig/fig_tree_2.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5756 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/agui/tree/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10119 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/conf.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.609280 autosubmit-4.0.79/docs/source/devguide/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2109 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/devguide/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2124 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.609280 autosubmit-4.0.79/docs/source/installation/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12768 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/installation/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.609280 autosubmit-4.0.79/docs/source/introduction/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   769052 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/introduction/fig1.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    93570 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/introduction/fig2.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    53843 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/introduction/fig3.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6099 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/introduction/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.613280 autosubmit-4.0.79/docs/source/moduledoc/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      130 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/moduledoc/autosubmit.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      445 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/moduledoc/config.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       99 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/moduledoc/database.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       89 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/moduledoc/git.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      128 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/moduledoc/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      185 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/moduledoc/job.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       94 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/moduledoc/monitor.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      547 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/moduledoc/platforms.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.613280 autosubmit-4.0.79/docs/source/qstartguide/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    50473 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/qstartguide/dummy.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     9400 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/qstartguide/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.613280 autosubmit-4.0.79/docs/source/troubleshooting/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    18379 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/troubleshooting/changelog.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    22857 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/troubleshooting/error-codes.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.613280 autosubmit-4.0.79/docs/source/troubleshooting/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    83094 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/troubleshooting/fig/monarch-da.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    68077 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/troubleshooting/fig/new_dependencies_0.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    68077 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/troubleshooting/fig/new_dependencies_1.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2770 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/troubleshooting/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.613280 autosubmit-4.0.79/docs/source/unused_figs/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    49607 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/unused_figs/group_chunk.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    32622 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/unused_figs/horizontal-vertical.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   106298 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/unused_figs/wrapper.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   251472 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/unused_figs/wrapper_expression.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19009 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/unused_figs/wrapper_hybrid.png
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.613280 autosubmit-4.0.79/docs/source/userguide/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.613280 autosubmit-4.0.79/docs/source/userguide/configure/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    30910 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/userguide/configure/develop_a_project.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20565 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/userguide/configure/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.613280 autosubmit-4.0.79/docs/source/userguide/create/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6907 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/userguide/create/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1877 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/userguide/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.613280 autosubmit-4.0.79/docs/source/userguide/manage/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    14283 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/userguide/manage/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.613280 autosubmit-4.0.79/docs/source/userguide/run/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    16002 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/userguide/run/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.613280 autosubmit-4.0.79/docs/source/userguide/wrappers/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.617280 autosubmit-4.0.79/docs/source/userguide/wrappers/fig/
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)   198622 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/userguide/wrappers/fig/dasim.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    23826 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/userguide/wrappers/fig/horizontal_remote.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   308786 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/userguide/wrappers/fig/multiple_wrappers.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    17531 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/userguide/wrappers/fig/rerun.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    33805 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/userguide/wrappers/fig/vertical-horizontal.png
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)    33140 2023-02-02 09:02:16.000000 autosubmit-4.0.79/docs/source/userguide/wrappers/fig/vertical-mixed.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11646 2023-05-02 11:09:16.000000 autosubmit-4.0.79/docs/source/userguide/wrappers/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      712 2023-05-02 11:09:16.000000 autosubmit-4.0.79/environment.yml
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.617280 autosubmit-4.0.79/log/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.79/log/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2023-05-02 11:09:16.000000 autosubmit-4.0.79/log/fd_show.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13696 2023-05-02 11:09:16.000000 autosubmit-4.0.79/log/log.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      457 2023-05-08 14:15:56.000000 autosubmit-4.0.79/requeriments.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-05-08 14:19:10.629279 autosubmit-4.0.79/setup.cfg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3086 2023-05-08 14:15:56.000000 autosubmit-4.0.79/setup.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.617280 autosubmit-4.0.79/test/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.617280 autosubmit-4.0.79/test/integration/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/integration/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1315 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/integration/test_db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2874 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/integration/test_job.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.617280 autosubmit-4.0.79/test/regression/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       33 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/.gitignore
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2429 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/README
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.617280 autosubmit-4.0.79/test/regression/db/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       90 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/db/.gitignore
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.617280 autosubmit-4.0.79/test/regression/default_conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1368 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/default_conf/platforms.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2946 2023-05-08 14:11:38.000000 autosubmit-4.0.79/test/regression/local_asparser_test.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.589280 autosubmit-4.0.79/test/regression/test_ecmwf_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.617280 autosubmit-4.0.79/test/regression/test_ecmwf_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_ecmwf_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2459 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/regression/test_ecmwf_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      577 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_ecmwf_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_ecmwf_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.617280 autosubmit-4.0.79/test/regression/test_ecmwf_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       97 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_ecmwf_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.589280 autosubmit-4.0.79/test/regression/test_large_experiment_on_moore_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.621279 autosubmit-4.0.79/test/regression/test_large_experiment_on_moore_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_large_experiment_on_moore_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2456 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/regression/test_large_experiment_on_moore_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_large_experiment_on_moore_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_large_experiment_on_moore_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.621279 autosubmit-4.0.79/test/regression/test_large_experiment_on_moore_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_large_experiment_on_moore_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.589280 autosubmit-4.0.79/test/regression/test_mistral_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.621279 autosubmit-4.0.79/test/regression/test_mistral_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mistral_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2457 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/regression/test_mistral_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      353 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mistral_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mistral_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.621279 autosubmit-4.0.79/test/regression/test_mistral_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mistral_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.589280 autosubmit-4.0.79/test/regression/test_mn3_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.621279 autosubmit-4.0.79/test/regression/test_mn3_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn3_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/regression/test_mn3_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      538 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn3_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn3_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.621279 autosubmit-4.0.79/test/regression/test_mn3_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn3_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.589280 autosubmit-4.0.79/test/regression/test_mn3_with_paramiko_python/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.621279 autosubmit-4.0.79/test/regression/test_mn3_with_paramiko_python/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn3_with_paramiko_python/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2464 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/regression/test_mn3_with_paramiko_python/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn3_with_paramiko_python/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn3_with_paramiko_python/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.621279 autosubmit-4.0.79/test/regression/test_mn3_with_paramiko_python/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/regression/test_mn3_with_paramiko_python/src/TEST_NOLEAP.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.589280 autosubmit-4.0.79/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.621279 autosubmit-4.0.79/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      656 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.621279 autosubmit-4.0.79/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.589280 autosubmit-4.0.79/test/regression/test_mn4_horizontal_wrapper_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.621279 autosubmit-4.0.79/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      647 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.621279 autosubmit-4.0.79/test/regression/test_mn4_horizontal_wrapper_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn4_horizontal_wrapper_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.589280 autosubmit-4.0.79/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.621279 autosubmit-4.0.79/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      656 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.621279 autosubmit-4.0.79/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.589280 autosubmit-4.0.79/test/regression/test_mn4_vertical_wrapper_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.621279 autosubmit-4.0.79/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      640 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      208 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.625279 autosubmit-4.0.79/test/regression/test_mn4_vertical_wrapper_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn4_vertical_wrapper_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.593280 autosubmit-4.0.79/test/regression/test_mn4_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.625279 autosubmit-4.0.79/test/regression/test_mn4_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      586 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn4_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/regression/test_mn4_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      538 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn4_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn4_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.625279 autosubmit-4.0.79/test/regression/test_mn4_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn4_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.593280 autosubmit-4.0.79/test/regression/test_mn4_with_paramiko_python/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.625279 autosubmit-4.0.79/test/regression/test_mn4_with_paramiko_python/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn4_with_paramiko_python/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2464 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/regression/test_mn4_with_paramiko_python/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn4_with_paramiko_python/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_mn4_with_paramiko_python/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.625279 autosubmit-4.0.79/test/regression/test_mn4_with_paramiko_python/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/regression/test_mn4_with_paramiko_python/src/TEST_NOLEAP.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.593280 autosubmit-4.0.79/test/regression/test_moore_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.625279 autosubmit-4.0.79/test/regression/test_moore_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_moore_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2455 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/regression/test_moore_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      352 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_moore_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_moore_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.625279 autosubmit-4.0.79/test/regression/test_moore_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_moore_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.593280 autosubmit-4.0.79/test/regression/test_moore_with_paramiko_python/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.625279 autosubmit-4.0.79/test/regression/test_moore_with_paramiko_python/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_moore_with_paramiko_python/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2457 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/regression/test_moore_with_paramiko_python/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      218 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_moore_with_paramiko_python/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_moore_with_paramiko_python/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.625279 autosubmit-4.0.79/test/regression/test_moore_with_paramiko_python/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/regression/test_moore_with_paramiko_python/src/TEST_NOLEAP.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.593280 autosubmit-4.0.79/test/regression/test_sedema_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.625279 autosubmit-4.0.79/test/regression/test_sedema_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_sedema_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2456 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/regression/test_sedema_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      353 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_sedema_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_sedema_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.625279 autosubmit-4.0.79/test/regression/test_sedema_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_sedema_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.593280 autosubmit-4.0.79/test/regression/test_sedema_with_paramiko_python/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.625279 autosubmit-4.0.79/test/regression/test_sedema_with_paramiko_python/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_sedema_with_paramiko_python/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2458 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/regression/test_sedema_with_paramiko_python/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      218 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_sedema_with_paramiko_python/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/test_sedema_with_paramiko_python/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.625279 autosubmit-4.0.79/test/regression/test_sedema_with_paramiko_python/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/regression/test_sedema_with_paramiko_python/src/TEST_NOLEAP.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2775 2022-11-21 08:34:36.000000 autosubmit-4.0.79/test/regression/tests.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1135 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/regression/tests_commands.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5968 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/regression/tests_log.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5504 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/regression/tests_runner.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3603 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/regression/tests_utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:19:10.629279 autosubmit-4.0.79/test/unit/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2039 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/unit/README_PIP.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-12-20 13:25:07.000000 autosubmit-4.0.79/test/unit/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1104 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/unit/test_basic_config.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4581 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/unit/test_catlog.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13253 2021-10-05 14:18:20.000000 autosubmit-4.0.79/test/unit/test_chunk_date_lib.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13319 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/unit/test_database_managers.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2490 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/unit/test_db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    22969 2023-05-08 14:14:23.000000 autosubmit-4.0.79/test/unit/test_dic_jobs.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2729 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/unit/test_expid.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19073 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/unit/test_history.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12868 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/unit/test_job.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1015 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/unit/test_job_common.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    47843 2023-05-08 14:14:23.000000 autosubmit-4.0.79/test/unit/test_job_graph.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    59633 2023-05-08 14:14:23.000000 autosubmit-4.0.79/test/unit/test_job_grouping.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12769 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/unit/test_job_list.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2374 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/unit/test_job_package.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      815 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/unit/test_log.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3772 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/unit/test_machinefiles_wrapper.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4878 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/unit/test_paramiko_platform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5244 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/unit/test_pjm.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4528 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/unit/test_platform_monitor.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      393 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/unit/test_setup.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2177 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/unit/test_slurm_platform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3130 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/unit/test_statistics.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6724 2023-05-02 11:09:16.000000 autosubmit-4.0.79/test/unit/test_strategies.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    81739 2023-05-08 14:14:23.000000 autosubmit-4.0.79/test/unit/test_wrappers.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.151228 autosubmit-4.0.80/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      226 2023-06-28 10:21:26.000000 autosubmit-4.0.80/.gitignore
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1361 2023-06-28 10:21:26.000000 autosubmit-4.0.80/.gitlab-ci.yml
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      937 2023-06-28 10:21:26.000000 autosubmit-4.0.80/.readthedocs.yaml
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.80/CHANGELOG
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      722 2023-06-28 10:21:26.000000 autosubmit-4.0.80/CONTRIBUTING.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    35147 2021-10-05 14:18:20.000000 autosubmit-4.0.80/LICENSE
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      119 2021-10-05 14:18:20.000000 autosubmit-4.0.80/MANIFEST.in
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3347 2023-06-30 08:32:54.151228 autosubmit-4.0.80/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5651 2023-06-28 10:21:26.000000 autosubmit-4.0.80/README.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2287 2023-06-28 10:21:26.000000 autosubmit-4.0.80/README_PIP.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        7 2023-06-30 08:32:33.000000 autosubmit-4.0.80/VERSION
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.107229 autosubmit-4.0.80/autosubmit/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.80/autosubmit/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   322349 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/autosubmit.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.107229 autosubmit-4.0.80/autosubmit/database/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.80/autosubmit/database/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.107229 autosubmit-4.0.80/autosubmit/database/data/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      258 2021-10-05 14:18:20.000000 autosubmit-4.0.80/autosubmit/database/data/autosubmit.sql
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19910 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/database/db_common.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7593 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/database/db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6065 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/database/db_structure.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.107229 autosubmit-4.0.80/autosubmit/experiment/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.80/autosubmit/experiment/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5280 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/experiment/experiment_common.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8450 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/experiment/statistics.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.107229 autosubmit-4.0.80/autosubmit/git/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.80/autosubmit/git/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13703 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/git/autosubmit_git.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.107229 autosubmit-4.0.80/autosubmit/helpers/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.80/autosubmit/helpers/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5776 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/helpers/autosubmit_helper.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      194 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/helpers/data_transfer.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3304 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/helpers/parameters.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1428 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/helpers/utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.107229 autosubmit-4.0.80/autosubmit/history/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.80/autosubmit/history/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.107229 autosubmit-4.0.80/autosubmit/history/data_classes/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.80/autosubmit/history/data_classes/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2432 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/history/data_classes/experiment_run.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10305 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/history/data_classes/job_data.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.111229 autosubmit-4.0.80/autosubmit/history/database_managers/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.80/autosubmit/history/database_managers/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5688 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/history/database_managers/database_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2409 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/history/database_managers/database_models.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19251 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/history/database_managers/experiment_history_db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6456 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/history/database_managers/experiment_status_db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    18844 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/history/experiment_history.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2382 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/history/experiment_status.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1952 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/history/internal_logging.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.111229 autosubmit-4.0.80/autosubmit/history/platform_monitor/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.80/autosubmit/history/platform_monitor/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.111229 autosubmit-4.0.80/autosubmit/history/platform_monitor/output_examples/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/history/platform_monitor/output_examples/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      185 2022-11-21 08:34:36.000000 autosubmit-4.0.80/autosubmit/history/platform_monitor/output_examples/pending.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      554 2022-11-21 08:34:36.000000 autosubmit-4.0.80/autosubmit/history/platform_monitor/output_examples/wrapper1.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      549 2022-11-21 08:34:36.000000 autosubmit-4.0.80/autosubmit/history/platform_monitor/output_examples/wrapper2.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6105 2022-11-21 08:34:36.000000 autosubmit-4.0.80/autosubmit/history/platform_monitor/output_examples/wrapper_big.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1025 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/history/platform_monitor/platform_monitor.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2298 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/history/platform_monitor/platform_utils.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2475 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/history/platform_monitor/slurm_monitor.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3454 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/history/platform_monitor/slurm_monitor_item.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10951 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/history/strategies.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2784 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/history/utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.111229 autosubmit-4.0.80/autosubmit/job/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.80/autosubmit/job/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    99372 2023-06-28 13:10:30.000000 autosubmit-4.0.80/autosubmit/job/job.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10907 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/job/job_common.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20136 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/job/job_dict.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13797 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/job/job_grouping.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   127858 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/job/job_list.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4609 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/job/job_list_persistence.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3565 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/job/job_package_persistence.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    62148 2023-06-28 10:59:42.000000 autosubmit-4.0.80/autosubmit/job/job_packager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    38100 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/job/job_packages.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11580 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/job/job_utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.111229 autosubmit-4.0.80/autosubmit/monitor/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.80/autosubmit/monitor/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10182 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/monitor/diagram.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    26910 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/monitor/monitor.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1414 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/monitor/utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.111229 autosubmit-4.0.80/autosubmit/notifications/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.80/autosubmit/notifications/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4049 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/notifications/mail_notifier.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1196 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/notifications/notifier.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.111229 autosubmit-4.0.80/autosubmit/platforms/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.80/autosubmit/platforms/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13279 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/ecplatform.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.115229 autosubmit-4.0.80/autosubmit/platforms/headers/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.80/autosubmit/platforms/headers/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5514 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/headers/ec_cca_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4100 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/headers/ec_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1826 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/headers/local_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7391 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/headers/lsf_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2972 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/headers/pbs10_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3497 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/headers/pbs11_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2963 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/headers/pbs12_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5750 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/headers/pjm_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2214 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/headers/ps_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3603 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/headers/sge_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8083 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/headers/slurm_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10469 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/locplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5557 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/lsfplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    53819 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/paramiko_platform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11370 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/paramiko_submitter.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5224 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/pbsplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20846 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/pjmplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    27527 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/platform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4184 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/psplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4617 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/sgeplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    32072 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/slurmplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1316 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/submitter.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.115229 autosubmit-4.0.80/autosubmit/platforms/wrappers/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.80/autosubmit/platforms/wrappers/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    38627 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/wrappers/wrapper_builder.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     9302 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/platforms/wrappers/wrapper_factory.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.115229 autosubmit-4.0.80/autosubmit/statistics/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.80/autosubmit/statistics/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2869 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/statistics/jobs_stat.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6724 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/statistics/statistics.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1818 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/statistics/stats_summary.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1830 2023-06-28 10:21:26.000000 autosubmit-4.0.80/autosubmit/statistics/utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.107229 autosubmit-4.0.80/autosubmit.egg-info/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3347 2023-06-30 08:32:53.000000 autosubmit-4.0.80/autosubmit.egg-info/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13041 2023-06-30 08:32:53.000000 autosubmit-4.0.80/autosubmit.egg-info/SOURCES.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-06-30 08:32:53.000000 autosubmit-4.0.80/autosubmit.egg-info/dependency_links.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      427 2023-06-30 08:32:53.000000 autosubmit-4.0.80/autosubmit.egg-info/requires.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       20 2023-06-30 08:32:53.000000 autosubmit-4.0.80/autosubmit.egg-info/top_level.txt
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.115229 autosubmit-4.0.80/bin/
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     3086 2023-06-28 10:21:26.000000 autosubmit-4.0.80/bin/autosubmit
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.115229 autosubmit-4.0.80/docs/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7869 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/Makefile
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)  1513786 2021-10-05 14:18:20.000000 autosubmit-4.0.80/docs/autosubmit.pdf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.115229 autosubmit-4.0.80/docs/source/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.115229 autosubmit-4.0.80/docs/source/agui/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.115229 autosubmit-4.0.80/docs/source/agui/experiment/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.115229 autosubmit-4.0.80/docs/source/agui/experiment/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   112356 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/experiment/fig/fig_experiment.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1430 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/experiment/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.119229 autosubmit-4.0.80/docs/source/agui/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    25707 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/fig/fig1_gui.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   140255 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/fig/fig2_gui.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   184237 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/fig/fig3_gui.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   114416 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/fig/fig4_gui.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    44047 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/fig/fig5_gui.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   248267 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/fig/fig_ev_1.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   248251 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/fig/fig_tree_1.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   241752 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/fig/fig_tree_2.png
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.123229 autosubmit-4.0.80/docs/source/agui/graph/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.123229 autosubmit-4.0.80/docs/source/agui/graph/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   122929 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/graph/fig/fig_graph_1.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   123449 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/graph/fig/fig_graph_2.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   213843 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/graph/fig/fig_graph_3.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    57438 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/graph/fig/fig_graph_4.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6535 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/graph/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4263 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.123229 autosubmit-4.0.80/docs/source/agui/log/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.127229 autosubmit-4.0.80/docs/source/agui/log/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    25433 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/log/fig/fig_log_1.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   117240 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/log/fig/fig_log_2.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1125 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/log/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.127229 autosubmit-4.0.80/docs/source/agui/performance/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.127229 autosubmit-4.0.80/docs/source/agui/performance/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   174233 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/performance/fig/fig_performance_1.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      910 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/performance/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.127229 autosubmit-4.0.80/docs/source/agui/statistics/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.127229 autosubmit-4.0.80/docs/source/agui/statistics/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    56486 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/statistics/fig/fig_stat_1.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   101911 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/statistics/fig/fig_stat_2.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      988 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/statistics/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.127229 autosubmit-4.0.80/docs/source/agui/tree/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.127229 autosubmit-4.0.80/docs/source/agui/tree/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   114354 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/tree/fig/fig_tree_2.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5756 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/agui/tree/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10217 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/conf.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.131229 autosubmit-4.0.80/docs/source/devguide/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2109 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/devguide/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2124 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.131229 autosubmit-4.0.80/docs/source/installation/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12768 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/installation/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.131229 autosubmit-4.0.80/docs/source/introduction/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   769052 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/introduction/fig1.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    93570 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/introduction/fig2.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    53843 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/introduction/fig3.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6099 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/introduction/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.131229 autosubmit-4.0.80/docs/source/moduledoc/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      130 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/moduledoc/autosubmit.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      445 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/moduledoc/config.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       99 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/moduledoc/database.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       89 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/moduledoc/git.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      128 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/moduledoc/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      185 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/moduledoc/job.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       94 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/moduledoc/monitor.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      547 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/moduledoc/platforms.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.131229 autosubmit-4.0.80/docs/source/qstartguide/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    50473 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/qstartguide/dummy.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     9400 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/qstartguide/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.135228 autosubmit-4.0.80/docs/source/troubleshooting/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    18379 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/troubleshooting/changelog.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    22857 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/troubleshooting/error-codes.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.135228 autosubmit-4.0.80/docs/source/troubleshooting/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    83094 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/troubleshooting/fig/monarch-da.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    68077 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/troubleshooting/fig/new_dependencies_0.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    68077 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/troubleshooting/fig/new_dependencies_1.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2770 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/troubleshooting/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.135228 autosubmit-4.0.80/docs/source/unused_figs/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    49607 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/unused_figs/group_chunk.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    32622 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/unused_figs/horizontal-vertical.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   106298 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/unused_figs/wrapper.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   251472 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/unused_figs/wrapper_expression.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19009 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/unused_figs/wrapper_hybrid.png
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.135228 autosubmit-4.0.80/docs/source/userguide/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.135228 autosubmit-4.0.80/docs/source/userguide/configure/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    30910 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/userguide/configure/develop_a_project.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20565 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/userguide/configure/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.139228 autosubmit-4.0.80/docs/source/userguide/create/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6907 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/userguide/create/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1877 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/userguide/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.139228 autosubmit-4.0.80/docs/source/userguide/manage/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    14283 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/userguide/manage/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.139228 autosubmit-4.0.80/docs/source/userguide/run/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    16002 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/userguide/run/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.139228 autosubmit-4.0.80/docs/source/userguide/wrappers/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.139228 autosubmit-4.0.80/docs/source/userguide/wrappers/fig/
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)   198622 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/userguide/wrappers/fig/dasim.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    23826 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/userguide/wrappers/fig/horizontal_remote.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   308786 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/userguide/wrappers/fig/multiple_wrappers.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    17531 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/userguide/wrappers/fig/rerun.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    33805 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/userguide/wrappers/fig/vertical-horizontal.png
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)    33140 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/userguide/wrappers/fig/vertical-mixed.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11646 2023-06-28 10:21:26.000000 autosubmit-4.0.80/docs/source/userguide/wrappers/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      702 2023-06-28 10:21:26.000000 autosubmit-4.0.80/environment.yml
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.139228 autosubmit-4.0.80/log/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.80/log/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2023-06-28 10:21:26.000000 autosubmit-4.0.80/log/fd_show.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13696 2023-06-28 10:21:26.000000 autosubmit-4.0.80/log/log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      464 2023-06-28 13:40:33.000000 autosubmit-4.0.80/requeriments.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-06-30 08:32:54.151228 autosubmit-4.0.80/setup.cfg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3061 2023-06-28 10:21:26.000000 autosubmit-4.0.80/setup.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.139228 autosubmit-4.0.80/test/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.143228 autosubmit-4.0.80/test/integration/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/integration/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1315 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/integration/test_db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2874 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/integration/test_job.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.143228 autosubmit-4.0.80/test/regression/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       33 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/.gitignore
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2429 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/README
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.143228 autosubmit-4.0.80/test/regression/db/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       90 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/db/.gitignore
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.143228 autosubmit-4.0.80/test/regression/default_conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1368 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/default_conf/platforms.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2946 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/regression/local_asparser_test.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.103229 autosubmit-4.0.80/test/regression/test_ecmwf_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.143228 autosubmit-4.0.80/test/regression/test_ecmwf_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_ecmwf_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2459 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/regression/test_ecmwf_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      577 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_ecmwf_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_ecmwf_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.143228 autosubmit-4.0.80/test/regression/test_ecmwf_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       97 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_ecmwf_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.103229 autosubmit-4.0.80/test/regression/test_large_experiment_on_moore_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.143228 autosubmit-4.0.80/test/regression/test_large_experiment_on_moore_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_large_experiment_on_moore_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2456 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/regression/test_large_experiment_on_moore_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_large_experiment_on_moore_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_large_experiment_on_moore_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.143228 autosubmit-4.0.80/test/regression/test_large_experiment_on_moore_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_large_experiment_on_moore_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.103229 autosubmit-4.0.80/test/regression/test_mistral_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.143228 autosubmit-4.0.80/test/regression/test_mistral_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mistral_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2457 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/regression/test_mistral_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      353 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mistral_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mistral_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.143228 autosubmit-4.0.80/test/regression/test_mistral_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mistral_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.103229 autosubmit-4.0.80/test/regression/test_mn3_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.143228 autosubmit-4.0.80/test/regression/test_mn3_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn3_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/regression/test_mn3_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      538 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn3_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn3_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.143228 autosubmit-4.0.80/test/regression/test_mn3_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn3_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.103229 autosubmit-4.0.80/test/regression/test_mn3_with_paramiko_python/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.143228 autosubmit-4.0.80/test/regression/test_mn3_with_paramiko_python/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn3_with_paramiko_python/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2464 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/regression/test_mn3_with_paramiko_python/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn3_with_paramiko_python/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn3_with_paramiko_python/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.143228 autosubmit-4.0.80/test/regression/test_mn3_with_paramiko_python/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/regression/test_mn3_with_paramiko_python/src/TEST_NOLEAP.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.103229 autosubmit-4.0.80/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.147228 autosubmit-4.0.80/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      656 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.147228 autosubmit-4.0.80/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.103229 autosubmit-4.0.80/test/regression/test_mn4_horizontal_wrapper_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.147228 autosubmit-4.0.80/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      647 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.147228 autosubmit-4.0.80/test/regression/test_mn4_horizontal_wrapper_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn4_horizontal_wrapper_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.103229 autosubmit-4.0.80/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.147228 autosubmit-4.0.80/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      656 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.147228 autosubmit-4.0.80/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.103229 autosubmit-4.0.80/test/regression/test_mn4_vertical_wrapper_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.147228 autosubmit-4.0.80/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      640 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      208 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.147228 autosubmit-4.0.80/test/regression/test_mn4_vertical_wrapper_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn4_vertical_wrapper_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.103229 autosubmit-4.0.80/test/regression/test_mn4_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.147228 autosubmit-4.0.80/test/regression/test_mn4_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      586 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn4_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/regression/test_mn4_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      538 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn4_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn4_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.147228 autosubmit-4.0.80/test/regression/test_mn4_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn4_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.103229 autosubmit-4.0.80/test/regression/test_mn4_with_paramiko_python/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.147228 autosubmit-4.0.80/test/regression/test_mn4_with_paramiko_python/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn4_with_paramiko_python/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2464 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/regression/test_mn4_with_paramiko_python/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn4_with_paramiko_python/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_mn4_with_paramiko_python/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.147228 autosubmit-4.0.80/test/regression/test_mn4_with_paramiko_python/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/regression/test_mn4_with_paramiko_python/src/TEST_NOLEAP.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.103229 autosubmit-4.0.80/test/regression/test_moore_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.147228 autosubmit-4.0.80/test/regression/test_moore_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_moore_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2455 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/regression/test_moore_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      352 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_moore_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_moore_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.147228 autosubmit-4.0.80/test/regression/test_moore_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_moore_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.103229 autosubmit-4.0.80/test/regression/test_moore_with_paramiko_python/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.147228 autosubmit-4.0.80/test/regression/test_moore_with_paramiko_python/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_moore_with_paramiko_python/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2457 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/regression/test_moore_with_paramiko_python/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      218 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_moore_with_paramiko_python/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_moore_with_paramiko_python/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.151228 autosubmit-4.0.80/test/regression/test_moore_with_paramiko_python/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/regression/test_moore_with_paramiko_python/src/TEST_NOLEAP.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.103229 autosubmit-4.0.80/test/regression/test_sedema_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.151228 autosubmit-4.0.80/test/regression/test_sedema_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_sedema_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2456 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/regression/test_sedema_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      353 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_sedema_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_sedema_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.151228 autosubmit-4.0.80/test/regression/test_sedema_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_sedema_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.103229 autosubmit-4.0.80/test/regression/test_sedema_with_paramiko_python/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.151228 autosubmit-4.0.80/test/regression/test_sedema_with_paramiko_python/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_sedema_with_paramiko_python/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2458 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/regression/test_sedema_with_paramiko_python/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      218 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_sedema_with_paramiko_python/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/test_sedema_with_paramiko_python/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.151228 autosubmit-4.0.80/test/regression/test_sedema_with_paramiko_python/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/regression/test_sedema_with_paramiko_python/src/TEST_NOLEAP.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2775 2022-11-21 08:34:36.000000 autosubmit-4.0.80/test/regression/tests.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1135 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/regression/tests_commands.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5968 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/regression/tests_log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5504 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/regression/tests_runner.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3603 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/regression/tests_utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-30 08:32:54.151228 autosubmit-4.0.80/test/unit/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2039 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/README_PIP.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-12-20 13:25:07.000000 autosubmit-4.0.80/test/unit/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1104 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_basic_config.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4581 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_catlog.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13253 2021-10-05 14:18:20.000000 autosubmit-4.0.80/test/unit/test_chunk_date_lib.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13319 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_database_managers.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2490 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     9696 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_dependencies.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    22969 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_dic_jobs.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4664 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_expid.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19073 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_history.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    14748 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_job.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1015 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_job_common.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    47843 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_job_graph.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    59633 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_job_grouping.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12769 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_job_list.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8531 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_job_package.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      815 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3772 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_machinefiles_wrapper.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4878 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_paramiko_platform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5244 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_pjm.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4528 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_platform_monitor.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      393 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_setup.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2887 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_slurm_platform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3130 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_statistics.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6724 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_strategies.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    81739 2023-06-28 10:21:26.000000 autosubmit-4.0.80/test/unit/test_wrappers.py
```

### Comparing `autosubmit-4.0.79/.gitlab-ci.yml` & `autosubmit-4.0.80/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/CONTRIBUTING.md` & `autosubmit-4.0.80/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/LICENSE` & `autosubmit-4.0.80/LICENSE`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/PKG-INFO` & `autosubmit-4.0.80/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmit
-Version: 4.0.79
+Version: 4.0.80
 Summary: Autosubmit is a Python-based workflow manager to create, manage and monitor complex tasks involving different substeps, such as scientific computational experiments. These workflows may involve multiple computing systems for their completion, from HPCs to post-processing clusters or workstations. Autosubmit can orchestrate all the tasks integrating the workflow by managing their dependencies, interfacing with all the platforms involved, and handling eventual errors.
 Home-page: http://www.bsc.es/projects/earthscience/autosubmit/
 Download-URL: https://earth.bsc.es/wiki/doku.php?id=tools:autosubmit
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
 License: GNU GPL v3
 Keywords: climate,weather,workflow,HPC
```

### Comparing `autosubmit-4.0.79/README.md` & `autosubmit-4.0.80/README.md`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/README_PIP.md` & `autosubmit-4.0.80/README_PIP.md`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/autosubmit.py` & `autosubmit-4.0.80/autosubmit/autosubmit.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,56 +25,49 @@
 from .platforms.paramiko_submitter import ParamikoSubmitter
 from .platforms.platform import Platform
 from .notifications.notifier import Notifier
 from .notifications.mail_notifier import MailNotifier
 from bscearth.utils.date import date2str
 from pathlib import Path
 from autosubmitconfigparser.config.yamlparser import YAMLParserFactory
+from ruamel.yaml import YAML
 from configparser import ConfigParser
 
 from .monitor.monitor import Monitor
 from .database.db_common import get_autosubmit_version, check_experiment_exists
-from .database.db_common import delete_experiment, update_experiment_descrip_version, get_experiment_descrip
+from .database.db_common import delete_experiment, get_experiment_descrip
 from .database.db_structure import get_structure
 from .experiment.experiment_common import copy_experiment
 from .experiment.experiment_common import new_experiment
 from .database.db_common import create_db
 from .job.job_grouping import JobGrouping
 from .job.job_list_persistence import JobListPersistencePkl
 from .job.job_list_persistence import JobListPersistenceDb
 from .job.job_package_persistence import JobPackagePersistence
-from .job.job_packages import JobPackageThread, JobPackageBase
 from .job.job_list import JobList
 from .job.job_utils import SubJob, SubJobManager
-from .job.job import Job
+from autosubmit.helpers.parameters import PARAMETERS
 from .git.autosubmit_git import AutosubmitGit
 from .job.job_common import Status
 from autosubmitconfigparser.config.configcommon import AutosubmitConfig
 from autosubmitconfigparser.config.basicconfig import BasicConfig
 import locale
 from distutils.util import strtobool
 from log.log import Log, AutosubmitError, AutosubmitCritical
-from typing import Set, Union
+from typing import Dict, Set, Tuple, Union
 from autosubmit.database.db_common import update_experiment_descrip_version
-
-import sqlite3
-
-# try:
-#    import pythondialog as dialog
-# except Exception:
 dialog = None
 from time import sleep
 import argparse
 import subprocess
 import json
 import tarfile
 import time
 import copy
 import os
-import glob
 import pwd
 import sys
 import shutil
 import re
 import random
 import signal
 import datetime
@@ -802,14 +795,15 @@
 
             if not os.path.exists(tmp_path):
                 os.mkdir(tmp_path)
             if not os.path.exists(aslogs_path):
                 os.mkdir(aslogs_path)
             if owner:
                 os.chmod(tmp_path, 0o775)
+
                 Log.set_file(os.path.join(aslogs_path, args.command + '.log'), "out", log_level)
                 Log.set_file(os.path.join(aslogs_path, args.command + '_err.log'), "err")
                 if args.command in ["run"]:
                     if os.path.exists(os.path.join(aslogs_path, 'jobs_active_status.log')):
                         os.remove(os.path.join(aslogs_path, 'jobs_active_status.log'))
                     if os.path.exists(os.path.join(aslogs_path, 'jobs_failed_status.log')):
                         os.remove(os.path.join(aslogs_path, 'jobs_failed_status.log'))
@@ -1034,33 +1028,111 @@
             # if ends with .conf convert it to AS4 yaml file
             if conf_file.endswith(".conf"):
                 try:
                     AutosubmitConfig.ini_to_yaml(os.path.join(BasicConfig.LOCAL_ROOT_DIR, exp_id,"conf"),
                                                  os.path.join(BasicConfig.LOCAL_ROOT_DIR, exp_id,"conf",conf_file.replace(copy_id,exp_id)))
                 except Exception as e:
                     Log.warning("Error converting {0} to yml: {1}".format(conf_file.replace(copy_id,exp_id),str(e)))
+
     @staticmethod
-    def generate_as_config(exp_id,dummy=False,minimal_configuration=False,local=False):
-        # obtain from autosubmitconfigparser package
-        # get all as_conf_files from autosubmitconfigparser package
-        files = resource_listdir('autosubmitconfigparser.config', 'files')
-        for as_conf_file in files:
+    def generate_as_config(
+            exp_id: str,
+            dummy: bool=False,
+            minimal_configuration: bool=False,
+            local: bool=False,
+            parameters: Dict[str, Union[Dict, List, str]] = None
+    ) -> None:
+        """Retrieve the configuration from autosubmitconfigparser package.
+
+        :param exp_id: Experiment ID
+        :param dummy: Whether the experiment is a dummy one or not.
+        :param minimal_configuration: Whether the experiment is configured with minimal configuration or not.
+        :param local: Whether the experiment project type is local or not.
+        :param parameters: Optional list of parameters to be used when processing the configuration files.
+        :return: None
+        """
+
+        def add_comments_to_yaml(yaml_data, parameters, keys=None):
+            """A recursive generator that visits every leaf node and yields the flatten parameter."""
+            if keys is None:
+                keys = []
+            if isinstance(yaml_data, dict):
+                for key, value in yaml_data.items():
+                    if isinstance(value, dict):
+                        add_comments_to_yaml(value, parameters, [*keys, key])
+                    else:
+                        parameter_key = '.'.join([*keys, key]).upper()
+                        if parameter_key in parameters:
+                            comment = parameters[parameter_key]
+                            yaml_data.yaml_set_comment_before_after_key(key, before=comment, indent=yaml_data.lc.col)
+
+        def recurse_into_parameters(parameters: Dict[str, Union[Dict, List, str]], keys=None) -> Tuple[str, str]:
+            """Recurse into the ``PARAMETERS`` dictionary, and emits a dictionary.
+
+            The key in the dictionary is the flattened parameter key/ID, and the value
+            is the parameter documentation.
+
+            :param parameters: Global parameters dictionary.
+            :param keys: For recursion, the accumulated keys.
+            :return: A dictionary with the
+            """
+            if keys is None:
+                keys = []
+            if isinstance(parameters, dict):
+                for key, value in parameters.items():
+                    if isinstance(value, dict):
+                        yield from recurse_into_parameters(value, [*keys, key])
+                    else:
+                        key = key.upper()
+                        # Here's the reason why ``recurse_into_yaml`` and ``recurse_into_parameters``
+                        # are not one single ``recurse_into_dict`` function. The parameters have some
+                        # keys that contain ``${PARENT}.key`` as that is how they are displayed in
+                        # the Sphinx docs. So we need to detect it and handle it. p.s. We also know
+                        # the max-length of the parameters dict is 2! See the ``autosubmit.helpers.parameters``
+                        # module for more.
+                        if not key.startswith(f'{keys[0]}.'):
+                            yield '.'.join([*keys, key]).upper(), value
+                        else:
+                            yield key, value
+
+        template_files = resource_listdir('autosubmitconfigparser.config', 'files')
+        if parameters is None:
+            parameters = PARAMETERS
+        parameter_comments = dict(recurse_into_parameters(parameters))
+
+        for as_conf_file in template_files:
+            origin = resource_filename('autosubmitconfigparser.config', str(Path('files', as_conf_file)))
+            target = None
+
             if dummy:
-                if as_conf_file.endswith("dummy.yml"):
-                    shutil.copy(resource_filename('autosubmitconfigparser.config', 'files/'+as_conf_file), os.path.join(BasicConfig.LOCAL_ROOT_DIR, exp_id, "conf",as_conf_file.split("-")[0]+"_"+exp_id+".yml"))
+                if as_conf_file.endswith('dummy.yml'):
+                    file_name = f'{as_conf_file.split("-")[0]}_{exp_id}.yml'
+                    target = Path(BasicConfig.LOCAL_ROOT_DIR, exp_id, 'conf', file_name)
             elif minimal_configuration:
-                if not local:
-                    if as_conf_file.endswith("git-minimal.yml"):
-                        shutil.copy(resource_filename('autosubmitconfigparser.config', 'files/'+as_conf_file), os.path.join(BasicConfig.LOCAL_ROOT_DIR, exp_id, "conf","minimal.yml"))
-                else:
-                    if as_conf_file.endswith("local-minimal.yml"):
-                        shutil.copy(resource_filename('autosubmitconfigparser.config', 'files/' + as_conf_file),os.path.join(BasicConfig.LOCAL_ROOT_DIR, exp_id, "conf", "minimal.yml"))
+                if (not local and as_conf_file.endswith('git-minimal.yml')) or as_conf_file.endswith("local-minimal.yml"):
+                    target = Path(BasicConfig.LOCAL_ROOT_DIR, exp_id, 'conf/minimal.yml')
             else:
-                if not as_conf_file.endswith("dummy.yml") and not as_conf_file.endswith("minimal.yml"):
-                    shutil.copy(resource_filename('autosubmitconfigparser.config', 'files/'+as_conf_file), os.path.join(BasicConfig.LOCAL_ROOT_DIR, exp_id, "conf",as_conf_file[:-4]+"_"+exp_id+".yml"))
+                if not as_conf_file.endswith('dummy.yml') and not as_conf_file.endswith('minimal.yml'):
+                    file_name = f'{Path(as_conf_file).stem}_{exp_id}.yml'
+                    target = Path(BasicConfig.LOCAL_ROOT_DIR, exp_id, 'conf', file_name)
+
+            # Here we annotate the copied configuration with comments from the Python source code.
+            # This means the YAML configuration files contain the exact same comments from our
+            # Python code, which is also displayed in our Sphinx documentation (be careful with what
+            # you write!)
+            #
+            # The previous code was simply doing a shutil(origin, target). This does not modify
+            # much that logic, except we add comments before writing the copy...
+            if origin and target:
+                with open(origin, 'r') as input, open(target, 'w+') as output:
+                    yaml = YAML(typ='rt')
+                    yaml_data = yaml.load(input)
+                    add_comments_to_yaml(yaml_data, parameter_comments)
+                    yaml.dump(yaml_data, output)
+
     @staticmethod
     def as_conf_default_values(exp_id,hpc="local",minimal_configuration=False,git_repo="",git_branch="main",git_as_conf=""):
         """
         Replace default values in as_conf files
         :param exp_id: experiment id
         :param hpc: platform
         :param minimal_configuration: minimal configuration
@@ -3847,16 +3919,16 @@
         :type jobs_conf: bool
         :param expid: experiment identifier
         :type expid: str
         """
         try:
             Autosubmit._check_ownership(expid, raise_error=True)
             as_conf = AutosubmitConfig(expid, BasicConfig, YAMLParserFactory())
-            # as_conf.reload(force_load=True)
-            as_conf.check_conf_files(False)
+            as_conf.reload(force_load=True)
+            #as_conf.check_conf_files(False)
         except (AutosubmitError, AutosubmitCritical):
             raise
         except BaseException as e:
             raise AutosubmitCritical("Error while reading the configuration files", 7064, str(e))
         try:
             if "Expdef" in as_conf.wrong_config:
                 as_conf.show_messages()
@@ -4400,25 +4472,25 @@
             with portalocker.Lock(os.path.join(tmp_path, 'autosubmit.lock'), timeout=1) as fh:
                 try:
                     Log.info(
                         "Preparing .lock file to avoid multiple instances with same expid.")
 
                     as_conf = AutosubmitConfig(expid, BasicConfig, YAMLParserFactory())
                     # Get original configuration
-                    as_conf.check_conf_files(running_time=False, only_experiment_data=True, no_log=True)
+                    as_conf.reload(force_load=True,only_experiment_data=True)
                     # Getting output type provided by the user in config, 'pdf' as default
                     try:
                         if not Autosubmit._copy_code(as_conf, expid, as_conf.experiment_data.get("PROJECT",{}).get("PROJECT_TYPE","none"), False):
                             return False
                     except AutosubmitCritical as e:
                         raise
                     except BaseException as e:
                         raise AutosubmitCritical("Error obtaining the project data, check the parameters related to PROJECT and GIT/SVN or LOCAL sections", code=7014,trace=str(e))
                     # Update configuration with the new config in the dist ( if any )
-                    as_conf.check_conf_files(running_time=False,force_load=True, only_experiment_data=False, no_log=False)
+                    as_conf.check_conf_files(running_time=False,force_load=True, no_log=False)
                     if len(as_conf.experiment_data.get("JOBS",{})) == 0 and "CUSTOM_CONFIG" in as_conf.experiment_data.get("DEFAULT",{}):
                         raise AutosubmitCritical(f'Job list is empty\nCheck if there are YML files in {as_conf.experiment_data.get("DEFAULT","").get("CUSTOM_CONFIG","")}', code=7015)
                     output_type = as_conf.get_output_type()
 
                     if not os.path.exists(os.path.join(exp_path, "pkl")):
                         raise AutosubmitCritical(
                             "The pkl folder doesn't exists. Make sure that the 'pkl' folder exists in the following path: {}".format(
@@ -4546,14 +4618,17 @@
                                 job.parents = job.parents - referenced_jobs_to_remove
                             Autosubmit.generate_scripts_andor_wrappers(
                                 as_conf, job_list_wrappers, jobs_wr, packages_persistence, True)
 
                             packages = packages_persistence.load(True)
                         else:
                             packages = None
+                        Log.info("\nSaving unified data..")
+                        as_conf.save()
+                        Log.info("")
 
                         Log.info("\nPlotting the jobs list...")
                         monitor_exp = Monitor()
                         # if output is set, use output
                         monitor_exp.generate_output(expid, job_list.get_job_list(),
                                                     os.path.join(
                                                         exp_path, "/tmp/LOG_", expid),
```

### Comparing `autosubmit-4.0.79/autosubmit/database/db_common.py` & `autosubmit-4.0.80/autosubmit/database/db_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/database/db_manager.py` & `autosubmit-4.0.80/autosubmit/database/db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/database/db_structure.py` & `autosubmit-4.0.80/autosubmit/database/db_structure.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/experiment/experiment_common.py` & `autosubmit-4.0.80/autosubmit/experiment/experiment_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/experiment/statistics.py` & `autosubmit-4.0.80/autosubmit/experiment/statistics.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/git/autosubmit_git.py` & `autosubmit-4.0.80/autosubmit/git/autosubmit_git.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/helpers/autosubmit_helper.py` & `autosubmit-4.0.80/autosubmit/helpers/autosubmit_helper.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/helpers/utils.py` & `autosubmit-4.0.80/autosubmit/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/history/data_classes/experiment_run.py` & `autosubmit-4.0.80/autosubmit/history/data_classes/experiment_run.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/history/data_classes/job_data.py` & `autosubmit-4.0.80/autosubmit/history/data_classes/job_data.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/history/database_managers/database_manager.py` & `autosubmit-4.0.80/autosubmit/history/database_managers/database_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/history/database_managers/database_models.py` & `autosubmit-4.0.80/autosubmit/history/database_managers/database_models.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/history/database_managers/experiment_history_db_manager.py` & `autosubmit-4.0.80/autosubmit/history/database_managers/experiment_history_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/history/database_managers/experiment_status_db_manager.py` & `autosubmit-4.0.80/autosubmit/history/database_managers/experiment_status_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/history/experiment_history.py` & `autosubmit-4.0.80/autosubmit/history/experiment_history.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/history/experiment_status.py` & `autosubmit-4.0.80/autosubmit/history/experiment_status.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/history/internal_logging.py` & `autosubmit-4.0.80/autosubmit/history/internal_logging.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/history/platform_monitor/output_examples/wrapper1.txt` & `autosubmit-4.0.80/autosubmit/history/platform_monitor/output_examples/wrapper1.txt`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/history/platform_monitor/output_examples/wrapper2.txt` & `autosubmit-4.0.80/autosubmit/history/platform_monitor/output_examples/wrapper2.txt`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/history/platform_monitor/output_examples/wrapper_big.txt` & `autosubmit-4.0.80/autosubmit/history/platform_monitor/output_examples/wrapper_big.txt`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/history/platform_monitor/platform_monitor.py` & `autosubmit-4.0.80/autosubmit/history/platform_monitor/platform_monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/history/platform_monitor/platform_utils.py` & `autosubmit-4.0.80/autosubmit/history/platform_monitor/platform_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/history/platform_monitor/slurm_monitor.py` & `autosubmit-4.0.80/autosubmit/history/platform_monitor/slurm_monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/history/platform_monitor/slurm_monitor_item.py` & `autosubmit-4.0.80/autosubmit/history/platform_monitor/slurm_monitor_item.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/history/strategies.py` & `autosubmit-4.0.80/autosubmit/history/strategies.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/history/utils.py` & `autosubmit-4.0.80/autosubmit/history/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/job/job.py` & `autosubmit-4.0.80/autosubmit/job/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,91 +42,145 @@
 from bscearth.utils.date import date2str, parse_date, previous_day, chunk_end_date, chunk_start_date, Log, subs_dates
 from time import sleep
 from threading import Thread
 from autosubmit.platforms.paramiko_submitter import ParamikoSubmitter
 from log.log import Log, AutosubmitCritical, AutosubmitError
 from typing import List, Union
 from functools import reduce
-Log.get_logger("Autosubmit")
 from autosubmitconfigparser.config.yamlparser import YAMLParserFactory
+from autosubmit.helpers.parameters import autosubmit_parameter, autosubmit_parameters
+
+Log.get_logger("Autosubmit")
 
 # A wrapper for encapsulate threads , TODO: Python 3+ to be replaced by the < from concurrent.futures >
 
 
 def threaded(fn):
     def wrapper(*args, **kwargs):
         thread = Thread(target=fn, args=args, kwargs=kwargs)
         thread.name = "JOB_" + str(args[0].name)
         thread.start()
         return thread
     return wrapper
 
 
+# This decorator contains groups of parameters, with each
+# parameter described. This is only for parameters which
+# are not properties of Job. Otherwise, please use the
+# ``autosubmit_parameter`` (singular!) decorator for the
+# ``@property`` annotated members. The variable groups
+# are cumulative, so you can add to ``job``, for instance,
+# in multiple files as long as the variable names are
+# unique per group.
+@autosubmit_parameters(
+    parameters={
+        'chunk': {
+            'day_before': 'Day before the start date.',
+            'chunk_end_in_days': 'Days passed from the start of the simulation until the end of the chunk.',
+            'chunk_start_date': 'Chunk start date.',
+            'chunk_start_year': 'Chunk start year.',
+            'chunk_start_month': 'Chunk start month.',
+            'chunk_start_day': 'Chunk start day.',
+            'chunk_start_hour': 'Chunk start hour.',
+            'chunk_end_date': 'Chunk end date.',
+            'chunk_end_year': 'Chunk end year.',
+            'chunk_end_month': 'Chunk end month.',
+            'chunk_end_day': 'Chunk end day.',
+            'chunk_end_hour': 'Chunk end hour.',
+            'prev': 'Days since start date at the chunk\'s start.',
+            'chunk_first': 'True if the current chunk is the first, false otherwise.',
+            'chunk_last': 'True if the current chunk is the last, false otherwise.',
+            'run_days': 'Chunk length in days.',
+            'notify_on': 'Determine the job statuses you want to be notified.'
+        },
+        'config': {
+            'config.autosubmit_version': 'Current version of Autosubmit.',
+            'config.totaljobs': 'Total number of jobs in the workflow.',
+            'config.maxwaitingjobs': 'Maximum number of jobs permitted in the waiting status.'
+        },
+        'experiment': {
+            'experiment.datelist': 'List of start dates',
+            'experiment.calendar': 'Calendar used for the experiment. Can be standard or noleap.',
+            'experiment.chunksize': 'Size of each chunk.',
+            'experiment.numchunks': 'Number of chunks of the experiment.',
+            'experiment.chunksizeunit': 'Unit of the chunk size. Can be hour, day, month, or year.',
+            'experiment.members': 'List of members.'
+        },
+        'default': {
+            'default.expid': 'Job experiment ID.',
+            'default.hpcarch': 'Default HPC platform name.',
+            'default.custom_config': 'Custom configuration location.',
+        },
+        'job': {
+            'rootdir': 'Experiment folder path.',
+            'projdir': 'Project folder path.',
+            'nummembers': 'Number of members of the experiment.'
+        },
+        'project': {
+            'project.project_type': 'Type of the project.',
+            'project.project_destination': 'Folder to hold the project sources.'
+        }
+    }
+)
 class Job(object):
-    """
-    Class to handle all the tasks with Jobs at HPC.
+    """Class to handle all the tasks with Jobs at HPC.
+
     A job is created by default with a name, a jobid, a status and a type.
     It can have children and parents. The inheritance reflects the dependency between jobs.
-    If Job2 must wait until Job1 is completed then Job2 is a child of Job1. Inversely Job1 is a parent of Job2
-
-    :param name: job's name
-    :type name: str
-    :param job_id: job's id
-    :type job_id: int
-    :param status: job initial status
-    :type status: Status
-    :param priority: job's priority
-    :type priority: int
+    If Job2 must wait until Job1 is completed then Job2 is a child of Job1.
+    Inversely Job1 is a parent of Job2
     """
 
     CHECK_ON_SUBMISSION = 'on_submission'
 
     def __str__(self):
         return "{0} STATUS: {1}".format(self.name, self.status)
 
     def __init__(self, name, job_id, status, priority):
+        self.splits = None
         self.script_name_wrapper = None
         self.delay_end = datetime.datetime.now()
-        self.delay_retrials = "0"
+        self._delay_retrials = "0"
         self.wrapper_type = None
         self._wrapper_queue = None
         self._platform = None
         self._queue = None
         self._partition = None
 
         self.retry_delay = "0"
         self.platform_name = None # type: str
-        self.section = None # type: str
-        self.wallclock = None # type: str
+        #: (str): Type of the job, as given on job configuration file. (job: TASKTYPE)
+        self._section = None # type: str
+        self._wallclock = None # type: str
         self.wchunkinc = None
-        self.tasks = '1'
-        self.nodes = ""
+        self._tasks = '1'
+        self._nodes = ""
         self.default_parameters = {'d': '%d%', 'd_': '%d_%', 'Y': '%Y%', 'Y_': '%Y_%',
                               'M': '%M%', 'M_': '%M_%', 'm': '%m%', 'm_': '%m_%'}
-        self.threads = '1'
-        self.processors = '1'
-        self.memory = ''
-        self.memory_per_task = ''
-        self.chunk = None
-        self.member = None
+        self._threads = '1'
+        self._processors = '1'
+        self._memory = ''
+        self._memory_per_task = ''
+        self._chunk = None
+        self._member = None
         self.date = None
         self.name = name
-        self.split = None
-        self.delay = None
-        self.frequency = None
-        self.synchronize = None
+        self._split = None
+        self._delay = None
+        self._frequency = None
+        self._synchronize = None
         self.skippable = False
         self.repacked = 0
         self._long_name = None
         self.long_name = name
         self.date_format = ''
         self.type = Type.BASH
-        self.hyperthreading = "none"
-        self.scratch_free_space = None
-        self.custom_directives = []
+        self._hyperthreading = "none"
+        self._scratch_free_space = None
+        self._custom_directives = []
         self.undefined_variables = set()
         self.log_retries = 5
         self.id = job_id
         self.file = None
         self.additional_files = []
         self.executable = None
         self.x11 = False
@@ -136,59 +190,278 @@
         self.status = status
         self.prev_status = status
         self.old_status = self.status
         self.new_status = status
         self.priority = priority
         self._parents = set()
         self._children = set()
-        self.fail_count = 0
+        #: (int) Number of failed attempts to run this job. (FAIL_COUNT)
+        self._fail_count = 0
         self.expid = name.split('_')[0] # type: str
         self.parameters = dict()
         self._tmp_path = os.path.join(
             BasicConfig.LOCAL_ROOT_DIR, self.expid, BasicConfig.LOCAL_TMP_DIR)
         self.write_start = False
         self._platform = None
         self.check = 'true'
         self.check_warnings = False
-        self.packed = False
+        self._packed = False
         self.hold = False # type: bool
         self.distance_weight = 0
         self.level = 0
-        self.export = "none"
-        self.dependencies = []
+        self._export = "none"
+        self._dependencies = []
         self.running = "once"
         self.start_time = None
         self.edge_info = dict()
         self.total_jobs = None
         self.max_waiting_jobs = None
         self.exclusive = ""
+
+    @property
+    @autosubmit_parameter(name='tasktype')
+    def section(self):
+        """Type of the job, as given on job configuration file."""
+        return self._section
+
+    @section.setter
+    def section(self, value):
+        self._section = value
+
+    @property
+    @autosubmit_parameter(name='jobname')
+    def name(self):
+        """Current job full name."""
+        return self._name
+
+    @name.setter
+    def name(self, value):
+        self._name = value
+
+    @property
+    @autosubmit_parameter(name='fail_count')
+    def fail_count(self):
+        """Number of failed attempts to run this job."""
+        return self._fail_count
+
+    @fail_count.setter
+    def fail_count(self, value):
+        self._fail_count = value
+
+    @property
+    @autosubmit_parameter(name='sdate')
+    def sdate(self):
+        """Current start date."""
+        return date2str(self.date, self.date_format)
+
+    @property
+    @autosubmit_parameter(name='member')
+    def member(self):
+        """Current member."""
+        return self._member
+
+    @member.setter
+    def member(self, value):
+        self._member = value
+
+    @property
+    @autosubmit_parameter(name='chunk')
+    def chunk(self):
+        """Current chunk."""
+        return self._chunk
+
+    @chunk.setter
+    def chunk(self, value):
+        self._chunk = value
+
+    @property
+    @autosubmit_parameter(name='split')
+    def split(self):
+        """Current split."""
+        return self._split
+
+    @split.setter
+    def split(self, value):
+        self._split = value
+
+    @property
+    @autosubmit_parameter(name='delay')
+    def delay(self):
+        """Current delay."""
+        return self._delay
+
+    @delay.setter
+    def delay(self, value):
+        self._delay = value
+
+    @property
+    @autosubmit_parameter(name='wallclock')
+    def wallclock(self):
+        """Duration for which nodes used by job will remain allocated."""
+        return self._wallclock
+
+    @wallclock.setter
+    def wallclock(self, value):
+        self._wallclock = value
+
+    @property
+    @autosubmit_parameter(name='hyperthreading')
+    def hyperthreading(self):
+        """Detects if hyperthreading is enabled or not."""
+        return self._hyperthreading
+
+    @hyperthreading.setter
+    def hyperthreading(self, value):
+        self._hyperthreading = value
+
+    @property
+    @autosubmit_parameter(name='nodes')
+    def nodes(self):
+        """Number of nodes that the job will use."""
+        return self._nodes
+
+    @nodes.setter
+    def nodes(self, value):
+        self._nodes = value
+
+    @property
+    @autosubmit_parameter(name=['numthreads', 'threads', 'cpus_per_task'])
+    def threads(self):
+        """Number of threads that the job will use."""
+        return self._threads
+
+    @threads.setter
+    def threads(self, value):
+        self._threads = value
+
+    @property
+    @autosubmit_parameter(name=['numtask', 'tasks', 'tasks_per_node'])
+    def tasks(self):
+        """Number of tasks that the job will use."""
+        return self._tasks
+
+    @tasks.setter
+    def tasks(self, value):
+        self._tasks = value
+
+    @property
+    @autosubmit_parameter(name='scratch_free_space')
+    def scratch_free_space(self):
+        """Percentage of free space required on the ``scratch``."""
+        return self._scratch_free_space
+
+    @scratch_free_space.setter
+    def scratch_free_space(self, value):
+        self._scratch_free_space = value
+
+    @property
+    @autosubmit_parameter(name='memory')
+    def memory(self):
+        """Memory requested for the job."""
+        return self._memory
+
+    @memory.setter
+    def memory(self, value):
+        self._memory = value
+
+    @property
+    @autosubmit_parameter(name='memory_per_task')
+    def memory_per_task(self):
+        """Memory requested per task."""
+        return self._memory_per_task
+
+    @memory_per_task.setter
+    def memory_per_task(self, value):
+        self._memory_per_task = value
+
+    @property
+    @autosubmit_parameter(name='frequency')
+    def frequency(self):
+        """TODO."""
+        return self._frequency
+
+    @frequency.setter
+    def frequency(self, value):
+        self._frequency = value
+
+    @property
+    @autosubmit_parameter(name='synchronize')
+    def synchronize(self):
+        """TODO."""
+        return self._synchronize
+
+    @synchronize.setter
+    def synchronize(self, value):
+        self._synchronize = value
+
+    @property
+    @autosubmit_parameter(name='dependencies')
+    def dependencies(self):
+        """Current job dependencies."""
+        return self._dependencies
+
+    @dependencies.setter
+    def dependencies(self, value):
+        self._dependencies = value
+
+    @property
+    @autosubmit_parameter(name='delay_retrials')
+    def delay_retrials(self):
+        """TODO"""
+        return self._delay_retrials
+
+    @delay_retrials.setter
+    def delay_retrials(self, value):
+        self._delay_retrials = value
+
+    @property
+    @autosubmit_parameter(name='packed')
+    def packed(self):
+        """TODO"""
+        return self._packed
+
+    @packed.setter
+    def packed(self, value):
+        self._packed = value
+
+    @property
+    @autosubmit_parameter(name='export')
+    def export(self):
+        """TODO."""
+        return self._export
+
+    @export.setter
+    def export(self, value):
+        self._export = value
+
+    @property
+    @autosubmit_parameter(name='custom_directives')
+    def custom_directives(self):
+        """List of custom directives."""
+        return self._custom_directives
+
+    @custom_directives.setter
+    def custom_directives(self, value):
+        self._custom_directives = value
+    @property
+    @autosubmit_parameter(name='splits')
+    def splits(self):
+        """Max number of splits."""
+        return self._splits
+    @splits.setter
+    def splits(self, value):
+        self._splits = value
+
     def __getstate__(self):
         odict = self.__dict__
         if '_platform' in odict:
             odict = odict.copy()  # copy the dict since we change it
             del odict['_platform']  # remove filehandle entry
         return odict
 
-    # def __str__(self):
-    #     return self.name
-
-    def print_job(self):
-        """
-        Prints debug information about the job
-        """
-        Log.debug('NAME: {0}', self.name)
-        Log.debug('JOBID: {0}', self.id)
-        Log.debug('STATUS: {0}', self.status)
-        Log.debug('PRIORITY: {0}', self.priority)
-        Log.debug('TYPE: {0}', self.type)
-        Log.debug('PARENTS: {0}', [p.name for p in self.parents])
-        Log.debug('CHILDREN: {0}', [c.name for c in self.children])
-        Log.debug('FAIL_COUNT: {0}', self.fail_count)
-        Log.debug('EXPID: {0}', self.expid)
-
     @property
     def parents(self):
         """
         Returns parent jobs list
 
         :return: parent jobs
         :rtype: set
@@ -240,17 +513,18 @@
 
         :param value: platforms to set
         :type value: HPCPlatform
         """
         self._platform = value
 
     @property
+    @autosubmit_parameter(name="current_queue")
     def queue(self):
         """
-        Returns the queue to be used by the job. Chooses between serial and parallel platforms
+        Returns the queue to be used by the job. Chooses between serial and parallel platforms.
 
         :return HPCPlatform object for the job to use
         :rtype: HPCPlatform
         """
         if self._queue is not None and len(str(self._queue)) > 0:
             return self._queue
         if self.is_serial:
@@ -351,40 +625,37 @@
     def total_processors(self):
         """
         Number of processors requested by job.
         Reduces ':' separated format  if necessary.
         """
         if ':' in str(self.processors):
             return reduce(lambda x, y: int(x) + int(y), self.processors.split(':'))
-        elif self.processors == "":
-            return 1
+        elif self.processors == "" or self.processors == "1":
+            if int(self.nodes) <= 1:
+                return 1
+            else:
+                return ""
         return int(self.processors)
 
     @property
     def total_wallclock(self):
         if self.wallclock:
             hours, minutes = self.wallclock.split(':')
             return float(minutes) / 60 + float(hours)
         return 0
 
-    def log_job(self):
-        """
-        Prints job information in log
-        """
-        Log.debug("{0}\t{1}\t{2}", "Job Name", "Job Id", "Job Status")
-        Log.debug("{0}\t\t{1}\t{2}", self.name, self.id, self.status)
-
-        #Log.status("{0}\t{1}\t{2}", "Job Name", "Job Id", "Job Status")
-        #Log.status("{0}\t\t{1}\t{2}", self.name, self.id, self.status)
-
-    def print_parameters(self):
-        """
-        Print sjob parameters in log
-        """
-        Log.info(self.parameters)
+    @property
+    @autosubmit_parameter(name=['numproc', 'processors'])
+    def processors(self):
+        """Number of processors that the job will use."""
+        return self._processors
+
+    @processors.setter
+    def processors(self, value):
+        self._processors = value
 
     def inc_fail_count(self):
         """
         Increments fail count
         """
         self.fail_count += 1
 
@@ -461,47 +732,14 @@
         Returns true if job has any parents, else return false
 
         :return: true if job has any parent, otherwise return false
         :rtype: bool
         """
         return self.parents.__len__()
 
-    def compare_by_status(self, other):
-        """
-        Compare jobs by status value
-
-        :param other: job to compare
-        :type other: Job
-        :return: comparison result
-        :rtype: bool
-        """
-        return self.status < other.status
-
-    def compare_by_id(self, other):
-        """
-        Compare jobs by ID
-
-        :param other: job to compare
-        :type other: Job
-        :return: comparison result
-        :rtype: bool
-        """
-        return self.id < other.id
-
-    def compare_by_name(self, other):
-        """
-        Compare jobs by name
-
-        :param other: job to compare
-        :type other: Job
-        :return: comparison result
-        :rtype: bool
-        """
-        return self.name < other.name
-
     def _get_from_stat(self, index):
         """
         Returns value from given row index position in STAT file associated to job
 
         :param index: row position to retrieve
         :type index: int
         :return: value in index position
@@ -551,23 +789,14 @@
         Returns job's start time
 
         :return: start time
         :rtype: str
         """
         return self._get_from_stat(0)
 
-    def check_retrials_submit_time(self):
-        """
-        Returns list of submit datetime for retrials from total stats file
-
-        :return: date and time
-        :rtype: list[int]
-        """
-        return self._get_from_total_stats(0)
-
     def check_retrials_end_time(self):
         """
         Returns list of end datetime for retrials from total stats file
 
         :return: date and time
         :rtype: list[int]
         """
@@ -845,14 +1074,15 @@
         else:
             format_ = "minute"
         time_params = {}
         for name, param in parts.items():
             if param:
                 time_params[name] = int(param)
         return datetime.timedelta(**time_params),format_
+
     # Duplicated for wrappers and jobs to fix in 4.0.0
     def is_over_wallclock(self, start_time, wallclock):
         """
         Check if the job is over the wallclock time, it is an alternative method to avoid platform issues
         :param start_time:
         :param wallclock:
         :return:
@@ -1000,39 +1230,40 @@
             Log.printlog("Job {0} completion check failed. There is no COMPLETED file".format(
                 self.name), 6009)
             if not over_wallclock:
                 self.status = default_status
             else:
                 return default_status
     def update_platform_parameters(self,as_conf,parameters,job_platform):
+        for key,value in as_conf.platforms_data.get(job_platform.name,{}).items():
+            parameters["CURRENT_"+key.upper()] = value
         parameters['CURRENT_ARCH'] = job_platform.name
         parameters['CURRENT_HOST'] = job_platform.host
         parameters['CURRENT_USER'] = job_platform.user
         parameters['CURRENT_PROJ'] = job_platform.project
         parameters['CURRENT_BUDG'] = job_platform.budget
         parameters['CURRENT_RESERVATION'] = job_platform.reservation
         parameters['CURRENT_EXCLUSIVITY'] = job_platform.exclusivity
         parameters['CURRENT_HYPERTHREADING'] = job_platform.hyperthreading
         parameters['CURRENT_TYPE'] = job_platform.type
         parameters['CURRENT_SCRATCH_DIR'] = job_platform.scratch
         parameters['CURRENT_PROJ_DIR'] = job_platform.project_dir
         parameters['CURRENT_ROOTDIR'] = job_platform.root_dir
         parameters['CURRENT_LOGDIR'] = job_platform.get_files_path()
-
         return parameters
+
     def update_platform_associated_parameters(self,as_conf, parameters, job_platform, chunk):
         self.executable = str(as_conf.jobs_data[self.section].get("EXECUTABLE", as_conf.platforms_data.get(job_platform.name,{}).get("EXECUTABLE","")))
         self.total_jobs = int(as_conf.jobs_data[self.section].get("TOTALJOBS", job_platform.total_jobs))
         self.max_waiting_jobs = int(as_conf.jobs_data[self.section].get("MAXWAITINGJOBS", job_platform.max_waiting_jobs))
-
         self.processors = str(as_conf.jobs_data[self.section].get("PROCESSORS",as_conf.platforms_data.get(job_platform.name,{}).get("PROCESSORS","1")))
+        self.nodes = str(as_conf.jobs_data[self.section].get("NODES",as_conf.platforms_data.get(job_platform.name,{}).get("NODES","")))
         self.exclusive = str(as_conf.jobs_data[self.section].get("EXCLUSIVE",as_conf.platforms_data.get(job_platform.name,{}).get("EXCLUSIVE",False)))
         self.threads = str(as_conf.jobs_data[self.section].get("THREADS",as_conf.platforms_data.get(job_platform.name,{}).get("THREADS","1")))
         self.tasks = str(as_conf.jobs_data[self.section].get("TASKS",as_conf.platforms_data.get(job_platform.name,{}).get("TASKS","1")))
-        self.nodes = str(as_conf.jobs_data[self.section].get("NODES",as_conf.platforms_data.get(job_platform.name,{}).get("NODES","")))
         self.hyperthreading = str(as_conf.jobs_data[self.section].get("HYPERTHREADING",as_conf.platforms_data.get(job_platform.name,{}).get("HYPERTHREADING","none")))
         if int(self.tasks) <= 1 and int(job_platform.processors_per_node) > 1 and int(self.processors) > int(job_platform.processors_per_node):
             self.tasks = job_platform.processors_per_node
         self.memory = str(as_conf.jobs_data[self.section].get("MEMORY",as_conf.platforms_data.get(job_platform.name,{}).get("MEMORY","")))
         self.memory_per_task = str(as_conf.jobs_data[self.section].get("MEMORY_PER_TASK",as_conf.platforms_data.get(job_platform.name,{}).get("MEMORY_PER_TASK","")))
         # These are to activate serial platform if neccesary
         self.queue = self.queue
@@ -1069,25 +1300,26 @@
         parameters['NUMPROC'] = self.processors
         parameters['PROCESSORS'] = self.processors
         parameters['MEMORY'] = self.memory
         parameters['MEMORY_PER_TASK'] = self.memory_per_task
         parameters['NUMTHREADS'] = self.threads
         parameters['THREADS'] = self.threads
         parameters['CPUS_PER_TASK'] = self.threads
-        parameters['NUMTASK'] = self.tasks
-        parameters['TASKS'] = self.tasks
+        parameters['NUMTASK'] = self._tasks
+        parameters['TASKS'] = self._tasks
         parameters['NODES'] = self.nodes
-        parameters['TASKS_PER_NODE'] = self.tasks
+        parameters['TASKS_PER_NODE'] = self._tasks
         parameters['WALLCLOCK'] = self.wallclock
         parameters['TASKTYPE'] = self.section
         parameters['SCRATCH_FREE_SPACE'] = self.scratch_free_space
         parameters['CUSTOM_DIRECTIVES'] = self.custom_directives
         parameters['HYPERTHREADING'] = self.hyperthreading
         parameters['CURRENT_QUEUE'] = self.queue
         return parameters
+
     def update_wrapper_parameters(self,as_conf, parameters):
         wrappers = as_conf.experiment_data.get("WRAPPERS", {})
         if len(wrappers) > 0:
             parameters['WRAPPER'] = as_conf.get_wrapper_type()
             parameters['WRAPPER' + "_POLICY"] = as_conf.get_wrapper_policy()
             parameters['WRAPPER' + "_METHOD"] = as_conf.get_wrapper_method().lower()
             parameters['WRAPPER' + "_JOBS"] = as_conf.get_wrapper_jobs()
@@ -1103,20 +1335,22 @@
             parameters[wrapper_section + "_METHOD"] = as_conf.get_wrapper_method(
                 as_conf.experiment_data["WRAPPERS"].get(wrapper_section)).lower()
             parameters[wrapper_section + "_JOBS"] = as_conf.get_wrapper_jobs(
                 as_conf.experiment_data["WRAPPERS"].get(wrapper_section))
             parameters[wrapper_section + "_EXTENSIBLE"] = int(
                 as_conf.get_extensible_wallclock(as_conf.experiment_data["WRAPPERS"].get(wrapper_section)))
         return parameters
+
     def update_job_parameters(self,as_conf, parameters):
         parameters['JOBNAME'] = self.name
         parameters['FAIL_COUNT'] = str(self.fail_count)
-        parameters['SDATE'] = date2str(self.date, self.date_format)
+        parameters['SDATE'] = self.sdate
         parameters['MEMBER'] = self.member
         parameters['SPLIT'] = self.split
+        parameters['SPLITS'] = self.splits
         parameters['DELAY'] = self.delay
         parameters['FREQUENCY'] = self.frequency
         parameters['SYNCHRONIZE'] = self.synchronize
         parameters['PACKED'] = self.packed
         parameters['CHUNK'] = 1
         if hasattr(self, 'RETRIALS'):
             parameters['RETRIALS'] = self.retrials
@@ -1180,74 +1414,64 @@
 
             if total_chunk == chunk:
                 parameters['CHUNK_LAST'] = 'TRUE'
             else:
                 parameters['CHUNK_LAST'] = 'FALSE'
         parameters['NUMMEMBERS'] = len(as_conf.get_member_list())
         parameters['DEPENDENCIES'] = str(as_conf.jobs_data[self.section].get("DEPENDENCIES",""))
-        # This shouldn't be necessary anymore as now all sub is done in the as_conf.reload()
-        # if len(self.export) > 0:
-        #     variables = re.findall('%(?<!%%)[a-zA-Z0-9_.]+%(?!%%)', self.export)
-        #     if len(variables) > 0:
-        #         variables = [variable[1:-1] for variable in variables]
-        #         for key in variables:
-        #             try:
-        #                 self.export = re.sub(
-        #                     '%(?<!%%)' + key + '%(?!%%)', parameters[key], self.export, flags=re.I)
-        #             except Exception as e:
-        #                 self.export = re.sub(
-        #                     '%(?<!%%)' + key + '%(?!%%)', "NOTFOUND", self.export, flags=re.I)
-        #                 Log.debug(
-        #                     "PARAMETER export: Variable: {0} doesn't exist".format(str(e)))
         self.dependencies = parameters['DEPENDENCIES']
         parameters['EXPORT'] = self.export
         parameters['PROJECT_TYPE'] = as_conf.get_project_type()
         self.wchunkinc = as_conf.get_wchunkinc(self.section)
         return parameters
+
     def update_parameters(self, as_conf, parameters,
                           default_parameters={'d': '%d%', 'd_': '%d_%', 'Y': '%Y%', 'Y_': '%Y_%',
                                               'M': '%M%', 'M_': '%M_%', 'm': '%m%', 'm_': '%m_%'}):
         """
         Refresh parameters value
 
         :param default_parameters:
         :type default_parameters: dict
         :param as_conf:
         :type as_conf: AutosubmitConfig
         :param parameters:
         :type parameters: dict
         """
-        chunk = 1
         as_conf.reload()
         parameters = parameters.copy()
         parameters.update(as_conf.parameters)
         parameters.update(default_parameters)
         parameters = as_conf.substitute_dynamic_variables(parameters,25)
         parameters['ROOTDIR'] = os.path.join(
             BasicConfig.LOCAL_ROOT_DIR, self.expid)
         parameters['PROJDIR'] = as_conf.get_project_dir()
         parameters = self.update_job_parameters(as_conf,parameters)
         parameters = self.update_platform_parameters(as_conf, parameters, self._platform)
         parameters = self.update_platform_associated_parameters(as_conf, parameters, self._platform, parameters['CHUNK'])
         parameters = self.update_wrapper_parameters(as_conf, parameters)
-        parameters = as_conf.substitute_dynamic_variables(parameters,25)
+        parameters = as_conf.normalize_parameters_keys(parameters,default_parameters)
+
+        parameters = as_conf.substitute_dynamic_variables(parameters,80)
         parameters = as_conf.normalize_parameters_keys(parameters,default_parameters)
         # For some reason, there is return but the assignee is also necessary
         self.parameters = parameters
-        # This returns is only being used by the mock , to change the mock
+        # This return is only being used by the mock , to change the mock
         return parameters
+
     def update_content_extra(self,as_conf,files):
         additional_templates = []
         for file in files:
             if as_conf.get_project_type().lower() == "none":
                 template = "%DEFAULT.EXPID%"
             else:
                 template = open(os.path.join(as_conf.get_project_dir(), file), 'r').read()
             additional_templates += [template]
         return additional_templates
+
     def update_content(self, as_conf):
         """
         Create the script content to be run for the job
 
         :param as_conf: config
         :type as_conf: config
         :return: script code
@@ -1577,20 +1801,14 @@
 
             # Launch second as threaded function only for slurm
             if job_data_dc and type(self.platform) is not str and self.platform.type == "slurm":
                 thread_write_finish = Thread(target=ExperimentHistory(self.expid, jobdata_dir_path=BasicConfig.JOBDATA_DIR, historiclog_dir_path=BasicConfig.HISTORICAL_LOG_DIR).write_platform_data_after_finish, args=(job_data_dc, self.platform))
                 thread_write_finish.name = "JOB_data_{}".format(self.name)
                 thread_write_finish.start()
 
-    def write_total_stat_by_retries_fix_newline(self):
-        path = os.path.join(self._tmp_path, self.name + '_TOTAL_STATS')
-        f = open(path, 'a')
-        f.write('\n')
-        f.close()
-
     def write_total_stat_by_retries(self,total_stats, first_retrial = False):
         """
         Writes all data to TOTAL_STATS file
         :param total_stats: data gathered by the wrapper
         :type total_stats: dict
         :param first_retrial: True if this is the first retry, False otherwise
         :type first_retrial: bool
```

### Comparing `autosubmit-4.0.79/autosubmit/job/job_common.py` & `autosubmit-4.0.80/autosubmit/job/job_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/job/job_dict.py` & `autosubmit-4.0.80/autosubmit/job/job_dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,15 +283,15 @@
             jobs.append(dic)
         else:
             if date is not None and len(str(date)) > 0:
                 self._get_date(jobs, dic, date, member, chunk)
             else:
                 for d in self._date_list:
                     self._get_date(jobs, dic, d, member, chunk)
-        if len(jobs) > 1 and isinstance(jobs[0], Iterable):
+        if len(jobs) > 0 and isinstance(jobs[0], list):
             try:
                 jobs_flattened = [job for jobs_to_flatten in jobs for job in jobs_to_flatten]
                 jobs = jobs_flattened
             except TypeError as e:
                 pass
         return jobs
 
@@ -351,14 +351,15 @@
             job = Job(name, 0, Status.WAITING, priority)
 
 
         job.section = section
         job.date = date
         job.member = member
         job.chunk = chunk
+        job.splits = self.experiment_data["JOBS"].get(job.section,{}).get("SPLITS", None)
         job.date_format = self._date_format
         job.delete_when_edgeless = str(parameters[section].get("DELETE_WHEN_EDGELESS", "true")).lower()
 
         if split > -1:
             job.split = split
 
         job.frequency = int(parameters[section].get( "FREQUENCY", 1))
```

### Comparing `autosubmit-4.0.79/autosubmit/job/job_grouping.py` & `autosubmit-4.0.80/autosubmit/job/job_grouping.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/job/job_list.py` & `autosubmit-4.0.80/autosubmit/job/job_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -390,173 +390,352 @@
         elif filter_value.lower().find("natural") != -1:
             if parent_value is None or parent_value in associative_list:
                 return True
         elif filter_value.lower().find("none") != -1:
             return False
         elif filter_value.find(",") != -1:
             aux_filter = filter_value.split(",")
-            if filter_type != "chunks":
+            if filter_type not in ["chunks", "splits"]:
                 for value in aux_filter:
                     if str(value).isdigit():
                         to_filter.append(associative_list[int(value)])
                     else:
                         to_filter.append(value)
             else:
                 to_filter = aux_filter
             del aux_filter
         elif filter_value.find(":") != -1:
             start_end = filter_value.split(":")
             start = start_end[0].strip("[]")
             end = start_end[1].strip("[]")
             del start_end
-            if filter_type == "chunks": # chunk directly
+            if filter_type not in ["chunks", "splits"]: # chunk directly
                 for value in range(int(start), int(end) + 1):
                     to_filter.append(value)
             else: # index
                 for value in range(int(start+1), int(end) + 1):
                     to_filter.append(value)
         else:
             to_filter.append(filter_value)
+
         if str(parent_value).upper() in str(to_filter).upper():
             return True
         else:
             return False
 
 
     @staticmethod
     def _check_relationship(relationships,level_to_check,value_to_check):
         """
         Check if the current_job_value is included in the filter_value
         :param relationship: current filter level to check.
-        :param level_to_check: can be a date, member or chunk.
-        :param value_to_check: can be a date, member or chunk.
+        :param level_to_check: can be a date, member, chunk or split.
+        :param value_to_check: Can be None, a date, a member, a chunk or a split.
         :return:
         """
-        optional = False
         filters = []
-        for filter_type, filter_data in relationships.items():
-            if isinstance(filter_data, collections.abc.Mapping):
-                current_filter = {}
-                if filter_type.upper().find(level_to_check.upper()) != -1:
-                    for filter_range in filter_data.keys():
-                        if str(value_to_check) is None or str(filter_range).upper().find(str(value_to_check).upper()) != -1:
-                            if filter_data[filter_range] is not None:
-                                if filter_type.find("?") != -1 or filter_range.find("?") != -1:
-                                    optional = True
-                                current_filter.update(filter_data[filter_range])
-                filters.append(current_filter)
+        for filter_range,filter_data in relationships.get(level_to_check,{}).items():
+            if not value_to_check or str(filter_range).upper() in "ALL" or str(value_to_check).upper() in str(filter_range).upper():
+                if filter_data:
+                    if "?" in filter_range:
+                        filter_data["OPTIONAL"] = True
+                    else:
+                        filter_data["OPTIONAL"] = relationships["OPTIONAL"]
+                filters.append(filter_data)
         # Normalize the filter return
         if len(filters) == 0:
             filters = [{}]
-        return filters,optional
+        return filters
+
+    @staticmethod
+    def _check_dates(relationships, current_job):
+        """
+        Check if the current_job_value is included in the filter_from and retrieve filter_to value
+        :param relationships: Remaining filters to apply.
+        :param current_job: Current job to check.
+        :return:  filters_to_apply
+        """
+        optional = False
+        filters_to_apply = JobList._check_relationship(relationships, "DATES_FROM", date2str(current_job.date))
+        # there could be multiple filters that apply... per example
+        # Current task date is 20020201, and member is fc2
+        # Dummy example, not specially usefull in a real case
+        #DATES_FROM:
+            #all:
+                #MEMBERS_FROM:
+                    #ALL: ...
+                #CHUNKS_FROM:
+                    #ALL: ...
+            #20020201:
+                #MEMBERS_FROM:
+                    #fc2:
+                        #DATES_TO: "20020201"
+                        #MEMBERS_TO: "fc2"
+                        #CHUNKS_TO: "ALL"
+                #SPLITS_FROM:
+                    #ALL:
+                        #SPLITS_TO: "1"
+        # this "for" iterates for ALL and fc2 as current task is selected in both filters
+        # The dict in this step is:
+        # [{MEMBERS_FROM{..},CHUNKS_FROM{...}},{MEMBERS_FROM{..},SPLITS_FROM{...}}]
+        for i,filter in enumerate(filters_to_apply):
+            # {MEMBERS_FROM{..},CHUNKS_FROM{...}} I want too look ALL filters not only one, but I want to go recursivily until get the  _TO filter
+            optional = filter.pop("OPTIONAL", False)
+            # This is not an if_else, because the current level ( dates ) could have two different filters.
+            # Second case commented: ( date_from 20020201 )
+            # Will enter, go recursivily to the similar methods and in the end it will do:
+            # Will enter members_from, and obtain [{DATES_TO: "20020201", MEMBERS_TO: "fc2", CHUNKS_TO: "ALL", CHUNKS_FROM{...}]
+            if "MEMBERS_FROM" in filter:
+                filters_to_apply_m = JobList._check_members({"MEMBERS_FROM": (filter.pop("MEMBERS_FROM")),"OPTIONAL":optional}, current_job)
+                if len(filters_to_apply_m) > 0:
+                    filters_to_apply[i].update(filters_to_apply_m)
+            # Will enter chunks_from, and obtain [{DATES_TO: "20020201", MEMBERS_TO: "fc2", CHUNKS_TO: "ALL", SPLITS_TO: "2"]
+            if "CHUNKS_FROM" in filter:
+                filters_to_apply_c = JobList._check_chunks({"CHUNKS_FROM": (filter.pop("CHUNKS_FROM")),"OPTIONAL":optional}, current_job)
+                if len(filters_to_apply_c) > 0 and len(filters_to_apply_c[0]) > 0:
+                    filters_to_apply[i].update(filters_to_apply_c)
+            #IGNORED
+            if "SPLITS_FROM" in filter:
+                filters_to_apply_s = JobList._check_splits({"SPLITS_FROM": (filter.pop("SPLITS_FROM")),"OPTIONAL":optional}, current_job)
+                if len(filters_to_apply_s) > 0:
+                    filters_to_apply[i].update(filters_to_apply_s)
+        # Unify filters from all filters_from where the current job is included to have a single SET of filters_to
+        if optional:
+            for i,filter in enumerate(filters_to_apply):
+                filters_to_apply[i]["OPTIONAL"] = True
+        filters_to_apply = JobList._unify_to_filters(filters_to_apply)
+        # {DATES_TO: "20020201", MEMBERS_TO: "fc2", CHUNKS_TO: "ALL", SPLITS_TO: "2"}
+        return filters_to_apply
+
+    @staticmethod
+    def _check_members(relationships, current_job):
+        """
+        Check if the current_job_value is included in the filter_from and retrieve filter_to value
+        :param relationships: Remaining filters to apply.
+        :param current_job: Current job to check.
+        :return: filters_to_apply
+        """
+        filters_to_apply = JobList._check_relationship(relationships, "MEMBERS_FROM", current_job.member)
+        optional = False
+        for i,filter in enumerate(filters_to_apply):
+            optional = filter.pop("OPTIONAL", False)
+            if "CHUNKS_FROM" in filter:
+                filters_to_apply_c = JobList._check_chunks({"CHUNKS_FROM": (filter.pop("CHUNKS_FROM")),"OPTIONAL":optional}, current_job)
+                if len(filters_to_apply_c) > 0:
+                    filters_to_apply[i].update(filters_to_apply_c)
+
+            if "SPLITS_FROM" in filter:
+                filters_to_apply_s = JobList._check_splits({"SPLITS_FROM": (filter.pop("SPLITS_FROM")),"OPTIONAL":optional}, current_job)
+                if len(filters_to_apply_s) > 0:
+                    filters_to_apply[i].update(filters_to_apply_s)
+        if optional:
+            for i,filter in enumerate(filters_to_apply):
+                filters_to_apply[i]["OPTIONAL"] = True
+        filters_to_apply = JobList._unify_to_filters(filters_to_apply)
+        return filters_to_apply
+
+    @staticmethod
+    def _check_chunks(relationships, current_job):
+        """
+        Check if the current_job_value is included in the filter_from and retrieve filter_to value
+        :param relationships: Remaining filters to apply.
+        :param current_job: Current job to check.
+        :return: filters_to_apply
+        """
+        optional = False
+        filters_to_apply = JobList._check_relationship(relationships, "CHUNKS_FROM", current_job.chunk)
+        for i,filter in enumerate(filters_to_apply):
+            optional = filter.pop("OPTIONAL", False)
+            if "SPLITS_FROM" in filter:
+                filters_to_apply_s = JobList._check_splits({"SPLITS_FROM": (filter.pop("SPLITS_FROM")),"OPTIONAL":optional}, current_job)
+                if len(filters_to_apply_s) > 0:
+                    filters_to_apply[i].update(filters_to_apply_s)
+        if optional:
+            for i,filter in enumerate(filters_to_apply):
+                filters_to_apply[i]["OPTIONAL"] = True
+        filters_to_apply = JobList._unify_to_filters(filters_to_apply)
+        return filters_to_apply
+
+    @staticmethod
+    def _check_splits(relationships, current_job):
+        """
+        Check if the current_job_value is included in the filter_from and retrieve filter_to value
+        :param relationships: Remaining filters to apply.
+        :param current_job: Current job to check.
+        :return: filters_to_apply
+        """
+
+        filters_to_apply = JobList._check_relationship(relationships, "SPLITS_FROM", current_job.split)
+        # No more FROM sections to check, unify _to FILTERS and return
+        filters_to_apply = JobList._unify_to_filters(filters_to_apply)
+        return filters_to_apply
+
+    @staticmethod
+    def _unify_to_filter(unified_filter,filter_to,filter_type):
+        """
+        Unify filter_to filters into a single dictionary
+        :param unified_filter: Single dictionary with all filters_to
+        :param filter_to: Current dictionary that contains the filters_to
+        :param filter_type: "DATES_TO", "MEMBERS_TO", "CHUNKS_TO", "SPLITS_TO"
+        :return: unified_filter
+        """
+        if "all" not in unified_filter[filter_type]:
+            aux = filter_to.pop(filter_type, None)
+            if aux:
+                aux = aux.split(",")
+                for element in aux:
+                    if element.lower().strip("?") in ["natural","none"] and len(unified_filter[filter_type]) > 0:
+                        continue
+                    else:
+                        if filter_to.get("OPTIONAL",False) and element[-1] != "?":
+                            element += "?"
+                        unified_filter[filter_type].add(element)
+    @staticmethod
+    def _normalize_to_filters(filter_to,filter_type):
+        """
+        Normalize filter_to filters to a single string or "all"
+        :param filter_to: Unified filter_to dictionary
+        :param filter_type: "DATES_TO", "MEMBERS_TO", "CHUNKS_TO", "SPLITS_TO"
+        :return:
+        """
+        if len(filter_to[filter_type]) == 0:
+            filter_to.pop(filter_type, None)
+        elif "all" in filter_to[filter_type]:
+            filter_to[filter_type] = "all"
+        else:
+            # transform to str separated by commas if multiple elements
+            filter_to[filter_type] = ",".join(filter_to[filter_type])
+
+    @staticmethod
+    def _unify_to_filters(filter_to_apply):
+        """
+        Unify all filter_to filters into a single dictionary ( of current selection )
+        :param filter_to_apply: Filters to apply
+        :return: Single dictionary with all filters_to
+        """
+        unified_filter = {"DATES_TO": set(), "MEMBERS_TO": set(), "CHUNKS_TO": set(), "SPLITS_TO": set()}
+        for filter_to in filter_to_apply:
+            if len(filter_to) > 0:
+                JobList._unify_to_filter(unified_filter,filter_to,"DATES_TO")
+                JobList._unify_to_filter(unified_filter,filter_to,"MEMBERS_TO")
+                JobList._unify_to_filter(unified_filter,filter_to,"CHUNKS_TO")
+                JobList._unify_to_filter(unified_filter,filter_to,"SPLITS_TO")
+                filter_to.pop("OPTIONAL", None)
+
+        JobList._normalize_to_filters(unified_filter,"DATES_TO")
+        JobList._normalize_to_filters(unified_filter,"MEMBERS_TO")
+        JobList._normalize_to_filters(unified_filter,"CHUNKS_TO")
+        JobList._normalize_to_filters(unified_filter,"SPLITS_TO")
+
+        return unified_filter
+
     @staticmethod
     def _filter_current_job(current_job,relationships):
         '''
-        Check if the current_job is included in the filter_value ( from)
-        :param current_job:
-        :param dependency:
-        :return:
+        This function will filter the current job based on the relationships given
+        :param current_job: Current job to filter
+        :param relationships: Relationships to apply
+        :return: dict() with the filters to apply, or empty dict() if no filters to apply
         '''
-        # Search all filters in dependency relationship that affect current_job
-        # First level can be Date,member or chunk or generic
-        # Second level can be member or chunk or generic
-        # Third level can only be chunked.
-        # If the filter is generic, it will be applied to all section jobs.
-        # Check Date then Member or Chunk then Chunk
-        optional = False
-        filters_to_apply = []
-        # this should be a list
-        if relationships is not None and len(relationships) > 0:
-            filters_to_apply,optional = JobList._check_relationship(relationships,"DATES_FROM",date2str(current_job.date))
-            if len(filters_to_apply[0]) > 0:
-                for filter_number in range(0, len(filters_to_apply)):
-                    if "MEMBERS_FROM" in filters_to_apply[filter_number]:
-                        filters_to_apply_m,optional = JobList._check_relationship(filters_to_apply[filter_number],"MEMBERS_FROM",current_job.member)
-                        if len(filters_to_apply_m) > 0:
-                            filters_to_apply,optional = filters_to_apply_m
-                        else:
-                            filters_to_apply_c,optional = JobList._check_relationship(filters_to_apply[filter_number],"CHUNKS_FROM",current_job.chunk)
-                            if len(filters_to_apply_c) > 0:
-                                filters_to_apply = filters_to_apply_c
-                    elif "CHUNKS_FROM" in filters_to_apply[filter_number]:
-                        filters_to_apply,optional = JobList._check_relationship(filters_to_apply[filter_number],"CHUNKS_FROM",current_job.chunk)
-            # Check Member then Chunk
-            if len(filters_to_apply[0]) == 0:
-                filters_to_apply,optional = JobList._check_relationship(relationships,"MEMBERS_FROM",current_job.member)
-                if len(filters_to_apply) > 0 and ( "CHUNKS_FROM" in filters_to_apply):
-                    filters_to_apply_c,optional = JobList._check_relationship(filters_to_apply,"CHUNKS_FROM",current_job.chunk)
-                    if len(filters_to_apply_c) > 0:
-                        filters_to_apply = filters_to_apply_c
-            #Check Chunk
-            if len(filters_to_apply[0]) == 0:
-                filters_to_apply,optional = JobList._check_relationship(relationships,"CHUNKS_FROM",current_job.chunk)
-            # Generic filter
-            if len(filters_to_apply[0]) == 0:
-                relationships.pop("CHUNKS_FROM",None)
-                relationships.pop("MEMBERS_FROM",None)
-                relationships.pop("DATES_FROM",None)
-                filters_to_apply = [relationships]
 
-        if len(filters_to_apply) == 1 and len(filters_to_apply[0]) == 0:
-            return [],optional
-        else:
-            return filters_to_apply,optional
+        # This function will look if the given relationship is set for the given job DATEs,MEMBER,CHUNK,SPLIT ( _from filters )
+        # And if it is, it will return the dependencies that need to be activated (_TO filters)
+        # _FROM behavior:
+        # DATES_FROM can contain MEMBERS_FROM,CHUNKS_FROM,SPLITS_FROM
+        # MEMBERS_FROM can contain CHUNKS_FROM,SPLITS_FROM
+        # CHUNKS_FROM can contain SPLITS_FROM
+        # SPLITS_FROM can contain nothing
+        # _TO behavior:
+        # TO keywords, can be in any of the _FROM filters and they will only affect the _FROM filter they are in.
+        # There are 4 keywords:
+        # 1. ALL: all the dependencies will be activated of the given filter type (dates, members, chunks or/and splits)
+        # 2. NONE: no dependencies will be activated of the given filter type (dates, members, chunks or/and splits)
+        # 3. NATURAL: this is the normal behavior, represents a way of letting the job to be activated if they would normally be activated.
+        # 4. ? : this is a weak dependency activation flag, The dependency will be activated but the job can fail without affecting the workflow.
+
+        filters_to_apply = {}
+        # Check if filter_from-filter_to relationship is set
+        if relationships is not None and len(relationships) > 0:
+            if "OPTIONAL" not in relationships:
+                relationships["OPTIONAL"] = False
+            # Look for a starting point, this can be if else becasue they're exclusive as a DATE_FROM can't be in a MEMBER_FROM and so on
+            if "DATES_FROM" in relationships:
+                filters_to_apply = JobList._check_dates(relationships, current_job)
+            elif "MEMBERS_FROM" in relationships:
+                filters_to_apply = JobList._check_members(relationships, current_job)
+            elif "CHUNKS_FROM" in relationships:
+                filters_to_apply = JobList._check_chunks(relationships, current_job)
+            elif "SPLITS_FROM" in relationships:
+                filters_to_apply = JobList._check_splits(relationships, current_job)
+            else:
+                relationships.pop("OPTIONAL", None)
+                relationships.pop("CHUNKS_FROM", None)
+                relationships.pop("MEMBERS_FROM", None)
+                relationships.pop("DATES_FROM", None)
+                relationships.pop("SPLITS_FROM", None)
+                filters_to_apply = relationships
+        return filters_to_apply
 
 
 
     @staticmethod
-    def _valid_parent(parent,member_list,date_list,chunk_list,is_a_natural_relation,filters_to_apply):
+    def _valid_parent(parent,member_list,date_list,chunk_list,is_a_natural_relation,filter_):
         '''
-        Check if the parent is valid for the current_job
+        Check if the parent is valid for the current job
         :param parent: job to check
-        :param member_list:
-        :param date_list:
-        :param chunk_list:
-        :param is_a_natural_relation:
-        :param filters_to_apply:
-        :return:
+        :param member_list: list of members
+        :param date_list: list of dates
+        :param chunk_list: list of chunks
+        :param is_a_natural_relation: if the relation is natural or not
+        :param filters_to_apply: filters to apply
+        :return: True if the parent is valid, False otherwise
         '''
         #check if current_parent is listed on dependency.relationships
-        optional = False
-        for filter_ in filters_to_apply:
-            associative_list = {}
-            dates_to = str(filter_.get("DATES_TO", "natural")).lower()
-            members_to = str(filter_.get("MEMBERS_TO", "natural")).lower()
-            chunks_to = str(filter_.get("CHUNKS_TO", "natural")).lower()
-            if not is_a_natural_relation:
-                if dates_to == "natural":
-                    dates_to = "none"
-                if members_to == "natural":
-                    members_to = "none"
-                if chunks_to == "natural":
-                    chunks_to = "none"
-
-
-            associative_list["dates"] = date_list
-            associative_list["members"] = member_list
-            associative_list["chunks"] = chunk_list
+        associative_list = {}
+        associative_list["dates"] = date_list
+        associative_list["members"] = member_list
+        associative_list["chunks"] = chunk_list
 
+        if parent.splits is not None:
+            associative_list["splits"] = [ str(split) for split in range(1,int(parent.splits)+1) ]
+        else:
+            associative_list["splits"] = None
+        dates_to = str(filter_.get("DATES_TO", "natural")).lower()
+        members_to = str(filter_.get("MEMBERS_TO", "natural")).lower()
+        chunks_to = str(filter_.get("CHUNKS_TO", "natural")).lower()
+        splits_to = str(filter_.get("SPLITS_TO", "natural")).lower()
+        if not is_a_natural_relation:
             if dates_to == "natural":
-                associative_list["dates"] = [date2str(parent.date)] if parent.date is not None else date_list
-
+                dates_to = "none"
             if members_to == "natural":
-                associative_list["members"] = [parent.member] if parent.member is not None else member_list
+                members_to = "none"
             if chunks_to == "natural":
-                associative_list["chunks"] = [parent.chunk] if parent.chunk is not None else chunk_list
-            parsed_parent_date = date2str(parent.date) if parent.date is not None else None
-            # Apply all filters to look if this parent is an appropriated candidate for the current_job
-            valid_dates   = JobList._apply_filter(parsed_parent_date, dates_to, associative_list["dates"], "dates")
-            valid_members = JobList._apply_filter(parent.member, members_to, associative_list["members"],"members")
-            valid_chunks  = JobList._apply_filter(parent.chunk, chunks_to, associative_list["chunks"], "chunks")
-
-            if valid_dates and valid_members and valid_chunks:
-                if dates_to.find("?") != -1 or members_to.find("?") != -1 or chunks_to.find("?") != -1:
-                    optional = True
-                return True,optional
-        return False,optional
+                chunks_to = "none"
+            if splits_to == "natural":
+                splits_to = "none"
+        if dates_to == "natural":
+            associative_list["dates"] = [date2str(parent.date)] if parent.date is not None else date_list
+        if members_to == "natural":
+            associative_list["members"] = [parent.member] if parent.member is not None else member_list
+        if chunks_to == "natural":
+            associative_list["chunks"] = [parent.chunk] if parent.chunk is not None else chunk_list
+        if splits_to == "natural":
+            associative_list["splits"] = [parent.split] if parent.split is not None else parent.splits
+        parsed_parent_date = date2str(parent.date) if parent.date is not None else None
+        # Apply all filters to look if this parent is an appropriated candidate for the current_job
+        valid_dates   = JobList._apply_filter(parsed_parent_date, dates_to, associative_list["dates"], "dates")
+        valid_members = JobList._apply_filter(parent.member, members_to, associative_list["members"], "members")
+        valid_chunks  = JobList._apply_filter(parent.chunk, chunks_to, associative_list["chunks"], "chunks")
+        valid_splits  = JobList._apply_filter(parent.split, splits_to, associative_list["splits"], "splits")
+        if valid_dates and valid_members and valid_chunks and valid_splits:
+            for value in [dates_to, members_to, chunks_to, splits_to]:
+                if "?" in value:
+                    return True, True
+            return True, False
+        return False,False
     @staticmethod
     def _manage_job_dependencies(dic_jobs, job, date_list, member_list, chunk_list, dependencies_keys, dependencies,
                                  graph):
         '''
         Manage the dependencies of a job
         :param dic_jobs:
         :param job:
@@ -581,79 +760,36 @@
                                                                                  job.date, date_list,
                                                                                  dependency)
             if skip:
                 continue
 
             other_parents = dic_jobs.get_jobs(dependency.section, None, None, None)
             parents_jobs = dic_jobs.get_jobs(dependency.section, date, member, chunk)
-            #if dependency.sign in ["+", "-"]:
-             #   natural_jobs = dic_jobs.get_jobs(dependency.section, date, member,chunk)
-            #else:
-            natural_jobs = dic_jobs.get_jobs(dependency.section, date, member,chunk)
-            if dependency.sign in ['?']:
-                optional_section = True
-            else:
-                optional_section = False
-            # Convert multi_array list into 1d list
-            if len(parents_jobs) > 0:
-                aux = []
-                for p_split in parents_jobs:
-                    if type(p_split) is not list:
-                        aux.append(p_split)
-                    else:
-                        for aux_job in p_split:
-                            aux.append(aux_job)
-                parents_jobs = aux
-            if len(natural_jobs) > 0:
-                aux = []
-                for p_split in natural_jobs:
-                    if type(p_split) is not list:
-                        aux.append(p_split)
-                    else:
-                        for aux_job in p_split:
-                            aux.append(aux_job)
-                natural_jobs = aux
+            natural_jobs = dic_jobs.get_jobs(dependency.section, date, member, chunk)
             all_parents = list(set(other_parents + parents_jobs))
             # Get dates_to, members_to, chunks_to of the deepest level of the relationship.
-            filters_to_apply,optional_from = JobList._filter_current_job(job,copy.deepcopy(dependency.relationships))
-            if len(filters_to_apply) == 0:
-                filters_to_apply.append({"DATES_TO": "natural", "MEMBERS_TO": "natural", "CHUNKS_TO": "natural"})
+            filters_to_apply = JobList._filter_current_job(job,copy.deepcopy(dependency.relationships))
             for parent in all_parents:
-                # Generic for all dependencies
-                if dependency.delay == -1 or chunk > dependency.delay:
-                    if isinstance(parent, list):
-                        if job.split is not None and len(str(job.split)) > 0:
-                            parent = list(filter(
-                                lambda _parent: _parent.split == job.split, parent))
-                            parent = parent[0]
-                        else:
-                            if dependency.splits is not None and len(str(dependency.splits)) > 0:
-                                parent = [_parent for _parent in parent if _parent.split in dependency.splits]
                 # If splits is not None, the job is a list of jobs
                 if parent.name == job.name:
                     continue
-                # Check if it is a natural relation based in autosubmit terms ( same date,member,chunk ).
-                if parent in natural_jobs and ((job.chunk is None or parent.chunk is None or parent.chunk <= job.chunk ) and (parent.split is None or job.split is None or parent.split <= job.split) ) :
+                # Check if it is a natural relation. The only difference is that a chunk can depend on a chunks <= than the current chunk
+                if parent in natural_jobs and (job.chunk is None or parent.chunk is None or parent.chunk <= job.chunk ):
                     natural_relationship = True
                 else:
                     natural_relationship = False
-                if job.name.find("a002_20120101_0_2_SIM") != -1:
-                    print("test")
                 # Check if the current parent is a valid parent based on the dependencies set on expdef.conf
-                valid,optional_to = JobList._valid_parent(parent, member_list, parsed_date_list, chunk_list, natural_relationship,filters_to_apply)
-                if not valid:
-                    continue
-                else:
-                    pass
+                valid,optional = JobList._valid_parent(parent, member_list, parsed_date_list, chunk_list, natural_relationship,filters_to_apply)
                 # If the parent is valid, add it to the graph
-                job.add_parent(parent)
-                JobList._add_edge(graph, job, parent)
-                # Could be more variables in the future
-                if optional_to or optional_from or optional_section:
-                    job.add_edge_info(parent.name,special_variables={"optional":True})
+                if valid:
+                    job.add_parent(parent)
+                    JobList._add_edge(graph, job, parent)
+                    # Could be more variables in the future
+                    if optional:
+                        job.add_edge_info(parent.name,special_variables={"optional":True})
             JobList.handle_frequency_interval_dependencies(chunk, chunk_list, date, date_list, dic_jobs, job, member,
                                                            member_list, dependency.section, graph, other_parents)
 
     @staticmethod
     def _calculate_dependency_metadata(chunk, chunk_list, member, member_list, date, date_list, dependency):
         skip = False
         if dependency.sign == '-':
```

### Comparing `autosubmit-4.0.79/autosubmit/job/job_list_persistence.py` & `autosubmit-4.0.80/autosubmit/job/job_list_persistence.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/job/job_package_persistence.py` & `autosubmit-4.0.80/autosubmit/job/job_package_persistence.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/job/job_packager.py` & `autosubmit-4.0.80/autosubmit/job/job_packager.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,18 +62,18 @@
         submitted_by_id = dict()
         for submitted_job in submitted_jobs:
             submitted_by_id[submitted_job.id] = submitted_job
         submitted_jobs_len = len(list(submitted_by_id.keys()))
 
         waiting_jobs = submitted_jobs_len + queuing_jobs_len
         # Calculate available space in Platform Queue
-        if job is not None and job.max_waiting_jobs != platform.max_waiting_jobs is not None:
-            self._max_wait_jobs_to_submit = job.max_waiting_jobs - waiting_jobs
+        if job is not None and job.max_waiting_jobs and platform.max_waiting_jobs and int(job.max_waiting_jobs) != int(platform.max_waiting_jobs):
+            self._max_wait_jobs_to_submit = int(job.max_waiting_jobs) - int(waiting_jobs)
         else:
-            self._max_wait_jobs_to_submit = platform.max_waiting_jobs - waiting_jobs
+            self._max_wait_jobs_to_submit = int(platform.max_waiting_jobs) - int(waiting_jobs)
         # .total_jobs is defined in each section of platforms_.yml, if not from there, it comes form autosubmit_.yml
         # .total_jobs Maximum number of jobs at the same time
         if job is not None and job.total_jobs != platform.total_jobs:
             self._max_jobs_to_submit = job.total_jobs - queuing_jobs_len
         else:
             self._max_jobs_to_submit = platform.total_jobs - queuing_jobs_len
         # Subtracting running jobs
@@ -82,34 +82,37 @@
         self.max_jobs = min(self._max_wait_jobs_to_submit,self._max_jobs_to_submit)
 
     def __init__(self, as_config, platform, jobs_list, hold=False):
         self.current_wrapper_section = "WRAPPERS"
         self._as_config = as_config
         self._platform = platform
         self._jobs_list = jobs_list
+        self._max_wait_jobs_to_submit = 9999999
         self.hold = hold
         # These are defined in the [wrapper] section of autosubmit_,conf
         self.wrapper_type = dict()
         self.wrapper_policy = dict()
         self.wrapper_method = dict()
         self.jobs_in_wrapper = dict()
         self.extensible_wallclock = dict()
         self.wrapper_info = list()
         self.calculate_job_limits(platform)
         self.special_variables = dict()
 
 
-
         #todo add default values
         #Wrapper building starts here
         for wrapper_section,wrapper_data in self._as_config.experiment_data.get("WRAPPERS",{}).items():
             if isinstance(wrapper_data,collections.abc.Mapping ):
                 self.wrapper_type[wrapper_section] = self._as_config.get_wrapper_type(wrapper_data)
                 self.wrapper_policy[wrapper_section] = self._as_config.get_wrapper_policy(wrapper_data)
-                self.wrapper_method[wrapper_section] = self._as_config.get_wrapper_method(wrapper_data).lower()
+                if self._as_config.get_wrapper_method(wrapper_data) is None:
+                    self.wrapper_method[wrapper_section] = "asthread"
+                else:
+                    self.wrapper_method[wrapper_section] = self._as_config.get_wrapper_method(wrapper_data).lower()
                 self.jobs_in_wrapper[wrapper_section] = self._as_config.get_wrapper_jobs(wrapper_data)
                 self.extensible_wallclock[wrapper_section] = self._as_config.get_extensible_wallclock(wrapper_data)
         self.wrapper_info = [self.wrapper_type,self.wrapper_policy,self.wrapper_method,self.jobs_in_wrapper,self.extensible_wallclock] # to pass to job_packages
         Log.debug("Number of jobs available: {0}", self._max_wait_jobs_to_submit)
         if self.hold:
             Log.debug("Number of jobs prepared: {0}", len(jobs_list.get_prepared(platform)))
             if len(jobs_list.get_prepared(platform)) > 0:
@@ -284,22 +287,14 @@
                                     dependencies_keys += self._as_config.jobs_data.get("DEPENDENCIES", "").split()
                                 if self._as_config.jobs_data[sectionN].get('MAX_WRAPPED',None) is not None and len(str(self._as_config.jobs_data[sectionN].get('MAX_WRAPPED',None))) > 0:
                                     wrapper_limits["max_by_section"][sectionN] = int(self._as_config.jobs_data[sectionN].get("MAX_WRAPPED"))
                                 else:
                                     wrapper_limits["max_by_section"][sectionN] = wrapper_limits["max"]
                                 wrapper_limits["min"] = min(self._as_config.jobs_data[sectionN].get("MIN_WRAPPED",min_value),min_value)
                         hard_limit_wrapper =  wrapper_limits["max"]
-                        #if self.wrapper_type[self.current_wrapper_section].lower() == "vertical":
-                        #    for k in dependencies_keys:
-                        #        if "-" in k:
-                        #            k_divided = k.split("-")
-                        #            if k_divided[0] not in self.jobs_in_wrapper[self.current_wrapper_section]:
-                        #                number = int(k_divided[1].strip(" "))
-                        #                if number < wrapper_limits["max"]:
-                        #                    hard_limit_wrapper = number
                         wrapper_limits["min"] = min(wrapper_limits["min"], hard_limit_wrapper)
                         wrapper_limits["min_v"] = self._as_config.get_min_wrapped_jobs_vertical(self._as_config.experiment_data["WRAPPERS"][self.current_wrapper_section])
                         wrapper_limits["min_h"] = self._as_config.get_min_wrapped_jobs_horizontal(self._as_config.experiment_data["WRAPPERS"][self.current_wrapper_section])
                         wrapper_limits["max"] = hard_limit_wrapper
                         if wrapper_limits["min"] < wrapper_limits["min_v"] * wrapper_limits["min_h"]:
                             wrapper_limits["min"] = max(wrapper_limits["min_v"],wrapper_limits["min_h"])
                         if len(self._jobs_list.jobs_to_run_first) > 0:
@@ -906,22 +901,28 @@
         for job in self.job_list:
             if job.section not in jobs_by_section:
                 jobs_by_section[job.section] = list()
             jobs_by_section[job.section].append(job)
         for section in jobs_by_section:
             current_package_by_section[section] = 0
             for job in jobs_by_section[section]:
+                if str(job.processors).isdigit() and str(job.nodes).isdigit() and int(job.nodes) > 1 and int(job.processors) <= 1:
+                    job.processors = 0
+                if job.total_processors == "":
+                    job_total_processors = 0
+                else:
+                    job_total_processors = int(job.total_processors)
                 if len(current_package) < self.wrapper_limits["max_h"] and len(current_package) < self.wrapper_limits["max"]  and current_package_by_section[section] < self.wrapper_limits["max_by_section"][section]:
                     if int(job.tasks) != 0 and int(job.tasks) != int(self.processors_node) and \
-                            int(job.tasks) < job.total_processors:
+                            int(job.tasks) < job_total_processors:
                         nodes = int(
-                            ceil(job.total_processors / float(job.tasks)))
+                            ceil(job_total_processors / float(job.tasks)))
                         total_processors = int(self.processors_node) * nodes
                     else:
-                        total_processors = job.total_processors
+                        total_processors = job_total_processors
                     if (self._current_processors + total_processors) <= int(self.max_processors):
                         current_package.append(job)
                         self._current_processors += total_processors
                     else:
                         current_package = [job]
                         self._current_processors = total_processors
                     current_package_by_section[section] += 1
```

### Comparing `autosubmit-4.0.79/autosubmit/job/job_packages.py` & `autosubmit-4.0.80/autosubmit/job/job_packages.py`

 * *Files 2% similar despite different names*

```diff
@@ -348,15 +348,29 @@
     :param dependency: Name of potential dependency
     :type dependency: String
     """
     FILE_PREFIX = 'ASThread'
 
     def __init__(self, jobs, dependency=None, jobs_resources=dict(),method='ASThread',configuration=None,wrapper_section="WRAPPERS", wrapper_info= {}):
         super(JobPackageThread, self).__init__(jobs)
-        # to be pass as "configuration"
+        """
+        :param dependency: Dependency
+        :type dependency: String
+        :param jobs_resources: Resources to be used by the jobs, if any
+        :type jobs_resources: Dictionary
+        :param method: Method to be used to submit the jobs, ASThread by default
+        :type method: String
+        :param configuration: Autosubmit configuration
+        :type configuration: Autosubmitconfigparser instance
+            
+        """
+        # This function is called from the JobPackageThread constructor
+        # and from the JobPackageThread.create_scripts function
+        # It is in charge of merging ( switch ) the wrapper info by checking if the value is defined by the user in the wrapper section, current wrapper section, job or platform in that order.
+        # Some variables are calculated in futher functions, like num_processors and wallclock.
         if len(wrapper_info) > 0 :
             self.wrapper_type = wrapper_info[0]
             self.wrapper_policy = wrapper_info[1]
             self.wrapper_method = wrapper_info[2]
             self.jobs_in_wrapper = wrapper_info[3]
             self.extensible_wallclock = wrapper_info[4]
         else:
@@ -366,78 +380,93 @@
             self.jobs_in_wrapper = None
             self.extensible_wallclock = 0
         self._job_scripts = {}
         # Seems like this one is not used at all in the class
         self._job_dependency = dependency
         self._common_script = None
         self._wallclock = '00:00'
-        self._num_processors = '0'
+        # depends on the type of wrapper
+        if not hasattr(self,"_num_processors"):
+            self._num_processors = '0'
         self._jobs_resources = jobs_resources
         self._wrapper_factory = self.platform.wrapper
         self.current_wrapper_section = wrapper_section
         self.inner_retrials = 0
         if configuration is not None:
-            self.inner_retrials = configuration.get_retrials()
+            self.inner_retrials = configuration.experiment_data["WRAPPERS"].get(self.current_wrapper_section,{}).get("INNER_RETRIALS",configuration.get_retrials())
+
             self.export = configuration.get_wrapper_export(configuration.experiment_data["WRAPPERS"][self.current_wrapper_section])
             if self.export.lower() != "none" and len(self.export) > 0:
                 for job in self.jobs:
                     if job.export.lower() != "none" and len(job.export) > 0:
-                        self.export == job.export
+                        self.export = job.export
                         break
             wr_queue = configuration.get_wrapper_queue(configuration.experiment_data["WRAPPERS"][self.current_wrapper_section])
             if wr_queue is not None and len(str(wr_queue)) > 0:
                 self.queue = wr_queue
             else:
                 self.queue = jobs[0].queue
             wr_partition = configuration.get_wrapper_partition(configuration.experiment_data["WRAPPERS"][self.current_wrapper_section])
-            if wr_partition is not None and len(str(wr_partition)) > 0:
+            if wr_partition and len(str(wr_partition)) > 0:
                 self.partition = wr_partition
             else:
                 self.partition = jobs[0].partition
-            wr_exclusive = configuration.experiment_data["WRAPPERS"].get(self.current_wrapper_section,{}).get("EXCLUSIVE",False)
-            if  wr_exclusive:
+            wr_exclusive = configuration.experiment_data["WRAPPERS"].get(self.current_wrapper_section,{}).get("EXCLUSIVE",None)
+            if wr_exclusive is not None:
                 self.exclusive = wr_exclusive
             else:
                 self.exclusive = jobs[0].exclusive
             wr_custom_directives = configuration.experiment_data["WRAPPERS"].get(self.current_wrapper_section,{}).get("CUSTOM_DIRECTIVES",[])
             if len(str(wr_custom_directives)) > 0:
                 self.custom_directives = wr_custom_directives
             else:
                 self.custom_directives = jobs[0].custom_directives
             wr_executable = configuration.experiment_data["WRAPPERS"].get(self.current_wrapper_section,{}).get("EXECUTABLE",None)
-            if wr_executable is None:
+            if wr_executable:
                 self.executable = wr_executable
             else:
                 self.executable = jobs[0].executable
+            wr_tasks = configuration.experiment_data["WRAPPERS"].get(self.current_wrapper_section,{}).get("TASKS",None)
+            if wr_tasks:
+                self.tasks = wr_tasks
+            else:
+                self.tasks = jobs[0].tasks
+            wr_nodes = configuration.experiment_data["WRAPPERS"].get(self.current_wrapper_section,{}).get("NODES",None)
+            if wr_nodes:
+                self.nodes = wr_nodes
+            else:
+                self.nodes = jobs[0].nodes
+            wr_threads = configuration.experiment_data["WRAPPERS"].get(self.current_wrapper_section,{}).get("THREADS",None)
+            if wr_threads:
+                self.threads = wr_threads
+            else:
+                self.threads = jobs[0].threads
         else:
             self.queue = jobs[0].queue
             self.partition = jobs[0].partition
+            self.nodes = jobs[0].nodes
+            self.tasks = jobs[0].tasks
+            self.threads = jobs[0].threads
         self.method = method
-        self._wrapper_factory.as_conf = configuration
-        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"] = configuration.experiment_data["WRAPPERS"][self.current_wrapper_section]
-        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"]["TYPE"] = self.wrapper_type
-        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"]["WRAPPER_POLICY"] = self.wrapper_policy
-        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"]["INNER_RETRIALS"] = self.inner_retrials
-        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"]["EXTEND_WALLCLOCK"] = self.extensible_wallclock
-        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"]["METHOD"] = self.wrapper_method
-        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"]["EXPORT"] = self.export
-        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"]["QUEUE"] = self.queue
-        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"]["PARTITION"] = self.partition
-        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"]["EXCLUSIVE"] = self.exclusive
-        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"]["EXECUTABLE"] = self.executable
-        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"]["CUSTOM_DIRECTIVES"] = self.custom_directives
-
-        pass
-
-
-
-
-
-
-#pipeline
+        self._wrapper_data = configuration.experiment_data["WRAPPERS"][self.current_wrapper_section]
+        self._wrapper_data["TYPE"] = self.wrapper_type
+        self._wrapper_data["WRAPPER_POLICY"] = self.wrapper_policy
+        self._wrapper_data["INNER_RETRIALS"] = self.inner_retrials
+        self._wrapper_data["EXTEND_WALLCLOCK"] = self.extensible_wallclock
+        self._wrapper_data["METHOD"] = self.wrapper_method
+        self._wrapper_data["EXPORT"] = self.export
+        self._wrapper_data["QUEUE"] = self.queue
+        self._wrapper_data["NODES"] = self.nodes
+        self._wrapper_data["TASKS"] = self.tasks
+        self._wrapper_data["THREADS"] = self.threads
+        self._wrapper_data["PROCESSORS"] = self._num_processors
+        self._wrapper_data["PARTITION"] = self.partition
+        self._wrapper_data["EXCLUSIVE"] = self.exclusive
+        self._wrapper_data["EXECUTABLE"] = self.executable
+        self._wrapper_data["CUSTOM_DIRECTIVES"] = self.custom_directives
     @property
     def name(self):
         return self._name
     @property
     def _jobs_scripts(self):
         self._jobs_resources['PROCESSORS_PER_NODE'] = self.platform.processors_per_node
         jobs_scripts = []
@@ -614,20 +643,21 @@
     """
     Class to manage a vertical thread-based package of jobs to be submitted by autosubmit
     :param jobs: 
     :type jobs:
     :param: dependency:
     """
     def __init__(self, jobs, dependency=None,configuration=None,wrapper_section="WRAPPERS", wrapper_info = {}):
-        super(JobPackageVertical, self).__init__(jobs, dependency,configuration=configuration,wrapper_section=wrapper_section, wrapper_info = wrapper_info)
+        self._num_processors = 0
         for job in jobs:
             if int(job.processors) >= int(self._num_processors):
                 self._num_processors = job.processors
-            self._threads = job.threads
-
+                self._threads = job.threads
+        super(JobPackageVertical, self).__init__(jobs, dependency,configuration=configuration,wrapper_section=wrapper_section, wrapper_info = wrapper_info)
+        for job in jobs:
             self._wallclock = sum_str_hours(self._wallclock, job.wallclock)
         self._name = self._expid + '_' + self.FILE_PREFIX + "_{0}_{1}_{2}".format(str(int(time.time())) +
                                                                                   str(random.randint(1, 10000)),
                                                                                   self._num_processors,
                                                                                   len(self._jobs))
 
     def parse_time(self):
@@ -691,15 +721,15 @@
             wallclock_by_level = None
 
         return self._wrapper_factory.get_wrapper(self._wrapper_factory.vertical_wrapper, name=self._name,
                                                  queue=self._queue, project=self._project, wallclock=self._wallclock,
                                                  num_processors=self._num_processors, jobs_scripts=self._jobs_scripts,
                                                  dependency=self._job_dependency, jobs_resources=self._jobs_resources,
                                                  expid=self._expid, rootdir=self.platform.root_dir,
-                                                 directives=self._custom_directives,threads=self._threads,method=self.method.lower(),retrials=self.inner_retrials, wallclock_by_level=wallclock_by_level,partition=self.partition)
+                                                 directives=self._custom_directives,threads=self._threads,method=self.method.lower(),retrials=self.inner_retrials, wallclock_by_level=wallclock_by_level,partition=self.partition,wrapper_data=self._wrapper_data)
 
 
 class JobPackageHorizontal(JobPackageThread):
     """
     Class to manage a horizontal thread-based package of jobs to be submitted by autosubmit
     """
 
@@ -721,15 +751,15 @@
 
     def _common_script_content(self):
         return self._wrapper_factory.get_wrapper(self._wrapper_factory.horizontal_wrapper, name=self._name,
                                                  queue=self._queue, project=self._project, wallclock=self._wallclock,
                                                  num_processors=self._num_processors, jobs_scripts=self._jobs_scripts,
                                                  dependency=self._job_dependency, jobs_resources=self._jobs_resources,
                                                  expid=self._expid, rootdir=self.platform.root_dir,
-                                                 directives=self._custom_directives,threads=self._threads,method=self.method.lower(),partition=self.partition)
+                                                 directives=self._custom_directives,threads=self._threads,method=self.method.lower(),partition=self.partition,wrapper_data=self._wrapper_data)
 
 class JobPackageHybrid(JobPackageThread):
     """
         Class to manage a hybrid (horizontal and vertical) thread-based package of jobs to be submitted by autosubmit
         """
 
     def __init__(self, jobs, num_processors, total_wallclock, dependency=None, jobs_resources=dict(),method="ASThread",configuration=None,wrapper_section="WRAPPERS"):
@@ -766,20 +796,20 @@
 
     def _common_script_content(self):
         return self._wrapper_factory.get_wrapper(self._wrapper_factory.hybrid_wrapper_vertical_horizontal,
                                                  name=self._name, queue=self._queue, project=self._project,
                                                  wallclock=self._wallclock, num_processors=self._num_processors,
                                                  jobs_scripts=self._jobs_scripts, dependency=self._job_dependency,
                                                  jobs_resources=self._jobs_resources, expid=self._expid,
-                                                 rootdir=self.platform.root_dir, directives=self._custom_directives,threads=self._threads,method=self.method.lower(),partition=self.partition)
+                                                 rootdir=self.platform.root_dir, directives=self._custom_directives,threads=self._threads,method=self.method.lower(),partition=self.partition,wrapper_data=self._wrapper_data)
 
 
 class JobPackageHorizontalVertical(JobPackageHybrid):
 
     def _common_script_content(self):
         return self._wrapper_factory.get_wrapper(self._wrapper_factory.hybrid_wrapper_horizontal_vertical,
                                                  name=self._name, queue=self._queue, project=self._project,
                                                  wallclock=self._wallclock, num_processors=self._num_processors,
                                                  jobs_scripts=self._jobs_scripts, dependency=self._job_dependency,
                                                  jobs_resources=self._jobs_resources, expid=self._expid,
-                                                 rootdir=self.platform.root_dir, directives=self._custom_directives,threads=self._threads,method=self.method.lower(),partition=self.partition)
+                                                 rootdir=self.platform.root_dir, directives=self._custom_directives,threads=self._threads,method=self.method.lower(),partition=self.partition,wrapper_data=self._wrapper_data)
```

### Comparing `autosubmit-4.0.79/autosubmit/job/job_utils.py` & `autosubmit-4.0.80/autosubmit/job/job_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/monitor/diagram.py` & `autosubmit-4.0.80/autosubmit/monitor/diagram.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/monitor/monitor.py` & `autosubmit-4.0.80/autosubmit/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/monitor/utils.py` & `autosubmit-4.0.80/autosubmit/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/notifications/mail_notifier.py` & `autosubmit-4.0.80/autosubmit/notifications/mail_notifier.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/notifications/notifier.py` & `autosubmit-4.0.80/autosubmit/notifications/notifier.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/platforms/ecplatform.py` & `autosubmit-4.0.80/autosubmit/platforms/ecplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/platforms/headers/ec_cca_header.py` & `autosubmit-4.0.80/autosubmit/platforms/headers/ec_cca_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/platforms/headers/ec_header.py` & `autosubmit-4.0.80/autosubmit/platforms/headers/ec_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/platforms/headers/local_header.py` & `autosubmit-4.0.80/autosubmit/platforms/headers/local_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/platforms/headers/lsf_header.py` & `autosubmit-4.0.80/autosubmit/platforms/headers/lsf_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/platforms/headers/pbs10_header.py` & `autosubmit-4.0.80/autosubmit/platforms/headers/pbs10_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/platforms/headers/pbs11_header.py` & `autosubmit-4.0.80/autosubmit/platforms/headers/pbs11_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/platforms/headers/pbs12_header.py` & `autosubmit-4.0.80/autosubmit/platforms/headers/pbs12_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/platforms/headers/pjm_header.py` & `autosubmit-4.0.80/autosubmit/platforms/headers/pjm_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/platforms/headers/ps_header.py` & `autosubmit-4.0.80/autosubmit/platforms/headers/ps_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/platforms/headers/sge_header.py` & `autosubmit-4.0.80/autosubmit/platforms/headers/sge_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/platforms/headers/slurm_header.py` & `autosubmit-4.0.80/autosubmit/platforms/headers/slurm_header.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,43 @@
         :rtype: str
         """
         # There is no queue, so directive is empty
         if job.parameters['CURRENT_QUEUE'] == '':
             return ""
         else:
             return "SBATCH --qos={0}".format(job.parameters['CURRENT_QUEUE'])
+    def get_proccesors_directive(self, job):
+        """
+        Returns processors directive for the specified job
 
+        :param job: job to create processors directive for
+        :type job: Job
+        :return: processors directive
+        :rtype: str
+        """
+        # There is no processors, so directive is empty
+        if job.nodes == "":
+            job_nodes = 0
+        else:
+            job_nodes = job.nodes
+        if job.processors == '' or job.processors == '1' and int(job_nodes) > 1:
+            return ""
+        else:
+            return "SBATCH -n {0}".format(job.processors)
+    def get_tasks_directive(self,job):
+        """
+        Returns tasks directive for the specified job
+        :param job: job to create tasks directive for
+        :return: tasks directive
+        :rtype: str
+        """
+        if job.num_tasks == '':
+            return ""
+        else:
+            return "SBATCH --ntasks-per-node {0}".format(job.tasks)
     def get_partition_directive(self, job):
         """
         Returns partition directive for the specified job
 
         :param job: job to create partition directive for
         :type job: Job
         :return: partition directive
@@ -168,15 +196,15 @@
 #%QUEUE_DIRECTIVE%
 #%PARTITION_DIRECTIVE%
 #%ACCOUNT_DIRECTIVE%
 #%MEMORY_DIRECTIVE%
 #%THREADS_PER_TASK_DIRECTIVE%
 #%TASKS_PER_NODE_DIRECTIVE%
 #%NODES_DIRECTIVE%
-#SBATCH -n %NUMPROC%
+#%NUMPROC_DIRECTIVE%
 #SBATCH -t %WALLCLOCK%:00
 #SBATCH -J %JOBNAME%
 #SBATCH --output=%CURRENT_SCRATCH_DIR%/%CURRENT_PROJ_DIR%/%CURRENT_USER%/%DEFAULT.EXPID%/LOG_%DEFAULT.EXPID%/%OUT_LOG_DIRECTIVE%
 #SBATCH --error=%CURRENT_SCRATCH_DIR%/%CURRENT_PROJ_DIR%/%CURRENT_USER%/%DEFAULT.EXPID%/LOG_%DEFAULT.EXPID%/%ERR_LOG_DIRECTIVE%
 %CUSTOM_DIRECTIVES%
 #%X11%
 #
@@ -191,15 +219,15 @@
 #%QUEUE_DIRECTIVE%
 #%PARTITION_DIRECTIVE%
 #%ACCOUNT_DIRECTIVE%
 #%MEMORY_DIRECTIVE%
 #%MEMORY_PER_TASK_DIRECTIVE%
 #%THREADS_PER_TASK_DIRECTIVE%
 #%NODES_DIRECTIVE%
-#SBATCH -n %NUMPROC%
+#%NUMPROC_DIRECTIVE%
 #%TASKS_PER_NODE_DIRECTIVE%
 #SBATCH -t %WALLCLOCK%:00
 #SBATCH -J %JOBNAME%
 #SBATCH --output=%CURRENT_SCRATCH_DIR%/%CURRENT_PROJ_DIR%/%CURRENT_USER%/%DEFAULT.EXPID%/LOG_%DEFAULT.EXPID%/%OUT_LOG_DIRECTIVE%
 #SBATCH --error=%CURRENT_SCRATCH_DIR%/%CURRENT_PROJ_DIR%/%CURRENT_USER%/%DEFAULT.EXPID%/LOG_%DEFAULT.EXPID%/%ERR_LOG_DIRECTIVE%
 %CUSTOM_DIRECTIVES%
 #%X11%
```

### Comparing `autosubmit-4.0.79/autosubmit/platforms/locplatform.py` & `autosubmit-4.0.80/autosubmit/platforms/locplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/platforms/lsfplatform.py` & `autosubmit-4.0.80/autosubmit/platforms/lsfplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/platforms/paramiko_platform.py` & `autosubmit-4.0.80/autosubmit/platforms/paramiko_platform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1183,14 +1183,17 @@
             err_filename = "{0}.cmd.err".format(job.name)
         header = header.replace('%OUT_LOG_DIRECTIVE%', out_filename)
         header = header.replace('%ERR_LOG_DIRECTIVE%', err_filename)
 
         if hasattr(self.header, 'get_queue_directive'):
             header = header.replace(
                 '%QUEUE_DIRECTIVE%', self.header.get_queue_directive(job))
+        if hasattr(self.header, 'get_proccesors_directive'):
+            header = header.replace(
+                '%NUMPROC_DIRECTIVE%', self.header.get_proccesors_directive(job))
         if hasattr(self.header, 'get_partition_directive'):
             header = header.replace(
                 '%PARTITION_DIRECTIVE%', self.header.get_partition_directive(job))
         if hasattr(self.header, 'get_tasks_per_node'):
             header = header.replace(
                 '%TASKS_PER_NODE_DIRECTIVE%', self.header.get_tasks_per_node(job))
         if hasattr(self.header, 'get_threads_per_task'):
```

### Comparing `autosubmit-4.0.79/autosubmit/platforms/paramiko_submitter.py` & `autosubmit-4.0.80/autosubmit/platforms/paramiko_submitter.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/platforms/pbsplatform.py` & `autosubmit-4.0.80/autosubmit/platforms/pbsplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/platforms/pjmplatform.py` & `autosubmit-4.0.80/autosubmit/platforms/pjmplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/platforms/platform.py` & `autosubmit-4.0.80/autosubmit/platforms/platform.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import locale
 import os
 
 import traceback
 from autosubmit.job.job_common import Status
 from typing import List, Union
 
+from autosubmit.helpers.parameters import autosubmit_parameter
 from log.log import AutosubmitCritical, AutosubmitError, Log
 
 class Platform(object):
     """
     Class to manage the connections to the different platforms.
     """
 
@@ -16,56 +17,177 @@
         """
         :param config:
         :param expid:
         :param name:
         """
         self.connected = False
         self.expid = expid # type: str
-        self.name = name # type: str
+        self._name = name # type: str
         self.config = config
         self.tmp_path = os.path.join(
             self.config.get("LOCAL_ROOT_DIR"), self.expid, self.config.get("LOCAL_TMP_DIR"))
         self._serial_platform = None
         self._serial_queue = None
         self._serial_partition = None
         self._default_queue = None
         self._partition = None
         self.ec_queue = "hpc"
         self.processors_per_node = "1"
         self.scratch_free_space = None
         self.custom_directives = None
-        self.host = ''
-        self.user = ''
-        self.project = ''
-        self.budget = ''
-        self.reservation = ''
-        self.exclusivity = ''
-        self.type = ''
-        self.scratch = ''
-        self.project_dir = ''
+        self._host = ''
+        self._user = ''
+        self._project = ''
+        self._budget = ''
+        self._reservation = ''
+        self._exclusivity = ''
+        self._type = ''
+        self._scratch = ''
+        self._project_dir = ''
         self.temp_dir = ''
-        self.root_dir = ''
+        self._root_dir = ''
         self.service = None
         self.scheduler = None
         self.directory = None
-        self.hyperthreading = False
+        self._hyperthreading = False
         self.max_wallclock = '2:00'
         self.total_jobs = 20
         self.max_processors = "480"
         self._allow_arrays = False
         self._allow_wrappers = False
         self._allow_python_jobs = True
         self.mkdir_cmd = None
         self.get_cmd = None
         self.put_cmd = None
         self._submit_hold_cmd = None
         self._submit_command_name = None
         self._submit_cmd = None
         self._checkhost_cmd = None
         self.cancel_cmd = None
+
+    @property
+    @autosubmit_parameter(name='current_arch')
+    def name(self):
+        """Platform name."""
+        return self._name
+
+    @name.setter
+    def name(self, value):
+        self._name = value
+
+    @property
+    @autosubmit_parameter(name='current_host')
+    def host(self):
+        """Platform url."""
+        return self._host
+
+    @host.setter
+    def host(self, value):
+        self._host = value
+
+    @property
+    @autosubmit_parameter(name='current_user')
+    def user(self):
+        """Platform user."""
+        return self._user
+
+    @user.setter
+    def user(self, value):
+        self._user = value
+
+    @property
+    @autosubmit_parameter(name='current_proj')
+    def project(self):
+        """Platform project."""
+        return self._project
+
+    @project.setter
+    def project(self, value):
+        self._project = value
+
+    @property
+    @autosubmit_parameter(name='current_budg')
+    def budget(self):
+        """Platform budget."""
+        return self._budget
+
+    @budget.setter
+    def budget(self, value):
+        self._budget = value
+
+    @property
+    @autosubmit_parameter(name='current_reservation')
+    def reservation(self):
+        """You can configure your reservation id for the given platform."""
+        return self._reservation
+
+    @reservation.setter
+    def reservation(self, value):
+        self._reservation = value
+
+    @property
+    @autosubmit_parameter(name='current_exclusivity')
+    def exclusivity(self):
+        """True if you want to request exclusivity nodes."""
+        return self._exclusivity
+
+    @exclusivity.setter
+    def exclusivity(self, value):
+        self._exclusivity = value
+
+    @property
+    @autosubmit_parameter(name='current_hyperthreading')
+    def hyperthreading(self):
+        """TODO"""
+        return self._hyperthreading
+
+    @hyperthreading.setter
+    def hyperthreading(self, value):
+        self._hyperthreading = value
+
+    @property
+    @autosubmit_parameter(name='current_type')
+    def type(self):
+        """Platform scheduler type."""
+        return self._type
+
+    @type.setter
+    def type(self, value):
+        self._type = value
+
+    @property
+    @autosubmit_parameter(name='current_scratch_dir')
+    def scratch(self):
+        """Platform's scratch folder path."""
+        return self._scratch
+
+    @scratch.setter
+    def scratch(self, value):
+        self._scratch = value
+
+    @property
+    @autosubmit_parameter(name='current_proj_dir')
+    def project_dir(self):
+        """Platform's project folder path."""
+        return self._project_dir
+
+    @project_dir.setter
+    def project_dir(self, value):
+        self._project_dir = value
+
+    @property
+    @autosubmit_parameter(name='current_rootdir')
+    def root_dir(self):
+        """Platform's experiment folder path."""
+        return self._root_dir
+
+    @root_dir.setter
+    def root_dir(self, value):
+        self._root_dir = value
+
     def get_exclusive_directive(self, job):
         """
         Returns exclusive directive for the specified job
         :param job: job to create exclusive directive for
         :type job: Job
         :return: exclusive directive
         :rtype: str
@@ -193,28 +315,32 @@
         if self._serial_platform is None:
             return self
         return self._serial_platform
 
     @serial_platform.setter
     def serial_platform(self, value):
         self._serial_platform = value
+
     @property
+    @autosubmit_parameter(name='current_partition')
     def partition(self):
         """
-        Partition to use for jobs
+        Partition to use for jobs.
+
         :return: queue's name
         :rtype: str
         """
         if self._partition is None:
             return ''
         return self._partition
 
     @partition.setter
     def partition(self, value):
         self._partition = value
+
     @property
     def queue(self):
         """
         Queue to use for jobs
         :return: queue's name
         :rtype: str
         """
@@ -520,17 +646,18 @@
             if self.get_file(filename, True):
                 return True
             else:
                 return False
         else:
             return False
 
+    @autosubmit_parameter(name='current_logdir')
     def get_files_path(self):
         """
-        Get the path to the platform's LOG directory
+        The platform's LOG directory.
 
         :return: platform's LOG directory
         :rtype: str
         """
         if self.type == "local":
             path = os.path.join(
                 self.root_dir, self.config.get("LOCAL_TMP_DIR"), 'LOG_{0}'.format(self.expid))
```

### Comparing `autosubmit-4.0.79/autosubmit/platforms/psplatform.py` & `autosubmit-4.0.80/autosubmit/platforms/psplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/platforms/sgeplatform.py` & `autosubmit-4.0.80/autosubmit/platforms/sgeplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/platforms/slurmplatform.py` & `autosubmit-4.0.80/autosubmit/platforms/slurmplatform.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,15 @@
         try:
             valid_packages_to_submit = [ package for package in valid_packages_to_submit if package.x11 != True]
             if len(valid_packages_to_submit) > 0:
                 package = valid_packages_to_submit[0]
                 try:
                     jobs_id = self.submit_Script(hold=hold)
                 except AutosubmitError as e:
+                    Log.error(f'TRACE:{e.trace}\n{e.message}')
                     jobnames = [job.name for job in valid_packages_to_submit[0].jobs]
                     for jobname in jobnames:
                         jobid = self.get_jobid_by_jobname(jobname)
                         #cancel bad submitted job if jobid is encountered
                         for id_ in jobid:
                             self.cancel_job(id_)
                     jobs_id = None
@@ -610,30 +611,32 @@
 {kwargs["queue"]}
 {kwargs["partition"]}
 {kwargs["dependency"]}
 #SBATCH -A {kwargs["project"]}
 #SBATCH --output={kwargs["name"]}.out
 #SBATCH --error={kwargs["name"]}.err
 #SBATCH -t {kwargs["wallclock"]}:00
-#SBATCH -n {kwargs["num_processors"]}
-#SBATCH --cpus-per-task={kwargs["threads"]}
+{kwargs["threads"]}
+{kwargs["nodes"]}
+{kwargs["num_processors"]}
+{kwargs["tasks"]}
 {kwargs["exclusive"]}
 {kwargs["custom_directives"]}
 
 #
 ###############################################################################
 """
         if kwargs["method"] == 'srun':
             language = kwargs["executable"]
             if language is None or len(language) == 0:
                 language = "#!/bin/bash"
             return language + wr_header
         else:
             language = kwargs["executable"]
-            if language is None or len(language) == 0:
+            if language is None or len(language) == 0 or "bash" in language:
                 language = "#!/usr/bin/env python3"
             return language + wr_header
 
     @staticmethod
     def allocated_nodes():
         return """os.system("scontrol show hostnames $SLURM_JOB_NODELIST > node_list_{0}".format(node_id))"""
```

### Comparing `autosubmit-4.0.79/autosubmit/platforms/submitter.py` & `autosubmit-4.0.80/autosubmit/platforms/submitter.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/platforms/wrappers/wrapper_builder.py` & `autosubmit-4.0.80/autosubmit/platforms/wrappers/wrapper_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,18 +28,19 @@
     def __init__(self):
         self._builder = None
     def construct(self, builder):
         self._builder = builder
 
         header = self._builder.build_header()
         job_thread = self._builder.build_job_thread()
-        if "bash" not in header[0:15]:
-            main = self._builder.build_main()
-        else:
-            nodes,main = self._builder.build_main() #What to do with nodes?
+        #if "bash" not in header[0:15]:
+
+        main = self._builder.build_main()
+        #else:
+        #    nodes,main = self._builder.build_main() #What to do with nodes?
         # change to WrapperScript object
         wrapper_script = header + job_thread + main
         wrapper_script = wrapper_script.replace("_NEWLINE_", '\\n')
 
         return wrapper_script
 class WrapperBuilder(object):
     def __init__(self, **kwargs):
```

### Comparing `autosubmit-4.0.79/autosubmit/platforms/wrappers/wrapper_factory.py` & `autosubmit-4.0.80/autosubmit/platforms/wrappers/wrapper_factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,22 +28,29 @@
     def __init__(self, platform):
         self.as_conf = None
         self.platform = platform
         self.wrapper_director = WrapperDirector()
         self.exception = "This type of wrapper is not supported for this platform"
 
     def get_wrapper(self, wrapper_builder, **kwargs):
-        wrapper_data = self.as_conf.experiment_data["CURRENT_WRAPPER"]
+        wrapper_data = kwargs['wrapper_data']
         kwargs['allocated_nodes'] = self.allocated_nodes()
         kwargs['dependency'] = self.dependency(kwargs['dependency'])
         kwargs['queue'] = self.queue(kwargs['queue'])
         kwargs['partition'] = self.partition(wrapper_data['PARTITION'])
         kwargs["exclusive"] = self.exclusive(wrapper_data['EXCLUSIVE'])
         kwargs["custom_directives"] = self.custom_directives(wrapper_data["CUSTOM_DIRECTIVES"])
         kwargs["executable"] = wrapper_data["EXECUTABLE"]
+        kwargs['nodes'] = self.nodes(wrapper_data['NODES'])
+        kwargs['tasks'] = self.tasks(wrapper_data['TASKS'])
+        kwargs['threads'] = self.threads(kwargs['threads'])
+        if str(wrapper_data['NODES']).isdigit() and int(wrapper_data['NODES']) > 1 and kwargs['num_processors'] == '1':
+            kwargs['num_processors'] = "#"
+        else:
+            kwargs['num_processors'] = self.processors(kwargs['num_processors'])
         kwargs['header_directive'] = self.header_directives(**kwargs)
         builder = wrapper_builder(**kwargs)
         return self.wrapper_director.construct(builder)
 
     def vertical_wrapper(self, **kwargs):
         raise NotImplemented(self.exception)
 
@@ -62,16 +69,24 @@
     def allocated_nodes(self):
         return ''
 
     def dependency(self, dependency):
         return '#' if dependency is None else self.dependency_directive(dependency)
     def queue(self, queue):
         return '#' if not queue else self.queue_directive(queue)
+    def processors(self, processors):
+        return '#' if not processors or processors == "0" else self.processors_directive(processors)
+    def nodes(self, nodes):
+        return '#' if not nodes else self.nodes_directive(nodes)
+    def tasks(self, tasks):
+        return '#' if not tasks else self.tasks_directive(tasks)
     def partition(self, partition):
         return '#' if not partition else self.partition_directive(partition)
+    def threads(self, threads):
+        return '#' if not threads or threads in ["0","1"] else self.threads_directive(threads)
     def exclusive(self, exclusive):
         return '#' if not exclusive or str(exclusive).lower() == "false" else self.exclusive_directive(exclusive)
     def custom_directives(self, custom_directives):
         return '#' if not custom_directives else self.get_custom_directives(custom_directives)
     def get_custom_directives(self, custom_directives):
         """
         Returns custom directives for the specified job
@@ -80,24 +95,29 @@
         """
         # There is no custom directives, so directive is empty
         if custom_directives != '':
             return '\n'.join(str(s) for s in custom_directives)
         return ""
 
     def dependency_directive(self, dependency):
-        pass
+        raise NotImplemented(self.exception)
     def queue_directive(self, queue):
-        pass
+        raise NotImplemented(self.exception)
+    def processors_directive(self, processors):
+        raise NotImplemented(self.exception)
+    def nodes_directive(self, nodes):
+        raise NotImplemented(self.exception)
+    def tasks_directive(self, tasks):
+        raise NotImplemented(self.exception)
     def partition_directive(self, partition):
-        pass
+        raise NotImplemented(self.exception)
     def exclusive_directive(self, exclusive):
-        pass
-
-
-
+        raise NotImplemented(self.exception)
+    def threads_directive(self, threads):
+        raise NotImplemented(self.exception)
 
 class SlurmWrapperFactory(WrapperFactory):
 
     def vertical_wrapper(self, **kwargs):
         return PythonVerticalWrapperBuilder(**kwargs)
 
     def horizontal_wrapper(self, **kwargs):
@@ -123,19 +143,27 @@
         return self.platform.allocated_nodes()
 
     def dependency_directive(self, dependency):
         return '#SBATCH --dependency=afterok:{0}'.format(dependency)
 
     def queue_directive(self, queue):
         return '#SBATCH --qos={0}'.format(queue)
-
     def partition_directive(self, partition):
         return '#SBATCH --partition={0}'.format(partition)
     def exclusive_directive(self, exclusive):
         return '#SBATCH --exclusive'
+    def tasks_directive(self, tasks):
+        return '#SBATCH --ntasks-per-node={0}'.format(tasks)
+    def nodes_directive(self, nodes):
+        return '#SBATCH -N {0}'.format(nodes)
+    def processors_directive(self, processors):
+        return '#SBATCH -n {0}'.format(processors)
+    def threads_directive(self, threads):
+        return '#SBATCH --cpus-per-task={0}'.format(threads)
+
 
 
 class LSFWrapperFactory(WrapperFactory):
 
     def vertical_wrapper(self, **kwargs):
         return PythonVerticalWrapperBuilder(**kwargs)
```

### Comparing `autosubmit-4.0.79/autosubmit/statistics/jobs_stat.py` & `autosubmit-4.0.80/autosubmit/statistics/jobs_stat.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/statistics/statistics.py` & `autosubmit-4.0.80/autosubmit/statistics/statistics.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/statistics/stats_summary.py` & `autosubmit-4.0.80/autosubmit/statistics/stats_summary.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit/statistics/utils.py` & `autosubmit-4.0.80/autosubmit/statistics/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/autosubmit.egg-info/PKG-INFO` & `autosubmit-4.0.80/autosubmit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmit
-Version: 4.0.79
+Version: 4.0.80
 Summary: Autosubmit is a Python-based workflow manager to create, manage and monitor complex tasks involving different substeps, such as scientific computational experiments. These workflows may involve multiple computing systems for their completion, from HPCs to post-processing clusters or workstations. Autosubmit can orchestrate all the tasks integrating the workflow by managing their dependencies, interfacing with all the platforms involved, and handling eventual errors.
 Home-page: http://www.bsc.es/projects/earthscience/autosubmit/
 Download-URL: https://earth.bsc.es/wiki/doku.php?id=tools:autosubmit
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
 License: GNU GPL v3
 Keywords: climate,weather,workflow,HPC
```

### Comparing `autosubmit-4.0.79/autosubmit.egg-info/SOURCES.txt` & `autosubmit-4.0.80/autosubmit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 autosubmit/experiment/experiment_common.py
 autosubmit/experiment/statistics.py
 autosubmit/git/__init__.py
 autosubmit/git/autosubmit_git.py
 autosubmit/helpers/__init__.py
 autosubmit/helpers/autosubmit_helper.py
 autosubmit/helpers/data_transfer.py
+autosubmit/helpers/parameters.py
 autosubmit/helpers/utils.py
 autosubmit/history/__init__.py
 autosubmit/history/experiment_history.py
 autosubmit/history/experiment_status.py
 autosubmit/history/internal_logging.py
 autosubmit/history/strategies.py
 autosubmit/history/utils.py
@@ -274,14 +275,15 @@
 test/unit/README_PIP.md
 test/unit/__init__.py
 test/unit/test_basic_config.py
 test/unit/test_catlog.py
 test/unit/test_chunk_date_lib.py
 test/unit/test_database_managers.py
 test/unit/test_db_manager.py
+test/unit/test_dependencies.py
 test/unit/test_dic_jobs.py
 test/unit/test_expid.py
 test/unit/test_history.py
 test/unit/test_job.py
 test/unit/test_job_common.py
 test/unit/test_job_graph.py
 test/unit/test_job_grouping.py
```

### Comparing `autosubmit-4.0.79/bin/autosubmit` & `autosubmit-4.0.80/bin/autosubmit`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/Makefile` & `autosubmit-4.0.80/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/autosubmit.pdf` & `autosubmit-4.0.80/docs/autosubmit.pdf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/experiment/fig/fig_experiment.jpg` & `autosubmit-4.0.80/docs/source/agui/experiment/fig/fig_experiment.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/experiment/index.rst` & `autosubmit-4.0.80/docs/source/agui/experiment/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/fig/fig1_gui.png` & `autosubmit-4.0.80/docs/source/agui/fig/fig1_gui.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/fig/fig2_gui.png` & `autosubmit-4.0.80/docs/source/agui/fig/fig2_gui.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/fig/fig3_gui.png` & `autosubmit-4.0.80/docs/source/agui/fig/fig3_gui.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/fig/fig4_gui.jpg` & `autosubmit-4.0.80/docs/source/agui/fig/fig4_gui.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/fig/fig5_gui.jpg` & `autosubmit-4.0.80/docs/source/agui/fig/fig5_gui.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/fig/fig_ev_1.png` & `autosubmit-4.0.80/docs/source/agui/fig/fig_ev_1.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/fig/fig_tree_1.png` & `autosubmit-4.0.80/docs/source/agui/fig/fig_tree_1.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/fig/fig_tree_2.png` & `autosubmit-4.0.80/docs/source/agui/fig/fig_tree_2.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/graph/fig/fig_graph_1.jpg` & `autosubmit-4.0.80/docs/source/agui/graph/fig/fig_graph_1.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/graph/fig/fig_graph_2.jpg` & `autosubmit-4.0.80/docs/source/agui/graph/fig/fig_graph_2.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/graph/fig/fig_graph_3.jpg` & `autosubmit-4.0.80/docs/source/agui/graph/fig/fig_graph_3.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/graph/fig/fig_graph_4.jpg` & `autosubmit-4.0.80/docs/source/agui/graph/fig/fig_graph_4.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/graph/index.rst` & `autosubmit-4.0.80/docs/source/agui/graph/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/index.rst` & `autosubmit-4.0.80/docs/source/agui/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/log/fig/fig_log_1.jpg` & `autosubmit-4.0.80/docs/source/agui/log/fig/fig_log_1.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/log/fig/fig_log_2.jpg` & `autosubmit-4.0.80/docs/source/agui/log/fig/fig_log_2.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/log/index.rst` & `autosubmit-4.0.80/docs/source/agui/log/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/performance/fig/fig_performance_1.jpg` & `autosubmit-4.0.80/docs/source/agui/performance/fig/fig_performance_1.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/performance/index.rst` & `autosubmit-4.0.80/docs/source/agui/performance/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/statistics/fig/fig_stat_1.jpg` & `autosubmit-4.0.80/docs/source/agui/statistics/fig/fig_stat_1.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/statistics/fig/fig_stat_2.jpg` & `autosubmit-4.0.80/docs/source/agui/statistics/fig/fig_stat_2.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/statistics/index.rst` & `autosubmit-4.0.80/docs/source/agui/statistics/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/tree/fig/fig_tree_2.jpg` & `autosubmit-4.0.80/docs/source/agui/tree/fig/fig_tree_2.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/agui/tree/index.rst` & `autosubmit-4.0.80/docs/source/agui/tree/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/conf.py` & `autosubmit-4.0.80/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,29 +16,31 @@
 import os
 # import shlex
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.insert(0, os.path.abspath('../..'))
+sys.path.append(os.path.abspath('ext'))  # path to custom extensions.
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.imgmath',
     'sphinx.ext.autosectionlabel',
     'sphinx_rtd_theme',
-    'sphinx_reredirects'
+    'sphinx_reredirects',
+    'autosubmit_variables'
 ]
 
 autosectionlabel_prefix_document = True
 
 numfig = True
 numfig_format = {'figure': '%s', 'table': '%s', 'code-block': '%s'}
```

### Comparing `autosubmit-4.0.79/docs/source/devguide/index.rst` & `autosubmit-4.0.80/docs/source/devguide/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/index.rst` & `autosubmit-4.0.80/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/installation/index.rst` & `autosubmit-4.0.80/docs/source/installation/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/introduction/fig1.png` & `autosubmit-4.0.80/docs/source/introduction/fig1.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/introduction/fig2.png` & `autosubmit-4.0.80/docs/source/introduction/fig2.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/introduction/fig3.png` & `autosubmit-4.0.80/docs/source/introduction/fig3.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/introduction/index.rst` & `autosubmit-4.0.80/docs/source/introduction/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/moduledoc/platforms.rst` & `autosubmit-4.0.80/docs/source/moduledoc/platforms.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/qstartguide/dummy.png` & `autosubmit-4.0.80/docs/source/qstartguide/dummy.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/qstartguide/index.rst` & `autosubmit-4.0.80/docs/source/qstartguide/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/troubleshooting/changelog.rst` & `autosubmit-4.0.80/docs/source/troubleshooting/changelog.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/troubleshooting/error-codes.rst` & `autosubmit-4.0.80/docs/source/troubleshooting/error-codes.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/troubleshooting/fig/monarch-da.png` & `autosubmit-4.0.80/docs/source/troubleshooting/fig/monarch-da.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/troubleshooting/fig/new_dependencies_0.png` & `autosubmit-4.0.80/docs/source/troubleshooting/fig/new_dependencies_0.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/troubleshooting/fig/new_dependencies_1.png` & `autosubmit-4.0.80/docs/source/troubleshooting/fig/new_dependencies_1.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/troubleshooting/index.rst` & `autosubmit-4.0.80/docs/source/troubleshooting/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/unused_figs/group_chunk.png` & `autosubmit-4.0.80/docs/source/unused_figs/group_chunk.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/unused_figs/horizontal-vertical.png` & `autosubmit-4.0.80/docs/source/unused_figs/horizontal-vertical.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/unused_figs/wrapper.png` & `autosubmit-4.0.80/docs/source/unused_figs/wrapper.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/unused_figs/wrapper_expression.png` & `autosubmit-4.0.80/docs/source/unused_figs/wrapper_expression.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/unused_figs/wrapper_hybrid.png` & `autosubmit-4.0.80/docs/source/unused_figs/wrapper_hybrid.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/userguide/configure/develop_a_project.rst` & `autosubmit-4.0.80/docs/source/userguide/configure/develop_a_project.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/userguide/configure/index.rst` & `autosubmit-4.0.80/docs/source/userguide/configure/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/userguide/create/index.rst` & `autosubmit-4.0.80/docs/source/userguide/create/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/userguide/index.rst` & `autosubmit-4.0.80/docs/source/userguide/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/userguide/manage/index.rst` & `autosubmit-4.0.80/docs/source/userguide/manage/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/userguide/run/index.rst` & `autosubmit-4.0.80/docs/source/userguide/run/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/userguide/wrappers/fig/dasim.png` & `autosubmit-4.0.80/docs/source/userguide/wrappers/fig/dasim.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/userguide/wrappers/fig/horizontal_remote.png` & `autosubmit-4.0.80/docs/source/userguide/wrappers/fig/horizontal_remote.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/userguide/wrappers/fig/multiple_wrappers.png` & `autosubmit-4.0.80/docs/source/userguide/wrappers/fig/multiple_wrappers.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/userguide/wrappers/fig/rerun.png` & `autosubmit-4.0.80/docs/source/userguide/wrappers/fig/rerun.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/userguide/wrappers/fig/vertical-horizontal.png` & `autosubmit-4.0.80/docs/source/userguide/wrappers/fig/vertical-horizontal.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/userguide/wrappers/fig/vertical-mixed.png` & `autosubmit-4.0.80/docs/source/userguide/wrappers/fig/vertical-mixed.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/docs/source/userguide/wrappers/index.rst` & `autosubmit-4.0.80/docs/source/userguide/wrappers/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/environment.yml` & `autosubmit-4.0.80/environment.yml`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 - bcrypt
 - pip
 - mock
 - portalocker
 - networkx
 - sqlite
 - pip:
-  - autosubmitconfigparser == 1.0.27
+  - autosubmitconfigparser
   - argparse>=1.4.0
   - bcrypt>=3.2.0
   - python-dateutil>=2.8.2
   - matplotlib>=3.5.1
   - numpy<1.22
   - py3dotplus>=1.1.0
   - pyparsing>=3.0.7
```

### Comparing `autosubmit-4.0.79/log/fd_show.py` & `autosubmit-4.0.80/log/fd_show.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/log/log.py` & `autosubmit-4.0.80/log/log.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/setup.py` & `autosubmit-4.0.80/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     description='Autosubmit is a Python-based workflow manager to create, manage and monitor complex tasks involving different substeps, such as scientific computational experiments. These workflows may involve multiple computing systems for their completion, from HPCs to post-processing clusters or workstations. Autosubmit can orchestrate all the tasks integrating the workflow by managing their dependencies, interfacing with all the platforms involved, and handling eventual errors.',
     long_description=open('README_PIP.md').read(),
     author='Daniel Beltran Mora',
     author_email='daniel.beltran@bsc.es',
     url='http://www.bsc.es/projects/earthscience/autosubmit/',
     download_url='https://earth.bsc.es/wiki/doku.php?id=tools:autosubmit',
     keywords=['climate', 'weather', 'workflow', 'HPC'],
-    install_requires=['ruamel.yaml==0.17.21','ruamel.yaml.clib==0.2.7','autosubmitconfigparser==1.0.29','bcrypt>=3.2','packaging>19','six>=1.10.0','configobj>=5.0.6','argparse>=1.4.0','python-dateutil>=2.8.2','matplotlib<3.6','numpy<1.22','py3dotplus>=1.1.0','pyparsing>=3.0.7','paramiko>=2.9.2','mock>=4.0.3','portalocker>=2.3.2','networkx==2.6.3','requests>=2.27.1','bscearth.utils>=0.5.2','cryptography>=36.0.1','setuptools>=60.8.2','xlib>=0.21','pip>=22.0.3','pythondialog','pytest','nose','coverage','PyNaCl>=1.4.0','Pygments'],
+    install_requires=['ruamel.yaml==0.17.21','cython','autosubmitconfigparser','bcrypt>=3.2','packaging>19','six>=1.10.0','configobj>=5.0.6','argparse>=1.4.0','python-dateutil>=2.8.2','matplotlib<3.6','numpy<1.22','py3dotplus>=1.1.0','pyparsing>=3.0.7','paramiko>=2.9.2','mock>=4.0.3','portalocker>=2.3.2','networkx==2.6.3','requests>=2.27.1','bscearth.utils>=0.5.2','cryptography>=36.0.1','setuptools>=60.8.2','xlib>=0.21','pip>=22.0.3','pythondialog','pytest','nose','coverage','PyNaCl>=1.4.0','Pygments'],
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Operating System :: POSIX :: Linux",
     ],
     packages=find_packages(),
```

### Comparing `autosubmit-4.0.79/test/integration/test_db_manager.py` & `autosubmit-4.0.80/test/integration/test_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/integration/test_job.py` & `autosubmit-4.0.80/test/integration/test_job.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/README` & `autosubmit-4.0.80/test/regression/README`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/default_conf/platforms.conf` & `autosubmit-4.0.80/test/regression/default_conf/platforms.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/local_asparser_test.py` & `autosubmit-4.0.80/test/regression/local_asparser_test.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_ecmwf_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.80/test/regression/test_ecmwf_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_ecmwf_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.80/test/regression/test_ecmwf_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_ecmwf_with_paramiko/conf/jobs.conf` & `autosubmit-4.0.80/test/regression/test_ecmwf_with_paramiko/conf/jobs.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_large_experiment_on_moore_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.80/test/regression/test_large_experiment_on_moore_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_large_experiment_on_moore_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.80/test/regression/test_large_experiment_on_moore_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_mistral_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.80/test/regression/test_mistral_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_mistral_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.80/test/regression/test_mistral_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_mn3_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.80/test/regression/test_mn3_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_mn3_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.80/test/regression/test_mn3_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_mn3_with_paramiko/conf/jobs.conf` & `autosubmit-4.0.80/test/regression/test_mn3_with_paramiko/conf/jobs.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_mn3_with_paramiko_python/conf/autosubmit.conf` & `autosubmit-4.0.80/test/regression/test_mn3_with_paramiko_python/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_mn3_with_paramiko_python/conf/expdef.conf` & `autosubmit-4.0.80/test/regression/test_mn3_with_paramiko_python/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.80/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.80/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.80/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.80/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.80/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.80/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.80/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.80/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_mn4_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.80/test/regression/test_mn4_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_mn4_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.80/test/regression/test_mn4_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_mn4_with_paramiko/conf/jobs.conf` & `autosubmit-4.0.80/test/regression/test_mn4_with_paramiko/conf/jobs.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_mn4_with_paramiko_python/conf/autosubmit.conf` & `autosubmit-4.0.80/test/regression/test_mn4_with_paramiko_python/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_mn4_with_paramiko_python/conf/expdef.conf` & `autosubmit-4.0.80/test/regression/test_mn4_with_paramiko_python/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_moore_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.80/test/regression/test_moore_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_moore_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.80/test/regression/test_moore_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_moore_with_paramiko_python/conf/autosubmit.conf` & `autosubmit-4.0.80/test/regression/test_moore_with_paramiko_python/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_moore_with_paramiko_python/conf/expdef.conf` & `autosubmit-4.0.80/test/regression/test_moore_with_paramiko_python/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_sedema_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.80/test/regression/test_sedema_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_sedema_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.80/test/regression/test_sedema_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_sedema_with_paramiko_python/conf/autosubmit.conf` & `autosubmit-4.0.80/test/regression/test_sedema_with_paramiko_python/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/test_sedema_with_paramiko_python/conf/expdef.conf` & `autosubmit-4.0.80/test/regression/test_sedema_with_paramiko_python/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/tests.conf` & `autosubmit-4.0.80/test/regression/tests.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/tests_commands.py` & `autosubmit-4.0.80/test/regression/tests_commands.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/tests_log.py` & `autosubmit-4.0.80/test/regression/tests_log.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/tests_runner.py` & `autosubmit-4.0.80/test/regression/tests_runner.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/regression/tests_utils.py` & `autosubmit-4.0.80/test/regression/tests_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/unit/README_PIP.md` & `autosubmit-4.0.80/test/unit/README_PIP.md`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/unit/test_basic_config.py` & `autosubmit-4.0.80/test/unit/test_basic_config.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/unit/test_catlog.py` & `autosubmit-4.0.80/test/unit/test_catlog.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/unit/test_chunk_date_lib.py` & `autosubmit-4.0.80/test/unit/test_chunk_date_lib.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/unit/test_database_managers.py` & `autosubmit-4.0.80/test/unit/test_database_managers.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/unit/test_db_manager.py` & `autosubmit-4.0.80/test/unit/test_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/unit/test_dic_jobs.py` & `autosubmit-4.0.80/test/unit/test_dic_jobs.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/unit/test_history.py` & `autosubmit-4.0.80/test/unit/test_history.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/unit/test_job.py` & `autosubmit-4.0.80/test/unit/test_job.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import sys
 from autosubmitconfigparser.config.configcommon import AutosubmitConfig
 from autosubmit.job.job_common import Status
 from autosubmit.job.job import Job
 from autosubmit.platforms.platform import Platform
 from mock import Mock, MagicMock
 from mock import patch
+import datetime
 
 # compatibility with both versions (2 & 3)
 from sys import version_info
 
 if version_info.major == 2:
     import builtins as builtins
 else:
@@ -254,14 +255,41 @@
         # act
         self.job.check_completion()
 
         # assert
         exists_mock.assert_called_once_with(os.path.join(self.job._tmp_path, self.job.name + '_COMPLETED'))
         self.assertEqual(Status.FAILED, self.job.status)
 
+    def test_total_processors(self):
+        for test in [
+            {
+                'processors': '',
+                'nodes': 0,
+                'expected': 1
+            },
+            {
+                'processors': '',
+                'nodes': 10,
+                'expected': ''
+            },
+            {
+                'processors': '42',
+                'nodes': 2,
+                'expected': 42
+            },
+            {
+                'processors': '1:9',
+                'nodes': 0,
+                'expected': 10
+            }
+        ]:
+            self.job.processors = test['processors']
+            self.job.nodes = test['nodes']
+            self.assertEqual(self.job.total_processors, test['expected'])
+
     def test_job_script_checking_contains_the_right_default_variables(self):
         # This test (and feature) was implemented in order to avoid
         # false positives on the checking process with auto-ecearth3
         # Arrange
         section = "RANDOM-SECTION"
         self.job.section = section
         self.job.parameters['ROOTDIR'] = "none"
@@ -284,38 +312,60 @@
         }
         self.as_conf.jobs_data[section] = options
 
         dummy_serial_platform = MagicMock()
         dummy_serial_platform.name = 'serial'
         dummy_platform = MagicMock()
         dummy_platform.serial_platform = dummy_serial_platform
+        dummy_platform.name = 'dummy_platform'
+
         self.as_conf.substitute_dynamic_variables = MagicMock()
         default = {'d': '%d%', 'd_': '%d_%', 'Y': '%Y%', 'Y_': '%Y_%',
                                               'M': '%M%', 'M_': '%M_%', 'm': '%m%', 'm_': '%m_%'}
         self.as_conf.substitute_dynamic_variables.return_value = default
         dummy_platform.custom_directives = '["whatever"]'
-        self.as_conf.dynamic_variables = MagicMock()
+        self.as_conf.dynamic_variables = {}
         self.as_conf.parameters = MagicMock()
         self.as_conf.return_value = {}
         self.as_conf.normalize_parameters_keys = MagicMock()
         self.as_conf.normalize_parameters_keys.return_value = default
         self.job._platform = dummy_platform
+        self.as_conf.platforms_data = { "dummy_platform":{ "whatever":"dummy_value", "whatever2":"dummy_value2"} }
+
         parameters = {}
         # Act
         parameters = self.job.update_parameters(self.as_conf, parameters)
         # Assert
+        self.assertTrue('CURRENT_WHATEVER' in parameters)
+        self.assertTrue('CURRENT_WHATEVER2' in parameters)
+
+        self.assertEqual('dummy_value', parameters['CURRENT_WHATEVER'])
+        self.assertEqual('dummy_value2', parameters['CURRENT_WHATEVER2'])
         self.assertTrue('d' in parameters)
         self.assertTrue('d_' in parameters)
         self.assertTrue('Y' in parameters)
         self.assertTrue('Y_' in parameters)
         self.assertEqual('%d%', parameters['d'])
         self.assertEqual('%d_%', parameters['d_'])
         self.assertEqual('%Y%', parameters['Y'])
         self.assertEqual('%Y_%', parameters['Y_'])
 
+    def test_sdate(self):
+        """Test that the property getter for ``sdate`` works as expected."""
+        for test in [
+            [None, None, ''],
+            [datetime.datetime(1975, 5, 25, 22, 0, 0, 0, datetime.timezone.utc), 'H', '1975052522'],
+            [datetime.datetime(1975, 5, 25, 22, 30, 0, 0, datetime.timezone.utc), 'M', '197505252230'],
+            [datetime.datetime(1975, 5, 25, 22, 30, 0, 0, datetime.timezone.utc), 'S', '19750525223000'],
+            [datetime.datetime(1975, 5, 25, 22, 30, 0, 0, datetime.timezone.utc), None, '19750525']
+        ]:
+            self.job.date = test[0]
+            self.job.date_format = test[1]
+            self.assertEquals(test[2], self.job.sdate)
+
 import inspect
 class FakeBasicConfig:
     def __init__(self):
         pass
     def props(self):
         pr = {}
         for name in dir(self):
```

### Comparing `autosubmit-4.0.79/test/unit/test_job_common.py` & `autosubmit-4.0.80/test/unit/test_job_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/unit/test_job_graph.py` & `autosubmit-4.0.80/test/unit/test_job_graph.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/unit/test_job_grouping.py` & `autosubmit-4.0.80/test/unit/test_job_grouping.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/unit/test_job_list.py` & `autosubmit-4.0.80/test/unit/test_job_list.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/unit/test_log.py` & `autosubmit-4.0.80/test/unit/test_log.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/unit/test_machinefiles_wrapper.py` & `autosubmit-4.0.80/test/unit/test_machinefiles_wrapper.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/unit/test_paramiko_platform.py` & `autosubmit-4.0.80/test/unit/test_paramiko_platform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/unit/test_pjm.py` & `autosubmit-4.0.80/test/unit/test_pjm.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/unit/test_platform_monitor.py` & `autosubmit-4.0.80/test/unit/test_platform_monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/unit/test_slurm_platform.py` & `autosubmit-4.0.80/test/unit/test_slurm_platform.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,36 @@
         submit_platform_script.touch(exist_ok=True)
 
         self.platform = SlurmPlatform(expid='a000', name='local', config=self.config)
 
     def tearDown(self) -> None:
         self.local_root_dir.cleanup()
 
+    def test_properties(self):
+        props = {
+            'name': 'foo',
+            'host': 'localhost1',
+            'user': 'sam',
+            'project': 'proj1',
+            'budget': 100,
+            'reservation': 1,
+            'exclusivity': True,
+            'hyperthreading': True,
+            'type': 'SuperSlurm',
+            'scratch': '/scratch/1',
+            'project_dir': '/proj1',
+            'root_dir': '/root_1',
+            'partition': 'inter',
+            'queue': 'prio1'
+        }
+        for prop, value in props.items():
+            setattr(self.platform, prop, value)
+        for prop, value in props.items():
+            self.assertEqual(value, getattr(self.platform, prop))
+
     def test_slurm_platform_submit_script_raises_autosubmit_critical_with_trace(self):
         package = MagicMock()
         package.jobs.return_value = []
         valid_packages_to_submit = [
             package
         ]
```

### Comparing `autosubmit-4.0.79/test/unit/test_statistics.py` & `autosubmit-4.0.80/test/unit/test_statistics.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/unit/test_strategies.py` & `autosubmit-4.0.80/test/unit/test_strategies.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.79/test/unit/test_wrappers.py` & `autosubmit-4.0.80/test/unit/test_wrappers.py`

 * *Files identical despite different names*

