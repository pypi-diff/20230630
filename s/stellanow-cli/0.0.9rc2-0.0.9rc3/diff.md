# Comparing `tmp/stellanow_cli-0.0.9rc2.tar.gz` & `tmp/stellanow_cli-0.0.9rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stellanow_cli-0.0.9rc2.tar", last modified: Thu Jun 29 23:25:56 2023, max compression
+gzip compressed data, was "stellanow_cli-0.0.9rc3.tar", last modified: Fri Jun 30 13:18:27 2023, max compression
```

## Comparing `stellanow_cli-0.0.9rc2.tar` & `stellanow_cli-0.0.9rc3.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:56.356438 stellanow_cli-0.0.9rc2/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       98 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/MANIFEST.in
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     8331 2023-06-29 23:25:56.353947 stellanow_cli-0.0.9rc2/PKG-INFO
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      225 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/Pipfile
--rw-r--r--   0 tom-kandziora   (501) staff       (20)    10889 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/README.md
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     8154 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/README.public
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-29 23:25:56.356616 stellanow_cli-0.0.9rc2/setup.cfg
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2284 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/setup.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:55.847907 stellanow_cli-0.0.9rc2/stellanow_cli/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1090 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:55.920005 stellanow_cli-0.0.9rc2/stellanow_cli/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1277 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1348 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/__pycache__/_run.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1307 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/__pycache__/_version.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2100 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/__pycache__/cli.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1173 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/_run.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1117 2023-06-29 23:24:44.000000 stellanow_cli-0.0.9rc2/stellanow_cli/_version.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:55.940373 stellanow_cli-0.0.9rc2/stellanow_cli/api/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1231 2023-06-27 21:31:01.000000 stellanow_cli-0.0.9rc2/stellanow_cli/api/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:55.952749 stellanow_cli-0.0.9rc2/stellanow_cli/api/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1453 2023-06-29 22:10:25.000000 stellanow_cli-0.0.9rc2/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2272 2023-06-29 23:05:14.000000 stellanow_cli-0.0.9rc2/stellanow_cli/api/__pycache__/datatypes.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     5626 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1537 2023-06-29 22:49:17.000000 stellanow_cli-0.0.9rc2/stellanow_cli/api/datatypes.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     6572 2023-06-20 14:47:52.000000 stellanow_cli-0.0.9rc2/stellanow_cli/api/stellanow_api.py
--rwxr-xr-x   0 tom-kandziora   (501) staff       (20)     2058 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/cli.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:55.966576 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1146 2023-06-20 14:47:50.000000 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:55.983944 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1363 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2580 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     7210 2023-06-29 23:24:22.000000 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/__pycache__/csharp_code_generator.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2226 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/code_generator.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     6687 2023-06-29 23:24:22.000000 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/csharp_code_generator.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:55.993435 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/templates/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-10 10:14:46.000000 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/templates/.footer.template
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      126 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/templates/.header.template
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      544 2023-06-29 23:22:51.000000 stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/templates/csharp.template
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:56.097124 stellanow_cli-0.0.9rc2/stellanow_cli/commands/
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:56.113798 stellanow_cli-0.0.9rc2/stellanow_cli/commands/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     4538 2023-06-27 15:44:57.000000 stellanow_cli-0.0.9rc2/stellanow_cli/commands/__pycache__/command_config.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3732 2023-06-27 15:44:40.000000 stellanow_cli-0.0.9rc2/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2125 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/commands/__pycache__/events.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     5175 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/commands/__pycache__/generate.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     4595 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1090 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/commands/_init__.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     4934 2023-06-27 15:44:51.000000 stellanow_cli-0.0.9rc2/stellanow_cli/commands/command_config.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     4607 2023-06-27 15:44:32.000000 stellanow_cli-0.0.9rc2/stellanow_cli/commands/configure.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1990 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/commands/events.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     5203 2023-06-20 14:47:52.000000 stellanow_cli-0.0.9rc2/stellanow_cli/commands/generate.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     5210 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/commands/plan.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:56.192814 stellanow_cli-0.0.9rc2/stellanow_cli/config/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1276 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/config/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:56.220354 stellanow_cli-0.0.9rc2/stellanow_cli/config/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1705 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2193 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/config/__pycache__/config.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1622 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/config/__pycache__/dev.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1618 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/config/__pycache__/int.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1612 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/config/config.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1246 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/config/dev.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1242 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/config/int.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:56.250350 stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2208 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/StellaNowAPIExceptions.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2163 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/StellaNowCLIException.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1090 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:56.263467 stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3138 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/__pycache__/StellaNowAPIExceptions.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3177 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/__pycache__/StellaNowCLIException.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1288 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:56.298151 stellanow_cli-0.0.9rc2/stellanow_cli/utils/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1090 2023-06-27 14:25:32.000000 stellanow_cli-0.0.9rc2/stellanow_cli/utils/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:56.312616 stellanow_cli-0.0.9rc2/stellanow_cli/utils/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1283 2023-06-27 15:44:10.000000 stellanow_cli-0.0.9rc2/stellanow_cli/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1693 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc2/stellanow_cli/utils/__pycache__/logger.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2908 2023-06-27 15:44:40.000000 stellanow_cli-0.0.9rc2/stellanow_cli/utils/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1631 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/stellanow_cli/utils/logger.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2240 2023-06-27 14:21:56.000000 stellanow_cli-0.0.9rc2/stellanow_cli/utils/utils.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:55.908949 stellanow_cli-0.0.9rc2/stellanow_cli.egg-info/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     8331 2023-06-29 23:25:55.000000 stellanow_cli-0.0.9rc2/stellanow_cli.egg-info/PKG-INFO
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2988 2023-06-29 23:25:55.000000 stellanow_cli-0.0.9rc2/stellanow_cli.egg-info/SOURCES.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)        1 2023-06-29 23:25:55.000000 stellanow_cli-0.0.9rc2/stellanow_cli.egg-info/dependency_links.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       52 2023-06-29 23:25:55.000000 stellanow_cli-0.0.9rc2/stellanow_cli.egg-info/entry_points.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       46 2023-06-29 23:25:55.000000 stellanow_cli-0.0.9rc2/stellanow_cli.egg-info/requires.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       14 2023-06-29 23:25:55.000000 stellanow_cli-0.0.9rc2/stellanow_cli.egg-info/top_level.txt
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:56.329497 stellanow_cli-0.0.9rc2/tests/
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-29 23:25:56.350161 stellanow_cli-0.0.9rc2/tests/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1837 2023-06-18 17:07:08.000000 stellanow_cli-0.0.9rc2/tests/__pycache__/test_generate_class_handles_all_valueTypes.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2853 2023-06-20 14:47:41.000000 stellanow_cli-0.0.9rc2/tests/test_command_configure.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3313 2023-06-20 14:47:54.000000 stellanow_cli-0.0.9rc2/tests/test_generate_class_handles_all_valueTypes.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.324788 stellanow_cli-0.0.9rc3/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       98 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/MANIFEST.in
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     8331 2023-06-30 13:18:27.324207 stellanow_cli-0.0.9rc3/PKG-INFO
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      225 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/Pipfile
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)    10889 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/README.md
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     8154 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/README.public
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-30 13:18:27.324874 stellanow_cli-0.0.9rc3/setup.cfg
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2284 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/setup.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.223629 stellanow_cli-0.0.9rc3/stellanow_cli/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1090 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.265027 stellanow_cli-0.0.9rc3/stellanow_cli/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1277 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc3/stellanow_cli/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1348 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc3/stellanow_cli/__pycache__/_run.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1307 2023-06-30 12:14:52.000000 stellanow_cli-0.0.9rc3/stellanow_cli/__pycache__/_version.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2100 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc3/stellanow_cli/__pycache__/cli.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1173 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/_run.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1117 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/_version.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.268261 stellanow_cli-0.0.9rc3/stellanow_cli/api/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1231 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/api/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.271755 stellanow_cli-0.0.9rc3/stellanow_cli/api/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1453 2023-06-29 22:10:25.000000 stellanow_cli-0.0.9rc3/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2272 2023-06-29 23:05:14.000000 stellanow_cli-0.0.9rc3/stellanow_cli/api/__pycache__/datatypes.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     5618 2023-06-30 10:39:47.000000 stellanow_cli-0.0.9rc3/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1537 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/api/datatypes.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     6564 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/api/stellanow_api.py
+-rwxr-xr-x   0 tom-kandziora   (501) staff       (20)     2058 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/cli.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.274985 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1146 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.279881 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1363 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2580 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     7205 2023-06-30 10:44:58.000000 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/__pycache__/csharp_code_generator.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2226 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/code_generator.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     6680 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/csharp_code_generator.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.282647 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/templates/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-10 10:14:46.000000 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/templates/.footer.template
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      126 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/templates/.header.template
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      544 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/templates/csharp.template
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.288596 stellanow_cli-0.0.9rc3/stellanow_cli/commands/
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.297241 stellanow_cli-0.0.9rc3/stellanow_cli/commands/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4538 2023-06-27 15:44:57.000000 stellanow_cli-0.0.9rc3/stellanow_cli/commands/__pycache__/command_config.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3735 2023-06-30 12:21:54.000000 stellanow_cli-0.0.9rc3/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2135 2023-06-30 12:21:55.000000 stellanow_cli-0.0.9rc3/stellanow_cli/commands/__pycache__/events.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     5197 2023-06-30 12:19:26.000000 stellanow_cli-0.0.9rc3/stellanow_cli/commands/__pycache__/generate.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4617 2023-06-30 12:14:51.000000 stellanow_cli-0.0.9rc3/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1090 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/commands/_init__.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4934 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/commands/command_config.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4617 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/commands/configure.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2005 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/commands/events.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     5246 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/commands/generate.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     5253 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/commands/plan.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.300490 stellanow_cli-0.0.9rc3/stellanow_cli/config/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1276 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/config/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.303453 stellanow_cli-0.0.9rc3/stellanow_cli/config/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1705 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc3/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2193 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc3/stellanow_cli/config/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1622 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc3/stellanow_cli/config/__pycache__/dev.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1618 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc3/stellanow_cli/config/__pycache__/int.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1612 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/config/config.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1246 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/config/dev.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1242 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/config/int.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.305559 stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1090 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.308077 stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1288 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3146 2023-06-30 10:39:47.000000 stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/__pycache__/api_exceptions.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3170 2023-06-30 10:39:47.000000 stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/__pycache__/cli_exceptions.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2201 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/api_exceptions.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2163 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/cli_exceptions.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.310624 stellanow_cli-0.0.9rc3/stellanow_cli/utils/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1090 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/utils/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.317469 stellanow_cli-0.0.9rc3/stellanow_cli/utils/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1283 2023-06-27 15:44:10.000000 stellanow_cli-0.0.9rc3/stellanow_cli/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1693 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc3/stellanow_cli/utils/__pycache__/logger.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2908 2023-06-27 15:44:40.000000 stellanow_cli-0.0.9rc3/stellanow_cli/utils/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1631 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/utils/logger.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2240 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/utils/utils.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.252151 stellanow_cli-0.0.9rc3/stellanow_cli.egg-info/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     8331 2023-06-30 13:18:26.000000 stellanow_cli-0.0.9rc3/stellanow_cli.egg-info/PKG-INFO
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2958 2023-06-30 13:18:26.000000 stellanow_cli-0.0.9rc3/stellanow_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)        1 2023-06-30 13:18:26.000000 stellanow_cli-0.0.9rc3/stellanow_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       52 2023-06-30 13:18:26.000000 stellanow_cli-0.0.9rc3/stellanow_cli.egg-info/entry_points.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       46 2023-06-30 13:18:26.000000 stellanow_cli-0.0.9rc3/stellanow_cli.egg-info/requires.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       14 2023-06-30 13:18:26.000000 stellanow_cli-0.0.9rc3/stellanow_cli.egg-info/top_level.txt
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.319203 stellanow_cli-0.0.9rc3/tests/
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.323525 stellanow_cli-0.0.9rc3/tests/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2940 2023-06-30 10:44:58.000000 stellanow_cli-0.0.9rc3/tests/__pycache__/test_generate_class_handles_all_valueTypes.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2853 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/tests/test_command_configure.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3313 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/tests/test_generate_class_handles_all_valueTypes.py
```

### Comparing `stellanow_cli-0.0.9rc2/PKG-INFO` & `stellanow_cli-0.0.9rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stellanow_cli
-Version: 0.0.9rc2
+Version: 0.0.9rc3
 Summary: Command-line interface for the StellaNow SDK code generation and comparison tool.
 Requires-Python: >=3.10
 
 StellaNow CLI Tool
 ==================
 
 Welcome to the StellaNow CLI tool. This tool automates the process of generating class code from StellaNow event specifications and provides a summary of changes between the generated classes and the specifications fetched from the API. It's recommended to use this tool in conjunction with the StellaNow SDK's to ensure that your application's message classes are up-to-date with the latest specifications.
```

### Comparing `stellanow_cli-0.0.9rc2/README.md` & `stellanow_cli-0.0.9rc3/README.md`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/README.public` & `stellanow_cli-0.0.9rc3/README.public`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/setup.py` & `stellanow_cli-0.0.9rc3/setup.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/__init__.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/__pycache__/_run.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/__pycache__/_run.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/__pycache__/_version.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/__pycache__/_version.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 20 14:47:41 2023 UTC, .py size: 1117 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0dbc 9164 5d04 0000  o..........d]...
+00000000: 6f0d 0d0a 0000 0000 85b5 9e64 5d04 0000  o..........d]...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 0c00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 5a01 6402 5300 2903 613b 0400  Z.d.Z.d.S.).a;..
 00000040: 000a 436f 7079 7269 6768 7420 2843 2920  ..Copyright (C) 
 00000050: 3230 3232 2d32 3032 3320 5374 656c 6c61  2022-2023 Stella
 00000060: 2054 6563 686e 6f6c 6f67 6965 7320 2855   Technologies (U
 00000070: 4b29 204c 696d 6974 6564 2e0a 0a50 6572  K) Limited...Per
@@ -66,15 +66,15 @@
 00000410: 5749 5345 2c20 4152 4953 494e 470a 4652  WISE, ARISING.FR
 00000420: 4f4d 2c20 4f55 5420 4f46 204f 5220 494e  OM, OUT OF OR IN
 00000430: 2043 4f4e 4e45 4354 494f 4e20 5749 5448   CONNECTION WITH
 00000440: 2054 4845 2053 4f46 5457 4152 4520 4f52   THE SOFTWARE OR
 00000450: 2054 4845 2055 5345 204f 5220 4f54 4845   THE USE OR OTHE
 00000460: 5220 4445 414c 494e 4753 0a49 4e20 5448  R DEALINGS.IN TH
 00000470: 4520 534f 4654 5741 5245 2e0a 7a09 302e  E SOFTWARE..z.0.
-00000480: 302e 392e 7263 314e 2902 da07 5f5f 646f  0.9.rc1N)...__do
+00000480: 302e 392e 7263 334e 2902 da07 5f5f 646f  0.9.rc3N)...__do
 00000490: 635f 5fda 0b5f 5f76 6572 7369 6f6e 5f5f  c__..__version__
 000004a0: a900 7203 0000 0072 0300 0000 fa56 2f55  ..r....r.....V/U
 000004b0: 7365 7273 2f74 6f6d 2d6b 616e 647a 696f  sers/tom-kandzio
 000004c0: 7261 2f44 6576 4c6f 6361 6c2f 7374 656c  ra/DevLocal/stel
 000004d0: 6c61 2f73 7465 6c6c 612d 6e6f 772f 5374  la/stella-now/St
 000004e0: 656c 6c61 4e6f 7743 4c49 2f73 7465 6c6c  ellaNowCLI/stell
 000004f0: 616e 6f77 5f63 6c69 2f5f 7665 7273 696f  anow_cli/_versio
```

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/__pycache__/cli.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/__pycache__/cli.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/_run.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/_run.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/_version.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 IN THE SOFTWARE.
 """
 
-__version__ = "0.0.9.rc2"
+__version__ = "0.0.9.rc3"
```

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/api/__init__.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/api/__init__.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/api/__pycache__/datatypes.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/api/__pycache__/datatypes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 20 14:47:52 2023 UTC, .py size: 6572 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 18bc 9164 ac19 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 7ab0 9e64 a419 0000  o.......z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6404  Z.d.d.l.m.Z...d.
 00000060: 6405 6c07 6d08 5a08 0100 6406 6407 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
@@ -173,25 +173,25 @@
 00000ac0: 0da1 00a0 0e64 0574 0f83 00a1 02a0 0e64  .....d.t.......d
 00000ad0: 06a1 017c 005f 077c 02a0 0da1 00a0 0e64  ...|._.|.......d
 00000ae0: 0574 0f83 00a1 02a0 0e64 07a1 017c 005f  .t.......d...|._
 00000af0: 0274 00a0 0164 08a1 0101 0064 0053 0029  .t...d.....d.S.)
 00000b00: 094e 7a1e 4175 7468 656e 7469 6361 7469  .Nz.Authenticati
 00000b10: 6e67 2074 6f20 7468 6520 4150 4920 2e2e  ng to the API ..
 00000b20: 2e20 5a0a 6261 636b 6f66 6669 6365 2905  . Z.backoffice).
-00000b30: 5a08 7265 616c 6d5f 6964 da08 7573 6572  Z.realm_id..user
-00000b40: 6e61 6d65 da05 656d 6169 6cda 0870 6173  name..email..pas
+00000b30: 5a08 7265 616c 6d5f 6964 5a08 7573 6572  Z.realm_idZ.user
+00000b40: 6e61 6d65 5a05 656d 6169 6c5a 0870 6173  nameZ.emailZ.pas
 00000b50: 7377 6f72 645a 0963 6c69 656e 745f 6964  swordZ.client_id
 00000b60: a901 721d 0000 0072 1b00 0000 7211 0000  ..r....r....r...
 00000b70: 0072 1500 0000 7a19 4175 7468 656e 7469  .r....z.Authenti
 00000b80: 6361 7469 6f6e 2053 7563 6365 7373 6675  cation Successfu
 00000b90: 6c29 10da 066c 6f67 6765 72da 0469 6e66  l)...logger..inf
 00000ba0: 6f72 1500 0000 7222 0000 0072 1200 0000  or....r"...r....
 00000bb0: 7210 0000 0072 1100 0000 7214 0000 00da  r....r....r.....
 00000bc0: 0872 6571 7565 7374 73da 0470 6f73 7472  .requests..postr
-00000bd0: 0f00 0000 da08 6175 7468 5f75 726c 7225  ......auth_urlr%
+00000bd0: 0f00 0000 5a08 6175 7468 5f75 726c 7225  ....Z.auth_urlr%
 00000be0: 0000 0072 1d00 0000 721e 0000 0072 1f00  ...r....r....r..
 00000bf0: 0000 a903 7217 0000 00da 0462 6f64 7972  ....r......bodyr
 00000c00: 2300 0000 7218 0000 0072 1800 0000 7219  #...r....r....r.
 00000c10: 0000 0072 1600 0000 5900 0000 7320 0000  ...r....Y...s ..
 00000c20: 000a 010a 020a 0104 0304 0104 0104 0102  ................
 00000c30: 0106 fb06 0806 0112 020a 011a 021a 010e  ................
 00000c40: 027a 1653 7465 6c6c 6141 5049 2e61 7574  .z.StellaAPI.aut
@@ -204,23 +204,23 @@
 00000cb0: 067c 006a 076a 087c 0164 038d 027d 027c  .|.j.j.|.d...}.|
 00000cc0: 00a0 097c 02a1 0101 007c 02a0 0aa1 00a0  ...|.....|......
 00000cd0: 0b64 0474 0c83 00a1 02a0 0b64 05a1 017c  .d.t.......d...|
 00000ce0: 005f 047c 02a0 0aa1 00a0 0b64 0474 0c83  ._.|.......d.t..
 00000cf0: 00a1 02a0 0b64 02a1 017c 005f 0074 02a0  .....d...|._.t..
 00000d00: 0364 06a1 0101 0064 0053 0029 074e 7a18  .d.....d.S.).Nz.
 00000d10: 4150 4920 546f 6b65 6e20 5265 6672 6573  API Token Refres
-00000d20: 6869 6e67 202e 2e2e 7215 0000 0072 2900  hing ...r....r).
+00000d20: 6869 6e67 202e 2e2e 7215 0000 0072 2600  hing ...r....r&.
 00000d30: 0000 721b 0000 0072 1100 0000 7a1c 4150  ..r....r....z.AP
 00000d40: 4920 546f 6b65 6e20 5265 6672 6573 6820  I Token Refresh 
 00000d50: 5375 6363 6573 7366 756c 290d 7215 0000  Successful).r...
-00000d60: 0072 1600 0000 722a 0000 0072 2b00 0000  .r....r*...r+...
-00000d70: 7214 0000 0072 2c00 0000 722d 0000 0072  r....r,...r-...r
-00000d80: 0f00 0000 da10 6175 7468 5f72 6566 7265  ......auth_refre
+00000d60: 0072 1600 0000 7227 0000 0072 2800 0000  .r....r'...r(...
+00000d70: 7214 0000 0072 2900 0000 722a 0000 0072  r....r)...r*...r
+00000d80: 0f00 0000 5a10 6175 7468 5f72 6566 7265  ....Z.auth_refre
 00000d90: 7368 5f75 726c 7225 0000 0072 1d00 0000  sh_urlr%...r....
-00000da0: 721e 0000 0072 1f00 0000 722f 0000 0072  r....r....r/...r
+00000da0: 721e 0000 0072 1f00 0000 722b 0000 0072  r....r....r+...r
 00000db0: 1800 0000 7218 0000 0072 1900 0000 7222  ....r....r....r"
 00000dc0: 0000 0072 0000 0073 1600 0000 0a01 0c01  ...r...s........
 00000dd0: 0a02 0a02 0602 0601 1202 0a01 1a02 1a01  ................
 00000de0: 0e02 7a16 5374 656c 6c61 4150 492e 6175  ..z.StellaAPI.au
 00000df0: 7468 5f72 6566 7265 7368 da06 7265 7475  th_refresh..retu
 00000e00: 726e 4e63 0100 0000 0000 0000 0000 0000  rnNc............
 00000e10: 0700 0000 0700 0000 6300 0000 73a0 0000  ........c...s...
@@ -246,32 +246,32 @@
 00000f50: 0000 7340 0000 0081 007c 005d 1b7d 0174  ..s@.....|.].}.t
 00000f60: 007c 01a0 0164 00a1 017c 01a0 0164 01a1  .|...d...|...d..
 00000f70: 017c 01a0 0164 02a1 017c 01a0 0164 03a1  .|...d...|...d..
 00000f80: 017c 01a0 0164 04a1 0164 058d 0556 0001  .|...d...d...V..
 00000f90: 0071 0264 0653 0029 07da 0269 64da 046e  .q.d.S.)...id..n
 00000fa0: 616d 65da 0869 7341 6374 6976 65da 0963  ame..isActive..c
 00000fb0: 7265 6174 6564 4174 da09 7570 6461 7465  reatedAt..update
-00000fc0: 6441 7429 0572 3a00 0000 723b 0000 0072  dAt).r:...r;...r
-00000fd0: 3c00 0000 723d 0000 0072 3e00 0000 4e29  <...r=...r>...N)
+00000fc0: 6441 7429 0572 3500 0000 7236 0000 0072  dAt).r5...r6...r
+00000fd0: 3700 0000 7238 0000 0072 3900 0000 4e29  7...r8...r9...N)
 00000fe0: 0272 0800 0000 721e 0000 0029 02da 022e  .r....r....)....
 00000ff0: 30da 0565 7665 6e74 7218 0000 0072 1800  0..eventr....r..
 00001000: 0000 7219 0000 00da 093c 6765 6e65 7870  ..r......<genexp
 00001010: 723e 9300 0000 7316 0000 0002 8004 0002  r>....s.........
 00001020: 0702 fa08 0108 0108 0108 0108 0104 fb0a  ................
 00001030: ff7a 2753 7465 6c6c 6141 5049 2e67 6574  .z'StellaAPI.get
 00001040: 5f65 7665 6e74 732e 3c6c 6f63 616c 733e  _events.<locals>
 00001050: 2e3c 6765 6e65 7870 723e 290c da09 6974  .<genexpr>)...it
 00001060: 6572 746f 6f6c 73da 0563 6f75 6e74 720f  ertools..countr.
-00001070: 0000 00da 0a65 7665 6e74 735f 7572 6cda  .....events_url.
+00001070: 0000 005a 0a65 7665 6e74 735f 7572 6cda  ...Z.events_url.
 00001080: 0666 6f72 6d61 7472 1300 0000 7214 0000  .formatr....r...
-00001090: 0072 2c00 0000 721e 0000 0072 2500 0000  .r,...r....r%...
+00001090: 0072 2900 0000 721e 0000 0072 2500 0000  .r)...r....r%...
 000010a0: 721d 0000 0072 1f00 0000 2907 7217 0000  r....r....).r...
 000010b0: 005a 0970 6167 655f 7369 7a65 5a0b 7061  .Z.page_sizeZ.pa
-000010c0: 6765 5f6e 756d 6265 72da 0375 726c 7238  ge_number..urlr8
-000010d0: 0000 0072 2300 0000 da06 6576 656e 7473  ...r#.....events
+000010c0: 6765 5f6e 756d 6265 72da 0375 726c 7233  ge_number..urlr3
+000010d0: 0000 0072 2300 0000 5a06 6576 656e 7473  ...r#...Z.events
 000010e0: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
 000010f0: 0a67 6574 5f65 7665 6e74 7385 0000 0073  .get_events....s
 00001100: 2000 0000 0280 0401 1001 1001 1001 04ff   ...............
 00001110: 1002 0e02 0a01 1a02 0401 0601 0602 0207  ................
 00001120: 0ef9 04f4 7a14 5374 656c 6c61 4150 492e  ....z.StellaAPI.
 00001130: 6765 745f 6576 656e 7473 da08 6576 656e  get_events..even
 00001140: 745f 6964 6302 0000 0000 0000 0000 0000  t_idc...........
@@ -284,69 +284,69 @@
 000011b0: 6406 6407 8400 7c05 a006 6408 740a 8300  d.d...|...d.t...
 000011c0: a102 4400 8301 7d06 6409 6407 8400 7c05  ..D...}.d.d...|.
 000011d0: a006 640a 740a 8300 a102 4400 8301 7d07  ..d.t.....D...}.
 000011e0: 740b 7c05 a006 640b a101 7c05 a006 640c  t.|...d...|...d.
 000011f0: a101 7c05 a006 640d a101 7c05 a006 640e  ..|...d...|...d.
 00001200: a101 7c05 a006 640f a101 7c05 a006 6410  ..|...d...|...d.
 00001210: a101 7c07 7c06 6411 8d08 5300 2912 4e29  ..|.|.d...S.).N)
-00001220: 0272 3400 0000 5a07 6576 656e 7449 6472  .r4...Z.eventIdr
-00001230: 3500 0000 7236 0000 0072 3700 0000 721b  5...r6...r7...r.
+00001220: 0272 2f00 0000 da07 6576 656e 7449 6472  .r/.....eventIdr
+00001230: 3000 0000 7231 0000 0072 3200 0000 721b  0...r1...r2...r.
 00001240: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
 00001250: 0200 0000 0600 0000 5300 0000 f31a 0000  ........S.......
 00001260: 0067 007c 005d 097d 0174 0064 0069 007c  .g.|.].}.t.d.i.|
 00001270: 01a4 018e 0191 0271 0253 00a9 0172 1800  .......q.S...r..
-00001280: 0000 2901 7206 0000 0029 0272 3f00 0000  ..).r....).r?...
+00001280: 0000 2901 7206 0000 0029 0272 3a00 0000  ..).r....).r:...
 00001290: da06 656e 7469 7479 7218 0000 0072 1800  ..entityr....r..
 000012a0: 0000 7219 0000 00da 0a3c 6c69 7374 636f  ..r......<listco
 000012b0: 6d70 3ea7 0000 00f3 0200 0000 1a00 7a2f  mp>...........z/
 000012c0: 5374 656c 6c61 4150 492e 6765 745f 6576  StellaAPI.get_ev
 000012d0: 656e 745f 6465 7461 696c 732e 3c6c 6f63  ent_details.<loc
 000012e0: 616c 733e 2e3c 6c69 7374 636f 6d70 3eda  als>.<listcomp>.
 000012f0: 0865 6e74 6974 6965 7363 0100 0000 0000  .entitiesc......
 00001300: 0000 0000 0000 0200 0000 0600 0000 5300  ..............S.
-00001310: 0000 724a 0000 0072 4b00 0000 2901 7207  ..rJ...rK...).r.
-00001320: 0000 0029 0272 3f00 0000 da05 6669 656c  ...).r?.....fiel
+00001310: 0000 7244 0000 0072 4500 0000 2901 7207  ..rD...rE...).r.
+00001320: 0000 0029 0272 3a00 0000 da05 6669 656c  ...).r:.....fiel
 00001330: 6472 1800 0000 7218 0000 0072 1900 0000  dr....r....r....
-00001340: 724d 0000 00aa 0000 0072 4e00 0000 da06  rM.......rN.....
-00001350: 6669 656c 6473 723a 0000 0072 3b00 0000  fieldsr:...r;...
-00001360: da0b 6465 7363 7269 7074 696f 6e72 3c00  ..descriptionr<.
-00001370: 0000 723d 0000 0072 3e00 0000 2908 723a  ..r=...r>...).r:
-00001380: 0000 0072 3b00 0000 7252 0000 0072 3c00  ...r;...rR...r<.
-00001390: 0000 723d 0000 0072 3e00 0000 7251 0000  ..r=...r>...rQ..
-000013a0: 0072 4f00 0000 290c 720f 0000 00da 0965  .rO...).r......e
-000013b0: 7665 6e74 5f75 726c 7245 0000 0072 1300  vent_urlrE...r..
-000013c0: 0000 7214 0000 0072 2c00 0000 721e 0000  ..r....r,...r...
+00001340: 7247 0000 00aa 0000 0072 4800 0000 da06  rG.......rH.....
+00001350: 6669 656c 6473 7235 0000 0072 3600 0000  fieldsr5...r6...
+00001360: da0b 6465 7363 7269 7074 696f 6e72 3700  ..descriptionr7.
+00001370: 0000 7238 0000 0072 3900 0000 2908 7235  ..r8...r9...).r5
+00001380: 0000 0072 3600 0000 724c 0000 0072 3700  ...r6...rL...r7.
+00001390: 0000 7238 0000 0072 3900 0000 724b 0000  ..r8...r9...rK..
+000013a0: 0072 4900 0000 290c 720f 0000 005a 0965  .rI...).r....Z.e
+000013b0: 7665 6e74 5f75 726c 723f 0000 0072 1300  vent_urlr?...r..
+000013c0: 0000 7214 0000 0072 2900 0000 721e 0000  ..r....r)...r...
 000013d0: 0072 2500 0000 721d 0000 0072 1f00 0000  .r%...r....r....
 000013e0: 7221 0000 0072 0900 0000 2908 7217 0000  r!...r....).r...
-000013f0: 0072 4900 0000 7246 0000 0072 3800 0000  .rI...rF...r8...
-00001400: 7223 0000 0072 1b00 0000 724f 0000 0072  r#...r....rO...r
-00001410: 5100 0000 7218 0000 0072 1800 0000 7219  Q...r....r....r.
+000013f0: 0072 4200 0000 7240 0000 0072 3300 0000  .rB...r@...r3...
+00001400: 7223 0000 0072 1b00 0000 7249 0000 0072  r#...r....rI...r
+00001410: 4b00 0000 7218 0000 0072 1800 0000 7219  K...r....r....r.
 00001420: 0000 00da 1167 6574 5f65 7665 6e74 5f64  .....get_event_d
 00001430: 6574 6169 6c73 9d00 0000 7322 0000 0014  etails....s"....
 00001440: 0110 010e 020a 0112 0218 0318 0302 0308  ................
 00001450: 0108 0108 0108 0108 0108 0102 0102 0106  ................
 00001460: f87a 1b53 7465 6c6c 6141 5049 2e67 6574  .z.StellaAPI.get
 00001470: 5f65 7665 6e74 5f64 6574 6169 6c73 290e  _event_details).
 00001480: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
 00001490: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
 000014a0: 6d65 5f5f 7204 0000 00da 0373 7472 721a  me__r......strr.
 000014b0: 0000 0072 2500 0000 7216 0000 0072 2200  ...r%...r....r".
-000014c0: 0000 7202 0000 0072 0800 0000 7248 0000  ..r....r....rH..
-000014d0: 0072 0900 0000 7254 0000 0072 1800 0000  .r....rT...r....
+000014c0: 0000 7202 0000 0072 0800 0000 7241 0000  ..r....r....rA..
+000014d0: 0072 0900 0000 724d 0000 0072 1800 0000  .r....rM...r....
 000014e0: 7218 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
 000014f0: 0e00 0000 3000 0000 730e 0000 0008 001e  ....0...s.......
 00001500: 0108 0c08 1c08 1918 1316 1872 0e00 0000  ...........r....
-00001510: 2917 da07 5f5f 646f 635f 5f72 4200 0000  )...__doc__rB...
-00001520: 721d 0000 00da 076c 6f67 6769 6e67 722c  r......loggingr,
+00001510: 2917 da07 5f5f 646f 635f 5f72 3d00 0000  )...__doc__r=...
+00001520: 721d 0000 00da 076c 6f67 6769 6e67 7229  r......loggingr)
 00001530: 0000 00da 0674 7970 696e 6772 0200 0000  .....typingr....
-00001540: da06 636f 6e66 6967 7204 0000 00da 0964  ..configr......d
+00001540: 5a06 636f 6e66 6967 7204 0000 00da 0964  Z.configr......d
 00001550: 6174 6174 7970 6573 7206 0000 0072 0700  atatypesr....r..
-00001560: 0000 7208 0000 0072 0900 0000 5a21 6578  ..r....r....Z!ex
-00001570: 6365 7074 696f 6e73 2e53 7465 6c6c 614e  ceptions.StellaN
-00001580: 6f77 4150 4945 7863 6570 7469 6f6e 7372  owAPIExceptionsr
-00001590: 0a00 0000 720b 0000 0072 0c00 0000 720d  ....r....r....r.
-000015a0: 0000 00da 0967 6574 4c6f 6767 6572 7255  .....getLoggerrU
-000015b0: 0000 0072 2a00 0000 720e 0000 0072 1800  ...r*...r....r..
-000015c0: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-000015d0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-000015e0: 1600 0000 0400 0816 0801 0801 0801 0c02  ................
-000015f0: 0c02 1801 1806 0a08 1203                 ..........
+00001560: 0000 7208 0000 0072 0900 0000 5a19 6578  ..r....r....Z.ex
+00001570: 6365 7074 696f 6e73 2e61 7069 5f65 7863  ceptions.api_exc
+00001580: 6570 7469 6f6e 7372 0a00 0000 720b 0000  eptionsr....r...
+00001590: 0072 0c00 0000 720d 0000 00da 0967 6574  .r....r......get
+000015a0: 4c6f 6767 6572 724e 0000 0072 2700 0000  LoggerrN...r'...
+000015b0: 720e 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
+000015c0: 1800 0000 7219 0000 00da 083c 6d6f 6475  ....r......<modu
+000015d0: 6c65 3e01 0000 0073 1600 0000 0400 0816  le>....s........
+000015e0: 0801 0801 0801 0c02 0c02 1801 1806 0a08  ................
+000015f0: 1203                                     ..
```

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/api/datatypes.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/api/datatypes.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/api/stellanow_api.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/api/stellanow_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from ..config import Config
 from .datatypes import (
     StellaEntity,
     StellaField,
     StellaEvent,
     StellaEventDetailed
 )
-from ..exceptions.StellaNowAPIExceptions import (
+from ..exceptions.api_exceptions import (
     StellaAPIForbiddenError,
     StellaAPINotFoundError,
     StellaAPIUnauthorisedError,
     StellaAPIWrongCredentialsError
 )
```

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/cli.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/cli.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/__init__.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/__init__.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/__pycache__/csharp_code_generator.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/__pycache__/csharp_code_generator.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 29 23:24:22 2023 UTC, .py size: 6687 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a612 9e64 1f1a 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 26b2 9e64 181a 0000  o.......&..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 0801 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
 00000060: 0100 6401 6404 6c08 6d08 5a08 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6405 6c09 6d0a 5a0a 0100 6406 6407 6c0b  d.l.m.Z...d.d.l.
@@ -107,345 +107,345 @@
 000006a0: 6e63 0100 0000 0000 0000 0000 0000 0200  nc..............
 000006b0: 0000 0700 0000 4300 0000 731e 0000 0064  ......C...s....d
 000006c0: 0164 0264 0364 0464 0564 0664 079c 067d  .d.d.d.d.d.d...}
 000006d0: 017c 01a0 007c 0064 08a1 0253 0029 094e  .|...|.d...S.).N
 000006e0: da07 6465 6369 6d61 6cda 0369 6e74 da04  ..decimal..int..
 000006f0: 626f 6f6c da06 7374 7269 6e67 5a08 4461  bool..stringZ.Da
 00000700: 7465 4f6e 6c79 da08 4461 7465 5469 6d65  teOnly..DateTime
-00000710: a906 5a07 4465 6369 6d61 6c5a 0749 6e74  ..Z.DecimalZ.Int
-00000720: 6567 6572 5a07 426f 6f6c 6561 6eda 0653  egerZ.Boolean..S
-00000730: 7472 696e 675a 0444 6174 6572 1700 0000  tringZ.Dater....
+00000710: a906 da07 4465 6369 6d61 6cda 0749 6e74  ....Decimal..Int
+00000720: 6567 6572 da07 426f 6f6c 6561 6eda 0653  eger..Boolean..S
+00000730: 7472 696e 67da 0444 6174 6572 1700 0000  tring..Dater....
 00000740: da06 6f62 6a65 6374 a901 da03 6765 74a9  ..object....get.
 00000750: 0272 1100 0000 da07 6d61 7070 696e 67a9  .r......mapping.
-00000760: 0072 1f00 0000 fa73 2f55 7365 7273 2f74  .r.....s/Users/t
+00000760: 0072 2300 0000 fa73 2f55 7365 7273 2f74  .r#....s/Users/t
 00000770: 6f6d 2d6b 616e 647a 696f 7261 2f44 6576  om-kandziora/Dev
 00000780: 4c6f 6361 6c2f 7374 656c 6c61 2f73 7465  Local/stella/ste
 00000790: 6c6c 612d 6e6f 772f 5374 656c 6c61 4e6f  lla-now/StellaNo
 000007a0: 7743 4c49 2f73 7465 6c6c 616e 6f77 5f63  wCLI/stellanow_c
 000007b0: 6c69 2f63 6f64 655f 6765 6e65 7261 746f  li/code_generato
 000007c0: 7273 2f63 7368 6172 705f 636f 6465 5f67  rs/csharp_code_g
 000007d0: 656e 6572 6174 6f72 2e70 79da 1266 6965  enerator.py..fie
 000007e0: 6c64 5f74 7970 655f 6d61 7070 696e 672c  ld_type_mapping,
 000007f0: 0000 00f3 1000 0000 0202 0201 0201 0201  ................
-00000800: 0201 0201 06fa 0c08 7221 0000 0063 0100  ........r!...c..
+00000800: 0201 0201 06fa 0c08 7225 0000 0063 0100  ........r%...c..
 00000810: 0000 0000 0000 0000 0000 0200 0000 0700  ................
 00000820: 0000 4300 0000 731e 0000 0064 0164 0264  ..C...s....d.d.d
 00000830: 0364 0464 0564 0664 079c 067d 017c 01a0  .d.d.d.d...}.|..
 00000840: 007c 0064 04a1 0253 0029 084e 7a2d 2e54  .|.d...S.).Nz-.T
 00000850: 6f53 7472 696e 6728 2246 3222 2c20 4375  oString("F2", Cu
 00000860: 6c74 7572 6549 6e66 6f2e 496e 7661 7269  ltureInfo.Invari
 00000870: 616e 7443 756c 7475 7265 297a 0b2e 546f  antCulture)z..To
 00000880: 5374 7269 6e67 2829 7a15 2e54 6f53 7472  String()z..ToStr
 00000890: 696e 6728 292e 546f 4c6f 7765 7228 29da  ing().ToLower().
 000008a0: 007a 172e 546f 5374 7269 6e67 2822 7979  .z..ToString("yy
 000008b0: 7979 2d4d 4d2d 6464 2229 7a21 2e54 6f53  yy-MM-dd")z!.ToS
 000008c0: 7472 696e 6728 2279 7979 792d 4d4d 2d64  tring("yyyy-MM-d
 000008d0: 6454 4848 3a6d 6d3a 7373 5a22 2972 1800  dTHH:mm:ssZ")r..
-000008e0: 0000 721b 0000 0072 1d00 0000 721f 0000  ..r....r....r...
-000008f0: 0072 1f00 0000 7220 0000 00da 1466 6965  .r....r .....fie
+000008e0: 0000 721f 0000 0072 2100 0000 7223 0000  ..r....r!...r#..
+000008f0: 0072 2300 0000 7224 0000 00da 1466 6965  .r#...r$.....fie
 00000900: 6c64 5f66 6f72 6d61 745f 6d61 7070 696e  ld_format_mappin
-00000910: 6738 0000 0072 2200 0000 7224 0000 00da  g8...r"...r$....
+00000910: 6738 0000 0072 2600 0000 7228 0000 00da  g8...r&...r(....
 00000920: 0477 6f72 6463 0100 0000 0000 0000 0000  .wordc..........
-00000930: 0000 0200 0000 0200 0000 4300 0000 731c  ..........C...s.
+00000930: 0000 0200 0000 0200 0000 4300 0000 731e  ..........C...s.
 00000940: 0000 0067 0064 01a2 017d 017c 007c 0176  ...g.d...}.|.|.v
-00000950: 0072 0c7c 0064 0217 0053 007c 0053 0029  .r.|.d...S.|.S.)
-00000960: 034e 294d 5a08 6162 7374 7261 6374 da02  .N)MZ.abstract..
-00000970: 6173 da04 6261 7365 7215 0000 00da 0562  as..baser......b
-00000980: 7265 616b da04 6279 7465 da04 6361 7365  reak..byte..case
-00000990: 5a05 6361 7463 68da 0463 6861 72da 0763  Z.catch..char..c
-000009a0: 6865 636b 6564 da05 636c 6173 73da 0563  hecked..class..c
-000009b0: 6f6e 7374 da08 636f 6e74 696e 7565 7213  onst..continuer.
-000009c0: 0000 00da 0764 6566 6175 6c74 5a08 6465  .....defaultZ.de
-000009d0: 6c65 6761 7465 5a02 646f 5a06 646f 7562  legateZ.doZ.doub
-000009e0: 6c65 da04 656c 7365 da04 656e 756d da05  le..else..enum..
-000009f0: 6576 656e 745a 0865 7870 6c69 6369 745a  eventZ.explicitZ
-00000a00: 0665 7874 6572 6eda 0566 616c 7365 da07  .extern..false..
-00000a10: 6669 6e61 6c6c 79da 0566 6978 6564 da05  finally..fixed..
-00000a20: 666c 6f61 74da 0366 6f72 5a07 666f 7265  float..forZ.fore
-00000a30: 6163 685a 0467 6f74 6fda 0269 665a 0869  achZ.goto..ifZ.i
-00000a40: 6d70 6c69 6369 74da 0269 6e72 1400 0000  mplicit..inr....
-00000a50: 5a09 696e 7465 7266 6163 655a 0869 6e74  Z.interfaceZ.int
-00000a60: 6572 6e61 6cda 0269 73da 046c 6f63 6b5a  ernal..is..lockZ
-00000a70: 046c 6f6e 67da 096e 616d 6573 7061 6365  .long..namespace
-00000a80: da03 6e65 77da 046e 756c 6c72 1a00 0000  ..new..nullr....
-00000a90: da08 6f70 6572 6174 6f72 da03 6f75 74da  ..operator..out.
-00000aa0: 086f 7665 7272 6964 65da 0670 6172 616d  .override..param
-00000ab0: 735a 0770 7269 7661 7465 5a09 7072 6f74  sZ.privateZ.prot
-00000ac0: 6563 7465 645a 0670 7562 6c69 63da 0872  ectedZ.public..r
-00000ad0: 6561 646f 6e6c 79da 0372 6566 7212 0000  eadonly..refr...
-00000ae0: 005a 0573 6279 7465 5a06 7365 616c 6564  .Z.sbyteZ.sealed
-00000af0: 5a05 7368 6f72 745a 0673 697a 656f 665a  Z.shortZ.sizeofZ
-00000b00: 0a73 7461 636b 616c 6c6f 635a 0673 7461  .stackallocZ.sta
-00000b10: 7469 6372 1600 0000 da06 7374 7275 6374  ticr......struct
-00000b20: 5a06 7377 6974 6368 da04 7468 6973 da05  Z.switch..this..
-00000b30: 7468 726f 77da 0474 7275 65da 0374 7279  throw..true..try
-00000b40: 5a06 7479 7065 6f66 5a04 7569 6e74 5a05  Z.typeofZ.uintZ.
-00000b50: 756c 6f6e 675a 0975 6e63 6865 636b 6564  ulongZ.unchecked
-00000b60: da06 756e 7361 6665 5a06 7573 686f 7274  ..unsafeZ.ushort
-00000b70: 5a05 7573 696e 675a 0776 6972 7475 616c  Z.usingZ.virtual
-00000b80: 5a04 766f 6964 5a08 766f 6c61 7469 6c65  Z.voidZ.volatile
-00000b90: da05 7768 696c 65da 015f 721f 0000 0029  ..while.._r....)
-00000ba0: 0272 2500 0000 5a0e 7265 7365 7276 6564  .r%...Z.reserved
-00000bb0: 5f77 6f72 6473 721f 0000 0072 1f00 0000  _wordsr....r....
-00000bc0: 7220 0000 00da 1565 7363 6170 655f 7265  r .....escape_re
-00000bd0: 7365 7276 6564 5f77 6f72 6473 4400 0000  served_wordsD...
-00000be0: 7304 0000 0008 0114 0c72 4e00 0000 6300  s........rN...c.
-00000bf0: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-00000c00: 0000 0040 0000 0073 4800 0000 6500 5a01  ...@...sH...e.Z.
-00000c10: 6400 5a02 5500 6503 6504 6401 3c00 6503  d.Z.U.e.e.d.<.e.
-00000c20: 6504 6402 3c00 6503 6504 6403 3c00 6503  e.d.<.e.e.d.<.e.
-00000c30: 6504 6404 3c00 6505 6405 6506 6602 6406  e.d.<.e.d.e.f.d.
-00000c40: 6407 8404 8301 5a07 6408 6409 8400 5a08  d.....Z.d.d...Z.
-00000c50: 640a 5300 290b da0b 4353 6861 7270 4669  d.S.)...CSharpFi
-00000c60: 656c 64da 0d6f 7269 6769 6e61 6c5f 6e61  eld..original_na
-00000c70: 6d65 da0b 6373 6861 7270 5f6e 616d 65da  me..csharp_name.
-00000c80: 0474 7970 65da 0666 6f72 6d61 74da 0566  .type..format..f
-00000c90: 6965 6c64 6302 0000 0000 0000 0000 0000  ieldc...........
-00000ca0: 0002 0000 0006 0000 0043 0000 0073 2800  .........C...s(.
-00000cb0: 0000 7c00 7c01 6a00 7401 7402 7c01 6a00  ..|.|.j.t.t.|.j.
-00000cc0: 8301 8301 7403 7c01 6a04 8301 7405 7c01  ....t.|.j...t.|.
-00000cd0: 6a04 8301 6401 8d04 5300 2902 4e29 0472  j...d...S.).N).r
-00000ce0: 5000 0000 7251 0000 0072 5200 0000 7253  P...rQ...rR...rS
-00000cf0: 0000 0029 06da 046e 616d 6572 4e00 0000  ...)...namerN...
-00000d00: 720f 0000 0072 2100 0000 da09 7661 6c75  r....r!.....valu
-00000d10: 6554 7970 6572 2400 0000 2902 da03 636c  eTyper$...)...cl
-00000d20: 7372 5400 0000 721f 0000 0072 1f00 0000  srT...r....r....
-00000d30: 7220 0000 00da 1166 726f 6d5f 7374 656c  r .....from_stel
-00000d40: 6c61 5f66 6965 6c64 5b00 0000 730c 0000  la_field[...s...
-00000d50: 0002 0204 010c 0108 0108 0106 fc7a 1d43  .............z.C
-00000d60: 5368 6172 7046 6965 6c64 2e66 726f 6d5f  SharpField.from_
-00000d70: 7374 656c 6c61 5f66 6965 6c64 6301 0000  stella_fieldc...
-00000d80: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00000d90: 0043 0000 0073 1200 0000 7c00 6a00 9b00  .C...s....|.j...
-00000da0: 6401 7c00 6a01 9b00 9d03 5300 2902 4eda  d.|.j.....S.).N.
-00000db0: 0120 2902 7252 0000 0072 5100 0000 a901  . ).rR...rQ.....
-00000dc0: da04 7365 6c66 721f 0000 0072 1f00 0000  ..selfr....r....
-00000dd0: 7220 0000 00da 2474 6f5f 636f 6e73 7472  r ....$to_constr
-00000de0: 7563 746f 725f 7061 7261 6d65 7465 725f  uctor_parameter_
-00000df0: 6465 636c 6172 6174 696f 6e64 0000 0073  declarationd...s
-00000e00: 0200 0000 1201 7a30 4353 6861 7270 4669  ......z0CSharpFi
-00000e10: 656c 642e 746f 5f63 6f6e 7374 7275 6374  eld.to_construct
-00000e20: 6f72 5f70 6172 616d 6574 6572 5f64 6563  or_parameter_dec
-00000e30: 6c61 7261 7469 6f6e 4e29 09da 085f 5f6e  larationN)...__n
-00000e40: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000e50: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-00000e60: 0373 7472 da0f 5f5f 616e 6e6f 7461 7469  .str..__annotati
-00000e70: 6f6e 735f 5fda 0b63 6c61 7373 6d65 7468  ons__..classmeth
-00000e80: 6f64 7208 0000 0072 5800 0000 725c 0000  odr....rX...r\..
-00000e90: 0072 1f00 0000 721f 0000 0072 1f00 0000  .r....r....r....
-00000ea0: 7220 0000 0072 4f00 0000 5400 0000 7310  r ...rO...T...s.
-00000eb0: 0000 000a 0008 0208 0108 0108 0102 0210  ................
-00000ec0: 010c 0872 4f00 0000 6300 0000 0000 0000  ...rO...c.......
-00000ed0: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000ee0: 0073 4000 0000 6500 5a01 6400 5a02 5500  .s@...e.Z.d.Z.U.
-00000ef0: 6503 6504 6401 3c00 6503 6504 6402 3c00  e.e.d.<.e.e.d.<.
-00000f00: 6505 6403 6506 6602 6404 6405 8404 8301  e.d.e.f.d.d.....
-00000f10: 5a07 6406 6407 8400 5a08 6408 6409 8400  Z.d.d...Z.d.d...
-00000f20: 5a09 640a 5300 290b da0c 4353 6861 7270  Z.d.S.)...CSharp
-00000f30: 456e 7469 7479 7250 0000 0072 5100 0000  EntityrP...rQ...
-00000f40: da06 656e 7469 7479 6302 0000 0000 0000  ..entityc.......
-00000f50: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
-00000f60: 0073 1c00 0000 7c00 7c01 6a00 7401 7402  .s....|.|.j.t.t.
-00000f70: 7c01 6a00 8301 8301 6401 1700 6402 8d02  |.j.....d...d...
-00000f80: 5300 2903 4e5a 0249 64a9 0272 5000 0000  S.).NZ.Id..rP...
-00000f90: 7251 0000 0029 0372 5500 0000 724e 0000  rQ...).rU...rN..
-00000fa0: 0072 0f00 0000 2902 7257 0000 0072 6400  .r....).rW...rd.
-00000fb0: 0000 721f 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-00000fc0: 0072 5800 0000 6d00 0000 7308 0000 0002  .rX...m...s.....
-00000fd0: 0204 0110 0106 fe7a 1e43 5368 6172 7045  .......z.CSharpE
-00000fe0: 6e74 6974 792e 6672 6f6d 5f73 7465 6c6c  ntity.from_stell
-00000ff0: 615f 6669 656c 6463 0100 0000 0000 0000  a_fieldc........
-00001000: 0000 0000 0100 0000 0500 0000 4300 0000  ............C...
-00001010: 7316 0000 0064 017c 006a 009b 0064 027c  s....d.|.j...d.|
-00001020: 006a 019b 0064 039d 0553 0029 044e 7a10  .j...d...S.).Nz.
-00001030: 6e65 7720 456e 7469 7479 5479 7065 2822  new EntityType("
-00001040: 7a03 222c 20fa 0129 7265 0000 0072 5a00  z.", ..)re...rZ.
-00001050: 0000 721f 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-00001060: 00da 1a74 6f5f 656e 7469 7479 5f74 7970  ...to_entity_typ
-00001070: 655f 6465 636c 6172 6174 696f 6e74 0000  e_declarationt..
-00001080: 0073 0200 0000 1601 7a27 4353 6861 7270  .s......z'CSharp
-00001090: 456e 7469 7479 2e74 6f5f 656e 7469 7479  Entity.to_entity
-000010a0: 5f74 7970 655f 6465 636c 6172 6174 696f  _type_declaratio
-000010b0: 6e63 0100 0000 0000 0000 0000 0000 0100  nc..............
-000010c0: 0000 0200 0000 4300 0000 730c 0000 0064  ......C...s....d
-000010d0: 017c 006a 009b 009d 0253 0029 024e 7a07  .|.j.....S.).Nz.
-000010e0: 7374 7269 6e67 2029 0172 5100 0000 725a  string ).rQ...rZ
-000010f0: 0000 0072 1f00 0000 721f 0000 0072 2000  ...r....r....r .
-00001100: 0000 725c 0000 0077 0000 0073 0200 0000  ..r\...w...s....
-00001110: 0c01 7a31 4353 6861 7270 456e 7469 7479  ..z1CSharpEntity
-00001120: 2e74 6f5f 636f 6e73 7472 7563 746f 725f  .to_constructor_
-00001130: 7061 7261 6d65 7465 725f 6465 636c 6172  parameter_declar
-00001140: 6174 696f 6e4e 290a 725d 0000 0072 5e00  ationN).r]...r^.
-00001150: 0000 725f 0000 0072 6000 0000 7261 0000  ..r_...r`...ra..
-00001160: 0072 6200 0000 7209 0000 0072 5800 0000  .rb...r....rX...
-00001170: 7267 0000 0072 5c00 0000 721f 0000 0072  rg...r\...r....r
-00001180: 1f00 0000 721f 0000 0072 2000 0000 7263  ....r....r ...rc
-00001190: 0000 0068 0000 0073 0e00 0000 0a00 0802  ...h...s........
-000011a0: 0801 0202 1001 0806 0c03 7263 0000 0063  ..........rc...c
-000011b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000011c0: 0800 0000 4000 0000 7356 0000 0065 005a  ....@...sV...e.Z
-000011d0: 0164 005a 0265 0364 0165 0464 0265 0566  .d.Z.e.d.e.d.e.f
-000011e0: 0464 0364 0484 0483 015a 0665 0364 0565  .d.d.....Z.e.d.e
-000011f0: 0564 0265 0566 0464 0664 0784 0483 015a  .d.e.f.d.d.....Z
-00001200: 0765 0864 0165 0464 0865 0564 0265 0965  .e.d.e.d.e.d.e.e
-00001210: 0519 0066 0664 0964 0a84 0483 015a 0a64  ...f.d.d.....Z.d
-00001220: 0b53 0029 0cda 1343 7368 6172 7043 6f64  .S.)...CsharpCod
-00001230: 6547 656e 6572 6174 6f72 7233 0000 0072  eGeneratorr3...r
-00001240: 1200 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00001250: 0007 0000 000c 0000 004b 0000 0073 bc00  .........K...s..
-00001260: 0000 7400 a001 6401 a101 7d02 7c01 a002  ..t...d...}.|...
-00001270: 6402 6403 a102 7d03 6404 6405 8400 7c00  d.d...}.d.d...|.
-00001280: 6a03 4400 8301 7d04 6406 6405 8400 7c00  j.D...}.d.d...|.
-00001290: 6a04 4400 8301 7d05 7c05 7320 7405 8300  j.D...}.|.s t...
-000012a0: 8201 7c02 6a06 7407 7c00 6a08 8301 7c00  ..|.j.t.|.j...|.
-000012b0: 6a08 6407 a009 6407 a009 6408 6405 8400  j.d...d...d.d...
-000012c0: 7c05 4400 8301 a101 6407 a009 6409 6405  |.D.....d...d.d.
-000012d0: 8400 7c04 4400 8301 a101 6702 a101 6407  ..|.D.....g...d.
-000012e0: a009 640a 6405 8400 7c05 4400 8301 a101  ..d.d...|.D.....
-000012f0: 7c04 7c03 740a 6a0b 740c 7c00 8301 640b  |.|.t.j.t.|...d.
-00001300: 640c 8d02 7c00 6a0d 740e a00f a100 a010  d...|.j.t.......
-00001310: 640d a101 640e 8d09 7d06 7c06 5300 290f  d...d...}.|.S.).
-00001320: 4eda 0663 7368 6172 7072 3d00 0000 7a15  N..csharpr=...z.
-00001330: 5374 656c 6c61 4e6f 7753 444b 2e4d 6573  StellaNowSDK.Mes
-00001340: 7361 6765 7363 0100 0000 0000 0000 0000  sagesc..........
-00001350: 0000 0200 0000 0500 0000 5300 0000 f316  ..........S.....
-00001360: 0000 0067 007c 005d 077d 0174 00a0 017c  ...g.|.].}.t...|
-00001370: 01a1 0191 0271 0253 0072 1f00 0000 2902  .....q.S.r....).
-00001380: 724f 0000 0072 5800 0000 a902 da02 2e30  rO...rX........0
-00001390: 7254 0000 0072 1f00 0000 721f 0000 0072  rT...r....r....r
-000013a0: 2000 0000 da0a 3c6c 6973 7463 6f6d 703e   .....<listcomp>
-000013b0: 8200 0000 f302 0000 0016 007a 3643 7368  ...........z6Csh
-000013c0: 6172 7043 6f64 6547 656e 6572 6174 6f72  arpCodeGenerator
-000013d0: 2e67 656e 6572 6174 655f 636c 6173 732e  .generate_class.
-000013e0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-000013f0: 6d70 3e63 0100 0000 0000 0000 0000 0000  mp>c............
-00001400: 0200 0000 0500 0000 5300 0000 726a 0000  ........S...rj..
-00001410: 0072 1f00 0000 2902 7263 0000 0072 5800  .r....).rc...rX.
-00001420: 0000 a902 726c 0000 0072 6400 0000 721f  ....rl...rd...r.
-00001430: 0000 0072 1f00 0000 7220 0000 0072 6d00  ...r....r ...rm.
-00001440: 0000 8300 0000 726e 0000 007a 022c 2063  ......rn...z., c
-00001450: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00001460: 0400 0000 5300 0000 f314 0000 0067 007c  ....S........g.|
-00001470: 005d 067d 017c 01a0 00a1 0091 0271 0253  .].}.|.......q.S
-00001480: 0072 1f00 0000 a901 725c 0000 0072 6f00  .r......r\...ro.
-00001490: 0000 721f 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-000014a0: 0072 6d00 0000 8b00 0000 f302 0000 0014  .rm.............
-000014b0: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-000014c0: 0000 0400 0000 5300 0000 7270 0000 0072  ......S...rp...r
-000014d0: 1f00 0000 7271 0000 0072 6b00 0000 721f  ....rq...rk...r.
-000014e0: 0000 0072 1f00 0000 7220 0000 0072 6d00  ...r....r ...rm.
-000014f0: 0000 8c00 0000 7272 0000 0063 0100 0000  ......rr...c....
-00001500: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00001510: 5300 0000 7270 0000 0072 1f00 0000 2901  S...rp...r....).
-00001520: 7267 0000 0072 6f00 0000 721f 0000 0072  rg...ro...r....r
-00001530: 1f00 0000 7220 0000 0072 6d00 0000 8e00  ....r ...rm.....
-00001540: 0000 7272 0000 00e9 0400 0000 2901 da06  ..rr........)...
-00001550: 696e 6465 6e74 7a12 2559 2d25 6d2d 2564  indentz.%Y-%m-%d
-00001560: 5425 483a 254d 3a25 535a 2909 5a09 636c  T%H:%M:%SZ).Z.cl
-00001570: 6173 734e 616d 655a 0965 7665 6e74 4e61  assNameZ.eventNa
-00001580: 6d65 5a14 636f 6e73 7472 7563 746f 7241  meZ.constructorA
-00001590: 7267 756d 656e 7473 5a0c 656e 7469 7469  rgumentsZ.entiti
-000015a0: 6573 4c69 7374 da06 6669 656c 6473 723d  esList..fieldsr=
-000015b0: 0000 005a 0965 7665 6e74 4a73 6f6e da07  ...Z.eventJson..
-000015c0: 6576 656e 7449 64da 0974 696d 6573 7461  eventId..timesta
-000015d0: 6d70 2911 7268 0000 005a 0d6c 6f61 645f  mp).rh...Z.load_
-000015e0: 7465 6d70 6c61 7465 721c 0000 0072 7500  templater....ru.
-000015f0: 0000 da08 656e 7469 7469 6573 720d 0000  ....entitiesr...
-00001600: 005a 0672 656e 6465 7272 0e00 0000 7255  .Z.renderr....rU
-00001610: 0000 00da 046a 6f69 6eda 046a 736f 6eda  .....join..json.
-00001620: 0564 756d 7073 7202 0000 00da 0269 6472  .dumpsr......idr
-00001630: 0400 0000 da06 7574 636e 6f77 da08 7374  ......utcnow..st
-00001640: 7266 7469 6d65 2907 7233 0000 00da 066b  rftime).r3.....k
-00001650: 7761 7267 73da 0874 656d 706c 6174 6572  wargs..templater
-00001660: 3d00 0000 7275 0000 0072 7800 0000 da08  =...ru...rx.....
-00001670: 7265 6e64 6572 6564 721f 0000 0072 1f00  renderedr....r..
-00001680: 0000 7220 0000 00da 0e67 656e 6572 6174  ..r .....generat
-00001690: 655f 636c 6173 737c 0000 0073 2a00 0000  e_class|...s*...
-000016a0: 0a02 0c02 1002 1001 0401 0601 0402 0801  ................
-000016b0: 0401 0401 1201 1201 04fe 1204 0201 0201  ................
-000016c0: 1001 0401 0c01 06f4 040f 7a22 4373 6861  ..........z"Csha
-000016d0: 7270 436f 6465 4765 6e65 7261 746f 722e  rpCodeGenerator.
-000016e0: 6765 6e65 7261 7465 5f63 6c61 7373 da0a  generate_class..
-000016f0: 6576 656e 745f 6e61 6d65 6301 0000 0000  event_namec.....
-00001700: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00001710: 0000 0073 0e00 0000 7400 7c00 8301 9b00  ...s....t.|.....
-00001720: 6401 9d02 5300 2902 4e7a 0a4d 6573 7361  d...S.).Nz.Messa
-00001730: 6765 2e63 7329 0172 0e00 0000 2901 7283  ge.cs).r....).r.
-00001740: 0000 0072 1f00 0000 721f 0000 0072 2000  ...r....r....r .
-00001750: 0000 da1c 6765 745f 6669 6c65 5f6e 616d  ....get_file_nam
-00001760: 655f 666f 725f 6576 656e 745f 6e61 6d65  e_for_event_name
-00001770: 9800 0000 7302 0000 000e 027a 3043 7368  ....s......z0Csh
-00001780: 6172 7043 6f64 6547 656e 6572 6174 6f72  arpCodeGenerator
-00001790: 2e67 6574 5f66 696c 655f 6e61 6d65 5f66  .get_file_name_f
-000017a0: 6f72 5f65 7665 6e74 5f6e 616d 65da 0d65  or_event_name..e
-000017b0: 7869 7374 696e 675f 636f 6465 6303 0000  xisting_codec...
-000017c0: 0000 0000 0000 0000 0009 0000 0006 0000  ................
-000017d0: 0043 0000 0073 7400 0000 7400 a001 6401  .C...st...t...d.
-000017e0: 7c02 a102 7d03 7c03 6400 7500 720d 7402  |...}.|.d.u.r.t.
-000017f0: 8300 8201 7c03 a003 6402 a101 7d04 7c00  ....|...d...}.|.
-00001800: 6a04 7c01 6601 6900 6403 7c04 6901 a401  j.|.f.i.d.|.i...
-00001810: 8e01 7d05 7405 7c02 8301 7d06 7405 7c05  ..}.t.|...}.t.|.
-00001820: 8301 7d07 7406 a007 7c06 6a08 6404 6405  ..}.t...|.j.d.d.
-00001830: 8d01 7c07 6a08 6404 6405 8d01 a102 7d08  ..|.j.d.d.....}.
-00001840: 6406 6407 8400 7c08 4400 8301 5300 2908  d.d...|.D...S.).
-00001850: 4e7a 0f6e 616d 6573 7061 6365 2028 2e2a  Nz.namespace (.*
-00001860: 293b 720a 0000 0072 3d00 0000 5429 01da  );r....r=...T)..
-00001870: 086b 6565 7065 6e64 7363 0100 0000 0000  .keependsc......
-00001880: 0000 0000 0000 0200 0000 0400 0000 7300  ..............s.
-00001890: 0000 733c 0000 0081 007c 005d 197d 017c  ..s<.....|.].}.|
-000018a0: 01a0 0064 00a1 0173 187c 01a0 0064 01a1  ...d...s.|...d..
-000018b0: 0172 027c 01a0 0064 02a1 0173 027c 01a0  .r.|...d...s.|..
-000018c0: 0064 03a1 0173 027c 0156 0001 0071 0264  .d...s.|.V...q.d
-000018d0: 0453 0029 057a 022d 207a 022b 207a 032d  .S.).z.- z.+ z.-
-000018e0: 2d2d 7a03 2b2b 2b4e 2901 da0a 7374 6172  --z.+++N)...star
-000018f0: 7473 7769 7468 2902 726c 0000 00da 046c  tswith).rl.....l
-00001900: 696e 6572 1f00 0000 721f 0000 0072 2000  iner....r....r .
-00001910: 0000 da09 3c67 656e 6578 7072 3eae 0000  ....<genexpr>...
-00001920: 0073 0c00 0000 0280 1a00 0801 02ff 0801  .s..............
-00001930: 0eff 7a2f 4373 6861 7270 436f 6465 4765  ..z/CsharpCodeGe
-00001940: 6e65 7261 746f 722e 6765 745f 6469 6666  nerator.get_diff
-00001950: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
-00001960: 7072 3e29 09da 0272 65da 0673 6561 7263  pr>)...re..searc
-00001970: 6872 0c00 0000 da05 6772 6f75 7072 8200  hr......groupr..
-00001980: 0000 7210 0000 00da 0764 6966 666c 6962  ..r......difflib
-00001990: 5a0c 756e 6966 6965 645f 6469 6666 da0a  Z.unified_diff..
-000019a0: 7370 6c69 746c 696e 6573 2909 7257 0000  splitlines).rW..
-000019b0: 0072 3300 0000 7285 0000 005a 106e 616d  .r3...r....Z.nam
-000019c0: 6573 7061 6365 5f73 6561 7263 6872 3d00  espace_searchr=.
-000019d0: 0000 5a08 6e65 775f 636f 6465 5a19 6578  ..Z.new_codeZ.ex
-000019e0: 6973 7469 6e67 5f63 6f64 655f 6e6f 5f63  isting_code_no_c
-000019f0: 6f6d 6d65 6e74 735a 146e 6577 5f63 6f64  ommentsZ.new_cod
-00001a00: 655f 6e6f 5f63 6f6d 6d65 6e74 73da 0464  e_no_comments..d
-00001a10: 6966 6672 1f00 0000 721f 0000 0072 2000  iffr....r....r .
-00001a20: 0000 da08 6765 745f 6469 6666 9c00 0000  ....get_diff....
-00001a30: 7316 0000 000c 0308 0106 010a 0216 0208  s...............
-00001a40: 0208 010e 030a 0104 ff0e 037a 1c43 7368  ...........z.Csh
-00001a50: 6172 7043 6f64 6547 656e 6572 6174 6f72  arpCodeGenerator
-00001a60: 2e67 6574 5f64 6966 664e 290b 725d 0000  .get_diffN).r]..
-00001a70: 0072 5e00 0000 725f 0000 00da 0c73 7461  .r^...r_.....sta
-00001a80: 7469 636d 6574 686f 6472 0700 0000 7260  ticmethodr....r`
-00001a90: 0000 0072 8200 0000 7284 0000 0072 6200  ...r....r....rb.
-00001aa0: 0000 7205 0000 0072 9000 0000 721f 0000  ..r....r....r...
-00001ab0: 0072 1f00 0000 721f 0000 0072 2000 0000  .r....r....r ...
-00001ac0: 7268 0000 007b 0000 0073 0e00 0000 0800  rh...{...s......
-00001ad0: 0201 1401 021b 1401 0203 2001 7268 0000  .......... .rh..
-00001ae0: 0029 22da 075f 5f64 6f63 5f5f 728d 0000  .)"..__doc__r...
-00001af0: 0072 7a00 0000 da07 6c6f 6767 696e 6772  .rz.....loggingr
-00001b00: 8a00 0000 da0b 6461 7461 636c 6173 7365  ......dataclasse
-00001b10: 7372 0200 0000 7203 0000 0072 0400 0000  sr....r....r....
-00001b20: da06 7479 7069 6e67 7205 0000 00da 0361  ..typingr......a
-00001b30: 7069 7207 0000 0072 0800 0000 7209 0000  pir....r....r...
-00001b40: 005a 0e63 6f64 655f 6765 6e65 7261 746f  .Z.code_generato
-00001b50: 7272 0b00 0000 da20 6578 6365 7074 696f  rr..... exceptio
-00001b60: 6e73 2e53 7465 6c6c 614e 6f77 434c 4945  ns.StellaNowCLIE
-00001b70: 7863 6570 7469 6f6e 720c 0000 0072 0d00  xceptionr....r..
-00001b80: 0000 5a0b 7574 696c 732e 7574 696c 7372  ..Z.utils.utilsr
-00001b90: 0e00 0000 720f 0000 0072 1000 0000 da09  ....r....r......
-00001ba0: 6765 744c 6f67 6765 7272 5d00 0000 da06  getLoggerr].....
-00001bb0: 6c6f 6767 6572 7260 0000 0072 2100 0000  loggerr`...r!...
-00001bc0: 7224 0000 0072 4e00 0000 724f 0000 0072  r$...rN...rO...r
-00001bd0: 6300 0000 7268 0000 0072 1f00 0000 721f  c...rh...r....r.
-00001be0: 0000 0072 1f00 0000 7220 0000 00da 083c  ...r....r .....<
-00001bf0: 6d6f 6475 6c65 3e01 0000 0073 2a00 0000  module>....s*...
-00001c00: 0400 0816 0801 0801 0801 1002 0c01 0c01  ................
-00001c10: 1402 0c01 1001 1404 0a03 1203 120c 120c  ................
-00001c20: 0210 1001 0213 1001 1412                 ..........
+00000950: 0072 0d7c 009b 0064 029d 0253 007c 0053  .r.|...d...S.|.S
+00000960: 0029 034e 294d 5a08 6162 7374 7261 6374  .).N)MZ.abstract
+00000970: da02 6173 da04 6261 7365 7215 0000 00da  ..as..baser.....
+00000980: 0562 7265 616b 5a04 6279 7465 da04 6361  .breakZ.byte..ca
+00000990: 7365 5a05 6361 7463 68da 0463 6861 72da  seZ.catch..char.
+000009a0: 0763 6865 636b 6564 da05 636c 6173 73da  .checked..class.
+000009b0: 0563 6f6e 7374 da08 636f 6e74 696e 7565  .const..continue
+000009c0: 7213 0000 00da 0764 6566 6175 6c74 5a08  r......defaultZ.
+000009d0: 6465 6c65 6761 7465 5a02 646f 5a06 646f  delegateZ.doZ.do
+000009e0: 7562 6c65 da04 656c 7365 da04 656e 756d  uble..else..enum
+000009f0: da05 6576 656e 745a 0865 7870 6c69 6369  ..eventZ.explici
+00000a00: 745a 0665 7874 6572 6e5a 0566 616c 7365  tZ.externZ.false
+00000a10: da07 6669 6e61 6c6c 79da 0566 6978 6564  ..finally..fixed
+00000a20: da05 666c 6f61 74da 0366 6f72 5a07 666f  ..float..forZ.fo
+00000a30: 7265 6163 685a 0467 6f74 6fda 0269 665a  reachZ.goto..ifZ
+00000a40: 0869 6d70 6c69 6369 74da 0269 6e72 1400  .implicit..inr..
+00000a50: 0000 5a09 696e 7465 7266 6163 655a 0869  ..Z.interfaceZ.i
+00000a60: 6e74 6572 6e61 6cda 0269 73da 046c 6f63  nternal..is..loc
+00000a70: 6b5a 046c 6f6e 67da 096e 616d 6573 7061  kZ.long..namespa
+00000a80: 6365 da03 6e65 775a 046e 756c 6c72 1e00  ce..newZ.nullr..
+00000a90: 0000 da08 6f70 6572 6174 6f72 da03 6f75  ....operator..ou
+00000aa0: 74da 086f 7665 7272 6964 65da 0670 6172  t..override..par
+00000ab0: 616d 735a 0770 7269 7661 7465 5a09 7072  amsZ.privateZ.pr
+00000ac0: 6f74 6563 7465 645a 0670 7562 6c69 63da  otectedZ.public.
+00000ad0: 0872 6561 646f 6e6c 79da 0372 6566 7212  .readonly..refr.
+00000ae0: 0000 005a 0573 6279 7465 5a06 7365 616c  ...Z.sbyteZ.seal
+00000af0: 6564 da05 7368 6f72 745a 0673 697a 656f  ed..shortZ.sizeo
+00000b00: 665a 0a73 7461 636b 616c 6c6f 635a 0673  fZ.stackallocZ.s
+00000b10: 7461 7469 6372 1600 0000 da06 7374 7275  taticr......stru
+00000b20: 6374 5a06 7377 6974 6368 da04 7468 6973  ctZ.switch..this
+00000b30: da05 7468 726f 77da 0474 7275 65da 0374  ..throw..true..t
+00000b40: 7279 5a06 7479 7065 6f66 5a04 7569 6e74  ryZ.typeofZ.uint
+00000b50: 5a05 756c 6f6e 675a 0975 6e63 6865 636b  Z.ulongZ.uncheck
+00000b60: 6564 5a06 756e 7361 6665 5a06 7573 686f  edZ.unsafeZ.usho
+00000b70: 7274 5a05 7573 696e 675a 0776 6972 7475  rtZ.usingZ.virtu
+00000b80: 616c 5a04 766f 6964 5a08 766f 6c61 7469  alZ.voidZ.volati
+00000b90: 6c65 da05 7768 696c 65da 015f 7223 0000  le..while.._r#..
+00000ba0: 0029 0272 2900 0000 5a0e 7265 7365 7276  .).r)...Z.reserv
+00000bb0: 6564 5f77 6f72 6473 7223 0000 0072 2300  ed_wordsr#...r#.
+00000bc0: 0000 7224 0000 00da 1565 7363 6170 655f  ..r$.....escape_
+00000bd0: 7265 7365 7276 6564 5f77 6f72 6473 4400  reserved_wordsD.
+00000be0: 0000 7304 0000 0008 0116 0c72 4f00 0000  ..s........rO...
+00000bf0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000c00: 0004 0000 0040 0000 0073 4800 0000 6500  .....@...sH...e.
+00000c10: 5a01 6400 5a02 5500 6503 6504 6401 3c00  Z.d.Z.U.e.e.d.<.
+00000c20: 6503 6504 6402 3c00 6503 6504 6403 3c00  e.e.d.<.e.e.d.<.
+00000c30: 6503 6504 6404 3c00 6505 6405 6506 6602  e.e.d.<.e.d.e.f.
+00000c40: 6406 6407 8404 8301 5a07 6408 6409 8400  d.d.....Z.d.d...
+00000c50: 5a08 640a 5300 290b da0b 4353 6861 7270  Z.d.S.)...CSharp
+00000c60: 4669 656c 64da 0d6f 7269 6769 6e61 6c5f  Field..original_
+00000c70: 6e61 6d65 da0b 6373 6861 7270 5f6e 616d  name..csharp_nam
+00000c80: 65da 0474 7970 65da 0666 6f72 6d61 74da  e..type..format.
+00000c90: 0566 6965 6c64 6302 0000 0000 0000 0000  .fieldc.........
+00000ca0: 0000 0002 0000 0006 0000 0043 0000 0073  ...........C...s
+00000cb0: 2800 0000 7c00 7c01 6a00 7401 7402 7c01  (...|.|.j.t.t.|.
+00000cc0: 6a00 8301 8301 7403 7c01 6a04 8301 7405  j.....t.|.j...t.
+00000cd0: 7c01 6a04 8301 6401 8d04 5300 2902 4e29  |.j...d...S.).N)
+00000ce0: 0472 5100 0000 7252 0000 0072 5300 0000  .rQ...rR...rS...
+00000cf0: 7254 0000 0029 06da 046e 616d 6572 4f00  rT...)...namerO.
+00000d00: 0000 720f 0000 0072 2500 0000 da09 7661  ..r....r%.....va
+00000d10: 6c75 6554 7970 6572 2800 0000 2902 da03  lueTyper(...)...
+00000d20: 636c 7372 5500 0000 7223 0000 0072 2300  clsrU...r#...r#.
+00000d30: 0000 7224 0000 00da 1166 726f 6d5f 7374  ..r$.....from_st
+00000d40: 656c 6c61 5f66 6965 6c64 5b00 0000 730c  ella_field[...s.
+00000d50: 0000 0002 0204 010c 0108 0108 0106 fc7a  ...............z
+00000d60: 1d43 5368 6172 7046 6965 6c64 2e66 726f  .CSharpField.fro
+00000d70: 6d5f 7374 656c 6c61 5f66 6965 6c64 6301  m_stella_fieldc.
+00000d80: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00000d90: 0000 0043 0000 0073 1200 0000 7c00 6a00  ...C...s....|.j.
+00000da0: 9b00 6401 7c00 6a01 9b00 9d03 5300 2902  ..d.|.j.....S.).
+00000db0: 4efa 0120 2902 7253 0000 0072 5200 0000  N.. ).rS...rR...
+00000dc0: a901 da04 7365 6c66 7223 0000 0072 2300  ....selfr#...r#.
+00000dd0: 0000 7224 0000 00da 2474 6f5f 636f 6e73  ..r$....$to_cons
+00000de0: 7472 7563 746f 725f 7061 7261 6d65 7465  tructor_paramete
+00000df0: 725f 6465 636c 6172 6174 696f 6e64 0000  r_declarationd..
+00000e00: 0073 0200 0000 1201 7a30 4353 6861 7270  .s......z0CSharp
+00000e10: 4669 656c 642e 746f 5f63 6f6e 7374 7275  Field.to_constru
+00000e20: 6374 6f72 5f70 6172 616d 6574 6572 5f64  ctor_parameter_d
+00000e30: 6563 6c61 7261 7469 6f6e 4e29 09da 085f  eclarationN)..._
+00000e40: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00000e50: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00000e60: 5fda 0373 7472 da0f 5f5f 616e 6e6f 7461  _..str..__annota
+00000e70: 7469 6f6e 735f 5fda 0b63 6c61 7373 6d65  tions__..classme
+00000e80: 7468 6f64 7208 0000 0072 5900 0000 725d  thodr....rY...r]
+00000e90: 0000 0072 2300 0000 7223 0000 0072 2300  ...r#...r#...r#.
+00000ea0: 0000 7224 0000 0072 5000 0000 5400 0000  ..r$...rP...T...
+00000eb0: 7310 0000 000a 0008 0208 0108 0108 0102  s...............
+00000ec0: 0210 010c 0872 5000 0000 6300 0000 0000  .....rP...c.....
+00000ed0: 0000 0000 0000 0000 0000 0004 0000 0040  ...............@
+00000ee0: 0000 0073 4000 0000 6500 5a01 6400 5a02  ...s@...e.Z.d.Z.
+00000ef0: 5500 6503 6504 6401 3c00 6503 6504 6402  U.e.e.d.<.e.e.d.
+00000f00: 3c00 6505 6403 6506 6602 6404 6405 8404  <.e.d.e.f.d.d...
+00000f10: 8301 5a07 6406 6407 8400 5a08 6408 6409  ..Z.d.d...Z.d.d.
+00000f20: 8400 5a09 640a 5300 290b da0c 4353 6861  ..Z.d.S.)...CSha
+00000f30: 7270 456e 7469 7479 7251 0000 0072 5200  rpEntityrQ...rR.
+00000f40: 0000 da06 656e 7469 7479 6302 0000 0000  ....entityc.....
+00000f50: 0000 0000 0000 0002 0000 0005 0000 0043  ...............C
+00000f60: 0000 0073 1c00 0000 7c00 7c01 6a00 7401  ...s....|.|.j.t.
+00000f70: 7402 7c01 6a00 8301 8301 6401 1700 6402  t.|.j.....d...d.
+00000f80: 8d02 5300 2903 4e5a 0249 64a9 0272 5100  ..S.).NZ.Id..rQ.
+00000f90: 0000 7252 0000 0029 0372 5600 0000 724f  ..rR...).rV...rO
+00000fa0: 0000 0072 0f00 0000 2902 7258 0000 0072  ...r....).rX...r
+00000fb0: 6500 0000 7223 0000 0072 2300 0000 7224  e...r#...r#...r$
+00000fc0: 0000 0072 5900 0000 6d00 0000 7308 0000  ...rY...m...s...
+00000fd0: 0002 0204 0110 0106 fe7a 1e43 5368 6172  .........z.CShar
+00000fe0: 7045 6e74 6974 792e 6672 6f6d 5f73 7465  pEntity.from_ste
+00000ff0: 6c6c 615f 6669 656c 6463 0100 0000 0000  lla_fieldc......
+00001000: 0000 0000 0000 0100 0000 0500 0000 4300  ..............C.
+00001010: 0000 7316 0000 0064 017c 006a 009b 0064  ..s....d.|.j...d
+00001020: 027c 006a 019b 0064 039d 0553 0029 044e  .|.j...d...S.).N
+00001030: 7a10 6e65 7720 456e 7469 7479 5479 7065  z.new EntityType
+00001040: 2822 7a03 222c 20fa 0129 7266 0000 0072  ("z.", ..)rf...r
+00001050: 5b00 0000 7223 0000 0072 2300 0000 7224  [...r#...r#...r$
+00001060: 0000 00da 1a74 6f5f 656e 7469 7479 5f74  .....to_entity_t
+00001070: 7970 655f 6465 636c 6172 6174 696f 6e74  ype_declarationt
+00001080: 0000 0073 0200 0000 1601 7a27 4353 6861  ...s......z'CSha
+00001090: 7270 456e 7469 7479 2e74 6f5f 656e 7469  rpEntity.to_enti
+000010a0: 7479 5f74 7970 655f 6465 636c 6172 6174  ty_type_declarat
+000010b0: 696f 6e63 0100 0000 0000 0000 0000 0000  ionc............
+000010c0: 0100 0000 0200 0000 4300 0000 730c 0000  ........C...s...
+000010d0: 0064 017c 006a 009b 009d 0253 0029 024e  .d.|.j.....S.).N
+000010e0: 7a07 7374 7269 6e67 2029 0172 5200 0000  z.string ).rR...
+000010f0: 725b 0000 0072 2300 0000 7223 0000 0072  r[...r#...r#...r
+00001100: 2400 0000 725d 0000 0077 0000 0073 0200  $...r]...w...s..
+00001110: 0000 0c01 7a31 4353 6861 7270 456e 7469  ....z1CSharpEnti
+00001120: 7479 2e74 6f5f 636f 6e73 7472 7563 746f  ty.to_constructo
+00001130: 725f 7061 7261 6d65 7465 725f 6465 636c  r_parameter_decl
+00001140: 6172 6174 696f 6e4e 290a 725e 0000 0072  arationN).r^...r
+00001150: 5f00 0000 7260 0000 0072 6100 0000 7262  _...r`...ra...rb
+00001160: 0000 0072 6300 0000 7209 0000 0072 5900  ...rc...r....rY.
+00001170: 0000 7268 0000 0072 5d00 0000 7223 0000  ..rh...r]...r#..
+00001180: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
+00001190: 7264 0000 0068 0000 0073 0e00 0000 0a00  rd...h...s......
+000011a0: 0802 0801 0202 1001 0806 0c03 7264 0000  ............rd..
+000011b0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+000011c0: 0000 0800 0000 4000 0000 7356 0000 0065  ......@...sV...e
+000011d0: 005a 0164 005a 0265 0364 0165 0464 0265  .Z.d.Z.e.d.e.d.e
+000011e0: 0566 0464 0364 0484 0483 015a 0665 0364  .f.d.d.....Z.e.d
+000011f0: 0565 0564 0265 0566 0464 0664 0784 0483  .e.d.e.f.d.d....
+00001200: 015a 0765 0864 0165 0464 0865 0564 0265  .Z.e.d.e.d.e.d.e
+00001210: 0965 0519 0066 0664 0964 0a84 0483 015a  .e...f.d.d.....Z
+00001220: 0a64 0b53 0029 0cda 1343 7368 6172 7043  .d.S.)...CsharpC
+00001230: 6f64 6547 656e 6572 6174 6f72 7236 0000  odeGeneratorr6..
+00001240: 0072 1200 0000 6301 0000 0000 0000 0000  .r....c.........
+00001250: 0000 0007 0000 000c 0000 004b 0000 0073  ...........K...s
+00001260: bc00 0000 7400 a001 6401 a101 7d02 7c01  ....t...d...}.|.
+00001270: a002 6402 6403 a102 7d03 6404 6405 8400  ..d.d...}.d.d...
+00001280: 7c00 6a03 4400 8301 7d04 6406 6405 8400  |.j.D...}.d.d...
+00001290: 7c00 6a04 4400 8301 7d05 7c05 7320 7405  |.j.D...}.|.s t.
+000012a0: 8300 8201 7c02 6a06 7407 7c00 6a08 8301  ....|.j.t.|.j...
+000012b0: 7c00 6a08 6407 a009 6407 a009 6408 6405  |.j.d...d...d.d.
+000012c0: 8400 7c05 4400 8301 a101 6407 a009 6409  ..|.D.....d...d.
+000012d0: 6405 8400 7c04 4400 8301 a101 6702 a101  d...|.D.....g...
+000012e0: 6407 a009 640a 6405 8400 7c05 4400 8301  d...d.d...|.D...
+000012f0: a101 7c04 7c03 740a 6a0b 740c 7c00 8301  ..|.|.t.j.t.|...
+00001300: 640b 640c 8d02 7c00 6a0d 740e a00f a100  d.d...|.j.t.....
+00001310: a010 640d a101 640e 8d09 7d06 7c06 5300  ..d...d...}.|.S.
+00001320: 290f 4e5a 0663 7368 6172 7072 3f00 0000  ).NZ.csharpr?...
+00001330: 7a15 5374 656c 6c61 4e6f 7753 444b 2e4d  z.StellaNowSDK.M
+00001340: 6573 7361 6765 7363 0100 0000 0000 0000  essagesc........
+00001350: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
+00001360: f316 0000 0067 007c 005d 077d 0174 00a0  .....g.|.].}.t..
+00001370: 017c 01a1 0191 0271 0253 0072 2300 0000  .|.....q.S.r#...
+00001380: 2902 7250 0000 0072 5900 0000 a902 da02  ).rP...rY.......
+00001390: 2e30 7255 0000 0072 2300 0000 7223 0000  .0rU...r#...r#..
+000013a0: 0072 2400 0000 da0a 3c6c 6973 7463 6f6d  .r$.....<listcom
+000013b0: 703e 8200 0000 f302 0000 0016 007a 3643  p>...........z6C
+000013c0: 7368 6172 7043 6f64 6547 656e 6572 6174  sharpCodeGenerat
+000013d0: 6f72 2e67 656e 6572 6174 655f 636c 6173  or.generate_clas
+000013e0: 732e 3c6c 6f63 616c 733e 2e3c 6c69 7374  s.<locals>.<list
+000013f0: 636f 6d70 3e63 0100 0000 0000 0000 0000  comp>c..........
+00001400: 0000 0200 0000 0500 0000 5300 0000 726a  ..........S...rj
+00001410: 0000 0072 2300 0000 2902 7264 0000 0072  ...r#...).rd...r
+00001420: 5900 0000 a902 726c 0000 0072 6500 0000  Y.....rl...re...
+00001430: 7223 0000 0072 2300 0000 7224 0000 0072  r#...r#...r$...r
+00001440: 6d00 0000 8300 0000 726e 0000 007a 022c  m.......rn...z.,
+00001450: 2063 0100 0000 0000 0000 0000 0000 0200   c..............
+00001460: 0000 0400 0000 5300 0000 f314 0000 0067  ......S........g
+00001470: 007c 005d 067d 017c 01a0 00a1 0091 0271  .|.].}.|.......q
+00001480: 0253 0072 2300 0000 a901 725d 0000 0072  .S.r#.....r]...r
+00001490: 6f00 0000 7223 0000 0072 2300 0000 7224  o...r#...r#...r$
+000014a0: 0000 0072 6d00 0000 8b00 0000 f302 0000  ...rm...........
+000014b0: 0014 0063 0100 0000 0000 0000 0000 0000  ...c............
+000014c0: 0200 0000 0400 0000 5300 0000 7270 0000  ........S...rp..
+000014d0: 0072 2300 0000 7271 0000 0072 6b00 0000  .r#...rq...rk...
+000014e0: 7223 0000 0072 2300 0000 7224 0000 0072  r#...r#...r$...r
+000014f0: 6d00 0000 8c00 0000 7272 0000 0063 0100  m.......rr...c..
+00001500: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00001510: 0000 5300 0000 7270 0000 0072 2300 0000  ..S...rp...r#...
+00001520: 2901 7268 0000 0072 6f00 0000 7223 0000  ).rh...ro...r#..
+00001530: 0072 2300 0000 7224 0000 0072 6d00 0000  .r#...r$...rm...
+00001540: 8e00 0000 7272 0000 00e9 0400 0000 2901  ....rr........).
+00001550: da06 696e 6465 6e74 7a12 2559 2d25 6d2d  ..indentz.%Y-%m-
+00001560: 2564 5425 483a 254d 3a25 535a 2909 da09  %dT%H:%M:%SZ)...
+00001570: 636c 6173 734e 616d 655a 0965 7665 6e74  classNameZ.event
+00001580: 4e61 6d65 5a14 636f 6e73 7472 7563 746f  NameZ.constructo
+00001590: 7241 7267 756d 656e 7473 5a0c 656e 7469  rArgumentsZ.enti
+000015a0: 7469 6573 4c69 7374 da06 6669 656c 6473  tiesList..fields
+000015b0: 723f 0000 005a 0965 7665 6e74 4a73 6f6e  r?...Z.eventJson
+000015c0: 5a07 6576 656e 7449 64da 0974 696d 6573  Z.eventId..times
+000015d0: 7461 6d70 2911 7269 0000 005a 0d6c 6f61  tamp).ri...Z.loa
+000015e0: 645f 7465 6d70 6c61 7465 7220 0000 0072  d_templater ...r
+000015f0: 7600 0000 da08 656e 7469 7469 6573 720d  v.....entitiesr.
+00001600: 0000 005a 0672 656e 6465 7272 0e00 0000  ...Z.renderr....
+00001610: 7256 0000 00da 046a 6f69 6eda 046a 736f  rV.....join..jso
+00001620: 6eda 0564 756d 7073 7202 0000 00da 0269  n..dumpsr......i
+00001630: 6472 0400 0000 da06 7574 636e 6f77 da08  dr......utcnow..
+00001640: 7374 7266 7469 6d65 2907 7236 0000 00da  strftime).r6....
+00001650: 066b 7761 7267 73da 0874 656d 706c 6174  .kwargs..templat
+00001660: 6572 3f00 0000 7276 0000 0072 7800 0000  er?...rv...rx...
+00001670: da08 7265 6e64 6572 6564 7223 0000 0072  ..renderedr#...r
+00001680: 2300 0000 7224 0000 00da 0e67 656e 6572  #...r$.....gener
+00001690: 6174 655f 636c 6173 737c 0000 0073 2a00  ate_class|...s*.
+000016a0: 0000 0a02 0c02 1002 1001 0401 0601 0402  ................
+000016b0: 0801 0401 0401 1201 1201 04fe 1204 0201  ................
+000016c0: 0201 1001 0401 0c01 06f4 040f 7a22 4373  ............z"Cs
+000016d0: 6861 7270 436f 6465 4765 6e65 7261 746f  harpCodeGenerato
+000016e0: 722e 6765 6e65 7261 7465 5f63 6c61 7373  r.generate_class
+000016f0: da0a 6576 656e 745f 6e61 6d65 6301 0000  ..event_namec...
+00001700: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00001710: 0043 0000 0073 0e00 0000 7400 7c00 8301  .C...s....t.|...
+00001720: 9b00 6401 9d02 5300 2902 4e7a 0a4d 6573  ..d...S.).Nz.Mes
+00001730: 7361 6765 2e63 7329 0172 0e00 0000 2901  sage.cs).r....).
+00001740: 7283 0000 0072 2300 0000 7223 0000 0072  r....r#...r#...r
+00001750: 2400 0000 da1c 6765 745f 6669 6c65 5f6e  $.....get_file_n
+00001760: 616d 655f 666f 725f 6576 656e 745f 6e61  ame_for_event_na
+00001770: 6d65 9800 0000 7302 0000 000e 027a 3043  me....s......z0C
+00001780: 7368 6172 7043 6f64 6547 656e 6572 6174  sharpCodeGenerat
+00001790: 6f72 2e67 6574 5f66 696c 655f 6e61 6d65  or.get_file_name
+000017a0: 5f66 6f72 5f65 7665 6e74 5f6e 616d 65da  _for_event_name.
+000017b0: 0d65 7869 7374 696e 675f 636f 6465 6303  .existing_codec.
+000017c0: 0000 0000 0000 0000 0000 0009 0000 0006  ................
+000017d0: 0000 0043 0000 0073 7400 0000 7400 a001  ...C...st...t...
+000017e0: 6401 7c02 a102 7d03 7c03 6400 7500 720d  d.|...}.|.d.u.r.
+000017f0: 7402 8300 8201 7c03 a003 6402 a101 7d04  t.....|...d...}.
+00001800: 7c00 6a04 7c01 6601 6900 6403 7c04 6901  |.j.|.f.i.d.|.i.
+00001810: a401 8e01 7d05 7405 7c02 8301 7d06 7405  ....}.t.|...}.t.
+00001820: 7c05 8301 7d07 7406 a007 7c06 6a08 6404  |...}.t...|.j.d.
+00001830: 6405 8d01 7c07 6a08 6404 6405 8d01 a102  d...|.j.d.d.....
+00001840: 7d08 6406 6407 8400 7c08 4400 8301 5300  }.d.d...|.D...S.
+00001850: 2908 4e7a 0f6e 616d 6573 7061 6365 2028  ).Nz.namespace (
+00001860: 2e2a 293b 720a 0000 0072 3f00 0000 5429  .*);r....r?...T)
+00001870: 01da 086b 6565 7065 6e64 7363 0100 0000  ...keependsc....
+00001880: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00001890: 7300 0000 733c 0000 0081 007c 005d 197d  s...s<.....|.].}
+000018a0: 017c 01a0 0064 00a1 0173 187c 01a0 0064  .|...d...s.|...d
+000018b0: 01a1 0172 027c 01a0 0064 02a1 0173 027c  ...r.|...d...s.|
+000018c0: 01a0 0064 03a1 0173 027c 0156 0001 0071  ...d...s.|.V...q
+000018d0: 0264 0453 0029 057a 022d 207a 022b 207a  .d.S.).z.- z.+ z
+000018e0: 032d 2d2d 7a03 2b2b 2b4e 2901 da0a 7374  .---z.+++N)...st
+000018f0: 6172 7473 7769 7468 2902 726c 0000 00da  artswith).rl....
+00001900: 046c 696e 6572 2300 0000 7223 0000 0072  .liner#...r#...r
+00001910: 2400 0000 da09 3c67 656e 6578 7072 3eae  $.....<genexpr>.
+00001920: 0000 0073 0c00 0000 0280 1a00 0801 02ff  ...s............
+00001930: 0801 0eff 7a2f 4373 6861 7270 436f 6465  ....z/CsharpCode
+00001940: 4765 6e65 7261 746f 722e 6765 745f 6469  Generator.get_di
+00001950: 6666 2e3c 6c6f 6361 6c73 3e2e 3c67 656e  ff.<locals>.<gen
+00001960: 6578 7072 3e29 09da 0272 65da 0673 6561  expr>)...re..sea
+00001970: 7263 6872 0c00 0000 da05 6772 6f75 7072  rchr......groupr
+00001980: 8200 0000 7210 0000 00da 0764 6966 666c  ....r......diffl
+00001990: 6962 da0c 756e 6966 6965 645f 6469 6666  ib..unified_diff
+000019a0: da0a 7370 6c69 746c 696e 6573 2909 7258  ..splitlines).rX
+000019b0: 0000 0072 3600 0000 7285 0000 005a 106e  ...r6...r....Z.n
+000019c0: 616d 6573 7061 6365 5f73 6561 7263 6872  amespace_searchr
+000019d0: 3f00 0000 5a08 6e65 775f 636f 6465 5a19  ?...Z.new_codeZ.
+000019e0: 6578 6973 7469 6e67 5f63 6f64 655f 6e6f  existing_code_no
+000019f0: 5f63 6f6d 6d65 6e74 735a 146e 6577 5f63  _commentsZ.new_c
+00001a00: 6f64 655f 6e6f 5f63 6f6d 6d65 6e74 73da  ode_no_comments.
+00001a10: 0464 6966 6672 2300 0000 7223 0000 0072  .diffr#...r#...r
+00001a20: 2400 0000 da08 6765 745f 6469 6666 9c00  $.....get_diff..
+00001a30: 0000 7316 0000 000c 0308 0106 010a 0216  ..s.............
+00001a40: 0208 0208 010e 030a 0104 ff0e 037a 1c43  .............z.C
+00001a50: 7368 6172 7043 6f64 6547 656e 6572 6174  sharpCodeGenerat
+00001a60: 6f72 2e67 6574 5f64 6966 664e 290b 725e  or.get_diffN).r^
+00001a70: 0000 0072 5f00 0000 7260 0000 00da 0c73  ...r_...r`.....s
+00001a80: 7461 7469 636d 6574 686f 6472 0700 0000  taticmethodr....
+00001a90: 7261 0000 0072 8200 0000 7284 0000 0072  ra...r....r....r
+00001aa0: 6300 0000 7205 0000 0072 9100 0000 7223  c...r....r....r#
+00001ab0: 0000 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
+00001ac0: 0000 7269 0000 007b 0000 0073 0e00 0000  ..ri...{...s....
+00001ad0: 0800 0201 1401 021b 1401 0203 2001 7269  ............ .ri
+00001ae0: 0000 0029 22da 075f 5f64 6f63 5f5f 728d  ...)"..__doc__r.
+00001af0: 0000 0072 7a00 0000 5a07 6c6f 6767 696e  ...rz...Z.loggin
+00001b00: 6772 8a00 0000 da0b 6461 7461 636c 6173  gr......dataclas
+00001b10: 7365 7372 0200 0000 7203 0000 0072 0400  sesr....r....r..
+00001b20: 0000 da06 7479 7069 6e67 7205 0000 005a  ....typingr....Z
+00001b30: 0361 7069 7207 0000 0072 0800 0000 7209  .apir....r....r.
+00001b40: 0000 005a 0e63 6f64 655f 6765 6e65 7261  ...Z.code_genera
+00001b50: 746f 7272 0b00 0000 5a19 6578 6365 7074  torr....Z.except
+00001b60: 696f 6e73 2e63 6c69 5f65 7863 6570 7469  ions.cli_excepti
+00001b70: 6f6e 7372 0c00 0000 720d 0000 005a 0b75  onsr....r....Z.u
+00001b80: 7469 6c73 2e75 7469 6c73 720e 0000 0072  tils.utilsr....r
+00001b90: 0f00 0000 7210 0000 005a 0967 6574 4c6f  ....r....Z.getLo
+00001ba0: 6767 6572 725e 0000 00da 066c 6f67 6765  ggerr^.....logge
+00001bb0: 7272 6100 0000 7225 0000 0072 2800 0000  rra...r%...r(...
+00001bc0: 724f 0000 0072 5000 0000 7264 0000 0072  rO...rP...rd...r
+00001bd0: 6900 0000 7223 0000 0072 2300 0000 7223  i...r#...r#...r#
+00001be0: 0000 0072 2400 0000 da08 3c6d 6f64 756c  ...r$.....<modul
+00001bf0: 653e 0100 0000 732a 0000 0004 0008 1608  e>....s*........
+00001c00: 0108 0108 0110 020c 010c 0114 020c 0110  ................
+00001c10: 0114 040a 0312 0312 0c12 0c02 1010 0102  ................
+00001c20: 1310 0114 12                             .....
```

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/code_generator.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/code_generator.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/csharp_code_generator.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/csharp_code_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 from dataclasses import asdict, dataclass
 from datetime import datetime
 from typing import Iterator
 
 from ..api import StellaEventDetailed, StellaField, StellaEntity
 from .code_generator import CodeGenerator
-from ..exceptions.StellaNowCLIException import (
+from ..exceptions.cli_exceptions import (
     StellaNowCLINamespaceNotFoundException,
     StellaNowCLINoEntityAssociatedWithEventException
 )
 from ..utils.utils import snake_to_camel, snake_to_lower_camel, remove_comments
 
 
 logger = logging.getLogger(__name__)
@@ -74,15 +74,15 @@
         "long", "namespace", "new", "null", "object", "operator", "out", "override", "params",
         "private", "protected", "public", "readonly", "ref", "return", "sbyte", "sealed",
         "short", "sizeof", "stackalloc", "static", "string", "struct", "switch", "this", "throw",
         "true", "try", "typeof", "uint", "ulong", "unchecked", "unsafe", "ushort", "using", "virtual",
         "void", "volatile", "while"
     ]
 
-    return word + "_" if word in reserved_words else word
+    return f"{word}_" if word in reserved_words else word
 
 
 @dataclass
 class CSharpField:
     original_name: str
     csharp_name: str
     type: str
```

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/code_generators/templates/csharp.template` & `stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/templates/csharp.template`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/commands/__pycache__/command_config.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/commands/__pycache__/command_config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 27 15:44:32 2023 UTC, .py size: 4607 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e003 9b64 ff11 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 99c8 9e64 0912 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6403 6404 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 0100 6403 6405 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 0100 6503 a00a 650b a101 5a0c 6501 6a0d  ..e...e...Z.e.j.
@@ -108,127 +108,127 @@
 000006b0: 6c61 6e6f 775f 636c 692f 636f 6d6d 616e  lanow_cli/comman
 000006c0: 6473 2f63 6f6e 6669 6775 7265 2e70 79da  ds/configure.py.
 000006d0: 0a3c 6c69 7374 636f 6d70 3e27 0000 0073  .<listcomp>'...s
 000006e0: 0200 0000 1200 7210 0000 0029 01da 0e63  ......r....)...c
 000006f0: 6173 655f 7365 6e73 6974 6976 6529 02da  ase_sensitive)..
 00000700: 0668 6964 6465 6eda 0474 7970 6563 0300  .hidden..typec..
 00000710: 0000 0000 0000 0000 0000 0d00 0000 0800  ................
-00000720: 0000 4300 0000 73cc 0100 0074 0064 017c  ..C...s....t.d.|
-00000730: 019b 009d 0283 0101 007c 006a 017d 037c  .........|.j.}.|
-00000740: 036a 027c 0164 0264 0364 048d 037d 047c  .j.|.d.d.d...}.|
-00000750: 036a 027c 0164 0564 0364 048d 037d 057c  .j.|.d.d.d...}.|
-00000760: 036a 027c 0164 0664 0364 048d 037d 067c  .j.|.d.d.d...}.|
-00000770: 036a 027c 0164 0764 0364 048d 037d 0764  .j.|.d.d.d...}.d
-00000780: 087d 0864 097d 0909 0074 036a 0464 0b7c  .}.d.}...t.j.d.|
-00000790: 0464 0c8d 027d 0474 05a0 067c 087c 04a1  .d...}.t...|.|..
-000007a0: 0273 4274 05a0 067c 097c 04a1 0272 436e  .sBt...|.|...rCn
-000007b0: 0674 07a0 0864 0da1 0101 0071 2f09 0074  .t...d.....q/..t
-000007c0: 036a 0464 0e64 0a7c 0564 0f64 108d 047d  .j.d.d.|.d.d...}
-000007d0: 0574 05a0 0664 117c 05a1 0272 5a6e 0674  .t...d.|...rZn.t
-000007e0: 07a0 0864 12a1 0101 0071 4a09 0074 036a  ...d.....qJ..t.j
-000007f0: 0464 137c 0664 0c8d 027d 0674 097c 0683  .d.|.d...}.t.|..
-00000800: 0172 6d6e 0674 07a0 0864 14a1 0101 0071  .rmn.t...d.....q
-00000810: 6109 0074 036a 0464 157c 0764 0c8d 027d  a..t.j.d.|.d...}
-00000820: 0774 097c 0783 0172 806e 0674 07a0 0864  .t.|...r.n.t...d
-00000830: 14a1 0101 0071 7474 0a6a 0ba0 0c64 16a1  .....qtt.j...d..
-00000840: 017d 0a74 0a6a 0d74 0a6a 0ba0 0e7c 0a64  .}.t.j.t.j...|.d
-00000850: 17a1 0264 0a64 188d 0201 0074 0fa0 10a1  ...d.d.....t....
-00000860: 007d 0374 0a6a 0ba0 0e7c 0a64 1764 19a1  .}.t.j...|.d.d..
-00000870: 037d 0b74 0a6a 0ba0 117c 0ba1 0172 af7c  .}.t.j...|...r.|
-00000880: 03a0 127c 0ba1 0101 007c 047c 057c 067c  ...|.....|.|.|.|
-00000890: 0764 1a9c 047c 037c 013c 007c 0264 0375  .d...|.|.<.|.d.u
-000008a0: 0172 c27c 027c 037c 0119 0064 1b3c 0074  .r.|.|.|...d.<.t
-000008b0: 137c 0b64 1c83 028f 0d7d 0c7c 03a0 147c  .|.d.....}.|...|
-000008c0: 0ca1 0101 0057 0064 0304 0004 0083 0301  .....W.d........
-000008d0: 006e 0831 0073 d777 0101 0001 0001 0059  .n.1.s.w.......Y
-000008e0: 0001 0074 0064 1d7c 019b 0064 1e9d 0383  ...t.d.|...d....
-000008f0: 0101 0064 0353 0029 1f7a 8053 6574 7320  ...d.S.).z.Sets 
-00000900: 7570 2074 6865 206e 6563 6573 7361 7279  up the necessary
-00000910: 2063 7265 6465 6e74 6961 6c73 2061 6e64   credentials and
-00000920: 2063 6f6e 6669 6775 7261 7469 6f6e 7320   configurations 
-00000930: 666f 7220 6120 7370 6563 6966 6963 2070  for a specific p
-00000940: 726f 6669 6c65 206f 7220 666f 7220 7468  rofile or for th
-00000950: 6520 4445 4641 554c 5420 7072 6f66 696c  e DEFAULT profil
-00000960: 6520 6966 206e 6f6e 650a 2020 2020 6973  e if none.    is
-00000970: 2073 7065 6369 6669 6564 2e7a 2350 726f   specified.z#Pro
-00000980: 7669 6465 2063 6f6e 6669 6775 7261 7469  vide configurati
-00000990: 6f6e 2066 6f72 2070 726f 6669 6c65 3a20  on for profile: 
-000009a0: da0a 6163 6365 7373 5f6b 6579 4e29 01da  ..access_keyN)..
-000009b0: 0866 616c 6c62 6163 6bda 0c61 6363 6573  .fallback..acces
-000009c0: 735f 746f 6b65 6eda 0f6f 7267 616e 697a  s_token..organiz
-000009d0: 6174 696f 6e5f 6964 da0a 7072 6f6a 6563  ation_id..projec
-000009e0: 745f 6964 7a33 5c62 5b41 2d5a 612d 7a30  t_idz3\b[A-Za-z0
-000009f0: 2d39 2e5f 252b 2d5d 2b40 5b41 2d5a 612d  -9._%+-]+@[A-Za-
-00000a00: 7a30 2d39 2e2d 5d2b 5c2e 5b41 2d5a 7c61  z0-9.-]+\.[A-Z|a
-00000a10: 2d7a 5d7b 322c 7d5c 627a 105e 5b61 2d7a  -z]{2,}\bz.^[a-z
-00000a20: 412d 5a30 2d39 5f2d 5d2b 2454 7a0a 4163  A-Z0-9_-]+$Tz.Ac
-00000a30: 6365 7373 204b 6579 2901 7208 0000 007a  cess Key).r....z
-00000a40: 8b49 6e76 616c 6964 2061 6363 6573 7320  .Invalid access 
-00000a50: 6b65 7920 666f 726d 6174 2e20 4974 2073  key format. It s
-00000a60: 686f 756c 6420 6265 2061 2076 616c 6964  hould be a valid
-00000a70: 2065 6d61 696c 2061 6464 7265 7373 206f   email address o
-00000a80: 7220 6120 7374 7269 6e67 2063 6f6e 7461  r a string conta
-00000a90: 696e 696e 6720 6f6e 6c79 2061 6c70 6861  ining only alpha
-00000aa0: 6e75 6d65 7269 6320 6368 6172 6163 7465  numeric characte
-00000ab0: 7273 2c20 6461 7368 6573 2c20 616e 6420  rs, dashes, and 
-00000ac0: 756e 6465 7273 636f 7265 732e 7a0c 4163  underscores.z.Ac
-00000ad0: 6365 7373 2054 6f6b 656e 4629 03da 0a68  cess TokenF)...h
-00000ae0: 6964 655f 696e 7075 7472 0800 0000 da0c  ide_inputr......
-00000af0: 7368 6f77 5f64 6566 6175 6c74 7a0a 5e5c  show_defaultz.^\
-00000b00: 537b 382c 3634 7d24 7a59 496e 7661 6c69  S{8,64}$zYInvali
-00000b10: 6420 6163 6365 7373 2074 6f6b 656e 2066  d access token f
-00000b20: 6f72 6d61 742e 2049 7420 7368 6f75 6c64  ormat. It should
-00000b30: 2063 6f6e 7461 696e 206e 6f20 7768 6974   contain no whit
-00000b40: 6573 7061 6365 2061 6e64 2062 6520 382d  espace and be 8-
-00000b50: 3634 2063 6861 7261 6374 6572 7320 6c6f  64 characters lo
-00000b60: 6e67 2e7a 0f4f 7267 616e 697a 6174 696f  ng.z.Organizatio
-00000b70: 6e20 4944 7a33 496e 7661 6c69 6420 6f72  n IDz3Invalid or
-00000b80: 6761 6e69 7a61 7469 6f6e 2049 442e 2049  ganization ID. I
-00000b90: 7420 7368 6f75 6c64 2062 6520 6120 7661  t should be a va
-00000ba0: 6c69 6420 5555 4944 2e7a 0a50 726f 6a65  lid UUID.z.Proje
-00000bb0: 6374 2049 44fa 017e 7a0a 2e73 7465 6c6c  ct ID..~z..stell
-00000bc0: 616e 6f77 2901 da08 6578 6973 745f 6f6b  anow)...exist_ok
-00000bd0: 7a0a 636f 6e66 6967 2e69 6e69 2904 7214  z.config.ini).r.
-00000be0: 0000 0072 1600 0000 7217 0000 0072 1800  ...r....r....r..
-00000bf0: 0000 da03 656e 76da 0177 7a1b 436f 6e66  ....env..wz.Conf
-00000c00: 6967 7572 6174 696f 6e20 666f 7220 7072  iguration for pr
-00000c10: 6f66 696c 6520 277a 1427 2073 6176 6564  ofile 'z.' saved
-00000c20: 2073 7563 6365 7373 6675 6c6c 7929 15da   successfully)..
-00000c30: 0570 7269 6e74 da03 6f62 6ada 0367 6574  .print..obj..get
-00000c40: da05 636c 6963 6b72 0900 0000 da02 7265  ..clickr......re
-00000c50: da05 6d61 7463 68da 066c 6f67 6765 72da  ..match..logger.
-00000c60: 0565 7272 6f72 7203 0000 00da 026f 73da  .errorr......os.
-00000c70: 0470 6174 68da 0a65 7870 616e 6475 7365  .path..expanduse
-00000c80: 72da 086d 616b 6564 6972 73da 046a 6f69  r..makedirs..joi
-00000c90: 6eda 0c63 6f6e 6669 6770 6172 7365 72da  n..configparser.
-00000ca0: 0c43 6f6e 6669 6750 6172 7365 72da 0665  .ConfigParser..e
-00000cb0: 7869 7374 73da 0472 6561 64da 046f 7065  xists..read..ope
-00000cc0: 6eda 0577 7269 7465 290d da03 6374 785a  n..write)...ctxZ
-00000cd0: 0770 726f 6669 6c65 721d 0000 00da 0663  .profiler......c
-00000ce0: 6f6e 6669 6772 1400 0000 7216 0000 0072  onfigr....r....r
-00000cf0: 1700 0000 7218 0000 005a 0b65 6d61 696c  ....r....Z.email
-00000d00: 5f72 6567 6578 5a0c 7374 7269 6e67 5f72  _regexZ.string_r
-00000d10: 6567 6578 da04 686f 6d65 5a0b 636f 6e66  egex..homeZ.conf
-00000d20: 6967 5f66 696c 655a 0a63 6f6e 6669 6766  ig_fileZ.configf
-00000d30: 696c 6572 0b00 0000 720b 0000 0072 0f00  iler....r....r..
-00000d40: 0000 7205 0000 0023 0000 0073 6200 0000  ..r....#...sb...
-00000d50: 0e0a 0602 1002 1001 1001 1001 0402 0401  ................
-00000d60: 0201 0e01 1801 0201 0a02 02fb 0208 1201  ................
-00000d70: 0c01 0201 0a02 02fb 0207 0e01 0801 0201  ................
-00000d80: 0a02 02fb 0207 0e01 0801 0201 0a02 02fb  ................
-00000d90: 0c08 1803 0803 1003 0c01 0a01 0204 0201  ................
-00000da0: 0201 0201 0afc 0808 0c01 0c03 0c01 1cff  ................
-00000db0: 1403 2913 da07 5f5f 646f 635f 5f72 2200  ..)...__doc__r".
-00000dc0: 0000 722c 0000 005a 076c 6f67 6769 6e67  ..r,...Z.logging
-00000dd0: 7227 0000 0072 2300 0000 5a0b 7574 696c  r'...r#...Z.util
-00000de0: 732e 7574 696c 7372 0300 0000 7233 0000  s.utilsr....r3..
-00000df0: 0072 0400 0000 5a09 6765 744c 6f67 6765  .r....Z.getLogge
-00000e00: 72da 085f 5f6e 616d 655f 5f72 2500 0000  r..__name__r%...
-00000e10: da07 636f 6d6d 616e 64da 066f 7074 696f  ..command..optio
-00000e20: 6eda 0643 686f 6963 65da 0c70 6173 735f  n..Choice..pass_
-00000e30: 636f 6e74 6578 7472 0500 0000 da0d 636f  contextr......co
-00000e40: 6e66 6967 7572 655f 636d 6472 0b00 0000  nfigure_cmdr....
-00000e50: 720b 0000 0072 0b00 0000 720f 0000 00da  r....r....r.....
-00000e60: 083c 6d6f 6475 6c65 3e01 0000 0073 2200  .<module>....s".
-00000e70: 0000 0400 0816 0801 0801 0801 0801 0c02  ................
-00000e80: 0c01 0a02 0a03 0a01 0201 04ff 2203 0401  ............"...
-00000e90: 1001 084d                                ...M
+00000720: 0000 4300 0000 73d0 0100 0074 00a0 0164  ..C...s....t...d
+00000730: 017c 019b 009d 02a1 0101 007c 006a 027d  .|.........|.j.}
+00000740: 037c 036a 037c 0164 0264 0364 048d 037d  .|.j.|.d.d.d...}
+00000750: 047c 036a 037c 0164 0564 0364 048d 037d  .|.j.|.d.d.d...}
+00000760: 057c 036a 037c 0164 0664 0364 048d 037d  .|.j.|.d.d.d...}
+00000770: 067c 036a 037c 0164 0764 0364 048d 037d  .|.j.|.d.d.d...}
+00000780: 0764 087d 0864 097d 0909 0074 006a 0464  .d.}.d.}...t.j.d
+00000790: 0b7c 0464 0c8d 027d 0474 05a0 067c 087c  .|.d...}.t...|.|
+000007a0: 04a1 0273 4374 05a0 067c 097c 04a1 0272  ...sCt...|.|...r
+000007b0: 446e 0674 07a0 0864 0da1 0101 0071 3009  Dn.t...d.....q0.
+000007c0: 0074 006a 0464 0e64 0a7c 0564 0f64 108d  .t.j.d.d.|.d.d..
+000007d0: 047d 0574 05a0 0664 117c 05a1 0272 5b6e  .}.t...d.|...r[n
+000007e0: 0674 07a0 0864 12a1 0101 0071 4b09 0074  .t...d.....qK..t
+000007f0: 006a 0464 137c 0664 0c8d 027d 0674 097c  .j.d.|.d...}.t.|
+00000800: 0683 0172 6e6e 0674 07a0 0864 14a1 0101  ...rnn.t...d....
+00000810: 0071 6209 0074 006a 0464 157c 0764 0c8d  .qb..t.j.d.|.d..
+00000820: 027d 0774 097c 0783 0172 816e 0674 07a0  .}.t.|...r.n.t..
+00000830: 0864 14a1 0101 0071 7574 0a6a 0ba0 0c64  .d.....qut.j...d
+00000840: 16a1 017d 0a74 0a6a 0d74 0a6a 0ba0 0e7c  ...}.t.j.t.j...|
+00000850: 0a64 17a1 0264 0a64 188d 0201 0074 0fa0  .d...d.d.....t..
+00000860: 10a1 007d 0374 0a6a 0ba0 0e7c 0a64 1764  ...}.t.j...|.d.d
+00000870: 19a1 037d 0b74 0a6a 0ba0 117c 0ba1 0172  ...}.t.j...|...r
+00000880: b07c 03a0 127c 0ba1 0101 007c 047c 057c  .|...|.....|.|.|
+00000890: 067c 0764 1a9c 047c 037c 013c 007c 0264  .|.d...|.|.<.|.d
+000008a0: 0375 0172 c37c 027c 037c 0119 0064 1b3c  .u.r.|.|.|...d.<
+000008b0: 0074 137c 0b64 1c83 028f 0d7d 0c7c 03a0  .t.|.d.....}.|..
+000008c0: 147c 0ca1 0101 0057 0064 0304 0004 0083  .|.....W.d......
+000008d0: 0301 006e 0831 0073 d877 0101 0001 0001  ...n.1.s.w......
+000008e0: 0059 0001 0074 00a0 0164 1d7c 019b 0064  .Y...t...d.|...d
+000008f0: 1e9d 03a1 0101 0064 0353 0029 1f7a 8053  .......d.S.).z.S
+00000900: 6574 7320 7570 2074 6865 206e 6563 6573  ets up the neces
+00000910: 7361 7279 2063 7265 6465 6e74 6961 6c73  sary credentials
+00000920: 2061 6e64 2063 6f6e 6669 6775 7261 7469   and configurati
+00000930: 6f6e 7320 666f 7220 6120 7370 6563 6966  ons for a specif
+00000940: 6963 2070 726f 6669 6c65 206f 7220 666f  ic profile or fo
+00000950: 7220 7468 6520 4445 4641 554c 5420 7072  r the DEFAULT pr
+00000960: 6f66 696c 6520 6966 206e 6f6e 650a 2020  ofile if none.  
+00000970: 2020 6973 2073 7065 6369 6669 6564 2e7a    is specified.z
+00000980: 2350 726f 7669 6465 2063 6f6e 6669 6775  #Provide configu
+00000990: 7261 7469 6f6e 2066 6f72 2070 726f 6669  ration for profi
+000009a0: 6c65 3a20 da0a 6163 6365 7373 5f6b 6579  le: ..access_key
+000009b0: 4e29 01da 0866 616c 6c62 6163 6bda 0c61  N)...fallback..a
+000009c0: 6363 6573 735f 746f 6b65 6eda 0f6f 7267  ccess_token..org
+000009d0: 616e 697a 6174 696f 6e5f 6964 da0a 7072  anization_id..pr
+000009e0: 6f6a 6563 745f 6964 7a33 5c62 5b41 2d5a  oject_idz3\b[A-Z
+000009f0: 612d 7a30 2d39 2e5f 252b 2d5d 2b40 5b41  a-z0-9._%+-]+@[A
+00000a00: 2d5a 612d 7a30 2d39 2e2d 5d2b 5c2e 5b41  -Za-z0-9.-]+\.[A
+00000a10: 2d5a 7c61 2d7a 5d7b 322c 7d5c 627a 105e  -Z|a-z]{2,}\bz.^
+00000a20: 5b61 2d7a 412d 5a30 2d39 5f2d 5d2b 2454  [a-zA-Z0-9_-]+$T
+00000a30: 7a0a 4163 6365 7373 204b 6579 2901 7208  z.Access Key).r.
+00000a40: 0000 007a 8b49 6e76 616c 6964 2061 6363  ...z.Invalid acc
+00000a50: 6573 7320 6b65 7920 666f 726d 6174 2e20  ess key format. 
+00000a60: 4974 2073 686f 756c 6420 6265 2061 2076  It should be a v
+00000a70: 616c 6964 2065 6d61 696c 2061 6464 7265  alid email addre
+00000a80: 7373 206f 7220 6120 7374 7269 6e67 2063  ss or a string c
+00000a90: 6f6e 7461 696e 696e 6720 6f6e 6c79 2061  ontaining only a
+00000aa0: 6c70 6861 6e75 6d65 7269 6320 6368 6172  lphanumeric char
+00000ab0: 6163 7465 7273 2c20 6461 7368 6573 2c20  acters, dashes, 
+00000ac0: 616e 6420 756e 6465 7273 636f 7265 732e  and underscores.
+00000ad0: 7a0c 4163 6365 7373 2054 6f6b 656e 4629  z.Access TokenF)
+00000ae0: 03da 0a68 6964 655f 696e 7075 7472 0800  ...hide_inputr..
+00000af0: 0000 da0c 7368 6f77 5f64 6566 6175 6c74  ....show_default
+00000b00: 7a0a 5e5c 537b 382c 3634 7d24 7a59 496e  z.^\S{8,64}$zYIn
+00000b10: 7661 6c69 6420 6163 6365 7373 2074 6f6b  valid access tok
+00000b20: 656e 2066 6f72 6d61 742e 2049 7420 7368  en format. It sh
+00000b30: 6f75 6c64 2063 6f6e 7461 696e 206e 6f20  ould contain no 
+00000b40: 7768 6974 6573 7061 6365 2061 6e64 2062  whitespace and b
+00000b50: 6520 382d 3634 2063 6861 7261 6374 6572  e 8-64 character
+00000b60: 7320 6c6f 6e67 2e7a 0f4f 7267 616e 697a  s long.z.Organiz
+00000b70: 6174 696f 6e20 4944 7a33 496e 7661 6c69  ation IDz3Invali
+00000b80: 6420 6f72 6761 6e69 7a61 7469 6f6e 2049  d organization I
+00000b90: 442e 2049 7420 7368 6f75 6c64 2062 6520  D. It should be 
+00000ba0: 6120 7661 6c69 6420 5555 4944 2e7a 0a50  a valid UUID.z.P
+00000bb0: 726f 6a65 6374 2049 44fa 017e 7a0a 2e73  roject ID..~z..s
+00000bc0: 7465 6c6c 616e 6f77 2901 da08 6578 6973  tellanow)...exis
+00000bd0: 745f 6f6b 7a0a 636f 6e66 6967 2e69 6e69  t_okz.config.ini
+00000be0: 2904 7214 0000 0072 1600 0000 7217 0000  ).r....r....r...
+00000bf0: 0072 1800 0000 da03 656e 76da 0177 7a1b  .r......env..wz.
+00000c00: 436f 6e66 6967 7572 6174 696f 6e20 666f  Configuration fo
+00000c10: 7220 7072 6f66 696c 6520 277a 1427 2073  r profile 'z.' s
+00000c20: 6176 6564 2073 7563 6365 7373 6675 6c6c  aved successfull
+00000c30: 7929 15da 0563 6c69 636b da04 6563 686f  y)...click..echo
+00000c40: da03 6f62 6ada 0367 6574 7209 0000 00da  ..obj..getr.....
+00000c50: 0272 65da 056d 6174 6368 da06 6c6f 6767  .re..match..logg
+00000c60: 6572 da05 6572 726f 7272 0300 0000 da02  er..errorr......
+00000c70: 6f73 da04 7061 7468 da0a 6578 7061 6e64  os..path..expand
+00000c80: 7573 6572 da08 6d61 6b65 6469 7273 da04  user..makedirs..
+00000c90: 6a6f 696e da0c 636f 6e66 6967 7061 7273  join..configpars
+00000ca0: 6572 da0c 436f 6e66 6967 5061 7273 6572  er..ConfigParser
+00000cb0: da06 6578 6973 7473 da04 7265 6164 da04  ..exists..read..
+00000cc0: 6f70 656e da05 7772 6974 6529 0dda 0363  open..write)...c
+00000cd0: 7478 5a07 7072 6f66 696c 6572 1d00 0000  txZ.profiler....
+00000ce0: da06 636f 6e66 6967 7214 0000 0072 1600  ..configr....r..
+00000cf0: 0000 7217 0000 0072 1800 0000 5a0b 656d  ..r....r....Z.em
+00000d00: 6169 6c5f 7265 6765 785a 0c73 7472 696e  ail_regexZ.strin
+00000d10: 675f 7265 6765 78da 0468 6f6d 655a 0b63  g_regex..homeZ.c
+00000d20: 6f6e 6669 675f 6669 6c65 5a0a 636f 6e66  onfig_fileZ.conf
+00000d30: 6967 6669 6c65 720b 0000 0072 0b00 0000  igfiler....r....
+00000d40: 720f 0000 0072 0500 0000 2300 0000 7362  r....r....#...sb
+00000d50: 0000 0010 0a06 0210 0210 0110 0110 0104  ................
+00000d60: 0204 0102 010e 0118 0102 010a 0202 fb02  ................
+00000d70: 0812 010c 0102 010a 0202 fb02 070e 0108  ................
+00000d80: 0102 010a 0202 fb02 070e 0108 0102 010a  ................
+00000d90: 0202 fb0c 0818 0308 0310 030c 010a 0102  ................
+00000da0: 0402 0102 0102 010a fc08 080c 010c 030c  ................
+00000db0: 011c ff16 0329 13da 075f 5f64 6f63 5f5f  .....)...__doc__
+00000dc0: 721f 0000 0072 2c00 0000 5a07 6c6f 6767  r....r,...Z.logg
+00000dd0: 696e 6772 2700 0000 7223 0000 005a 0b75  ingr'...r#...Z.u
+00000de0: 7469 6c73 2e75 7469 6c73 7203 0000 0072  tils.utilsr....r
+00000df0: 3300 0000 7204 0000 005a 0967 6574 4c6f  3...r....Z.getLo
+00000e00: 6767 6572 da08 5f5f 6e61 6d65 5f5f 7225  gger..__name__r%
+00000e10: 0000 00da 0763 6f6d 6d61 6e64 da06 6f70  .....command..op
+00000e20: 7469 6f6e da06 4368 6f69 6365 da0c 7061  tion..Choice..pa
+00000e30: 7373 5f63 6f6e 7465 7874 7205 0000 00da  ss_contextr.....
+00000e40: 0d63 6f6e 6669 6775 7265 5f63 6d64 720b  .configure_cmdr.
+00000e50: 0000 0072 0b00 0000 720b 0000 0072 0f00  ...r....r....r..
+00000e60: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000e70: 7322 0000 0004 0008 1608 0108 0108 0108  s"..............
+00000e80: 010c 020c 010a 020a 030a 0102 0104 ff22  ..............."
+00000e90: 0304 0110 0108 4d                        ......M
```

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/commands/__pycache__/events.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/commands/__pycache__/events.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 20 14:47:41 2023 UTC, .py size: 1990 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0dbc 9164 c607 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 8dc8 9e64 d507 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6404 6405 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6501 6a07 6406 6407 8d01  m.Z...e.j.d.d...
 00000060: 6505 6506 6501 6a08 6408 6406 8400 8301  e.e.e.j.d.d.....
 00000070: 8301 8301 8301 5a09 6509 5a0a 6402 5300  ......Z.e.Z.d.S.
@@ -76,58 +76,59 @@
 000004b0: 0a49 4e20 5448 4520 534f 4654 5741 5245  .IN THE SOFTWARE
 000004c0: 2e0a e900 0000 004e 2901 da0b 5072 6574  .......N)...Pret
 000004d0: 7479 5461 626c 65e9 0100 0000 2902 da0d  tyTable.....)...
 000004e0: 636f 6d6d 6f6e 5f6f 7074 696f 6eda 0b6c  common_option..l
 000004f0: 6f61 645f 636f 6e66 6967 da06 6576 656e  oad_config..even
 00000500: 7473 2901 da04 6e61 6d65 6304 0000 0000  ts)...namec.....
 00000510: 0000 0000 0000 0008 0000 0008 0000 004b  ...............K
-00000520: 0000 0073 8000 0000 7400 6401 7c02 9b00  ...s....t.d.|...
-00000530: 6402 7c03 9b00 6403 9d05 8301 0100 7c01  d.|...d.......|.
-00000540: a001 a100 7d05 7402 6700 6404 a201 8301  ....}.t.g.d.....
-00000550: 7d06 7c05 4400 5d11 7d07 7c06 a003 7c07  }.|.D.].}.|...|.
-00000560: 6a04 7c07 6a05 7c07 6a06 7c07 6a07 7c07  j.|.j.|.j.|.j.|.
-00000570: 6a08 6705 a101 0100 7117 7400 7c06 8301  j.g.....q.t.|...
-00000580: 0100 7c05 4400 5d0e 7d07 7400 6405 7c07  ..|.D.].}.t.d.|.
-00000590: 6a04 9b00 6406 7c07 6a05 9b00 9d04 8301  j...d.|.j.......
-000005a0: 0100 712f 6407 5300 2908 7a6e 4665 7463  ..q/d.S.).znFetc
-000005b0: 6865 7320 7468 6520 6c61 7465 7374 2065  hes the latest e
-000005c0: 7665 6e74 2073 7065 6369 6669 6361 7469  vent specificati
-000005d0: 6f6e 7320 6672 6f6d 2074 6865 2041 5049  ons from the API
-000005e0: 2061 6e64 206f 7574 7075 7420 6120 6c69   and output a li
-000005f0: 7374 206f 6620 7468 6520 6576 656e 7473  st of the events
-00000600: 2069 6e74 6f20 7468 6520 7465 726d 696e   into the termin
-00000610: 616c 2070 726f 6d70 742e 7a12 0a0a 4f72  al prompt.z...Or
-00000620: 6761 6e69 7a61 7469 6f6e 4964 3a20 7a0c  ganizationId: z.
-00000630: 0a50 726f 6a65 6374 4964 3a20 7a02 0a0a  .ProjectId: z...
-00000640: 2905 5a07 4576 656e 7449 447a 0a45 7665  ).Z.EventIDz.Eve
-00000650: 6e74 204e 616d 657a 0949 7320 4163 7469  nt Namez.Is Acti
-00000660: 7665 7a0a 4372 6561 7465 6420 4174 7a0a  vez.Created Atz.
-00000670: 5570 6461 7465 6420 4174 7a04 4944 3a20  Updated Atz.ID: 
-00000680: 7a08 2c20 4e61 6d65 3a20 4e29 09da 0570  z., Name: N)...p
-00000690: 7269 6e74 da0a 6765 745f 6576 656e 7473  rint..get_events
-000006a0: 7202 0000 00da 0761 6464 5f72 6f77 da02  r......add_row..
-000006b0: 6964 7207 0000 00da 0869 7341 6374 6976  idr......isActiv
-000006c0: 65da 0963 7265 6174 6564 4174 da09 7570  e..createdAt..up
-000006d0: 6461 7465 6441 7429 08da 0363 7478 da0a  datedAt)...ctx..
-000006e0: 7374 656c 6c61 5f61 7069 da0f 6f72 6761  stella_api..orga
-000006f0: 6e69 7a61 7469 6f6e 5f69 64da 0a70 726f  nization_id..pro
-00000700: 6a65 6374 5f69 64da 066b 7761 7267 73da  ject_id..kwargs.
-00000710: 075f 6576 656e 7473 da05 7461 626c 65da  ._events..table.
-00000720: 0565 7665 6e74 a900 7217 0000 00fa 5d2f  .event..r.....]/
-00000730: 5573 6572 732f 746f 6d2d 6b61 6e64 7a69  Users/tom-kandzi
-00000740: 6f72 612f 4465 764c 6f63 616c 2f73 7465  ora/DevLocal/ste
-00000750: 6c6c 612f 7374 656c 6c61 2d6e 6f77 2f53  lla/stella-now/S
-00000760: 7465 6c6c 614e 6f77 434c 492f 7374 656c  tellaNowCLI/stel
-00000770: 6c61 6e6f 775f 636c 692f 636f 6d6d 616e  lanow_cli/comman
-00000780: 6473 2f65 7665 6e74 732e 7079 7206 0000  ds/events.pyr...
-00000790: 001e 0000 0073 1200 0000 1607 0802 0c02  .....s..........
-000007a0: 0803 2001 0802 0802 1a01 04ff 290b da07  .. .........)...
-000007b0: 5f5f 646f 635f 5fda 0563 6c69 636b da0b  __doc__..click..
-000007c0: 7072 6574 7479 7461 626c 6572 0200 0000  prettytabler....
-000007d0: da0e 636f 6d6d 616e 645f 636f 6e66 6967  ..command_config
-000007e0: 7204 0000 0072 0500 0000 da07 636f 6d6d  r....r......comm
-000007f0: 616e 64da 0c70 6173 735f 636f 6e74 6578  and..pass_contex
-00000800: 7472 0600 0000 da0a 6576 656e 7473 5f63  tr......events_c
-00000810: 6d64 7217 0000 0072 1700 0000 7217 0000  mdr....r....r...
-00000820: 0072 1800 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000830: 0100 0000 7314 0000 0004 0008 160c 0210  ....s...........
-00000840: 020a 0302 0102 0104 0110 0108 13         .............
+00000520: 0000 0073 8600 0000 7400 a001 6401 7c02  ...s....t...d.|.
+00000530: 9b00 6402 7c03 9b00 6403 9d05 a101 0100  ..d.|...d.......
+00000540: 7c01 a002 a100 7d05 7403 6700 6404 a201  |.....}.t.g.d...
+00000550: 8301 7d06 7c05 4400 5d11 7d07 7c06 a004  ..}.|.D.].}.|...
+00000560: 7c07 6a05 7c07 6a06 7c07 6a07 7c07 6a08  |.j.|.j.|.j.|.j.
+00000570: 7c07 6a09 6705 a101 0100 7118 7400 a001  |.j.g.....q.t...
+00000580: 7c06 a101 0100 7c05 4400 5d0f 7d07 7400  |.....|.D.].}.t.
+00000590: a001 6405 7c07 6a05 9b00 6406 7c07 6a06  ..d.|.j...d.|.j.
+000005a0: 9b00 9d04 a101 0100 7131 6407 5300 2908  ........q1d.S.).
+000005b0: 7a6e 4665 7463 6865 7320 7468 6520 6c61  znFetches the la
+000005c0: 7465 7374 2065 7665 6e74 2073 7065 6369  test event speci
+000005d0: 6669 6361 7469 6f6e 7320 6672 6f6d 2074  fications from t
+000005e0: 6865 2041 5049 2061 6e64 206f 7574 7075  he API and outpu
+000005f0: 7420 6120 6c69 7374 206f 6620 7468 6520  t a list of the 
+00000600: 6576 656e 7473 2069 6e74 6f20 7468 6520  events into the 
+00000610: 7465 726d 696e 616c 2070 726f 6d70 742e  terminal prompt.
+00000620: 7a12 0a0a 4f72 6761 6e69 7a61 7469 6f6e  z...Organization
+00000630: 4964 3a20 7a0c 0a50 726f 6a65 6374 4964  Id: z..ProjectId
+00000640: 3a20 7a02 0a0a 2905 5a07 4576 656e 7449  : z...).Z.EventI
+00000650: 447a 0a45 7665 6e74 204e 616d 657a 0949  Dz.Event Namez.I
+00000660: 7320 4163 7469 7665 7a0a 4372 6561 7465  s Activez.Create
+00000670: 6420 4174 7a0a 5570 6461 7465 6420 4174  d Atz.Updated At
+00000680: 7a04 4944 3a20 7a08 2c20 4e61 6d65 3a20  z.ID: z., Name: 
+00000690: 4e29 0ada 0563 6c69 636b da04 6563 686f  N)...click..echo
+000006a0: da0a 6765 745f 6576 656e 7473 7202 0000  ..get_eventsr...
+000006b0: 00da 0761 6464 5f72 6f77 da02 6964 7207  ...add_row..idr.
+000006c0: 0000 00da 0869 7341 6374 6976 65da 0963  .....isActive..c
+000006d0: 7265 6174 6564 4174 da09 7570 6461 7465  reatedAt..update
+000006e0: 6441 7429 08da 0363 7478 da0a 7374 656c  dAt)...ctx..stel
+000006f0: 6c61 5f61 7069 da0f 6f72 6761 6e69 7a61  la_api..organiza
+00000700: 7469 6f6e 5f69 64da 0a70 726f 6a65 6374  tion_id..project
+00000710: 5f69 64da 066b 7761 7267 73da 075f 6576  _id..kwargs.._ev
+00000720: 656e 7473 da05 7461 626c 65da 0565 7665  ents..table..eve
+00000730: 6e74 a900 7218 0000 00fa 5d2f 5573 6572  nt..r.....]/User
+00000740: 732f 746f 6d2d 6b61 6e64 7a69 6f72 612f  s/tom-kandziora/
+00000750: 4465 764c 6f63 616c 2f73 7465 6c6c 612f  DevLocal/stella/
+00000760: 7374 656c 6c61 2d6e 6f77 2f53 7465 6c6c  stella-now/Stell
+00000770: 614e 6f77 434c 492f 7374 656c 6c61 6e6f  aNowCLI/stellano
+00000780: 775f 636c 692f 636f 6d6d 616e 6473 2f65  w_cli/commands/e
+00000790: 7665 6e74 732e 7079 7206 0000 001e 0000  vents.pyr.......
+000007a0: 0073 1200 0000 1807 0802 0c02 0803 2001  .s............ .
+000007b0: 0a02 0802 1c01 04ff 290b da07 5f5f 646f  ........)...__do
+000007c0: 635f 5f72 0800 0000 da0b 7072 6574 7479  c__r......pretty
+000007d0: 7461 626c 6572 0200 0000 da0e 636f 6d6d  tabler......comm
+000007e0: 616e 645f 636f 6e66 6967 7204 0000 0072  and_configr....r
+000007f0: 0500 0000 da07 636f 6d6d 616e 64da 0c70  ......command..p
+00000800: 6173 735f 636f 6e74 6578 7472 0600 0000  ass_contextr....
+00000810: da0a 6576 656e 7473 5f63 6d64 7218 0000  ..events_cmdr...
+00000820: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00000830: da08 3c6d 6f64 756c 653e 0100 0000 7314  ..<module>....s.
+00000840: 0000 0004 0008 160c 0210 020a 0302 0102  ................
+00000850: 0104 0110 0108 13                        .......
```

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/commands/__pycache__/generate.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/commands/__pycache__/generate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 20 14:47:52 2023 UTC, .py size: 5203 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 18bc 9164 5314 0000  o..........dS...
+00000000: 6f0d 0d0a 0000 0000 4ec8 9e64 7e14 0000  o.......N..d~...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0019 0000 0040 0000 0073 4e01 0000 6400  .....@...sN...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 0100 6405  d.l.m.Z.m.Z...d.
 00000070: 6406 6c0a 5400 6407 6408 6c0b 6d0c 5a0c  d.l.T.d.d.l.m.Z.
@@ -132,193 +132,194 @@
 00000830: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
 00000840: 6c6e 616d 655f 5fda 0373 7472 7213 0000  lname__..strr...
 00000850: 0072 1500 0000 7211 0000 0072 1100 0000  .r....r....r....
 00000860: 7211 0000 0072 1200 0000 720c 0000 0029  r....r....r....)
 00000870: 0000 0073 0600 0000 0800 1201 0c04 720c  ...s..........r.
 00000880: 0000 00da 0d73 6b69 7070 6564 5f66 696c  .....skipped_fil
 00000890: 6573 6301 0000 0000 0000 0000 0000 0003  esc.............
-000008a0: 0000 0005 0000 0043 0000 0073 6400 0000  .......C...sd...
-000008b0: 7c00 7230 7400 6401 8301 0100 7401 6402  |.r0t.d.....t.d.
-000008c0: 6403 6702 8301 7d01 7c00 4400 5d0b 7d02  d.g...}.|.D.].}.
-000008d0: 7c01 a002 7c02 6a03 7c02 6a04 6702 a101  |...|.j.|.j.g...
-000008e0: 0100 710e 7400 7c01 8301 0100 7400 6404  ..q.t.|.....t.d.
-000008f0: 8301 0100 7400 6405 8301 0100 7400 6406  ....t.d.....t.d.
-00000900: 8301 0100 7400 6407 8301 0100 6400 5300  ....t.d.....d.S.
-00000910: 6400 5300 2908 4e7a 500a 3d3d 3d3d 3d3d  d.S.).NzP.======
-00000920: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000930: 3d3d 3d3d 3d3d 3d3d 0a20 2020 2020 2020  ========.       
-00000940: 2020 5355 4d4d 4152 590a 3d3d 3d3d 3d3d    SUMMARY.======
-00000950: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000960: 3d3d 3d3d 3d3d 3d3d 0ada 0446 696c 657a  ========...Filez
-00000970: 0f53 6b69 7070 696e 6720 5265 6173 6f6e  .Skipping Reason
-00000980: 7a1f 0a53 6b69 7070 6564 2052 6561 736f  z..Skipped Reaso
-00000990: 6e20 2d20 4578 706c 616e 6174 696f 6e3a  n - Explanation:
-000009a0: 0a7a 642d 2046 696c 6520 416c 7265 6164  .zd- File Alread
-000009b0: 7920 4578 6973 7420 2d20 4578 6973 7469  y Exist - Existi
-000009c0: 6e67 2063 6c61 7373 6573 2063 616e 2774  ng classes can't
-000009d0: 2062 6520 6f76 6572 7269 6465 6e2e 2055   be overriden. U
-000009e0: 7365 202d 2d66 6f72 6365 2074 6f20 6f76  se --force to ov
-000009f0: 6572 7269 6465 2074 6869 7320 7072 6f74  erride this prot
-00000a00: 6563 7469 6f6e 2e7a 632d 204d 6973 7369  ection.zc- Missi
-00000a10: 6e67 2045 7665 6e74 2043 6f6e 6669 6775  ng Event Configu
-00000a20: 7261 7469 6f6e 202d 2043 6865 636b 2069  ration - Check i
-00000a30: 6620 7468 6520 7370 6563 6966 6965 6420  f the specified 
-00000a40: 6576 656e 7420 646f 6573 2065 7869 7374  event does exist
-00000a50: 7320 696e 2074 6865 6e20 4f70 6572 6174  s in then Operat
-00000a60: 6f72 7320 436f 6e73 6f6c 652e 7a5c 2d20  ors Console.z\- 
-00000a70: 4e6f 2045 6e74 6974 7920 4173 736f 6369  No Entity Associ
-00000a80: 6174 6564 2057 6974 6820 4576 656e 7420  ated With Event 
-00000a90: 2d20 4576 656e 7420 6578 6973 7473 2c20  - Event exists, 
-00000aa0: 6275 7420 6974 2069 7320 6e6f 7420 6174  but it is not at
-00000ab0: 7461 6368 6564 2074 6f20 616e 7920 656e  tached to any en
-00000ac0: 7469 7479 2074 7970 652e 2905 da05 7072  tity type.)...pr
-00000ad0: 696e 7472 0200 0000 5a07 6164 645f 726f  intr....Z.add_ro
-00000ae0: 7772 0d00 0000 720e 0000 0029 0372 1a00  wr....r....).r..
-00000af0: 0000 da05 7461 626c 655a 0c73 6b69 7070  ....tableZ.skipp
-00000b00: 6564 5f66 696c 6572 1100 0000 7211 0000  ed_filer....r...
-00000b10: 0072 1200 0000 da14 7072 696e 745f 736b  .r......print_sk
-00000b20: 6970 7065 645f 7265 7375 6c74 3200 0000  ipped_result2...
-00000b30: 7316 0000 0004 0108 010c 0208 0314 0108  s...............
-00000b40: 0208 0208 0108 010c 0104 f272 1e00 0000  ...........r....
-00000b50: da08 6765 6e65 7261 7465 2901 da04 6e61  ..generate)...na
-00000b60: 6d65 7a0b 2d2d 6e61 6d65 7370 6163 657a  mez.--namespacez
-00000b70: 022d 6eda 007a 2854 6865 206e 616d 6573  .-n..z(The names
-00000b80: 7061 6365 2066 6f72 2074 6865 2067 656e  pace for the gen
-00000b90: 6572 6174 6564 2063 6c61 7373 6573 2e29  erated classes.)
-00000ba0: 02da 0764 6566 6175 6c74 da04 6865 6c70  ...default..help
-00000bb0: 7a0d 2d2d 6465 7374 696e 6174 696f 6e7a  z.--destinationz
-00000bc0: 022d 64da 012e 7a2c 5468 6520 6469 7265  .-d...z,The dire
-00000bd0: 6374 6f72 7920 746f 2073 6176 6520 7468  ctory to save th
-00000be0: 6520 6765 6e65 7261 7465 6420 636c 6173  e generated clas
-00000bf0: 7365 732e 7a07 2d2d 666f 7263 657a 022d  ses.z.--forcez.-
-00000c00: 6654 7a19 4f76 6572 7772 6974 6520 6578  fTz.Overwrite ex
-00000c10: 6973 7469 6e67 2066 696c 6573 2e29 02da  isting files.)..
-00000c20: 0769 735f 666c 6167 7223 0000 007a 082d  .is_flagr#...z.-
-00000c30: 2d65 7665 6e74 737a 022d 657a 244c 6973  -eventsz.-ez$Lis
-00000c40: 7420 6f66 2073 7065 6369 6669 6320 6576  t of specific ev
-00000c50: 656e 7473 2074 6f20 6765 6e65 7261 7465  ents to generate
-00000c60: 2e29 02da 086d 756c 7469 706c 6572 2300  .)...multipler#.
-00000c70: 0000 7a0a 2d2d 6c61 6e67 7561 6765 7a02  ..z.--languagez.
-00000c80: 2d6c 5a06 6373 6861 7270 4629 01da 0e63  -lZ.csharpF)...c
-00000c90: 6173 655f 7365 6e73 6974 6976 657a 3354  ase_sensitivez3T
-00000ca0: 6865 2070 726f 6772 616d 6d69 6e67 206c  he programming l
-00000cb0: 616e 6775 6167 6520 666f 7220 7468 6520  anguage for the 
-00000cc0: 6765 6e65 7261 7465 6420 636c 6173 7365  generated classe
-00000cd0: 732e 2903 da04 7479 7065 7222 0000 0072  s.)...typer"...r
-00000ce0: 2300 0000 da03 6374 78da 0a73 7465 6c6c  #.....ctx..stell
-00000cf0: 615f 6170 69da 0b64 6573 7469 6e61 7469  a_api..destinati
-00000d00: 6f6e da05 666f 7263 65da 0665 7665 6e74  on..force..event
-00000d10: 73da 086c 616e 6775 6167 65da 066b 7761  s..language..kwa
-00000d20: 7267 7363 0600 0000 0000 0000 0000 0000  rgsc............
-00000d30: 1200 0000 0b00 0000 4b00 0000 73a2 0100  ........K...s...
-00000d40: 0074 0064 0183 0101 007c 05a0 01a1 009b  .t.d.....|......
-00000d50: 0064 029d 027d 077a 0e74 0274 03a0 0464  .d...}.z.t.t...d
-00000d60: 037c 059b 0064 049d 03a1 017c 0783 027d  .|...d.....|...}
-00000d70: 0857 006e 0b04 0074 0579 2401 0001 0001  .W.n...t.y$.....
-00000d80: 0074 067c 0583 0182 0177 007c 0472 2b74  .t.|.....w.|.r+t
-00000d90: 077c 0483 016e 0274 0783 007d 0974 0783  .|...n.t...}.t..
-00000da0: 007d 0a7c 01a0 08a1 007d 0b7c 0b44 005d  .}.|.....}.|.D.]
-00000db0: 8a7d 0c7c 0472 417c 0c6a 097c 0476 0172  .}.|.rA|.j.|.v.r
-00000dc0: 4171 377c 09a0 0a7c 0c6a 09a1 0101 0074  Aq7|...|.j.....t
-00000dd0: 0064 057c 0c6a 099b 009d 0283 0101 007c  .d.|.j.........|
-00000de0: 0883 007d 0d74 0b6a 0ca0 0d7c 027c 0da0  ...}.t.j...|.|..
-00000df0: 0e7c 0c6a 09a1 01a1 027d 0e7c 0373 7374  .|.j.....}.|.sst
-00000e00: 0b6a 0ca0 0f7c 0ea1 0172 7374 0064 0683  .j...|...rst.d..
-00000e10: 0101 007c 0aa0 1074 117c 0c6a 0964 0783  ...|...t.|.j.d..
-00000e20: 02a1 0101 0071 3764 087d 0f7a 0f7c 0d6a  .....q7d.}.z.|.j
-00000e30: 127c 01a0 137c 0c6a 14a1 0166 0169 007c  .|...|.j...f.i.|
-00000e40: 06a4 018e 017d 0f57 006e 2004 0074 1579  .....}.W.n ..t.y
-00000e50: a401 007d 1001 007a 1474 0064 0683 0101  ...}...z.t.d....
-00000e60: 007c 0aa0 1074 117c 0c6a 097c 106a 1683  .|...t.|.j.|.j..
-00000e70: 02a1 0101 0057 0059 0064 087d 107e 1071  .....W.Y.d.}.~.q
-00000e80: 3764 087d 107e 1077 0177 007c 0f72 c174  7d.}.~.w.w.|.r.t
-00000e90: 177c 0e64 0983 028f 0d7d 117c 11a0 187c  .|.d.....}.|...|
-00000ea0: 0fa1 0101 0057 0064 0804 0004 0083 0301  .....W.d........
-00000eb0: 006e 0831 0073 bc77 0101 0001 0001 0059  .n.1.s.w.......Y
-00000ec0: 0001 0071 3774 1974 1a7c 0a83 0164 0a64  ...q7t.t.|...d.d
-00000ed0: 0b84 007c 0944 0083 0117 0083 0101 0064  ...|.D.........d
-00000ee0: 0853 0029 0c7a 8446 6574 6368 6573 2074  .S.).z.Fetches t
-00000ef0: 6865 206c 6174 6573 7420 6576 656e 7420  he latest event 
-00000f00: 7370 6563 6966 6963 6174 696f 6e73 2066  specifications f
-00000f10: 726f 6d20 7468 6520 4150 4920 616e 6420  rom the API and 
-00000f20: 6765 6e65 7261 7465 7320 636f 7272 6573  generates corres
-00000f30: 706f 6e64 696e 6720 636c 6173 7320 636f  ponding class co
-00000f40: 6465 2069 6e20 7468 6520 6465 7369 7265  de in the desire
-00000f50: 640a 2020 2020 7072 6f67 7261 6d6d 696e  d.    programmin
-00000f60: 6720 6c61 6e67 7561 6765 2e7a 0d47 656e  g language.z.Gen
-00000f70: 6572 6174 696e 672e 2e2e 5a0d 436f 6465  erating...Z.Code
-00000f80: 4765 6e65 7261 746f 727a 1e73 7465 6c6c  Generatorz.stell
-00000f90: 616e 6f77 5f63 6c69 2e63 6f64 655f 6765  anow_cli.code_ge
-00000fa0: 6e65 7261 746f 7273 2e5a 0f5f 636f 6465  nerators.Z._code
-00000fb0: 5f67 656e 6572 6174 6f72 7a1c 4765 6e65  _generatorz.Gene
-00000fc0: 7261 7469 6e67 2063 6c61 7373 2066 6f72  rating class for
-00000fd0: 2065 7665 6e74 3a20 7a0b 536b 6970 7065   event: z.Skippe
-00000fe0: 6420 2e2e 2e7a 1246 696c 6520 416c 7265  d ...z.File Alre
-00000ff0: 6164 7920 4578 6973 744e da01 7763 0100  ady ExistN..wc..
-00001000: 0000 0000 0000 0000 0000 0200 0000 0500  ................
-00001010: 0000 5300 0000 7316 0000 0067 007c 005d  ..S...s....g.|.]
-00001020: 077d 0174 007c 0164 0083 0291 0271 0253  .}.t.|.d.....q.S
-00001030: 0029 017a 1b4d 6973 7369 6e67 2045 7665  .).z.Missing Eve
-00001040: 6e74 2043 6f6e 6669 6775 7261 7469 6f6e  nt Configuration
-00001050: 2901 720c 0000 0029 02da 022e 30da 0966  ).r....)....0..f
-00001060: 696c 655f 6e61 6d65 7211 0000 0072 1100  ile_namer....r..
-00001070: 0000 7212 0000 00da 0a3c 6c69 7374 636f  ..r......<listco
-00001080: 6d70 3e85 0000 0073 0200 0000 1600 7a1c  mp>....s......z.
-00001090: 6765 6e65 7261 7465 2e3c 6c6f 6361 6c73  generate.<locals
-000010a0: 3e2e 3c6c 6973 7463 6f6d 703e 291b 721c  >.<listcomp>).r.
-000010b0: 0000 00da 0a63 6170 6974 616c 697a 65da  .....capitalize.
-000010c0: 0767 6574 6174 7472 da09 696d 706f 7274  .getattr..import
-000010d0: 6c69 62da 0d69 6d70 6f72 745f 6d6f 6475  lib..import_modu
-000010e0: 6c65 da0b 496d 706f 7274 4572 726f 7272  le..ImportErrorr
-000010f0: 0b00 0000 da03 7365 745a 0a67 6574 5f65  ......setZ.get_e
-00001100: 7665 6e74 7372 2000 0000 da07 6469 7363  ventsr .....disc
-00001110: 6172 64da 026f 73da 0470 6174 68da 046a  ard..os..path..j
-00001120: 6f69 6e5a 1c67 6574 5f66 696c 655f 6e61  oinZ.get_file_na
-00001130: 6d65 5f66 6f72 5f65 7665 6e74 5f6e 616d  me_for_event_nam
-00001140: 65da 0665 7869 7374 73da 0361 6464 720c  e..exists..addr.
-00001150: 0000 005a 0e67 656e 6572 6174 655f 636c  ...Z.generate_cl
-00001160: 6173 735a 1167 6574 5f65 7665 6e74 5f64  assZ.get_event_d
-00001170: 6574 6169 6c73 da02 6964 720a 0000 00da  etails..idr.....
-00001180: 076d 6573 7361 6765 da04 6f70 656e da05  .message..open..
-00001190: 7772 6974 6572 1e00 0000 da04 6c69 7374  writer......list
-000011a0: 2912 7229 0000 0072 2a00 0000 722b 0000  ).r)...r*...r+..
-000011b0: 0072 2c00 0000 722d 0000 0072 2e00 0000  .r,...r-...r....
-000011c0: 722f 0000 005a 1467 656e 6572 6174 6f72  r/...Z.generator
-000011d0: 5f63 6c61 7373 5f6e 616d 655a 0f67 656e  _class_nameZ.gen
-000011e0: 6572 6174 6f72 5f63 6c61 7373 5a10 6576  erator_classZ.ev
-000011f0: 656e 7473 5f6e 6f74 5f66 6f75 6e64 5a0e  ents_not_foundZ.
-00001200: 6576 656e 7473 5f73 6b69 7070 6564 5a07  events_skippedZ.
-00001210: 5f65 7665 6e74 735a 0565 7665 6e74 da09  _eventsZ.event..
-00001220: 6765 6e65 7261 746f 725a 0966 696c 655f  generatorZ.file_
-00001230: 7061 7468 da04 636f 6465 da01 65da 0466  path..code..e..f
-00001240: 696c 6572 1100 0000 7211 0000 0072 1200  iler....r....r..
-00001250: 0000 721f 0000 0044 0000 0073 5400 0000  ..r....D...sT...
-00001260: 0815 0e02 0201 1201 0201 08ff 0c02 0801  ................
-00001270: 02ff 1203 0601 0802 0801 0e01 0201 0c02  ................
-00001280: 1001 0602 1603 1001 0801 1201 0201 0402  ................
-00001290: 0202 1e01 0e01 0801 1401 0c01 0880 02fd  ................
-000012a0: 0405 0c01 0c01 1cff 0280 0203 0601 0c01  ................
-000012b0: 02ff 08ff 2920 da07 5f5f 646f 635f 5fda  ....) ..__doc__.
-000012c0: 0563 6c69 636b 7236 0000 00da 076c 6f67  .clickr6.....log
-000012d0: 6769 6e67 723b 0000 005a 0b70 7265 7474  gingr;...Z.prett
-000012e0: 7974 6162 6c65 7202 0000 00da 0674 7970  ytabler......typ
-000012f0: 696e 6772 0300 0000 7204 0000 005a 0361  ingr....r....Z.a
-00001300: 7069 5a0e 636f 6d6d 616e 645f 636f 6e66  piZ.command_conf
-00001310: 6967 7208 0000 0072 0900 0000 5a20 6578  igr....r....Z ex
-00001320: 6365 7074 696f 6e73 2e53 7465 6c6c 614e  ceptions.StellaN
-00001330: 6f77 434c 4945 7863 6570 7469 6f6e 720a  owCLIExceptionr.
-00001340: 0000 0072 0b00 0000 da09 6765 744c 6f67  ...r......getLog
-00001350: 6765 7272 1600 0000 da06 6c6f 6767 6572  gerr......logger
-00001360: 720c 0000 0072 1e00 0000 da07 636f 6d6d  r....r......comm
-00001370: 616e 64da 066f 7074 696f 6eda 0643 686f  and..option..Cho
-00001380: 6963 65da 0c70 6173 735f 636f 6e74 6578  ice..pass_contex
-00001390: 745a 0953 7465 6c6c 6141 5049 7219 0000  tZ.StellaAPIr...
-000013a0: 00da 0462 6f6f 6cda 0464 6963 7472 1f00  ...bool..dictr..
-000013b0: 0000 da0c 6765 6e65 7261 7465 5f63 6d64  ....generate_cmd
-000013c0: 7211 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
-000013d0: 1200 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-000013e0: 0000 7350 0000 0004 0008 1608 0108 0108  ..sP............
-000013f0: 010c 0210 0108 0210 0110 010a 050e 0312  ................
-00001400: 090a 1202 0102 0110 0110 0110 0110 0118  ................
-00001410: 0102 0104 ff04 0202 0102 0102 ff02 0202  ................
-00001420: fe02 0302 fd02 0402 fc06 0502 fb02 0602  ................
-00001430: fa0a 071c f908 3b                        ......;
+000008a0: 0000 0005 0000 0043 0000 0073 7000 0000  .......C...sp...
+000008b0: 7c00 7236 7400 a001 6401 a101 0100 7402  |.r6t...d.....t.
+000008c0: 6402 6403 6702 8301 7d01 7c00 4400 5d0b  d.d.g...}.|.D.].
+000008d0: 7d02 7c01 a003 7c02 6a04 7c02 6a05 6702  }.|...|.j.|.j.g.
+000008e0: a101 0100 710f 7400 a001 7c01 a101 0100  ....q.t...|.....
+000008f0: 7400 a001 6404 a101 0100 7400 a001 6405  t...d.....t...d.
+00000900: a101 0100 7400 a001 6406 a101 0100 7400  ....t...d.....t.
+00000910: a001 6407 a101 0100 6400 5300 6400 5300  ..d.....d.S.d.S.
+00000920: 2908 4e7a 500a 3d3d 3d3d 3d3d 3d3d 3d3d  ).NzP.==========
+00000930: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000940: 3d3d 3d3d 0a20 2020 2020 2020 2020 5355  ====.         SU
+00000950: 4d4d 4152 590a 3d3d 3d3d 3d3d 3d3d 3d3d  MMARY.==========
+00000960: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000970: 3d3d 3d3d 0ada 0446 696c 657a 0f53 6b69  ====...Filez.Ski
+00000980: 7070 696e 6720 5265 6173 6f6e 7a1f 0a53  pping Reasonz..S
+00000990: 6b69 7070 6564 2052 6561 736f 6e20 2d20  kipped Reason - 
+000009a0: 4578 706c 616e 6174 696f 6e3a 0a7a 642d  Explanation:.zd-
+000009b0: 2046 696c 6520 416c 7265 6164 7920 4578   File Already Ex
+000009c0: 6973 7420 2d20 4578 6973 7469 6e67 2063  ist - Existing c
+000009d0: 6c61 7373 6573 2063 616e 2774 2062 6520  lasses can't be 
+000009e0: 6f76 6572 7269 6465 6e2e 2055 7365 202d  overriden. Use -
+000009f0: 2d66 6f72 6365 2074 6f20 6f76 6572 7269  -force to overri
+00000a00: 6465 2074 6869 7320 7072 6f74 6563 7469  de this protecti
+00000a10: 6f6e 2e7a 632d 204d 6973 7369 6e67 2045  on.zc- Missing E
+00000a20: 7665 6e74 2043 6f6e 6669 6775 7261 7469  vent Configurati
+00000a30: 6f6e 202d 2043 6865 636b 2069 6620 7468  on - Check if th
+00000a40: 6520 7370 6563 6966 6965 6420 6576 656e  e specified even
+00000a50: 7420 646f 6573 2065 7869 7374 7320 696e  t does exists in
+00000a60: 2074 6865 6e20 4f70 6572 6174 6f72 7320   then Operators 
+00000a70: 436f 6e73 6f6c 652e 7a5c 2d20 4e6f 2045  Console.z\- No E
+00000a80: 6e74 6974 7920 4173 736f 6369 6174 6564  ntity Associated
+00000a90: 2057 6974 6820 4576 656e 7420 2d20 4576   With Event - Ev
+00000aa0: 656e 7420 6578 6973 7473 2c20 6275 7420  ent exists, but 
+00000ab0: 6974 2069 7320 6e6f 7420 6174 7461 6368  it is not attach
+00000ac0: 6564 2074 6f20 616e 7920 656e 7469 7479  ed to any entity
+00000ad0: 2074 7970 652e 2906 da05 636c 6963 6bda   type.)...click.
+00000ae0: 0465 6368 6f72 0200 0000 5a07 6164 645f  .echor....Z.add_
+00000af0: 726f 7772 0d00 0000 720e 0000 0029 0372  rowr....r....).r
+00000b00: 1a00 0000 da05 7461 626c 655a 0c73 6b69  ......tableZ.ski
+00000b10: 7070 6564 5f66 696c 6572 1100 0000 7211  pped_filer....r.
+00000b20: 0000 0072 1200 0000 da14 7072 696e 745f  ...r......print_
+00000b30: 736b 6970 7065 645f 7265 7375 6c74 3200  skipped_result2.
+00000b40: 0000 7316 0000 0004 010a 010c 0208 0314  ..s.............
+00000b50: 010a 020a 020a 010a 010e 0104 f272 1f00  .............r..
+00000b60: 0000 da08 6765 6e65 7261 7465 2901 da04  ....generate)...
+00000b70: 6e61 6d65 7a0b 2d2d 6e61 6d65 7370 6163  namez.--namespac
+00000b80: 657a 022d 6eda 007a 2854 6865 206e 616d  ez.-n..z(The nam
+00000b90: 6573 7061 6365 2066 6f72 2074 6865 2067  espace for the g
+00000ba0: 656e 6572 6174 6564 2063 6c61 7373 6573  enerated classes
+00000bb0: 2e29 02da 0764 6566 6175 6c74 da04 6865  .)...default..he
+00000bc0: 6c70 7a0d 2d2d 6465 7374 696e 6174 696f  lpz.--destinatio
+00000bd0: 6e7a 022d 64da 012e 7a2c 5468 6520 6469  nz.-d...z,The di
+00000be0: 7265 6374 6f72 7920 746f 2073 6176 6520  rectory to save 
+00000bf0: 7468 6520 6765 6e65 7261 7465 6420 636c  the generated cl
+00000c00: 6173 7365 732e 7a07 2d2d 666f 7263 657a  asses.z.--forcez
+00000c10: 022d 6654 7a19 4f76 6572 7772 6974 6520  .-fTz.Overwrite 
+00000c20: 6578 6973 7469 6e67 2066 696c 6573 2e29  existing files.)
+00000c30: 02da 0769 735f 666c 6167 7224 0000 007a  ...is_flagr$...z
+00000c40: 082d 2d65 7665 6e74 737a 022d 657a 244c  .--eventsz.-ez$L
+00000c50: 6973 7420 6f66 2073 7065 6369 6669 6320  ist of specific 
+00000c60: 6576 656e 7473 2074 6f20 6765 6e65 7261  events to genera
+00000c70: 7465 2e29 02da 086d 756c 7469 706c 6572  te.)...multipler
+00000c80: 2400 0000 7a0a 2d2d 6c61 6e67 7561 6765  $...z.--language
+00000c90: 7a02 2d6c 5a06 6373 6861 7270 4629 01da  z.-lZ.csharpF)..
+00000ca0: 0e63 6173 655f 7365 6e73 6974 6976 657a  .case_sensitivez
+00000cb0: 3354 6865 2070 726f 6772 616d 6d69 6e67  3The programming
+00000cc0: 206c 616e 6775 6167 6520 666f 7220 7468   language for th
+00000cd0: 6520 6765 6e65 7261 7465 6420 636c 6173  e generated clas
+00000ce0: 7365 732e 2903 da04 7479 7065 7223 0000  ses.)...typer#..
+00000cf0: 0072 2400 0000 da03 6374 78da 0a73 7465  .r$.....ctx..ste
+00000d00: 6c6c 615f 6170 69da 0b64 6573 7469 6e61  lla_api..destina
+00000d10: 7469 6f6e da05 666f 7263 65da 0665 7665  tion..force..eve
+00000d20: 6e74 73da 086c 616e 6775 6167 65da 066b  nts..language..k
+00000d30: 7761 7267 7363 0600 0000 0000 0000 0000  wargsc..........
+00000d40: 0000 1200 0000 0b00 0000 4b00 0000 73aa  ..........K...s.
+00000d50: 0100 0074 00a0 0164 01a1 0101 007c 05a0  ...t...d.....|..
+00000d60: 02a1 009b 0064 029d 027d 077a 0e74 0374  .....d...}.z.t.t
+00000d70: 04a0 0564 037c 059b 0064 049d 03a1 017c  ...d.|...d.....|
+00000d80: 0783 027d 0857 006e 0b04 0074 0679 2501  ...}.W.n...t.y%.
+00000d90: 0001 0001 0074 077c 0583 0182 0177 007c  .....t.|.....w.|
+00000da0: 0472 2c74 087c 0483 016e 0274 0883 007d  .r,t.|...n.t...}
+00000db0: 0974 0883 007d 0a7c 01a0 09a1 007d 0b7c  .t...}.|.....}.|
+00000dc0: 0b44 005d 8d7d 0c7c 0472 427c 0c6a 0a7c  .D.].}.|.rB|.j.|
+00000dd0: 0476 0172 4271 387c 09a0 0b7c 0c6a 0aa1  .v.rBq8|...|.j..
+00000de0: 0101 0074 00a0 0164 057c 0c6a 0a9b 009d  ...t...d.|.j....
+00000df0: 02a1 0101 007c 0883 007d 0d74 0c6a 0da0  .....|...}.t.j..
+00000e00: 0e7c 027c 0da0 0f7c 0c6a 0aa1 01a1 027d  .|.|...|.j.....}
+00000e10: 0e7c 0373 7674 0c6a 0da0 107c 0ea1 0172  .|.svt.j...|...r
+00000e20: 7674 00a0 0164 06a1 0101 007c 0aa0 1174  vt...d.....|...t
+00000e30: 127c 0c6a 0a64 0783 02a1 0101 0071 3864  .|.j.d.......q8d
+00000e40: 087d 0f7a 0f7c 0d6a 137c 01a0 147c 0c6a  .}.z.|.j.|...|.j
+00000e50: 15a1 0166 0169 007c 06a4 018e 017d 0f57  ...f.i.|.....}.W
+00000e60: 006e 2104 0074 1679 a801 007d 1001 007a  .n!..t.y...}...z
+00000e70: 1574 00a0 0164 06a1 0101 007c 0aa0 1174  .t...d.....|...t
+00000e80: 127c 0c6a 0a7c 106a 1783 02a1 0101 0057  .|.j.|.j.......W
+00000e90: 0059 0064 087d 107e 1071 3864 087d 107e  .Y.d.}.~.q8d.}.~
+00000ea0: 1077 0177 007c 0f72 c574 187c 0e64 0983  .w.w.|.r.t.|.d..
+00000eb0: 028f 0d7d 117c 11a0 197c 0fa1 0101 0057  ...}.|...|.....W
+00000ec0: 0064 0804 0004 0083 0301 006e 0831 0073  .d.........n.1.s
+00000ed0: c077 0101 0001 0001 0059 0001 0071 3874  .w.......Y...q8t
+00000ee0: 1a74 1b7c 0a83 0164 0a64 0b84 007c 0944  .t.|...d.d...|.D
+00000ef0: 0083 0117 0083 0101 0064 0853 0029 0c7a  .........d.S.).z
+00000f00: 8446 6574 6368 6573 2074 6865 206c 6174  .Fetches the lat
+00000f10: 6573 7420 6576 656e 7420 7370 6563 6966  est event specif
+00000f20: 6963 6174 696f 6e73 2066 726f 6d20 7468  ications from th
+00000f30: 6520 4150 4920 616e 6420 6765 6e65 7261  e API and genera
+00000f40: 7465 7320 636f 7272 6573 706f 6e64 696e  tes correspondin
+00000f50: 6720 636c 6173 7320 636f 6465 2069 6e20  g class code in 
+00000f60: 7468 6520 6465 7369 7265 640a 2020 2020  the desired.    
+00000f70: 7072 6f67 7261 6d6d 696e 6720 6c61 6e67  programming lang
+00000f80: 7561 6765 2e7a 0d47 656e 6572 6174 696e  uage.z.Generatin
+00000f90: 672e 2e2e 5a0d 436f 6465 4765 6e65 7261  g...Z.CodeGenera
+00000fa0: 746f 727a 1e73 7465 6c6c 616e 6f77 5f63  torz.stellanow_c
+00000fb0: 6c69 2e63 6f64 655f 6765 6e65 7261 746f  li.code_generato
+00000fc0: 7273 2e5a 0f5f 636f 6465 5f67 656e 6572  rs.Z._code_gener
+00000fd0: 6174 6f72 7a1c 4765 6e65 7261 7469 6e67  atorz.Generating
+00000fe0: 2063 6c61 7373 2066 6f72 2065 7665 6e74   class for event
+00000ff0: 3a20 7a0b 536b 6970 7065 6420 2e2e 2e7a  : z.Skipped ...z
+00001000: 1246 696c 6520 416c 7265 6164 7920 4578  .File Already Ex
+00001010: 6973 744e da01 7763 0100 0000 0000 0000  istN..wc........
+00001020: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
+00001030: 7316 0000 0067 007c 005d 077d 0174 007c  s....g.|.].}.t.|
+00001040: 0164 0083 0291 0271 0253 0029 017a 1b4d  .d.....q.S.).z.M
+00001050: 6973 7369 6e67 2045 7665 6e74 2043 6f6e  issing Event Con
+00001060: 6669 6775 7261 7469 6f6e 2901 720c 0000  figuration).r...
+00001070: 0029 02da 022e 30da 0966 696c 655f 6e61  .)....0..file_na
+00001080: 6d65 7211 0000 0072 1100 0000 7212 0000  mer....r....r...
+00001090: 00da 0a3c 6c69 7374 636f 6d70 3e85 0000  ...<listcomp>...
+000010a0: 0073 0200 0000 1600 7a1c 6765 6e65 7261  .s......z.genera
+000010b0: 7465 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  te.<locals>.<lis
+000010c0: 7463 6f6d 703e 291c 721c 0000 0072 1d00  tcomp>).r....r..
+000010d0: 0000 da0a 6361 7069 7461 6c69 7a65 da07  ....capitalize..
+000010e0: 6765 7461 7474 72da 0969 6d70 6f72 746c  getattr..importl
+000010f0: 6962 da0d 696d 706f 7274 5f6d 6f64 756c  ib..import_modul
+00001100: 65da 0b49 6d70 6f72 7445 7272 6f72 720b  e..ImportErrorr.
+00001110: 0000 00da 0373 6574 5a0a 6765 745f 6576  .....setZ.get_ev
+00001120: 656e 7473 7221 0000 00da 0764 6973 6361  entsr!.....disca
+00001130: 7264 da02 6f73 da04 7061 7468 da04 6a6f  rd..os..path..jo
+00001140: 696e 5a1c 6765 745f 6669 6c65 5f6e 616d  inZ.get_file_nam
+00001150: 655f 666f 725f 6576 656e 745f 6e61 6d65  e_for_event_name
+00001160: da06 6578 6973 7473 da03 6164 6472 0c00  ..exists..addr..
+00001170: 0000 5a0e 6765 6e65 7261 7465 5f63 6c61  ..Z.generate_cla
+00001180: 7373 5a11 6765 745f 6576 656e 745f 6465  ssZ.get_event_de
+00001190: 7461 696c 73da 0269 6472 0a00 0000 da07  tails..idr......
+000011a0: 6d65 7373 6167 65da 046f 7065 6eda 0577  message..open..w
+000011b0: 7269 7465 721f 0000 00da 046c 6973 7429  riter......list)
+000011c0: 1272 2a00 0000 722b 0000 0072 2c00 0000  .r*...r+...r,...
+000011d0: 722d 0000 0072 2e00 0000 722f 0000 0072  r-...r....r/...r
+000011e0: 3000 0000 5a14 6765 6e65 7261 746f 725f  0...Z.generator_
+000011f0: 636c 6173 735f 6e61 6d65 5a0f 6765 6e65  class_nameZ.gene
+00001200: 7261 746f 725f 636c 6173 735a 1065 7665  rator_classZ.eve
+00001210: 6e74 735f 6e6f 745f 666f 756e 645a 0e65  nts_not_foundZ.e
+00001220: 7665 6e74 735f 736b 6970 7065 645a 075f  vents_skippedZ._
+00001230: 6576 656e 7473 5a05 6576 656e 74da 0967  eventsZ.event..g
+00001240: 656e 6572 6174 6f72 5a09 6669 6c65 5f70  eneratorZ.file_p
+00001250: 6174 68da 0463 6f64 65da 0165 da04 6669  ath..code..e..fi
+00001260: 6c65 7211 0000 0072 1100 0000 7212 0000  ler....r....r...
+00001270: 0072 2000 0000 4400 0000 7354 0000 000a  .r ...D...sT....
+00001280: 150e 0202 0112 0102 0108 ff0c 0208 0102  ................
+00001290: ff12 0306 0108 0208 010e 0102 010c 0212  ................
+000012a0: 0106 0216 0310 010a 0112 0102 0104 0202  ................
+000012b0: 021e 010e 010a 0114 010c 0108 8002 fd04  ................
+000012c0: 050c 010c 011c ff02 8002 0306 010c 0102  ................
+000012d0: ff08 ff29 20da 075f 5f64 6f63 5f5f 721c  ...) ..__doc__r.
+000012e0: 0000 0072 3700 0000 da07 6c6f 6767 696e  ...r7.....loggin
+000012f0: 6772 3c00 0000 5a0b 7072 6574 7479 7461  gr<...Z.prettyta
+00001300: 626c 6572 0200 0000 da06 7479 7069 6e67  bler......typing
+00001310: 7203 0000 0072 0400 0000 5a03 6170 695a  r....r....Z.apiZ
+00001320: 0e63 6f6d 6d61 6e64 5f63 6f6e 6669 6772  .command_configr
+00001330: 0800 0000 7209 0000 005a 1965 7863 6570  ....r....Z.excep
+00001340: 7469 6f6e 732e 636c 695f 6578 6365 7074  tions.cli_except
+00001350: 696f 6e73 720a 0000 0072 0b00 0000 da09  ionsr....r......
+00001360: 6765 744c 6f67 6765 7272 1600 0000 da06  getLoggerr......
+00001370: 6c6f 6767 6572 720c 0000 0072 1f00 0000  loggerr....r....
+00001380: da07 636f 6d6d 616e 64da 066f 7074 696f  ..command..optio
+00001390: 6eda 0643 686f 6963 65da 0c70 6173 735f  n..Choice..pass_
+000013a0: 636f 6e74 6578 745a 0953 7465 6c6c 6141  contextZ.StellaA
+000013b0: 5049 7219 0000 00da 0462 6f6f 6cda 0464  PIr......bool..d
+000013c0: 6963 7472 2000 0000 da0c 6765 6e65 7261  ictr .....genera
+000013d0: 7465 5f63 6d64 7211 0000 0072 1100 0000  te_cmdr....r....
+000013e0: 7211 0000 0072 1200 0000 da08 3c6d 6f64  r....r......<mod
+000013f0: 756c 653e 0100 0000 7350 0000 0004 0008  ule>....sP......
+00001400: 1608 0108 0108 010c 0210 0108 0210 0110  ................
+00001410: 010a 050e 0312 090a 1202 0102 0110 0110  ................
+00001420: 0110 0110 0118 0102 0104 ff04 0202 0102  ................
+00001430: 0102 ff02 0202 fe02 0302 fd02 0402 fc06  ................
+00001440: 0502 fb02 0602 fa0a 071c f908 3b         ............;
```

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 20 14:47:41 2023 UTC, .py size: 5210 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0dbc 9164 5a14 0000  o..........dZ...
+00000000: 6f0d 0d0a 0000 0000 34c7 9e64 8514 0000  o.......4..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 d600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6403 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 0100 6401 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 0100 6405 6406 6c0a 6d0b 5a0b 6d0c 5a0c  ..d.d.l.m.Z.m.Z.
@@ -123,166 +123,167 @@
 000007a0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0373  .__qualname__..s
 000007b0: 7472 7211 0000 0072 1300 0000 720f 0000  trr....r....r...
 000007c0: 0072 0f00 0000 720f 0000 0072 1000 0000  .r....r....r....
 000007d0: 720a 0000 0027 0000 0073 0600 0000 0800  r....'...s......
 000007e0: 1201 0c04 720a 0000 00da 0d73 6b69 7070  ....r......skipp
 000007f0: 6564 5f66 696c 6573 da06 7265 7475 726e  ed_files..return
 00000800: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00000810: 0005 0000 0043 0000 0073 5c00 0000 7c00  .....C...s\...|.
-00000820: 722c 7400 6401 8301 0100 7401 6402 6403  r,t.d.....t.d.d.
-00000830: 6702 8301 7d01 7c00 4400 5d0b 7d02 7c01  g...}.|.D.].}.|.
-00000840: a002 7c02 6a03 7c02 6a04 6702 a101 0100  ..|.j.|.j.g.....
-00000850: 710e 7400 7c01 8301 0100 7400 6404 8301  q.t.|.....t.d...
-00000860: 0100 7400 6405 8301 0100 7400 6406 8301  ..t.d.....t.d...
-00000870: 0100 6400 5300 6400 5300 2907 4e7a 500a  ..d.S.d.S.).NzP.
-00000880: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000890: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a20  ==============. 
-000008a0: 2020 2020 2020 2020 5355 4d4d 4152 590a          SUMMARY.
-000008b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000008c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0ada  ==============..
-000008d0: 0446 696c 657a 1852 6561 736f 6e20 666f  .Filez.Reason fo
-000008e0: 7220 6e6f 7420 636f 6d70 6172 696e 677a  r not comparingz
-000008f0: 1f0a 536b 6970 7065 6420 5265 6173 6f6e  ..Skipped Reason
-00000900: 202d 2045 7870 6c61 6e61 7469 6f6e 3a0a   - Explanation:.
-00000910: 7a4c 2d20 4e6f 7420 4175 746f 2d47 656e  zL- Not Auto-Gen
-00000920: 6572 6174 6564 202d 2049 7420 6c6f 6f6b  erated - It look
-00000930: 7320 6c69 6b65 2074 6865 2066 696c 6520  s like the file 
-00000940: 7761 7320 6e6f 7420 6765 6e65 7261 7465  was not generate
-00000950: 6420 6279 2074 6869 7320 434c 492e 7a4c  d by this CLI.zL
-00000960: 2d20 4576 656e 7420 4944 204e 6f74 2046  - Event ID Not F
-00000970: 6f75 6e64 202d 2054 6865 2049 4420 6f66  ound - The ID of
-00000980: 2074 6865 2065 7665 6e74 2069 7320 6d69   the event is mi
-00000990: 7373 696e 6720 696e 2074 6865 2068 6561  ssing in the hea
-000009a0: 6465 7220 636f 6d6d 656e 742e 2905 da05  der comment.)...
-000009b0: 7072 696e 7472 0200 0000 da07 6164 645f  printr......add_
-000009c0: 726f 7772 0b00 0000 720c 0000 0029 0372  rowr....r....).r
-000009d0: 1800 0000 da05 7461 626c 65da 0c73 6b69  ......table..ski
-000009e0: 7070 6564 5f66 696c 6572 0f00 0000 720f  pped_filer....r.
-000009f0: 0000 0072 1000 0000 da0d 7072 696e 745f  ...r......print_
-00000a00: 7375 6d6d 6172 7930 0000 0073 1400 0000  summary0...s....
-00000a10: 0401 0801 0c02 0803 1401 0802 0802 0801  ................
-00000a20: 0c01 04f3 721f 0000 00da 0470 6c61 6e29  ....r......plan)
-00000a30: 01da 046e 616d 657a 0b2d 2d69 6e70 7574  ...namez.--input
-00000a40: 5f64 6972 7a02 2d69 da01 2e7a 2d54 6865  _dirz.-i...z-The
-00000a50: 2064 6972 6563 746f 7279 2074 6f20 7265   directory to re
-00000a60: 6164 2067 656e 6572 6174 6564 2063 6c61  ad generated cla
-00000a70: 7373 6573 2066 726f 6d2e 2902 da07 6465  sses from.)...de
-00000a80: 6661 756c 74da 0468 656c 7063 0300 0000  fault..helpc....
-00000a90: 0000 0000 0000 0000 1200 0000 0b00 0000  ................
-00000aa0: 4b00 0000 73cc 0100 0074 0064 0183 0101  K...s....t.d....
-00000ab0: 0064 0274 0183 0069 017d 0464 037d 0567  .d.t...i.}.d.}.g
-00000ac0: 007d 0674 026a 037c 029b 0064 049d 0264  .}.t.j.|...d...d
-00000ad0: 0564 068d 0244 005d c87d 0774 046a 05a0  .d...D.].}.t.j..
-00000ae0: 067c 07a1 0172 2071 1774 0064 077c 079b  .|...r q.t.d.|..
-00000af0: 009d 0283 0101 0074 046a 05a0 077c 07a1  .......t.j...|..
-00000b00: 015c 027d 087d 097c 04a0 087c 09a1 017d  .\.}.}.|...|...}
-00000b10: 0a7c 0a72 cb74 097c 0764 0883 028f 0c7d  .|.r.t.|.d.....}
-00000b20: 0b7c 0ba0 0aa1 007d 0c57 0064 0904 0004  .|.....}.W.d....
-00000b30: 0083 0301 006e 0831 0073 4a77 0101 0001  .....n.1.sJw....
-00000b40: 0001 0059 0001 007c 057c 0c76 0172 6574  ...Y...|.|.v.ret
-00000b50: 0ba0 0c64 0a7c 079b 0064 0b9d 03a1 0101  ...d.|...d......
-00000b60: 007c 06a0 0d74 0e7c 0764 0c83 02a1 0101  .|...t.|.d......
-00000b70: 0071 1774 0fa0 1064 0d7c 0ca1 027d 0d7c  .q.t...d.|...}.|
-00000b80: 0d64 0975 0072 8174 0ba0 0c64 0a7c 079b  .d.u.r.t...d.|..
-00000b90: 0064 0e9d 03a1 0101 007c 06a0 0d74 0e7c  .d.......|...t.|
-00000ba0: 0764 0f83 02a1 0101 0071 177c 0da0 1164  .d.......q.|...d
-00000bb0: 10a1 017d 0e7a 1e7c 01a0 127c 0ea1 017d  ...}.z.|...|...}
-00000bc0: 0f74 1374 01a0 147c 0f7c 0ca1 0283 017d  .t.t...|.|.....}
-00000bd0: 107c 1072 a374 0064 1183 0101 0074 0064  .|.r.t.d.....t.d
-00000be0: 12a0 157c 10a1 0183 0101 0057 0071 1757  ...|.......W.q.W
-00000bf0: 006e 2104 0074 1679 c501 007d 1101 007a  .n!..t.y...}...z
-00000c00: 1574 0ba0 0c7c 116a 17a1 0101 007c 06a0  .t...|.j.....|..
-00000c10: 0d74 0e7c 077c 116a 1783 02a1 0101 0057  .t.|.|.j.......W
-00000c20: 0059 0064 097d 117e 1171 1764 097d 117e  .Y.d.}.~.q.d.}.~
-00000c30: 1177 0177 0074 0064 1383 0101 0071 1774  .w.w.t.d.....q.t
-00000c40: 0ba0 1864 147c 099b 0064 157c 079b 0064  ...d.|...d.|...d
-00000c50: 169d 05a1 0101 007c 06a0 0d74 0e7c 0764  .......|...t.|.d
-00000c60: 1783 02a1 0101 0071 1774 197c 0683 0101  .......q.t.|....
-00000c70: 0064 0953 0029 187a 7843 6f6d 7061 7265  .d.S.).zxCompare
-00000c80: 7320 6375 7272 656e 746c 7920 6765 6e65  s currently gene
-00000c90: 7261 7465 6420 636c 6173 7365 7320 7769  rated classes wi
-00000ca0: 7468 2074 6865 2073 7065 6369 6669 6361  th the specifica
-00000cb0: 7469 6f6e 7320 6665 7463 6865 6420 6672  tions fetched fr
-00000cc0: 6f6d 2074 6865 2041 5049 2061 6e64 2070  om the API and p
-00000cd0: 726f 7669 6465 7320 6120 7375 6d6d 6172  rovides a summar
-00000ce0: 7920 6f66 0a20 2020 2063 6861 6e67 6573  y of.    changes
-00000cf0: 2e7a 0b50 6c61 6e6e 696e 672e 2e2e 7a03  .z.Planning...z.
-00000d00: 2e63 737a 3954 6869 7320 6669 6c65 2069  .csz9This file i
-00000d10: 7320 6175 746f 2d67 656e 6572 6174 6564  s auto-generated
-00000d20: 2062 7920 5374 656c 6c61 4e6f 7743 4c49   by StellaNowCLI
-00000d30: 2e20 444f 204e 4f54 2045 4449 542e 7a03  . DO NOT EDIT.z.
-00000d40: 2f2a 2a54 2901 da09 7265 6375 7273 6976  /**T)...recursiv
-00000d50: 657a 343d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ez4=============
-00000d60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000d70: 3d0a 436f 6d70 6172 6973 6f6e 2066 6f72  =.Comparison for
-00000d80: 2066 696c 653a 20da 0172 4e7a 0953 6b69   file: ..rNz.Ski
-00000d90: 7070 696e 6720 7a23 2062 6563 6175 7365  pping z# because
-00000da0: 2069 7420 7761 7320 6e6f 7420 6175 746f   it was not auto
-00000db0: 2d67 656e 6572 6174 6564 2e7a 124e 6f74  -generated.z.Not
-00000dc0: 2041 7574 6f2d 4765 6e65 7261 7465 647a   Auto-Generatedz
-00000dd0: 5745 7665 6e74 2049 443a 2028 5b30 2d39  WEvent ID: ([0-9
-00000de0: 612d 6641 2d46 5d7b 387d 2d5b 302d 3961  a-fA-F]{8}-[0-9a
-00000df0: 2d66 412d 465d 7b34 7d2d 5b30 2d39 612d  -fA-F]{4}-[0-9a-
-00000e00: 6641 2d46 5d7b 347d 2d5b 302d 3961 2d66  fA-F]{4}-[0-9a-f
-00000e10: 412d 465d 7b34 7d2d 5b30 2d39 612d 6641  A-F]{4}-[0-9a-fA
-00000e20: 2d46 5d7b 3132 7d29 7a1f 2062 6563 6175  -F]{12})z. becau
-00000e30: 7365 206e 6f20 4576 656e 7420 4944 2077  se no Event ID w
-00000e40: 6173 2066 6f75 6e64 2e7a 1245 7665 6e74  as found.z.Event
-00000e50: 2049 4420 4e6f 7420 466f 756e 6472 0400   ID Not Foundr..
-00000e60: 0000 7a11 4368 616e 6765 7320 4465 7465  ..z.Changes Dete
-00000e70: 6374 6564 3ada 007a 144e 6f20 6368 616e  cted:..z.No chan
-00000e80: 6765 7320 6465 7465 6374 6564 2e7a 214e  ges detected.z!N
-00000e90: 6f20 6765 6e65 7261 746f 7220 666f 756e  o generator foun
-00000ea0: 6420 666f 7220 6669 6c65 2074 7970 6520  d for file type 
-00000eb0: 7a0b 2e20 536b 6970 7069 6e67 2072 2200  z.. Skipping r".
-00000ec0: 0000 7a14 556e 7375 7070 6f72 7465 6420  ..z.Unsupported 
-00000ed0: 4c61 6e67 7561 6765 291a 721b 0000 0072  Language).r....r
-00000ee0: 0800 0000 da04 676c 6f62 5a05 6967 6c6f  ......globZ.iglo
-00000ef0: 62da 026f 73da 0470 6174 68da 0569 7364  b..os..path..isd
-00000f00: 6972 da08 7370 6c69 7465 7874 da03 6765  ir..splitext..ge
-00000f10: 74da 046f 7065 6eda 0472 6561 64da 066c  t..open..read..l
-00000f20: 6f67 6765 72da 0777 6172 6e69 6e67 da06  ogger..warning..
-00000f30: 6170 7065 6e64 720a 0000 00da 0272 65da  appendr......re.
-00000f40: 0673 6561 7263 68da 0567 726f 7570 da11  .search..group..
-00000f50: 6765 745f 6576 656e 745f 6465 7461 696c  get_event_detail
-00000f60: 73da 046c 6973 745a 0867 6574 5f64 6966  s..listZ.get_dif
-00000f70: 66da 046a 6f69 6e72 0900 0000 da07 6d65  f..joinr......me
-00000f80: 7373 6167 65da 0565 7272 6f72 721f 0000  ssage..errorr...
-00000f90: 0029 12da 0363 7478 da0a 7374 656c 6c61  .)...ctx..stella
-00000fa0: 5f61 7069 5a09 696e 7075 745f 6469 72da  _apiZ.input_dir.
-00000fb0: 066b 7761 7267 73da 0a67 656e 6572 6174  .kwargs..generat
-00000fc0: 6f72 735a 1661 7574 6f5f 6765 6e65 7261  orsZ.auto_genera
-00000fd0: 7465 645f 636f 6d6d 656e 7472 1800 0000  ted_commentr....
-00000fe0: 720b 0000 00da 015f da03 6578 74da 0967  r......_..ext..g
-00000ff0: 656e 6572 6174 6f72 da01 665a 0d65 7869  enerator..fZ.exi
-00001000: 7374 696e 675f 636f 6465 5a0f 6576 656e  sting_codeZ.even
-00001010: 745f 6964 5f73 6561 7263 68da 0865 7665  t_id_search..eve
-00001020: 6e74 5f69 645a 0c65 7665 6e74 5f64 6574  nt_idZ.event_det
-00001030: 6169 6c5a 0464 6966 66da 0165 720f 0000  ailZ.diff..er...
-00001040: 0072 0f00 0000 7210 0000 0072 2000 0000  .r....r....r ...
-00001050: 4100 0000 735c 0000 0008 0806 0404 ff04  A...s\..........
-00001060: 0504 0218 030c 0202 010e 0210 010a 0104  ................
-00001070: 020c 010a 011c ff08 0412 0110 0102 0104  ................
-00001080: 0302 0102 0104 fe08 0412 0110 0102 010a  ................
-00001090: 0202 020a 0110 0204 0108 010e 0104 0104  ................
-000010a0: fd0e 040c 0112 010c 0108 8002 fd0a 0518  ................
-000010b0: 0312 010c 0229 1bda 075f 5f64 6f63 5f5f  .....)...__doc__
-000010c0: 7229 0000 0072 3300 0000 7228 0000 00da  r)...r3...r(....
-000010d0: 0563 6c69 636b da07 6c6f 6767 696e 67da  .click..logging.
-000010e0: 0b70 7265 7474 7974 6162 6c65 7202 0000  .prettytabler...
-000010f0: 00da 0674 7970 696e 6772 0300 0000 da0e  ...typingr......
-00001100: 636f 6d6d 616e 645f 636f 6e66 6967 7205  command_configr.
-00001110: 0000 0072 0600 0000 5a0f 636f 6465 5f67  ...r....Z.code_g
-00001120: 656e 6572 6174 6f72 7372 0800 0000 5a20  eneratorsr....Z 
-00001130: 6578 6365 7074 696f 6e73 2e53 7465 6c6c  exceptions.Stell
-00001140: 614e 6f77 434c 4945 7863 6570 7469 6f6e  aNowCLIException
-00001150: 7209 0000 00da 0967 6574 4c6f 6767 6572  r......getLogger
-00001160: 7214 0000 0072 3000 0000 720a 0000 0072  r....r0...r....r
-00001170: 1f00 0000 da07 636f 6d6d 616e 64da 066f  ......command..o
-00001180: 7074 696f 6eda 0c70 6173 735f 636f 6e74  ption..pass_cont
-00001190: 6578 7472 2000 0000 da08 706c 616e 5f63  extr .....plan_c
-000011a0: 6d64 720f 0000 0072 0f00 0000 720f 0000  mdr....r....r...
-000011b0: 0072 1000 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-000011c0: 0100 0000 732a 0000 0004 0008 1608 0108  ....s*..........
-000011d0: 0108 0108 010c 020c 0110 020c 010c 010a  ................
-000011e0: 020e 0316 090a 1102 0102 0110 0104 0112  ................
-000011f0: 0108 45                                  ..E
+00000810: 0005 0000 0043 0000 0073 6600 0000 7c00  .....C...sf...|.
+00000820: 7231 7400 a001 6401 a101 0100 7402 6402  r1t...d.....t.d.
+00000830: 6403 6702 8301 7d01 7c00 4400 5d0b 7d02  d.g...}.|.D.].}.
+00000840: 7c01 a003 7c02 6a04 7c02 6a05 6702 a101  |...|.j.|.j.g...
+00000850: 0100 710f 7400 a001 7c01 a101 0100 7400  ..q.t...|.....t.
+00000860: a001 6404 a101 0100 7400 a001 6405 a101  ..d.....t...d...
+00000870: 0100 7400 a001 6406 a101 0100 6400 5300  ..t...d.....d.S.
+00000880: 6400 5300 2907 4e7a 500a 3d3d 3d3d 3d3d  d.S.).NzP.======
+00000890: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000008a0: 3d3d 3d3d 3d3d 3d3d 0a20 2020 2020 2020  ========.       
+000008b0: 2020 5355 4d4d 4152 590a 3d3d 3d3d 3d3d    SUMMARY.======
+000008c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000008d0: 3d3d 3d3d 3d3d 3d3d 0ada 0446 696c 657a  ========...Filez
+000008e0: 1852 6561 736f 6e20 666f 7220 6e6f 7420  .Reason for not 
+000008f0: 636f 6d70 6172 696e 677a 1f0a 536b 6970  comparingz..Skip
+00000900: 7065 6420 5265 6173 6f6e 202d 2045 7870  ped Reason - Exp
+00000910: 6c61 6e61 7469 6f6e 3a0a 7a4c 2d20 4e6f  lanation:.zL- No
+00000920: 7420 4175 746f 2d47 656e 6572 6174 6564  t Auto-Generated
+00000930: 202d 2049 7420 6c6f 6f6b 7320 6c69 6b65   - It looks like
+00000940: 2074 6865 2066 696c 6520 7761 7320 6e6f   the file was no
+00000950: 7420 6765 6e65 7261 7465 6420 6279 2074  t generated by t
+00000960: 6869 7320 434c 492e 7a4c 2d20 4576 656e  his CLI.zL- Even
+00000970: 7420 4944 204e 6f74 2046 6f75 6e64 202d  t ID Not Found -
+00000980: 2054 6865 2049 4420 6f66 2074 6865 2065   The ID of the e
+00000990: 7665 6e74 2069 7320 6d69 7373 696e 6720  vent is missing 
+000009a0: 696e 2074 6865 2068 6561 6465 7220 636f  in the header co
+000009b0: 6d6d 656e 742e 2906 da05 636c 6963 6bda  mment.)...click.
+000009c0: 0465 6368 6f72 0200 0000 da07 6164 645f  .echor......add_
+000009d0: 726f 7772 0b00 0000 720c 0000 0029 0372  rowr....r....).r
+000009e0: 1800 0000 da05 7461 626c 65da 0c73 6b69  ......table..ski
+000009f0: 7070 6564 5f66 696c 6572 0f00 0000 720f  pped_filer....r.
+00000a00: 0000 0072 1000 0000 da0d 7072 696e 745f  ...r......print_
+00000a10: 7375 6d6d 6172 7930 0000 0073 1400 0000  summary0...s....
+00000a20: 0401 0a01 0c02 0803 1401 0a02 0a02 0a01  ................
+00000a30: 0e01 04f3 7220 0000 00da 0470 6c61 6e29  ....r .....plan)
+00000a40: 01da 046e 616d 657a 0b2d 2d69 6e70 7574  ...namez.--input
+00000a50: 5f64 6972 7a02 2d69 da01 2e7a 2d54 6865  _dirz.-i...z-The
+00000a60: 2064 6972 6563 746f 7279 2074 6f20 7265   directory to re
+00000a70: 6164 2067 656e 6572 6174 6564 2063 6c61  ad generated cla
+00000a80: 7373 6573 2066 726f 6d2e 2902 da07 6465  sses from.)...de
+00000a90: 6661 756c 74da 0468 656c 7063 0300 0000  fault..helpc....
+00000aa0: 0000 0000 0000 0000 1200 0000 0b00 0000  ................
+00000ab0: 4b00 0000 73d6 0100 0074 00a0 0164 01a1  K...s....t...d..
+00000ac0: 0101 0064 0274 0283 0069 017d 0464 037d  ...d.t...i.}.d.}
+00000ad0: 0567 007d 0674 036a 047c 029b 0064 049d  .g.}.t.j.|...d..
+00000ae0: 0264 0564 068d 0244 005d cc7d 0774 056a  .d.d...D.].}.t.j
+00000af0: 06a0 077c 07a1 0172 2171 1874 00a0 0164  ...|...r!q.t...d
+00000b00: 077c 079b 009d 02a1 0101 0074 056a 06a0  .|.........t.j..
+00000b10: 087c 07a1 015c 027d 087d 097c 04a0 097c  .|...\.}.}.|...|
+00000b20: 09a1 017d 0a7c 0a72 d074 0a7c 0764 0883  ...}.|.r.t.|.d..
+00000b30: 028f 0c7d 0b7c 0ba0 0ba1 007d 0c57 0064  ...}.|.....}.W.d
+00000b40: 0904 0004 0083 0301 006e 0831 0073 4c77  .........n.1.sLw
+00000b50: 0101 0001 0001 0059 0001 007c 057c 0c76  .......Y...|.|.v
+00000b60: 0172 6774 0ca0 0d64 0a7c 079b 0064 0b9d  .rgt...d.|...d..
+00000b70: 03a1 0101 007c 06a0 0e74 0f7c 0764 0c83  .....|...t.|.d..
+00000b80: 02a1 0101 0071 1874 10a0 1164 0d7c 0ca1  .....q.t...d.|..
+00000b90: 027d 0d7c 0d64 0975 0072 8374 0ca0 0d64  .}.|.d.u.r.t...d
+00000ba0: 0a7c 079b 0064 0e9d 03a1 0101 007c 06a0  .|...d.......|..
+00000bb0: 0e74 0f7c 0764 0f83 02a1 0101 0071 187c  .t.|.d.......q.|
+00000bc0: 0da0 1264 10a1 017d 0e7a 207c 01a0 137c  ...d...}.z |...|
+00000bd0: 0ea1 017d 0f74 1474 02a0 157c 0f7c 0ca1  ...}.t.t...|.|..
+00000be0: 0283 017d 107c 1072 a774 00a0 0164 11a1  ...}.|.r.t...d..
+00000bf0: 0101 0074 00a0 0164 12a0 167c 10a1 01a1  ...t...d...|....
+00000c00: 0101 0057 0071 1857 006e 2104 0074 1779  ...W.q.W.n!..t.y
+00000c10: c901 007d 1101 007a 1574 0ca0 0d7c 116a  ...}...z.t...|.j
+00000c20: 18a1 0101 007c 06a0 0e74 0f7c 077c 116a  .....|...t.|.|.j
+00000c30: 1883 02a1 0101 0057 0059 0064 097d 117e  .......W.Y.d.}.~
+00000c40: 1171 1864 097d 117e 1177 0177 0074 00a0  .q.d.}.~.w.w.t..
+00000c50: 0164 13a1 0101 0071 1874 0ca0 1964 147c  .d.....q.t...d.|
+00000c60: 099b 0064 157c 079b 0064 169d 05a1 0101  ...d.|...d......
+00000c70: 007c 06a0 0e74 0f7c 0764 1783 02a1 0101  .|...t.|.d......
+00000c80: 0071 1874 1a7c 0683 0101 0064 0953 0029  .q.t.|.....d.S.)
+00000c90: 187a 7843 6f6d 7061 7265 7320 6375 7272  .zxCompares curr
+00000ca0: 656e 746c 7920 6765 6e65 7261 7465 6420  ently generated 
+00000cb0: 636c 6173 7365 7320 7769 7468 2074 6865  classes with the
+00000cc0: 2073 7065 6369 6669 6361 7469 6f6e 7320   specifications 
+00000cd0: 6665 7463 6865 6420 6672 6f6d 2074 6865  fetched from the
+00000ce0: 2041 5049 2061 6e64 2070 726f 7669 6465   API and provide
+00000cf0: 7320 6120 7375 6d6d 6172 7920 6f66 0a20  s a summary of. 
+00000d00: 2020 2063 6861 6e67 6573 2e7a 0b50 6c61     changes.z.Pla
+00000d10: 6e6e 696e 672e 2e2e 7a03 2e63 737a 3954  nning...z..csz9T
+00000d20: 6869 7320 6669 6c65 2069 7320 6175 746f  his file is auto
+00000d30: 2d67 656e 6572 6174 6564 2062 7920 5374  -generated by St
+00000d40: 656c 6c61 4e6f 7743 4c49 2e20 444f 204e  ellaNowCLI. DO N
+00000d50: 4f54 2045 4449 542e 7a03 2f2a 2a54 2901  OT EDIT.z./**T).
+00000d60: da09 7265 6375 7273 6976 657a 343d 3d3d  ..recursivez4===
+00000d70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000d80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 436f 6d70  ===========.Comp
+00000d90: 6172 6973 6f6e 2066 6f72 2066 696c 653a  arison for file:
+00000da0: 20da 0172 4e7a 0953 6b69 7070 696e 6720   ..rNz.Skipping 
+00000db0: 7a23 2062 6563 6175 7365 2069 7420 7761  z# because it wa
+00000dc0: 7320 6e6f 7420 6175 746f 2d67 656e 6572  s not auto-gener
+00000dd0: 6174 6564 2e7a 124e 6f74 2041 7574 6f2d  ated.z.Not Auto-
+00000de0: 4765 6e65 7261 7465 647a 5745 7665 6e74  GeneratedzWEvent
+00000df0: 2049 443a 2028 5b30 2d39 612d 6641 2d46   ID: ([0-9a-fA-F
+00000e00: 5d7b 387d 2d5b 302d 3961 2d66 412d 465d  ]{8}-[0-9a-fA-F]
+00000e10: 7b34 7d2d 5b30 2d39 612d 6641 2d46 5d7b  {4}-[0-9a-fA-F]{
+00000e20: 347d 2d5b 302d 3961 2d66 412d 465d 7b34  4}-[0-9a-fA-F]{4
+00000e30: 7d2d 5b30 2d39 612d 6641 2d46 5d7b 3132  }-[0-9a-fA-F]{12
+00000e40: 7d29 7a1f 2062 6563 6175 7365 206e 6f20  })z. because no 
+00000e50: 4576 656e 7420 4944 2077 6173 2066 6f75  Event ID was fou
+00000e60: 6e64 2e7a 1245 7665 6e74 2049 4420 4e6f  nd.z.Event ID No
+00000e70: 7420 466f 756e 6472 0400 0000 7a11 4368  t Foundr....z.Ch
+00000e80: 616e 6765 7320 4465 7465 6374 6564 3ada  anges Detected:.
+00000e90: 007a 144e 6f20 6368 616e 6765 7320 6465  .z.No changes de
+00000ea0: 7465 6374 6564 2e7a 214e 6f20 6765 6e65  tected.z!No gene
+00000eb0: 7261 746f 7220 666f 756e 6420 666f 7220  rator found for 
+00000ec0: 6669 6c65 2074 7970 6520 7a0b 2e20 536b  file type z.. Sk
+00000ed0: 6970 7069 6e67 2072 2300 0000 7a14 556e  ipping r#...z.Un
+00000ee0: 7375 7070 6f72 7465 6420 4c61 6e67 7561  supported Langua
+00000ef0: 6765 291b 721b 0000 0072 1c00 0000 7208  ge).r....r....r.
+00000f00: 0000 00da 0467 6c6f 625a 0569 676c 6f62  .....globZ.iglob
+00000f10: da02 6f73 da04 7061 7468 da05 6973 6469  ..os..path..isdi
+00000f20: 72da 0873 706c 6974 6578 74da 0367 6574  r..splitext..get
+00000f30: da04 6f70 656e da04 7265 6164 da06 6c6f  ..open..read..lo
+00000f40: 6767 6572 da07 7761 726e 696e 67da 0661  gger..warning..a
+00000f50: 7070 656e 6472 0a00 0000 da02 7265 da06  ppendr......re..
+00000f60: 7365 6172 6368 da05 6772 6f75 70da 1167  search..group..g
+00000f70: 6574 5f65 7665 6e74 5f64 6574 6169 6c73  et_event_details
+00000f80: da04 6c69 7374 5a08 6765 745f 6469 6666  ..listZ.get_diff
+00000f90: da04 6a6f 696e 7209 0000 00da 076d 6573  ..joinr......mes
+00000fa0: 7361 6765 da05 6572 726f 7272 2000 0000  sage..errorr ...
+00000fb0: 2912 da03 6374 78da 0a73 7465 6c6c 615f  )...ctx..stella_
+00000fc0: 6170 695a 0969 6e70 7574 5f64 6972 da06  apiZ.input_dir..
+00000fd0: 6b77 6172 6773 da0a 6765 6e65 7261 746f  kwargs..generato
+00000fe0: 7273 5a16 6175 746f 5f67 656e 6572 6174  rsZ.auto_generat
+00000ff0: 6564 5f63 6f6d 6d65 6e74 7218 0000 0072  ed_commentr....r
+00001000: 0b00 0000 da01 5fda 0365 7874 da09 6765  ......_..ext..ge
+00001010: 6e65 7261 746f 72da 0166 5a0d 6578 6973  nerator..fZ.exis
+00001020: 7469 6e67 5f63 6f64 655a 0f65 7665 6e74  ting_codeZ.event
+00001030: 5f69 645f 7365 6172 6368 da08 6576 656e  _id_search..even
+00001040: 745f 6964 5a0c 6576 656e 745f 6465 7461  t_idZ.event_deta
+00001050: 696c 5a04 6469 6666 da01 6572 0f00 0000  ilZ.diff..er....
+00001060: 720f 0000 0072 1000 0000 7221 0000 0041  r....r....r!...A
+00001070: 0000 0073 5c00 0000 0a08 0604 04ff 0405  ...s\...........
+00001080: 0402 1803 0c02 0201 1002 1001 0a01 0402  ................
+00001090: 0c01 0a01 1cff 0804 1201 1001 0201 0403  ................
+000010a0: 0201 0201 04fe 0804 1201 1001 0201 0a02  ................
+000010b0: 0202 0a01 1002 0401 0a01 1001 0401 04fd  ................
+000010c0: 0e04 0c01 1201 0c01 0880 02fd 0c05 1803  ................
+000010d0: 1201 0c02 291b da07 5f5f 646f 635f 5f72  ....)...__doc__r
+000010e0: 2a00 0000 7234 0000 0072 2900 0000 721b  *...r4...r)...r.
+000010f0: 0000 00da 076c 6f67 6769 6e67 da0b 7072  .....logging..pr
+00001100: 6574 7479 7461 626c 6572 0200 0000 da06  ettytabler......
+00001110: 7479 7069 6e67 7203 0000 00da 0e63 6f6d  typingr......com
+00001120: 6d61 6e64 5f63 6f6e 6669 6772 0500 0000  mand_configr....
+00001130: 7206 0000 005a 0f63 6f64 655f 6765 6e65  r....Z.code_gene
+00001140: 7261 746f 7273 7208 0000 005a 1965 7863  ratorsr....Z.exc
+00001150: 6570 7469 6f6e 732e 636c 695f 6578 6365  eptions.cli_exce
+00001160: 7074 696f 6e73 7209 0000 00da 0967 6574  ptionsr......get
+00001170: 4c6f 6767 6572 7214 0000 0072 3100 0000  Loggerr....r1...
+00001180: 720a 0000 0072 2000 0000 da07 636f 6d6d  r....r .....comm
+00001190: 616e 64da 066f 7074 696f 6eda 0c70 6173  and..option..pas
+000011a0: 735f 636f 6e74 6578 7472 2100 0000 da08  s_contextr!.....
+000011b0: 706c 616e 5f63 6d64 720f 0000 0072 0f00  plan_cmdr....r..
+000011c0: 0000 720f 0000 0072 1000 0000 da08 3c6d  ..r....r......<m
+000011d0: 6f64 756c 653e 0100 0000 732a 0000 0004  odule>....s*....
+000011e0: 0008 1608 0108 0108 0108 010c 020c 0110  ................
+000011f0: 020c 010c 010a 020e 0316 090a 1102 0102  ................
+00001200: 0110 0104 0112 0108 45                   ........E
```

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/commands/_init__.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/commands/_init__.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/commands/command_config.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/commands/command_config.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/commands/configure.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/commands/configure.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                    "If no profile is specified, the configurations will be stored under the 'DEFAULT' profile.")
 @click.option('--env', hidden=True, type=click.Choice([e.value for e in Env], case_sensitive=False))
 @click.pass_context
 def configure(ctx, profile, env):
     """Sets up the necessary credentials and configurations for a specific profile or for the DEFAULT profile if none
     is specified."""
 
-    print(f'Provide configuration for profile: {profile}')
+    click.echo(f'Provide configuration for profile: {profile}')
 
     config = ctx.obj
 
     access_key = config.get(profile, "access_key", fallback=None)
     access_token = config.get(profile, "access_token", fallback=None)
     organization_id = config.get(profile, "organization_id", fallback=None)
     project_id = config.get(profile, "project_id", fallback=None)
@@ -108,11 +108,11 @@
     if env is not None:
         config[profile]['env'] = env
 
     # Write the updated configuration to the file
     with open(config_file, "w") as configfile:
         config.write(configfile)
 
-    print(f"Configuration for profile '{profile}' saved successfully")
+    click.echo(f"Configuration for profile '{profile}' saved successfully")
 
 
 configure_cmd = configure
```

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/commands/events.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/commands/events.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,24 +30,24 @@
 @click.command(name='events')
 @common_option
 @load_config
 @click.pass_context
 def events(ctx, stella_api, organization_id, project_id, **kwargs):
     """Fetches the latest event specifications from the API and output a list of the events into the terminal prompt."""
 
-    print(f"\n\nOrganizationId: {organization_id}\nProjectId: {project_id}\n\n")
+    click.echo(f"\n\nOrganizationId: {organization_id}\nProjectId: {project_id}\n\n")
 
     _events = stella_api.get_events()
 
     table = PrettyTable(['EventID', 'Event Name', "Is Active", "Created At", "Updated At"])
 
     # Populate the table with data from your SkippedFile instances
     for event in _events:
         table.add_row([event.id, event.name, event.isActive, event.createdAt, event.updatedAt])
 
-    print(table)
+    click.echo(table)
 
     for event in _events:
-        print(f'ID: {event.id}, Name: {event.name}')
+        click.echo(f'ID: {event.id}, Name: {event.name}')
 
 
 events_cmd = events
```

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/commands/generate.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/commands/generate.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import os
 
 from prettytable import PrettyTable
 from typing import Any, List
 
 from ..api import *
 from .command_config import common_option, load_config
-from ..exceptions.StellaNowCLIException import (
+from ..exceptions.cli_exceptions import (
     StellaNowCLIException,
     StellaNowCLILanguageNotSupportedException
 )
 
 logger = logging.getLogger(__name__)
 
 
@@ -45,28 +45,28 @@
 
     def __iter__(self):
         return iter([self.filename, self.reason])
 
 
 def print_skipped_result(skipped_files: List[SkippedFile]):
     if skipped_files:
-        print("\n==============================\n         SUMMARY\n==============================\n")
+        click.echo("\n==============================\n         SUMMARY\n==============================\n")
 
         table = PrettyTable(['File', 'Skipping Reason'])
 
         # Populate the table with data from your SkippedFile instances
         for skipped_file in skipped_files:
             table.add_row([skipped_file.filename, skipped_file.reason])
 
-        print(table)
+        click.echo(table)
 
-        print("\nSkipped Reason - Explanation:\n")
-        print("- File Already Exist - Existing classes can't be overriden. Use --force to override this protection.")
-        print("- Missing Event Configuration - Check if the specified event does exists in then Operators Console.")
-        print("- No Entity Associated With Event - Event exists, but it is not attached to any entity type.")
+        click.echo("\nSkipped Reason - Explanation:\n")
+        click.echo("- File Already Exist - Existing classes can't be overriden. Use --force to override this protection.")
+        click.echo("- Missing Event Configuration - Check if the specified event does exists in then Operators Console.")
+        click.echo("- No Entity Associated With Event - Event exists, but it is not attached to any entity type.")
 
 
 @click.command(name='generate')
 @common_option
 @load_config
 @click.option('--namespace', '-n', default='', help='The namespace for the generated classes.')
 @click.option('--destination', '-d', default='.', help='The directory to save the generated classes.')
@@ -82,15 +82,15 @@
         force: bool,
         events: List[str],
         language: str,
         **kwargs: dict[str, Any]
 ):
     """Fetches the latest event specifications from the API and generates corresponding class code in the desired
     programming language."""
-    print('Generating...')
+    click.echo('Generating...')
 
     generator_class_name = f"{language.capitalize()}CodeGenerator"
     try:
         generator_class = getattr(importlib.import_module(f"stellanow_cli.code_generators.{language}_code_generator"),
                                   generator_class_name)
     except ImportError:
         raise StellaNowCLILanguageNotSupportedException(language)
@@ -100,31 +100,31 @@
 
     _events = stella_api.get_events()
     for event in _events:
         if events and event.name not in events:
             continue
 
         events_not_found.discard(event.name)  # remove event from 'not found' list
-        print(f'Generating class for event: {event.name}')
+        click.echo(f'Generating class for event: {event.name}')
 
         generator = generator_class()
 
         # Save the code to a file
         file_path = os.path.join(destination, generator.get_file_name_for_event_name(event.name))
         if not force and os.path.exists(file_path):
-            print('Skipped ...')
+            click.echo('Skipped ...')
             events_skipped.add(SkippedFile(event.name, 'File Already Exist'))  # add event to skipped list
             continue
 
         code = None
 
         try:
             code = generator.generate_class(stella_api.get_event_details(event.id), **kwargs)
         except StellaNowCLIException as e:
-            print('Skipped ...')
+            click.echo('Skipped ...')
             events_skipped.add(SkippedFile(event.name, e.message))  # add event to skipped list
             continue
 
         if code:
             with open(file_path, "w") as file:
                 file.write(code)
```

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/commands/plan.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/commands/plan.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import logging
 
 from prettytable import PrettyTable
 from typing import List
 
 from .command_config import common_option, load_config
 from ..code_generators import CsharpCodeGenerator
-from ..exceptions.StellaNowCLIException import StellaNowCLIException
+from ..exceptions.cli_exceptions import StellaNowCLIException
 
 logger = logging.getLogger(__name__)
 
 
 class SkippedFile:
     def __init__(self, filename: str, reason: str):
         self.filename = filename
@@ -43,38 +43,38 @@
 
     def __iter__(self):
         return iter([self.filename, self.reason])
 
 
 def print_summary(skipped_files: List[SkippedFile]) -> None:
     if skipped_files:
-        print("\n==============================\n         SUMMARY\n==============================\n")
+        click.echo("\n==============================\n         SUMMARY\n==============================\n")
 
         table = PrettyTable(['File', 'Reason for not comparing'])
 
         # Populate the table with data from your SkippedFile instances
         for skipped_file in skipped_files:
             table.add_row([skipped_file.filename, skipped_file.reason])
 
-        print(table)
+        click.echo(table)
 
-        print("\nSkipped Reason - Explanation:\n")
-        print("- Not Auto-Generated - It looks like the file was not generated by this CLI.")
-        print("- Event ID Not Found - The ID of the event is missing in the header comment.")
+        click.echo("\nSkipped Reason - Explanation:\n")
+        click.echo("- Not Auto-Generated - It looks like the file was not generated by this CLI.")
+        click.echo("- Event ID Not Found - The ID of the event is missing in the header comment.")
 
 
 @click.command(name='plan')
 @common_option
 @load_config
 @click.option('--input_dir', '-i', default='.', help='The directory to read generated classes from.')
 @click.pass_context
 def plan(ctx, stella_api, input_dir, **kwargs):
     """Compares currently generated classes with the specifications fetched from the API and provides a summary of
     changes."""
-    print('Planning...')
+    click.echo('Planning...')
 
     # We will need to map the file extensions to the appropriate code generators
     generators = {
         '.cs': CsharpCodeGenerator()
     }
 
     # This is the unique comment that should be present in all auto-generated files
@@ -84,15 +84,15 @@
 
     # Let's iterate over all the files in the input directory
     for filename in glob.iglob(f'{input_dir}/**', recursive=True):
         # Skip if the filename is a directory
         if os.path.isdir(filename):
             continue
 
-        print(f"==============================\nComparison for file: {filename}")
+        click.echo(f"==============================\nComparison for file: {filename}")
         _, ext = os.path.splitext(filename)
         generator = generators.get(ext)
 
         if generator:
             with open(filename, 'r') as f:
                 existing_code = f.read()
 
@@ -115,23 +115,23 @@
             event_id = event_id_search.group(1)
 
             try:
                 event_detail = stella_api.get_event_details(event_id)
 
                 diff = list(CsharpCodeGenerator.get_diff(event_detail, existing_code))
                 if diff:
-                    print("Changes Detected:")
-                    print(''.join(diff))
+                    click.echo("Changes Detected:")
+                    click.echo(''.join(diff))
                     continue
             except StellaNowCLIException as e:
                 logger.warning(e.message)
                 skipped_files.append(SkippedFile(filename, e.message))
                 continue
 
-            print(f"No changes detected.")
+            click.echo(f"No changes detected.")
 
         else:
             logger.error(f'No generator found for file type {ext}. Skipping {filename}.')
             skipped_files.append(SkippedFile(filename, "Unsupported Language"))
 
     print_summary(skipped_files)
```

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/config/__init__.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/config/__pycache__/config.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/config/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/config/__pycache__/dev.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/config/__pycache__/dev.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/config/__pycache__/int.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/config/__pycache__/int.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/config/config.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/config/config.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/config/dev.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/config/dev.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/config/int.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/config/int.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/StellaNowAPIExceptions.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/api_exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 IN THE SOFTWARE.
 """
 
 from typing import List
 
-from .StellaNowCLIException import StellaNowCLIException
+from .cli_exceptions import StellaNowCLIException
 
 
 class StellaAPIError(StellaNowCLIException):
     """Exception raised for errors in the Stella API."""
 
 
 class StellaAPIForbiddenError(StellaAPIError):
```

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/StellaNowCLIException.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/cli_exceptions.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/__init__.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/__pycache__/StellaNowAPIExceptions.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/__pycache__/api_exceptions.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 20 14:47:41 2023 UTC, .py size: 2208 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-00000000: 6f0d 0d0a 0000 0000 0dbc 9164 a008 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 84b0 9e64 9908 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6403  Z.d.d.l.m.Z...d.
-00000040: 6404 6c03 6d03 5a03 0100 4700 6405 6406  d.l.m.Z...G.d.d.
-00000050: 8400 6406 6503 8303 5a04 4700 6407 6408  ..d.e...Z.G.d.d.
-00000060: 8400 6408 6504 8303 5a05 4700 6409 640a  ..d.e...Z.G.d.d.
-00000070: 8400 640a 6504 8303 5a06 4700 640b 640c  ..d.e...Z.G.d.d.
-00000080: 8400 640c 6504 8303 5a07 4700 640d 640e  ..d.e...Z.G.d.d.
-00000090: 8400 640e 6504 8303 5a08 640f 5300 2910  ..d.e...Z.d.S.).
+00000040: 6404 6c03 6d04 5a04 0100 4700 6405 6406  d.l.m.Z...G.d.d.
+00000050: 8400 6406 6504 8303 5a05 4700 6407 6408  ..d.e...Z.G.d.d.
+00000060: 8400 6408 6505 8303 5a06 4700 6409 640a  ..d.e...Z.G.d.d.
+00000070: 8400 640a 6505 8303 5a07 4700 640b 640c  ..d.e...Z.G.d.d.
+00000080: 8400 640c 6505 8303 5a08 4700 640d 640e  ..d.e...Z.G.d.d.
+00000090: 8400 640e 6505 8303 5a09 640f 5300 2910  ..d.e...Z.d.S.).
 000000a0: 613b 0400 000a 436f 7079 7269 6768 7420  a;....Copyright 
 000000b0: 2843 2920 3230 3232 2d32 3032 3320 5374  (C) 2022-2023 St
 000000c0: 656c 6c61 2054 6563 686e 6f6c 6f67 6965  ella Technologie
 000000d0: 7320 2855 4b29 204c 696d 6974 6564 2e0a  s (UK) Limited..
 000000e0: 0a50 6572 6d69 7373 696f 6e20 6973 2068  .Permission is h
 000000f0: 6572 6562 7920 6772 616e 7465 642c 2066  ereby granted, f
 00000100: 7265 6520 6f66 2063 6861 7267 652c 2074  ree of charge, t
@@ -85,113 +85,113 @@
 00000540: 6c6c 6141 5049 4572 726f 727a 2e45 7863  llaAPIErrorz.Exc
 00000550: 6570 7469 6f6e 2072 6169 7365 6420 666f  eption raised fo
 00000560: 7220 6572 726f 7273 2069 6e20 7468 6520  r errors in the 
 00000570: 5374 656c 6c61 2041 5049 2e4e 2904 da08  Stella API.N)...
 00000580: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
 00000590: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
 000005a0: 5f5f da07 5f5f 646f 635f 5fa9 0072 0a00  __..__doc__..r..
-000005b0: 0000 720a 0000 00fa 6f2f 5573 6572 732f  ..r.....o/Users/
+000005b0: 0000 720a 0000 00fa 672f 5573 6572 732f  ..r.....g/Users/
 000005c0: 746f 6d2d 6b61 6e64 7a69 6f72 612f 4465  tom-kandziora/De
 000005d0: 764c 6f63 616c 2f73 7465 6c6c 612f 7374  vLocal/stella/st
 000005e0: 656c 6c61 2d6e 6f77 2f53 7465 6c6c 614e  ella-now/StellaN
 000005f0: 6f77 434c 492f 7374 656c 6c61 6e6f 775f  owCLI/stellanow_
-00000600: 636c 692f 6578 6365 7074 696f 6e73 2f53  cli/exceptions/S
-00000610: 7465 6c6c 614e 6f77 4150 4945 7863 6570  tellaNowAPIExcep
-00000620: 7469 6f6e 732e 7079 7205 0000 001c 0000  tions.pyr.......
-00000630: 0073 0400 0000 0800 0801 7205 0000 0063  .s........r....c
-00000640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000650: 0300 0000 0000 0000 f320 0000 0065 005a  ......... ...e.Z
-00000660: 0164 005a 0264 015a 0387 0066 0164 0264  .d.Z.d.Z...f.d.d
-00000670: 0384 085a 0487 0004 005a 0553 0029 04da  ...Z.....Z.S.)..
-00000680: 1753 7465 6c6c 6141 5049 466f 7262 6964  .StellaAPIForbid
-00000690: 6465 6e45 7272 6f72 7a53 4578 6365 7074  denErrorzSExcept
-000006a0: 696f 6e20 7261 6973 6564 2066 6f72 2077  ion raised for w
-000006b0: 6865 6e20 7472 7969 6e67 2074 6f20 6163  hen trying to ac
-000006c0: 6365 7373 2074 6865 2053 7465 6c6c 6120  cess the Stella 
-000006d0: 4150 4920 6672 6f6d 2062 6c61 636b 6c69  API from blackli
-000006e0: 7374 6564 2061 6464 7265 7373 2e63 0100  sted address.c..
-000006f0: 0000 0000 0000 0000 0000 0100 0000 0400  ................
-00000700: 0000 0300 0000 f312 0000 0074 0083 00a0  ...........t....
-00000710: 0164 0169 00a1 0201 0064 0053 0029 024e  .d.i.....d.S.).N
-00000720: da09 466f 7262 6964 6465 6ea9 02da 0573  ..Forbidden....s
-00000730: 7570 6572 da08 5f5f 696e 6974 5f5f a901  uper..__init__..
-00000740: da04 7365 6c66 a901 da09 5f5f 636c 6173  ..self....__clas
-00000750: 735f 5f72 0a00 0000 720b 0000 0072 1200  s__r....r....r..
-00000760: 0000 2300 0000 f302 0000 0012 017a 2053  ..#..........z S
-00000770: 7465 6c6c 6141 5049 466f 7262 6964 6465  tellaAPIForbidde
-00000780: 6e45 7272 6f72 2e5f 5f69 6e69 745f 5fa9  nError.__init__.
-00000790: 0672 0600 0000 7207 0000 0072 0800 0000  .r....r....r....
-000007a0: 7209 0000 0072 1200 0000 da0d 5f5f 636c  r....r......__cl
-000007b0: 6173 7363 656c 6c5f 5f72 0a00 0000 720a  asscell__r....r.
-000007c0: 0000 0072 1500 0000 720b 0000 0072 0d00  ...r....r....r..
-000007d0: 0000 2000 0000 f306 0000 0008 0004 0114  .. .............
-000007e0: 0272 0d00 0000 6300 0000 0000 0000 0000  .r....c.........
-000007f0: 0000 0000 0000 0003 0000 0000 0000 0072  ...............r
-00000800: 0c00 0000 2904 da16 5374 656c 6c61 4150  ....)...StellaAP
-00000810: 494e 6f74 466f 756e 6445 7272 6f72 7a4e  INotFoundErrorzN
-00000820: 4578 6365 7074 696f 6e20 7261 6973 6564  Exception raised
-00000830: 2066 6f72 2077 6865 6e20 6120 7265 7175   for when a requ
-00000840: 6573 7465 6420 6f62 6a65 6374 2064 6f65  ested object doe
-00000850: 7320 6e6f 7420 6578 6973 7420 696e 2074  s not exist in t
-00000860: 6865 2053 7465 6c6c 6120 4150 492e 6302  he Stella API.c.
-00000870: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00000880: 0000 0003 0000 00f3 1200 0000 7400 8300  ............t...
-00000890: a001 6401 7c01 a102 0100 6400 5300 2902  ..d.|.....d.S.).
-000008a0: 4e7a 094e 6f74 2046 6f75 6e64 7210 0000  Nz.Not Foundr...
-000008b0: 00a9 0272 1400 0000 da07 6465 7461 696c  ...r......detail
-000008c0: 7372 1500 0000 720a 0000 0072 0b00 0000  sr....r....r....
-000008d0: 7212 0000 002a 0000 0072 1700 0000 7a1f  r....*...r....z.
-000008e0: 5374 656c 6c61 4150 494e 6f74 466f 756e  StellaAPINotFoun
-000008f0: 6445 7272 6f72 2e5f 5f69 6e69 745f 5f72  dError.__init__r
-00000900: 1800 0000 720a 0000 0072 0a00 0000 7215  ....r....r....r.
-00000910: 0000 0072 0b00 0000 721b 0000 0027 0000  ...r....r....'..
-00000920: 0072 1a00 0000 721b 0000 0063 0000 0000  .r....r....c....
-00000930: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00000940: 0000 0000 720c 0000 0029 04da 1a53 7465  ....r....)...Ste
-00000950: 6c6c 6141 5049 556e 6175 7468 6f72 6973  llaAPIUnauthoris
-00000960: 6564 4572 726f 727a 6b45 7863 6570 7469  edErrorzkExcepti
-00000970: 6f6e 2072 6169 7365 6420 666f 7220 7768  on raised for wh
-00000980: 656e 2072 6571 7565 7374 2069 7320 6e6f  en request is no
-00000990: 7420 6175 7468 6f72 6973 6564 2074 6f20  t authorised to 
-000009a0: 6265 2070 6572 666f 726d 6564 2062 7920  be performed by 
-000009b0: 7265 7175 6573 7469 6e67 2065 6e74 6974  requesting entit
-000009c0: 7920 696e 2074 6865 2053 7465 6c6c 6120  y in the Stella 
-000009d0: 4150 492e 6302 0000 0000 0000 0000 0000  API.c...........
-000009e0: 0002 0000 0004 0000 0003 0000 0072 1c00  .............r..
-000009f0: 0000 2902 4e5a 0c55 6e61 7574 686f 7269  ..).NZ.Unauthori
-00000a00: 7365 6472 1000 0000 721d 0000 0072 1500  sedr....r....r..
-00000a10: 0000 720a 0000 0072 0b00 0000 7212 0000  ..r....r....r...
-00000a20: 0031 0000 0072 1700 0000 7a23 5374 656c  .1...r....z#Stel
-00000a30: 6c61 4150 4955 6e61 7574 686f 7269 7365  laAPIUnauthorise
-00000a40: 6445 7272 6f72 2e5f 5f69 6e69 745f 5f72  dError.__init__r
-00000a50: 1800 0000 720a 0000 0072 0a00 0000 7215  ....r....r....r.
-00000a60: 0000 0072 0b00 0000 721f 0000 002e 0000  ...r....r.......
-00000a70: 0072 1a00 0000 721f 0000 0063 0000 0000  .r....r....c....
-00000a80: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00000a90: 0000 0000 720c 0000 0029 04da 1e53 7465  ....r....)...Ste
-00000aa0: 6c6c 6141 5049 5772 6f6e 6743 7265 6465  llaAPIWrongCrede
-00000ab0: 6e74 6961 6c73 4572 726f 727a 4545 7863  ntialsErrorzEExc
-00000ac0: 6570 7469 6f6e 2072 6169 7365 6420 666f  eption raised fo
-00000ad0: 7220 7772 6f6e 6720 6372 6564 656e 7469  r wrong credenti
-00000ae0: 616c 7320 6475 7269 6e67 2061 7574 6820  als during auth 
-00000af0: 696e 2074 6865 2053 7465 6c6c 6120 4150  in the Stella AP
-00000b00: 492e 6301 0000 0000 0000 0000 0000 0001  I.c.............
-00000b10: 0000 0004 0000 0003 0000 0072 0e00 0000  ...........r....
-00000b20: 2902 4e7a 3755 6e61 7574 686f 7269 7a65  ).Nz7Unauthorize
-00000b30: 643a 2050 726f 7669 6465 6420 7573 6572  d: Provided user
-00000b40: 6e61 6d65 206f 7220 7061 7373 776f 7264  name or password
-00000b50: 2069 7320 696e 7661 6c69 642e 7210 0000   is invalid.r...
-00000b60: 0072 1300 0000 7215 0000 0072 0a00 0000  .r....r....r....
-00000b70: 720b 0000 0072 1200 0000 3800 0000 7217  r....r....8...r.
-00000b80: 0000 007a 2753 7465 6c6c 6141 5049 5772  ...z'StellaAPIWr
-00000b90: 6f6e 6743 7265 6465 6e74 6961 6c73 4572  ongCredentialsEr
-00000ba0: 726f 722e 5f5f 696e 6974 5f5f 7218 0000  ror.__init__r...
-00000bb0: 0072 0a00 0000 720a 0000 0072 1500 0000  .r....r....r....
-00000bc0: 720b 0000 0072 2000 0000 3500 0000 721a  r....r ...5...r.
-00000bd0: 0000 0072 2000 0000 4e29 0972 0900 0000  ...r ...N).r....
-00000be0: da06 7479 7069 6e67 7202 0000 0072 0400  ..typingr....r..
-00000bf0: 0000 7205 0000 0072 0d00 0000 721b 0000  ..r....r....r...
-00000c00: 0072 1f00 0000 7220 0000 0072 0a00 0000  .r....r ...r....
-00000c10: 720a 0000 0072 0a00 0000 720b 0000 00da  r....r....r.....
-00000c20: 083c 6d6f 6475 6c65 3e01 0000 0073 1000  .<module>....s..
-00000c30: 0000 0400 0c16 0c02 1003 1004 1007 1007  ................
-00000c40: 1407                                     ..
+00000600: 636c 692f 6578 6365 7074 696f 6e73 2f61  cli/exceptions/a
+00000610: 7069 5f65 7863 6570 7469 6f6e 732e 7079  pi_exceptions.py
+00000620: 7205 0000 001c 0000 0073 0400 0000 0800  r........s......
+00000630: 0801 7205 0000 0063 0000 0000 0000 0000  ..r....c........
+00000640: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+00000650: f320 0000 0065 005a 0164 005a 0264 015a  . ...e.Z.d.Z.d.Z
+00000660: 0387 0066 0164 0264 0384 085a 0487 0004  ...f.d.d...Z....
+00000670: 005a 0553 0029 04da 1753 7465 6c6c 6141  .Z.S.)...StellaA
+00000680: 5049 466f 7262 6964 6465 6e45 7272 6f72  PIForbiddenError
+00000690: 7a53 4578 6365 7074 696f 6e20 7261 6973  zSException rais
+000006a0: 6564 2066 6f72 2077 6865 6e20 7472 7969  ed for when tryi
+000006b0: 6e67 2074 6f20 6163 6365 7373 2074 6865  ng to access the
+000006c0: 2053 7465 6c6c 6120 4150 4920 6672 6f6d   Stella API from
+000006d0: 2062 6c61 636b 6c69 7374 6564 2061 6464   blacklisted add
+000006e0: 7265 7373 2e63 0100 0000 0000 0000 0000  ress.c..........
+000006f0: 0000 0100 0000 0400 0000 0300 0000 f312  ................
+00000700: 0000 0074 0083 00a0 0164 0169 00a1 0201  ...t.....d.i....
+00000710: 0064 0053 0029 024e da09 466f 7262 6964  .d.S.).N..Forbid
+00000720: 6465 6ea9 02da 0573 7570 6572 da08 5f5f  den....super..__
+00000730: 696e 6974 5f5f a901 da04 7365 6c66 a901  init__....self..
+00000740: da09 5f5f 636c 6173 735f 5f72 0a00 0000  ..__class__r....
+00000750: 720b 0000 0072 1200 0000 2300 0000 f302  r....r....#.....
+00000760: 0000 0012 017a 2053 7465 6c6c 6141 5049  .....z StellaAPI
+00000770: 466f 7262 6964 6465 6e45 7272 6f72 2e5f  ForbiddenError._
+00000780: 5f69 6e69 745f 5fa9 0672 0600 0000 7207  _init__..r....r.
+00000790: 0000 0072 0800 0000 7209 0000 0072 1200  ...r....r....r..
+000007a0: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
+000007b0: 5f72 0a00 0000 720a 0000 0072 1500 0000  _r....r....r....
+000007c0: 720b 0000 0072 0d00 0000 2000 0000 f306  r....r.... .....
+000007d0: 0000 0008 0004 0114 0272 0d00 0000 6300  .........r....c.
+000007e0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+000007f0: 0000 0000 0000 0072 0c00 0000 2904 da16  .......r....)...
+00000800: 5374 656c 6c61 4150 494e 6f74 466f 756e  StellaAPINotFoun
+00000810: 6445 7272 6f72 7a4e 4578 6365 7074 696f  dErrorzNExceptio
+00000820: 6e20 7261 6973 6564 2066 6f72 2077 6865  n raised for whe
+00000830: 6e20 6120 7265 7175 6573 7465 6420 6f62  n a requested ob
+00000840: 6a65 6374 2064 6f65 7320 6e6f 7420 6578  ject does not ex
+00000850: 6973 7420 696e 2074 6865 2053 7465 6c6c  ist in the Stell
+00000860: 6120 4150 492e 6302 0000 0000 0000 0000  a API.c.........
+00000870: 0000 0002 0000 0004 0000 0003 0000 00f3  ................
+00000880: 1200 0000 7400 8300 a001 6401 7c01 a102  ....t.....d.|...
+00000890: 0100 6400 5300 2902 4e7a 094e 6f74 2046  ..d.S.).Nz.Not F
+000008a0: 6f75 6e64 7210 0000 00a9 0272 1400 0000  oundr......r....
+000008b0: da07 6465 7461 696c 7372 1500 0000 720a  ..detailsr....r.
+000008c0: 0000 0072 0b00 0000 7212 0000 002a 0000  ...r....r....*..
+000008d0: 0072 1700 0000 7a1f 5374 656c 6c61 4150  .r....z.StellaAP
+000008e0: 494e 6f74 466f 756e 6445 7272 6f72 2e5f  INotFoundError._
+000008f0: 5f69 6e69 745f 5f72 1800 0000 720a 0000  _init__r....r...
+00000900: 0072 0a00 0000 7215 0000 0072 0b00 0000  .r....r....r....
+00000910: 721b 0000 0027 0000 0072 1a00 0000 721b  r....'...r....r.
+00000920: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000930: 0000 0000 0300 0000 0000 0000 720c 0000  ............r...
+00000940: 0029 04da 1a53 7465 6c6c 6141 5049 556e  .)...StellaAPIUn
+00000950: 6175 7468 6f72 6973 6564 4572 726f 727a  authorisedErrorz
+00000960: 6b45 7863 6570 7469 6f6e 2072 6169 7365  kException raise
+00000970: 6420 666f 7220 7768 656e 2072 6571 7565  d for when reque
+00000980: 7374 2069 7320 6e6f 7420 6175 7468 6f72  st is not author
+00000990: 6973 6564 2074 6f20 6265 2070 6572 666f  ised to be perfo
+000009a0: 726d 6564 2062 7920 7265 7175 6573 7469  rmed by requesti
+000009b0: 6e67 2065 6e74 6974 7920 696e 2074 6865  ng entity in the
+000009c0: 2053 7465 6c6c 6120 4150 492e 6302 0000   Stella API.c...
+000009d0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+000009e0: 0003 0000 0072 1c00 0000 2902 4e5a 0c55  .....r....).NZ.U
+000009f0: 6e61 7574 686f 7269 7365 6472 1000 0000  nauthorisedr....
+00000a00: 721d 0000 0072 1500 0000 720a 0000 0072  r....r....r....r
+00000a10: 0b00 0000 7212 0000 0031 0000 0072 1700  ....r....1...r..
+00000a20: 0000 7a23 5374 656c 6c61 4150 4955 6e61  ..z#StellaAPIUna
+00000a30: 7574 686f 7269 7365 6445 7272 6f72 2e5f  uthorisedError._
+00000a40: 5f69 6e69 745f 5f72 1800 0000 720a 0000  _init__r....r...
+00000a50: 0072 0a00 0000 7215 0000 0072 0b00 0000  .r....r....r....
+00000a60: 721f 0000 002e 0000 0072 1a00 0000 721f  r........r....r.
+00000a70: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000a80: 0000 0000 0300 0000 0000 0000 720c 0000  ............r...
+00000a90: 0029 04da 1e53 7465 6c6c 6141 5049 5772  .)...StellaAPIWr
+00000aa0: 6f6e 6743 7265 6465 6e74 6961 6c73 4572  ongCredentialsEr
+00000ab0: 726f 727a 4545 7863 6570 7469 6f6e 2072  rorzEException r
+00000ac0: 6169 7365 6420 666f 7220 7772 6f6e 6720  aised for wrong 
+00000ad0: 6372 6564 656e 7469 616c 7320 6475 7269  credentials duri
+00000ae0: 6e67 2061 7574 6820 696e 2074 6865 2053  ng auth in the S
+00000af0: 7465 6c6c 6120 4150 492e 6301 0000 0000  tella API.c.....
+00000b00: 0000 0000 0000 0001 0000 0004 0000 0003  ................
+00000b10: 0000 0072 0e00 0000 2902 4e7a 3755 6e61  ...r....).Nz7Una
+00000b20: 7574 686f 7269 7a65 643a 2050 726f 7669  uthorized: Provi
+00000b30: 6465 6420 7573 6572 6e61 6d65 206f 7220  ded username or 
+00000b40: 7061 7373 776f 7264 2069 7320 696e 7661  password is inva
+00000b50: 6c69 642e 7210 0000 0072 1300 0000 7215  lid.r....r....r.
+00000b60: 0000 0072 0a00 0000 720b 0000 0072 1200  ...r....r....r..
+00000b70: 0000 3800 0000 7217 0000 007a 2753 7465  ..8...r....z'Ste
+00000b80: 6c6c 6141 5049 5772 6f6e 6743 7265 6465  llaAPIWrongCrede
+00000b90: 6e74 6961 6c73 4572 726f 722e 5f5f 696e  ntialsError.__in
+00000ba0: 6974 5f5f 7218 0000 0072 0a00 0000 720a  it__r....r....r.
+00000bb0: 0000 0072 1500 0000 720b 0000 0072 2000  ...r....r....r .
+00000bc0: 0000 3500 0000 721a 0000 0072 2000 0000  ..5...r....r ...
+00000bd0: 4e29 0a72 0900 0000 da06 7479 7069 6e67  N).r......typing
+00000be0: 7202 0000 005a 0e63 6c69 5f65 7863 6570  r....Z.cli_excep
+00000bf0: 7469 6f6e 7372 0400 0000 7205 0000 0072  tionsr....r....r
+00000c00: 0d00 0000 721b 0000 0072 1f00 0000 7220  ....r....r....r 
+00000c10: 0000 0072 0a00 0000 720a 0000 0072 0a00  ...r....r....r..
+00000c20: 0000 720b 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000c30: 3e01 0000 0073 1000 0000 0400 0c16 0c02  >....s..........
+00000c40: 1003 1004 1007 1007 1407                 ..........
```

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/__pycache__/StellaNowCLIException.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/__pycache__/cli_exceptions.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 20 14:47:41 2023 UTC, .py size: 2163 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -87,113 +87,113 @@
 00000560: 0300 0000 731e 0000 007c 017c 005f 007c  ....s....|.|._.|
 00000570: 027c 005f 0174 0283 00a0 037c 006a 00a1  .|._.t.....|.j..
 00000580: 0101 0064 0053 0029 014e 2904 da07 6d65  ...d.S.).N)...me
 00000590: 7373 6167 65da 0764 6574 6169 6c73 da05  ssage..details..
 000005a0: 7375 7065 72da 085f 5f69 6e69 745f 5f29  super..__init__)
 000005b0: 03da 0473 656c 6672 0200 0000 7203 0000  ...selfr....r...
 000005c0: 00a9 01da 095f 5f63 6c61 7373 5f5f a900  .....__class__..
-000005d0: fa6e 2f55 7365 7273 2f74 6f6d 2d6b 616e  .n/Users/tom-kan
+000005d0: fa67 2f55 7365 7273 2f74 6f6d 2d6b 616e  .g/Users/tom-kan
 000005e0: 647a 696f 7261 2f44 6576 4c6f 6361 6c2f  dziora/DevLocal/
 000005f0: 7374 656c 6c61 2f73 7465 6c6c 612d 6e6f  stella/stella-no
 00000600: 772f 5374 656c 6c61 4e6f 7743 4c49 2f73  w/StellaNowCLI/s
 00000610: 7465 6c6c 616e 6f77 5f63 6c69 2f65 7863  tellanow_cli/exc
-00000620: 6570 7469 6f6e 732f 5374 656c 6c61 4e6f  eptions/StellaNo
-00000630: 7743 4c49 4578 6365 7074 696f 6e2e 7079  wCLIException.py
-00000640: 7205 0000 001b 0000 0073 0600 0000 0601  r........s......
-00000650: 0601 1201 7a1e 5374 656c 6c61 4e6f 7743  ....z.StellaNowC
-00000660: 4c49 4578 6365 7074 696f 6e2e 5f5f 696e  LIException.__in
-00000670: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
-00000680: 0001 0000 0003 0000 0043 0000 0073 1200  .........C...s..
-00000690: 0000 7c00 6a00 9b00 6401 7c00 6a01 9b00  ..|.j...d.|.j...
-000006a0: 9d03 5300 2902 4eda 0120 2902 7202 0000  ..S.).N.. ).r...
-000006b0: 0072 0300 0000 a901 7206 0000 0072 0900  .r......r....r..
-000006c0: 0000 7209 0000 0072 0a00 0000 da07 5f5f  ..r....r......__
-000006d0: 7374 725f 5f20 0000 00f3 0200 0000 1201  str__ ..........
-000006e0: 7a1d 5374 656c 6c61 4e6f 7743 4c49 4578  z.StellaNowCLIEx
-000006f0: 6365 7074 696f 6e2e 5f5f 7374 725f 5f29  ception.__str__)
-00000700: 07da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00000710: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00000720: 616d 655f 5fda 075f 5f64 6f63 5f5f 7205  ame__..__doc__r.
-00000730: 0000 0072 0d00 0000 da0d 5f5f 636c 6173  ...r......__clas
-00000740: 7363 656c 6c5f 5f72 0900 0000 7209 0000  scell__r....r...
-00000750: 0072 0700 0000 720a 0000 0072 0100 0000  .r....r....r....
-00000760: 1800 0000 7308 0000 0008 0004 010c 0210  ....s...........
-00000770: 0572 0100 0000 6300 0000 0000 0000 0000  .r....c.........
-00000780: 0000 0000 0000 0003 0000 0000 0000 00f3  ................
-00000790: 2000 0000 6500 5a01 6400 5a02 6401 5a03   ...e.Z.d.Z.d.Z.
-000007a0: 8700 6601 6402 6403 8408 5a04 8700 0400  ..f.d.d...Z.....
-000007b0: 5a05 5300 2904 da29 5374 656c 6c61 4e6f  Z.S.)..)StellaNo
-000007c0: 7743 4c49 4c61 6e67 7561 6765 4e6f 7453  wCLILanguageNotS
-000007d0: 7570 706f 7274 6564 4578 6365 7074 696f  upportedExceptio
-000007e0: 6e7a 3645 7863 6570 7469 6f6e 2072 6169  nz6Exception rai
-000007f0: 7365 6420 666f 7220 756e 7375 7070 6f72  sed for unsuppor
-00000800: 7465 6420 6c61 6e67 7561 6765 7320 6279  ted languages by
-00000810: 2074 6865 2043 4c49 2e63 0200 0000 0000   the CLI.c......
-00000820: 0000 0000 0000 0200 0000 0500 0000 0300  ................
-00000830: 0000 731a 0000 0074 0083 00a0 0164 017c  ..s....t.....d.|
-00000840: 019b 0064 029d 0369 00a1 0201 0064 0053  ...d...i.....d.S
-00000850: 0029 034e 7a13 436f 6465 2067 656e 6572  .).Nz.Code gener
-00000860: 6174 6f72 2066 6f72 207a 0b20 6e6f 7420  ator for z. not 
-00000870: 666f 756e 642e a902 7204 0000 0072 0500  found...r....r..
-00000880: 0000 2902 7206 0000 00da 086c 616e 6775  ..).r......langu
-00000890: 6167 6572 0700 0000 7209 0000 0072 0a00  ager....r....r..
-000008a0: 0000 7205 0000 0027 0000 0073 0200 0000  ..r....'...s....
-000008b0: 1a01 7a32 5374 656c 6c61 4e6f 7743 4c49  ..z2StellaNowCLI
-000008c0: 4c61 6e67 7561 6765 4e6f 7453 7570 706f  LanguageNotSuppo
-000008d0: 7274 6564 4578 6365 7074 696f 6e2e 5f5f  rtedException.__
-000008e0: 696e 6974 5f5f a906 720f 0000 0072 1000  init__..r....r..
-000008f0: 0000 7211 0000 0072 1200 0000 7205 0000  ..r....r....r...
-00000900: 0072 1300 0000 7209 0000 0072 0900 0000  .r....r....r....
-00000910: 7207 0000 0072 0a00 0000 7215 0000 0024  r....r....r....$
-00000920: 0000 00f3 0600 0000 0800 0401 1402 7215  ..............r.
-00000930: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000940: 0000 0000 0300 0000 0000 0000 7214 0000  ............r...
-00000950: 0029 04da 2653 7465 6c6c 614e 6f77 434c  .)..&StellaNowCL
-00000960: 494e 616d 6573 7061 6365 4e6f 7446 6f75  INamespaceNotFou
-00000970: 6e64 4578 6365 7074 696f 6e7a 3945 7863  ndExceptionz9Exc
-00000980: 6570 7469 6f6e 2072 6169 7365 6420 7768  eption raised wh
-00000990: 656e 2061 206e 616d 6573 7061 6365 2069  en a namespace i
-000009a0: 7320 6e6f 7420 666f 756e 6420 696e 2061  s not found in a
-000009b0: 2066 696c 652e 6301 0000 0000 0000 0000   file.c.........
-000009c0: 0000 0001 0000 0004 0000 0003 0000 00f3  ................
-000009d0: 1200 0000 7400 8300 a001 6401 6900 a102  ....t.....d.i...
-000009e0: 0100 6400 5300 2902 4e7a 124e 6f20 4e61  ..d.S.).Nz.No Na
-000009f0: 6d65 7370 6163 6520 466f 756e 6472 1600  mespace Foundr..
-00000a00: 0000 720c 0000 0072 0700 0000 7209 0000  ..r....r....r...
-00000a10: 0072 0a00 0000 7205 0000 002e 0000 0072  .r....r........r
-00000a20: 0e00 0000 7a2f 5374 656c 6c61 4e6f 7743  ....z/StellaNowC
-00000a30: 4c49 4e61 6d65 7370 6163 654e 6f74 466f  LINamespaceNotFo
-00000a40: 756e 6445 7863 6570 7469 6f6e 2e5f 5f69  undException.__i
-00000a50: 6e69 745f 5f72 1800 0000 7209 0000 0072  nit__r....r....r
-00000a60: 0900 0000 7207 0000 0072 0a00 0000 721a  ....r....r....r.
-00000a70: 0000 002b 0000 0072 1900 0000 721a 0000  ...+...r....r...
-00000a80: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000a90: 0000 0300 0000 0000 0000 7214 0000 0029  ..........r....)
-00000aa0: 04da 3053 7465 6c6c 614e 6f77 434c 494e  ..0StellaNowCLIN
-00000ab0: 6f45 6e74 6974 7941 7373 6f63 6961 7465  oEntityAssociate
-00000ac0: 6457 6974 6845 7665 6e74 4578 6365 7074  dWithEventExcept
-00000ad0: 696f 6e7a 6c45 7863 6570 7469 6f6e 2072  ionzlException r
-00000ae0: 6169 7365 6420 7768 656e 2061 6e20 6576  aised when an ev
-00000af0: 656e 7420 646f 6573 206e 6f74 2068 6176  ent does not hav
-00000b00: 6520 616e 7920 6173 736f 6369 6174 6564  e any associated
-00000b10: 2065 6e74 6974 6965 732e 2049 7420 6973   entities. It is
-00000b20: 206e 6f74 2061 2076 616c 6964 2065 7665   not a valid eve
-00000b30: 6e74 2066 6f72 2069 6e67 6573 7469 6f6e  nt for ingestion
-00000b40: 2e63 0100 0000 0000 0000 0000 0000 0100  .c..............
-00000b50: 0000 0400 0000 0300 0000 721b 0000 0029  ..........r....)
-00000b60: 024e 7a1f 4e6f 2045 6e74 6974 7920 4173  .Nz.No Entity As
-00000b70: 736f 6369 6174 6564 2057 6974 6820 4576  sociated With Ev
-00000b80: 656e 7472 1600 0000 720c 0000 0072 0700  entr....r....r..
-00000b90: 0000 7209 0000 0072 0a00 0000 7205 0000  ..r....r....r...
-00000ba0: 0035 0000 0072 0e00 0000 7a39 5374 656c  .5...r....z9Stel
-00000bb0: 6c61 4e6f 7743 4c49 4e6f 456e 7469 7479  laNowCLINoEntity
-00000bc0: 4173 736f 6369 6174 6564 5769 7468 4576  AssociatedWithEv
-00000bd0: 656e 7445 7863 6570 7469 6f6e 2e5f 5f69  entException.__i
-00000be0: 6e69 745f 5f72 1800 0000 7209 0000 0072  nit__r....r....r
-00000bf0: 0900 0000 7207 0000 0072 0a00 0000 721c  ....r....r....r.
-00000c00: 0000 0032 0000 0072 1900 0000 721c 0000  ...2...r....r...
-00000c10: 004e 2906 7212 0000 00da 0945 7863 6570  .N).r......Excep
-00000c20: 7469 6f6e 7201 0000 0072 1500 0000 721a  tionr....r....r.
-00000c30: 0000 0072 1c00 0000 7209 0000 0072 0900  ...r....r....r..
-00000c40: 0000 7209 0000 0072 0a00 0000 da08 3c6d  ..r....r......<m
-00000c50: 6f64 756c 653e 0100 0000 730a 0000 0004  odule>....s.....
-00000c60: 0010 1710 0c10 0714 07                   .........
+00000620: 6570 7469 6f6e 732f 636c 695f 6578 6365  eptions/cli_exce
+00000630: 7074 696f 6e73 2e70 7972 0500 0000 1b00  ptions.pyr......
+00000640: 0000 7306 0000 0006 0106 0112 017a 1e53  ..s..........z.S
+00000650: 7465 6c6c 614e 6f77 434c 4945 7863 6570  tellaNowCLIExcep
+00000660: 7469 6f6e 2e5f 5f69 6e69 745f 5f63 0100  tion.__init__c..
+00000670: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00000680: 0000 4300 0000 7312 0000 007c 006a 009b  ..C...s....|.j..
+00000690: 0064 017c 006a 019b 009d 0353 0029 024e  .d.|.j.....S.).N
+000006a0: da01 2029 0272 0200 0000 7203 0000 00a9  .. ).r....r.....
+000006b0: 0172 0600 0000 7209 0000 0072 0900 0000  .r....r....r....
+000006c0: 720a 0000 00da 075f 5f73 7472 5f5f 2000  r......__str__ .
+000006d0: 0000 f302 0000 0012 017a 1d53 7465 6c6c  .........z.Stell
+000006e0: 614e 6f77 434c 4945 7863 6570 7469 6f6e  aNowCLIException
+000006f0: 2e5f 5f73 7472 5f5f 2907 da08 5f5f 6e61  .__str__)...__na
+00000700: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000710: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
+00000720: 5f5f 646f 635f 5f72 0500 0000 720d 0000  __doc__r....r...
+00000730: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
+00000740: 7209 0000 0072 0900 0000 7207 0000 0072  r....r....r....r
+00000750: 0a00 0000 7201 0000 0018 0000 0073 0800  ....r........s..
+00000760: 0000 0800 0401 0c02 1005 7201 0000 0063  ..........r....c
+00000770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000780: 0300 0000 0000 0000 f320 0000 0065 005a  ......... ...e.Z
+00000790: 0164 005a 0264 015a 0387 0066 0164 0264  .d.Z.d.Z...f.d.d
+000007a0: 0384 085a 0487 0004 005a 0553 0029 04da  ...Z.....Z.S.)..
+000007b0: 2953 7465 6c6c 614e 6f77 434c 494c 616e  )StellaNowCLILan
+000007c0: 6775 6167 654e 6f74 5375 7070 6f72 7465  guageNotSupporte
+000007d0: 6445 7863 6570 7469 6f6e 7a36 4578 6365  dExceptionz6Exce
+000007e0: 7074 696f 6e20 7261 6973 6564 2066 6f72  ption raised for
+000007f0: 2075 6e73 7570 706f 7274 6564 206c 616e   unsupported lan
+00000800: 6775 6167 6573 2062 7920 7468 6520 434c  guages by the CL
+00000810: 492e 6302 0000 0000 0000 0000 0000 0002  I.c.............
+00000820: 0000 0005 0000 0003 0000 0073 1a00 0000  ...........s....
+00000830: 7400 8300 a001 6401 7c01 9b00 6402 9d03  t.....d.|...d...
+00000840: 6900 a102 0100 6400 5300 2903 4e7a 1343  i.....d.S.).Nz.C
+00000850: 6f64 6520 6765 6e65 7261 746f 7220 666f  ode generator fo
+00000860: 7220 7a0b 206e 6f74 2066 6f75 6e64 2ea9  r z. not found..
+00000870: 0272 0400 0000 7205 0000 0029 0272 0600  .r....r....).r..
+00000880: 0000 da08 6c61 6e67 7561 6765 7207 0000  ....languager...
+00000890: 0072 0900 0000 720a 0000 0072 0500 0000  .r....r....r....
+000008a0: 2700 0000 7302 0000 001a 017a 3253 7465  '...s......z2Ste
+000008b0: 6c6c 614e 6f77 434c 494c 616e 6775 6167  llaNowCLILanguag
+000008c0: 654e 6f74 5375 7070 6f72 7465 6445 7863  eNotSupportedExc
+000008d0: 6570 7469 6f6e 2e5f 5f69 6e69 745f 5fa9  eption.__init__.
+000008e0: 0672 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
+000008f0: 7212 0000 0072 0500 0000 7213 0000 0072  r....r....r....r
+00000900: 0900 0000 7209 0000 0072 0700 0000 720a  ....r....r....r.
+00000910: 0000 0072 1500 0000 2400 0000 f306 0000  ...r....$.......
+00000920: 0008 0004 0114 0272 1500 0000 6300 0000  .......r....c...
+00000930: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00000940: 0000 0000 0072 1400 0000 2904 da26 5374  .....r....)..&St
+00000950: 656c 6c61 4e6f 7743 4c49 4e61 6d65 7370  ellaNowCLINamesp
+00000960: 6163 654e 6f74 466f 756e 6445 7863 6570  aceNotFoundExcep
+00000970: 7469 6f6e 7a39 4578 6365 7074 696f 6e20  tionz9Exception 
+00000980: 7261 6973 6564 2077 6865 6e20 6120 6e61  raised when a na
+00000990: 6d65 7370 6163 6520 6973 206e 6f74 2066  mespace is not f
+000009a0: 6f75 6e64 2069 6e20 6120 6669 6c65 2e63  ound in a file.c
+000009b0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000009c0: 0400 0000 0300 0000 f312 0000 0074 0083  .............t..
+000009d0: 00a0 0164 0169 00a1 0201 0064 0053 0029  ...d.i.....d.S.)
+000009e0: 024e 7a12 4e6f 204e 616d 6573 7061 6365  .Nz.No Namespace
+000009f0: 2046 6f75 6e64 7216 0000 0072 0c00 0000   Foundr....r....
+00000a00: 7207 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+00000a10: 0500 0000 2e00 0000 720e 0000 007a 2f53  ........r....z/S
+00000a20: 7465 6c6c 614e 6f77 434c 494e 616d 6573  tellaNowCLINames
+00000a30: 7061 6365 4e6f 7446 6f75 6e64 4578 6365  paceNotFoundExce
+00000a40: 7074 696f 6e2e 5f5f 696e 6974 5f5f 7218  ption.__init__r.
+00000a50: 0000 0072 0900 0000 7209 0000 0072 0700  ...r....r....r..
+00000a60: 0000 720a 0000 0072 1a00 0000 2b00 0000  ..r....r....+...
+00000a70: 7219 0000 0072 1a00 0000 6300 0000 0000  r....r....c.....
+00000a80: 0000 0000 0000 0000 0000 0003 0000 0000  ................
+00000a90: 0000 0072 1400 0000 2904 da30 5374 656c  ...r....)..0Stel
+00000aa0: 6c61 4e6f 7743 4c49 4e6f 456e 7469 7479  laNowCLINoEntity
+00000ab0: 4173 736f 6369 6174 6564 5769 7468 4576  AssociatedWithEv
+00000ac0: 656e 7445 7863 6570 7469 6f6e 7a6c 4578  entExceptionzlEx
+00000ad0: 6365 7074 696f 6e20 7261 6973 6564 2077  ception raised w
+00000ae0: 6865 6e20 616e 2065 7665 6e74 2064 6f65  hen an event doe
+00000af0: 7320 6e6f 7420 6861 7665 2061 6e79 2061  s not have any a
+00000b00: 7373 6f63 6961 7465 6420 656e 7469 7469  ssociated entiti
+00000b10: 6573 2e20 4974 2069 7320 6e6f 7420 6120  es. It is not a 
+00000b20: 7661 6c69 6420 6576 656e 7420 666f 7220  valid event for 
+00000b30: 696e 6765 7374 696f 6e2e 6301 0000 0000  ingestion.c.....
+00000b40: 0000 0000 0000 0001 0000 0004 0000 0003  ................
+00000b50: 0000 0072 1b00 0000 2902 4e7a 1f4e 6f20  ...r....).Nz.No 
+00000b60: 456e 7469 7479 2041 7373 6f63 6961 7465  Entity Associate
+00000b70: 6420 5769 7468 2045 7665 6e74 7216 0000  d With Eventr...
+00000b80: 0072 0c00 0000 7207 0000 0072 0900 0000  .r....r....r....
+00000b90: 720a 0000 0072 0500 0000 3500 0000 720e  r....r....5...r.
+00000ba0: 0000 007a 3953 7465 6c6c 614e 6f77 434c  ...z9StellaNowCL
+00000bb0: 494e 6f45 6e74 6974 7941 7373 6f63 6961  INoEntityAssocia
+00000bc0: 7465 6457 6974 6845 7665 6e74 4578 6365  tedWithEventExce
+00000bd0: 7074 696f 6e2e 5f5f 696e 6974 5f5f 7218  ption.__init__r.
+00000be0: 0000 0072 0900 0000 7209 0000 0072 0700  ...r....r....r..
+00000bf0: 0000 720a 0000 0072 1c00 0000 3200 0000  ..r....r....2...
+00000c00: 7219 0000 0072 1c00 0000 4e29 0672 1200  r....r....N).r..
+00000c10: 0000 da09 4578 6365 7074 696f 6e72 0100  ....Exceptionr..
+00000c20: 0000 7215 0000 0072 1a00 0000 721c 0000  ..r....r....r...
+00000c30: 0072 0900 0000 7209 0000 0072 0900 0000  .r....r....r....
+00000c40: 720a 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000c50: 0000 0073 0a00 0000 0400 1017 100c 1007  ...s............
+00000c60: 1407                                     ..
```

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/exceptions/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/utils/__init__.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/utils/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/utils/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/utils/__pycache__/logger.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/utils/__pycache__/logger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/utils/__pycache__/utils.cpython-310.pyc` & `stellanow_cli-0.0.9rc3/stellanow_cli/utils/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/utils/logger.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/utils/logger.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli/utils/utils.py` & `stellanow_cli-0.0.9rc3/stellanow_cli/utils/utils.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli.egg-info/PKG-INFO` & `stellanow_cli-0.0.9rc3/stellanow_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stellanow-cli
-Version: 0.0.9rc2
+Version: 0.0.9rc3
 Summary: Command-line interface for the StellaNow SDK code generation and comparison tool.
 Requires-Python: >=3.10
 
 StellaNow CLI Tool
 ==================
 
 Welcome to the StellaNow CLI tool. This tool automates the process of generating class code from StellaNow event specifications and provides a summary of changes between the generated classes and the specifications fetched from the API. It's recommended to use this tool in conjunction with the StellaNow SDK's to ensure that your application's message classes are up-to-date with the latest specifications.
```

### Comparing `stellanow_cli-0.0.9rc2/stellanow_cli.egg-info/SOURCES.txt` & `stellanow_cli-0.0.9rc3/stellanow_cli.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -47,20 +47,20 @@
 stellanow_cli/config/config.py
 stellanow_cli/config/dev.py
 stellanow_cli/config/int.py
 stellanow_cli/config/__pycache__/__init__.cpython-310.pyc
 stellanow_cli/config/__pycache__/config.cpython-310.pyc
 stellanow_cli/config/__pycache__/dev.cpython-310.pyc
 stellanow_cli/config/__pycache__/int.cpython-310.pyc
-stellanow_cli/exceptions/StellaNowAPIExceptions.py
-stellanow_cli/exceptions/StellaNowCLIException.py
 stellanow_cli/exceptions/__init__.py
-stellanow_cli/exceptions/__pycache__/StellaNowAPIExceptions.cpython-310.pyc
-stellanow_cli/exceptions/__pycache__/StellaNowCLIException.cpython-310.pyc
+stellanow_cli/exceptions/api_exceptions.py
+stellanow_cli/exceptions/cli_exceptions.py
 stellanow_cli/exceptions/__pycache__/__init__.cpython-310.pyc
+stellanow_cli/exceptions/__pycache__/api_exceptions.cpython-310.pyc
+stellanow_cli/exceptions/__pycache__/cli_exceptions.cpython-310.pyc
 stellanow_cli/utils/__init__.py
 stellanow_cli/utils/logger.py
 stellanow_cli/utils/utils.py
 stellanow_cli/utils/__pycache__/__init__.cpython-310.pyc
 stellanow_cli/utils/__pycache__/logger.cpython-310.pyc
 stellanow_cli/utils/__pycache__/utils.cpython-310.pyc
 tests/test_command_configure.py
```

### Comparing `stellanow_cli-0.0.9rc2/tests/test_command_configure.py` & `stellanow_cli-0.0.9rc3/tests/test_command_configure.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc2/tests/test_generate_class_handles_all_valueTypes.py` & `stellanow_cli-0.0.9rc3/tests/test_generate_class_handles_all_valueTypes.py`

 * *Files identical despite different names*

