# Comparing `tmp/stdocker-1.1.0.tar.gz` & `tmp/stdocker-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdocker-1.1.0.tar", last modified: Fri Jun 30 08:09:09 2023, max compression
+gzip compressed data, was "stdocker-1.1.1.tar", last modified: Fri Jun 30 09:14:08 2023, max compression
```

## Comparing `stdocker-1.1.0.tar` & `stdocker-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 sunfeng   (1000) sunfeng   (1000)        0 2023-06-30 08:09:09.044449 stdocker-1.1.0/
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    27710 2023-06-30 08:09:09.044449 stdocker-1.1.0/PKG-INFO
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    18587 2023-06-30 08:05:30.000000 stdocker-1.1.0/README.md
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       38 2023-06-30 08:09:09.044449 stdocker-1.1.0/setup.cfg
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)     1644 2022-08-23 10:32:44.000000 stdocker-1.1.0/setup.py
-drwxrwxr-x   0 sunfeng   (1000) sunfeng   (1000)        0 2023-06-30 08:09:09.040449 stdocker-1.1.0/stdocker/
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        0 2022-08-22 10:00:30.000000 stdocker-1.1.0/stdocker/__init__.py
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    18523 2023-06-30 08:00:19.000000 stdocker-1.1.0/stdocker/cli.py
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      632 2023-01-17 10:40:06.000000 stdocker-1.1.0/stdocker/config.py
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)     5654 2022-11-04 07:15:18.000000 stdocker-1.1.0/stdocker/env_handler.py
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)     1395 2022-09-01 02:43:21.000000 stdocker-1.1.0/stdocker/env_parser.py
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      532 2022-09-01 03:32:56.000000 stdocker-1.1.0/stdocker/utils.py
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       22 2023-06-30 07:50:13.000000 stdocker-1.1.0/stdocker/version.py
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      748 2022-09-01 02:19:41.000000 stdocker-1.1.0/stdocker/yaml_parser.py
-drwxrwxr-x   0 sunfeng   (1000) sunfeng   (1000)        0 2023-06-30 08:09:09.040449 stdocker-1.1.0/stdocker.egg-info/
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    27710 2023-06-30 08:09:08.000000 stdocker-1.1.0/stdocker.egg-info/PKG-INFO
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      408 2023-06-30 08:09:09.000000 stdocker-1.1.0/stdocker.egg-info/SOURCES.txt
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        1 2023-06-30 08:09:08.000000 stdocker-1.1.0/stdocker.egg-info/dependency_links.txt
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       48 2023-06-30 08:09:08.000000 stdocker-1.1.0/stdocker.egg-info/entry_points.txt
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        1 2023-06-30 08:09:08.000000 stdocker-1.1.0/stdocker.egg-info/not-zip-safe
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       98 2023-06-30 08:09:08.000000 stdocker-1.1.0/stdocker.egg-info/requires.txt
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        9 2023-06-30 08:09:08.000000 stdocker-1.1.0/stdocker.egg-info/top_level.txt
+drwxrwxr-x   0 sunfeng   (1000) sunfeng   (1000)        0 2023-06-30 09:14:08.500172 stdocker-1.1.1/
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    27852 2023-06-30 09:14:08.500172 stdocker-1.1.1/PKG-INFO
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    18587 2023-06-30 09:08:00.000000 stdocker-1.1.1/README.md
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       38 2023-06-30 09:14:08.500172 stdocker-1.1.1/setup.cfg
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)     1644 2022-08-23 10:32:44.000000 stdocker-1.1.1/setup.py
+drwxrwxr-x   0 sunfeng   (1000) sunfeng   (1000)        0 2023-06-30 09:14:08.500172 stdocker-1.1.1/stdocker/
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        0 2022-08-22 10:00:30.000000 stdocker-1.1.1/stdocker/__init__.py
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    18519 2023-06-30 08:50:28.000000 stdocker-1.1.1/stdocker/cli.py
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      632 2023-01-17 10:40:06.000000 stdocker-1.1.1/stdocker/config.py
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)     5654 2022-11-04 07:15:18.000000 stdocker-1.1.1/stdocker/env_handler.py
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)     1395 2022-09-01 02:43:21.000000 stdocker-1.1.1/stdocker/env_parser.py
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      532 2022-09-01 03:32:56.000000 stdocker-1.1.1/stdocker/utils.py
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       22 2023-06-30 09:07:02.000000 stdocker-1.1.1/stdocker/version.py
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      748 2022-09-01 02:19:41.000000 stdocker-1.1.1/stdocker/yaml_parser.py
+drwxrwxr-x   0 sunfeng   (1000) sunfeng   (1000)        0 2023-06-30 09:14:08.500172 stdocker-1.1.1/stdocker.egg-info/
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    27852 2023-06-30 09:14:08.000000 stdocker-1.1.1/stdocker.egg-info/PKG-INFO
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      408 2023-06-30 09:14:08.000000 stdocker-1.1.1/stdocker.egg-info/SOURCES.txt
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        1 2023-06-30 09:14:08.000000 stdocker-1.1.1/stdocker.egg-info/dependency_links.txt
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       48 2023-06-30 09:14:08.000000 stdocker-1.1.1/stdocker.egg-info/entry_points.txt
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        1 2023-06-30 09:14:08.000000 stdocker-1.1.1/stdocker.egg-info/not-zip-safe
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       98 2023-06-30 09:14:08.000000 stdocker-1.1.1/stdocker.egg-info/requires.txt
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        9 2023-06-30 09:14:08.000000 stdocker-1.1.1/stdocker.egg-info/top_level.txt
```

### Comparing `stdocker-1.1.0/PKG-INFO` & `stdocker-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdocker
-Version: 1.1.0
+Version: 1.1.1
 Summary: Shinetech Docker CLI.
 Home-page: https://github.com/winds1983/stdocker
 Author: Jason Sun
 Author-email: sunf@shinetechsoftware.com
 License: MIT
 Description: # Shinetech Docker CLI
         
@@ -44,15 +44,15 @@
         
         ```shell
         sudo pip3 install stdocker
         ```
         
         If you get error `ERROR: Could not find a version that satisfies the requirement`, please use the following command to install:
         ```shell
-        python3 -m pip install stdocker==1.1.0
+        python3 -m pip install stdocker==1.1.1
         ```
         
         It based on the internal docker project `Shinetech Docker`, please install it first. If you do not have permission to use Shinetech Docker, please ignore this package.
         
         After the installation is successful, you can run the `stdocker` command in any directory and perform the operations you need.
         
         ## Use Cases
@@ -243,15 +243,15 @@
         stdocker build <ENV>
         ```
         
         If `ENV` is empty, it will guide you to create your customized configuration, otherwise will base on your specified env to build services.
         
         ```shell
         stdocker build
-        stdocker build --env=magento_244
+        stdocker build --env=magento_246
         ```
         
         ### Export and import database
         
         ```shell
         stdocker database <ACTION{import|export}>
         ```
@@ -484,14 +484,21 @@
         
         All notable changes to this project will be documented in this file.
         
         The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this
         project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
         
         
+        ## [1.1.1] - 2023-06-30
+        
+        ### Added
+        
+        - Fix install or upgrade docker compose command
+        
+        
         ## [1.1.0] - 2023-06-30
         
         ### Added
         
         - Add install or upgrade docker compose command
```

### Comparing `stdocker-1.1.0/README.md` & `stdocker-1.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 ```shell
 sudo pip3 install stdocker
 ```
 
 If you get error `ERROR: Could not find a version that satisfies the requirement`, please use the following command to install:
 ```shell
-python3 -m pip install stdocker==1.1.0
+python3 -m pip install stdocker==1.1.1
 ```
 
 It based on the internal docker project `Shinetech Docker`, please install it first. If you do not have permission to use Shinetech Docker, please ignore this package.
 
 After the installation is successful, you can run the `stdocker` command in any directory and perform the operations you need.
 
 ## Use Cases
@@ -235,15 +235,15 @@
 stdocker build <ENV>
 ```
 
 If `ENV` is empty, it will guide you to create your customized configuration, otherwise will base on your specified env to build services.
 
 ```shell
 stdocker build
-stdocker build --env=magento_244
+stdocker build --env=magento_246
 ```
 
 ### Export and import database
 
 ```shell
 stdocker database <ACTION{import|export}>
 ```
```

### Comparing `stdocker-1.1.0/setup.py` & `stdocker-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `stdocker-1.1.0/stdocker/cli.py` & `stdocker-1.1.1/stdocker/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -455,17 +455,17 @@
 
 @cli.command()
 @click.pass_context
 @click.argument('version', required=False)
 def setup_docker_compose(ctx: click.Context, version: Any) -> None:
     """Install or upgrade docker compose"""
     if version:
-        os.system('bash bin/upgrade_docker_compose.sh ' + version)
+        os.system('bash bin/setup_docker_compose.sh ' + version)
     else:
-        os.system('bash bin/upgrade_docker_compose.sh')
+        os.system('bash bin/setup_docker_compose.sh')
 
 
 def main():
     cli()
 
 
 if __name__ == '__main__':
```

### Comparing `stdocker-1.1.0/stdocker/config.py` & `stdocker-1.1.1/stdocker/config.py`

 * *Files identical despite different names*

### Comparing `stdocker-1.1.0/stdocker/env_handler.py` & `stdocker-1.1.1/stdocker/env_handler.py`

 * *Files identical despite different names*

### Comparing `stdocker-1.1.0/stdocker/env_parser.py` & `stdocker-1.1.1/stdocker/env_parser.py`

 * *Files identical despite different names*

### Comparing `stdocker-1.1.0/stdocker/utils.py` & `stdocker-1.1.1/stdocker/utils.py`

 * *Files identical despite different names*

### Comparing `stdocker-1.1.0/stdocker/yaml_parser.py` & `stdocker-1.1.1/stdocker/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `stdocker-1.1.0/stdocker.egg-info/PKG-INFO` & `stdocker-1.1.1/stdocker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdocker
-Version: 1.1.0
+Version: 1.1.1
 Summary: Shinetech Docker CLI.
 Home-page: https://github.com/winds1983/stdocker
 Author: Jason Sun
 Author-email: sunf@shinetechsoftware.com
 License: MIT
 Description: # Shinetech Docker CLI
         
@@ -44,15 +44,15 @@
         
         ```shell
         sudo pip3 install stdocker
         ```
         
         If you get error `ERROR: Could not find a version that satisfies the requirement`, please use the following command to install:
         ```shell
-        python3 -m pip install stdocker==1.1.0
+        python3 -m pip install stdocker==1.1.1
         ```
         
         It based on the internal docker project `Shinetech Docker`, please install it first. If you do not have permission to use Shinetech Docker, please ignore this package.
         
         After the installation is successful, you can run the `stdocker` command in any directory and perform the operations you need.
         
         ## Use Cases
@@ -243,15 +243,15 @@
         stdocker build <ENV>
         ```
         
         If `ENV` is empty, it will guide you to create your customized configuration, otherwise will base on your specified env to build services.
         
         ```shell
         stdocker build
-        stdocker build --env=magento_244
+        stdocker build --env=magento_246
         ```
         
         ### Export and import database
         
         ```shell
         stdocker database <ACTION{import|export}>
         ```
@@ -484,14 +484,21 @@
         
         All notable changes to this project will be documented in this file.
         
         The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this
         project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
         
         
+        ## [1.1.1] - 2023-06-30
+        
+        ### Added
+        
+        - Fix install or upgrade docker compose command
+        
+        
         ## [1.1.0] - 2023-06-30
         
         ### Added
         
         - Add install or upgrade docker compose command
```

