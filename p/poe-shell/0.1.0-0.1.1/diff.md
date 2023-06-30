# Comparing `tmp/poe_shell-0.1.0.tar.gz` & `tmp/poe_shell-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poe_shell-0.1.0.tar", max compression
+gzip compressed data, was "poe_shell-0.1.1.tar", max compression
```

## Comparing `poe_shell-0.1.0.tar` & `poe_shell-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-06-30 03:02:37.314727 poe_shell-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-30 03:02:37.314864 poe_shell-0.1.0/poe_shell/__init__.py
--rw-r--r--   0        0        0     1414 2023-06-30 03:17:38.442897 poe_shell-0.1.0/poe_shell/__main__.py
--rw-r--r--   0        0        0        0 2023-06-30 03:02:37.315128 poe_shell-0.1.0/poe_shell/handlers/__init__.py
--rw-r--r--   0        0        0      942 2023-06-30 03:28:19.430015 poe_shell-0.1.0/poe_shell/handlers/chat_handler.py
--rw-r--r--   0        0        0      291 2023-06-30 03:22:17.474038 poe_shell-0.1.0/poe_shell/handlers/handler.py
--rw-r--r--   0        0        0      375 2023-06-30 03:22:44.232937 poe_shell-0.1.0/poe_shell/handlers/one_off_handler.py
--rw-r--r--   0        0        0     1632 2023-06-30 03:28:52.616388 poe_shell-0.1.0/poe_shell/handlers/shell_handler.py
--rw-r--r--   0        0        0      840 2023-06-30 03:02:37.315763 poe_shell-0.1.0/poe_shell/poe_client.py
--rw-r--r--   0        0        0     1245 2023-06-30 03:02:37.315873 poe_shell-0.1.0/poe_shell/roles.py
--rw-r--r--   0        0        0      646 2023-06-30 03:02:37.315982 poe_shell-0.1.0/poe_shell/utils.py
--rw-r--r--   0        0        0      374 2023-06-30 03:02:37.316582 poe_shell-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      374 1970-01-01 00:00:00.000000 poe_shell-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      760 2023-06-30 04:11:45.326714 poe_shell-0.1.1/README.md
+-rw-r--r--   0        0        0       35 2023-06-30 07:35:34.125904 poe_shell-0.1.1/poe_shell/__init__.py
+-rw-r--r--   0        0        0     1438 2023-06-30 07:36:12.466988 poe_shell-0.1.1/poe_shell/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-30 03:02:37.315128 poe_shell-0.1.1/poe_shell/handlers/__init__.py
+-rw-r--r--   0        0        0      942 2023-06-30 03:28:19.430015 poe_shell-0.1.1/poe_shell/handlers/chat_handler.py
+-rw-r--r--   0        0        0      291 2023-06-30 03:22:17.474038 poe_shell-0.1.1/poe_shell/handlers/handler.py
+-rw-r--r--   0        0        0      375 2023-06-30 03:22:44.232937 poe_shell-0.1.1/poe_shell/handlers/one_off_handler.py
+-rw-r--r--   0        0        0     1632 2023-06-30 03:28:52.616388 poe_shell-0.1.1/poe_shell/handlers/shell_handler.py
+-rw-r--r--   0        0        0      840 2023-06-30 03:02:37.315763 poe_shell-0.1.1/poe_shell/poe_client.py
+-rw-r--r--   0        0        0     1245 2023-06-30 03:02:37.315873 poe_shell-0.1.1/poe_shell/roles.py
+-rw-r--r--   0        0        0      646 2023-06-30 03:02:37.315982 poe_shell-0.1.1/poe_shell/utils.py
+-rw-r--r--   0        0        0      424 2023-06-30 07:40:50.655841 poe_shell-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 poe_shell-0.1.1/PKG-INFO
```

### Comparing `poe_shell-0.1.0/poe_shell/__main__.py` & `poe_shell-0.1.1/poe_shell/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typer
 import sys
 
-from poe_client import PoeClient
+from .poe_client import PoeClient
 
 app = typer.Typer()
 
 
 @app.command()
 def main(
     message: str = typer.Argument(
@@ -60,9 +60,13 @@
 
         OneOffHandler(client).handle(message)
 
     else:
         typer.echo("Use --help for more information.")
 
 
+def cli():
+    app()
+
+
 if __name__ == "__main__":
     app()
```

### Comparing `poe_shell-0.1.0/poe_shell/handlers/chat_handler.py` & `poe_shell-0.1.1/poe_shell/handlers/chat_handler.py`

 * *Files identical despite different names*

### Comparing `poe_shell-0.1.0/poe_shell/handlers/shell_handler.py` & `poe_shell-0.1.1/poe_shell/handlers/shell_handler.py`

 * *Files identical despite different names*

### Comparing `poe_shell-0.1.0/poe_shell/poe_client.py` & `poe_shell-0.1.1/poe_shell/poe_client.py`

 * *Files identical despite different names*

### Comparing `poe_shell-0.1.0/poe_shell/roles.py` & `poe_shell-0.1.1/poe_shell/roles.py`

 * *Files identical despite different names*

### Comparing `poe_shell-0.1.0/poe_shell/utils.py` & `poe_shell-0.1.1/poe_shell/utils.py`

 * *Files identical despite different names*

