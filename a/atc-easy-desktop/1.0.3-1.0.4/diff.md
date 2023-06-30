# Comparing `tmp/atc_easy_desktop-1.0.3.tar.gz` & `tmp/atc_easy_desktop-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atc_easy_desktop-1.0.3.tar", last modified: Fri Jun 30 02:34:42 2023, max compression
+gzip compressed data, was "atc_easy_desktop-1.0.4.tar", last modified: Fri Jun 30 02:43:39 2023, max compression
```

## Comparing `atc_easy_desktop-1.0.3.tar` & `atc_easy_desktop-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 02:34:42.208234 atc_easy_desktop-1.0.3/
--rw-rw-rw-   0        0        0     1205 2023-06-30 02:34:42.208234 atc_easy_desktop-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-06-30 02:00:34.000000 atc_easy_desktop-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 02:34:42.196267 atc_easy_desktop-1.0.3/atc_easy_desktop/
--rw-rw-rw-   0        0        0       43 2023-06-30 02:00:34.000000 atc_easy_desktop-1.0.3/atc_easy_desktop/__init__.py
--rw-rw-rw-   0        0        0     1909 2023-06-30 02:31:04.000000 atc_easy_desktop-1.0.3/atc_easy_desktop/atc_easy_desktop.py
-drwxrwxrwx   0        0        0        0 2023-06-30 02:34:42.207271 atc_easy_desktop-1.0.3/atc_easy_desktop.egg-info/
--rw-rw-rw-   0        0        0     1205 2023-06-30 02:34:42.000000 atc_easy_desktop-1.0.3/atc_easy_desktop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-06-30 02:34:42.000000 atc_easy_desktop-1.0.3/atc_easy_desktop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 02:34:42.000000 atc_easy_desktop-1.0.3/atc_easy_desktop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-30 02:34:42.000000 atc_easy_desktop-1.0.3/atc_easy_desktop.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-30 02:34:42.000000 atc_easy_desktop-1.0.3/atc_easy_desktop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 02:34:42.208234 atc_easy_desktop-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      744 2023-06-30 02:34:20.000000 atc_easy_desktop-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 02:43:39.530593 atc_easy_desktop-1.0.4/
+-rw-rw-rw-   0        0        0     1205 2023-06-30 02:43:39.529596 atc_easy_desktop-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-06-30 02:00:34.000000 atc_easy_desktop-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 02:43:39.525606 atc_easy_desktop-1.0.4/atc_easy_desktop/
+-rw-rw-rw-   0        0        0       43 2023-06-30 02:00:34.000000 atc_easy_desktop-1.0.4/atc_easy_desktop/__init__.py
+-rw-rw-rw-   0        0        0     1858 2023-06-30 02:41:55.000000 atc_easy_desktop-1.0.4/atc_easy_desktop/atc_easy_desktop.py
+drwxrwxrwx   0        0        0        0 2023-06-30 02:43:39.529596 atc_easy_desktop-1.0.4/atc_easy_desktop.egg-info/
+-rw-rw-rw-   0        0        0     1205 2023-06-30 02:43:39.000000 atc_easy_desktop-1.0.4/atc_easy_desktop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-30 02:43:39.000000 atc_easy_desktop-1.0.4/atc_easy_desktop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 02:43:39.000000 atc_easy_desktop-1.0.4/atc_easy_desktop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-30 02:43:39.000000 atc_easy_desktop-1.0.4/atc_easy_desktop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-30 02:43:39.000000 atc_easy_desktop-1.0.4/atc_easy_desktop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 02:43:39.530593 atc_easy_desktop-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      744 2023-06-30 02:42:40.000000 atc_easy_desktop-1.0.4/setup.py
```

### Comparing `atc_easy_desktop-1.0.3/PKG-INFO` & `atc_easy_desktop-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atc_easy_desktop
-Version: 1.0.3
+Version: 1.0.4
 Summary: Thư viện sử dụng để code game trên màn hình desktop
 Home-page: UNKNOWN
 Author: Chienbg200
 Author-email: chienbg200400@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `atc_easy_desktop-1.0.3/README.md` & `atc_easy_desktop-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `atc_easy_desktop-1.0.3/atc_easy_desktop/atc_easy_desktop.py` & `atc_easy_desktop-1.0.4/atc_easy_desktop/atc_easy_desktop.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,10 +41,7 @@
         if class_name == "WorkerW":
             child = win32gui.FindWindowEx(hwnd, 0, "SHELLDLL_DefView", "")
             if child != 0:
                 sys_listview = win32gui.FindWindowEx(child, 0, "SysListView32", "FolderView")
                 extra.append(sys_listview)
                 return False
         return True
-
-oke = EasyDesktop()
-print(oke.get_screen_size())
```

### Comparing `atc_easy_desktop-1.0.3/atc_easy_desktop.egg-info/PKG-INFO` & `atc_easy_desktop-1.0.4/atc_easy_desktop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atc-easy-desktop
-Version: 1.0.3
+Version: 1.0.4
 Summary: Thư viện sử dụng để code game trên màn hình desktop
 Home-page: UNKNOWN
 Author: Chienbg200
 Author-email: chienbg200400@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `atc_easy_desktop-1.0.3/setup.py` & `atc_easy_desktop-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='atc_easy_desktop',
-    version='1.0.3',
+    version='1.0.4',
     description='Thư viện sử dụng để code game trên màn hình desktop',
     long_description=long_description,
     author='Chienbg200',
     author_email='chienbg200400@gmail.com',
     packages=['atc_easy_desktop'],
     install_requires=[
         'pywin32',
```

