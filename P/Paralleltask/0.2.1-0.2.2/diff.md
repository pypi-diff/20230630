# Comparing `tmp/Paralleltask-0.2.1.tar.gz` & `tmp/Paralleltask-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/data/project/huj/00_software/Paralleltask/dist/.tmp-1dtgch98/Paralleltask-0.2.1.tar", last modified: Sun Jan 29 01:06:25 2023, max compression
+gzip compressed data, was "/data/project/huj/00_software/Paralleltask/dist/.tmp-ssn8a67e/Paralleltask-0.2.2.tar", last modified: Fri Jun 30 02:52:54 2023, max compression
```

## Comparing `Paralleltask-0.2.1.tar` & `Paralleltask-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 huj       (1001) company   (1000)        0 2023-01-29 01:14:58.000000 Paralleltask-0.2.1/
--rw-r--r--   0 huj       (1001) company   (1000)    35149 2022-02-17 01:15:20.000000 Paralleltask-0.2.1/LICENSE
--rw-r--r--   0 huj       (1001) company   (1000)     3402 2023-01-29 01:14:58.000000 Paralleltask-0.2.1/PKG-INFO
--rw-r--r--   0 huj       (1001) company   (1000)     2942 2022-02-17 01:15:20.000000 Paralleltask-0.2.1/README.md
--rw-r--r--   0 huj       (1001) company   (1000)       38 2023-01-29 01:14:58.000000 Paralleltask-0.2.1/setup.cfg
--rw-r--r--   0 huj       (1001) company   (1000)      933 2023-01-29 01:12:28.000000 Paralleltask-0.2.1/setup.py
-drwxr-xr-x   0 huj       (1001) company   (1000)        0 2023-01-29 01:14:53.000000 Paralleltask-0.2.1/src/
-drwxr-xr-x   0 huj       (1001) company   (1000)        0 2023-01-29 01:14:57.000000 Paralleltask-0.2.1/src/Paralleltask.egg-info/
--rw-r--r--   0 huj       (1001) company   (1000)     3402 2023-01-29 01:14:52.000000 Paralleltask-0.2.1/src/Paralleltask.egg-info/PKG-INFO
--rw-r--r--   0 huj       (1001) company   (1000)      451 2023-01-29 01:14:52.000000 Paralleltask-0.2.1/src/Paralleltask.egg-info/SOURCES.txt
--rw-r--r--   0 huj       (1001) company   (1000)        1 2023-01-29 01:14:52.000000 Paralleltask-0.2.1/src/Paralleltask.egg-info/dependency_links.txt
--rw-r--r--   0 huj       (1001) company   (1000)       60 2023-01-29 01:14:52.000000 Paralleltask-0.2.1/src/Paralleltask.egg-info/entry_points.txt
--rw-r--r--   0 huj       (1001) company   (1000)        1 2023-01-16 08:46:55.000000 Paralleltask-0.2.1/src/Paralleltask.egg-info/not-zip-safe
--rw-r--r--   0 huj       (1001) company   (1000)        7 2023-01-29 01:14:52.000000 Paralleltask-0.2.1/src/Paralleltask.egg-info/requires.txt
--rw-r--r--   0 huj       (1001) company   (1000)       13 2023-01-29 01:14:52.000000 Paralleltask-0.2.1/src/Paralleltask.egg-info/top_level.txt
-drwxr-xr-x   0 huj       (1001) company   (1000)        0 2023-01-29 01:14:58.000000 Paralleltask-0.2.1/src/paralleltask/
--rw-r--r--   0 huj       (1001) company   (1000)      104 2022-02-17 01:15:20.000000 Paralleltask-0.2.1/src/paralleltask/__init__.py
--rw-r--r--   0 huj       (1001) company   (1000)     5868 2023-01-29 01:12:28.000000 Paralleltask-0.2.1/src/paralleltask/__main__.py
--rw-r--r--   0 huj       (1001) company   (1000)     1200 2023-01-16 07:27:20.000000 Paralleltask-0.2.1/src/paralleltask/cluster.cfg
--rw-r--r--   0 huj       (1001) company   (1000)     3521 2022-02-17 01:15:20.000000 Paralleltask-0.2.1/src/paralleltask/kit.py
--rw-r--r--   0 huj       (1001) company   (1000)    16149 2023-01-29 01:12:28.000000 Paralleltask-0.2.1/src/paralleltask/task_control.py
+drwxr-xr-x   0 huj       (1001) company   (1000)        0 2023-06-30 02:53:04.000000 Paralleltask-0.2.2/
+-rw-r--r--   0 huj       (1001) company   (1000)    35149 2022-02-17 01:15:20.000000 Paralleltask-0.2.2/LICENSE
+-rw-r--r--   0 huj       (1001) company   (1000)     3402 2023-06-30 02:53:04.000000 Paralleltask-0.2.2/PKG-INFO
+-rw-r--r--   0 huj       (1001) company   (1000)     2942 2022-02-17 01:15:20.000000 Paralleltask-0.2.2/README.md
+-rw-r--r--   0 huj       (1001) company   (1000)       38 2023-06-30 02:53:04.000000 Paralleltask-0.2.2/setup.cfg
+-rw-r--r--   0 huj       (1001) company   (1000)      933 2023-06-30 02:51:04.000000 Paralleltask-0.2.2/setup.py
+drwxr-xr-x   0 huj       (1001) company   (1000)        0 2023-06-30 02:52:59.000000 Paralleltask-0.2.2/src/
+drwxr-xr-x   0 huj       (1001) company   (1000)        0 2023-06-30 02:53:02.000000 Paralleltask-0.2.2/src/Paralleltask.egg-info/
+-rw-r--r--   0 huj       (1001) company   (1000)     3402 2023-06-30 02:52:59.000000 Paralleltask-0.2.2/src/Paralleltask.egg-info/PKG-INFO
+-rw-r--r--   0 huj       (1001) company   (1000)      451 2023-06-30 02:52:59.000000 Paralleltask-0.2.2/src/Paralleltask.egg-info/SOURCES.txt
+-rw-r--r--   0 huj       (1001) company   (1000)        1 2023-06-30 02:52:59.000000 Paralleltask-0.2.2/src/Paralleltask.egg-info/dependency_links.txt
+-rw-r--r--   0 huj       (1001) company   (1000)       60 2023-06-30 02:52:59.000000 Paralleltask-0.2.2/src/Paralleltask.egg-info/entry_points.txt
+-rw-r--r--   0 huj       (1001) company   (1000)        1 2023-01-16 08:46:55.000000 Paralleltask-0.2.2/src/Paralleltask.egg-info/not-zip-safe
+-rw-r--r--   0 huj       (1001) company   (1000)        7 2023-06-30 02:52:59.000000 Paralleltask-0.2.2/src/Paralleltask.egg-info/requires.txt
+-rw-r--r--   0 huj       (1001) company   (1000)       13 2023-06-30 02:52:59.000000 Paralleltask-0.2.2/src/Paralleltask.egg-info/top_level.txt
+drwxr-xr-x   0 huj       (1001) company   (1000)        0 2023-06-30 02:53:03.000000 Paralleltask-0.2.2/src/paralleltask/
+-rw-r--r--   0 huj       (1001) company   (1000)      104 2022-02-17 01:15:20.000000 Paralleltask-0.2.2/src/paralleltask/__init__.py
+-rw-r--r--   0 huj       (1001) company   (1000)     5868 2023-01-29 01:12:28.000000 Paralleltask-0.2.2/src/paralleltask/__main__.py
+-rw-r--r--   0 huj       (1001) company   (1000)     1200 2023-01-16 07:27:20.000000 Paralleltask-0.2.2/src/paralleltask/cluster.cfg
+-rw-r--r--   0 huj       (1001) company   (1000)     3521 2022-02-17 01:15:20.000000 Paralleltask-0.2.2/src/paralleltask/kit.py
+-rw-r--r--   0 huj       (1001) company   (1000)    16260 2023-06-30 02:51:04.000000 Paralleltask-0.2.2/src/paralleltask/task_control.py
```

### Comparing `Paralleltask-0.2.1/LICENSE` & `Paralleltask-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Paralleltask-0.2.1/PKG-INFO` & `Paralleltask-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Paralleltask
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple and lightweight parallel task engine
 Home-page: https://github.com/moold/ParallelTask
 Author: Hu Jiang
 Author-email: mooldhu@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Paralleltask-0.2.1/README.md` & `Paralleltask-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `Paralleltask-0.2.1/setup.py` & `Paralleltask-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Paralleltask",
-    version="0.2.1",
+    version="0.2.2",
     author="Hu Jiang",
     author_email="mooldhu@gmail.com",
     description="A simple and lightweight parallel task engine",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/moold/ParallelTask",
     license="GPLv3",
```

### Comparing `Paralleltask-0.2.1/src/Paralleltask.egg-info/PKG-INFO` & `Paralleltask-0.2.2/src/Paralleltask.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Paralleltask
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple and lightweight parallel task engine
 Home-page: https://github.com/moold/ParallelTask
 Author: Hu Jiang
 Author-email: mooldhu@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Paralleltask-0.2.1/src/paralleltask/__main__.py` & `Paralleltask-0.2.2/src/paralleltask/__main__.py`

 * *Files identical despite different names*

### Comparing `Paralleltask-0.2.1/src/paralleltask/cluster.cfg` & `Paralleltask-0.2.2/src/paralleltask/cluster.cfg`

 * *Files identical despite different names*

### Comparing `Paralleltask-0.2.1/src/paralleltask/kit.py` & `Paralleltask-0.2.2/src/paralleltask/kit.py`

 * *Files identical despite different names*

### Comparing `Paralleltask-0.2.1/src/paralleltask/task_control.py` & `Paralleltask-0.2.2/src/paralleltask/task_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,16 @@
 							paramters = lines[i].split("=")
 							lines[i] = paramters[0] + '=' + os.path.abspath(paramters[1]) if \
 								paramters[1] and len(paramters) == 2 else lines[i]
 						elif '>' in lines[i]:
 							paramters = lines[i].split(">")
 							lines[i] = paramters[0] + '>' + os.path.abspath(paramters[1]) if \
 								paramters[1] and len(paramters) == 2 else lines[i]
+						elif lines[i].startswith('|'):
+							lines[i] = '|' + os.path.abspath(os.path.expanduser(lines[i][1:]))
 						else:
 							lines[i] = os.path.abspath(os.path.expanduser(lines[i]))
 				tasks.append(" ".join(lines))
 		return tasks
 
 	def _init_subtasks(self, tasks):
 		group_tasks = []
```

