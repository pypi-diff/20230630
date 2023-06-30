# Comparing `tmp/openssm-0.0.0.0.tar.gz` & `tmp/openssm-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openssm-0.0.0.0.tar", last modified: Sun Jun 25 02:28:30 2023, max compression
+gzip compressed data, was "openssm-0.1.0.tar", max compression
```

## Comparing `openssm-0.0.0.0.tar` & `openssm-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,44 @@
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-25 02:28:30.331567 openssm-0.0.0.0/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      573 2023-06-24 21:58:25.000000 openssm-0.0.0.0/LICENSE.md
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     4852 2023-06-25 02:28:30.331340 openssm-0.0.0.0/PKG-INFO
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     3584 2023-06-24 21:58:25.000000 openssm-0.0.0.0/README.md
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        8 2023-06-25 02:28:26.000000 openssm-0.0.0.0/VERSION
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1666 2023-06-25 02:28:21.000000 openssm-0.0.0.0/pyproject.toml
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       22 2023-06-25 02:23:28.000000 openssm-0.0.0.0/requirements.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       38 2023-06-25 02:28:30.331642 openssm-0.0.0.0/setup.cfg
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-25 02:28:30.326037 openssm-0.0.0.0/src/
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-25 02:28:30.329455 openssm-0.0.0.0/src/openssm.egg-info/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     6148 2023-06-24 22:19:35.000000 openssm-0.0.0.0/src/openssm.egg-info/.DS_Store
--rw-------   0 thevinhluong102   (501) staff       (20)     4852 2023-06-25 02:28:30.000000 openssm-0.0.0.0/src/openssm.egg-info/PKG-INFO
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      315 2023-06-25 02:28:30.000000 openssm-0.0.0.0/src/openssm.egg-info/SOURCES.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        1 2023-06-25 02:28:30.000000 openssm-0.0.0.0/src/openssm.egg-info/dependency_links.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       27 2023-06-25 02:28:30.000000 openssm-0.0.0.0/src/openssm.egg-info/requires.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        4 2023-06-25 02:28:30.000000 openssm-0.0.0.0/src/openssm.egg-info/top_level.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        1 2023-06-24 22:20:34.000000 openssm-0.0.0.0/src/openssm.egg-info/zip-safe
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-25 02:28:30.330876 openssm-0.0.0.0/src/ssm/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       19 2023-06-25 02:23:28.000000 openssm-0.0.0.0/src/ssm/__init__.py
+-rw-r--r--   0        0        0      573 2023-06-23 03:02:10.966991 openssm-0.1.0/LICENSE.md
+-rw-r--r--   0        0        0     6914 2023-06-28 22:45:05.438359 openssm-0.1.0/README.md
+-rw-r--r--   0        0        0     1906 2023-06-28 22:38:58.361415 openssm-0.1.0/openssm/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 01:07:44.427623 openssm-0.1.0/openssm/__init__.py
+-rw-r--r--   0        0        0       39 2023-06-26 22:01:23.102867 openssm-0.1.0/openssm/archive/models/README.md
+-rw-r--r--   0        0        0       48 2023-06-26 22:01:23.102968 openssm-0.1.0/openssm/archive/models/pre_trained/README.md
+-rw-r--r--   0        0        0        0 2023-06-26 22:01:23.102992 openssm-0.1.0/openssm/archive/models/test.py
+-rw-r--r--   0        0        0       50 2023-06-26 22:01:23.103133 openssm-0.1.0/openssm/archive/models/user_trained/README.md
+-rw-r--r--   0        0        0       54 2023-06-26 22:01:23.103241 openssm-0.1.0/openssm/archive/models/validation/README.md
+-rw-r--r--   0        0        0       45 2023-06-26 22:01:23.103348 openssm-0.1.0/openssm/archive/models/version_control/README.md
+-rw-r--r--   0        0        0        0 2023-06-26 22:01:23.103399 openssm-0.1.0/openssm/archive/training/README.md
+-rw-r--r--   0        0        0        0 2023-06-26 22:01:23.103472 openssm-0.1.0/openssm/archive/training/fine_tuning/README.md
+-rw-r--r--   0        0        0        0 2023-06-26 22:01:23.103541 openssm-0.1.0/openssm/archive/training/validation/README.md
+-rw-r--r--   0        0        0       19 2023-06-26 22:01:23.103656 openssm-0.1.0/openssm/core/__init__.py
+-rw-r--r--   0        0        0     1452 2023-06-30 00:59:08.392644 openssm-0.1.0/openssm/core/adapter/abstract_adapter.py
+-rw-r--r--   0        0        0      779 2023-06-30 00:25:24.109372 openssm-0.1.0/openssm/core/adapter/base_adapter.py
+-rw-r--r--   0        0        0     2511 2023-06-26 22:27:58.943445 openssm-0.1.0/openssm/core/adapter/llama_index_adapter.py
+-rw-r--r--   0        0        0      199 2023-06-29 18:11:08.807277 openssm-0.1.0/openssm/core/backend/abstract_backend.py
+-rw-r--r--   0        0        0      197 2023-06-30 00:59:34.626526 openssm-0.1.0/openssm/core/backend/base_backend.py
+-rw-r--r--   0        0        0      108 2023-06-26 22:01:23.104217 openssm-0.1.0/openssm/core/config.py
+-rw-r--r--   0        0        0     2557 2023-06-26 22:01:23.104334 openssm-0.1.0/openssm/core/db.py
+-rw-r--r--   0        0        0     2015 2023-06-26 22:01:23.103785 openssm-0.1.0/openssm/core/old_abstract/ssm.py
+-rw-r--r--   0        0        0      821 2023-06-30 00:23:55.379436 openssm-0.1.0/openssm/core/slm/abstract_slm.py
+-rw-r--r--   0        0        0      492 2023-06-30 00:24:07.069670 openssm-0.1.0/openssm/core/slm/base_slm.py
+-rw-r--r--   0        0        0     2283 2023-06-26 23:07:56.491649 openssm-0.1.0/openssm/core/slm/gpt3_slm.py
+-rw-r--r--   0        0        0      417 2023-06-26 22:01:23.104723 openssm-0.1.0/openssm/core/slm/memory/conversation_db.py
+-rw-r--r--   0        0        0     2557 2023-06-26 22:01:23.104816 openssm-0.1.0/openssm/core/slm/memory/db.py
+-rw-r--r--   0        0        0     2159 2023-06-26 22:01:23.104938 openssm-0.1.0/openssm/core/slm/memory/sqlite_conversation_db.py
+-rw-r--r--   0        0        0     2425 2023-06-29 23:12:46.371782 openssm-0.1.0/openssm/core/ssm/abstract_ssm.py
+-rw-r--r--   0        0        0     2291 2023-06-30 00:57:17.005182 openssm-0.1.0/openssm/core/ssm/base_ssm.py
+-rw-r--r--   0        0        0     1397 2023-06-26 23:10:02.329337 openssm-0.1.0/openssm/core/ssm/gpt3_llama_index_ssm.py
+-rw-r--r--   0        0        0       58 2023-06-26 22:01:23.105328 openssm-0.1.0/openssm/industrial/interpretability/README.md
+-rw-r--r--   0        0        0       60 2023-06-26 22:01:23.105422 openssm-0.1.0/openssm/industrial/monitoring/README.md
+-rw-r--r--   0        0        0        0 2023-06-26 22:01:23.105470 openssm-0.1.0/openssm/industrial/security/README.md
+-rw-r--r--   0        0        0        0 2023-06-26 22:01:23.105561 openssm-0.1.0/openssm/industrial/security/audit/README.md
+-rw-r--r--   0        0        0        0 2023-06-26 22:01:23.105659 openssm-0.1.0/openssm/industrial/security/best_practices/README.md
+-rw-r--r--   0        0        0       63 2023-06-26 22:01:23.105800 openssm-0.1.0/openssm/integration/README.md
+-rw-r--r--   0        0        0     3574 2023-06-26 22:01:23.105923 openssm-0.1.0/openssm/integration/llamaindex/README.md
+-rw-r--r--   0        0        0       34 2023-06-26 22:01:23.106015 openssm-0.1.0/openssm/integration/testing_tools/README.md
+-rw-r--r--   0        0        0       19 2023-06-26 22:01:23.106104 openssm-0.1.0/openssm/old_ssm/__init__.py
+-rw-r--r--   0        0        0     2015 2023-06-26 22:01:23.106226 openssm-0.1.0/openssm/old_ssm/abstract/ssm.py
+-rw-r--r--   0        0        0      310 2023-06-30 01:39:44.768524 openssm-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8465 1970-01-01 00:00:00.000000 openssm-0.1.0/setup.py
+-rw-r--r--   0        0        0     7394 1970-01-01 00:00:00.000000 openssm-0.1.0/PKG-INFO
```

### Comparing `openssm-0.0.0.0/LICENSE.md` & `openssm-0.1.0/LICENSE.md`

 * *Files identical despite different names*

