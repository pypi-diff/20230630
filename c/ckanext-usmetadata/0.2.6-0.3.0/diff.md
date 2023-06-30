# Comparing `tmp/ckanext-usmetadata-0.2.6.tar.gz` & `tmp/ckanext-usmetadata-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-usmetadata-0.2.6.tar", last modified: Tue Apr  4 14:25:24 2023, max compression
+gzip compressed data, was "ckanext-usmetadata-0.3.0.tar", last modified: Fri Jun 30 17:42:45 2023, max compression
```

## Comparing `ckanext-usmetadata-0.2.6.tar` & `ckanext-usmetadata-0.3.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:25:24.004851 ckanext-usmetadata-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-04 14:25:24.004851 ckanext-usmetadata-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:25:24.000851 ckanext-usmetadata-0.2.6/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:25:24.000851 ckanext-usmetadata-0.2.6/ckanext/usmetadata/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27535 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/db_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:25:24.000851 ckanext-usmetadata-0.2.6/ckanext/usmetadata/fanstatic/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/fanstatic/add_subagency.js
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/fanstatic/dataset_edit_form.js
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/fanstatic/dataset_url.js
--rw-r--r--   0 runner    (1001) docker     (123)    13046 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/fanstatic/redactions.js
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/fanstatic/resource_form.css
--rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/fanstatic/resource_form.js
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/fanstatic/webassets.yml
--rw-r--r--   0 runner    (1001) docker     (123)    17625 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    75906 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/media_types.json
--rw-r--r--   0 runner    (1001) docker     (123)    18644 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:25:24.000851 ckanext-usmetadata-0.2.6/ckanext/usmetadata/public/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:25:23.996851 ckanext-usmetadata-0.2.6/ckanext/usmetadata/public/base/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:25:24.000851 ckanext-usmetadata-0.2.6/ckanext/usmetadata/public/base/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/public/base/images/inventory-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/public/redacted_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    71431 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/public/redaction_clear.png
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/resource_formats.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:25:24.000851 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/footer.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:25:24.000851 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/organization/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/organization/activity_stream.html
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/organization/bulk_process.html
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/organization/member_new.html
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/organization/read_base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:25:24.000851 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/read.html
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/read_base.html
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/resource_read.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:25:24.004851 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/expanded_common_core_fields.html
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/info.html
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/metadata_info.html
--rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/package_basic_fields.html
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/package_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/package_metadata_fields.html
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/required_common_core_fields.html
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/required_if_applicable_common_core_fields.html
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/resource_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/resource_item.html
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/resources.html
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/stages.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:25:24.004851 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/snippets/activity_item.html
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/snippets/license.html
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/snippets/organization.html
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/snippets/package_item.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:25:24.004851 ckanext-usmetadata-0.2.6/ckanext_usmetadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext_usmetadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext_usmetadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext_usmetadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext_usmetadata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext_usmetadata.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext_usmetadata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/ckanext_usmetadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-04 14:25:24.004851 ckanext-usmetadata-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-04 14:25:23.000000 ckanext-usmetadata-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:45.731770 ckanext-usmetadata-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-30 17:42:45.731770 ckanext-usmetadata-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:45.723770 ckanext-usmetadata-0.3.0/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:45.723770 ckanext-usmetadata-0.3.0/ckanext/usmetadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27535 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/db_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:45.727770 ckanext-usmetadata-0.3.0/ckanext/usmetadata/fanstatic/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/fanstatic/add_subagency.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/fanstatic/dataset_edit_form.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/fanstatic/dataset_url.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13046 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/fanstatic/redactions.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/fanstatic/resource_form.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/fanstatic/resource_form.js
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/fanstatic/webassets.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    17613 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75906 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/media_types.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18184 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:45.727770 ckanext-usmetadata-0.3.0/ckanext/usmetadata/public/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:45.723770 ckanext-usmetadata-0.3.0/ckanext/usmetadata/public/base/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:45.727770 ckanext-usmetadata-0.3.0/ckanext/usmetadata/public/base/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/public/base/images/inventory-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/public/redacted_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    71431 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/public/redaction_clear.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/resource_formats.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:45.727770 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/footer.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:45.727770 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/organization/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/organization/activity_stream.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/organization/bulk_process.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/organization/member_new.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/organization/read_base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:45.727770 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/read.html
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/read_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/resource_read.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:45.727770 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/expanded_common_core_fields.html
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/info.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/metadata_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/package_basic_fields.html
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/package_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/package_metadata_fields.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/required_common_core_fields.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/required_if_applicable_common_core_fields.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/resource_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/resource_item.html
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/resources.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/stages.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:45.727770 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/snippets/activity_item.html
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/snippets/license.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/snippets/organization.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/snippets/package_item.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:45.731770 ckanext-usmetadata-0.3.0/ckanext_usmetadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext_usmetadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext_usmetadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext_usmetadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext_usmetadata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext_usmetadata.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext_usmetadata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/ckanext_usmetadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-30 17:42:45.731770 ckanext-usmetadata-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-30 17:42:45.000000 ckanext-usmetadata-0.3.0/setup.py
```

### Comparing `ckanext-usmetadata-0.2.6/PKG-INFO` & `ckanext-usmetadata-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,36 @@
-Metadata-Version: 2.1
-Name: ckanext-usmetadata
-Version: 0.2.6
-Summary: US Metadata Plugin for CKAN
-Home-page: https://github.com/GSA/ckanext-usmetadata
-Author: Data.gov
-Author-email: datagovhelp@gsa.gov
-License: Public Domain
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-
 # ckanext-usmetadata
 
 ![Github Actions](https://github.com/GSA/ckanext-usmetadata/actions/workflows/test.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/ckanext-usmetadata.svg)](https://badge.fury.io/py/ckanext-usmetadata)
 
 This CKAN Extension expands CKAN to offer a number of custom fields related to the [DCAT-US Schema](https://resources.data.gov/schemas/dcat-us/v1.1/)
 
 ### Installation
 
-To install this package, activate CKAN virtualenv (e.g. "source /path/to/virtenv/bin/activate"), then run
-
-
-    (virtenv) 'pip install -e git+https://github.com/gsa/usmetadata#egg=ckanext-usmetadata'
-    (virtenv) 'python setup.py develop'
+Add `ckanext-usmetadata` to your requirements.txt, and then pip install
     
 Then in your CKAN .ini file, add `usmetadata`
 to your ckan.plugins line:
 
 	ckan.plugins = (other plugins here...) usmetadata
 
 ### Requirements
 
 This extension is compatible with these versions of CKAN.
 
 CKAN version | Compatibility
 ------------ | -------------
-<=2.8        | no
-2.9          | yes
+<=2.9        | no
+2.10         | yes
 
 ### Development
 
 You may also install by cloning the git repo, then running ''python setup.py develop'' from the root of your source
-directory, which will install an egg link so that you can modify the code and see results without yest [localhost:5000](http://localhost:5000/).
+directory, which will install an egg link so that you can modify the code and see results [localhost:5000](http://localhost:5000/).
 
 Clean up any containers and volumes.
 
     $ make down
 
 Open a shell to run commands in the container.
 
@@ -69,21 +53,18 @@
 
     $ make test
 
 Lint the code.
 
     $ make lint
 
-
 ### Matrix builds
 
 In order to support multiple versions of CKAN, or even upgrade to new versions
 of CKAN, we support development and testing through the `CKAN_VERSION`
 environment variable.
 
     $ make CKAN_VERSION=2.9 test
     
 ## Credit / Copying
 
 Credit to the original owner of the repo.  Everything here is built on top of the original foundation.
-
-
```

### Comparing `ckanext-usmetadata-0.2.6/README.md` & `ckanext-usmetadata-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,48 @@
+Metadata-Version: 2.1
+Name: ckanext-usmetadata
+Version: 0.3.0
+Summary: US Metadata Plugin for CKAN
+Home-page: https://github.com/GSA/ckanext-usmetadata
+Author: Data.gov
+Author-email: datagovhelp@gsa.gov
+License: Public Domain
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+
 # ckanext-usmetadata
 
 ![Github Actions](https://github.com/GSA/ckanext-usmetadata/actions/workflows/test.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/ckanext-usmetadata.svg)](https://badge.fury.io/py/ckanext-usmetadata)
 
 This CKAN Extension expands CKAN to offer a number of custom fields related to the [DCAT-US Schema](https://resources.data.gov/schemas/dcat-us/v1.1/)
 
 ### Installation
 
-To install this package, activate CKAN virtualenv (e.g. "source /path/to/virtenv/bin/activate"), then run
-
-
-    (virtenv) 'pip install -e git+https://github.com/gsa/usmetadata#egg=ckanext-usmetadata'
-    (virtenv) 'python setup.py develop'
+Add `ckanext-usmetadata` to your requirements.txt, and then pip install
     
 Then in your CKAN .ini file, add `usmetadata`
 to your ckan.plugins line:
 
 	ckan.plugins = (other plugins here...) usmetadata
 
 ### Requirements
 
 This extension is compatible with these versions of CKAN.
 
 CKAN version | Compatibility
 ------------ | -------------
-<=2.8        | no
-2.9          | yes
+<=2.9        | no
+2.10         | yes
 
 ### Development
 
 You may also install by cloning the git repo, then running ''python setup.py develop'' from the root of your source
-directory, which will install an egg link so that you can modify the code and see results without yest [localhost:5000](http://localhost:5000/).
+directory, which will install an egg link so that you can modify the code and see results [localhost:5000](http://localhost:5000/).
 
 Clean up any containers and volumes.
 
     $ make down
 
 Open a shell to run commands in the container.
 
@@ -57,19 +65,20 @@
 
     $ make test
 
 Lint the code.
 
     $ make lint
 
-
 ### Matrix builds
 
 In order to support multiple versions of CKAN, or even upgrade to new versions
 of CKAN, we support development and testing through the `CKAN_VERSION`
 environment variable.
 
     $ make CKAN_VERSION=2.9 test
     
 ## Credit / Copying
 
 Credit to the original owner of the repo.  Everything here is built on top of the original foundation.
+
+
```

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/blueprint.py` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/blueprint.py`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/db_utils.py` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/db_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 cached_tables = {}
 
 
 def get_organization_title(dataset_id):
     query = "select id, title from package where package.id = '" + dataset_id + "'"
     connection = model.Session.connection()
     res = connection.execute(query).fetchone()
-    return res._row[1]
+    return res[1]
 
 
 def get_parent_organizations(c):
     items = {}
 
     if not c.userobj:
         return items
@@ -40,10 +40,10 @@
                 "where package_extra.key = 'is_parent' and package_extra.value = 'true' " \
                 "and package.id = package_extra.package_id and package.state = 'active' " \
                 "and package.owner_org in " + str(tuple(ids))
 
     connection = model.Session.connection()
     res = connection.execute(query).fetchall()
     for result in res:
-        items[result._row[0]] = result._row[1]
+        items[result[0]] = result[1]
 
     return items
```

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/fanstatic/dataset_edit_form.js` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/fanstatic/dataset_edit_form.js`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/fanstatic/dataset_url.js` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/fanstatic/dataset_url.js`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/fanstatic/redactions.js` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/fanstatic/redactions.js`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/fanstatic/resource_form.css` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/fanstatic/resource_form.css`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/fanstatic/resource_form.js` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/fanstatic/resource_form.js`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/helper.py` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import copy
 from logging import getLogger
 import re
 
 import ckan.lib.helpers as h
 import ckan.plugins as p
+import ckan.lib.navl.validators as ckan_validators
 
 log = getLogger(__name__)
 
 REDACTION_STROKE_REGEX = re.compile(
     r'(\[\[REDACTED-EX B[\d]\]\])'
 )
 
@@ -128,49 +129,53 @@
         except TypeError:
             # The given value is already invalid from another validator
             return value
 
     return string_validator
 
 
+def string(value):
+    return str(value)
+
+
 # excluded title, description, tags and last update as they're part of the default ckan dataset metadata
 required_metadata = (
-    {'id': 'title', 'validators': [p.toolkit.get_validator('not_empty'), str]},
-    {'id': 'notes', 'validators': [p.toolkit.get_validator('not_empty'), str]},
-    {'id': 'publisher', 'validators': [p.toolkit.get_validator('not_empty'), str, string_length_validator(max=300)]},
-    {'id': 'contact_name', 'validators': [p.toolkit.get_validator('not_empty'), str, string_length_validator(max=300)]},
-    {'id': 'contact_email', 'validators': [p.toolkit.get_validator('not_empty'), str, string_length_validator(max=200)]},
+    {'id': 'title', 'validators': [ckan_validators.not_empty, string]},
+    {'id': 'notes', 'validators': [ckan_validators.not_empty, string]},
+    {'id': 'publisher', 'validators': [ckan_validators.not_empty, string, string_length_validator(max=300)]},
+    {'id': 'contact_name', 'validators': [ckan_validators.not_empty, string, string_length_validator(max=300)]},
+    {'id': 'contact_email', 'validators': [ckan_validators.not_empty, string, string_length_validator(max=200)]},
     # TODO should this unique_id be validated against any other unique IDs for this agency?
-    {'id': 'unique_id', 'validators': [p.toolkit.get_validator('not_empty'), str, string_length_validator(max=100)]},
-    {'id': 'modified', 'validators': [p.toolkit.get_validator('not_empty'), str, string_length_validator(max=100)]},
-    {'id': 'public_access_level', 'validators': [str, public_access_level_validator]},
-    {'id': 'bureau_code', 'validators': [str, bureau_code_validator, string_length_validator(max=2100)]},
-    {'id': 'program_code', 'validators': [str, program_code_validator, string_length_validator(max=2100)]}
+    {'id': 'unique_id', 'validators': [ckan_validators.not_empty, string, string_length_validator(max=100)]},
+    {'id': 'modified', 'validators': [ckan_validators.not_empty, string, string_length_validator(max=100)]},
+    {'id': 'public_access_level', 'validators': [string, public_access_level_validator]},
+    {'id': 'bureau_code', 'validators': [string, bureau_code_validator, string_length_validator(max=2100)]},
+    {'id': 'program_code', 'validators': [string, program_code_validator, string_length_validator(max=2100)]}
 )
 
 
 # used to bypass validation on create
 required_metadata_update = (
-    {'id': 'public_access_level', 'validators': [str, public_access_level_validator]},
+    {'id': 'public_access_level', 'validators': [string, public_access_level_validator]},
     {'id': 'publisher', 'validators': [string_length_validator(max=300)]},
     {'id': 'contact_name', 'validators': [string_length_validator(max=300)]},
     {'id': 'contact_email', 'validators': [string_length_validator(max=200)]},
     # TODO should this unique_id be validated against any other unique IDs for this agency?
     {'id': 'unique_id', 'validators': [string_length_validator(max=100)]},
     {'id': 'modified', 'validators': [string_length_validator(max=100)]},
-    {'id': 'bureau_code', 'validators': [str, bureau_code_validator]},
-    {'id': 'program_code', 'validators': [str, program_code_validator]}
+    {'id': 'bureau_code', 'validators': [string, bureau_code_validator]},
+    {'id': 'program_code', 'validators': [string, program_code_validator]}
 )
 
 # some of these could be excluded (e.g. related_documents) which can be captured from other ckan default data
 expanded_metadata = (
     # issued
-    {'id': 'release_date', 'validators': [str, release_date_validator]},
-    {'id': 'accrual_periodicity', 'validators': [str, accrual_periodicity_validator]},
-    {'id': 'language', 'validators': [str, language_validator]},
+    {'id': 'release_date', 'validators': [string, release_date_validator]},
+    {'id': 'accrual_periodicity', 'validators': [string, accrual_periodicity_validator]},
+    {'id': 'language', 'validators': [string, language_validator]},
     {'id': 'data_quality', 'validators': [string_length_validator(max=1000)]},
     {'id': 'publishing_status', 'validators': [string_length_validator(max=1000)]},
     {'id': 'is_parent', 'validators': [string_length_validator(max=1000)]},
     {'id': 'parent_dataset', 'validators': [string_length_validator(max=1000)]},
     # theme
     {'id': 'category', 'validators': [string_length_validator(max=1000)]},
     # describedBy
@@ -296,49 +301,49 @@
 media_types = list(set([row[1] for row in list(h.resource_formats().values())]))
 
 
 # all required_metadata should be required
 def get_req_metadata_for_create():
     log.debug('get_req_metadata_for_create')
     new_req_meta = copy.copy(required_metadata)
-    validator = p.toolkit.get_validator('not_empty')
+    validator = ckan_validators.not_empty
     for meta in new_req_meta:
         meta['validators'].append(validator)
     return new_req_meta
 
 
 # used to bypass validation on create
 def get_req_metadata_for_update():
     log.debug('get_req_metadata_for_update')
     new_req_meta = copy.copy(required_metadata_update)
-    validator = p.toolkit.get_validator('ignore_missing')
+    validator = ckan_validators.ignore_missing
     for meta in new_req_meta:
         meta['validators'].insert(0, validator)
     return new_req_meta
 
 
 def get_req_metadata_for_show_update():
     new_req_meta = copy.copy(required_metadata)
-    validator = p.toolkit.get_validator('ignore_missing')
+    validator = ckan_validators.ignore_missing
     for meta in new_req_meta:
         meta['validators'].insert(0, validator)
     return new_req_meta
 
 
 for meta in required_if_applicable_metadata:
-    meta['validators'].insert(0, p.toolkit.get_validator('ignore_missing'))
+    meta['validators'].insert(0, ckan_validators.ignore_missing)
 
 for meta in expanded_metadata:
-    meta['validators'].insert(0, p.toolkit.get_validator('ignore_missing'))
+    meta['validators'].insert(0, ckan_validators.ignore_missing)
 
 for meta in required_if_applicable_metadata_by_pass_validation:
-    meta['validators'].insert(0, p.toolkit.get_validator('ignore_missing'))
+    meta['validators'].insert(0, ckan_validators.ignore_missing)
 
 for meta in expanded_metadata_by_pass_validation:
-    meta['validators'].insert(0, p.toolkit.get_validator('ignore_missing'))
+    meta['validators'].insert(0, ckan_validators.ignore_missing)
 
 schema_updates_for_create = [{meta['id']: meta['validators'] + [p.toolkit.get_converter('convert_to_extras')]} for meta
                              in (get_req_metadata_for_create() + required_if_applicable_metadata + expanded_metadata)]
 schema_updates_for_update = [{meta['id']: meta['validators'] + [p.toolkit.get_converter('convert_to_extras')]} for meta
                              in (get_req_metadata_for_update() + required_if_applicable_metadata + expanded_metadata)]
 schema_updates_for_show = [{meta['id']: meta['validators'] + [p.toolkit.get_converter('convert_from_extras')]} for meta
                            in
```

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/media_types.json` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/media_types.json`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/plugin.py` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import collections
 import re
 from logging import getLogger
 
 from ckan.common import json
-import ckan.lib.helpers as h
 import ckan.lib.base as base
+import ckan.lib.navl.validators as ckan_validators
 import ckan.logic as logic
 import ckan.plugins as p
 from ckan.plugins.toolkit import requires_ckan_version, c
 from . import db_utils
 from . import blueprint
 from . import helper as local_helper
 
@@ -23,15 +23,14 @@
     This plugin adds fields for the metadata (known as the DCAT-US) defined at
     https://resources.data.gov/schemas/dcat-us/v1.1/
     """
     p.implements(p.ITemplateHelpers, inherit=False)
     p.implements(p.IConfigurer, inherit=False)
     p.implements(p.IDatasetForm, inherit=False)
     p.implements(p.IResourceController, inherit=True)
-    p.implements(p.interfaces.IRoutes, inherit=True)
     p.implements(p.interfaces.IPackageController, inherit=True)
     p.implements(p.interfaces.IOrganizationController, inherit=True)
     p.implements(p.IFacets, inherit=True)
     p.implements(p.IBlueprint)
 
     # IConfigurer
     def update_config(self, config):
@@ -75,20 +74,14 @@
         for redact in re.findall(local_helper.REDACTION_STROKE_REGEX, data):
             data = data.replace(redact, mask)
         data = data.replace('[[/REDACTED]]', mask)
         # render our custom snippet
         return data
 
     @classmethod
-    def usmetadata_shorten(cls, plain=None, extract_length=180):
-        if not extract_length or len(plain) < extract_length:
-            return plain
-        return str(h.truncate(plain, length=extract_length, indicator='...', whole_word=True))
-
-    @classmethod
     def resource_redacted_icon(cls, package, resource, field):
         redacted_key = 'redacted_' + field
         if 'extras' in package:
             extras = dict([(x['key'], x['value']) for x in package['extras']])
             if 'public_access_level' not in extras:
                 return ''
             if extras['public_access_level'] not in ['non-public', 'restricted public']:
@@ -320,21 +313,21 @@
         # registers itself as the default (above).
         #
         # return ['dataset', 'package']
         return []
 
     def _default_extras_schema(self):
         schema = {
-            'id': [p.toolkit.get_validator('ignore')],
-            'key': [p.toolkit.get_validator('not_empty'), str],
-            'value': [p.toolkit.get_validator('not_missing')],
-            'state': [p.toolkit.get_validator('ignore')],
-            'deleted': [p.toolkit.get_validator('ignore_missing')],
-            'revision_timestamp': [p.toolkit.get_validator('ignore')],
-            '__extras': [p.toolkit.get_validator('ignore')],
+            'id': [ckan_validators.ignore],
+            'key': [ckan_validators.not_empty, local_helper.string],
+            'value': [ckan_validators.not_missing],
+            'state': [ckan_validators.ignore],
+            'deleted': [ckan_validators.ignore_missing],
+            'revision_timestamp': [ckan_validators.ignore],
+            '__extras': [ckan_validators.ignore],
         }
         return schema
 
     # See ckan.plugins.interfaces.IDatasetForm
     def _create_package_schema(self, schema):
         log.debug("_create_package_schema called")
         try:
@@ -349,32 +342,32 @@
         except RuntimeError:
             # This is called when 'factories.dataset' creates the dataset
             for update in local_helper.schema_updates_for_create:
                 schema.update(update)
 
         # use convert_to_tags functions for taxonomy
         schema.update({
-            'tag_string': [p.toolkit.get_validator('not_empty'),
+            'tag_string': [ckan_validators.not_empty,
                            p.toolkit.get_converter('convert_to_tags')],
             'extras': self._default_extras_schema()
             # 'resources': {
-            # 'name': [p.toolkit.get_validator('not_empty')],
-            # 'format': [p.toolkit.get_validator('not_empty')],
+            # 'name': [ckan_validators.not_empty],
+            # 'format': [ckan_validators.not_empty],
             # }
         })
         return schema
 
     def _modify_package_schema_update(self, schema):
         log.debug("_modify_package_schema_update called")
         for update in local_helper.schema_updates_for_update:
             schema.update(update)
 
         # use convert_to_tags functions for taxonomy
         schema.update({
-            'tag_string': [p.toolkit.get_validator('ignore_empty'),
+            'tag_string': [ckan_validators.ignore_empty,
                            p.toolkit.get_converter('convert_to_tags')],
             'extras': self._default_extras_schema()
         })
         return schema
 
     def _modify_package_schema_show(self, schema):
         log.debug("_modify_package_schema_update_show called")
@@ -440,15 +433,14 @@
             'license_options': local_helper.license_options,
             'is_parent_options': local_helper.is_parent_options,
             'load_data_into_dict': self.load_data_into_dict,
             'accrual_periodicity': local_helper.accrual_periodicity,
             'publishing_status_options': local_helper.publishing_status_options,
             'always_private': True,
             'usmetadata_filter': self.usmetadata_filter,
-            'usmetadata_shorten': self.usmetadata_shorten,
             'redacted_icon': self.redacted_icon,
             'resource_redacted_icon': self.resource_redacted_icon,
             'get_action': logic.get_action
         }
 
     def get_blueprint(self):
         return blueprint.datapusher
```

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/public/base/images/inventory-logo.png` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/public/base/images/inventory-logo.png`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/public/redacted_icon.png` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/public/redacted_icon.png`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/public/redaction_clear.png` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/public/redaction_clear.png`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/resource_formats.json` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/resource_formats.json`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/footer.html` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/footer.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+{% ckan_extends %}
 <footer class="site-footer">
   <div class="container">
     {% block footer_content %}
       <nav class="footer-links">
         {% block footer_nav %}
           <ul class="unstyled">
             {% block footer_links %}
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
+{% ckan_extends %}
 {% block footer_content %}  {% block footer_nav %}
     * {% block footer_links %}
     * {{__('About_{0}').format(g.site_title)_}}
     * {% endblock %}
     * {% block footer_links_ckan %} {% set api_url = 'http://docs.ckan.org/en/
       {0}/api.html'.format(g.ckan_doc_version) %}
     * {{__('CKAN_API')_}}
```

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/organization/bulk_process.html` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/organization/bulk_process.html`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
             {{ _('Datasets') }}
           {%- endif -%}
         {% endblock %}
       </h3>
       {% block form %}
         {% if c.page.item_count %}
           <form method="POST" data-module="basic-form">
+            {{ h.csrf_input() }}
             <table class="table table-bordered table-header table-hover table-bulk-edit table-edit-hover" data-module="table-selectable-rows">
               <col width="8">
               <col width="120">
               <thead>
                 <tr>
                   <th></th>
                   <th class="table-actions">
@@ -44,29 +45,28 @@
                       </button>
                     </div>
                   </th>
                 </tr>
               </thead>
               <tbody>
                 {% for package in c.packages %}
-                  {% set truncate = truncate or 180 %}
-                  {% set truncate_title = truncate_title or 80 %}
                   {% set title = package.title or package.name %}
-                  {% set notes = h.markdown_extract(package.notes, extract_length=truncate) %}
+                  {% set notes = h.markdown_extract(package.notes, extract_length=180) %}
                   <tr>
                     <td>
                       <input type="checkbox" name="dataset_{{ package.id }}">
                     </td>
                     <td class="context">
                       <a href="{% url_for controller='dataset', action='edit', id=package.name %}" class="edit pull-right">
                         {{ _('Edit') }}
                       </a>
                       <h3 class="dataset-heading">
                         {{ h.redacted_icon(package,'title')|safe }}
-                        {{ h.link_to(h.truncate(h.usmetadata_filter(title), truncate_title), h.url_for(controller='dataset', action='read', id=package.name), class="redacted-md") }}
+                        {{ set link_truncate = h.usmetadata_filter(title) | truncate(80) }}
+                        {{ h.link_to(link_truncate, h.url_for(controller='dataset', action='read', id=package.name), class="redacted-md") }}
                         {% if package.get('state', '').startswith('draft') %}
                           <span class="label label-info">{{ _('Draft') }}</span>
                         {% elif package.get('state', '').startswith('deleted') %}
                           <span class="label label-important">{{ _('Deleted') }}</span>
                         {% endif %}
                         {% if package.private %}
                           <span class="label label-important">{{ _('Private') }}</span>
```

#### html2text {}

```diff
@@ -2,25 +2,27 @@
 ****** {{ _('Edit datasets') }} ******
 **** {% block page_heading %} {%- if c.page.item_count -%} {{ c.page.item_count
 }} datasets{{ _(" found for \"{query}\"").format(query=c.q) if c.q }} {%- elif
 request.params -%} {{ _('Sorry no datasets found for "{query}"').format
 (query=c.q) }} {%- else -%} {{ _('Datasets') }} {%- endif -%} {% endblock %}
 ****
 {% block form %} {% if c.page.item_count %}
+{{ h.csrf_input() }}
   {% if c.userobj.sysadmin %}
     {{ _('Make public') }}    {{ _('Make private') }}
   {% endif %}
     {{ _('Delete') }}
   {{__('Edit')_}}
-  **** {{ h.redacted_icon(package,'title')|safe }} {{ h.link_to(h.truncate
-  (h.usmetadata_filter(title), truncate_title), h.url_for(controller='dataset',
-  action='read', id=package.name), class="redacted-md") }} {% if package.get
-  ('state', '').startswith('draft') %} {{ _('Draft') }} {% elif package.get
-�('state', '').startswith('deleted') %} {{ _('Deleted') }} {% endif %} {% if
-  package.private %} {{ _('Private') }} {% endif %} ****
+  **** {{ h.redacted_icon(package,'title')|safe }} {{ set link_truncate =
+  h.usmetadata_filter(title) | truncate(80) }} {{ h.link_to(link_truncate,
+  h.url_for(controller='dataset', action='read', id=package.name),
+  class="redacted-md") }} {% if package.get('state', '').startswith('draft') %}
+�{{ _('Draft') }} {% elif package.get('state', '').startswith('deleted') %} {
+  { _('Deleted') }} {% endif %} {% if package.private %} {{ _('Private') }} {%
+  endif %} ****
   {% if notes %}
   {{ h.redacted_icon(package,'notes')|safe }}  {{ h.usmetadata_filter
   (notes)|urlize }}
   {% endif %}
 {% else %}
 {{ _('This organization has no datasets associated to it') }}
 {% endif %} {% endblock %}
```

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/organization/member_new.html` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/organization/member_new.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 {% ckan_extends %}
 
 {% block form %}
   <form class="dataset-form form-horizontal add-member-form" method='post'>
+    {{ h.csrf_input() }}
     <div class="row-fluid">
       <div class="control-group control-medium">
         {% if not user %}
           <label class="control-label" for="username">
             {{ _('Existing User') }}
           </label>
           <span>
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
 {% ckan_extends %} {% block form %}
+{{ h.csrf_input() }}
 {% if not user %}  {{ _('Existing User') }}   {{ _('If you wish to add an
 existing user, search for their username below.') }}  {% endif %}
 {% if user %}  [{{ user.name }}     ] {% else %} [username            ] {%
 endif %}
 {% if c.userobj.sysadmin %} {% if not user %}
 {{ _('or') }}
  {{ _('New User') }}   {{ _('If you wish to invite a new user, enter their
```

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/organization/read_base.html` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/organization/read_base.html`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 {% block content_action %}
   {% if h.check_access('organization_update', {'id': c.group_dict.id}) %}
     {% link_for _('Admin'), controller='organization', action='edit', id=c.group_dict.name, class_='btn', icon='wrench' %}
   {% endif %}
 {% endblock %}
 
 {% block content_primary_nav %}
-  {{ h.build_nav_icon('organization_read', _('Datasets'), id=c.group_dict.name) }}
-  {{ h.build_nav_icon('organization_about', _('About'), id=c.group_dict.name) }}
+  {{ h.build_nav_icon('organization.read', _('Datasets'), id=c.group_dict.name) }}
+  {{ h.build_nav_icon('organization.about', _('About'), id=c.group_dict.name) }}
 {% endblock %}
 
 {% block secondary_content %}
   {% snippet 'snippets/organization.html', organization=c.group_dict, show_nums=true %}
 
   {% block organization_facets %}{% endblock %}
 {% endblock %}
```

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/base.html` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/base.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/read.html` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/read.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/resource_read.html` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/resource_read.html`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,14 @@
                 <p>{% trans dataset=c.package.title, url=h.url_for(controller='dataset', action='read', id=c.package['name']) %}Source: <a href="{{ url }}">{{ dataset }}</a>{% endtrans %}
               {% endif %}
             {% endif %}
           {% endblock %}
         </div>
       </div>
       {% block data_preview %}
-        {{ super() }}
       {% endblock %}
     </section>
   {% endblock %}
 {% endblock %}
 
 {% block primary_content %}
   {% block resource_additional_information %}
@@ -109,18 +108,18 @@
               <tr>
                 <th scope="row">{{ _('License') }}</th>
                 <td>{% snippet "snippets/license.html", pkg_dict=pkg, text_only=True %}</td>
               </tr>
 
               {% for key, value in h.format_resource_items(res.items()) %}
                 {% if key != 'labels' and 'redacted ' not in key %}
-                  {% if res['labels'][key] %}
+                  {% if res[key] %}
                     <tr class="toggle-more">
                         <th scope="row">
-                            {{ res['labels'][key] }}
+                            {{ res[key] }}
                         </th>
                         <td>
                             {{ h.resource_redacted_icon(c.package,res,key)|safe }}
                             <span class="redacted-md">{{ h.usmetadata_filter(value|string) }}</span>
                         </td>
                     </tr>
                   {% else %}
@@ -130,15 +129,14 @@
                             {{ h.resource_redacted_icon(c.package,res,key)|safe }}
                             <span class="redacted-md">{{ h.usmetadata_filter(value|string) }}</span>
                         </td>
                     </tr>
                   {% endif %}
                 {% endif %}
               {% endfor %}
-
             </tbody>
           </table>
         </div>
       </section>
     {% endif %}
   {% endblock %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -32,27 +32,26 @@
 %}
 **** {{ _('From the dataset abstract') }} ****
      {{ h.markdown_extract(c.package.get('notes')) }}
 {% if c.userobj %}
 {% trans dataset=c.package.title, url=h.url_for(controller='dataset',
 action='read', id=c.package['name']) %}Source: {{_dataset_}}{% endtrans %} {%
 endif %} {% endif %} {% endblock %}
-{% block data_preview %} {{ super() }} {% endblock %}  {% endblock %} {%
-endblock %} {% block primary_content %} {% block
-resource_additional_information %} {% if res %}
+{% block data_preview %} {% endblock %}  {% endblock %} {% endblock %} {% block
+primary_content %} {% block resource_additional_information %} {% if res %}
 ***** {{ _('Additional Information') }} *****
-{{ _('Field') }}         {{ _('Value') }}
-                         {{ h.render_datetime(res.last_modified) or
-{{ _('Last updated') }}  h.render_datetime(res.revision_timestamp) or
-                         h.render_datetime(res.created) or _('unknown') }}
-{{ _('Created') }}       {{ h.render_datetime(res.created) or _('unknown') }}
-                         {{ h.resource_redacted_icon
-{{ _('Format') }}        (c.package,res,'format')|safe }} {
-                         { h.usmetadata_filter(res.mimetype_inner or
-                         res.mimetype or res.format or _('unknown')) }}
-{{ _('License') }}       {% snippet "snippets/license.html", pkg_dict=pkg,
-                         text_only=True %}
-{{ res['labels'][key] }} {{ h.resource_redacted_icon(c.package,res,key)|safe }}
-                         {{ h.usmetadata_filter(value|string) }}
-{{ key }}                {{ h.resource_redacted_icon(c.package,res,key)|safe }}
-                         {{ h.usmetadata_filter(value|string) }}
+{{ _('Field') }}        {{ _('Value') }}
+                        {{ h.render_datetime(res.last_modified) or
+{{ _('Last updated') }} h.render_datetime(res.revision_timestamp) or
+                        h.render_datetime(res.created) or _('unknown') }}
+{{ _('Created') }}      {{ h.render_datetime(res.created) or _('unknown') }}
+                        {{ h.resource_redacted_icon
+{{ _('Format') }}       (c.package,res,'format')|safe }} {{ h.usmetadata_filter
+                        (res.mimetype_inner or res.mimetype or res.format or _
+                        ('unknown')) }}
+{{ _('License') }}      {% snippet "snippets/license.html", pkg_dict=pkg,
+                        text_only=True %}
+{{ res[key] }}          {{ h.resource_redacted_icon(c.package,res,key)|safe }}
+                        {{ h.usmetadata_filter(value|string) }}
+{{ key }}               {{ h.resource_redacted_icon(c.package,res,key)|safe }}
+                        {{ h.usmetadata_filter(value|string) }}
  {% endif %} {% endblock %} {% endblock %}
```

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/expanded_common_core_fields.html` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/expanded_common_core_fields.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/info.html` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/info.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/metadata_info.html` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/metadata_info.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/package_basic_fields.html` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/package_basic_fields.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/package_metadata_fields.html` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/package_metadata_fields.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/required_common_core_fields.html` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/required_common_core_fields.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/required_if_applicable_common_core_fields.html` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/required_if_applicable_common_core_fields.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/resource_form.html` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/resource_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/resource_item.html` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/resource_item.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/resources.html` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/resources.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/package/snippets/stages.html` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/package/snippets/stages.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/snippets/organization.html` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/snippets/organization.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/ckanext/usmetadata/templates/snippets/package_item.html` & `ckanext-usmetadata-0.3.0/ckanext/usmetadata/templates/snippets/package_item.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 {#{% ckan_extends %}#}
-{% set truncate = truncate or 180 %}
-{% set truncate_title = truncate_title or 80 %}
 {% set title = h.usmetadata_filter(package.title or package.name) %}
-{% set notes = h.usmetadata_shorten(h.usmetadata_filter(package.notes), extract_length=truncate) %}
+{% set notes = h.usmetadata_filter(package.notes) | truncate(180) %}
 
 <li class="{{ item_class or "dataset-item" }}">
     {% block package_item_content -%}
     <div class="dataset-content">
         {% for extra in package.extras -%}
         {%- if extra['key'] == 'public_access_level' and extra['value'] == 'public' -%}
             <span class="dataset-private label label-inverse pull-right">
@@ -25,15 +23,15 @@
                 <i class="icon-lock"></i>
                 {{ _('restricted public') }}
             </span>
         {% endif %}
         {%- endfor %}
         <h3 class="dataset-heading">
             {{ h.redacted_icon(package, 'title')|safe }}
-            {{ h.link_to(h.truncate(h.usmetadata_filter(title), truncate_title),
+            {{ h.link_to(h.usmetadata_filter(title)|truncate(80),
                     h.url_for(controller='dataset', action='read', id=package.name),
                     class='redacted-md') }}
             {% if package.get('state', '').startswith('draft') %}
                 <span class="label label-info">{{ _('Draft') }}</span>
             {% elif package.get('state', '').startswith('deleted') %}
                 <span class="label label-important">{{ _('Deleted') }}</span>
             {% endif %}
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
-{#{% ckan_extends %}#} {% set truncate = truncate or 180 %} {% set
-truncate_title = truncate_title or 80 %} {% set title = h.usmetadata_filter
-(package.title or package.name) %} {% set notes = h.usmetadata_shorten
-(h.usmetadata_filter(package.notes), extract_length=truncate) %}
+{#{% ckan_extends %}#} {% set title = h.usmetadata_filter(package.title or
+package.name) %} {% set notes = h.usmetadata_filter(package.notes) | truncate
+(180) %}
  }}"> {% block package_item_content -%}
 {% for extra in package.extras -%} {%- if extra['key'] == 'public_access_level'
 and extra['value'] == 'public' -%}   {{ _('Public') }}  {% endif %} {%- if
 extra['key'] == 'public_access_level' and extra['value'] == 'non-public' -%}
 {{ _('Non-public') }}  {% endif %} {%- if extra['key'] == 'public_access_level'
 and extra['value'] == 'restricted public' -%}   {{ _('restricted public') }}
 {% endif %} {%- endfor %}
-**** {{ h.redacted_icon(package, 'title')|safe }} {{ h.link_to(h.truncate
-(h.usmetadata_filter(title), truncate_title), h.url_for(controller='dataset',
+**** {{ h.redacted_icon(package, 'title')|safe }} {{ h.link_to
+(h.usmetadata_filter(title)|truncate(80), h.url_for(controller='dataset',
 action='read', id=package.name), class='redacted-md') }} {% if package.get
 ('state', '').startswith('draft') %} {{ _('Draft') }} {% elif package.get
 ('state', '').startswith('deleted') %} {{ _('Deleted') }} {% endif %} {
 { h.popular('recent views', package.tracking_summary.recent, min=10) if
 package.tracking_summary }} ****
 {%- if banner -%} {{ _('Popular') }} {% endif %} {%- if notes -%} {
 { h.redacted_icon(package, 'notes')|safe }}
```

### Comparing `ckanext-usmetadata-0.2.6/ckanext_usmetadata.egg-info/PKG-INFO` & `ckanext-usmetadata-0.3.0/ckanext_usmetadata.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-usmetadata
-Version: 0.2.6
+Version: 0.3.0
 Summary: US Metadata Plugin for CKAN
 Home-page: https://github.com/GSA/ckanext-usmetadata
 Author: Data.gov
 Author-email: datagovhelp@gsa.gov
 License: Public Domain
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -15,38 +15,34 @@
 ![Github Actions](https://github.com/GSA/ckanext-usmetadata/actions/workflows/test.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/ckanext-usmetadata.svg)](https://badge.fury.io/py/ckanext-usmetadata)
 
 This CKAN Extension expands CKAN to offer a number of custom fields related to the [DCAT-US Schema](https://resources.data.gov/schemas/dcat-us/v1.1/)
 
 ### Installation
 
-To install this package, activate CKAN virtualenv (e.g. "source /path/to/virtenv/bin/activate"), then run
-
-
-    (virtenv) 'pip install -e git+https://github.com/gsa/usmetadata#egg=ckanext-usmetadata'
-    (virtenv) 'python setup.py develop'
+Add `ckanext-usmetadata` to your requirements.txt, and then pip install
     
 Then in your CKAN .ini file, add `usmetadata`
 to your ckan.plugins line:
 
 	ckan.plugins = (other plugins here...) usmetadata
 
 ### Requirements
 
 This extension is compatible with these versions of CKAN.
 
 CKAN version | Compatibility
 ------------ | -------------
-<=2.8        | no
-2.9          | yes
+<=2.9        | no
+2.10         | yes
 
 ### Development
 
 You may also install by cloning the git repo, then running ''python setup.py develop'' from the root of your source
-directory, which will install an egg link so that you can modify the code and see results without yest [localhost:5000](http://localhost:5000/).
+directory, which will install an egg link so that you can modify the code and see results [localhost:5000](http://localhost:5000/).
 
 Clean up any containers and volumes.
 
     $ make down
 
 Open a shell to run commands in the container.
 
@@ -69,15 +65,14 @@
 
     $ make test
 
 Lint the code.
 
     $ make lint
 
-
 ### Matrix builds
 
 In order to support multiple versions of CKAN, or even upgrade to new versions
 of CKAN, we support development and testing through the `CKAN_VERSION`
 environment variable.
 
     $ make CKAN_VERSION=2.9 test
```

### Comparing `ckanext-usmetadata-0.2.6/ckanext_usmetadata.egg-info/SOURCES.txt` & `ckanext-usmetadata-0.3.0/ckanext_usmetadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.2.6/setup.py` & `ckanext-usmetadata-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the relevant file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='ckanext-usmetadata',
-    version='0.2.6',
+    version='0.3.0',
     description='US Metadata Plugin for CKAN',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         'Programming Language :: Python :: 3'
     ],  # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     keywords='',
```

