# Comparing `tmp/skga-0.0.9.tar.gz` & `tmp/skga-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skga-0.0.9.tar", last modified: Thu Jun 15 16:30:54 2023, max compression
+gzip compressed data, was "skga-1.0.0.tar", last modified: Fri Jun 30 02:37:04 2023, max compression
```

## Comparing `skga-0.0.9.tar` & `skga-1.0.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 16:30:54.421740 skga-0.0.9/
--rw-r--r--   0 leosauberman   (501) staff       (20)     1517 2023-05-07 22:28:59.000000 skga-0.0.9/LICENSE
--rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-15 16:30:54.421550 skga-0.0.9/PKG-INFO
--rw-r--r--   0 leosauberman   (501) staff       (20)      623 2023-05-07 22:04:48.000000 skga-0.0.9/README.md
--rw-r--r--   0 leosauberman   (501) staff       (20)     2126 2023-06-01 19:08:45.000000 skga-0.0.9/pyproject.toml
--rw-r--r--   0 leosauberman   (501) staff       (20)       38 2023-06-15 16:30:54.421985 skga-0.0.9/setup.cfg
--rw-r--r--   0 leosauberman   (501) staff       (20)     2425 2023-06-15 16:30:51.000000 skga-0.0.9/setup.py
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 16:30:54.410505 skga-0.0.9/skga/
--rw-r--r--   0 leosauberman   (501) staff       (20)       39 2023-06-15 12:11:54.000000 skga-0.0.9/skga/__init__.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     8659 2023-06-15 16:10:12.000000 skga-0.0.9/skga/adaptee.py
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 16:30:54.417715 skga-0.0.9/skga/hbrkga/
--rw-r--r--   0 leosauberman   (501) staff       (20)      308 2023-06-15 13:16:50.000000 skga-0.0.9/skga/hbrkga/__init__.py
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 16:30:54.421161 skga-0.0.9/skga/hbrkga/brkga_mp_ipr/
--rw-r--r--   0 leosauberman   (501) staff       (20)     1654 2023-05-07 22:04:48.000000 skga-0.0.9/skga/hbrkga/brkga_mp_ipr/__init__.py
--rw-r--r--   0 leosauberman   (501) staff       (20)    39540 2023-06-15 13:18:38.000000 skga-0.0.9/skga/hbrkga/brkga_mp_ipr/algorithm.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     5319 2023-05-07 22:04:48.000000 skga-0.0.9/skga/hbrkga/brkga_mp_ipr/enums.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     1293 2023-05-07 22:04:48.000000 skga-0.0.9/skga/hbrkga/brkga_mp_ipr/exceptions.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     1305 2023-06-15 13:18:16.000000 skga-0.0.9/skga/hbrkga/brkga_mp_ipr/exploitation_method.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     6571 2023-06-15 13:13:31.000000 skga-0.0.9/skga/hbrkga/brkga_mp_ipr/types.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     6239 2023-06-15 13:13:31.000000 skga-0.0.9/skga/hbrkga/brkga_mp_ipr/types_io.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     2803 2023-05-07 22:04:48.000000 skga-0.0.9/skga/hbrkga/data_utils.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     7539 2023-06-15 13:13:31.000000 skga-0.0.9/skga/hbrkga/exploitation_method_BO.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     7785 2023-06-15 13:19:37.000000 skga-0.0.9/skga/hbrkga/exploitation_method_BO_only_elites.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     3899 2023-06-15 13:13:31.000000 skga-0.0.9/skga/hbrkga/exploitation_method_random_search.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     2873 2023-06-15 13:13:31.000000 skga-0.0.9/skga/hbrkga/main-BO-only-elites.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     2575 2023-06-15 13:13:31.000000 skga-0.0.9/skga/hbrkga/main-BO.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     2585 2023-06-15 13:13:31.000000 skga-0.0.9/skga/hbrkga/main-randomwalk.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     1316 2023-06-15 13:13:31.000000 skga-0.0.9/skga/hbrkga/nn_decoder_PT.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     5042 2023-06-15 13:13:31.000000 skga-0.0.9/skga/hbrkga/nn_instance_PT.py
--rw-r--r--   0 leosauberman   (501) staff       (20)       62 2023-06-01 19:48:13.000000 skga-0.0.9/skga/hbrkga/test.py
--rw-r--r--   0 leosauberman   (501) staff       (20)    10790 2023-05-07 22:04:48.000000 skga-0.0.9/skga/main.py
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 16:30:54.413700 skga-0.0.9/skga.egg-info/
--rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-15 16:30:54.000000 skga-0.0.9/skga.egg-info/PKG-INFO
--rw-r--r--   0 leosauberman   (501) staff       (20)      848 2023-06-15 16:30:54.000000 skga-0.0.9/skga.egg-info/SOURCES.txt
--rw-r--r--   0 leosauberman   (501) staff       (20)        1 2023-06-15 16:30:54.000000 skga-0.0.9/skga.egg-info/dependency_links.txt
--rw-r--r--   0 leosauberman   (501) staff       (20)      850 2023-06-15 16:30:54.000000 skga-0.0.9/skga.egg-info/requires.txt
--rw-r--r--   0 leosauberman   (501) staff       (20)        5 2023-06-15 16:30:54.000000 skga-0.0.9/skga.egg-info/top_level.txt
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-30 02:37:04.496979 skga-1.0.0/
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1517 2023-06-16 20:19:28.000000 skga-1.0.0/LICENSE
+-rw-r--r--   0 leosauberman   (501) staff       (20)     3135 2023-06-30 02:37:04.496818 skga-1.0.0/PKG-INFO
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2397 2023-06-16 20:28:37.000000 skga-1.0.0/README.md
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2126 2023-06-16 20:19:28.000000 skga-1.0.0/pyproject.toml
+-rw-r--r--   0 leosauberman   (501) staff       (20)       38 2023-06-30 02:37:04.497075 skga-1.0.0/setup.cfg
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2425 2023-06-19 14:43:54.000000 skga-1.0.0/setup.py
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-30 02:37:04.491681 skga-1.0.0/skga/
+-rw-r--r--   0 leosauberman   (501) staff       (20)       39 2023-06-16 20:19:28.000000 skga-1.0.0/skga/__init__.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     8659 2023-06-16 20:19:28.000000 skga-1.0.0/skga/adaptee.py
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-30 02:37:04.495262 skga-1.0.0/skga/hbrkga/
+-rw-r--r--   0 leosauberman   (501) staff       (20)      308 2023-06-16 20:19:28.000000 skga-1.0.0/skga/hbrkga/__init__.py
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-30 02:37:04.496536 skga-1.0.0/skga/hbrkga/brkga_mp_ipr/
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1654 2023-06-16 20:19:28.000000 skga-1.0.0/skga/hbrkga/brkga_mp_ipr/__init__.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)    39540 2023-06-16 20:19:28.000000 skga-1.0.0/skga/hbrkga/brkga_mp_ipr/algorithm.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     5319 2023-06-16 20:19:28.000000 skga-1.0.0/skga/hbrkga/brkga_mp_ipr/enums.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1293 2023-06-16 20:19:28.000000 skga-1.0.0/skga/hbrkga/brkga_mp_ipr/exceptions.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1305 2023-06-16 20:19:28.000000 skga-1.0.0/skga/hbrkga/brkga_mp_ipr/exploitation_method.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     6571 2023-06-16 20:19:28.000000 skga-1.0.0/skga/hbrkga/brkga_mp_ipr/types.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     6239 2023-06-16 20:19:28.000000 skga-1.0.0/skga/hbrkga/brkga_mp_ipr/types_io.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2803 2023-06-16 20:19:28.000000 skga-1.0.0/skga/hbrkga/data_utils.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     7539 2023-06-16 20:19:28.000000 skga-1.0.0/skga/hbrkga/exploitation_method_BO.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     7785 2023-06-16 20:19:28.000000 skga-1.0.0/skga/hbrkga/exploitation_method_BO_only_elites.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     3899 2023-06-16 20:19:28.000000 skga-1.0.0/skga/hbrkga/exploitation_method_random_search.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2873 2023-06-16 20:19:28.000000 skga-1.0.0/skga/hbrkga/main-BO-only-elites.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2575 2023-06-16 20:19:28.000000 skga-1.0.0/skga/hbrkga/main-BO.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2585 2023-06-16 20:19:28.000000 skga-1.0.0/skga/hbrkga/main-randomwalk.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1316 2023-06-16 20:19:28.000000 skga-1.0.0/skga/hbrkga/nn_decoder_PT.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     5042 2023-06-16 20:19:28.000000 skga-1.0.0/skga/hbrkga/nn_instance_PT.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)       62 2023-06-16 20:19:28.000000 skga-1.0.0/skga/hbrkga/test.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)    10790 2023-06-16 20:19:28.000000 skga-1.0.0/skga/main.py
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-30 02:37:04.492716 skga-1.0.0/skga.egg-info/
+-rw-r--r--   0 leosauberman   (501) staff       (20)     3135 2023-06-30 02:37:04.000000 skga-1.0.0/skga.egg-info/PKG-INFO
+-rw-r--r--   0 leosauberman   (501) staff       (20)      848 2023-06-30 02:37:04.000000 skga-1.0.0/skga.egg-info/SOURCES.txt
+-rw-r--r--   0 leosauberman   (501) staff       (20)        1 2023-06-30 02:37:04.000000 skga-1.0.0/skga.egg-info/dependency_links.txt
+-rw-r--r--   0 leosauberman   (501) staff       (20)      850 2023-06-30 02:37:04.000000 skga-1.0.0/skga.egg-info/requires.txt
+-rw-r--r--   0 leosauberman   (501) staff       (20)        5 2023-06-30 02:37:04.000000 skga-1.0.0/skga.egg-info/top_level.txt
```

### Comparing `skga-0.0.9/LICENSE` & `skga-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skga-0.0.9/pyproject.toml` & `skga-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skga-0.0.9/setup.py` & `skga-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="skga",
-    version="0.0.9",
+    version="1.0.0",
     description="The python package implementing the HyperBRKGA algorithm optimizes hyperparameters of machine learning algorithms through a hybrid approach based on genetic algorithms.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MLRG-CEFET-RJ/skga",
     author="Leonardo Sauberman, João Pedro Nogueira, Eduardo Bezerra",
     author_email="leonardo.moraes@aluno.cefet-rj.br, joao.carneiro@aluno.cefet-rj.br, ebezerra@cefet-rj.br",
     license="BSD License",
```

### Comparing `skga-0.0.9/skga/adaptee.py` & `skga-1.0.0/skga/adaptee.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.9/skga/hbrkga/brkga_mp_ipr/__init__.py` & `skga-1.0.0/skga/hbrkga/brkga_mp_ipr/__init__.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.9/skga/hbrkga/brkga_mp_ipr/algorithm.py` & `skga-1.0.0/skga/hbrkga/brkga_mp_ipr/algorithm.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.9/skga/hbrkga/brkga_mp_ipr/enums.py` & `skga-1.0.0/skga/hbrkga/brkga_mp_ipr/enums.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.9/skga/hbrkga/brkga_mp_ipr/exceptions.py` & `skga-1.0.0/skga/hbrkga/brkga_mp_ipr/exceptions.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.9/skga/hbrkga/brkga_mp_ipr/exploitation_method.py` & `skga-1.0.0/skga/hbrkga/brkga_mp_ipr/exploitation_method.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.9/skga/hbrkga/brkga_mp_ipr/types.py` & `skga-1.0.0/skga/hbrkga/brkga_mp_ipr/types.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.9/skga/hbrkga/brkga_mp_ipr/types_io.py` & `skga-1.0.0/skga/hbrkga/brkga_mp_ipr/types_io.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.9/skga/hbrkga/data_utils.py` & `skga-1.0.0/skga/hbrkga/data_utils.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.9/skga/hbrkga/exploitation_method_BO.py` & `skga-1.0.0/skga/hbrkga/exploitation_method_BO.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.9/skga/hbrkga/exploitation_method_BO_only_elites.py` & `skga-1.0.0/skga/hbrkga/exploitation_method_BO_only_elites.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.9/skga/hbrkga/exploitation_method_random_search.py` & `skga-1.0.0/skga/hbrkga/exploitation_method_random_search.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.9/skga/hbrkga/main-BO-only-elites.py` & `skga-1.0.0/skga/hbrkga/main-BO-only-elites.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.9/skga/hbrkga/main-BO.py` & `skga-1.0.0/skga/hbrkga/main-BO.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.9/skga/hbrkga/main-randomwalk.py` & `skga-1.0.0/skga/hbrkga/main-randomwalk.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.9/skga/hbrkga/nn_decoder_PT.py` & `skga-1.0.0/skga/hbrkga/nn_decoder_PT.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.9/skga/hbrkga/nn_instance_PT.py` & `skga-1.0.0/skga/hbrkga/nn_instance_PT.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.9/skga/main.py` & `skga-1.0.0/skga/main.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.9/skga.egg-info/SOURCES.txt` & `skga-1.0.0/skga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skga-0.0.9/skga.egg-info/requires.txt` & `skga-1.0.0/skga.egg-info/requires.txt`

 * *Files identical despite different names*

