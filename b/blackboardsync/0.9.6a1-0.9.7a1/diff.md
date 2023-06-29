# Comparing `tmp/blackboardsync-0.9.6a1.tar.gz` & `tmp/blackboardsync-0.9.7a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackboardsync-0.9.6a1.tar", last modified: Thu Jun 29 14:28:20 2023, max compression
+gzip compressed data, was "blackboardsync-0.9.7a1.tar", last modified: Thu Jun 29 23:39:35 2023, max compression
```

## Comparing `blackboardsync-0.9.6a1.tar` & `blackboardsync-0.9.7a1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.570581 blackboardsync-0.9.6a1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.562580 blackboardsync-0.9.6a1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.562580 blackboardsync-0.9.6a1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/.github/ISSUE_TEMPLATE/unisupport.yml
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.562580 blackboardsync-0.9.6a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-29 14:28:20.570581 blackboardsync-0.9.6a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)   109550 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/UNIVERSITIES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.566581 blackboardsync-0.9.6a1/blackboard_sync/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.566581 blackboardsync-0.9.6a1/blackboard_sync/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/assets/alert.png
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/assets/alert.svg
--rw-r--r--   0 runner    (1001) docker     (123)   110234 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/assets/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/assets/watermark.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.566581 blackboardsync-0.9.6a1/blackboard_sync/blackboard/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/blackboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29706 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/blackboard/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/blackboard/blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/institutions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.566581 blackboardsync-0.9.6a1/blackboard_sync/qt/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/qt/LoginWebView.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/qt/PersistenceWarning.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/qt/SettingsWindow.ui
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/qt/SetupWizard.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/qt/UniNotSupportedDialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/qt/qt_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    11124 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/sync_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    13787 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/universities.json
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.566581 blackboardsync-0.9.6a1/blackboardsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-29 14:28:20.000000 blackboardsync-0.9.6a1/blackboardsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-29 14:28:20.000000 blackboardsync-0.9.6a1/blackboardsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 14:28:20.000000 blackboardsync-0.9.6a1/blackboardsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-29 14:28:20.000000 blackboardsync-0.9.6a1/blackboardsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 14:28:20.000000 blackboardsync-0.9.6a1/blackboardsync.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.570581 blackboardsync-0.9.6a1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.570581 blackboardsync-0.9.6a1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.570581 blackboardsync-0.9.6a1/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/docs/dev/bb_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/docs/dev/qt_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/docs/dev/sync_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.570581 blackboardsync-0.9.6a1/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/packaging/pkg_macos.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/packaging/pkg_win.nsi
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/packaging/pyinst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 14:28:20.570581 blackboardsync-0.9.6a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.570581 blackboardsync-0.9.6a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/tests/test_blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/tests/test_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/tests/test_sync_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:39:35.667551 blackboardsync-0.9.7a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:39:35.663551 blackboardsync-0.9.7a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:39:35.663551 blackboardsync-0.9.7a1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/.github/ISSUE_TEMPLATE/unisupport.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:39:35.663551 blackboardsync-0.9.7a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-29 23:39:35.667551 blackboardsync-0.9.7a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)   109550 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/UNIVERSITIES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:39:35.663551 blackboardsync-0.9.7a1/blackboard_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:39:35.663551 blackboardsync-0.9.7a1/blackboard_sync/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/assets/alert.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/assets/alert.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   110234 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/assets/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/assets/watermark.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:39:35.663551 blackboardsync-0.9.7a1/blackboard_sync/blackboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/blackboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29706 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/blackboard/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/blackboard/blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/institutions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:39:35.663551 blackboardsync-0.9.7a1/blackboard_sync/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/qt/LoginWebView.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/qt/PersistenceWarning.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/qt/SettingsWindow.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/qt/SetupWizard.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/qt/UniNotSupportedDialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/qt/qt_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/sync_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13787 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/universities.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/blackboard_sync/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:39:35.667551 blackboardsync-0.9.7a1/blackboardsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-29 23:39:35.000000 blackboardsync-0.9.7a1/blackboardsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-29 23:39:35.000000 blackboardsync-0.9.7a1/blackboardsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 23:39:35.000000 blackboardsync-0.9.7a1/blackboardsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-29 23:39:35.000000 blackboardsync-0.9.7a1/blackboardsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 23:39:35.000000 blackboardsync-0.9.7a1/blackboardsync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:39:35.667551 blackboardsync-0.9.7a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:39:35.667551 blackboardsync-0.9.7a1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:39:35.667551 blackboardsync-0.9.7a1/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/docs/dev/bb_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/docs/dev/qt_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/docs/dev/sync_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:39:35.667551 blackboardsync-0.9.7a1/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/packaging/pkg_macos.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/packaging/pkg_win.nsi
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/packaging/pyinst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 23:39:35.667551 blackboardsync-0.9.7a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:39:35.667551 blackboardsync-0.9.7a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/tests/test_blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/tests/test_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-29 23:38:50.000000 blackboardsync-0.9.7a1/tests/test_sync_config.py
```

### Comparing `blackboardsync-0.9.6a1/.github/ISSUE_TEMPLATE/unisupport.yml` & `blackboardsync-0.9.7a1/.github/ISSUE_TEMPLATE/unisupport.yml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/.github/workflows/build.yml` & `blackboardsync-0.9.7a1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/.gitignore` & `blackboardsync-0.9.7a1/.gitignore`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/CHANGELOG.md` & `blackboardsync-0.9.7a1/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.9.7] - 2023-06-30
+
+### Fixed
+- Issues with redownloading all files after changing download location
+
+### Changed
+- WebDav downloads are now also multithreaded
+
 ## [0.9.6] - 2023-06-29
 
 ### Changed
 - Changing download since to an earlier year will cause a redownload
 - PyInstaller has been upgraded to 5.13, and other dependencies have also been upgraded
 
 ### Fixed
```

### Comparing `blackboardsync-0.9.6a1/CONTRIBUTING.md` & `blackboardsync-0.9.7a1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/LICENSE` & `blackboardsync-0.9.7a1/LICENSE`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/PKG-INFO` & `blackboardsync-0.9.7a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.9.6a1
+Version: 0.9.7a1
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `blackboardsync-0.9.6a1/Pipfile` & `blackboardsync-0.9.7a1/Pipfile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/Pipfile.lock` & `blackboardsync-0.9.7a1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/README.md` & `blackboardsync-0.9.7a1/README.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/UNIVERSITIES.md` & `blackboardsync-0.9.7a1/UNIVERSITIES.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/__about__.py` & `blackboardsync-0.9.7a1/blackboard_sync/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,14 @@
     "__copyright__",
 ]
 
 __title__ = "BlackboardSync"
 __summary__ = "Automatic Syncing Of Your Blackboard Content"
 __uri__ = "https://github.com/jacobszpz/BlackboardSync"
 
-__version__ = "0.9.6-alpha.1"
+__version__ = "0.9.7-alpha.1"
 
 __author__ = "Jacob Sánchez"
 __email__ = "jacobszpz@protonmail.com"
 
 __license__ = "GNU General Public License v2"
 __copyright__ = f"2023, {__author__}"
```

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/__init__.py` & `blackboardsync-0.9.7a1/blackboard_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/__main__.py` & `blackboardsync-0.9.7a1/blackboard_sync/__main__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/assets/alert.png` & `blackboardsync-0.9.7a1/blackboard_sync/assets/alert.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/assets/alert.svg` & `blackboardsync-0.9.7a1/blackboard_sync/assets/alert.svg`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/assets/logo.ico` & `blackboardsync-0.9.7a1/blackboard_sync/assets/logo.ico`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/assets/logo.png` & `blackboardsync-0.9.7a1/blackboard_sync/assets/logo.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/assets/watermark.png` & `blackboardsync-0.9.7a1/blackboard_sync/assets/watermark.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/blackboard/__init__.py` & `blackboardsync-0.9.7a1/blackboard_sync/blackboard/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/blackboard/api.py` & `blackboardsync-0.9.7a1/blackboard_sync/blackboard/api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/blackboard/blackboard.py` & `blackboardsync-0.9.7a1/blackboard_sync/blackboard/blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/config.py` & `blackboardsync-0.9.7a1/blackboard_sync/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,16 +82,19 @@
 
     @property
     def last_sync_time(self) -> Optional[datetime]:
         return self._sync.getdate('last_sync_time')
 
     @last_sync_time.setter
     @Config.persist
-    def last_sync_time(self, last: datetime) -> None:
-        self._sync['last_sync_time'] = last.isoformat()
+    def last_sync_time(self, last: Optional[datetime]) -> None:
+        if last is None:
+            self.remove_option('Sync', 'last_sync_time')
+        else:
+            self._sync['last_sync_time'] = last.isoformat()
 
     @property
     def download_location(self) -> Optional[Path]:
         # Default download location
         default = Path(Path.home(), 'Downloads', 'BlackboardSync')
         return self._sync.getpath('download_location') or default
```

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/download.py` & `blackboardsync-0.9.7a1/blackboard_sync/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,16 +154,22 @@
                     if child.contentHandler is not None:
                         self._handle_file(child, file_path, course_id, depth + 1)
             except ValueError:
                 pass
 
         # Omit file if it hasn't been modified since last sync
         elif res in (BBResourceType.file, BBResourceType.document) and has_changed:
-            attachments = self._sess.fetch_file_attachments(course_id=course_id,
-                                                            content_id=content.id)
+            attachments = []
+
+            try:
+                attachments = self._sess.fetch_file_attachments(course_id=course_id,
+                                                                content_id=content.id)
+
+            except RequestException:
+                self.logger.warn(f"Error while getting attachments for {course_id}")
 
             if len(attachments) > 1:
                 file_path.mkdir(exist_ok=True, parents=True)
                 body_path = file_path
 
             for attachment in attachments:
                 download_path = Path(body_path / attachment.fileName)
@@ -191,15 +197,15 @@
 
             # Parse content.body for more attachments
             parser = ContentParser(content.body, self._sess.base_url)
 
             for body_link in parser.links:
                 safe_title = sanitize_filename(body_link.text, replacement_text='_')
                 download_path = Path(file_path / safe_title)
-                self._download_webdav_file(body_link.href, download_path)
+                self.executor.submit(self._download_webdav_file, body_link.href, download_path)
 
             with Path(file_path, f"{content.title_path_safe}.html").open('w') as html_content:
                 html_content.write(parser.body)
 
     def download(self) -> Optional[datetime]:
         """Retrieve the user's courses, and start download of all contents
 
@@ -244,15 +250,15 @@
 
                 for content in course_contents:
 
                     if self.cancelled:
                         break
 
                     self._handle_file(content, course_path, course.id, 1)
-        self.executor.shutdown(wait=True, cancel_futures=True)
+        self.executor.shutdown(wait=True, cancel_futures=self.cancelled)
 
         if self.cancelled:
             return None
         return start_time
 
     def cancel(self) -> None:
         """Cancel the download job."""
```

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/institutions.py` & `blackboardsync-0.9.7a1/blackboard_sync/institutions.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/qt/LoginWebView.ui` & `blackboardsync-0.9.7a1/blackboard_sync/qt/LoginWebView.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/qt/PersistenceWarning.ui` & `blackboardsync-0.9.7a1/blackboard_sync/qt/PersistenceWarning.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/qt/SettingsWindow.ui` & `blackboardsync-0.9.7a1/blackboard_sync/qt/SettingsWindow.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/qt/SetupWizard.ui` & `blackboardsync-0.9.7a1/blackboard_sync/qt/SetupWizard.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/qt/UniNotSupportedDialog.ui` & `blackboardsync-0.9.7a1/blackboard_sync/qt/UniNotSupportedDialog.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/qt/__init__.py` & `blackboardsync-0.9.7a1/blackboard_sync/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/qt/qt_elements.py` & `blackboardsync-0.9.7a1/blackboard_sync/qt/qt_elements.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/sync.py` & `blackboardsync-0.9.7a1/blackboard_sync/sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,20 +100,21 @@
             self._update_next_sync()
 
     def setup(self, university_index: int, download_location: Path,
               min_year: Optional[int] = None) -> None:
         """Setup the university information."""
         self.university_index = university_index
         self._config.download_location = download_location
-        self._config.min_year = min_year
 
         # If min_year has decreased, redownload
         if (self._config.min_year or 0) > (min_year or 0):
             self.last_sync_time = None
 
+        self._config.min_year = min_year
+
     def auth(self, cookie_jar: RequestsCookieJar) -> bool:
         """Create a new Blackboard session with the given credentials.
 
         Will start syncing automatically if login successful.
 
         :param bool persistence: If true, login will be saved in the OS designated keyring.
         """
@@ -243,16 +244,17 @@
     def last_sync_time(self, last_time: Optional[datetime]):
         """Updates the last sync time recorded."""
         self._config.last_sync_time = last_time
         self._update_next_sync()
 
     def _update_next_sync(self) -> None:
         """Store a calculated datetime when next sync should take place."""
-        self._next_sync = (self._config.last_sync_time +
-                           timedelta(seconds=self._sync_interval))
+        if self.last_sync_time is not None:
+            self._next_sync = (self._config.last_sync_time +
+                               timedelta(seconds=self._sync_interval))
 
     @property
     def next_sync(self) -> datetime:
         """Time when last sync will be outdated."""
         return self._next_sync
 
     @property
```

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/sync_controller.py` & `blackboardsync-0.9.7a1/blackboard_sync/sync_controller.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/universities.json` & `blackboardsync-0.9.7a1/blackboard_sync/universities.json`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/updates.py` & `blackboardsync-0.9.7a1/blackboard_sync/updates.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/blackboard_sync/webdav.py` & `blackboardsync-0.9.7a1/blackboard_sync/webdav.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/blackboardsync.egg-info/PKG-INFO` & `blackboardsync-0.9.7a1/blackboardsync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.9.6a1
+Version: 0.9.7a1
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `blackboardsync-0.9.6a1/blackboardsync.egg-info/SOURCES.txt` & `blackboardsync-0.9.7a1/blackboardsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/docs/Makefile` & `blackboardsync-0.9.7a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/docs/conf.py` & `blackboardsync-0.9.7a1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/docs/index.rst` & `blackboardsync-0.9.7a1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/docs/make.bat` & `blackboardsync-0.9.7a1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/main.py` & `blackboardsync-0.9.7a1/main.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/packaging/pkg_macos.sh` & `blackboardsync-0.9.7a1/packaging/pkg_macos.sh`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/packaging/pkg_win.nsi` & `blackboardsync-0.9.7a1/packaging/pkg_win.nsi`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/packaging/pyinst.py` & `blackboardsync-0.9.7a1/packaging/pyinst.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/pyproject.toml` & `blackboardsync-0.9.7a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/tests/strategies.py` & `blackboardsync-0.9.7a1/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/tests/test_api.py` & `blackboardsync-0.9.7a1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/tests/test_blackboard.py` & `blackboardsync-0.9.7a1/tests/test_blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/tests/test_download.py` & `blackboardsync-0.9.7a1/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/tests/test_qt.py` & `blackboardsync-0.9.7a1/tests/test_qt.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.6a1/tests/test_sync_config.py` & `blackboardsync-0.9.7a1/tests/test_sync_config.py`

 * *Files identical despite different names*

