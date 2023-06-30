# Comparing `tmp/umirobot-22.4.6.tar.gz` & `tmp/umirobot-22.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umirobot-22.4.6.tar", last modified: Thu Jun 23 01:51:44 2022, max compression
+gzip compressed data, was "umirobot-22.4.9.tar", last modified: Thu Jun 23 08:01:48 2022, max compression
```

## Comparing `umirobot-22.4.6.tar` & `umirobot-22.4.9.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 01:51:44.142952 umirobot-22.4.6/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 01:51:44.130951 umirobot-22.4.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 01:51:44.130951 umirobot-22.4.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      997 2022-06-23 01:51:39.000000 umirobot-22.4.6/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-06-23 01:51:39.000000 umirobot-22.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-06-23 01:51:44.142952 umirobot-22.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-06-23 01:51:39.000000 umirobot-22.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-06-23 01:51:39.000000 umirobot-22.4.6/installer.py
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-06-23 01:51:39.000000 umirobot-22.4.6/installer.spec
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-06-23 01:51:39.000000 umirobot-22.4.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-23 01:51:44.142952 umirobot-22.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1478 2022-06-23 01:51:39.000000 umirobot-22.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 01:51:44.134951 umirobot-22.4.6/umirobot/
--rw-r--r--   0 runner    (1001) docker     (121)      807 2022-06-23 01:51:39.000000 umirobot-22.4.6/umirobot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      888 2022-06-23 01:51:39.000000 umirobot-22.4.6/umirobot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10625 2022-06-23 01:51:39.000000 umirobot-22.4.6/umirobot/_umirobot.py
--rw-r--r--   0 runner    (1001) docker     (121)     2981 2022-06-23 01:51:39.000000 umirobot-22.4.6/umirobot/_umirobot_communication_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 01:51:44.138951 umirobot-22.4.6/umirobot/gui/
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-06-23 01:51:39.000000 umirobot-22.4.6/umirobot/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27753 2022-06-23 01:51:39.000000 umirobot-22.4.6/umirobot/gui/_umirobot_main_window.py
--rw-r--r--   0 runner    (1001) docker     (121)    35777 2022-06-23 01:51:39.000000 umirobot-22.4.6/umirobot/gui/_umirobot_main_window_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)   353566 2022-06-23 01:51:39.000000 umirobot-22.4.6/umirobot/gui/icon.png
--rw-r--r--   0 runner    (1001) docker     (121)     4112 2022-06-23 01:51:39.000000 umirobot-22.4.6/umirobot/gui/umirobot.png
--rw-r--r--   0 runner    (1001) docker     (121)    37145 2022-06-23 01:51:39.000000 umirobot-22.4.6/umirobot/gui/umirobot_main_window.ui
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 01:51:44.142952 umirobot-22.4.6/umirobot/shared_memory/
--rw-r--r--   0 runner    (1001) docker     (121)      876 2022-06-23 01:51:39.000000 umirobot-22.4.6/umirobot/shared_memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2728 2022-06-23 01:51:39.000000 umirobot-22.4.6/umirobot/shared_memory/test_umirobot_shared_memory.py
--rw-r--r--   0 runner    (1001) docker     (121)      915 2022-06-23 01:51:39.000000 umirobot-22.4.6/umirobot/shared_memory/umirobot_shared_memory_common.py
--rw-r--r--   0 runner    (1001) docker     (121)     4653 2022-06-23 01:51:39.000000 umirobot-22.4.6/umirobot/shared_memory/umirobot_shared_memory_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     3340 2022-06-23 01:51:39.000000 umirobot-22.4.6/umirobot/shared_memory/umirobot_shared_memory_receiver.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 01:51:44.134951 umirobot-22.4.6/umirobot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-06-23 01:51:44.000000 umirobot-22.4.6/umirobot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-06-23 01:51:44.000000 umirobot-22.4.6/umirobot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-23 01:51:44.000000 umirobot-22.4.6/umirobot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-06-23 01:51:44.000000 umirobot-22.4.6/umirobot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-23 01:51:44.000000 umirobot-22.4.6/umirobot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 08:01:48.390799 umirobot-22.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 08:01:48.386799 umirobot-22.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 08:01:48.390799 umirobot-22.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      997 2022-06-23 08:01:40.000000 umirobot-22.4.9/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-23 08:01:40.000000 umirobot-22.4.9/.install.sh
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-06-23 08:01:40.000000 umirobot-22.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-06-23 08:01:48.390799 umirobot-22.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      709 2022-06-23 08:01:40.000000 umirobot-22.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      234 2022-06-23 08:01:40.000000 umirobot-22.4.9/installer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      987 2022-06-23 08:01:40.000000 umirobot-22.4.9/installer.spec
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-06-23 08:01:40.000000 umirobot-22.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-23 08:01:48.394799 umirobot-22.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1478 2022-06-23 08:01:40.000000 umirobot-22.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 08:01:48.390799 umirobot-22.4.9/umirobot/
+-rw-r--r--   0 runner    (1001) docker     (121)      807 2022-06-23 08:01:40.000000 umirobot-22.4.9/umirobot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      888 2022-06-23 08:01:40.000000 umirobot-22.4.9/umirobot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10625 2022-06-23 08:01:40.000000 umirobot-22.4.9/umirobot/_umirobot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2981 2022-06-23 08:01:40.000000 umirobot-22.4.9/umirobot/_umirobot_communication_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 08:01:48.390799 umirobot-22.4.9/umirobot/gui/
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2022-06-23 08:01:40.000000 umirobot-22.4.9/umirobot/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27753 2022-06-23 08:01:40.000000 umirobot-22.4.9/umirobot/gui/_umirobot_main_window.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35777 2022-06-23 08:01:40.000000 umirobot-22.4.9/umirobot/gui/_umirobot_main_window_ui.py
+-rw-r--r--   0 runner    (1001) docker     (121)   353566 2022-06-23 08:01:40.000000 umirobot-22.4.9/umirobot/gui/icon.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4112 2022-06-23 08:01:40.000000 umirobot-22.4.9/umirobot/gui/umirobot.png
+-rw-r--r--   0 runner    (1001) docker     (121)    37145 2022-06-23 08:01:40.000000 umirobot-22.4.9/umirobot/gui/umirobot_main_window.ui
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 08:01:48.390799 umirobot-22.4.9/umirobot/shared_memory/
+-rw-r--r--   0 runner    (1001) docker     (121)      876 2022-06-23 08:01:40.000000 umirobot-22.4.9/umirobot/shared_memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2728 2022-06-23 08:01:40.000000 umirobot-22.4.9/umirobot/shared_memory/test_umirobot_shared_memory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      915 2022-06-23 08:01:40.000000 umirobot-22.4.9/umirobot/shared_memory/umirobot_shared_memory_common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4653 2022-06-23 08:01:40.000000 umirobot-22.4.9/umirobot/shared_memory/umirobot_shared_memory_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3340 2022-06-23 08:01:40.000000 umirobot-22.4.9/umirobot/shared_memory/umirobot_shared_memory_receiver.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 08:01:48.390799 umirobot-22.4.9/umirobot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-06-23 08:01:48.000000 umirobot-22.4.9/umirobot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      834 2022-06-23 08:01:48.000000 umirobot-22.4.9/umirobot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-23 08:01:48.000000 umirobot-22.4.9/umirobot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-06-23 08:01:48.000000 umirobot-22.4.9/umirobot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-23 08:01:48.000000 umirobot-22.4.9/umirobot.egg-info/top_level.txt
```

### Comparing `umirobot-22.4.6/.github/workflows/python-package.yml` & `umirobot-22.4.9/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `umirobot-22.4.6/LICENSE` & `umirobot-22.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `umirobot-22.4.6/PKG-INFO` & `umirobot-22.4.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umirobot
-Version: 22.4.6
+Version: 22.4.9
 Summary: UMIRobot control code and GUI for Python.
 Home-page: https://github.com/mmmarinho/umirobot-py
 Author: Murilo M. Marinho
 Author-email: murilo@g.ecc.u-tokyo.ac.jp
 License: GPLv3
 Description: # UMIRobot Python [![Python package](https://github.com/mmmarinho/umirobot-py/actions/workflows/python-package.yml/badge.svg)](https://github.com/mmmarinho/umirobot-py/actions/workflows/python-package.yml)[![PyPI version](https://badge.fury.io/py/umirobot.svg)](https://badge.fury.io/py/umirobot)
```

### Comparing `umirobot-22.4.6/README.md` & `umirobot-22.4.9/README.md`

 * *Files identical despite different names*

### Comparing `umirobot-22.4.6/installer.spec` & `umirobot-22.4.9/installer.spec`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 block_cipher = None
 
 
 a = Analysis(
     ['installer.py'],
     pathex=[],
     binaries=[],
-    datas=[],
+    datas=[('umirobot/gui/umirobot.png','umirobot/gui')],
     hiddenimports=['numpy'],
     hookspath=[],
     hooksconfig={},
     runtime_hooks=[],
     excludes=[],
     win_no_prefer_redirects=False,
     win_private_assemblies=False,
@@ -41,10 +41,10 @@
     target_arch=None,
     codesign_identity=None,
     entitlements_file=None,
 )
 app = BUNDLE(
     exe,
     name='UMIRobotGUI.app',
-    icon=None,
+    icon='umirobot/gui/icon.png',
     bundle_identifier=None,
 )
```

### Comparing `umirobot-22.4.6/setup.py` & `umirobot-22.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `umirobot-22.4.6/umirobot/__init__.py` & `umirobot-22.4.9/umirobot/__init__.py`

 * *Files identical despite different names*

### Comparing `umirobot-22.4.6/umirobot/__main__.py` & `umirobot-22.4.9/umirobot/__main__.py`

 * *Files identical despite different names*

### Comparing `umirobot-22.4.6/umirobot/_umirobot.py` & `umirobot-22.4.9/umirobot/_umirobot.py`

 * *Files identical despite different names*

### Comparing `umirobot-22.4.6/umirobot/_umirobot_communication_loop.py` & `umirobot-22.4.9/umirobot/_umirobot_communication_loop.py`

 * *Files identical despite different names*

### Comparing `umirobot-22.4.6/umirobot/gui/__init__.py` & `umirobot-22.4.9/umirobot/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `umirobot-22.4.6/umirobot/gui/_umirobot_main_window.py` & `umirobot-22.4.9/umirobot/gui/_umirobot_main_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 # Regenerate UI with 'pyuic6 umirobot_main_window.ui -o _umirobot_main_window_ui.py'
 class UMIRobotMainWindow(QMainWindow):
     def __init__(self, umi_robot_shared_memory_receiver):
         super(UMIRobotMainWindow, self).__init__()
         self.ui = Ui_MainWindow()
         self.ui.setupUi(self)
 
-        self.statusBar().showMessage("Copyright (c) 2020-2021 Murilo M. Marinho (www.murilomarinho.info)")
+        self.statusBar().showMessage("Copyright (c) 2020-2022 Murilo M. Marinho (www.murilomarinho.info)")
 
         self.umi_robot_shared_memory_receiver = umi_robot_shared_memory_receiver
         self.is_open = False
         self.qd = [0, 0, 0, 0, 0, 0]
         self.q_min = -90
         self.q_max = 90
```

### Comparing `umirobot-22.4.6/umirobot/gui/_umirobot_main_window_ui.py` & `umirobot-22.4.9/umirobot/gui/_umirobot_main_window_ui.py`

 * *Files identical despite different names*

### Comparing `umirobot-22.4.6/umirobot/gui/icon.png` & `umirobot-22.4.9/umirobot/gui/icon.png`

 * *Files identical despite different names*

### Comparing `umirobot-22.4.6/umirobot/gui/umirobot.png` & `umirobot-22.4.9/umirobot/gui/umirobot.png`

 * *Files identical despite different names*

### Comparing `umirobot-22.4.6/umirobot/gui/umirobot_main_window.ui` & `umirobot-22.4.9/umirobot/gui/umirobot_main_window.ui`

 * *Files identical despite different names*

### Comparing `umirobot-22.4.6/umirobot/shared_memory/__init__.py` & `umirobot-22.4.9/umirobot/shared_memory/__init__.py`

 * *Files identical despite different names*

### Comparing `umirobot-22.4.6/umirobot/shared_memory/test_umirobot_shared_memory.py` & `umirobot-22.4.9/umirobot/shared_memory/test_umirobot_shared_memory.py`

 * *Files identical despite different names*

### Comparing `umirobot-22.4.6/umirobot/shared_memory/umirobot_shared_memory_common.py` & `umirobot-22.4.9/umirobot/shared_memory/umirobot_shared_memory_common.py`

 * *Files identical despite different names*

### Comparing `umirobot-22.4.6/umirobot/shared_memory/umirobot_shared_memory_provider.py` & `umirobot-22.4.9/umirobot/shared_memory/umirobot_shared_memory_provider.py`

 * *Files identical despite different names*

### Comparing `umirobot-22.4.6/umirobot/shared_memory/umirobot_shared_memory_receiver.py` & `umirobot-22.4.9/umirobot/shared_memory/umirobot_shared_memory_receiver.py`

 * *Files identical despite different names*

### Comparing `umirobot-22.4.6/umirobot.egg-info/PKG-INFO` & `umirobot-22.4.9/umirobot.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umirobot
-Version: 22.4.6
+Version: 22.4.9
 Summary: UMIRobot control code and GUI for Python.
 Home-page: https://github.com/mmmarinho/umirobot-py
 Author: Murilo M. Marinho
 Author-email: murilo@g.ecc.u-tokyo.ac.jp
 License: GPLv3
 Description: # UMIRobot Python [![Python package](https://github.com/mmmarinho/umirobot-py/actions/workflows/python-package.yml/badge.svg)](https://github.com/mmmarinho/umirobot-py/actions/workflows/python-package.yml)[![PyPI version](https://badge.fury.io/py/umirobot.svg)](https://badge.fury.io/py/umirobot)
```

### Comparing `umirobot-22.4.6/umirobot.egg-info/SOURCES.txt` & `umirobot-22.4.9/umirobot.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.install.sh
 LICENSE
 README.md
 installer.py
 installer.spec
 requirements.txt
 setup.py
 .github/workflows/python-package.yml
```

