# Comparing `tmp/hezar-0.12.0.tar.gz` & `tmp/hezar-0.13.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hezar-0.12.0.tar", max compression
+gzip compressed data, was "hezar-0.13.3.tar", max compression
```

## Comparing `hezar-0.12.0.tar` & `hezar-0.13.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0     1065 2023-03-30 06:57:20.923678 hezar-0.12.0/LICENSE
--rw-r--r--   0        0        0     4227 2023-06-13 09:02:49.559875 hezar-0.12.0/README.md
--rw-r--r--   0        0        0      238 2023-05-17 05:46:22.196509 hezar-0.12.0/hezar/__init__.py
--rw-r--r--   0        0        0     6271 2023-05-20 21:02:11.140547 hezar-0.12.0/hezar/builders.py
--rw-r--r--   0        0        0    10248 2023-06-22 07:08:55.140905 hezar-0.12.0/hezar/configs.py
--rw-r--r--   0        0        0      740 2023-05-21 18:54:19.956201 hezar-0.12.0/hezar/constants.py
--rw-r--r--   0        0        0       75 2023-05-29 07:02:39.134582 hezar-0.12.0/hezar/data/__init__.py
--rw-r--r--   0        0        0     3708 2023-03-06 08:47:57.729206 hezar-0.12.0/hezar/data/data_collators.py
--rw-r--r--   0        0        0      129 2023-02-27 14:30:03.533478 hezar-0.12.0/hezar/data/datasets/__init__.py
--rw-r--r--   0        0        0      339 2023-04-11 10:15:40.865625 hezar-0.12.0/hezar/data/datasets/dataset.py
--rw-r--r--   0        0        0     3177 2023-04-26 07:18:05.021932 hezar-0.12.0/hezar/data/datasets/text_classification_dataset.py
--rw-r--r--   0        0        0       26 2023-02-27 13:58:04.862187 hezar-0.12.0/hezar/data/utils/__init__.py
--rw-r--r--   0        0        0     1547 2023-04-26 07:18:05.021932 hezar-0.12.0/hezar/data/utils/data_utils.py
--rw-r--r--   0        0        0      127 2023-05-21 18:54:19.956201 hezar-0.12.0/hezar/embeddings/__init__.py
--rw-r--r--   0        0        0     4146 2023-06-11 12:19:24.750092 hezar-0.12.0/hezar/embeddings/embedding.py
--rw-r--r--   0        0        0     3122 2023-05-29 07:28:46.468064 hezar-0.12.0/hezar/embeddings/fasttext.py
--rw-r--r--   0        0        0     3081 2023-05-29 07:28:46.480064 hezar-0.12.0/hezar/embeddings/word2vec.py
--rw-r--r--   0        0        0      282 2023-05-29 07:02:39.134582 hezar-0.12.0/hezar/models/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 09:12:34.341429 hezar-0.12.0/hezar/models/audio_classification/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 10:12:24.186008 hezar-0.12.0/hezar/models/image2text/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 08:51:35.484556 hezar-0.12.0/hezar/models/image2text/crnn/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 08:51:41.116344 hezar-0.12.0/hezar/models/image2text/trocr/__init__.py
--rw-r--r--   0        0        0      144 2023-03-30 11:32:46.534855 hezar-0.12.0/hezar/models/language_modeling/__init__.py
--rw-r--r--   0        0        0       69 2023-03-12 09:06:49.418541 hezar-0.12.0/hezar/models/language_modeling/bert/__init__.py
--rw-r--r--   0        0        0     1136 2023-04-11 10:17:52.306691 hezar-0.12.0/hezar/models/language_modeling/bert/bert_lm.py
--rw-r--r--   0        0        0      720 2023-04-11 10:15:40.869625 hezar-0.12.0/hezar/models/language_modeling/bert/bert_lm_config.py
--rw-r--r--   0        0        0       93 2023-02-23 22:01:19.874524 hezar-0.12.0/hezar/models/language_modeling/distilbert/__init__.py
--rw-r--r--   0        0        0     1208 2023-04-11 10:17:52.306691 hezar-0.12.0/hezar/models/language_modeling/distilbert/distilbert_lm.py
--rw-r--r--   0        0        0      586 2023-04-11 10:15:40.869625 hezar-0.12.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
--rw-r--r--   0        0        0       81 2023-03-30 11:32:10.710583 hezar-0.12.0/hezar/models/language_modeling/roberta/__init__.py
--rw-r--r--   0        0        0     1172 2023-04-11 10:17:52.306691 hezar-0.12.0/hezar/models/language_modeling/roberta/roberta_lm.py
--rw-r--r--   0        0        0      780 2023-04-11 10:15:40.869625 hezar-0.12.0/hezar/models/language_modeling/roberta/roberta_lm_config.py
--rw-r--r--   0        0        0     9544 2023-06-21 10:13:50.379727 hezar-0.12.0/hezar/models/model.py
--rw-r--r--   0        0        0        0 2023-04-05 08:19:28.666981 hezar-0.12.0/hezar/models/sequence_labeling/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 08:19:28.666981 hezar-0.12.0/hezar/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 11:10:19.495328 hezar-0.12.0/hezar/models/speech_recognition/wav2vec/__init__.py
--rw-r--r--   0        0        0      240 2023-03-31 21:16:38.915201 hezar-0.12.0/hezar/models/text_classification/__init__.py
--rw-r--r--   0        0        0      135 2023-03-12 07:18:24.393055 hezar-0.12.0/hezar/models/text_classification/bert/__init__.py
--rw-r--r--   0        0        0     2679 2023-04-11 10:17:52.306691 hezar-0.12.0/hezar/models/text_classification/bert/bert_text_classification.py
--rw-r--r--   0        0        0      808 2023-04-11 10:15:40.869625 hezar-0.12.0/hezar/models/text_classification/bert/bert_text_classification_config.py
--rw-r--r--   0        0        0      159 2023-03-04 19:50:13.301724 hezar-0.12.0/hezar/models/text_classification/distilbert/__init__.py
--rw-r--r--   0        0        0     2813 2023-04-20 12:05:09.995882 hezar-0.12.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py
--rw-r--r--   0        0        0      711 2023-05-24 07:34:43.436658 hezar-0.12.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
--rw-r--r--   0        0        0      147 2023-03-31 21:16:38.919201 hezar-0.12.0/hezar/models/text_classification/roberta/__init__.py
--rw-r--r--   0        0        0     2943 2023-04-11 10:17:52.306691 hezar-0.12.0/hezar/models/text_classification/roberta/roberta_text_classification.py
--rw-r--r--   0        0        0      905 2023-04-11 10:15:40.869625 hezar-0.12.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py
--rw-r--r--   0        0        0        0 2023-04-11 10:12:24.186008 hezar-0.12.0/hezar/models/text_detection/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 10:12:24.186008 hezar-0.12.0/hezar/models/text_detection/ctpn/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 10:12:24.186008 hezar-0.12.0/hezar/models/text_detection/dbnet/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 08:19:28.666981 hezar-0.12.0/hezar/models/text_summarization/__init__.py
--rw-r--r--   0        0        0      104 2023-03-11 07:23:51.576283 hezar-0.12.0/hezar/preprocessors/__init__.py
--rw-r--r--   0        0        0        0 2023-02-28 18:59:54.953875 hezar-0.12.0/hezar/preprocessors/normalizers/__init__.py
--rw-r--r--   0        0        0        0 2023-03-01 17:42:58.020976 hezar-0.12.0/hezar/preprocessors/normalizers/nfkc.py
--rw-r--r--   0        0        0        0 2023-02-28 18:59:54.953875 hezar-0.12.0/hezar/preprocessors/normalizers/nfkd.py
--rw-r--r--   0        0        0        0 2023-02-28 18:59:54.953875 hezar-0.12.0/hezar/preprocessors/normalizers/normalizer.py
--rw-r--r--   0        0        0     2218 2023-05-12 08:41:30.512170 hezar-0.12.0/hezar/preprocessors/preprocessor.py
--rw-r--r--   0        0        0      298 2023-03-06 08:47:57.729206 hezar-0.12.0/hezar/preprocessors/tokenizers/__init__.py
--rw-r--r--   0        0        0     4623 2023-05-21 18:54:19.956201 hezar-0.12.0/hezar/preprocessors/tokenizers/bpe.py
--rw-r--r--   0        0        0     5181 2023-05-21 18:54:19.956201 hezar-0.12.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
--rw-r--r--   0        0        0    15394 2023-06-11 12:16:36.618164 hezar-0.12.0/hezar/preprocessors/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     4215 2023-05-21 18:54:19.956201 hezar-0.12.0/hezar/preprocessors/tokenizers/wordpiece.py
--rw-r--r--   0        0        0     7443 2023-06-13 08:52:35.482356 hezar-0.12.0/hezar/registry.py
--rw-r--r--   0        0        0       29 2023-02-23 22:01:19.878524 hezar-0.12.0/hezar/trainers/__init__.py
--rw-r--r--   0        0        0    13853 2023-06-11 12:16:36.614164 hezar-0.12.0/hezar/trainers/trainer.py
--rw-r--r--   0        0        0     1773 2023-04-20 12:02:00.811155 hezar-0.12.0/hezar/trainers/trainer_utils.py
--rw-r--r--   0        0        0      135 2023-03-19 11:54:11.276216 hezar-0.12.0/hezar/utils/__init__.py
--rw-r--r--   0        0        0     2435 2023-05-20 21:02:11.140547 hezar-0.12.0/hezar/utils/config_utils.py
--rw-r--r--   0        0        0      482 2023-03-21 17:28:57.241651 hezar-0.12.0/hezar/utils/context_managers.py
--rw-r--r--   0        0        0     2773 2023-06-09 14:53:27.229341 hezar-0.12.0/hezar/utils/hub_utils.py
--rw-r--r--   0        0        0      374 2023-03-04 09:40:29.111460 hezar-0.12.0/hezar/utils/logging.py
--rw-r--r--   0        0        0        0 2023-03-12 08:35:41.141839 hezar-0.12.0/hezar/utils/model_utils.py
--rw-r--r--   0        0        0     1579 2023-06-24 13:47:40.065364 hezar-0.12.0/pyproject.toml
--rw-r--r--   0        0        0     6604 1970-01-01 00:00:00.000000 hezar-0.12.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-30 06:57:28.300613 hezar-0.13.3/LICENSE
+-rw-r--r--   0        0        0     4227 2023-06-30 06:57:28.300613 hezar-0.13.3/README.md
+-rw-r--r--   0        0        0      238 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/__init__.py
+-rw-r--r--   0        0        0     6271 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/builders.py
+-rw-r--r--   0        0        0    10248 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/configs.py
+-rw-r--r--   0        0        0      740 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/constants.py
+-rw-r--r--   0        0        0       75 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/data/__init__.py
+-rw-r--r--   0        0        0     3708 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/data/data_collators.py
+-rw-r--r--   0        0        0      129 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/data/datasets/__init__.py
+-rw-r--r--   0        0        0      339 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/data/datasets/dataset.py
+-rw-r--r--   0        0        0     3177 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/data/datasets/text_classification_dataset.py
+-rw-r--r--   0        0        0       26 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/data/utils/__init__.py
+-rw-r--r--   0        0        0     1547 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/data/utils/data_utils.py
+-rw-r--r--   0        0        0      127 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/embeddings/__init__.py
+-rw-r--r--   0        0        0     4146 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/embeddings/embedding.py
+-rw-r--r--   0        0        0     3122 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/embeddings/fasttext.py
+-rw-r--r--   0        0        0     3081 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/embeddings/word2vec.py
+-rw-r--r--   0        0        0      282 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/audio_classification/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/image2text/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/image2text/crnn/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/image2text/trocr/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/language_modeling/__init__.py
+-rw-r--r--   0        0        0       69 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/language_modeling/bert/__init__.py
+-rw-r--r--   0        0        0     1136 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/language_modeling/bert/bert_lm.py
+-rw-r--r--   0        0        0      720 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/language_modeling/bert/bert_lm_config.py
+-rw-r--r--   0        0        0       93 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/language_modeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     1208 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/language_modeling/distilbert/distilbert_lm.py
+-rw-r--r--   0        0        0      586 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
+-rw-r--r--   0        0        0       81 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/language_modeling/roberta/__init__.py
+-rw-r--r--   0        0        0     1172 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/language_modeling/roberta/roberta_lm.py
+-rw-r--r--   0        0        0      780 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/language_modeling/roberta/roberta_lm_config.py
+-rw-r--r--   0        0        0     9544 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/model.py
+-rw-r--r--   0        0        0        0 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/speech_recognition/wav2vec/__init__.py
+-rw-r--r--   0        0        0      240 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_classification/__init__.py
+-rw-r--r--   0        0        0      135 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_classification/bert/__init__.py
+-rw-r--r--   0        0        0     2679 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_classification/bert/bert_text_classification.py
+-rw-r--r--   0        0        0      808 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_classification/bert/bert_text_classification_config.py
+-rw-r--r--   0        0        0      159 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_classification/distilbert/__init__.py
+-rw-r--r--   0        0        0     2813 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_classification/distilbert/distilbert_text_classification.py
+-rw-r--r--   0        0        0      711 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
+-rw-r--r--   0        0        0      147 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_classification/roberta/__init__.py
+-rw-r--r--   0        0        0     2943 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_classification/roberta/roberta_text_classification.py
+-rw-r--r--   0        0        0      905 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_classification/roberta/roberta_text_classification_config.py
+-rw-r--r--   0        0        0        0 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_detection/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_detection/ctpn/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_detection/dbnet/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_summarization/__init__.py
+-rw-r--r--   0        0        0      104 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/preprocessors/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/preprocessors/normalizers/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/preprocessors/normalizers/nfkc.py
+-rw-r--r--   0        0        0        0 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/preprocessors/normalizers/nfkd.py
+-rw-r--r--   0        0        0        0 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/preprocessors/normalizers/normalizer.py
+-rw-r--r--   0        0        0     2218 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0      298 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/preprocessors/tokenizers/__init__.py
+-rw-r--r--   0        0        0     4623 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/preprocessors/tokenizers/bpe.py
+-rw-r--r--   0        0        0     5181 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
+-rw-r--r--   0        0        0    15394 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/preprocessors/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     4215 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/preprocessors/tokenizers/wordpiece.py
+-rw-r--r--   0        0        0     7443 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/registry.py
+-rw-r--r--   0        0        0       29 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/trainers/__init__.py
+-rw-r--r--   0        0        0    13853 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/trainers/trainer.py
+-rw-r--r--   0        0        0     1773 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/trainers/trainer_utils.py
+-rw-r--r--   0        0        0      135 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/utils/__init__.py
+-rw-r--r--   0        0        0     2435 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/utils/config_utils.py
+-rw-r--r--   0        0        0      482 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/utils/context_managers.py
+-rw-r--r--   0        0        0     2773 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/utils/hub_utils.py
+-rw-r--r--   0        0        0      374 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/utils/logging.py
+-rw-r--r--   0        0        0        0 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/utils/model_utils.py
+-rw-r--r--   0        0        0     1579 2023-06-30 06:57:28.304613 hezar-0.13.3/pyproject.toml
+-rw-r--r--   0        0        0     6604 1970-01-01 00:00:00.000000 hezar-0.13.3/PKG-INFO
```

### Comparing `hezar-0.12.0/LICENSE` & `hezar-0.13.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/README.md` & `hezar-0.13.3/README.md`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/builders.py` & `hezar-0.13.3/hezar/builders.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/configs.py` & `hezar-0.13.3/hezar/configs.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/constants.py` & `hezar-0.13.3/hezar/constants.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/data/data_collators.py` & `hezar-0.13.3/hezar/data/data_collators.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/data/datasets/text_classification_dataset.py` & `hezar-0.13.3/hezar/data/datasets/text_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/data/utils/data_utils.py` & `hezar-0.13.3/hezar/data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/embeddings/embedding.py` & `hezar-0.13.3/hezar/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/embeddings/fasttext.py` & `hezar-0.13.3/hezar/embeddings/fasttext.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/embeddings/word2vec.py` & `hezar-0.13.3/hezar/embeddings/word2vec.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/models/language_modeling/bert/bert_lm.py` & `hezar-0.13.3/hezar/models/language_modeling/bert/bert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/models/language_modeling/bert/bert_lm_config.py` & `hezar-0.13.3/hezar/models/language_modeling/bert/bert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/models/language_modeling/distilbert/distilbert_lm.py` & `hezar-0.13.3/hezar/models/language_modeling/distilbert/distilbert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py` & `hezar-0.13.3/hezar/models/language_modeling/distilbert/distilbert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/models/language_modeling/roberta/roberta_lm.py` & `hezar-0.13.3/hezar/models/language_modeling/roberta/roberta_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/models/language_modeling/roberta/roberta_lm_config.py` & `hezar-0.13.3/hezar/models/language_modeling/roberta/roberta_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/models/model.py` & `hezar-0.13.3/hezar/models/model.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/models/text_classification/bert/bert_text_classification.py` & `hezar-0.13.3/hezar/models/text_classification/bert/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/models/text_classification/bert/bert_text_classification_config.py` & `hezar-0.13.3/hezar/models/text_classification/bert/bert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py` & `hezar-0.13.3/hezar/models/text_classification/distilbert/distilbert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py` & `hezar-0.13.3/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/models/text_classification/roberta/roberta_text_classification.py` & `hezar-0.13.3/hezar/models/text_classification/roberta/roberta_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py` & `hezar-0.13.3/hezar/models/text_classification/roberta/roberta_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/preprocessors/preprocessor.py` & `hezar-0.13.3/hezar/preprocessors/preprocessor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/preprocessors/tokenizers/bpe.py` & `hezar-0.13.3/hezar/preprocessors/tokenizers/bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py` & `hezar-0.13.3/hezar/preprocessors/tokenizers/sentencepiece_bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/preprocessors/tokenizers/tokenizer.py` & `hezar-0.13.3/hezar/preprocessors/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/preprocessors/tokenizers/wordpiece.py` & `hezar-0.13.3/hezar/preprocessors/tokenizers/wordpiece.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/registry.py` & `hezar-0.13.3/hezar/registry.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/trainers/trainer.py` & `hezar-0.13.3/hezar/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/trainers/trainer_utils.py` & `hezar-0.13.3/hezar/trainers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/utils/config_utils.py` & `hezar-0.13.3/hezar/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/hezar/utils/hub_utils.py` & `hezar-0.13.3/hezar/utils/hub_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.12.0/pyproject.toml` & `hezar-0.13.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hezar"
-version = "0.12.0"
+version = "0.13.3"
 packages = [{ include = "hezar" }]
 description = "Hezar: A seamless AI framework & library for Persian"
 license = "MIT"
 authors = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 maintainers = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 repository = "https://github.com/hezarai/hezar"
 homepage = "https://github.com/hezarai"
```

### Comparing `hezar-0.12.0/PKG-INFO` & `hezar-0.13.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hezar
-Version: 0.12.0
+Version: 0.13.3
 Summary: Hezar: A seamless AI framework & library for Persian
 Home-page: https://github.com/hezarai
 License: MIT
 Keywords: packaging,poetry
 Author: Aryan Shekarlaban
 Author-email: arxyzan@gmail.com
 Maintainer: Aryan Shekarlaban
```

