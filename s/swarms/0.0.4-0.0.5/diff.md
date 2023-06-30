# Comparing `tmp/swarms-0.0.4.tar.gz` & `tmp/swarms-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.0.4.tar", last modified: Fri Jun 30 18:08:11 2023, max compression
+gzip compressed data, was "swarms-0.0.5.tar", last modified: Fri Jun 30 19:30:07 2023, max compression
```

## Comparing `swarms-0.0.4.tar` & `swarms-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:08:11.927374 swarms-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 18:08:00.000000 swarms-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-30 18:08:11.927374 swarms-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-06-30 18:08:00.000000 swarms-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 18:08:11.927374 swarms-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-30 18:08:00.000000 swarms-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:08:11.927374 swarms-0.0.4/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-30 18:08:00.000000 swarms-0.0.4/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:08:11.927374 swarms-0.0.4/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:08:00.000000 swarms-0.0.4/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-06-30 18:08:00.000000 swarms-0.0.4/swarms/agents/swarms.py
--rw-r--r--   0 runner    (1001) docker     (123)    29450 2023-06-30 18:08:00.000000 swarms-0.0.4/swarms/agents/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:08:11.927374 swarms-0.0.4/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-30 18:08:11.000000 swarms-0.0.4/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-30 18:08:11.000000 swarms-0.0.4/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 18:08:11.000000 swarms-0.0.4/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-30 18:08:11.000000 swarms-0.0.4/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 18:08:11.000000 swarms-0.0.4/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:30:07.878474 swarms-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 19:29:56.000000 swarms-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-30 19:30:07.878474 swarms-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-06-30 19:29:56.000000 swarms-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 19:30:07.878474 swarms-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-30 19:29:56.000000 swarms-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:30:07.878474 swarms-0.0.5/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-30 19:29:56.000000 swarms-0.0.5/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:30:07.878474 swarms-0.0.5/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:56.000000 swarms-0.0.5/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-06-30 19:29:56.000000 swarms-0.0.5/swarms/agents/swarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29450 2023-06-30 19:29:56.000000 swarms-0.0.5/swarms/agents/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:30:07.878474 swarms-0.0.5/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-30 19:30:07.000000 swarms-0.0.5/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-30 19:30:07.000000 swarms-0.0.5/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:30:07.000000 swarms-0.0.5/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-30 19:30:07.000000 swarms-0.0.5/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 19:30:07.000000 swarms-0.0.5/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.0.4/LICENSE` & `swarms-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.0.4/PKG-INFO` & `swarms-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.0.4
+Version: 0.0.5
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.0.4/README.md` & `swarms-0.0.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,36 @@
 
 ## Table of Contents
 1. [Installation](#installation)
 2. [Usage](#usage)
 3. [Sharing](#sharing)
 
 ## Installation
+There are 2 methods, one is through `git clone` and the other is by `pip install swarms`
+
+# Method1
+* Pip install `python3 -m pip install swarms`
+
+* Create new python file and unleash superintelligence
+
+```python
+
+from swarms import BossNode
+
+boss_node = BossNode()
+
+#create and execute a task
+task = boss_node.create_task("Write a weather report for SF today")
+
+#or 
+# task = boss_node.create_task('Find a video of Elon Musk and make him look like a cat')
+
+boss_node.execute(task)
+```
+
 ```bash
 git clone https://github.com/kyegomez/swarms.git
 cd swarms
 pip install -r requirements.txt
 ```
 
 ## Usage
@@ -159,8 +181,22 @@
 * Integrate hf agents as tools
 
 * [Integrate tools from here](https://integrations.langchain.com/)
 
 
 * Create extensive and useful examples 
 
-* And, recreate exampels and usage in readme.
+* And, recreate exampels and usage in readme.
+
+* Create a worker Swarm class, where it's just workers who are equal and that can self scale. If they need help they'll just spawn an entirely new worker and they can spawn more workers
+
+
+
+
+
+# Optimization
+
+* Reliability => The swarm needs to be reliable. How do we quantify reliability -> Reliability is obtaining an desired output with a basic and un-detailed input. 
+
+* Speed => How long does it take the swarm to accomplish a task, such as `let's respond to all the emails`, we need to minimize this => we can do this by cultivating an efficient communication layer, critiquing, and self-alignment with meta prompting.
+
+* Scalability => Asynchrony, Concurrent, and self-healing.
```

### Comparing `swarms-0.0.4/setup.py` & `swarms-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.0.4',
+  version = '0.0.5',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.0.4/swarms/agents/utils.py` & `swarms-0.0.5/swarms/agents/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-0.0.4/swarms.egg-info/PKG-INFO` & `swarms-0.0.5/swarms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.0.4
+Version: 0.0.5
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.0.4/swarms.egg-info/requires.txt` & `swarms-0.0.5/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

