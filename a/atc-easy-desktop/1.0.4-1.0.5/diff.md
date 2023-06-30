# Comparing `tmp/atc_easy_desktop-1.0.4.tar.gz` & `tmp/atc_easy_desktop-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atc_easy_desktop-1.0.4.tar", last modified: Fri Jun 30 02:43:39 2023, max compression
+gzip compressed data, was "atc_easy_desktop-1.0.5.tar", last modified: Fri Jun 30 08:04:14 2023, max compression
```

## Comparing `atc_easy_desktop-1.0.4.tar` & `atc_easy_desktop-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 02:43:39.530593 atc_easy_desktop-1.0.4/
--rw-rw-rw-   0        0        0     1205 2023-06-30 02:43:39.529596 atc_easy_desktop-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-06-30 02:00:34.000000 atc_easy_desktop-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 02:43:39.525606 atc_easy_desktop-1.0.4/atc_easy_desktop/
--rw-rw-rw-   0        0        0       43 2023-06-30 02:00:34.000000 atc_easy_desktop-1.0.4/atc_easy_desktop/__init__.py
--rw-rw-rw-   0        0        0     1858 2023-06-30 02:41:55.000000 atc_easy_desktop-1.0.4/atc_easy_desktop/atc_easy_desktop.py
-drwxrwxrwx   0        0        0        0 2023-06-30 02:43:39.529596 atc_easy_desktop-1.0.4/atc_easy_desktop.egg-info/
--rw-rw-rw-   0        0        0     1205 2023-06-30 02:43:39.000000 atc_easy_desktop-1.0.4/atc_easy_desktop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-06-30 02:43:39.000000 atc_easy_desktop-1.0.4/atc_easy_desktop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 02:43:39.000000 atc_easy_desktop-1.0.4/atc_easy_desktop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-30 02:43:39.000000 atc_easy_desktop-1.0.4/atc_easy_desktop.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-30 02:43:39.000000 atc_easy_desktop-1.0.4/atc_easy_desktop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 02:43:39.530593 atc_easy_desktop-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      744 2023-06-30 02:42:40.000000 atc_easy_desktop-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:04:14.905834 atc_easy_desktop-1.0.5/
+-rw-rw-rw-   0        0        0     1205 2023-06-30 08:04:14.905834 atc_easy_desktop-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-06-30 02:00:34.000000 atc_easy_desktop-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 08:04:14.890701 atc_easy_desktop-1.0.5/atc_easy_desktop/
+-rw-rw-rw-   0        0        0       43 2023-06-30 02:00:34.000000 atc_easy_desktop-1.0.5/atc_easy_desktop/__init__.py
+-rw-rw-rw-   0        0        0     1835 2023-06-30 08:01:06.000000 atc_easy_desktop-1.0.5/atc_easy_desktop/atc_easy_desktop.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:04:14.904836 atc_easy_desktop-1.0.5/atc_easy_desktop.egg-info/
+-rw-rw-rw-   0        0        0     1205 2023-06-30 08:04:14.000000 atc_easy_desktop-1.0.5/atc_easy_desktop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-30 08:04:14.000000 atc_easy_desktop-1.0.5/atc_easy_desktop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 08:04:14.000000 atc_easy_desktop-1.0.5/atc_easy_desktop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-30 08:04:14.000000 atc_easy_desktop-1.0.5/atc_easy_desktop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-30 08:04:14.000000 atc_easy_desktop-1.0.5/atc_easy_desktop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 08:04:14.906830 atc_easy_desktop-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      744 2023-06-30 08:01:06.000000 atc_easy_desktop-1.0.5/setup.py
```

### Comparing `atc_easy_desktop-1.0.4/PKG-INFO` & `atc_easy_desktop-1.0.5/atc_easy_desktop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: atc_easy_desktop
-Version: 1.0.4
+Name: atc-easy-desktop
+Version: 1.0.5
 Summary: Thư viện sử dụng để code game trên màn hình desktop
 Home-page: UNKNOWN
 Author: Chienbg200
 Author-email: chienbg200400@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `atc_easy_desktop-1.0.4/README.md` & `atc_easy_desktop-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `atc_easy_desktop-1.0.4/atc_easy_desktop/atc_easy_desktop.py` & `atc_easy_desktop-1.0.5/atc_easy_desktop/atc_easy_desktop.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 class EasyDesktop:
     def __init__(self):
         self.desktop = self._get_desktop_window()
 
     def go_to_xy(self, idx, x, y):
         lparam = (y << 16) | x
-        print(lparam)
         win32gui.SendMessage(self.desktop, commctrl.LVM_SETITEMPOSITION, idx, lparam)
 
     def get_item_count(self):
         return win32gui.SendMessage(self.desktop, commctrl.LVM_GETITEMCOUNT, 0, 0)
 
     def get_screen_size(self):
         monitor_info = win32api.GetMonitorInfo(win32api.EnumDisplayMonitors(None, None)[0][0])
```

### Comparing `atc_easy_desktop-1.0.4/atc_easy_desktop.egg-info/PKG-INFO` & `atc_easy_desktop-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: atc-easy-desktop
-Version: 1.0.4
+Name: atc_easy_desktop
+Version: 1.0.5
 Summary: Thư viện sử dụng để code game trên màn hình desktop
 Home-page: UNKNOWN
 Author: Chienbg200
 Author-email: chienbg200400@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `atc_easy_desktop-1.0.4/setup.py` & `atc_easy_desktop-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='atc_easy_desktop',
-    version='1.0.4',
+    version='1.0.5',
     description='Thư viện sử dụng để code game trên màn hình desktop',
     long_description=long_description,
     author='Chienbg200',
     author_email='chienbg200400@gmail.com',
     packages=['atc_easy_desktop'],
     install_requires=[
         'pywin32',
```

