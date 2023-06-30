# Comparing `tmp/healdata_utils-0.0.7a0.tar.gz` & `tmp/healdata_utils-0.0.8a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healdata_utils-0.0.7a0.tar", last modified: Tue Jun 13 02:15:46 2023, max compression
+gzip compressed data, was "healdata_utils-0.0.8a0.tar", last modified: Fri Jun 30 14:53:24 2023, max compression
```

## Comparing `healdata_utils-0.0.7a0.tar` & `healdata_utils-0.0.8a0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:15:46.654014 healdata_utils-0.0.7a0/
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-06-13 02:15:46.654014 healdata_utils-0.0.7a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 02:15:46.654014 healdata_utils-0.0.7a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:15:46.642014 healdata_utils-0.0.7a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:15:46.646014 healdata_utils-0.0.7a0/src/healdata_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:15:46.650014 healdata_utils-0.0.7a0/src/healdata_utils/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:15:46.650014 healdata_utils-0.0.7a0/src/healdata_utils/transforms/csvdata/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/transforms/csvdata/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:15:46.650014 healdata_utils-0.0.7a0/src/healdata_utils/transforms/csvtemplate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/transforms/csvtemplate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/transforms/csvtemplate/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/transforms/csvtemplate/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:15:46.650014 healdata_utils-0.0.7a0/src/healdata_utils/transforms/frictionless/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/transforms/frictionless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/transforms/frictionless/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:15:46.650014 healdata_utils-0.0.7a0/src/healdata_utils/transforms/jsontemplate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/transforms/jsontemplate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/transforms/jsontemplate/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/transforms/jsontemplate/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:15:46.650014 healdata_utils-0.0.7a0/src/healdata_utils/transforms/readstat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/transforms/readstat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/transforms/readstat/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:15:46.650014 healdata_utils-0.0.7a0/src/healdata_utils/transforms/redcapcsv/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/transforms/redcapcsv/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/transforms/redcapcsv/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/transforms/redcapcsv/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/transforms/redcapcsv/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:15:46.650014 healdata_utils-0.0.7a0/src/healdata_utils/types/
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/types/typesets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:15:46.654014 healdata_utils-0.0.7a0/src/healdata_utils/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/validators/frictionless.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/validators/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/src/healdata_utils/validators/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:15:46.650014 healdata_utils-0.0.7a0/src/healdata_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-06-13 02:15:46.000000 healdata_utils-0.0.7a0/src/healdata_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-13 02:15:46.000000 healdata_utils-0.0.7a0/src/healdata_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 02:15:46.000000 healdata_utils-0.0.7a0/src/healdata_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 02:15:46.000000 healdata_utils-0.0.7a0/src/healdata_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-13 02:15:46.000000 healdata_utils-0.0.7a0/src/healdata_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-13 02:15:46.000000 healdata_utils-0.0.7a0/src/healdata_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:15:46.654014 healdata_utils-0.0.7a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-13 02:15:33.000000 healdata_utils-0.0.7a0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.525761 healdata_utils-0.0.8a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-06-30 14:53:24.525761 healdata_utils-0.0.8a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-06-30 14:53:14.000000 healdata_utils-0.0.8a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:53:24.525761 healdata_utils-0.0.8a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.517761 healdata_utils-0.0.8a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/src/healdata_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/src/healdata_utils/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/src/healdata_utils/transforms/csvdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/csvdata/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/src/healdata_utils/transforms/csvtemplate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/csvtemplate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/csvtemplate/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/csvtemplate/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/src/healdata_utils/transforms/frictionless/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/frictionless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/frictionless/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/src/healdata_utils/transforms/jsontemplate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/jsontemplate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/jsontemplate/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/jsontemplate/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/src/healdata_utils/transforms/readstat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/readstat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/readstat/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/src/healdata_utils/transforms/redcapcsv/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/redcapcsv/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/redcapcsv/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/redcapcsv/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/redcapcsv/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/src/healdata_utils/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/types/typesets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/src/healdata_utils/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/validators/frictionless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/validators/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/validators/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/src/healdata_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-06-30 14:53:24.000000 healdata_utils-0.0.8a0/src/healdata_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-30 14:53:24.000000 healdata_utils-0.0.8a0/src/healdata_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:53:24.000000 healdata_utils-0.0.8a0/src/healdata_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-30 14:53:24.000000 healdata_utils-0.0.8a0/src/healdata_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-30 14:53:24.000000 healdata_utils-0.0.8a0/src/healdata_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-30 14:53:24.000000 healdata_utils-0.0.8a0/src/healdata_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/tests/test_utils.py
```

### Comparing `healdata_utils-0.0.7a0/PKG-INFO` & `healdata_utils-0.0.8a0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,37 @@
-Metadata-Version: 2.1
-Name: healdata_utils
-Version: 0.0.7a0
-Summary: Data packaging tools for the HEAL data ecosystem
-Home-page: https://github.com/norc-heal/healdata-utils
-Author: Michael Kranz
-Author-email: kranz-michael@norc.org
-Description-Content-Type: text/markdown
+--8<-- [start:intro]
 
 # HEAL Data Utilities
 
 The HEAL data utilities python package provides data packaging tools for the HEAL data ecosystem to facilitate data discovery,sharing, and harmonization with a focus on the HEAL platform data consultancy (DSC).
  
 Currently, the focus of the repo is on generating data-dictionaries (see Variable level metadata section below). However, in the future, this will be expanded for all heal specific data packaging functions (e.g., study and file level metadata and data).
 
 ## Installation
 
 To install the latest official release of healdata-utils, from your computer's command prompt, run:
 
-`pip install healdata-utils`
-
-to install the working, un-released version from this git repository, run:
+`pip install healdata-utils --pre` (**NOTE: currently in pre-lease**)
 
 `pip install git+https://github.com/norc-heal/healdata-utils.git`
 
 
-### Variable level metadata (data dictionaries)
+## Variable level metadata (data dictionaries)
 
 [![Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/norc-heal/healdata-utils/HEAD?labpath=notebooks%2Fdemos%2Finputs-to-heal-data-dictionary.ipynb) 
 
 The healdata-utils variable level metadata (vlmd) tool inputs a variety of different input file types and exports HEAL-formatted data dictionaries (JSON and CSV formats). Additionally, exported validation (ie "error") reports provide the user information as to a. if the exported data dictionary is valid according to HEAL specifications (see the schema repository [here](https://github.com/norc-heal/heal-metadata-schemas/tree/main/variable-level-metadata-schema)).
 
+For support formats and more detailed software specific instructions and recommendations, [see here](docs/supported_input_formats.md)
 
-## Basic usage 
+### Basic usage 
 
 The vlmd tool can be used via python or the command line.
 
-### Using from python
+#### Using from python
 
 From your current working directory in python, run:
 
 ```python
 from healdata_utils.cli import convert_to_vlmd
 
 # description and title are optional. If submitting through platform, can fill these out there.
@@ -65,51 +57,59 @@
 
 input_descriptions
 
 ```
 
 The `input_descriptions` object contains the choice for `inputtype` as the key and the description as the value.
 
-### Using from the command line
+#### Using from the command line
 
 From your current working directory run:
 (note the `\` at the end of each line signals a line continuation for ease in understanding the long one line command.) Again the `--title` and `--description` options are optional.
 For descriptions on the different flags/options, run `vlmd --help`
 
 ```bash
 
 vlmd --filepath "data/example_pyreadstat_output.sav" \
 --outputdir "output-cli" \
 --title "Healdata-utils Demonstration Data Dictionary" \
 --description "This is a proof of concept to demonstrate the healdata-utils functionality" 
 ```
 
-### Output
+#### Output
 
-Both the python and command line routes will result in a JSON and CSV version of the HEAL  data dictionary in the output folder along with 
-the validation reports in the `errors` folder. See below:
+Both the python and command line routes will result in a JSON and CSV version of the HEAL  data dictionary in the output folder along with the validation reports in the `errors` folder. See below:
 
 - `input/input/my-redcap-data-dictionary-export.csv` : your input file
 
 - `output/errors/heal-csv-errors.json`: outputted validation report for table in csv file against frictionless schema
     - see schema [here](https://github.com/norc-heal/heal-metadata-schemas/blob/main/variable-level-metadata-schema/schemas/frictionless/csvtemplate/fields.json)
 - `output/errors/heal-json-errors.json`:  outputted jsonschema validation report.
     - see schema [here](https://github.com/norc-heal/heal-metadata-schemas/blob/main/variable-level-metadata-schema/schemas/jsonschema/data-dictionary.json)
 
+!!! important
+    The main difference* between the CSV and JSON data dictionary validation lies in the way the data dictionaries are structured and the additional metadata included in the JSON data dictionary.
+    
+    The CSV data dictionary is a plain tabular representation with no additional metadata, while the JSON dataset includes fields along with additional metadata in the form of a root description and title.
+
+    * for field-specific differences, see the schemas in the documentation. 
+    
+
 - `output/heal-csvtemplate-data-dictionary.csv`: This is the CSV data dictionary
 - `output/heal-jsontemplate-data-dictionary.json`: This is the JSON version of the data dictionary
 
 > Note, only the JSON version will have the user-specified `title` and `description`
 
-
-### Examples
+### Interactive notebooks
 
 See the below notebooks demonstrating use and workflows using the `convert_to_vlmd` in python and `vlmd` in the command line. 
 
 > Clicking on the "binder badges" will bring you to an interactive notebook page where you can test out the notebooks. Here, healdata-utils comes pre-installed.
 
 1. Generating a heal data dictionary from a variety of input files 
 
 - [click here for static notebook ](notebooks/demos/inputs-to-heal-data-dictionary.ipynb) 
 - click binder badge for interactive [![Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/norc-heal/healdata-utils/HEAD?labpath=notebooks%2Fdemos%2Finputs-to-heal-data-dictionary.ipynb) 
 
 2. [in development] Creating and iterating over a csv data dictionary to create a valid data dictionary file [click here](notebooks/demos/demo-csvtemplate-validation.ipynb)
+
+--8<-- [end:intro]
```

### Comparing `healdata_utils-0.0.7a0/README.md` & `healdata_utils-0.0.8a0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,46 @@
+Metadata-Version: 2.1
+Name: healdata_utils
+Version: 0.0.8a0
+Summary: Data packaging tools for the HEAL data ecosystem
+Home-page: https://github.com/norc-heal/healdata-utils
+Author: Michael Kranz
+Author-email: kranz-michael@norc.org
+Description-Content-Type: text/markdown
+
+--8<-- [start:intro]
+
 # HEAL Data Utilities
 
 The HEAL data utilities python package provides data packaging tools for the HEAL data ecosystem to facilitate data discovery,sharing, and harmonization with a focus on the HEAL platform data consultancy (DSC).
  
 Currently, the focus of the repo is on generating data-dictionaries (see Variable level metadata section below). However, in the future, this will be expanded for all heal specific data packaging functions (e.g., study and file level metadata and data).
 
 ## Installation
 
 To install the latest official release of healdata-utils, from your computer's command prompt, run:
 
-`pip install healdata-utils`
-
-to install the working, un-released version from this git repository, run:
+`pip install healdata-utils --pre` (**NOTE: currently in pre-lease**)
 
 `pip install git+https://github.com/norc-heal/healdata-utils.git`
 
 
-### Variable level metadata (data dictionaries)
+## Variable level metadata (data dictionaries)
 
 [![Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/norc-heal/healdata-utils/HEAD?labpath=notebooks%2Fdemos%2Finputs-to-heal-data-dictionary.ipynb) 
 
 The healdata-utils variable level metadata (vlmd) tool inputs a variety of different input file types and exports HEAL-formatted data dictionaries (JSON and CSV formats). Additionally, exported validation (ie "error") reports provide the user information as to a. if the exported data dictionary is valid according to HEAL specifications (see the schema repository [here](https://github.com/norc-heal/heal-metadata-schemas/tree/main/variable-level-metadata-schema)).
 
+For support formats and more detailed software specific instructions and recommendations, [see here](docs/supported_input_formats.md)
 
-## Basic usage 
+### Basic usage 
 
 The vlmd tool can be used via python or the command line.
 
-### Using from python
+#### Using from python
 
 From your current working directory in python, run:
 
 ```python
 from healdata_utils.cli import convert_to_vlmd
 
 # description and title are optional. If submitting through platform, can fill these out there.
@@ -56,51 +66,59 @@
 
 input_descriptions
 
 ```
 
 The `input_descriptions` object contains the choice for `inputtype` as the key and the description as the value.
 
-### Using from the command line
+#### Using from the command line
 
 From your current working directory run:
 (note the `\` at the end of each line signals a line continuation for ease in understanding the long one line command.) Again the `--title` and `--description` options are optional.
 For descriptions on the different flags/options, run `vlmd --help`
 
 ```bash
 
 vlmd --filepath "data/example_pyreadstat_output.sav" \
 --outputdir "output-cli" \
 --title "Healdata-utils Demonstration Data Dictionary" \
 --description "This is a proof of concept to demonstrate the healdata-utils functionality" 
 ```
 
-### Output
+#### Output
 
-Both the python and command line routes will result in a JSON and CSV version of the HEAL  data dictionary in the output folder along with 
-the validation reports in the `errors` folder. See below:
+Both the python and command line routes will result in a JSON and CSV version of the HEAL  data dictionary in the output folder along with the validation reports in the `errors` folder. See below:
 
 - `input/input/my-redcap-data-dictionary-export.csv` : your input file
 
 - `output/errors/heal-csv-errors.json`: outputted validation report for table in csv file against frictionless schema
     - see schema [here](https://github.com/norc-heal/heal-metadata-schemas/blob/main/variable-level-metadata-schema/schemas/frictionless/csvtemplate/fields.json)
 - `output/errors/heal-json-errors.json`:  outputted jsonschema validation report.
     - see schema [here](https://github.com/norc-heal/heal-metadata-schemas/blob/main/variable-level-metadata-schema/schemas/jsonschema/data-dictionary.json)
 
+!!! important
+    The main difference* between the CSV and JSON data dictionary validation lies in the way the data dictionaries are structured and the additional metadata included in the JSON data dictionary.
+    
+    The CSV data dictionary is a plain tabular representation with no additional metadata, while the JSON dataset includes fields along with additional metadata in the form of a root description and title.
+
+    * for field-specific differences, see the schemas in the documentation. 
+    
+
 - `output/heal-csvtemplate-data-dictionary.csv`: This is the CSV data dictionary
 - `output/heal-jsontemplate-data-dictionary.json`: This is the JSON version of the data dictionary
 
 > Note, only the JSON version will have the user-specified `title` and `description`
 
-
-### Examples
+### Interactive notebooks
 
 See the below notebooks demonstrating use and workflows using the `convert_to_vlmd` in python and `vlmd` in the command line. 
 
 > Clicking on the "binder badges" will bring you to an interactive notebook page where you can test out the notebooks. Here, healdata-utils comes pre-installed.
 
 1. Generating a heal data dictionary from a variety of input files 
 
 - [click here for static notebook ](notebooks/demos/inputs-to-heal-data-dictionary.ipynb) 
 - click binder badge for interactive [![Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/norc-heal/healdata-utils/HEAD?labpath=notebooks%2Fdemos%2Finputs-to-heal-data-dictionary.ipynb) 
 
 2. [in development] Creating and iterating over a csv data dictionary to create a valid data dictionary file [click here](notebooks/demos/demo-csvtemplate-validation.ipynb)
+
+--8<-- [end:intro]
```

### Comparing `healdata_utils-0.0.7a0/setup.py` & `healdata_utils-0.0.8a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def generate_long_description():
     return Path("README.md").read_text()
 
 
 setup(
     name='healdata_utils',
-    version='0.0.7-alpha',
+    version='0.0.8-alpha',
     author='Michael Kranz',
     author_email='kranz-michael@norc.org',
     long_description=generate_long_description(),
     long_description_content_type="text/markdown",    
     description='Data packaging tools for the HEAL data ecosystem',
     #TODO: change url to HEAL once migrated.
     url='https://github.com/norc-heal/healdata-utils',
```

### Comparing `healdata_utils-0.0.7a0/src/healdata_utils/cli.py` & `healdata_utils-0.0.8a0/src/healdata_utils/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 choice_fxn = {
     'data.csv':convert_datacsv,
     'template.csv':convert_templatecsv,
     'csv': convert_templatecsv, #maintained for backwards compatibility
     'sav': convert_readstat,
     'dta':convert_readstat,
-    'por':convert_readstat,
+    #'por':convert_readstat,
     'sas7bdat':convert_readstat,
     'template.json':convert_templatejson,
     'json':convert_templatejson, #maintain for bwds compat
     "redcap.csv":convert_redcapcsv
 
 }
 
@@ -42,14 +42,15 @@
 }
 
 def convert_to_vlmd(
     filepath,
     data_dictionary_props={},
     inputtype=None,
     outputdir=None,
+    sas7bcat_filepath=None
 
     ):
     """
     Writes a data dictionary (i.e. variable level metadata) to a HEAL metadata JSON file using a registered function.
 
     Parameters
     ----------
@@ -77,29 +78,38 @@
     NOTE
     ----
     In future versions, this will be more of a package bundled with corresponding schemas (whether csv or JSON),better organization 
     (e.g., see frictionless Package). 
     However, right now, it simply returns the csvtemplate and jsontemplate as specified
     in the heal specification repository.
     This is an intermediate solution to socialize a proof-of-concept.
+
+    TODO
+    --------
+    make sub command for each file format rather than just one function? Added sas7bcat and can predict additional complexity
     
     """
 
     filepath = Path(filepath)
     
     #infer input type
     if not inputtype:
         inputtype = ''.join(filepath.suffixes)[1:].lower()
 
     ## add dd title
     if not data_dictionary_props.get('title'):
         data_dictionary_props['title'] = filepath.stem
 
+    
     # get data dictionary package based on the input type
-    data_dictionary_package = choice_fxn[inputtype](filepath,data_dictionary_props)
+    if sas7bcat_filepath:
+        data_dictionary_package = choice_fxn[inputtype](filepath,data_dictionary_props,sas7bcat_file_path=sas7bcat_filepath,) 
+    else:
+        data_dictionary_package = choice_fxn[inputtype](filepath,data_dictionary_props)
+
 
     #TODO: currently only validates fields (ie table) but no reason it cant validate entire data package
     package_csv = validate_vlmd_csv(data_dictionary_package['templatecsv']['data_dictionary'],to_sync_fields=True)
     package_json = validate_vlmd_json(data_dictionary_package['templatejson'])
 
     # TODO: in future just return the packages (eg reports nested within package and not out of)
     # for now, keep same (report_xxx and templatexxx)
@@ -132,20 +142,20 @@
                 quoting=csv.QUOTE_NONNUMERIC)
 
         )
 
         # print errors
 
         if not report_json['valid']:
-            print("JSON data dictionary not valid, see heal-json-errors.json")
+            print("JSON data dictionary not valid, see heal-json-errors.json for errors.")
+            print(f"(view the outputted data dictionary at {jsontemplate_path})")
  
         if not report_csv['valid']:
-            print("CSV data dictionary not valid, see heal-csv-errors.json and")
-            print("heal-csv-errors-summary.txt (which is a more human-readable error report)")
-        
+            print("CSV data dictionary not valid, see heal-csv-errors.json")
+            print(f"(view the outputted data dictionary at {csvtemplate_path})")
         
         # write error reports to file
         errordir = Path(outputdir).joinpath('errors')
         errordir.mkdir(exist_ok=True)
         errordir.joinpath('heal-json-errors.json').write_text(
             json.dumps(report_json,indent=4)
         )
@@ -163,21 +173,22 @@
 
 @click.command()
 @click.option('--filepath',required=True,help='Path to the file you want to convert to a HEAL data dictionary')
 @click.option('--title',default=None,help='The title of your data dictionary. If not specified, then the file name will be used')
 @click.option('--description',default=None,help='Description of data dictionary')
 @click.option('--inputtype',default=None,type=click.Choice(list(choice_fxn.keys())),help='The type of your input file.')
 @click.option('--outputdir',default="",help='The folder where you want to output your HEAL data dictionary')
-def main(filepath,title,description,inputtype,outputdir):
+@click.option('--sas7bcat-filepath',default=None,help="[FOR SAS7BDAT ONLY]: Path to a sas catalog file (sas7bcat). Needed for value formats if a sas (sas7bdat) input file")
+def main(filepath,title,description,inputtype,outputdir,sas7bcat_filepath):
     data_dictionary_props = {'title':title,'description':description}
 
     #save dds and error reports to files
     data_dictionaries = convert_to_vlmd(
         filepath=filepath,
         data_dictionary_props=data_dictionary_props,
         outputdir=outputdir,
         inputtype=inputtype,
-
+        sas7bcat_filepath=sas7bcat_filepath
     )
      
 if __name__=='__main__':
     main()
```

### Comparing `healdata_utils-0.0.7a0/src/healdata_utils/io.py` & `healdata_utils-0.0.8a0/src/healdata_utils/io.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.7a0/src/healdata_utils/transforms/csvdata/conversion.py` & `healdata_utils-0.0.8a0/src/healdata_utils/transforms/csvdata/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.7a0/src/healdata_utils/transforms/csvtemplate/conversion.py` & `healdata_utils-0.0.8a0/src/healdata_utils/transforms/csvtemplate/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.7a0/src/healdata_utils/transforms/csvtemplate/mappings.py` & `healdata_utils-0.0.8a0/src/healdata_utils/transforms/csvtemplate/mappings.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.7a0/src/healdata_utils/transforms/frictionless/conversion.py` & `healdata_utils-0.0.8a0/src/healdata_utils/transforms/frictionless/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.7a0/src/healdata_utils/transforms/jsontemplate/conversion.py` & `healdata_utils-0.0.8a0/src/healdata_utils/transforms/jsontemplate/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.7a0/src/healdata_utils/transforms/jsontemplate/mappings.py` & `healdata_utils-0.0.8a0/src/healdata_utils/transforms/jsontemplate/mappings.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.7a0/src/healdata_utils/transforms/readstat/conversion.py` & `healdata_utils-0.0.8a0/src/healdata_utils/transforms/readstat/conversion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import pandas as pd
 from healdata_utils.utils import to_int_if_base10
 from healdata_utils.io import read_pyreadstat
+from healdata_utils.types import typesets
 from ..jsontemplate.conversion import convert_templatejson
-
 from datetime import datetime
 
 
 def convert_readstat(file_path,
-    data_dictionary_props={}):
+    data_dictionary_props={},
+    sas7bcat_file_path=None,):
     """
     Converts a "metadata-rich" (ie statistical software file) 
     into a HEAL-specified data dictionary in both csv format and json format.
 
     This function relies on [readstat](https://github.com/Roche/pyreadstat) which supports SPSS (sav and por), 
     SAS (sas7bdat), and Stata (dta). 
 
     > Currently, this function uses both data and metadata to generate 
     a HEAL specified data dictionary. That is, types are inferred from the 
     data (so at least test or synthetic data needed) while everything else is taken 
     from the metadata (eg missing values, variable labels, variable value labels etc)
 
     Parameters
     ----------
-    csvtemplate : str or path-like or any object
+    file_path : str or path-like or any object
         Data or path to data with the data being a tabular HEAL-specified data dictionary.
         This input can be any data object or path-like string excepted by a frictionless Resource object.
     data_dictionary_props : dict
         The HEAL-specified data dictionary properties.
-    mappings : dict, optional
-        Mappings (which can be a dictionary of either lambda functions or other to-be-mapped objects).
-        Default: specified fieldmap.
+    
+    sas7bcat_file_path : str or path-like
+        Path to a sas catalog file (sas7bcat). Needed for value formats if a sas (sas7bdat) input file
 
     Returns
     -------
     dict
         A dictionary with two keys:
             - 'templatejson': the HEAL-specified JSON object.
             - 'templatecsv': the HEAL-specified tabular template.
@@ -59,19 +60,17 @@
         Values are a list of character values (A to Z and _ for SAS, a to z for SATA) 
         representing user defined missing values in SAS and STATA. 
         This appears when using user_missing=True in read_sas7bdat or read_dta 
         if user defined missing values are present.
 
     """
     
-    _,meta = read_pyreadstat(file_path,user_missing=True) # get user missing values (for stata/sas will make string so need sep call to infer types)
+    _,meta = read_pyreadstat(file_path,catalog_file=sas7bcat_file_path,user_missing=True) # get user missing values (for stata/sas will make string so need sep call to infer types)
     df,_ = read_pyreadstat(file_path) # dont fill user defined missing vals (to get correct types)
-    df = df.convert_dtypes() #TODO: use visions package for inference (from pandas profile project)
-    fields = pd.io.json.build_table_schema(df,index=False)['fields'] #converts to frictionless Table Schema
-
+    fields = typesets.infer_frictionless_fields(df)
 
     for field in fields:
         field.pop('extDtype',None)
         fieldname = field['name']
 
         value_labels = meta.variable_value_labels.get(fieldname)
         missing_values = meta.missing_user_values.get(fieldname,[])
@@ -92,16 +91,14 @@
         if value_labels:
             field['encodings'] = value_labels
             #NOTE: enums are assumed if labels represent entire set of values
             # this avoids value labels that are, for example, partials such as top/bottom encodings
             enums = set(value_labels.keys()).difference(set(missing_values))
             constraints_enums = {'constraints':{'enum':[str(v) for v in enums]}}
             field.update(constraints_enums)
-
-        #NOTE/TODO: for SPSS no functionality for incorporating missing ranges
         
         if missing_values:
             field['missingValues'] = missing_values
 
         variable_label = meta.column_names_to_labels.get(fieldname)
         if variable_label:
             field['description'] = variable_label
```

### Comparing `healdata_utils-0.0.7a0/src/healdata_utils/transforms/redcapcsv/conversion.py` & `healdata_utils-0.0.8a0/src/healdata_utils/transforms/redcapcsv/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.7a0/src/healdata_utils/transforms/redcapcsv/headers.py` & `healdata_utils-0.0.8a0/src/healdata_utils/transforms/redcapcsv/headers.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.7a0/src/healdata_utils/transforms/redcapcsv/mappings.py` & `healdata_utils-0.0.8a0/src/healdata_utils/transforms/redcapcsv/mappings.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.7a0/src/healdata_utils/transforms/redcapcsv/schema.py` & `healdata_utils-0.0.8a0/src/healdata_utils/transforms/redcapcsv/schema.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.7a0/src/healdata_utils/types/typesets.py` & `healdata_utils-0.0.8a0/src/healdata_utils/types/typesets.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.7a0/src/healdata_utils/utils.py` & `healdata_utils-0.0.8a0/src/healdata_utils/utils.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.7a0/src/healdata_utils/validators/jsonschema.py` & `healdata_utils-0.0.8a0/src/healdata_utils/validators/jsonschema.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.7a0/src/healdata_utils/validators/validate.py` & `healdata_utils-0.0.8a0/src/healdata_utils/validators/validate.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.7a0/src/healdata_utils.egg-info/PKG-INFO` & `healdata_utils-0.0.8a0/src/healdata_utils.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 Metadata-Version: 2.1
 Name: healdata-utils
-Version: 0.0.7a0
+Version: 0.0.8a0
 Summary: Data packaging tools for the HEAL data ecosystem
 Home-page: https://github.com/norc-heal/healdata-utils
 Author: Michael Kranz
 Author-email: kranz-michael@norc.org
 Description-Content-Type: text/markdown
 
+--8<-- [start:intro]
+
 # HEAL Data Utilities
 
 The HEAL data utilities python package provides data packaging tools for the HEAL data ecosystem to facilitate data discovery,sharing, and harmonization with a focus on the HEAL platform data consultancy (DSC).
  
 Currently, the focus of the repo is on generating data-dictionaries (see Variable level metadata section below). However, in the future, this will be expanded for all heal specific data packaging functions (e.g., study and file level metadata and data).
 
 ## Installation
 
 To install the latest official release of healdata-utils, from your computer's command prompt, run:
 
-`pip install healdata-utils`
-
-to install the working, un-released version from this git repository, run:
+`pip install healdata-utils --pre` (**NOTE: currently in pre-lease**)
 
 `pip install git+https://github.com/norc-heal/healdata-utils.git`
 
 
-### Variable level metadata (data dictionaries)
+## Variable level metadata (data dictionaries)
 
 [![Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/norc-heal/healdata-utils/HEAD?labpath=notebooks%2Fdemos%2Finputs-to-heal-data-dictionary.ipynb) 
 
 The healdata-utils variable level metadata (vlmd) tool inputs a variety of different input file types and exports HEAL-formatted data dictionaries (JSON and CSV formats). Additionally, exported validation (ie "error") reports provide the user information as to a. if the exported data dictionary is valid according to HEAL specifications (see the schema repository [here](https://github.com/norc-heal/heal-metadata-schemas/tree/main/variable-level-metadata-schema)).
 
+For support formats and more detailed software specific instructions and recommendations, [see here](docs/supported_input_formats.md)
 
-## Basic usage 
+### Basic usage 
 
 The vlmd tool can be used via python or the command line.
 
-### Using from python
+#### Using from python
 
 From your current working directory in python, run:
 
 ```python
 from healdata_utils.cli import convert_to_vlmd
 
 # description and title are optional. If submitting through platform, can fill these out there.
@@ -65,51 +66,59 @@
 
 input_descriptions
 
 ```
 
 The `input_descriptions` object contains the choice for `inputtype` as the key and the description as the value.
 
-### Using from the command line
+#### Using from the command line
 
 From your current working directory run:
 (note the `\` at the end of each line signals a line continuation for ease in understanding the long one line command.) Again the `--title` and `--description` options are optional.
 For descriptions on the different flags/options, run `vlmd --help`
 
 ```bash
 
 vlmd --filepath "data/example_pyreadstat_output.sav" \
 --outputdir "output-cli" \
 --title "Healdata-utils Demonstration Data Dictionary" \
 --description "This is a proof of concept to demonstrate the healdata-utils functionality" 
 ```
 
-### Output
+#### Output
 
-Both the python and command line routes will result in a JSON and CSV version of the HEAL  data dictionary in the output folder along with 
-the validation reports in the `errors` folder. See below:
+Both the python and command line routes will result in a JSON and CSV version of the HEAL  data dictionary in the output folder along with the validation reports in the `errors` folder. See below:
 
 - `input/input/my-redcap-data-dictionary-export.csv` : your input file
 
 - `output/errors/heal-csv-errors.json`: outputted validation report for table in csv file against frictionless schema
     - see schema [here](https://github.com/norc-heal/heal-metadata-schemas/blob/main/variable-level-metadata-schema/schemas/frictionless/csvtemplate/fields.json)
 - `output/errors/heal-json-errors.json`:  outputted jsonschema validation report.
     - see schema [here](https://github.com/norc-heal/heal-metadata-schemas/blob/main/variable-level-metadata-schema/schemas/jsonschema/data-dictionary.json)
 
+!!! important
+    The main difference* between the CSV and JSON data dictionary validation lies in the way the data dictionaries are structured and the additional metadata included in the JSON data dictionary.
+    
+    The CSV data dictionary is a plain tabular representation with no additional metadata, while the JSON dataset includes fields along with additional metadata in the form of a root description and title.
+
+    * for field-specific differences, see the schemas in the documentation. 
+    
+
 - `output/heal-csvtemplate-data-dictionary.csv`: This is the CSV data dictionary
 - `output/heal-jsontemplate-data-dictionary.json`: This is the JSON version of the data dictionary
 
 > Note, only the JSON version will have the user-specified `title` and `description`
 
-
-### Examples
+### Interactive notebooks
 
 See the below notebooks demonstrating use and workflows using the `convert_to_vlmd` in python and `vlmd` in the command line. 
 
 > Clicking on the "binder badges" will bring you to an interactive notebook page where you can test out the notebooks. Here, healdata-utils comes pre-installed.
 
 1. Generating a heal data dictionary from a variety of input files 
 
 - [click here for static notebook ](notebooks/demos/inputs-to-heal-data-dictionary.ipynb) 
 - click binder badge for interactive [![Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/norc-heal/healdata-utils/HEAD?labpath=notebooks%2Fdemos%2Finputs-to-heal-data-dictionary.ipynb) 
 
 2. [in development] Creating and iterating over a csv data dictionary to create a valid data dictionary file [click here](notebooks/demos/demo-csvtemplate-validation.ipynb)
+
+--8<-- [end:intro]
```

### Comparing `healdata_utils-0.0.7a0/src/healdata_utils.egg-info/SOURCES.txt` & `healdata_utils-0.0.8a0/src/healdata_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.7a0/tests/test_cli.py` & `healdata_utils-0.0.8a0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.7a0/tests/test_schemas.py` & `healdata_utils-0.0.8a0/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.7a0/tests/test_utils.py` & `healdata_utils-0.0.8a0/tests/test_utils.py`

 * *Files identical despite different names*

