# Comparing `tmp/crunch-cli-1.5.0.tar.gz` & `tmp/crunch-cli-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crunch-cli-1.5.0.tar", last modified: Sat Jun 17 13:17:52 2023, max compression
+gzip compressed data, was "crunch-cli-1.5.1.tar", last modified: Fri Jun 30 10:13:20 2023, max compression
```

## Comparing `crunch-cli-1.5.0.tar` & `crunch-cli-1.5.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:17:52.053924 crunch-cli-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-17 13:17:52.053924 crunch-cli-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:17:52.053924 crunch-cli-1.5.0/crunch/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:17:52.053924 crunch-cli-1.5.0/crunch/command/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/command/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/command/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/command/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/command/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/command/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:17:52.053924 crunch-cli-1.5.0/crunch/demo-project/
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/demo-project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/demo-project/files.json
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/demo-project/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/demo-project/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/ensure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:17:52.053924 crunch-cli-1.5.0/crunch_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-17 13:17:52.000000 crunch-cli-1.5.0/crunch_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-17 13:17:52.000000 crunch-cli-1.5.0/crunch_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 13:17:52.000000 crunch-cli-1.5.0/crunch_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-17 13:17:52.000000 crunch-cli-1.5.0/crunch_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 13:17:52.000000 crunch-cli-1.5.0/crunch_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-17 13:17:52.000000 crunch-cli-1.5.0/crunch_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-17 13:17:52.000000 crunch-cli-1.5.0/crunch_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 13:17:52.053924 crunch-cli-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:13:20.892974 crunch-cli-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-30 10:13:20.888974 crunch-cli-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:13:20.888974 crunch-cli-1.5.1/crunch/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:13:20.888974 crunch-cli-1.5.1/crunch/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/command/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/command/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/command/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/command/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/command/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:13:20.888974 crunch-cli-1.5.1/crunch/demo-project/
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/demo-project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/demo-project/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/demo-project/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/demo-project/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/ensure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:13:20.888974 crunch-cli-1.5.1/crunch_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-30 10:13:20.000000 crunch-cli-1.5.1/crunch_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-30 10:13:20.000000 crunch-cli-1.5.1/crunch_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:13:20.000000 crunch-cli-1.5.1/crunch_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 10:13:20.000000 crunch-cli-1.5.1/crunch_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:13:20.000000 crunch-cli-1.5.1/crunch_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-30 10:13:20.000000 crunch-cli-1.5.1/crunch_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 10:13:20.000000 crunch-cli-1.5.1/crunch_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 10:13:20.892974 crunch-cli-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/setup.py
```

### Comparing `crunch-cli-1.5.0/crunch/command/convert.py` & `crunch-cli-1.5.1/crunch/command/convert.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.0/crunch/command/download.py` & `crunch-cli-1.5.1/crunch/command/download.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.0/crunch/command/push.py` & `crunch-cli-1.5.1/crunch/command/push.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import tarfile
 import tempfile
 import shutil
 
 import gitignorefile
 
 from .. import constants, utils
+from .setup import _setup_demo
 
 
 def _list_files(
     directory_path: str,
 ):
     for root, dirs, files in os.walk(directory_path, topdown=False):
         if root.startswith(f"{directory_path}/"):
@@ -63,39 +64,46 @@
 ):
     project_name = utils.read_project_name()
     push_token = utils.read_token()
 
     fds = []
 
     try:
+        if not os.path.exists(constants.DOT_GITIGNORE_FILE):
+            _setup_demo(".",  [constants.DOT_GITIGNORE_FILE])
+
         with tempfile.NamedTemporaryFile(prefix="submission-", suffix=".tar", dir=constants.DOT_CRUNCHDAO_DIRECTORY) as tmp:
             with tarfile.open(fileobj=tmp, mode="w") as tar:
                 for file in _list_code_files(model_directory_path):
                     print(f"compress {file}")
                     tar.add(file)
 
             tmp.seek(0)
 
-            files = [
-                ("codeFile", ('code.tar', tmp, "application/x-tar"))
-            ]
-
-            for path, name in _list_model_files(model_directory_path):
-                print(f"model {name}")
-
-                fd = open(path, "rb")
-                fds.append(fd)
-
-                files.append(("modelFiles", (name, fd)))
-
             if export_path:
                 print(f"export {export_path}")
-                shutil.copyfile(tmp.name, export_path)
+
+                with open(export_path, "wb") as fd:
+                    shutil.copyfileobj(tmp, fd)
             else:
                 print(f"export project/{project_name}")
+
+                files = [
+                    ("codeFile", ('code.tar', tmp, "application/x-tar"))
+                ]
+
+                for path, name in _list_model_files(model_directory_path):
+                    print(f"model {name}")
+
+                    fd = open(path, "rb")
+                    fds.append(fd)
+
+                    files.append(("modelFiles", (name, fd)))
+                    print(f"export project/{project_name}")
+
                 submission = session.post(
                     f"/v1/projects/{project_name}/submissions",
                     data={
                         "message": message,
                         "mainFilePath": main_file_path,
                         "modelDirectoryPath": model_directory_path,
                         "pushToken": push_token,
@@ -112,8 +120,7 @@
 
 def push_summary(submission, session: utils.CustomSession):
     print("\n---")
     print(f"submission #{submission['number']} succesfully uploaded!")
 
     url = session.format_web_url(f"/project/submissions/{submission['number']}")
     print(f"Find it on your dashboard: {url}")
-
```

### Comparing `crunch-cli-1.5.0/crunch/command/setup.py` & `crunch-cli-1.5.1/crunch/command/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,24 +17,28 @@
             print(f"delete {directory}")
             shutil.rmtree(directory)
         else:
             print(f"{directory}: already exists (use --force to override)")
             raise click.Abort()
 
 
-def _setup_demo(directory: str):
-    def read_data(file_name):
-        resource = "/".join(["..", "demo-project", file_name])
-        return pkgutil.get_data(__package__, resource)
+def _read_demo_file(file_name: str):
+    resource = "/".join(["..", "demo-project", file_name])
+    return pkgutil.get_data(__package__, resource)
 
-    files = json.loads(read_data("files.json").decode("utf-8"))
+
+def _setup_demo(directory: str, filter: list = None):
+    files = json.loads(_read_demo_file("files.json").decode("utf-8"))
     for file in files:
+        if filter and file not in filter:
+            continue
+
         print(f"use {file}")
 
-        content = read_data(file)
+        content = _read_demo_file(file)
 
         path = os.path.join(directory, file)
         with open(path, "wb") as fd:
             fd.write(content)
 
 
 def _setup_submission(directory: str, code_tar: io.BytesIO):
```

### Comparing `crunch-cli-1.5.0/crunch/command/test.py` & `crunch-cli-1.5.1/crunch/command/test.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.0/crunch/constants.py` & `crunch-cli-1.5.1/crunch/constants.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.0/crunch/demo-project/.gitignore` & `crunch-cli-1.5.1/crunch/demo-project/.gitignore`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.0/crunch/demo-project/main.py` & `crunch-cli-1.5.1/crunch/demo-project/main.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.0/crunch/ensure.py` & `crunch-cli-1.5.1/crunch/ensure.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.0/crunch/inline.py` & `crunch-cli-1.5.1/crunch/inline.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.0/crunch/library.py` & `crunch-cli-1.5.1/crunch/library.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.0/crunch/main.py` & `crunch-cli-1.5.1/crunch/main.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.0/crunch/tester.py` & `crunch-cli-1.5.1/crunch/tester.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.0/crunch/utils.py` & `crunch-cli-1.5.1/crunch/utils.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.0/crunch_cli.egg-info/SOURCES.txt` & `crunch-cli-1.5.1/crunch_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.0/setup.py` & `crunch-cli-1.5.1/setup.py`

 * *Files identical despite different names*

