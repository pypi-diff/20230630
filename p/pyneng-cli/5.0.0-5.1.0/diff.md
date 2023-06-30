# Comparing `tmp/pyneng-cli-5.0.0.tar.gz` & `tmp/pyneng-cli-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/vagrant/repos/uk/pyneng-cli/dist/.tmp-k2ti_w8n/pyneng-cli-5.0.0.tar", last modified: Sun Mar 19 17:45:16 2023, max compression
+gzip compressed data, was "/home/vagrant/repos/pyneng-cli/dist/.tmp-kcpkvnmz/pyneng-cli-5.1.0.tar", last modified: Fri Jun 30 18:03:06 2023, max compression
```

## Comparing `pyneng-cli-5.0.0.tar` & `pyneng-cli-5.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-03-19 17:45:16.712054 pyneng-cli-5.0.0/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1075 2023-03-19 17:34:58.000000 pyneng-cli-5.0.0/LICENSE
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6242 2023-03-19 17:45:16.712054 pyneng-cli-5.0.0/PKG-INFO
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5840 2023-03-19 17:34:58.000000 pyneng-cli-5.0.0/README.md
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       98 2023-03-19 17:34:58.000000 pyneng-cli-5.0.0/pyproject.toml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      810 2023-03-19 17:45:16.712054 pyneng-cli-5.0.0/setup.cfg
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-03-19 17:45:16.700055 pyneng-cli-5.0.0/src/
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-03-19 17:45:16.708054 pyneng-cli-5.0.0/src/pyneng_cli/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1584 2023-03-19 17:44:49.000000 pyneng-cli-5.0.0/src/pyneng_cli/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       63 2023-03-19 17:34:58.000000 pyneng-cli-5.0.0/src/pyneng_cli/exceptions.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    10315 2023-03-19 17:44:49.000000 pyneng-cli-5.0.0/src/pyneng_cli/pyneng.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5870 2023-03-19 17:34:58.000000 pyneng-cli-5.0.0/src/pyneng_cli/pyneng_docs.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    10003 2023-03-19 17:39:56.000000 pyneng-cli-5.0.0/src/pyneng_cli/utils.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-03-19 17:45:16.712054 pyneng-cli-5.0.0/src/pyneng_cli.egg-info/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6242 2023-03-19 17:45:16.000000 pyneng-cli-5.0.0/src/pyneng_cli.egg-info/PKG-INFO
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      407 2023-03-19 17:45:16.000000 pyneng-cli-5.0.0/src/pyneng_cli.egg-info/SOURCES.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        1 2023-03-19 17:45:16.000000 pyneng-cli-5.0.0/src/pyneng_cli.egg-info/dependency_links.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       49 2023-03-19 17:45:16.000000 pyneng-cli-5.0.0/src/pyneng_cli.egg-info/entry_points.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       92 2023-03-19 17:45:16.000000 pyneng-cli-5.0.0/src/pyneng_cli.egg-info/requires.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       11 2023-03-19 17:45:16.000000 pyneng-cli-5.0.0/src/pyneng_cli.egg-info/top_level.txt
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-06-30 18:03:05.995795 pyneng-cli-5.1.0/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1075 2023-06-30 18:02:38.000000 pyneng-cli-5.1.0/LICENSE
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6242 2023-06-30 18:03:05.995795 pyneng-cli-5.1.0/PKG-INFO
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5840 2023-06-30 18:02:38.000000 pyneng-cli-5.1.0/README.md
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       98 2023-06-30 18:02:38.000000 pyneng-cli-5.1.0/pyproject.toml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      810 2023-06-30 18:03:05.995795 pyneng-cli-5.1.0/setup.cfg
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-06-30 18:03:05.983789 pyneng-cli-5.1.0/src/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-06-30 18:03:05.987791 pyneng-cli-5.1.0/src/pyneng_cli/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1584 2023-06-30 18:02:38.000000 pyneng-cli-5.1.0/src/pyneng_cli/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       63 2023-06-30 18:02:38.000000 pyneng-cli-5.1.0/src/pyneng_cli/exceptions.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    10314 2023-06-30 18:02:38.000000 pyneng-cli-5.1.0/src/pyneng_cli/pyneng.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5870 2023-06-30 18:02:38.000000 pyneng-cli-5.1.0/src/pyneng_cli/pyneng_docs.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    10003 2023-06-30 18:02:38.000000 pyneng-cli-5.1.0/src/pyneng_cli/utils.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-06-30 18:03:05.995795 pyneng-cli-5.1.0/src/pyneng_cli.egg-info/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6242 2023-06-30 18:03:05.000000 pyneng-cli-5.1.0/src/pyneng_cli.egg-info/PKG-INFO
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      407 2023-06-30 18:03:05.000000 pyneng-cli-5.1.0/src/pyneng_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        1 2023-06-30 18:03:05.000000 pyneng-cli-5.1.0/src/pyneng_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       49 2023-06-30 18:03:05.000000 pyneng-cli-5.1.0/src/pyneng_cli.egg-info/entry_points.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       92 2023-06-30 18:03:05.000000 pyneng-cli-5.1.0/src/pyneng_cli.egg-info/requires.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       11 2023-06-30 18:03:05.000000 pyneng-cli-5.1.0/src/pyneng_cli.egg-info/top_level.txt
```

### Comparing `pyneng-cli-5.0.0/LICENSE` & `pyneng-cli-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneng-cli-5.0.0/PKG-INFO` & `pyneng-cli-5.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneng-cli
-Version: 5.0.0
+Version: 5.1.0
 Summary: CLI tool for testing tasks from the book Python for Network Engineers
 Home-page: https://github.com/natenka/pyneng-cli
 Author: Natasha Samoylenko
 Author-email: "Natasha Samoylenko" <natasha.samoylenko@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `pyneng-cli-5.0.0/README.md` & `pyneng-cli-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyneng-cli-5.0.0/setup.cfg` & `pyneng-cli-5.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyneng-cli
-version = 5.0.0
+version = 5.1.0
 description = CLI tool for testing tasks from the book Python for Network Engineers
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/natenka/pyneng-cli
 author = Natasha Samoylenko
 author_email = "Natasha Samoylenko" <natasha.samoylenko@gmail.com>
 license = MIT
```

### Comparing `pyneng-cli-5.0.0/src/pyneng_cli/__init__.py` & `pyneng-cli-5.1.0/src/pyneng_cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "5.0.0"
+__version__ = "5.1.0"
 
 ANSWERS_URL = "https://github.com/natenka/pyneng-tasks-solutions"
 # needed for tasks/tests updates
 TASKS_URL = "https://github.com/natenka/pynenguk-tasks"
 TASKS_LOCAL_REPO = ".pynenguk-tasks"
 LANG_TASKS_URL = {
     "uk": "https://github.com/natenka/pynenguk-tasks",
```

### Comparing `pyneng-cli-5.0.0/src/pyneng_cli/pyneng.py` & `pyneng-cli-5.1.0/src/pyneng_cli/pyneng.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
 @click.option(
     "--all",
     "git_add_all_to_github",
     is_flag=True,
     help="Add git add .",
 )
 @click.option("--ignore-ssl-cert", default=False)
-@click.version_option(version="5.0.0")
+@click.version_option(version="5.1.0")
 def cli(
     tasks,
     disable_verbose,
     answer,
     debug,
     default_branch,
     git_add_all_to_github,
@@ -269,15 +269,15 @@
 
     if update_tasks_tests:
         LANG = click.prompt(
             "Please select a language from the following",
             type=click.Choice(["uk", "en", "ru"]),
         )
         if update_tests_only:
-            tasks_files = None
+            task_files = None
             msg = green("Tests updated successfully")
         else:
             msg = green("Tasks and tests updated successfully")
 
         upd = update_tasks_and_tests(
             task_files, test_files, branch=DEFAULT_BRANCH, lang=LANG
         )
```

### Comparing `pyneng-cli-5.0.0/src/pyneng_cli/pyneng_docs.py` & `pyneng-cli-5.1.0/src/pyneng_cli/pyneng_docs.py`

 * *Files identical despite different names*

### Comparing `pyneng-cli-5.0.0/src/pyneng_cli/utils.py` & `pyneng-cli-5.1.0/src/pyneng_cli/utils.py`

 * *Files identical despite different names*

### Comparing `pyneng-cli-5.0.0/src/pyneng_cli.egg-info/PKG-INFO` & `pyneng-cli-5.1.0/src/pyneng_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneng-cli
-Version: 5.0.0
+Version: 5.1.0
 Summary: CLI tool for testing tasks from the book Python for Network Engineers
 Home-page: https://github.com/natenka/pyneng-cli
 Author: Natasha Samoylenko
 Author-email: "Natasha Samoylenko" <natasha.samoylenko@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

