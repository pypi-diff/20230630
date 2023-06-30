# Comparing `tmp/distool-0.1.8.tar.gz` & `tmp/distool-0.1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distool-0.1.8.tar", last modified: Fri Jun 30 07:15:07 2023, max compression
+gzip compressed data, was "distool-0.1.8.1.tar", last modified: Fri Jun 30 07:16:58 2023, max compression
```

## Comparing `distool-0.1.8.tar` & `distool-0.1.8.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:15:07.119969 distool-0.1.8/
--rw-r--r--   0 michilegorov   (501) staff       (20)     1068 2023-02-27 19:53:19.000000 distool-0.1.8/LICENSE.txt
--rw-r--r--   0 michilegorov   (501) staff       (20)     5957 2023-06-30 07:15:07.120061 distool-0.1.8/PKG-INFO
--rw-r--r--   0 michilegorov   (501) staff       (20)     5129 2023-06-30 07:09:08.000000 distool-0.1.8/README.md
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:15:07.110573 distool-0.1.8/distool/
--rw-r--r--   0 michilegorov   (501) staff       (20)      284 2023-06-30 07:00:58.000000 distool-0.1.8/distool/__init__.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:15:07.111796 distool-0.1.8/distool/base/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.8/distool/base/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      569 2023-02-27 19:15:03.000000 distool-0.1.8/distool/base/estimators.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:15:07.112053 distool-0.1.8/distool/data/
--rw-r--r--   0 michilegorov   (501) staff       (20)   240820 2023-06-11 14:13:26.000000 distool-0.1.8/distool/data/symptoms.json
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:15:07.113611 distool-0.1.8/distool/estimators/
--rw-r--r--   0 michilegorov   (501) staff       (20)      140 2023-06-30 07:00:58.000000 distool-0.1.8/distool/estimators/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     2151 2023-06-30 07:00:58.000000 distool-0.1.8/distool/estimators/classifiers.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:15:07.115765 distool-0.1.8/distool/feature_extraction/
--rw-r--r--   0 michilegorov   (501) staff       (20)      209 2023-06-29 20:39:26.000000 distool-0.1.8/distool/feature_extraction/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     3539 2023-06-29 20:39:26.000000 distool-0.1.8/distool/feature_extraction/anamnesis.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     1100 2023-06-29 20:39:26.000000 distool-0.1.8/distool/feature_extraction/dumb_extractor.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     4973 2023-06-29 20:39:26.000000 distool-0.1.8/distool/feature_extraction/smart_extractor.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      499 2023-03-12 08:11:10.000000 distool-0.1.8/distool/feature_extraction/symptom.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     2505 2023-03-25 07:58:05.000000 distool-0.1.8/distool/feature_extraction/symptom_collection.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      327 2023-02-27 19:15:03.000000 distool-0.1.8/distool/feature_extraction/symptom_status.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:15:07.116172 distool-0.1.8/distool/interpretation/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.8/distool/interpretation/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     2514 2023-06-30 07:00:58.000000 distool-0.1.8/distool/interpretation/explainer.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:15:07.116443 distool-0.1.8/distool/metrics/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-06-11 14:13:04.000000 distool-0.1.8/distool/metrics/__init__.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:15:07.116922 distool-0.1.8/distool/metrics/extractor/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-06-11 14:13:04.000000 distool-0.1.8/distool/metrics/extractor/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     2475 2023-06-11 14:13:26.000000 distool-0.1.8/distool/metrics/extractor/compute.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     7709 2023-06-29 20:39:26.000000 distool-0.1.8/distool/metrics/extractor/create_showcase.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:15:07.117375 distool-0.1.8/distool/models/
--rw-r--r--   0 michilegorov   (501) staff       (20)      144 2023-06-30 07:00:58.000000 distool-0.1.8/distool/models/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     3360 2023-06-29 20:39:26.000000 distool-0.1.8/distool/models/urgency_classifier.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:15:07.117961 distool-0.1.8/distool/tests/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.8/distool/tests/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      959 2023-06-30 07:00:58.000000 distool-0.1.8/distool/tests/conftest.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:15:07.118583 distool-0.1.8/distool/tests/estimators/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:00:58.000000 distool-0.1.8/distool/tests/estimators/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      419 2023-06-30 07:00:58.000000 distool-0.1.8/distool/tests/estimators/test_classifier.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      787 2023-06-30 07:00:58.000000 distool-0.1.8/distool/tests/estimators/test_fedot_classifier.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:15:07.118909 distool-0.1.8/distool/tests/explainer/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.8/distool/tests/explainer/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     1346 2023-06-30 07:00:58.000000 distool-0.1.8/distool/tests/explainer/test_explainer.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:15:07.119245 distool-0.1.8/distool/tests/extractors/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.8/distool/tests/extractors/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     1630 2023-06-29 20:39:26.000000 distool-0.1.8/distool/tests/extractors/test_symptom_extractor.py
--rw-r--r--   0 michilegorov   (501) staff       (20)       37 2023-02-27 19:15:03.000000 distool-0.1.8/distool/tests/test_base.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:15:07.111510 distool-0.1.8/distool.egg-info/
--rw-r--r--   0 michilegorov   (501) staff       (20)     5957 2023-06-30 07:15:07.000000 distool-0.1.8/distool.egg-info/PKG-INFO
--rw-r--r--   0 michilegorov   (501) staff       (20)     1384 2023-06-30 07:15:07.000000 distool-0.1.8/distool.egg-info/SOURCES.txt
--rw-r--r--   0 michilegorov   (501) staff       (20)        1 2023-06-30 07:15:07.000000 distool-0.1.8/distool.egg-info/dependency_links.txt
--rw-r--r--   0 michilegorov   (501) staff       (20)       64 2023-06-30 07:15:07.000000 distool-0.1.8/distool.egg-info/requires.txt
--rw-r--r--   0 michilegorov   (501) staff       (20)       17 2023-06-30 07:15:07.000000 distool-0.1.8/distool.egg-info/top_level.txt
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:15:07.119703 distool-0.1.8/examples/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-04 10:03:31.000000 distool-0.1.8/examples/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     1116 2023-06-29 20:39:26.000000 distool-0.1.8/examples/pipeline_example.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      115 2023-02-04 10:03:31.000000 distool-0.1.8/pyproject.toml
--rw-r--r--   0 michilegorov   (501) staff       (20)       79 2023-06-30 07:15:07.120322 distool-0.1.8/setup.cfg
--rw-r--r--   0 michilegorov   (501) staff       (20)     1314 2023-06-30 07:15:00.000000 distool-0.1.8/setup.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:16:58.389843 distool-0.1.8.1/
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1068 2023-02-27 19:53:19.000000 distool-0.1.8.1/LICENSE.txt
+-rw-r--r--   0 michilegorov   (501) staff       (20)     5975 2023-06-30 07:16:58.389960 distool-0.1.8.1/PKG-INFO
+-rw-r--r--   0 michilegorov   (501) staff       (20)     5129 2023-06-30 07:09:08.000000 distool-0.1.8.1/README.md
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:16:58.380377 distool-0.1.8.1/distool/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      284 2023-06-30 07:00:58.000000 distool-0.1.8.1/distool/__init__.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:16:58.381682 distool-0.1.8.1/distool/base/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.8.1/distool/base/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      569 2023-02-27 19:15:03.000000 distool-0.1.8.1/distool/base/estimators.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:16:58.382092 distool-0.1.8.1/distool/data/
+-rw-r--r--   0 michilegorov   (501) staff       (20)   240820 2023-06-11 14:13:26.000000 distool-0.1.8.1/distool/data/symptoms.json
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:16:58.383109 distool-0.1.8.1/distool/estimators/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      140 2023-06-30 07:00:58.000000 distool-0.1.8.1/distool/estimators/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     2151 2023-06-30 07:00:58.000000 distool-0.1.8.1/distool/estimators/classifiers.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:16:58.385054 distool-0.1.8.1/distool/feature_extraction/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      209 2023-06-29 20:39:26.000000 distool-0.1.8.1/distool/feature_extraction/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     3539 2023-06-29 20:39:26.000000 distool-0.1.8.1/distool/feature_extraction/anamnesis.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1100 2023-06-29 20:39:26.000000 distool-0.1.8.1/distool/feature_extraction/dumb_extractor.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     4973 2023-06-29 20:39:26.000000 distool-0.1.8.1/distool/feature_extraction/smart_extractor.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      499 2023-03-12 08:11:10.000000 distool-0.1.8.1/distool/feature_extraction/symptom.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     2505 2023-03-25 07:58:05.000000 distool-0.1.8.1/distool/feature_extraction/symptom_collection.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      327 2023-02-27 19:15:03.000000 distool-0.1.8.1/distool/feature_extraction/symptom_status.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:16:58.385501 distool-0.1.8.1/distool/interpretation/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.8.1/distool/interpretation/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     2514 2023-06-30 07:00:58.000000 distool-0.1.8.1/distool/interpretation/explainer.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:16:58.385813 distool-0.1.8.1/distool/metrics/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-06-11 14:13:04.000000 distool-0.1.8.1/distool/metrics/__init__.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:16:58.386319 distool-0.1.8.1/distool/metrics/extractor/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-06-11 14:13:04.000000 distool-0.1.8.1/distool/metrics/extractor/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     2475 2023-06-11 14:13:26.000000 distool-0.1.8.1/distool/metrics/extractor/compute.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     7709 2023-06-29 20:39:26.000000 distool-0.1.8.1/distool/metrics/extractor/create_showcase.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:16:58.386821 distool-0.1.8.1/distool/models/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      144 2023-06-30 07:00:58.000000 distool-0.1.8.1/distool/models/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     3360 2023-06-29 20:39:26.000000 distool-0.1.8.1/distool/models/urgency_classifier.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:16:58.387522 distool-0.1.8.1/distool/tests/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.8.1/distool/tests/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      959 2023-06-30 07:00:58.000000 distool-0.1.8.1/distool/tests/conftest.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:16:58.388400 distool-0.1.8.1/distool/tests/estimators/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:00:58.000000 distool-0.1.8.1/distool/tests/estimators/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      419 2023-06-30 07:00:58.000000 distool-0.1.8.1/distool/tests/estimators/test_classifier.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      787 2023-06-30 07:00:58.000000 distool-0.1.8.1/distool/tests/estimators/test_fedot_classifier.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:16:58.388749 distool-0.1.8.1/distool/tests/explainer/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.8.1/distool/tests/explainer/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1346 2023-06-30 07:00:58.000000 distool-0.1.8.1/distool/tests/explainer/test_explainer.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:16:58.389085 distool-0.1.8.1/distool/tests/extractors/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.8.1/distool/tests/extractors/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1630 2023-06-29 20:39:26.000000 distool-0.1.8.1/distool/tests/extractors/test_symptom_extractor.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)       37 2023-02-27 19:15:03.000000 distool-0.1.8.1/distool/tests/test_base.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:16:58.381302 distool-0.1.8.1/distool.egg-info/
+-rw-r--r--   0 michilegorov   (501) staff       (20)     5975 2023-06-30 07:16:58.000000 distool-0.1.8.1/distool.egg-info/PKG-INFO
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1384 2023-06-30 07:16:58.000000 distool-0.1.8.1/distool.egg-info/SOURCES.txt
+-rw-r--r--   0 michilegorov   (501) staff       (20)        1 2023-06-30 07:16:58.000000 distool-0.1.8.1/distool.egg-info/dependency_links.txt
+-rw-r--r--   0 michilegorov   (501) staff       (20)       64 2023-06-30 07:16:58.000000 distool-0.1.8.1/distool.egg-info/requires.txt
+-rw-r--r--   0 michilegorov   (501) staff       (20)       17 2023-06-30 07:16:58.000000 distool-0.1.8.1/distool.egg-info/top_level.txt
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-30 07:16:58.389531 distool-0.1.8.1/examples/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-04 10:03:31.000000 distool-0.1.8.1/examples/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1116 2023-06-29 20:39:26.000000 distool-0.1.8.1/examples/pipeline_example.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      115 2023-02-04 10:03:31.000000 distool-0.1.8.1/pyproject.toml
+-rw-r--r--   0 michilegorov   (501) staff       (20)       79 2023-06-30 07:16:58.390296 distool-0.1.8.1/setup.cfg
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1332 2023-06-30 07:16:55.000000 distool-0.1.8.1/setup.py
```

### Comparing `distool-0.1.8/LICENSE.txt` & `distool-0.1.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `distool-0.1.8/PKG-INFO` & `distool-0.1.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: distool
-Version: 0.1.8
-Summary: Disease processing tool kit
+Version: 0.1.8.1
+Summary: Disease processing tool kit in Russian
 Home-page: https://github.com/nirma-patient-intake/disease/
 Download-URL: https://github.com/NIRMA-PATIENT-INTAKE/disease/archive/refs/tags/distool.tar.gz
 Author: NIRMA Team of ITMO University
 Author-email: egorovmichil9@gmail.com
 License: MIT
 Keywords: NLP,Disease,Health Condition
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: markdown
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Классификатор заболеваний
 
 **Patient-intake** - модуль, обеспечивающий дистанционное взаимодействие пациента и медицинского учреждения с помощью диалоговых агентов. Реализован на языке Python.
 
 Модуль позволяет предсказывать возможное заболевание пациента на основе введенной им информации, присваивать диагнозу степень срочности приема, а также выводить интерпретацию результатов работы модели. Для обучения модели создан датасет, содержащий информацию о болезнях и их симптомах.
```

### Comparing `distool-0.1.8/README.md` & `distool-0.1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `distool-0.1.8/distool/base/estimators.py` & `distool-0.1.8.1/distool/base/estimators.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.8/distool/data/symptoms.json` & `distool-0.1.8.1/distool/data/symptoms.json`

 * *Files identical despite different names*

### Comparing `distool-0.1.8/distool/estimators/classifiers.py` & `distool-0.1.8.1/distool/estimators/classifiers.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.8/distool/feature_extraction/anamnesis.py` & `distool-0.1.8.1/distool/feature_extraction/anamnesis.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.8/distool/feature_extraction/dumb_extractor.py` & `distool-0.1.8.1/distool/feature_extraction/dumb_extractor.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.8/distool/feature_extraction/smart_extractor.py` & `distool-0.1.8.1/distool/feature_extraction/smart_extractor.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.8/distool/feature_extraction/symptom_collection.py` & `distool-0.1.8.1/distool/feature_extraction/symptom_collection.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.8/distool/interpretation/explainer.py` & `distool-0.1.8.1/distool/interpretation/explainer.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.8/distool/metrics/extractor/compute.py` & `distool-0.1.8.1/distool/metrics/extractor/compute.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.8/distool/metrics/extractor/create_showcase.py` & `distool-0.1.8.1/distool/metrics/extractor/create_showcase.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.8/distool/models/urgency_classifier.py` & `distool-0.1.8.1/distool/models/urgency_classifier.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.8/distool/tests/conftest.py` & `distool-0.1.8.1/distool/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.8/distool/tests/estimators/test_fedot_classifier.py` & `distool-0.1.8.1/distool/tests/estimators/test_fedot_classifier.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.8/distool/tests/explainer/test_explainer.py` & `distool-0.1.8.1/distool/tests/explainer/test_explainer.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.8/distool/tests/extractors/test_symptom_extractor.py` & `distool-0.1.8.1/distool/tests/extractors/test_symptom_extractor.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.8/distool.egg-info/PKG-INFO` & `distool-0.1.8.1/distool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: distool
-Version: 0.1.8
-Summary: Disease processing tool kit
+Version: 0.1.8.1
+Summary: Disease processing tool kit in Russian
 Home-page: https://github.com/nirma-patient-intake/disease/
 Download-URL: https://github.com/NIRMA-PATIENT-INTAKE/disease/archive/refs/tags/distool.tar.gz
 Author: NIRMA Team of ITMO University
 Author-email: egorovmichil9@gmail.com
 License: MIT
 Keywords: NLP,Disease,Health Condition
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: markdown
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Классификатор заболеваний
 
 **Patient-intake** - модуль, обеспечивающий дистанционное взаимодействие пациента и медицинского учреждения с помощью диалоговых агентов. Реализован на языке Python.
 
 Модуль позволяет предсказывать возможное заболевание пациента на основе введенной им информации, присваивать диагнозу степень срочности приема, а также выводить интерпретацию результатов работы модели. Для обучения модели создан датасет, содержащий информацию о болезнях и их симптомах.
```

### Comparing `distool-0.1.8/distool.egg-info/SOURCES.txt` & `distool-0.1.8.1/distool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `distool-0.1.8/examples/pipeline_example.py` & `distool-0.1.8.1/examples/pipeline_example.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.8/setup.py` & `distool-0.1.8.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from distutils.core import setup
 
 from setuptools import find_packages
 
 setup(
     name="distool",
+    description="Disease processing tool kit in Russian",
     packages=find_packages(),
     package_data={"distool": ["data/symptoms.json"]},
     include_package_data=True,
     long_description=open("./README.md").read(),
-    long_description_content_type="markdown",
-    version="0.1.8",
+    long_description_content_type="text/markdown",
+    version="0.1.8.1",
     license="MIT",
-    description="Disease processing tool kit",
     author="NIRMA Team of ITMO University",
     author_email="egorovmichil9@gmail.com",
     url="https://github.com/nirma-patient-intake/disease/",
     download_url="https://github.com/NIRMA-PATIENT-INTAKE/disease/archive/refs/tags/distool.tar.gz",
     keywords=[
         "NLP",
         "Disease",
```

