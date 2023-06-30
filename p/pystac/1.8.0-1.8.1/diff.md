# Comparing `tmp/pystac-1.8.0.tar.gz` & `tmp/pystac-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystac-1.8.0.tar", last modified: Fri Jun 30 14:11:52 2023, max compression
+gzip compressed data, was "pystac-1.8.1.tar", last modified: Fri Jun 30 16:52:37 2023, max compression
```

## Comparing `pystac-1.8.0.tar` & `pystac-1.8.1.tar`

### file list

```diff
@@ -1,77 +1,90 @@
-drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-06-30 14:11:52.032371 pystac-1.8.0/
--rw-r--r--   0 gadomski   (501) staff       (20)      564 2021-07-20 20:04:15.000000 pystac-1.8.0/LICENSE
--rw-r--r--   0 gadomski   (501) staff       (20)       61 2023-06-07 15:48:57.000000 pystac-1.8.0/MANIFEST.in
--rw-r--r--   0 gadomski   (501) staff       (20)     4383 2023-06-30 14:11:52.031734 pystac-1.8.0/PKG-INFO
--rw-r--r--   0 gadomski   (501) staff       (20)     2952 2023-06-07 15:48:57.000000 pystac-1.8.0/README.md
--rw-r--r--   0 gadomski   (501) staff       (20)     2801 2023-06-27 22:31:38.000000 pystac-1.8.0/pyproject.toml
-drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-06-30 14:11:51.986770 pystac-1.8.0/pystac/
--rw-r--r--   0 gadomski   (501) staff       (20)     8046 2023-06-23 15:34:24.000000 pystac-1.8.0/pystac/__init__.py
--rw-r--r--   0 gadomski   (501) staff       (20)     9248 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/asset.py
--rw-r--r--   0 gadomski   (501) staff       (20)    12464 2023-06-02 16:16:56.000000 pystac-1.8.0/pystac/cache.py
--rw-r--r--   0 gadomski   (501) staff       (20)    46127 2023-06-26 22:05:11.000000 pystac-1.8.0/pystac/catalog.py
--rw-r--r--   0 gadomski   (501) staff       (20)    27635 2023-06-22 16:22:40.000000 pystac-1.8.0/pystac/collection.py
--rw-r--r--   0 gadomski   (501) staff       (20)     7625 2023-06-02 16:16:56.000000 pystac-1.8.0/pystac/common_metadata.py
--rw-r--r--   0 gadomski   (501) staff       (20)     3718 2023-06-22 16:22:40.000000 pystac-1.8.0/pystac/errors.py
-drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-06-30 14:11:52.016310 pystac-1.8.0/pystac/extensions/
--rw-r--r--   0 gadomski   (501) staff       (20)        0 2023-06-02 16:16:56.000000 pystac-1.8.0/pystac/extensions/__init__.py
--rw-r--r--   0 gadomski   (501) staff       (20)     7608 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/base.py
--rw-r--r--   0 gadomski   (501) staff       (20)    21024 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/classification.py
--rw-r--r--   0 gadomski   (501) staff       (20)    22597 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/datacube.py
--rw-r--r--   0 gadomski   (501) staff       (20)    24359 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/eo.py
--rw-r--r--   0 gadomski   (501) staff       (20)    10047 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/file.py
--rw-r--r--   0 gadomski   (501) staff       (20)     3581 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/grid.py
--rw-r--r--   0 gadomski   (501) staff       (20)     3940 2023-06-02 16:16:56.000000 pystac-1.8.0/pystac/extensions/hooks.py
--rw-r--r--   0 gadomski   (501) staff       (20)     9742 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/item_assets.py
--rw-r--r--   0 gadomski   (501) staff       (20)    28917 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/label.py
--rw-r--r--   0 gadomski   (501) staff       (20)     6409 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/mgrs.py
--rw-r--r--   0 gadomski   (501) staff       (20)    19814 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/pointcloud.py
--rw-r--r--   0 gadomski   (501) staff       (20)    15108 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/projection.py
--rw-r--r--   0 gadomski   (501) staff       (20)    25804 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/raster.py
--rw-r--r--   0 gadomski   (501) staff       (20)    22627 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/sar.py
--rw-r--r--   0 gadomski   (501) staff       (20)    10631 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/sat.py
--rw-r--r--   0 gadomski   (501) staff       (20)    12344 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/scientific.py
--rw-r--r--   0 gadomski   (501) staff       (20)     9312 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/storage.py
--rw-r--r--   0 gadomski   (501) staff       (20)    10084 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/table.py
--rw-r--r--   0 gadomski   (501) staff       (20)    10622 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/timestamps.py
--rw-r--r--   0 gadomski   (501) staff       (20)    11015 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/version.py
--rw-r--r--   0 gadomski   (501) staff       (20)    11174 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/view.py
--rw-r--r--   0 gadomski   (501) staff       (20)     6112 2023-06-23 15:34:24.000000 pystac-1.8.0/pystac/extensions/xarray_assets.py
-drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-06-30 14:11:52.021758 pystac-1.8.0/pystac/html/
--rw-r--r--   0 gadomski   (501) staff       (20)      827 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/html/JSON.jinja2
--rw-r--r--   0 gadomski   (501) staff       (20)     1439 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/html/Macros.jinja2
--rw-r--r--   0 gadomski   (501) staff       (20)       66 2023-06-02 16:16:56.000000 pystac-1.8.0/pystac/html/__init__.py
--rw-r--r--   0 gadomski   (501) staff       (20)      359 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/html/jinja_env.py
--rw-r--r--   0 gadomski   (501) staff       (20)    20499 2023-06-26 22:05:11.000000 pystac-1.8.0/pystac/item.py
--rw-r--r--   0 gadomski   (501) staff       (20)     9440 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/item_collection.py
--rw-r--r--   0 gadomski   (501) staff       (20)    22077 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/layout.py
--rw-r--r--   0 gadomski   (501) staff       (20)    17998 2023-06-27 22:31:38.000000 pystac-1.8.0/pystac/link.py
--rw-r--r--   0 gadomski   (501) staff       (20)      932 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/media_type.py
--rw-r--r--   0 gadomski   (501) staff       (20)     3972 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/provider.py
--rw-r--r--   0 gadomski   (501) staff       (20)        0 2023-06-02 16:16:56.000000 pystac-1.8.0/pystac/py.typed
--rw-r--r--   0 gadomski   (501) staff       (20)      987 2023-06-02 16:16:56.000000 pystac-1.8.0/pystac/rel_type.py
-drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-06-30 14:11:52.026064 pystac-1.8.0/pystac/serialization/
--rw-r--r--   0 gadomski   (501) staff       (20)      414 2023-06-02 16:16:56.000000 pystac-1.8.0/pystac/serialization/__init__.py
--rw-r--r--   0 gadomski   (501) staff       (20)     4173 2023-06-02 16:16:56.000000 pystac-1.8.0/pystac/serialization/common_properties.py
--rw-r--r--   0 gadomski   (501) staff       (20)     8962 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/serialization/identify.py
--rw-r--r--   0 gadomski   (501) staff       (20)     7279 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/serialization/migrate.py
--rw-r--r--   0 gadomski   (501) staff       (20)    16039 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/stac_io.py
--rw-r--r--   0 gadomski   (501) staff       (20)    24329 2023-06-27 22:31:38.000000 pystac-1.8.0/pystac/stac_object.py
-drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-06-30 14:11:52.027064 pystac-1.8.0/pystac/static/
--rw-r--r--   0 gadomski   (501) staff       (20)        0 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/static/__init__.py
--rw-r--r--   0 gadomski   (501) staff       (20)    10356 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/summaries.py
--rw-r--r--   0 gadomski   (501) staff       (20)    17667 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/utils.py
-drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-06-30 14:11:52.030145 pystac-1.8.0/pystac/validation/
--rw-r--r--   0 gadomski   (501) staff       (20)     7021 2023-06-22 16:22:40.000000 pystac-1.8.0/pystac/validation/__init__.py
-drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-06-30 14:11:52.030903 pystac-1.8.0/pystac/validation/jsonschemas/
--rw-r--r--   0 gadomski   (501) staff       (20)        0 2023-06-22 16:22:40.000000 pystac-1.8.0/pystac/validation/jsonschemas/__init__.py
--rw-r--r--   0 gadomski   (501) staff       (20)     3104 2023-06-27 22:31:38.000000 pystac-1.8.0/pystac/validation/local_validator.py
--rw-r--r--   0 gadomski   (501) staff       (20)    13733 2023-06-02 16:16:56.000000 pystac-1.8.0/pystac/validation/schema_uri_map.py
--rw-r--r--   0 gadomski   (501) staff       (20)    10370 2023-06-22 16:22:40.000000 pystac-1.8.0/pystac/validation/stac_validator.py
--rw-r--r--   0 gadomski   (501) staff       (20)     2441 2023-06-30 14:08:08.000000 pystac-1.8.0/pystac/version.py
-drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-06-30 14:11:51.993028 pystac-1.8.0/pystac.egg-info/
--rw-r--r--   0 gadomski   (501) staff       (20)     4383 2023-06-30 14:11:51.000000 pystac-1.8.0/pystac.egg-info/PKG-INFO
--rw-r--r--   0 gadomski   (501) staff       (20)     1677 2023-06-30 14:11:51.000000 pystac-1.8.0/pystac.egg-info/SOURCES.txt
--rw-r--r--   0 gadomski   (501) staff       (20)        1 2023-06-30 14:11:51.000000 pystac-1.8.0/pystac.egg-info/dependency_links.txt
--rw-r--r--   0 gadomski   (501) staff       (20)      701 2023-06-30 14:11:51.000000 pystac-1.8.0/pystac.egg-info/requires.txt
--rw-r--r--   0 gadomski   (501) staff       (20)        7 2023-06-30 14:11:51.000000 pystac-1.8.0/pystac.egg-info/top_level.txt
--rw-r--r--   0 gadomski   (501) staff       (20)       38 2023-06-30 14:11:52.032598 pystac-1.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.025838 pystac-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-30 16:52:21.000000 pystac-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-30 16:52:21.000000 pystac-1.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-30 16:52:37.025838 pystac-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-06-30 16:52:21.000000 pystac-1.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-30 16:52:21.000000 pystac-1.8.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.013837 pystac-1.8.1/pystac/
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46127 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27635 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/common_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.021838 pystac-1.8.1/pystac/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21024 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22597 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/datacube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24359 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/eo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/item_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28917 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/mgrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25804 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22627 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/sar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/sat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/scientific.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11174 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/xarray_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.021838 pystac-1.8.1/pystac/html/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/html/JSON.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/html/Macros.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/html/jinja_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20499 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/item_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22077 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17998 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/media_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/rel_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.021838 pystac-1.8.1/pystac/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/serialization/common_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/serialization/identify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/serialization/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16039 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/stac_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/stac_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.021838 pystac-1.8.1/pystac/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/summaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17667 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.021838 pystac-1.8.1/pystac/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.021838 pystac-1.8.1/pystac/validation/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.021838 pystac-1.8.1/pystac/validation/jsonschemas/geojson/
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/jsonschemas/geojson/Feature.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/jsonschemas/geojson/Geometry.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.009837 pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.025838 pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/basics.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/datetime.json
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/instrument.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/item.json
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/licensing.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/provider.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/local_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/schema_uri_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/stac_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.013837 pystac-1.8.1/pystac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-30 16:52:37.000000 pystac-1.8.1/pystac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-30 16:52:37.000000 pystac-1.8.1/pystac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:52:37.000000 pystac-1.8.1/pystac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-30 16:52:37.000000 pystac-1.8.1/pystac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 16:52:37.000000 pystac-1.8.1/pystac.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:52:37.025838 pystac-1.8.1/setup.cfg
```

### Comparing `pystac-1.8.0/LICENSE` & `pystac-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/PKG-INFO` & `pystac-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystac
-Version: 1.8.0
+Version: 1.8.1
 Summary: Python library for working with the SpatioTemporal Asset Catalog (STAC) specification
 Author-email: Rob Emanuele <rdemanuele@gmail.com>, Jon Duckworth <duckontheweb@gmail.com>
 Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/stac-utils/pystac
 Project-URL: documentation, https://pystac.readthedocs.io
 Project-URL: repository, https://github.com/stac-utils/pystac.git
```

### Comparing `pystac-1.8.0/README.md` & `pystac-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pyproject.toml` & `pystac-1.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/__init__.py` & `pystac-1.8.1/pystac/__init__.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/asset.py` & `pystac-1.8.1/pystac/asset.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/cache.py` & `pystac-1.8.1/pystac/cache.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/catalog.py` & `pystac-1.8.1/pystac/catalog.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/collection.py` & `pystac-1.8.1/pystac/collection.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/common_metadata.py` & `pystac-1.8.1/pystac/common_metadata.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/errors.py` & `pystac-1.8.1/pystac/errors.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/extensions/base.py` & `pystac-1.8.1/pystac/extensions/base.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/extensions/classification.py` & `pystac-1.8.1/pystac/extensions/classification.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/extensions/datacube.py` & `pystac-1.8.1/pystac/extensions/datacube.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/extensions/eo.py` & `pystac-1.8.1/pystac/extensions/eo.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/extensions/file.py` & `pystac-1.8.1/pystac/extensions/file.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/extensions/grid.py` & `pystac-1.8.1/pystac/extensions/grid.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/extensions/hooks.py` & `pystac-1.8.1/pystac/extensions/hooks.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/extensions/item_assets.py` & `pystac-1.8.1/pystac/extensions/item_assets.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/extensions/label.py` & `pystac-1.8.1/pystac/extensions/label.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/extensions/mgrs.py` & `pystac-1.8.1/pystac/extensions/mgrs.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/extensions/pointcloud.py` & `pystac-1.8.1/pystac/extensions/pointcloud.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/extensions/projection.py` & `pystac-1.8.1/pystac/extensions/projection.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/extensions/raster.py` & `pystac-1.8.1/pystac/extensions/raster.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/extensions/sar.py` & `pystac-1.8.1/pystac/extensions/sar.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/extensions/sat.py` & `pystac-1.8.1/pystac/extensions/sat.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/extensions/scientific.py` & `pystac-1.8.1/pystac/extensions/scientific.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/extensions/storage.py` & `pystac-1.8.1/pystac/extensions/storage.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/extensions/table.py` & `pystac-1.8.1/pystac/extensions/table.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/extensions/timestamps.py` & `pystac-1.8.1/pystac/extensions/timestamps.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/extensions/version.py` & `pystac-1.8.1/pystac/extensions/version.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/extensions/view.py` & `pystac-1.8.1/pystac/extensions/view.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/extensions/xarray_assets.py` & `pystac-1.8.1/pystac/extensions/xarray_assets.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/html/JSON.jinja2` & `pystac-1.8.1/pystac/html/JSON.jinja2`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/html/Macros.jinja2` & `pystac-1.8.1/pystac/html/Macros.jinja2`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/item.py` & `pystac-1.8.1/pystac/item.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/item_collection.py` & `pystac-1.8.1/pystac/item_collection.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/layout.py` & `pystac-1.8.1/pystac/layout.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/link.py` & `pystac-1.8.1/pystac/link.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/media_type.py` & `pystac-1.8.1/pystac/media_type.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/provider.py` & `pystac-1.8.1/pystac/provider.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/rel_type.py` & `pystac-1.8.1/pystac/rel_type.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/serialization/common_properties.py` & `pystac-1.8.1/pystac/serialization/common_properties.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/serialization/identify.py` & `pystac-1.8.1/pystac/serialization/identify.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/serialization/migrate.py` & `pystac-1.8.1/pystac/serialization/migrate.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/stac_io.py` & `pystac-1.8.1/pystac/stac_io.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/stac_object.py` & `pystac-1.8.1/pystac/stac_object.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/summaries.py` & `pystac-1.8.1/pystac/summaries.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/utils.py` & `pystac-1.8.1/pystac/utils.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/validation/__init__.py` & `pystac-1.8.1/pystac/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/validation/local_validator.py` & `pystac-1.8.1/pystac/validation/local_validator.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/validation/schema_uri_map.py` & `pystac-1.8.1/pystac/validation/schema_uri_map.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/validation/stac_validator.py` & `pystac-1.8.1/pystac/validation/stac_validator.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.0/pystac/version.py` & `pystac-1.8.1/pystac/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from typing import Optional
 
-__version__ = "1.8.0"
+__version__ = "1.8.1"
 """Library version"""
 
 
 class STACVersion:
     DEFAULT_STAC_VERSION = "1.0.0"
     """Latest STAC version supported by PySTAC"""
```

### Comparing `pystac-1.8.0/pystac.egg-info/PKG-INFO` & `pystac-1.8.1/pystac.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystac
-Version: 1.8.0
+Version: 1.8.1
 Summary: Python library for working with the SpatioTemporal Asset Catalog (STAC) specification
 Author-email: Rob Emanuele <rdemanuele@gmail.com>, Jon Duckworth <duckontheweb@gmail.com>
 Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/stac-utils/pystac
 Project-URL: documentation, https://pystac.readthedocs.io
 Project-URL: repository, https://github.com/stac-utils/pystac.git
```

### Comparing `pystac-1.8.0/pystac.egg-info/SOURCES.txt` & `pystac-1.8.1/pystac.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -59,8 +59,18 @@
 pystac/serialization/identify.py
 pystac/serialization/migrate.py
 pystac/static/__init__.py
 pystac/validation/__init__.py
 pystac/validation/local_validator.py
 pystac/validation/schema_uri_map.py
 pystac/validation/stac_validator.py
-pystac/validation/jsonschemas/__init__.py
+pystac/validation/jsonschemas/__init__.py
+pystac/validation/jsonschemas/geojson/Feature.json
+pystac/validation/jsonschemas/geojson/Geometry.json
+pystac/validation/jsonschemas/stac-spec/v1.0.0/basics.json
+pystac/validation/jsonschemas/stac-spec/v1.0.0/catalog.json
+pystac/validation/jsonschemas/stac-spec/v1.0.0/collection.json
+pystac/validation/jsonschemas/stac-spec/v1.0.0/datetime.json
+pystac/validation/jsonschemas/stac-spec/v1.0.0/instrument.json
+pystac/validation/jsonschemas/stac-spec/v1.0.0/item.json
+pystac/validation/jsonschemas/stac-spec/v1.0.0/licensing.json
+pystac/validation/jsonschemas/stac-spec/v1.0.0/provider.json
```

### Comparing `pystac-1.8.0/pystac.egg-info/requires.txt` & `pystac-1.8.1/pystac.egg-info/requires.txt`

 * *Files identical despite different names*

