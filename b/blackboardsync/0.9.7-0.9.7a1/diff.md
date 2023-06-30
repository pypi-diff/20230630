# Comparing `tmp/blackboardsync-0.9.7.tar.gz` & `tmp/blackboardsync-0.9.7a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackboardsync-0.9.7.tar", last modified: Fri Jun 30 13:59:52 2023, max compression
+gzip compressed data, was "blackboardsync-0.9.7a1.tar", last modified: Thu Jun 29 23:39:35 2023, max compression
```

## Comparing `blackboardsync-0.9.7.tar` & `blackboardsync-0.9.7a1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:59:52.209743 blackboardsync-0.9.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:59:52.205743 blackboardsync-0.9.7/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:59:52.205743 blackboardsync-0.9.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/.github/ISSUE_TEMPLATE/unisupport.yml
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:59:52.205743 blackboardsync-0.9.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-06-30 13:59:52.209743 blackboardsync-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)   109529 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/UNIVERSITIES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:59:52.205743 blackboardsync-0.9.7/blackboard_sync/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:59:52.205743 blackboardsync-0.9.7/blackboard_sync/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/assets/alert.png
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/assets/alert.svg
--rw-r--r--   0 runner    (1001) docker     (123)   110234 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/assets/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/assets/watermark.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:59:52.205743 blackboardsync-0.9.7/blackboard_sync/blackboard/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/blackboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29706 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/blackboard/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/blackboard/blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/institutions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:59:52.205743 blackboardsync-0.9.7/blackboard_sync/qt/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/qt/LoginWebView.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/qt/PersistenceWarning.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/qt/SettingsWindow.ui
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/qt/SetupWizard.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/qt/UniNotSupportedDialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/qt/qt_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/sync_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    13787 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/universities.json
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/blackboard_sync/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:59:52.209743 blackboardsync-0.9.7/blackboardsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-06-30 13:59:52.000000 blackboardsync-0.9.7/blackboardsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-30 13:59:52.000000 blackboardsync-0.9.7/blackboardsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:59:52.000000 blackboardsync-0.9.7/blackboardsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-30 13:59:52.000000 blackboardsync-0.9.7/blackboardsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 13:59:52.000000 blackboardsync-0.9.7/blackboardsync.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:59:52.209743 blackboardsync-0.9.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:59:52.209743 blackboardsync-0.9.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:59:52.209743 blackboardsync-0.9.7/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/docs/dev/bb_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/docs/dev/qt_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/docs/dev/sync_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:59:52.209743 blackboardsync-0.9.7/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/packaging/pkg_macos.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/packaging/pkg_win.nsi
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/packaging/pyinst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 13:59:52.209743 blackboardsync-0.9.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:59:52.209743 blackboardsync-0.9.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/tests/test_blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/tests/test_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-30 13:59:10.000000 blackboardsync-0.9.7/tests/test_sync_config.py
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

### Comparing `blackboardsync-0.9.7/.github/ISSUE_TEMPLATE/unisupport.yml` & `blackboardsync-0.9.7a1/.github/ISSUE_TEMPLATE/unisupport.yml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/.github/workflows/build.yml` & `blackboardsync-0.9.7a1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/.gitignore` & `blackboardsync-0.9.7a1/.gitignore`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/CHANGELOG.md` & `blackboardsync-0.9.7a1/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 ## [Unreleased]
 
 ## [0.9.7] - 2023-06-30
 
 ### Fixed
 - Issues with redownloading all files after changing download location
-- Potential issue where remaining downloads would be cancelled at the end of sync
 
 ### Changed
 - WebDav downloads are now also multithreaded
 
 ## [0.9.6] - 2023-06-29
 
 ### Changed
```

### Comparing `blackboardsync-0.9.7/CONTRIBUTING.md` & `blackboardsync-0.9.7a1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/LICENSE` & `blackboardsync-0.9.7a1/LICENSE`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/PKG-INFO` & `blackboardsync-0.9.7a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.9.7
+Version: 0.9.7a1
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `blackboardsync-0.9.7/Pipfile` & `blackboardsync-0.9.7a1/Pipfile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/Pipfile.lock` & `blackboardsync-0.9.7a1/Pipfile.lock`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998453548085901%*

 * *Differences: {"'default'": '{\'charset-normalizer\': {\'markers\': "python_full_version >= \'3.7.0\'"}}',*

 * * "'develop'": '{\'charset-normalizer\': {\'markers\': "python_full_version >= \'3.7.0\'"}, '*

 * *              "'python-lsp-server': {'hashes': "*

 * *              "['sha256:a31b0525be6ec831c7d2b476b744e5aa5074633e1d1b77ee97f332cde15983ea', "*

 * *              "'sha256:f4ae64834da1d4312067a8ee05a76c7652167c3c90d1cef44022366d695c4c0e'], "*

 * *              '\'version\': \'==1.7.3\'}, \'rich\': {\'markers\': "python_full_version >= ' […]*

```diff
@@ -114,15 +114,15 @@
                 "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
                 "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
                 "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
                 "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
                 "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
                 "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "markers": "python_version >= '3.7'",
+            "markers": "python_full_version >= '3.7.0'",
             "version": "==3.1.0"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
@@ -639,15 +639,15 @@
                 "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
                 "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
                 "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
                 "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
                 "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
                 "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "markers": "python_version >= '3.7'",
+            "markers": "python_full_version >= '3.7.0'",
             "version": "==3.1.0"
         },
         "click": {
             "hashes": [
                 "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
                 "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
@@ -1296,19 +1296,19 @@
             "version": "==1.0.0"
         },
         "python-lsp-server": {
             "extras": [
                 "all"
             ],
             "hashes": [
-                "sha256:c84254485a4d9431b24ecefd59741d21c00165611bcf6037bd7d54d0ed06a197",
-                "sha256:f8053f7aefcb60af4e91f3fab1a093b15ba0c4688ba67e6ab69e7b73e997b2cb"
+                "sha256:a31b0525be6ec831c7d2b476b744e5aa5074633e1d1b77ee97f332cde15983ea",
+                "sha256:f4ae64834da1d4312067a8ee05a76c7652167c3c90d1cef44022366d695c4c0e"
             ],
             "index": "pypi",
-            "version": "==1.7.4"
+            "version": "==1.7.3"
         },
         "pytoolconfig": {
             "extras": [
                 "global"
             ],
             "hashes": [
                 "sha256:239ba9d3e537b91d0243275a497700ea39a5e259ddb80421c366e3b288bf30fe",
@@ -1366,23 +1366,23 @@
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
                 "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec",
                 "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"
             ],
-            "markers": "python_version >= '3.7'",
+            "markers": "python_full_version >= '3.7.0'",
             "version": "==13.4.2"
         },
         "rope": {
             "hashes": [
-                "sha256:2ed32d72cd2c4395bb1d569e38fd4f15d6080cfadd61b6e5c565fd39e3f677aa",
-                "sha256:f48d708132c0e062b411308732ca13933b976486b4b53d1e804f94ed08d69503"
+                "sha256:0767424ed40ce237dcf1c1f5088054fef960e5b19f4a0850783a259a3600d7bd",
+                "sha256:3de1d1f1cf2412540c6a150067fe25298175e7c2b72455b6ca8395f61678da82"
             ],
-            "version": "==1.9.0"
+            "version": "==1.8.0"
         },
         "secretstorage": {
             "hashes": [
                 "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
                 "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
             ],
             "markers": "sys_platform == 'linux'",
```

### Comparing `blackboardsync-0.9.7/README.md` & `blackboardsync-0.9.7a1/README.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/UNIVERSITIES.md` & `blackboardsync-0.9.7a1/UNIVERSITIES.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/__about__.py` & `blackboardsync-0.9.7a1/blackboard_sync/__about__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,14 @@
     "__copyright__",
 ]
 
 __title__ = "BlackboardSync"
 __summary__ = "Automatic Syncing Of Your Blackboard Content"
 __uri__ = "https://github.com/jacobszpz/BlackboardSync"
 
-__version__ = "0.9.7"
+__version__ = "0.9.7-alpha.1"
 
 __author__ = "Jacob Sánchez"
 __email__ = "jacobszpz@protonmail.com"
 
 __license__ = "GNU General Public License v2"
 __copyright__ = f"2023, {__author__}"
```

### Comparing `blackboardsync-0.9.7/blackboard_sync/__init__.py` & `blackboardsync-0.9.7a1/blackboard_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/__main__.py` & `blackboardsync-0.9.7a1/blackboard_sync/__main__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/assets/alert.png` & `blackboardsync-0.9.7a1/blackboard_sync/assets/alert.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/assets/alert.svg` & `blackboardsync-0.9.7a1/blackboard_sync/assets/alert.svg`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/assets/logo.ico` & `blackboardsync-0.9.7a1/blackboard_sync/assets/logo.ico`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/assets/logo.png` & `blackboardsync-0.9.7a1/blackboard_sync/assets/logo.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/assets/watermark.png` & `blackboardsync-0.9.7a1/blackboard_sync/assets/watermark.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/blackboard/__init__.py` & `blackboardsync-0.9.7a1/blackboard_sync/blackboard/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/blackboard/api.py` & `blackboardsync-0.9.7a1/blackboard_sync/blackboard/api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/blackboard/blackboard.py` & `blackboardsync-0.9.7a1/blackboard_sync/blackboard/blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/config.py` & `blackboardsync-0.9.7a1/blackboard_sync/config.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/download.py` & `blackboardsync-0.9.7a1/blackboard_sync/download.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/institutions.py` & `blackboardsync-0.9.7a1/blackboard_sync/institutions.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/qt/LoginWebView.ui` & `blackboardsync-0.9.7a1/blackboard_sync/qt/LoginWebView.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/qt/PersistenceWarning.ui` & `blackboardsync-0.9.7a1/blackboard_sync/qt/PersistenceWarning.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/qt/SettingsWindow.ui` & `blackboardsync-0.9.7a1/blackboard_sync/qt/SettingsWindow.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/qt/SetupWizard.ui` & `blackboardsync-0.9.7a1/blackboard_sync/qt/SetupWizard.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/qt/UniNotSupportedDialog.ui` & `blackboardsync-0.9.7a1/blackboard_sync/qt/UniNotSupportedDialog.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/qt/__init__.py` & `blackboardsync-0.9.7a1/blackboard_sync/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/qt/qt_elements.py` & `blackboardsync-0.9.7a1/blackboard_sync/qt/qt_elements.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/sync.py` & `blackboardsync-0.9.7a1/blackboard_sync/sync.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/sync_controller.py` & `blackboardsync-0.9.7a1/blackboard_sync/sync_controller.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/universities.json` & `blackboardsync-0.9.7a1/blackboard_sync/universities.json`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/updates.py` & `blackboardsync-0.9.7a1/blackboard_sync/updates.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboard_sync/webdav.py` & `blackboardsync-0.9.7a1/blackboard_sync/webdav.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/blackboardsync.egg-info/PKG-INFO` & `blackboardsync-0.9.7a1/blackboardsync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.9.7
+Version: 0.9.7a1
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `blackboardsync-0.9.7/blackboardsync.egg-info/SOURCES.txt` & `blackboardsync-0.9.7a1/blackboardsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/docs/Makefile` & `blackboardsync-0.9.7a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/docs/conf.py` & `blackboardsync-0.9.7a1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/docs/index.rst` & `blackboardsync-0.9.7a1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/docs/make.bat` & `blackboardsync-0.9.7a1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/main.py` & `blackboardsync-0.9.7a1/main.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/packaging/pkg_macos.sh` & `blackboardsync-0.9.7a1/packaging/pkg_macos.sh`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/packaging/pkg_win.nsi` & `blackboardsync-0.9.7a1/packaging/pkg_win.nsi`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/packaging/pyinst.py` & `blackboardsync-0.9.7a1/packaging/pyinst.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/pyproject.toml` & `blackboardsync-0.9.7a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/tests/strategies.py` & `blackboardsync-0.9.7a1/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/tests/test_api.py` & `blackboardsync-0.9.7a1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/tests/test_blackboard.py` & `blackboardsync-0.9.7a1/tests/test_blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/tests/test_download.py` & `blackboardsync-0.9.7a1/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/tests/test_qt.py` & `blackboardsync-0.9.7a1/tests/test_qt.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.7/tests/test_sync_config.py` & `blackboardsync-0.9.7a1/tests/test_sync_config.py`

 * *Files identical despite different names*

