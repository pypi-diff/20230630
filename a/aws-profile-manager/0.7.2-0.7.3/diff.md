# Comparing `tmp/aws-profile-manager-0.7.2.tar.gz` & `tmp/aws-profile-manager-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-profile-manager-0.7.2.tar", last modified: Sun Jan 29 19:53:11 2023, max compression
+gzip compressed data, was "aws-profile-manager-0.7.3.tar", last modified: Fri Jun 30 11:22:34 2023, max compression
```

## Comparing `aws-profile-manager-0.7.2.tar` & `aws-profile-manager-0.7.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 19:53:11.401929 aws-profile-manager-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-01-29 19:53:11.401929 aws-profile-manager-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 19:53:11.393929 aws-profile-manager-0.7.2/aws_profile_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 19:53:11.397929 aws-profile-manager-0.7.2/aws_profile_manager/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/commands/profile-add.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/commands/profile-current.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/commands/profile-edit.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/commands/profile-list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/commands/profile-remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/commands/profile-switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/commands/rotate-keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 19:53:11.397929 aws-profile-manager-0.7.2/aws_profile_manager/common/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/common/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 19:53:11.397929 aws-profile-manager-0.7.2/aws_profile_manager/profile_add/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/profile_add/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/profile_add/add.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 19:53:11.397929 aws-profile-manager-0.7.2/aws_profile_manager/profile_edit/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/profile_edit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/profile_edit/edit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 19:53:11.397929 aws-profile-manager-0.7.2/aws_profile_manager/profile_switch/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/profile_switch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/profile_switch/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 19:53:11.401929 aws-profile-manager-0.7.2/aws_profile_manager/rotate_keys/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/rotate_keys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/rotate_keys/rotate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 19:53:11.401929 aws-profile-manager-0.7.2/aws_profile_manager/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/aws_profile_manager/tests/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 19:53:11.397929 aws-profile-manager-0.7.2/aws_profile_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-01-29 19:53:11.000000 aws-profile-manager-0.7.2/aws_profile_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-01-29 19:53:11.000000 aws-profile-manager-0.7.2/aws_profile_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-29 19:53:11.000000 aws-profile-manager-0.7.2/aws_profile_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-29 19:53:11.000000 aws-profile-manager-0.7.2/aws_profile_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-01-29 19:53:11.000000 aws-profile-manager-0.7.2/aws_profile_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-29 19:53:11.000000 aws-profile-manager-0.7.2/aws_profile_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-29 19:53:11.401929 aws-profile-manager-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-01-29 19:52:56.000000 aws-profile-manager-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:22:34.699245 aws-profile-manager-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-06-30 11:22:34.699245 aws-profile-manager-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:22:34.691244 aws-profile-manager-0.7.3/aws_profile_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:22:34.695245 aws-profile-manager-0.7.3/aws_profile_manager/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/commands/profile-add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/commands/profile-current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/commands/profile-edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/commands/profile-list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/commands/profile-remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/commands/profile-switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/commands/rotate-keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:22:34.695245 aws-profile-manager-0.7.3/aws_profile_manager/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/common/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:22:34.695245 aws-profile-manager-0.7.3/aws_profile_manager/profile_add/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/profile_add/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/profile_add/add.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:22:34.695245 aws-profile-manager-0.7.3/aws_profile_manager/profile_edit/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/profile_edit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/profile_edit/edit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:22:34.695245 aws-profile-manager-0.7.3/aws_profile_manager/profile_switch/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/profile_switch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/profile_switch/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:22:34.699245 aws-profile-manager-0.7.3/aws_profile_manager/rotate_keys/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/rotate_keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/rotate_keys/rotate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:22:34.699245 aws-profile-manager-0.7.3/aws_profile_manager/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/aws_profile_manager/tests/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:22:34.695245 aws-profile-manager-0.7.3/aws_profile_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-06-30 11:22:34.000000 aws-profile-manager-0.7.3/aws_profile_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-30 11:22:34.000000 aws-profile-manager-0.7.3/aws_profile_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 11:22:34.000000 aws-profile-manager-0.7.3/aws_profile_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-30 11:22:34.000000 aws-profile-manager-0.7.3/aws_profile_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 11:22:34.000000 aws-profile-manager-0.7.3/aws_profile_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-30 11:22:34.000000 aws-profile-manager-0.7.3/aws_profile_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 11:22:34.699245 aws-profile-manager-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-30 11:22:18.000000 aws-profile-manager-0.7.3/setup.py
```

### Comparing `aws-profile-manager-0.7.2/LICENSE` & `aws-profile-manager-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-profile-manager-0.7.2/PKG-INFO` & `aws-profile-manager-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-profile-manager
-Version: 0.7.2
+Version: 0.7.3
 Summary: This util allows you to manager your AWS profiles like add, remove, update and switch default AWS CLI profile
 Home-page: https://github.com/99stealth/aws-profile-manager
 Author: Roman Banakh
 Author-email: banakh.ri@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aws-profile-manager-0.7.2/README.md` & `aws-profile-manager-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `aws-profile-manager-0.7.2/aws_profile_manager/cli.py` & `aws-profile-manager-0.7.3/aws_profile_manager/cli.py`

 * *Files identical despite different names*

### Comparing `aws-profile-manager-0.7.2/aws_profile_manager/commands/profile-add.py` & `aws-profile-manager-0.7.3/aws_profile_manager/commands/profile-add.py`

 * *Files identical despite different names*

### Comparing `aws-profile-manager-0.7.2/aws_profile_manager/commands/profile-edit.py` & `aws-profile-manager-0.7.3/aws_profile_manager/commands/profile-edit.py`

 * *Files identical despite different names*

### Comparing `aws-profile-manager-0.7.2/aws_profile_manager/commands/profile-list.py` & `aws-profile-manager-0.7.3/aws_profile_manager/commands/profile-list.py`

 * *Files identical despite different names*

### Comparing `aws-profile-manager-0.7.2/aws_profile_manager/commands/profile-remove.py` & `aws-profile-manager-0.7.3/aws_profile_manager/commands/profile-remove.py`

 * *Files identical despite different names*

### Comparing `aws-profile-manager-0.7.2/aws_profile_manager/commands/profile-switch.py` & `aws-profile-manager-0.7.3/aws_profile_manager/commands/profile-switch.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 import click
 import logging
 from aws_profile_manager import Common, Switch
 
 @click.command()
-def cli():
+@click.option('--aws-profile-name', required=False, help="AWS profile to switch", type=str)
+def cli(aws_profile_name):
     """ Switch default AWS profile in your ~/.aws/credentials """
     common = Common()
     switch = Switch()
 
     users_home = common.get_users_home()
     all_profiles = common.get_all_profiles(users_home)
-    new_default_profile_name = None
-    if "default" not in all_profiles:
-        logging.warning(f"There is no [default] profile in your {users_home}/.aws/credentials. It will be automatically created")
+    new_default_profile_name = aws_profile_name
+    if not new_default_profile_name:
+        if "default" not in all_profiles:
+            logging.warning(f"There is no [default] profile in your {users_home}/.aws/credentials. It will be automatically created")
+        else:
+            defaults_backup = switch.get_defaults_backup(all_profiles)
+            if defaults_backup:
+                logging.warning(f"Your current default is \033[1m{defaults_backup}\033[0m (excluded from options below)\n")
+            else:
+                new_default_profile_name = switch.ask_new_name_for_default_profile(users_home, all_profiles)
+                if new_default_profile_name:
+                    all_profiles = switch.create_backup_for_default(all_profiles, new_default_profile_name)
+        new_default = common.choose_profile(all_profiles, operation="switch your current default", skip_profiles=["default", new_default_profile_name, defaults_backup])
     else:
-        defaults_backup = switch.get_defaults_backup(all_profiles)
-        if defaults_backup:
-            logging.warning(f"Your current default is \033[1m{defaults_backup}\033[0m (excluded from options below)\n")
+        if new_default_profile_name in all_profiles:
+            new_default = new_default_profile_name
         else:
-            new_default_profile_name = switch.ask_new_name_for_default_profile(users_home, all_profiles)
-            if new_default_profile_name:
-                all_profiles = switch.create_backup_for_default(all_profiles, new_default_profile_name)
-    new_default = common.choose_profile(all_profiles, operation="switch your current default", skip_profiles=["default", new_default_profile_name, defaults_backup])
+            logging.error(f"No such profile \033[1m{new_default_profile_name}\033[0m\n in profiles' list")
+            exit(1)
     new_profiles_list = common.generate_new_profile_list(all_profiles, new_default)
-    common.rewrite_credentials_file(new_profiles_list, users_home)
+    common.rewrite_credentials_file(new_profiles_list, users_home)
+    logging.info(f'Default profile has been changed to \033[1m{new_default}\033[0m')
```

### Comparing `aws-profile-manager-0.7.2/aws_profile_manager/commands/rotate-keys.py` & `aws-profile-manager-0.7.3/aws_profile_manager/commands/rotate-keys.py`

 * *Files identical despite different names*

### Comparing `aws-profile-manager-0.7.2/aws_profile_manager/common/common.py` & `aws-profile-manager-0.7.3/aws_profile_manager/common/common.py`

 * *Files identical despite different names*

### Comparing `aws-profile-manager-0.7.2/aws_profile_manager/profile_add/add.py` & `aws-profile-manager-0.7.3/aws_profile_manager/profile_add/add.py`

 * *Files identical despite different names*

### Comparing `aws-profile-manager-0.7.2/aws_profile_manager/profile_edit/edit.py` & `aws-profile-manager-0.7.3/aws_profile_manager/profile_edit/edit.py`

 * *Files identical despite different names*

### Comparing `aws-profile-manager-0.7.2/aws_profile_manager/profile_switch/switch.py` & `aws-profile-manager-0.7.3/aws_profile_manager/profile_switch/switch.py`

 * *Files identical despite different names*

### Comparing `aws-profile-manager-0.7.2/aws_profile_manager/rotate_keys/rotate.py` & `aws-profile-manager-0.7.3/aws_profile_manager/rotate_keys/rotate.py`

 * *Files identical despite different names*

### Comparing `aws-profile-manager-0.7.2/aws_profile_manager/tests/common.py` & `aws-profile-manager-0.7.3/aws_profile_manager/tests/common.py`

 * *Files identical despite different names*

### Comparing `aws-profile-manager-0.7.2/aws_profile_manager/tests/switch.py` & `aws-profile-manager-0.7.3/aws_profile_manager/tests/switch.py`

 * *Files identical despite different names*

### Comparing `aws-profile-manager-0.7.2/aws_profile_manager.egg-info/PKG-INFO` & `aws-profile-manager-0.7.3/aws_profile_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-profile-manager
-Version: 0.7.2
+Version: 0.7.3
 Summary: This util allows you to manager your AWS profiles like add, remove, update and switch default AWS CLI profile
 Home-page: https://github.com/99stealth/aws-profile-manager
 Author: Roman Banakh
 Author-email: banakh.ri@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aws-profile-manager-0.7.2/aws_profile_manager.egg-info/SOURCES.txt` & `aws-profile-manager-0.7.3/aws_profile_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws-profile-manager-0.7.2/setup.py` & `aws-profile-manager-0.7.3/setup.py`

 * *Files identical despite different names*

