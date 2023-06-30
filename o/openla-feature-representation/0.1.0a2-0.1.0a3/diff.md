# Comparing `tmp/openla_feature_representation-0.1.0a2.tar.gz` & `tmp/openla_feature_representation-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openla_feature_representation-0.1.0a2.tar", max compression
+gzip compressed data, was "openla_feature_representation-0.1.0a3.tar", max compression
```

## Comparing `openla_feature_representation-0.1.0a2.tar` & `openla_feature_representation-0.1.0a3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1061 2023-06-12 07:23:54.810526 openla_feature_representation-0.1.0a2/LICENSE
--rw-r--r--   0        0        0     1183 2023-06-23 06:28:03.604738 openla_feature_representation-0.1.0a2/README.md
--rw-r--r--   0        0        0       32 2023-06-23 06:28:03.604924 openla_feature_representation-0.1.0a2/openla_feature_representation/__init__.py
--rw-r--r--   0        0        0    15978 2023-06-23 06:28:03.605122 openla_feature_representation-0.1.0a2/openla_feature_representation/openla_e2vec.py
--rw-r--r--   0        0        0      485 2023-06-23 06:30:16.971431 openla_feature_representation-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0     1825 1970-01-01 00:00:00.000000 openla_feature_representation-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-12 07:23:54.810526 openla_feature_representation-0.1.0a3/LICENSE
+-rw-r--r--   0        0        0     1183 2023-06-30 01:56:26.082473 openla_feature_representation-0.1.0a3/README.md
+-rw-r--r--   0        0        0       32 2023-06-23 06:28:03.604924 openla_feature_representation-0.1.0a3/openla_feature_representation/__init__.py
+-rw-r--r--   0        0        0    15978 2023-06-28 05:02:19.897260 openla_feature_representation-0.1.0a3/openla_feature_representation/openla_e2vec.py
+-rw-r--r--   0        0        0      478 2023-06-30 01:56:34.966128 openla_feature_representation-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0     1818 1970-01-01 00:00:00.000000 openla_feature_representation-0.1.0a3/PKG-INFO
```

### Comparing `openla_feature_representation-0.1.0a2/LICENSE` & `openla_feature_representation-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `openla_feature_representation-0.1.0a2/README.md` & `openla_feature_representation-0.1.0a3/README.md`

 * *Files identical despite different names*

### Comparing `openla_feature_representation-0.1.0a2/openla_feature_representation/openla_e2vec.py` & `openla_feature_representation-0.1.0a3/openla_feature_representation/openla_e2vec.py`

 * *Files identical despite different names*

### Comparing `openla_feature_representation-0.1.0a2/PKG-INFO` & `openla_feature_representation-0.1.0a3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: openla-feature-representation
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: A Python module that adds features to OpenLA data to make it easier to use for ML
-Author: Yuma Miyazaki
-Author-email: miyazaki@limu.ait.kyushu-u.ac.jp
+Author: LIMU
+Author-email: repository@limu.ait.kyushu-u.ac.jp
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fasttext-wheel (>=0.9.2,<0.10.0)
```

