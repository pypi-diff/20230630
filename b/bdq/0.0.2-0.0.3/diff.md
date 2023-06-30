# Comparing `tmp/bdq-0.0.2.tar.gz` & `tmp/bdq-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdq-0.0.2.tar", last modified: Fri Jun 30 12:38:57 2023, max compression
+gzip compressed data, was "bdq-0.0.3.tar", last modified: Fri Jun 30 12:47:54 2023, max compression
```

## Comparing `bdq-0.0.2.tar` & `bdq-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:38:57.897768 bdq-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 12:38:46.000000 bdq-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21028 2023-06-30 12:38:57.897768 bdq-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20421 2023-06-30 12:38:46.000000 bdq-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:38:57.893768 bdq-0.0.2/bdq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:38:57.893768 bdq-0.0.2/bdq/bdq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21028 2023-06-30 12:38:57.000000 bdq-0.0.2/bdq/bdq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-30 12:38:57.000000 bdq-0.0.2/bdq/bdq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:38:57.000000 bdq-0.0.2/bdq/bdq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:38:57.000000 bdq-0.0.2/bdq/bdq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-30 12:38:46.000000 bdq-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 12:38:57.897768 bdq-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:47:54.357176 bdq-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 12:47:44.000000 bdq-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21028 2023-06-30 12:47:54.357176 bdq-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20421 2023-06-30 12:47:44.000000 bdq-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:47:54.357176 bdq-0.0.3/bdq/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-30 12:47:44.000000 bdq-0.0.3/bdq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-06-30 12:47:44.000000 bdq-0.0.3/bdq/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-06-30 12:47:44.000000 bdq-0.0.3/bdq/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-30 12:47:44.000000 bdq-0.0.3/bdq/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-06-30 12:47:44.000000 bdq-0.0.3/bdq/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-06-30 12:47:44.000000 bdq-0.0.3/bdq/spark_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:47:54.357176 bdq-0.0.3/bdq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21028 2023-06-30 12:47:54.000000 bdq-0.0.3/bdq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-30 12:47:54.000000 bdq-0.0.3/bdq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:47:54.000000 bdq-0.0.3/bdq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-30 12:47:54.000000 bdq-0.0.3/bdq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-30 12:47:44.000000 bdq-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 12:47:54.357176 bdq-0.0.3/setup.cfg
```

### Comparing `bdq-0.0.2/LICENSE` & `bdq-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bdq-0.0.2/PKG-INFO` & `bdq-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6264 710a  : 2.1.Name: bdq.
-00000020: 5665 7273 696f 6e3a 2030 2e30 2e32 0a53  Version: 0.0.2.S
+00000020: 5665 7273 696f 6e3a 2030 2e30 2e33 0a53  Version: 0.0.3.S
 00000030: 756d 6d61 7279 3a20 4269 6720 4461 7461  ummary: Big Data
 00000040: 2051 7561 6c69 7479 2c20 6120 7365 7420   Quality, a set 
 00000050: 6f66 2074 6f6f 6c73 2f66 756e 6374 696f  of tools/functio
 00000060: 6e20 7468 6174 2068 656c 7020 796f 7520  n that help you 
 00000070: 6576 6572 7920 6461 7920 6173 7365 7274  every day assert
 00000080: 2071 7561 6c69 7479 206f 6620 6461 7461   quality of data
 00000090: 7365 7473 2079 6f75 2068 6176 6520 7072  sets you have pr
```

### Comparing `bdq-0.0.2/README.md` & `bdq-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bdq-0.0.2/bdq/bdq.egg-info/PKG-INFO` & `bdq-0.0.3/bdq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6264 710a  : 2.1.Name: bdq.
-00000020: 5665 7273 696f 6e3a 2030 2e30 2e32 0a53  Version: 0.0.2.S
+00000020: 5665 7273 696f 6e3a 2030 2e30 2e33 0a53  Version: 0.0.3.S
 00000030: 756d 6d61 7279 3a20 4269 6720 4461 7461  ummary: Big Data
 00000040: 2051 7561 6c69 7479 2c20 6120 7365 7420   Quality, a set 
 00000050: 6f66 2074 6f6f 6c73 2f66 756e 6374 696f  of tools/functio
 00000060: 6e20 7468 6174 2068 656c 7020 796f 7520  n that help you 
 00000070: 6576 6572 7920 6461 7920 6173 7365 7274  every day assert
 00000080: 2071 7561 6c69 7479 206f 6620 6461 7461   quality of data
 00000090: 7365 7473 2079 6f75 2068 6176 6520 7072  sets you have pr
```

