# Comparing `tmp/superagi_client-1.0.0.tar.gz` & `tmp/superagi_client-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superagi_client-1.0.0.tar", last modified: Thu Jun 29 10:22:33 2023, max compression
+gzip compressed data, was "superagi_client-1.0.1.tar", last modified: Fri Jun 30 05:33:38 2023, max compression
```

## Comparing `superagi_client-1.0.0.tar` & `superagi_client-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 10:22:33.412951 superagi_client-1.0.0/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-28 12:07:33.000000 superagi_client-1.0.0/LICENSE
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      188 2023-06-29 10:22:33.412951 superagi_client-1.0.0/PKG-INFO
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       76 2023-06-28 12:10:34.000000 superagi_client-1.0.0/README.md
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       38 2023-06-29 10:22:33.412951 superagi_client-1.0.0/setup.cfg
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      307 2023-06-29 10:22:20.000000 superagi_client-1.0.0/setup.py
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 10:22:33.408951 superagi_client-1.0.0/superagi/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:44:17.000000 superagi_client-1.0.0/superagi/__init__.py
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 10:22:33.408951 superagi_client-1.0.0/superagi/tools/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:51:45.000000 superagi_client-1.0.0/superagi/tools/__init__.py
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)     6706 2023-06-29 10:14:39.000000 superagi_client-1.0.0/superagi/tools/base_tool.py
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 10:22:33.412951 superagi_client-1.0.0/superagi_client.egg-info/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      188 2023-06-29 10:22:33.000000 superagi_client-1.0.0/superagi_client.egg-info/PKG-INFO
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      296 2023-06-29 10:22:33.000000 superagi_client-1.0.0/superagi_client.egg-info/SOURCES.txt
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        1 2023-06-29 10:22:33.000000 superagi_client-1.0.0/superagi_client.egg-info/dependency_links.txt
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       16 2023-06-29 10:22:33.000000 superagi_client-1.0.0/superagi_client.egg-info/requires.txt
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        9 2023-06-29 10:22:33.000000 superagi_client-1.0.0/superagi_client.egg-info/top_level.txt
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-30 05:33:38.229311 superagi_client-1.0.1/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-28 12:07:33.000000 superagi_client-1.0.1/LICENSE
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      188 2023-06-30 05:33:38.229311 superagi_client-1.0.1/PKG-INFO
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       76 2023-06-28 12:10:34.000000 superagi_client-1.0.1/README.md
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       38 2023-06-30 05:33:38.229311 superagi_client-1.0.1/setup.cfg
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      307 2023-06-30 05:30:05.000000 superagi_client-1.0.1/setup.py
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-30 05:33:38.225311 superagi_client-1.0.1/superagi/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:44:17.000000 superagi_client-1.0.1/superagi/__init__.py
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-30 05:33:38.225311 superagi_client-1.0.1/superagi/tools/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:51:45.000000 superagi_client-1.0.1/superagi/tools/__init__.py
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)     6603 2023-06-30 05:10:33.000000 superagi_client-1.0.1/superagi/tools/base_tool.py
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-30 05:33:38.229311 superagi_client-1.0.1/superagi_client.egg-info/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      188 2023-06-30 05:33:38.000000 superagi_client-1.0.1/superagi_client.egg-info/PKG-INFO
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      296 2023-06-30 05:33:38.000000 superagi_client-1.0.1/superagi_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        1 2023-06-30 05:33:38.000000 superagi_client-1.0.1/superagi_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       16 2023-06-30 05:33:38.000000 superagi_client-1.0.1/superagi_client.egg-info/requires.txt
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        9 2023-06-30 05:33:38.000000 superagi_client-1.0.1/superagi_client.egg-info/top_level.txt
```

### Comparing `superagi_client-1.0.0/superagi/tools/base_tool.py` & `superagi_client-1.0.1/superagi/tools/base_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,17 +86,15 @@
 
     @abstractmethod
     def _execute(self, *args: Any, **kwargs: Any):
         pass
 
     @property
     def max_token_limit(self):
-        token_limit = self.get_tool_config("MAX_TOOL_TOKEN_LIMIT")
-        if token_limit is None:
-            token_limit = 600
+        token_limit = 600
         return token_limit
 
     def _parse_input(
             self,
             tool_input: Union[str, Dict],
     ) -> Union[str, Dict[str, Any]]:
         """Convert tool input to pydantic model."""
```

