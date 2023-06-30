# Comparing `tmp/ag_llama_api-0.0.8.tar.gz` & `tmp/ag_llama_api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ag_llama_api-0.0.8.tar", last modified: Thu Jun 29 14:41:58 2023, max compression
+gzip compressed data, was "dist\ag_llama_api-0.0.9.tar", last modified: Thu Jun 29 15:06:56 2023, max compression
```

## Comparing `ag_llama_api-0.0.8.tar` & `ag_llama_api-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 14:41:58.160498 ag_llama_api-0.0.8/
--rw-rw-rw-   0        0        0      764 2023-06-29 14:41:58.159508 ag_llama_api-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 14:41:58.140162 ag_llama_api-0.0.8/ag_llama_api/
--rw-rw-rw-   0        0        0     2186 2023-06-27 12:34:01.000000 ag_llama_api-0.0.8/ag_llama_api/__init__.py
--rw-rw-rw-   0        0        0     9143 2023-06-29 13:58:28.000000 ag_llama_api-0.0.8/ag_llama_api/__main__.py
--rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_api-0.0.8/ag_llama_api/choice.py
--rw-rw-rw-   0        0        0    13782 2023-06-29 14:41:54.000000 ag_llama_api-0.0.8/ag_llama_api/model.py
--rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_api-0.0.8/ag_llama_api/tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:41:58.149090 ag_llama_api-0.0.8/ag_llama_api.egg-info/
--rw-rw-rw-   0        0        0      764 2023-06-29 14:41:58.000000 ag_llama_api-0.0.8/ag_llama_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2023-06-29 14:41:58.000000 ag_llama_api-0.0.8/ag_llama_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 14:41:58.000000 ag_llama_api-0.0.8/ag_llama_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      305 2023-06-29 14:41:58.000000 ag_llama_api-0.0.8/ag_llama_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-29 14:41:58.000000 ag_llama_api-0.0.8/ag_llama_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 14:41:58.160994 ag_llama_api-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2567 2023-06-29 13:52:31.000000 ag_llama_api-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:41:58.154050 ag_llama_api-0.0.8/tests/
--rw-rw-rw-   0        0        0     1121 2023-06-28 17:09:17.000000 ag_llama_api-0.0.8/tests/test_choice.py
--rw-rw-rw-   0        0        0     2982 2023-06-10 04:41:23.000000 ag_llama_api-0.0.8/tests/test_model.py
--rw-rw-rw-   0        0        0     1945 2023-06-10 04:41:23.000000 ag_llama_api-0.0.8/tests/test_tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:41:58.157553 ag_llama_api-0.0.8/utils/
--rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_api-0.0.8/utils/download.py
--rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_api-0.0.8/utils/render.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:06:56.116680 ag_llama_api-0.0.9/
+-rw-rw-rw-   0        0        0      764 2023-06-29 15:06:56.115225 ag_llama_api-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-29 15:06:56.095848 ag_llama_api-0.0.9/ag_llama_api/
+-rw-rw-rw-   0        0        0     2186 2023-06-27 12:34:01.000000 ag_llama_api-0.0.9/ag_llama_api/__init__.py
+-rw-rw-rw-   0        0        0     9143 2023-06-29 13:58:28.000000 ag_llama_api-0.0.9/ag_llama_api/__main__.py
+-rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_api-0.0.9/ag_llama_api/choice.py
+-rw-rw-rw-   0        0        0    13842 2023-06-29 15:06:01.000000 ag_llama_api-0.0.9/ag_llama_api/model.py
+-rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_api-0.0.9/ag_llama_api/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:06:56.105272 ag_llama_api-0.0.9/ag_llama_api.egg-info/
+-rw-rw-rw-   0        0        0      764 2023-06-29 15:06:56.000000 ag_llama_api-0.0.9/ag_llama_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2023-06-29 15:06:56.000000 ag_llama_api-0.0.9/ag_llama_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 15:06:56.000000 ag_llama_api-0.0.9/ag_llama_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      305 2023-06-29 15:06:56.000000 ag_llama_api-0.0.9/ag_llama_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-29 15:06:56.000000 ag_llama_api-0.0.9/ag_llama_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 15:06:56.116680 ag_llama_api-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2567 2023-06-29 13:52:31.000000 ag_llama_api-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:06:56.110231 ag_llama_api-0.0.9/tests/
+-rw-rw-rw-   0        0        0     1121 2023-06-28 17:09:17.000000 ag_llama_api-0.0.9/tests/test_choice.py
+-rw-rw-rw-   0        0        0     2982 2023-06-10 04:41:23.000000 ag_llama_api-0.0.9/tests/test_model.py
+-rw-rw-rw-   0        0        0     1945 2023-06-10 04:41:23.000000 ag_llama_api-0.0.9/tests/test_tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:06:56.113702 ag_llama_api-0.0.9/utils/
+-rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_api-0.0.9/utils/download.py
+-rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_api-0.0.9/utils/render.py
```

### Comparing `ag_llama_api-0.0.8/PKG-INFO` & `ag_llama_api-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag_llama_api
-Version: 0.0.8
+Version: 0.0.9
 Summary: ag_llama_api Test Package for Somthing
 Author: AA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ag_llama_api-0.0.8/ag_llama_api/__init__.py` & `ag_llama_api-0.0.9/ag_llama_api/__init__.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api-0.0.8/ag_llama_api/__main__.py` & `ag_llama_api-0.0.9/ag_llama_api/__main__.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api-0.0.8/ag_llama_api/choice.py` & `ag_llama_api-0.0.9/ag_llama_api/choice.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api-0.0.8/ag_llama_api/model.py` & `ag_llama_api-0.0.9/ag_llama_api/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,14 +306,15 @@
         nvidia_smi.nvmlInit()
         gpus_count = nvidia_smi.nvmlDeviceGetCount()
         logger.debug(f"Found {gpus_count} GPUs")
         handles = []
         for index in range(gpus_count):
             try:
                 handles.append(nvidia_smi.nvmlDeviceGetHandleByIndex(index))
+                logger.debug(f"Got handle for GPU {index}")
             except Exception as e:
                 logger.error(f"Failed to get handle for GPU {index}: {e}")
         
         for handle in handles:
             logger.debug(f"GPU {handle} memory info: {nvidia_smi.nvmlDeviceGetMemoryInfo(handle)}")
         
         logger.debug("Clearing GPU cache")
```

### Comparing `ag_llama_api-0.0.8/ag_llama_api/tokenizer.py` & `ag_llama_api-0.0.9/ag_llama_api/tokenizer.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api-0.0.8/ag_llama_api.egg-info/PKG-INFO` & `ag_llama_api-0.0.9/ag_llama_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag-llama-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: ag_llama_api Test Package for Somthing
 Author: AA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ag_llama_api-0.0.8/setup.py` & `ag_llama_api-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api-0.0.8/tests/test_choice.py` & `ag_llama_api-0.0.9/tests/test_choice.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api-0.0.8/tests/test_model.py` & `ag_llama_api-0.0.9/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api-0.0.8/tests/test_tokenizer.py` & `ag_llama_api-0.0.9/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api-0.0.8/utils/download.py` & `ag_llama_api-0.0.9/utils/download.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api-0.0.8/utils/render.py` & `ag_llama_api-0.0.9/utils/render.py`

 * *Files identical despite different names*

