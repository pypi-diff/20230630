# Comparing `tmp/LbNightlyTools-3.0.8.tar.gz` & `tmp/LbNightlyTools-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "public/LbNightlyTools-3.0.8.tar", last modified: Wed Apr 22 07:28:04 2020, max compression
+gzip compressed data, was "public/LbNightlyTools-3.0.9.tar", last modified: Thu May 14 12:42:19 2020, max compression
```

## Comparing `LbNightlyTools-3.0.8.tar` & `LbNightlyTools-3.0.9.tar`

### file list

```diff
@@ -1,461 +1,461 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/
--rw-rw-rw-   0 root         (0) root         (0)    35147 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/COPYING
--rw-r--r--   0 root         (0) root         (0)      896 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4772 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/.cproject
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/cmt/
--rw-rw-rw-   0 root         (0) root         (0)       47 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/cmt/requirements
--rw-rw-rw-   0 root         (0) root         (0)       79 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/cmt/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)       72 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      954 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/setup.csh
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/utils/
--rw-rw-rw-   0 root         (0) root         (0)     1698 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/utils/add_ci_webhook.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/setup.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/cron/
--rwxrwxrwx   0 root         (0) root         (0)     1518 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/cron/cleanup_artifacts.sh
--rwxrwxrwx   0 root         (0) root         (0)     2118 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/cron/preheat_nightly_dashboard.sh
--rw-rw-rw-   0 root         (0) root         (0)      154 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/cron/logrotate.conf
--rwxrwxrwx   0 root         (0) root         (0)     2034 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/cron/clean_up_reduced_db.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/scripts/
--rwxrwxrwx   0 root         (0) root         (0)     1595 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/scripts/lbn-wrapcmd
--rwxrwxrwx   0 root         (0) root         (0)     2340 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/scripts/lbpr-collect
--rwxrwxrwx   0 root         (0) root         (0)     1053 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/scripts/lbn-get-configs
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/admin/
--rwxrwxrwx   0 root         (0) root         (0)     1901 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/admin/RpmHelpers.py
--rwxrwxrwx   0 root         (0) root         (0)     3723 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/admin/createLbScriptsRpm
--rw-rw-rw-   0 root         (0) root         (0)     1670 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/admin/LHCb_LbScripts.spectemplate
--rw-rw-rw-   0 root         (0) root         (0)      368 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/.project
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/jenkins/
--rwxrwxrwx   0 root         (0) root         (0)      943 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/utils.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/jenkins/mock/
--rwxrwxrwx   0 root         (0) root         (0)      936 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/mock/clean_checkout.sh
--rwxrwxrwx   0 root         (0) root         (0)      887 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/mock/clean_build.sh
--rwxrwxrwx   0 root         (0) root         (0)      864 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/mock/clean_preconditions.sh
--rwxrwxrwx   0 root         (0) root         (0)      904 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/mock/clean_enabled_slots.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/jenkins/testrunners/
--rwxrwxrwx   0 root         (0) root         (0)      382 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/testrunners/qmtest.sh
--rwxrwxrwx   0 root         (0) root         (0)      605 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/testrunners/lhcbpr.sh
--rwxrwxrwx   0 root         (0) root         (0)      387 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/testrunners/default.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/jenkins/nightly-builds/
--rwxrwxrwx   0 root         (0) root         (0)      966 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/nightly-builds/tests-poll.sh
--rwxrwxrwx   0 root         (0) root         (0)    15845 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/nightly-builds/gitlab-mr.py
--rwxrwxrwx   0 root         (0) root         (0)     2864 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/nightly-builds/checkout.sh
--rwxrwxrwx   0 root         (0) root         (0)     2571 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/nightly-builds/tests.sh
--rwxrwxrwx   0 root         (0) root         (0)     1403 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/nightly-builds/main.sh
--rwxrwxrwx   0 root         (0) root         (0)     1093 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/nightly-builds/release-poll.sh
--rwxrwxrwx   0 root         (0) root         (0)     2256 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/nightly-builds/gaudi_mr_poll.py
--rwxrwxrwx   0 root         (0) root         (0)      903 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/nightly-builds/preconditions.sh
--rwxrwxrwx   0 root         (0) root         (0)     3176 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/nightly-builds/build.sh
--rwxrwxrwx   0 root         (0) root         (0)      933 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/nightly-builds/release.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/jenkins/periodic-tests/
--rwxrwxrwx   0 root         (0) root         (0)     1219 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/periodic-tests/tests-pollqueue.sh
--rwxrwxrwx   0 root         (0) root         (0)     1170 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/periodic-tests/tests-poll.sh
--rwxrwxrwx   0 root         (0) root         (0)     2276 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/periodic-tests/tests.sh
--rwxrwxrwx   0 root         (0) root         (0)      892 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/periodic-tests/tests-getteststorun.sh
--rwxrwxrwx   0 root         (0) root         (0)     2410 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/mock.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/jenkins/utils.d/
--rw-rw-rw-   0 root         (0) root         (0)     7244 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/utils.d/build_slot.sh
--rw-rw-rw-   0 root         (0) root         (0)     5278 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/utils.d/set_common.sh
--rw-rw-rw-   0 root         (0) root         (0)     2639 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/utils.d/check_preconditions.sh
--rw-rw-rw-   0 root         (0) root         (0)     6055 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/utils.d/checkout_slot.sh
--rw-rw-rw-   0 root         (0) root         (0)     2029 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/utils.d/execute_preconditions.sh
--rwxrwxrwx   0 root         (0) root         (0)     2327 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/docker.sh
--rwxrwxrwx   0 root         (0) root         (0)     2364 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/testMock.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/jenkins/docker-home/
--rw-rw-rw-   0 root         (0) root         (0)      131 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/docker-home/.bashrc
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/jenkins/docker-home/.ssh/
--rw-rw-rw-   0 root         (0) root         (0)      234 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/docker-home/.ssh/config
--rw-rw-rw-   0 root         (0) root         (0)      183 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/jenkins/docker-home/.bash_profile
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/periodic_tests/
--rw-rw-rw-   0 root         (0) root         (0)      883 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/periodic_tests/starter_schedule.xml
--rw-rw-rw-   0 root         (0) root         (0)      402 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/periodic_tests/scheduleIncorrect.xml
--rw-rw-rw-   0 root         (0) root         (0)      486 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/periodic_tests/lhcbpr_schedule.xml
--rw-rw-rw-   0 root         (0) root         (0)      742 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/periodic_tests/schedule.xml
--rw-rw-rw-   0 root         (0) root         (0)    15857 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/periodic_tests/slotbuilds.json
--rw-rw-rw-   0 root         (0) root         (0)      398 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/testing-slot-lbcore-664.json
--rw-rw-rw-   0 root         (0) root         (0)      381 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/testing-slot-2b.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/fix_glimpse/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/fix_glimpse/untouched/
--rw-rw-rw-   0 root         (0) root         (0)       12 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/fix_glimpse/untouched/.glimpse_filenames
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/fix_glimpse/levelA/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/fix_glimpse/levelA/levelB/
--rw-rw-rw-   0 root         (0) root         (0)       10 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/fix_glimpse/levelA/levelB/.glimpse_filenames
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/fix_glimpse/level1/
--rw-rw-rw-   0 root         (0) root         (0)       54 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/fix_glimpse/level1/.glimpse_filenames
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/fix_glimpse/level1/level2/
--rw-rw-rw-   0 root         (0) root         (0)       19 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/fix_glimpse/level1/level2/.glimpse_filenames
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/fix_glimpse/docs/
--rw-rw-rw-   0 root         (0) root         (0)       12 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/fix_glimpse/docs/.glimpse_filenames
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/indexer/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/build.dir/
--rw-rw-rw-   0 root         (0) root         (0)       18 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/build.dir/IgnoredSource.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/InstallArea/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/InstallArea/cmake/
--rw-rw-rw-   0 root         (0) root         (0)       23 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/InstallArea/cmake/AProjectConfig.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/InstallArea/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/InstallArea/python/MyPackage/
--rw-rw-rw-   0 root         (0) root         (0)       23 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/InstallArea/python/MyPackage/MyPackage_user_confDb.py
--rw-rw-rw-   0 root         (0) root         (0)       19 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/InstallArea/python/MyPackage/MyPackage_confDb.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/InstallArea/python/MyPackage/SomeModule.py
--rw-rw-rw-   0 root         (0) root         (0)       16 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/InstallArea/python/MyPackage/SomethingConf.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/InstallArea/python/MyPackage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/InstallArea/python/MyPackage/MyPackageConf.py
--rw-rw-rw-   0 root         (0) root         (0)       26 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/InstallArea/python/AProject_merged_confDb.py
--rw-rw-rw-   0 root         (0) root         (0)       24 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/InstallArea/python/GeneratedPython.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/InstallArea/include/
--rw-rw-rw-   0 root         (0) root         (0)       14 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/InstallArea/include/MyHeader.h
--rw-rw-rw-   0 root         (0) root         (0)       24 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/InstallArea/include/GeneratedHeader.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/MyPackage/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/MyPackage/Headers/
--rw-rw-rw-   0 root         (0) root         (0)       14 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/MyPackage/Headers/MyHeader.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/MyPackage/scripts/
--rw-rw-rw-   0 root         (0) root         (0)       11 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/MyPackage/scripts/MyScript
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/MyPackage/src/
--rw-rw-rw-   0 root         (0) root         (0)       15 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/MyPackage/src/MySource.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/MyPackage/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/MyPackage/python/MyPackage/
--rw-rw-rw-   0 root         (0) root         (0)       18 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/MyPackage/python/MyPackage/SomeModule.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/indexer/AProject/MyPackage/python/MyPackage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/testing-slot-with-shared.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/coverity/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/coverity/configs/
--rw-rw-rw-   0 root         (0) root         (0)      110 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/coverity/configs/coverity_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/coverity/build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/coverity/build/TEST/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/coverity/build/TEST/TEST_HEAD/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/coverity/build/TEST/TEST_HEAD/InstallArea/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/coverity/build/TEST/TEST_HEAD/InstallArea/.empty
--rw-rw-rw-   0 root         (0) root         (0)      256 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/coverity/build/TEST/TEST_HEAD/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      310 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/coverity/build/TEST/TEST_HEAD/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/coverity/bin/
--rwxrwxrwx   0 root         (0) root         (0)     1694 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/coverity/bin/cov-commit-defects
--rwxrwxrwx   0 root         (0) root         (0)     1695 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/coverity/bin/cov-analyze
--rwxrwxrwx   0 root         (0) root         (0)     1545 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/coverity/bin/cov-build
--rw-rw-rw-   0 root         (0) root         (0)      414 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/testing-slot-2.json
--rw-rw-rw-   0 root         (0) root         (0)      279 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/testing-slot-lbcore-192.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/tools/
--rw-rw-rw-   0 root         (0) root         (0)      658 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/tools/manifest.xml
--rw-rw-rw-   0 root         (0) root         (0)      103 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/tools/mini_manifest.xml
--rw-rw-rw-   0 root         (0) root         (0)     1272 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/tools/manifest_do0.xml
--rw-rw-rw-   0 root         (0) root         (0)     1074 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/tools/manifest_with_pkgs.xml
--rw-rw-rw-   0 root         (0) root         (0)      219 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/testing-slot.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/artifacts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/artifacts/packs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/artifacts/packs/src/
--rw-rw-rw-   0 root         (0) root         (0)     2387 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/artifacts/packs/src/TestProject.HEAD.testing-slot.src.zip
--rw-rw-rw-   0 root         (0) root         (0)      244 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/data-packs.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmt/Lbcom/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmt/Lbcom/cmt/
--rw-rw-rw-   0 root         (0) root         (0)       19 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmt/Lbcom/cmt/project.cmt
--rw-rw-rw-   0 root         (0) root         (0)      559 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmt/conf.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmt/Online/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmt/Online/cmt/
--rw-rw-rw-   0 root         (0) root         (0)      115 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmt/Online/cmt/project.cmt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmt/Brunel/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmt/Brunel/cmt/
--rw-rw-rw-   0 root         (0) root         (0)       41 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmt/Brunel/cmt/project.cmt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmt/Rec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmt/Rec/cmt/
--rw-rw-rw-   0 root         (0) root         (0)       22 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmt/Rec/cmt/project.cmt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmt/Gaudi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmt/Gaudi/cmt/
--rw-rw-rw-   0 root         (0) root         (0)       26 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmt/Gaudi/cmt/project.cmt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmt/LHCb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmt/LHCb/cmt/
--rw-rw-rw-   0 root         (0) root         (0)       50 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmt/LHCb/cmt/project.cmt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmt/NewProj/
--rw-rw-rw-   0 root         (0) root         (0)       40 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmt/NewProj/project.info
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmake/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmake/Lbcom/
--rw-rw-rw-   0 root         (0) root         (0)       54 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmake/Lbcom/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)      561 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmake/conf.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmake/Online/
--rw-rw-rw-   0 root         (0) root         (0)      117 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmake/Online/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmake/Brunel/
--rw-rw-rw-   0 root         (0) root         (0)      111 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmake/Brunel/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmake/Rec/
--rw-rw-rw-   0 root         (0) root         (0)       52 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmake/Rec/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmake/Gaudi/
--rw-rw-rw-   0 root         (0) root         (0)       29 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmake/Gaudi/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)       25 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmake/Gaudi/toolchain.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmake/LHCb/
--rw-rw-rw-   0 root         (0) root         (0)       85 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmake/LHCb/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmake/NewProj/
--rw-rw-rw-   0 root         (0) root         (0)       40 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/collect_deps/cmake/NewProj/project.info
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/broken/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/broken/BadCMake/
--rw-rw-rw-   0 root         (0) root         (0)       14 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/collect_deps/broken/BadCMake/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/broken/BadCMT/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/broken/BadCMT/cmt/
--rw-rw-rw-   0 root         (0) root         (0)       21 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/collect_deps/broken/BadCMT/cmt/project.cmt
--rw-rw-rw-   0 root         (0) root         (0)      295 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/collect_deps/broken/conf.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/collect_deps/broken/Gaudi/
--rw-rw-rw-   0 root         (0) root         (0)       29 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/collect_deps/broken/Gaudi/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)       25 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/collect_deps/broken/Gaudi/toolchain.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/build_tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/build_tests/orig/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/build_tests/orig/dummy/
--rw-rw-rw-   0 root         (0) root         (0)      392 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/build_tests/orig/dummy/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      364 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/testing-slot-env.json
--rw-rw-rw-   0 root         (0) root         (0)     6009 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/ci-test-hook-content.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/rpm/
--rw-rw-rw-   0 root         (0) root         (0)     2977 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/rpm/PARAM_TMVAWeights.spec
--rw-rw-rw-   0 root         (0) root         (0)      617 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/rpm/manifest.xml
--rw-rw-rw-   0 root         (0) root         (0)     1265 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/rpm/Brunel_v46r0.spec
--rw-rw-rw-   0 root         (0) root         (0)      961 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/rpm/datapkg-slot-config.json
--rw-rw-rw-   0 root         (0) root         (0)      915 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/rpm/slot-configdo0.json
--rw-rw-rw-   0 root         (0) root         (0)     7195 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/rpm/LCG_68_externalsDict.json
--rw-rw-rw-   0 root         (0) root         (0)     1272 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/rpm/manifest_do0.xml
--rw-rw-rw-   0 root         (0) root         (0)     1981 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/rpm/glimpse_Brunel_v46r0.spec
--rw-rw-rw-   0 root         (0) root         (0)     1630 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/rpm/Brunel_v46r0_x86_64-slc6-gcc48-opt.spec
--rw-rw-rw-   0 root         (0) root         (0)     2476 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/rpm/Gaudi_v27r0_x86_64-slc6-gcc49-do0.spec
--rw-rw-rw-   0 root         (0) root         (0)      915 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/rpm/slot-config.json
--rw-rw-rw-   0 root         (0) root         (0)     2977 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/rpm/PARAM_TMVAWeights_rel5.spec
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/testdata/rpm/rel/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/rpm/rel/PARAM_TMVAWeights_v1r4-1.0.0-toto.noarch.rpm
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/rpm/rel/PARAM_TMVAWeights_v1r2-1.0.0-1.noarch.rpm
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/rpm/rel/PARAM_TMVAWeights_v1r4-1.0.0-1.noarch.rpm
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/testdata/rpm/rel/PARAM_TMVAWeights_v1r4-1.0.0-4.noarch.rpm
--rw-rw-rw-   0 root         (0) root         (0)      463 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/.pydevproject
--rw-rw-rw-   0 root         (0) root         (0)    11051 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     2532 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)       54 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      290 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/docs/
--rw-rw-rw-   0 root         (0) root         (0)     7965 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/pylint.rc
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/docs/examples/
--rwxrwxrwx   0 root         (0) root         (0)     1247 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/examples/lbpr-example
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/docs/operation/
--rw-rw-rw-   0 root         (0) root         (0)    26491 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/operation/NightlyBuildsOperation.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/docs/operation/images/
--rw-rw-rw-   0 root         (0) root         (0)      788 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/operation/images/jenkins-jobs.dot
--rw-rw-rw-   0 root         (0) root         (0)    32492 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/operation/images/jenkins-jobs.dot.png
--rw-rw-rw-   0 root         (0) root         (0)      974 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/operation/Makefile
--rw-rw-rw-   0 root         (0) root         (0)    11284 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/operation/NightlyBuildsOperation.rst
--rw-rw-rw-   0 root         (0) root         (0)    25549 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/Interactive builds of LHCb projects.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     2628 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/jenkins-scripts.dot
--rw-rw-rw-   0 root         (0) root         (0)   142880 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/jenkins-scripts.dot.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/docs/note/
--rw-rw-rw-   0 root         (0) root         (0)     2326 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/design.tex
--rw-rw-rw-   0 root         (0) root         (0)     2299 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/introduction.tex
--rw-rw-rw-   0 root         (0) root         (0)    32577 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/cite.sty
--rw-rw-rw-   0 root         (0) root         (0)     3132 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/appendix.tex
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/docs/note/figs/
--rw-rw-rw-   0 root         (0) root         (0)    14116 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/figs/lhcb-logo.pdf
--rw-rw-rw-   0 root         (0) root         (0)   134216 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/figs/old-summary.png
--rw-rw-rw-   0 root         (0) root         (0)   101416 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/figs/cdash-3.png
--rw-rw-rw-   0 root         (0) root         (0)    60108 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/figs/cdash-1.png
--rw-rw-rw-   0 root         (0) root         (0)   173109 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/figs/jenkins-3.png
--rw-rw-rw-   0 root         (0) root         (0)   162025 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/figs/cdash-4.png
--rw-rw-rw-   0 root         (0) root         (0)    81047 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/figs/jenkins-2.png
--rw-rw-rw-   0 root         (0) root         (0)    91381 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/figs/jenkins-1.png
--rw-rw-rw-   0 root         (0) root         (0)    97134 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/figs/cdash-2.png
--rw-rw-rw-   0 root         (0) root         (0)   160146 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/figs/lhcb-logo.eps
--rw-rw-rw-   0 root         (0) root         (0)      185 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/README.txt
--rw-rw-rw-   0 root         (0) root         (0)     2787 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/preamble.tex
--rw-rw-rw-   0 root         (0) root         (0)   946715 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/LHCb-INT-2013-006.pdf
--rw-rw-rw-   0 root         (0) root         (0)      567 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/conclusions.tex
--rwxrwxrwx   0 root         (0) root         (0)     3645 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/listsymbols
--rw-rw-rw-   0 root         (0) root         (0)     5975 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/dashboard.tex
--rw-rw-rw-   0 root         (0) root         (0)     5159 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/bibliography.bib
--rw-rw-rw-   0 root         (0) root         (0)     5596 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/lhcb-int-2013-006.kilepr
--rw-rw-rw-   0 root         (0) root         (0)     1363 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/requirements.tex
--rw-rw-rw-   0 root         (0) root         (0)    24755 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/LHCb.bst
--rw-rw-rw-   0 root         (0) root         (0)    28733 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/unsrturl.bst
--rw-rw-rw-   0 root         (0) root         (0)     1681 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     2478 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/title-LHCb-ANA.tex
--rw-rw-rw-   0 root         (0) root         (0)     1586 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/main.tex
--rw-rw-rw-   0 root         (0) root         (0)    33058 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/implementation.tex
--rw-rw-rw-   0 root         (0) root         (0)    61172 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/note/mciteplus.sty
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/docs/configuration/
--rw-rw-rw-   0 root         (0) root         (0)     3047 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/configuration/Example.py
--rw-rw-rw-   0 root         (0) root         (0)     1318 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/docs/LHCbPR2.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/merge_requests/
--rw-rw-rw-   0 root         (0) root         (0)       23 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/merge_requests/_id
--rw-rw-rw-   0 root         (0) root         (0)       11 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/merge_requests/language
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/merge_requests/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/merge_requests/views/mrs/
--rw-rw-rw-   0 root         (0) root         (0)      756 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/merge_requests/views/mrs/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/merge_requests/views/mr_slots_by_ref_slot/
--rw-rw-rw-   0 root         (0) root         (0)      307 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/merge_requests/views/mr_slots_by_ref_slot/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/deployment/
--rw-rw-rw-   0 root         (0) root         (0)       18 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/deployment/_id
--rw-rw-rw-   0 root         (0) root         (0)       10 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/deployment/language
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/deployment/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/deployment/views/ready/
--rw-rw-rw-   0 root         (0) root         (0)      920 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/deployment/views/ready/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/nightlies_summaries/
--rw-rw-rw-   0 root         (0) root         (0)       27 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/nightlies_summaries/_id
--rw-rw-rw-   0 root         (0) root         (0)       10 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/nightlies_summaries/language
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/nightlies_summaries/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/nightlies_summaries/views/by_app_version/
--rw-rw-rw-   0 root         (0) root         (0)       97 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/nightlies_summaries/views/by_app_version/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/frontend-stats/
--rw-rw-rw-   0 root         (0) root         (0)       22 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/frontend-stats/_id
--rw-rw-rw-   0 root         (0) root         (0)       82 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/frontend-stats/couchapp.json
--rw-rw-rw-   0 root         (0) root         (0)       10 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/frontend-stats/language
--rw-rw-rw-   0 root         (0) root         (0)      176 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/frontend-stats/.couchappignore
--rw-rw-rw-   0 root         (0) root         (0)      679 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/frontend-stats/README.md
--rw-rw-rw-   0 root         (0) root         (0)      115 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/frontend-stats/.couchapprc
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/frontend-stats/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/frontend-stats/views/byDate/
--rw-rw-rw-   0 root         (0) root         (0)     2489 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/frontend-stats/views/byDate/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/auth/
--rw-rw-rw-   0 root         (0) root         (0)     1085 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/auth/validate_doc_update.js
--rw-rw-rw-   0 root         (0) root         (0)      982 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/Push CouchDB Nightly Builds.launch
--rwxrwxrwx   0 root         (0) root         (0)     3494 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/webapp_testbench.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/periodic_summaries/
--rw-rw-rw-   0 root         (0) root         (0)       26 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/periodic_summaries/_id
--rw-rw-rw-   0 root         (0) root         (0)       10 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/periodic_summaries/language
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/periodic_summaries/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/periodic_summaries/views/byTime/
--rw-rw-rw-   0 root         (0) root         (0)       74 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/periodic_summaries/views/byTime/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/names/
--rw-rw-rw-   0 root         (0) root         (0)       14 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/names/_id
--rw-rw-rw-   0 root         (0) root         (0)       10 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/names/language
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/names/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/names/views/platforms/
--rw-rw-rw-   0 root         (0) root         (0)      149 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/names/views/platforms/reduce.js
--rw-rw-rw-   0 root         (0) root         (0)      140 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/names/views/platforms/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/names/views/slots/
--rw-rw-rw-   0 root         (0) root         (0)      149 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/names/views/slots/reduce.js
--rw-rw-rw-   0 root         (0) root         (0)       81 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/names/views/slots/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/names/views/projects/
--rw-rw-rw-   0 root         (0) root         (0)      149 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/names/views/projects/reduce.js
--rw-rw-rw-   0 root         (0) root         (0)      142 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/names/views/projects/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/old_dashboard/
--rw-rw-rw-   0 root         (0) root         (0)       21 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/old_dashboard/_id
--rw-rw-rw-   0 root         (0) root         (0)       10 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/old_dashboard/language
--rw-rw-rw-   0 root         (0) root         (0)      791 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/old_dashboard/rewrites.json
--rw-rw-rw-   0 root         (0) root         (0)     1744 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/README.md
--rw-rw-rw-   0 root         (0) root         (0)      486 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/build_id_index.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/summaries/
--rw-rw-rw-   0 root         (0) root         (0)       17 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/summaries/_id
--rw-rw-rw-   0 root         (0) root         (0)       10 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/summaries/language
--rw-rw-rw-   0 root         (0) root         (0)      264 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/summaries/rewrites.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/summaries/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/summaries/views/lastBuildId/
--rw-rw-rw-   0 root         (0) root         (0)      190 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/summaries/views/lastBuildId/reduce.js
--rw-rw-rw-   0 root         (0) root         (0)       89 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/summaries/views/lastBuildId/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/summaries/views/byDay/
--rw-rw-rw-   0 root         (0) root         (0)      347 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/summaries/views/byDay/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/releases/
--rw-rw-rw-   0 root         (0) root         (0)       16 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/releases/_id
--rw-rw-rw-   0 root         (0) root         (0)       10 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/releases/language
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/releases/lists/
--rw-rw-rw-   0 root         (0) root         (0)      153 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/releases/lists/projectBuildIds.js
--rw-rw-rw-   0 root         (0) root         (0)      185 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/releases/rewrites.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/releases/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/couchdb/releases/views/projectBuildIds/
--rw-rw-rw-   0 root         (0) root         (0)      165 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/releases/views/projectBuildIds/map.js
--rw-rw-rw-   0 root         (0) root         (0)       12 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/couchdb/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/python/LbPeriodicTools/
--rw-rw-rw-   0 root         (0) root         (0)     1600 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbPeriodicTools/TestSchedule.xsd
--rw-rw-rw-   0 root         (0) root         (0)     4133 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbPeriodicTools/LbPeriodicStarter.py
--rw-rw-rw-   0 root         (0) root         (0)    10843 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbPeriodicTools/LbPeriodicTest.py
--rw-rw-rw-   0 root         (0) root         (0)    10085 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbPeriodicTools/_entry_points.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbPeriodicTools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2147 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbPeriodicTools/LbPeriodicTestSchedule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/python/LbPeriodicTools/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3611 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbPeriodicTools/tests/TestStarter.py
--rw-rw-rw-   0 root         (0) root         (0)     4173 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbPeriodicTools/tests/TestXMLParsing.py
--rw-rw-rw-   0 root         (0) root         (0)     2340 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbPeriodicTools/tests/TestLHCbPR.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbPeriodicTools/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/python/LbTools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbTools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4235 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbTools/Manifest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/python/LbTools/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3869 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbTools/tests/TestXMLParsing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/python/LbNightlyTools.egg-info/
--rw-r--r--   0 root         (0) root         (0)      896 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/python/LbNightlyTools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      123 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/python/LbNightlyTools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      236 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/python/LbNightlyTools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)    12185 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/python/LbNightlyTools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     2748 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/python/LbNightlyTools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       61 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/python/LbNightlyTools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-04-22 07:27:45.000000 LbNightlyTools-3.0.8/python/LbNightlyTools.egg-info/not-zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/python/LbPR/
--rw-rw-rw-   0 root         (0) root         (0)     3004 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbPR/LbPRJobManager.py
--rw-rw-rw-   0 root         (0) root         (0)    13825 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbPR/_entry_points.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbPR/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/python/LbMsg/
--rwxrwxrwx   0 root         (0) root         (0)     3411 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbMsg/BuildMsg.py
--rw-rw-rw-   0 root         (0) root         (0)     4725 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbMsg/Common.py
--rw-rw-rw-   0 root         (0) root         (0)     3363 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbMsg/TestMsg.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbMsg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/python/LbRPMTools/
--rw-rw-rw-   0 root         (0) root         (0)    22655 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbRPMTools/LHCbExternalsSpecBuilder.py
--rw-rw-rw-   0 root         (0) root         (0)    16260 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbRPMTools/LHCbLbScriptsSpecBuilder.py
--rw-rw-rw-   0 root         (0) root         (0)    49470 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbRPMTools/LHCbRPMSpecBuilder.py
--rw-rw-rw-   0 root         (0) root         (0)    10023 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbRPMTools/LHCbCompatSpecBuilder.py
--rw-rw-rw-   0 root         (0) root         (0)    10051 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbRPMTools/LHCbGenericSpecBuilder.py
--rw-rw-rw-   0 root         (0) root         (0)     8660 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbRPMTools/LHCbMetaSpecBuilder.py
--rw-rw-rw-   0 root         (0) root         (0)    28105 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbRPMTools/PackageSlot.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbRPMTools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/python/LbRPMTools/tests/
--rw-rw-rw-   0 root         (0) root         (0)    13491 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbRPMTools/tests/TestSpec.py
--rw-rw-rw-   0 root         (0) root         (0)    13068 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbRPMTools/tests/TestPackageSlot.py
--rw-rw-rw-   0 root         (0) root         (0)     5904 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbRPMTools/tests/TestExternalSpec.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbRPMTools/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/
--rw-rw-rw-   0 root         (0) root         (0)     6052 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/ProcUtils.py
--rw-rw-rw-   0 root         (0) root         (0)    42540 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/Utils.py
--rw-rw-rw-   0 root         (0) root         (0)    18491 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/HTMLUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     4285 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/LbScriptsUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     3649 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/CheckSlotPreconditions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/
--rw-rw-rw-   0 root         (0) root         (0)    11736 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/EnabledSlots.py
--rw-rw-rw-   0 root         (0) root         (0)    14486 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/Test.py
--rw-rw-rw-   0 root         (0) root         (0)     7624 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/Index.py
--rw-rw-rw-   0 root         (0) root         (0)    15853 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/CollectBuildLogs.py
--rw-rw-rw-   0 root         (0) root         (0)    23886 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/Install.py
--rw-rw-rw-   0 root         (0) root         (0)      999 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/listzip.php
--rwxrwxrwx   0 root         (0) root         (0)    26588 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/Common.py
--rw-rw-rw-   0 root         (0) root         (0)     4597 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/Preconditions.py
--rw-rw-rw-   0 root         (0) root         (0)    34123 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/Build.py
--rw-rw-rw-   0 root         (0) root         (0)     3014 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/extract.php
--rw-rw-rw-   0 root         (0) root         (0)    12214 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/GitlabMR.py
--rw-rw-rw-   0 root         (0) root         (0)    28433 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/_entry_points.py
--rw-rw-rw-   0 root         (0) root         (0)    17598 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/Release.py
--rw-rw-rw-   0 root         (0) root         (0)      890 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14858 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/Checkout.py
--rw-rw-rw-   0 root         (0) root         (0)     4373 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/ArtifactsServer.py
--rw-rw-rw-   0 root         (0) root         (0)    12018 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/BuildLogScanner.py
--rw-rw-rw-   0 root         (0) root         (0)    39104 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/CheckoutMethods.py
--rw-rw-rw-   0 root         (0) root         (0)    84038 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/Configuration.py
--rwxrwxrwx   0 root         (0) root         (0)     5098 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/GetNightlyRefs.py
--rw-rw-rw-   0 root         (0) root         (0)    14597 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/MergeRequestBuilds.py
--rw-rw-rw-   0 root         (0) root         (0)    25212 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/BuildMethods.py
--rw-rw-rw-   0 root         (0) root         (0)     6769 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/GitlabUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     1478 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2103 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_config_pickle.py
--rw-rw-rw-   0 root         (0) root         (0)     1758 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_jobconfig.py
--rw-rw-rw-   0 root         (0) root         (0)     3573 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_gitlab_mr_script.py
--rw-rw-rw-   0 root         (0) root         (0)     1869 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_indexer.py
--rw-rw-rw-   0 root         (0) root         (0)    25318 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_config_load.py
--rw-rw-rw-   0 root         (0) root         (0)     1539 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_retry.py
--rw-rw-rw-   0 root         (0) root         (0)     4900 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_checkout_script.py
--rw-rw-rw-   0 root         (0) root         (0)     5892 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_coverity_support.py
--rw-rw-rw-   0 root         (0) root         (0)    18039 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_build_script.py
--rw-rw-rw-   0 root         (0) root         (0)     7901 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_release_poll.py
--rw-rw-rw-   0 root         (0) root         (0)     2565 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_install.py
--rw-rw-rw-   0 root         (0) root         (0)     3223 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_copytree.py
--rw-rw-rw-   0 root         (0) root         (0)     1404 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     6722 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_build.py
--rw-rw-rw-   0 root         (0) root         (0)     3204 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1322 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_precond.py
--rw-rw-rw-   0 root         (0) root         (0)    14547 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_enabled_slots_script.py
--rw-rw-rw-   0 root         (0) root         (0)     1098 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    20507 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_checkout.py
--rw-rw-rw-   0 root         (0) root         (0)    12665 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_rel_gen_script.py
--rw-rw-rw-   0 root         (0) root         (0)    15015 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     5596 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_pack.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/python/LbNightlyTools/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      166 2020-04-22 07:28:04.000000 LbNightlyTools-3.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    11343 2020-04-22 07:27:35.000000 LbNightlyTools-3.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/COPYING
+-rw-r--r--   0 root         (0) root         (0)      896 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4772 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/.cproject
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/cmt/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/cmt/requirements
+-rw-rw-rw-   0 root         (0) root         (0)       79 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/cmt/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)       72 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      954 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/setup.csh
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1698 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/utils/add_ci_webhook.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/setup.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/cron/
+-rwxrwxrwx   0 root         (0) root         (0)     1518 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/cron/cleanup_artifacts.sh
+-rwxrwxrwx   0 root         (0) root         (0)     2118 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/cron/preheat_nightly_dashboard.sh
+-rw-rw-rw-   0 root         (0) root         (0)      154 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/cron/logrotate.conf
+-rwxrwxrwx   0 root         (0) root         (0)     2034 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/cron/clean_up_reduced_db.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)     1595 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/scripts/lbn-wrapcmd
+-rwxrwxrwx   0 root         (0) root         (0)     2340 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/scripts/lbpr-collect
+-rwxrwxrwx   0 root         (0) root         (0)     1053 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/scripts/lbn-get-configs
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/admin/
+-rwxrwxrwx   0 root         (0) root         (0)     1901 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/admin/RpmHelpers.py
+-rwxrwxrwx   0 root         (0) root         (0)     3723 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/admin/createLbScriptsRpm
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/admin/LHCb_LbScripts.spectemplate
+-rw-rw-rw-   0 root         (0) root         (0)      368 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/.project
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/jenkins/
+-rwxrwxrwx   0 root         (0) root         (0)      943 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/utils.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/jenkins/mock/
+-rwxrwxrwx   0 root         (0) root         (0)      936 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/mock/clean_checkout.sh
+-rwxrwxrwx   0 root         (0) root         (0)      887 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/mock/clean_build.sh
+-rwxrwxrwx   0 root         (0) root         (0)      864 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/mock/clean_preconditions.sh
+-rwxrwxrwx   0 root         (0) root         (0)      904 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/mock/clean_enabled_slots.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/jenkins/testrunners/
+-rwxrwxrwx   0 root         (0) root         (0)      382 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/testrunners/qmtest.sh
+-rwxrwxrwx   0 root         (0) root         (0)      605 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/testrunners/lhcbpr.sh
+-rwxrwxrwx   0 root         (0) root         (0)      387 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/testrunners/default.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/jenkins/nightly-builds/
+-rwxrwxrwx   0 root         (0) root         (0)      966 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/nightly-builds/tests-poll.sh
+-rwxrwxrwx   0 root         (0) root         (0)    15845 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/nightly-builds/gitlab-mr.py
+-rwxrwxrwx   0 root         (0) root         (0)     2864 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/nightly-builds/checkout.sh
+-rwxrwxrwx   0 root         (0) root         (0)     2571 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/nightly-builds/tests.sh
+-rwxrwxrwx   0 root         (0) root         (0)     1403 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/nightly-builds/main.sh
+-rwxrwxrwx   0 root         (0) root         (0)     1093 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/nightly-builds/release-poll.sh
+-rwxrwxrwx   0 root         (0) root         (0)     2256 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/nightly-builds/gaudi_mr_poll.py
+-rwxrwxrwx   0 root         (0) root         (0)      903 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/nightly-builds/preconditions.sh
+-rwxrwxrwx   0 root         (0) root         (0)     3176 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/nightly-builds/build.sh
+-rwxrwxrwx   0 root         (0) root         (0)      933 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/nightly-builds/release.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/jenkins/periodic-tests/
+-rwxrwxrwx   0 root         (0) root         (0)     1219 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/periodic-tests/tests-pollqueue.sh
+-rwxrwxrwx   0 root         (0) root         (0)     1170 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/periodic-tests/tests-poll.sh
+-rwxrwxrwx   0 root         (0) root         (0)     2276 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/periodic-tests/tests.sh
+-rwxrwxrwx   0 root         (0) root         (0)      892 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/periodic-tests/tests-getteststorun.sh
+-rwxrwxrwx   0 root         (0) root         (0)     2410 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/mock.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/jenkins/utils.d/
+-rw-rw-rw-   0 root         (0) root         (0)     7244 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/utils.d/build_slot.sh
+-rw-rw-rw-   0 root         (0) root         (0)     5278 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/utils.d/set_common.sh
+-rw-rw-rw-   0 root         (0) root         (0)     2639 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/utils.d/check_preconditions.sh
+-rw-rw-rw-   0 root         (0) root         (0)     6055 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/utils.d/checkout_slot.sh
+-rw-rw-rw-   0 root         (0) root         (0)     2029 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/utils.d/execute_preconditions.sh
+-rwxrwxrwx   0 root         (0) root         (0)     2327 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/docker.sh
+-rwxrwxrwx   0 root         (0) root         (0)     2364 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/testMock.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/jenkins/docker-home/
+-rw-rw-rw-   0 root         (0) root         (0)      131 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/docker-home/.bashrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/jenkins/docker-home/.ssh/
+-rw-rw-rw-   0 root         (0) root         (0)      234 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/docker-home/.ssh/config
+-rw-rw-rw-   0 root         (0) root         (0)      183 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/jenkins/docker-home/.bash_profile
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/periodic_tests/
+-rw-rw-rw-   0 root         (0) root         (0)      883 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/periodic_tests/starter_schedule.xml
+-rw-rw-rw-   0 root         (0) root         (0)      402 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/periodic_tests/scheduleIncorrect.xml
+-rw-rw-rw-   0 root         (0) root         (0)      486 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/periodic_tests/lhcbpr_schedule.xml
+-rw-rw-rw-   0 root         (0) root         (0)      742 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/periodic_tests/schedule.xml
+-rw-rw-rw-   0 root         (0) root         (0)    15857 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/periodic_tests/slotbuilds.json
+-rw-rw-rw-   0 root         (0) root         (0)      398 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/testing-slot-lbcore-664.json
+-rw-rw-rw-   0 root         (0) root         (0)      381 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/testing-slot-2b.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/fix_glimpse/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/fix_glimpse/untouched/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/fix_glimpse/untouched/.glimpse_filenames
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/fix_glimpse/levelA/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/fix_glimpse/levelA/levelB/
+-rw-rw-rw-   0 root         (0) root         (0)       10 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/fix_glimpse/levelA/levelB/.glimpse_filenames
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/fix_glimpse/level1/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/fix_glimpse/level1/.glimpse_filenames
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/fix_glimpse/level1/level2/
+-rw-rw-rw-   0 root         (0) root         (0)       19 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/fix_glimpse/level1/level2/.glimpse_filenames
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/fix_glimpse/docs/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/fix_glimpse/docs/.glimpse_filenames
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/indexer/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/build.dir/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/build.dir/IgnoredSource.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/InstallArea/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/InstallArea/cmake/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/InstallArea/cmake/AProjectConfig.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/InstallArea/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/InstallArea/python/MyPackage/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/InstallArea/python/MyPackage/MyPackage_user_confDb.py
+-rw-rw-rw-   0 root         (0) root         (0)       19 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/InstallArea/python/MyPackage/MyPackage_confDb.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/InstallArea/python/MyPackage/SomeModule.py
+-rw-rw-rw-   0 root         (0) root         (0)       16 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/InstallArea/python/MyPackage/SomethingConf.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/InstallArea/python/MyPackage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/InstallArea/python/MyPackage/MyPackageConf.py
+-rw-rw-rw-   0 root         (0) root         (0)       26 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/InstallArea/python/AProject_merged_confDb.py
+-rw-rw-rw-   0 root         (0) root         (0)       24 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/InstallArea/python/GeneratedPython.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/InstallArea/include/
+-rw-rw-rw-   0 root         (0) root         (0)       14 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/InstallArea/include/MyHeader.h
+-rw-rw-rw-   0 root         (0) root         (0)       24 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/InstallArea/include/GeneratedHeader.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/MyPackage/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/MyPackage/Headers/
+-rw-rw-rw-   0 root         (0) root         (0)       14 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/MyPackage/Headers/MyHeader.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/MyPackage/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)       11 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/MyPackage/scripts/MyScript
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/MyPackage/src/
+-rw-rw-rw-   0 root         (0) root         (0)       15 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/MyPackage/src/MySource.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/MyPackage/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/MyPackage/python/MyPackage/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/MyPackage/python/MyPackage/SomeModule.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/indexer/AProject/MyPackage/python/MyPackage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/testing-slot-with-shared.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/coverity/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/coverity/configs/
+-rw-rw-rw-   0 root         (0) root         (0)      110 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/coverity/configs/coverity_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/coverity/build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/coverity/build/TEST/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/coverity/build/TEST/TEST_HEAD/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/coverity/build/TEST/TEST_HEAD/InstallArea/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/coverity/build/TEST/TEST_HEAD/InstallArea/.empty
+-rw-rw-rw-   0 root         (0) root         (0)      256 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/coverity/build/TEST/TEST_HEAD/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      310 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/coverity/build/TEST/TEST_HEAD/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/coverity/bin/
+-rwxrwxrwx   0 root         (0) root         (0)     1694 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/coverity/bin/cov-commit-defects
+-rwxrwxrwx   0 root         (0) root         (0)     1695 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/coverity/bin/cov-analyze
+-rwxrwxrwx   0 root         (0) root         (0)     1545 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/coverity/bin/cov-build
+-rw-rw-rw-   0 root         (0) root         (0)      414 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/testing-slot-2.json
+-rw-rw-rw-   0 root         (0) root         (0)      279 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/testing-slot-lbcore-192.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      658 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/tools/manifest.xml
+-rw-rw-rw-   0 root         (0) root         (0)      103 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/tools/mini_manifest.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/tools/manifest_do0.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/tools/manifest_with_pkgs.xml
+-rw-rw-rw-   0 root         (0) root         (0)      219 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/testing-slot.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/artifacts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/artifacts/packs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/artifacts/packs/src/
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/artifacts/packs/src/TestProject.HEAD.testing-slot.src.zip
+-rw-rw-rw-   0 root         (0) root         (0)      244 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/data-packs.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmt/Lbcom/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmt/Lbcom/cmt/
+-rw-rw-rw-   0 root         (0) root         (0)       19 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmt/Lbcom/cmt/project.cmt
+-rw-rw-rw-   0 root         (0) root         (0)      559 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmt/conf.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmt/Online/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmt/Online/cmt/
+-rw-rw-rw-   0 root         (0) root         (0)      115 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmt/Online/cmt/project.cmt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmt/Brunel/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmt/Brunel/cmt/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmt/Brunel/cmt/project.cmt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmt/Rec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmt/Rec/cmt/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmt/Rec/cmt/project.cmt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmt/Gaudi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmt/Gaudi/cmt/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmt/Gaudi/cmt/project.cmt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmt/LHCb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmt/LHCb/cmt/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmt/LHCb/cmt/project.cmt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmt/NewProj/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmt/NewProj/project.info
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmake/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmake/Lbcom/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmake/Lbcom/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)      561 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmake/conf.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmake/Online/
+-rw-rw-rw-   0 root         (0) root         (0)      117 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmake/Online/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmake/Brunel/
+-rw-rw-rw-   0 root         (0) root         (0)      111 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmake/Brunel/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmake/Rec/
+-rw-rw-rw-   0 root         (0) root         (0)       52 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmake/Rec/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmake/Gaudi/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmake/Gaudi/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)       25 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmake/Gaudi/toolchain.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmake/LHCb/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmake/LHCb/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmake/NewProj/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/collect_deps/cmake/NewProj/project.info
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/broken/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/broken/BadCMake/
+-rw-rw-rw-   0 root         (0) root         (0)       14 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/collect_deps/broken/BadCMake/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/broken/BadCMT/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/broken/BadCMT/cmt/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/collect_deps/broken/BadCMT/cmt/project.cmt
+-rw-rw-rw-   0 root         (0) root         (0)      295 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/collect_deps/broken/conf.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/collect_deps/broken/Gaudi/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/collect_deps/broken/Gaudi/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)       25 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/collect_deps/broken/Gaudi/toolchain.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/build_tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/build_tests/orig/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/build_tests/orig/dummy/
+-rw-rw-rw-   0 root         (0) root         (0)      392 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/build_tests/orig/dummy/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      364 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/testing-slot-env.json
+-rw-rw-rw-   0 root         (0) root         (0)     6009 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/ci-test-hook-content.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/rpm/
+-rw-rw-rw-   0 root         (0) root         (0)     2977 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/rpm/PARAM_TMVAWeights.spec
+-rw-rw-rw-   0 root         (0) root         (0)      617 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/rpm/manifest.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1265 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/rpm/Brunel_v46r0.spec
+-rw-rw-rw-   0 root         (0) root         (0)      961 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/rpm/datapkg-slot-config.json
+-rw-rw-rw-   0 root         (0) root         (0)      915 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/rpm/slot-configdo0.json
+-rw-rw-rw-   0 root         (0) root         (0)     7195 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/rpm/LCG_68_externalsDict.json
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/rpm/manifest_do0.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/rpm/glimpse_Brunel_v46r0.spec
+-rw-rw-rw-   0 root         (0) root         (0)     1630 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/rpm/Brunel_v46r0_x86_64-slc6-gcc48-opt.spec
+-rw-rw-rw-   0 root         (0) root         (0)     2476 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/rpm/Gaudi_v27r0_x86_64-slc6-gcc49-do0.spec
+-rw-rw-rw-   0 root         (0) root         (0)      915 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/rpm/slot-config.json
+-rw-rw-rw-   0 root         (0) root         (0)     2977 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/rpm/PARAM_TMVAWeights_rel5.spec
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/testdata/rpm/rel/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/rpm/rel/PARAM_TMVAWeights_v1r4-1.0.0-toto.noarch.rpm
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/rpm/rel/PARAM_TMVAWeights_v1r2-1.0.0-1.noarch.rpm
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/rpm/rel/PARAM_TMVAWeights_v1r4-1.0.0-1.noarch.rpm
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/testdata/rpm/rel/PARAM_TMVAWeights_v1r4-1.0.0-4.noarch.rpm
+-rw-rw-rw-   0 root         (0) root         (0)      463 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/.pydevproject
+-rw-rw-rw-   0 root         (0) root         (0)    11051 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     2532 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)       54 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      290 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     7965 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/pylint.rc
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/docs/examples/
+-rwxrwxrwx   0 root         (0) root         (0)     1247 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/examples/lbpr-example
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/docs/operation/
+-rw-rw-rw-   0 root         (0) root         (0)    26491 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/operation/NightlyBuildsOperation.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/docs/operation/images/
+-rw-rw-rw-   0 root         (0) root         (0)      788 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/operation/images/jenkins-jobs.dot
+-rw-rw-rw-   0 root         (0) root         (0)    32492 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/operation/images/jenkins-jobs.dot.png
+-rw-rw-rw-   0 root         (0) root         (0)      974 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/operation/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)    11284 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/operation/NightlyBuildsOperation.rst
+-rw-rw-rw-   0 root         (0) root         (0)    25549 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/Interactive builds of LHCb projects.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     2628 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/jenkins-scripts.dot
+-rw-rw-rw-   0 root         (0) root         (0)   142880 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/jenkins-scripts.dot.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/docs/note/
+-rw-rw-rw-   0 root         (0) root         (0)     2326 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/design.tex
+-rw-rw-rw-   0 root         (0) root         (0)     2299 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/introduction.tex
+-rw-rw-rw-   0 root         (0) root         (0)    32577 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/cite.sty
+-rw-rw-rw-   0 root         (0) root         (0)     3132 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/appendix.tex
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/docs/note/figs/
+-rw-rw-rw-   0 root         (0) root         (0)    14116 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/figs/lhcb-logo.pdf
+-rw-rw-rw-   0 root         (0) root         (0)   134216 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/figs/old-summary.png
+-rw-rw-rw-   0 root         (0) root         (0)   101416 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/figs/cdash-3.png
+-rw-rw-rw-   0 root         (0) root         (0)    60108 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/figs/cdash-1.png
+-rw-rw-rw-   0 root         (0) root         (0)   173109 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/figs/jenkins-3.png
+-rw-rw-rw-   0 root         (0) root         (0)   162025 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/figs/cdash-4.png
+-rw-rw-rw-   0 root         (0) root         (0)    81047 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/figs/jenkins-2.png
+-rw-rw-rw-   0 root         (0) root         (0)    91381 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/figs/jenkins-1.png
+-rw-rw-rw-   0 root         (0) root         (0)    97134 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/figs/cdash-2.png
+-rw-rw-rw-   0 root         (0) root         (0)   160146 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/figs/lhcb-logo.eps
+-rw-rw-rw-   0 root         (0) root         (0)      185 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/README.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2787 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/preamble.tex
+-rw-rw-rw-   0 root         (0) root         (0)   946715 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/LHCb-INT-2013-006.pdf
+-rw-rw-rw-   0 root         (0) root         (0)      567 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/conclusions.tex
+-rwxrwxrwx   0 root         (0) root         (0)     3645 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/listsymbols
+-rw-rw-rw-   0 root         (0) root         (0)     5975 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/dashboard.tex
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/bibliography.bib
+-rw-rw-rw-   0 root         (0) root         (0)     5596 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/lhcb-int-2013-006.kilepr
+-rw-rw-rw-   0 root         (0) root         (0)     1363 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/requirements.tex
+-rw-rw-rw-   0 root         (0) root         (0)    24755 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/LHCb.bst
+-rw-rw-rw-   0 root         (0) root         (0)    28733 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/unsrturl.bst
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     2478 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/title-LHCb-ANA.tex
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/main.tex
+-rw-rw-rw-   0 root         (0) root         (0)    33058 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/implementation.tex
+-rw-rw-rw-   0 root         (0) root         (0)    61172 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/note/mciteplus.sty
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/docs/configuration/
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/configuration/Example.py
+-rw-rw-rw-   0 root         (0) root         (0)     1318 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/docs/LHCbPR2.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/merge_requests/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/merge_requests/_id
+-rw-rw-rw-   0 root         (0) root         (0)       11 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/merge_requests/language
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/merge_requests/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/merge_requests/views/mrs/
+-rw-rw-rw-   0 root         (0) root         (0)      756 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/merge_requests/views/mrs/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/merge_requests/views/mr_slots_by_ref_slot/
+-rw-rw-rw-   0 root         (0) root         (0)      307 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/merge_requests/views/mr_slots_by_ref_slot/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/deployment/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/deployment/_id
+-rw-rw-rw-   0 root         (0) root         (0)       10 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/deployment/language
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/deployment/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/deployment/views/ready/
+-rw-rw-rw-   0 root         (0) root         (0)      920 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/deployment/views/ready/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/nightlies_summaries/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/nightlies_summaries/_id
+-rw-rw-rw-   0 root         (0) root         (0)       10 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/nightlies_summaries/language
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/nightlies_summaries/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/nightlies_summaries/views/by_app_version/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/nightlies_summaries/views/by_app_version/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/frontend-stats/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/frontend-stats/_id
+-rw-rw-rw-   0 root         (0) root         (0)       82 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/frontend-stats/couchapp.json
+-rw-rw-rw-   0 root         (0) root         (0)       10 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/frontend-stats/language
+-rw-rw-rw-   0 root         (0) root         (0)      176 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/frontend-stats/.couchappignore
+-rw-rw-rw-   0 root         (0) root         (0)      679 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/frontend-stats/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      115 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/frontend-stats/.couchapprc
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/frontend-stats/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/frontend-stats/views/byDate/
+-rw-rw-rw-   0 root         (0) root         (0)     2489 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/frontend-stats/views/byDate/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/auth/
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/auth/validate_doc_update.js
+-rw-rw-rw-   0 root         (0) root         (0)      982 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/Push CouchDB Nightly Builds.launch
+-rwxrwxrwx   0 root         (0) root         (0)     3494 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/webapp_testbench.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/periodic_summaries/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/periodic_summaries/_id
+-rw-rw-rw-   0 root         (0) root         (0)       10 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/periodic_summaries/language
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/periodic_summaries/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/periodic_summaries/views/byTime/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/periodic_summaries/views/byTime/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/names/
+-rw-rw-rw-   0 root         (0) root         (0)       14 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/names/_id
+-rw-rw-rw-   0 root         (0) root         (0)       10 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/names/language
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/names/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/names/views/platforms/
+-rw-rw-rw-   0 root         (0) root         (0)      149 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/names/views/platforms/reduce.js
+-rw-rw-rw-   0 root         (0) root         (0)      140 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/names/views/platforms/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/names/views/slots/
+-rw-rw-rw-   0 root         (0) root         (0)      149 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/names/views/slots/reduce.js
+-rw-rw-rw-   0 root         (0) root         (0)       81 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/names/views/slots/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/names/views/projects/
+-rw-rw-rw-   0 root         (0) root         (0)      149 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/names/views/projects/reduce.js
+-rw-rw-rw-   0 root         (0) root         (0)      142 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/names/views/projects/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/old_dashboard/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/old_dashboard/_id
+-rw-rw-rw-   0 root         (0) root         (0)       10 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/old_dashboard/language
+-rw-rw-rw-   0 root         (0) root         (0)      791 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/old_dashboard/rewrites.json
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      486 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/build_id_index.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/summaries/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/summaries/_id
+-rw-rw-rw-   0 root         (0) root         (0)       10 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/summaries/language
+-rw-rw-rw-   0 root         (0) root         (0)      264 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/summaries/rewrites.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/summaries/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/summaries/views/lastBuildId/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/summaries/views/lastBuildId/reduce.js
+-rw-rw-rw-   0 root         (0) root         (0)       89 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/summaries/views/lastBuildId/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/summaries/views/byDay/
+-rw-rw-rw-   0 root         (0) root         (0)      347 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/summaries/views/byDay/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/releases/
+-rw-rw-rw-   0 root         (0) root         (0)       16 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/releases/_id
+-rw-rw-rw-   0 root         (0) root         (0)       10 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/releases/language
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/releases/lists/
+-rw-rw-rw-   0 root         (0) root         (0)      153 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/releases/lists/projectBuildIds.js
+-rw-rw-rw-   0 root         (0) root         (0)      185 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/releases/rewrites.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/releases/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/couchdb/releases/views/projectBuildIds/
+-rw-rw-rw-   0 root         (0) root         (0)      165 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/releases/views/projectBuildIds/map.js
+-rw-rw-rw-   0 root         (0) root         (0)       12 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/couchdb/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/python/LbPeriodicTools/
+-rw-rw-rw-   0 root         (0) root         (0)     1600 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbPeriodicTools/TestSchedule.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     4133 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbPeriodicTools/LbPeriodicStarter.py
+-rw-rw-rw-   0 root         (0) root         (0)    10843 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbPeriodicTools/LbPeriodicTest.py
+-rw-rw-rw-   0 root         (0) root         (0)    10085 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbPeriodicTools/_entry_points.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbPeriodicTools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2147 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbPeriodicTools/LbPeriodicTestSchedule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/python/LbPeriodicTools/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3611 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbPeriodicTools/tests/TestStarter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4173 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbPeriodicTools/tests/TestXMLParsing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2340 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbPeriodicTools/tests/TestLHCbPR.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbPeriodicTools/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/python/LbTools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbTools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4235 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbTools/Manifest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/python/LbTools/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3869 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbTools/tests/TestXMLParsing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/python/LbNightlyTools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      896 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/python/LbNightlyTools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      123 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/python/LbNightlyTools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      236 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/python/LbNightlyTools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)    12185 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/python/LbNightlyTools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     2748 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/python/LbNightlyTools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/python/LbNightlyTools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-05-14 12:41:28.000000 LbNightlyTools-3.0.9/python/LbNightlyTools.egg-info/not-zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/python/LbPR/
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbPR/LbPRJobManager.py
+-rw-rw-rw-   0 root         (0) root         (0)    13502 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbPR/_entry_points.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbPR/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/python/LbMsg/
+-rwxrwxrwx   0 root         (0) root         (0)     3411 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbMsg/BuildMsg.py
+-rw-rw-rw-   0 root         (0) root         (0)     4725 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbMsg/Common.py
+-rw-rw-rw-   0 root         (0) root         (0)     3363 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbMsg/TestMsg.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbMsg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/python/LbRPMTools/
+-rw-rw-rw-   0 root         (0) root         (0)    22655 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbRPMTools/LHCbExternalsSpecBuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)    16260 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbRPMTools/LHCbLbScriptsSpecBuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)    49470 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbRPMTools/LHCbRPMSpecBuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)    10023 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbRPMTools/LHCbCompatSpecBuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)    10051 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbRPMTools/LHCbGenericSpecBuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)     8660 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbRPMTools/LHCbMetaSpecBuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)    28105 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbRPMTools/PackageSlot.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbRPMTools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/python/LbRPMTools/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    13491 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbRPMTools/tests/TestSpec.py
+-rw-rw-rw-   0 root         (0) root         (0)    13068 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbRPMTools/tests/TestPackageSlot.py
+-rw-rw-rw-   0 root         (0) root         (0)     5904 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbRPMTools/tests/TestExternalSpec.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbRPMTools/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/
+-rw-rw-rw-   0 root         (0) root         (0)     6052 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/ProcUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)    42586 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/Utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    18491 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/HTMLUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4285 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/LbScriptsUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3649 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/CheckSlotPreconditions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/
+-rw-rw-rw-   0 root         (0) root         (0)    11736 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/EnabledSlots.py
+-rw-rw-rw-   0 root         (0) root         (0)    14479 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/Test.py
+-rw-rw-rw-   0 root         (0) root         (0)     7624 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/Index.py
+-rw-rw-rw-   0 root         (0) root         (0)    15853 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/CollectBuildLogs.py
+-rw-rw-rw-   0 root         (0) root         (0)    23904 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/Install.py
+-rw-rw-rw-   0 root         (0) root         (0)      999 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/listzip.php
+-rwxrwxrwx   0 root         (0) root         (0)    26588 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/Common.py
+-rw-rw-rw-   0 root         (0) root         (0)     4597 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/Preconditions.py
+-rw-rw-rw-   0 root         (0) root         (0)    34123 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/Build.py
+-rw-rw-rw-   0 root         (0) root         (0)     3014 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/extract.php
+-rw-rw-rw-   0 root         (0) root         (0)    12214 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/GitlabMR.py
+-rw-rw-rw-   0 root         (0) root         (0)    28433 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/_entry_points.py
+-rw-rw-rw-   0 root         (0) root         (0)    17630 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/Release.py
+-rw-rw-rw-   0 root         (0) root         (0)      890 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14858 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/Checkout.py
+-rw-rw-rw-   0 root         (0) root         (0)     4373 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/ArtifactsServer.py
+-rw-rw-rw-   0 root         (0) root         (0)    12018 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/BuildLogScanner.py
+-rw-rw-rw-   0 root         (0) root         (0)    39193 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/CheckoutMethods.py
+-rw-rw-rw-   0 root         (0) root         (0)    84038 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/Configuration.py
+-rwxrwxrwx   0 root         (0) root         (0)     4987 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/GetNightlyRefs.py
+-rw-rw-rw-   0 root         (0) root         (0)    14597 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/MergeRequestBuilds.py
+-rw-rw-rw-   0 root         (0) root         (0)    25212 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/BuildMethods.py
+-rw-rw-rw-   0 root         (0) root         (0)     6769 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/GitlabUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2103 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_config_pickle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1758 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_jobconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     3573 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_gitlab_mr_script.py
+-rw-rw-rw-   0 root         (0) root         (0)     1869 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_indexer.py
+-rw-rw-rw-   0 root         (0) root         (0)    25318 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_config_load.py
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_retry.py
+-rw-rw-rw-   0 root         (0) root         (0)     4900 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_checkout_script.py
+-rw-rw-rw-   0 root         (0) root         (0)     5892 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_coverity_support.py
+-rw-rw-rw-   0 root         (0) root         (0)    18039 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_build_script.py
+-rw-rw-rw-   0 root         (0) root         (0)     7901 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_release_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)     2565 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_install.py
+-rw-rw-rw-   0 root         (0) root         (0)     3223 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_copytree.py
+-rw-rw-rw-   0 root         (0) root         (0)     1404 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6722 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_build.py
+-rw-rw-rw-   0 root         (0) root         (0)     3204 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1322 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_precond.py
+-rw-rw-rw-   0 root         (0) root         (0)    14547 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_enabled_slots_script.py
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    20507 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_checkout.py
+-rw-rw-rw-   0 root         (0) root         (0)    12665 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_rel_gen_script.py
+-rw-rw-rw-   0 root         (0) root         (0)    15015 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5596 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_pack.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/python/LbNightlyTools/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      166 2020-05-14 12:42:19.000000 LbNightlyTools-3.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)    11343 2020-05-14 12:41:20.000000 LbNightlyTools-3.0.9/setup.py
```

### Comparing `LbNightlyTools-3.0.8/COPYING` & `LbNightlyTools-3.0.9/COPYING`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/PKG-INFO` & `LbNightlyTools-3.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: LbNightlyTools
-Version: 3.0.8
+Version: 3.0.9
 Summary: LHCb Nightly tools
 Home-page: https://gitlab.cern.ch/lhcb-core/LbNightlyTools
 Author: CERN - LHCb Core Software
 Author-email: lhcb-core-soft@cern.ch
 License: UNKNOWN
 Description: LbNightlyTools
         ===============
```

### Comparing `LbNightlyTools-3.0.8/.cproject` & `LbNightlyTools-3.0.9/.cproject`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/setup.csh` & `LbNightlyTools-3.0.9/setup.csh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/utils/add_ci_webhook.py` & `LbNightlyTools-3.0.9/utils/add_ci_webhook.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/setup.sh` & `LbNightlyTools-3.0.9/setup.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/cron/cleanup_artifacts.sh` & `LbNightlyTools-3.0.9/cron/cleanup_artifacts.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/cron/preheat_nightly_dashboard.sh` & `LbNightlyTools-3.0.9/cron/preheat_nightly_dashboard.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/cron/clean_up_reduced_db.sh` & `LbNightlyTools-3.0.9/cron/clean_up_reduced_db.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/scripts/lbn-wrapcmd` & `LbNightlyTools-3.0.9/scripts/lbn-wrapcmd`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/scripts/lbpr-collect` & `LbNightlyTools-3.0.9/scripts/lbpr-collect`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/scripts/lbn-get-configs` & `LbNightlyTools-3.0.9/scripts/lbn-get-configs`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/admin/RpmHelpers.py` & `LbNightlyTools-3.0.9/admin/RpmHelpers.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/admin/createLbScriptsRpm` & `LbNightlyTools-3.0.9/admin/createLbScriptsRpm`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/admin/LHCb_LbScripts.spectemplate` & `LbNightlyTools-3.0.9/admin/LHCb_LbScripts.spectemplate`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/utils.sh` & `LbNightlyTools-3.0.9/jenkins/utils.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/mock/clean_checkout.sh` & `LbNightlyTools-3.0.9/jenkins/mock/clean_checkout.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/mock/clean_build.sh` & `LbNightlyTools-3.0.9/jenkins/mock/clean_build.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/mock/clean_preconditions.sh` & `LbNightlyTools-3.0.9/jenkins/mock/clean_preconditions.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/mock/clean_enabled_slots.sh` & `LbNightlyTools-3.0.9/jenkins/mock/clean_enabled_slots.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/testrunners/lhcbpr.sh` & `LbNightlyTools-3.0.9/jenkins/testrunners/lhcbpr.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/nightly-builds/tests-poll.sh` & `LbNightlyTools-3.0.9/jenkins/nightly-builds/tests-poll.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/nightly-builds/gitlab-mr.py` & `LbNightlyTools-3.0.9/jenkins/nightly-builds/gitlab-mr.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/nightly-builds/checkout.sh` & `LbNightlyTools-3.0.9/jenkins/nightly-builds/checkout.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/nightly-builds/tests.sh` & `LbNightlyTools-3.0.9/jenkins/nightly-builds/tests.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/nightly-builds/main.sh` & `LbNightlyTools-3.0.9/jenkins/nightly-builds/main.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/nightly-builds/release-poll.sh` & `LbNightlyTools-3.0.9/jenkins/nightly-builds/release-poll.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/nightly-builds/gaudi_mr_poll.py` & `LbNightlyTools-3.0.9/jenkins/nightly-builds/gaudi_mr_poll.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/nightly-builds/preconditions.sh` & `LbNightlyTools-3.0.9/jenkins/nightly-builds/preconditions.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/nightly-builds/build.sh` & `LbNightlyTools-3.0.9/jenkins/nightly-builds/build.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/nightly-builds/release.sh` & `LbNightlyTools-3.0.9/jenkins/nightly-builds/release.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/periodic-tests/tests-pollqueue.sh` & `LbNightlyTools-3.0.9/jenkins/periodic-tests/tests-pollqueue.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/periodic-tests/tests-poll.sh` & `LbNightlyTools-3.0.9/jenkins/periodic-tests/tests-poll.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/periodic-tests/tests.sh` & `LbNightlyTools-3.0.9/jenkins/periodic-tests/tests.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/periodic-tests/tests-getteststorun.sh` & `LbNightlyTools-3.0.9/jenkins/periodic-tests/tests-getteststorun.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/mock.sh` & `LbNightlyTools-3.0.9/jenkins/mock.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/utils.d/build_slot.sh` & `LbNightlyTools-3.0.9/jenkins/utils.d/build_slot.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/utils.d/set_common.sh` & `LbNightlyTools-3.0.9/jenkins/utils.d/set_common.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/utils.d/check_preconditions.sh` & `LbNightlyTools-3.0.9/jenkins/utils.d/check_preconditions.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/utils.d/checkout_slot.sh` & `LbNightlyTools-3.0.9/jenkins/utils.d/checkout_slot.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/utils.d/execute_preconditions.sh` & `LbNightlyTools-3.0.9/jenkins/utils.d/execute_preconditions.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/docker.sh` & `LbNightlyTools-3.0.9/jenkins/docker.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/jenkins/testMock.sh` & `LbNightlyTools-3.0.9/jenkins/testMock.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/periodic_tests/starter_schedule.xml` & `LbNightlyTools-3.0.9/testdata/periodic_tests/starter_schedule.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/periodic_tests/schedule.xml` & `LbNightlyTools-3.0.9/testdata/periodic_tests/schedule.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/periodic_tests/slotbuilds.json` & `LbNightlyTools-3.0.9/testdata/periodic_tests/slotbuilds.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/coverity/bin/cov-commit-defects` & `LbNightlyTools-3.0.9/testdata/coverity/bin/cov-commit-defects`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/coverity/bin/cov-analyze` & `LbNightlyTools-3.0.9/testdata/coverity/bin/cov-analyze`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/coverity/bin/cov-build` & `LbNightlyTools-3.0.9/testdata/coverity/bin/cov-build`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/tools/manifest.xml` & `LbNightlyTools-3.0.9/testdata/tools/manifest.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/tools/manifest_do0.xml` & `LbNightlyTools-3.0.9/testdata/tools/manifest_do0.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/tools/manifest_with_pkgs.xml` & `LbNightlyTools-3.0.9/testdata/tools/manifest_with_pkgs.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/artifacts/packs/src/TestProject.HEAD.testing-slot.src.zip` & `LbNightlyTools-3.0.9/testdata/artifacts/packs/src/TestProject.HEAD.testing-slot.src.zip`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/collect_deps/cmt/conf.json` & `LbNightlyTools-3.0.9/testdata/collect_deps/cmt/conf.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/collect_deps/cmake/conf.json` & `LbNightlyTools-3.0.9/testdata/collect_deps/cmake/conf.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/ci-test-hook-content.json` & `LbNightlyTools-3.0.9/testdata/ci-test-hook-content.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/rpm/PARAM_TMVAWeights.spec` & `LbNightlyTools-3.0.9/testdata/rpm/PARAM_TMVAWeights.spec`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/rpm/manifest.xml` & `LbNightlyTools-3.0.9/testdata/rpm/manifest.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/rpm/Brunel_v46r0.spec` & `LbNightlyTools-3.0.9/testdata/rpm/Brunel_v46r0.spec`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/rpm/datapkg-slot-config.json` & `LbNightlyTools-3.0.9/testdata/rpm/datapkg-slot-config.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/rpm/slot-configdo0.json` & `LbNightlyTools-3.0.9/testdata/rpm/slot-configdo0.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/rpm/LCG_68_externalsDict.json` & `LbNightlyTools-3.0.9/testdata/rpm/LCG_68_externalsDict.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/rpm/manifest_do0.xml` & `LbNightlyTools-3.0.9/testdata/rpm/manifest_do0.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/rpm/glimpse_Brunel_v46r0.spec` & `LbNightlyTools-3.0.9/testdata/rpm/glimpse_Brunel_v46r0.spec`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/rpm/Brunel_v46r0_x86_64-slc6-gcc48-opt.spec` & `LbNightlyTools-3.0.9/testdata/rpm/Brunel_v46r0_x86_64-slc6-gcc48-opt.spec`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/rpm/Gaudi_v27r0_x86_64-slc6-gcc49-do0.spec` & `LbNightlyTools-3.0.9/testdata/rpm/Gaudi_v27r0_x86_64-slc6-gcc49-do0.spec`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/rpm/slot-config.json` & `LbNightlyTools-3.0.9/testdata/rpm/slot-config.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/testdata/rpm/PARAM_TMVAWeights_rel5.spec` & `LbNightlyTools-3.0.9/testdata/rpm/PARAM_TMVAWeights_rel5.spec`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/CHANGELOG.md` & `LbNightlyTools-3.0.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/.gitlab-ci.yml` & `LbNightlyTools-3.0.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/pylint.rc` & `LbNightlyTools-3.0.9/docs/pylint.rc`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/examples/lbpr-example` & `LbNightlyTools-3.0.9/docs/examples/lbpr-example`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/operation/NightlyBuildsOperation.html` & `LbNightlyTools-3.0.9/docs/operation/NightlyBuildsOperation.html`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/operation/images/jenkins-jobs.dot` & `LbNightlyTools-3.0.9/docs/operation/images/jenkins-jobs.dot`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/operation/images/jenkins-jobs.dot.png` & `LbNightlyTools-3.0.9/docs/operation/images/jenkins-jobs.dot.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/operation/Makefile` & `LbNightlyTools-3.0.9/docs/operation/Makefile`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/operation/NightlyBuildsOperation.rst` & `LbNightlyTools-3.0.9/docs/operation/NightlyBuildsOperation.rst`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/Interactive builds of LHCb projects.ipynb` & `LbNightlyTools-3.0.9/docs/Interactive builds of LHCb projects.ipynb`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/jenkins-scripts.dot` & `LbNightlyTools-3.0.9/docs/jenkins-scripts.dot`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/jenkins-scripts.dot.png` & `LbNightlyTools-3.0.9/docs/jenkins-scripts.dot.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/design.tex` & `LbNightlyTools-3.0.9/docs/note/design.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/introduction.tex` & `LbNightlyTools-3.0.9/docs/note/introduction.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/cite.sty` & `LbNightlyTools-3.0.9/docs/note/cite.sty`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/appendix.tex` & `LbNightlyTools-3.0.9/docs/note/appendix.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/figs/lhcb-logo.pdf` & `LbNightlyTools-3.0.9/docs/note/figs/lhcb-logo.pdf`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/figs/old-summary.png` & `LbNightlyTools-3.0.9/docs/note/figs/old-summary.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/figs/cdash-3.png` & `LbNightlyTools-3.0.9/docs/note/figs/cdash-3.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/figs/cdash-1.png` & `LbNightlyTools-3.0.9/docs/note/figs/cdash-1.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/figs/jenkins-3.png` & `LbNightlyTools-3.0.9/docs/note/figs/jenkins-3.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/figs/cdash-4.png` & `LbNightlyTools-3.0.9/docs/note/figs/cdash-4.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/figs/jenkins-2.png` & `LbNightlyTools-3.0.9/docs/note/figs/jenkins-2.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/figs/jenkins-1.png` & `LbNightlyTools-3.0.9/docs/note/figs/jenkins-1.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/figs/cdash-2.png` & `LbNightlyTools-3.0.9/docs/note/figs/cdash-2.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/figs/lhcb-logo.eps` & `LbNightlyTools-3.0.9/docs/note/figs/lhcb-logo.eps`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/preamble.tex` & `LbNightlyTools-3.0.9/docs/note/preamble.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/LHCb-INT-2013-006.pdf` & `LbNightlyTools-3.0.9/docs/note/LHCb-INT-2013-006.pdf`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/conclusions.tex` & `LbNightlyTools-3.0.9/docs/note/conclusions.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/listsymbols` & `LbNightlyTools-3.0.9/docs/note/listsymbols`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/dashboard.tex` & `LbNightlyTools-3.0.9/docs/note/dashboard.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/bibliography.bib` & `LbNightlyTools-3.0.9/docs/note/bibliography.bib`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/lhcb-int-2013-006.kilepr` & `LbNightlyTools-3.0.9/docs/note/lhcb-int-2013-006.kilepr`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/requirements.tex` & `LbNightlyTools-3.0.9/docs/note/requirements.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/LHCb.bst` & `LbNightlyTools-3.0.9/docs/note/LHCb.bst`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/unsrturl.bst` & `LbNightlyTools-3.0.9/docs/note/unsrturl.bst`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/Makefile` & `LbNightlyTools-3.0.9/docs/note/Makefile`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/title-LHCb-ANA.tex` & `LbNightlyTools-3.0.9/docs/note/title-LHCb-ANA.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/main.tex` & `LbNightlyTools-3.0.9/docs/note/main.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/implementation.tex` & `LbNightlyTools-3.0.9/docs/note/implementation.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/note/mciteplus.sty` & `LbNightlyTools-3.0.9/docs/note/mciteplus.sty`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/configuration/Example.py` & `LbNightlyTools-3.0.9/docs/configuration/Example.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/docs/LHCbPR2.md` & `LbNightlyTools-3.0.9/docs/LHCbPR2.md`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/couchdb/merge_requests/views/mrs/map.js` & `LbNightlyTools-3.0.9/couchdb/merge_requests/views/mrs/map.js`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/couchdb/deployment/views/ready/map.js` & `LbNightlyTools-3.0.9/couchdb/deployment/views/ready/map.js`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/couchdb/frontend-stats/README.md` & `LbNightlyTools-3.0.9/couchdb/frontend-stats/README.md`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/couchdb/frontend-stats/views/byDate/map.js` & `LbNightlyTools-3.0.9/couchdb/frontend-stats/views/byDate/map.js`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/couchdb/auth/validate_doc_update.js` & `LbNightlyTools-3.0.9/couchdb/auth/validate_doc_update.js`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/couchdb/Push CouchDB Nightly Builds.launch` & `LbNightlyTools-3.0.9/couchdb/Push CouchDB Nightly Builds.launch`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/couchdb/webapp_testbench.py` & `LbNightlyTools-3.0.9/couchdb/webapp_testbench.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/couchdb/old_dashboard/rewrites.json` & `LbNightlyTools-3.0.9/couchdb/old_dashboard/rewrites.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/couchdb/README.md` & `LbNightlyTools-3.0.9/couchdb/README.md`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbPeriodicTools/TestSchedule.xsd` & `LbNightlyTools-3.0.9/python/LbPeriodicTools/TestSchedule.xsd`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbPeriodicTools/LbPeriodicStarter.py` & `LbNightlyTools-3.0.9/python/LbPeriodicTools/LbPeriodicStarter.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbPeriodicTools/LbPeriodicTest.py` & `LbNightlyTools-3.0.9/python/LbPeriodicTools/LbPeriodicTest.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbPeriodicTools/_entry_points.py` & `LbNightlyTools-3.0.9/python/LbPeriodicTools/_entry_points.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbPeriodicTools/LbPeriodicTestSchedule.py` & `LbNightlyTools-3.0.9/python/LbPeriodicTools/LbPeriodicTestSchedule.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbPeriodicTools/tests/TestStarter.py` & `LbNightlyTools-3.0.9/python/LbPeriodicTools/tests/TestStarter.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbPeriodicTools/tests/TestXMLParsing.py` & `LbNightlyTools-3.0.9/python/LbPeriodicTools/tests/TestXMLParsing.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbPeriodicTools/tests/TestLHCbPR.py` & `LbNightlyTools-3.0.9/python/LbPeriodicTools/tests/TestLHCbPR.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbTools/Manifest.py` & `LbNightlyTools-3.0.9/python/LbTools/Manifest.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbTools/tests/TestXMLParsing.py` & `LbNightlyTools-3.0.9/python/LbTools/tests/TestXMLParsing.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools.egg-info/PKG-INFO` & `LbNightlyTools-3.0.9/python/LbNightlyTools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: LbNightlyTools
-Version: 3.0.8
+Version: 3.0.9
 Summary: LHCb Nightly tools
 Home-page: https://gitlab.cern.ch/lhcb-core/LbNightlyTools
 Author: CERN - LHCb Core Software
 Author-email: lhcb-core-soft@cern.ch
 License: UNKNOWN
 Description: LbNightlyTools
         ===============
```

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools.egg-info/SOURCES.txt` & `LbNightlyTools-3.0.9/python/LbNightlyTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools.egg-info/entry_points.txt` & `LbNightlyTools-3.0.9/python/LbNightlyTools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbPR/LbPRJobManager.py` & `LbNightlyTools-3.0.9/python/LbPR/LbPRJobManager.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbPR/_entry_points.py` & `LbNightlyTools-3.0.9/python/LbPR/_entry_points.py`

 * *Files 3% similar despite different names*

```diff
@@ -250,23 +250,14 @@
 data_dict['app_version_datetime'] = '{app_version_datetime}'
 dash.update(doc_name, data_dict)
 END`
 
 # Set environment for throughput tests
 if [[ '{handlers}' == *"Throughput"* ]] ; then
     source /cvmfs/projects.cern.ch/intelsw/psxe/linux/19-all-setup.sh
-    if [ -d ../lhcb-benchmark-scripts ] ; then
-    (cd ../lhcb-benchmark-scripts
-        git fetch --all
-        git reset --hard origin/master
-    )
-    else
-    git clone --quiet ssh://git@gitlab.cern.ch:7999/lhcb-core/lhcb-benchmark-scripts.git ../lhcb-benchmark-scripts
-    fi
-    ln -sfv ../lhcb-benchmark-scripts/* .
 fi
 
 if [ -z "$LHCBPR_MOCK_OUTPUT_PATH" ]
 then
     {run_cmd} 2>&1 | tee run.log
 else
     OUTPUT_PATH="$LHCBPR_MOCK_OUTPUT_PATH"
```

### Comparing `LbNightlyTools-3.0.8/python/LbMsg/BuildMsg.py` & `LbNightlyTools-3.0.9/python/LbMsg/BuildMsg.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbMsg/Common.py` & `LbNightlyTools-3.0.9/python/LbMsg/Common.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbMsg/TestMsg.py` & `LbNightlyTools-3.0.9/python/LbMsg/TestMsg.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbRPMTools/LHCbExternalsSpecBuilder.py` & `LbNightlyTools-3.0.9/python/LbRPMTools/LHCbExternalsSpecBuilder.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbRPMTools/LHCbLbScriptsSpecBuilder.py` & `LbNightlyTools-3.0.9/python/LbRPMTools/LHCbLbScriptsSpecBuilder.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbRPMTools/LHCbRPMSpecBuilder.py` & `LbNightlyTools-3.0.9/python/LbRPMTools/LHCbRPMSpecBuilder.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbRPMTools/LHCbCompatSpecBuilder.py` & `LbNightlyTools-3.0.9/python/LbRPMTools/LHCbCompatSpecBuilder.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbRPMTools/LHCbGenericSpecBuilder.py` & `LbNightlyTools-3.0.9/python/LbRPMTools/LHCbGenericSpecBuilder.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbRPMTools/LHCbMetaSpecBuilder.py` & `LbNightlyTools-3.0.9/python/LbRPMTools/LHCbMetaSpecBuilder.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbRPMTools/PackageSlot.py` & `LbNightlyTools-3.0.9/python/LbRPMTools/PackageSlot.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbRPMTools/tests/TestSpec.py` & `LbNightlyTools-3.0.9/python/LbRPMTools/tests/TestSpec.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbRPMTools/tests/TestPackageSlot.py` & `LbNightlyTools-3.0.9/python/LbRPMTools/tests/TestPackageSlot.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbRPMTools/tests/TestExternalSpec.py` & `LbNightlyTools-3.0.9/python/LbRPMTools/tests/TestExternalSpec.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/ProcUtils.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/ProcUtils.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/Utils.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/Utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                     output[fd].append(data)
                     files[fd][1].write(data)
                 else:
                     # Ignore hang up or errors.
                     close_unregister_and_remove(fd)
         retcode = proc.wait()
 
-    return retcode, ''.join(out), ''.join(err)
+    return retcode, b''.join(out), b''.join(err)
 
 
 def log_call(*args, **kwargs):
     '''
     Wrapper for Popen to run a command and collect the output.
 
     The arguments are those of Popen, with the addition of
@@ -202,15 +202,15 @@
     err = []
 
     files = dict((x.fileno(), x) for x in (proc.stdout, proc.stderr) if x)
     output = {proc.stdout.fileno(): out}
     if proc.stderr:
         output[proc.stderr.fileno()] = err
     spilled_output = dict(
-        (x.fileno(), '') for x in (proc.stdout, proc.stderr) if x)
+        (x.fileno(), b'') for x in (proc.stdout, proc.stderr) if x)
 
     poller.register(proc.stdout, select_POLLIN_POLLPRI)
     if proc.stderr:
         poller.register(proc.stderr, select_POLLIN_POLLPRI)
 
     def close_unregister_and_remove(fd):
         poller.unregister(fd)
@@ -227,26 +227,30 @@
         for fd, mode in ready:
             if mode & select_POLLIN_POLLPRI:
                 data = os.read(fd, 4096)
                 if not data:
                     close_unregister_and_remove(fd)
                 output[fd].append(data)
                 data = spilled_output[fd] + data
-                spilled_output[fd] = ''
+                spilled_output[fd] = b''
                 for line in data.splitlines(True):
-                    if line.endswith('\n'):
-                        log(log_level, line.rstrip())
+                    if line.endswith(b'\n'):
+                        log(log_level, line.decode().rstrip())
                     else:
                         spilled_output[fd] += line
             else:
                 # Ignore hang up or errors.
                 close_unregister_and_remove(fd)
     retcode = proc.wait()
 
-    return {'retcode': retcode, 'stdout': ''.join(out), 'stderr': ''.join(err)}
+    return {
+        'retcode': retcode,
+        'stdout': b''.join(out),
+        'stderr': b''.join(err)
+    }
 
 
 def _retry_wrapper(func, check=None):
     '''
     Decorator to add retrying to functions.
     The optional predicate 'check' can be used to map the output of 'func' to
     success or failure (default: True -> success)
```

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/HTMLUtils.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/HTMLUtils.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/LbScriptsUtils.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/LbScriptsUtils.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/CheckSlotPreconditions.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/CheckSlotPreconditions.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/EnabledSlots.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/EnabledSlots.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/Test.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/Test.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 '''
 
 import os
 import shutil
 import json
 import codecs
 from datetime import datetime, timedelta
-from subprocess import call, Popen
+from subprocess import call
 
 from LbNightlyTools.Utils import chdir, ensureDirs
 from LbNightlyTools.Utils import cpuinfo as get_cpuinfo, write_json
 from LbNightlyTools.Utils import Dashboard, JobParams
 from LbNightlyTools.Scripts.Build import unpackArtifacts, wipeDir
 from LbPlatformUtils import requires
```

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/Index.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/Index.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/CollectBuildLogs.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/CollectBuildLogs.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/Install.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/Install.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 def _list_ssh(url):
     '''
     Implementation of listdir for SSH.
     '''
     host, path = url.split(':', 1)
     proc = Popen(['ssh', host, 'ls -a1 %r' % path], stdout=PIPE)
-    return proc.communicate()[0].splitlines()
+    return proc.communicate()[0].decode().splitlines()
 
 
 def _url_protocol(url):
     '''
     @return the protocol id of the given URL
     '''
     if re.match(r'https?://', url):
@@ -616,15 +616,15 @@
                     index_installed = True
             if os.path.exists(os.path.join(dest, 'slot.patch')):
                 self.log.warning('Applying patch file: %s' % os.path.join(
                     dest, 'slot.patch'))
                 command = ['patch', '-p1', '-f', '-i', 'slot.patch']
                 proc = Popen(command, cwd=dest, stdout=PIPE, stderr=STDOUT)
                 out, _ = proc.communicate()
-                self.log.debug('output of %s:\n%s', command, out)
+                self.log.debug('output of %s:\n%s', command, out.decode())
 
             if index_installed:
                 fixGlimpseIndexes(
                     f for f in findGlimpseFilenames(dest)
                     if f not in pre_existing_indexes)
 
             # if 'confSummary.py' was just installed and actually exists,
```

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/listzip.php` & `LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/listzip.php`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/Common.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/Common.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/Preconditions.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/Preconditions.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/Build.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/Build.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/extract.php` & `LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/extract.php`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/GitlabMR.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/GitlabMR.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/_entry_points.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/_entry_points.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/Release.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/Release.py`

 * *Files 1% similar despite different names*

```diff
@@ -467,14 +467,15 @@
          env.get('CMTPROJECTPATH', '')])
     proc = Popen(['cmt', 'show', 'projects'],
                  cwd=build_dir,
                  env=env,
                  stdout=PIPE,
                  stderr=PIPE)
     out, _err = proc.communicate()
+    out = out.decode()
 
     # no check because we must have a dependency on LCGCMT
     match = re.search(r'LCGCMT_([^ ]+)', out)
     if not match:
         logging.error(
             'problem with "cmt show projects":\n'
             '--- output ---\n%s\n--------------', out)
@@ -497,15 +498,15 @@
     if 'DBASE' in out or 'PARAM' in out:
         proc = Popen(['cmt', 'show', 'uses'],
                      cwd=container_dir,
                      env=env,
                      stdout=PIPE,
                      stderr=PIPE)
         out, _err = proc.communicate()
-        out = out.splitlines()
+        out = out.decode().splitlines()
         data_pkgs = [
             x.replace(' ', ',').split(',')[1:4:2] for x in out
             if re.search(r'DBASE|PARAM', x)
         ]
 
         def findVersion(pkg):
             v = (x.split()[3] for x in out
```

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/__init__.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/Scripts/Checkout.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/Scripts/Checkout.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/ArtifactsServer.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/ArtifactsServer.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/BuildLogScanner.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/BuildLogScanner.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/CheckoutMethods.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/CheckoutMethods.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,15 @@
         self.path = path
 
         if url and 'gitlab.cern.ch' in url:
             # fetch merge request branches (if it's a gitlab repository)
             proc = Popen(['git', 'config', '--get-all', 'remote.origin.fetch'],
                          cwd=self.path,
                          stdout=PIPE)
-            if 'origin/merge-requests' not in proc.communicate()[0]:
+            if 'origin/merge-requests' not in proc.communicate()[0].decode():
                 # it must be configured
                 __log__.getChild('git').debug(
                     'getting merge-requests branches')
                 fetch = ('+refs/merge-requests/*/head:'
                          'refs/remotes/origin/merge-requests/*')
                 log_call(
                     ['git', 'config', '--add', 'remote.origin.fetch', fetch],
@@ -236,34 +236,35 @@
 
     def remotes(self):
         '''
         Return the remote repositories defined for fetch, as a dictionary
         name -> url.
         '''
         proc = Popen(['git', 'remote', '-v'], cwd=self.path, stdout=PIPE)
-        lines = proc.communicate()[0].splitlines()
+        lines = proc.communicate()[0].decode().splitlines()
         pattern = re.compile(r'(\S+)\s+(\S+)\s+\(fetch\)$')
         return dict(
             m.groups() for m in filter(None, map(pattern.match, lines)))
 
     def branches(self):
         '''
         Return a list of all branches (local and remote) known by the
         repository.
         '''
         proc = Popen(['git', 'branch', '-a'], cwd=self.path, stdout=PIPE)
         return set(branch[2:].rstrip()
-                   for branch in proc.communicate()[0].splitlines())
+                   for branch in proc.communicate()[0].decode().splitlines())
 
     def tags(self):
         '''
         Return a list of all tags known by the repository.
         '''
         proc = Popen(['git', 'tag'], cwd=self.path, stdout=PIPE)
-        return set(tag.strip() for tag in proc.communicate()[0].splitlines())
+        return set(
+            tag.strip() for tag in proc.communicate()[0].decode().splitlines())
 
     def add_remote(self, name, url, retry=True):
         '''
         Add a new remote repository definition.
         '''
         __log__.getChild('git').debug('adding remote %s as %s', url, name)
         log_call(['git', 'remote', 'add', name, url], cwd=self.path)
@@ -332,18 +333,18 @@
                     cwd=self.path,
                     retry=3,
                     retry_sleep=30)
             except RuntimeError as err:
                 __log__.warning(str(err))
             return [
                 os.path.join(self.path,
-                             l.split()[1])
-                for l in Popen(['git', 'submodule', 'status', '--recursive'],
-                               cwd=self.path,
-                               stdout=PIPE).communicate()[0].splitlines()
+                             l.split()[1]) for l in
+                Popen(['git', 'submodule', 'status', '--recursive'],
+                      cwd=self.path,
+                      stdout=PIPE).communicate()[0].decode().splitlines()
             ]
         return []
 
     def merge(self, commit, extra_args=None):
         '''
         Merge the specified commit into the current branch.
         '''
@@ -401,15 +402,16 @@
 
     def rev_parse(self, *args):
         '''
         Simple wrapper around "git rev-parse".
         '''
         cmd = ['git', 'rev-parse']
         cmd.extend(args)
-        return Popen(cmd, cwd=self.path, stdout=PIPE).communicate()[0].strip()
+        return Popen(
+            cmd, cwd=self.path, stdout=PIPE).communicate()[0].decode().strip()
 
     def show_branch(self, *args):
         '''
         Simple wrapper around "git show-branch".
         '''
         cmd = ['git', 'show-branch']
         cmd.extend(args)
@@ -523,15 +525,15 @@
     def prepare(self):
         '''
         Fetch merge request special branches from GitLab, if needed.
         '''
         proc = Popen(['git', 'config', '--get-all', 'remote.origin.fetch'],
                      cwd=self.path,
                      stdout=PIPE)
-        if 'origin/merge-requests' not in proc.communicate()[0]:
+        if 'origin/merge-requests' not in proc.communicate()[0].decode():
             # it must be configured
             __log__.getChild('git').debug('getting merge-requests branches')
             fetch = ('+refs/merge-requests/*/head:'
                      'refs/remotes/origin/merge-requests/*')
             log_call(['git', 'config', '--add', 'remote.origin.fetch', fetch],
                      cwd=self.path)
             retry_log_call(['git', 'fetch', '-q', 'origin'],
@@ -814,20 +816,20 @@
                     '--format=%(refname),'
                 ],
                              cwd=repo.path,
                              stdout=PIPE)
                 # (test requested commit first)
                 log.debug('looking for an equivalent commit')
                 for ref in eval('[{!r},'.format(commit_requested) +
-                                proc.communicate()[0] + ']'):
+                                proc.communicate()[0].decode() + ']'):
                     if repo.rev_parse(ref + ':') == tree:
                         proc = Popen(['git', 'rev-list', '--max-count=1', ref],
                                      cwd=repo.path,
                                      stdout=PIPE)
-                        commit = proc.communicate()[0].strip()
+                        commit = proc.communicate()[0].decode().strip()
                         log.debug('reusing commit %s (%s)', commit, ref)
                         break  # we found a commit with the same content
                 else:  # we could not find it, so we stick to HEAD
                     log.debug('none found')
 
             repo.tag(tag_name(), commit=commit, force=True)
             repo.push_tag(tag_name(), remote='lhcb-nightlies', force=True)
```

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/Configuration.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/Configuration.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/MergeRequestBuilds.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/MergeRequestBuilds.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/BuildMethods.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/BuildMethods.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/GitlabUtils.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/GitlabUtils.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/__init__.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/__init__.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_config_pickle.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_config_pickle.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_jobconfig.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_jobconfig.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_gitlab_mr_script.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_gitlab_mr_script.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_indexer.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_indexer.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_config_load.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_config_load.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_retry.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_checkout_script.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_checkout_script.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_coverity_support.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_coverity_support.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_build_script.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_build_script.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_release_poll.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_release_poll.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_install.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_copytree.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_copytree.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/tests/__main__.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_build.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/tests/utils.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/tests/utils.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_precond.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_precond.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_enabled_slots_script.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_enabled_slots_script.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_utils.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_checkout.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_checkout.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_rel_gen_script.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_rel_gen_script.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_configuration.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/tests/test_pack.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/tests/test_pack.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/python/LbNightlyTools/tests/__init__.py` & `LbNightlyTools-3.0.9/python/LbNightlyTools/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-3.0.8/setup.py` & `LbNightlyTools-3.0.9/setup.py`

 * *Files identical despite different names*

