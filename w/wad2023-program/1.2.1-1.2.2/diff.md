# Comparing `tmp/wad2023-program-1.2.1.tar.gz` & `tmp/wad2023-program-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wad2023-program-1.2.1.tar", last modified: Thu Jun 29 19:35:02 2023, max compression
+gzip compressed data, was "wad2023-program-1.2.2.tar", last modified: Fri Jun 30 08:18:31 2023, max compression
```

## Comparing `wad2023-program-1.2.1.tar` & `wad2023-program-1.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:35:02.985097 wad2023-program-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-29 19:34:52.000000 wad2023-program-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-29 19:35:02.985097 wad2023-program-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-29 19:34:52.000000 wad2023-program-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-29 19:34:52.000000 wad2023-program-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 19:35:02.985097 wad2023-program-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:35:02.981096 wad2023-program-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:35:02.981096 wad2023-program-1.2.1/src/wad2023_program/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-29 19:34:52.000000 wad2023-program-1.2.1/src/wad2023_program/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-06-29 19:34:52.000000 wad2023-program-1.2.1/src/wad2023_program/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-29 19:34:52.000000 wad2023-program-1.2.1/src/wad2023_program/app_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-29 19:34:52.000000 wad2023-program-1.2.1/src/wad2023_program/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-29 19:34:52.000000 wad2023-program-1.2.1/src/wad2023_program/program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:35:02.985097 wad2023-program-1.2.1/src/wad2023_program.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-29 19:35:02.000000 wad2023-program-1.2.1/src/wad2023_program.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-29 19:35:02.000000 wad2023-program-1.2.1/src/wad2023_program.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:35:02.000000 wad2023-program-1.2.1/src/wad2023_program.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-29 19:35:02.000000 wad2023-program-1.2.1/src/wad2023_program.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-29 19:35:02.000000 wad2023-program-1.2.1/src/wad2023_program.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 19:35:02.000000 wad2023-program-1.2.1/src/wad2023_program.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:18:31.717188 wad2023-program-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-30 08:18:21.000000 wad2023-program-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-30 08:18:31.717188 wad2023-program-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-30 08:18:21.000000 wad2023-program-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-30 08:18:21.000000 wad2023-program-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 08:18:31.717188 wad2023-program-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:18:31.713189 wad2023-program-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:18:31.717188 wad2023-program-1.2.2/src/wad2023_program/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-30 08:18:21.000000 wad2023-program-1.2.2/src/wad2023_program/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-06-30 08:18:21.000000 wad2023-program-1.2.2/src/wad2023_program/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-30 08:18:21.000000 wad2023-program-1.2.2/src/wad2023_program/app_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-30 08:18:21.000000 wad2023-program-1.2.2/src/wad2023_program/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-30 08:18:21.000000 wad2023-program-1.2.2/src/wad2023_program/program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:18:31.717188 wad2023-program-1.2.2/src/wad2023_program.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-30 08:18:31.000000 wad2023-program-1.2.2/src/wad2023_program.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-30 08:18:31.000000 wad2023-program-1.2.2/src/wad2023_program.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 08:18:31.000000 wad2023-program-1.2.2/src/wad2023_program.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-30 08:18:31.000000 wad2023-program-1.2.2/src/wad2023_program.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-30 08:18:31.000000 wad2023-program-1.2.2/src/wad2023_program.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 08:18:31.000000 wad2023-program-1.2.2/src/wad2023_program.egg-info/top_level.txt
```

### Comparing `wad2023-program-1.2.1/LICENSE` & `wad2023-program-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.2.1/PKG-INFO` & `wad2023-program-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wad2023-program
-Version: 1.2.1
+Version: 1.2.2
 Summary: Script to retrieve the program for WeAreDevelopers 2023 conference
 Author-email: Daryl Stark <daryl@dstark.nl>
 License: MIT License
         
         Copyright (c) 2023 Daryl Stark
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `wad2023-program-1.2.1/README.md` & `wad2023-program-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.2.1/pyproject.toml` & `wad2023-program-1.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.1.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "wad2023-program"
-version = "1.2.1"
+version = "1.2.2"
 description = "Script to retrieve the program for WeAreDevelopers 2023 conference"
 readme = "README.md"
 authors = [{ name = "Daryl Stark", email = "daryl@dstark.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -40,15 +40,15 @@
 homepage = "https://github.com/DarylStark/WeAreDevelopers_2023_Program"
 repository = "https://github.com/DarylStark/WeAreDevelopers_2023_Program"
 
 [project.scripts]
 wad23 = "wad2023_program.__main__:main"
 
 [tool.bumpver]
-current_version = "1.2.1"
+current_version = "1.2.2"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "Version {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `wad2023-program-1.2.1/src/wad2023_program/__main__.py` & `wad2023-program-1.2.2/src/wad2023_program/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,27 +62,29 @@
 
 
 def start(
         sort: SortField = SortField.START_TIME,
         in_title: str = '',
         in_speaker: str = '',
         in_description: str = '',
+        find: str = '',
         stage: str = '',
         output: DataOutput = DataOutput.TABLE,
         cache: bool = True
 ) -> None:
     """Script function for the program.
 
     The function that gets called when starting the script.
 
     Args:
         sort: the field on what to sort.
         in_title: filter on words in the title.
         in_speaker: filter on words in the speakers.
         in_description: filter on words in the description.
+        find: filter on words in the description _or_ in the title.
         stage: specify a specific stage.
         output: specifies what kind of output the user wants.
         cache: specifies if the cache has to be used.
     """
     # Get the program
     program = get_program(cache=cache)
 
@@ -97,14 +99,19 @@
                               in session.title.lower(), program))
     if len(in_speaker) > 0:
         program = list(filter(lambda session: in_speaker.lower()
                               in session.speaker.lower(), program))
     if len(in_description) > 0:
         program = list(filter(lambda session: in_description.lower()
                               in session.description.lower(), program))
+    if len(find) > 0:
+        program = list(filter(lambda session:
+                              find in session.description.lower() or
+                              find in session.title.lower(),
+                              program))
     if len(stage) > 0:
         program = list(filter(lambda session:
                               session.stage_name.lower() == stage.lower(),
                               program))
 
     # Create a Rich console for a beautiful display
     console = Console()
@@ -130,24 +137,25 @@
                 item.speaker
             )
 
         # Show the nice table
         console.print(table)
 
     if output == DataOutput.CSV:
-        console.print(
+        print(
             '"Date";"Start";"End";"Stage";"Title";"Description";"Speakers"')
         for item in program:
-            console.print(
+            description = item.description.replace('"', '\\"')
+            print(
                 f'"{item.start_time_berlin:%Y-%m-%d}";' +
                 f'"{item.start_time_berlin:%H:%M:%S}";' +
                 f'"{item.end_time_berlin:%H:%M:%S}";' +
                 f'"{item.stage_name}";' +
                 f'"{item.title}";' +
-                f'"{item.description}";' +
+                f'"{description}";' +
                 f'"{item.speaker}"')
 
     if output == DataOutput.DETAILS:
         for item in program:
             table = Table(box=box.MINIMAL, show_header=False)
             table.add_column('Field')
             table.add_column('Information')
```

### Comparing `wad2023-program-1.2.1/src/wad2023_program/app_config.py` & `wad2023-program-1.2.2/src/wad2023_program/app_config.py`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.2.1/src/wad2023_program/model.py` & `wad2023-program-1.2.2/src/wad2023_program/model.py`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.2.1/src/wad2023_program/program.py` & `wad2023-program-1.2.2/src/wad2023_program/program.py`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.2.1/src/wad2023_program.egg-info/PKG-INFO` & `wad2023-program-1.2.2/src/wad2023_program.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wad2023-program
-Version: 1.2.1
+Version: 1.2.2
 Summary: Script to retrieve the program for WeAreDevelopers 2023 conference
 Author-email: Daryl Stark <daryl@dstark.nl>
 License: MIT License
         
         Copyright (c) 2023 Daryl Stark
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

