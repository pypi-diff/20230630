# Comparing `tmp/audio-separator-0.1.4.tar.gz` & `tmp/audio_separator-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio-separator-0.1.4.tar", last modified: Fri Jun 30 07:16:45 2023, max compression
+gzip compressed data, was "audio_separator-0.1.5.tar", max compression
```

## Comparing `audio-separator-0.1.4.tar` & `audio_separator-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,10 @@
-drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 07:16:45.600453 audio-separator-0.1.4/
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)     1069 2023-06-30 05:57:58.000000 audio-separator-0.1.4/LICENSE
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)     3028 2023-06-30 07:16:45.600116 audio-separator-0.1.4/PKG-INFO
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2614 2023-06-30 07:16:33.000000 audio-separator-0.1.4/README.md
-drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 07:16:45.587673 audio-separator-0.1.4/audio_separator/
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:26:40.000000 audio-separator-0.1.4/audio_separator/__init__.py
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)    10882 2023-06-30 07:16:33.000000 audio-separator-0.1.4/audio_separator/audio_separator.py
-drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 07:16:45.599129 audio-separator-0.1.4/audio_separator/utils/
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 05:58:37.000000 audio-separator-0.1.4/audio_separator/utils/__init__.py
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2135 2023-06-30 05:58:37.000000 audio-separator-0.1.4/audio_separator/utils/pyrb.py
--rwxr-xr-x   0 andrew.beveridge   (503) staff       (20)     1112 2023-06-30 07:16:33.000000 audio-separator-0.1.4/audio_separator/utils/separate.py
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)    24840 2023-06-30 06:51:10.000000 audio-separator-0.1.4/audio_separator/utils/spec_utils.py
-drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 07:16:45.592276 audio-separator-0.1.4/audio_separator.egg-info/
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)     3028 2023-06-30 07:16:45.000000 audio-separator-0.1.4/audio_separator.egg-info/PKG-INFO
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)      459 2023-06-30 07:16:45.000000 audio-separator-0.1.4/audio_separator.egg-info/SOURCES.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)        1 2023-06-30 07:16:45.000000 audio-separator-0.1.4/audio_separator.egg-info/dependency_links.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)       72 2023-06-30 07:16:45.000000 audio-separator-0.1.4/audio_separator.egg-info/entry_points.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)      100 2023-06-30 07:16:45.000000 audio-separator-0.1.4/audio_separator.egg-info/requires.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)       16 2023-06-30 07:16:45.000000 audio-separator-0.1.4/audio_separator.egg-info/top_level.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)       38 2023-06-30 07:16:45.600519 audio-separator-0.1.4/setup.cfg
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)      997 2023-06-30 07:16:33.000000 audio-separator-0.1.4/setup.py
+-rw-r--r--   0        0        0     1069 2023-06-30 05:57:58.913442 audio_separator-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4596 2023-06-30 18:01:59.321311 audio_separator-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 06:26:40.206117 audio_separator-0.1.5/audio_separator/__init__.py
+-rw-r--r--   0        0        0    10882 2023-06-30 07:16:33.458446 audio_separator-0.1.5/audio_separator/audio_separator.py
+-rw-r--r--   0        0        0        0 2023-06-30 05:58:37.414385 audio_separator-0.1.5/audio_separator/utils/__init__.py
+-rw-r--r--   0        0        0     2135 2023-06-30 05:58:37.421373 audio_separator-0.1.5/audio_separator/utils/pyrb.py
+-rwxr-xr-x   0        0        0     1112 2023-06-30 07:16:33.459360 audio_separator-0.1.5/audio_separator/utils/separate.py
+-rw-r--r--   0        0        0    24840 2023-06-30 06:51:10.010639 audio_separator-0.1.5/audio_separator/utils/spec_utils.py
+-rw-r--r--   0        0        0      601 2023-06-30 18:08:14.411842 audio_separator-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5421 1970-01-01 00:00:00.000000 audio_separator-0.1.5/PKG-INFO
```

### Comparing `audio-separator-0.1.4/LICENSE` & `audio_separator-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `audio-separator-0.1.4/audio_separator/audio_separator.py` & `audio_separator-0.1.5/audio_separator/audio_separator.py`

 * *Files identical despite different names*

### Comparing `audio-separator-0.1.4/audio_separator/utils/pyrb.py` & `audio_separator-0.1.5/audio_separator/utils/pyrb.py`

 * *Files identical despite different names*

### Comparing `audio-separator-0.1.4/audio_separator/utils/separate.py` & `audio_separator-0.1.5/audio_separator/utils/separate.py`

 * *Files identical despite different names*

### Comparing `audio-separator-0.1.4/audio_separator/utils/spec_utils.py` & `audio_separator-0.1.5/audio_separator/utils/spec_utils.py`

 * *Files identical despite different names*

