# Comparing `tmp/idocker-1.1.0.tar.gz` & `tmp/idocker-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idocker-1.1.0.tar", last modified: Wed Jun 28 07:05:23 2023, max compression
+gzip compressed data, was "idocker-1.2.0.tar", last modified: Fri Jun 30 03:02:25 2023, max compression
```

## Comparing `idocker-1.1.0.tar` & `idocker-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 pon       (1001) pon       (1001)        0 2023-06-28 07:05:23.417278 idocker-1.1.0/
--rw-rw-r--   0 pon       (1001) pon       (1001)     2756 2023-06-28 07:05:23.417278 idocker-1.1.0/PKG-INFO
--rw-rw-r--   0 pon       (1001) pon       (1001)     1917 2023-01-31 04:58:15.000000 idocker-1.1.0/README.md
-drwxrwxr-x   0 pon       (1001) pon       (1001)        0 2023-06-28 07:05:23.409278 idocker-1.1.0/idocker/
--rw-rw-r--   0 pon       (1001) pon       (1001)      101 2023-06-28 07:00:37.000000 idocker-1.1.0/idocker/__init__.py
-drwxrwxr-x   0 pon       (1001) pon       (1001)        0 2023-06-28 07:05:23.417278 idocker-1.1.0/idocker/cli/
--rw-rw-r--   0 pon       (1001) pon       (1001)        0 2023-01-31 02:12:48.000000 idocker-1.1.0/idocker/cli/__init__.py
--rw-rw-r--   0 pon       (1001) pon       (1001)     2571 2023-06-28 07:04:12.000000 idocker-1.1.0/idocker/cli/main.py
-drwxrwxr-x   0 pon       (1001) pon       (1001)        0 2023-06-28 07:05:23.413278 idocker-1.1.0/idocker.egg-info/
--rw-rw-r--   0 pon       (1001) pon       (1001)     2756 2023-06-28 07:05:23.000000 idocker-1.1.0/idocker.egg-info/PKG-INFO
--rw-rw-r--   0 pon       (1001) pon       (1001)      280 2023-06-28 07:05:23.000000 idocker-1.1.0/idocker.egg-info/SOURCES.txt
--rw-rw-r--   0 pon       (1001) pon       (1001)        1 2023-06-28 07:05:23.000000 idocker-1.1.0/idocker.egg-info/dependency_links.txt
--rw-rw-r--   0 pon       (1001) pon       (1001)       49 2023-06-28 07:05:23.000000 idocker-1.1.0/idocker.egg-info/entry_points.txt
--rw-rw-r--   0 pon       (1001) pon       (1001)       18 2023-06-28 07:05:23.000000 idocker-1.1.0/idocker.egg-info/requires.txt
--rw-rw-r--   0 pon       (1001) pon       (1001)        8 2023-06-28 07:05:23.000000 idocker-1.1.0/idocker.egg-info/top_level.txt
--rw-rw-r--   0 pon       (1001) pon       (1001)       38 2023-06-28 07:05:23.417278 idocker-1.1.0/setup.cfg
--rw-rw-r--   0 pon       (1001) pon       (1001)     1305 2023-02-08 10:45:30.000000 idocker-1.1.0/setup.py
+drwxrwxr-x   0 pon       (1001) pon       (1001)        0 2023-06-30 03:02:24.994943 idocker-1.2.0/
+-rw-rw-r--   0 pon       (1001) pon       (1001)     2857 2023-06-30 03:02:24.994943 idocker-1.2.0/PKG-INFO
+-rw-rw-r--   0 pon       (1001) pon       (1001)     2018 2023-06-28 07:08:12.000000 idocker-1.2.0/README.md
+drwxrwxr-x   0 pon       (1001) pon       (1001)        0 2023-06-30 03:02:24.978943 idocker-1.2.0/idocker/
+-rw-rw-r--   0 pon       (1001) pon       (1001)      101 2023-06-30 03:01:31.000000 idocker-1.2.0/idocker/__init__.py
+drwxrwxr-x   0 pon       (1001) pon       (1001)        0 2023-06-30 03:02:24.994943 idocker-1.2.0/idocker/cli/
+-rw-rw-r--   0 pon       (1001) pon       (1001)        0 2023-01-31 02:12:48.000000 idocker-1.2.0/idocker/cli/__init__.py
+-rw-rw-r--   0 pon       (1001) pon       (1001)     4024 2023-06-30 03:01:24.000000 idocker-1.2.0/idocker/cli/main.py
+drwxrwxr-x   0 pon       (1001) pon       (1001)        0 2023-06-30 03:02:24.986943 idocker-1.2.0/idocker.egg-info/
+-rw-rw-r--   0 pon       (1001) pon       (1001)     2857 2023-06-30 03:02:24.000000 idocker-1.2.0/idocker.egg-info/PKG-INFO
+-rw-rw-r--   0 pon       (1001) pon       (1001)      280 2023-06-30 03:02:24.000000 idocker-1.2.0/idocker.egg-info/SOURCES.txt
+-rw-rw-r--   0 pon       (1001) pon       (1001)        1 2023-06-30 03:02:24.000000 idocker-1.2.0/idocker.egg-info/dependency_links.txt
+-rw-rw-r--   0 pon       (1001) pon       (1001)       49 2023-06-30 03:02:24.000000 idocker-1.2.0/idocker.egg-info/entry_points.txt
+-rw-rw-r--   0 pon       (1001) pon       (1001)       18 2023-06-30 03:02:24.000000 idocker-1.2.0/idocker.egg-info/requires.txt
+-rw-rw-r--   0 pon       (1001) pon       (1001)        8 2023-06-30 03:02:24.000000 idocker-1.2.0/idocker.egg-info/top_level.txt
+-rw-rw-r--   0 pon       (1001) pon       (1001)       38 2023-06-30 03:02:24.994943 idocker-1.2.0/setup.cfg
+-rw-rw-r--   0 pon       (1001) pon       (1001)     1305 2023-02-08 10:45:30.000000 idocker-1.2.0/setup.py
```

### Comparing `idocker-1.1.0/idocker/cli/main.py` & `idocker-1.2.0/idocker/cli/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Dict
+from typing import List, Dict, Optional
 from concurrent.futures.thread import ThreadPoolExecutor
 import click
 import docker
 from rich.console import Console
 from docker.models.containers import Container
 
 
@@ -83,11 +83,50 @@
             'cpu'.rjust(10, " "),
         ])
 
     for container_info in containers_info:
         console.print('   '.join(container_info))
 
 
+@idocker_cli.command()
+def port():
+    client = docker.from_env()
+
+    containers: List[Container] = client.containers.list(all=True)
+
+    console.print(f'There is a total of {len(containers)} container')
+
+    for container in containers:
+        try:
+            container_info = client.containers.get(container.id)
+            # ports like:
+            # - {'3000/tcp': [{'HostIp': '0.0.0.0', 'HostPort': '8000'}, {'HostIp': '::', 'HostPort': '8000'}]}
+            # - {'2379/tcp': None, '2380/tcp': None}
+            ports = container_info.attrs['NetworkSettings']['Ports']
+
+            ports: Dict[str, Optional[List[Dict[str, str]]]]
+
+            console.print(container.name, style="#c2a064")
+
+            if not ports:
+                console.print("    no network config", style='#c85662')
+                continue
+
+            console.print(
+                f"    {'Host'.ljust(8, ' ')} -> {'Container'.ljust(8, ' ')}", style='#62ae90')
+            for port in ports:
+                mappings = ports.get(port, [])
+                if not mappings:
+                    # console.print("    no port bind")
+                    continue
+                for mapping in mappings:
+                    host_port = f"{mapping['HostPort']}".ljust(8, ' ')
+                    container_port = f"{mapping['HostPort']}".ljust(8, ' ')
+                    console.print(f"    {host_port} -> {container_port}")
+        finally:
+            print()
+
+
 cli = click.CommandCollection(sources=[idocker_cli])
 
 if __name__ == '__main__':
     cli()
```

### Comparing `idocker-1.1.0/setup.py` & `idocker-1.2.0/setup.py`

 * *Files identical despite different names*

