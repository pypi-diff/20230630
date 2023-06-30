# Comparing `tmp/cognite_sdk-6.5.6.tar.gz` & `tmp/cognite_sdk-6.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.5.6.tar", max compression
+gzip compressed data, was "cognite_sdk-6.5.7.tar", max compression
```

## Comparing `cognite_sdk-6.5.6.tar` & `cognite_sdk-6.5.7.tar`

### file list

```diff
@@ -1,115 +1,115 @@
--rw-r--r--   0        0        0    11349 2023-06-29 08:45:42.686113 cognite_sdk-6.5.6/LICENSE
--rw-r--r--   0        0        0     3945 2023-06-29 08:45:42.686113 cognite_sdk-6.5.6/README.md
--rw-r--r--   0        0        0      574 2023-06-29 08:45:42.686113 cognite_sdk-6.5.6/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 08:45:42.686113 cognite_sdk-6.5.6/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     7558 2023-06-29 08:45:42.686113 cognite_sdk-6.5.6/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    49210 2023-06-29 08:45:42.686113 cognite_sdk-6.5.6/cognite/client/_api/assets.py
--rw-r--r--   0        0        0     1157 2023-06-29 08:45:42.686113 cognite_sdk-6.5.6/cognite/client/_api/data_modeling/__init__.py
--rw-r--r--   0        0        0     8056 2023-06-29 08:45:42.686113 cognite_sdk-6.5.6/cognite/client/_api/data_modeling/containers.py
--rw-r--r--   0        0        0     9702 2023-06-29 08:45:42.686113 cognite_sdk-6.5.6/cognite/client/_api/data_modeling/data_models.py
--rw-r--r--   0        0        0    37850 2023-06-29 08:45:42.686113 cognite_sdk-6.5.6/cognite/client/_api/data_modeling/instances.py
--rw-r--r--   0        0        0     6620 2023-06-29 08:45:42.686113 cognite_sdk-6.5.6/cognite/client/_api/data_modeling/spaces.py
--rw-r--r--   0        0        0     8221 2023-06-29 08:45:42.686113 cognite_sdk-6.5.6/cognite/client/_api/data_modeling/views.py
--rw-r--r--   0        0        0    11115 2023-06-29 08:45:42.686113 cognite_sdk-6.5.6/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54681 2023-06-29 08:45:42.686113 cognite_sdk-6.5.6/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    87544 2023-06-29 08:45:42.686113 cognite_sdk-6.5.6/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12424 2023-06-29 08:45:42.686113 cognite_sdk-6.5.6/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-06-29 08:45:42.686113 cognite_sdk-6.5.6/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    21384 2023-06-29 08:45:42.686113 cognite_sdk-6.5.6/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17504 2023-06-29 08:45:42.686113 cognite_sdk-6.5.6/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41590 2023-06-29 08:45:42.686113 cognite_sdk-6.5.6/cognite/client/_api/files.py
--rw-r--r--   0        0        0    45636 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    50175 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9619 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6088 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24756 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22919 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    38200 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7936 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32072 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    28258 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19276 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    22021 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     5083 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4691 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9705 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     1881 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    38337 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_api_client.py
--rw-r--r--   0        0        0     5391 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      215 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_constants.py
--rw-r--r--   0        0        0     6937 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/beta.py
--rw-r--r--   0        0        0     4631 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/config.py
--rw-r--r--   0        0        0    19252 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/credentials.py
--rw-r--r--   0        0        0     8794 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    19074 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8753 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34185 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    33708 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     4087 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/__init__.py
--rw-r--r--   0        0        0     1224 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/_core.py
--rw-r--r--   0        0        0     1239 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/_validation.py
--rw-r--r--   0        0        0     5154 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/aggregations.py
--rw-r--r--   0        0        0    11348 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/containers.py
--rw-r--r--   0        0        0     7670 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/data_models.py
--rw-r--r--   0        0        0     4710 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/data_types.py
--rw-r--r--   0        0        0     9519 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/filters.py
--rw-r--r--   0        0        0     6968 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/ids.py
--rw-r--r--   0        0        0    30982 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/instances.py
--rw-r--r--   0        0        0     2944 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/spaces.py
--rw-r--r--   0        0        0    15081 2023-06-29 08:45:42.690113 cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/views.py
--rw-r--r--   0        0        0     6691 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33969 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11015 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14376 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13671 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16695 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16556 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6349 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5885 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4120 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12267 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17675 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    16892 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11855 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12090 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    23040 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    12116 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11469 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2382 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2475 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2770 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9383 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/py.typed
--rw-r--r--   0        0        0     9006 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     7559 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9853 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     7748 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4260 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2981 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    24536 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3341 2023-06-29 08:45:42.694113 cognite_sdk-6.5.6/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     2151 2023-06-29 08:45:42.698113 cognite_sdk-6.5.6/pyproject.toml
--rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.5.6/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-06-29 19:29:50.294174 cognite_sdk-6.5.7/LICENSE
+-rw-r--r--   0        0        0     3945 2023-06-29 19:29:50.294174 cognite_sdk-6.5.7/README.md
+-rw-r--r--   0        0        0      574 2023-06-29 19:29:50.294174 cognite_sdk-6.5.7/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 19:29:50.294174 cognite_sdk-6.5.7/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     7558 2023-06-29 19:29:50.294174 cognite_sdk-6.5.7/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    49210 2023-06-29 19:29:50.294174 cognite_sdk-6.5.7/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0     1157 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/data_modeling/__init__.py
+-rw-r--r--   0        0        0     8056 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/data_modeling/containers.py
+-rw-r--r--   0        0        0     9702 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/data_modeling/data_models.py
+-rw-r--r--   0        0        0    37850 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/data_modeling/instances.py
+-rw-r--r--   0        0        0     6620 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/data_modeling/spaces.py
+-rw-r--r--   0        0        0     8221 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/data_modeling/views.py
+-rw-r--r--   0        0        0    11115 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54681 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87544 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12424 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    21384 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17504 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41590 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    45636 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    50175 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9619 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6088 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24756 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22919 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    38200 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     7936 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32072 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    28258 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19276 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    22021 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     5083 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4691 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9705 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     1881 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    38337 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     5391 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      215 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6937 2023-06-29 19:29:50.298174 cognite_sdk-6.5.7/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/beta.py
+-rw-r--r--   0        0        0     4631 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/config.py
+-rw-r--r--   0        0        0    19252 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8794 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    19074 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     8753 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34185 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    33708 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     4087 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/__init__.py
+-rw-r--r--   0        0        0     1224 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/_core.py
+-rw-r--r--   0        0        0     1239 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/_validation.py
+-rw-r--r--   0        0        0     5154 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/aggregations.py
+-rw-r--r--   0        0        0    11348 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/containers.py
+-rw-r--r--   0        0        0     7670 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/data_models.py
+-rw-r--r--   0        0        0     4710 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/data_types.py
+-rw-r--r--   0        0        0     9519 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/filters.py
+-rw-r--r--   0        0        0     6968 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/ids.py
+-rw-r--r--   0        0        0    30913 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/instances.py
+-rw-r--r--   0        0        0     2944 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/spaces.py
+-rw-r--r--   0        0        0    15081 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/views.py
+-rw-r--r--   0        0        0     6691 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    33969 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11015 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14376 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13671 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16695 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16556 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6349 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5885 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4120 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12267 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17675 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8699 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    16892 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11855 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12090 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    23040 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    12116 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11469 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2382 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2475 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2770 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9383 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/py.typed
+-rw-r--r--   0        0        0     9006 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     7559 2023-06-29 19:29:50.302174 cognite_sdk-6.5.7/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9853 2023-06-29 19:29:50.306174 cognite_sdk-6.5.7/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-06-29 19:29:50.306174 cognite_sdk-6.5.7/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     7748 2023-06-29 19:29:50.306174 cognite_sdk-6.5.7/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-06-29 19:29:50.306174 cognite_sdk-6.5.7/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-06-29 19:29:50.306174 cognite_sdk-6.5.7/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-06-29 19:29:50.306174 cognite_sdk-6.5.7/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4260 2023-06-29 19:29:50.306174 cognite_sdk-6.5.7/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2981 2023-06-29 19:29:50.306174 cognite_sdk-6.5.7/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    24536 2023-06-29 19:29:50.306174 cognite_sdk-6.5.7/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-06-29 19:29:50.306174 cognite_sdk-6.5.7/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-06-29 19:29:50.306174 cognite_sdk-6.5.7/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2151 2023-06-29 19:29:50.306174 cognite_sdk-6.5.7/pyproject.toml
+-rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.5.7/PKG-INFO
```

### Comparing `cognite_sdk-6.5.6/LICENSE` & `cognite_sdk-6.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/README.md` & `cognite_sdk-6.5.7/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/__init__.py` & `cognite_sdk-6.5.7/cognite/client/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/annotations.py` & `cognite_sdk-6.5.7/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/assets.py` & `cognite_sdk-6.5.7/cognite/client/_api/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/data_modeling/__init__.py` & `cognite_sdk-6.5.7/cognite/client/_api/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/data_modeling/containers.py` & `cognite_sdk-6.5.7/cognite/client/_api/data_modeling/containers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/data_modeling/data_models.py` & `cognite_sdk-6.5.7/cognite/client/_api/data_modeling/data_models.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/data_modeling/instances.py` & `cognite_sdk-6.5.7/cognite/client/_api/data_modeling/instances.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/data_modeling/spaces.py` & `cognite_sdk-6.5.7/cognite/client/_api/data_modeling/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/data_modeling/views.py` & `cognite_sdk-6.5.7/cognite/client/_api/data_modeling/views.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/data_sets.py` & `cognite_sdk-6.5.7/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.5.7/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/datapoints.py` & `cognite_sdk-6.5.7/cognite/client/_api/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/diagrams.py` & `cognite_sdk-6.5.7/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.5.7/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/events.py` & `cognite_sdk-6.5.7/cognite/client/_api/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.5.7/cognite/client/_api/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/files.py` & `cognite_sdk-6.5.7/cognite/client/_api/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/functions.py` & `cognite_sdk-6.5.7/cognite/client/_api/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/geospatial.py` & `cognite_sdk-6.5.7/cognite/client/_api/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/iam.py` & `cognite_sdk-6.5.7/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/labels.py` & `cognite_sdk-6.5.7/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/raw.py` & `cognite_sdk-6.5.7/cognite/client/_api/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/relationships.py` & `cognite_sdk-6.5.7/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/sequences.py` & `cognite_sdk-6.5.7/cognite/client/_api/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.5.7/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/templates.py` & `cognite_sdk-6.5.7/cognite/client/_api/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/three_d.py` & `cognite_sdk-6.5.7/cognite/client/_api/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/time_series.py` & `cognite_sdk-6.5.7/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.5.7/cognite/client/_api/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.5.7/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.5.7/cognite/client/_api/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.5.7/cognite/client/_api/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.5.7/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api/vision.py` & `cognite_sdk-6.5.7/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_api_client.py` & `cognite_sdk-6.5.7/cognite/client/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_cognite_client.py` & `cognite_sdk-6.5.7/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_http_client.py` & `cognite_sdk-6.5.7/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.5.7/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.5.7/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.5.7/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.5.7/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.5.7/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.5.7/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.5.7/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.5.7/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.5.7/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.5.7/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/config.py` & `cognite_sdk-6.5.7/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/credentials.py` & `cognite_sdk-6.5.7/cognite/client/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/_base.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/assets.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/__init__.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/_core.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/_validation.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/aggregations.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/aggregations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/containers.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/containers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/data_models.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/data_models.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/data_types.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/data_types.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/filters.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/filters.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/ids.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/ids.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/instances.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/instances.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import json
 from abc import abstractmethod
 from collections import defaultdict
-from dataclasses import asdict, dataclass
+from dataclasses import dataclass
 from typing import (
     Any,
     Dict,
     ItemsView,
     Iterator,
     KeysView,
     List,
@@ -38,15 +38,15 @@
     ContainerId,
     ContainerIdentifier,
     EdgeId,
     NodeId,
     ViewId,
     ViewIdentifier,
 )
-from cognite.client.utils._text import convert_all_keys_to_camel_case_recursive, convert_all_keys_to_snake_case
+from cognite.client.utils._text import convert_all_keys_to_snake_case
 
 PropertyValue = Union[str, int, float, bool, dict, List[str], List[int], List[float], List[bool], List[dict]]
 Space = str
 PropertyIdentifier = str
 
 
 @dataclass
@@ -62,23 +62,23 @@
     properties: Mapping[str, PropertyValue]
 
     @classmethod
     def load(cls, data: dict) -> NodeOrEdgeData:
         return cls(**convert_all_keys_to_snake_case(data))
 
     def dump(self, camel_case: bool = False) -> dict:
-        output = asdict(self)
+        output: Dict[str, Any] = {"properties": dict(self.properties.items())}
         if self.source:
             if isinstance(self.source, (ContainerId, ViewId)):
                 output["source"] = self.source.dump(camel_case)
             elif isinstance(self.source, dict):
                 output["source"] = self.source
             else:
                 raise TypeError(f"source must be ContainerId, ViewId or a dict, but was {type(self.source)}")
-        return convert_all_keys_to_camel_case_recursive(output) if camel_case else output
+        return output
 
 
 class InstanceCore(DataModelingResource):
     """A node or edge
     Args:
         instance_type (Literal["node", "edge"]) The type of instance.
         space (str): The workspace for the instance.a unique identifier for the space.
```

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/spaces.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/data_modeling/views.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/data_modeling/views.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/events.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/files.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/functions.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/iam.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/labels.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/raw.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/shared.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/templates.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/transformations/common.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-6.5.7/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/exceptions.py` & `cognite_sdk-6.5.7/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/testing.py` & `cognite_sdk-6.5.7/cognite/client/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/utils/__init__.py` & `cognite_sdk-6.5.7/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.5.7/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.5.7/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/utils/_graph.py` & `cognite_sdk-6.5.7/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/utils/_identifier.py` & `cognite_sdk-6.5.7/cognite/client/utils/_identifier.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/utils/_logging.py` & `cognite_sdk-6.5.7/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.5.7/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.5.7/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.5.7/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/utils/_text.py` & `cognite_sdk-6.5.7/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/utils/_time.py` & `cognite_sdk-6.5.7/cognite/client/utils/_time.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/utils/_validation.py` & `cognite_sdk-6.5.7/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.5.7/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.6/pyproject.toml` & `cognite_sdk-6.5.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.5.6"
+version = "6.5.7"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 license = "Apache-2.0"
```

### Comparing `cognite_sdk-6.5.6/PKG-INFO` & `cognite_sdk-6.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.5.6
+Version: 6.5.7
 Summary: Cognite Python SDK
 License: Apache-2.0
 Author: Erlend Vollset
 Author-email: erlend.vollset@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.5.6 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.5.7 Summary: Cognite Python
 SDK License: Apache-2.0 Author: Erlend Vollset Author-email:
 erlend.vollset@cognite.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-
 Extra: all Provides-Extra: functions Provides-Extra: geo Provides-Extra: numpy
```

