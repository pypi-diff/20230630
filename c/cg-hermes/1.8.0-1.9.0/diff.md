# Comparing `tmp/cg-hermes-1.8.0.tar.gz` & `tmp/cg-hermes-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cg-hermes-1.8.0.tar", max compression
+gzip compressed data, was "cg-hermes-1.9.0.tar", max compression
```

## Comparing `cg-hermes-1.8.0.tar` & `cg-hermes-1.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       22 2022-12-15 13:51:11.485368 cg-hermes-1.8.0/cg_hermes/__init__.py
--rw-r--r--   0        0        0      289 2022-12-15 13:51:11.485368 cg-hermes-1.8.0/cg_hermes/__main__.py
--rw-r--r--   0        0        0        0 2022-12-15 13:51:11.485368 cg-hermes-1.8.0/cg_hermes/cli/__init__.py
--rw-r--r--   0        0        0     1010 2022-12-15 13:51:11.485368 cg-hermes-1.8.0/cg_hermes/cli/base.py
--rw-r--r--   0        0        0      916 2022-12-15 13:51:11.485368 cg-hermes-1.8.0/cg_hermes/cli/common.py
--rw-r--r--   0        0        0     1482 2022-12-15 13:51:11.485368 cg-hermes-1.8.0/cg_hermes/cli/convert.py
--rw-r--r--   0        0        0     3377 2022-12-15 13:51:11.489368 cg-hermes-1.8.0/cg_hermes/cli/export.py
--rw-r--r--   0        0        0     2972 2022-12-15 13:51:11.489368 cg-hermes-1.8.0/cg_hermes/cli/validate.py
--rw-r--r--   0        0        0    21295 2022-12-15 13:51:11.489368 cg-hermes-1.8.0/cg_hermes/config/balsamic.py
--rw-r--r--   0        0        0     1590 2022-12-15 13:51:11.489368 cg-hermes-1.8.0/cg_hermes/config/balsamic_qc.py
--rw-r--r--   0        0        0     5366 2022-12-15 13:51:11.489368 cg-hermes-1.8.0/cg_hermes/config/balsamic_umi.py
--rw-r--r--   0        0        0      845 2022-12-15 13:51:11.489368 cg-hermes-1.8.0/cg_hermes/config/fluffy.py
--rw-r--r--   0        0        0     2164 2022-12-15 13:51:11.489368 cg-hermes-1.8.0/cg_hermes/config/microsalt.py
--rw-r--r--   0        0        0     7876 2022-12-15 13:51:11.489368 cg-hermes-1.8.0/cg_hermes/config/mip_dna.py
--rw-r--r--   0        0        0     4543 2022-12-15 13:51:11.489368 cg-hermes-1.8.0/cg_hermes/config/mip_rna.py
--rw-r--r--   0        0        0     4167 2022-12-15 13:51:11.489368 cg-hermes-1.8.0/cg_hermes/config/mutant.py
--rw-r--r--   0        0        0      675 2022-12-15 13:51:11.489368 cg-hermes-1.8.0/cg_hermes/config/nextflow.py
--rw-r--r--   0        0        0      231 2022-12-15 13:51:11.489368 cg-hermes-1.8.0/cg_hermes/config/pipelines.py
--rw-r--r--   0        0        0     2002 2022-12-15 13:51:11.489368 cg-hermes-1.8.0/cg_hermes/config/rnafusion.py
--rw-r--r--   0        0        0    13650 2022-12-15 13:51:11.489368 cg-hermes-1.8.0/cg_hermes/config/tags.py
--rw-r--r--   0        0        0    12398 2022-12-15 13:51:11.489368 cg-hermes-1.8.0/cg_hermes/deliverables.py
--rw-r--r--   0        0        0      364 2022-12-15 13:51:11.489368 cg-hermes-1.8.0/cg_hermes/exceptions.py
--rw-r--r--   0        0        0        0 2022-12-15 13:51:11.489368 cg-hermes-1.8.0/cg_hermes/models/__init__.py
--rw-r--r--   0        0        0     2482 2022-12-15 13:51:11.489368 cg-hermes-1.8.0/cg_hermes/models/pipeline_deliverables.py
--rw-r--r--   0        0        0      689 2022-12-15 13:51:11.489368 cg-hermes-1.8.0/cg_hermes/models/tags.py
--rw-r--r--   0        0        0     1788 2022-12-15 13:51:11.489368 cg-hermes-1.8.0/cg_hermes/validate.py
--rw-r--r--   0        0        0      774 2022-12-15 13:51:11.489368 cg-hermes-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     1020 1970-01-01 00:00:00.000000 cg-hermes-1.8.0/setup.py
--rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 cg-hermes-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-02-21 10:56:17.260483 cg-hermes-1.9.0/cg_hermes/__init__.py
+-rw-r--r--   0        0        0      289 2023-02-21 10:56:17.260483 cg-hermes-1.9.0/cg_hermes/__main__.py
+-rw-r--r--   0        0        0        0 2023-02-21 10:56:17.260483 cg-hermes-1.9.0/cg_hermes/cli/__init__.py
+-rw-r--r--   0        0        0     1010 2023-02-21 10:56:17.260483 cg-hermes-1.9.0/cg_hermes/cli/base.py
+-rw-r--r--   0        0        0      916 2023-02-21 10:56:17.260483 cg-hermes-1.9.0/cg_hermes/cli/common.py
+-rw-r--r--   0        0        0     1482 2023-02-21 10:56:17.260483 cg-hermes-1.9.0/cg_hermes/cli/convert.py
+-rw-r--r--   0        0        0     3377 2023-02-21 10:56:17.260483 cg-hermes-1.9.0/cg_hermes/cli/export.py
+-rw-r--r--   0        0        0     2972 2023-02-21 10:56:17.260483 cg-hermes-1.9.0/cg_hermes/cli/validate.py
+-rw-r--r--   0        0        0    21295 2023-02-21 10:56:17.264483 cg-hermes-1.9.0/cg_hermes/config/balsamic.py
+-rw-r--r--   0        0        0     1590 2023-02-21 10:56:17.264483 cg-hermes-1.9.0/cg_hermes/config/balsamic_qc.py
+-rw-r--r--   0        0        0     5366 2023-02-21 10:56:17.264483 cg-hermes-1.9.0/cg_hermes/config/balsamic_umi.py
+-rw-r--r--   0        0        0      845 2023-02-21 10:56:17.264483 cg-hermes-1.9.0/cg_hermes/config/fluffy.py
+-rw-r--r--   0        0        0     2164 2023-02-21 10:56:17.264483 cg-hermes-1.9.0/cg_hermes/config/microsalt.py
+-rw-r--r--   0        0        0     7876 2023-02-21 10:56:17.264483 cg-hermes-1.9.0/cg_hermes/config/mip_dna.py
+-rw-r--r--   0        0        0     4543 2023-02-21 10:56:17.264483 cg-hermes-1.9.0/cg_hermes/config/mip_rna.py
+-rw-r--r--   0        0        0     4167 2023-02-21 10:56:17.264483 cg-hermes-1.9.0/cg_hermes/config/mutant.py
+-rw-r--r--   0        0        0      675 2023-02-21 10:56:17.264483 cg-hermes-1.9.0/cg_hermes/config/nextflow.py
+-rw-r--r--   0        0        0      231 2023-02-21 10:56:17.264483 cg-hermes-1.9.0/cg_hermes/config/pipelines.py
+-rw-r--r--   0        0        0     2289 2023-02-21 10:56:17.264483 cg-hermes-1.9.0/cg_hermes/config/rnafusion.py
+-rw-r--r--   0        0        0    13784 2023-02-21 10:56:17.264483 cg-hermes-1.9.0/cg_hermes/config/tags.py
+-rw-r--r--   0        0        0    12398 2023-02-21 10:56:17.264483 cg-hermes-1.9.0/cg_hermes/deliverables.py
+-rw-r--r--   0        0        0      364 2023-02-21 10:56:17.264483 cg-hermes-1.9.0/cg_hermes/exceptions.py
+-rw-r--r--   0        0        0        0 2023-02-21 10:56:17.264483 cg-hermes-1.9.0/cg_hermes/models/__init__.py
+-rw-r--r--   0        0        0     2482 2023-02-21 10:56:17.264483 cg-hermes-1.9.0/cg_hermes/models/pipeline_deliverables.py
+-rw-r--r--   0        0        0      689 2023-02-21 10:56:17.264483 cg-hermes-1.9.0/cg_hermes/models/tags.py
+-rw-r--r--   0        0        0     1788 2023-02-21 10:56:17.264483 cg-hermes-1.9.0/cg_hermes/validate.py
+-rw-r--r--   0        0        0      774 2023-02-21 10:56:17.264483 cg-hermes-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1020 1970-01-01 00:00:00.000000 cg-hermes-1.9.0/setup.py
+-rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 cg-hermes-1.9.0/PKG-INFO
```

### Comparing `cg-hermes-1.8.0/cg_hermes/cli/base.py` & `cg-hermes-1.9.0/cg_hermes/cli/base.py`

 * *Files identical despite different names*

### Comparing `cg-hermes-1.8.0/cg_hermes/cli/common.py` & `cg-hermes-1.9.0/cg_hermes/cli/common.py`

 * *Files identical despite different names*

### Comparing `cg-hermes-1.8.0/cg_hermes/cli/convert.py` & `cg-hermes-1.9.0/cg_hermes/cli/convert.py`

 * *Files identical despite different names*

### Comparing `cg-hermes-1.8.0/cg_hermes/cli/export.py` & `cg-hermes-1.9.0/cg_hermes/cli/export.py`

 * *Files identical despite different names*

### Comparing `cg-hermes-1.8.0/cg_hermes/cli/validate.py` & `cg-hermes-1.9.0/cg_hermes/cli/validate.py`

 * *Files identical despite different names*

### Comparing `cg-hermes-1.8.0/cg_hermes/config/balsamic.py` & `cg-hermes-1.9.0/cg_hermes/config/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-hermes-1.8.0/cg_hermes/config/balsamic_qc.py` & `cg-hermes-1.9.0/cg_hermes/config/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-hermes-1.8.0/cg_hermes/config/balsamic_umi.py` & `cg-hermes-1.9.0/cg_hermes/config/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-hermes-1.8.0/cg_hermes/config/fluffy.py` & `cg-hermes-1.9.0/cg_hermes/config/fluffy.py`

 * *Files identical despite different names*

### Comparing `cg-hermes-1.8.0/cg_hermes/config/microsalt.py` & `cg-hermes-1.9.0/cg_hermes/config/microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-hermes-1.8.0/cg_hermes/config/mip_dna.py` & `cg-hermes-1.9.0/cg_hermes/config/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-hermes-1.8.0/cg_hermes/config/mip_rna.py` & `cg-hermes-1.9.0/cg_hermes/config/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-hermes-1.8.0/cg_hermes/config/mutant.py` & `cg-hermes-1.9.0/cg_hermes/config/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-hermes-1.8.0/cg_hermes/config/nextflow.py` & `cg-hermes-1.9.0/cg_hermes/config/nextflow.py`

 * *Files identical despite different names*

### Comparing `cg-hermes-1.8.0/cg_hermes/config/rnafusion.py` & `cg-hermes-1.9.0/cg_hermes/config/rnafusion.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,61 +7,66 @@
 from cg_hermes.config.nextflow import NEXTFLOW_COMMON_TAGS
 
 RNAFUSION_COMMON_TAGS = {
     frozenset({"arriba"}): {
         "is_mandatory": True,
         "bundle_id": True,
         "tags": ["arriba", "fusion"],
-        "used_by": ["cg"],
+        "used_by": ["deliver"],
     },
     frozenset({"arriba-visualisation", "arriba"}): {
         "is_mandatory": True,
         "bundle_id": True,
-        "tags": ["arriba-visualisation", "visualization", "arriba"],
-        "used_by": ["cg"],
+        "tags": ["arriba-visualisation", "visualization", "arriba", "research"],
+        "used_by": ["deliver", "scout"],
     },
     frozenset({"fusioncatcher"}): {
         "is_mandatory": True,
         "tags": ["fusioncatcher", "fusion"],
-        "used_by": ["cg"],
+        "used_by": ["deliver"],
     },
     frozenset({"fusioncatcher-summary", "fusioncatcher"}): {
         "is_mandatory": True,
         "tags": ["fusioncatcher-summary"],
-        "used_by": ["cg"],
+        "used_by": ["deliver"],
     },
     frozenset({"pizzly"}): {
         "is_mandatory": True,
         "tags": ["pizzly", "fusion"],
-        "used_by": ["cg"],
+        "used_by": ["deliver"],
     },
     frozenset({"star-fusion"}): {
         "is_mandatory": True,
         "tags": ["star-fusion", "fusion"],
-        "used_by": ["cg"],
+        "used_by": ["deliver"],
     },
     frozenset({"squid"}): {
         "is_mandatory": True,
         "tags": ["squid", "fusion"],
-        "used_by": ["cg"],
+        "used_by": ["deliver"],
     },
     frozenset({"fusionreport", "report"}): {
         "is_mandatory": True,
-        "tags": ["fusionreport"],
-        "used_by": ["cg"],
+        "tags": ["fusionreport", "research"],
+        "used_by": ["deliver", "scout"],
     },
     frozenset({"fusioninspector", "report"}): {
         "is_mandatory": True,
         "tags": ["fusioninspector"],
-        "used_by": ["cg"]
+        "used_by": ["deliver"]
+    },
+    frozenset({"fusioninspector-html", "report"}): {
+        "is_mandatory": True,
+        "tags": ["fusioninspector-html", "research"],
+        "used_by": ["deliver", "scout"]
     },
     frozenset({"multiqc-html", "report"}): {
         "is_mandatory": True,
-        "tags": ["multiqc-html"],
-        "used_by": ["deliver"],
+        "tags": ["multiqc-html", "rna"],
+        "used_by": ["deliver", "scout"],
     },
 }
 
 NXF_RNAFUSION_COMMON_TAGS = {**RNAFUSION_COMMON_TAGS, **NEXTFLOW_COMMON_TAGS}
 
 
 #
```

### Comparing `cg-hermes-1.8.0/cg_hermes/config/tags.py` & `cg-hermes-1.9.0/cg_hermes/config/tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 RAW_DATA = {
     "fastq": {"description": "Files with raw data in fastq format"},
     "fasta": {"description": "Files with raw data in fasta format"},
     "forward-strand": {"description": "Reads from forward strand"},
     "reverse-strand": {"description": "Reads from reverse strand"},
     "unpaired-reads": {"description": "Reads that could not be paired"},
+    "rna": {"description": "Data generated from RNA samples"},
 }
 
 
 VARIANT_COMMON = {
     "cnv": {"description": "Copy number variants"},
     "normal": {"description": "Associated with normal sample"},
     "germline": {"description": "Associated with germline variants"},
@@ -226,14 +227,15 @@
         "description": "Pangolin typing report with only qc_pass samples included"
     },
 }
 
 RNAFUSION_SPECIFIC = {
     "arriba-visualisation": {"description": "Arriba visualization"},
     "fusionreport": {"description": "Fusion-report analysis"},
+    "fusioninspector-html": {"description": "Fusioninspector report"},
 }
 
 NEXTFLOW_SPECIFIC = {
     "samplesheet-valid": {"description": "Validated samplesheet"},
     "software-versions": {"description": "List of all software used and their versions"},
 }
```

### Comparing `cg-hermes-1.8.0/cg_hermes/deliverables.py` & `cg-hermes-1.9.0/cg_hermes/deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-hermes-1.8.0/cg_hermes/models/pipeline_deliverables.py` & `cg-hermes-1.9.0/cg_hermes/models/pipeline_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-hermes-1.8.0/cg_hermes/models/tags.py` & `cg-hermes-1.9.0/cg_hermes/models/tags.py`

 * *Files identical despite different names*

### Comparing `cg-hermes-1.8.0/cg_hermes/validate.py` & `cg-hermes-1.9.0/cg_hermes/validate.py`

 * *Files identical despite different names*

### Comparing `cg-hermes-1.8.0/pyproject.toml` & `cg-hermes-1.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cg-hermes"
-version = "1.8.0"
+version = "1.9.0"
 description = "Convert information between pipelines and CG"
 authors = ["Måns Magnusson <mans.magnusson@scilifelab.se>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pydantic = "^1.7.3"
 coloredlogs = "^14.0"
```

### Comparing `cg-hermes-1.8.0/setup.py` & `cg-hermes-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'typing-extensions>=3.7.4,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['hermes = cg_hermes.__main__:main']}
 
 setup_kwargs = {
     'name': 'cg-hermes',
-    'version': '1.8.0',
+    'version': '1.9.0',
     'description': 'Convert information between pipelines and CG',
     'long_description': 'None',
     'author': 'Måns Magnusson',
     'author_email': 'mans.magnusson@scilifelab.se',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `cg-hermes-1.8.0/PKG-INFO` & `cg-hermes-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg-hermes
-Version: 1.8.0
+Version: 1.9.0
 Summary: Convert information between pipelines and CG
 Author: Måns Magnusson
 Author-email: mans.magnusson@scilifelab.se
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

