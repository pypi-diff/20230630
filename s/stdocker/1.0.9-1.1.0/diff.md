# Comparing `tmp/stdocker-1.0.9.tar.gz` & `tmp/stdocker-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdocker-1.0.9.tar", last modified: Fri Sep  9 10:43:07 2022, max compression
+gzip compressed data, was "stdocker-1.1.0.tar", last modified: Fri Jun 30 08:09:09 2023, max compression
```

## Comparing `stdocker-1.0.9.tar` & `stdocker-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 sunfeng   (1000) sunfeng   (1000)        0 2022-09-09 10:43:07.153344 stdocker-1.0.9/
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    22680 2022-09-09 10:43:07.153344 stdocker-1.0.9/PKG-INFO
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    16068 2022-09-09 10:24:53.000000 stdocker-1.0.9/README.md
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       38 2022-09-09 10:43:07.153344 stdocker-1.0.9/setup.cfg
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)     1644 2022-08-23 10:32:44.000000 stdocker-1.0.9/setup.py
-drwxrwxr-x   0 sunfeng   (1000) sunfeng   (1000)        0 2022-09-09 10:43:07.153344 stdocker-1.0.9/stdocker/
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        0 2022-08-22 10:00:30.000000 stdocker-1.0.9/stdocker/__init__.py
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    13631 2022-09-09 10:23:07.000000 stdocker-1.0.9/stdocker/cli.py
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      328 2022-09-09 06:53:04.000000 stdocker-1.0.9/stdocker/config.py
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)     5457 2022-09-08 09:39:09.000000 stdocker-1.0.9/stdocker/env_handler.py
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)     1395 2022-09-01 02:43:21.000000 stdocker-1.0.9/stdocker/env_parser.py
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      532 2022-09-01 03:32:56.000000 stdocker-1.0.9/stdocker/utils.py
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       22 2022-09-09 10:26:06.000000 stdocker-1.0.9/stdocker/version.py
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      748 2022-09-01 02:19:41.000000 stdocker-1.0.9/stdocker/yaml_parser.py
-drwxrwxr-x   0 sunfeng   (1000) sunfeng   (1000)        0 2022-09-09 10:43:07.153344 stdocker-1.0.9/stdocker.egg-info/
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    22680 2022-09-09 10:43:07.000000 stdocker-1.0.9/stdocker.egg-info/PKG-INFO
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      408 2022-09-09 10:43:07.000000 stdocker-1.0.9/stdocker.egg-info/SOURCES.txt
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        1 2022-09-09 10:43:07.000000 stdocker-1.0.9/stdocker.egg-info/dependency_links.txt
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       48 2022-09-09 10:43:07.000000 stdocker-1.0.9/stdocker.egg-info/entry_points.txt
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        1 2022-09-09 10:32:04.000000 stdocker-1.0.9/stdocker.egg-info/not-zip-safe
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       98 2022-09-09 10:43:07.000000 stdocker-1.0.9/stdocker.egg-info/requires.txt
--rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        9 2022-09-09 10:43:07.000000 stdocker-1.0.9/stdocker.egg-info/top_level.txt
+drwxrwxr-x   0 sunfeng   (1000) sunfeng   (1000)        0 2023-06-30 08:09:09.044449 stdocker-1.1.0/
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    27710 2023-06-30 08:09:09.044449 stdocker-1.1.0/PKG-INFO
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    18587 2023-06-30 08:05:30.000000 stdocker-1.1.0/README.md
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       38 2023-06-30 08:09:09.044449 stdocker-1.1.0/setup.cfg
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)     1644 2022-08-23 10:32:44.000000 stdocker-1.1.0/setup.py
+drwxrwxr-x   0 sunfeng   (1000) sunfeng   (1000)        0 2023-06-30 08:09:09.040449 stdocker-1.1.0/stdocker/
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        0 2022-08-22 10:00:30.000000 stdocker-1.1.0/stdocker/__init__.py
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    18523 2023-06-30 08:00:19.000000 stdocker-1.1.0/stdocker/cli.py
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      632 2023-01-17 10:40:06.000000 stdocker-1.1.0/stdocker/config.py
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)     5654 2022-11-04 07:15:18.000000 stdocker-1.1.0/stdocker/env_handler.py
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)     1395 2022-09-01 02:43:21.000000 stdocker-1.1.0/stdocker/env_parser.py
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      532 2022-09-01 03:32:56.000000 stdocker-1.1.0/stdocker/utils.py
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       22 2023-06-30 07:50:13.000000 stdocker-1.1.0/stdocker/version.py
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      748 2022-09-01 02:19:41.000000 stdocker-1.1.0/stdocker/yaml_parser.py
+drwxrwxr-x   0 sunfeng   (1000) sunfeng   (1000)        0 2023-06-30 08:09:09.040449 stdocker-1.1.0/stdocker.egg-info/
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)    27710 2023-06-30 08:09:08.000000 stdocker-1.1.0/stdocker.egg-info/PKG-INFO
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)      408 2023-06-30 08:09:09.000000 stdocker-1.1.0/stdocker.egg-info/SOURCES.txt
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        1 2023-06-30 08:09:08.000000 stdocker-1.1.0/stdocker.egg-info/dependency_links.txt
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       48 2023-06-30 08:09:08.000000 stdocker-1.1.0/stdocker.egg-info/entry_points.txt
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        1 2023-06-30 08:09:08.000000 stdocker-1.1.0/stdocker.egg-info/not-zip-safe
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)       98 2023-06-30 08:09:08.000000 stdocker-1.1.0/stdocker.egg-info/requires.txt
+-rw-rw-r--   0 sunfeng   (1000) sunfeng   (1000)        9 2023-06-30 08:09:08.000000 stdocker-1.1.0/stdocker.egg-info/top_level.txt
```

### Comparing `stdocker-1.0.9/PKG-INFO` & `stdocker-1.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdocker
-Version: 1.0.9
+Version: 1.1.0
 Summary: Shinetech Docker CLI.
 Home-page: https://github.com/winds1983/stdocker
 Author: Jason Sun
 Author-email: sunf@shinetechsoftware.com
 License: MIT
 Description: # Shinetech Docker CLI
         
@@ -26,28 +26,33 @@
           * [Export and import database](#export-and-import-database)
             * [Export database](#export-database)
             * [Import database](#import-database)
           * [Show the local environment and workspace information](#show-the-local-environment-and-workspace-information)
           * [List all environments](#list-all-environments)
           * [Initial workspace](#initial-workspace)
           * [Create and setup project](#create-and-setup-project)
-            * [Create a new project based on a base template or framework skeleton](#create-a-new-project-based-on-a-base-template-or-framework-skeleton)
-            * [Create a new Magento project based on the source code or composer](#create-a-new-Magento-project-based-on-the-source-code-or-composer)
+            * [Create a new PHP project based on a base template or framework skeleton](#create-a-new-php-project-based-on-a-base-template-or-framework-skeleton)
+            * [Create a new Magento project based on the source code or composer](#create-a-new-magento-project-based-on-the-source-code-or-composer)
+            * [Create a new Javascript project based on a base template or framework skeleton](#create-a-new-javascript-project-based-on-a-base-template-or-framework-skeleton)
             * [Build an existing project based on existing code and database](#build-an-existing-project-based-on-existing-code-and-database)
           * [Upgrade Shinetech Docker](#upgrade-shinetech-docker)
+          * [Switch network mode for a container](#switch-network-mode-for-a-container)
+          * [Edit or show configuration of docker-compose.yml](#edit-or-show-configuration-of-docker-compose-yml)
+          * [Show or live tail docker container logs](#show-or-live-tail-docker-container-logs)
+          * [Install or upgrade docker compose](#install-or-upgrade-docker-compose)
         
         ## Getting Started
         
         ```shell
-        pip3 install stdocker
+        sudo pip3 install stdocker
         ```
         
         If you get error `ERROR: Could not find a version that satisfies the requirement`, please use the following command to install:
         ```shell
-        python3 -m pip install stdocker==1.0.9
+        python3 -m pip install stdocker==1.1.0
         ```
         
         It based on the internal docker project `Shinetech Docker`, please install it first. If you do not have permission to use Shinetech Docker, please ignore this package.
         
         After the installation is successful, you can run the `stdocker` command in any directory and perform the operations you need.
         
         ## Use Cases
@@ -72,27 +77,32 @@
           --version               Show the version and exit.
           --help                  Show this message and exit.
         
         Commands:
           about                   Show the local environment and workspace...
           bash                    Bash session for running container
           build                   Build local development environment with your...
-          compose                 Execute sudo docker-compose * command
           configure               Configure local environment, will guide you...
+          create-js-project       Create a new Javascript project based on a base...
           create-magento-project  Create a new Magento project based on the...
-          create-project          Create a new project based on a base template...
+          create-php-project      Create a new PHP project based on a base...
           database                Export or import database
+          docker-compose          Execute sudo docker-compose * command
+          docker-exec             Execute sudo docker exec * command
+          docker-run              Execute sudo docker * command
+          editor                  Edit or show configuration of docker-compose.yml
           envs                    List all environments
-          exec                    Execute sudo docker exec * command
-          restart                 Restart specified docker service
-          run                     Execute sudo docker * command
+          logs                    Show or live tail docker container logs
+          restart                 Restarts all stopped and running services, or...
+          setup-docker-compose    Install or upgrade docker compose
           setup-project           Build a existing project based on existing code...
           start                   Launch docker services
           status                  List all running containers
           stop                    Stop docker services
+          switch-network          Switch network mode for a container
           upgrade                 Upgrade Shinetech Docker
           workspace               Initial workspace
         ```
         
         For the detailed usage of each command, you can use the following command to view:
         
         ```shell
@@ -103,38 +113,38 @@
         stdocker create-project --help
         ```
         
         ### Run docker command
         
         If you want to run `sudo docker *` command, you can use our command like this:
         ```shell
-        stdocker run <DOCKER_COMMAND>
+        stdocker docker-run <DOCKER_COMMAND>
         ```
         You can check `sudo docker` and see which original command we supported. Please use double quotes if `DOCKER_COMMAND` contains spaces or other parameters.
         
         e.g:
         ```shell
-        stdocker run info
+        stdocker docker-run info
         ```
         This command is equivalent to:
         ```shell
         sudo docker info
         ```
         
         ### Run docker-compose command
         
         If you want to run `sudo docker-compose *` command, you can use our command like this:
         ```shell
-        stdocker compose <DOCKER_COMPOSE_COMMAND>
+        stdocker docker-compose <DOCKER_COMPOSE_COMMAND>
         ```
         You can check `sudo docker-compose` and see which original command we supported. Please use double quotes if `DOCKER_COMPOSE_COMMAND` contains spaces or other parameters.
         
         e.g:
         ```shell
-        stdocker compose ps
+        stdocker docker-compose ps
         ```
         This command is equivalent to:
         ```shell
         sudo docker-compose ps
         ```
         You will see the following result:
         ```
@@ -155,21 +165,21 @@
         **NOTE:**
         You can also use `stdocker status` list all running docker containers.
         
         ### Run docker exec command
         
         If you want to run `sudo docker exec *` command, you can use our command like this:
         ```shell
-        stdocker exec <COMMAND>
+        stdocker docker-exec <COMMAND>
         ```
         You can check `sudo docker exec --help` and see which original command we supported. Please use double quotes if `COMMAND` contains spaces or other parameters.
         
         e.g:
         ```shell
-        stdocker exec "-it stdev_phpfpm_1 /bin/bash"
+        stdocker docker-exec "-it stdev_phpfpm_1 /bin/bash"
         ```
         This command is equivalent to:
         ```shell
         sudo docker exec -it stdev_phpfpm_1 /bin/bash
         ```
         
         ### Log in to the specified server using SSH
@@ -209,14 +219,15 @@
         
         ```shell
         stdocker restart <SERVICE>
         ```
         
         e.g:
         ```shell
+        stdocker restart # Restart all services
         stdocker restart nginx
         stdocker restart phpfpm
         ```
         
         ### Configure local environment
         
         It will guide you through creating your .env and docker-compose.yml
@@ -244,20 +255,20 @@
         ```shell
         stdocker database <ACTION{import|export}>
         ```
         
         #### Export database:
         ```shell
         stdocker database export --dbname=test
-        stdocker database export --dbname=test --backup_sql_file=test_20220823.sql
+        stdocker database export --dbname=test --backup-sql-file=test_20220823.sql
         ```
         
         #### Import database:
         ```shell
-        stdocker database import --dbname=test --backup_sql_file=test_20220823.sql
+        stdocker database import --dbname=test --backup-sql-file=test_20220823.sql
         ```
         
         ### Show the local environment and workspace information
         
         ```shell
         stdocker about
         ```
@@ -314,38 +325,42 @@
         
         ```shell
         stdocker workspace
         ```
         
         ### Create and setup project
         
-        #### Create a new project based on a base template or framework skeleton
+        #### Create a new PHP project based on a base template or framework skeleton
         
         ```shell
-        stdocker create-project [OPTIONS]
+        stdocker create-php-project [OPTIONS]
         ```
         
-        Initial a Magento 2 project:
+        Create a Magento 2 project:
         ```shell
-        stdocker create-project --platform=magento --project-name=m2project --target-version=2.4.5
+        stdocker create-php-project --platform=magento --project-name=m2project --target-version=2.4.5
         ```
         
-        Initial a Symfony project:
+        e.g:
+        
+        Create a Symfony project:
         ```shell
-        stdocker init-project --platform=symfony --project-name=sfproject
+        stdocker create-php-project --platform=symfony --project-name=sfproject
         ```
         
         #### Create a new Magento project based on the source code or composer
         
         Please download the Magento source code from the official website first if use source code to create project.
         
         ```shell
         stdocker create-magento-project [OPTIONS]
         ```
         
+        e.g:
+        
         Create a Magento 2.4.5 project with source code:
         ```shell
         stdocker create-magento-project --target-version=2.4.5 --source-code-file=/home/sunfeng/Downloads/adobe-commerce-2.4.5-2022-07-21-08-24-23.zip
         ```
         
         Create a Magento 2.4.5 project with custom project name:
         ```shell
@@ -353,14 +368,27 @@
         ```
         
         Create a Magento 2.4.5 project with composer:
         ```shell
         stdocker create-magento-project --target-version=2.4.5
         ```
         
+        #### Create a new Javascript project based on a base template or framework skeleton
+        
+        ```shell
+        stdocker create-js-project [OPTIONS]
+        ```
+        
+        e.g:
+        
+        Create a React project:
+        ```shell
+        stdocker create-js-project --platform=react --project-name=reactproject
+        ```
+        
         #### Build an existing project based on existing code and database
         
         ```shell
         stdocker setup-project [OPTIONS]
         ```
         
         Setup HP project:
@@ -380,26 +408,168 @@
         ```
         
         If you want to restart docker services after upgrade, please use the following command:
         ```shell
         stdocker upgrade --force
         ```
         
+        ### Switch network mode for a container
+        
+        ```shell
+        stdocker switch-network [OPTIONS] SERVICE
+        ```
+        
+        ```shell
+        stdocker switch-network phpfpm --network-mode=host
+        stdocker switch-network phpfpm --network-mode=bridge
+        ```
+        
+        ### Edit or show configuration of docker-compose.yml
+        
+        ```shell
+        stdocker editor [OPTIONS]
+        ```
+        
+        Show the configuration in terminal:
+        ```shell
+        stdocker editor
+        ```
+        
+        Edit the configuration via vim:
+        ```shell
+        stdocker editor --edit-mode
+        ```
+        
+        ### Show or live tail docker container logs
+        
+        ```shell
+        stdocker logs [OPTIONS] SERVICE
+        ```
+        
+        Show all logs for specified container
+        ```shell
+        stdocker logs phpfpm
+        ```
+        
+        Tail logs for specified container
+        ```shell
+        stdocker logs phpfpm --follow
+        ```
+        
+        ### Install or upgrade docker compose
+        
+        ```shell
+        stdocker setup-docker-compose [OPTIONS] [VERSION]
+        ```
+        
+        Install or upgrade to default version:
+        ```shell
+        stdocker setup-docker-compose
+        ```
+        
+        Install or upgrade to default version:
+        ```shell
+        stdocker setup-docker-compose 1.29.2
+        stdocker setup-docker-compose v2.19.1
+        ```
+        
+        **NOTE:** Find the newest version from https://github.com/docker/compose/releases
+        - v1: https://github.com/docker/compose/releases/download/1.29.2/docker-compose-Linux-x86_64
+        - v2: https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64
+        
         
         [pypi_badge]: https://badge.fury.io/py/stdocker.svg
         [pypi_link]: http://badge.fury.io/py/stdocker
         
         # Changelog
         
         All notable changes to this project will be documented in this file.
         
         The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this
         project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
         
         
+        ## [1.1.0] - 2023-06-30
+        
+        ### Added
+        
+        - Add install or upgrade docker compose command
+        
+        
+        ## [1.0.18] - 2023-05-04
+        
+        ### Fixed
+        
+        - Fix project name and directory bugs for create Magento project
+        
+        
+        ## [1.0.17] - 2023-01-17
+        
+        ### Added
+        
+        - Add Magento 2 PWA project creation support
+        
+        
+        ## [1.0.16] - 2023-01-04
+        
+        ### Added
+        
+        - Add Vue Storefront and NuxtJS project creation support
+        
+        
+        ## [1.0.15] - 2022-12-16
+        
+        ### Added
+        
+        - Improve start and stop command to support the specified services
+        
+        
+        ## [1.0.14] - 2022-12-15
+        
+        ### Added
+        
+        - Show or live tail docker container logs
+        
+        
+        ## [1.0.13] - 2022-11-18
+        
+        ### Added
+        
+        - Add switch docker container network command
+        - Add edit or show configuration of docker-compose.yml command
+        - Update command docs
+        - Build publish script
+        
+        
+        ## [1.0.12] - 2022-11-10
+        
+        ### Added
+        
+        - Add create js project command
+        - Rebuild restart command for restarts all stopped and running services
+        
+        
+        ## [1.0.11] - 2022-11-04
+        
+        ### Added
+        
+        - Add Webgrind to env list
+        
+        ### Fixed
+        
+        - Fix yes or no display issue for env list
+        
+        ## [1.0.10] - 2022-09-13
+        
+        ### Added
+        
+        - Add CakePHP, CodeIgniter and Drupal project creation
+        - Fix bugs and adjust warning message color
+        
+        
         ## [1.0.9] - 2022-09-09
         
         ### Added
         
         - Rebuild create and setup project command
         - Update project creation parameters
         - Add composer auth.json in about command
```

### Comparing `stdocker-1.0.9/README.md` & `stdocker-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -18,28 +18,33 @@
   * [Export and import database](#export-and-import-database)
     * [Export database](#export-database)
     * [Import database](#import-database)
   * [Show the local environment and workspace information](#show-the-local-environment-and-workspace-information)
   * [List all environments](#list-all-environments)
   * [Initial workspace](#initial-workspace)
   * [Create and setup project](#create-and-setup-project)
-    * [Create a new project based on a base template or framework skeleton](#create-a-new-project-based-on-a-base-template-or-framework-skeleton)
-    * [Create a new Magento project based on the source code or composer](#create-a-new-Magento-project-based-on-the-source-code-or-composer)
+    * [Create a new PHP project based on a base template or framework skeleton](#create-a-new-php-project-based-on-a-base-template-or-framework-skeleton)
+    * [Create a new Magento project based on the source code or composer](#create-a-new-magento-project-based-on-the-source-code-or-composer)
+    * [Create a new Javascript project based on a base template or framework skeleton](#create-a-new-javascript-project-based-on-a-base-template-or-framework-skeleton)
     * [Build an existing project based on existing code and database](#build-an-existing-project-based-on-existing-code-and-database)
   * [Upgrade Shinetech Docker](#upgrade-shinetech-docker)
+  * [Switch network mode for a container](#switch-network-mode-for-a-container)
+  * [Edit or show configuration of docker-compose.yml](#edit-or-show-configuration-of-docker-compose-yml)
+  * [Show or live tail docker container logs](#show-or-live-tail-docker-container-logs)
+  * [Install or upgrade docker compose](#install-or-upgrade-docker-compose)
 
 ## Getting Started
 
 ```shell
-pip3 install stdocker
+sudo pip3 install stdocker
 ```
 
 If you get error `ERROR: Could not find a version that satisfies the requirement`, please use the following command to install:
 ```shell
-python3 -m pip install stdocker==1.0.9
+python3 -m pip install stdocker==1.1.0
 ```
 
 It based on the internal docker project `Shinetech Docker`, please install it first. If you do not have permission to use Shinetech Docker, please ignore this package.
 
 After the installation is successful, you can run the `stdocker` command in any directory and perform the operations you need.
 
 ## Use Cases
@@ -64,27 +69,32 @@
   --version               Show the version and exit.
   --help                  Show this message and exit.
 
 Commands:
   about                   Show the local environment and workspace...
   bash                    Bash session for running container
   build                   Build local development environment with your...
-  compose                 Execute sudo docker-compose * command
   configure               Configure local environment, will guide you...
+  create-js-project       Create a new Javascript project based on a base...
   create-magento-project  Create a new Magento project based on the...
-  create-project          Create a new project based on a base template...
+  create-php-project      Create a new PHP project based on a base...
   database                Export or import database
+  docker-compose          Execute sudo docker-compose * command
+  docker-exec             Execute sudo docker exec * command
+  docker-run              Execute sudo docker * command
+  editor                  Edit or show configuration of docker-compose.yml
   envs                    List all environments
-  exec                    Execute sudo docker exec * command
-  restart                 Restart specified docker service
-  run                     Execute sudo docker * command
+  logs                    Show or live tail docker container logs
+  restart                 Restarts all stopped and running services, or...
+  setup-docker-compose    Install or upgrade docker compose
   setup-project           Build a existing project based on existing code...
   start                   Launch docker services
   status                  List all running containers
   stop                    Stop docker services
+  switch-network          Switch network mode for a container
   upgrade                 Upgrade Shinetech Docker
   workspace               Initial workspace
 ```
 
 For the detailed usage of each command, you can use the following command to view:
 
 ```shell
@@ -95,38 +105,38 @@
 stdocker create-project --help
 ```
 
 ### Run docker command
 
 If you want to run `sudo docker *` command, you can use our command like this:
 ```shell
-stdocker run <DOCKER_COMMAND>
+stdocker docker-run <DOCKER_COMMAND>
 ```
 You can check `sudo docker` and see which original command we supported. Please use double quotes if `DOCKER_COMMAND` contains spaces or other parameters.
 
 e.g:
 ```shell
-stdocker run info
+stdocker docker-run info
 ```
 This command is equivalent to:
 ```shell
 sudo docker info
 ```
 
 ### Run docker-compose command
 
 If you want to run `sudo docker-compose *` command, you can use our command like this:
 ```shell
-stdocker compose <DOCKER_COMPOSE_COMMAND>
+stdocker docker-compose <DOCKER_COMPOSE_COMMAND>
 ```
 You can check `sudo docker-compose` and see which original command we supported. Please use double quotes if `DOCKER_COMPOSE_COMMAND` contains spaces or other parameters.
 
 e.g:
 ```shell
-stdocker compose ps
+stdocker docker-compose ps
 ```
 This command is equivalent to:
 ```shell
 sudo docker-compose ps
 ```
 You will see the following result:
 ```
@@ -147,21 +157,21 @@
 **NOTE:**
 You can also use `stdocker status` list all running docker containers.
 
 ### Run docker exec command
 
 If you want to run `sudo docker exec *` command, you can use our command like this:
 ```shell
-stdocker exec <COMMAND>
+stdocker docker-exec <COMMAND>
 ```
 You can check `sudo docker exec --help` and see which original command we supported. Please use double quotes if `COMMAND` contains spaces or other parameters.
 
 e.g:
 ```shell
-stdocker exec "-it stdev_phpfpm_1 /bin/bash"
+stdocker docker-exec "-it stdev_phpfpm_1 /bin/bash"
 ```
 This command is equivalent to:
 ```shell
 sudo docker exec -it stdev_phpfpm_1 /bin/bash
 ```
 
 ### Log in to the specified server using SSH
@@ -201,14 +211,15 @@
 
 ```shell
 stdocker restart <SERVICE>
 ```
 
 e.g:
 ```shell
+stdocker restart # Restart all services
 stdocker restart nginx
 stdocker restart phpfpm
 ```
 
 ### Configure local environment
 
 It will guide you through creating your .env and docker-compose.yml
@@ -236,20 +247,20 @@
 ```shell
 stdocker database <ACTION{import|export}>
 ```
 
 #### Export database:
 ```shell
 stdocker database export --dbname=test
-stdocker database export --dbname=test --backup_sql_file=test_20220823.sql
+stdocker database export --dbname=test --backup-sql-file=test_20220823.sql
 ```
 
 #### Import database:
 ```shell
-stdocker database import --dbname=test --backup_sql_file=test_20220823.sql
+stdocker database import --dbname=test --backup-sql-file=test_20220823.sql
 ```
 
 ### Show the local environment and workspace information
 
 ```shell
 stdocker about
 ```
@@ -306,38 +317,42 @@
 
 ```shell
 stdocker workspace
 ```
 
 ### Create and setup project
 
-#### Create a new project based on a base template or framework skeleton
+#### Create a new PHP project based on a base template or framework skeleton
 
 ```shell
-stdocker create-project [OPTIONS]
+stdocker create-php-project [OPTIONS]
 ```
 
-Initial a Magento 2 project:
+Create a Magento 2 project:
 ```shell
-stdocker create-project --platform=magento --project-name=m2project --target-version=2.4.5
+stdocker create-php-project --platform=magento --project-name=m2project --target-version=2.4.5
 ```
 
-Initial a Symfony project:
+e.g:
+
+Create a Symfony project:
 ```shell
-stdocker init-project --platform=symfony --project-name=sfproject
+stdocker create-php-project --platform=symfony --project-name=sfproject
 ```
 
 #### Create a new Magento project based on the source code or composer
 
 Please download the Magento source code from the official website first if use source code to create project.
 
 ```shell
 stdocker create-magento-project [OPTIONS]
 ```
 
+e.g:
+
 Create a Magento 2.4.5 project with source code:
 ```shell
 stdocker create-magento-project --target-version=2.4.5 --source-code-file=/home/sunfeng/Downloads/adobe-commerce-2.4.5-2022-07-21-08-24-23.zip
 ```
 
 Create a Magento 2.4.5 project with custom project name:
 ```shell
@@ -345,14 +360,27 @@
 ```
 
 Create a Magento 2.4.5 project with composer:
 ```shell
 stdocker create-magento-project --target-version=2.4.5
 ```
 
+#### Create a new Javascript project based on a base template or framework skeleton
+
+```shell
+stdocker create-js-project [OPTIONS]
+```
+
+e.g:
+
+Create a React project:
+```shell
+stdocker create-js-project --platform=react --project-name=reactproject
+```
+
 #### Build an existing project based on existing code and database
 
 ```shell
 stdocker setup-project [OPTIONS]
 ```
 
 Setup HP project:
@@ -372,10 +400,74 @@
 ```
 
 If you want to restart docker services after upgrade, please use the following command:
 ```shell
 stdocker upgrade --force
 ```
 
+### Switch network mode for a container
+
+```shell
+stdocker switch-network [OPTIONS] SERVICE
+```
+
+```shell
+stdocker switch-network phpfpm --network-mode=host
+stdocker switch-network phpfpm --network-mode=bridge
+```
+
+### Edit or show configuration of docker-compose.yml
+
+```shell
+stdocker editor [OPTIONS]
+```
+
+Show the configuration in terminal:
+```shell
+stdocker editor
+```
+
+Edit the configuration via vim:
+```shell
+stdocker editor --edit-mode
+```
+
+### Show or live tail docker container logs
+
+```shell
+stdocker logs [OPTIONS] SERVICE
+```
+
+Show all logs for specified container
+```shell
+stdocker logs phpfpm
+```
+
+Tail logs for specified container
+```shell
+stdocker logs phpfpm --follow
+```
+
+### Install or upgrade docker compose
+
+```shell
+stdocker setup-docker-compose [OPTIONS] [VERSION]
+```
+
+Install or upgrade to default version:
+```shell
+stdocker setup-docker-compose
+```
+
+Install or upgrade to default version:
+```shell
+stdocker setup-docker-compose 1.29.2
+stdocker setup-docker-compose v2.19.1
+```
+
+**NOTE:** Find the newest version from https://github.com/docker/compose/releases
+- v1: https://github.com/docker/compose/releases/download/1.29.2/docker-compose-Linux-x86_64
+- v2: https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64
+
 
 [pypi_badge]: https://badge.fury.io/py/stdocker.svg
 [pypi_link]: http://badge.fury.io/py/stdocker
```

### Comparing `stdocker-1.0.9/setup.py` & `stdocker-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `stdocker-1.0.9/stdocker/cli.py` & `stdocker-1.1.0/stdocker/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,16 +12,17 @@
                      'Run pip3 install "stdocker[cli]" to fix this.')
     sys.exit(1)
 
 from .version import __version__
 from .config import install_dir
 from .config import current_dir
 from .config import base_domain
-from .config import platforms
+from .config import php_platforms, js_platforms, js_languages
 from .config import projects
+from .config import network_modes
 
 
 """
 Check if project name is valid
 """
 def check_project_name(ctx, param, value):
     if not param.required and value is None:
@@ -36,55 +37,89 @@
     return value
 
 
 @click.group()
 @click.option('-d', '--working-dir', default=install_dir,
               type=click.Path(dir_okay=True),
               help="Location of the installation directory, defaults to " + install_dir + ".")
-@click.version_option(version=__version__)
+@click.version_option(version=__version__, prog_name='Shinetech Docker CLI')
 @click.pass_context
 def cli(ctx: click.Context, working_dir: Any) -> None:
     """Shinetech Docker CLI"""
     ctx.obj = {}
     ctx.obj['WORKING_DIR'] = working_dir
     ctx.obj['CURRENT_DIR'] = current_dir
     # All scripts will based on working dir to run
     os.chdir(working_dir)  # Debug directory: /var/www/html/Shinetech/shinetech-docker
 
 
 @cli.command()
 @click.pass_context
 @click.argument('command', required=True)
-def run(ctx: click.Context, command: Any) -> None:
+def docker_run(ctx: click.Context, command: Any) -> None:
     """Execute sudo docker * command"""
     os.system('sudo docker ' + command)
 
 
 @cli.command()
 @click.pass_context
 @click.argument('command', required=True)
-def exec(ctx: click.Context, command: Any) -> None:
+def docker_exec(ctx: click.Context, command: Any) -> None:
     """Execute sudo docker exec * command"""
     os.system('sudo docker exec ' + command)
 
 
 @cli.command()
 @click.pass_context
 @click.argument('command', required=True)
-def compose(ctx: click.Context, command: Any) -> None:
+def docker_compose(ctx: click.Context, command: Any) -> None:
     """Execute sudo docker-compose * command"""
     os.system('sudo docker-compose ' + command)
 
 
 @cli.command()
 @click.pass_context
-@click.argument('service', required=True)
+@click.argument('service', required=False)
+def start(ctx: click.Context, service: Any) -> None:
+    """Launch docker services"""
+    if service:
+        # https://docs.docker.com/engine/reference/commandline/compose_start/
+        os.system('sudo docker-compose start ' + service)
+    else:
+        click.echo(click.style(f"Start docker services", fg='green'))
+        os.system('bash bin/launch.sh')
+
+
+@cli.command()
+@click.pass_context
+@click.argument('service', required=False)
+def stop(ctx: click.Context, service: Any) -> None:
+    """Stop docker services"""
+    if service:
+        # https://docs.docker.com/engine/reference/commandline/compose_stop/
+        os.system('sudo docker-compose stop ' + service)
+    else:
+        click.echo(click.style(f"Stop docker services", fg='green'))
+        os.system('bash bin/stop.sh')
+
+
+@cli.command()
+@click.pass_context
+@click.argument('service', required=False)
 def restart(ctx: click.Context, service: Any) -> None:
-    """Restart specified docker service"""
-    os.system('sudo docker-compose restart ' + service)
+    """Restarts all stopped and running services, or the specified services only."""
+    if service:
+        # https://docs.docker.com/engine/reference/commandline/compose_restart/
+        os.system('sudo docker-compose restart ' + service)
+    else:
+        # https://stackoverflow.com/questions/38221463/command-for-restarting-all-running-docker-containers
+        # sudo docker restart $(docker ps -a -q)
+        # sudo docker restart $(docker ps -q)
+        # Restart all running containers
+        os.system('sudo docker-compose restart')
 
 
 @cli.command()
 @click.pass_context
 def configure(ctx: click.Context) -> None:
     """Configure local environment, will guide you through creating your .env and docker-compose.yml."""
     os.system('python3 install/configurator.py')
@@ -98,45 +133,29 @@
 def build(ctx: click.Context, env: Any) -> None:
     """Build local development environment with your configuration"""
     os.system('bash builder.sh ' + env)
 
 
 @cli.command()
 @click.pass_context
-def start(ctx: click.Context) -> None:
-    """Launch docker services"""
-    click.echo(click.style(f"Start to launch docker services", fg='green'))
-    os.system('bash bin/launch.sh')
-
-
-@cli.command()
-@click.pass_context
-def stop(ctx: click.Context) -> None:
-    """Stop docker services"""
-    click.echo(click.style(f"Start to stop docker services", fg='green'))
-    os.system('bash bin/stop.sh')
-
-
-@cli.command()
-@click.pass_context
 @click.option('--dbname', required=True,
               help="Specify the database name to export or import.")
 @click.option('--backup-sql-file',
               help="Specifies the backup SQL file path, "
                    "which can be used for imported source file and exported target file or directory. "
                    "The default is the specified file in the current directory.")
 @click.argument('action', type=click.Choice(['import', 'export']), required=True)
 def database(ctx: click.Context, action: Any, dbname: Any, backup_sql_file: Any) -> None:
     """Export or import database"""
     if dbname is None:
-        click.echo(click.style(f"Invalid database name", fg='red'))
+        click.echo(click.style(f"ERROR: Invalid database name", fg='red'))
         exit(1)
     if action == 'import':
         if backup_sql_file is None:
-            click.echo(click.style(f"Invalid source backup SQL file", fg='red'))
+            click.echo(click.style(f"ERROR: Invalid source backup SQL file", fg='red'))
             exit(1)
         os.system('bash bin/import_db.sh ' + dbname + ' ' + backup_sql_file + ' ' + current_dir)
     elif action == 'export':
         command = 'bash bin/export_db.sh ' + dbname + ' ' + current_dir
         if backup_sql_file is not None:
             command += ' ' + backup_sql_file
         os.system(command)
@@ -189,18 +208,18 @@
 @click.pass_context
 def about(ctx: click.Context) -> None:
     """Show the local environment and workspace information"""
     working_dir = ctx.obj['WORKING_DIR']
     env_handler = EnvHandler(working_dir=working_dir)
     env_values = env_handler.get_env_values()
 
-    click.echo(click.style(f"Current environment:", fg='yellow', bold=True))
+    click.echo(click.style(f"Current environment:", fg='green', bold=True))
     click.echo(click.style(f" - {env_values['DEFAULT_ENV']}", fg='cyan'))
 
-    click.echo(click.style(f"Your workspace information:", fg='yellow', bold=True))
+    click.echo(click.style(f"Your workspace information:", fg='green', bold=True))
     click.echo(click.style(f" - Workspace: {env_values['WORKSPACE']}", fg='cyan'))
     click.echo(
         click.style(f" - Project Directory: {env_values['DOCUMENT_ROOT']}", fg='cyan'))
     click.echo(click.style(f" - Nginx VHosts: {env_values['NGINX_VHOSTS_DIR']}", fg='cyan'))
     click.echo(click.style(f" - Nginx Log: {env_values['NGINX_LOG_DIR']}", fg='cyan'))
     click.echo(
         click.style(f" - Apache VHosts: {env_values['APACHE_VHOSTS_DIR']}", fg='cyan'))
@@ -224,93 +243,135 @@
 @cli.command()
 @click.pass_context
 @click.option('--project-name', required=True,
               type=click.Choice(projects),
               help="Specify project name.")
 @click.option('--db-sql-file', required=True,
               help="SQL backup file for initializing the database.")
+@click.option('--vendor-file', required=False,
+              help="Composer vendor file, pull from remote by default.")
 @click.option('--country', required=False,
               help="Build project by country, such as HP project have multiple independent countries and regions.")
 @click.option('--multiple-domain/--no-multiple-domain', default=False,
               help="Use multiple domains for multiple sites, single domain is used by default. "
                    "This option takes effect if --country is not empty. "
                    "e.g: For HP project, If No will use hp.dev.php9.cc for all country sites, "
                    "if Yes will use <country>.hp.dev.php9.cc for different sites.")
-def setup_project(ctx: click.Context, project_name: Any, db_sql_file: Any, country: Any, multiple_domain: Any) -> None:
+def setup_project(ctx: click.Context, project_name: Any, db_sql_file: Any, vendor_file: Any, country: Any, multiple_domain: Any) -> None:
     """Build a existing project based on existing code and database"""
     working_dir = ctx.obj['WORKING_DIR']
     env_handler = EnvHandler(working_dir=working_dir)
     env_values = env_handler.get_env_values()
     workspace_dir = env_values['WORKSPACE']
     current_env_configs = env_handler.get_current_env_configs()
     webserver = current_env_configs['services']['webserver']
 
     domain = project_name + base_domain
     if multiple_domain and country is not None:
         domain = project_name + '-' + country + base_domain
 
     project_dir = workspace_dir + '/www/' + domain
     if os.path.exists(project_dir):
-        click.echo(click.style(f"NOTE: The project directory {project_dir} already exists.", fg='cyan'))
+        click.echo(click.style(f"WARNING: The project directory {project_dir} already exists.", fg='yellow'))
         click.confirm('Do you confirm to override and create project?', abort=True)
 
     command = 'bash bin/setup_project.sh ' \
               + current_dir + ' ' + workspace_dir + ' ' + webserver + ' ' + project_name
 
     if db_sql_file is not None:
         command += ' ' + db_sql_file
     else:
         command += ' ""'
 
+    if vendor_file is not None:
+        command += ' ' + vendor_file
+    else:
+        command += ' ""'
+
     if country is not None:
         command += ' ' + country
         if multiple_domain:
             command += ' y'
         else:
             command += ' n'
 
     os.system(command)
 
 
 @cli.command()
 @click.pass_context
 @click.option('--platform', required=True, default='generic',
-              type=click.Choice(platforms),
-              help="Specifies the framework used by the project.")
+              type=click.Choice(php_platforms),
+              help="Specifies the PHP framework used by the project.")
 @click.option('--project-name', required=True,
               callback=check_project_name,
               help="Specify project name.")
 @click.option('--target-version', required=False,
               help="Specify framework version. e.g: 2.4.5, 2.4.4-p1 for Magento")
-def create_project(ctx: click.Context, platform: Any, project_name: Any, target_version: Any) -> None:
-    """Create a new project based on a base template or framework skeleton"""
+def create_php_project(ctx: click.Context, platform: Any, project_name: Any, target_version: Any) -> None:
+    """Create a new PHP project based on a base template or framework skeleton"""
     working_dir = ctx.obj['WORKING_DIR']
     env_handler = EnvHandler(working_dir=working_dir)
     env_values = env_handler.get_env_values()
     workspace_dir = env_values['WORKSPACE']
     current_env_configs = env_handler.get_current_env_configs()
     webserver = current_env_configs['services']['webserver']
 
     domain = project_name + base_domain
 
     project_dir = workspace_dir + '/www/' + domain
     if os.path.exists(project_dir):
-        click.echo(click.style(f"NOTE: The project directory {project_dir} already exists.", fg='cyan'))
+        click.echo(click.style(f"WARNING: The project directory {project_dir} already exists.", fg='yellow'))
         click.confirm('Do you confirm to override and create project?', abort=True)
 
-    command = 'bash bin/create_project.sh ' \
+    command = 'bash bin/create_php_project.sh ' \
               + current_dir + ' ' + workspace_dir + ' ' + webserver + ' ' + platform + ' ' + project_name
     if target_version is not None:
         command += ' ' + target_version
 
     os.system(command)
 
 
 @cli.command()
 @click.pass_context
+@click.option('--platform', required=True,
+              type=click.Choice(js_platforms),
+              help="Specifies the Javascript framework used by the project.")
+@click.option('--project-name', required=True,
+              callback=check_project_name,
+              help="Specify project name.")
+@click.option('--programming-language', required=False, default='javascript',
+              type=click.Choice(js_languages),
+              help="Specify programming language. e.g: JavaScript or TypeScript")
+def create_js_project(ctx: click.Context, platform: Any, project_name: Any, programming_language: Any) -> None:
+    """Create a new Javascript project based on a base template or framework skeleton"""
+    working_dir = ctx.obj['WORKING_DIR']
+    env_handler = EnvHandler(working_dir=working_dir)
+    env_values = env_handler.get_env_values()
+    workspace_dir = env_values['WORKSPACE']
+    current_env_configs = env_handler.get_current_env_configs()
+    webserver = current_env_configs['services']['webserver']
+
+    domain = project_name + base_domain
+
+    project_dir = workspace_dir + '/www/' + domain
+    if os.path.exists(project_dir):
+        click.echo(click.style(f"WARNING: The project directory {project_dir} already exists.", fg='yellow'))
+        click.confirm('Do you confirm to override and create project?', abort=True)
+
+    command = 'bash bin/create_js_project.sh ' \
+              + current_dir + ' ' + workspace_dir + ' ' + webserver + ' ' + platform + ' ' + project_name
+    if programming_language is not None:
+        command += ' ' + programming_language
+
+    os.system(command)
+
+
+@cli.command()
+@click.pass_context
 @click.option('--target-version', required=True,
               help="Specify Magento version. e.g: 2.4.5, 2.4.4-p1")
 @click.option('--source-code-file', required=False,
               help="Specify Magento original source code file. "
                    "If not specified, composer will be used for installation, "
                    "otherwise the specified source code package will be used.")
 @click.option('--project-name', required=False,
@@ -321,24 +382,24 @@
     working_dir = ctx.obj['WORKING_DIR']
     env_handler = EnvHandler(working_dir=working_dir)
     env_values = env_handler.get_env_values()
     workspace_dir = env_values['WORKSPACE']
     current_env_configs = env_handler.get_current_env_configs()
     webserver = current_env_configs['services']['webserver']
 
-    if target_version is not None:
+    if target_version is not None and project_name is None:
         # 2.4.5 > 245
         version = convert_version(target_version)
         project_name = 'm' + version  # e.g: m245
 
     project_domain = project_name + base_domain
 
     project_dir = workspace_dir + '/www/' + project_domain
     if os.path.exists(project_dir):
-        click.echo(click.style(f"NOTE: The Magento project {project_dir} already exists.", fg='cyan'))
+        click.echo(click.style(f"WARNING: The project directory {project_dir} already exists.", fg='yellow'))
         click.confirm('Do you confirm to override and create project?', abort=True)
 
     command = 'bash bin/create_magento_project.sh ' \
               + current_dir + ' ' + workspace_dir + ' ' + webserver + ' ' + project_name + ' ' + target_version
     if source_code_file is not None:
         command += ' ' + source_code_file
 
@@ -348,13 +409,64 @@
 @cli.command()
 @click.pass_context
 def status(ctx: click.Context) -> None:
     """List all running containers"""
     os.system('sudo docker-compose ps')
 
 
+@cli.command()
+@click.pass_context
+@click.argument('service', required=True)
+@click.option('--network-mode', required=False, default="bridge",
+              type=click.Choice(network_modes),
+              help="The type of network a container uses.")
+def switch_network(ctx: click.Context, service: Any, network_mode: Any) -> None:
+    """Switch network mode for a container"""
+    os.system('bash bin/switch_network.sh ' + service + ' ' + network_mode)
+
+
+@cli.command()
+@click.pass_context
+@click.option('--edit-mode/--no-edit-mode', default=False,
+              help="Edit or show configuration of docker-compose.yml")
+def editor(ctx: click.Context, edit_mode: Any) -> None:
+    """Edit or show configuration of docker-compose.yml"""
+    if edit_mode:
+        os.system('vim docker-compose.yml')
+    else:
+        os.system('cat docker-compose.yml')
+
+
+@cli.command()
+@click.pass_context
+@click.argument('service', required=True)
+@click.option('--follow/--no-follow', default=False,
+              help="To tail the logs for specified container")
+def logs(ctx: click.Context, service: Any, follow: Any) -> None:
+    """Show or live tail docker container logs"""
+    # https://docs.docker.com/engine/reference/commandline/logs/
+    # https://www.papertrail.com/solution/tips/how-to-live-tail-docker-logs/
+    # List containers by docker container ls
+    container_name = 'stdev_' + service + '_1'  # e.g: stdev_phpfpm_1
+    if follow:
+        os.system('sudo docker container logs --follow ' + container_name)
+    else:
+        os.system('sudo docker container logs ' + container_name)
+
+
+@cli.command()
+@click.pass_context
+@click.argument('version', required=False)
+def setup_docker_compose(ctx: click.Context, version: Any) -> None:
+    """Install or upgrade docker compose"""
+    if version:
+        os.system('bash bin/upgrade_docker_compose.sh ' + version)
+    else:
+        os.system('bash bin/upgrade_docker_compose.sh')
+
+
 def main():
     cli()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `stdocker-1.0.9/stdocker/env_handler.py` & `stdocker-1.1.0/stdocker/env_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,19 +123,19 @@
     def list_env_table(self):
         current_env = self.get_current_env()
         customized_envs = self.list_customized_detailed_envs()
         # env_names = self.list_customized_env_names()
         services = ['webserver', 'php', 'mysql', 'mariadb',
                     'phpmyadmin', 'elasticsearch', 'elasticvue',
                     'redis', 'phpredisadmin', 'rabbitmq', 'mailcatcher',
-                    'mongo', 'mongoexpress', 'postgres', 'pgweb', 'memcached']
+                    'mongo', 'mongoexpress', 'postgres', 'pgweb', 'memcached', 'webgrind']
         service_names = ['Web Server', 'PHP', 'MySQL', 'MariaDB',
                          'phpMyAdmin', 'Elasticsearch', 'Elasticvue',
                          'Redis', 'phpRedisAdmin', 'RabbitMQ', 'Mailcatcher',
-                         'MongoDB', 'Mongo Express', 'PostgreSQL', 'Pgweb', 'Memcached']
+                         'MongoDB', 'Mongo Express', 'PostgreSQL', 'Pgweb', 'Memcached', 'Webgrind']
 
         table = BeautifulTable(maxwidth=200)
         columns_headers = ['Env Code'] + service_names
 
         env_detail_names = []
         for item in customized_envs:
             env_detail_names.append(item['name'])
@@ -147,16 +147,18 @@
                 services_status.append(colored(env, 'red'))
             else:
                 services_status.append(env)
 
             for service in services:
                 status = 'N'
                 if service in item['services'].keys():
-                    if item['services'][service] is True:
+                    if item['services'][service] is True or item['services'][service] == 'yes':
                         status = 'Y'
+                    elif item['services'][service] is False or item['services'][service] == 'no':
+                        status = 'N'
                     else:
                         status = item['services'][service]
 
                 if env == current_env:
                     services_status.append(colored(status, 'red'))
                 else:
                     services_status.append(status)
```

### Comparing `stdocker-1.0.9/stdocker/env_parser.py` & `stdocker-1.1.0/stdocker/env_parser.py`

 * *Files identical despite different names*

### Comparing `stdocker-1.0.9/stdocker/utils.py` & `stdocker-1.1.0/stdocker/utils.py`

 * *Files identical despite different names*

### Comparing `stdocker-1.0.9/stdocker/yaml_parser.py` & `stdocker-1.1.0/stdocker/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `stdocker-1.0.9/stdocker.egg-info/PKG-INFO` & `stdocker-1.1.0/stdocker.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdocker
-Version: 1.0.9
+Version: 1.1.0
 Summary: Shinetech Docker CLI.
 Home-page: https://github.com/winds1983/stdocker
 Author: Jason Sun
 Author-email: sunf@shinetechsoftware.com
 License: MIT
 Description: # Shinetech Docker CLI
         
@@ -26,28 +26,33 @@
           * [Export and import database](#export-and-import-database)
             * [Export database](#export-database)
             * [Import database](#import-database)
           * [Show the local environment and workspace information](#show-the-local-environment-and-workspace-information)
           * [List all environments](#list-all-environments)
           * [Initial workspace](#initial-workspace)
           * [Create and setup project](#create-and-setup-project)
-            * [Create a new project based on a base template or framework skeleton](#create-a-new-project-based-on-a-base-template-or-framework-skeleton)
-            * [Create a new Magento project based on the source code or composer](#create-a-new-Magento-project-based-on-the-source-code-or-composer)
+            * [Create a new PHP project based on a base template or framework skeleton](#create-a-new-php-project-based-on-a-base-template-or-framework-skeleton)
+            * [Create a new Magento project based on the source code or composer](#create-a-new-magento-project-based-on-the-source-code-or-composer)
+            * [Create a new Javascript project based on a base template or framework skeleton](#create-a-new-javascript-project-based-on-a-base-template-or-framework-skeleton)
             * [Build an existing project based on existing code and database](#build-an-existing-project-based-on-existing-code-and-database)
           * [Upgrade Shinetech Docker](#upgrade-shinetech-docker)
+          * [Switch network mode for a container](#switch-network-mode-for-a-container)
+          * [Edit or show configuration of docker-compose.yml](#edit-or-show-configuration-of-docker-compose-yml)
+          * [Show or live tail docker container logs](#show-or-live-tail-docker-container-logs)
+          * [Install or upgrade docker compose](#install-or-upgrade-docker-compose)
         
         ## Getting Started
         
         ```shell
-        pip3 install stdocker
+        sudo pip3 install stdocker
         ```
         
         If you get error `ERROR: Could not find a version that satisfies the requirement`, please use the following command to install:
         ```shell
-        python3 -m pip install stdocker==1.0.9
+        python3 -m pip install stdocker==1.1.0
         ```
         
         It based on the internal docker project `Shinetech Docker`, please install it first. If you do not have permission to use Shinetech Docker, please ignore this package.
         
         After the installation is successful, you can run the `stdocker` command in any directory and perform the operations you need.
         
         ## Use Cases
@@ -72,27 +77,32 @@
           --version               Show the version and exit.
           --help                  Show this message and exit.
         
         Commands:
           about                   Show the local environment and workspace...
           bash                    Bash session for running container
           build                   Build local development environment with your...
-          compose                 Execute sudo docker-compose * command
           configure               Configure local environment, will guide you...
+          create-js-project       Create a new Javascript project based on a base...
           create-magento-project  Create a new Magento project based on the...
-          create-project          Create a new project based on a base template...
+          create-php-project      Create a new PHP project based on a base...
           database                Export or import database
+          docker-compose          Execute sudo docker-compose * command
+          docker-exec             Execute sudo docker exec * command
+          docker-run              Execute sudo docker * command
+          editor                  Edit or show configuration of docker-compose.yml
           envs                    List all environments
-          exec                    Execute sudo docker exec * command
-          restart                 Restart specified docker service
-          run                     Execute sudo docker * command
+          logs                    Show or live tail docker container logs
+          restart                 Restarts all stopped and running services, or...
+          setup-docker-compose    Install or upgrade docker compose
           setup-project           Build a existing project based on existing code...
           start                   Launch docker services
           status                  List all running containers
           stop                    Stop docker services
+          switch-network          Switch network mode for a container
           upgrade                 Upgrade Shinetech Docker
           workspace               Initial workspace
         ```
         
         For the detailed usage of each command, you can use the following command to view:
         
         ```shell
@@ -103,38 +113,38 @@
         stdocker create-project --help
         ```
         
         ### Run docker command
         
         If you want to run `sudo docker *` command, you can use our command like this:
         ```shell
-        stdocker run <DOCKER_COMMAND>
+        stdocker docker-run <DOCKER_COMMAND>
         ```
         You can check `sudo docker` and see which original command we supported. Please use double quotes if `DOCKER_COMMAND` contains spaces or other parameters.
         
         e.g:
         ```shell
-        stdocker run info
+        stdocker docker-run info
         ```
         This command is equivalent to:
         ```shell
         sudo docker info
         ```
         
         ### Run docker-compose command
         
         If you want to run `sudo docker-compose *` command, you can use our command like this:
         ```shell
-        stdocker compose <DOCKER_COMPOSE_COMMAND>
+        stdocker docker-compose <DOCKER_COMPOSE_COMMAND>
         ```
         You can check `sudo docker-compose` and see which original command we supported. Please use double quotes if `DOCKER_COMPOSE_COMMAND` contains spaces or other parameters.
         
         e.g:
         ```shell
-        stdocker compose ps
+        stdocker docker-compose ps
         ```
         This command is equivalent to:
         ```shell
         sudo docker-compose ps
         ```
         You will see the following result:
         ```
@@ -155,21 +165,21 @@
         **NOTE:**
         You can also use `stdocker status` list all running docker containers.
         
         ### Run docker exec command
         
         If you want to run `sudo docker exec *` command, you can use our command like this:
         ```shell
-        stdocker exec <COMMAND>
+        stdocker docker-exec <COMMAND>
         ```
         You can check `sudo docker exec --help` and see which original command we supported. Please use double quotes if `COMMAND` contains spaces or other parameters.
         
         e.g:
         ```shell
-        stdocker exec "-it stdev_phpfpm_1 /bin/bash"
+        stdocker docker-exec "-it stdev_phpfpm_1 /bin/bash"
         ```
         This command is equivalent to:
         ```shell
         sudo docker exec -it stdev_phpfpm_1 /bin/bash
         ```
         
         ### Log in to the specified server using SSH
@@ -209,14 +219,15 @@
         
         ```shell
         stdocker restart <SERVICE>
         ```
         
         e.g:
         ```shell
+        stdocker restart # Restart all services
         stdocker restart nginx
         stdocker restart phpfpm
         ```
         
         ### Configure local environment
         
         It will guide you through creating your .env and docker-compose.yml
@@ -244,20 +255,20 @@
         ```shell
         stdocker database <ACTION{import|export}>
         ```
         
         #### Export database:
         ```shell
         stdocker database export --dbname=test
-        stdocker database export --dbname=test --backup_sql_file=test_20220823.sql
+        stdocker database export --dbname=test --backup-sql-file=test_20220823.sql
         ```
         
         #### Import database:
         ```shell
-        stdocker database import --dbname=test --backup_sql_file=test_20220823.sql
+        stdocker database import --dbname=test --backup-sql-file=test_20220823.sql
         ```
         
         ### Show the local environment and workspace information
         
         ```shell
         stdocker about
         ```
@@ -314,38 +325,42 @@
         
         ```shell
         stdocker workspace
         ```
         
         ### Create and setup project
         
-        #### Create a new project based on a base template or framework skeleton
+        #### Create a new PHP project based on a base template or framework skeleton
         
         ```shell
-        stdocker create-project [OPTIONS]
+        stdocker create-php-project [OPTIONS]
         ```
         
-        Initial a Magento 2 project:
+        Create a Magento 2 project:
         ```shell
-        stdocker create-project --platform=magento --project-name=m2project --target-version=2.4.5
+        stdocker create-php-project --platform=magento --project-name=m2project --target-version=2.4.5
         ```
         
-        Initial a Symfony project:
+        e.g:
+        
+        Create a Symfony project:
         ```shell
-        stdocker init-project --platform=symfony --project-name=sfproject
+        stdocker create-php-project --platform=symfony --project-name=sfproject
         ```
         
         #### Create a new Magento project based on the source code or composer
         
         Please download the Magento source code from the official website first if use source code to create project.
         
         ```shell
         stdocker create-magento-project [OPTIONS]
         ```
         
+        e.g:
+        
         Create a Magento 2.4.5 project with source code:
         ```shell
         stdocker create-magento-project --target-version=2.4.5 --source-code-file=/home/sunfeng/Downloads/adobe-commerce-2.4.5-2022-07-21-08-24-23.zip
         ```
         
         Create a Magento 2.4.5 project with custom project name:
         ```shell
@@ -353,14 +368,27 @@
         ```
         
         Create a Magento 2.4.5 project with composer:
         ```shell
         stdocker create-magento-project --target-version=2.4.5
         ```
         
+        #### Create a new Javascript project based on a base template or framework skeleton
+        
+        ```shell
+        stdocker create-js-project [OPTIONS]
+        ```
+        
+        e.g:
+        
+        Create a React project:
+        ```shell
+        stdocker create-js-project --platform=react --project-name=reactproject
+        ```
+        
         #### Build an existing project based on existing code and database
         
         ```shell
         stdocker setup-project [OPTIONS]
         ```
         
         Setup HP project:
@@ -380,26 +408,168 @@
         ```
         
         If you want to restart docker services after upgrade, please use the following command:
         ```shell
         stdocker upgrade --force
         ```
         
+        ### Switch network mode for a container
+        
+        ```shell
+        stdocker switch-network [OPTIONS] SERVICE
+        ```
+        
+        ```shell
+        stdocker switch-network phpfpm --network-mode=host
+        stdocker switch-network phpfpm --network-mode=bridge
+        ```
+        
+        ### Edit or show configuration of docker-compose.yml
+        
+        ```shell
+        stdocker editor [OPTIONS]
+        ```
+        
+        Show the configuration in terminal:
+        ```shell
+        stdocker editor
+        ```
+        
+        Edit the configuration via vim:
+        ```shell
+        stdocker editor --edit-mode
+        ```
+        
+        ### Show or live tail docker container logs
+        
+        ```shell
+        stdocker logs [OPTIONS] SERVICE
+        ```
+        
+        Show all logs for specified container
+        ```shell
+        stdocker logs phpfpm
+        ```
+        
+        Tail logs for specified container
+        ```shell
+        stdocker logs phpfpm --follow
+        ```
+        
+        ### Install or upgrade docker compose
+        
+        ```shell
+        stdocker setup-docker-compose [OPTIONS] [VERSION]
+        ```
+        
+        Install or upgrade to default version:
+        ```shell
+        stdocker setup-docker-compose
+        ```
+        
+        Install or upgrade to default version:
+        ```shell
+        stdocker setup-docker-compose 1.29.2
+        stdocker setup-docker-compose v2.19.1
+        ```
+        
+        **NOTE:** Find the newest version from https://github.com/docker/compose/releases
+        - v1: https://github.com/docker/compose/releases/download/1.29.2/docker-compose-Linux-x86_64
+        - v2: https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64
+        
         
         [pypi_badge]: https://badge.fury.io/py/stdocker.svg
         [pypi_link]: http://badge.fury.io/py/stdocker
         
         # Changelog
         
         All notable changes to this project will be documented in this file.
         
         The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this
         project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
         
         
+        ## [1.1.0] - 2023-06-30
+        
+        ### Added
+        
+        - Add install or upgrade docker compose command
+        
+        
+        ## [1.0.18] - 2023-05-04
+        
+        ### Fixed
+        
+        - Fix project name and directory bugs for create Magento project
+        
+        
+        ## [1.0.17] - 2023-01-17
+        
+        ### Added
+        
+        - Add Magento 2 PWA project creation support
+        
+        
+        ## [1.0.16] - 2023-01-04
+        
+        ### Added
+        
+        - Add Vue Storefront and NuxtJS project creation support
+        
+        
+        ## [1.0.15] - 2022-12-16
+        
+        ### Added
+        
+        - Improve start and stop command to support the specified services
+        
+        
+        ## [1.0.14] - 2022-12-15
+        
+        ### Added
+        
+        - Show or live tail docker container logs
+        
+        
+        ## [1.0.13] - 2022-11-18
+        
+        ### Added
+        
+        - Add switch docker container network command
+        - Add edit or show configuration of docker-compose.yml command
+        - Update command docs
+        - Build publish script
+        
+        
+        ## [1.0.12] - 2022-11-10
+        
+        ### Added
+        
+        - Add create js project command
+        - Rebuild restart command for restarts all stopped and running services
+        
+        
+        ## [1.0.11] - 2022-11-04
+        
+        ### Added
+        
+        - Add Webgrind to env list
+        
+        ### Fixed
+        
+        - Fix yes or no display issue for env list
+        
+        ## [1.0.10] - 2022-09-13
+        
+        ### Added
+        
+        - Add CakePHP, CodeIgniter and Drupal project creation
+        - Fix bugs and adjust warning message color
+        
+        
         ## [1.0.9] - 2022-09-09
         
         ### Added
         
         - Rebuild create and setup project command
         - Update project creation parameters
         - Add composer auth.json in about command
```

