# Comparing `tmp/dbm-agent-8.33.8.tar.gz` & `tmp/dbm-agent-8.33.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbm-agent-8.33.8.tar", last modified: Sat May 20 14:38:38 2023, max compression
+gzip compressed data, was "dbm-agent-8.33.9.tar", last modified: Sat May 27 07:31:59 2023, max compression
```

## Comparing `dbm-agent-8.33.8.tar` & `dbm-agent-8.33.9.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.522565 dbm-agent-8.33.8/
--rw-r--r--   0 root         (0) root         (0)      626 2023-05-20 14:38:38.522565 dbm-agent-8.33.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4453 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.497565 dbm-agent-8.33.8/bin/
--rw-r--r--   0 root         (0) root         (0)      898 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/bin/dbm-agent
--rw-r--r--   0 root         (0) root         (0)      322 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/bin/dbm-bt-conn-stack
--rw-r--r--   0 root         (0) root         (0)      794 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/bin/dbma-cli-init
--rw-r--r--   0 root         (0) root         (0)     2613 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/bin/dbma-cli-mysql
--rw-r--r--   0 root         (0) root         (0)     2267 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/bin/dbma-cli-redis
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.499565 dbm-agent-8.33.8/dbm_agent.egg-info/
--rw-r--r--   0 root         (0) root         (0)      626 2023-05-20 14:38:38.000000 dbm-agent-8.33.8/dbm_agent.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2989 2023-05-20 14:38:38.000000 dbm-agent-8.33.8/dbm_agent.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-20 14:38:38.000000 dbm-agent-8.33.8/dbm_agent.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-20 14:38:38.000000 dbm-agent-8.33.8/dbm_agent.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-20 14:38:38.000000 dbm-agent-8.33.8/dbm_agent.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.499565 dbm-agent-8.33.8/dbma/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.501565 dbm-agent-8.33.8/dbma/bil/
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/bil/__init__.py
--rw-r--r--   0 root         (0) root         (0)      411 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/bil/cmdexecutor.py
--rw-r--r--   0 root         (0) root         (0)     3740 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/bil/daemon.py
--rw-r--r--   0 root         (0) root         (0)     2527 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/bil/fs.py
--rw-r--r--   0 root         (0) root         (0)      225 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/bil/fun.py
--rw-r--r--   0 root         (0) root         (0)      700 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/bil/net.py
--rw-r--r--   0 root         (0) root         (0)     6795 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/bil/osuser.py
--rw-r--r--   0 root         (0) root         (0)      542 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/bil/sudos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.502565 dbm-agent-8.33.8/dbma/components/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.504565 dbm-agent-8.33.8/dbma/components/mysql/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.505565 dbm-agent-8.33.8/dbma/components/mysql/backups/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/backups/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/backups/cloneplugin.py
--rw-r--r--   0 root         (0) root         (0)     5674 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/commons.py
--rw-r--r--   0 root         (0) root         (0)    21072 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/config.py
--rw-r--r--   0 root         (0) root         (0)      517 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    15167 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/install.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/instance.py
--rw-r--r--   0 root         (0) root         (0)     3996 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/replica.py
--rw-r--r--   0 root         (0) root         (0)     1134 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.506565 dbm-agent-8.33.8/dbma/components/mysql/views/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/views/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13670 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/views/defaultsview.py
--rw-r--r--   0 root         (0) root         (0)     4375 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/views/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.506565 dbm-agent-8.33.8/dbma/components/orchestrator/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/orchestrator/__init__.py
--rw-r--r--   0 root         (0) root         (0)      326 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/orchestrator/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2907 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/orchestrator/install.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.509565 dbm-agent-8.33.8/dbma/components/redis/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1561 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/redis/commons.py
--rw-r--r--   0 root         (0) root         (0)     2778 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/redis/config.py
--rw-r--r--   0 root         (0) root         (0)      550 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/redis/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     7308 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/redis/install.py
--rw-r--r--   0 root         (0) root         (0)     2312 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/redis/systemd.py
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/redis/uninstall.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.512565 dbm-agent-8.33.8/dbma/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.512565 dbm-agent-8.33.8/dbma/core/agent/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/agent/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3462 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/agent/init.py
--rw-r--r--   0 root         (0) root         (0)      117 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/agent/upgrade.py
--rw-r--r--   0 root         (0) root         (0)     3679 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/configs.py
--rw-r--r--   0 root         (0) root         (0)      739 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/exception.py
--rw-r--r--   0 root         (0) root         (0)     3471 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/httpserver.py
--rw-r--r--   0 root         (0) root         (0)      829 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/messages.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/router.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.513565 dbm-agent-8.33.8/dbma/core/threads/
--rw-r--r--   0 root         (0) root         (0)       90 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/threads/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1987 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/threads/backends.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.513565 dbm-agent-8.33.8/dbma/core/views/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/views/__init__.py
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/views/dbmagentview.py
--rw-r--r--   0 root         (0) root         (0)      466 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/views/response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.495565 dbm-agent-8.33.8/dbma/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.521565 dbm-agent-8.33.8/dbma/static/cnfs/
--rw-r--r--   0 root         (0) root         (0)     1396 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/auto-inseption-db.sql
--rw-r--r--   0 root         (0) root         (0)      168 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/create-innodb-cluster.js
--rw-r--r--   0 root         (0) root         (0)      286 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/dbm-backup-proxyd.service.jinja
--rw-r--r--   0 root         (0) root         (0)      385 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/dbm-monitor-gatewayd.service.jinja
--rw-r--r--   0 root         (0) root         (0)      514 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/init-5.7.x.sql
--rw-r--r--   0 root         (0) root         (0)     1370 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/init-8.0.x.sql
--rw-r--r--   0 root         (0) root         (0)     6681 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/init-users.sql.jinja
--rw-r--r--   0 root         (0) root         (0)    10688 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-5.7-init-only.jinja
--rw-r--r--   0 root         (0) root         (0)    10850 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-5.7.25.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    14664 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0-init-only.jinja
--rw-r--r--   0 root         (0) root         (0)    17621 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.17.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17631 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.18.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17687 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.19.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17766 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.20.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17766 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.21.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.22.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.23.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.25.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.26.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17528 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.27.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17528 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.28.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17528 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.29.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17799 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.30.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    18787 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.31.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    18776 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.32.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    18774 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.33.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)      465 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysqld.service.jinja
--rw-r--r--   0 root         (0) root         (0)      681 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/redis.conf.jinja
--rw-r--r--   0 root         (0) root         (0)      710 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/redisd.service.jinja
--rw-r--r--   0 root         (0) root         (0)      362 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/zabbix-agentd.service
--rw-r--r--   0 root         (0) root         (0)    10464 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/zabbix_agentd.conf.jinja
--rw-r--r--   0 root         (0) root         (0)      258 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/zoo.cnf.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.521565 dbm-agent-8.33.8/dbma/static/sql-scripts/
--rw-r--r--   0 root         (0) root         (0)     9468 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/sql-scripts/常用SQL.md
--rw-r--r--   0 root         (0) root         (0)      346 2023-05-20 14:37:15.000000 dbm-agent-8.33.8/dbma/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-20 14:38:38.522565 dbm-agent-8.33.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1950 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.973061 dbm-agent-8.33.9/
+-rw-r--r--   0 root         (0) root         (0)      626 2023-05-27 07:31:59.972061 dbm-agent-8.33.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4453 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.937062 dbm-agent-8.33.9/bin/
+-rw-r--r--   0 root         (0) root         (0)      923 2023-05-27 07:30:06.000000 dbm-agent-8.33.9/bin/dbm-agent
+-rw-r--r--   0 root         (0) root         (0)      322 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/bin/dbm-bt-conn-stack
+-rw-r--r--   0 root         (0) root         (0)      817 2023-05-27 07:29:36.000000 dbm-agent-8.33.9/bin/dbma-cli-init
+-rw-r--r--   0 root         (0) root         (0)     2636 2023-05-27 07:29:33.000000 dbm-agent-8.33.9/bin/dbma-cli-mysql
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-05-27 07:29:31.000000 dbm-agent-8.33.9/bin/dbma-cli-redis
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.939062 dbm-agent-8.33.9/dbm_agent.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      626 2023-05-27 07:31:59.000000 dbm-agent-8.33.9/dbm_agent.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2989 2023-05-27 07:31:59.000000 dbm-agent-8.33.9/dbm_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-27 07:31:59.000000 dbm-agent-8.33.9/dbm_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-27 07:31:59.000000 dbm-agent-8.33.9/dbm_agent.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-27 07:31:59.000000 dbm-agent-8.33.9/dbm_agent.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.939062 dbm-agent-8.33.9/dbma/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.941062 dbm-agent-8.33.9/dbma/bil/
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/bil/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/bil/cmdexecutor.py
+-rw-r--r--   0 root         (0) root         (0)     3764 2023-05-27 07:30:34.000000 dbm-agent-8.33.9/dbma/bil/daemon.py
+-rw-r--r--   0 root         (0) root         (0)     2527 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/bil/fs.py
+-rw-r--r--   0 root         (0) root         (0)      223 2023-05-27 07:30:39.000000 dbm-agent-8.33.9/dbma/bil/fun.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/bil/net.py
+-rw-r--r--   0 root         (0) root         (0)     6795 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/bil/osuser.py
+-rw-r--r--   0 root         (0) root         (0)      542 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/bil/sudos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.942062 dbm-agent-8.33.9/dbma/components/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/components/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.944062 dbm-agent-8.33.9/dbma/components/mysql/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/components/mysql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.944062 dbm-agent-8.33.9/dbma/components/mysql/backups/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/components/mysql/backups/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-05-27 07:26:51.000000 dbm-agent-8.33.9/dbma/components/mysql/backups/cloneplugin.py
+-rw-r--r--   0 root         (0) root         (0)     5673 2023-05-27 07:25:58.000000 dbm-agent-8.33.9/dbma/components/mysql/commons.py
+-rw-r--r--   0 root         (0) root         (0)    21071 2023-05-27 07:26:05.000000 dbm-agent-8.33.9/dbma/components/mysql/config.py
+-rw-r--r--   0 root         (0) root         (0)      515 2023-05-27 07:26:09.000000 dbm-agent-8.33.9/dbma/components/mysql/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    15232 2023-05-27 07:26:14.000000 dbm-agent-8.33.9/dbma/components/mysql/install.py
+-rw-r--r--   0 root         (0) root         (0)      644 2023-05-27 07:26:20.000000 dbm-agent-8.33.9/dbma/components/mysql/instance.py
+-rw-r--r--   0 root         (0) root         (0)     3994 2023-05-27 07:26:23.000000 dbm-agent-8.33.9/dbma/components/mysql/replica.py
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-05-27 07:26:29.000000 dbm-agent-8.33.9/dbma/components/mysql/source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.945062 dbm-agent-8.33.9/dbma/components/mysql/views/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/components/mysql/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13668 2023-05-27 07:26:38.000000 dbm-agent-8.33.9/dbma/components/mysql/views/defaultsview.py
+-rw-r--r--   0 root         (0) root         (0)     4373 2023-05-27 07:26:44.000000 dbm-agent-8.33.9/dbma/components/mysql/views/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.946062 dbm-agent-8.33.9/dbma/components/orchestrator/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/components/orchestrator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      324 2023-05-27 07:26:58.000000 dbm-agent-8.33.9/dbma/components/orchestrator/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2023-05-27 07:27:01.000000 dbm-agent-8.33.9/dbma/components/orchestrator/install.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.948062 dbm-agent-8.33.9/dbma/components/redis/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/components/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1623 2023-05-27 07:27:34.000000 dbm-agent-8.33.9/dbma/components/redis/commons.py
+-rw-r--r--   0 root         (0) root         (0)     2776 2023-05-27 07:27:09.000000 dbm-agent-8.33.9/dbma/components/redis/config.py
+-rw-r--r--   0 root         (0) root         (0)      548 2023-05-27 07:27:39.000000 dbm-agent-8.33.9/dbma/components/redis/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     7306 2023-05-27 07:27:47.000000 dbm-agent-8.33.9/dbma/components/redis/install.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-05-27 07:27:52.000000 dbm-agent-8.33.9/dbma/components/redis/systemd.py
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-27 07:27:57.000000 dbm-agent-8.33.9/dbma/components/redis/uninstall.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.950062 dbm-agent-8.33.9/dbma/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.951062 dbm-agent-8.33.9/dbma/core/agent/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/core/agent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3460 2023-05-27 07:29:03.000000 dbm-agent-8.33.9/dbma/core/agent/init.py
+-rw-r--r--   0 root         (0) root         (0)      115 2023-05-27 07:29:07.000000 dbm-agent-8.33.9/dbma/core/agent/upgrade.py
+-rw-r--r--   0 root         (0) root         (0)     3677 2023-05-27 07:28:10.000000 dbm-agent-8.33.9/dbma/core/configs.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-27 07:28:18.000000 dbm-agent-8.33.9/dbma/core/exception.py
+-rw-r--r--   0 root         (0) root         (0)     3469 2023-05-27 07:28:26.000000 dbm-agent-8.33.9/dbma/core/httpserver.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-05-27 07:28:34.000000 dbm-agent-8.33.9/dbma/core/messages.py
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-27 07:28:39.000000 dbm-agent-8.33.9/dbma/core/router.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.951062 dbm-agent-8.33.9/dbma/core/threads/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/core/threads/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-05-27 07:28:57.000000 dbm-agent-8.33.9/dbma/core/threads/backends.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.952062 dbm-agent-8.33.9/dbma/core/views/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/core/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/core/views/dbmagentview.py
+-rw-r--r--   0 root         (0) root         (0)      466 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/core/views/response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.936062 dbm-agent-8.33.9/dbma/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.971062 dbm-agent-8.33.9/dbma/static/cnfs/
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/auto-inseption-db.sql
+-rw-r--r--   0 root         (0) root         (0)      168 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/create-innodb-cluster.js
+-rw-r--r--   0 root         (0) root         (0)      286 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/dbm-backup-proxyd.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      385 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/dbm-monitor-gatewayd.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      514 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/init-5.7.x.sql
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/init-8.0.x.sql
+-rw-r--r--   0 root         (0) root         (0)     6681 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/init-users.sql.jinja
+-rw-r--r--   0 root         (0) root         (0)    10688 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-5.7-init-only.jinja
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-5.7.25.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    14664 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0-init-only.jinja
+-rw-r--r--   0 root         (0) root         (0)    17621 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.17.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17631 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.18.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17687 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.19.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17766 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.20.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17766 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.21.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.22.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.23.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.25.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.26.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17528 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.27.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17528 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.28.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17528 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.29.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17799 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.30.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    18787 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.31.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    18776 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.32.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    18774 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.33.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)      465 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/mysqld.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      681 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/redis.conf.jinja
+-rw-r--r--   0 root         (0) root         (0)      710 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/redisd.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      362 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/zabbix-agentd.service
+-rw-r--r--   0 root         (0) root         (0)    10464 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/zabbix_agentd.conf.jinja
+-rw-r--r--   0 root         (0) root         (0)      258 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/cnfs/zoo.cnf.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 07:31:59.972061 dbm-agent-8.33.9/dbma/static/sql-scripts/
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/dbma/static/sql-scripts/常用SQL.md
+-rw-r--r--   0 root         (0) root         (0)      344 2023-05-27 07:31:24.000000 dbm-agent-8.33.9/dbma/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-27 07:31:59.973061 dbm-agent-8.33.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-05-20 14:15:43.000000 dbm-agent-8.33.9/setup.py
```

### Comparing `dbm-agent-8.33.8/PKG-INFO` & `dbm-agent-8.33.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbm-agent
-Version: 8.33.8
+Version: 8.33.9
 Summary: dbm-agent 数据库管理中心客户端程序
 Home-page: https://github.com/Neeky/dbm-agent
 Author: Neeky
 Author-email: neeky@live.com
 Maintainer: Neeky
 Maintainer-email: neeky@live.com
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dbm-agent-8.33.8/README.md` & `dbm-agent-8.33.9/README.md`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/bin/dbm-agent` & `dbm-agent-8.33.9/bin/dbm-agent`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 #!/usr/bin/evn python3
+# -*- coding: utf8 -*-
 
-# (c) 2019, LeXing Jinag <neeky@live.com 1721900707@qq.com https://www.sqlpy.com/>
-# Copyright: (c) 2019, dbm Project
-# GNU General Public License v3.0+ (see COPYING or https://www.gnu.org/licenses/gpl-3.0.txt)
+"""
+(c) 2019, LeXing Jinag <neeky@live.com 1721900707@qq.com https://www.sqlpy.com/>
+Copyright: (c) 2019, dbm Project
+GNU General Public License v3.0+ (see COPYING or https://www.gnu.org/licenses/gpl-3.0.txt)
+"""
 
 
 import argparse
 from dbma.core.httpserver import start, stop
 from dbma.version import DBM_AGENT_VESION
```

### Comparing `dbm-agent-8.33.8/bin/dbma-cli-init` & `dbm-agent-8.33.9/bin/dbma-cli-init`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/evn python3
+# -*- coding: utf8 -*-
 
 """
 完成 dbm-agent 的初始化操作
 """
 
 import argparse
 from dbma.bil.net import get_ip_by_card_name
```

### Comparing `dbm-agent-8.33.8/bin/dbma-cli-mysql` & `dbm-agent-8.33.9/bin/dbma-cli-mysql`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+# -*- coding: utf8 -*-
 
 """
 实例单实例架构下的 MySQL 安装与卸载
 """
 
 import time
 import logging
```

### Comparing `dbm-agent-8.33.8/bin/dbma-cli-redis` & `dbm-agent-8.33.9/bin/dbma-cli-redis`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-# -*- encoding: utf8 -*-
+# -*- coding: utf8 -*-
 
 """
 dbm-agent Redis 的命令行接口
 """
 
 import re
 import time
```

### Comparing `dbm-agent-8.33.8/dbm_agent.egg-info/PKG-INFO` & `dbm-agent-8.33.9/dbm_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbm-agent
-Version: 8.33.8
+Version: 8.33.9
 Summary: dbm-agent 数据库管理中心客户端程序
 Home-page: https://github.com/Neeky/dbm-agent
 Author: Neeky
 Author-email: neeky@live.com
 Maintainer: Neeky
 Maintainer-email: neeky@live.com
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dbm-agent-8.33.8/dbm_agent.egg-info/SOURCES.txt` & `dbm-agent-8.33.9/dbm_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/bil/daemon.py` & `dbm-agent-8.33.9/dbma/bil/daemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# -*- coding: utf8 -*-
+
 import os
 import sys
 import stat
 import time
 import fcntl
 import errno
 import signal
```

### Comparing `dbm-agent-8.33.8/dbma/bil/fs.py` & `dbm-agent-8.33.9/dbma/bil/fs.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/bil/net.py` & `dbm-agent-8.33.9/dbma/bil/net.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/bil/osuser.py` & `dbm-agent-8.33.9/dbma/bil/osuser.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/bil/sudos.py` & `dbm-agent-8.33.9/dbma/bil/sudos.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/components/mysql/backups/cloneplugin.py` & `dbm-agent-8.33.9/dbma/components/mysql/backups/cloneplugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- encoding: utf-8 -*-
+# -*- coding: utf-8 -*-
 
 """MySQL 克隆插件备份逻辑
 
 CLONE LOCAL DATA DIRECTORY [=] 'clone_dir';
 """
```

### Comparing `dbm-agent-8.33.8/dbma/components/mysql/commons.py` & `dbm-agent-8.33.9/dbma/components/mysql/commons.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- encoding: utf-8 -*-
+# -*- coding: utf-8 -*-
 
 """MySQL 组件的公共函数
 """
 
 import re
 import logging
 import shutil
@@ -201,8 +201,9 @@
     logging.info(messages.FUN_STARTS.format(fname()))
 
     with dbma_mysql_cnx(port) as cursor:
         sql = "set @@global.read_only=OFF; set @@global.super_read_only=OFF;"
         cursor.execute(sql)
         logging.info("make mysql instance 127.0.0.1:{} writable .".format(port))
         logging.info("sql = {}".format(cursor.statement))
+
     logging.info(messages.FUN_ENDS.format(fname()))
```

### Comparing `dbm-agent-8.33.8/dbma/components/mysql/config.py` & `dbm-agent-8.33.9/dbma/components/mysql/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- encoding: utf-8 -*-
+# -*- coding: utf-8 -*-
 
 """MySQL 配置文件相关的逻辑
 
 作者: 蒋乐兴|neeky@live.com
 时间: 2023-03
 """
 
@@ -553,15 +553,15 @@
         """计算内存相关的值"""
         if self.innodb_buffer_pool_size.endswith("M"):
             # M 级别
             self.innodb_buffer_pool_instances = 1
             self.innodb_log_buffer_size = "64M"
         elif self.innodb_buffer_pool_size.endswith("G"):
             # G 级别
-            size = re.match("\d*", self.innodb_buffer_pool_size).group(0)
+            size = re.match(r"\d*", self.innodb_buffer_pool_size).group(0)
             size = int(size)
             if size <= 2:
                 self.innodb_buffer_pool_instances = 1
                 self.innodb_log_buffer_size = "64M"
             elif size <= 4:
                 self.innodb_buffer_pool_instances = size
                 self.innodb_log_buffer_size = "128M"
```

### Comparing `dbm-agent-8.33.8/dbma/components/mysql/exceptions.py` & `dbm-agent-8.33.9/dbma/components/mysql/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- encoding: utf-8 -*-
+# -*- coding: utf-8 -*-
 
 """异常树"""
 
 from dbma.core.exception import DBMAgentException
 
 
 class MySQLTemplateFileNotExistsException(DBMAgentException):
```

### Comparing `dbm-agent-8.33.8/dbma/components/mysql/install.py` & `dbm-agent-8.33.9/dbma/components/mysql/install.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- encoding: utf-8 -*-
+# -*- coding: utf-8 -*-
 
 """MySQL 安装相关的逻辑实现
 
 作者: 蒋乐兴|neeky@live.com
 时间: 2023-03
 """
 
@@ -51,15 +51,19 @@
 
     # 检查版本号并根据版本号生成配置文件
     if version.startswith("8.0"):
         sql_file = Path(dbma.__file__).parent / "static/cnfs/init-8.0.x.sql"
     elif version.startswith("5.7"):
         sql_file = Path(dbma.__file__).parent / "static/cnfs/init-5.7.x.sql"
     else:
-        message = "mysql version is '{}', can't create init-sql-file .".format(version)
+        message = (
+            "mysql version is '{}' not suported, can't create init-sql-file .".format(
+                version
+            )
+        )
         logging.error(message)
         raise ValueError(messages)
     logging.info("init sql file = {}".format(sql_file))
 
     # 复制文件
     shutil.copy(sql_file, dbm_agent_config.mysql_init_user_sql_file)
     logging.info(messages.FUN_ENDS.format(fname()))
```

### Comparing `dbm-agent-8.33.8/dbma/components/mysql/instance.py` & `dbm-agent-8.33.9/dbma/components/mysql/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- encoding: utf-8 -*-
+# -*- coding: utf-8 -*-
 
 """在 MySQL 实例层面相关的函数
 
 作者: 蒋乐兴|neeky@live.com
 时间: 2023-03
 """
```

### Comparing `dbm-agent-8.33.8/dbma/components/mysql/replica.py` & `dbm-agent-8.33.9/dbma/components/mysql/replica.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- encoding: utf-8 -*-
+# -*- coding: utf-8 -*-
 
 """MySQL 备机相关的操作
 
 作者: 蒋乐兴|neeky@live.com
 时间: 2023-03
 """
```

### Comparing `dbm-agent-8.33.8/dbma/components/mysql/source.py` & `dbm-agent-8.33.9/dbma/components/mysql/source.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- encoding: utf-8 -*-
+# -*- coding: utf-8 -*-
 
 """MySQL 源实例相关的操作
 
 作者: 蒋乐兴|neeky@live.com
 时间: 2023-04
 """
```

### Comparing `dbm-agent-8.33.8/dbma/components/mysql/views/defaultsview.py` & `dbm-agent-8.33.9/dbma/components/mysql/views/defaultsview.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- encoding: utf-8 -*-
+# -*- coding: utf-8 -*-
 
 """MySQL 安装的相关接口
 """
 
 import re
 import logging
 from aiohttp import web
```

### Comparing `dbm-agent-8.33.8/dbma/components/mysql/views/handlers.py` & `dbm-agent-8.33.9/dbma/components/mysql/views/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- encoding: utf-8 -*-
+# -*- coding: utf-8 -*-
 
 """dbm-agent 收到操作请求(task)之后，如果请求中没有带 task_id ，说明要求同步执行；如果有带 task_id 那么我们要把 task 放到后台线程中执行。
 
 """
 
 import logging
 from pathlib import Path
```

### Comparing `dbm-agent-8.33.8/dbma/components/orchestrator/install.py` & `dbm-agent-8.33.9/dbma/components/orchestrator/install.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- encoding: utf-8 -*-
+# -*- coding: utf-8 -*-
 
 """安装 orchestrator
 """
 
 import re
 import tarfile
 import logging
```

### Comparing `dbm-agent-8.33.8/dbma/components/redis/commons.py` & `dbm-agent-8.33.9/dbma/components/redis/commons.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# -*- coding: utf-8 -*-
+
+"""
+Redis 相关的公共函数
+"""
+
 import re
 from pathlib import Path
 
 from dbma.bil.fs import is_file_exists
 from dbma.core.configs import dbm_agent_config
 
 # Redis 的默认端口号
```

### Comparing `dbm-agent-8.33.8/dbma/components/redis/config.py` & `dbm-agent-8.33.9/dbma/components/redis/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- encoding: utf-8 -*-
+# -*- coding: utf-8 -*-
 
 """Resdis 自动化配置"""
 
 import logging
 from pathlib import Path
 from jinja2 import Template
 from datetime import datetime
```

### Comparing `dbm-agent-8.33.8/dbma/components/redis/exceptions.py` & `dbm-agent-8.33.9/dbma/components/redis/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- encoding: utf-8 -*-
+# -*- coding: utf-8 -*-
 
 """Resdis 相关的异常"""
 
 from dbma.core.exception import (
     FileExistsException,
     FileNotExistsException,
     DirectoryExistsException,
```

### Comparing `dbm-agent-8.33.8/dbma/components/redis/install.py` & `dbm-agent-8.33.9/dbma/components/redis/install.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- encoding: utf-8 -*-
+# -*- coding: utf-8 -*-
 
 """Redis 环境的安装"""
 
 
 import os
 import tarfile
 import logging
```

### Comparing `dbm-agent-8.33.8/dbma/components/redis/systemd.py` & `dbm-agent-8.33.9/dbma/components/redis/systemd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- encoding: utf-8 -*-
+# -*- coding: utf-8 -*-
 
 """Resdis systemd 相关的配置"""
 
 import logging
 from pathlib import Path
 from jinja2 import Template
 from datetime import datetime
```

### Comparing `dbm-agent-8.33.8/dbma/core/agent/init.py` & `dbm-agent-8.33.9/dbma/core/agent/init.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- encoding: utf-8 -*-
+# -*- coding: utf-8 -*-
 
 """dbm-agent 安装
 
 作者: 蒋乐兴|neeky@live.com
 时间: 2023-03
 """
```

### Comparing `dbm-agent-8.33.8/dbma/core/configs.py` & `dbm-agent-8.33.9/dbma/core/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- encoding: utf-8 -*-
+# -*- coding: utf-8 -*-
 
 """dbm-agent 的配置文件
 
 作者: 蒋乐兴|neeky@live.com
 时间: 2023-03
 """
```

### Comparing `dbm-agent-8.33.8/dbma/core/exception.py` & `dbm-agent-8.33.9/dbma/core/exception.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- encoding: utf-8 -*-
+# -*- coding: utf-8 -*-
 
 """dbm-agent exceptions
 
 """
 
 
 class DBMAgentException(Exception):
```

### Comparing `dbm-agent-8.33.8/dbma/core/httpserver.py` & `dbm-agent-8.33.9/dbma/core/httpserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- encoding: utf-8 -*-
+# -*- coding: utf-8 -*-
 
 """dbm-agent http-server
 
 """
 
 import os
 import logging
```

### Comparing `dbm-agent-8.33.8/dbma/core/messages.py` & `dbm-agent-8.33.9/dbma/core/messages.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- encoding: utf-8 -*-
+# -*- coding: utf-8 -*-
 
 """代码写到一定的量之后发现，实在是太多的字符串常量了。另人难过的差不多的语境，不同时期的拼写还不一致。
 作者: 蒋乐兴|neeky
 时间: 2023-03
 """
 
 # 函数开执行
```

### Comparing `dbm-agent-8.33.8/dbma/core/threads/backends.py` & `dbm-agent-8.33.9/dbma/core/threads/backends.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- encoding: utf-8 -*-
+# -*- coding: utf-8 -*-
 
 """dbm-agent 周期性任务
 
 作者: 蒋乐兴|neeky@live.com
 时间: 2023-03
 """
```

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/auto-inseption-db.sql` & `dbm-agent-8.33.9/dbma/static/cnfs/auto-inseption-db.sql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/init-5.7.x.sql` & `dbm-agent-8.33.9/dbma/static/cnfs/init-5.7.x.sql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/init-8.0.x.sql` & `dbm-agent-8.33.9/dbma/static/cnfs/init-8.0.x.sql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/init-users.sql.jinja` & `dbm-agent-8.33.9/dbma/static/cnfs/init-users.sql.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/mysql-5.7-init-only.jinja` & `dbm-agent-8.33.9/dbma/static/cnfs/mysql-5.7-init-only.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/mysql-5.7.25.cnf.jinja` & `dbm-agent-8.33.9/dbma/static/cnfs/mysql-5.7.25.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0-init-only.jinja` & `dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0-init-only.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.17.cnf.jinja` & `dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.17.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.18.cnf.jinja` & `dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.18.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.19.cnf.jinja` & `dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.19.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.20.cnf.jinja` & `dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.20.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.21.cnf.jinja` & `dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.21.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.22.cnf.jinja` & `dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.22.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.23.cnf.jinja` & `dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.23.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.25.cnf.jinja` & `dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.25.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.26.cnf.jinja` & `dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.26.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.27.cnf.jinja` & `dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.27.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.28.cnf.jinja` & `dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.28.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.29.cnf.jinja` & `dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.29.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.30.cnf.jinja` & `dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.30.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.31.cnf.jinja` & `dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.31.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.32.cnf.jinja` & `dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.32.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.33.cnf.jinja` & `dbm-agent-8.33.9/dbma/static/cnfs/mysql-8.0.33.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/redis.conf.jinja` & `dbm-agent-8.33.9/dbma/static/cnfs/redis.conf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/redisd.service.jinja` & `dbm-agent-8.33.9/dbma/static/cnfs/redisd.service.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/cnfs/zabbix_agentd.conf.jinja` & `dbm-agent-8.33.9/dbma/static/cnfs/zabbix_agentd.conf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/dbma/static/sql-scripts/常用SQL.md` & `dbm-agent-8.33.9/dbma/static/sql-scripts/常用SQL.md`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.8/setup.py` & `dbm-agent-8.33.9/setup.py`

 * *Files identical despite different names*

