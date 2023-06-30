# Comparing `tmp/disco-generation-1.0.0.tar.gz` & `tmp/disco-generation-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disco-generation-1.0.0.tar", last modified: Wed Feb  8 17:12:08 2023, max compression
+gzip compressed data, was "disco-generation-1.1.0.tar", last modified: Fri Jun 30 14:27:55 2023, max compression
```

## Comparing `disco-generation-1.0.0.tar` & `disco-generation-1.1.0.tar`

### file list

```diff
@@ -1,61 +1,66 @@
-drwxr-xr-x   0 jrozen   (183784237) NLE\Domain Users (1222672855)        0 2023-02-08 17:12:08.155434 disco-generation-1.0.0/
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)    21077 2023-01-26 15:44:36.000000 disco-generation-1.0.0/LICENSE
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     3100 2023-02-08 17:12:08.155276 disco-generation-1.0.0/PKG-INFO
-drwxr-xr-x   0 jrozen   (183784237) NLE\Domain Users (1222672855)        0 2023-02-08 17:12:08.142909 disco-generation-1.0.0/disco/
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)      172 2023-02-08 09:45:54.000000 disco-generation-1.0.0/disco/__init__.py
-drwxr-xr-x   0 jrozen   (183784237) NLE\Domain Users (1222672855)        0 2023-02-08 17:12:08.144935 disco-generation-1.0.0/disco/distributions/
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)      438 2023-02-06 14:42:54.000000 disco-generation-1.0.0/disco/distributions/__init__.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     5226 2023-02-06 14:42:50.000000 disco-generation-1.0.0/disco/distributions/base_distribution.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     1986 2023-02-06 14:42:45.000000 disco-generation-1.0.0/disco/distributions/context_distribution.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     2431 2023-02-06 14:42:41.000000 disco-generation-1.0.0/disco/distributions/dataset_context_distribution.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)      538 2023-02-06 14:42:36.000000 disco-generation-1.0.0/disco/distributions/distribution.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     8845 2023-02-06 14:42:30.000000 disco-generation-1.0.0/disco/distributions/lm_distribution.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     1441 2023-02-06 14:43:02.000000 disco-generation-1.0.0/disco/distributions/single_context_distribution.py
-drwxr-xr-x   0 jrozen   (183784237) NLE\Domain Users (1222672855)        0 2023-02-08 17:12:08.146205 disco-generation-1.0.0/disco/metrics/
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)      175 2023-02-06 14:42:19.000000 disco-generation-1.0.0/disco/metrics/__init__.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     1052 2023-02-06 14:42:14.000000 disco-generation-1.0.0/disco/metrics/base.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     1843 2023-02-06 14:42:09.000000 disco-generation-1.0.0/disco/metrics/js.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     1571 2023-02-06 14:42:04.000000 disco-generation-1.0.0/disco/metrics/kl.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     1372 2023-02-06 14:41:58.000000 disco-generation-1.0.0/disco/metrics/tv.py
-drwxr-xr-x   0 jrozen   (183784237) NLE\Domain Users (1222672855)        0 2023-02-08 17:12:08.148141 disco-generation-1.0.0/disco/samplers/
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)      259 2023-02-06 14:41:52.000000 disco-generation-1.0.0/disco/samplers/__init__.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     1951 2023-02-06 14:41:48.000000 disco-generation-1.0.0/disco/samplers/accumulation_sampler.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     2281 2023-02-06 14:41:43.000000 disco-generation-1.0.0/disco/samplers/quasi_rejection_sampler.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)      401 2023-02-06 14:41:02.000000 disco-generation-1.0.0/disco/samplers/sampler.py
-drwxr-xr-x   0 jrozen   (183784237) NLE\Domain Users (1222672855)        0 2023-02-08 17:12:08.149900 disco-generation-1.0.0/disco/scorers/
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)      361 2023-02-06 14:40:53.000000 disco-generation-1.0.0/disco/scorers/__init__.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     1476 2023-02-06 14:40:48.000000 disco-generation-1.0.0/disco/scorers/boolean_scorer.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     1978 2023-02-06 14:40:45.000000 disco-generation-1.0.0/disco/scorers/exponential_scorer.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     1299 2023-02-06 14:40:40.000000 disco-generation-1.0.0/disco/scorers/pipeline_scorer.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     2437 2023-02-06 14:40:33.000000 disco-generation-1.0.0/disco/scorers/positive_scorer.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     1163 2023-02-06 14:40:26.000000 disco-generation-1.0.0/disco/scorers/scorer.py
-drwxr-xr-x   0 jrozen   (183784237) NLE\Domain Users (1222672855)        0 2023-02-08 17:12:08.150833 disco-generation-1.0.0/disco/tuners/
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)      209 2023-02-06 14:39:16.000000 disco-generation-1.0.0/disco/tuners/__init__.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)      849 2023-02-06 14:39:11.000000 disco-generation-1.0.0/disco/tuners/cdpg_tuner.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)      803 2023-02-06 14:39:07.000000 disco-generation-1.0.0/disco/tuners/dpg_tuner.py
-drwxr-xr-x   0 jrozen   (183784237) NLE\Domain Users (1222672855)        0 2023-02-08 17:12:08.152377 disco-generation-1.0.0/disco/tuners/loggers/
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)      118 2023-02-06 14:40:16.000000 disco-generation-1.0.0/disco/tuners/loggers/__init__.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)      982 2023-02-06 14:40:12.000000 disco-generation-1.0.0/disco/tuners/loggers/base.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)      854 2023-02-06 14:40:02.000000 disco-generation-1.0.0/disco/tuners/loggers/console.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     3020 2023-02-06 14:39:58.000000 disco-generation-1.0.0/disco/tuners/loggers/json.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     1991 2023-02-06 14:39:53.000000 disco-generation-1.0.0/disco/tuners/loggers/neptune.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     1430 2023-02-06 14:39:48.000000 disco-generation-1.0.0/disco/tuners/loggers/wandb.py
-drwxr-xr-x   0 jrozen   (183784237) NLE\Domain Users (1222672855)        0 2023-02-08 17:12:08.153071 disco-generation-1.0.0/disco/tuners/losses/
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)      141 2023-02-06 14:39:31.000000 disco-generation-1.0.0/disco/tuners/losses/__init__.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)      249 2023-02-06 14:39:26.000000 disco-generation-1.0.0/disco/tuners/losses/base.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     2123 2023-02-06 14:39:23.000000 disco-generation-1.0.0/disco/tuners/losses/kl.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)    20145 2023-02-06 14:38:25.000000 disco-generation-1.0.0/disco/tuners/tuner.py
-drwxr-xr-x   0 jrozen   (183784237) NLE\Domain Users (1222672855)        0 2023-02-08 17:12:08.154149 disco-generation-1.0.0/disco/utils/
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)      234 2023-02-06 14:37:55.000000 disco-generation-1.0.0/disco/utils/__init__.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)      893 2023-02-06 14:37:51.000000 disco-generation-1.0.0/disco/utils/device.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)      844 2023-02-06 14:37:44.000000 disco-generation-1.0.0/disco/utils/helpers.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     2145 2023-02-06 14:37:39.000000 disco-generation-1.0.0/disco/utils/moving_average.py
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)      655 2023-02-06 14:37:32.000000 disco-generation-1.0.0/disco/utils/observable.py
-drwxr-xr-x   0 jrozen   (183784237) NLE\Domain Users (1222672855)        0 2023-02-08 17:12:08.155053 disco-generation-1.0.0/disco_generation.egg-info/
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     3100 2023-02-08 17:12:08.000000 disco-generation-1.0.0/disco_generation.egg-info/PKG-INFO
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     1450 2023-02-08 17:12:08.000000 disco-generation-1.0.0/disco_generation.egg-info/SOURCES.txt
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)        1 2023-02-08 17:12:08.000000 disco-generation-1.0.0/disco_generation.egg-info/dependency_links.txt
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)       76 2023-02-08 17:12:08.000000 disco-generation-1.0.0/disco_generation.egg-info/requires.txt
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)        6 2023-02-08 17:12:08.000000 disco-generation-1.0.0/disco_generation.egg-info/top_level.txt
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)       38 2023-02-08 17:12:08.155484 disco-generation-1.0.0/setup.cfg
--rw-r--r--   0 jrozen   (183784237) NLE\Domain Users (1222672855)     3554 2023-02-08 17:11:18.000000 disco-generation-1.0.0/setup.py
+drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-06-30 14:27:55.212954 disco-generation-1.1.0/
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)    21077 2023-05-09 12:38:18.000000 disco-generation-1.1.0/LICENSE
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     3586 2023-06-30 14:27:55.211954 disco-generation-1.1.0/PKG-INFO
+drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-06-30 14:27:55.080955 disco-generation-1.1.0/disco/
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      173 2023-06-30 09:33:57.000000 disco-generation-1.1.0/disco/__init__.py
+drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-06-30 14:27:55.099955 disco-generation-1.1.0/disco/distributions/
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      438 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/distributions/__init__.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     5295 2023-06-09 09:08:25.000000 disco-generation-1.1.0/disco/distributions/base_distribution.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1986 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/distributions/context_distribution.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     2431 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/distributions/dataset_context_distribution.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      538 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/distributions/distribution.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     9812 2023-06-14 14:05:23.000000 disco-generation-1.1.0/disco/distributions/lm_distribution.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1441 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/distributions/single_context_distribution.py
+drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-06-30 14:27:55.112955 disco-generation-1.1.0/disco/metrics/
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      175 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/metrics/__init__.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1052 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/metrics/base.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1843 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/metrics/js.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1571 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/metrics/kl.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1372 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/metrics/tv.py
+drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-06-30 14:27:55.124955 disco-generation-1.1.0/disco/samplers/
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      259 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/samplers/__init__.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1951 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/samplers/accumulation_sampler.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     6839 2023-06-21 14:04:06.000000 disco-generation-1.1.0/disco/samplers/quasi_rejection_sampler.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      401 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/samplers/sampler.py
+drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-06-30 14:27:55.138954 disco-generation-1.1.0/disco/scorers/
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      361 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/scorers/__init__.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1476 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/scorers/boolean_scorer.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1978 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/scorers/exponential_scorer.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1299 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/scorers/pipeline_scorer.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     2437 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/scorers/positive_scorer.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1163 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/scorers/scorer.py
+drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-06-30 14:27:55.153954 disco-generation-1.1.0/disco/tuners/
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      279 2023-05-25 09:00:48.000000 disco-generation-1.1.0/disco/tuners/__init__.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1127 2023-05-25 09:00:48.000000 disco-generation-1.1.0/disco/tuners/cdpg_tuner.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1020 2023-05-25 09:00:48.000000 disco-generation-1.1.0/disco/tuners/dpg_tuner.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1153 2023-05-25 09:00:48.000000 disco-generation-1.1.0/disco/tuners/fcdpg_tuner.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1161 2023-05-25 09:00:48.000000 disco-generation-1.1.0/disco/tuners/fdpg_tuner.py
+drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-06-30 14:27:55.168954 disco-generation-1.1.0/disco/tuners/loggers/
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      118 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/tuners/loggers/__init__.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      982 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/tuners/loggers/base.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      854 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/tuners/loggers/console.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     3020 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/tuners/loggers/json.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1991 2023-06-14 12:51:08.000000 disco-generation-1.1.0/disco/tuners/loggers/neptune.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1430 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/tuners/loggers/wandb.py
+drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-06-30 14:27:55.184954 disco-generation-1.1.0/disco/tuners/losses/
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      225 2023-05-25 09:00:48.000000 disco-generation-1.1.0/disco/tuners/losses/__init__.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      249 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/tuners/losses/base.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     2235 2023-05-25 09:00:48.000000 disco-generation-1.1.0/disco/tuners/losses/js.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     2123 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/tuners/losses/kl.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     2261 2023-05-25 09:00:48.000000 disco-generation-1.1.0/disco/tuners/losses/reverse_kl.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     2125 2023-05-25 09:00:48.000000 disco-generation-1.1.0/disco/tuners/losses/tv.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)    21279 2023-06-21 14:04:06.000000 disco-generation-1.1.0/disco/tuners/tuner.py
+drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-06-30 14:27:55.195954 disco-generation-1.1.0/disco/utils/
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      234 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/utils/__init__.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      893 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/utils/device.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1155 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/utils/helpers.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     2145 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/utils/moving_average.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      655 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/utils/observable.py
+drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-06-30 14:27:55.208954 disco-generation-1.1.0/disco_generation.egg-info/
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     3586 2023-06-30 14:27:54.000000 disco-generation-1.1.0/disco_generation.egg-info/PKG-INFO
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1591 2023-06-30 14:27:54.000000 disco-generation-1.1.0/disco_generation.egg-info/SOURCES.txt
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)        1 2023-06-30 14:27:54.000000 disco-generation-1.1.0/disco_generation.egg-info/dependency_links.txt
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)       76 2023-06-30 14:27:54.000000 disco-generation-1.1.0/disco_generation.egg-info/requires.txt
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)        6 2023-06-30 14:27:54.000000 disco-generation-1.1.0/disco_generation.egg-info/top_level.txt
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)       38 2023-06-30 14:27:55.213954 disco-generation-1.1.0/setup.cfg
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     3881 2023-06-30 13:55:16.000000 disco-generation-1.1.0/setup.py
```

### Comparing `disco-generation-1.0.0/LICENSE` & `disco-generation-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `disco-generation-1.0.0/disco/distributions/base_distribution.py` & `disco-generation-1.1.0/disco/distributions/base_distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # disco
 # Copyright (C) 2022-present NAVER Corp.
 # Creative Commons Attribution-NonCommercial-ShareAlike 4.0 license
 
 import torch
 from tqdm.autonotebook import trange
+import copy
 
 from disco.scorers.positive_scorer import Product
 from disco.scorers.exponential_scorer import ExponentialScorer
 from disco.scorers.boolean_scorer import BooleanScorer
 from .distribution import Distribution
 from .single_context_distribution import SingleContextDistribution
 from disco.samplers.accumulation_sampler import AccumulationSampler
@@ -18,14 +19,17 @@
 
 class BaseDistribution(Distribution):
     """
     Base distribution class, which can be used
     to build an EBM.
     """
 
+    def clone(self):
+        return copy.deepcopy(self)
+
     def constrain(self,
             features, moments=None,
             proposal=None, context_distribution=SingleContextDistribution(''), context_sampling_size=1,
             n_samples=2**9, iterations=1000, learning_rate=0.05, tolerance=1e-5, sampling_size=2**5
         ):
         """
         Constrains features to the base according to their moments,
```

### Comparing `disco-generation-1.0.0/disco/distributions/context_distribution.py` & `disco-generation-1.1.0/disco/distributions/context_distribution.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.0.0/disco/distributions/dataset_context_distribution.py` & `disco-generation-1.1.0/disco/distributions/dataset_context_distribution.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.0.0/disco/distributions/distribution.py` & `disco-generation-1.1.0/disco/distributions/distribution.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.0.0/disco/distributions/lm_distribution.py` & `disco-generation-1.1.0/disco/distributions/lm_distribution.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,47 +16,42 @@
 class LMDistribution(BaseDistribution):
     """
     Language model distribution class, a core class for all NLP
     use-cases, relying on Huggingface's Transformers library.
     """
 
     def __init__(self,
-            network="gpt2", tokenizer="gpt2", nature="causal", freeze=True,
+            model="gpt2", tokenizer=None, auto=AutoModelForCausalLM, freeze=True,
             length=40, device="cpu",
             **config
         ):
         """
         Parameters
         ----------
-        network: string
+        model: string
             Transformers' name of a causal or seq2seq language model 
         tokenizer: string
             Transformers' name for the related tokenizer
-        nature: string
-            "causal" or "seq2seq" to use the correct config class from Transformers
+        auto: class
+            auto class from Transformers, default is AutoModelForCausalLM
+            but AutoModelForSeq2SeqLM is also valid
         freeze: boolean
             flag to eventually (not) freeze the network's parameters
         length: int
             number of tokens in the samples
         device: string
             reference of the computing device
         config: kwarg
             parameters and values passed to transformers' ```generate(…)```
         """
 
-        assert nature in ["causal", "seq2seq"], "only causal and seq2seq model are handled."
-        self.nature = nature
-        klass = AutoModelForCausalLM if "causal" == nature else AutoModelForSeq2SeqLM
+        self.tokenizer= AutoTokenizer.from_pretrained(tokenizer if tokenizer else model)
+        assert auto in [AutoModelForCausalLM, AutoModelForSeq2SeqLM], "only AutoModel, AutoModelForCausalLM and AutoModelForSeq2SeqLM are valid options."
+        self._load_network(auto, model)
     
-        self.tokenizer= AutoTokenizer.from_pretrained(tokenizer)
-        self.tokenizer.pad_token = self.tokenizer.eos_token
-        self.network = klass.from_pretrained(
-                network,
-                pad_token_id=self.tokenizer.eos_token_id
-            )
         self.device = device
         self.network.to(self.device)
         self.network.eval() # to make sure scoring is consistent
         if freeze:
             self.freeze(True)
 
         self.length = length
@@ -71,14 +66,20 @@
         self.params = default_params.copy()
         self.params.update(config)
 
         self.scorable = True if all(\
                 [default_params[k] == self.params[k] for k in default_params.keys()]\
             ) else False
 
+    def _load_network(self, auto, model):
+        self.network = auto.from_pretrained(model)
+        if not self.network.config.is_encoder_decoder:
+            self.tokenizer.pad_token = self.tokenizer.eos_token
+            self.network.config.pad_token_id = self.tokenizer.eos_token_id
+
     def to(self, device):
         self.device = device
         self.network.to(self.device)
 
     def freeze(self, frozen=True):
         """Freeze (or unfreeze) parameters for gradient computation.
 
@@ -112,15 +113,16 @@
 
         assert self.scorable, "this distribution's parameters make it unscorable."
         shapes = set([s.token_ids.shape for s in samples])
         assert 1 == len(shapes), "sequences of token_ids should have the same shape, but got: {shapes}."
 
         device = self.device
 
-        context = self.tokenizer.convert_ids_to_tokens(self.tokenizer.bos_token_id) if "" == context else context
+        if not self.network.config.is_encoder_decoder:
+            context = self.tokenizer.bos_token if "" == context else context
         tokenized_context = self.tokenizer([context] * len(samples), return_tensors="pt", add_special_tokens=True)
         tokenized_context["input_ids"] = tokenized_context["input_ids"].to(device)
         tokenized_context["attention_mask"] = tokenized_context["attention_mask"].to(device)
 
         tokenized_samples = dict()
         tokenized_samples["input_ids"] = torch.stack([sample.token_ids for sample in samples]).to(device)
 
@@ -129,30 +131,37 @@
                 self.tokenizer.eos_token_id
             )
         tokenized_samples["attention_mask"] = torch.where(
                 self.tokenizer.pad_token_id == tokenized_samples["input_ids"],
                 0, 1
             )
         for i, ix in enumerate(first_eos_indices):
-            tokenized_samples["attention_mask"][i][ix] = 1
+            if None != self.network.config.forced_bos_token_id and\
+                self.network.config.forced_bos_token_id == tokenized_samples["input_ids"][i][0]:
+                    tokenized_samples["attention_mask"][i][0] = 0
+            else:
+                tokenized_samples["attention_mask"][i][0] = 1  # at least score one token
+            if ix != -1:  # if there is an eos token
+                tokenized_samples["attention_mask"][i][ix] = 1  # score first eos token
+                tokenized_samples["attention_mask"][i][ix + 1:] = 0  # ignore everything after it
         tokenized_samples["attention_mask"] = tokenized_samples["attention_mask"].to(device)
 
-        if "causal" == self.nature:
+        if self.network.config.is_encoder_decoder:
+            shift = None
+            last = None
+            inputs = tokenized_context
+            labels = tokenized_samples["input_ids"]
+        else:
             shift = tokenized_context["input_ids"].shape[-1] - 1
             last = -1
             inputs = {
                 "input_ids": torch.cat((tokenized_context["input_ids"], tokenized_samples["input_ids"]), 1),
                 "attention_mask": torch.cat((tokenized_context["attention_mask"], tokenized_samples["attention_mask"]), 1)
             }
             labels = inputs["input_ids"]
-        else:
-            shift = None
-            last = None
-            inputs = tokenized_context
-            labels = tokenized_samples["input_ids"]
 
         if grad:
             outputs = self.network(**inputs, labels=labels)
         else:
             with torch.no_grad():
                 outputs = self.network(**inputs, labels=labels)
     
@@ -178,24 +187,26 @@
             flag to eventually return token-level tensor of scores
         
         Returns
         -------
         tuple of (list of Sample(tokens, text), tensor of logprobs)
         """
     
-        context = self.tokenizer.convert_ids_to_tokens(self.tokenizer.bos_token_id) if "" == context else context
+        if not self.network.config.is_encoder_decoder and not context:
+            context = self.tokenizer.bos_token
         input_ids = self.tokenizer([context] * sampling_size, return_tensors="pt", add_special_tokens=True).input_ids.to(self.device)
         n_context_tokens = input_ids.shape[-1]
 
-        if "causal" == self.nature:
-            shift = n_context_tokens
+        if self.network.config.is_encoder_decoder:
+            shift = 1
             last = None
         else:
-            shift = 1
+            shift = n_context_tokens
             last = None
+
         outputs = self.network.generate(input_ids,
             output_scores=True, return_dict_in_generate=True,
             max_new_tokens=self.length,
             do_sample=True, **self.params)
 
         all_logprobs = torch.stack(outputs.scores, dim=1).log_softmax(-1)  # [sampling_size, length, vocab]
         token_seq_logprobs = torch.gather(
@@ -214,15 +225,18 @@
                         -1,
                         outputs.sequences[:, shift:last][:, 1:])
                     ),
                 dim=1
             )
         non_pad_log_scores = torch.where(-1 != non_pad_tokens, token_seq_logprobs, torch.tensor(0.).to(self.device))
         for i, ix in enumerate(first_eos_indices):
-            non_pad_log_scores[i][ix] = token_seq_logprobs[i][ix]
+            non_pad_log_scores[i][0] = token_seq_logprobs[i][0]  # at least score one token
+            if ix != -1: # if there an eos token
+                non_pad_log_scores[i][ix] = token_seq_logprobs[i][ix]  # keep the first eos scores
+                non_pad_log_scores[i][ix + 1:] = 0. # ignore everything after eos
         
         seq_logprobs = non_pad_log_scores.sum(dim=1) if sum else non_pad_log_scores
 
         output_tokens = outputs.sequences[:, shift:] # [sampling_size, length]
 
         return (
                 [TextSample(ots, self.tokenizer.decode(ots)) for ots in output_tokens],
```

### Comparing `disco-generation-1.0.0/disco/distributions/single_context_distribution.py` & `disco-generation-1.1.0/disco/distributions/single_context_distribution.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.0.0/disco/metrics/base.py` & `disco-generation-1.1.0/disco/metrics/base.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.0.0/disco/metrics/js.py` & `disco-generation-1.1.0/disco/metrics/js.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.0.0/disco/metrics/kl.py` & `disco-generation-1.1.0/disco/metrics/kl.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.0.0/disco/metrics/tv.py` & `disco-generation-1.1.0/disco/metrics/tv.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.0.0/disco/samplers/accumulation_sampler.py` & `disco-generation-1.1.0/disco/samplers/accumulation_sampler.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.0.0/disco/samplers/quasi_rejection_sampler.py` & `disco-generation-1.1.0/disco/tuners/losses/kl.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,59 @@
 # disco
 # Copyright (C) 2022-present NAVER Corp.
 # Creative Commons Attribution-NonCommercial-ShareAlike 4.0 license
 
 import torch
+from .base import BaseLoss
 
-from . import Sampler
-from disco.utils.device import get_device
-
-
-class QuasiRejectionSampler(Sampler):
+class KLLoss(BaseLoss):
     """
-    Quasi Rejection-Sampling class
+    Kullback-Leibler divergence loss for DPG
     """
-
-    def __init__(self, target, proposal, beta=1):
+    def __init__(self, use_baseline=True):
         """
         Parameters
         ----------
-        target: distribution
-            Energy-based model to (log-)score the samples
-        proposal: distribution
-            distribution to generate the samples
-        beta: float
-            coefficient to control the sampling
+        use_baseline: boolean
+            use a baseline to reduce variance
         """
+        super(KLLoss, self).__init__()
+        self.use_baseline = use_baseline
 
-        super(QuasiRejectionSampler, self).__init__(target, proposal)
-        self.beta = beta
-        self.n_samples = 0
-        self.n_accepted_samples = 0
-
-    def sample(self, sampling_size=32, context=''):
-        """Generates samples according to the QRS algorithm
+    def __call__(self, samples, context, proposal_log_scores, target_log_scores, model_log_scores, z):
+        """
+        Computes the KL loss on a given minibatch of samples
+        ∇ loss = (target(x) / q(x)) * ∇ log π(x)
 
         Parameters
         ----------
-        sampling_size: int
-            number of requested samples when sampling
+        samples: list of items
+            samples from the proposal network
         context: text
-            contextual text for which to sample
-
+            context for the samples
+        proposal_log_scores: array of floats
+            log-probabilities for the samples according to the proposal
+        target_log_scores: array of floats
+            log-probabilities for the samples according to the target
+        model_log_scores: array of floats
+            log-probabilities for the samples according to the model network
+        z: float
+            estimation of the partition function of the EBM
+ 
         Returns
         -------
-        tuple of accepted samples and their log-scores
+        mean loss across the minibatch
         """
 
-        samples, proposal_log_scores = self.proposal.sample(sampling_size=sampling_size, context=context)
-        self.n_samples += len(samples)
-
-        device = get_device(proposal_log_scores)
-
-        target_log_scores = self.target.log_score(samples=samples, context=context).to(device)
-
-        rs = torch.clamp(
-                torch.exp(target_log_scores - proposal_log_scores) / self.beta,
-                min=0.0, max=1.0
-            )
-
-        us = torch.rand(len(rs)).to(device)
-        accepted_samples = [x for k, x in zip(us < rs, samples) if k]
-        self.n_accepted_samples += len(accepted_samples)
-        accepted_log_scores = torch.tensor([s for k, s in zip(us < rs, proposal_log_scores) if k]).to(device)
-
-        return accepted_samples, accepted_log_scores
-
-    def get_acceptance_rate(self):
-        """Computes the acceptance rate, that is the number of accepted samples
-        over the total sampled ones
-        
-        Returns
-        -------
-        acceptance rate as float between 0 and 1"""
+        normalized_target_log_scores = target_log_scores - torch.log(z)
+        rewards = torch.exp(normalized_target_log_scores - proposal_log_scores)
+        self.metric_updated.dispatch('rewards', rewards.mean())
+        if self.use_baseline:
+            importance_ratios = (model_log_scores.detach() - proposal_log_scores).exp()
+            advantage = rewards - importance_ratios
+            loss = -torch.mean(advantage * model_log_scores)
+            self.metric_updated.dispatch('importance_ratios', importance_ratios.mean())
+            self.metric_updated.dispatch('advantage', advantage.mean())
+        else:
+            loss = -torch.mean(rewards * model_log_scores)
 
-        return self.n_accepted_samples / self.n_samples
+        return loss
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `disco-generation-1.0.0/disco/scorers/boolean_scorer.py` & `disco-generation-1.1.0/disco/scorers/boolean_scorer.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.0.0/disco/scorers/exponential_scorer.py` & `disco-generation-1.1.0/disco/scorers/exponential_scorer.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.0.0/disco/scorers/pipeline_scorer.py` & `disco-generation-1.1.0/disco/scorers/pipeline_scorer.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.0.0/disco/scorers/positive_scorer.py` & `disco-generation-1.1.0/disco/scorers/positive_scorer.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.0.0/disco/scorers/scorer.py` & `disco-generation-1.1.0/disco/scorers/scorer.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.0.0/disco/tuners/dpg_tuner.py` & `disco-generation-1.1.0/disco/tuners/dpg_tuner.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 from .cdpg_tuner import CDPGTuner
 from disco.distributions.single_context_distribution import SingleContextDistribution
 
 class DPGTuner(CDPGTuner):
     """
     DPG tuning class,
     a specific case of CDPG with a single, fixed, context.
+
+    The algorithm has been introduced in
+    "Distributional Reinforcement Learning for Energy-Based Sequential Models"
+    Tetiana Parshakova, Jean-Marc Andreoli, Marc Dymetman
+    https://arxiv.org/abs/1912.08517
     """
 
     def __init__(self, *args, context="", **kwargs):
         """
         Parameters
         ----------
         context: text
@@ -20,8 +25,8 @@
         """
 
         super(DPGTuner, self).__init__(
                 *args,
                 context_distribution=SingleContextDistribution(context),
                 context_sampling_size=1,
                 **kwargs
-            )
+            )
```

### Comparing `disco-generation-1.0.0/disco/tuners/loggers/base.py` & `disco-generation-1.1.0/disco/tuners/loggers/base.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.0.0/disco/tuners/loggers/console.py` & `disco-generation-1.1.0/disco/tuners/loggers/console.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.0.0/disco/tuners/loggers/json.py` & `disco-generation-1.1.0/disco/tuners/loggers/json.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.0.0/disco/tuners/loggers/neptune.py` & `disco-generation-1.1.0/disco/tuners/loggers/neptune.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.0.0/disco/tuners/loggers/wandb.py` & `disco-generation-1.1.0/disco/tuners/loggers/wandb.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.0.0/disco/tuners/losses/kl.py` & `disco-generation-1.1.0/disco/tuners/losses/reverse_kl.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,64 @@
 # disco
 # Copyright (C) 2022-present NAVER Corp.
 # Creative Commons Attribution-NonCommercial-ShareAlike 4.0 license
 
-import torch
 from .base import BaseLoss
+import torch
+from .misc.ema_baseline import EMABaseline
 
-class KLLoss(BaseLoss):
+class ReverseKLLoss(BaseLoss):
     """
-    Kullback-Leibler divergence loss for DPG
+    Reverse Kullback-Leibler divergence loss for DPG
     """
-    def __init__(self, use_baseline=True):
+    def __init__(self, use_baseline=False, ema_weight=0.99):
         """
         Parameters
         ----------
-        use_baseline: boolean
+        baseline: boolean
             use a baseline to reduce variance
+        ema_weight: float
+            weight to compute the exponential moving average of the rewards
         """
-        super(KLLoss, self).__init__()
+        super(ReverseKLLoss, self).__init__()
         self.use_baseline = use_baseline
+        if use_baseline:
+            self.baseline = EMABaseline(ema_weight)
 
-    def __call__(self, samples, context, proposal_log_scores, target_log_scores, model_log_scores, z):
+    def __call__(self, samples, context, scores, ebm_scores, target_scores, z):
         """
-        Computes the KL loss on a given minibatch of samples
-        ∇ loss = (target(x) / q(x)) * ∇ log π(x)
+        Computes the Reverse KL "loss" on a given minibatch of samples
 
         Parameters
         ----------
         samples: list of items
-            samples from the proposal network
+            samples from the proposal model
         context: text
             context for the samples
-        proposal_log_scores: array of floats
-            log-probabilities for the samples according to the proposal
-        target_log_scores: array of floats
-            log-probabilities for the samples according to the target
-        model_log_scores: array of floats
-            log-probabilities for the samples according to the model network
+        scores: array of floats
+            logprobabilities for the samples according to the proposal
+        ebm_scores: array of floats
+            logscores for the samples according to the ebm
+        target_scores: array of floats
+            logprobabilities for the samples according to the target model
         z: float
             estimation of the partition function of the EBM
  
         Returns
         -------
         mean loss across the minibatch
         """
 
-        normalized_target_log_scores = target_log_scores - torch.log(z)
-        rewards = torch.exp(normalized_target_log_scores - proposal_log_scores)
+        importance_ratios = torch.exp(target_scores.detach() - scores)
+        normalized_ebm_scores = ebm_scores - z.log()
+        rewards = importance_ratios * \
+                (target_scores.detach() - normalized_ebm_scores + 1)
+        self.metric_updated.dispatch('importance_ratios', importance_ratios.mean())
         self.metric_updated.dispatch('rewards', rewards.mean())
         if self.use_baseline:
-            importance_ratios = (model_log_scores.detach() - proposal_log_scores).exp()
-            advantage = rewards - importance_ratios
-            loss = -torch.mean(advantage * model_log_scores)
-            self.metric_updated.dispatch('importance_ratios', importance_ratios.mean())
+            advantage = self.baseline.advantage(rewards)
+            loss = torch.mean(advantage * target_scores)
             self.metric_updated.dispatch('advantage', advantage.mean())
         else:
-            loss = -torch.mean(rewards * model_log_scores)
+            loss = torch.mean(rewards * target_scores)
 
         return loss
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `disco-generation-1.0.0/disco/tuners/tuner.py` & `disco-generation-1.1.0/disco/tuners/tuner.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         "sampling_size": 2**5, # number of samples requested per sampling
         "context_sampling_size": 2**4, # number of different contexts to sample
         "divergence_evaluation_interval": 2**4, # number of gradient steps between evaluation of divergence
                                                 # (also used to eventually update proposal when offline tuning)
         "proposal_update_metric": "kl" # the proposal will be updated if the model is better according to this metric
     }
 
-    def __init__(self, model, target, proposal=None, context_distribution=SingleContextDistribution(), loss=KLLoss(), features=[], 
+    def __init__(self, model, target, proposal=None, context_distribution=SingleContextDistribution(), loss=JSLoss(), features=[], 
             track_metrics=["kl", "tv", "js"], track_divergence_from_base=False, **params):
         """
         Parameters
         ----------
         model: distribution
             model distribution, to be tuned
         target: product
@@ -99,39 +99,14 @@
         else:
             self.proposal = model
             self.learning = "online"
         self.model = model
 
         self.context_distribution = context_distribution
 
-        if self.params["proposal_update_metric"] not in track_metrics:
-            track_metrics.append(self.params["proposal_update_metric"])
-
-        self.z = defaultdict(MovingAverage)
-        self.divergence_estimates_target_proposal = dict()
-        self.divergence_estimates_target_model = dict()
-        for metric in track_metrics:
-            assert metric in divergence_pointwise_estimates_funcs, \
-                    f"Unknown metric {metric}. " \
-                    f"Options are: {list(divergence_pointwise_estimates_funcs.keys())}"
-            self.divergence_estimates_target_proposal[metric] = defaultdict(MovingAverage)
-            self.divergence_estimates_target_model[metric] = defaultdict(MovingAverage)
-
-        self.track_divergence_from_base = track_divergence_from_base
-        if self.track_divergence_from_base:
-            self.divergence_estimates_proposal_base = dict()
-            self.divergence_estimates_model_base = dict()
-            for metric in track_metrics:
-                assert metric in divergence_pointwise_estimates_funcs, \
-                        f"Unknown metric {metric}. " \
-                        f"Options are: {list(divergence_pointwise_estimates_funcs.keys())}"
-                self.divergence_estimates_proposal_base[metric] = defaultdict(MovingAverage)
-                self.divergence_estimates_model_base[metric] = defaultdict(MovingAverage)
-
-
         self._loss = loss
 
         self.features = list(features)
 
         if "AdamW" == self.params["optimizer"]:
             self.optimizer = torch.optim.AdamW(self.model.network.parameters(), lr=self.params["learning_rate"])
         if "SGD" == self.params["optimizer"]:
@@ -150,32 +125,75 @@
         self.parameters_updated = Observable()
         self.step_idx_updated = Observable()
         self.ministep_idx_updated = Observable()
         self.metric_updated = Observable()
         self.proposal_updated = Observable()
         self.eval_samples_updated = Observable()
 
+        # setup metrics to track
         forward(self._loss.metric_updated, self.metric_updated)
 
+        if self.params["proposal_update_metric"] not in track_metrics:
+            track_metrics.append(self.params["proposal_update_metric"])
+
+        self.z = defaultdict(MovingAverage)
+        self.divergence_estimates_target_proposal = dict()
+        self.divergence_estimates_target_model = dict()
+        for metric in track_metrics:
+            assert metric in divergence_pointwise_estimates_funcs, \
+                    f"Unknown metric {metric}. " \
+                    f"Options are: {list(divergence_pointwise_estimates_funcs.keys())}"
+            self.divergence_estimates_target_proposal[metric] = defaultdict(MovingAverage)
+            self.divergence_estimates_target_model[metric] = defaultdict(MovingAverage)
+
+        self.track_divergence_from_base = track_divergence_from_base
+        if self.track_divergence_from_base:
+            self.divergence_estimates_proposal_base = dict()
+            self.divergence_estimates_model_base = dict()
+            for metric in track_metrics:
+                assert metric in divergence_pointwise_estimates_funcs, \
+                        f"Unknown metric {metric}. " \
+                        f"Options are: {list(divergence_pointwise_estimates_funcs.keys())}"
+                self.divergence_estimates_proposal_base[metric] = defaultdict(MovingAverage)
+                self.divergence_estimates_model_base[metric] = defaultdict(MovingAverage)
+
+        self.features_moments_proposal = dict()
+        self.features_moments_target = dict()
+        for (label, feature) in self.features:
+            self.features_moments_proposal[label] = defaultdict(MovingAverage)
+            self.features_moments_target[label] = defaultdict(MovingAverage)
         if self.features:
-            self.eval_samples_updated.enroll(self.report_feature_moments)
+            self.eval_samples_updated.enroll(self._update_features_moments)
 
-    def report_feature_moments(self, context, samples, proposal_log_scores, model_log_scores, target_log_scores):
+    def _update_features_moments(self, context, samples, proposal_log_scores, model_log_scores, target_log_scores):
+        """
+        Improves the importance sampling estimates of the feature moments
+        specified on construction of the Tuner
 
+        Parameters
+        ----------
+        context: text
+            context for the samples
+        samples: list of items
+            samples from the proposal network
+        proposal_log_scores: array of floats
+            log-probabilities for the samples according to the proposal
+        model_log_scores: array of floats
+            log-probabilities for the samples according to the model
+        target_log_scores: array of floats
+            log-probabilities for the samples according to the target
+        """
         device = get_device(proposal_log_scores)
         model_log_scores = model_log_scores.to(device)
         logweights = model_log_scores - proposal_log_scores
         importance_ratios = torch.exp(logweights)
-        moments = {}
         for (label, feature) in self.features:
             proposal_moment_pointwise_estimates = feature.log_score(samples, context).exp().to(device)
-            moments[f"proposal_{label}"] = torch.mean(proposal_moment_pointwise_estimates)
-            moments[f"model_{label}"] = torch.mean((importance_ratios * proposal_moment_pointwise_estimates))
-        for k, v in moments.items():
-            self.metric_updated.dispatch(k, v)
+            self.features_moments_proposal[label][context] += proposal_moment_pointwise_estimates
+            self.features_moments_target[label][context] += importance_ratios * proposal_moment_pointwise_estimates
 
     def _update_moving_z(self, proposal_log_scores, target_log_scores, context):
         """
         Improves the `z` importance sampling estimate of Z 
         by averaging new samples
 
         Parameters
@@ -282,28 +300,28 @@
                 to_same_device(model_log_scores, base_log_scores, proposal_log_scores)
 
         for divergence_type, _ in self.divergence_estimates_target_proposal.items():
             self.divergence_estimates_model_base[divergence_type][context] += \
                 divergence_pointwise_estimates_funcs[divergence_type](
                     model_log_scores, base_log_scores, torch.as_tensor(1), proposal_log_scores)
 
-    def _report_and_reset_divergence_estimate(self, divergence_estimates_dict, arguments_name):
+    def _report_and_reset_importance_sampling_estimate(self, estimates_dict, distributions_name):
         """
-        Reports all tracked divergences in the divergence_estimates_dict using
-        as key name a concatentation of the divergence type name and the arguments_name
+        Reports all tracked metrics in the estimates_dict using
+        as key name a concatentation of the metric name and the distributions_name
 
-        divergence_estimates_dict: dictionary of strings to MovingAverage
-            The dictionary tracking divergence estimates
-        argument_name: string
-            A name that identifies the pair of distributions which divergence we are tracking
+        estimates_dict: dictionary (string, dictionary(string, MovingAverage))
+            The dictionary tracking metric estimates for each context
+        distributions_name: string
+            A name that identifies the distributions of which we are tracking the metric
         """
-        for divergence_type, moving_averages in divergence_estimates_dict.items():
-            self.metric_updated.dispatch(f"{divergence_type}_{arguments_name}",
+        for metric_name, moving_averages in estimates_dict.items():
+            self.metric_updated.dispatch(f"{metric_name}_{distributions_name}",
                     average(moving_averages))
-            divergence_estimates_dict[divergence_type] = defaultdict(MovingAverage)
+            estimates_dict[metric_name] = defaultdict(MovingAverage)
 
     def _update_proposal_if_better(self):
         """
             Checks if D(p||.) is lower for model than for the proposal
             and if so, updates the proposal
         """
         if average(self.divergence_estimates_target_proposal[self.params["proposal_update_metric"]]) > \
@@ -409,12 +427,14 @@
             for s in t:
                 self.step_idx_updated.dispatch(s)
                 self._step()
 
                 if  0 == (s + 1) % self.params["divergence_evaluation_interval"]:
                     if "offline" == self.learning:
                         self._update_proposal_if_better()
-                    self._report_and_reset_divergence_estimate(self.divergence_estimates_target_model, 'target_model')
-                    self._report_and_reset_divergence_estimate(self.divergence_estimates_target_proposal, 'target_proposal')
+                    self._report_and_reset_importance_sampling_estimate(self.divergence_estimates_target_model, 'target_model')
+                    self._report_and_reset_importance_sampling_estimate(self.divergence_estimates_target_proposal, 'target_proposal')
                     if self.track_divergence_from_base:
-                        self._report_and_reset_divergence_estimate(self.divergence_estimates_model_base, 'model_base')
-                        self._report_and_reset_divergence_estimate(self.divergence_estimates_proposal_base, 'proposal_base')
+                        self._report_and_reset_importance_sampling_estimate(self.divergence_estimates_model_base, 'model_base')
+                        self._report_and_reset_importance_sampling_estimate(self.divergence_estimates_proposal_base, 'proposal_base')
+                    self._report_and_reset_importance_sampling_estimate(self.features_moments_proposal, 'proposal')
+                    self._report_and_reset_importance_sampling_estimate(self.features_moments_target, 'target')
```

### Comparing `disco-generation-1.0.0/disco/utils/device.py` & `disco-generation-1.1.0/disco/utils/device.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.0.0/disco/utils/moving_average.py` & `disco-generation-1.1.0/disco/utils/moving_average.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.0.0/disco/utils/observable.py` & `disco-generation-1.1.0/disco/utils/observable.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.0.0/disco_generation.egg-info/SOURCES.txt` & `disco-generation-1.1.0/disco_generation.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -22,24 +22,29 @@
 disco/scorers/exponential_scorer.py
 disco/scorers/pipeline_scorer.py
 disco/scorers/positive_scorer.py
 disco/scorers/scorer.py
 disco/tuners/__init__.py
 disco/tuners/cdpg_tuner.py
 disco/tuners/dpg_tuner.py
+disco/tuners/fcdpg_tuner.py
+disco/tuners/fdpg_tuner.py
 disco/tuners/tuner.py
 disco/tuners/loggers/__init__.py
 disco/tuners/loggers/base.py
 disco/tuners/loggers/console.py
 disco/tuners/loggers/json.py
 disco/tuners/loggers/neptune.py
 disco/tuners/loggers/wandb.py
 disco/tuners/losses/__init__.py
 disco/tuners/losses/base.py
+disco/tuners/losses/js.py
 disco/tuners/losses/kl.py
+disco/tuners/losses/reverse_kl.py
+disco/tuners/losses/tv.py
 disco/utils/__init__.py
 disco/utils/device.py
 disco/utils/helpers.py
 disco/utils/moving_average.py
 disco/utils/observable.py
 disco_generation.egg-info/PKG-INFO
 disco_generation.egg-info/SOURCES.txt
```

### Comparing `disco-generation-1.0.0/setup.py` & `disco-generation-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,32 +2,38 @@
 # Copyright (C) 2022-present NAVER Corp.
 # Creative Commons Attribution-NonCommercial-ShareAlike 4.0 license
 
 from setuptools import setup, find_packages
 
 setup(
     name='disco-generation',
-    version='1.0.0',
+    version='1.1.0',
     description='A toolkit for distributional control of generative models',
     url='https://github.com/naver/disco',
     author='Naver Labs Europe', author_email='jos.rozen@naverlabs.com',
     license='Creative Commons Attribution-NonCommercial-ShareAlike 4.0',
-    long_description="""The 🕺🏽 **disco** toolkit allows to control the properties of the generations by language models and other generative systems to match human preferences while avoiding catastrophic forgetting.
+    long_description="""The 🕺🏽 **disco** toolkit allows to control language models and other generative systems to match human preferences while avoiding catastrophic forgetting.
 
-To achieve this in **disco**, we first represent in what ways we want to update original model as a target distribution and then, generate samples from this new distribution through a combination of learning or monte-carlo methods, as follows.
+To achieve this, **disco** decouples the problem of expressing _what_ properties the model should have from _how_ to actually get the desired model as separate steps.
 
-**Step 1: We express how the target distribution *should* be**
+**Step 1: ⚓ We express how the target distribution *should* be**
 
-To have a handle on the generative model, we define some feature over the generated samples. It can be anything we can compute. For example, on a language model it can be as simple as whether the generated text contains a certain word or as complex as the compilability of some generated piece of code. Importantly, there is no need for the feature to be differentiable.  
-Then, we can express our preferences on the target distribution by defining the target *moments* of this feature. For example, we might want to ask that a certain word appears 50% of the time when sampling from the model; or that 100% of the generated code is compilable. The resulting target distribution is expressed as an energy-based model or EBM, which is an unnormalized probability distribution that respects the desired moments while avoiding catastrophic forgetting, as a result of having minimal KL divergence to the original model.  
-This representation of the target distribution can *score* samples, but cannot directly be used to *generate* them.
+First, we define some feature over the generated samples that matters to us. It can be anything we can compute. For example, on a language model it can be as simple as whether the generated text contains a certain word or as complex as the compilability of some generated piece of code. Importantly, there is no need for the feature to be differentiable.
 
-**Step 2: We generate samples from the target distribution**
+Then, we can express our preferences on the target distribution by deciding how prevalent the feature should be. For example, we might want to ask that a certain word appears 50% of the time when sampling from the model; or that 100% of the generated code is compilable. The resulting target distribution is expressed as an energy-based model or EBM, which is an unnormalized probability distribution that respects the desired moments while avoiding catastrophic forgetting, as a result of having minimal KL divergence to the original model.
 
-To generate samples from the target distribution, if not perfectly, we can tune a model to approximate it. The resulting model can generate samples directly from a close approximation of the target distribution. Furthermore, it can be used jointly with Quasi-Rejection Sampling (QRS), a Monte Carlo sampling technique that allows the generation of samples that are even more representative of the target distribution.  
+The resulting representation of the target distribution can *score* samples, but cannot directly be used to *generate* them.
+
+**Step 2: 🎯 Approximate the target distribution**
+
+To generate samples from the target distribution we can tune a model to approximate it. We do this by minimizing the divergence to the target distribution. While techniques such as reinforcement learning from human feedback (RLHF) are restricted to using one kind of divergence only (specifically, reverse KL divergence), **disco** is more general, allowing the use of the full class of f-divergences, including both forward and reverse KL divergence, Jensen-Shannon, and total variation distance.
+
+**Step 3: 💬 Generate content that matches the preferences**
+
+The resulting model can generate samples directly from a close approximation of the target distribution. Furthermore, it can be used jointly with Quasi-Rejection Sampling (QRS), a Monte Carlo sampling technique that allows the generation of samples that are even more representative of the target distribution.
 Alternatively, it is then possible to use decoding methods such as nucleus sampling, top-k sampling, or beam search, which would return samples from a further updated target distribution.""",
     long_description_content_type='text/markdown',
     packages=find_packages(include=['disco', 'disco.*']),
     python_requires='>=3.8, <3.11',
     install_requires=['torch', 'transformers',
             'numpy', 'scipy',
             'datasets', 'spacy',
@@ -41,8 +47,8 @@
         'Operating System :: MacOS',
         'Operating System :: Microsoft :: Windows',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
-)
+)
```

