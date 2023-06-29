# Comparing `tmp/c_custom_code_checker-1.0.3.tar.gz` & `tmp/c_custom_code_checker-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c_custom_code_checker-1.0.3.tar", last modified: Mon Jun 26 22:33:35 2023, max compression
+gzip compressed data, was "c_custom_code_checker-1.0.4.tar", last modified: Thu Jun 29 22:05:44 2023, max compression
```

## Comparing `c_custom_code_checker-1.0.3.tar` & `c_custom_code_checker-1.0.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 22:33:35.904306 c_custom_code_checker-1.0.3/
--rw-rw-rw-   0        0        0     5096 2023-06-26 22:33:35.903305 c_custom_code_checker-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4577 2023-06-25 20:41:57.000000 c_custom_code_checker-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 22:33:35.837355 c_custom_code_checker-1.0.3/c_custom_code_checker/
--rw-rw-rw-   0        0        0       22 2023-06-24 13:04:57.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 22:33:35.858338 c_custom_code_checker-1.0.3/c_custom_code_checker/constants/
--rw-rw-rw-   0        0        0      169 2023-06-24 11:35:28.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/constants/__init__.py
--rw-rw-rw-   0        0        0      164 2023-06-18 11:56:47.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/constants/criterion_keys.py
--rw-rw-rw-   0        0        0      800 2023-06-26 22:04:39.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/constants/rules_reserved_keys.py
--rw-rw-rw-   0        0        0      388 2023-06-25 16:52:24.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/constants/strings.py
--rw-rw-rw-   0        0        0      345 2023-06-23 22:02:21.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/constants/target_keys.py
-drwxrwxrwx   0        0        0        0 2023-06-26 22:33:35.866311 c_custom_code_checker-1.0.3/c_custom_code_checker/enums/
--rw-rw-rw-   0        0        0       78 2023-06-24 12:38:52.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/enums/__init__.py
--rw-rw-rw-   0        0        0     1587 2023-06-25 16:36:40.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/enums/criterion_enum.py
--rw-rw-rw-   0        0        0     1949 2023-06-26 22:09:23.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/enums/target_enum.py
-drwxrwxrwx   0        0        0        0 2023-06-26 22:33:35.883319 c_custom_code_checker-1.0.3/c_custom_code_checker/exceptions/
--rw-rw-rw-   0        0        0      442 2023-06-24 11:30:38.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/exceptions/__init__.py
--rw-rw-rw-   0        0        0      193 2023-06-19 23:09:18.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/exceptions/criterion_not_respected_exception.py
--rw-rw-rw-   0        0        0      184 2023-06-18 11:43:14.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/exceptions/criterion_value_missing_exception.py
--rw-rw-rw-   0        0        0      176 2023-06-15 23:54:12.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/exceptions/invalid_criterion_exception.py
--rw-rw-rw-   0        0        0      170 2023-06-15 23:46:33.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/exceptions/invalid_target_exception.py
--rw-rw-rw-   0        0        0      173 2023-06-21 00:25:53.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/exceptions/lib_clang_not_found_exception.py
--rw-rw-rw-   0        0        0      177 2023-06-15 23:33:03.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/exceptions/rule_missing_criterion_exception.py
--rw-rw-rw-   0        0        0      173 2023-06-15 23:30:38.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/exceptions/rule_missing_target_exception.py
-drwxrwxrwx   0        0        0        0 2023-06-26 22:33:35.887305 c_custom_code_checker-1.0.3/c_custom_code_checker/handlers/
--rw-rw-rw-   0        0        0      181 2023-06-24 12:42:42.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/handlers/__init__.py
--rw-rw-rw-   0        0        0     2081 2023-06-25 16:36:40.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/handlers/criterion_handlers.py
--rw-rw-rw-   0        0        0     3723 2023-06-26 22:20:21.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/main.py
-drwxrwxrwx   0        0        0        0 2023-06-26 22:33:35.890305 c_custom_code_checker-1.0.3/c_custom_code_checker/models/
--rw-rw-rw-   0        0        0       33 2023-06-24 11:31:03.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/models/__init__.py
--rw-rw-rw-   0        0        0      869 2023-06-25 16:36:40.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/models/rule_model.py
-drwxrwxrwx   0        0        0        0 2023-06-26 22:33:35.897316 c_custom_code_checker-1.0.3/c_custom_code_checker/parsers/
--rw-rw-rw-   0        0        0       72 2023-06-24 11:31:32.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/parsers/__init__.py
--rw-rw-rw-   0        0        0     4044 2023-06-26 22:23:27.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/parsers/code_parser.py
--rw-rw-rw-   0        0        0     3089 2023-06-25 16:36:40.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/parsers/rule_parser.py
-drwxrwxrwx   0        0        0        0 2023-06-26 22:33:35.902307 c_custom_code_checker-1.0.3/c_custom_code_checker/utlis/
--rw-rw-rw-   0        0        0      180 2023-06-24 11:34:06.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/utlis/__init__.py
--rw-rw-rw-   0        0        0      977 2023-06-25 16:36:40.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/utlis/console_utils.py
--rw-rw-rw-   0        0        0      465 2023-06-17 12:15:39.000000 c_custom_code_checker-1.0.3/c_custom_code_checker/utlis/files_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-26 22:33:35.850336 c_custom_code_checker-1.0.3/c_custom_code_checker.egg-info/
--rw-rw-rw-   0        0        0     5096 2023-06-26 22:33:35.000000 c_custom_code_checker-1.0.3/c_custom_code_checker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1688 2023-06-26 22:33:35.000000 c_custom_code_checker-1.0.3/c_custom_code_checker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 22:33:35.000000 c_custom_code_checker-1.0.3/c_custom_code_checker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-26 22:33:35.000000 c_custom_code_checker-1.0.3/c_custom_code_checker.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       71 2023-06-26 22:33:35.000000 c_custom_code_checker-1.0.3/c_custom_code_checker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-26 22:33:35.000000 c_custom_code_checker-1.0.3/c_custom_code_checker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      718 2023-06-26 22:32:58.000000 c_custom_code_checker-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-26 22:33:35.904306 c_custom_code_checker-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      378 2023-06-26 22:33:12.000000 c_custom_code_checker-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:05:44.608195 c_custom_code_checker-1.0.4/
+-rw-rw-rw-   0        0        0     5181 2023-06-29 22:05:44.606191 c_custom_code_checker-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4662 2023-06-26 22:34:49.000000 c_custom_code_checker-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 22:05:44.505192 c_custom_code_checker-1.0.4/c_custom_code_checker/
+-rw-rw-rw-   0        0        0       22 2023-06-24 13:04:57.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:05:44.539197 c_custom_code_checker-1.0.4/c_custom_code_checker/constants/
+-rw-rw-rw-   0        0        0      169 2023-06-24 11:35:28.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/constants/__init__.py
+-rw-rw-rw-   0        0        0      164 2023-06-18 11:56:47.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/constants/criterion_keys.py
+-rw-rw-rw-   0        0        0      800 2023-06-26 22:04:39.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/constants/rules_reserved_keys.py
+-rw-rw-rw-   0        0        0      388 2023-06-25 16:52:24.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/constants/strings.py
+-rw-rw-rw-   0        0        0      345 2023-06-23 22:02:21.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/constants/target_keys.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:05:44.550207 c_custom_code_checker-1.0.4/c_custom_code_checker/enums/
+-rw-rw-rw-   0        0        0       78 2023-06-24 12:38:52.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/enums/__init__.py
+-rw-rw-rw-   0        0        0     1587 2023-06-25 16:36:40.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/enums/criterion_enum.py
+-rw-rw-rw-   0        0        0     1949 2023-06-26 22:09:23.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/enums/target_enum.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:05:44.573196 c_custom_code_checker-1.0.4/c_custom_code_checker/exceptions/
+-rw-rw-rw-   0        0        0      442 2023-06-24 11:30:38.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      193 2023-06-19 23:09:18.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/exceptions/criterion_not_respected_exception.py
+-rw-rw-rw-   0        0        0      184 2023-06-18 11:43:14.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/exceptions/criterion_value_missing_exception.py
+-rw-rw-rw-   0        0        0      176 2023-06-15 23:54:12.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/exceptions/invalid_criterion_exception.py
+-rw-rw-rw-   0        0        0      170 2023-06-15 23:46:33.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/exceptions/invalid_target_exception.py
+-rw-rw-rw-   0        0        0      173 2023-06-21 00:25:53.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/exceptions/lib_clang_not_found_exception.py
+-rw-rw-rw-   0        0        0      177 2023-06-15 23:33:03.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/exceptions/rule_missing_criterion_exception.py
+-rw-rw-rw-   0        0        0      173 2023-06-15 23:30:38.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/exceptions/rule_missing_target_exception.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:05:44.581196 c_custom_code_checker-1.0.4/c_custom_code_checker/handlers/
+-rw-rw-rw-   0        0        0      181 2023-06-24 12:42:42.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/handlers/__init__.py
+-rw-rw-rw-   0        0        0     2081 2023-06-25 16:36:40.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/handlers/criterion_handlers.py
+-rw-rw-rw-   0        0        0     4546 2023-06-29 22:05:10.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/main.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:05:44.585392 c_custom_code_checker-1.0.4/c_custom_code_checker/models/
+-rw-rw-rw-   0        0        0       33 2023-06-24 11:31:03.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/models/__init__.py
+-rw-rw-rw-   0        0        0      869 2023-06-25 16:36:40.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/models/rule_model.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:05:44.597198 c_custom_code_checker-1.0.4/c_custom_code_checker/parsers/
+-rw-rw-rw-   0        0        0       72 2023-06-24 11:31:32.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/parsers/__init__.py
+-rw-rw-rw-   0        0        0     4044 2023-06-26 22:23:27.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/parsers/code_parser.py
+-rw-rw-rw-   0        0        0     3089 2023-06-25 16:36:40.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/parsers/rule_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:05:44.604191 c_custom_code_checker-1.0.4/c_custom_code_checker/utlis/
+-rw-rw-rw-   0        0        0      180 2023-06-24 11:34:06.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/utlis/__init__.py
+-rw-rw-rw-   0        0        0      977 2023-06-25 16:36:40.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/utlis/console_utils.py
+-rw-rw-rw-   0        0        0      465 2023-06-17 12:15:39.000000 c_custom_code_checker-1.0.4/c_custom_code_checker/utlis/files_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:05:44.525193 c_custom_code_checker-1.0.4/c_custom_code_checker.egg-info/
+-rw-rw-rw-   0        0        0     5181 2023-06-29 22:05:44.000000 c_custom_code_checker-1.0.4/c_custom_code_checker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1688 2023-06-29 22:05:44.000000 c_custom_code_checker-1.0.4/c_custom_code_checker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 22:05:44.000000 c_custom_code_checker-1.0.4/c_custom_code_checker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-29 22:05:44.000000 c_custom_code_checker-1.0.4/c_custom_code_checker.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       71 2023-06-29 22:05:44.000000 c_custom_code_checker-1.0.4/c_custom_code_checker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-29 22:05:44.000000 c_custom_code_checker-1.0.4/c_custom_code_checker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      718 2023-06-29 21:18:04.000000 c_custom_code_checker-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-29 22:05:44.610192 c_custom_code_checker-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      378 2023-06-29 21:17:45.000000 c_custom_code_checker-1.0.4/setup.py
```

### Comparing `c_custom_code_checker-1.0.3/PKG-INFO` & `c_custom_code_checker-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c_custom_code_checker
-Version: 1.0.3
+Version: 1.0.4
 Summary: Syntax checker with custom rules for c language. Create rules with your team and consider using this tool to help verify the projects developed
 Author-email: Yago Caetano <yago_caetano@outlook.com>
 Project-URL: Homepage, https://github.com/Yago-Caetano/c-custom-code-checker
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -114,15 +114,15 @@
 
 |   Target Value    |   Description |
 |-------------------|---------------|
 |  "functions"        |   This rule target are the functions declaration            |
 |   "globals"        |   This rule target are the global variables                |
 |   "variables"      |   This rule target are the local variables                 |
 |   "macros"          |  This rule target are Macros declarations                     |
-
+|   "enums"          |  This rule target are enums declaration                      |
 
 ## Contributing
 
 Thank you for your interest in contributing to this project! We welcome contributions from the community, as they help make this project better.
 
 To contribute, please follow these guidelines:
```

### Comparing `c_custom_code_checker-1.0.3/README.md` & `c_custom_code_checker-1.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 |   Target Value    |   Description |
 |-------------------|---------------|
 |  "functions"        |   This rule target are the functions declaration            |
 |   "globals"        |   This rule target are the global variables                |
 |   "variables"      |   This rule target are the local variables                 |
 |   "macros"          |  This rule target are Macros declarations                     |
-
+|   "enums"          |  This rule target are enums declaration                      |
 
 ## Contributing
 
 Thank you for your interest in contributing to this project! We welcome contributions from the community, as they help make this project better.
 
 To contribute, please follow these guidelines:
```

### Comparing `c_custom_code_checker-1.0.3/c_custom_code_checker/constants/rules_reserved_keys.py` & `c_custom_code_checker-1.0.4/c_custom_code_checker/constants/rules_reserved_keys.py`

 * *Files identical despite different names*

### Comparing `c_custom_code_checker-1.0.3/c_custom_code_checker/enums/criterion_enum.py` & `c_custom_code_checker-1.0.4/c_custom_code_checker/enums/criterion_enum.py`

 * *Files identical despite different names*

### Comparing `c_custom_code_checker-1.0.3/c_custom_code_checker/enums/target_enum.py` & `c_custom_code_checker-1.0.4/c_custom_code_checker/enums/target_enum.py`

 * *Files identical despite different names*

### Comparing `c_custom_code_checker-1.0.3/c_custom_code_checker/handlers/criterion_handlers.py` & `c_custom_code_checker-1.0.4/c_custom_code_checker/handlers/criterion_handlers.py`

 * *Files identical despite different names*

### Comparing `c_custom_code_checker-1.0.3/c_custom_code_checker/main.py` & `c_custom_code_checker-1.0.4/c_custom_code_checker/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from c_custom_code_checker.parsers.rule_parser import RuleParser
 from c_custom_code_checker.utlis.console_utils import  print_exception, print_failure, print_header, print_process, print_success
 from c_custom_code_checker.utlis.files_utils import search_files_by_keyword
 
 
 ruleParser = RuleParser()
 lib_clang_path = None
+show_complete_log = True
 
 def get_libclang_install_dir():
     path_env = os.getenv("PATH")
     platform_name = platform.system()
 
     if path_env:
         paths = path_env.split(os.pathsep)
@@ -44,59 +45,77 @@
     #check if there is libclang environment variable
     lib_clang_path = get_libclang_install_dir()
     if (lib_clang_path == None):
         raise LibClangNotFoundException()
     
 
 def check_rules(files,rules_directory):
+
+    global show_complete_log
     rules = []
+
     ret_files = search_files_by_keyword(rules_directory,"rule","json")
 
     if(len(ret_files) == 0):
         print_failure(StringsConstants.NO_RULES_FOUND)
         return -1
     
-    pbar = tqdm(ret_files)
-    for file in pbar:
-        pbar.set_description(f'Reading rule: {file}')
-        rules.append(ruleParser.parse_file(file))
+    if(show_complete_log == True):
+        pbar = tqdm(ret_files)
+        for file in pbar:
+            pbar.set_description(f'Reading rule: {file}')
+            rules.append(ruleParser.parse_file(file))
+    else:
+        for file in ret_files:
+            rules.append(ruleParser.parse_file(file))
 
     return rules
 
 def check_code(files,rules):
 
     global lib_clang_path
+    global show_complete_log
 
-    print_process(StringsConstants.CODE_CHECKING_TITLE)
+    if(show_complete_log == True):
+        print_process(StringsConstants.CODE_CHECKING_TITLE)
 
-    code_parser = CodeParser(rules,lib_clang_path)
-    pbar = tqdm(files)
+        code_parser = CodeParser(rules,lib_clang_path)
+        pbar = tqdm(files)
 
-    for code in pbar:
-        pbar.set_description(f"{code}")
-        code_parser.parse_code_file(code)
+        for code in pbar:
+            pbar.set_description(f"{code}")
+            code_parser.parse_code_file(code)
+    else:
+        code_parser = CodeParser(rules,lib_clang_path)
+
+        for code in files:
+            code_parser.parse_code_file(code)
 
 
 def startup(files,rules_directory):
 
+    global show_complete_log
+
     try:
 
         check_prerequisites()
 
-        print_header()
-        print_process(StringsConstants.PARSING_RULES_TITLE)
+        if(show_complete_log == True):
+            print_header()
+            print_process(StringsConstants.PARSING_RULES_TITLE)
 
         rules = check_rules(files,rules_directory)
 
     except Exception as e:
         print_exception(e)
         print_failure(StringsConstants.RULE_PARSING_FAILED)
         return -1
-
-    print_success(StringsConstants.RULE_PARSING_SUCCEDED)
+    
+    if(show_complete_log == True):
+        print_success(StringsConstants.RULE_PARSING_SUCCEDED)
 
     try:
         check_code(files,rules)
         print_success(StringsConstants.CODE_CHECKING_SUCCEDED)
         return 0
     except Exception as e:
         print_exception(e)
@@ -104,14 +123,15 @@
     
 
 
 def main():
     parser = argparse.ArgumentParser(description=StringsConstants.TITLE)
     parser.add_argument("--input","-i",nargs="+",help="List of C files to analyse",required=True)
     parser.add_argument("--rules_path","-r",help="Path to rules",required=True)
+    parser.add_argument("--simple_out","-s",help="Shows a simple output, only containing relevant data",required=False,action='store_false')
 
     args = parser.parse_args()
 
     in_files = []
 
     for input_record in args.input:
 
@@ -123,12 +143,17 @@
                 in_files.append(file_path)
 
         else:
             in_files.append(input_record)
 
     rules_path = args.rules_path
 
+    global show_complete_log
+
+    if(args.simple_out != None):
+        show_complete_log = args.simple_out
+
     return startup(in_files,rules_path)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `c_custom_code_checker-1.0.3/c_custom_code_checker/models/rule_model.py` & `c_custom_code_checker-1.0.4/c_custom_code_checker/models/rule_model.py`

 * *Files identical despite different names*

### Comparing `c_custom_code_checker-1.0.3/c_custom_code_checker/parsers/code_parser.py` & `c_custom_code_checker-1.0.4/c_custom_code_checker/parsers/code_parser.py`

 * *Files identical despite different names*

### Comparing `c_custom_code_checker-1.0.3/c_custom_code_checker/parsers/rule_parser.py` & `c_custom_code_checker-1.0.4/c_custom_code_checker/parsers/rule_parser.py`

 * *Files identical despite different names*

### Comparing `c_custom_code_checker-1.0.3/c_custom_code_checker/utlis/console_utils.py` & `c_custom_code_checker-1.0.4/c_custom_code_checker/utlis/console_utils.py`

 * *Files identical despite different names*

### Comparing `c_custom_code_checker-1.0.3/c_custom_code_checker.egg-info/PKG-INFO` & `c_custom_code_checker-1.0.4/c_custom_code_checker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c-custom-code-checker
-Version: 1.0.3
+Version: 1.0.4
 Summary: Syntax checker with custom rules for c language. Create rules with your team and consider using this tool to help verify the projects developed
 Author-email: Yago Caetano <yago_caetano@outlook.com>
 Project-URL: Homepage, https://github.com/Yago-Caetano/c-custom-code-checker
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -114,15 +114,15 @@
 
 |   Target Value    |   Description |
 |-------------------|---------------|
 |  "functions"        |   This rule target are the functions declaration            |
 |   "globals"        |   This rule target are the global variables                |
 |   "variables"      |   This rule target are the local variables                 |
 |   "macros"          |  This rule target are Macros declarations                     |
-
+|   "enums"          |  This rule target are enums declaration                      |
 
 ## Contributing
 
 Thank you for your interest in contributing to this project! We welcome contributions from the community, as they help make this project better.
 
 To contribute, please follow these guidelines:
```

### Comparing `c_custom_code_checker-1.0.3/c_custom_code_checker.egg-info/SOURCES.txt` & `c_custom_code_checker-1.0.4/c_custom_code_checker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `c_custom_code_checker-1.0.3/pyproject.toml` & `c_custom_code_checker-1.0.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","art>=6.0","clang>=16.0.1.1","colorama>=0.4.4","libclang>=16.0.0","tqdm>=4.65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "c_custom_code_checker"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Yago Caetano", email="yago_caetano@outlook.com" },
 ]
 description = "Syntax checker with custom rules for c language. Create rules with your team and consider using this tool to help verify the projects developed"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

