# Comparing `tmp/im_openai-0.4.1.tar.gz` & `tmp/im_openai-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "im_openai-0.4.1.tar", last modified: Thu Jun 29 22:55:09 2023, max compression
+gzip compressed data, was "im_openai-0.4.2.tar", last modified: Thu Jun 29 23:17:01 2023, max compression
```

## Comparing `im_openai-0.4.1.tar` & `im_openai-0.4.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-29 22:55:09.543399 im_openai-0.4.1/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      150 2023-06-20 23:30:14.000000 im_openai-0.4.1/AUTHORS.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3560 2023-06-22 20:28:17.000000 im_openai-0.4.1/CONTRIBUTING.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-06-20 23:30:14.000000 im_openai-0.4.1/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)      261 2023-06-22 20:24:41.000000 im_openai-0.4.1/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2799 2023-06-29 22:55:09.543841 im_openai-0.4.1/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1553 2023-06-24 00:40:31.000000 im_openai-0.4.1/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-29 22:55:09.502725 im_openai-0.4.1/docs/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-20 23:30:14.000000 im_openai-0.4.1/docs/Makefile
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.4.1/docs/authors.rst
--rwxr-xr-x   0 vscode    (1000) vscode    (1000)     4874 2023-06-20 23:30:14.000000 im_openai-0.4.1/docs/conf.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2023-06-20 23:30:14.000000 im_openai-0.4.1/docs/contributing.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.4.1/docs/history.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-20 23:30:14.000000 im_openai-0.4.1/docs/index.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1175 2023-06-20 23:30:14.000000 im_openai-0.4.1/docs/installation.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-06-20 23:30:14.000000 im_openai-0.4.1/docs/make.bat
--rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2023-06-22 20:24:52.000000 im_openai-0.4.1/docs/readme.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       92 2023-06-20 23:30:14.000000 im_openai-0.4.1/docs/usage.rst
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-29 22:55:09.518377 im_openai-0.4.1/im_openai/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2023-06-23 16:59:08.000000 im_openai-0.4.1/im_openai/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3872 2023-06-29 18:15:38.000000 im_openai-0.4.1/im_openai/client.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2081 2023-06-29 22:49:14.000000 im_openai-0.4.1/im_openai/langchain_util.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2812 2023-06-29 18:15:40.000000 im_openai-0.4.1/im_openai/patch.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      423 2023-06-23 21:56:38.000000 im_openai-0.4.1/im_openai/template.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-29 22:55:09.535440 im_openai-0.4.1/im_openai.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2799 2023-06-29 22:55:09.000000 im_openai-0.4.1/im_openai.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-06-29 22:55:09.000000 im_openai-0.4.1/im_openai.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-29 22:55:09.000000 im_openai-0.4.1/im_openai.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-29 22:55:09.000000 im_openai-0.4.1/im_openai.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-06-29 22:55:09.000000 im_openai-0.4.1/im_openai.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      426 2023-06-29 22:55:09.545443 im_openai-0.4.1/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1350 2023-06-29 22:51:20.000000 im_openai-0.4.1/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-29 22:55:09.541516 im_openai-0.4.1/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-06-20 23:30:14.000000 im_openai-0.4.1/tests/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-06-20 23:30:14.000000 im_openai-0.4.1/tests/test_im_openai.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-29 23:17:01.134739 im_openai-0.4.2/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      150 2023-06-20 23:30:14.000000 im_openai-0.4.2/AUTHORS.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3560 2023-06-22 20:28:17.000000 im_openai-0.4.2/CONTRIBUTING.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-06-20 23:30:14.000000 im_openai-0.4.2/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      261 2023-06-22 20:24:41.000000 im_openai-0.4.2/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2922 2023-06-29 23:17:01.135214 im_openai-0.4.2/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1553 2023-06-24 00:40:31.000000 im_openai-0.4.2/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-29 23:17:01.089197 im_openai-0.4.2/docs/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-20 23:30:14.000000 im_openai-0.4.2/docs/Makefile
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.4.2/docs/authors.rst
+-rwxr-xr-x   0 vscode    (1000) vscode    (1000)     4874 2023-06-20 23:30:14.000000 im_openai-0.4.2/docs/conf.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2023-06-20 23:30:14.000000 im_openai-0.4.2/docs/contributing.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.4.2/docs/history.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-20 23:30:14.000000 im_openai-0.4.2/docs/index.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1175 2023-06-20 23:30:14.000000 im_openai-0.4.2/docs/installation.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-06-20 23:30:14.000000 im_openai-0.4.2/docs/make.bat
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2023-06-22 20:24:52.000000 im_openai-0.4.2/docs/readme.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       92 2023-06-20 23:30:14.000000 im_openai-0.4.2/docs/usage.rst
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-29 23:17:01.106474 im_openai-0.4.2/im_openai/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2023-06-23 16:59:08.000000 im_openai-0.4.2/im_openai/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3872 2023-06-29 18:15:38.000000 im_openai-0.4.2/im_openai/client.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2039 2023-06-29 23:15:53.000000 im_openai-0.4.2/im_openai/langchain_util.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2812 2023-06-29 18:15:40.000000 im_openai-0.4.2/im_openai/patch.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      423 2023-06-23 21:56:38.000000 im_openai-0.4.2/im_openai/template.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-29 23:17:01.123010 im_openai-0.4.2/im_openai.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2922 2023-06-29 23:17:00.000000 im_openai-0.4.2/im_openai.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-06-29 23:17:01.000000 im_openai-0.4.2/im_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-29 23:17:00.000000 im_openai-0.4.2/im_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-29 23:17:00.000000 im_openai-0.4.2/im_openai.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-06-29 23:17:00.000000 im_openai-0.4.2/im_openai.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      426 2023-06-29 23:17:01.136841 im_openai-0.4.2/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1350 2023-06-29 23:16:21.000000 im_openai-0.4.2/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-29 23:17:01.132584 im_openai-0.4.2/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-06-20 23:30:14.000000 im_openai-0.4.2/tests/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-06-20 23:30:14.000000 im_openai-0.4.2/tests/test_im_openai.py
```

### Comparing `im_openai-0.4.1/CONTRIBUTING.rst` & `im_openai-0.4.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.1/LICENSE` & `im_openai-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.1/PKG-INFO` & `im_openai-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im_openai
-Version: 0.4.1
+Version: 0.4.2
 Summary: Wrapper library for openai to send events to the Imaginary Programming monitor
 Home-page: https://github.com/alecf/im_openai
 Author: Alec Flett
 Author-email: alec@thegp.com
 License: MIT license
 Keywords: im_openai
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -100,7 +100,16 @@
 ## 0.3.0 (2023-06-28)
 
 - add support for chat templates (as objects instead of arrays)
 
 ## 0.4.0 (2023-06-29)
 
 - switch event reporting to be async / non-blocking
+
+## 0.4.1 (2023-06-29)
+
+- add utility for formatting langchain messages
+
+## 0.4.2 (2023-06-29)
+
+- remove stray breakpoint
+
```

### Comparing `im_openai-0.4.1/README.md` & `im_openai-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.1/docs/Makefile` & `im_openai-0.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.1/docs/conf.py` & `im_openai-0.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.1/docs/installation.rst` & `im_openai-0.4.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.1/docs/make.bat` & `im_openai-0.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.1/im_openai/client.py` & `im_openai-0.4.2/im_openai/client.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.1/im_openai/langchain_util.py` & `im_openai-0.4.2/im_openai/langchain_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,13 +43,11 @@
             "content": f"{{{message.variable_name}}}",
         }
         return [formatted_messages]
     elif isinstance(message, BaseMessagePromptTemplate):
         vars = message.input_variables
         # create a fake dictionary mapping name -> '{name}'
         vars_as_templates = {v: f"{{{v}}}" for v in vars}
-        breakpoint()
         formatted_messages = message.format_messages(**vars_as_templates)
         return format_chat_template(formatted_messages)
     else:
-        breakpoint()
         raise ValueError(f"Got unknown type {message}")
```

### Comparing `im_openai-0.4.1/im_openai/patch.py` & `im_openai-0.4.2/im_openai/patch.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.1/im_openai.egg-info/PKG-INFO` & `im_openai-0.4.2/im_openai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-openai
-Version: 0.4.1
+Version: 0.4.2
 Summary: Wrapper library for openai to send events to the Imaginary Programming monitor
 Home-page: https://github.com/alecf/im_openai
 Author: Alec Flett
 Author-email: alec@thegp.com
 License: MIT license
 Keywords: im_openai
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -100,7 +100,16 @@
 ## 0.3.0 (2023-06-28)
 
 - add support for chat templates (as objects instead of arrays)
 
 ## 0.4.0 (2023-06-29)
 
 - switch event reporting to be async / non-blocking
+
+## 0.4.1 (2023-06-29)
+
+- add utility for formatting langchain messages
+
+## 0.4.2 (2023-06-29)
+
+- remove stray breakpoint
+
```

### Comparing `im_openai-0.4.1/im_openai.egg-info/SOURCES.txt` & `im_openai-0.4.2/im_openai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.1/setup.py` & `im_openai-0.4.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="im_openai",
     name="im_openai",
     packages=find_packages(include=["im_openai", "im_openai.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/alecf/im_openai",
-    version="0.4.1",
+    version="0.4.2",
     zip_safe=False,
 )
```

### Comparing `im_openai-0.4.1/tests/test_im_openai.py` & `im_openai-0.4.2/tests/test_im_openai.py`

 * *Files identical despite different names*

