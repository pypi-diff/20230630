# Comparing `tmp/chatglm-cli-0.0.1.tar.gz` & `tmp/chatglm-cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatglm-cli-0.0.1.tar", last modified: Wed Jun 28 09:31:19 2023, max compression
+gzip compressed data, was "chatglm-cli-0.1.1.tar", last modified: Fri Jun 30 08:01:05 2023, max compression
```

## Comparing `chatglm-cli-0.0.1.tar` & `chatglm-cli-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-28 09:31:19.017538 chatglm-cli-0.0.1/
--rw-r--r--   0 mroy       (501) staff       (20)      196 2023-06-28 09:31:19.017427 chatglm-cli-0.0.1/PKG-INFO
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-28 09:31:19.017085 chatglm-cli-0.0.1/chatglm_cli.egg-info/
--rw-r--r--   0 mroy       (501) staff       (20)      196 2023-06-28 09:31:18.000000 chatglm-cli-0.0.1/chatglm_cli.egg-info/PKG-INFO
--rw-r--r--   0 mroy       (501) staff       (20)      295 2023-06-28 09:31:19.000000 chatglm-cli-0.0.1/chatglm_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mroy       (501) staff       (20)        1 2023-06-28 09:31:18.000000 chatglm-cli-0.0.1/chatglm_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mroy       (501) staff       (20)       47 2023-06-28 09:31:18.000000 chatglm-cli-0.0.1/chatglm_cli.egg-info/entry_points.txt
--rw-r--r--   0 mroy       (501) staff       (20)        1 2023-06-28 09:31:18.000000 chatglm-cli-0.0.1/chatglm_cli.egg-info/not-zip-safe
--rw-r--r--   0 mroy       (501) staff       (20)       19 2023-06-28 09:31:18.000000 chatglm-cli-0.0.1/chatglm_cli.egg-info/requires.txt
--rw-r--r--   0 mroy       (501) staff       (20)       11 2023-06-28 09:31:18.000000 chatglm-cli-0.0.1/chatglm_cli.egg-info/top_level.txt
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-28 09:31:19.017272 chatglm-cli-0.0.1/chatglmcli/
--rw-r--r--   0 mroy       (501) staff       (20)        0 2023-06-28 09:19:02.000000 chatglm-cli-0.0.1/chatglmcli/__init__.py
--rw-r--r--   0 mroy       (501) staff       (20)     3815 2023-06-28 09:17:04.000000 chatglm-cli-0.0.1/chatglmcli/cmd.py
--rw-r--r--   0 mroy       (501) staff       (20)       38 2023-06-28 09:31:19.017579 chatglm-cli-0.0.1/setup.cfg
--rw-r--r--   0 mroy       (501) staff       (20)     1193 2023-06-28 09:18:32.000000 chatglm-cli-0.0.1/setup.py
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-30 08:01:05.318636 chatglm-cli-0.1.1/
+-rw-r--r--   0 mroy       (501) staff       (20)      196 2023-06-30 08:01:05.318528 chatglm-cli-0.1.1/PKG-INFO
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-30 08:01:05.318168 chatglm-cli-0.1.1/chatglm_cli.egg-info/
+-rw-r--r--   0 mroy       (501) staff       (20)      196 2023-06-30 08:01:05.000000 chatglm-cli-0.1.1/chatglm_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mroy       (501) staff       (20)      295 2023-06-30 08:01:05.000000 chatglm-cli-0.1.1/chatglm_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mroy       (501) staff       (20)        1 2023-06-30 08:01:05.000000 chatglm-cli-0.1.1/chatglm_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mroy       (501) staff       (20)       47 2023-06-30 08:01:05.000000 chatglm-cli-0.1.1/chatglm_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mroy       (501) staff       (20)        1 2023-06-28 09:31:18.000000 chatglm-cli-0.1.1/chatglm_cli.egg-info/not-zip-safe
+-rw-r--r--   0 mroy       (501) staff       (20)       26 2023-06-30 08:01:05.000000 chatglm-cli-0.1.1/chatglm_cli.egg-info/requires.txt
+-rw-r--r--   0 mroy       (501) staff       (20)       11 2023-06-30 08:01:05.000000 chatglm-cli-0.1.1/chatglm_cli.egg-info/top_level.txt
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-30 08:01:05.318372 chatglm-cli-0.1.1/chatglmcli/
+-rw-r--r--   0 mroy       (501) staff       (20)        0 2023-06-28 09:19:02.000000 chatglm-cli-0.1.1/chatglmcli/__init__.py
+-rw-r--r--   0 mroy       (501) staff       (20)     3856 2023-06-30 08:00:44.000000 chatglm-cli-0.1.1/chatglmcli/cmd.py
+-rw-r--r--   0 mroy       (501) staff       (20)       38 2023-06-30 08:01:05.318674 chatglm-cli-0.1.1/setup.cfg
+-rw-r--r--   0 mroy       (501) staff       (20)     1200 2023-06-30 08:01:00.000000 chatglm-cli-0.1.1/setup.py
```

### Comparing `chatglm-cli-0.0.1/chatglmcli/cmd.py` & `chatglm-cli-0.1.1/chatglmcli/cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,9 +103,9 @@
 
         submitBtn.click(predict, [user_input, chatbot, max_length, top_p, temperature, history, past_key_values],
                         [chatbot, history, past_key_values], show_progress=True)
         submitBtn.click(reset_user_input, [], [user_input])
 
         emptyBtn.click(reset_state, outputs=[chatbot, history, past_key_values], show_progress=True)
 
-    demo.queue(concurrency_count=10).launch(share=False, inbrowser=True)
+    demo.queue(concurrency_count=10).launch(share=False, inbrowser=True,server_name="0.0.0.0", server_port=17888)
```

### Comparing `chatglm-cli-0.0.1/setup.py` & `chatglm-cli-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 
 setup(name='chatglm-cli',
-    version='0.0.1',
+    version='0.1.1',
     description='chatglm llm cli',
     url='https://github.com/xxx',
     author='auth',
     author_email='xxx@gmail.com',
     license='MIT',
     include_package_data=True,
     zip_safe=False,
@@ -35,15 +35,15 @@
         # 'numpy',
         # 'pypdf',
         # "scikit-learn",
         # 'langchain',
         # 'websockets',
         # 'websocket-client',
         'gradio',
-        'chatglm-llm',
+        'chatglm-llm>=1.4.3',
         # 'unstructured',
         # 'aiowebsocket',
         ],
     entry_points={
         'console_scripts': [
             'ai-cli=chatglmcli.cmd:main',
         ]
```

