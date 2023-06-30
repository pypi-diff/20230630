# Comparing `tmp/pystac-1.7.3.tar.gz` & `tmp/pystac-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystac-1.7.3.tar", last modified: Wed Apr 26 11:44:19 2023, max compression
+gzip compressed data, was "pystac-1.8.0.tar", last modified: Fri Jun 30 14:11:52 2023, max compression
```

## Comparing `pystac-1.7.3.tar` & `pystac-1.8.0.tar`

### file list

```diff
@@ -1,75 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:44:19.257161 pystac-1.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-26 11:44:09.000000 pystac-1.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-26 11:44:19.257161 pystac-1.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-04-26 11:44:09.000000 pystac-1.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:44:19.245160 pystac-1.7.3/pystac/
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    41568 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    25699 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/common_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:44:19.253161 pystac-1.7.3/pystac/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    25076 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/datacube.py
--rw-r--r--   0 runner    (1001) docker     (123)    21463 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/eo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/item_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)    28872 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/label.py
--rw-r--r--   0 runner    (1001) docker     (123)    19934 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    15365 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)    23926 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/sar.py
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/sat.py
--rw-r--r--   0 runner    (1001) docker     (123)    12416 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/scientific.py
--rw-r--r--   0 runner    (1001) docker     (123)     9380 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/timestamps.py
--rw-r--r--   0 runner    (1001) docker     (123)    11084 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:44:19.257161 pystac-1.7.3/pystac/html/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/html/Asset.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/html/Catalog.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/html/Collection.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/html/Item.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/html/ItemCollection.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/html/Link.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/html/Macros.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/html/Provider.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/html/jinja_env.py
--rw-r--r--   0 runner    (1001) docker     (123)    19333 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/item_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    23111 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/link.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/media_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/rel_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:44:19.257161 pystac-1.7.3/pystac/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/serialization/common_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/serialization/identify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/serialization/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)    15838 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/stac_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    22399 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/stac_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/summaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:44:19.257161 pystac-1.7.3/pystac/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/validation/schema_uri_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/validation/stac_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:44:19.249160 pystac-1.7.3/pystac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-26 11:44:19.000000 pystac-1.7.3/pystac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-26 11:44:19.000000 pystac-1.7.3/pystac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:44:19.000000 pystac-1.7.3/pystac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:44:19.000000 pystac-1.7.3/pystac.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 11:44:19.000000 pystac-1.7.3/pystac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-26 11:44:19.000000 pystac-1.7.3/pystac.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-26 11:44:19.261160 pystac-1.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-26 11:44:09.000000 pystac-1.7.3/setup.py
+drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-06-30 14:11:52.032371 pystac-1.8.0/
+-rw-r--r--   0 gadomski   (501) staff       (20)      564 2021-07-20 20:04:15.000000 pystac-1.8.0/LICENSE
+-rw-r--r--   0 gadomski   (501) staff       (20)       61 2023-06-07 15:48:57.000000 pystac-1.8.0/MANIFEST.in
+-rw-r--r--   0 gadomski   (501) staff       (20)     4383 2023-06-30 14:11:52.031734 pystac-1.8.0/PKG-INFO
+-rw-r--r--   0 gadomski   (501) staff       (20)     2952 2023-06-07 15:48:57.000000 pystac-1.8.0/README.md
+-rw-r--r--   0 gadomski   (501) staff       (20)     2801 2023-06-27 22:31:38.000000 pystac-1.8.0/pyproject.toml
+drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-06-30 14:11:51.986770 pystac-1.8.0/pystac/
+-rw-r--r--   0 gadomski   (501) staff       (20)     8046 2023-06-23 15:34:24.000000 pystac-1.8.0/pystac/__init__.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     9248 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/asset.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    12464 2023-06-02 16:16:56.000000 pystac-1.8.0/pystac/cache.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    46127 2023-06-26 22:05:11.000000 pystac-1.8.0/pystac/catalog.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    27635 2023-06-22 16:22:40.000000 pystac-1.8.0/pystac/collection.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     7625 2023-06-02 16:16:56.000000 pystac-1.8.0/pystac/common_metadata.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     3718 2023-06-22 16:22:40.000000 pystac-1.8.0/pystac/errors.py
+drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-06-30 14:11:52.016310 pystac-1.8.0/pystac/extensions/
+-rw-r--r--   0 gadomski   (501) staff       (20)        0 2023-06-02 16:16:56.000000 pystac-1.8.0/pystac/extensions/__init__.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     7608 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/base.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    21024 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/classification.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    22597 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/datacube.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    24359 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/eo.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    10047 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/file.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     3581 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/grid.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     3940 2023-06-02 16:16:56.000000 pystac-1.8.0/pystac/extensions/hooks.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     9742 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/item_assets.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    28917 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/label.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     6409 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/mgrs.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    19814 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/pointcloud.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    15108 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/projection.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    25804 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/raster.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    22627 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/sar.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    10631 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/sat.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    12344 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/scientific.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     9312 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/storage.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    10084 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/table.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    10622 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/timestamps.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    11015 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/version.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    11174 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/extensions/view.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     6112 2023-06-23 15:34:24.000000 pystac-1.8.0/pystac/extensions/xarray_assets.py
+drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-06-30 14:11:52.021758 pystac-1.8.0/pystac/html/
+-rw-r--r--   0 gadomski   (501) staff       (20)      827 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/html/JSON.jinja2
+-rw-r--r--   0 gadomski   (501) staff       (20)     1439 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/html/Macros.jinja2
+-rw-r--r--   0 gadomski   (501) staff       (20)       66 2023-06-02 16:16:56.000000 pystac-1.8.0/pystac/html/__init__.py
+-rw-r--r--   0 gadomski   (501) staff       (20)      359 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/html/jinja_env.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    20499 2023-06-26 22:05:11.000000 pystac-1.8.0/pystac/item.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     9440 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/item_collection.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    22077 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/layout.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    17998 2023-06-27 22:31:38.000000 pystac-1.8.0/pystac/link.py
+-rw-r--r--   0 gadomski   (501) staff       (20)      932 2023-06-14 15:40:42.000000 pystac-1.8.0/pystac/media_type.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     3972 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/provider.py
+-rw-r--r--   0 gadomski   (501) staff       (20)        0 2023-06-02 16:16:56.000000 pystac-1.8.0/pystac/py.typed
+-rw-r--r--   0 gadomski   (501) staff       (20)      987 2023-06-02 16:16:56.000000 pystac-1.8.0/pystac/rel_type.py
+drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-06-30 14:11:52.026064 pystac-1.8.0/pystac/serialization/
+-rw-r--r--   0 gadomski   (501) staff       (20)      414 2023-06-02 16:16:56.000000 pystac-1.8.0/pystac/serialization/__init__.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     4173 2023-06-02 16:16:56.000000 pystac-1.8.0/pystac/serialization/common_properties.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     8962 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/serialization/identify.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     7279 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/serialization/migrate.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    16039 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/stac_io.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    24329 2023-06-27 22:31:38.000000 pystac-1.8.0/pystac/stac_object.py
+drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-06-30 14:11:52.027064 pystac-1.8.0/pystac/static/
+-rw-r--r--   0 gadomski   (501) staff       (20)        0 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/static/__init__.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    10356 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/summaries.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    17667 2023-06-07 15:48:57.000000 pystac-1.8.0/pystac/utils.py
+drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-06-30 14:11:52.030145 pystac-1.8.0/pystac/validation/
+-rw-r--r--   0 gadomski   (501) staff       (20)     7021 2023-06-22 16:22:40.000000 pystac-1.8.0/pystac/validation/__init__.py
+drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-06-30 14:11:52.030903 pystac-1.8.0/pystac/validation/jsonschemas/
+-rw-r--r--   0 gadomski   (501) staff       (20)        0 2023-06-22 16:22:40.000000 pystac-1.8.0/pystac/validation/jsonschemas/__init__.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     3104 2023-06-27 22:31:38.000000 pystac-1.8.0/pystac/validation/local_validator.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    13733 2023-06-02 16:16:56.000000 pystac-1.8.0/pystac/validation/schema_uri_map.py
+-rw-r--r--   0 gadomski   (501) staff       (20)    10370 2023-06-22 16:22:40.000000 pystac-1.8.0/pystac/validation/stac_validator.py
+-rw-r--r--   0 gadomski   (501) staff       (20)     2441 2023-06-30 14:08:08.000000 pystac-1.8.0/pystac/version.py
+drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-06-30 14:11:51.993028 pystac-1.8.0/pystac.egg-info/
+-rw-r--r--   0 gadomski   (501) staff       (20)     4383 2023-06-30 14:11:51.000000 pystac-1.8.0/pystac.egg-info/PKG-INFO
+-rw-r--r--   0 gadomski   (501) staff       (20)     1677 2023-06-30 14:11:51.000000 pystac-1.8.0/pystac.egg-info/SOURCES.txt
+-rw-r--r--   0 gadomski   (501) staff       (20)        1 2023-06-30 14:11:51.000000 pystac-1.8.0/pystac.egg-info/dependency_links.txt
+-rw-r--r--   0 gadomski   (501) staff       (20)      701 2023-06-30 14:11:51.000000 pystac-1.8.0/pystac.egg-info/requires.txt
+-rw-r--r--   0 gadomski   (501) staff       (20)        7 2023-06-30 14:11:51.000000 pystac-1.8.0/pystac.egg-info/top_level.txt
+-rw-r--r--   0 gadomski   (501) staff       (20)       38 2023-06-30 14:11:52.032598 pystac-1.8.0/setup.cfg
```

### Comparing `pystac-1.7.3/LICENSE` & `pystac-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pystac-1.7.3/PKG-INFO` & `pystac-1.8.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,88 @@
 Metadata-Version: 2.1
 Name: pystac
-Version: 1.7.3
-Summary: Python library for working with Spatiotemporal Asset Catalog (STAC).
-Home-page: https://github.com/stac-utils/pystac
-Author: stac-utils
-Author-email: stac@radiant.earth
-License: Apache Software License 2.0
-Project-URL: Tracker, https://github.com/stac-utils/pystac/issues
-Project-URL: Documentation, https://pystac.readthedocs.io/en/latest/
-Project-URL: GitHub Discussions, https://github.com/radiantearth/stac-spec/discussions/categories/pystac
+Version: 1.8.0
+Summary: Python library for working with the SpatioTemporal Asset Catalog (STAC) specification
+Author-email: Rob Emanuele <rdemanuele@gmail.com>, Jon Duckworth <duckontheweb@gmail.com>
+Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
+License: Apache-2.0
+Project-URL: homepage, https://github.com/stac-utils/pystac
+Project-URL: documentation, https://pystac.readthedocs.io
+Project-URL: repository, https://github.com/stac-utils/pystac.git
+Project-URL: changelog, https://github.com/stac-utils/pystac/blob/main/CHANGELOG.md
+Project-URL: discussions, https://github.com/radiantearth/stac-spec/discussions/categories/stac-software
 Keywords: pystac,imagery,raster,catalog,STAC
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: validation
+Provides-Extra: bench
+Provides-Extra: docs
+Provides-Extra: jinja2
 Provides-Extra: orjson
+Provides-Extra: test
 Provides-Extra: urllib3
+Provides-Extra: validation
 License-File: LICENSE
 
 # PySTAC
 
 [![Build Status](https://github.com/stac-utils/pystac/workflows/CI/badge.svg?branch=main)](https://github.com/stac-utils/pystac/actions/workflows/continuous-integration.yml)
 [![PyPI version](https://badge.fury.io/py/pystac.svg)](https://badge.fury.io/py/pystac)
 [![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/pystac)](https://anaconda.org/conda-forge/pystac)
 [![Documentation](https://readthedocs.org/projects/pystac/badge/?version=latest)](https://pystac.readthedocs.io/en/latest/)
 [![codecov](https://codecov.io/gh/stac-utils/pystac/branch/main/graph/badge.svg)](https://codecov.io/gh/stac-utils/pystac)
 [![Gitter](https://badges.gitter.im/SpatioTemporal-Asset-Catalog/python.svg)](https://gitter.im/SpatioTemporal-Asset-Catalog/python?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
-PySTAC is a library for working with [SpatioTemporal Asset Catalog](https://stacspec.org) in Python 3.
+PySTAC is a library for working with the [SpatioTemporal Asset Catalog](https://stacspec.org) specification in Python 3.
 
 ## Installation
 
 ### Install from PyPi (recommended)
 
 ```shell
 pip install pystac
 ```
 
 If you would like to enable the validation feature utilizing the
 [jsonschema](https://pypi.org/project/jsonschema/) project, install with the optional
 `validation` requirements:
 
 ```shell
-pip install pystac[validation]
+pip install 'pystac[validation]'
 ```
 
 If you would like to use the [`orjson`](https://pypi.org/project/orjson/) instead of the
 standard `json` library for JSON serialization/deserialization, install with the
 optional `orjson` requirements:
 
 ```shell
-pip install pystac[orjson]
+pip install 'pystac[orjson]'
 ```
 
 If you would like to use a custom `RetryStacIO` class for automatically retrying
 network requests when reading with PySTAC, you'll need
 [`urllib3`](https://urllib3.readthedocs.io/en/stable/):
 
 ```shell
-pip install pystac[urllib3]
+pip install 'pystac[urllib3]'
+```
+
+If you are using jupyter notebooks and want to enable pretty display of pystac objects you'll need [`jinja2`](https://pypi.org/project/Jinja2/)
+
+```shell
+pip install 'pystac[jinja2]'
 ```
 
 ### Install from source
 
 ```shell
 git clone https://github.com/stac-utils/pystac.git
 cd pystac
```

### Comparing `pystac-1.7.3/README.md` & `pystac-1.8.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,46 +4,52 @@
 [![PyPI version](https://badge.fury.io/py/pystac.svg)](https://badge.fury.io/py/pystac)
 [![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/pystac)](https://anaconda.org/conda-forge/pystac)
 [![Documentation](https://readthedocs.org/projects/pystac/badge/?version=latest)](https://pystac.readthedocs.io/en/latest/)
 [![codecov](https://codecov.io/gh/stac-utils/pystac/branch/main/graph/badge.svg)](https://codecov.io/gh/stac-utils/pystac)
 [![Gitter](https://badges.gitter.im/SpatioTemporal-Asset-Catalog/python.svg)](https://gitter.im/SpatioTemporal-Asset-Catalog/python?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
-PySTAC is a library for working with [SpatioTemporal Asset Catalog](https://stacspec.org) in Python 3.
+PySTAC is a library for working with the [SpatioTemporal Asset Catalog](https://stacspec.org) specification in Python 3.
 
 ## Installation
 
 ### Install from PyPi (recommended)
 
 ```shell
 pip install pystac
 ```
 
 If you would like to enable the validation feature utilizing the
 [jsonschema](https://pypi.org/project/jsonschema/) project, install with the optional
 `validation` requirements:
 
 ```shell
-pip install pystac[validation]
+pip install 'pystac[validation]'
 ```
 
 If you would like to use the [`orjson`](https://pypi.org/project/orjson/) instead of the
 standard `json` library for JSON serialization/deserialization, install with the
 optional `orjson` requirements:
 
 ```shell
-pip install pystac[orjson]
+pip install 'pystac[orjson]'
 ```
 
 If you would like to use a custom `RetryStacIO` class for automatically retrying
 network requests when reading with PySTAC, you'll need
 [`urllib3`](https://urllib3.readthedocs.io/en/stable/):
 
 ```shell
-pip install pystac[urllib3]
+pip install 'pystac[urllib3]'
+```
+
+If you are using jupyter notebooks and want to enable pretty display of pystac objects you'll need [`jinja2`](https://pypi.org/project/Jinja2/)
+
+```shell
+pip install 'pystac[jinja2]'
 ```
 
 ### Install from source
 
 ```shell
 git clone https://github.com/stac-utils/pystac.git
 cd pystac
```

### Comparing `pystac-1.7.3/pystac/__init__.py` & `pystac-1.8.0/pystac/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,64 +63,75 @@
     get_stac_version,
     set_stac_version,
 )
 from pystac.media_type import MediaType
 from pystac.rel_type import RelType
 from pystac.stac_io import StacIO
 from pystac.stac_object import STACObject, STACObjectType
-from pystac.link import Link, HIERARCHICAL_LINKS, HREF
+from pystac.link import Link, HIERARCHICAL_LINKS
 from pystac.catalog import Catalog, CatalogType
 from pystac.collection import (
     Collection,
     Extent,
     SpatialExtent,
     TemporalExtent,
 )
 from pystac.common_metadata import CommonMetadata
 from pystac.summaries import RangeSummary, Summaries
 from pystac.asset import Asset
 from pystac.item import Item
 from pystac.item_collection import ItemCollection
 from pystac.provider import ProviderRole, Provider
+from pystac.utils import HREF
 import pystac.validation
 
 import pystac.extensions.hooks
+import pystac.extensions.classification
 import pystac.extensions.datacube
 import pystac.extensions.eo
 import pystac.extensions.file
+import pystac.extensions.grid
 import pystac.extensions.item_assets
 import pystac.extensions.label
+import pystac.extensions.mgrs
 import pystac.extensions.pointcloud
 import pystac.extensions.projection
+import pystac.extensions.raster
 import pystac.extensions.sar
 import pystac.extensions.sat
 import pystac.extensions.scientific
 import pystac.extensions.storage
 import pystac.extensions.table
 import pystac.extensions.timestamps
 import pystac.extensions.version
 import pystac.extensions.view
+import pystac.extensions.xarray_assets
 
 EXTENSION_HOOKS = pystac.extensions.hooks.RegisteredExtensionHooks(
     [
+        pystac.extensions.classification.CLASSIFICATION_EXTENSION_HOOKS,
         pystac.extensions.datacube.DATACUBE_EXTENSION_HOOKS,
         pystac.extensions.eo.EO_EXTENSION_HOOKS,
         pystac.extensions.file.FILE_EXTENSION_HOOKS,
+        pystac.extensions.grid.GRID_EXTENSION_HOOKS,
         pystac.extensions.item_assets.ITEM_ASSETS_EXTENSION_HOOKS,
         pystac.extensions.label.LABEL_EXTENSION_HOOKS,
+        pystac.extensions.mgrs.MGRS_EXTENSION_HOOKS,
         pystac.extensions.pointcloud.POINTCLOUD_EXTENSION_HOOKS,
         pystac.extensions.projection.PROJECTION_EXTENSION_HOOKS,
+        pystac.extensions.raster.RASTER_EXTENSION_HOOKS,
         pystac.extensions.sar.SAR_EXTENSION_HOOKS,
         pystac.extensions.sat.SAT_EXTENSION_HOOKS,
         pystac.extensions.scientific.SCIENTIFIC_EXTENSION_HOOKS,
         pystac.extensions.storage.STORAGE_EXTENSION_HOOKS,
         pystac.extensions.table.TABLE_EXTENSION_HOOKS,
         pystac.extensions.timestamps.TIMESTAMPS_EXTENSION_HOOKS,
         pystac.extensions.version.VERSION_EXTENSION_HOOKS,
         pystac.extensions.view.VIEW_EXTENSION_HOOKS,
+        pystac.extensions.xarray_assets.XARRAY_ASSETS_EXTENSION_HOOKS,
     ]
 )
 
 
 def read_file(href: HREF, stac_io: Optional[StacIO] = None) -> STACObject:
     """Reads a STAC object from a file.
```

### Comparing `pystac-1.7.3/pystac/asset.py` & `pystac-1.8.0/pystac/asset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+import os
+import shutil
 from copy import copy, deepcopy
 from html import escape
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type, TypeVar, Union
 
 from pystac import common_metadata, utils
 from pystac.html.jinja_env import get_jinja_env
 
@@ -67,15 +69,15 @@
         href: str,
         title: Optional[str] = None,
         description: Optional[str] = None,
         media_type: Optional[str] = None,
         roles: Optional[List[str]] = None,
         extra_fields: Optional[Dict[str, Any]] = None,
     ) -> None:
-        self.href = href
+        self.href = utils.make_posix_style(href)
         self.title = title
         self.description = description
         self.media_type = media_type
         self.roles = roles
         self.extra_fields = extra_fields or {}
 
         # The Item which owns this Asset.
@@ -108,18 +110,18 @@
             if self.owner is not None:
                 item_self = self.owner.get_self_href()
                 if item_self is not None:
                     return utils.make_absolute_href(self.href, item_self)
             return None
 
     def to_dict(self) -> Dict[str, Any]:
-        """Generate a dictionary representing the JSON of this Asset.
+        """Returns this Asset as a dictionary.
 
         Returns:
-            dict: A serialization of the Asset that can be written out as JSON.
+            dict: A serialization of the Asset.
         """
 
         d: Dict[str, Any] = {"href": self.href}
 
         if self.media_type is not None:
             d["type"] = self.media_type
 
@@ -177,16 +179,16 @@
 
     def __repr__(self) -> str:
         return "<Asset href={}>".format(self.href)
 
     def _repr_html_(self) -> str:
         jinja_env = get_jinja_env()
         if jinja_env:
-            template = jinja_env.get_template("Asset.jinja2")
-            return str(template.render(asset=self))
+            template = jinja_env.get_template("JSON.jinja2")
+            return str(template.render(dict=self.to_dict()))
         else:
             return escape(repr(self))
 
     @classmethod
     def from_dict(cls: Type[A], d: Dict[str, Any]) -> A:
         """Constructs an Asset from a dict.
 
@@ -207,7 +209,70 @@
             href=href,
             media_type=media_type,
             title=title,
             description=description,
             roles=roles,
             extra_fields=properties,
         )
+
+    def move(self, href: str) -> Asset:
+        """Moves this asset's file to a new location on the local filesystem,
+        setting the asset href accordingly.
+
+        Modifies the asset in place, and returns the same asset.
+
+        Args:
+            href: The new asset location. Must be a local path. If relative
+                it must be relative to the owner object.
+
+        Returns:
+            Asset: The asset with the updated href.
+        """
+        src = _absolute_href(self.href, self.owner, "move")
+        dst = _absolute_href(href, self.owner, "move")
+        shutil.move(src, dst)
+        self.href = href
+        return self
+
+    def copy(self, href: str) -> Asset:
+        """Copies this asset's file to a new location on the local filesystem,
+        setting the asset href accordingly.
+
+        Modifies the asset in place, and returns the same asset.
+
+        Args:
+            href: The new asset location. Must be a local path. If relative
+                it must be relative to the owner object.
+
+        Returns:
+            Asset: The asset with the updated href.
+        """
+        src = _absolute_href(self.href, self.owner, "copy")
+        dst = _absolute_href(href, self.owner, "copy")
+        shutil.copy2(src, dst)
+        self.href = href
+        return self
+
+    def delete(self) -> None:
+        """Delete this asset's file. Does not delete the asset from the item
+        that owns it. See :func:`~pystac.Item.delete_asset` for that.
+
+        Does not modify the asset.
+        """
+        href = _absolute_href(self.href, self.owner, "delete")
+        os.remove(href)
+
+
+def _absolute_href(
+    href: str, owner: Optional[Union[Item, Collection]], action: str = "access"
+) -> str:
+    if utils.is_absolute_href(href):
+        return href
+    else:
+        item_self = owner.get_self_href() if owner else None
+        if item_self is None:
+            raise ValueError(
+                f"Cannot {action} file if asset href ('{href}') is relative "
+                "and owner item is not set. Hint: try using "
+                ":func:`~pystac.Item.make_asset_hrefs_absolute`"
+            )
+        return utils.make_absolute_href(href, item_self)
```

### Comparing `pystac-1.7.3/pystac/cache.py` & `pystac-1.8.0/pystac/cache.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.3/pystac/catalog.py` & `pystac-1.8.0/pystac/catalog.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from __future__ import annotations
 
 import os
+import warnings
 from copy import deepcopy
-from html import escape
+from itertools import chain
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
+    Iterator,
     List,
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
 )
 
 import pystac
 from pystac.cache import ResolvedObjectCache
 from pystac.errors import STACTypeError
-from pystac.html.jinja_env import get_jinja_env
 from pystac.layout import (
     BestPracticesLayoutStrategy,
     HrefLayoutStrategy,
     LayoutTemplate,
 )
 from pystac.link import Link
 from pystac.serialization import (
@@ -200,22 +201,14 @@
         self.catalog_type: CatalogType = catalog_type
 
         self._resolved_objects.cache(self)
 
     def __repr__(self) -> str:
         return "<Catalog id={}>".format(self.id)
 
-    def _repr_html_(self) -> str:
-        jinja_env = get_jinja_env()
-        if jinja_env:
-            template = jinja_env.get_template("Catalog.jinja2")
-            return str(template.render(catalog=self))
-        else:
-            return escape(repr(self))
-
     def set_root(self, root: Optional["Catalog"]) -> None:
         STACObject.set_root(self, root)
         if root is not None:
             root._resolved_objects = ResolvedObjectCache.merge(
                 root._resolved_objects, self._resolved_objects
             )
 
@@ -233,128 +226,183 @@
         ]
 
     def add_child(
         self,
         child: Union["Catalog", Collection],
         title: Optional[str] = None,
         strategy: Optional[HrefLayoutStrategy] = None,
-    ) -> None:
+        set_parent: bool = True,
+    ) -> Link:
         """Adds a link to a child :class:`~pystac.Catalog` or
-        :class:`~pystac.Collection`. This method will set the child's parent to this
-        object, and its root to this Catalog's root.
+        :class:`~pystac.Collection`.
+
+        This method will set the child's parent to this object and potentially
+        override its self_link (unless ``set_parent`` is False).
+
+        It will always set its root to this Catalog's root.
 
         Args:
             child : The child to add.
             title : Optional title to give to the :class:`~pystac.Link`
             strategy : The layout strategy to use for setting the
                 self href of the child. If not provided, defaults to
                 :class:`~pystac.layout.BestPracticesLayoutStrategy`.
+            set_parent : Whether to set the parent on the child as well.
+                Defaults to True.
+
+        Returns:
+            Link: The link created for the child
         """
 
         # Prevent typo confusion
         if isinstance(child, pystac.Item):
             raise pystac.STACError("Cannot add item as child. Use add_item instead.")
 
         if strategy is None:
             strategy = BestPracticesLayoutStrategy()
 
         child.set_root(self.get_root())
-        child.set_parent(self)
+        if set_parent:
+            child.set_parent(self)
+        else:
+            child._allow_parent_to_override_href = False
 
         # set self link
         self_href = self.get_self_href()
-        if self_href:
+        if self_href and set_parent:
             child_href = strategy.get_href(child, os.path.dirname(self_href))
             child.set_self_href(child_href)
 
-        self.add_link(Link.child(child, title=title))
-
-    def add_children(self, children: Iterable[Union["Catalog", Collection]]) -> None:
+        child_link = Link.child(child, title=title)
+        self.add_link(child_link)
+        return child_link
+
+    def add_children(
+        self, children: Iterable[Union["Catalog", Collection]]
+    ) -> List[Link]:
         """Adds links to multiple :class:`~pystac.Catalog` or `~pystac.Collection`
         objects. This method will set each child's parent to this object, and their
         root to this Catalog's root.
 
         Args:
             children : The children to add.
+
+        Returns:
+            List[Link]: An array of links created for the children
         """
-        for child in children:
-            self.add_child(child)
+        return [self.add_child(child) for child in children]
 
     def add_item(
         self,
         item: Item,
         title: Optional[str] = None,
         strategy: Optional[HrefLayoutStrategy] = None,
-    ) -> None:
+        set_parent: bool = True,
+    ) -> Link:
         """Adds a link to an :class:`~pystac.Item`.
-        This method will set the item's parent to this object, and its root to
-        this Catalog's root.
+
+        This method will set the item's parent to this object and potentially
+        override its self_link (unless ``set_parent`` is False)
+
+        It will always set its root to this Catalog's root.
 
         Args:
             item : The item to add.
             title : Optional title to give to the :class:`~pystac.Link`
             strategy : The layout strategy to use for setting the
                 self href of the item. If not provided, defaults to
                 :class:`~pystac.layout.BestPracticesLayoutStrategy`.
+            set_parent : Whether to set the parent on the item as well.
+                Defaults to True.
+
+        Returns:
+            Link: The link created for the item
         """
 
         # Prevent typo confusion
         if isinstance(item, pystac.Catalog):
             raise pystac.STACError("Cannot add catalog as item. Use add_child instead.")
 
         if strategy is None:
             strategy = BestPracticesLayoutStrategy()
 
         item.set_root(self.get_root())
-        item.set_parent(self)
+        if set_parent:
+            item.set_parent(self)
+        else:
+            item._allow_parent_to_override_href = False
 
         # set self link
         self_href = self.get_self_href()
-        if self_href:
+        if self_href and set_parent:
             item_href = strategy.get_href(item, os.path.dirname(self_href))
             item.set_self_href(item_href)
 
-        self.add_link(Link.item(item, title=title))
+        item_link = Link.item(item, title=title)
+        self.add_link(item_link)
+        return item_link
 
     def add_items(
         self,
         items: Iterable[Item],
         strategy: Optional[HrefLayoutStrategy] = None,
-    ) -> None:
+    ) -> List[Link]:
         """Adds links to multiple :class:`Items <pystac.Item>`.
 
         This method will set each item's parent to this object, and their root to
         this Catalog's root.
 
         Args:
             items : The items to add.
             strategy : The layout strategy to use for setting the
                 self href of the items. If not provided, defaults to
                 :class:`~pystac.layout.BestPracticesLayoutStrategy`.
+
+        Returns:
+            List[Link]: A list of links created for the item
         """
-        for item in items:
-            self.add_item(item, strategy=strategy)
+        return [self.add_item(item, strategy=strategy) for item in items]
 
     def get_child(
-        self, id: str, recursive: bool = False
+        self, id: str, recursive: bool = False, sort_links_by_id: bool = True
     ) -> Optional[Union["Catalog", Collection]]:
         """Gets the child of this catalog with the given ID, if it exists.
 
         Args:
             id : The ID of the child to find.
             recursive : If True, search this catalog and all children for the
                 item; otherwise, only search the children of this catalog. Defaults
                 to False.
+            sort_links_by_id : If True, links containing the ID will be checked
+                first. If links do not contain the ID then setting this to False
+                will improve performance. Defaults to True.
 
         Return:
             Optional Catalog or Collection: The child with the given ID,
             or None if not found.
         """
         if not recursive:
-            return next((c for c in self.get_children() if c.id == id), None)
+            children: Iterable[Union[pystac.Catalog, pystac.Collection]]
+            if not sort_links_by_id:
+                children = self.get_children()
+            else:
+
+                def sort_function(links: List[Link]) -> List[Link]:
+                    return sorted(
+                        links,
+                        key=lambda x: (href := x.get_href()) is None or id not in href,
+                    )
+
+                children = map(
+                    lambda x: cast(Union[pystac.Catalog, pystac.Collection], x),
+                    self.get_stac_objects(
+                        pystac.RelType.CHILD, modify_links=sort_function
+                    ),
+                )
+            return next((c for c in children if c.id == id), None)
         else:
             for root, _, _ in self.walk():
                 child = root.get_child(id, recursive=False)
                 if child is not None:
                     return child
             return None
 
@@ -421,43 +469,74 @@
                     new_links.append(link)
                 else:
                     child.set_parent(None)
                     child.set_root(None)
         self.links = new_links
 
     def get_item(self, id: str, recursive: bool = False) -> Optional[Item]:
-        """Returns an item with a given ID.
+        """
+        DEPRECATED.
+
+        .. deprecated:: 1.8
+            Use :meth:`next(pystac.Catalog.get_items(id), None)` instead.
+
+        Returns an item with a given ID.
 
         Args:
             id : The ID of the item to find.
             recursive : If True, search this catalog and all children for the
                 item; otherwise, only search the items of this catalog. Defaults
                 to False.
 
         Return:
             Item or None: The item with the given ID, or None if not found.
         """
+        warnings.warn(
+            "get_item is deprecated and will be removed in v2. "
+            "Use next(self.get_items(id), None) instead",
+            DeprecationWarning,
+        )
         if not recursive:
             return next((i for i in self.get_items() if i.id == id), None)
         else:
             for root, _, _ in self.walk():
                 item = root.get_item(id, recursive=False)
                 if item is not None:
                     return item
             return None
 
-    def get_items(self) -> Iterable[Item]:
-        """Return all items of this catalog.
+    def get_items(self, *ids: str, recursive: bool = False) -> Iterator[Item]:
+        """Return all items or specific items of this catalog.
+
+        Args:
+            *ids : The IDs of the items to include.
+            recursive : If True, search this catalog and all children for the
+                item; otherwise, only search the items of this catalog. Defaults
+                to False.
 
         Return:
-            Iterable[Item]: Generator of items whose parent is this catalog.
+            Iterator[Item]: Generator of items whose parent is this catalog, and
+                (if recursive) all catalogs or collections connected to this catalog
+                through child links.
         """
-        return map(
-            lambda x: cast(pystac.Item, x), self.get_stac_objects(pystac.RelType.ITEM)
-        )
+        items: Iterator[Item]
+        if not recursive:
+            items = map(
+                lambda x: cast(pystac.Item, x),
+                self.get_stac_objects(pystac.RelType.ITEM),
+            )
+        else:
+            items = chain(
+                self.get_items(recursive=False),
+                *(child.get_items(recursive=True) for child in self.get_children()),
+            )
+        if ids:
+            yield from (i for i in items if i.id in ids)
+        else:
+            yield from items
 
     def clear_items(self) -> None:
         """Removes all items from this catalog.
 
         Return:
             Catalog: Returns ``self``
         """
@@ -486,26 +565,37 @@
                 if item.id != item_id:
                     new_links.append(link)
                 else:
                     item.set_parent(None)
                     item.set_root(None)
         self.links = new_links
 
-    def get_all_items(self) -> Iterable[Item]:
-        """Get all items from this catalog and all subcatalogs. Will traverse
+    def get_all_items(self) -> Iterator[Item]:
+        """
+        DEPRECATED.
+
+        .. deprecated:: 1.8
+            Use :meth:`pystac.Catalog.get_items(recursive=True)` instead.
+
+        Get all items from this catalog and all subcatalogs. Will traverse
         any subcatalogs recursively.
 
         Returns:
             Generator[Item]: All items that belong to this catalog, and all
                 catalogs or collections connected to this catalog through
                 child links.
         """
-        yield from self.get_items()
-        for child in self.get_children():
-            yield from child.get_all_items()
+        warnings.warn(
+            "get_item is deprecated and will be removed in v2",
+            DeprecationWarning,
+        )
+        return chain(
+            self.get_items(),
+            *(child.get_all_items() for child in self.get_children()),
+        )
 
     def get_item_links(self) -> List[Link]:
         """Return all item links of this catalog.
 
         Return:
             List[Link]: List of links of this catalog with ``rel == 'item'``
         """
@@ -563,28 +653,26 @@
                     clone.add_link(link.clone())
             else:
                 clone.add_link(link.clone())
 
         return clone
 
     def make_all_asset_hrefs_relative(self) -> None:
-        """Makes all the HREFs of assets belonging to items in this catalog
-        and all children to be relative, recursively.
-        """
-        for _, _, items in self.walk():
-            for item in items:
-                item.make_asset_hrefs_relative()
+        """Recursively makes all the HREFs of assets in this catalog relative"""
+        for item in self.get_items(recursive=True):
+            item.make_asset_hrefs_relative()
+        for collection in self.get_all_collections():
+            collection.make_asset_hrefs_relative()
 
     def make_all_asset_hrefs_absolute(self) -> None:
-        """Makes all the HREFs of assets belonging to items in this catalog
-        and all children to be absolute, recursively.
-        """
-        for _, _, items in self.walk():
-            for item in items:
-                item.make_asset_hrefs_absolute()
+        """Recursively makes all the HREFs of assets in this catalog absolute"""
+        for item in self.get_items(recursive=True):
+            item.make_asset_hrefs_absolute()
+        for collection in self.get_all_collections():
+            collection.make_asset_hrefs_absolute()
 
     def normalize_and_save(
         self,
         root_href: str,
         catalog_type: Optional[CatalogType] = None,
         strategy: Optional[HrefLayoutStrategy] = None,
         stac_io: Optional[pystac.StacIO] = None,
@@ -652,51 +740,69 @@
         else:
             _strategy = strategy
 
         # Normalizing requires an absolute path
         if not is_absolute_href(root_href):
             root_href = make_absolute_href(root_href, os.getcwd(), start_is_dir=True)
 
-        def process_item(item: Item, _root_href: str) -> Callable[[], None]:
+        def process_item(
+            item: Item, _root_href: str, parent: Optional[Catalog]
+        ) -> Optional[Callable[[], None]]:
             if not skip_unresolved:
                 item.resolve_links()
 
+            # Abort as the intended parent is not the actual parent
+            # https://github.com/stac-utils/pystac/issues/1116
+            if parent is not None and item.get_parent() != parent:
+                return None
+
             new_self_href = _strategy.get_href(item, _root_href)
 
             def fn() -> None:
                 item.set_self_href(new_self_href)
 
             return fn
 
         def process_catalog(
-            cat: Catalog, _root_href: str, is_root: bool
+            cat: Catalog,
+            _root_href: str,
+            is_root: bool,
+            parent: Optional[Catalog] = None,
         ) -> List[Callable[[], None]]:
             setter_funcs: List[Callable[[], None]] = []
 
             if not skip_unresolved:
                 cat.resolve_links()
 
+            # Abort as the intended parent is not the actual parent
+            # https://github.com/stac-utils/pystac/issues/1116
+            if parent is not None and cat.get_parent() != parent:
+                return setter_funcs
+
             new_self_href = _strategy.get_href(cat, _root_href, is_root)
             new_root = os.path.dirname(new_self_href)
 
             for link in cat.get_links():
                 if skip_unresolved and not link.is_resolved():
                     continue
                 elif link.rel == pystac.RelType.ITEM:
                     link.resolve_stac_object(root=self.get_root())
-                    setter_funcs.append(
-                        process_item(cast(pystac.Item, link.target), new_root)
+                    item_fn = process_item(
+                        cast(pystac.Item, link.target), new_root, cat
                     )
+                    if item_fn is not None:
+                        setter_funcs.append(item_fn)
                 elif link.rel == pystac.RelType.CHILD:
                     link.resolve_stac_object(root=self.get_root())
                     setter_funcs.extend(
                         process_catalog(
                             cast(Union[pystac.Catalog, pystac.Collection], link.target),
                             new_root,
                             is_root=False,
+                            parent=cat,
                         )
                     )
 
             def fn() -> None:
                 cat.set_self_href(new_self_href)
 
             setter_funcs.append(fn)
@@ -921,29 +1027,49 @@
         """
         for _, _, items in self.walk():
             # items is a generator, so we need to consume it to resolve the
             # items
             for item in items:
                 pass
 
-    def validate_all(self) -> None:
-        """Validates each catalog, collection contained within this catalog.
+    def validate_all(
+        self, max_items: Optional[int] = None, recursive: bool = True
+    ) -> int:
+        """Validates each catalog, collection, item contained within this catalog.
 
         Walks through the children and items of the catalog and validates each
         stac object.
 
+        Args:
+            max_items : The maximum number of STAC items to validate. Default
+                is None which means, validate them all.
+            recursive : Whether to validate catalog, collections, and items contained
+                within child objects.
+
+        Returns:
+            int : Number of STAC items validated.
+
         Raises:
             STACValidationError: Raises this error on any item that is invalid.
                 Will raise on the first invalid stac object encountered.
         """
+        n = 0
         self.validate()
         for child in self.get_children():
-            child.validate_all()
+            if recursive:
+                inner_max_items = None if max_items is None else max_items - n
+                n += child.validate_all(max_items=inner_max_items, recursive=True)
+            else:
+                child.validate()
         for item in self.get_items():
+            if max_items is not None and n >= max_items:
+                break
             item.validate()
+            n += 1
+        return n
 
     def _object_links(self) -> List[Union[str, pystac.RelType]]:
         return [
             pystac.RelType.CHILD,
             pystac.RelType.ITEM,
             *pystac.EXTENSION_HOOKS.get_extended_object_links(self),
         ]
@@ -1070,15 +1196,15 @@
         preserve_dict: bool = True,
     ) -> C:
         if migrate:
             info = identify_stac_object(d)
             d = migrate_to_latest(d, info)
 
         if not cls.matches_object_type(d):
-            raise STACTypeError(f"{d} does not represent a {cls.__name__} instance")
+            raise STACTypeError(d, cls)
 
         catalog_type = CatalogType.determine_type(d)
 
         if preserve_dict:
             d = deepcopy(d)
 
         id = d.pop("id")
@@ -1121,16 +1247,14 @@
     def from_file(
         cls: Type[C], href: str, stac_io: Optional[pystac.StacIO] = None
     ) -> C:
         if stac_io is None:
             stac_io = pystac.StacIO.default()
 
         result = super().from_file(href, stac_io)
-        if not isinstance(result, Catalog):
-            raise pystac.STACTypeError(f"{result} is not a {Catalog}.")
         result._stac_io = stac_io
 
         return result
 
     @classmethod
     def matches_object_type(cls, d: Dict[str, Any]) -> bool:
         return identify_stac_object_type(d) == STACObjectType.CATALOG
```

### Comparing `pystac-1.7.3/pystac/collection.py` & `pystac-1.8.0/pystac/collection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import warnings
 from copy import deepcopy
 from datetime import datetime
-from html import escape
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     Iterable,
     List,
     Optional,
@@ -17,29 +16,34 @@
     Union,
     cast,
 )
 
 from dateutil import tz
 
 import pystac
-from pystac import CatalogType, STACObjectType
+from pystac import CatalogType, STACError, STACObjectType
 from pystac.asset import Asset
 from pystac.catalog import Catalog
 from pystac.errors import DeprecatedWarning, ExtensionNotImplemented, STACTypeError
-from pystac.html.jinja_env import get_jinja_env
 from pystac.layout import HrefLayoutStrategy
 from pystac.link import Link
 from pystac.provider import Provider
 from pystac.serialization import (
     identify_stac_object,
     identify_stac_object_type,
     migrate_to_latest,
 )
 from pystac.summaries import Summaries
-from pystac.utils import datetime_to_str, str_to_datetime
+from pystac.utils import (
+    datetime_to_str,
+    is_absolute_href,
+    make_absolute_href,
+    make_relative_href,
+    str_to_datetime,
+)
 
 if TYPE_CHECKING:
     from pystac.item import Item
 
 C = TypeVar("C", bound="Collection")
 
 TemporalIntervals = Union[List[List[datetime]], List[List[Optional[datetime]]]]
@@ -82,18 +86,18 @@
             self.bboxes: List[List[float]] = [cast(List[float], bboxes)]
         else:
             self.bboxes = cast(List[List[float]], bboxes)
 
         self.extra_fields = extra_fields or {}
 
     def to_dict(self) -> Dict[str, Any]:
-        """Generate a dictionary representing the JSON of this SpatialExtent.
+        """Returns this spatial extent as a dictionary.
 
         Returns:
-            dict: A serialization of the SpatialExtent that can be written out as JSON.
+            dict: A serialization of the SpatialExtent.
         """
         d = {"bbox": self.bboxes, **self.extra_fields}
         return d
 
     def clone(self) -> SpatialExtent:
         """Clones this object.
 
@@ -208,18 +212,18 @@
             self.intervals = intervals
         else:
             self.intervals = intervals
 
         self.extra_fields = extra_fields or {}
 
     def to_dict(self) -> Dict[str, Any]:
-        """Generate a dictionary representing the JSON of this TemporalExtent.
+        """Returns this temporal extent as a dictionary.
 
         Returns:
-            dict: A serialization of the TemporalExtent that can be written out as JSON.
+            dict: A serialization of the TemporalExtent.
         """
         encoded_intervals: List[List[Optional[str]]] = []
         for i in self.intervals:
             start = None
             end = None
 
             if i[0] is not None:
@@ -307,18 +311,18 @@
         extra_fields: Optional[Dict[str, Any]] = None,
     ):
         self.spatial = spatial
         self.temporal = temporal
         self.extra_fields = extra_fields or {}
 
     def to_dict(self) -> Dict[str, Any]:
-        """Generate a dictionary representing the JSON of this Extent.
+        """Returns this extent as a dictionary.
 
         Returns:
-            dict: A serialization of the Extent that can be written out as JSON.
+            dict: A serialization of the Extent.
         """
         d = {
             "spatial": self.spatial.to_dict(),
             "temporal": self.temporal.to_dict(),
             **self.extra_fields,
         }
 
@@ -536,30 +540,24 @@
         if assets is not None:
             for k, asset in assets.items():
                 self.add_asset(k, asset)
 
     def __repr__(self) -> str:
         return "<Collection id={}>".format(self.id)
 
-    def _repr_html_(self) -> str:
-        jinja_env = get_jinja_env()
-        if jinja_env:
-            template = jinja_env.get_template("Collection.jinja2")
-            return str(template.render(catalog=self))
-        else:
-            return escape(repr(self))
-
     def add_item(
         self,
         item: Item,
         title: Optional[str] = None,
         strategy: Optional[HrefLayoutStrategy] = None,
-    ) -> None:
-        super().add_item(item, title, strategy)
+        set_parent: bool = True,
+    ) -> Link:
+        link = super().add_item(item, title, strategy, set_parent)
         item.set_collection(self)
+        return link
 
     def to_dict(
         self, include_self_link: bool = True, transform_hrefs: bool = True
     ) -> Dict[str, Any]:
         d = super().to_dict(
             include_self_link=include_self_link, transform_hrefs=transform_hrefs
         )
@@ -622,15 +620,15 @@
         from pystac.extensions.version import CollectionVersionExtension
 
         if migrate:
             info = identify_stac_object(d)
             d = migrate_to_latest(d, info)
 
         if not cls.matches_object_type(d):
-            raise STACTypeError(f"{d} does not represent a {cls.__name__} instance")
+            raise STACTypeError(d, cls)
 
         catalog_type = CatalogType.determine_type(d)
 
         if preserve_dict:
             d = deepcopy(d)
 
         id = d.pop("id")
@@ -690,14 +688,35 @@
                 )
             # Collection asset deprecation checks pending version extension support
         except ExtensionNotImplemented:
             pass
 
         return collection
 
+    def get_item(self, id: str, recursive: bool = False) -> Optional[Item]:
+        """Returns an item with a given ID.
+
+        Args:
+            id : The ID of the item to find.
+            recursive : If True, search this collection and all children for the
+                item; otherwise, only search the items of this collection. Defaults
+                to False.
+
+        Return:
+            Item or None: The item with the given ID, or None if not found.
+        """
+        try:
+            return next(self.get_items(id, recursive=recursive), None)
+        except TypeError as e:
+            if any("recursive" in arg for arg in e.args):
+                # For inherited classes that do not yet support recursive
+                # See https://github.com/stac-utils/pystac-client/issues/485
+                return super().get_item(id, recursive=recursive)
+            raise e
+
     def get_assets(
         self,
         media_type: Optional[Union[str, pystac.MediaType]] = None,
         role: Optional[str] = None,
     ) -> Dict[str, Asset]:
         """Get this collection's assets.
 
@@ -707,50 +726,93 @@
             role: If set, filter the assets such that only those with a matching
                 ``role`` are returned.
 
         Returns:
             Dict[str, Asset]: A dictionary of assets that match ``media_type``
             and/or ``role`` if set or else all of this collection's assets.
         """
-        if media_type is None and role is None:
-            return dict(self.assets.items())
-        assets = dict()
-        for key, asset in self.assets.items():
-            if (media_type is None or asset.media_type == media_type) and (
-                role is None or asset.has_role(role)
-            ):
-                assets[key] = asset
-        return assets
+        return {
+            k: deepcopy(v)
+            for k, v in self.assets.items()
+            if (media_type is None or v.media_type == media_type)
+            and (role is None or v.has_role(role))
+        }
 
     def add_asset(self, key: str, asset: Asset) -> None:
-        """Adds an Asset to this item.
+        """Adds an Asset to this collection.
 
         Args:
             key : The unique key of this asset.
             asset : The Asset to add.
         """
         asset.set_owner(self)
         self.assets[key] = asset
 
+    def delete_asset(self, key: str) -> None:
+        """Deletes the asset at the given key, and removes the asset's data
+        file from the local filesystem.
+
+        It is an error to attempt to delete an asset's file if it is on a
+        remote filesystem.
+
+        To delete the asset without removing the file, use
+        `del collection.assets["key"]`.
+
+        Args:
+            key: The unique key of this asset.
+        """
+        asset = self.assets[key]
+        asset.set_owner(self)
+        asset.delete()
+
+        del self.assets[key]
+
+    def make_asset_hrefs_relative(self) -> Collection:
+        """Modify each asset's HREF to be relative to this collection's self HREF.
+
+        Returns:
+            Collection: self
+        """
+        self_href = self.get_self_href()
+        for asset in self.assets.values():
+            if is_absolute_href(asset.href):
+                if self_href is None:
+                    raise STACError(
+                        "Cannot make asset HREFs relative " "if no self_href is set."
+                    )
+                asset.href = make_relative_href(asset.href, self_href)
+        return self
+
+    def make_asset_hrefs_absolute(self) -> Collection:
+        """Modify each asset's HREF to be absolute.
+
+        Any asset HREFs that are relative will be modified to absolute based on this
+        collection's self HREF.
+
+        Returns:
+            Collection: self
+        """
+        self_href = self.get_self_href()
+        for asset in self.assets.values():
+            if not is_absolute_href(asset.href):
+                if self_href is None:
+                    raise STACError(
+                        "Cannot make relative asset HREFs absolute "
+                        "if no self_href is set."
+                    )
+                asset.href = make_absolute_href(asset.href, self_href)
+        return self
+
     def update_extent_from_items(self) -> None:
         """
         Update datetime and bbox based on all items to a single bbox and time window.
         """
-        self.extent = Extent.from_items(self.get_all_items())
+        self.extent = Extent.from_items(self.get_items(recursive=True))
 
     def full_copy(
         self, root: Optional["Catalog"] = None, parent: Optional["Catalog"] = None
     ) -> Collection:
         return cast(Collection, super().full_copy(root, parent))
 
     @classmethod
-    def from_file(
-        cls: Type[C], href: str, stac_io: Optional[pystac.StacIO] = None
-    ) -> C:
-        result = super().from_file(href, stac_io)
-        if not isinstance(result, Collection):
-            raise pystac.STACTypeError(f"{result} is not a {Collection}.")
-        return result
-
-    @classmethod
     def matches_object_type(cls, d: Dict[str, Any]) -> bool:
         return identify_stac_object_type(d) == STACObjectType.COLLECTION
```

### Comparing `pystac-1.7.3/pystac/common_metadata.py` & `pystac-1.8.0/pystac/common_metadata.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.3/pystac/errors.py` & `pystac-1.8.0/pystac/errors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Optional, Union
+from typing import Any, Dict, Optional, Union
 
 
 class TemplateError(Exception):
     """Exception thrown when an error occurs during converting a template
     string into data for :class:`~pystac.layout.LayoutTemplate`
     """
 
@@ -20,15 +20,36 @@
 
 class STACTypeError(Exception):
     """A STACTypeError is raised when encountering a representation of
     a STAC entity that is not correct for the context; for example, if
     a Catalog JSON was read in as an Item.
     """
 
-    pass
+    def __init__(
+        self,
+        bad_dict: Dict[str, Any],
+        expected: type,
+        extra_message: Optional[str] = "",
+    ):
+        """
+        Construct an exception with an appropriate error message from bad_dict and the
+        expected that it didn't align with.
+
+        Args:
+            bad_dict: Dictionary that did not match the expected type
+            expected: The expected type.
+            extra_message: message that will be appended to the exception message.
+        """
+        message = (
+            f"JSON (id = {bad_dict.get('id', 'unknown')}) does not represent"
+            f" a {expected.__name__} instance."
+        )
+        if extra_message:
+            message += " " + extra_message
+        super().__init__(message)
 
 
 class DuplicateObjectKeyError(Exception):
     """Raised when deserializing a JSON object containing a duplicate key."""
 
     pass
 
@@ -70,14 +91,18 @@
     def __init__(
         self, obj: Union[str, Any], prop: str, msg: Optional[str] = None
     ) -> None:
         msg = msg or f"{repr(obj)} does not have required property {prop}"
         super().__init__(msg)
 
 
+class STACLocalValidationError(Exception):
+    """Schema not available locally"""
+
+
 class STACValidationError(Exception):
     """Represents a validation error. Thrown by validation calls if the STAC JSON
     is invalid.
 
     Args:
         source : Source of the exception. Type will be determined by the
             validation implementation. For the default JsonSchemaValidator this will a
```

### Comparing `pystac-1.7.3/pystac/extensions/base.py` & `pystac-1.8.0/pystac/extensions/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -109,14 +109,19 @@
     @classmethod
     @abstractmethod
     def get_schema_uri(cls) -> str:
         """Gets the schema URI associated with this extension."""
         raise NotImplementedError
 
     @classmethod
+    def get_schema_uris(cls) -> List[str]:
+        """Gets a list of schema URIs associated with this extension."""
+        return [cls.get_schema_uri()]
+
+    @classmethod
     def add_to(cls, obj: S) -> None:
         """Add the schema URI for this extension to the
         :attr:`~pystac.STACObject.stac_extensions` list for the given object, if it is
         not already present."""
         if obj.stac_extensions is None:
             obj.stac_extensions = [cls.get_schema_uri()]
         elif not cls.has_extension(obj):
@@ -131,27 +136,33 @@
                 uri for uri in obj.stac_extensions if uri != cls.get_schema_uri()
             ]
 
     @classmethod
     def has_extension(cls, obj: S) -> bool:
         """Check if the given object implements this extension by checking
         :attr:`pystac.STACObject.stac_extensions` for this extension's schema URI."""
-        return (
-            obj.stac_extensions is not None
-            and cls.get_schema_uri() in obj.stac_extensions
+        return obj.stac_extensions is not None and any(
+            uri in obj.stac_extensions for uri in cls.get_schema_uris()
         )
 
     @classmethod
     def validate_owner_has_extension(
-        cls, asset: pystac.Asset, add_if_missing: bool
+        cls,
+        asset: pystac.Asset,
+        add_if_missing: bool = False,
     ) -> None:
         """Given an :class:`~pystac.Asset`, checks if the asset's owner has this
         extension's schema URI in its :attr:`~pystac.STACObject.stac_extensions` list.
         If ``add_if_missing`` is ``True``, the schema URI will be added to the owner.
 
+        Args:
+            asset : The asset whose owner should be validated.
+            add_if_missing : Whether to add the schema URI to the owner if it is
+                not already present. Defaults to False.
+
         Raises:
             STACError : If ``add_if_missing`` is ``True`` and ``asset.owner`` is
                 ``None``.
         """
         if asset.owner is None:
             if add_if_missing:
                 raise pystac.STACError(
@@ -159,24 +170,32 @@
                     "Use Asset.set_owner or set add_if_missing=False."
                 )
             else:
                 return
         return cls.validate_has_extension(cast(S, asset.owner), add_if_missing)
 
     @classmethod
-    def validate_has_extension(cls, obj: S, add_if_missing: bool) -> None:
+    def validate_has_extension(cls, obj: S, add_if_missing: bool = False) -> None:
         """Given a :class:`~pystac.STACObject`, checks if the object has this
         extension's schema URI in its :attr:`~pystac.STACObject.stac_extensions` list.
         If ``add_if_missing`` is ``True``, the schema URI will be added to the object.
 
         Args:
             obj : The object to validate.
             add_if_missing : Whether to add the schema URI to the object if it is
-                not already present.
+                not already present. Defaults to False.
         """
         if add_if_missing:
             cls.add_to(obj)
 
         if not cls.has_extension(obj):
             raise pystac.ExtensionNotImplemented(
                 f"Could not find extension schema URI {cls.get_schema_uri()} in object."
             )
+
+    @classmethod
+    def _ext_error_message(cls, obj: Any) -> str:
+        contents = [f"{cls.__name__} does not apply to type '{type(obj).__name__}'"]
+        if hasattr(cls, "summaries") and isinstance(obj, pystac.Collection):
+            hint = f"Hint: Did you mean to use `{cls.__name__}.summaries` instead?"
+            contents.append(hint)
+        return ". ".join(contents)
```

### Comparing `pystac-1.7.3/pystac/extensions/datacube.py` & `pystac-1.8.0/pystac/extensions/datacube.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,26 +122,15 @@
             # from a temporal dimension. Just key off of type for now.
             # See https://github.com/stac-extensions/datacube/issues/5
             return TemporalDimension(d)
         else:
             return AdditionalDimension(d)
 
 
-class HorizontalSpatialDimension(Dimension):
-    @property
-    def axis(self) -> HorizontalSpatialDimensionAxis:
-        """Axis of the spatial dimension. Must be one of ``"x"`` or ``"y"``."""
-        return get_required(
-            self.properties.get(DIM_AXIS_PROP), "cube:dimension", DIM_AXIS_PROP
-        )
-
-    @axis.setter
-    def axis(self, v: HorizontalSpatialDimensionAxis) -> None:
-        self.properties[DIM_TYPE_PROP] = v
-
+class SpatialDimension(Dimension):
     @property
     def extent(self) -> List[float]:
         """Extent (lower and upper bounds) of the dimension as two-dimensional array.
         Open intervals with ``None`` are not allowed."""
         return get_required(
             self.properties.get(DIM_EXTENT_PROP), "cube:dimension", DIM_EXTENT_PROP
         )
@@ -190,101 +179,52 @@
     def reference_system(self, v: Optional[Union[str, float, Dict[str, Any]]]) -> None:
         if v is None:
             self.properties.pop(DIM_REF_SYS_PROP, None)
         else:
             self.properties[DIM_REF_SYS_PROP] = v
 
 
-class VerticalSpatialDimension(Dimension):
+class HorizontalSpatialDimension(SpatialDimension):
     @property
-    def axis(self) -> VerticalSpatialDimensionAxis:
-        """Axis of the spatial dimension. Always ``"z"``."""
+    def axis(self) -> HorizontalSpatialDimensionAxis:
+        """Axis of the spatial dimension. Must be one of ``"x"`` or ``"y"``."""
         return get_required(
             self.properties.get(DIM_AXIS_PROP), "cube:dimension", DIM_AXIS_PROP
         )
 
     @axis.setter
-    def axis(self, v: VerticalSpatialDimensionAxis) -> None:
-        self.properties[DIM_TYPE_PROP] = v
-
-    @property
-    def extent(self) -> Optional[List[Optional[float]]]:
-        """If the dimension consists of `ordinal
-        <https://en.wikipedia.org/wiki/Level_of_measurement#Ordinal_scale>`__ values,
-        the extent (lower and upper bounds) of the values as two-dimensional array. Use
-        null for open intervals."""
-        return self.properties.get(DIM_EXTENT_PROP)
-
-    @extent.setter
-    def extent(self, v: Optional[List[Optional[float]]]) -> None:
-        if v is None:
-            self.properties.pop(DIM_EXTENT_PROP, None)
-        else:
-            self.properties[DIM_EXTENT_PROP] = v
-
-    @property
-    def values(self) -> Optional[Union[List[float], List[str]]]:
-        """A set of all potential values, especially useful for `nominal
-        <https://en.wikipedia.org/wiki/Level_of_measurement#Nominal_level>`__ values."""
-
-        return self.properties.get(DIM_VALUES_PROP)
+    def axis(self, v: HorizontalSpatialDimensionAxis) -> None:
+        self.properties[DIM_AXIS_PROP] = v
 
-    @values.setter
-    def values(self, v: Optional[Union[List[float], List[str]]]) -> None:
-        if v is None:
-            self.properties.pop(DIM_VALUES_PROP, None)
-        else:
-            self.properties[DIM_VALUES_PROP] = v
 
+class VerticalSpatialDimension(SpatialDimension):
     @property
-    def step(self) -> Optional[float]:
-        """If the dimension consists of `interval
-        <https://en.wikipedia.org/wiki/Level_of_measurement#Interval_scale>`__ values,
-        the space between the values. Use null for irregularly spaced steps."""
-        return self.properties.get(DIM_STEP_PROP)
-
-    @step.setter
-    def step(self, v: Optional[float]) -> None:
-        self.properties[DIM_STEP_PROP] = v
+    def axis(self) -> VerticalSpatialDimensionAxis:
+        """Axis of the spatial dimension. Must be ``"z"``."""
+        return get_required(
+            self.properties.get(DIM_AXIS_PROP), "cube:dimension", DIM_AXIS_PROP
+        )
 
-    def clear_step(self) -> None:
-        """Setting step to None sets it to the null value,
-        which means irregularly spaced steps. Use clear_step
-        to remove it from the properties."""
-        self.properties.pop(DIM_STEP_PROP, None)
+    @axis.setter
+    def axis(self, v: VerticalSpatialDimensionAxis) -> None:
+        self.properties[DIM_AXIS_PROP] = v
 
     @property
     def unit(self) -> Optional[str]:
         """The unit of measurement for the data, preferably compliant to `UDUNITS-2
         <https://ncics.org/portfolio/other-resources/udunits2/>`__ units (singular)."""
         return self.properties.get(DIM_UNIT_PROP)
 
     @unit.setter
     def unit(self, v: Optional[str]) -> None:
         if v is None:
             self.properties.pop(DIM_UNIT_PROP, None)
         else:
             self.properties[DIM_UNIT_PROP] = v
 
-    @property
-    def reference_system(self) -> Optional[Union[str, float, Dict[str, Any]]]:
-        """The spatial reference system for the data, specified as `numerical EPSG code
-        <http://www.epsg-registry.org/>`__, `WKT2 (ISO 19162) string
-        <http://docs.opengeospatial.org/is/18-010r7/18-010r7.html>`__ or `PROJJSON
-        object <https://proj.org/specifications/projjson.html>`__.
-        Defaults to EPSG code 4326."""
-        return self.properties.get(DIM_REF_SYS_PROP)
-
-    @reference_system.setter
-    def reference_system(self, v: Optional[Union[str, float, Dict[str, Any]]]) -> None:
-        if v is None:
-            self.properties.pop(DIM_REF_SYS_PROP, None)
-        else:
-            self.properties[DIM_REF_SYS_PROP] = v
-
 
 class TemporalDimension(Dimension):
     @property
     def extent(self) -> Optional[List[Optional[str]]]:
         """Extent (lower and upper bounds) of the dimension as two-dimensional array.
         The dates and/or times must be strings compliant to `ISO 8601
         <https://en.wikipedia.org/wiki/ISO_8601>`__. ``None`` is allowed for open date
@@ -530,41 +470,45 @@
     """
 
     def apply(
         self,
         dimensions: Dict[str, Dimension],
         variables: Optional[Dict[str, Variable]] = None,
     ) -> None:
-        """Applies label extension properties to the extended
+        """Applies Datacube Extension properties to the extended
         :class:`~pystac.Collection`, :class:`~pystac.Item` or :class:`~pystac.Asset`.
 
         Args:
-            dimensions : Dictionary mapping dimension name to a :class:`Dimension`
-                object.
+            dimensions : Dictionary mapping dimension name to :class:`Dimension`
+                objects.
             variables : Dictionary mapping variable name to a :class:`Variable`
                 object.
         """
         self.dimensions = dimensions
         self.variables = variables
 
     @property
     def dimensions(self) -> Dict[str, Dimension]:
-        """Dictionary mapping dimension name to a :class:`Dimension` object."""
+        """A dictionary where each key is the name of a dimension and each
+        value is a :class:`~Dimension` object.
+        """
         result = get_required(
             self._get_property(DIMENSIONS_PROP, Dict[str, Any]), self, DIMENSIONS_PROP
         )
         return {k: Dimension.from_dict(v) for k, v in result.items()}
 
     @dimensions.setter
     def dimensions(self, v: Dict[str, Dimension]) -> None:
         self._set_property(DIMENSIONS_PROP, {k: dim.to_dict() for k, dim in v.items()})
 
     @property
     def variables(self) -> Optional[Dict[str, Variable]]:
-        """Dictionary mapping variable name to a :class:`Variable` object."""
+        """A dictionary where each key is the name of a variable and each
+        value is a :class:`~Variable` object.
+        """
         result = self._get_property(VARIABLES_PROP, Dict[str, Any])
 
         if result is None:
             return None
         return {k: Variable.from_dict(v) for k, v in result.items()}
 
     @variables.setter
@@ -598,17 +542,15 @@
         if isinstance(obj, pystac.Item):
             cls.validate_has_extension(obj, add_if_missing)
             return cast(DatacubeExtension[T], ItemDatacubeExtension(obj))
         elif isinstance(obj, pystac.Asset):
             cls.validate_owner_has_extension(obj, add_if_missing)
             return cast(DatacubeExtension[T], AssetDatacubeExtension(obj))
         else:
-            raise pystac.ExtensionTypeError(
-                f"Datacube extension does not apply to type '{type(obj).__name__}'"
-            )
+            raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
 
 class CollectionDatacubeExtension(DatacubeExtension[pystac.Collection]):
     """A concrete implementation of :class:`DatacubeExtension` on an
     :class:`~pystac.Collection` that extends the properties of the Item to include
     properties defined in the :stac-ext:`Datacube Extension <datacube>`.
```

### Comparing `pystac-1.7.3/pystac/extensions/eo.py` & `pystac-1.8.0/pystac/extensions/eo.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,20 +25,33 @@
 from pystac.extensions.hooks import ExtensionHooks
 from pystac.serialization.identify import STACJSONDescription, STACVersionID
 from pystac.summaries import RangeSummary
 from pystac.utils import get_required, map_opt
 
 T = TypeVar("T", pystac.Item, pystac.Asset)
 
-SCHEMA_URI: str = "https://stac-extensions.github.io/eo/v1.0.0/schema.json"
+SCHEMA_URI: str = "https://stac-extensions.github.io/eo/v1.1.0/schema.json"
+SCHEMA_URIS: List[str] = [
+    "https://stac-extensions.github.io/eo/v1.0.0/schema.json",
+    SCHEMA_URI,
+]
 PREFIX: str = "eo:"
 
 # Field names
 BANDS_PROP: str = PREFIX + "bands"
 CLOUD_COVER_PROP: str = PREFIX + "cloud_cover"
+SNOW_COVER_PROP: str = PREFIX + "snow_cover"
+
+
+def validated_percentage(v: Optional[float]) -> Optional[float]:
+    if v is not None and not isinstance(v, (float, int)) or isinstance(v, bool):
+        raise ValueError(f"Invalid percentage: {v} must be number")
+    if v is not None and not 0 <= v <= 100:
+        raise ValueError(f"Invalid percentage: {v} must be between 0 and 100")
+    return v
 
 
 class Band:
     """Represents Band information attached to an Item that implements the eo extension.
 
     Use :meth:`Band.create` to create a new Band.
     """
@@ -213,18 +226,18 @@
         else:
             self.properties.pop("solar_illumination", None)
 
     def __repr__(self) -> str:
         return "<Band name={}>".format(self.name)
 
     def to_dict(self) -> Dict[str, Any]:
-        """Returns the dictionary representing the JSON of this Band.
+        """Returns this band as a dictionary.
 
         Returns:
-            dict: The wrapped dict of the Band that can be written out as JSON.
+            dict: The serialization of this Band.
         """
         return self.properties
 
     @staticmethod
     def band_range(common_name: str) -> Optional[Tuple[float, float]]:
         """Gets the band range for a common band name.
 
@@ -292,28 +305,35 @@
     .. code-block:: python
 
        >>> item: pystac.Item = ...
        >>> eo_ext = EOExtension.ext(item)
     """
 
     def apply(
-        self, bands: Optional[List[Band]] = None, cloud_cover: Optional[float] = None
+        self,
+        bands: Optional[List[Band]] = None,
+        cloud_cover: Optional[float] = None,
+        snow_cover: Optional[float] = None,
     ) -> None:
         """Applies Electro-Optical Extension properties to the extended
         :class:`~pystac.Item` or :class:`~pystac.Asset`.
 
         Args:
             bands : A list of available bands where each item is a :class:`~Band`
                 object. If given, requires at least one band.
             cloud_cover : The estimate of cloud cover as a percentage
                 (0-100) of the entire scene. If not available the field should not
                 be provided.
+            snow_cover : The estimate of snow cover as a percentage
+                (0-100) of the entire scene. If not available the field should not
+                be provided.
         """
         self.bands = bands
-        self.cloud_cover = cloud_cover
+        self.cloud_cover = validated_percentage(cloud_cover)
+        self.snow_cover = validated_percentage(snow_cover)
 
     @property
     def bands(self) -> Optional[List[Band]]:
         """Gets or sets a list of available bands where each item is a :class:`~Band`
         object (or ``None`` if no bands have been set). If not available the field
         should not be provided.
         """
@@ -339,21 +359,39 @@
         Returns:
             float or None
         """
         return self._get_property(CLOUD_COVER_PROP, float)
 
     @cloud_cover.setter
     def cloud_cover(self, v: Optional[float]) -> None:
-        self._set_property(CLOUD_COVER_PROP, v)
+        self._set_property(CLOUD_COVER_PROP, validated_percentage(v), pop_if_none=True)
+
+    @property
+    def snow_cover(self) -> Optional[float]:
+        """Get or sets the estimate of snow cover as a percentage
+        (0-100) of the entire scene. If not available the field should not be provided.
+
+        Returns:
+            float or None
+        """
+        return self._get_property(SNOW_COVER_PROP, float)
+
+    @snow_cover.setter
+    def snow_cover(self, v: Optional[float]) -> None:
+        self._set_property(SNOW_COVER_PROP, validated_percentage(v), pop_if_none=True)
 
     @classmethod
     def get_schema_uri(cls) -> str:
         return SCHEMA_URI
 
     @classmethod
+    def get_schema_uris(cls) -> List[str]:
+        return SCHEMA_URIS
+
+    @classmethod
     def ext(cls, obj: T, add_if_missing: bool = False) -> EOExtension[T]:
         """Extends the given STAC Object with properties from the
         :stac-ext:`Electro-Optical Extension <eo>`.
 
         This extension can be applied to instances of :class:`~pystac.Item` or
         :class:`~pystac.Asset`.
 
@@ -364,17 +402,15 @@
         if isinstance(obj, pystac.Item):
             cls.validate_has_extension(obj, add_if_missing)
             return cast(EOExtension[T], ItemEOExtension(obj))
         elif isinstance(obj, pystac.Asset):
             cls.validate_owner_has_extension(obj, add_if_missing)
             return cast(EOExtension[T], AssetEOExtension(obj))
         else:
-            raise pystac.ExtensionTypeError(
-                f"EO extension does not apply to type '{type(obj).__name__}'"
-            )
+            raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
     @classmethod
     def summaries(
         cls, obj: pystac.Collection, add_if_missing: bool = False
     ) -> SummariesEOExtension:
         """Returns the extended summaries object for the given collection."""
         cls.validate_has_extension(obj, add_if_missing)
@@ -417,14 +453,43 @@
             if any(asset_bands):
                 bands = asset_bands
 
         if bands is not None:
             return [Band(b) for b in bands]
         return None
 
+    def get_assets(
+        self,
+        name: Optional[str] = None,
+        common_name: Optional[str] = None,
+    ) -> Dict[str, pystac.Asset]:
+        """Get the item's assets where eo:bands are defined.
+
+        Args:
+            name: If set, filter the assets such that only those with a
+                matching ``eo:band.name`` are returned.
+            common_name: If set, filter the assets such that only those with a matching
+                ``eo:band.common_name`` are returned.
+
+        Returns:
+            Dict[str, Asset]: A dictionary of assets that match ``name``
+                and/or ``common_name`` if set or else all of this item's assets were
+                eo:bands are defined.
+        """
+        kwargs = {"name": name, "common_name": common_name}
+        return {
+            key: asset
+            for key, asset in self.item.get_assets().items()
+            if BANDS_PROP in asset.extra_fields
+            and all(
+                v is None or any(v == b.get(k) for b in asset.extra_fields[BANDS_PROP])
+                for k, v in kwargs.items()
+            )
+        }
+
     def __repr__(self) -> str:
         return "<ItemEOExtension Item id={}>".format(self.item.id)
 
 
 class AssetEOExtension(EOExtension[pystac.Asset]):
     """A concrete implementation of :class:`EOExtension` on an :class:`~pystac.Asset`
     that extends the Asset fields to include properties defined in the
@@ -492,18 +557,32 @@
         """
         return self.summaries.get_range(CLOUD_COVER_PROP)
 
     @cloud_cover.setter
     def cloud_cover(self, v: Optional[RangeSummary[float]]) -> None:
         self._set_summary(CLOUD_COVER_PROP, v)
 
+    @property
+    def snow_cover(self) -> Optional[RangeSummary[float]]:
+        """Get or sets the summary of :attr:`EOExtension.snow_cover` values
+        for this Collection.
+        """
+        return self.summaries.get_range(SNOW_COVER_PROP)
+
+    @snow_cover.setter
+    def snow_cover(self, v: Optional[RangeSummary[float]]) -> None:
+        self._set_summary(SNOW_COVER_PROP, v)
+
 
 class EOExtensionHooks(ExtensionHooks):
     schema_uri: str = SCHEMA_URI
-    prev_extension_ids = {"eo"}
+    prev_extension_ids = {
+        "eo",
+        *[uri for uri in SCHEMA_URIS if uri != SCHEMA_URI],
+    }
     stac_object_types = {pystac.STACObjectType.ITEM}
 
     def migrate(
         self, obj: Dict[str, Any], version: STACVersionID, info: STACJSONDescription
     ) -> None:
         if version < "0.9":
             # Some eo fields became common_metadata
```

### Comparing `pystac-1.7.3/pystac/extensions/file.py` & `pystac-1.8.0/pystac/extensions/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,17 +223,15 @@
 
         This extension can be applied to instances of :class:`~pystac.Asset`.
         """
         if isinstance(obj, pystac.Asset):
             cls.validate_owner_has_extension(obj, add_if_missing)
             return cls(obj)
         else:
-            raise pystac.ExtensionTypeError(
-                f"File Info extension does not apply to type '{type(obj).__name__}'"
-            )
+            raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
 
 class FileExtensionHooks(ExtensionHooks):
     schema_uri: str = SCHEMA_URI
     prev_extension_ids = {"file"}
     stac_object_types = {pystac.STACObjectType.ITEM}
```

### Comparing `pystac-1.7.3/pystac/extensions/grid.py` & `pystac-1.8.0/pystac/extensions/grid.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """Implements the :stac-ext:`Grid Extension <grid>`."""
 
 from __future__ import annotations
 
 import re
-from typing import Any, Dict, Optional, Pattern, Set, Union
+from typing import Any, Dict, List, Optional, Pattern, Set, Union
 
 import pystac
 from pystac.extensions.base import ExtensionManagementMixin, PropertiesExtension
 from pystac.extensions.hooks import ExtensionHooks
 
 SCHEMA_URI: str = "https://stac-extensions.github.io/grid/v1.1.0/schema.json"
+SCHEMA_URIS: List[str] = [
+    "https://stac-extensions.github.io/grid/v1.0.0/schema.json",
+    SCHEMA_URI,
+]
 PREFIX: str = "grid:"
 
 # Field names
 CODE_PROP: str = PREFIX + "code"  # required
 
 CODE_REGEX: str = r"[A-Z0-9]+-[-_.A-Za-z0-9]+"
 CODE_PATTERN: Pattern[str] = re.compile(CODE_REGEX)
@@ -77,33 +81,35 @@
         self._set_property(CODE_PROP, validated_code(v), pop_if_none=False)
 
     @classmethod
     def get_schema_uri(cls) -> str:
         return SCHEMA_URI
 
     @classmethod
+    def get_schema_uris(cls) -> List[str]:
+        return SCHEMA_URIS
+
+    @classmethod
     def ext(cls, obj: pystac.Item, add_if_missing: bool = False) -> GridExtension:
         """Extends the given STAC Object with properties from the :stac-ext:`Grid
         Extension <grid>`.
 
         This extension can be applied to instances of :class:`~pystac.Item`.
 
         Raises:
 
             pystac.ExtensionTypeError : If an invalid object type is passed.
         """
         if isinstance(obj, pystac.Item):
             cls.validate_has_extension(obj, add_if_missing)
             return GridExtension(obj)
         else:
-            raise pystac.ExtensionTypeError(
-                f"Grid Extension does not apply to type '{type(obj).__name__}'"
-            )
+            raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
 
 class GridExtensionHooks(ExtensionHooks):
     schema_uri: str = SCHEMA_URI
-    prev_extension_ids: Set[str] = set()
+    prev_extension_ids: Set[str] = {*[uri for uri in SCHEMA_URIS if uri != SCHEMA_URI]}
     stac_object_types = {pystac.STACObjectType.ITEM}
 
 
-Grid_EXTENSION_HOOKS: ExtensionHooks = GridExtensionHooks()
+GRID_EXTENSION_HOOKS: ExtensionHooks = GridExtensionHooks()
```

### Comparing `pystac-1.7.3/pystac/extensions/hooks.py` & `pystac-1.8.0/pystac/extensions/hooks.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.3/pystac/extensions/item_assets.py` & `pystac-1.8.0/pystac/extensions/item_assets.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,16 +26,21 @@
     Items for this Collection.
 
     See the :stac-ext:`Asset Object <item-assets#asset-object>` for details.
     """
 
     properties: Dict[str, Any]
 
-    def __init__(self, properties: Dict[str, Any]) -> None:
+    owner: Optional[pystac.Collection]
+
+    def __init__(
+        self, properties: Dict[str, Any], owner: Optional[pystac.Collection] = None
+    ) -> None:
         self.properties = properties
+        self.owner = owner
 
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, AssetDefinition):
             return NotImplemented
         return self.to_dict() == o.to_dict()
 
     @classmethod
@@ -103,14 +108,25 @@
         """
         if extra_fields:
             self.properties.update(extra_fields)
         self.title = title
         self.description = description
         self.media_type = media_type
         self.roles = roles
+        self.owner = None
+
+    def set_owner(self, obj: pystac.Collection) -> None:
+        """Sets the owning item of this AssetDefinition.
+
+        The owning item will be used to resolve relative HREFs of this asset.
+
+        Args:
+            obj: The Collection that owns this asset.
+        """
+        self.owner = obj
 
     @property
     def title(self) -> Optional[str]:
         """Gets or sets the displayed title for clients and users."""
         return self.properties.get(ASSET_TITLE_PROP)
 
     @title.setter
@@ -159,15 +175,15 @@
     def roles(self, v: Optional[List[str]]) -> None:
         if v is None:
             self.properties.pop(ASSET_ROLES_PROP, None)
         else:
             self.properties[ASSET_ROLES_PROP] = v
 
     def to_dict(self) -> Dict[str, Any]:
-        """Returns a JSON-like dictionary representing this ``AssetDefinition``."""
+        """Returns a dictionary representing this ``AssetDefinition``."""
         return deepcopy(self.properties)
 
     def create_asset(self, href: str) -> pystac.Asset:
         """Creates a new :class:`~pystac.Asset` instance using the fields from this
         ``AssetDefinition`` and the given ``href``."""
         return pystac.Asset(
             href=href,
@@ -198,15 +214,15 @@
     @property
     def item_assets(self) -> Dict[str, AssetDefinition]:
         """Gets or sets a dictionary of assets that can be found in member Items. Maps
         the asset key to an :class:`AssetDefinition` instance."""
         result: Dict[str, Any] = get_required(
             self.collection.extra_fields.get(ITEM_ASSETS_PROP), self, ITEM_ASSETS_PROP
         )
-        return {k: AssetDefinition(v) for k, v in result.items()}
+        return {k: AssetDefinition(v, self.collection) for k, v in result.items()}
 
     @item_assets.setter
     def item_assets(self, v: Dict[str, AssetDefinition]) -> None:
         self.collection.extra_fields[ITEM_ASSETS_PROP] = {
             k: asset_def.properties for k, asset_def in v.items()
         }
 
@@ -228,17 +244,15 @@
 
             pystac.ExtensionTypeError : If an invalid object type is passed.
         """
         if isinstance(obj, pystac.Collection):
             cls.validate_has_extension(obj, add_if_missing)
             return cls(obj)
         else:
-            raise pystac.ExtensionTypeError(
-                f"Item Assets extension does not apply to type '{type(obj).__name__}'"
-            )
+            raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
 
 class ItemAssetsExtensionHooks(ExtensionHooks):
     schema_uri: str = SCHEMA_URI
     prev_extension_ids = {"asset", "item-assets"}
     stac_object_types = {pystac.STACObjectType.COLLECTION}
```

### Comparing `pystac-1.7.3/pystac/extensions/label.py` & `pystac-1.8.0/pystac/extensions/label.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 import pystac
 from pystac.extensions.base import ExtensionManagementMixin, SummariesExtension
 from pystac.extensions.hooks import ExtensionHooks
 from pystac.serialization.identify import STACJSONDescription, STACVersionID
 from pystac.utils import StringEnum, get_required, map_opt
 
 SCHEMA_URI = "https://stac-extensions.github.io/label/v1.0.1/schema.json"
-
+SCHEMA_URIS = [
+    "https://stac-extensions.github.io/label/v1.0.0/schema.json",
+    SCHEMA_URI,
+]
 PREFIX = "label:"
 
 PROPERTIES_PROP = PREFIX + "properties"
 CLASSES_PROP = PREFIX + "classes"
 DESCRIPTION_PROP = PREFIX + "description"
 TYPE_PROP = PREFIX + "type"
 TASKS_PROP = PREFIX + "tasks"
@@ -137,15 +140,15 @@
 
         if not isinstance(o, dict):
             return NotImplemented
 
         return self.to_dict() == o
 
     def to_dict(self) -> Dict[str, Any]:
-        """Returns the dictionary representing the JSON of this instance."""
+        """Returns this label classes object as a dictionary."""
         return self.properties
 
 
 class LabelCount:
     """Contains counts for categorical data.
 
     Use :meth:`LabelCount.create` to create a new instance.
@@ -193,15 +196,15 @@
         return get_required(self.properties.get("count"), self, "count")
 
     @count.setter
     def count(self, v: int) -> None:
         self.properties["count"] = v
 
     def to_dict(self) -> Dict[str, Any]:
-        """Returns the dictionary representing the JSON of this instance."""
+        """Returns this label count object as a dictionary."""
         return self.properties
 
     def __eq__(self, o: object) -> bool:
         if isinstance(o, LabelCount):
             o = o.to_dict()
 
         if not isinstance(o, dict):
@@ -258,15 +261,15 @@
         return get_required(self.properties.get("value"), self, "value")
 
     @value.setter
     def value(self, v: float) -> None:
         self.properties["value"] = v
 
     def to_dict(self) -> Dict[str, Any]:
-        """Returns the dictionary representing the JSON of this LabelStatistics."""
+        """Returns this label statistics object as a dictionary."""
         return self.properties
 
     def __eq__(self, o: object) -> bool:
         if isinstance(o, LabelStatistics):
             o = o.to_dict()
 
         if not isinstance(o, dict):
@@ -413,15 +416,15 @@
 
                 add_counts(self.counts)
                 add_counts(other.counts)
                 new_counts = [LabelCount.create(k, v) for k, v in count_by_prop.items()]
         return LabelOverview.create(self.property_key, counts=new_counts)
 
     def to_dict(self) -> Dict[str, Any]:
-        """Returns the dictionary representing the JSON of this LabelOverview."""
+        """Returns this label overview as a dictionary."""
         return self.properties
 
     def __eq__(self, o: object) -> bool:
         if isinstance(o, LabelOverview):
             o = o.to_dict()
 
         if not isinstance(o, dict):
@@ -688,27 +691,29 @@
         )
 
     @classmethod
     def get_schema_uri(cls) -> str:
         return SCHEMA_URI
 
     @classmethod
+    def get_schema_uris(cls) -> List[str]:
+        return SCHEMA_URIS
+
+    @classmethod
     def ext(cls, obj: pystac.Item, add_if_missing: bool = False) -> LabelExtension:
         """Extends the given STAC Object with properties from the :stac-ext:`Label
         Extension <label>`.
 
         This extension can be applied to instances of :class:`~pystac.Item`.
         """
         if isinstance(obj, pystac.Item):
             cls.validate_has_extension(obj, add_if_missing)
             return cls(obj)
         else:
-            raise pystac.ExtensionTypeError(
-                f"Label extension does not apply to type '{type(obj).__name__}'"
-            )
+            raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
     @classmethod
     def summaries(
         cls, obj: pystac.Collection, add_if_missing: bool = False
     ) -> SummariesLabelExtension:
         """Returns the extended summaries object for the given collection."""
         cls.validate_has_extension(obj, add_if_missing)
@@ -787,15 +792,15 @@
         self._set_summary(METHODS_PROP, v)
 
 
 class LabelExtensionHooks(ExtensionHooks):
     schema_uri: str = SCHEMA_URI
     prev_extension_ids = {
         "label",
-        "https://stac-extensions.github.io/label/v1.0.0/schema.json",
+        *[uri for uri in SCHEMA_URIS if uri != SCHEMA_URI],
     }
     stac_object_types = {pystac.STACObjectType.ITEM}
 
     def get_object_links(
         self, so: pystac.STACObject
     ) -> Optional[List[Union[str, pystac.RelType]]]:
         if isinstance(so, pystac.Item):
```

### Comparing `pystac-1.7.3/pystac/extensions/pointcloud.py` & `pystac-1.8.0/pystac/extensions/pointcloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         return "<Schema name={} size={} type={}>".format(
             self.properties.get("name"),
             self.properties.get("size"),
             self.properties.get("type"),
         )
 
     def to_dict(self) -> Dict[str, Any]:
-        """Returns a JSON-like dictionary representing this ``Schema``."""
+        """Returns this schema as a dictionary."""
         return self.properties
 
 
 class Statistic:
     """Defines a single statistic for Pointcloud channel or dimension
 
     Use :meth:`Statistic.create` to create a new instance of
@@ -305,15 +305,15 @@
         else:
             self.properties.pop("variance", None)
 
     def __repr__(self) -> str:
         return "<Statistic statistics={}>".format(str(self.properties))
 
     def to_dict(self) -> Dict[str, Any]:
-        """Returns a JSON-like dictionary representing this ``Statistic``."""
+        """Returns this statistic as a dictionary."""
         return self.properties
 
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, Statistic):
             return NotImplemented
         return self.to_dict() == o.to_dict()
 
@@ -454,17 +454,15 @@
             if obj.owner is not None and not isinstance(obj.owner, pystac.Item):
                 raise pystac.ExtensionTypeError(
                     "Pointcloud extension does not apply to Collection Assets."
                 )
             cls.validate_owner_has_extension(obj, add_if_missing)
             return cast(PointcloudExtension[T], AssetPointcloudExtension(obj))
         else:
-            raise pystac.ExtensionTypeError(
-                f"Pointcloud extension does not apply to type '{type(obj).__name__}'"
-            )
+            raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
     @classmethod
     def summaries(
         cls, obj: pystac.Collection, add_if_missing: bool = False
     ) -> SummariesPointcloudExtension:
         cls.validate_has_extension(obj, add_if_missing)
         return SummariesPointcloudExtension(obj)
```

### Comparing `pystac-1.7.3/pystac/extensions/projection.py` & `pystac-1.8.0/pystac/extensions/projection.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,14 +260,18 @@
         self._set_property(TRANSFORM_PROP, v)
 
     @classmethod
     def get_schema_uri(cls) -> str:
         return SCHEMA_URI
 
     @classmethod
+    def get_schema_uris(cls) -> List[str]:
+        return SCHEMA_URIS
+
+    @classmethod
     def ext(cls, obj: T, add_if_missing: bool = False) -> ProjectionExtension[T]:
         """Extends the given STAC Object with properties from the :stac-ext:`Projection
         Extension <projection>`.
 
         This extension can be applied to instances of :class:`~pystac.Item` or
         :class:`~pystac.Asset`.
 
@@ -278,35 +282,24 @@
         if isinstance(obj, pystac.Item):
             cls.validate_has_extension(obj, add_if_missing)
             return cast(ProjectionExtension[T], ItemProjectionExtension(obj))
         elif isinstance(obj, pystac.Asset):
             cls.validate_owner_has_extension(obj, add_if_missing)
             return cast(ProjectionExtension[T], AssetProjectionExtension(obj))
         else:
-            raise pystac.ExtensionTypeError(
-                f"Projection extension does not apply to type '{type(obj).__name__}'"
-            )
+            raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
     @classmethod
     def summaries(
         cls, obj: pystac.Collection, add_if_missing: bool = False
     ) -> SummariesProjectionExtension:
         """Returns the extended summaries object for the given collection."""
         cls.validate_has_extension(obj, add_if_missing)
         return SummariesProjectionExtension(obj)
 
-    @classmethod
-    def has_extension(cls, obj: Union[pystac.Item, pystac.Collection]) -> bool:
-        if isinstance(obj, pystac.Item) or isinstance(obj, pystac.Collection):
-            return obj.stac_extensions is not None and any(
-                uri in obj.stac_extensions for uri in SCHEMA_URIS
-            )
-        else:
-            return False
-
 
 class ItemProjectionExtension(ProjectionExtension[pystac.Item]):
     """A concrete implementation of :class:`ProjectionExtension` on an
     :class:`~pystac.Item` that extends the properties of the Item to include properties
     defined in the :stac-ext:`Projection Extension <projection>`.
 
     This class should generally not be instantiated directly. Instead, call
@@ -372,12 +365,16 @@
     @epsg.setter
     def epsg(self, v: Optional[List[int]]) -> None:
         self._set_summary(EPSG_PROP, v)
 
 
 class ProjectionExtensionHooks(ExtensionHooks):
     schema_uri: str = SCHEMA_URI
-    prev_extension_ids = {"proj", "projection"}
+    prev_extension_ids = {
+        "proj",
+        "projection",
+        *[uri for uri in SCHEMA_URIS if uri != SCHEMA_URI],
+    }
     stac_object_types = {pystac.STACObjectType.ITEM}
 
 
 PROJECTION_EXTENSION_HOOKS: ExtensionHooks = ProjectionExtensionHooks()
```

### Comparing `pystac-1.7.3/pystac/extensions/raster.py` & `pystac-1.8.0/pystac/extensions/raster.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,41 @@
 """Implements the :stac-ext:`Raster Extension <raster>`."""
 
 from __future__ import annotations
 
-from typing import Any, Dict, Iterable, List, Optional, Union
+from typing import (
+    Any,
+    Dict,
+    Generic,
+    Iterable,
+    List,
+    Optional,
+    Set,
+    TypeVar,
+    Union,
+    cast,
+)
 
 import pystac
+import pystac.extensions.item_assets as item_assets
 from pystac.extensions.base import (
     ExtensionManagementMixin,
     PropertiesExtension,
     SummariesExtension,
 )
+from pystac.extensions.hooks import ExtensionHooks
 from pystac.utils import StringEnum, get_opt, get_required, map_opt
 
-SCHEMA_URI = "https://stac-extensions.github.io/raster/v1.1.0/schema.json"
+T = TypeVar("T", pystac.Asset, item_assets.AssetDefinition)
 
+SCHEMA_URI = "https://stac-extensions.github.io/raster/v1.1.0/schema.json"
+SCHEMA_URIS = [
+    "https://stac-extensions.github.io/raster/v1.0.0/schema.json",
+    SCHEMA_URI,
+]
 BANDS_PROP = "raster:bands"
 
 
 class Sampling(StringEnum):
     AREA = "area"
     POINT = "point"
 
@@ -188,18 +206,18 @@
     def valid_percent(self, v: Optional[float]) -> None:
         if v is not None:
             self.properties["valid_percent"] = v
         else:
             self.properties.pop("valid_percent", None)
 
     def to_dict(self) -> Dict[str, Any]:
-        """Returns the dictionary representing the JSON of those Statistics.
+        """Returns these statistics as a dictionary.
 
         Returns:
-            dict: The wrapped dict of the Statistics that can be written out as JSON.
+            dict: The serialization of the Statistics.
         """
         return self.properties
 
     @staticmethod
     def from_dict(d: Dict[str, Any]) -> Statistics:
         """Constructs an Statistics from a dict.
 
@@ -324,18 +342,18 @@
         return get_required(self.properties.get("buckets"), self, "buckets")
 
     @buckets.setter
     def buckets(self, v: List[int]) -> None:
         self.properties["buckets"] = v
 
     def to_dict(self) -> Dict[str, Any]:
-        """Returns the dictionary representing the JSON of this histogram.
+        """Returns this histogram as a dictionary.
 
         Returns:
-            dict: The wrapped dict of the Histogram that can be written out as JSON.
+            dict: The serialization of the Histogram.
         """
         return self.properties
 
     @staticmethod
     def from_dict(d: Dict[str, Any]) -> Histogram:
         """Constructs an Histogram from a dict.
 
@@ -627,55 +645,44 @@
         else:
             self.properties.pop("histogram", None)
 
     def __repr__(self) -> str:
         return "<Raster Band>"
 
     def to_dict(self) -> Dict[str, Any]:
-        """Returns the dictionary representing the JSON of this Band.
+        """Returns this band as a dictionary.
 
         Returns:
-            dict: The wrapped dict of the Band that can be written out as JSON.
+            dict: The serialization of the Band.
         """
         return self.properties
 
 
 class RasterExtension(
-    PropertiesExtension, ExtensionManagementMixin[Union[pystac.Item, pystac.Collection]]
+    Generic[T],
+    PropertiesExtension,
+    ExtensionManagementMixin[Union[pystac.Item, pystac.Collection]],
 ):
     """An abstract class that can be used to extend the properties of an
-    :class:`~pystac.Item` or :class:`~pystac.Asset` with properties from
+    :class:`~pystac.Item`, :class:`~pystac.Asset`, or
+    :class:`~pystac.extension.item_assets.AssetDefinition` with properties from
     the :stac-ext:`Raster Extension <raster>`. This class is generic over
     the type of STAC Object to be extended (e.g. :class:`~pystac.Item`,
     :class:`~pystac.Asset`).
 
     This class will generally not be used directly. Instead, use the concrete
     implementation associated with the STAC Object you want to extend (e.g.
-    :class:`~ItemRasterExtension` to extend an :class:`~pystac.Item`).
+    :class:`~ItemRasterExtension` to extend an :class:`~pystac.Item`).  You may
+    prefer to use the `ext` class method of this class to construct the correct
+    instance type for you.
     """
 
-    asset_href: str
-    """The ``href`` value of the :class:`~pystac.Asset` being extended."""
-
     properties: Dict[str, Any]
     """The :class:`~pystac.Asset` fields, including extension properties."""
 
-    additional_read_properties: Optional[Iterable[Dict[str, Any]]] = None
-    """If present, this will be a list containing 1 dictionary representing the
-    properties of the owning :class:`~pystac.Item`."""
-
-    def __init__(self, asset: pystac.Asset):
-        self.asset_href = asset.href
-        self.properties = asset.extra_fields
-        if asset.owner and isinstance(asset.owner, pystac.Item):
-            self.additional_read_properties = [asset.owner.properties]
-
-    def __repr__(self) -> str:
-        return "<AssetRasterExtension Asset href={}>".format(self.asset_href)
-
     def apply(self, bands: List[RasterBand]) -> None:
         """Applies raster extension properties to the extended :class:`pystac.Item` or
         :class:`pystac.Asset`.
 
         Args:
             bands : a list of :class:`~pystac.RasterBand` objects that represent
                 the available raster bands.
@@ -703,40 +710,87 @@
         )
 
     @classmethod
     def get_schema_uri(cls) -> str:
         return SCHEMA_URI
 
     @classmethod
-    def ext(cls, obj: pystac.Asset, add_if_missing: bool = False) -> RasterExtension:
+    def get_schema_uris(cls) -> List[str]:
+        return SCHEMA_URIS
+
+    @classmethod
+    def ext(cls, obj: T, add_if_missing: bool = False) -> RasterExtension[T]:
         """Extends the given STAC Object with properties from the :stac-ext:`Raster
         Extension <raster>`.
 
         This extension can be applied to instances of :class:`~pystac.Asset`.
 
         Raises:
 
             pystac.ExtensionTypeError : If an invalid object type is passed.
         """
         if isinstance(obj, pystac.Asset):
             cls.validate_owner_has_extension(obj, add_if_missing)
-            return cls(obj)
-        else:
-            raise pystac.ExtensionTypeError(
-                f"Raster extension does not apply to type '{type(obj).__name__}'"
+            return cast(RasterExtension[T], AssetRasterExtension(obj))
+        elif isinstance(obj, item_assets.AssetDefinition):
+            cls.validate_has_extension(
+                cast(Union[pystac.Item, pystac.Collection], obj.owner), add_if_missing
             )
+            return cast(RasterExtension[T], ItemAssetsRasterExtension(obj))
+        else:
+            raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
     @classmethod
     def summaries(
         cls, obj: pystac.Collection, add_if_missing: bool = False
     ) -> SummariesRasterExtension:
         cls.validate_has_extension(obj, add_if_missing)
         return SummariesRasterExtension(obj)
 
 
+class AssetRasterExtension(RasterExtension[pystac.Asset]):
+    asset_href: str
+    """The ``href`` value of the :class:`~pystac.Asset` being extended."""
+
+    properties: Dict[str, Any]
+    """The :class:`~pystac.Asset` fields, including extension properties."""
+
+    additional_read_properties: Optional[Iterable[Dict[str, Any]]] = None
+    """If present, this will be a list containing 1 dictionary representing the
+    properties of the owning :class:`~pystac.Item`."""
+
+    def __init__(self, asset: pystac.Asset):
+        self.asset_href = asset.href
+        self.properties = asset.extra_fields
+        if asset.owner and isinstance(asset.owner, pystac.Item):
+            self.additional_read_properties = [asset.owner.properties]
+
+    def __repr__(self) -> str:
+        return "<AssetRasterExtension Asset href={}>".format(self.asset_href)
+
+
+class ItemAssetsRasterExtension(RasterExtension[item_assets.AssetDefinition]):
+    asset_definition: item_assets.AssetDefinition
+    """A reference to the :class:`~pystac.extensions.item_assets.AssetDefinition`
+    being extended."""
+
+    properties: Dict[str, Any]
+    """The :class:`~pystac.extensions.item_assets.AssetDefinition` fields, including
+    extension properties."""
+
+    def __init__(self, item_asset: item_assets.AssetDefinition):
+        self.properties = item_asset.properties
+        self.asset_definition = item_asset
+
+    def __repr__(self) -> str:
+        return "<ItemAssetsRasterExtension AssetDefinition={}>".format(
+            self.asset_definition
+        )
+
+
 class SummariesRasterExtension(SummariesExtension):
     """A concrete implementation of :class:`~SummariesExtension` that extends
     the ``summaries`` field of a :class:`~pystac.Collection` to include properties
     defined in the :stac-ext:`Raster Extension <raster>`.
     """
 
     @property
@@ -748,7 +802,16 @@
             lambda bands: [RasterBand(b) for b in bands],
             self.summaries.get_list(BANDS_PROP),
         )
 
     @bands.setter
     def bands(self, v: Optional[List[RasterBand]]) -> None:
         self._set_summary(BANDS_PROP, map_opt(lambda x: [b.to_dict() for b in x], v))
+
+
+class RasterExtensionHooks(ExtensionHooks):
+    schema_uri: str = SCHEMA_URI
+    prev_extension_ids: Set[str] = {*[uri for uri in SCHEMA_URIS if uri != SCHEMA_URI]}
+    stac_object_types = {pystac.STACObjectType.ITEM, pystac.STACObjectType.COLLECTION}
+
+
+RASTER_EXTENSION_HOOKS: ExtensionHooks = RasterExtensionHooks()
```

### Comparing `pystac-1.7.3/pystac/extensions/sar.py` & `pystac-1.8.0/pystac/extensions/sar.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,17 +318,15 @@
             if obj.owner is not None and not isinstance(obj.owner, pystac.Item):
                 raise pystac.ExtensionTypeError(
                     "SAR extension does not apply to Collection Assets."
                 )
             cls.validate_owner_has_extension(obj, add_if_missing)
             return cast(SarExtension[T], AssetSarExtension(obj))
         else:
-            raise pystac.ExtensionTypeError(
-                f"SAR extension does not apply to type '{type(obj).__name__}'"
-            )
+            raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
     @classmethod
     def summaries(
         cls, obj: pystac.Collection, add_if_missing: bool = False
     ) -> SummariesSarExtension:
         """Returns the extended summaries object for the given collection."""
         cls.validate_has_extension(obj, add_if_missing)
```

### Comparing `pystac-1.7.3/pystac/extensions/sat.py` & `pystac-1.8.0/pystac/extensions/sat.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,17 +149,15 @@
         if isinstance(obj, pystac.Item):
             cls.validate_has_extension(obj, add_if_missing)
             return cast(SatExtension[T], ItemSatExtension(obj))
         elif isinstance(obj, pystac.Asset):
             cls.validate_owner_has_extension(obj, add_if_missing)
             return cast(SatExtension[T], AssetSatExtension(obj))
         else:
-            raise pystac.ExtensionTypeError(
-                f"Satellite extension does not apply to type '{type(obj).__name__}'"
-            )
+            raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
     @classmethod
     def summaries(
         cls, obj: pystac.Collection, add_if_missing: bool = False
     ) -> SummariesSatExtension:
         """Returns the extended summaries object for the given collection."""
         cls.validate_has_extension(obj, add_if_missing)
```

### Comparing `pystac-1.7.3/pystac/extensions/scientific.py` & `pystac-1.8.0/pystac/extensions/scientific.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,17 +240,15 @@
         if isinstance(obj, pystac.Collection):
             cls.validate_has_extension(obj, add_if_missing)
             return cast(ScientificExtension[T], CollectionScientificExtension(obj))
         if isinstance(obj, pystac.Item):
             cls.validate_has_extension(obj, add_if_missing)
             return cast(ScientificExtension[T], ItemScientificExtension(obj))
         else:
-            raise pystac.ExtensionTypeError(
-                f"Scientific extension does not apply to type '{type(obj).__name__}'"
-            )
+            raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
     @classmethod
     def summaries(
         cls, obj: pystac.Collection, add_if_missing: bool = False
     ) -> SummariesScientificExtension:
         """Returns the extended summaries object for the given collection."""
         cls.validate_has_extension(obj, add_if_missing)
```

### Comparing `pystac-1.7.3/pystac/extensions/storage.py` & `pystac-1.8.0/pystac/extensions/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,17 +151,15 @@
         if isinstance(obj, pystac.Item):
             cls.validate_has_extension(obj, add_if_missing)
             return cast(StorageExtension[T], ItemStorageExtension(obj))
         elif isinstance(obj, pystac.Asset):
             cls.validate_owner_has_extension(obj, add_if_missing)
             return cast(StorageExtension[T], AssetStorageExtension(obj))
         else:
-            raise pystac.ExtensionTypeError(
-                f"StorageExtension does not apply to type '{type(obj).__name__}'"
-            )
+            raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
     @classmethod
     def summaries(
         cls, obj: pystac.Collection, add_if_missing: bool = False
     ) -> SummariesStorageExtension:
         """Returns the extended summaries object for the given collection."""
         cls.validate_has_extension(obj, add_if_missing)
```

### Comparing `pystac-1.7.3/pystac/extensions/table.py` & `pystac-1.8.0/pystac/extensions/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     def col_type(self, v: Optional[str]) -> None:
         if v is None:
             self.properties.pop(COL_TYPE_PROP, None)
         else:
             self.properties[COL_TYPE_PROP] = v
 
     def to_dict(self) -> Dict[str, Any]:
-        """Returns a JSON-like dictionary representing this ``Column``."""
+        """Returns a dictionary representing this ``Column``."""
         return self.properties
 
 
 class Table:
     """Object containing a high-level summary about a table"""
 
     properties: Dict[str, Any]
@@ -107,15 +107,15 @@
     def description(self, v: Optional[str]) -> None:
         if v is None:
             self.properties.pop(COL_DESCRIPTION_PROP, None)
         else:
             self.properties[COL_DESCRIPTION_PROP] = v
 
     def to_dict(self) -> Dict[str, Any]:
-        """Returns a JSON-like dictionary representing this ``Table``."""
+        """Returns a dictionary representing this ``Table``."""
         return self.properties
 
 
 class TableExtension(
     Generic[T],
     PropertiesExtension,
     ExtensionManagementMixin[Union[pystac.Collection, pystac.Item]],
@@ -157,17 +157,15 @@
         if isinstance(obj, pystac.Item):
             cls.validate_has_extension(obj, add_if_missing)
             return cast(TableExtension[T], ItemTableExtension(obj))
         if isinstance(obj, pystac.Asset):
             cls.validate_owner_has_extension(obj, add_if_missing)
             return cast(TableExtension[T], AssetTableExtension(obj))
         else:
-            raise pystac.ExtensionTypeError(
-                f"Table extension does not apply to type '{type(obj).__name__}'"
-            )
+            raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
     @property
     def columns(self) -> Optional[List[Column]]:
         """A list of :class:`Column` objects describing each column"""
         v = self.properties.get(COLUMNS_PROP)
         if v is None:
             return None
```

### Comparing `pystac-1.7.3/pystac/extensions/timestamps.py` & `pystac-1.8.0/pystac/extensions/timestamps.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,17 +130,15 @@
         if isinstance(obj, pystac.Item):
             cls.validate_has_extension(obj, add_if_missing)
             return cast(TimestampsExtension[T], ItemTimestampsExtension(obj))
         elif isinstance(obj, pystac.Asset):
             cls.validate_owner_has_extension(obj, add_if_missing)
             return cast(TimestampsExtension[T], AssetTimestampsExtension(obj))
         else:
-            raise pystac.ExtensionTypeError(
-                f"Timestamps extension does not apply to type '{type(obj).__name__}'"
-            )
+            raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
     @classmethod
     def summaries(
         cls, obj: pystac.Collection, add_if_missing: bool = False
     ) -> SummariesTimestampsExtension:
         """Returns the extended summaries object for the given collection."""
         cls.validate_has_extension(obj, add_if_missing)
```

### Comparing `pystac-1.7.3/pystac/extensions/version.py` & `pystac-1.8.0/pystac/extensions/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,17 +215,15 @@
         if isinstance(obj, pystac.Collection):
             cls.validate_has_extension(obj, add_if_missing)
             return cast(VersionExtension[T], CollectionVersionExtension(obj))
         if isinstance(obj, pystac.Item):
             cls.validate_has_extension(obj, add_if_missing)
             return cast(VersionExtension[T], ItemVersionExtension(obj))
         else:
-            raise pystac.ExtensionTypeError(
-                f"Version extension does not apply to type '{type(obj).__name__}'"
-            )
+            raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
 
 class CollectionVersionExtension(VersionExtension[pystac.Collection]):
     """A concrete implementation of :class:`VersionExtension` on a
     :class:`~pystac.Collection` that extends the properties of the Collection to
     include properties defined in the :stac-ext:`Versioning Indicators Extension
     <version>`.
```

### Comparing `pystac-1.7.3/pystac/extensions/view.py` & `pystac-1.8.0/pystac/extensions/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,17 +159,15 @@
         if isinstance(obj, pystac.Item):
             cls.validate_has_extension(obj, add_if_missing)
             return cast(ViewExtension[T], ItemViewExtension(obj))
         elif isinstance(obj, pystac.Asset):
             cls.validate_owner_has_extension(obj, add_if_missing)
             return cast(ViewExtension[T], AssetViewExtension(obj))
         else:
-            raise pystac.ExtensionTypeError(
-                f"View extension does not apply to type '{type(obj).__name__}'"
-            )
+            raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
     @classmethod
     def summaries(
         cls, obj: pystac.Collection, add_if_missing: bool = False
     ) -> SummariesViewExtension:
         """Returns the extended summaries object for the given collection."""
         cls.validate_has_extension(obj, add_if_missing)
```

### Comparing `pystac-1.7.3/pystac/item.py` & `pystac-1.8.0/pystac/item.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from __future__ import annotations
 
 import warnings
 from copy import copy, deepcopy
-from html import escape
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type, TypeVar, Union, cast
 
 import pystac
 from pystac import RelType, STACError, STACObjectType
 from pystac.asset import Asset
 from pystac.catalog import Catalog
 from pystac.collection import Collection
 from pystac.errors import DeprecatedWarning, ExtensionNotImplemented
-from pystac.html.jinja_env import get_jinja_env
 from pystac.link import Link
 from pystac.serialization import (
     identify_stac_object,
     identify_stac_object_type,
     migrate_to_latest,
 )
 from pystac.stac_object import STACObject
@@ -168,22 +166,14 @@
         if assets is not None:
             for k, asset in assets.items():
                 self.add_asset(k, asset)
 
     def __repr__(self) -> str:
         return "<Item id={}>".format(self.id)
 
-    def _repr_html_(self) -> str:
-        jinja_env = get_jinja_env()
-        if jinja_env:
-            template = jinja_env.get_template("Item.jinja2")
-            return str(template.render(item=self))
-        else:
-            return escape(repr(self))
-
     def set_self_href(self, href: Optional[str]) -> None:
         """Sets the absolute HREF that is represented by the ``rel == 'self'``
         :class:`~pystac.Link`.
 
         Changing the self HREF of the item will ensure that all asset HREFs
         remain valid. If asset HREFs are relative, the HREFs will change
         to point to the same location based on the new item self HREF,
@@ -252,77 +242,83 @@
             role: If set, filter the assets such that only those with a matching
                 ``role`` are returned.
 
         Returns:
             Dict[str, Asset]: A dictionary of assets that match ``media_type``
                 and/or ``role`` if set or else all of this item's assets.
         """
-        if media_type is None and role is None:
-            return dict(self.assets.items())
-        assets = dict()
-        for key, asset in self.assets.items():
-            if (media_type is None or asset.media_type == media_type) and (
-                role is None or asset.has_role(role)
-            ):
-                assets[key] = asset
-        return assets
+        return {
+            k: deepcopy(v)
+            for k, v in self.assets.items()
+            if (media_type is None or v.media_type == media_type)
+            and (role is None or v.has_role(role))
+        }
 
     def add_asset(self, key: str, asset: Asset) -> None:
         """Adds an Asset to this item.
 
         Args:
             key : The unique key of this asset.
             asset : The Asset to add.
         """
         asset.set_owner(self)
         self.assets[key] = asset
 
+    def delete_asset(self, key: str) -> None:
+        """Deletes the asset at the given key, and removes the asset's data
+        file from the local filesystem.
+
+        It is an error to attempt to delete an asset's file if it is on a
+        remote filesystem.
+
+        To delete the asset without removing the file, use `del item.assets["key"]`.
+
+        Args:
+            key: The unique key of this asset.
+        """
+        asset = self.assets[key]
+        asset.set_owner(self)
+        asset.delete()
+
+        del self.assets[key]
+
     def make_asset_hrefs_relative(self) -> Item:
         """Modify each asset's HREF to be relative to this item's self HREF.
 
         Returns:
             Item: self
         """
-
-        self_href = None
+        self_href = self.get_self_href()
         for asset in self.assets.values():
-            href = asset.href
-            if is_absolute_href(href):
+            if is_absolute_href(asset.href):
                 if self_href is None:
-                    self_href = self.get_self_href()
-                    if self_href is None:
-                        raise STACError(
-                            "Cannot make asset HREFs relative "
-                            "if no self_href is set."
-                        )
+                    raise STACError(
+                        "Cannot make asset HREFs relative " "if no self_href is set."
+                    )
                 asset.href = make_relative_href(asset.href, self_href)
         return self
 
     def make_asset_hrefs_absolute(self) -> Item:
         """Modify each asset's HREF to be absolute.
 
         Any asset HREFs that are relative will be modified to absolute based on this
         item's self HREF.
 
         Returns:
             Item: self
         """
-        self_href = None
+        self_href = self.get_self_href()
         for asset in self.assets.values():
-            href = asset.href
-            if not is_absolute_href(href):
+            if not is_absolute_href(asset.href):
                 if self_href is None:
-                    self_href = self.get_self_href()
-                    if self_href is None:
-                        raise STACError(
-                            "Cannot make relative asset HREFs absolute "
-                            "if no self_href is set."
-                        )
+                    raise STACError(
+                        "Cannot make relative asset HREFs absolute "
+                        "if no self_href is set."
+                    )
                 asset.href = make_absolute_href(asset.href, self_href)
-
         return self
 
     def set_collection(self, collection: Optional[Collection]) -> Item:
         """Set the collection of this item.
 
         This method will replace any existing Collection link and attribute for
         this item.
@@ -349,15 +345,70 @@
             Collection or None: If this item belongs to a collection, returns
             a reference to the collection. Otherwise returns None.
         """
         collection_link = self.get_single_link(pystac.RelType.COLLECTION)
         if collection_link is None:
             return None
         else:
-            return cast(Collection, collection_link.resolve_stac_object().target)
+            return cast(
+                Collection, collection_link.resolve_stac_object(self.get_root()).target
+            )
+
+    def add_derived_from(self, *items: Union[Item, str]) -> Item:
+        """Add one or more items that this is derived from.
+
+        This method will add to any existing "derived_from" links.
+
+        Args:
+            items : Items (or href of items) to add to derived_from links.
+
+        Returns:
+            Item: self
+        """
+        for item in items:
+            self.add_link(Link.derived_from(item))
+        return self
+
+    def remove_derived_from(self, item_id: str) -> None:
+        """Remove an item that this is derived from.
+
+        This method will remove from existing "derived_from" links.
+
+        Args:
+            item_id : ID of item to remove from derived_from links.
+        """
+        new_links: List[pystac.Link] = []
+
+        for link in self.links:
+            if link.rel != pystac.RelType.DERIVED_FROM:
+                new_links.append(link)
+            else:
+                try:
+                    item = cast(Item, link.resolve_stac_object().target)
+                except Exception as e:
+                    raise pystac.STACError(
+                        "Link failed to resolve. Use remove_links instead."
+                    ) from e
+                if item.id != item_id:
+                    new_links.append(link)
+        self.links = new_links
+
+    def get_derived_from(self) -> List[Item]:
+        """Get the items that this is derived from.
+
+        Returns:
+            List[Item]: Returns a reference to the derived_from items.
+        """
+        links = self.get_links(pystac.RelType.DERIVED_FROM)
+        try:
+            return [cast(Item, link.resolve_stac_object().target) for link in links]
+        except Exception as e:
+            raise pystac.STACError(
+                "Link failed to resolve. Use get_links instead."
+            ) from e
 
     def to_dict(
         self, include_self_link: bool = True, transform_hrefs: bool = True
     ) -> Dict[str, Any]:
         links = self.links
         if not include_self_link:
             links = [x for x in links if x.rel != pystac.RelType.SELF]
@@ -431,17 +482,15 @@
             d = deepcopy(d)
 
         if migrate:
             info = identify_stac_object(d)
             d = migrate_to_latest(d, info)
 
         if not cls.matches_object_type(d):
-            raise pystac.STACTypeError(
-                f"{d} does not represent a {cls.__name__} instance"
-            )
+            raise pystac.STACTypeError(d, cls)
 
         # some fields are passed through to __init__
         pass_through_fields = [
             "id",
             "geometry",
             "bbox",
             "stac_extensions",
@@ -504,30 +553,18 @@
 
     def full_copy(
         self, root: Optional[Catalog] = None, parent: Optional[Catalog] = None
     ) -> Item:
         return cast(Item, super().full_copy(root, parent))
 
     @classmethod
-    def from_file(
-        cls: Type[T], href: str, stac_io: Optional[pystac.StacIO] = None
-    ) -> T:
-        result = super().from_file(href, stac_io)
-        if not isinstance(result, Item):
-            raise pystac.STACTypeError(f"{result} is not a {Item}.")
-        return result
-
-    @classmethod
     def matches_object_type(cls, d: Dict[str, Any]) -> bool:
         for field in ("type", "stac_version"):
             if field not in d:
-                raise pystac.STACTypeError(
-                    f"{d} does not represent a {cls.__name__} instance"
-                    f"'{field}' is missing."
-                )
+                raise pystac.STACTypeError(d, cls, f"'{field}' is missing.")
         return identify_stac_object_type(d) == STACObjectType.ITEM
 
     @property
     def __geo_interface__(self) -> Dict[str, Any]:
         """Returns this item as a dictionary.
 
         This just calls `to_dict` without self links or transforming any hrefs.
```

### Comparing `pystac-1.7.3/pystac/item_collection.py` & `pystac-1.8.0/pystac/item_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         if not isinstance(other, ItemCollection):
             return NotImplemented
 
         combined = [*self.items, *other.items]
         return ItemCollection(items=combined)
 
     def to_dict(self, transform_hrefs: bool = False) -> Dict[str, Any]:
-        """Serializes an :class:`ItemCollection` instance to a JSON-like dictionary.
+        """Serializes an :class:`ItemCollection` instance to a dictionary.
 
         Args:
             transform_hrefs: If True, transform the HREF of hierarchical links
                 of Items based on the type of catalog the Item belongs to (if any).
                 I.e. if the item belongs to a root catalog that is
                 RELATIVE_PUBLISHED or SELF_CONTAINED,
                 hierarchical link HREFs will be transformed to be relative to the
@@ -144,14 +144,22 @@
             "type": "FeatureCollection",
             "features": [
                 item.to_dict(transform_hrefs=transform_hrefs) for item in self.items
             ],
             **self.extra_fields,
         }
 
+    def _repr_html_(self) -> str:
+        jinja_env = get_jinja_env()
+        if jinja_env:
+            template = jinja_env.get_template("JSON.jinja2")
+            return str(template.render(dict=self.to_dict()))
+        else:
+            return escape(repr(self))
+
     def clone(self) -> ItemCollection:
         """Creates a clone of this instance. This clone is a deep copy; all
         :class:`~pystac.Item` instances are cloned and all additional top-level fields
         are deep copied."""
         return self.__class__(
             items=[item.clone() for item in self.items],
             extra_fields=deepcopy(self.extra_fields),
@@ -171,15 +179,15 @@
             preserve_dict: If False, the dict parameter ``d`` may be modified
                 during this method call. Otherwise the dict is not mutated.
                 Defaults to True, which results results in a deepcopy of the
                 parameter. Set to False when possible to avoid the performance
                 hit of a deepcopy.
         """
         if not cls.is_item_collection(d):
-            raise STACTypeError("Dict is not a valid ItemCollection")
+            raise STACTypeError(d, cls)
 
         items = [
             pystac.Item.from_dict(item, preserve_dict=preserve_dict, root=root)
             for item in d.get("features", [])
         ]
         extra_fields = {k: v for k, v in d.items() if k not in ("features", "type")}
 
@@ -243,15 +251,7 @@
 
         # Prior to STAC 0.9 ItemCollections did not have a stac_version field and could
         #  only be identified by the fact that all of their 'features' are STAC Items.
         return all(
             identify_stac_object_type(feature) == pystac.STACObjectType.ITEM
             for feature in d.get("features", [])
         )
-
-    def _repr_html_(self) -> str:
-        jinja_env = get_jinja_env()
-        if jinja_env:
-            template = jinja_env.get_template("ItemCollection.jinja2")
-            return str(template.render(item_collection=self))
-        else:
-            return escape(repr(self))
```

### Comparing `pystac-1.7.3/pystac/layout.py` & `pystac-1.8.0/pystac/layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
+import posixpath
 import warnings
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 from string import Formatter
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Union
 
 import pystac
-from pystac.utils import JoinType, join_path_or_url, safe_urlparse
 
 if TYPE_CHECKING:
     from pystac.catalog import Catalog
     from pystac.collection import Collection
     from pystac.item import Item
     from pystac.stac_object import STACObject
 
@@ -422,59 +422,44 @@
         )
 
         if fallback_strategy is None:
             fallback_strategy = BestPracticesLayoutStrategy()
         self.fallback_strategy = fallback_strategy
 
     def get_catalog_href(self, cat: Catalog, parent_dir: str, is_root: bool) -> str:
-        parsed_parent_dir = safe_urlparse(parent_dir)
-        join_type = JoinType.from_parsed_uri(parsed_parent_dir)
-
         if is_root or self.catalog_template is None:
             return self.fallback_strategy.get_catalog_href(cat, parent_dir, is_root)
         else:
             template_path = self.catalog_template.substitute(cat)
             if not template_path.endswith(".json"):
-                template_path = join_path_or_url(
-                    join_type, template_path, cat.DEFAULT_FILE_NAME
-                )
+                template_path = posixpath.join(template_path, cat.DEFAULT_FILE_NAME)
 
-            return join_path_or_url(join_type, parent_dir, template_path)
+            return posixpath.join(parent_dir, template_path)
 
     def get_collection_href(
         self, col: Collection, parent_dir: str, is_root: bool
     ) -> str:
-        parsed_parent_dir = safe_urlparse(parent_dir)
-        join_type = JoinType.from_parsed_uri(parsed_parent_dir)
-
         if is_root or self.collection_template is None:
             return self.fallback_strategy.get_collection_href(col, parent_dir, is_root)
         else:
             template_path = self.collection_template.substitute(col)
             if not template_path.endswith(".json"):
-                template_path = join_path_or_url(
-                    join_type, template_path, col.DEFAULT_FILE_NAME
-                )
+                template_path = posixpath.join(template_path, col.DEFAULT_FILE_NAME)
 
-            return join_path_or_url(join_type, parent_dir, template_path)
+            return posixpath.join(parent_dir, template_path)
 
     def get_item_href(self, item: Item, parent_dir: str) -> str:
-        parsed_parent_dir = safe_urlparse(parent_dir)
-        join_type = JoinType.from_parsed_uri(parsed_parent_dir)
-
         if self.item_template is None:
             return self.fallback_strategy.get_item_href(item, parent_dir)
         else:
             template_path = self.item_template.substitute(item)
             if not template_path.endswith(".json"):
-                template_path = join_path_or_url(
-                    join_type, template_path, "{}.json".format(item.id)
-                )
+                template_path = posixpath.join(template_path, "{}.json".format(item.id))
 
-            return join_path_or_url(join_type, parent_dir, template_path)
+            return posixpath.join(parent_dir, template_path)
 
 
 class BestPracticesLayoutStrategy(HrefLayoutStrategy):
     """Layout strategy that represents the catalog layout described
     in the :stac-spec:`STAC Best Practices documentation
     <best-practices.md>`
 
@@ -485,44 +470,35 @@
     ID will be made, and the item ID will be used in the filename, i.e.
     ``${id}/${id}.json``
 
     All paths are appended to the parent directory.
     """
 
     def get_catalog_href(self, cat: Catalog, parent_dir: str, is_root: bool) -> str:
-        parsed_parent_dir = safe_urlparse(parent_dir)
-        join_type = JoinType.from_parsed_uri(parsed_parent_dir)
-
         if is_root:
             cat_root = parent_dir
         else:
-            cat_root = join_path_or_url(join_type, parent_dir, "{}".format(cat.id))
+            cat_root = posixpath.join(parent_dir, "{}".format(cat.id))
 
-        return join_path_or_url(join_type, cat_root, cat.DEFAULT_FILE_NAME)
+        return posixpath.join(cat_root, cat.DEFAULT_FILE_NAME)
 
     def get_collection_href(
         self, col: Collection, parent_dir: str, is_root: bool
     ) -> str:
-        parsed_parent_dir = safe_urlparse(parent_dir)
-        join_type = JoinType.from_parsed_uri(parsed_parent_dir)
-
         if is_root:
             col_root = parent_dir
         else:
-            col_root = join_path_or_url(join_type, parent_dir, "{}".format(col.id))
+            col_root = posixpath.join(parent_dir, "{}".format(col.id))
 
-        return join_path_or_url(join_type, col_root, col.DEFAULT_FILE_NAME)
+        return posixpath.join(col_root, col.DEFAULT_FILE_NAME)
 
     def get_item_href(self, item: Item, parent_dir: str) -> str:
-        parsed_parent_dir = safe_urlparse(parent_dir)
-        join_type = JoinType.from_parsed_uri(parsed_parent_dir)
-
-        item_root = join_path_or_url(join_type, parent_dir, "{}".format(item.id))
+        item_root = posixpath.join(parent_dir, "{}".format(item.id))
 
-        return join_path_or_url(join_type, item_root, "{}.json".format(item.id))
+        return posixpath.join(item_root, "{}.json".format(item.id))
 
 
 class AsIsLayoutStrategy(HrefLayoutStrategy):
     """Layout strategy that simply preserves the current href of all objects.
 
     If any object doesn't have a self href, a ValueError is raised.
     """
```

### Comparing `pystac-1.7.3/pystac/link.py` & `pystac-1.8.0/pystac/link.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,31 +3,35 @@
 import os
 from copy import copy
 from html import escape
 from typing import TYPE_CHECKING, Any, Dict, Optional, Type, TypeVar, Union
 
 import pystac
 from pystac.html.jinja_env import get_jinja_env
-from pystac.utils import is_absolute_href, make_absolute_href, make_relative_href
+from pystac.utils import (
+    HREF,
+    is_absolute_href,
+    make_absolute_href,
+    make_posix_style,
+    make_relative_href,
+)
 
 if TYPE_CHECKING:
     from pystac.catalog import Catalog
     from pystac.collection import Collection
     from pystac.item import Item
     from pystac.stac_object import STACObject
 
     PathLike = os.PathLike[str]
 
 else:
     PathLike = os.PathLike
 
 L = TypeVar("L", bound="Link")
 
-HREF = Union[str, os.PathLike]
-
 #: Hierarchical links provide structure to STAC catalogs.
 HIERARCHICAL_LINKS = [
     pystac.RelType.ROOT,
     pystac.RelType.CHILD,
     pystac.RelType.PARENT,
     pystac.RelType.COLLECTION,
     pystac.RelType.ITEM,
@@ -63,15 +67,15 @@
             object JSON.
     """
 
     rel: Union[str, pystac.RelType]
     """The relation of the link (e.g. 'child', 'item'). Registered rel Types are
     preferred. See :class:`~pystac.RelType` for common media types."""
 
-    media_type: Optional[str]
+    media_type: Optional[Union[str, pystac.MediaType]]
     """Optional description of the media type. Registered Media Types are preferred.
     See :class:`~pystac.MediaType` for common media types."""
 
     extra_fields: Dict[str, Any]
     """Optional, additional fields for this link. This is used by extensions as a
     way to serialize and deserialize properties on link object JSON."""
 
@@ -84,24 +88,24 @@
     _target_object: Optional[STACObject]
     _title: Optional[str]
 
     def __init__(
         self,
         rel: Union[str, pystac.RelType],
         target: Union[str, STACObject],
-        media_type: Optional[str] = None,
+        media_type: Optional[Union[str, pystac.MediaType]] = None,
         title: Optional[str] = None,
         extra_fields: Optional[Dict[str, Any]] = None,
     ) -> None:
         self.rel = rel
         if isinstance(target, str):
             if rel == pystac.RelType.SELF:
                 self._target_href = make_absolute_href(target)
             else:
-                self._target_href = target
+                self._target_href = make_posix_style(target)
             self._target_object = None
         else:
             self._target_href = None
             self._target_object = target
         self.media_type = media_type
         self.title = title
         self.extra_fields = extra_fields or {}
@@ -175,18 +179,19 @@
         ):
             root = self.owner.get_root()
             rel_links = [
                 *HIERARCHICAL_LINKS,
                 *pystac.EXTENSION_HOOKS.get_extended_object_links(self.owner),
             ]
             # if a hierarchical link with an owner and root, and relative catalog
-            if root and root.is_relative() and self.rel in rel_links:
-                owner_href = self.owner.get_self_href()
-                if owner_href is not None:
-                    href = make_relative_href(href, owner_href)
+            if root and root.is_relative():
+                if self.rel in rel_links or root.target_in_hierarchy(self.target):
+                    owner_href = self.owner.get_self_href()
+                    if owner_href is not None:
+                        href = make_relative_href(href, owner_href)
 
         return href
 
     @property
     def absolute_href(self) -> str:
         """Returns the absolute HREF for this link.
 
@@ -260,16 +265,16 @@
 
     def __repr__(self) -> str:
         return "<Link rel={} target={}>".format(self.rel, self.target)
 
     def _repr_html_(self) -> str:
         jinja_env = get_jinja_env()
         if jinja_env:
-            template = jinja_env.get_template("Link.jinja2")
-            return str(template.render(link=self))
+            template = jinja_env.get_template("JSON.jinja2")
+            return str(template.render(dict=self.to_dict()))
         else:
             return escape(repr(self))
 
     def resolve_stac_object(self, root: Optional[Catalog] = None) -> Link:
         """Resolves a STAC object from the HREF of this link, if the link is not
         already resolved.
 
@@ -330,15 +335,18 @@
 
         if (
             self.owner
             and self.rel in [pystac.RelType.CHILD, pystac.RelType.ITEM]
             and isinstance(self.owner, pystac.Catalog)
         ):
             assert self._target_object
-            self._target_object.set_parent(self.owner)
+            # Do nothing if the object wants to keep its parent
+            # https://github.com/stac-utils/pystac/issues/1116
+            if self._target_object._allow_parent_to_override_href:
+                self._target_object.set_parent(self.owner)
 
         return self
 
     def is_resolved(self) -> bool:
         """Determines if the link's target is a resolved STACObject.
 
         Returns:
@@ -355,33 +363,33 @@
 
         Returns:
             bool: True if the link's rel type is hierarchical.
         """
         return self.rel in HIERARCHICAL_LINKS
 
     def to_dict(self, transform_href: bool = True) -> Dict[str, Any]:
-        """Generate a dictionary representing the JSON of this serialized Link.
+        """Returns this link as a dictionary.
 
         Args:
             transform_href : If ``True``, transform the HREF based on the type of
                 catalog the owner belongs to (if any). I.e. if the link owner
                 belongs to a root catalog that is RELATIVE_PUBLISHED or SELF_CONTAINED,
                 the HREF will be transformed to be relative to the catalog root
                 if this is a hierarchical link relation.
         Returns:
-            dict : A serialization of the Link that can be written out as JSON.
+            dict : A serialization of the Link.
         """
 
         d: Dict[str, Any] = {
-            "rel": self.rel,
+            "rel": str(self.rel),
             "href": self.get_href(transform_href=transform_href),
         }
 
         if self.media_type is not None:
-            d["type"] = self.media_type
+            d["type"] = str(self.media_type)
 
         if self.title is not None:
             d["title"] = self.title
 
         for k, v in self.extra_fields.items():
             d[k] = v
 
@@ -464,14 +472,26 @@
     def item(cls: Type[L], item: Item, title: Optional[str] = None) -> L:
         """Creates a link to an Item."""
         return cls(
             pystac.RelType.ITEM, item, title=title, media_type=pystac.MediaType.JSON
         )
 
     @classmethod
+    def derived_from(
+        cls: Type[L], item: Union[Item, str], title: Optional[str] = None
+    ) -> L:
+        """Creates a link to a derived_from Item."""
+        return cls(
+            pystac.RelType.DERIVED_FROM,
+            item,
+            title=title,
+            media_type=pystac.MediaType.JSON,
+        )
+
+    @classmethod
     def canonical(
         cls: Type[L],
         item_or_collection: Union[Item, Collection],
         title: Optional[str] = None,
     ) -> L:
         """Creates a canonical link to an Item or Collection."""
         return cls(
```

### Comparing `pystac-1.7.3/pystac/media_type.py` & `pystac-1.8.0/pystac/media_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,9 +14,10 @@
     HTML = "text/html"
     JPEG = "image/jpeg"
     JPEG2000 = "image/jp2"
     JSON = "application/json"
     PNG = "image/png"
     TEXT = "text/plain"
     TIFF = "image/tiff"
+    KML = "application/vnd.google-earth.kml+xml"
     XML = "application/xml"
     PDF = "application/pdf"
```

### Comparing `pystac-1.7.3/pystac/provider.py` & `pystac-1.8.0/pystac/provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,24 +71,24 @@
         if not isinstance(o, Provider):
             return NotImplemented
         return self.to_dict() == o.to_dict()
 
     def _repr_html_(self) -> str:
         jinja_env = get_jinja_env()
         if jinja_env:
-            template = jinja_env.get_template("Provider.jinja2")
-            return str(template.render(provider=self))
+            template = jinja_env.get_template("JSON.jinja2")
+            return str(template.render(dict=self.to_dict()))
         else:
             return escape(repr(self))
 
     def to_dict(self) -> Dict[str, Any]:
-        """Generate a dictionary representing the JSON of this Provider.
+        """Returns this provider as a dictionary.
 
         Returns:
-            dict: A serialization of the Provider that can be written out as JSON.
+            dict: A serialization of the Provider.
         """
         d: Dict[str, Any] = {"name": self.name}
         if self.description is not None:
             d["description"] = self.description
         if self.roles is not None:
             d["roles"] = self.roles
         if self.url is not None:
```

### Comparing `pystac-1.7.3/pystac/rel_type.py` & `pystac-1.8.0/pystac/rel_type.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.3/pystac/serialization/common_properties.py` & `pystac-1.8.0/pystac/serialization/common_properties.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.3/pystac/serialization/identify.py` & `pystac-1.8.0/pystac/serialization/identify.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from enum import Enum
 from functools import total_ordering
-from typing import TYPE_CHECKING, Any, Dict, Optional, Set, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 import pystac
 from pystac.version import STACVersion
 
 if TYPE_CHECKING:
     from pystac.stac_object import STACObjectType
 
@@ -156,21 +156,21 @@
             has been identified as potential valid versions of the stac object.
         extensions : List of extension schema URIs for extensions this
             object implements
     """
 
     object_type: STACObjectType
     version_range: STACVersionRange
-    extensions: Set[str]
+    extensions: List[str]
 
     def __init__(
         self,
         object_type: STACObjectType,
         version_range: STACVersionRange,
-        extensions: Set[str],
+        extensions: List[str],
     ) -> None:
         self.object_type = object_type
         self.version_range = version_range
         self.extensions = extensions
 
     def __repr__(self) -> str:
         return "<{} {} ext={}>".format(
@@ -244,15 +244,16 @@
     Returns:
         STACJSONDescription: The description of the STAC object serialized in the
         given dict.
     """
     object_type = identify_stac_object_type(json_dict)
 
     if object_type is None:
-        raise pystac.STACTypeError("JSON does not represent a STAC object.")
+        extra_message = f"'type' attribute is {json_dict.get('type', 'not set')}"
+        raise pystac.STACTypeError(json_dict, pystac.STACObject, extra_message)
 
     version_range = STACVersionRange()
 
     stac_version = json_dict.get("stac_version")
     stac_extensions = json_dict.get("stac_extensions", None)
 
     if stac_version is None:
@@ -262,16 +263,8 @@
 
     if stac_extensions is not None:
         version_range.set_min(STACVersionID("0.8.0"))
 
     if stac_extensions is None:
         stac_extensions = []
 
-        # Between 1.0.0-beta.2 and 1.0.0-RC1, STAC extensions changed from
-        # being split between 'common' and custom extensions, with common
-        # extensions having short names that were used in the stac_extensions
-        # property list, to being mostly externalized from the core spec and
-        # always identified with the schema URI as the identifier. This
-        # code translates the short name IDs used pre-1.0.0-RC1 to the
-        # relevant extension schema uri identifier.
-
-    return STACJSONDescription(object_type, version_range, set(stac_extensions))
+    return STACJSONDescription(object_type, version_range, stac_extensions)
```

### Comparing `pystac-1.7.3/pystac/serialization/migrate.py` & `pystac-1.8.0/pystac/serialization/migrate.py`

 * *Files 3% similar despite different names*

```diff
@@ -180,28 +180,22 @@
     version = info.version_range.latest_valid_version()
 
     object_migrations = _get_object_migrations()
     removed_extension_migrations = _get_removed_extension_migrations()
 
     if version != STACVersion.DEFAULT_STAC_VERSION:
         object_migrations[info.object_type](result, version, info)
-        if "stac_extensions" not in result:
-            # Force stac_extensions property, as it makes
-            # downstream migration less complex
-            result["stac_extensions"] = []
-        pystac.EXTENSION_HOOKS.migrate(result, version, info)
+        result["stac_version"] = STACVersion.DEFAULT_STAC_VERSION
 
-        for ext in result["stac_extensions"][:]:
-            if ext in removed_extension_migrations:
-                object_types, migration_fn = removed_extension_migrations[ext]
-                if object_types is None or info.object_type in object_types:
-                    if migration_fn:
-                        migration_fn(result, version, info)
-                    result["stac_extensions"].remove(ext)
+    # Ensure stac_extensions property for consistency
+    result["stac_extensions"] = result.get("stac_extensions", None) or []
 
-        result["stac_version"] = STACVersion.DEFAULT_STAC_VERSION
-    else:
-        # Ensure stac_extensions property for consistency
-        if "stac_extensions" not in result:
-            result["stac_extensions"] = []
+    pystac.EXTENSION_HOOKS.migrate(result, version, info)
+    for ext in result["stac_extensions"][:]:
+        if ext in removed_extension_migrations:
+            object_types, migration_fn = removed_extension_migrations[ext]
+            if object_types is None or info.object_type in object_types:
+                if migration_fn:
+                    migration_fn(result, version, info)
+                result["stac_extensions"].remove(ext)
 
     return result
```

### Comparing `pystac-1.7.3/pystac/stac_io.py` & `pystac-1.8.0/pystac/stac_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
 
 import json
+import logging
 import os
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple
 from urllib.error import HTTPError
 from urllib.request import Request, urlopen
 
 import pystac
-from pystac.link import HREF
 from pystac.serialization import (
     identify_stac_object,
     identify_stac_object_type,
     merge_common_properties,
     migrate_to_latest,
 )
-from pystac.utils import safe_urlparse
+from pystac.utils import HREF, safe_urlparse
 
 # Use orjson if available
 try:
     import orjson
 except ImportError:
     orjson = None  # type: ignore[assignment]
 
@@ -32,14 +32,17 @@
     HAS_URLLIB3 = True
 
 if TYPE_CHECKING:
     from pystac.catalog import Catalog
     from pystac.stac_object import STACObject
 
 
+logger = logging.getLogger(__name__)
+
+
 class StacIO(ABC):
     _default_io: Optional[Callable[[], StacIO]] = None
 
     def __init__(self, headers: Optional[Dict[str, str]] = None):
         self.headers = headers or {}
 
     @abstractmethod
@@ -288,14 +291,15 @@
         Args:
 
             href : The URI of the file to open.
         """
         href_contents: str
         if _is_url(href):
             try:
+                logger.debug(f"GET {href} Headers: {self.headers}")
                 req = Request(href, headers=self.headers)
                 with urlopen(req) as f:
                     href_contents = f.read().decode("utf-8")
             except HTTPError as e:
                 raise Exception("Could not read uri {}".format(href)) from e
         else:
             with open(href, encoding="utf-8") as f:
@@ -317,14 +321,16 @@
         file system.
 
         Args:
 
             href : The path to which the file will be written.
             txt : The string content to write to the file.
         """
+        if _is_url(href):
+            raise NotImplementedError("DefaultStacIO cannot write to urls")
         href = os.fspath(href)
         dirname = os.path.dirname(href)
         if dirname != "" and not os.path.isdir(dirname):
             os.makedirs(dirname)
         with open(href, "w", encoding="utf-8") as f:
             f.write(txt)
```

### Comparing `pystac-1.7.3/pystac/stac_object.py` & `pystac-1.8.0/pystac/stac_object.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
+from html import escape
 from typing import (
     TYPE_CHECKING,
     Any,
+    Callable,
     Dict,
     Iterable,
     List,
     Optional,
+    Set,
     Type,
     TypeVar,
     Union,
     cast,
 )
 
 import pystac
 from pystac import STACError
+from pystac.html.jinja_env import get_jinja_env
 from pystac.link import Link
-from pystac.utils import StringEnum, is_absolute_href, make_absolute_href
+from pystac.utils import (
+    StringEnum,
+    is_absolute_href,
+    make_absolute_href,
+    make_posix_style,
+)
 
 if TYPE_CHECKING:
     from pystac.catalog import Catalog
 
 S = TypeVar("S", bound="STACObject")
 
 
@@ -46,14 +55,17 @@
     this STAC Object."""
 
     stac_extensions: List[str]
     """A list of schema URIs for STAC Extensions implemented by this STAC Object."""
 
     STAC_OBJECT_TYPE: STACObjectType
 
+    _allow_parent_to_override_href: bool = True
+    """Private attribute for whether parent objects should override on normalization"""
+
     def __init__(self, stac_extensions: List[str]) -> None:
         self.links = []
         self.stac_extensions = stac_extensions
 
     def validate(self) -> List[Any]:
         """Validate this STACObject.
 
@@ -121,14 +133,51 @@
             if link.is_hierarchical():
                 remove.append(link)
             else:
                 keep.append(link)
         self.links = keep
         return remove
 
+    def target_in_hierarchy(self, target: Union[str, STACObject]) -> bool:
+        """Determine if target is somewhere in the hierarchical link tree of
+        a STACObject.
+
+        Args:
+            target: A string or STACObject to search for
+
+        Returns:
+            bool: Returns True if the target was found in the hierarchical link tree
+                for the current STACObject
+        """
+
+        def traverse(
+            obj: Union[str, STACObject], visited: Set[Union[str, STACObject]]
+        ) -> bool:
+            if obj == target:
+                return True
+            if isinstance(obj, str):
+                return False
+
+            new_targets = [
+                link.target
+                for link in obj.links
+                if link.is_hierarchical() and link.target not in visited
+            ]
+            if target in new_targets:
+                return True
+
+            for subtree in new_targets:
+                visited.add(subtree)
+                if traverse(subtree, visited):
+                    return True
+
+            return False
+
+        return traverse(self, set([self]))
+
     def get_single_link(
         self,
         rel: Optional[Union[str, pystac.RelType]] = None,
         media_type: Optional[Union[str, pystac.MediaType]] = None,
     ) -> Optional[Link]:
         """Get a single :class:`~pystac.Link` instance associated with this
         object.
@@ -342,31 +391,40 @@
         """
 
         self.remove_links(pystac.RelType.PARENT)
         if parent is not None:
             self.add_link(Link.parent(parent))
 
     def get_stac_objects(
-        self, rel: Union[str, pystac.RelType], typ: Optional[Type[STACObject]] = None
+        self,
+        rel: Union[str, pystac.RelType],
+        typ: Optional[Type[STACObject]] = None,
+        modify_links: Optional[Callable[[List[Link]], List[Link]]] = None,
     ) -> Iterable[STACObject]:
         """Gets the :class:`~pystac.STACObject` instances that are linked to
         by links with their ``rel`` property matching the passed in argument.
 
         Args:
             rel : The relation to match each :class:`~pystac.Link`'s
                 ``rel`` property against.
             typ : If not ``None``, objects will only be yielded if they are instances of
                 ``typ``.
+            modify_links : A function that modifies the list of links before they are
+                iterated over. For instance, this option can be used to sort the list
+                so that links matching a particular pattern are earlier in the iterator.
 
         Returns:
             Iterable[STACObjects]: A possibly empty iterable of STACObjects that are
             connected to this object through links with the given ``rel`` and are of
             type ``typ`` (if given).
         """
         links = self.links[:]
+        if modify_links:
+            links = modify_links(links)
+
         for i in range(0, len(links)):
             link = links[i]
             if link.rel == rel:
                 link.resolve_stac_object(root=self.get_root())
                 if typ is None or isinstance(link.target, typ):
                     yield cast(STACObject, link.target)
 
@@ -501,30 +559,38 @@
         """
         raise NotImplementedError
 
     @abstractmethod
     def to_dict(
         self, include_self_link: bool = True, transform_hrefs: bool = True
     ) -> Dict[str, Any]:
-        """Generate a dictionary representing the JSON of this serialized object.
+        """Returns this object as a dictionary.
 
         Args:
             include_self_link : If True, the dict will contain a self link
                 to this object. If False, the self link will be omitted.
             transform_hrefs: If True, transform the HREF of hierarchical links
                 based on the type of catalog this object belongs to (if any).
                 I.e. if this object belongs to a root catalog that is
                 RELATIVE_PUBLISHED or SELF_CONTAINED,
                 hierarchical link HREFs will be transformed to be relative to the
                 catalog root.
 
-            dict: A serialization of the object that can be written out as JSON.
+            dict: A serialization of the object.
         """
         raise NotImplementedError
 
+    def _repr_html_(self) -> str:
+        jinja_env = get_jinja_env()
+        if jinja_env:
+            template = jinja_env.get_template("JSON.jinja2")
+            return str(template.render(dict=self.to_dict(transform_hrefs=False)))
+        else:
+            return escape(repr(self))
+
     @abstractmethod
     def clone(self) -> STACObject:
         """Clones this object.
 
         Cloning an object will make a copy of all properties and links of the object;
         however, it will not make copies of the targets of links (i.e. it is not a
         deep copy). To copy a STACObject fully, with all linked elements also copied,
@@ -549,27 +615,25 @@
         Returns:
             The specific STACObject implementation class that is represented
             by the JSON read from the file located at HREF.
         """
         if cls == STACObject:
             return cast(S, pystac.read_file(href))
 
+        href = make_posix_style(href)
+
         if stac_io is None:
             stac_io = pystac.StacIO.default()
 
         if not is_absolute_href(href):
             href = make_absolute_href(href)
 
         d = stac_io.read_json(href)
         o = cls.from_dict(d, href=href, migrate=True, preserve_dict=False)
 
-        # Set the self HREF, if it's not already set to something else.
-        if o.get_self_href() is None:
-            o.set_self_href(href)
-
         # If this is a root catalog, set the root to the catalog instance.
         root_link = o.get_root_link()
         if root_link is not None:
             if not root_link.is_resolved():
                 if root_link.get_absolute_href() == href:
                     o.set_root(cast(pystac.Catalog, o))
         return o
```

### Comparing `pystac-1.7.3/pystac/summaries.py` & `pystac-1.8.0/pystac/summaries.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 
+import json
 import numbers
+import sys
 from abc import abstractmethod
 from copy import deepcopy
 from enum import Enum
 from functools import lru_cache
 from typing import (
     TYPE_CHECKING,
     Any,
@@ -14,22 +16,42 @@
     List,
     Optional,
     Protocol,
     TypeVar,
     Union,
 )
 
+if sys.version_info[:2] < (3, 9):
+    from importlib_resources import files as importlib_resources_files
+else:
+    from importlib.resources import files as importlib_resources_files
+
 import pystac
 from pystac.utils import get_required
 
 if TYPE_CHECKING:
     from pystac.collection import Collection
     from pystac.item import Item
 
 
+def __getattr__(name: str) -> Any:
+    if name == "FIELDS_JSON_URL":
+        import warnings
+
+        warnings.warn(
+            "FIELDS_JSON_URL is deprecated and will be removed in v2",
+            DeprecationWarning,
+        )
+        return (
+            "https://cdn.jsdelivr.net/npm/@radiantearth/"
+            "stac-fields/fields-normalized.json"
+        )
+    raise AttributeError(f"module {__name__!r} has no attribute {name!r}")
+
+
 class _Comparable_x(Protocol):
     """Protocol for annotating comparable types.
 
     For matching __lt__ that takes an 'x' parameter
     (e.g. float)
     """
 
@@ -80,21 +102,25 @@
 
         return self.to_dict() == o.to_dict()
 
     def __repr__(self) -> str:
         return self.to_dict().__repr__()
 
 
-FIELDS_JSON_URL = (
-    "https://cdn.jsdelivr.net/npm/@radiantearth/stac-fields/fields-normalized.json"
-)
-
-
 @lru_cache(maxsize=None)
-def _get_fields_json(url: str) -> Dict[str, Any]:
+def _get_fields_json(url: Optional[str]) -> Dict[str, Any]:
+    if url is None:
+        # Every time pystac is released this file gets pulled from
+        # https://cdn.jsdelivr.net/npm/@radiantearth/stac-fields/fields-normalized.json
+        jsonfields: Dict[str, Any] = json.loads(
+            importlib_resources_files("pystac.static")
+            .joinpath("fields-normalized.json")
+            .read_text()
+        )
+        return jsonfields
     return pystac.StacIO.default().read_json(url)
 
 
 class SummaryStrategy(Enum):
     ARRAY = "v"
     RANGE = "r"
     SCHEMA = "s"
@@ -114,26 +140,15 @@
         fields (str): the path to the json file with field descriptions.
         If no file is passed, a default one will be used.
     """
 
     summaryfields: Dict[str, SummaryStrategy]
 
     def __init__(self, fields: Optional[str] = None):
-        fieldspath = fields or FIELDS_JSON_URL
-        try:
-            jsonfields = _get_fields_json(fieldspath)
-        except Exception as e:
-            if fields is None:
-                raise Exception(
-                    "Could not read fields definition file at "
-                    f"{fields} or it is invalid.\n"
-                    "Try using a local fields definition file."
-                )
-            else:
-                raise e
+        jsonfields = _get_fields_json(fields)
         self._set_field_definitions(jsonfields)
 
     def _set_field_definitions(self, fields: Dict[str, Any]) -> None:
         self.summaryfields = {}
         for name, desc in fields["metadata"].items():
             if isinstance(desc, dict):
                 strategy_value = desc.get("summary", True)
@@ -176,15 +191,15 @@
                         summary.append(v)
                     summaries.add(k, summary)
 
     def summarize(self, source: Union[Collection, Iterable[Item]]) -> Summaries:
         """Creates summaries from items"""
         summaries = Summaries.empty()
         if isinstance(source, pystac.Collection):
-            for item in source.get_all_items():
+            for item in source.get_items(recursive=True):
                 self._update_with_item(summaries, item)
         else:
             for item in source:
                 self._update_with_item(summaries, item)
 
         return summaries
```

### Comparing `pystac-1.7.3/pystac/utils.py` & `pystac-1.8.0/pystac/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,50 @@
 import os
 import posixpath
+import warnings
 from datetime import datetime, timezone
 from enum import Enum
-from typing import Any, Callable, Dict, List, Optional, TypeVar, Union, cast
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    TypeVar,
+    Union,
+    cast,
+)
 from urllib.parse import ParseResult as URLParseResult
 from urllib.parse import urljoin, urlparse, urlunparse
 
 import dateutil.parser
 
 from pystac.errors import RequiredPropertyMissing
 
-# Allow for modifying the path library for testability
-# (i.e. testing Windows path manipulation on non-Windows systems)
-_pathlib = os.path
+if TYPE_CHECKING:
+    PathLike = os.PathLike[str]
+else:
+    PathLike = os.PathLike
+
+HREF = Union[str, os.PathLike]
+
+
+def make_posix_style(href: HREF) -> str:
+    """Converts double back slashes and single back slashes to single forward
+    slashes for converting Windows paths to Posix style.
+
+    Args:
+        href (Union[str, os.PathLike]) : The href string or path-like object.
+
+    Returns:
+        str : The converted href in string form.
+    """
+    _href = str(os.fspath(href))
+    return _href.replace("\\\\", "/").replace("\\", "/")
 
 
 def safe_urlparse(href: str) -> URLParseResult:
     """Wrapper around :func:`urllib.parse.urlparse` that returns consistent results for
     both Windows and UNIX file paths.
 
     For Windows paths, this function will include the drive prefix (e.g. ``"D:\\"``) as
@@ -26,15 +54,21 @@
     Args:
         href (str) : The HREF to parse. May be a local file path or URL.
 
     Returns:
         urllib.parse.ParseResult : The named tuple representing the parsed HREF.
     """
     parsed = urlparse(href)
-    if parsed.scheme != "" and href.lower().startswith("{}:\\".format(parsed.scheme)):
+    if parsed.scheme != "" and (
+        href.lower().startswith("{}:\\".format(parsed.scheme))
+        or (
+            href.lower().startswith("{}:/".format(parsed.scheme))
+            and not href.lower().startswith("{}://".format(parsed.scheme))
+        )
+    ):
         return URLParseResult(
             scheme="",
             netloc="",
             path="{}:{}".format(
                 # We use this more complicated formulation because parsed.scheme
                 # converts to lower-case
                 href[: len(parsed.scheme)],
@@ -53,66 +87,94 @@
     value."""
 
     def __str__(self) -> str:
         return cast(str, self.value)
 
 
 class JoinType(StringEnum):
-    """Allowed join types for :func:`~pystac.utils.join_path_or_url`."""
+    """DEPRECATED.
+
+    .. deprecated:: 1.8.0
+        No longer used internally by pystac.
+
+    Allowed join types for :func:`~pystac.utils.join_path_or_url`.
+    """
 
     @staticmethod
     def from_parsed_uri(parsed_uri: URLParseResult) -> "JoinType":
-        """Determines the appropriate join type based on the scheme of the parsed
+        """DEPRECATED.
+
+        .. deprecated:: 1.8.0
+            No longer used internally by pystac.
+
+        Determines the appropriate join type based on the scheme of the parsed
         result.
 
         Args:
             parsed_uri (urllib.parse.ParseResult) : A named tuple representing the
                 parsed URI.
 
         Returns:
             JoinType : The join type for the URI.
         """
+        warnings.warn(
+            message=(
+                "from_parsed_uri is deprecated and will be removed in pystac "
+                "version 2.0.0. It is no longer used internally by pystac."
+            ),
+            category=DeprecationWarning,
+        )
         if parsed_uri.scheme == "":
             return JoinType.PATH
         else:
             return JoinType.URL
 
     PATH = "path"
     URL = "url"
 
 
 def join_path_or_url(join_type: JoinType, *args: str) -> str:
-    """Functions similarly to :func:`os.path.join`, but can be used to join either a
+    """DEPRECATED.
+
+    .. deprecated:: 1.8.0
+        No longer used internally by pystac.
+
+    Functions similarly to :func:`os.path.join`, but can be used to join either a
     local file path or a URL.
 
     Args:
         join_type (JoinType) : One of ``JoinType.PATH`` or ``JoinType.URL``. If
             ``JoinType.PATH``, then :func:`os.path.join` is used for the join.
             If ``JoinType.URL``, then :func:`posixpath.join` is used.
         *args (str): Additional positional string arguments to be joined.
 
     Returns:
         str : The joined path
-
     """
-
+    warnings.warn(
+        message=(
+            "join_path_or_url is deprecated and will be removed in pystac "
+            "version 2.0.0. It is no longer used internally by pystac."
+        ),
+        category=DeprecationWarning,
+    )
     if join_type == JoinType.PATH:
-        return _pathlib.join(*args)
+        return os.path.join(*args)
     else:
         return posixpath.join(*args)
 
 
 def _make_relative_href_url(
     parsed_source: URLParseResult,
     parsed_start: URLParseResult,
     start_is_dir: bool = False,
 ) -> str:
     # If the start path is not a directory, get the parent directory
     start_dir = (
-        parsed_start.path if start_is_dir else _pathlib.dirname(parsed_start.path)
+        parsed_start.path if start_is_dir else os.path.dirname(parsed_start.path)
     )
 
     # Strip the leading slashes from both paths
     start_dir = start_dir.lstrip("/")
     source_path = parsed_source.path.lstrip("/")
 
     # Get the relative path
@@ -121,39 +183,43 @@
     # Ensure we retain a trailing slash from the original source path
     if parsed_source.path.endswith("/"):
         rel_url += "/"
 
     # Prepend the "./", if necessary
     if rel_url != "./" and not rel_url.startswith("../"):
         rel_url = "./" + rel_url
+
     return rel_url
 
 
 def _make_relative_href_path(
     parsed_source: URLParseResult,
     parsed_start: URLParseResult,
     start_is_dir: bool = False,
 ) -> str:
     # If the start path is not a directory, get the parent directory
     start_dir = (
-        parsed_start.path if start_is_dir else _pathlib.dirname(parsed_start.path)
+        parsed_start.path if start_is_dir else os.path.dirname(parsed_start.path)
     )
 
     # Strip the leading slashes from both paths
     start_dir = start_dir.lstrip("/")
     source_path = parsed_source.path.lstrip("/")
 
-    relpath = _pathlib.relpath(source_path, start_dir)
+    # posixpath doesn't play well with windows drive letters, so we have to use
+    # the os-specific path library for the relpath function. This means we can
+    # only handle windows paths on windows machines.
+    relpath = make_posix_style(os.path.relpath(source_path, start_dir))
 
     # Ensure we retain a trailing slash from the original source path
     if parsed_source.path.endswith("/"):
         relpath += "/"
 
-    if relpath != "./" and not relpath.startswith(".." + _pathlib.sep):
-        relpath = _pathlib.join(".", relpath)
+    if relpath != "./" and not relpath.startswith("../"):
+        relpath = "./" + relpath
 
     return relpath
 
 
 def make_relative_href(
     source_href: str, start_href: str, start_is_dir: bool = False
 ) -> str:
@@ -169,24 +235,26 @@
         start_is_dir : If ``True``, ``start_href`` is treated as a directory.
             Otherwise, ``start_href`` is considered to be a path to a file. Defaults to
             ``False``.
 
     Returns:
         str: The relative HREF.
     """
+    source_href = make_posix_style(source_href)
+    start_href = make_posix_style(start_href)
 
     parsed_source = safe_urlparse(source_href)
     parsed_start = safe_urlparse(start_href)
     if not (
         parsed_source.scheme == parsed_start.scheme
         and parsed_source.netloc == parsed_start.netloc
     ):
         return source_href
 
-    if JoinType.from_parsed_uri(parsed_start) == JoinType.PATH:
+    if parsed_start.scheme == "":
         return _make_relative_href_path(parsed_source, parsed_start, start_is_dir)
     else:
         return _make_relative_href_url(parsed_source, parsed_start, start_is_dir)
 
 
 def _make_absolute_href_url(
     parsed_source: URLParseResult,
@@ -222,30 +290,34 @@
 
 def _make_absolute_href_path(
     parsed_source: URLParseResult,
     parsed_start: URLParseResult,
     start_is_dir: bool = False,
 ) -> str:
     # If the source is already absolute, just return it
-    if _pathlib.isabs(parsed_source.path):
+    if os.path.isabs(parsed_source.path):
         return urlunparse(parsed_source)
 
     # If the start path is not a directory, get the parent directory
     start_dir = (
-        parsed_start.path if start_is_dir else _pathlib.dirname(parsed_start.path)
+        parsed_start.path if start_is_dir else os.path.dirname(parsed_start.path)
     )
 
     # Join the start directory to the relative path and find the absolute path
-    abs_path = _pathlib.abspath(_pathlib.join(start_dir, parsed_source.path))
+    abs_path = make_posix_style(
+        os.path.abspath(os.path.join(start_dir, parsed_source.path))
+    )
 
     # Account for the normalization of abspath for
     # things like /vsitar// prefixes by replacing the
     # original start_dir text when abspath modifies the start_dir.
-    if not start_dir == _pathlib.abspath(start_dir):
-        abs_path = abs_path.replace(_pathlib.abspath(start_dir), start_dir)
+    if not start_dir == make_posix_style(os.path.abspath(start_dir)):
+        abs_path = abs_path.replace(
+            make_posix_style(os.path.abspath(start_dir)), start_dir
+        )
 
     return abs_path
 
 
 def make_absolute_href(
     source_href: str, start_href: Optional[str] = None, start_is_dir: bool = False
 ) -> str:
@@ -268,21 +340,21 @@
     Returns:
         str: The absolute HREF.
     """
     if start_href is None:
         start_href = os.getcwd()
         start_is_dir = True
 
+    source_href = make_posix_style(source_href)
+    start_href = make_posix_style(start_href)
+
     parsed_start = safe_urlparse(start_href)
     parsed_source = safe_urlparse(source_href)
 
-    if (
-        JoinType.from_parsed_uri(parsed_source) == JoinType.URL
-        or JoinType.from_parsed_uri(parsed_start) == JoinType.URL
-    ):
+    if parsed_source.scheme != "" or parsed_start.scheme != "":
         return _make_absolute_href_url(parsed_source, parsed_start, start_is_dir)
     else:
         return _make_absolute_href_path(parsed_source, parsed_start, start_is_dir)
 
 
 def is_absolute_href(href: str) -> bool:
     """Determines if an HREF is absolute or not.
@@ -292,15 +364,15 @@
     Args:
         href : The HREF to consider.
 
     Returns:
         bool: ``True`` if the given HREF is absolute, ``False`` if it is relative.
     """
     parsed = safe_urlparse(href)
-    return parsed.scheme != "" or _pathlib.isabs(parsed.path)
+    return parsed.scheme != "" or os.path.isabs(parsed.path)
 
 
 def datetime_to_str(dt: datetime, timespec: str = "auto") -> str:
     """Converts a :class:`datetime.datetime` instance to an ISO8601 string in the
     `RFC 3339, section 5.6
     <https://datatracker.ietf.org/doc/html/rfc3339#section-5.6>`__ format required by
     the :stac-spec:`STAC Spec <master/item-spec/common-metadata.md#date-and-time>`.
```

### Comparing `pystac-1.7.3/pystac/validation/__init__.py` & `pystac-1.8.0/pystac/validation/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     # If the version is before 1.0.0-rc.2, substitute extension short IDs for
     # their schemas.
     if stac_version_id < "1.0.0-rc.2":
 
         def _get_uri(ext: str) -> Optional[str]:
             return OldExtensionSchemaUriMap.get_extension_schema_uri(
                 ext,
-                stac_object_type,  # type:ignore
+                stac_object_type,
                 stac_version_id,
             )
 
         extensions = [uri for uri in map(_get_uri, extensions) if uri is not None]
 
     return RegisteredValidator.get_validator().validate(
         stac_dict, stac_object_type, stac_version, extensions, href
```

### Comparing `pystac-1.7.3/pystac/validation/schema_uri_map.py` & `pystac-1.8.0/pystac/validation/schema_uri_map.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.3/pystac/validation/stac_validator.py` & `pystac-1.8.0/pystac/validation/stac_validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import json
 import logging
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Optional, Tuple
 
 import pystac
 import pystac.utils
+from pystac.errors import STACLocalValidationError, STACValidationError
 from pystac.stac_object import STACObjectType
 from pystac.validation.schema_uri_map import DefaultSchemaUriMap, SchemaUriMap
 
 try:
     import jsonschema
     import jsonschema.exceptions
     import jsonschema.validators
+
+    from pystac.validation.local_validator import LocalValidator
+
+    HAS_JSONSCHEMA = True
 except ImportError:
-    jsonschema = None
+    HAS_JSONSCHEMA = False
 
 logger = logging.getLogger(__name__)
 
 
 class STACValidator(ABC):
     """STACValidator defines methods for validating STAC
     JSON. Implementations define methods for validating core objects and extension.
@@ -132,16 +137,16 @@
     This class requires the ``jsonschema`` library to be installed.
     """
 
     schema_uri_map: SchemaUriMap
     schema_cache: Dict[str, Dict[str, Any]]
 
     def __init__(self, schema_uri_map: Optional[SchemaUriMap] = None) -> None:
-        if jsonschema is None:
-            raise Exception("Cannot instantiate, requires jsonschema package")
+        if not HAS_JSONSCHEMA:
+            raise ImportError("Cannot instantiate, requires jsonschema package")
 
         if schema_uri_map is not None:
             self.schema_uri_map = schema_uri_map
         else:
             self.schema_uri_map = DefaultSchemaUriMap()
 
         self.schema_cache = {}
@@ -155,39 +160,53 @@
 
         resolver = jsonschema.validators.RefResolver(
             base_uri=schema_uri, referrer=schema, store=self.schema_cache
         )
 
         return schema, resolver
 
-    def _validate_from_uri(self, stac_dict: Dict[str, Any], schema_uri: str) -> None:
-        schema, resolver = self.get_schema_from_uri(schema_uri)
-        jsonschema.validate(instance=stac_dict, schema=schema, resolver=resolver)
-        for uri in resolver.store:
-            if uri not in self.schema_cache:
-                self.schema_cache[uri] = resolver.store[uri]
-
-    def _get_error_message(
+    def _validate_from_uri(
         self,
-        schema_uri: str,
+        stac_dict: Dict[str, Any],
         stac_object_type: STACObjectType,
-        extension_id: Optional[str],
-        href: Optional[str],
-        stac_id: Optional[str],
-    ) -> str:
-        s = "Validation failed for {} ".format(stac_object_type)
-        if href is not None:
-            s += "at {} ".format(href)
-        if stac_id is not None:
-            s += "with ID {} ".format(stac_id)
-        s += "against schema at {}".format(schema_uri)
-        if extension_id is not None:
-            s += " for STAC extension '{}'".format(extension_id)
-
-        return s
+        schema_uri: str,
+        href: Optional[str] = None,
+    ) -> None:
+        try:
+            resolver = None
+            try:
+                errors = LocalValidator()._validate_from_local(schema_uri, stac_dict)
+            except STACLocalValidationError:
+                schema, resolver = self.get_schema_from_uri(schema_uri)
+                # This block is cribbed (w/ change in error handling) from
+                # jsonschema.validate
+                cls = jsonschema.validators.validator_for(schema)
+                cls.check_schema(schema)
+                validator = cls(schema, resolver=resolver)
+                errors = list(validator.iter_errors(stac_dict))
+        except Exception as e:
+            logger.error(f"Exception while validating {stac_object_type} href: {href}")
+            logger.exception(e)
+            raise
+        if errors:
+            stac_id = stac_dict.get("id", None)
+            msg = f"Validation failed for {stac_object_type} "
+            if href is not None:
+                msg += f"at {href} "
+            if stac_id is not None:
+                msg += f"with ID {stac_id} "
+            msg += f"against schema at {schema_uri}"
+
+            best = jsonschema.exceptions.best_match(errors)
+            raise STACValidationError(msg, source=errors) from best
+
+        if resolver is not None:
+            for uri in resolver.store:
+                if uri not in self.schema_cache:
+                    self.schema_cache[uri] = resolver.store[uri]
 
     def validate_core(
         self,
         stac_dict: Dict[str, Any],
         stac_object_type: STACObjectType,
         stac_version: str,
         href: Optional[str] = None,
@@ -202,30 +221,31 @@
                 stac_dict. One of :class:`~pystac.STACObjectType`.
             stac_version : The version of STAC to validate the object against.
             href : Optional HREF of the STAC object being validated.
 
         Returns:
            str: URI for the JSON schema that was validated against, or None if
                no validation occurred.
+
+        Raises:
+           STACValidationError if stac_dict is not valid. The exception is raised from
+               the "best" error, as determined by the jsonschema library. To access all
+               jsonschema validation errors, use ``STACValidationError.source``.
+
         """
         schema_uri = self.schema_uri_map.get_object_schema_uri(
             stac_object_type, stac_version
         )
 
         if schema_uri is None:
             return None
 
-        try:
-            self._validate_from_uri(stac_dict, schema_uri)
-            return schema_uri
-        except jsonschema.exceptions.ValidationError as e:
-            msg = self._get_error_message(
-                schema_uri, stac_object_type, None, href, stac_dict.get("id")
-            )
-            raise pystac.STACValidationError(msg, source=e) from e
+        self._validate_from_uri(stac_dict, stac_object_type, schema_uri, href=href)
+
+        return schema_uri
 
     def validate_extension(
         self,
         stac_dict: Dict[str, Any],
         stac_object_type: STACObjectType,
         stac_version: str,
         extension_id: str,
@@ -242,26 +262,24 @@
             stac_version : The version of STAC to validate the object against.
             extension_id : The extension ID to validate against.
             href : Optional HREF of the STAC object being validated.
 
         Returns:
            str: URI for the JSON schema that was validated against, or None if
                no validation occurred.
+
+        Raises:
+           STACValidationError if stac_dict is not valid. The exception is raised from
+               the "best" error, as determined by the jsonschema library. To access all
+               jsonschema validation errors, use ``STACValidationError.source``.
+
         """
         schema_uri = extension_id
 
         if schema_uri is None:
             return None
+
         schema_uri = pystac.utils.make_absolute_href(schema_uri, href)
 
-        try:
-            self._validate_from_uri(stac_dict, schema_uri)
-            return schema_uri
-        except jsonschema.exceptions.ValidationError as e:
-            msg = self._get_error_message(
-                schema_uri, stac_object_type, extension_id, href, stac_dict.get("id")
-            )
-            raise pystac.STACValidationError(msg, source=e) from e
-        except Exception as e:
-            logger.error(f"Exception while validating {stac_object_type} href: {href}")
-            logger.exception(e)
-            raise
+        self._validate_from_uri(stac_dict, stac_object_type, schema_uri, href)
+
+        return schema_uri
```

### Comparing `pystac-1.7.3/pystac/version.py` & `pystac-1.8.0/pystac/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from typing import Optional
 
-__version__ = "1.7.3"
+__version__ = "1.8.0"
 """Library version"""
 
 
 class STACVersion:
     DEFAULT_STAC_VERSION = "1.0.0"
     """Latest STAC version supported by PySTAC"""
```

### Comparing `pystac-1.7.3/pystac.egg-info/PKG-INFO` & `pystac-1.8.0/pystac.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,88 @@
 Metadata-Version: 2.1
 Name: pystac
-Version: 1.7.3
-Summary: Python library for working with Spatiotemporal Asset Catalog (STAC).
-Home-page: https://github.com/stac-utils/pystac
-Author: stac-utils
-Author-email: stac@radiant.earth
-License: Apache Software License 2.0
-Project-URL: Tracker, https://github.com/stac-utils/pystac/issues
-Project-URL: Documentation, https://pystac.readthedocs.io/en/latest/
-Project-URL: GitHub Discussions, https://github.com/radiantearth/stac-spec/discussions/categories/pystac
+Version: 1.8.0
+Summary: Python library for working with the SpatioTemporal Asset Catalog (STAC) specification
+Author-email: Rob Emanuele <rdemanuele@gmail.com>, Jon Duckworth <duckontheweb@gmail.com>
+Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
+License: Apache-2.0
+Project-URL: homepage, https://github.com/stac-utils/pystac
+Project-URL: documentation, https://pystac.readthedocs.io
+Project-URL: repository, https://github.com/stac-utils/pystac.git
+Project-URL: changelog, https://github.com/stac-utils/pystac/blob/main/CHANGELOG.md
+Project-URL: discussions, https://github.com/radiantearth/stac-spec/discussions/categories/stac-software
 Keywords: pystac,imagery,raster,catalog,STAC
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: validation
+Provides-Extra: bench
+Provides-Extra: docs
+Provides-Extra: jinja2
 Provides-Extra: orjson
+Provides-Extra: test
 Provides-Extra: urllib3
+Provides-Extra: validation
 License-File: LICENSE
 
 # PySTAC
 
 [![Build Status](https://github.com/stac-utils/pystac/workflows/CI/badge.svg?branch=main)](https://github.com/stac-utils/pystac/actions/workflows/continuous-integration.yml)
 [![PyPI version](https://badge.fury.io/py/pystac.svg)](https://badge.fury.io/py/pystac)
 [![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/pystac)](https://anaconda.org/conda-forge/pystac)
 [![Documentation](https://readthedocs.org/projects/pystac/badge/?version=latest)](https://pystac.readthedocs.io/en/latest/)
 [![codecov](https://codecov.io/gh/stac-utils/pystac/branch/main/graph/badge.svg)](https://codecov.io/gh/stac-utils/pystac)
 [![Gitter](https://badges.gitter.im/SpatioTemporal-Asset-Catalog/python.svg)](https://gitter.im/SpatioTemporal-Asset-Catalog/python?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
-PySTAC is a library for working with [SpatioTemporal Asset Catalog](https://stacspec.org) in Python 3.
+PySTAC is a library for working with the [SpatioTemporal Asset Catalog](https://stacspec.org) specification in Python 3.
 
 ## Installation
 
 ### Install from PyPi (recommended)
 
 ```shell
 pip install pystac
 ```
 
 If you would like to enable the validation feature utilizing the
 [jsonschema](https://pypi.org/project/jsonschema/) project, install with the optional
 `validation` requirements:
 
 ```shell
-pip install pystac[validation]
+pip install 'pystac[validation]'
 ```
 
 If you would like to use the [`orjson`](https://pypi.org/project/orjson/) instead of the
 standard `json` library for JSON serialization/deserialization, install with the
 optional `orjson` requirements:
 
 ```shell
-pip install pystac[orjson]
+pip install 'pystac[orjson]'
 ```
 
 If you would like to use a custom `RetryStacIO` class for automatically retrying
 network requests when reading with PySTAC, you'll need
 [`urllib3`](https://urllib3.readthedocs.io/en/stable/):
 
 ```shell
-pip install pystac[urllib3]
+pip install 'pystac[urllib3]'
+```
+
+If you are using jupyter notebooks and want to enable pretty display of pystac objects you'll need [`jinja2`](https://pypi.org/project/Jinja2/)
+
+```shell
+pip install 'pystac[jinja2]'
 ```
 
 ### Install from source
 
 ```shell
 git clone https://github.com/stac-utils/pystac.git
 cd pystac
```

### Comparing `pystac-1.7.3/pystac.egg-info/SOURCES.txt` & `pystac-1.8.0/pystac.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE
+MANIFEST.in
 README.md
-setup.cfg
-setup.py
+pyproject.toml
 pystac/__init__.py
 pystac/asset.py
 pystac/cache.py
 pystac/catalog.py
 pystac/collection.py
 pystac/common_metadata.py
 pystac/errors.py
@@ -21,47 +21,46 @@
 pystac/stac_object.py
 pystac/summaries.py
 pystac/utils.py
 pystac/version.py
 pystac.egg-info/PKG-INFO
 pystac.egg-info/SOURCES.txt
 pystac.egg-info/dependency_links.txt
-pystac.egg-info/not-zip-safe
 pystac.egg-info/requires.txt
 pystac.egg-info/top_level.txt
 pystac/extensions/__init__.py
 pystac/extensions/base.py
+pystac/extensions/classification.py
 pystac/extensions/datacube.py
 pystac/extensions/eo.py
 pystac/extensions/file.py
 pystac/extensions/grid.py
 pystac/extensions/hooks.py
 pystac/extensions/item_assets.py
 pystac/extensions/label.py
+pystac/extensions/mgrs.py
 pystac/extensions/pointcloud.py
 pystac/extensions/projection.py
 pystac/extensions/raster.py
 pystac/extensions/sar.py
 pystac/extensions/sat.py
 pystac/extensions/scientific.py
 pystac/extensions/storage.py
 pystac/extensions/table.py
 pystac/extensions/timestamps.py
 pystac/extensions/version.py
 pystac/extensions/view.py
-pystac/html/Asset.jinja2
-pystac/html/Catalog.jinja2
-pystac/html/Collection.jinja2
-pystac/html/Item.jinja2
-pystac/html/ItemCollection.jinja2
-pystac/html/Link.jinja2
+pystac/extensions/xarray_assets.py
+pystac/html/JSON.jinja2
 pystac/html/Macros.jinja2
-pystac/html/Provider.jinja2
 pystac/html/__init__.py
 pystac/html/jinja_env.py
 pystac/serialization/__init__.py
 pystac/serialization/common_properties.py
 pystac/serialization/identify.py
 pystac/serialization/migrate.py
+pystac/static/__init__.py
 pystac/validation/__init__.py
+pystac/validation/local_validator.py
 pystac/validation/schema_uri_map.py
-pystac/validation/stac_validator.py
+pystac/validation/stac_validator.py
+pystac/validation/jsonschemas/__init__.py
```

### Comparing `pystac-1.7.3/setup.py` & `pystac-1.8.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,104 @@
-import os
-from glob import glob
-from os.path import basename, splitext
-
-from setuptools import find_packages, setup
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-with open(os.path.join(here, "README.md")) as readme_file:
-    readme = readme_file.read()
-
-setup(
-    name="pystac",
-    description=(
-        "Python library for working with Spatiotemporal Asset Catalog (STAC)."
-    ),
-    long_description=readme,
-    long_description_content_type="text/markdown",
-    author="stac-utils",
-    author_email="stac@radiant.earth",
-    url="https://github.com/stac-utils/pystac",
-    packages=find_packages(exclude=["tests*", "benchmarks*"]),
-    package_data={"": ["py.typed", "*.jinja2"]},
-    py_modules=[splitext(basename(path))[0] for path in glob("pystac/*.py")],
-    python_requires=">=3.8",
-    install_requires=["python-dateutil>=2.7.0"],
-    extras_require={
-        "validation": ["jsonschema>=4.0.1"],
-        "orjson": ["orjson>=3.5"],
-        "urllib3": ["urllib3>=1.26"],
-    },
-    license="Apache Software License 2.0",
-    license_files=["LICENSE"],
-    zip_safe=False,
-    keywords=["pystac", "imagery", "raster", "catalog", "STAC"],
-    classifiers=[
-        "Development Status :: 4 - Beta",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: Apache Software License",
-        "Natural Language :: English",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-    ],
-    project_urls={
-        "Tracker": "https://github.com/stac-utils/pystac/issues",
-        "Documentation": "https://pystac.readthedocs.io/en/latest/",
-        "GitHub Discussions": (
-            "https://github.com/radiantearth/stac-spec/discussions/categories/pystac"
-        ),
-    },
-    test_suite="tests",
-)
+[project]
+name = "pystac"
+description = "Python library for working with the SpatioTemporal Asset Catalog (STAC) specification"
+readme = "README.md"
+authors = [
+    { name = "Rob Emanuele", email = "rdemanuele@gmail.com" },
+    { name = "Jon Duckworth", email = "duckontheweb@gmail.com" }
+]
+maintainers = [
+    { name = "Pete Gadomski", email = "pete.gadomski@gmail.com" }
+]
+keywords = ["pystac", "imagery", "raster", "catalog", "STAC"]
+license = { text = "Apache-2.0" }
+classifiers=[
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: Apache Software License",
+    "Natural Language :: English",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+]
+requires-python = ">=3.8"
+dependencies = [
+    "importlib-resources>=5.12.0; python_version<'3.9'",
+    "python-dateutil>=2.7.0",
+]
+dynamic = ["version"]
+
+[project.optional-dependencies]
+bench = [
+    "asv~=0.5",
+    "virtualenv~=20.22",
+]
+docs = [
+    "Sphinx~=6.2",
+    "ipython~=8.12",
+    "jinja2<4.0",
+    "jupyter~=1.0",
+    "nbsphinx~=0.9",
+    "pydata-sphinx-theme~=0.13",
+    "sphinx-autobuild==2021.3.14",
+    "sphinx-design~=0.4",
+    "sphinxcontrib-fulltoc~=1.2",
+]
+jinja2 = [
+    "jinja2<4.0",
+]
+orjson = ["orjson>=3.5"]
+test = [
+    "black~=23.3",
+    "codespell~=2.2",
+    "coverage~=7.2",
+    "doc8~=1.1",
+    "html5lib~=1.1",
+    "jinja2<4.0",
+    "jsonschema~=4.17",
+    "mypy~=1.2",
+    "orjson~=3.8",
+    "pre-commit~=3.2",
+    "pytest-cov~=4.0",
+    "pytest-mock~=3.10",
+    "pytest-recording~=0.12",
+    "pytest~=7.3",
+    "ruff==0.0.275",
+    "types-html5lib~=1.1",
+    "types-orjson~=3.6",
+    "types-python-dateutil~=2.8",
+    "types-urllib3~=1.26",
+    # pytest-recording breakage with v5.0.0, need release of
+    # https://github.com/kiwicom/pytest-recording/pull/110 to remove this ceil
+    "vcrpy<5",
+]
+urllib3 = ["urllib3>=1.26"]
+validation = ["jsonschema>=4.0.1"]
+
+[project.urls]
+homepage = "https://github.com/stac-utils/pystac"
+documentation = "https://pystac.readthedocs.io"
+repository = "https://github.com/stac-utils/pystac.git"
+changelog = "https://github.com/stac-utils/pystac/blob/main/CHANGELOG.md"
+discussions = "https://github.com/radiantearth/stac-spec/discussions/categories/stac-software"
+
+[tool.setuptools.packages.find]
+include = ["pystac*"]
+exclude = ["tests*", "benchmarks*"]
+
+[tool.setuptools.dynamic]
+version = { attr = "pystac.version.__version__" }
+
+[tool.ruff]
+line-length = 88
+select = ["E", "F", "I"]
+
+[tool.pytest.ini_options]
+filterwarnings = [
+    "error",
+]
+
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
```

