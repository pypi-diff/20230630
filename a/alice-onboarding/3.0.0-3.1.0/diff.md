# Comparing `tmp/alice-onboarding-3.0.0.tar.gz` & `tmp/alice-onboarding-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alice-onboarding-3.0.0.tar", last modified: Wed Jun 28 07:55:15 2023, max compression
+gzip compressed data, was "alice-onboarding-3.1.0.tar", last modified: Fri Jun 30 10:38:10 2023, max compression
```

## Comparing `alice-onboarding-3.0.0.tar` & `alice-onboarding-3.1.0.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:15.521479 alice-onboarding-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-06-28 07:55:15.521479 alice-onboarding-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:15.505478 alice-onboarding-3.0.0/alice/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:15.505478 alice-onboarding-3.0.0/alice/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/auth/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/auth/auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/auth/auth_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/auth/cached_token_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/auth/token_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:15.509478 alice-onboarding-3.0.0/alice/onboarding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:15.509478 alice-onboarding-3.0.0/alice/onboarding/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/enums/certificate_locale.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/enums/decision.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/enums/document_side.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/enums/document_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/enums/document_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/enums/duplicates_resource_type.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/enums/match_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/enums/user_state.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/enums/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:15.509478 alice-onboarding-3.0.0/alice/onboarding/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/device_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:15.509478 alice-onboarding-3.0.0/alice/onboarding/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:15.509478 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:15.513479 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/document/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/document/authentic_nfc_chip_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/document/checked_info_code_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/document/coherent_document_dates_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/document/consistent_document_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/document/expected_document_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/document/face_in_document_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/document/face_matching_document_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/document/not_a_printed_document_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/document/not_a_screen_document_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/document/not_a_synthetic_document_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/document/uncompromised_document_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/document/unexpired_document_check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:15.513479 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/field/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/field/cheked_field_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/field/complete_mrz_name_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/field/consistent_field_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/field/expected_field_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/field/over_18_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/field/unexpired_date_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/field/valid_date_format_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/field/valid_date_range_check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:15.513479 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/selfie/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/selfie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/selfie/liveness_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/selfie/only_one_face_check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:15.513479 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/summary/only_one_device_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/checks/summary/only_one_ip_check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:15.517479 alice-onboarding-3.0.0/alice/onboarding/models/report/compliance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/compliance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/compliance/device_out.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/compliance/domain_events_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/compliance/user_event_out.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:15.517479 alice-onboarding-3.0.0/alice/onboarding/models/report/document/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/document/document_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/document/document_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/document/document_report_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/document/document_side.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/document/document_side_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/document/document_side_report_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/document/document_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:15.517479 alice-onboarding-3.0.0/alice/onboarding/models/report/face_matching/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/face_matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/face_matching/face_matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:15.517479 alice-onboarding-3.0.0/alice/onboarding/models/report/other_trusted_document/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/other_trusted_document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/other_trusted_document/other_trusted_document_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/other_trusted_document/other_trusted_document_report_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:15.517479 alice-onboarding-3.0.0/alice/onboarding/models/report/selfie/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/selfie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/selfie/selfie_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:15.517479 alice-onboarding-3.0.0/alice/onboarding/models/report/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/shared/bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/shared/href.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:15.517479 alice-onboarding-3.0.0/alice/onboarding/models/report/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/summary/external_user_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/report/summary/report_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/models/user_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    56105 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/onboarding.py
--rw-r--r--   0 runner    (1001) docker     (123)    63146 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/onboarding_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/onboarding_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/onboarding/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/public_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:15.517479 alice-onboarding-3.0.0/alice/sandbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/sandbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/sandbox/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/sandbox/sandbox_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/sandbox/sandbox_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:15.517479 alice-onboarding-3.0.0/alice/webhooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/webhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/webhooks/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/webhooks/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11234 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/alice/webhooks/webhooks_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:55:15.521479 alice-onboarding-3.0.0/alice_onboarding.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-06-28 07:55:15.000000 alice-onboarding-3.0.0/alice_onboarding.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-06-28 07:55:15.000000 alice-onboarding-3.0.0/alice_onboarding.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 07:55:15.000000 alice-onboarding-3.0.0/alice_onboarding.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 07:55:15.000000 alice-onboarding-3.0.0/alice_onboarding.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-28 07:55:15.000000 alice-onboarding-3.0.0/alice_onboarding.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-28 07:55:15.000000 alice-onboarding-3.0.0/alice_onboarding.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-28 07:55:15.521479 alice-onboarding-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-28 07:55:11.000000 alice-onboarding-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:10.854681 alice-onboarding-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-06-30 10:38:10.854681 alice-onboarding-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:10.846681 alice-onboarding-3.1.0/alice/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:10.846681 alice-onboarding-3.1.0/alice/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/auth/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/auth/auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/auth/auth_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/auth/cached_token_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/auth/token_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:10.850681 alice-onboarding-3.1.0/alice/onboarding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:10.850681 alice-onboarding-3.1.0/alice/onboarding/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/enums/certificate_locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/enums/decision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/enums/document_side.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/enums/document_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/enums/document_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/enums/duplicates_resource_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/enums/match_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/enums/user_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/enums/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:10.850681 alice-onboarding-3.1.0/alice/onboarding/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/device_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:10.850681 alice-onboarding-3.1.0/alice/onboarding/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:10.850681 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:10.850681 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/document/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/document/authentic_nfc_chip_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/document/checked_info_code_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/document/coherent_document_dates_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/document/consistent_document_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/document/expected_document_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/document/face_in_document_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/document/face_matching_document_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/document/not_a_printed_document_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/document/not_a_screen_document_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/document/not_a_synthetic_document_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/document/uncompromised_document_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/document/unexpired_document_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:10.850681 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/field/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/field/cheked_field_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/field/complete_mrz_name_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/field/consistent_field_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/field/expected_field_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/field/over_18_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/field/unexpired_date_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/field/valid_date_format_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/field/valid_date_range_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:10.850681 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/selfie/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/selfie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/selfie/liveness_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/selfie/only_one_face_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:10.854681 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/summary/only_one_device_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/checks/summary/only_one_ip_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:10.854681 alice-onboarding-3.1.0/alice/onboarding/models/report/compliance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/compliance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/compliance/device_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/compliance/domain_events_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/compliance/user_event_out.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:10.854681 alice-onboarding-3.1.0/alice/onboarding/models/report/document/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/document/document_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/document/document_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/document/document_report_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/document/document_side.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/document/document_side_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/document/document_side_report_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/document/document_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:10.854681 alice-onboarding-3.1.0/alice/onboarding/models/report/face_matching/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/face_matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/face_matching/face_matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:10.854681 alice-onboarding-3.1.0/alice/onboarding/models/report/other_trusted_document/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/other_trusted_document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/other_trusted_document/other_trusted_document_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/other_trusted_document/other_trusted_document_report_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:10.854681 alice-onboarding-3.1.0/alice/onboarding/models/report/selfie/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/selfie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/selfie/selfie_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:10.854681 alice-onboarding-3.1.0/alice/onboarding/models/report/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/shared/bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/shared/href.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:10.854681 alice-onboarding-3.1.0/alice/onboarding/models/report/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/summary/external_user_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/report/summary/report_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/models/user_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55466 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/onboarding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62237 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/onboarding_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/onboarding_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/onboarding/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/public_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:10.854681 alice-onboarding-3.1.0/alice/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/sandbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/sandbox/sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/sandbox/sandbox_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/sandbox/sandbox_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:10.854681 alice-onboarding-3.1.0/alice/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/webhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/webhooks/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/webhooks/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11234 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/alice/webhooks/webhooks_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:38:10.854681 alice-onboarding-3.1.0/alice_onboarding.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-06-30 10:38:10.000000 alice-onboarding-3.1.0/alice_onboarding.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-06-30 10:38:10.000000 alice-onboarding-3.1.0/alice_onboarding.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:38:10.000000 alice-onboarding-3.1.0/alice_onboarding.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:38:10.000000 alice-onboarding-3.1.0/alice_onboarding.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-30 10:38:10.000000 alice-onboarding-3.1.0/alice_onboarding.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 10:38:10.000000 alice-onboarding-3.1.0/alice_onboarding.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-30 10:38:10.854681 alice-onboarding-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-30 10:38:08.000000 alice-onboarding-3.1.0/setup.py
```

### Comparing `alice-onboarding-3.0.0/PKG-INFO` & `alice-onboarding-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alice-onboarding
-Version: 3.0.0
+Version: 3.1.0
 Summary: Alice Onboarding Python SDK
 Home-page: https://github.com/alice-biometrics/onboarding-python
 Author: Alice Biometrics
 Author-email: support@alicebiometrics.com
 License: Alice Copyright
 Keywords: onboarding,biometrics,kyc,alice
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alice-onboarding-3.0.0/README.md` & `alice-onboarding-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `alice-onboarding-3.0.0/alice/auth/auth.py` & `alice-onboarding-3.1.0/alice/auth/auth.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-3.0.0/alice/auth/auth_client.py` & `alice-onboarding-3.1.0/alice/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-3.0.0/alice/auth/auth_errors.py` & `alice-onboarding-3.1.0/alice/auth/auth_errors.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,28 @@
+from __future__ import annotations
+
 from dataclasses import dataclass
-from typing import Dict
 
 from meiga import Error
 from requests import Response
 
 
 @dataclass
 class AuthError(Error):
     operation: str
     code: int
-    message: Dict[str, str]
+    message: dict[str, str] | None  # type: ignore
 
     def __str__(self) -> str:
         return self.__repr__()
 
     def __repr__(self) -> str:
         return f"[AuthError: [operation: {self.operation} | code: {self.code} | message: {self.message}]]"
 
     @staticmethod
-    def from_response(operation: str, response: Response) -> "AuthError":
+    def from_response(operation: str, response: Response) -> AuthError:
         code = response.status_code
         try:
             message = response.json()
         except Exception:
             message = {"message": "no content"}
         return AuthError(operation=operation, code=code, message=message)
```

### Comparing `alice-onboarding-3.0.0/alice/auth/cached_token_stack.py` & `alice-onboarding-3.1.0/alice/auth/cached_token_stack.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-3.0.0/alice/auth/token_tools.py` & `alice-onboarding-3.1.0/alice/auth/token_tools.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-3.0.0/alice/onboarding/models/report/compliance/user_event_out.py` & `alice-onboarding-3.1.0/alice/onboarding/models/report/compliance/user_event_out.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-3.0.0/alice/onboarding/models/report/document/document_field.py` & `alice-onboarding-3.1.0/alice/onboarding/models/report/document/document_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import List, Optional
 
 from meiga import Error, Result, Success, isFailure
-from pydantic.main import BaseModel
+from pydantic import BaseModel, Field
 
 from alice.onboarding.models.report.checks.check import Check
 
 
 class ReportV1Field(BaseModel):
     """
     It collects the extracted OCR info
     """
 
     name: str
     value: Optional[str]
     score: Optional[int]
-    checks: List[Check] = []
+    checks: List[Check] = Field(default=[])
 
     def get_check(self, check_key: str) -> Result[Check, Error]:
         for doc_check in self.checks:
             if check_key == doc_check.key:
                 return Success(doc_check)
         return isFailure
```

### Comparing `alice-onboarding-3.0.0/alice/onboarding/models/report/document/document_report.py` & `alice-onboarding-3.1.0/alice/onboarding/models/report/document/document_report.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from datetime import datetime
 from typing import List, Union
 
 from meiga import Error, Result, Success, isFailure
-from pydantic import Field
-from pydantic.main import BaseModel
+from pydantic import BaseModel, Field
 
 from alice.onboarding.models.report.checks.check import Check
 from alice.onboarding.models.report.document.document_field import ReportV1Field
 from alice.onboarding.models.report.document.document_report_meta import (
     DocumentReportMeta,
 )
 from alice.onboarding.models.report.document.document_side_report import (
     DocumentSideReport,
 )
 
 
 class DocumentSidesDetailReport(BaseModel):
-    front: Union[DocumentSideReport, None] = None
-    back: Union[DocumentSideReport, None] = None
-    internal: Union[DocumentSideReport, None] = None
+    front: Union[DocumentSideReport, None] = Field(default=None)
+    back: Union[DocumentSideReport, None] = Field(default=None)
+    internal: Union[DocumentSideReport, None] = Field(default=None)
 
     def get_completed_sides(self) -> int:
         completed_sides = 0
         if self.front:
             completed_sides += 1
         if self.back:
             completed_sides += 1
```

### Comparing `alice-onboarding-3.0.0/alice/onboarding/models/report/document/document_side_report.py` & `alice-onboarding-3.1.0/alice/onboarding/models/report/document/document_side_report.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from datetime import datetime
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from meiga import Error, Result, Success, isFailure
-from pydantic import Field
-from pydantic.main import BaseModel
+from pydantic import BaseModel, Field
 
 from alice.onboarding.models.report.document.document_field import ReportV1Field
 from alice.onboarding.models.report.document.document_side import DocumentSide
 from alice.onboarding.models.report.document.document_side_report_meta import (
     DocumentSideReportMeta,
 )
 from alice.onboarding.models.report.shared.href import Href
@@ -22,16 +21,16 @@
     fields: List[ReportV1Field] = Field(
         default=[], description="Document info extracted from side"
     )
     media: Dict[str, Optional[Href]] = Field(
         description="Document side media resources"
     )
     meta: DocumentSideReportMeta
-    created_at: Optional[datetime]
-    forensics_scores: Optional[Dict[str, Any]]
+    created_at: Union[datetime, None] = Field(default=None)
+    forensics_scores: Union[Dict[str, Any], None] = Field(default=None)
 
     def get_field(self, field_name: str) -> Result[ReportV1Field, Error]:
         for side_field in self.fields:
             if field_name == side_field.name:
                 return Success(side_field)
         return isFailure
```

### Comparing `alice-onboarding-3.0.0/alice/onboarding/models/report/face_matching/face_matching.py` & `alice-onboarding-3.1.0/alice/onboarding/models/report/face_matching/face_matching.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from datetime import datetime
 
-from pydantic import Field
-from pydantic.main import BaseModel
+from pydantic import BaseModel, Field
 
 from alice.onboarding.models.report.document.document_side import DocumentSide
 
 
 class FaceMatchingMeta(BaseModel):
     """
     Face matching metadata
```

### Comparing `alice-onboarding-3.0.0/alice/onboarding/models/report/other_trusted_document/other_trusted_document_report.py` & `alice-onboarding-3.1.0/alice/onboarding/models/report/other_trusted_document/other_trusted_document_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     OtherTrustedDocumentReportMeta,
 )
 from alice.onboarding.models.report.shared.href import Href
 
 
 class OtherTrustedDocumentReport(BaseModel):
     """
-    A other trusted document report_v1 collects all the information extracted for a document during the onboarding process
+    The other trusted document report_v1 collects all the information extracted for a document during the onboarding process
     """
 
     id: str = Field(
         description="Unique identifier (UUID v4 standard)",
         min_length=16,
         max_length=36,
     )
```

### Comparing `alice-onboarding-3.0.0/alice/onboarding/models/report/report.py` & `alice-onboarding-3.1.0/alice/onboarding/models/report/report.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         max_length=36,
     )
     user_id: str = Field(
         description="Unique user identifier (UUID v4 standard)",
         min_length=16,
         max_length=36,
     )
-    version: int = Field(default=1, description="Report version", const=True)
+    version: int = Field(default=1, description="Report version")
     created_at: datetime = Field(description="Report creation time in ISO 8601 format")
     summary: ReportSummary = Field(description="User summary")
     selfies: List[SelfieReport] = Field(description="It collects all user selfies")
     documents: List[DocumentReport] = Field(
         description="It collects all user documents"
     )
     other_trusted_documents: List[OtherTrustedDocumentReport] = Field(
```

### Comparing `alice-onboarding-3.0.0/alice/onboarding/models/report/selfie/selfie_report.py` & `alice-onboarding-3.1.0/alice/onboarding/models/report/selfie/selfie_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from datetime import datetime
 from typing import Dict, List, Optional
 
 from meiga import Error, Result, Success, isFailure
-from pydantic import Field
-from pydantic.main import BaseModel
+from pydantic import BaseModel, Field
 
 from alice.onboarding.models.report.checks.check import Check
 from alice.onboarding.models.report.shared.href import Href
 
 
 class SelfieReport(BaseModel):
     """
```

### Comparing `alice-onboarding-3.0.0/alice/onboarding/models/report/summary/report_summary.py` & `alice-onboarding-3.1.0/alice/onboarding/models/report/summary/report_summary.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-3.0.0/alice/onboarding/onboarding.py` & `alice-onboarding-3.1.0/alice/onboarding/onboarding.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,21 +264,23 @@
             )
 
     @early_return
     def get_users_status(
         self,
         verbose: Optional[bool] = False,
         page: int = 1,
-        page_size: int = 0,
+        page_size: int = 10,
         descending: bool = True,
         authorized: bool = False,
         sort_by: Union[str, None] = None,
         filter_field: Union[str, None] = None,
         filter_value: Union[str, None] = None,
-    ) -> Result[List[Dict[str, str]], Union[OnboardingError, AuthError]]:
+    ) -> Result[
+        Dict[str, Union[List[Dict[str, str]], int]], Union[OnboardingError, AuthError]
+    ]:
         """
 
         Returns every UserStatus available for all the Users in the onboarding platform ordered by creation date.
 
         Parameters
         ----------
         verbose
@@ -297,15 +299,15 @@
             Field used for filtering the users.
         filter_value
             Value used for filtering the users.
 
 
         Returns
         -------
-            A Result where if the operation is successful it returns list of dict which represent the status of each user.
+            A Result where if the operation is successful it returns a dict which represent the status of each user.
             Otherwise, it returns an OnboardingError or AuthError.
         """
         verbose = self.verbose or verbose
         response = self.onboarding_client.get_users_status(
             verbose=verbose,
             page=page,
             page_size=page_size,
@@ -377,42 +379,51 @@
                 OnboardingError.from_response(
                     operation="add_user_feedback", response=response
                 )
             )
 
     @early_return
     def add_selfie(
-        self, user_id: str, media_data: bytes, verbose: Optional[bool] = False
+        self,
+        user_id: str,
+        media_data: bytes,
+        wait_for_completion: Optional[bool] = True,
+        verbose: Optional[bool] = False,
     ) -> Result[bool, Union[OnboardingError, AuthError]]:
         """
 
         This call is used to upload for the first time the video of the user's face to the onboarding service.
         This video will be used to extract the biometric face profile.
 
         Parameters
         ----------
         user_id
             User identifier
         media_data
             Binary media data.
+        wait_for_completion
+            This setting specifies whether or not the request should return immediately or wait for the operation to complete before returning.
         verbose
             Used for print service response as well as the time elapsed
 
 
         Returns
         -------
             A Result where if the operation is successful it returns True.
             Otherwise, it returns an OnboardingError or AuthError.
         """
         verbose = self.verbose or verbose
         response = self.onboarding_client.add_selfie(
-            user_id=user_id, media_data=media_data, verbose=verbose
+            user_id=user_id,
+            media_data=media_data,
+            wait_for_completion=wait_for_completion,
+            verbose=verbose,
         ).unwrap_or_return()
 
-        if response.status_code == 200:
+        if response.status_code in [200, 201]:
             return isSuccess
         else:
             return Failure(
                 OnboardingError.from_response(operation="add_selfie", response=response)
             )
 
     @early_return
@@ -1150,49 +1161,14 @@
             return Failure(
                 OnboardingError.from_response(
                     operation="screening_monitor_delete", response=response
                 )
             )
 
     @early_return
-    def screening_monitor_open_alerts(
-        self, start_index: int = 0, size: int = 100, verbose: bool = False
-    ) -> Result[bool, Union[OnboardingError, AuthError]]:
-        """
-        Retrieves from the monitoring list the users with open alerts
-
-        Parameters
-        ----------
-        start_index
-            DB index to start (0-2147483647)
-        size
-            Numbers of alerts to return (1-100).
-        verbose
-            Used for print service response as well as the time elapsed
-
-        Returns
-        -------
-            A Result where if the operation is successful it returns a dictionary.
-            Otherwise, it returns an OnboardingError or AuthError.
-        """
-        verbose = self.verbose or verbose
-        response = self.onboarding_client.screening_monitor_open_alerts(
-            start_index=start_index, size=size, verbose=verbose
-        ).unwrap_or_return()
-
-        if response.status_code == 200:
-            return Success(response.json())
-        else:
-            return Failure(
-                OnboardingError.from_response(
-                    operation="screening_monitor_open_alerts", response=response
-                )
-            )
-
-    @early_return
     def identify_user(
         self,
         target_user_id: str,
         probe_user_ids: List[str],
         version: Version = Version.DEFAULT,
         verbose: bool = False,
     ) -> Result[bool, Union[OnboardingError, AuthError]]:
@@ -1696,36 +1672,43 @@
             )
 
     def update_user_state(
         self,
         user_id: str,
         user_state: UserState,
         operator: str = "auto",
+        update_reasons: Optional[List[Dict[str, str]]] = None,
         verbose: bool = False,
     ) -> Result[bool, OnboardingError]:
         """
         Update the state of a user
         Parameters
         ----------
         user_state
             New State of the user
         user_id
             User identifier
         operator
             Who is accepting the user
+        update_reasons
+            List of reasons for status update
         verbose
             Used for print service response as well as the time elapsed
         Returns
         -------
             A Result where if the operation is successful it returns True.
             Otherwise, it returns an OnboardingError.
         """
         verbose = self.verbose or verbose
         response = self.onboarding_client.update_user_state(
-            user_id=user_id, user_state=user_state, operator=operator, verbose=verbose
+            user_id=user_id,
+            user_state=user_state,
+            operator=operator,
+            update_reasons=update_reasons,
+            verbose=verbose,
         ).unwrap_or_return()
 
         if response.status_code == 200:
             return isSuccess
         else:
             return Failure(
                 OnboardingError.from_response(
```

### Comparing `alice-onboarding-3.0.0/alice/onboarding/onboarding_client.py` & `alice-onboarding-3.1.0/alice/onboarding/onboarding_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,15 +278,15 @@
 
     @early_return
     @timeit
     def get_users_status(
         self,
         verbose: Optional[bool] = False,
         page: int = 1,
-        page_size: int = 0,
+        page_size: int = 10,
         descending: bool = True,
         authorized: bool = False,
         sort_by: Union[str, None] = None,
         filter_field: Union[str, None] = None,
         filter_value: Union[str, None] = None,
     ) -> Result[Response, Error]:
         """
@@ -406,27 +406,33 @@
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
     def add_selfie(
-        self, user_id: str, media_data: bytes, verbose: Optional[bool] = False
+        self,
+        user_id: str,
+        media_data: bytes,
+        wait_for_completion: Optional[bool] = True,
+        verbose: Optional[bool] = False,
     ) -> Result[Response, Error]:
         """
 
         This call is used to upload for the first time the video of the user's face to the onboarding service.
         This video will be used to extract the biometric face profile.
 
         Parameters
         ----------
         user_id
             User identifier
         media_data
             Binary media data.
+        wait_for_completion
+            This setting specifies whether or not the request should return immediately or wait for the operation to complete before returning.
         verbose
             Used for print service response as well as the time elapsed
 
 
         Returns
         -------
             A Result object with Response object [requests library] if Success
@@ -440,14 +446,15 @@
 
         files = {"video": ("video", media_data)}
 
         try:
             response = self.session.post(
                 f"{self.url}/user/selfie",
                 files=files,
+                data={"wait_for_completion": wait_for_completion},
                 headers=headers,
                 timeout=self.timeout,
             )
         except requests.exceptions.Timeout:
             return Failure(OnboardingError.timeout(operation="add_selfie"))
 
         print_response(response=response, verbose=verbose)
@@ -1311,56 +1318,14 @@
 
         print_response(response=response, verbose=verbose)
 
         return Success(response)
 
     @early_return
     @timeit
-    def screening_monitor_open_alerts(
-        self, start_index: int = 0, size: int = 100, verbose: bool = False
-    ) -> Result[Response, Error]:
-        """
-        Retrieves from the monitoring list the users with open alerts
-
-        Parameters
-        ----------
-        start_index
-            DB index to start (0-2147483647)
-        size
-            Numbers of alerts to return (1-100).
-        verbose
-            Used for print service response as well as the time elapsed
-
-
-        Returns
-        -------
-              A Result object with Response object [requests library] if Success
-        """
-        print_intro("screening_monitor_open_alerts", verbose=verbose)
-
-        backend_token = self.auth.create_backend_token().unwrap_or_return()
-        print_token("backend_token", backend_token, verbose=verbose)
-        headers = self._auth_headers(backend_token)
-
-        try:
-            response = self.session.get(
-                f"{self.url}/users/screening/monitor/alerts?start_index={start_index}&size={size}",
-                headers=headers,
-                timeout=self.timeout,
-            )
-        except requests.exceptions.Timeout:
-            return Failure(
-                OnboardingError.timeout(operation="screening_monitor_open_alerts")
-            )
-        print_response(response=response, verbose=verbose)
-
-        return Success(response)
-
-    @early_return
-    @timeit
     def identify_user(
         self,
         target_user_id: str,
         probe_user_ids: List[str],
         version: Version = Version.DEFAULT,
         verbose: bool = False,
     ) -> Result[Response, Error]:
@@ -1950,27 +1915,30 @@
 
     @timeit
     def update_user_state(
         self,
         user_id: str,
         user_state: UserState,
         operator: str = "auto",
+        update_reasons: Optional[List[Dict[str, str]]] = None,
         verbose: bool = False,
     ) -> Result[Response, Error]:
         """
         Update the state of a user
 
         Parameters
         ----------
         user_state
             New State of the user
         user_id
             User identifier
         operator
             Who is accepting the user
+        update_reasons
+            List of reasons for status update
         verbose
             Used for print service response as well as the time elapsed
 
 
         Returns
         -------
             A Response object [requests library]
@@ -1985,14 +1953,15 @@
         headers = self._auth_headers(backend_user_token)
         try:
             response = requests.patch(
                 f"{self.url}/user/state",
                 headers=headers,
                 json={
                     "state": user_state.value,
+                    "update_reasons": update_reasons,
                     "operator": operator,
                 },
                 timeout=self.timeout,
             )
         except requests.exceptions.Timeout:
             return Failure(OnboardingError.timeout(operation="update_user_state"))
```

### Comparing `alice-onboarding-3.0.0/alice/onboarding/onboarding_errors.py` & `alice-onboarding-3.1.0/alice/onboarding/onboarding_errors.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from requests import Response
 
 
 @dataclass
 class OnboardingError(Error):
     operation: str
     code: int
-    message: Optional[Dict[str, Any]] = None
+    message: Optional[Dict[str, Any]] = None  # type: ignore
 
     def __init__(
         self, operation: str, code: int, message: Optional[Dict[str, Any]] = None
     ):
         self.operation = operation
         self.code = code
         self.message = message
```

### Comparing `alice-onboarding-3.0.0/alice/onboarding/tools.py` & `alice-onboarding-3.1.0/alice/onboarding/tools.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-3.0.0/alice/public_api.py` & `alice-onboarding-3.1.0/alice/public_api.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-3.0.0/alice/sandbox/sandbox.py` & `alice-onboarding-3.1.0/alice/sandbox/sandbox.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-3.0.0/alice/sandbox/sandbox_client.py` & `alice-onboarding-3.1.0/alice/sandbox/sandbox_client.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-3.0.0/alice/sandbox/sandbox_errors.py` & `alice-onboarding-3.1.0/alice/sandbox/sandbox_errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from requests import Response
 
 
 @dataclass
 class SandboxError(Error):
     operation: str
     code: int
-    message: Optional[Dict[str, Any]] = None
+    message: Optional[Dict[str, Any]] = None  # type: ignore
 
     def __init__(
         self, operation: str, code: int, message: Optional[Dict[str, Any]] = None
     ):
         self.operation = operation
         self.code = code
         self.message = message
```

### Comparing `alice-onboarding-3.0.0/alice/webhooks/webhook.py` & `alice-onboarding-3.1.0/alice/webhooks/webhook.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-3.0.0/alice/webhooks/webhooks.py` & `alice-onboarding-3.1.0/alice/webhooks/webhooks.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-3.0.0/alice/webhooks/webhooks_client.py` & `alice-onboarding-3.1.0/alice/webhooks/webhooks_client.py`

 * *Files identical despite different names*

### Comparing `alice-onboarding-3.0.0/alice_onboarding.egg-info/PKG-INFO` & `alice-onboarding-3.1.0/alice_onboarding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alice-onboarding
-Version: 3.0.0
+Version: 3.1.0
 Summary: Alice Onboarding Python SDK
 Home-page: https://github.com/alice-biometrics/onboarding-python
 Author: Alice Biometrics
 Author-email: support@alicebiometrics.com
 License: Alice Copyright
 Keywords: onboarding,biometrics,kyc,alice
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alice-onboarding-3.0.0/alice_onboarding.egg-info/SOURCES.txt` & `alice-onboarding-3.1.0/alice_onboarding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alice-onboarding-3.0.0/setup.py` & `alice-onboarding-3.1.0/setup.py`

 * *Files identical despite different names*

