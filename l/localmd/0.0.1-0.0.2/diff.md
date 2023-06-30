# Comparing `tmp/localmd-0.0.1.tar.gz` & `tmp/localmd-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localmd-0.0.1.tar", last modified: Thu Jun 29 23:42:50 2023, max compression
+gzip compressed data, was "localmd-0.0.2.tar", last modified: Fri Jun 30 00:23:57 2023, max compression
```

## Comparing `localmd-0.0.1.tar` & `localmd-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 app2139   (1001) app2139   (1002)        0 2023-06-29 23:42:50.870629 localmd-0.0.1/
--rw-rw-r--   0 app2139   (1001) app2139   (1002)    35149 2022-08-31 20:35:38.000000 localmd-0.0.1/LICENSE
--rw-rw-r--   0 app2139   (1001) app2139   (1002)      269 2023-06-29 23:42:50.870629 localmd-0.0.1/PKG-INFO
--rw-rw-r--   0 app2139   (1001) app2139   (1002)       74 2022-08-31 20:35:38.000000 localmd-0.0.1/README.md
-drwxrwxr-x   0 app2139   (1001) app2139   (1002)        0 2023-06-29 23:42:50.866629 localmd-0.0.1/localmd/
--rw-rw-r--   0 app2139   (1001) app2139   (1002)        0 2022-08-31 20:39:26.000000 localmd-0.0.1/localmd/__init__.py
--rw-rw-r--   0 app2139   (1001) app2139   (1002)     1887 2023-06-29 20:25:19.000000 localmd-0.0.1/localmd/dataset.py
--rw-rw-r--   0 app2139   (1001) app2139   (1002)    26611 2023-06-29 21:52:01.000000 localmd-0.0.1/localmd/decomposition.py
--rw-rw-r--   0 app2139   (1001) app2139   (1002)     5918 2023-06-29 20:31:55.000000 localmd-0.0.1/localmd/evaluation.py
--rw-rw-r--   0 app2139   (1001) app2139   (1002)    22915 2023-06-29 21:42:49.000000 localmd-0.0.1/localmd/pmd_loader.py
--rw-rw-r--   0 app2139   (1001) app2139   (1002)     2602 2023-06-16 20:53:54.000000 localmd-0.0.1/localmd/preprocessing_utils.py
--rw-rw-r--   0 app2139   (1001) app2139   (1002)     3726 2023-06-29 21:09:18.000000 localmd-0.0.1/localmd/visualization.py
-drwxrwxr-x   0 app2139   (1001) app2139   (1002)        0 2023-06-29 23:42:50.866629 localmd-0.0.1/localmd.egg-info/
-drwxrwxr-x   0 app2139   (1001) app2139   (1002)        0 2023-06-29 23:42:50.870629 localmd-0.0.1/localmd.egg-info/.ipynb_checkpoints/
--rw-rw-r--   0 app2139   (1001) app2139   (1002)      212 2023-06-09 20:26:25.000000 localmd-0.0.1/localmd.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
--rw-rw-r--   0 app2139   (1001) app2139   (1002)      296 2023-06-09 20:26:25.000000 localmd-0.0.1/localmd.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-rw-r--   0 app2139   (1001) app2139   (1002)        1 2023-06-09 20:26:25.000000 localmd-0.0.1/localmd.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
--rw-rw-r--   0 app2139   (1001) app2139   (1002)      269 2023-06-29 23:42:50.000000 localmd-0.0.1/localmd.egg-info/PKG-INFO
--rw-rw-r--   0 app2139   (1001) app2139   (1002)      527 2023-06-29 23:42:50.000000 localmd-0.0.1/localmd.egg-info/SOURCES.txt
--rw-rw-r--   0 app2139   (1001) app2139   (1002)        1 2023-06-29 23:42:50.000000 localmd-0.0.1/localmd.egg-info/dependency_links.txt
--rw-rw-r--   0 app2139   (1001) app2139   (1002)       99 2023-06-29 23:42:50.000000 localmd-0.0.1/localmd.egg-info/requires.txt
--rw-rw-r--   0 app2139   (1001) app2139   (1002)        8 2023-06-29 23:42:50.000000 localmd-0.0.1/localmd.egg-info/top_level.txt
--rw-rw-r--   0 app2139   (1001) app2139   (1002)       38 2023-06-29 23:42:50.870629 localmd-0.0.1/setup.cfg
--rw-rw-r--   0 app2139   (1001) app2139   (1002)      830 2023-06-29 23:42:15.000000 localmd-0.0.1/setup.py
+drwxrwxr-x   0 app2139   (1001) app2139   (1002)        0 2023-06-30 00:23:57.942933 localmd-0.0.2/
+-rw-rw-r--   0 app2139   (1001) app2139   (1002)    35149 2022-08-31 20:35:38.000000 localmd-0.0.2/LICENSE
+-rw-rw-r--   0 app2139   (1001) app2139   (1002)      269 2023-06-30 00:23:57.942933 localmd-0.0.2/PKG-INFO
+-rw-rw-r--   0 app2139   (1001) app2139   (1002)       74 2022-08-31 20:35:38.000000 localmd-0.0.2/README.md
+drwxrwxr-x   0 app2139   (1001) app2139   (1002)        0 2023-06-30 00:23:57.942933 localmd-0.0.2/localmd/
+-rw-rw-r--   0 app2139   (1001) app2139   (1002)        0 2022-08-31 20:39:26.000000 localmd-0.0.2/localmd/__init__.py
+-rw-rw-r--   0 app2139   (1001) app2139   (1002)     1887 2023-06-29 20:25:19.000000 localmd-0.0.2/localmd/dataset.py
+-rw-rw-r--   0 app2139   (1001) app2139   (1002)    26611 2023-06-29 21:52:01.000000 localmd-0.0.2/localmd/decomposition.py
+-rw-rw-r--   0 app2139   (1001) app2139   (1002)     5918 2023-06-29 20:31:55.000000 localmd-0.0.2/localmd/evaluation.py
+-rw-rw-r--   0 app2139   (1001) app2139   (1002)    22915 2023-06-29 21:42:49.000000 localmd-0.0.2/localmd/pmd_loader.py
+-rw-rw-r--   0 app2139   (1001) app2139   (1002)     2602 2023-06-16 20:53:54.000000 localmd-0.0.2/localmd/preprocessing_utils.py
+-rw-rw-r--   0 app2139   (1001) app2139   (1002)     3726 2023-06-29 21:09:18.000000 localmd-0.0.2/localmd/visualization.py
+drwxrwxr-x   0 app2139   (1001) app2139   (1002)        0 2023-06-30 00:23:57.942933 localmd-0.0.2/localmd.egg-info/
+drwxrwxr-x   0 app2139   (1001) app2139   (1002)        0 2023-06-30 00:23:57.942933 localmd-0.0.2/localmd.egg-info/.ipynb_checkpoints/
+-rw-rw-r--   0 app2139   (1001) app2139   (1002)      212 2023-06-09 20:26:25.000000 localmd-0.0.2/localmd.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
+-rw-rw-r--   0 app2139   (1001) app2139   (1002)      296 2023-06-09 20:26:25.000000 localmd-0.0.2/localmd.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-rw-r--   0 app2139   (1001) app2139   (1002)        1 2023-06-09 20:26:25.000000 localmd-0.0.2/localmd.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
+-rw-rw-r--   0 app2139   (1001) app2139   (1002)      269 2023-06-30 00:23:57.000000 localmd-0.0.2/localmd.egg-info/PKG-INFO
+-rw-rw-r--   0 app2139   (1001) app2139   (1002)      527 2023-06-30 00:23:57.000000 localmd-0.0.2/localmd.egg-info/SOURCES.txt
+-rw-rw-r--   0 app2139   (1001) app2139   (1002)        1 2023-06-30 00:23:57.000000 localmd-0.0.2/localmd.egg-info/dependency_links.txt
+-rw-rw-r--   0 app2139   (1001) app2139   (1002)      110 2023-06-30 00:23:57.000000 localmd-0.0.2/localmd.egg-info/requires.txt
+-rw-rw-r--   0 app2139   (1001) app2139   (1002)        8 2023-06-30 00:23:57.000000 localmd-0.0.2/localmd.egg-info/top_level.txt
+-rw-rw-r--   0 app2139   (1001) app2139   (1002)       38 2023-06-30 00:23:57.942933 localmd-0.0.2/setup.cfg
+-rw-rw-r--   0 app2139   (1001) app2139   (1002)      843 2023-06-30 00:23:35.000000 localmd-0.0.2/setup.py
```

### Comparing `localmd-0.0.1/LICENSE` & `localmd-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `localmd-0.0.1/localmd/dataset.py` & `localmd-0.0.2/localmd/dataset.py`

 * *Files identical despite different names*

### Comparing `localmd-0.0.1/localmd/decomposition.py` & `localmd-0.0.2/localmd/decomposition.py`

 * *Files identical despite different names*

### Comparing `localmd-0.0.1/localmd/evaluation.py` & `localmd-0.0.2/localmd/evaluation.py`

 * *Files identical despite different names*

### Comparing `localmd-0.0.1/localmd/pmd_loader.py` & `localmd-0.0.2/localmd/pmd_loader.py`

 * *Files identical despite different names*

### Comparing `localmd-0.0.1/localmd/preprocessing_utils.py` & `localmd-0.0.2/localmd/preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `localmd-0.0.1/localmd/visualization.py` & `localmd-0.0.2/localmd/visualization.py`

 * *Files identical despite different names*

### Comparing `localmd-0.0.1/localmd.egg-info/SOURCES.txt` & `localmd-0.0.2/localmd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localmd-0.0.1/setup.py` & `localmd-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from setuptools import setup, find_packages
 from os import path
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-
 min_jax_version = "0.4.7"
 
 setup(
     name='localmd',
     description="Method for compressing calcium imaging data using spatially localized low-rank matrix decompositions",
     author='Amol Pasarkar',
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(),
     include_package_data=True,
-    install_requires=["numpy", "tifffile", "scipy", "tqdm", "jax>={}".format(min_jax_version), "jaxlib>={}".format(min_jax_version)],
+    install_requires=["numpy", "tifffile", "scipy", "jupyterlab", "tqdm", "jax>={}".format(min_jax_version), "jaxlib>={}".format(min_jax_version)],
     python_requires='>=3.8',
     extras_require={
         "cpu": "jax[cpu]>={}".format(min_jax_version),
         # CUDA: pip install localmd[cuda] -f https://storage.googleapis.com/jax-releases/jax_releases.html
         "cuda": "jax[cuda]>={}".format(min_jax_version),
     },
 )
```

