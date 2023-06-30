# Comparing `tmp/poetry_multiproject_plugin-1.3.0.tar.gz` & `tmp/poetry_multiproject_plugin-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_multiproject_plugin-1.3.0.tar", max compression
+gzip compressed data, was "poetry_multiproject_plugin-1.3.1.tar", max compression
```

## Comparing `poetry_multiproject_plugin-1.3.0.tar` & `poetry_multiproject_plugin-1.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1068 2022-01-23 14:15:18.822524 poetry_multiproject_plugin-1.3.0/LICENSE
--rw-r--r--   0        0        0     6182 2023-06-02 16:10:42.637369 poetry_multiproject_plugin-1.3.0/README.md
--rw-r--r--   0        0        0      122 2022-10-30 09:31:55.254657 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/__init__.py
--rw-r--r--   0        0        0        0 2022-01-27 21:12:19.215558 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/commands/__init__.py
--rw-r--r--   0        0        0       92 2022-10-29 17:34:08.279274 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/commands/buildproject/__init__.py
--rw-r--r--   0        0        0     2848 2023-02-15 17:23:23.134947 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/commands/buildproject/project.py
--rw-r--r--   0        0        0       88 2022-12-26 11:25:28.111604 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/commands/checkproject/__init__.py
--rw-r--r--   0        0        0     2462 2023-01-06 16:42:40.541575 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/commands/checkproject/check.py
--rw-r--r--   0        0        0        0 2022-10-29 17:34:08.280190 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/__init__.py
--rw-r--r--   0        0        0      118 2022-12-26 11:25:28.113080 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/check/__init__.py
--rw-r--r--   0        0        0     1080 2023-01-06 16:42:40.542392 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/check/mypy_checker.py
--rw-r--r--   0        0        0      106 2022-12-27 09:13:24.664513 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/deps/__init__.py
--rw-r--r--   0        0        0      683 2023-01-06 22:56:24.237617 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/deps/installer.py
--rw-r--r--   0        0        0      111 2023-02-13 19:04:54.452935 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/parsing/__init__.py
--rw-r--r--   0        0        0     1775 2023-06-02 15:48:12.775242 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/parsing/rewrite.py
--rw-r--r--   0        0        0      141 2022-10-29 17:34:08.281001 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/project/__init__.py
--rw-r--r--   0        0        0      274 2022-12-28 08:58:51.305973 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/project/cleanup.py
--rw-r--r--   0        0        0      541 2023-05-22 19:10:23.673577 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/project/create.py
--rw-r--r--   0        0        0      304 2022-12-26 11:25:28.115615 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/project/dist.py
--rw-r--r--   0        0        0      875 2023-02-13 19:04:54.455402 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/project/packages.py
--rw-r--r--   0        0        0     1028 2023-06-02 15:48:12.776344 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/project/prepare.py
--rw-r--r--   0        0        0      125 2022-10-29 17:34:08.284437 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/toml/__init__.py
--rw-r--r--   0        0        0     1634 2023-02-13 19:04:54.457639 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/toml/generate.py
--rw-r--r--   0        0        0      592 2023-02-12 16:50:12.589435 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/toml/packages.py
--rw-r--r--   0        0        0      631 2023-02-13 19:04:54.458759 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/toml/read.py
--rw-r--r--   0        0        0      909 2022-12-26 11:25:28.122982 poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/plugin.py
--rw-r--r--   0        0        0      841 2023-06-02 16:10:42.638022 poetry_multiproject_plugin-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     6938 1970-01-01 00:00:00.000000 poetry_multiproject_plugin-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-01-23 14:15:18.822524 poetry_multiproject_plugin-1.3.1/LICENSE
+-rw-r--r--   0        0        0     7152 2023-06-03 14:36:02.225062 poetry_multiproject_plugin-1.3.1/README.md
+-rw-r--r--   0        0        0      122 2022-10-30 09:31:55.254657 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-27 21:12:19.215558 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/commands/__init__.py
+-rw-r--r--   0        0        0       92 2022-10-29 17:34:08.279274 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/commands/buildproject/__init__.py
+-rw-r--r--   0        0        0     2848 2023-02-15 17:23:23.134947 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/commands/buildproject/project.py
+-rw-r--r--   0        0        0       88 2022-12-26 11:25:28.111604 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/commands/checkproject/__init__.py
+-rw-r--r--   0        0        0     2462 2023-01-06 16:42:40.541575 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/commands/checkproject/check.py
+-rw-r--r--   0        0        0        0 2022-10-29 17:34:08.280190 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/__init__.py
+-rw-r--r--   0        0        0      118 2022-12-26 11:25:28.113080 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/check/__init__.py
+-rw-r--r--   0        0        0     1080 2023-01-06 16:42:40.542392 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/check/mypy_checker.py
+-rw-r--r--   0        0        0      106 2022-12-27 09:13:24.664513 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/deps/__init__.py
+-rw-r--r--   0        0        0      683 2023-01-06 22:56:24.237617 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/deps/installer.py
+-rw-r--r--   0        0        0      111 2023-02-13 19:04:54.452935 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/parsing/__init__.py
+-rw-r--r--   0        0        0     1775 2023-06-02 15:48:12.775242 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/parsing/rewrite.py
+-rw-r--r--   0        0        0      141 2022-10-29 17:34:08.281001 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/project/__init__.py
+-rw-r--r--   0        0        0      274 2022-12-28 08:58:51.305973 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/project/cleanup.py
+-rw-r--r--   0        0        0      541 2023-05-22 19:10:23.673577 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/project/create.py
+-rw-r--r--   0        0        0      304 2022-12-26 11:25:28.115615 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/project/dist.py
+-rw-r--r--   0        0        0      922 2023-06-30 16:45:27.035223 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/project/packages.py
+-rw-r--r--   0        0        0     1097 2023-06-30 16:45:27.036018 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/project/prepare.py
+-rw-r--r--   0        0        0      125 2022-10-29 17:34:08.284437 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/toml/__init__.py
+-rw-r--r--   0        0        0     1634 2023-02-13 19:04:54.457639 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/toml/generate.py
+-rw-r--r--   0        0        0      592 2023-02-12 16:50:12.589435 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/toml/packages.py
+-rw-r--r--   0        0        0      631 2023-02-13 19:04:54.458759 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/toml/read.py
+-rw-r--r--   0        0        0      909 2022-12-26 11:25:28.122982 poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/plugin.py
+-rw-r--r--   0        0        0      841 2023-06-30 16:45:27.036556 poetry_multiproject_plugin-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7908 1970-01-01 00:00:00.000000 poetry_multiproject_plugin-1.3.1/PKG-INFO
```

### Comparing `poetry_multiproject_plugin-1.3.0/LICENSE` & `poetry_multiproject_plugin-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.3.0/README.md` & `poetry_multiproject_plugin-1.3.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -14,20 +14,33 @@
 The `build-project` command will make it possible to use relative package includes.
 This feature is very useful for monorepos and when sharing code between projects.
 
 The `check-project` command is useful to check that dependencies are added properly in a project.
 It uses the `MyPy` tool under the hood, and will output any errors from the static type checker.
 
 
+- [Use cases](#use-cases)
+- [Usage](#usage)
+- [Installation](#installation)
+- [What does it do?](#what-does-it-do)
+- [How is it different from the "poetry build" command?](#how-is-it-different-from-the-poetry-build-command)
+- [Organizing code](#organizing-code)
+
 ## Use cases
 
 ### Microservices and apps
 The main use case is to support having one or more microservices or apps in a Monorepo, and share code between the services with namespaced packages.
 The `build-project` command will collect the project-specific packages and build an installable artifact from it (i.e. a wheel or an sdist).
 
+### A basic building block for the Polylith Architecture
+The Multiproject plugin makes it possible to organize Python projects according to the Polylith Architecture.
+The plugin is the foundation for the __Python tools for the Polylith Architecture__ - also implemented as a __Poetry__ plugin.
+
+For more about Polylith, have a look at the [Python-specific Polylith documentation](https://davidvujic.github.io/python-polylith-docs/).
+
 ### Libraries?
 Building libraries is also supported, but you will need to consider that the code will likely share the same top namespace with other libraries 
 built from the same monorepo. It depends on your monorepo structure. This will likely be a problem when more than one of your libraries are installed into the same virtual environment.
 
 Since Python libraries by default are installed in a "flat" folder structure, two libraries with the same top namespace will collide.
 
 There is a way to solve this issue, by using the `--with-top-namespace` flag of the `build-project` command. See [usage for libraries](#usage-for-libraries).
@@ -156,27 +169,45 @@
     { include = "my_namespace/my_package", from = "../../shared" }
     { include = "my_namespace/my_other_package", from = "../../shared" }
 ]
 ```
 
 This plugin will allow relative package includes. You will now be able to share code between projects.
 
-An suggested Monorepo structure, with the shared code extracted into a separate folder structure:
+## Organizing code
+An example Monorepo structure, having the shared code extracted into a separate folder structure:
 
 ``` shell
 projects/
   my_app/
-    pyproject.toml (including a shared package)
+    pyproject.toml (including selected shared packages)
 
   my_service/
-    pyproject.toml (including other shared packages)
+    pyproject.toml (including selected shared packages)
 
 shared/
   my_namespace/
     my_package/
       __init__.py
       code.py
 
     my_other_package/
       __init__.py
       code.py
 ```
+
+A suggested structure, using [Polylith](https://davidvujic.github.io/python-polylith-docs/workspace/):
+
+``` shell
+workspace/
+  bases/
+  components/
+  development/
+  projects/
+
+  poetry.lock
+
+  pyproject.toml
+  workspace.toml
+
+  README.md
+```
```

### Comparing `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/commands/buildproject/project.py` & `poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/commands/buildproject/project.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/commands/checkproject/check.py` & `poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/commands/checkproject/check.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/check/mypy_checker.py` & `poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/check/mypy_checker.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/deps/installer.py` & `poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/deps/installer.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/parsing/rewrite.py` & `poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/parsing/rewrite.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/project/create.py` & `poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/project/create.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/project/packages.py` & `poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/project/packages.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,10 +22,12 @@
         to = f"{top_ns}/{p_to}" if top_ns and is_relative_path else p_to
 
         to = Path(destination / to)
 
         shutil.copytree(
             source,
             to,
-            ignore=shutil.ignore_patterns("__pycache__", ".mypy_cache"),
+            ignore=shutil.ignore_patterns(
+                "__pycache__", ".venv", ".mypy_cache", ".git"
+            ),
             dirs_exist_ok=True,
         )
```

### Comparing `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/project/prepare.py` & `poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/project/prepare.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,20 @@
 def copy_project(project_file: Path, destination: Path) -> Path:
     source = project_file.parent.as_posix()
 
     res = shutil.copytree(
         source,
         destination,
         ignore=shutil.ignore_patterns(
-            "*.pyc", "__pycache__", ".venv", ".mypy_cache", "node_modules"
+            "*.pyc",
+            "__pycache__",
+            ".venv",
+            ".mypy_cache",
+            "node_modules",
+            ".git",
         ),
         dirs_exist_ok=True,
     )
 
     return Path(res)
```

### Comparing `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/toml/generate.py` & `poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/toml/generate.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/toml/packages.py` & `poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/toml/packages.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/components/toml/read.py` & `poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/components/toml/read.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.3.0/poetry_multiproject_plugin/plugin.py` & `poetry_multiproject_plugin-1.3.1/poetry_multiproject_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.3.0/pyproject.toml` & `poetry_multiproject_plugin-1.3.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-multiproject-plugin"
-version = "1.3.0"
+version = "1.3.1"
 description = "A Poetry plugin that makes it possible to use relative package includes."
 authors = ["David Vujic"]
 homepage = "https://github.com/davidvujic/poetry-multiproject-plugin"
 repository = "https://github.com/davidvujic/poetry-multiproject-plugin"
 readme = "README.md"
 packages = [{include = "poetry_multiproject_plugin"}]
```

### Comparing `poetry_multiproject_plugin-1.3.0/PKG-INFO` & `poetry_multiproject_plugin-1.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-multiproject-plugin
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Poetry plugin that makes it possible to use relative package includes.
 Home-page: https://github.com/davidvujic/poetry-multiproject-plugin
 Author: David Vujic
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -32,20 +32,33 @@
 The `build-project` command will make it possible to use relative package includes.
 This feature is very useful for monorepos and when sharing code between projects.
 
 The `check-project` command is useful to check that dependencies are added properly in a project.
 It uses the `MyPy` tool under the hood, and will output any errors from the static type checker.
 
 
+- [Use cases](#use-cases)
+- [Usage](#usage)
+- [Installation](#installation)
+- [What does it do?](#what-does-it-do)
+- [How is it different from the "poetry build" command?](#how-is-it-different-from-the-poetry-build-command)
+- [Organizing code](#organizing-code)
+
 ## Use cases
 
 ### Microservices and apps
 The main use case is to support having one or more microservices or apps in a Monorepo, and share code between the services with namespaced packages.
 The `build-project` command will collect the project-specific packages and build an installable artifact from it (i.e. a wheel or an sdist).
 
+### A basic building block for the Polylith Architecture
+The Multiproject plugin makes it possible to organize Python projects according to the Polylith Architecture.
+The plugin is the foundation for the __Python tools for the Polylith Architecture__ - also implemented as a __Poetry__ plugin.
+
+For more about Polylith, have a look at the [Python-specific Polylith documentation](https://davidvujic.github.io/python-polylith-docs/).
+
 ### Libraries?
 Building libraries is also supported, but you will need to consider that the code will likely share the same top namespace with other libraries 
 built from the same monorepo. It depends on your monorepo structure. This will likely be a problem when more than one of your libraries are installed into the same virtual environment.
 
 Since Python libraries by default are installed in a "flat" folder structure, two libraries with the same top namespace will collide.
 
 There is a way to solve this issue, by using the `--with-top-namespace` flag of the `build-project` command. See [usage for libraries](#usage-for-libraries).
@@ -174,28 +187,46 @@
     { include = "my_namespace/my_package", from = "../../shared" }
     { include = "my_namespace/my_other_package", from = "../../shared" }
 ]
 ```
 
 This plugin will allow relative package includes. You will now be able to share code between projects.
 
-An suggested Monorepo structure, with the shared code extracted into a separate folder structure:
+## Organizing code
+An example Monorepo structure, having the shared code extracted into a separate folder structure:
 
 ``` shell
 projects/
   my_app/
-    pyproject.toml (including a shared package)
+    pyproject.toml (including selected shared packages)
 
   my_service/
-    pyproject.toml (including other shared packages)
+    pyproject.toml (including selected shared packages)
 
 shared/
   my_namespace/
     my_package/
       __init__.py
       code.py
 
     my_other_package/
       __init__.py
       code.py
 ```
 
+A suggested structure, using [Polylith](https://davidvujic.github.io/python-polylith-docs/workspace/):
+
+``` shell
+workspace/
+  bases/
+  components/
+  development/
+  projects/
+
+  poetry.lock
+
+  pyproject.toml
+  workspace.toml
+
+  README.md
+```
+
```

