# Comparing `tmp/mitreattack-python-2.0.8.tar.gz` & `tmp/mitreattack-python-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitreattack-python-2.0.8.tar", last modified: Thu Apr 20 16:55:52 2023, max compression
+gzip compressed data, was "mitreattack-python-2.0.9.tar", last modified: Sun Apr 23 22:28:22 2023, max compression
```

## Comparing `mitreattack-python-2.0.8.tar` & `mitreattack-python-2.0.9.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.664911 mitreattack-python-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-20 16:55:52.664911 mitreattack-python-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.652911 mitreattack-python-2.0.8/mitreattack/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.652911 mitreattack-python-2.0.8/mitreattack/attackToExcel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/attackToExcel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15226 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/attackToExcel/attackToExcel.py
--rw-r--r--   0 runner    (1001) docker     (123)    43100 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/attackToExcel/stixToDf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.652911 mitreattack-python-2.0.8/mitreattack/collections/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/collections/collection_to_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/collections/index_to_markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/collections/stix_to_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.652911 mitreattack-python-2.0.8/mitreattack/diffStix/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/diffStix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    88547 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/diffStix/changelog_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/download_stix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.652911 mitreattack-python-2.0.8/mitreattack/navlayers/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.656911 mitreattack-python-2.0.8/mitreattack/navlayers/core/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/layerobj.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/legenditem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/objlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/technique.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.656911 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/excel_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.656911 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   358460 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/fonts/monospace.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   317968 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/fonts/sans-serif.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    85240 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/fonts/serif.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    17843 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/matrix_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/svg_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    19848 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/svg_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/to_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)    18266 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/to_svg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.656911 mitreattack-python-2.0.8/mitreattack/navlayers/generators/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/generators/gen_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/generators/overview_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/generators/sum_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/generators/usage_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/layerExporter_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/layerGenerator_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.656911 mitreattack-python-2.0.8/mitreattack/navlayers/manipulators/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/manipulators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13317 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/manipulators/layerops.py
--rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/release_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.656911 mitreattack-python-2.0.8/mitreattack/stix20/
--rw-r--r--   0 runner    (1001) docker     (123)    61287 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/stix20/MitreAttackData.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/stix20/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/stix20/custom_attack_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.656911 mitreattack-python-2.0.8/mitreattack_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-20 16:55:52.000000 mitreattack-python-2.0.8/mitreattack_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-20 16:55:52.000000 mitreattack-python-2.0.8/mitreattack_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 16:55:52.000000 mitreattack-python-2.0.8/mitreattack_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-20 16:55:52.000000 mitreattack-python-2.0.8/mitreattack_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-20 16:55:52.000000 mitreattack-python-2.0.8/mitreattack_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-20 16:55:52.000000 mitreattack-python-2.0.8/mitreattack_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 16:55:52.664911 mitreattack-python-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.664911 mitreattack-python-2.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8158 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/tests/test_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/tests/test_mass.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/tests/test_to_excel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:28:22.879373 mitreattack-python-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-23 22:28:22.879373 mitreattack-python-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:28:22.871373 mitreattack-python-2.0.9/mitreattack/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:28:22.871373 mitreattack-python-2.0.9/mitreattack/attackToExcel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/attackToExcel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15226 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/attackToExcel/attackToExcel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43100 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/attackToExcel/stixToDf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:28:22.871373 mitreattack-python-2.0.9/mitreattack/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/collections/collection_to_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/collections/index_to_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/collections/stix_to_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:28:22.871373 mitreattack-python-2.0.9/mitreattack/diffStix/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/diffStix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88595 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/diffStix/changelog_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/download_stix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:28:22.871373 mitreattack-python-2.0.9/mitreattack/navlayers/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:28:22.875373 mitreattack-python-2.0.9/mitreattack/navlayers/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/core/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/core/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/core/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/core/layerobj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/core/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/core/legenditem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/core/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/core/objlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/core/technique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/core/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:28:22.875373 mitreattack-python-2.0.9/mitreattack/navlayers/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/exporters/excel_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:28:22.875373 mitreattack-python-2.0.9/mitreattack/navlayers/exporters/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   358460 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/exporters/fonts/monospace.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   317968 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/exporters/fonts/sans-serif.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    85240 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/exporters/fonts/serif.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    17843 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/exporters/matrix_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/exporters/svg_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19848 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/exporters/svg_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/exporters/to_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18266 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/exporters/to_svg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:28:22.875373 mitreattack-python-2.0.9/mitreattack/navlayers/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/generators/gen_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/generators/overview_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/generators/sum_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/generators/usage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/layerExporter_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/layerGenerator_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:28:22.875373 mitreattack-python-2.0.9/mitreattack/navlayers/manipulators/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/manipulators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13317 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/navlayers/manipulators/layerops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/release_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:28:22.875373 mitreattack-python-2.0.9/mitreattack/stix20/
+-rw-r--r--   0 runner    (1001) docker     (123)    61287 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/stix20/MitreAttackData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/stix20/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/mitreattack/stix20/custom_attack_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:28:22.875373 mitreattack-python-2.0.9/mitreattack_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-23 22:28:22.000000 mitreattack-python-2.0.9/mitreattack_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-23 22:28:22.000000 mitreattack-python-2.0.9/mitreattack_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 22:28:22.000000 mitreattack-python-2.0.9/mitreattack_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-23 22:28:22.000000 mitreattack-python-2.0.9/mitreattack_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-23 22:28:22.000000 mitreattack-python-2.0.9/mitreattack_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 22:28:22.000000 mitreattack-python-2.0.9/mitreattack_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 22:28:22.879373 mitreattack-python-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:28:22.879373 mitreattack-python-2.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8158 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/tests/test_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/tests/test_mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-23 22:11:31.000000 mitreattack-python-2.0.9/tests/test_to_excel.py
```

### Comparing `mitreattack-python-2.0.8/LICENSE.txt` & `mitreattack-python-2.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/NOTICE.txt` & `mitreattack-python-2.0.9/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/PKG-INFO` & `mitreattack-python-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitreattack-python
-Version: 2.0.8
+Version: 2.0.9
 Summary: MITRE ATT&CK python library
 Home-page: https://github.com/mitre-attack/mitreattack-python/
 Author: MITRE ATT&CK, MITRE Corporation
 Author-email: attack@mitre.org
 Maintainer: Jared Ondricek
 Maintainer-email: jondricek@mitre.org
 License: Apache 2.0
```

### Comparing `mitreattack-python-2.0.8/README.md` & `mitreattack-python-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/attackToExcel/attackToExcel.py` & `mitreattack-python-2.0.9/mitreattack/attackToExcel/attackToExcel.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/attackToExcel/stixToDf.py` & `mitreattack-python-2.0.9/mitreattack/attackToExcel/stixToDf.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/collections/collection_to_index.py` & `mitreattack-python-2.0.9/mitreattack/collections/collection_to_index.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/collections/index_to_markdown.py` & `mitreattack-python-2.0.9/mitreattack/collections/index_to_markdown.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/collections/stix_to_collection.py` & `mitreattack-python-2.0.9/mitreattack/collections/stix_to_collection.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/diffStix/changelog_helper.py` & `mitreattack-python-2.0.9/mitreattack/diffStix/changelog_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -421,26 +421,26 @@
                 new_mitigations[new_mitigation["id"]] = new_mitigation
 
         shared_mitigations = old_mitigations.keys() & new_mitigations.keys()
         brand_new_mitigations = new_mitigations.keys() - old_mitigations.keys()
         dropped_mitigations = old_mitigations.keys() - new_mitigations.keys()
 
         new_stix_obj["changelog_mitigations"] = {
-            "shared": [
+            "shared": sorted([
                 f"{get_attack_id(stix_obj=new_mitigations[stix_id])}: {new_mitigations[stix_id]['name']}"
                 for stix_id in shared_mitigations
-            ],
-            "new": [
+            ]),
+            "new": sorted([
                 f"{get_attack_id(stix_obj=new_mitigations[stix_id])}: {new_mitigations[stix_id]['name']}"
                 for stix_id in brand_new_mitigations
-            ],
-            "dropped": [
+            ]),
+            "dropped": sorted([
                 f"{get_attack_id(stix_obj=old_mitigations[stix_id])}: {old_mitigations[stix_id]['name']}"
                 for stix_id in dropped_mitigations
-            ],
+            ]),
         }
 
     def find_technique_detection_changes(self, new_stix_obj: dict, domain: str):
         """Find changes in the relationships between Techniques and Datacomponents.
 
         Parameters
         ----------
@@ -484,17 +484,17 @@
                 ] = f"{new_datasource_attack_id}: {new_datasource['name']} ({new_datacomponent['name']})"
 
         shared_detections = old_detections.keys() & new_detections.keys()
         brand_new_detections = new_detections.keys() - old_detections.keys()
         dropped_detections = old_detections.keys() - new_detections.keys()
 
         new_stix_obj["changelog_detections"] = {
-            "shared": [f"{new_detections[stix_id]}" for stix_id in shared_detections],
-            "new": [f"{new_detections[stix_id]}" for stix_id in brand_new_detections],
-            "dropped": [f"{old_detections[stix_id]}" for stix_id in dropped_detections],
+            "shared": sorted([f"{new_detections[stix_id]}" for stix_id in shared_detections]),
+            "new": sorted([f"{new_detections[stix_id]}" for stix_id in brand_new_detections]),
+            "dropped": sorted([f"{old_detections[stix_id]}" for stix_id in dropped_detections]),
         }
 
     def load_domain(self, domain: str):
         """Load data from directory according to domain.
 
         Parameters
         ----------
```

### Comparing `mitreattack-python-2.0.8/mitreattack/download_stix.py` & `mitreattack-python-2.0.9/mitreattack/download_stix.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/core/exceptions.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/core/filter.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/core/filter.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/core/gradient.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/core/gradient.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/core/helpers.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/core/helpers.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/core/layer.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/core/layer.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/core/layerobj.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/core/layerobj.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/core/layout.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/core/layout.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/core/legenditem.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/core/legenditem.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/core/metadata.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/core/metadata.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/core/objlink.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/core/objlink.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/core/technique.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/core/technique.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/core/versions.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/core/versions.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/exporters/excel_templates.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/exporters/excel_templates.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/exporters/fonts/monospace.ttf` & `mitreattack-python-2.0.9/mitreattack/navlayers/exporters/fonts/monospace.ttf`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/exporters/fonts/sans-serif.ttf` & `mitreattack-python-2.0.9/mitreattack/navlayers/exporters/fonts/sans-serif.ttf`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/exporters/fonts/serif.ttf` & `mitreattack-python-2.0.9/mitreattack/navlayers/exporters/fonts/serif.ttf`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/exporters/matrix_gen.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/exporters/matrix_gen.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/exporters/svg_objects.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/exporters/svg_objects.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/exporters/svg_templates.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/exporters/svg_templates.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/exporters/to_excel.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/exporters/to_excel.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/exporters/to_svg.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/exporters/to_svg.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/generators/gen_helpers.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/generators/gen_helpers.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/generators/overview_generator.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/generators/overview_generator.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/generators/sum_generator.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/generators/sum_generator.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/generators/usage_generator.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/generators/usage_generator.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/layerExporter_cli.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/layerExporter_cli.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/layerGenerator_cli.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/layerGenerator_cli.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/navlayers/manipulators/layerops.py` & `mitreattack-python-2.0.9/mitreattack/navlayers/manipulators/layerops.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/release_info.py` & `mitreattack-python-2.0.9/mitreattack/release_info.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/stix20/MitreAttackData.py` & `mitreattack-python-2.0.9/mitreattack/stix20/MitreAttackData.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack/stix20/custom_attack_objects.py` & `mitreattack-python-2.0.9/mitreattack/stix20/custom_attack_objects.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack_python.egg-info/PKG-INFO` & `mitreattack-python-2.0.9/mitreattack_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitreattack-python
-Version: 2.0.8
+Version: 2.0.9
 Summary: MITRE ATT&CK python library
 Home-page: https://github.com/mitre-attack/mitreattack-python/
 Author: MITRE ATT&CK, MITRE Corporation
 Author-email: attack@mitre.org
 Maintainer: Jared Ondricek
 Maintainer-email: jondricek@mitre.org
 License: Apache 2.0
```

### Comparing `mitreattack-python-2.0.8/mitreattack_python.egg-info/SOURCES.txt` & `mitreattack-python-2.0.9/mitreattack_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/mitreattack_python.egg-info/entry_points.txt` & `mitreattack-python-2.0.9/mitreattack_python.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/setup.py` & `mitreattack-python-2.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mitreattack-python",
-    version="2.0.8",
+    version="2.0.9",
     author="MITRE ATT&CK, MITRE Corporation",
     author_email="attack@mitre.org",
     description="MITRE ATT&CK python library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     maintainer="Jared Ondricek",
     maintainer_email="jondricek@mitre.org",
```

### Comparing `mitreattack-python-2.0.8/tests/test_cli.py` & `mitreattack-python-2.0.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/tests/test_collections.py` & `mitreattack-python-2.0.9/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/tests/test_layers.py` & `mitreattack-python-2.0.9/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/tests/test_mass.py` & `mitreattack-python-2.0.9/tests/test_mass.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.8/tests/test_to_excel.py` & `mitreattack-python-2.0.9/tests/test_to_excel.py`

 * *Files identical despite different names*

