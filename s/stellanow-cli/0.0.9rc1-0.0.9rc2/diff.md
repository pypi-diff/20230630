# Comparing `tmp/stellanow_cli-0.0.9rc1.tar.gz` & `tmp/stellanow_cli-0.0.9rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stellanow_cli-0.0.9rc1.tar", last modified: Tue Jun 20 16:33:27 2023, max compression
+gzip compressed data, was "stellanow_cli-0.0.9rc2.tar", last modified: Thu Jun 29 23:25:56 2023, max compression
```

## Comparing `stellanow_cli-0.0.9rc1.tar` & `stellanow_cli-0.0.9rc2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-20 16:33:27.036129 stellanow_cli-0.0.9rc1/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       98 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/MANIFEST.in
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     8331 2023-06-20 16:33:27.034650 stellanow_cli-0.0.9rc1/PKG-INFO
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      225 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/Pipfile
--rw-r--r--   0 tom-kandziora   (501) staff       (20)    10889 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/README.md
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     8154 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/README.public
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-20 16:33:27.036224 stellanow_cli-0.0.9rc1/setup.cfg
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2284 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/setup.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-20 16:33:26.413545 stellanow_cli-0.0.9rc1/stellanow_cli/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1090 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/stellanow_cli/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-20 16:33:26.661262 stellanow_cli-0.0.9rc1/stellanow_cli/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1277 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1348 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/__pycache__/_run.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1307 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/__pycache__/_version.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2100 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/__pycache__/cli.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1173 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/stellanow_cli/_run.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1117 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/stellanow_cli/_version.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-20 16:33:26.669887 stellanow_cli-0.0.9rc1/stellanow_cli/api/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1213 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/stellanow_cli/api/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-20 16:33:26.697893 stellanow_cli-0.0.9rc1/stellanow_cli/api/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1453 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2272 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/api/__pycache__/datatypes.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     5626 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1536 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/stellanow_cli/api/datatypes.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     6572 2023-06-20 14:47:52.000000 stellanow_cli-0.0.9rc1/stellanow_cli/api/stellanow_api.py
--rwxr-xr-x   0 tom-kandziora   (501) staff       (20)     2058 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/stellanow_cli/cli.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-20 16:33:26.722904 stellanow_cli-0.0.9rc1/stellanow_cli/code_generators/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1146 2023-06-20 14:47:50.000000 stellanow_cli-0.0.9rc1/stellanow_cli/code_generators/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-20 16:33:26.777161 stellanow_cli-0.0.9rc1/stellanow_cli/code_generators/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1363 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2580 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     5898 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/code_generators/__pycache__/csharp_code_generator.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2226 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/stellanow_cli/code_generators/code_generator.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     6050 2023-06-20 14:47:51.000000 stellanow_cli-0.0.9rc1/stellanow_cli/code_generators/csharp_code_generator.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-20 16:33:26.793703 stellanow_cli-0.0.9rc1/stellanow_cli/code_generators/templates/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-10 10:14:46.000000 stellanow_cli-0.0.9rc1/stellanow_cli/code_generators/templates/.footer.template
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      126 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/stellanow_cli/code_generators/templates/.header.template
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      534 2023-06-18 12:11:51.000000 stellanow_cli-0.0.9rc1/stellanow_cli/code_generators/templates/csharp.template
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-20 16:33:26.826005 stellanow_cli-0.0.9rc1/stellanow_cli/commands/
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-20 16:33:26.899185 stellanow_cli-0.0.9rc1/stellanow_cli/commands/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     4532 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/commands/__pycache__/command_config.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3726 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2125 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/commands/__pycache__/events.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     5175 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/commands/__pycache__/generate.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     4595 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1090 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/stellanow_cli/commands/_init__.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     4928 2023-06-20 14:47:50.000000 stellanow_cli-0.0.9rc1/stellanow_cli/commands/command_config.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     4601 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/stellanow_cli/commands/configure.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1990 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/stellanow_cli/commands/events.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     5203 2023-06-20 14:47:52.000000 stellanow_cli-0.0.9rc1/stellanow_cli/commands/generate.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     5210 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/stellanow_cli/commands/plan.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-20 16:33:26.905471 stellanow_cli-0.0.9rc1/stellanow_cli/config/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1276 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/stellanow_cli/config/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-20 16:33:26.940487 stellanow_cli-0.0.9rc1/stellanow_cli/config/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1705 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2193 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/config/__pycache__/config.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1622 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/config/__pycache__/dev.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1618 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/config/__pycache__/int.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1612 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/stellanow_cli/config/config.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1246 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/stellanow_cli/config/dev.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1242 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/stellanow_cli/config/int.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-20 16:33:26.975563 stellanow_cli-0.0.9rc1/stellanow_cli/exceptions/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2208 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/stellanow_cli/exceptions/StellaNowAPIExceptions.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2163 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/stellanow_cli/exceptions/StellaNowCLIException.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1090 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/stellanow_cli/exceptions/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-20 16:33:26.989860 stellanow_cli-0.0.9rc1/stellanow_cli/exceptions/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3138 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/exceptions/__pycache__/StellaNowAPIExceptions.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3177 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/exceptions/__pycache__/StellaNowCLIException.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1288 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/exceptions/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-20 16:33:26.992390 stellanow_cli-0.0.9rc1/stellanow_cli/utils/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       88 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/stellanow_cli/utils/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-20 16:33:27.016464 stellanow_cli-0.0.9rc1/stellanow_cli/utils/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      310 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1693 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/utils/__pycache__/logger.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2626 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc1/stellanow_cli/utils/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1631 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/stellanow_cli/utils/logger.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1926 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/stellanow_cli/utils/utils.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-20 16:33:26.588972 stellanow_cli-0.0.9rc1/stellanow_cli.egg-info/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     8331 2023-06-20 16:33:25.000000 stellanow_cli-0.0.9rc1/stellanow_cli.egg-info/PKG-INFO
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2988 2023-06-20 16:33:26.000000 stellanow_cli-0.0.9rc1/stellanow_cli.egg-info/SOURCES.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)        1 2023-06-20 16:33:25.000000 stellanow_cli-0.0.9rc1/stellanow_cli.egg-info/dependency_links.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       52 2023-06-20 16:33:25.000000 stellanow_cli-0.0.9rc1/stellanow_cli.egg-info/entry_points.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       46 2023-06-20 16:33:25.000000 stellanow_cli-0.0.9rc1/stellanow_cli.egg-info/requires.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       14 2023-06-20 16:33:25.000000 stellanow_cli-0.0.9rc1/stellanow_cli.egg-info/top_level.txt
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-20 16:33:27.019101 stellanow_cli-0.0.9rc1/tests/
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-20 16:33:27.028697 stellanow_cli-0.0.9rc1/tests/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1837 2023-06-18 17:07:08.000000 stellanow_cli-0.0.9rc1/tests/__pycache__/test_generate_class_handles_all_valueTypes.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2853 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc1/tests/test_command_configure.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3313 2023-06-20 14:47:54.000000 stellanow_cli-0.0.9rc1/tests/test_generate_class_handles_all_valueTypes.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:56.356438 stellanow_cli-0.0.9rc2/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       98 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/MANIFEST.in
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     8331 2023-06-29 23:25:56.353947 stellanow_cli-0.0.9rc2/PKG-INFO
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      225 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/Pipfile
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)    10889 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/README.md
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     8154 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/README.public
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-29 23:25:56.356616 stellanow_cli-0.0.9rc2/setup.cfg
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2284 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/setup.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:55.847907 stellanow_cli-0.0.9rc2/stellanow_cli/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1090 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:55.920005 stellanow_cli-0.0.9rc2/stellanow_cli/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1277 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1348 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/__pycache__/_run.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1307 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/__pycache__/_version.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2100 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/__pycache__/cli.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1173 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/_run.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1117 2023-06-29 23:24:44.000000 stellanow_cli-0.0.9rc2/stellanow_cli/_version.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:55.940373 stellanow_cli-0.0.9rc2/stellanow_cli/api/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1231 2023-06-27 21:31:01.000000 stellanow_cli-0.0.9rc2/stellanow_cli/api/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:55.952749 stellanow_cli-0.0.9rc2/stellanow_cli/api/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1453 2023-06-29 22:10:25.000000 stellanow_cli-0.0.9rc2/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2272 2023-06-29 23:05:14.000000 stellanow_cli-0.0.9rc2/stellanow_cli/api/__pycache__/datatypes.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     5626 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1537 2023-06-29 22:49:17.000000 stellanow_cli-0.0.9rc2/stellanow_cli/api/datatypes.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     6572 2023-06-20 14:47:52.000000 stellanow_cli-0.0.9rc2/stellanow_cli/api/stellanow_api.py
+-rwxr-xr-x   0 tom-kandziora   (501) staff       (20)     2058 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/cli.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:55.966576 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1146 2023-06-20 14:47:50.000000 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:55.983944 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1363 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2580 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     7210 2023-06-29 23:24:22.000000 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/__pycache__/csharp_code_generator.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2226 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/code_generator.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     6687 2023-06-29 23:24:22.000000 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/csharp_code_generator.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:55.993435 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/templates/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-10 10:14:46.000000 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/templates/.footer.template
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      126 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/templates/.header.template
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      544 2023-06-29 23:22:51.000000 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/templates/csharp.template
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:56.097124 stellanow_cli-0.0.9rc2/stellanow_cli/commands/
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:56.113798 stellanow_cli-0.0.9rc2/stellanow_cli/commands/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4538 2023-06-27 15:44:57.000000 stellanow_cli-0.0.9rc2/stellanow_cli/commands/__pycache__/command_config.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3732 2023-06-27 15:44:40.000000 stellanow_cli-0.0.9rc2/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2125 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/commands/__pycache__/events.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     5175 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/commands/__pycache__/generate.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4595 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1090 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/commands/_init__.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4934 2023-06-27 15:44:51.000000 stellanow_cli-0.0.9rc2/stellanow_cli/commands/command_config.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4607 2023-06-27 15:44:32.000000 stellanow_cli-0.0.9rc2/stellanow_cli/commands/configure.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1990 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/commands/events.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     5203 2023-06-20 14:47:52.000000 stellanow_cli-0.0.9rc2/stellanow_cli/commands/generate.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     5210 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/commands/plan.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:56.192814 stellanow_cli-0.0.9rc2/stellanow_cli/config/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1276 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/config/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:56.220354 stellanow_cli-0.0.9rc2/stellanow_cli/config/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1705 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2193 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/config/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1622 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/config/__pycache__/dev.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1618 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/config/__pycache__/int.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1612 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/config/config.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1246 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/config/dev.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1242 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/config/int.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:56.250350 stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2208 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/StellaNowAPIExceptions.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2163 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/StellaNowCLIException.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1090 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:56.263467 stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3138 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/__pycache__/StellaNowAPIExceptions.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3177 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/__pycache__/StellaNowCLIException.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1288 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/__pycache__/__init__.cpython-310.pyc
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:56.298151 stellanow_cli-0.0.9rc2/stellanow_cli/utils/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1090 2023-06-27 14:25:32.000000 stellanow_cli-0.0.9rc2/stellanow_cli/utils/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:56.312616 stellanow_cli-0.0.9rc2/stellanow_cli/utils/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1283 2023-06-27 15:44:10.000000 stellanow_cli-0.0.9rc2/stellanow_cli/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1693 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/utils/__pycache__/logger.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2908 2023-06-27 15:44:40.000000 stellanow_cli-0.0.9rc2/stellanow_cli/utils/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1631 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/utils/logger.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2240 2023-06-27 14:21:56.000000 stellanow_cli-0.0.9rc2/stellanow_cli/utils/utils.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:55.908949 stellanow_cli-0.0.9rc2/stellanow_cli.egg-info/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     8331 2023-06-29 23:25:55.000000 stellanow_cli-0.0.9rc2/stellanow_cli.egg-info/PKG-INFO
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2988 2023-06-29 23:25:55.000000 stellanow_cli-0.0.9rc2/stellanow_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)        1 2023-06-29 23:25:55.000000 stellanow_cli-0.0.9rc2/stellanow_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       52 2023-06-29 23:25:55.000000 stellanow_cli-0.0.9rc2/stellanow_cli.egg-info/entry_points.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       46 2023-06-29 23:25:55.000000 stellanow_cli-0.0.9rc2/stellanow_cli.egg-info/requires.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       14 2023-06-29 23:25:55.000000 stellanow_cli-0.0.9rc2/stellanow_cli.egg-info/top_level.txt
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:56.329497 stellanow_cli-0.0.9rc2/tests/
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:56.350161 stellanow_cli-0.0.9rc2/tests/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1837 2023-06-18 17:07:08.000000 stellanow_cli-0.0.9rc2/tests/__pycache__/test_generate_class_handles_all_valueTypes.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2853 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/tests/test_command_configure.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3313 2023-06-20 14:47:54.000000 stellanow_cli-0.0.9rc2/tests/test_generate_class_handles_all_valueTypes.py
```

### Comparing `stellanow_cli-0.0.9rc1/PKG-INFO` & `stellanow_cli-0.0.9rc2/stellanow_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: stellanow_cli
-Version: 0.0.9rc1
+Name: stellanow-cli
+Version: 0.0.9rc2
 Summary: Command-line interface for the StellaNow SDK code generation and comparison tool.
 Requires-Python: >=3.10
 
 StellaNow CLI Tool
 ==================
 
 Welcome to the StellaNow CLI tool. This tool automates the process of generating class code from StellaNow event specifications and provides a summary of changes between the generated classes and the specifications fetched from the API. It's recommended to use this tool in conjunction with the StellaNow SDK's to ensure that your application's message classes are up-to-date with the latest specifications.
```

### Comparing `stellanow_cli-0.0.9rc1/README.md` & `stellanow_cli-0.0.9rc2/README.md`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/README.public` & `stellanow_cli-0.0.9rc2/README.public`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/setup.py` & `stellanow_cli-0.0.9rc2/setup.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/__init__.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/stellanow_cli/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/__pycache__/_run.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/stellanow_cli/__pycache__/_run.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/__pycache__/_version.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/stellanow_cli/__pycache__/_version.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/__pycache__/cli.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/stellanow_cli/__pycache__/cli.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/_run.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/_run.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/_version.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/_version.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 IN THE SOFTWARE.
 """
 
-__version__ = "0.0.9.rc1"
+__version__ = "0.0.9.rc2"
```

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/api/__init__.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/api/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,8 +17,13 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 IN THE SOFTWARE.
 """
 
 from .stellanow_api import StellaAPI
-from .datatypes import (StellaEvent, StellaEntity, StellaField, StellaEventDetailed)
+from .datatypes import (
+    StellaEvent,
+    StellaEntity,
+    StellaField,
+    StellaEventDetailed
+)
```

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 20 14:47:41 2023 UTC, .py size: 1213 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0dbc 9164 bd04 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 1555 9b64 cf04 0000  o........U.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6404 5300 2905 613b 0400  m.Z...d.S.).a;..
 00000060: 000a 436f 7079 7269 6768 7420 2843 2920  ..Copyright (C) 
 00000070: 3230 3232 2d32 3032 3320 5374 656c 6c61  2022-2023 Stella
```

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/api/__pycache__/datatypes.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/stellanow_cli/api/__pycache__/datatypes.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 20 14:47:41 2023 UTC, .py size: 1536 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0dbc 9164 0006 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 6d0a 9e64 0106 0000  o.......m..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6502 4700 6404  d.l.m.Z...e.G.d.
 00000050: 6405 8400 6405 8302 8301 5a05 6502 4700  d...d.....Z.e.G.
 00000060: 6406 6407 8400 6407 8302 8301 5a06 6502  d.d...d.....Z.e.
 00000070: 4700 6408 6409 8400 6409 8302 8301 5a07  G.d.d...d.....Z.
@@ -96,15 +96,15 @@
 000005f0: 7204 0000 001b 0000 0073 0600 0000 0a00  r........s......
 00000600: 0802 0c01 7204 0000 0063 0000 0000 0000  ....r....c......
 00000610: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
 00000620: 0000 7326 0000 0065 005a 0164 005a 0255  ..s&...e.Z.d.Z.U
 00000630: 0065 0365 0464 013c 0065 0365 0464 023c  .e.e.d.<.e.e.d.<
 00000640: 0065 0365 0464 033c 0064 0453 0029 05da  .e.e.d.<.d.S.)..
 00000650: 0b53 7465 6c6c 6146 6965 6c64 7205 0000  .StellaFieldr...
-00000660: 0072 0600 0000 5a09 7661 6c75 6554 7970  .r....Z.valueTyp
+00000660: 0072 0600 0000 da09 7661 6c75 6554 7970  .r......valueTyp
 00000670: 654e 7207 0000 0072 0d00 0000 720d 0000  eNr....r....r...
 00000680: 0072 0d00 0000 720e 0000 0072 0f00 0000  .r....r....r....
 00000690: 2100 0000 7308 0000 000a 0008 0208 010c  !...s...........
 000006a0: 0172 0f00 0000 6300 0000 0000 0000 0000  .r....c.........
 000006b0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
 000006c0: 3600 0000 6500 5a01 6400 5a02 5500 6503  6...e.Z.d.Z.U.e.
 000006d0: 6504 6401 3c00 6503 6504 6402 3c00 6505  e.d.<.e.e.d.<.e.
@@ -112,31 +112,31 @@
 000006f0: 6504 6405 3c00 6406 5300 2907 da0b 5374  e.d.<.d.S.)...St
 00000700: 656c 6c61 4576 656e 7472 0500 0000 7206  ellaEventr....r.
 00000710: 0000 00da 0869 7341 6374 6976 65da 0963  .....isActive..c
 00000720: 7265 6174 6564 4174 da09 7570 6461 7465  reatedAt..update
 00000730: 6441 744e 2906 7208 0000 0072 0900 0000  dAtN).r....r....
 00000740: 720a 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
 00000750: 0462 6f6f 6c72 0d00 0000 720d 0000 0072  .boolr....r....r
-00000760: 0d00 0000 720e 0000 0072 1000 0000 2800  ....r....r....(.
+00000760: 0d00 0000 720e 0000 0072 1100 0000 2800  ....r....r....(.
 00000770: 0000 730c 0000 000a 0008 0208 0108 0108  ..s.............
-00000780: 010c 0172 1000 0000 6300 0000 0000 0000  ...r....c.......
+00000780: 010c 0172 1100 0000 6300 0000 0000 0000  ...r....c.......
 00000790: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
 000007a0: 0073 2e00 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
 000007b0: 6503 6504 6401 3c00 6505 6506 1900 6504  e.e.d.<.e.e...e.
 000007c0: 6402 3c00 6505 6507 1900 6504 6403 3c00  d.<.e.e...e.d.<.
 000007d0: 6404 5300 2905 da13 5374 656c 6c61 4576  d.S.)...StellaEv
 000007e0: 656e 7444 6574 6169 6c65 64da 0b64 6573  entDetailed..des
 000007f0: 6372 6970 7469 6f6e da06 6669 656c 6473  cription..fields
 00000800: da08 656e 7469 7469 6573 4e29 0872 0800  ..entitiesN).r..
 00000810: 0000 7209 0000 0072 0a00 0000 720b 0000  ..r....r....r...
 00000820: 0072 0c00 0000 7203 0000 0072 0f00 0000  .r....r....r....
 00000830: 7204 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
-00000840: 0d00 0000 720e 0000 0072 1500 0000 3100  ....r....r....1.
+00000840: 0d00 0000 720e 0000 0072 1600 0000 3100  ....r....r....1.
 00000850: 0000 7308 0000 000a 0008 020c 0110 0172  ..s............r
-00000860: 1500 0000 4e29 09da 075f 5f64 6f63 5f5f  ....N)...__doc__
+00000860: 1600 0000 4e29 09da 075f 5f64 6f63 5f5f  ....N)...__doc__
 00000870: da0b 6461 7461 636c 6173 7365 7372 0200  ..dataclassesr..
 00000880: 0000 da06 7479 7069 6e67 7203 0000 0072  ....typingr....r
-00000890: 0400 0000 720f 0000 0072 1000 0000 7215  ....r....r....r.
+00000890: 0400 0000 720f 0000 0072 1100 0000 7216  ....r....r....r.
 000008a0: 0000 0072 0d00 0000 720d 0000 0072 0d00  ...r....r....r..
 000008b0: 0000 720e 0000 00da 083c 6d6f 6475 6c65  ..r......<module
 000008c0: 3e01 0000 0073 1600 0000 0400 0c16 0c01  >....s..........
 000008d0: 0203 1001 0205 1001 0206 1001 0208 1601  ................
```

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/api/datatypes.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/api/datatypes.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -46,8 +46,8 @@
     updatedAt: str
 
 
 @dataclass
 class StellaEventDetailed(StellaEvent):
     description: str
     fields: List[StellaField]
-    entities: List[StellaEntity]
+    entities: List[StellaEntity]
```

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/api/stellanow_api.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/api/stellanow_api.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/cli.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/cli.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/code_generators/__init__.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/__init__.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/code_generators/code_generator.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/code_generator.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/code_generators/csharp_code_generator.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/csharp_code_generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,25 +21,25 @@
 """
 
 import difflib
 import json
 import logging
 import re
 
-from dataclasses import asdict
+from dataclasses import asdict, dataclass
 from datetime import datetime
 from typing import Iterator
 
-from ..api import StellaEventDetailed
+from ..api import StellaEventDetailed, StellaField, StellaEntity
 from .code_generator import CodeGenerator
 from ..exceptions.StellaNowCLIException import (
     StellaNowCLINamespaceNotFoundException,
     StellaNowCLINoEntityAssociatedWithEventException
 )
-from ..utils import snake_to_camel, snake_to_lower_camel, remove_comments
+from ..utils.utils import snake_to_camel, snake_to_lower_camel, remove_comments
 
 
 logger = logging.getLogger(__name__)
 
 
 def field_type_mapping(value_type: str) -> str:
     mapping = {
@@ -77,55 +77,78 @@
         "true", "try", "typeof", "uint", "ulong", "unchecked", "unsafe", "ushort", "using", "virtual",
         "void", "volatile", "while"
     ]
 
     return word + "_" if word in reserved_words else word
 
 
+@dataclass
+class CSharpField:
+    original_name: str
+    csharp_name: str
+    type: str
+    format: str
+
+    @classmethod
+    def from_stella_field(cls, field: StellaField):
+        return cls(
+            original_name=field.name,
+            csharp_name=escape_reserved_words(snake_to_lower_camel(field.name)),
+            type=field_type_mapping(field.valueType),
+            format=field_format_mapping(field.valueType)
+        )
+
+    def to_constructor_parameter_declaration(self):
+        return f'{self.type} {self.csharp_name}'
+
+
+@dataclass
+class CSharpEntity:
+    original_name: str
+    csharp_name: str
+
+    @classmethod
+    def from_stella_field(cls, entity: StellaEntity):
+        return cls(
+            original_name=entity.name,
+            csharp_name=escape_reserved_words(snake_to_lower_camel(entity.name)) + "Id",
+        )
+
+    def to_entity_type_declaration(self):
+        return f'new EntityType("{self.original_name}", {self.csharp_name})'
+
+    def to_constructor_parameter_declaration(self):
+        return f'string {self.csharp_name}'
+
+
 class CsharpCodeGenerator(CodeGenerator):
     @staticmethod
     def generate_class(event: StellaEventDetailed, **kwargs) -> str:
         template = CsharpCodeGenerator.load_template('csharp')
 
         namespace = kwargs.get('namespace', 'StellaNowSDK.Messages')
 
-        constructor_arguments = ', '.join([
-            ', '.join([
-                f'string {escape_reserved_words(snake_to_lower_camel(entity.name))}Id'
-                for entity in event.entities
-            ]),
-            ', '.join([
-                f'{field_type_mapping(field.valueType)} {escape_reserved_words(snake_to_lower_camel(field.name))}'
-                for field in event.fields
-            ])
-        ])
-        entities_list = ', '.join([f'new EntityType("{entity.name}", {entity.name}Id)' for entity in event.entities])
-
-        if not entities_list:
+        fields = [CSharpField.from_stella_field(field) for field in event.fields]
+        entities = [CSharpEntity.from_stella_field(entity) for entity in event.entities]
+        if not entities:
             raise StellaNowCLINoEntityAssociatedWithEventException()
 
-        event_json = json.dumps(asdict(event), indent=4)
-
-        timestamp = datetime.utcnow().strftime("%Y-%m-%dT%H:%M:%SZ")
-
         rendered = template.render(
             className=snake_to_camel(event.name),
             eventName=event.name,
-            constructorArguments=constructor_arguments,
-            entitiesList=entities_list,
-            fields=[{
-                'name': field.name,
-                'camel_name': escape_reserved_words(snake_to_lower_camel(field.name)),
-                'type': field_type_mapping(field.valueType),
-                'format': field_format_mapping(field.valueType)
-            } for field in event.fields],
+            constructorArguments=', '.join([
+                ', '.join([entity.to_constructor_parameter_declaration() for entity in entities]),
+                ', '.join([field.to_constructor_parameter_declaration() for field in fields])
+            ]),
+            entitiesList=', '.join([entity.to_entity_type_declaration() for entity in entities]),
+            fields=fields,
             namespace=namespace,
-            eventJson=event_json,
+            eventJson=json.dumps(asdict(event), indent=4),
             eventId=event.id,
-            timestamp=timestamp
+            timestamp=datetime.utcnow().strftime("%Y-%m-%dT%H:%M:%SZ")
         )
 
         return rendered
 
     @staticmethod
     def get_file_name_for_event_name(event_name: str) -> str:
         return f"{snake_to_camel(event_name)}Message.cs"
```

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/code_generators/templates/csharp.template` & `stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/templates/csharp.template`

 * *Files 17% similar despite different names*

```diff
@@ -9,13 +9,13 @@
 {
     public {{ className }}Message({{ constructorArguments }})
         : base(
             "{{ eventName }}",
             new List<EntityType>{ {{ entitiesList }} })
     {
         {%- for field in fields %}
-        AddField("{{ field.name }}", {{ field.camel_name }}{{ field.format }});
+        AddField("{{ field.original_name }}", {{ field.csharp_name }}{{ field.format }});
         {%- endfor %}
     }
 }
 
 {% include '.footer.template' %}
```

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/commands/__pycache__/command_config.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/stellanow_cli/commands/__pycache__/command_config.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 20 14:47:50 2023 UTC, .py size: 4928 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 16bc 9164 4013 0000  o..........d@...
+00000000: 6f0d 0d0a 0000 0000 f303 9b64 4613 0000  o..........dF...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6403 6404 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 0100 6403 6405 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 0100 6403 6406 6c0a 6d0b 5a0b 0100 6403  ..d.d.l.m.Z...d.
@@ -270,15 +270,15 @@
 000010d0: 0000 0008 010e 0104 2e72 4200 0000 2915  .........rB...).
 000010e0: da07 5f5f 646f 635f 5f72 3600 0000 7217  ..__doc__r6...r.
 000010f0: 0000 0072 4000 0000 da07 6c6f 6767 696e  ...r@.....loggin
 00001100: 6772 2d00 0000 da03 6170 6972 0300 0000  gr-.....apir....
 00001110: 5a0a 636f 6e66 6967 2e69 6e74 7204 0000  Z.config.intr...
 00001120: 00da 0663 6f6e 6669 6772 0500 0000 5a0c  ...configr....Z.
 00001130: 7574 696c 732e 6c6f 6767 6572 7206 0000  utils.loggerr...
-00001140: 00da 0575 7469 6c73 7207 0000 00da 0967  ...utilsr......g
-00001150: 6574 4c6f 6767 6572 da08 5f5f 6e61 6d65  etLogger..__name
-00001160: 5f5f 7232 0000 0072 1e00 0000 7242 0000  __r2...r....rB..
-00001170: 0072 0c00 0000 720c 0000 0072 0c00 0000  .r....r....r....
-00001180: 7210 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00001190: 0000 0073 1c00 0000 0400 0816 0801 0801  ...s............
-000011a0: 0801 0801 0c02 0c01 0c01 0c01 0c01 0a03  ................
-000011b0: 0803 0c1e                                ....
+00001140: 005a 0b75 7469 6c73 2e75 7469 6c73 7207  .Z.utils.utilsr.
+00001150: 0000 00da 0967 6574 4c6f 6767 6572 da08  .....getLogger..
+00001160: 5f5f 6e61 6d65 5f5f 7232 0000 0072 1e00  __name__r2...r..
+00001170: 0000 7242 0000 0072 0c00 0000 720c 0000  ..rB...r....r...
+00001180: 0072 0c00 0000 7210 0000 00da 083c 6d6f  .r....r......<mo
+00001190: 6475 6c65 3e01 0000 0073 1c00 0000 0400  dule>....s......
+000011a0: 0816 0801 0801 0801 0801 0c02 0c01 0c01  ................
+000011b0: 0c01 0c01 0a03 0803 0c1e                 ..........
```

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 20 14:47:41 2023 UTC, .py size: 4601 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0dbc 9164 f911 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 e003 9b64 ff11 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6403 6404 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 0100 6403 6405 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 0100 6503 a00a 650b a101 5a0c 6501 6a0d  ..e...e...Z.e.j.
@@ -215,19 +215,20 @@
 00000d60: 0201 0e01 1801 0201 0a02 02fb 0208 1201  ................
 00000d70: 0c01 0201 0a02 02fb 0207 0e01 0801 0201  ................
 00000d80: 0a02 02fb 0207 0e01 0801 0201 0a02 02fb  ................
 00000d90: 0c08 1803 0803 1003 0c01 0a01 0204 0201  ................
 00000da0: 0201 0201 0afc 0808 0c01 0c03 0c01 1cff  ................
 00000db0: 1403 2913 da07 5f5f 646f 635f 5f72 2200  ..)...__doc__r".
 00000dc0: 0000 722c 0000 005a 076c 6f67 6769 6e67  ..r,...Z.logging
-00000dd0: 7227 0000 0072 2300 0000 da05 7574 696c  r'...r#.....util
-00000de0: 7372 0300 0000 7233 0000 0072 0400 0000  sr....r3...r....
-00000df0: 5a09 6765 744c 6f67 6765 72da 085f 5f6e  Z.getLogger..__n
-00000e00: 616d 655f 5f72 2500 0000 da07 636f 6d6d  ame__r%.....comm
-00000e10: 616e 64da 066f 7074 696f 6eda 0643 686f  and..option..Cho
-00000e20: 6963 65da 0c70 6173 735f 636f 6e74 6578  ice..pass_contex
-00000e30: 7472 0500 0000 da0d 636f 6e66 6967 7572  tr......configur
-00000e40: 655f 636d 6472 0b00 0000 720b 0000 0072  e_cmdr....r....r
-00000e50: 0b00 0000 720f 0000 00da 083c 6d6f 6475  ....r......<modu
-00000e60: 6c65 3e01 0000 0073 2200 0000 0400 0816  le>....s".......
-00000e70: 0801 0801 0801 0801 0c02 0c01 0a02 0a03  ................
-00000e80: 0a01 0201 04ff 2203 0401 1001 084d       ......"......M
+00000dd0: 7227 0000 0072 2300 0000 5a0b 7574 696c  r'...r#...Z.util
+00000de0: 732e 7574 696c 7372 0300 0000 7233 0000  s.utilsr....r3..
+00000df0: 0072 0400 0000 5a09 6765 744c 6f67 6765  .r....Z.getLogge
+00000e00: 72da 085f 5f6e 616d 655f 5f72 2500 0000  r..__name__r%...
+00000e10: da07 636f 6d6d 616e 64da 066f 7074 696f  ..command..optio
+00000e20: 6eda 0643 686f 6963 65da 0c70 6173 735f  n..Choice..pass_
+00000e30: 636f 6e74 6578 7472 0500 0000 da0d 636f  contextr......co
+00000e40: 6e66 6967 7572 655f 636d 6472 0b00 0000  nfigure_cmdr....
+00000e50: 720b 0000 0072 0b00 0000 720f 0000 00da  r....r....r.....
+00000e60: 083c 6d6f 6475 6c65 3e01 0000 0073 2200  .<module>....s".
+00000e70: 0000 0400 0816 0801 0801 0801 0801 0c02  ................
+00000e80: 0c01 0a02 0a03 0a01 0201 04ff 2203 0401  ............"...
+00000e90: 1001 084d                                ...M
```

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/commands/__pycache__/events.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/stellanow_cli/commands/__pycache__/events.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/commands/__pycache__/generate.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/stellanow_cli/commands/__pycache__/generate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/commands/_init__.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/commands/_init__.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/commands/command_config.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/commands/command_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import logging
 import os
 
 from ..api import StellaAPI
 from ..config.int import ConfigInt
 from ..config import Env
 from ..utils.logger import setup_logger
-from ..utils import snake_to_camel
+from ..utils.utils import snake_to_camel
 
 
 logger = logging.getLogger(__name__)
 
 
 def common_option(f):
     """
```

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/commands/configure.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/commands/configure.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 import click
 import configparser
 import logging
 import os
 import re
 
-from ..utils import is_valid_uuid
+from ..utils.utils import is_valid_uuid
 from ..config import Env
 
 logger = logging.getLogger(__name__)
 
 
 @click.command(name='configure')
 @click.option('--profile', default='DEFAULT', prompt=False,
```

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/commands/events.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/commands/events.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/commands/generate.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/commands/plan.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/commands/plan.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/config/__init__.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/config/__pycache__/config.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/stellanow_cli/config/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/config/__pycache__/dev.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/stellanow_cli/config/__pycache__/dev.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/config/__pycache__/int.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/stellanow_cli/config/__pycache__/int.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/config/config.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/config/config.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/config/dev.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/config/dev.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/config/int.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/config/int.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/exceptions/StellaNowAPIExceptions.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/StellaNowAPIExceptions.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/exceptions/StellaNowCLIException.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/StellaNowCLIException.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/exceptions/__init__.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/exceptions/__pycache__/StellaNowAPIExceptions.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/__pycache__/StellaNowAPIExceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/exceptions/__pycache__/StellaNowCLIException.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/__pycache__/StellaNowCLIException.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/exceptions/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/utils/__pycache__/logger.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/stellanow_cli/utils/__pycache__/logger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/utils/__pycache__/utils.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/stellanow_cli/utils/__pycache__/utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 20 14:47:41 2023 UTC, .py size: 1926 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,165 +1,182 @@
-00000000: 6f0d 0d0a 0000 0000 0dbc 9164 8607 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 84f0 9a64 c008 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
+00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
-00000040: 5a02 6403 6404 8400 5a03 6405 6406 8400  Z.d.d...Z.d.d...
-00000050: 5a04 6407 6505 6408 6505 6604 6409 640a  Z.d.e.d.e.f.d.d.
-00000060: 8404 5a06 640e 640c 640d 8401 5a07 6402  ..Z.d.d.d...Z.d.
-00000070: 5300 290f 613b 0400 000a 436f 7079 7269  S.).a;....Copyri
-00000080: 6768 7420 2843 2920 3230 3232 2d32 3032  ght (C) 2022-202
-00000090: 3320 5374 656c 6c61 2054 6563 686e 6f6c  3 Stella Technol
-000000a0: 6f67 6965 7320 2855 4b29 204c 696d 6974  ogies (UK) Limit
-000000b0: 6564 2e0a 0a50 6572 6d69 7373 696f 6e20  ed...Permission 
-000000c0: 6973 2068 6572 6562 7920 6772 616e 7465  is hereby grante
-000000d0: 642c 2066 7265 6520 6f66 2063 6861 7267  d, free of charg
-000000e0: 652c 2074 6f20 616e 7920 7065 7273 6f6e  e, to any person
-000000f0: 206f 6274 6169 6e69 6e67 2061 2063 6f70   obtaining a cop
-00000100: 790a 6f66 2074 6869 7320 736f 6674 7761  y.of this softwa
-00000110: 7265 2061 6e64 2061 7373 6f63 6961 7465  re and associate
-00000120: 6420 646f 6375 6d65 6e74 6174 696f 6e20  d documentation 
-00000130: 6669 6c65 7320 2874 6865 2022 536f 6674  files (the "Soft
-00000140: 7761 7265 2229 2c20 746f 2064 6561 6c0a  ware"), to deal.
-00000150: 696e 2074 6865 2053 6f66 7477 6172 6520  in the Software 
-00000160: 7769 7468 6f75 7420 7265 7374 7269 6374  without restrict
-00000170: 696f 6e2c 2069 6e63 6c75 6469 6e67 2077  ion, including w
-00000180: 6974 686f 7574 206c 696d 6974 6174 696f  ithout limitatio
-00000190: 6e20 7468 6520 7269 6768 7473 0a74 6f20  n the rights.to 
-000001a0: 7573 652c 2063 6f70 792c 206d 6f64 6966  use, copy, modif
-000001b0: 792c 206d 6572 6765 2c20 7075 626c 6973  y, merge, publis
-000001c0: 682c 2064 6973 7472 6962 7574 652c 2073  h, distribute, s
-000001d0: 7562 6c69 6365 6e73 652c 2061 6e64 2f6f  ublicense, and/o
-000001e0: 7220 7365 6c6c 0a63 6f70 6965 7320 6f66  r sell.copies of
-000001f0: 2074 6865 2053 6f66 7477 6172 652c 2061   the Software, a
-00000200: 6e64 2074 6f20 7065 726d 6974 2070 6572  nd to permit per
-00000210: 736f 6e73 2074 6f20 7768 6f6d 2074 6865  sons to whom the
-00000220: 2053 6f66 7477 6172 6520 6973 0a66 7572   Software is.fur
-00000230: 6e69 7368 6564 2074 6f20 646f 2073 6f2c  nished to do so,
-00000240: 2073 7562 6a65 6374 2074 6f20 7468 6520   subject to the 
-00000250: 666f 6c6c 6f77 696e 6720 636f 6e64 6974  following condit
-00000260: 696f 6e73 3a0a 0a54 6865 2061 626f 7665  ions:..The above
-00000270: 2063 6f70 7972 6967 6874 206e 6f74 6963   copyright notic
-00000280: 6520 616e 6420 7468 6973 2070 6572 6d69  e and this permi
-00000290: 7373 696f 6e20 6e6f 7469 6365 2073 6861  ssion notice sha
-000002a0: 6c6c 2062 6520 696e 636c 7564 6564 2069  ll be included i
-000002b0: 6e0a 616c 6c20 636f 7069 6573 206f 7220  n.all copies or 
-000002c0: 7375 6273 7461 6e74 6961 6c20 706f 7274  substantial port
-000002d0: 696f 6e73 206f 6620 7468 6520 536f 6674  ions of the Soft
-000002e0: 7761 7265 2e0a 0a54 4845 2053 4f46 5457  ware...THE SOFTW
-000002f0: 4152 4520 4953 2050 524f 5649 4445 4420  ARE IS PROVIDED 
-00000300: 2241 5320 4953 222c 2057 4954 484f 5554  "AS IS", WITHOUT
-00000310: 2057 4152 5241 4e54 5920 4f46 2041 4e59   WARRANTY OF ANY
-00000320: 204b 494e 442c 2045 5850 5245 5353 204f   KIND, EXPRESS O
-00000330: 520a 494d 504c 4945 442c 2049 4e43 4c55  R.IMPLIED, INCLU
-00000340: 4449 4e47 2042 5554 204e 4f54 204c 494d  DING BUT NOT LIM
-00000350: 4954 4544 2054 4f20 5448 4520 5741 5252  ITED TO THE WARR
-00000360: 414e 5449 4553 204f 4620 4d45 5243 4841  ANTIES OF MERCHA
-00000370: 4e54 4142 494c 4954 592c 0a46 4954 4e45  NTABILITY,.FITNE
-00000380: 5353 2046 4f52 2041 2050 4152 5449 4355  SS FOR A PARTICU
-00000390: 4c41 5220 5055 5250 4f53 4520 414e 4420  LAR PURPOSE AND 
-000003a0: 4e4f 4e49 4e46 5249 4e47 454d 454e 542e  NONINFRINGEMENT.
-000003b0: 2049 4e20 4e4f 2045 5645 4e54 2053 4841   IN NO EVENT SHA
-000003c0: 4c4c 2054 4845 0a41 5554 484f 5253 204f  LL THE.AUTHORS O
-000003d0: 5220 434f 5059 5249 4748 5420 484f 4c44  R COPYRIGHT HOLD
-000003e0: 4552 5320 4245 204c 4941 424c 4520 464f  ERS BE LIABLE FO
-000003f0: 5220 414e 5920 434c 4149 4d2c 2044 414d  R ANY CLAIM, DAM
-00000400: 4147 4553 204f 5220 4f54 4845 520a 4c49  AGES OR OTHER.LI
-00000410: 4142 494c 4954 592c 2057 4845 5448 4552  ABILITY, WHETHER
-00000420: 2049 4e20 414e 2041 4354 494f 4e20 4f46   IN AN ACTION OF
-00000430: 2043 4f4e 5452 4143 542c 2054 4f52 5420   CONTRACT, TORT 
-00000440: 4f52 204f 5448 4552 5749 5345 2c20 4152  OR OTHERWISE, AR
-00000450: 4953 494e 470a 4652 4f4d 2c20 4f55 5420  ISING.FROM, OUT 
-00000460: 4f46 204f 5220 494e 2043 4f4e 4e45 4354  OF OR IN CONNECT
-00000470: 494f 4e20 5749 5448 2054 4845 2053 4f46  ION WITH THE SOF
-00000480: 5457 4152 4520 4f52 2054 4845 2055 5345  TWARE OR THE USE
-00000490: 204f 5220 4f54 4845 5220 4445 414c 494e   OR OTHER DEALIN
-000004a0: 4753 0a49 4e20 5448 4520 534f 4654 5741  GS.IN THE SOFTWA
-000004b0: 5245 2e0a e900 0000 004e 6301 0000 0000  RE.......Nc.....
-000004c0: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
-000004d0: 0000 0073 1e00 0000 7c00 a000 6401 a101  ...s....|...d...
-000004e0: 7d01 6402 a001 6403 6404 8400 7c01 4400  }.d...d.d...|.D.
-000004f0: 8301 a101 5300 2905 4eda 015f da00 6301  ....S.).N.._..c.
-00000500: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00000510: 0000 0073 0000 00f3 1800 0000 8100 7c00  ...s..........|.
-00000520: 5d07 7d01 7c01 a000 a100 5600 0100 7102  ].}.|.....V...q.
-00000530: 6400 5300 a901 4ea9 01da 0574 6974 6c65  d.S...N....title
-00000540: a902 da02 2e30 da01 78a9 0072 0b00 0000  .....0..x..r....
-00000550: fa59 2f55 7365 7273 2f74 6f6d 2d6b 616e  .Y/Users/tom-kan
-00000560: 647a 696f 7261 2f44 6576 4c6f 6361 6c2f  dziora/DevLocal/
-00000570: 7374 656c 6c61 2f73 7465 6c6c 612d 6e6f  stella/stella-no
-00000580: 772f 5374 656c 6c61 4e6f 7743 4c49 2f73  w/StellaNowCLI/s
-00000590: 7465 6c6c 616e 6f77 5f63 6c69 2f75 7469  tellanow_cli/uti
-000005a0: 6c73 2f75 7469 6c73 2e70 79da 093c 6765  ls/utils.py..<ge
-000005b0: 6e65 7870 723e 1d00 0000 f304 0000 0002  nexpr>..........
-000005c0: 8016 007a 2173 6e61 6b65 5f74 6f5f 6361  ...z!snake_to_ca
-000005d0: 6d65 6c2e 3c6c 6f63 616c 733e 2e3c 6765  mel.<locals>.<ge
-000005e0: 6e65 7870 723e a902 da05 7370 6c69 74da  nexpr>....split.
-000005f0: 046a 6f69 6e29 025a 0973 6e61 6b65 5f73  .join).Z.snake_s
-00000600: 7472 da0a 636f 6d70 6f6e 656e 7473 720b  tr..componentsr.
-00000610: 0000 0072 0b00 0000 720c 0000 00da 0e73  ...r....r......s
-00000620: 6e61 6b65 5f74 6f5f 6361 6d65 6c1b 0000  nake_to_camel...
-00000630: 0073 0400 0000 0a01 1401 7213 0000 0063  .s........r....c
-00000640: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000650: 0700 0000 4300 0000 732e 0000 007c 00a0  ....C...s....|..
-00000660: 0064 01a1 017d 017c 0164 0219 0064 03a0  .d...}.|.d...d..
-00000670: 0164 0464 0584 007c 0164 0664 0085 0219  .d.d...|.d.d....
-00000680: 0044 0083 01a1 0117 0053 0029 074e 7202  .D.......S.).Nr.
-00000690: 0000 0072 0100 0000 7203 0000 0063 0100  ...r....r....c..
-000006a0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-000006b0: 0000 7300 0000 7204 0000 0072 0500 0000  ..s...r....r....
-000006c0: 7206 0000 0072 0800 0000 720b 0000 0072  r....r....r....r
-000006d0: 0b00 0000 720c 0000 0072 0d00 0000 2200  ....r....r....".
-000006e0: 0000 720e 0000 007a 2773 6e61 6b65 5f74  ..r....z'snake_t
-000006f0: 6f5f 6c6f 7765 725f 6361 6d65 6c2e 3c6c  o_lower_camel.<l
-00000700: 6f63 616c 733e 2e3c 6765 6e65 7870 723e  ocals>.<genexpr>
-00000710: e901 0000 0072 0f00 0000 2902 da01 7372  .....r....)...sr
-00000720: 1200 0000 720b 0000 0072 0b00 0000 720c  ....r....r....r.
-00000730: 0000 00da 1473 6e61 6b65 5f74 6f5f 6c6f  .....snake_to_lo
-00000740: 7765 725f 6361 6d65 6c20 0000 0073 0400  wer_camel ...s..
-00000750: 0000 0a01 2401 7216 0000 00da 0463 6f64  ....$.r......cod
-00000760: 65da 0672 6574 7572 6e63 0100 0000 0000  e..returnc......
-00000770: 0000 0000 0000 0100 0000 0600 0000 4300  ..............C.
-00000780: 0000 7314 0000 0074 006a 0164 0164 027c  ..s....t.j.d.d.|
-00000790: 0074 006a 0264 038d 0453 0029 044e 7a09  .t.j.d...S.).Nz.
-000007a0: 2f5c 2a2e 2a3f 5c2a 2f72 0300 0000 2901  /\*.*?\*/r....).
-000007b0: da05 666c 6167 7329 03da 0272 65da 0373  ..flags)...re..s
-000007c0: 7562 da06 444f 5441 4c4c 2901 7217 0000  ub..DOTALL).r...
-000007d0: 0072 0b00 0000 720b 0000 0072 0c00 0000  .r....r....r....
-000007e0: da0f 7265 6d6f 7665 5f63 6f6d 6d65 6e74  ..remove_comment
-000007f0: 7325 0000 0073 0200 0000 1401 721d 0000  s%...s......r...
-00000800: 00e9 0400 0000 6302 0000 0000 0000 0000  ......c.........
-00000810: 0000 0003 0000 0008 0000 0043 0000 0073  ...........C...s
-00000820: 3400 0000 7a09 7400 6a01 7c00 7c01 6401  4...z.t.j.|.|.d.
-00000830: 8d02 7d02 5700 6e0a 0400 7402 7913 0100  ..}.W.n...t.y...
-00000840: 0100 0100 5900 6402 5300 7700 7403 7c02  ....Y.d.S.w.t.|.
-00000850: 8301 7c00 6b02 5300 2903 7afa 0a20 2020  ..|.k.S.).z..   
-00000860: 2043 6865 636b 2069 6620 7575 6964 5f74   Check if uuid_t
-00000870: 6f5f 7465 7374 2069 7320 6120 7661 6c69  o_test is a vali
-00000880: 6420 5555 4944 2e0a 0a20 2020 2050 6172  d UUID...    Par
-00000890: 616d 6574 6572 733a 0a20 2020 202a 2075  ameters:.    * u
-000008a0: 7569 645f 746f 5f74 6573 743a 2073 7472  uid_to_test: str
-000008b0: 202d 2054 6865 2073 7472 696e 6720 746f   - The string to
-000008c0: 2074 6573 7420 6173 2061 2055 5549 442e   test as a UUID.
-000008d0: 0a20 2020 202a 2076 6572 7369 6f6e 3a20  .    * version: 
-000008e0: 696e 7420 2d20 5555 4944 2076 6572 7369  int - UUID versi
-000008f0: 6f6e 2028 6465 6661 756c 7420 6973 2034  on (default is 4
-00000900: 292e 0a0a 2020 2020 5265 7475 726e 733a  )...    Returns:
-00000910: 0a20 2020 202a 2060 5472 7565 6020 6966  .    * `True` if
-00000920: 2075 7569 645f 746f 5f74 6573 7420 6973   uuid_to_test is
-00000930: 2061 2076 616c 6964 2055 5549 443b 206f   a valid UUID; o
-00000940: 7468 6572 7769 7365 2060 4661 6c73 6560  therwise `False`
-00000950: 2e0a 2020 2020 2901 da07 7665 7273 696f  ..    )...versio
-00000960: 6e46 2904 da04 7575 6964 da04 5555 4944  nF)...uuid..UUID
-00000970: da0a 5661 6c75 6545 7272 6f72 da03 7374  ..ValueError..st
-00000980: 7229 035a 0c75 7569 645f 746f 5f74 6573  r).Z.uuid_to_tes
-00000990: 7472 1f00 0000 5a08 7575 6964 5f6f 626a  tr....Z.uuid_obj
-000009a0: 720b 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
-000009b0: 0d69 735f 7661 6c69 645f 7575 6964 2900  .is_valid_uuid).
-000009c0: 0000 730c 0000 0002 0b12 010c 0106 0102  ..s.............
-000009d0: ff0c 0272 2400 0000 2901 721e 0000 0029  ...r$...).r....)
-000009e0: 08da 075f 5f64 6f63 5f5f 721a 0000 0072  ...__doc__r....r
-000009f0: 2000 0000 7213 0000 0072 1600 0000 7223   ...r....r....r#
-00000a00: 0000 0072 1d00 0000 7224 0000 0072 0b00  ...r....r$...r..
-00000a10: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
-00000a20: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00000a30: 0e00 0000 0400 0816 0801 0803 0805 1205  ................
-00000a40: 0e04                                     ..
+00000040: 5a02 6403 6404 8400 5a03 6410 6406 6407  Z.d.d...Z.d.d.d.
+00000050: 8401 5a04 6408 6505 6409 6505 6604 640a  ..Z.d.e.d.e.f.d.
+00000060: 640b 8404 5a06 640c 640d 8400 5a07 640e  d...Z.d.d...Z.d.
+00000070: 640f 8400 5a08 6402 5300 2911 613b 0400  d...Z.d.S.).a;..
+00000080: 000a 436f 7079 7269 6768 7420 2843 2920  ..Copyright (C) 
+00000090: 3230 3232 2d32 3032 3320 5374 656c 6c61  2022-2023 Stella
+000000a0: 2054 6563 686e 6f6c 6f67 6965 7320 2855   Technologies (U
+000000b0: 4b29 204c 696d 6974 6564 2e0a 0a50 6572  K) Limited...Per
+000000c0: 6d69 7373 696f 6e20 6973 2068 6572 6562  mission is hereb
+000000d0: 7920 6772 616e 7465 642c 2066 7265 6520  y granted, free 
+000000e0: 6f66 2063 6861 7267 652c 2074 6f20 616e  of charge, to an
+000000f0: 7920 7065 7273 6f6e 206f 6274 6169 6e69  y person obtaini
+00000100: 6e67 2061 2063 6f70 790a 6f66 2074 6869  ng a copy.of thi
+00000110: 7320 736f 6674 7761 7265 2061 6e64 2061  s software and a
+00000120: 7373 6f63 6961 7465 6420 646f 6375 6d65  ssociated docume
+00000130: 6e74 6174 696f 6e20 6669 6c65 7320 2874  ntation files (t
+00000140: 6865 2022 536f 6674 7761 7265 2229 2c20  he "Software"), 
+00000150: 746f 2064 6561 6c0a 696e 2074 6865 2053  to deal.in the S
+00000160: 6f66 7477 6172 6520 7769 7468 6f75 7420  oftware without 
+00000170: 7265 7374 7269 6374 696f 6e2c 2069 6e63  restriction, inc
+00000180: 6c75 6469 6e67 2077 6974 686f 7574 206c  luding without l
+00000190: 696d 6974 6174 696f 6e20 7468 6520 7269  imitation the ri
+000001a0: 6768 7473 0a74 6f20 7573 652c 2063 6f70  ghts.to use, cop
+000001b0: 792c 206d 6f64 6966 792c 206d 6572 6765  y, modify, merge
+000001c0: 2c20 7075 626c 6973 682c 2064 6973 7472  , publish, distr
+000001d0: 6962 7574 652c 2073 7562 6c69 6365 6e73  ibute, sublicens
+000001e0: 652c 2061 6e64 2f6f 7220 7365 6c6c 0a63  e, and/or sell.c
+000001f0: 6f70 6965 7320 6f66 2074 6865 2053 6f66  opies of the Sof
+00000200: 7477 6172 652c 2061 6e64 2074 6f20 7065  tware, and to pe
+00000210: 726d 6974 2070 6572 736f 6e73 2074 6f20  rmit persons to 
+00000220: 7768 6f6d 2074 6865 2053 6f66 7477 6172  whom the Softwar
+00000230: 6520 6973 0a66 7572 6e69 7368 6564 2074  e is.furnished t
+00000240: 6f20 646f 2073 6f2c 2073 7562 6a65 6374  o do so, subject
+00000250: 2074 6f20 7468 6520 666f 6c6c 6f77 696e   to the followin
+00000260: 6720 636f 6e64 6974 696f 6e73 3a0a 0a54  g conditions:..T
+00000270: 6865 2061 626f 7665 2063 6f70 7972 6967  he above copyrig
+00000280: 6874 206e 6f74 6963 6520 616e 6420 7468  ht notice and th
+00000290: 6973 2070 6572 6d69 7373 696f 6e20 6e6f  is permission no
+000002a0: 7469 6365 2073 6861 6c6c 2062 6520 696e  tice shall be in
+000002b0: 636c 7564 6564 2069 6e0a 616c 6c20 636f  cluded in.all co
+000002c0: 7069 6573 206f 7220 7375 6273 7461 6e74  pies or substant
+000002d0: 6961 6c20 706f 7274 696f 6e73 206f 6620  ial portions of 
+000002e0: 7468 6520 536f 6674 7761 7265 2e0a 0a54  the Software...T
+000002f0: 4845 2053 4f46 5457 4152 4520 4953 2050  HE SOFTWARE IS P
+00000300: 524f 5649 4445 4420 2241 5320 4953 222c  ROVIDED "AS IS",
+00000310: 2057 4954 484f 5554 2057 4152 5241 4e54   WITHOUT WARRANT
+00000320: 5920 4f46 2041 4e59 204b 494e 442c 2045  Y OF ANY KIND, E
+00000330: 5850 5245 5353 204f 520a 494d 504c 4945  XPRESS OR.IMPLIE
+00000340: 442c 2049 4e43 4c55 4449 4e47 2042 5554  D, INCLUDING BUT
+00000350: 204e 4f54 204c 494d 4954 4544 2054 4f20   NOT LIMITED TO 
+00000360: 5448 4520 5741 5252 414e 5449 4553 204f  THE WARRANTIES O
+00000370: 4620 4d45 5243 4841 4e54 4142 494c 4954  F MERCHANTABILIT
+00000380: 592c 0a46 4954 4e45 5353 2046 4f52 2041  Y,.FITNESS FOR A
+00000390: 2050 4152 5449 4355 4c41 5220 5055 5250   PARTICULAR PURP
+000003a0: 4f53 4520 414e 4420 4e4f 4e49 4e46 5249  OSE AND NONINFRI
+000003b0: 4e47 454d 454e 542e 2049 4e20 4e4f 2045  NGEMENT. IN NO E
+000003c0: 5645 4e54 2053 4841 4c4c 2054 4845 0a41  VENT SHALL THE.A
+000003d0: 5554 484f 5253 204f 5220 434f 5059 5249  UTHORS OR COPYRI
+000003e0: 4748 5420 484f 4c44 4552 5320 4245 204c  GHT HOLDERS BE L
+000003f0: 4941 424c 4520 464f 5220 414e 5920 434c  IABLE FOR ANY CL
+00000400: 4149 4d2c 2044 414d 4147 4553 204f 5220  AIM, DAMAGES OR 
+00000410: 4f54 4845 520a 4c49 4142 494c 4954 592c  OTHER.LIABILITY,
+00000420: 2057 4845 5448 4552 2049 4e20 414e 2041   WHETHER IN AN A
+00000430: 4354 494f 4e20 4f46 2043 4f4e 5452 4143  CTION OF CONTRAC
+00000440: 542c 2054 4f52 5420 4f52 204f 5448 4552  T, TORT OR OTHER
+00000450: 5749 5345 2c20 4152 4953 494e 470a 4652  WISE, ARISING.FR
+00000460: 4f4d 2c20 4f55 5420 4f46 204f 5220 494e  OM, OUT OF OR IN
+00000470: 2043 4f4e 4e45 4354 494f 4e20 5749 5448   CONNECTION WITH
+00000480: 2054 4845 2053 4f46 5457 4152 4520 4f52   THE SOFTWARE OR
+00000490: 2054 4845 2055 5345 204f 5220 4f54 4845   THE USE OR OTHE
+000004a0: 5220 4445 414c 494e 4753 0a49 4e20 5448  R DEALINGS.IN TH
+000004b0: 4520 534f 4654 5741 5245 2e0a e900 0000  E SOFTWARE......
+000004c0: 004e 6301 0000 0000 0000 0000 0000 0003  .Nc.............
+000004d0: 0000 0004 0000 0063 0000 0073 4e00 0000  .......c...sN...
+000004e0: 8100 7400 7c00 6a01 7402 8302 721e 7c00  ..t.|.j.t...r.|.
+000004f0: 6a01 a003 a100 4400 5d0f 5c02 7d01 7d02  j.....D.].\.}.}.
+00000500: 7c00 6a04 9b00 6401 7c01 9b00 9d03 7c02  |.j...d.|.....|.
+00000510: 6602 5600 0100 710c 6400 5300 7c00 6a04  f.V...q.d.S.|.j.
+00000520: 7c00 6a01 6602 5600 0100 6400 5300 2902  |.j.f.V...d.S.).
+00000530: 4eda 012e 2905 da0a 6973 696e 7374 616e  N...)...isinstan
+00000540: 6365 5a09 7661 6c75 6554 7970 65da 0464  ceZ.valueType..d
+00000550: 6963 74da 0569 7465 6d73 da04 6e61 6d65  ict..items..name
+00000560: 2903 da05 6669 656c 645a 116e 6573 7465  )...fieldZ.neste
+00000570: 645f 6669 656c 645f 6e61 6d65 5a17 6e65  d_field_nameZ.ne
+00000580: 7374 6564 5f66 6965 6c64 5f76 616c 7565  sted_field_value
+00000590: 5f74 7970 65a9 0072 0800 0000 fa59 2f55  _type..r.....Y/U
+000005a0: 7365 7273 2f74 6f6d 2d6b 616e 647a 696f  sers/tom-kandzio
+000005b0: 7261 2f44 6576 4c6f 6361 6c2f 7374 656c  ra/DevLocal/stel
+000005c0: 6c61 2f73 7465 6c6c 612d 6e6f 772f 5374  la/stella-now/St
+000005d0: 656c 6c61 4e6f 7743 4c49 2f73 7465 6c6c  ellaNowCLI/stell
+000005e0: 616e 6f77 5f63 6c69 2f75 7469 6c73 2f75  anow_cli/utils/u
+000005f0: 7469 6c73 2e70 79da 0d66 6c61 7474 656e  tils.py..flatten
+00000600: 5f66 6965 6c64 1b00 0000 730c 0000 0002  _field....s.....
+00000610: 800c 0112 0218 0104 ff12 0372 0a00 0000  ...........r....
+00000620: e904 0000 0063 0200 0000 0000 0000 0000  .....c..........
+00000630: 0000 0300 0000 0800 0000 4300 0000 7334  ..........C...s4
+00000640: 0000 007a 0974 006a 017c 007c 0164 018d  ...z.t.j.|.|.d..
+00000650: 027d 0257 006e 0a04 0074 0279 1301 0001  .}.W.n...t.y....
+00000660: 0001 0059 0064 0253 0077 0074 037c 0283  ...Y.d.S.w.t.|..
+00000670: 017c 006b 0253 0029 037a fa0a 2020 2020  .|.k.S.).z..    
+00000680: 4368 6563 6b20 6966 2075 7569 645f 746f  Check if uuid_to
+00000690: 5f74 6573 7420 6973 2061 2076 616c 6964  _test is a valid
+000006a0: 2055 5549 442e 0a0a 2020 2020 5061 7261   UUID...    Para
+000006b0: 6d65 7465 7273 3a0a 2020 2020 2a20 7575  meters:.    * uu
+000006c0: 6964 5f74 6f5f 7465 7374 3a20 7374 7220  id_to_test: str 
+000006d0: 2d20 5468 6520 7374 7269 6e67 2074 6f20  - The string to 
+000006e0: 7465 7374 2061 7320 6120 5555 4944 2e0a  test as a UUID..
+000006f0: 2020 2020 2a20 7665 7273 696f 6e3a 2069      * version: i
+00000700: 6e74 202d 2055 5549 4420 7665 7273 696f  nt - UUID versio
+00000710: 6e20 2864 6566 6175 6c74 2069 7320 3429  n (default is 4)
+00000720: 2e0a 0a20 2020 2052 6574 7572 6e73 3a0a  ...    Returns:.
+00000730: 2020 2020 2a20 6054 7275 6560 2069 6620      * `True` if 
+00000740: 7575 6964 5f74 6f5f 7465 7374 2069 7320  uuid_to_test is 
+00000750: 6120 7661 6c69 6420 5555 4944 3b20 6f74  a valid UUID; ot
+00000760: 6865 7277 6973 6520 6046 616c 7365 602e  herwise `False`.
+00000770: 0a20 2020 2029 01da 0776 6572 7369 6f6e  .    )...version
+00000780: 4629 04da 0475 7569 64da 0455 5549 44da  F)...uuid..UUID.
+00000790: 0a56 616c 7565 4572 726f 72da 0373 7472  .ValueError..str
+000007a0: 2903 5a0c 7575 6964 5f74 6f5f 7465 7374  ).Z.uuid_to_test
+000007b0: 720c 0000 005a 0875 7569 645f 6f62 6a72  r....Z.uuid_objr
+000007c0: 0800 0000 7208 0000 0072 0900 0000 da0d  ....r....r......
+000007d0: 6973 5f76 616c 6964 5f75 7569 6424 0000  is_valid_uuid$..
+000007e0: 0073 0c00 0000 020b 1201 0c01 0601 02ff  .s..............
+000007f0: 0c02 7211 0000 00da 0463 6f64 65da 0672  ..r......code..r
+00000800: 6574 7572 6e63 0100 0000 0000 0000 0000  eturnc..........
+00000810: 0000 0100 0000 0600 0000 4300 0000 7314  ..........C...s.
+00000820: 0000 0074 006a 0164 0164 027c 0074 006a  ...t.j.d.d.|.t.j
+00000830: 0264 038d 0453 0029 044e 7a09 2f5c 2a2e  .d...S.).Nz./\*.
+00000840: 2a3f 5c2a 2fda 0029 01da 0566 6c61 6773  *?\*/..)...flags
+00000850: 2903 da02 7265 da03 7375 62da 0644 4f54  )...re..sub..DOT
+00000860: 414c 4c29 0172 1200 0000 7208 0000 0072  ALL).r....r....r
+00000870: 0800 0000 7209 0000 00da 0f72 656d 6f76  ....r......remov
+00000880: 655f 636f 6d6d 656e 7473 3600 0000 7302  e_comments6...s.
+00000890: 0000 0014 0172 1900 0000 6301 0000 0000  .....r....c.....
+000008a0: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+000008b0: 0000 0073 1e00 0000 7c00 a000 6401 a101  ...s....|...d...
+000008c0: 7d01 6402 a001 6403 6404 8400 7c01 4400  }.d...d.d...|.D.
+000008d0: 8301 a101 5300 2905 4eda 015f 7214 0000  ....S.).N.._r...
+000008e0: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+000008f0: 0000 0300 0000 7300 0000 f318 0000 0081  ......s.........
+00000900: 007c 005d 077d 017c 01a0 00a1 0056 0001  .|.].}.|.....V..
+00000910: 0071 0264 0053 00a9 014e a901 da05 7469  .q.d.S...N....ti
+00000920: 746c 65a9 02da 022e 30da 0178 7208 0000  tle.....0..xr...
+00000930: 0072 0800 0000 7209 0000 00da 093c 6765  .r....r......<ge
+00000940: 6e65 7870 723e 3c00 0000 f304 0000 0002  nexpr><.........
+00000950: 8016 007a 2173 6e61 6b65 5f74 6f5f 6361  ...z!snake_to_ca
+00000960: 6d65 6c2e 3c6c 6f63 616c 733e 2e3c 6765  mel.<locals>.<ge
+00000970: 6e65 7870 723e a902 da05 7370 6c69 74da  nexpr>....split.
+00000980: 046a 6f69 6e29 025a 0973 6e61 6b65 5f73  .join).Z.snake_s
+00000990: 7472 da0a 636f 6d70 6f6e 656e 7473 7208  tr..componentsr.
+000009a0: 0000 0072 0800 0000 7209 0000 00da 0e73  ...r....r......s
+000009b0: 6e61 6b65 5f74 6f5f 6361 6d65 6c3a 0000  nake_to_camel:..
+000009c0: 0073 0400 0000 0a01 1401 7228 0000 0063  .s........r(...c
+000009d0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+000009e0: 0700 0000 4300 0000 732e 0000 007c 00a0  ....C...s....|..
+000009f0: 0064 01a1 017d 017c 0164 0219 0064 03a0  .d...}.|.d...d..
+00000a00: 0164 0464 0584 007c 0164 0664 0085 0219  .d.d...|.d.d....
+00000a10: 0044 0083 01a1 0117 0053 0029 074e 721a  .D.......S.).Nr.
+00000a20: 0000 0072 0100 0000 7214 0000 0063 0100  ...r....r....c..
+00000a30: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00000a40: 0000 7300 0000 721b 0000 0072 1c00 0000  ..s...r....r....
+00000a50: 721d 0000 0072 1f00 0000 7208 0000 0072  r....r....r....r
+00000a60: 0800 0000 7209 0000 0072 2200 0000 4100  ....r....r"...A.
+00000a70: 0000 7223 0000 007a 2773 6e61 6b65 5f74  ..r#...z'snake_t
+00000a80: 6f5f 6c6f 7765 725f 6361 6d65 6c2e 3c6c  o_lower_camel.<l
+00000a90: 6f63 616c 733e 2e3c 6765 6e65 7870 723e  ocals>.<genexpr>
+00000aa0: e901 0000 0072 2400 0000 2902 da01 7372  .....r$...)...sr
+00000ab0: 2700 0000 7208 0000 0072 0800 0000 7209  '...r....r....r.
+00000ac0: 0000 00da 1473 6e61 6b65 5f74 6f5f 6c6f  .....snake_to_lo
+00000ad0: 7765 725f 6361 6d65 6c3f 0000 0073 0400  wer_camel?...s..
+00000ae0: 0000 0a01 2401 722b 0000 0029 0172 0b00  ....$.r+...).r..
+00000af0: 0000 2909 da07 5f5f 646f 635f 5f72 1600  ..)...__doc__r..
+00000b00: 0000 720d 0000 0072 0a00 0000 7211 0000  ..r....r....r...
+00000b10: 0072 1000 0000 7219 0000 0072 2800 0000  .r....r....r(...
+00000b20: 722b 0000 0072 0800 0000 7208 0000 0072  r+...r....r....r
+00000b30: 0800 0000 7209 0000 00da 083c 6d6f 6475  ....r......<modu
+00000b40: 6c65 3e01 0000 0073 1000 0000 0400 0816  le>....s........
+00000b50: 0801 0803 0a09 1212 0804 0c05            ............
```

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/utils/logger.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/utils/logger.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli/utils/utils.py` & `stellanow_cli-0.0.9rc2/stellanow_cli/utils/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,26 +20,21 @@
 IN THE SOFTWARE.
 """
 
 import re
 import uuid
 
 
-def snake_to_camel(snake_str):
-    components = snake_str.split('_')
-    return ''.join(x.title() for x in components)
-
-
-def snake_to_lower_camel(s):
-    components = s.split('_')
-    return components[0] + ''.join(x.title() for x in components[1:])
-
-
-def remove_comments(code: str) -> str:
-    return re.sub(r'/\*.*?\*/', '', code, flags=re.DOTALL)
+def flatten_field(field):
+    if isinstance(field.valueType, dict):
+        # Handle nested types
+        for nested_field_name, nested_field_value_type in field.valueType.items():
+            yield f'{field.name}.{nested_field_name}', nested_field_value_type
+    else:
+        yield field.name, field.valueType
 
 
 def is_valid_uuid(uuid_to_test, version=4):
     """
     Check if uuid_to_test is a valid UUID.
 
     Parameters:
@@ -50,7 +45,21 @@
     * `True` if uuid_to_test is a valid UUID; otherwise `False`.
     """
     try:
         uuid_obj = uuid.UUID(uuid_to_test, version=version)
     except ValueError:
         return False
     return str(uuid_obj) == uuid_to_test
+
+
+def remove_comments(code: str) -> str:
+    return re.sub(r'/\*.*?\*/', '', code, flags=re.DOTALL)
+
+
+def snake_to_camel(snake_str):
+    components = snake_str.split('_')
+    return ''.join(x.title() for x in components)
+
+
+def snake_to_lower_camel(s):
+    components = s.split('_')
+    return components[0] + ''.join(x.title() for x in components[1:])
```

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli.egg-info/PKG-INFO` & `stellanow_cli-0.0.9rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: stellanow-cli
-Version: 0.0.9rc1
+Name: stellanow_cli
+Version: 0.0.9rc2
 Summary: Command-line interface for the StellaNow SDK code generation and comparison tool.
 Requires-Python: >=3.10
 
 StellaNow CLI Tool
 ==================
 
 Welcome to the StellaNow CLI tool. This tool automates the process of generating class code from StellaNow event specifications and provides a summary of changes between the generated classes and the specifications fetched from the API. It's recommended to use this tool in conjunction with the StellaNow SDK's to ensure that your application's message classes are up-to-date with the latest specifications.
```

### Comparing `stellanow_cli-0.0.9rc1/stellanow_cli.egg-info/SOURCES.txt` & `stellanow_cli-0.0.9rc2/stellanow_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/tests/__pycache__/test_generate_class_handles_all_valueTypes.cpython-310.pyc` & `stellanow_cli-0.0.9rc2/tests/__pycache__/test_generate_class_handles_all_valueTypes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/tests/test_command_configure.py` & `stellanow_cli-0.0.9rc2/tests/test_command_configure.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc1/tests/test_generate_class_handles_all_valueTypes.py` & `stellanow_cli-0.0.9rc2/tests/test_generate_class_handles_all_valueTypes.py`

 * *Files identical despite different names*

