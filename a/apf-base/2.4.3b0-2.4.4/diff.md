# Comparing `tmp/apf_base-2.4.3b0.tar.gz` & `tmp/apf_base-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/APF/APF/dist/.tmp-ctlkk1p6/apf_base-2.4.3b0.tar", last modified: Thu Jun  8 16:52:46 2023, max compression
+gzip compressed data, was "/home/runner/work/APF/APF/dist/.tmp-8x46x19q/apf_base-2.4.4.tar", last modified: Fri Jun 30 20:18:28 2023, max compression
```

## Comparing `apf_base-2.4.3b0.tar` & `apf_base-2.4.4.tar`

### file list

```diff
@@ -1,55 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf/consumers/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/consumers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/consumers/avro_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/consumers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/consumers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/consumers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/consumers/kafka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf/core/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf/core/management/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/management/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    15241 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf/core/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf/core/templates/step/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/templates/step/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf/core/templates/step/package/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/templates/step/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/templates/step/package/step.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/templates/step/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf/core/templates/step/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/templates/step/scripts/run_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/templates/step/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/templates/step/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/topic_management.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/metrics/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/metrics/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/metrics/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf/metrics/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/metrics/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/metrics/prometheus/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf/producers/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/producers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/producers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/producers/json_prod.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/producers/kafka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf_base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/scripts/apf
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:28.000000 apf_base-2.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-30 20:18:04.000000 apf_base-2.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-30 20:18:28.000000 apf_base-2.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-30 20:18:04.000000 apf_base-2.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:28.000000 apf_base-2.4.4/apf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:28.000000 apf_base-2.4.4/apf/consumers/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/consumers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/consumers/avro_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/consumers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/consumers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/consumers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/consumers/kafka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:28.000000 apf_base-2.4.4/apf/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:28.000000 apf_base-2.4.4/apf/core/management/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/core/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/core/management/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/core/secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/core/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:28.000000 apf_base-2.4.4/apf/core/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:28.000000 apf_base-2.4.4/apf/core/templates/step/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/core/templates/step/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:28.000000 apf_base-2.4.4/apf/core/templates/step/package/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/core/templates/step/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/core/templates/step/package/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/core/templates/step/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:28.000000 apf_base-2.4.4/apf/core/templates/step/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/core/templates/step/scripts/run_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/core/templates/step/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/core/templates/step/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/core/topic_management.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:28.000000 apf_base-2.4.4/apf/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/metrics/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/metrics/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/metrics/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:28.000000 apf_base-2.4.4/apf/metrics/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/metrics/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/metrics/prometheus/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:28.000000 apf_base-2.4.4/apf/metrics/pyroscope/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/metrics/pyroscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/metrics/pyroscope/profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:28.000000 apf_base-2.4.4/apf/producers/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/producers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/producers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/producers/json_prod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-06-30 20:18:04.000000 apf_base-2.4.4/apf/producers/kafka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:28.000000 apf_base-2.4.4/apf_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-30 20:18:28.000000 apf_base-2.4.4/apf_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-30 20:18:28.000000 apf_base-2.4.4/apf_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 20:18:28.000000 apf_base-2.4.4/apf_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-30 20:18:28.000000 apf_base-2.4.4/apf_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-30 20:18:28.000000 apf_base-2.4.4/apf_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:28.000000 apf_base-2.4.4/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-30 20:18:04.000000 apf_base-2.4.4/scripts/apf
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 20:18:28.000000 apf_base-2.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-30 20:18:04.000000 apf_base-2.4.4/setup.py
```

### Comparing `apf_base-2.4.3b0/LICENSE` & `apf_base-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.3b0/PKG-INFO` & `apf_base-2.4.4/apf_base.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: apf_base
-Version: 2.4.3b0
+Name: apf-base
+Version: 2.4.4
 Summary: ALeRCE Alert Processing Framework.
 Author: ALeRCE Team
 Author-email: contact@alerce.online
 Project-URL: Github, https://github.com/alercebroker/APF
 Project-URL: Documentation, https://apf.readthedocs.io/en/latest/index.html
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `apf_base-2.4.3b0/README.md` & `apf_base-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.3b0/apf/consumers/avro_file.py` & `apf_base-2.4.4/apf/consumers/avro_file.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.3b0/apf/consumers/csv.py` & `apf_base-2.4.4/apf/consumers/csv.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.3b0/apf/consumers/generic.py` & `apf_base-2.4.4/apf/consumers/generic.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.3b0/apf/consumers/json.py` & `apf_base-2.4.4/apf/consumers/json.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.3b0/apf/consumers/kafka.py` & `apf_base-2.4.4/apf/consumers/kafka.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.3b0/apf/core/__init__.py` & `apf_base-2.4.4/apf/core/__init__.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.3b0/apf/core/management/helpers.py` & `apf_base-2.4.4/apf/core/management/helpers.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.3b0/apf/core/secret_manager.py` & `apf_base-2.4.4/apf/core/secret_manager.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.3b0/apf/core/step.py` & `apf_base-2.4.4/apf/core/step.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from abc import abstractmethod
 import abc
 from typing import Any, Dict, Iterable, List, Type, Union
 from apf.consumers import GenericConsumer
-from apf.metrics.prometheus import DefaultPrometheusMetrics, PrometheusMetrics
 from apf.metrics.generic import GenericMetricsProducer
+from apf.metrics.prometheus import DefaultPrometheusMetrics, PrometheusMetrics
+from apf.metrics.pyroscope import profile
 from apf.producers import GenericProducer
 from apf.core import get_class
 import logging
 import datetime
 
 
 class DefaultConsumer(GenericConsumer):
@@ -390,14 +391,15 @@
         Parameters
         ----------
         key_field : str
             the key of the message which value will be used as key for the producer
         """
         self.producer.set_key_field(key_field)
 
+    @profile
     def start(self):
         """Start running the step."""
         self._pre_consume()
         for message in self.consumer.consume():
             preprocessed_msg = self._pre_execute(message)
             result = self.execute(preprocessed_msg)
             result = self._post_execute(result)
```

### Comparing `apf_base-2.4.3b0/apf/core/templates/step/package/step.py` & `apf_base-2.4.4/apf/core/templates/step/package/step.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.3b0/apf/core/templates/step/scripts/run_step.py` & `apf_base-2.4.4/apf/core/templates/step/scripts/run_step.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.3b0/apf/core/topic_management.py` & `apf_base-2.4.4/apf/core/topic_management.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.3b0/apf/metrics/generic.py` & `apf_base-2.4.4/apf/metrics/generic.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.3b0/apf/metrics/kafka.py` & `apf_base-2.4.4/apf/metrics/kafka.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.3b0/apf/metrics/log.py` & `apf_base-2.4.4/apf/metrics/log.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.3b0/apf/metrics/prometheus/prometheus.py` & `apf_base-2.4.4/apf/metrics/prometheus/prometheus.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.3b0/apf/producers/csv.py` & `apf_base-2.4.4/apf/producers/csv.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.3b0/apf/producers/generic.py` & `apf_base-2.4.4/apf/producers/generic.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.3b0/apf/producers/json_prod.py` & `apf_base-2.4.4/apf/producers/json_prod.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.3b0/apf/producers/kafka.py` & `apf_base-2.4.4/apf/producers/kafka.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.3b0/apf_base.egg-info/PKG-INFO` & `apf_base-2.4.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: apf-base
-Version: 2.4.3b0
+Name: apf_base
+Version: 2.4.4
 Summary: ALeRCE Alert Processing Framework.
 Author: ALeRCE Team
 Author-email: contact@alerce.online
 Project-URL: Github, https://github.com/alercebroker/APF
 Project-URL: Documentation, https://apf.readthedocs.io/en/latest/index.html
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `apf_base-2.4.3b0/apf_base.egg-info/SOURCES.txt` & `apf_base-2.4.4/apf_base.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 apf/core/templates/step/scripts/run_step.py
 apf/metrics/__init__.py
 apf/metrics/generic.py
 apf/metrics/kafka.py
 apf/metrics/log.py
 apf/metrics/prometheus/__init__.py
 apf/metrics/prometheus/prometheus.py
+apf/metrics/pyroscope/__init__.py
+apf/metrics/pyroscope/profile.py
 apf/producers/__init__.py
 apf/producers/csv.py
 apf/producers/generic.py
 apf/producers/json_prod.py
 apf/producers/kafka.py
 apf_base.egg-info/PKG-INFO
 apf_base.egg-info/SOURCES.txt
```

### Comparing `apf_base-2.4.3b0/setup.py` & `apf_base-2.4.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="apf_base",
-    version="2.4.3b",
+    version="2.4.4",
     description="ALeRCE Alert Processing Framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ALeRCE Team",
     author_email="contact@alerce.online",
     packages=find_namespace_packages(include=["apf.*"]),
     scripts=["scripts/apf"],
```

