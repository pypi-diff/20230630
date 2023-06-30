# Comparing `tmp/bytetrade-recommend-model-sdk-0.0.20.tar.gz` & `tmp/bytetrade-recommend-model-sdk-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.20.tar", last modified: Sun Jun 25 06:06:05 2023, max compression
+gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.21.tar", last modified: Fri Jun 30 04:33:56 2023, max compression
```

## Comparing `bytetrade-recommend-model-sdk-0.0.20.tar` & `bytetrade-recommend-model-sdk-0.0.21.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.274581 bytetrade-recommend-model-sdk-0.0.20/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-06-25 06:06:05.274581 bytetrade-recommend-model-sdk-0.0.20/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.270581 bytetrade-recommend-model-sdk-0.0.20/bytetrade_recommend_model_sdk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-06-25 06:06:05.000000 bytetrade-recommend-model-sdk-0.0.20/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2116 2023-06-25 06:06:05.000000 bytetrade-recommend-model-sdk-0.0.20/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-25 06:06:05.000000 bytetrade-recommend-model-sdk-0.0.20/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2023-06-25 06:06:05.000000 bytetrade-recommend-model-sdk-0.0.20/bytetrade_recommend_model_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-06-25 06:06:05.000000 bytetrade-recommend-model-sdk-0.0.20/bytetrade_recommend_model_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.270581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.270581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/embeddings/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/embeddings/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      489 2023-06-20 08:36:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/embeddings/bert_embedding.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/embeddings/embedding_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5430 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/embeddings/word2vec_embedding.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.270581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-02 06:43:29.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.270581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/config/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 22:12:28.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/config/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2023-06-16 07:42:45.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/config/content_similar_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2023-06-24 23:59:37.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/config/mind_base_config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.274581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/dataset/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 21:32:28.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/dataset/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4244 2023-06-25 00:55:03.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1769 2023-06-25 03:47:07.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1694 2023-06-25 03:52:55.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2180 2023-06-12 05:18:24.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2873 2023-06-09 01:37:52.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.274581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/eval/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 22:36:32.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/eval/__init_.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2023-06-07 22:40:09.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/eval/eval_operation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11614 2023-06-13 09:09:31.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-06-07 07:14:04.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/experiment_enum.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.274581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/model/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 22:01:07.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/model/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9414 2023-06-16 07:32:06.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/model/content_similar_model.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2066 2023-06-24 06:04:38.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.274581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 09:34:20.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/train/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       82 2023-06-24 11:18:18.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/train/mind_dnn_click_predictor_train_tool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.274581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/proto_class/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/proto_class/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2661 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/proto_class/embedding_pb2.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.274581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/recommend/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/recommend/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3354 2023-06-16 05:57:06.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/recommend/recommend_common_util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1774 2023-06-16 07:52:03.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/recommend/recommend_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/recommend/time_weight_decay_tool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.274581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1835 2023-06-25 05:52:52.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/resources/model_management.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 06:06:05.274581 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/tools/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/tools/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5147 2023-06-06 23:52:17.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/tools/aws_s3_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10416 2023-06-12 05:13:22.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/tools/common_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27487 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/tools/model_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-25 06:06:05.274581 bytetrade-recommend-model-sdk-0.0.20/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      978 2023-06-25 06:05:33.000000 bytetrade-recommend-model-sdk-0.0.20/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-30 04:33:56.854533 bytetrade-recommend-model-sdk-0.0.21/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.21/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-06-30 04:33:56.854533 bytetrade-recommend-model-sdk-0.0.21/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.21/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-30 04:33:56.850533 bytetrade-recommend-model-sdk-0.0.21/bytetrade_recommend_model_sdk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-06-30 04:33:56.000000 bytetrade-recommend-model-sdk-0.0.21/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2178 2023-06-30 04:33:56.000000 bytetrade-recommend-model-sdk-0.0.21/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-30 04:33:56.000000 bytetrade-recommend-model-sdk-0.0.21/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2023-06-30 04:33:56.000000 bytetrade-recommend-model-sdk-0.0.21/bytetrade_recommend_model_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-06-30 04:33:56.000000 bytetrade-recommend-model-sdk-0.0.21/bytetrade_recommend_model_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-30 04:33:56.850533 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-30 04:33:56.850533 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/embeddings/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/embeddings/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      489 2023-06-20 08:36:05.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/embeddings/bert_embedding.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/embeddings/embedding_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5430 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/embeddings/word2vec_embedding.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-30 04:33:56.850533 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-02 06:43:29.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-30 04:33:56.850533 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/config/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 22:12:28.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/config/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2023-06-16 07:42:45.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/config/content_similar_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      396 2023-06-29 08:30:08.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/config/dnn_click_predictor_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2023-06-24 23:59:37.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/config/mind_base_config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-30 04:33:56.854533 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/dataset/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 21:32:28.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/dataset/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4244 2023-06-25 00:55:03.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1769 2023-06-25 03:47:07.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2719 2023-06-29 08:05:51.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2180 2023-06-12 05:18:24.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2873 2023-06-09 01:37:52.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-30 04:33:56.854533 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/eval/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 22:36:32.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/eval/__init_.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2023-06-07 22:40:09.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/eval/eval_operation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11667 2023-06-28 14:10:48.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-30 04:33:56.854533 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/exp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 09:34:20.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/exp/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11826 2023-06-29 09:10:30.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-06-07 07:14:04.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/experiment_enum.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-30 04:33:56.854533 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 22:01:07.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/model/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10026 2023-06-30 04:24:52.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/model/content_similar_model.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2330 2023-06-29 06:08:52.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-30 04:33:56.854533 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/proto_class/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/proto_class/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2661 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/proto_class/embedding_pb2.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-30 04:33:56.854533 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/recommend/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/recommend/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3354 2023-06-16 05:57:06.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/recommend/recommend_common_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1774 2023-06-16 07:52:03.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/recommend/recommend_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/recommend/time_weight_decay_tool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-30 04:33:56.854533 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1901 2023-06-26 07:14:58.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/resources/model_management.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-30 04:33:56.854533 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/tools/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/tools/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5147 2023-06-06 23:52:17.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/tools/aws_s3_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10416 2023-06-12 05:13:22.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/tools/common_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27487 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/tools/model_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-30 04:33:56.854533 bytetrade-recommend-model-sdk-0.0.21/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      978 2023-06-30 04:28:56.000000 bytetrade-recommend-model-sdk-0.0.21/setup.py
```

### Comparing `bytetrade-recommend-model-sdk-0.0.20/README.md` & `bytetrade-recommend-model-sdk-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.20/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt` & `bytetrade-recommend-model-sdk-0.0.21/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,29 +11,30 @@
 recommend_model_sdk/embeddings/bert_embedding.py
 recommend_model_sdk/embeddings/embedding_tool.py
 recommend_model_sdk/embeddings/word2vec_embedding.py
 recommend_model_sdk/mind_sdk/__init__.py
 recommend_model_sdk/mind_sdk/experiment_enum.py
 recommend_model_sdk/mind_sdk/config/__init__.py
 recommend_model_sdk/mind_sdk/config/content_similar_config.py
+recommend_model_sdk/mind_sdk/config/dnn_click_predictor_config.py
 recommend_model_sdk/mind_sdk/config/mind_base_config.py
 recommend_model_sdk/mind_sdk/dataset/__init__.py
 recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py
 recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py
 recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py
 recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py
 recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py
 recommend_model_sdk/mind_sdk/eval/__init_.py
 recommend_model_sdk/mind_sdk/eval/eval_operation.py
 recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py
+recommend_model_sdk/mind_sdk/exp/__init__.py
+recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py
 recommend_model_sdk/mind_sdk/model/__init__.py
 recommend_model_sdk/mind_sdk/model/content_similar_model.py
 recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py
-recommend_model_sdk/mind_sdk/train/__init__.py
-recommend_model_sdk/mind_sdk/train/mind_dnn_click_predictor_train_tool.py
 recommend_model_sdk/proto_class/__init__.py
 recommend_model_sdk/proto_class/embedding_pb2.py
 recommend_model_sdk/recommend/__init__.py
 recommend_model_sdk/recommend/recommend_common_util.py
 recommend_model_sdk/recommend/recommend_tool.py
 recommend_model_sdk/recommend/time_weight_decay_tool.py
 recommend_model_sdk/resources/__init__.py
```

### Comparing `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/embeddings/embedding_tool.py` & `bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/embeddings/embedding_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/embeddings/word2vec_embedding.py` & `bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/embeddings/word2vec_embedding.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/config/content_similar_config.py` & `bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/config/content_similar_config.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py` & `bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py` & `bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py` & `bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
 from torch.utils.data import Dataset, DataLoader
-
+from tqdm import tqdm
 from recommend_model_sdk.mind_sdk.config.mind_base_config import MINDBaseConfig
 
 class MINDBehaviorsParsedDataset(Dataset):
     """
     Load behaviors for evaluation, (user, time) pair as session
     """
     def __init__(self, behaviors_path,config):
@@ -19,27 +19,48 @@
         """
         super(MINDBehaviorsParsedDataset, self).__init__()
         if isinstance(config,MINDBaseConfig) is False:
             raise ValueError("config is not MINDBaseConfig")
         self.__config = config
         self.__behaviors = pd.read_table(behaviors_path,
                                        header=None,
-                                       usecols=range(4),
+                                       skiprows=[0],
+                                       # usecols=range(4),
                                        names=[
                                            'user', 'clicked_news',
                                            'candidate_news', 'clicked','impression_id'
                                        ])
         # self.__behaviors.clicked_news.fillna(' ', inplace=True)
 
     def __len__(self):
         return len(self.__behaviors)
 
     def __getitem__(self, idx):
         row = self.__behaviors.iloc[idx]
         item = {
             "user": row.user,
-            "candidate_news": row.candidate_news.split(),
-            'clicked':row.clicked.split(),
+            # "candidate_news": row.candidate_news.split(),
+            "candidate_news_str": row.candidate_news,
+            'clicked_str': row.clicked,
+            # 'clicked':row.clicked.split(),
             "impression_id": row.impression_id,
-            "clicked_news":row.clicked_news.split()[:self.__config.num_clicked_news_a_user]
+            "impression_id_str":str(row.impression_id),
+            # "clicked_news":row.clicked_news.split()[:self.__config.num_clicked_news_a_user],
+            'clicked_news_str':row.clicked_news
         }
-        return item
+        return item
+    
+    
+    def get_news_id_set_and_impression_id_to_clicked_news_dict(self):
+        news_id_set = set()
+        impression_id_to_clicked_news_dict = dict()
+        for current_index in tqdm(range(len(self.__behaviors)),desc="get_all_news_id_and_impression_id"):
+            current_row = self.__getitem__(current_index)
+            for current_news_id in current_row['clicked_news']:
+                news_id_set.add(current_news_id)
+            for current_news_id in current_row['candidate_news']:
+                news_id_set.add(current_news_id)
+            impression_id_to_clicked_news_dict[current_row["impression_id"]] = current_row["clicked_news"]
+            
+        return news_id_set,impression_id_to_clicked_news_dict
+    
+
```

### Comparing `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py` & `bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py` & `bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/eval/eval_operation.py` & `bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/eval/eval_operation.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py` & `bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import json
 from multiprocessing import Pool
 import numpy as np
 import os
 import sys
 import torch
-from torch.utils.data import Dataset, DataLoader
+from torch.utils.data import  DataLoader
 from tqdm import tqdm
 
 
 from recommend_model_sdk.mind_sdk.config.mind_base_config import MINDBaseConfig
 from recommend_model_sdk.mind_sdk.experiment_enum import DatasetKindEnum
 from recommend_model_sdk.mind_sdk.dataset.mind_news_dataset import MINDNewsDataset
-from recommend_model_sdk.mind_sdk.dataset.mind_user_dataset import MINDUserDataset
 from recommend_model_sdk.mind_sdk.dataset.mind_behaviours_dataset import MINDBehaviorsDataset
 from recommend_model_sdk.mind_sdk.eval.eval_operation import calculate_single_user_metric
-from recommend_model_sdk.mind_sdk.model.content_similar_model import ContentSimilarModel
 from recommend_model_sdk.tools.aws_s3_tool import AWSS3Tool
 from recommend_model_sdk.tools.common_tool import CommonTool
 
 
 
 
 
@@ -221,18 +219,22 @@
                                                     user_vector)
 
             y_pred = click_probability.tolist()
             y_true = [
                 int(news[0].split('-')[1]) for news in minibatch['impressions']
             ]
 
-            tasks.append((y_true, y_pred))
+            tasks.append((
+                          , y_pred))
 
         with Pool(processes=num_workers) as pool:
-            results = pool.map(calculate_single_user_metric, tasks)
+            results = pool.map(# `calculate_single_user_metric` is a function that takes the true
+            # labels and predicted probabilities for a single user's impressions
+            # and calculates the following metrics:
+            calculate_single_user_metric, tasks)
 
         aucs, mrrs, ndcg5s, ndcg10s = np.array(results).T
 
         MEAN_AUCS = np.nanmean(aucs), 
         MEAN_MRRS = np.nanmean(mrrs), 
         MEAN_nDCG5S = np.nanmean(ndcg5s), 
         MEAN_nDCG10S = np.nanmean(ndcg10s)
```

### Comparing `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/model/content_similar_model.py` & `bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/model/content_similar_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,20 @@
         id_list = news["id"]
         if isinstance(id_list,list) is False:
             raise ValueError("id_list is not list")
         
         embedding_list = list()
         for current_news_id in id_list:        
             current_key = f'{current_news_id}_{self.__config.embedding_model_name}_{self.__config.embedding_model_version}'
-            current_embedding = self.__aws_tool.get_object_dict(self.__bucket_name,current_key)["dict"]["vec"]
+            current_embedding_info =  self.__aws_tool.get_object_dict(self.__bucket_name,current_key)["dict"]
+            if current_embedding_info["success"]:
+                current_embedding = current_embedding_info["vec"]
+                print(len(current_embedding))
+            else:
+                current_embedding = [0] * self.__config.embedding_dim
             embedding_list.append(current_embedding)
         tensor_embedding = torch.tensor(embedding_list)
         return tensor_embedding
         
     
     def get_prediction(self,candidate_news_vector,user_vec):
         if isinstance(candidate_news_vector,torch.Tensor) is False:
@@ -176,14 +181,22 @@
         user_embedding = stack_candidate_embedding.sum(axis=0,keepdims=True)
         return user_embedding
             
     
     def recall(self,candidate_news_id_to_embedding,limit):
         """
         """
+        if len(candidate_news_id_to_embedding) < 1:
+            result_tuple_list = list()
+            for current_tuple in self.__base_document_id_to_created_at_tuple_list:
+                result_tuple_list.append((current_tuple[0],0.5))
+                if len(result_tuple_list) >= limit:
+                    break
+            return result_tuple_list
+        
         self.__recommend_common_util.validate_candidate_document_id_to_item(candidate_news_id_to_embedding,self.__embedding_shape)
         user_embedding = self.get_user_vector(candidate_news_id_to_embedding)
         faiss.normalize_L2(user_embedding)
         consin_similar, nearest_indexes = self.__cosin_index.search(user_embedding, limit) # cosin similar,
         result_tuple_list = list()
         for current_similar,current_index in zip(consin_similar[0],nearest_indexes[0]):
               current_weight = (2 - (1 - current_similar)) * 1.0 / 2
```

### Comparing `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py` & `bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 import torch
 import torch.nn as nn
 from math import sqrt
 
+
+
 from recommend_model_sdk.mind_sdk.config.content_similar_config import ContentSimilarConfig
 
 
+
 class DNNClickPredictor(torch.nn.Module):
-    def __init__(self, config, hidden_size=None):
+    def __init__(self, config,init_weight=False, hidden_size=None):
         super(DNNClickPredictor, self).__init__()
         if isinstance(config, ContentSimilarConfig) is False:
             raise ValueError("ContentSimilarModel is not model")
         self.__config = config
-        input_size = self.__config.embedding_dim
+
+        input_size = 2*self.__config.embedding_dim
         if hidden_size is None: 
             hidden_size = int(sqrt(input_size))
-        self.dnn = nn.Sequential(
+        self.__dnn = nn.Sequential(
             nn.Linear(input_size, hidden_size),
             nn.ReLU(),
             nn.Linear(hidden_size, 1),
         )
+        if init_weight:
+            self.__dnn.apply(self.init_weights)
+        
+    def init_weights(self,m):
+        if isinstance(m, nn.Linear):
+            torch.nn.init.xavier_uniform(m.weight)
+            m.bias.data.fill_(0.01)
+
 
     def forward(self, candidate_news_vector, user_vector):
         """
         Args:
             candidate_news_vector: batch_size, X
             user_vector: batch_size, X
         Returns:
@@ -42,8 +54,8 @@
             raise ValueError("candidate_news_vector dimension is not 2")
         if user_vector.shape[1] != self.__config.embedding_dim:
             raise ValueError("candidate_news_vector dimension element is not right")
         
         if candidate_news_vector.shape[0] != user_vector.shape[0]:
             raise ValueError("candidate_news_vector and user_vector have different size")
         
-        return self.dnn(torch.cat((candidate_news_vector, user_vector),dim=1)).squeeze(dim=1)
+        return self.__dnn(torch.cat((candidate_news_vector, user_vector),dim=1)).squeeze(dim=1)
```

### Comparing `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/proto_class/embedding_pb2.py` & `bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/proto_class/embedding_pb2.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/recommend/recommend_common_util.py` & `bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/recommend/recommend_common_util.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/recommend/recommend_tool.py` & `bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/recommend/recommend_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/recommend/time_weight_decay_tool.py` & `bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/recommend/time_weight_decay_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/resources/model_management.json` & `bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/resources/model_management.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'word2vec_google'": "{'v1': {'embedding_dim': 300}, 'v2': {'embedding_dim': 300}}"}*

```diff
@@ -10,14 +10,15 @@
             "pg_embedding_mark_field": "bert_v1",
             "s3_bucket": "gpu-model-data"
         }
     },
     "word2vec_google": {
         "v1": {
             "active": false,
+            "embedding_dim": 300,
             "model_related_files": [
                 "GoogleNews-vectors-negative300.bin",
                 "tfidf.model",
                 "dictionary"
             ],
             "model_related_files_public": {
                 "GoogleNews-vectors-negative300.bin": true,
@@ -31,14 +32,15 @@
             },
             "mongodb_embedding_field": "word2vec_google_v1",
             "pg_embedding_mark_field": "word2vec_google_embedding",
             "s3_bucket": "gpu-model-data"
         },
         "v2": {
             "active": false,
+            "embedding_dim": 300,
             "model_related_files": [
                 "GoogleNews-vectors-negative300.bin",
                 "tfidf.model",
                 "dictionary"
             ],
             "model_related_files_public": {
                 "GoogleNews-vectors-negative300.bin": true,
```

### Comparing `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/tools/aws_s3_tool.py` & `bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/tools/aws_s3_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/tools/common_tool.py` & `bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/tools/common_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.20/recommend_model_sdk/tools/model_tool.py` & `bytetrade-recommend-model-sdk-0.0.21/recommend_model_sdk/tools/model_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.20/setup.py` & `bytetrade-recommend-model-sdk-0.0.21/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 sys.path.append(os.path.dirname(__file__) + "/recommend-model")
 
 
 
 
 setup(
     name="bytetrade-recommend-model-sdk",
-    version="0.0.20",
+    version="0.0.21",
     # packages=find_packages(exclude="unit_test"),
     install_requires=[
         "pandas==2.0.0",
         "gensim==4.3.1",
         "protobuf==4.21.8",
         "nltk==3.8.1",
         "boto3"
```

