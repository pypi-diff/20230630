# Comparing `tmp/git_init_repo-1.0.1.tar.gz` & `tmp/git_init_repo-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_init_repo-1.0.1.tar", last modified: Sun Jun 18 18:55:10 2023, max compression
+gzip compressed data, was "git_init_repo-1.0.2.tar", last modified: Thu Jun 29 22:48:25 2023, max compression
```

## Comparing `git_init_repo-1.0.1.tar` & `git_init_repo-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:55:10.873213 git_init_repo-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-18 18:55:01.000000 git_init_repo-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-18 18:55:10.873213 git_init_repo-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-18 18:55:01.000000 git_init_repo-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:55:10.873213 git_init_repo-1.0.1/api_queries/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-18 18:55:01.000000 git_init_repo-1.0.1/api_queries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:55:10.873213 git_init_repo-1.0.1/git_init_repo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-18 18:55:10.000000 git_init_repo-1.0.1/git_init_repo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-18 18:55:10.000000 git_init_repo-1.0.1/git_init_repo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 18:55:10.000000 git_init_repo-1.0.1/git_init_repo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 18:55:10.000000 git_init_repo-1.0.1/git_init_repo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-18 18:55:10.000000 git_init_repo-1.0.1/git_init_repo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 18:55:10.873213 git_init_repo-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-18 18:55:01.000000 git_init_repo-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:55:10.873213 git_init_repo-1.0.1/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-18 18:55:01.000000 git_init_repo-1.0.1/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-18 18:55:01.000000 git_init_repo-1.0.1/utils/vscode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:48:25.917933 git_init_repo-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-29 22:48:13.000000 git_init_repo-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-29 22:48:25.917933 git_init_repo-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-29 22:48:13.000000 git_init_repo-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:48:25.913933 git_init_repo-1.0.2/api_queries/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-29 22:48:13.000000 git_init_repo-1.0.2/api_queries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:48:25.913933 git_init_repo-1.0.2/git_init_repo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-29 22:48:25.000000 git_init_repo-1.0.2/git_init_repo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-29 22:48:25.000000 git_init_repo-1.0.2/git_init_repo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 22:48:25.000000 git_init_repo-1.0.2/git_init_repo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 22:48:25.000000 git_init_repo-1.0.2/git_init_repo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 22:48:25.000000 git_init_repo-1.0.2/git_init_repo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 22:48:25.917933 git_init_repo-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-29 22:48:13.000000 git_init_repo-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:48:25.913933 git_init_repo-1.0.2/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-29 22:48:13.000000 git_init_repo-1.0.2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-29 22:48:13.000000 git_init_repo-1.0.2/utils/vscode.py
```

### Comparing `git_init_repo-1.0.1/LICENSE` & `git_init_repo-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `git_init_repo-1.0.1/PKG-INFO` & `git_init_repo-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git_init_repo
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python script to initialize a git repository.
 Author: Thomas "Aiglon Dore" R.
 Author-email: aiglondore@outlook.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Repo init tool
```

### Comparing `git_init_repo-1.0.1/README.md` & `git_init_repo-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `git_init_repo-1.0.1/api_queries/__init__.py` & `git_init_repo-1.0.2/api_queries/__init__.py`

 * *Files identical despite different names*

### Comparing `git_init_repo-1.0.1/git_init_repo.egg-info/PKG-INFO` & `git_init_repo-1.0.2/git_init_repo.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-init-repo
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python script to initialize a git repository.
 Author: Thomas "Aiglon Dore" R.
 Author-email: aiglondore@outlook.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Repo init tool
```

### Comparing `git_init_repo-1.0.1/setup.py` & `git_init_repo-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='git_init_repo',
-    version='1.0.1',
+    version='1.0.2',
     description='A Python script to initialize a git repository.',
     author='Thomas \"Aiglon Dore\" R.',
     packages= find_packages(),
     install_requires=['aiohttp'],
     author_email='aiglondore@outlook.com',
     long_description="""# Repo init tool
 Provides a Python Package to easliy initiate git repos for Python
```

### Comparing `git_init_repo-1.0.1/utils/__init__.py` & `git_init_repo-1.0.2/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `git_init_repo-1.0.1/utils/vscode.py` & `git_init_repo-1.0.2/utils/vscode.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -24,29 +24,29 @@
         },
         {
             "command": "pip install -r requirements.txt",
             "label": "Install dependencies",
             "type": "shell",
             "problemMatcher": [],
             "dependsOn": [
-                "Upgrade pip"
+                "Install dev dependencies"
             ]
         },
         {
             "command": "pip install -r requirements-dev.txt",
             "label": "Install dev dependencies",
             "type": "shell",
             "problemMatcher": [],
             "dependsOn": [
-                "Install dependencies"
+                "Upgrade pip"
             ]
         },
         {
             "label": "Build environment",
             "dependsOn": [
-                "Install dev dependencies"
+                "Install dependencies"
             ]
         }]
     
     os.mkdir('.vscode')
     with open(r'.vscode/tasks.json', 'w') as f:
         json.dump(dict_tasks, f, indent=4)
```

