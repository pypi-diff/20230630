# Comparing `tmp/cumulus_library-0.3.2.tar.gz` & `tmp/cumulus_library-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumulus_library-0.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cumulus_library-0.3.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cumulus_library-0.3.2.tar` & `cumulus_library-0.3.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-lrwxr-xr-x   0        0        0        0 2023-06-29 19:41:10.761678 cumulus_library-0.3.2/.sqlfluff -> cumulus_library/.sqlfluff
--rw-r--r--   0        0        0      587 2023-06-29 19:41:10.761678 cumulus_library-0.3.2/README.md
--rw-r--r--   0        0        0      963 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/.sqlfluff
--rw-r--r--   0        0        0       45 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/__init__.py
--rw-r--r--   0        0        0      628 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/base_runner.py
--rwxr-xr-x   0        0        0    11182 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/cli.py
--rw-r--r--   0        0        0     5249 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/cli_parser.py
--rw-r--r--   0        0        0      272 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/errors.py
--rw-r--r--   0        0        0     1889 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/helper.py
--rw-r--r--   0        0        0      205 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/module_allowlist.json
--rw-r--r--   0        0        0     2343 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/parsers/fhir_valueset.py
--rw-r--r--   0        0        0        0 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/schema/__init__.py
--rw-r--r--   0        0        0     4848 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/schema/columns.py
--rw-r--r--   0        0        0     3346 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/schema/counts.py
--rw-r--r--   0        0        0     3364 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/schema/typesystem.py
--rw-r--r--   0        0        0     5876 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/schema/valueset.py
--rw-r--r--   0        0        0     2549 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/condition.sql
--rw-r--r--   0        0        0     2688 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/condition_codable_concept.sql
--rw-r--r--   0        0        0     4176 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/denormalizer.py
--rw-r--r--   0        0        0     2857 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/documentreference.sql
--rw-r--r--   0        0        0     3294 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/encounter.sql
--rw-r--r--   0        0        0     4126 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/fhir_define.sql
--rw-r--r--   0        0        0      661 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/manifest.toml
--rw-r--r--   0        0        0     1231 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/medication_request.sql
--rw-r--r--   0        0        0     1208 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/observation.sql
--rw-r--r--   0        0        0     2874 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/observation_lab.sql
--rw-r--r--   0        0        0     1272 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/observation_vital_signs.sql
--rw-r--r--   0        0        0     1691 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/patient.sql
--rw-r--r--   0        0        0     6521 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/patient_extensions.sql
--rw-r--r--   0        0        0     1426 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/setup.sql
--rw-r--r--   0        0        0     1472 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/study_period.sql
--rw-r--r--   0        0        0      824 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/template/counts.sql
--rw-r--r--   0        0        0      187 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/template/date_range.sql
--rw-r--r--   0        0        0      566 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/template/lab_observations.sql
--rw-r--r--   0        0        0     1562 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/template/manifest.toml
--rw-r--r--   0        0        0     1142 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/template/setup.sql
--rw-r--r--   0        0        0 10584966 2023-06-29 19:41:10.805678 cumulus_library-0.3.2/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv
--rw-r--r--   0        0        0 35303095 2023-06-29 19:41:10.905679 cumulus_library-0.3.2/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv
--rw-r--r--   0        0        0  1708185 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv
--rw-r--r--   0        0        0      394 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/studies/vocab/icd_legend.sql
--rw-r--r--   0        0        0      138 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/studies/vocab/manifest.toml
--rw-r--r--   0        0        0     4643 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/studies/vocab/vocab_icd_builder.py
--rw-r--r--   0        0        0    16059 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/study_parser.py
--rw-r--r--   0        0        0     1353 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja
--rw-r--r--   0        0        0      577 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/template_sql/create_view_as.sql.jinja
--rw-r--r--   0        0        0      610 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/template_sql/ctas.sql.jinja
--rw-r--r--   0        0        0       61 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/template_sql/drop_view_table.sql.jinja
--rw-r--r--   0        0        0     1798 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/template_sql/extension_denormalize.sql.jinja
--rw-r--r--   0        0        0      370 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/template_sql/insert_into.sql.jinja
--rw-r--r--   0        0        0       52 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/template_sql/show_tables.sql.jinja
--rw-r--r--   0        0        0       54 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/template_sql/show_views.sql.jinja
--rw-r--r--   0        0        0     7462 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/template_sql/templates.py
--rw-r--r--   0        0        0     2664 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/upload.py
--rw-r--r--   0        0        0     1588 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 cumulus_library-0.3.2/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/.sqlfluff -> cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0      587 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/README.md
+-rw-r--r--   0        0        0      963 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0       45 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/__init__.py
+-rw-r--r--   0        0        0      628 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/base_runner.py
+-rwxr-xr-x   0        0        0    11182 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/cli.py
+-rw-r--r--   0        0        0     5249 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/cli_parser.py
+-rw-r--r--   0        0        0      272 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/errors.py
+-rw-r--r--   0        0        0     1889 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/helper.py
+-rw-r--r--   0        0        0      205 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/module_allowlist.json
+-rw-r--r--   0        0        0     2343 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/parsers/fhir_valueset.py
+-rw-r--r--   0        0        0        0 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/schema/__init__.py
+-rw-r--r--   0        0        0     4848 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/schema/columns.py
+-rw-r--r--   0        0        0     3346 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/schema/counts.py
+-rw-r--r--   0        0        0     3364 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/schema/typesystem.py
+-rw-r--r--   0        0        0     5876 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/schema/valueset.py
+-rw-r--r--   0        0        0     2549 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/condition.sql
+-rw-r--r--   0        0        0     2688 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/condition_codable_concept.sql
+-rw-r--r--   0        0        0     4176 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/denormalizer.py
+-rw-r--r--   0        0        0     2857 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/documentreference.sql
+-rw-r--r--   0        0        0     3294 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/encounter.sql
+-rw-r--r--   0        0        0     4126 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/fhir_define.sql
+-rw-r--r--   0        0        0      661 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/manifest.toml
+-rw-r--r--   0        0        0     1231 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/medication_request.sql
+-rw-r--r--   0        0        0     1208 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/observation.sql
+-rw-r--r--   0        0        0     2874 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/observation_lab.sql
+-rw-r--r--   0        0        0     1272 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/observation_vital_signs.sql
+-rw-r--r--   0        0        0     1691 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/patient.sql
+-rw-r--r--   0        0        0     6521 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/patient_extensions.sql
+-rw-r--r--   0        0        0     1426 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/setup.sql
+-rw-r--r--   0        0        0     1472 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/study_period.sql
+-rw-r--r--   0        0        0      824 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/template/counts.sql
+-rw-r--r--   0        0        0      187 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/template/date_range.sql
+-rw-r--r--   0        0        0      566 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/template/lab_observations.sql
+-rw-r--r--   0        0        0     1562 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/template/manifest.toml
+-rw-r--r--   0        0        0     1142 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/template/setup.sql
+-rw-r--r--   0        0        0 10584966 2023-06-30 19:42:30.277433 cumulus_library-0.3.3/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv
+-rw-r--r--   0        0        0 35303095 2023-06-30 19:42:30.369432 cumulus_library-0.3.3/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv
+-rw-r--r--   0        0        0  1708185 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv
+-rw-r--r--   0        0        0      394 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/studies/vocab/icd_legend.sql
+-rw-r--r--   0        0        0      138 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/studies/vocab/manifest.toml
+-rw-r--r--   0        0        0     4643 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/studies/vocab/vocab_icd_builder.py
+-rw-r--r--   0        0        0    16059 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/study_parser.py
+-rw-r--r--   0        0        0     1430 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja
+-rw-r--r--   0        0        0      577 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/template_sql/create_view_as.sql.jinja
+-rw-r--r--   0        0        0      610 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/template_sql/ctas.sql.jinja
+-rw-r--r--   0        0        0       61 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/template_sql/drop_view_table.sql.jinja
+-rw-r--r--   0        0        0     1798 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/template_sql/extension_denormalize.sql.jinja
+-rw-r--r--   0        0        0      370 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/template_sql/insert_into.sql.jinja
+-rw-r--r--   0        0        0       52 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/template_sql/show_tables.sql.jinja
+-rw-r--r--   0        0        0       54 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/template_sql/show_views.sql.jinja
+-rw-r--r--   0        0        0     7462 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/template_sql/templates.py
+-rw-r--r--   0        0        0     2664 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/upload.py
+-rw-r--r--   0        0        0     1588 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 cumulus_library-0.3.3/PKG-INFO
```

### Comparing `cumulus_library-0.3.2/README.md` & `cumulus_library-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/.sqlfluff` & `cumulus_library-0.3.3/cumulus_library/.sqlfluff`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/base_runner.py` & `cumulus_library-0.3.3/cumulus_library/base_runner.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/cli.py` & `cumulus_library-0.3.3/cumulus_library/cli.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/cli_parser.py` & `cumulus_library-0.3.3/cumulus_library/cli_parser.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/helper.py` & `cumulus_library-0.3.3/cumulus_library/helper.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/parsers/fhir_valueset.py` & `cumulus_library-0.3.3/cumulus_library/parsers/fhir_valueset.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/schema/columns.py` & `cumulus_library-0.3.3/cumulus_library/schema/columns.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/schema/counts.py` & `cumulus_library-0.3.3/cumulus_library/schema/counts.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/schema/typesystem.py` & `cumulus_library-0.3.3/cumulus_library/schema/typesystem.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/schema/valueset.py` & `cumulus_library-0.3.3/cumulus_library/schema/valueset.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/studies/core/condition.sql` & `cumulus_library-0.3.3/cumulus_library/studies/core/condition.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/studies/core/condition_codable_concept.sql` & `cumulus_library-0.3.3/cumulus_library/studies/core/condition_codable_concept.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/studies/core/denormalizer.py` & `cumulus_library-0.3.3/cumulus_library/studies/core/denormalizer.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/studies/core/documentreference.sql` & `cumulus_library-0.3.3/cumulus_library/studies/core/documentreference.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/studies/core/encounter.sql` & `cumulus_library-0.3.3/cumulus_library/studies/core/encounter.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/studies/core/fhir_define.sql` & `cumulus_library-0.3.3/cumulus_library/studies/core/fhir_define.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/studies/core/manifest.toml` & `cumulus_library-0.3.3/cumulus_library/studies/core/manifest.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/studies/core/medication_request.sql` & `cumulus_library-0.3.3/cumulus_library/studies/core/medication_request.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/studies/core/observation.sql` & `cumulus_library-0.3.3/cumulus_library/studies/core/observation.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/studies/core/observation_lab.sql` & `cumulus_library-0.3.3/cumulus_library/studies/core/observation_lab.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/studies/core/observation_vital_signs.sql` & `cumulus_library-0.3.3/cumulus_library/studies/core/observation_vital_signs.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/studies/core/patient.sql` & `cumulus_library-0.3.3/cumulus_library/studies/core/patient.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/studies/core/patient_extensions.sql` & `cumulus_library-0.3.3/cumulus_library/studies/core/patient_extensions.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/studies/core/setup.sql` & `cumulus_library-0.3.3/cumulus_library/studies/core/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/studies/core/study_period.sql` & `cumulus_library-0.3.3/cumulus_library/studies/core/study_period.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/studies/template/counts.sql` & `cumulus_library-0.3.3/cumulus_library/studies/template/counts.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/studies/template/lab_observations.sql` & `cumulus_library-0.3.3/cumulus_library/studies/template/lab_observations.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/studies/template/manifest.toml` & `cumulus_library-0.3.3/cumulus_library/studies/template/manifest.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/studies/template/setup.sql` & `cumulus_library-0.3.3/cumulus_library/studies/template/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv` & `cumulus_library-0.3.3/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv` & `cumulus_library-0.3.3/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv` & `cumulus_library-0.3.3/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/studies/vocab/vocab_icd_builder.py` & `cumulus_library-0.3.3/cumulus_library/studies/vocab/vocab_icd_builder.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/study_parser.py` & `cumulus_library-0.3.3/cumulus_library/study_parser.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja` & `cumulus_library-0.3.3/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja`

 * *Files 9% similar despite different names*

```diff
@@ -26,30 +26,33 @@
             code,
             display
         FROM system_{{ loop.index0 }}
         {%- if not loop.last %}
         UNION 
         {%- endif -%}
         {%- endfor %}
-        ORDER BY id, priority
-    )
+    ),
 
-    SELECT
-        id,
-        code,
-        code_system,
-        display
-    FROM (
+    partitioned_table AS (
         SELECT
             id,
             code,
             code_system,
             display,
+            priority,
             ROW_NUMBER()
             OVER (
                 PARTITION BY id
             ) AS available_priority
         FROM union_table
-        GROUP BY id, code_system, code, display
+        GROUP BY id, priority, code_system, code, display
+        ORDER BY priority ASC
     )
+
+    SELECT
+        id,
+        code,
+        code_system,
+        display
+    FROM partitioned_table
     WHERE available_priority = 1
 );
```

### Comparing `cumulus_library-0.3.2/cumulus_library/template_sql/create_view_as.sql.jinja` & `cumulus_library-0.3.3/cumulus_library/template_sql/create_view_as.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/template_sql/ctas.sql.jinja` & `cumulus_library-0.3.3/cumulus_library/template_sql/ctas.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/template_sql/extension_denormalize.sql.jinja` & `cumulus_library-0.3.3/cumulus_library/template_sql/extension_denormalize.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/template_sql/templates.py` & `cumulus_library-0.3.3/cumulus_library/template_sql/templates.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/cumulus_library/upload.py` & `cumulus_library-0.3.3/cumulus_library/upload.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/pyproject.toml` & `cumulus_library-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.2/PKG-INFO` & `cumulus_library-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumulus-library
-Version: 0.3.2
+Version: 0.3.3
 Summary: Clinical study SQL generation for data derived from bulk FHIR
 Keywords: FHIR,SQL,Health Informatics
 Requires-Python: >= 3.9, <3.12
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

