# Comparing `tmp/xmen-0.9.6.tar.gz` & `tmp/xmen-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmen-0.9.6.tar", max compression
+gzip compressed data, was "xmen-0.9.7.tar", max compression
```

## Comparing `xmen-0.9.6.tar` & `xmen-0.9.7.tar`

### file list

```diff
@@ -1,62 +1,61 @@
--rw-r--r--   0        0        0    11357 2023-05-15 13:45:24.103799 xmen-0.9.6/LICENSE
--rw-r--r--   0        0        0     9296 2023-06-07 14:10:12.256707 xmen-0.9.6/README.md
--rw-r--r--   0        0        0     1061 2023-06-07 14:10:12.568713 xmen-0.9.6/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-15 13:45:25.657861 xmen-0.9.6/xmen/__init__.py
--rw-r--r--   0        0        0     5068 2023-05-15 13:45:25.694863 xmen-0.9.6/xmen/analysis.py
--rw-r--r--   0        0        0        0 2023-05-15 13:45:25.753865 xmen-0.9.6/xmen/cli/__init__.py
--rw-r--r--   0        0        0     7705 2023-06-07 14:10:12.598714 xmen-0.9.6/xmen/cli/cli.py
--rw-r--r--   0        0        0     2730 2023-06-07 14:10:12.635715 xmen-0.9.6/xmen/cli/dict.py
--rw-r--r--   0        0        0     2025 2023-06-07 14:10:12.647715 xmen-0.9.6/xmen/cli/index.py
--rw-r--r--   0        0        0     6382 2023-06-07 14:10:12.669715 xmen-0.9.6/xmen/cli/utils.py
--rw-r--r--   0        0        0      933 2023-05-15 13:45:25.945873 xmen-0.9.6/xmen/confhelper.py
--rw-r--r--   0        0        0      438 2023-05-24 13:46:51.901445 xmen-0.9.6/xmen/data/__init__.py
--rw-r--r--   0        0        0     2355 2023-05-24 13:46:51.921446 xmen-0.9.6/xmen/data/abbrevations.py
--rw-r--r--   0        0        0     4208 2023-05-16 20:37:32.693831 xmen-0.9.6/xmen/data/dataloaders.py
--rw-r--r--   0        0        0      698 2023-05-24 13:46:51.965447 xmen-0.9.6/xmen/data/filter.py
--rw-r--r--   0        0        0     2612 2023-05-15 13:45:26.087879 xmen-0.9.6/xmen/data/indexed_dataset.py
--rw-r--r--   0        0        0     1826 2023-05-15 13:45:26.092879 xmen-0.9.6/xmen/data/integrations.py
--rw-r--r--   0        0        0     1308 2023-05-24 13:46:51.969447 xmen-0.9.6/xmen/data/merge_concepts.py
--rw-r--r--   0        0        0     2386 2023-05-24 13:46:51.983447 xmen-0.9.6/xmen/data/retired_cuis.py
--rw-r--r--   0        0        0     2497 2023-05-24 13:46:52.000447 xmen-0.9.6/xmen/data/sampling.py
--rw-r--r--   0        0        0     2093 2023-05-24 13:46:52.039448 xmen-0.9.6/xmen/data/semantic_groups.py
--rw-r--r--   0        0        0     2577 2023-05-24 13:46:52.043448 xmen-0.9.6/xmen/data/semantic_types.py
--rw-r--r--   0        0        0     3228 2023-05-15 13:45:26.105879 xmen-0.9.6/xmen/data/util.py
--rw-r--r--   0        0        0    15495 2023-06-07 14:10:12.715716 xmen-0.9.6/xmen/evaluation.py
--rw-r--r--   0        0        0    18453 2023-05-16 10:44:55.440426 xmen-0.9.6/xmen/ext/neleval/annotation.py
--rw-r--r--   0        0        0    10874 2023-05-16 10:44:55.511428 xmen-0.9.6/xmen/ext/neleval/configs.py
--rw-r--r--   0        0        0     5429 2023-05-16 10:45:41.591263 xmen-0.9.6/xmen/ext/neleval/document.py
--rw-r--r--   0        0        0    10926 2023-05-16 10:44:55.603432 xmen-0.9.6/xmen/ext/neleval/evaluate.py
--rw-r--r--   0        0        0     5788 2023-05-16 10:44:55.635434 xmen-0.9.6/xmen/ext/neleval/prepare.py
--rw-r--r--   0        0        0     1086 2023-05-15 13:45:26.162881 xmen-0.9.6/xmen/ext/sapbert/LICENSE
--rw-r--r--   0        0        0     4663 2023-05-15 13:45:26.179882 xmen-0.9.6/xmen/ext/sapbert/README.md
--rw-r--r--   0        0        0      146 2023-05-15 13:45:26.202883 xmen-0.9.6/xmen/ext/sapbert/requirements.txt
--rwxr-xr-x   0        0        0      307 2023-05-15 13:45:26.250885 xmen-0.9.6/xmen/ext/sapbert/src/__init__.py
--rwxr-xr-x   0        0        0    11519 2023-05-16 19:26:23.559730 xmen-0.9.6/xmen/ext/sapbert/src/data_loader.py
--rwxr-xr-x   0        0        0     4898 2023-05-15 13:45:26.277886 xmen-0.9.6/xmen/ext/sapbert/src/metric_learning.py
--rwxr-xr-x   0        0        0     6626 2023-05-15 13:45:26.301887 xmen-0.9.6/xmen/ext/sapbert/src/model_wrapper.py
--rw-r--r--   0        0        0      533 2023-05-15 13:45:26.317888 xmen-0.9.6/xmen/ext/sapbert/train/.gitignore
--rwxr-xr-x   0        0        0      466 2023-05-15 13:45:26.320888 xmen-0.9.6/xmen/ext/sapbert/train/pretrain.sh
--rwxr-xr-x   0        0        0    10943 2023-05-15 13:45:26.338889 xmen-0.9.6/xmen/ext/sapbert/train/train.py
--rwxr-xr-x   0        0        0      522 2023-05-15 13:45:26.363890 xmen-0.9.6/xmen/ext/sapbert/train/xling_train.sh
--rw-r--r--   0        0        0     7632 2023-05-16 11:07:29.587327 xmen-0.9.6/xmen/ext/scispacy/umls_utils.py
--rw-r--r--   0        0        0     6328 2023-05-24 13:46:52.063449 xmen-0.9.6/xmen/kb.py
--rw-r--r--   0        0        0     1628 2023-05-15 13:45:26.428892 xmen-0.9.6/xmen/linkers/__init__.py
--rw-r--r--   0        0        0     6220 2023-06-07 14:10:12.732716 xmen-0.9.6/xmen/linkers/ensemble.py
--rw-r--r--   0        0        0     8770 2023-05-15 13:45:26.488895 xmen-0.9.6/xmen/linkers/faiss_indexer.py
--rw-r--r--   0        0        0     9722 2023-06-07 14:10:12.746717 xmen-0.9.6/xmen/linkers/sap_bert_linker.py
--rw-r--r--   0        0        0     9442 2023-05-24 13:46:52.069449 xmen-0.9.6/xmen/linkers/tf_idf_ngram_linker.py
--rw-r--r--   0        0        0      916 2023-05-15 13:45:26.567898 xmen-0.9.6/xmen/linkers/util.py
--rw-r--r--   0        0        0      510 2023-05-15 13:45:26.587899 xmen-0.9.6/xmen/log.py
--rw-r--r--   0        0        0      452 2023-05-15 13:45:26.881910 xmen-0.9.6/xmen/reranking/__init__.py
--rw-r--r--   0        0        0    20918 2023-06-07 14:10:12.760717 xmen-0.9.6/xmen/reranking/cross_encoder.py
--rw-r--r--   0        0        0     9852 2023-05-15 13:45:26.951913 xmen-0.9.6/xmen/reranking/list_wise.py
--rw-r--r--   0        0        0     5179 2023-05-15 13:45:26.990915 xmen-0.9.6/xmen/reranking/multiple_choice_util.py
--rw-r--r--   0        0        0     4914 2023-05-15 13:45:27.008916 xmen-0.9.6/xmen/reranking/ranking_util.py
--rw-r--r--   0        0        0     1160 2023-05-15 13:45:27.045917 xmen-0.9.6/xmen/reranking/rule_based.py
--rw-r--r--   0        0        0    14470 2023-06-07 14:10:12.815718 xmen-0.9.6/xmen/reranking/scored_cross_encoder.py
--rw-r--r--   0        0        0        0 2023-05-15 13:45:27.128920 xmen-0.9.6/xmen/resources/.gitkeep
--rw-r--r--   0        0        0       70 2023-05-15 13:45:27.132920 xmen-0.9.6/xmen/resources/Readme.md
--rw-r--r--   0        0        0     5743 2023-05-15 13:45:27.176922 xmen-0.9.6/xmen/resources/SemGroups-v03.txt
--rw-r--r--   0        0        0     5468 2023-05-15 13:45:27.211923 xmen-0.9.6/xmen/resources/SemGroups.txt
--rw-r--r--   0        0        0    10168 2023-05-16 20:37:32.742833 xmen-0.9.6/xmen/umls.py
--rw-r--r--   0        0        0    10679 1970-01-01 00:00:00.000000 xmen-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-15 13:45:24.103799 xmen-0.9.7/LICENSE
+-rw-r--r--   0        0        0     9196 2023-06-30 08:19:16.677129 xmen-0.9.7/README.md
+-rw-r--r--   0        0        0     1472 2023-06-30 08:21:56.435624 xmen-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0      162 2023-06-18 17:41:07.071750 xmen-0.9.7/xmen/__init__.py
+-rw-r--r--   0        0        0     5068 2023-05-15 13:45:25.694863 xmen-0.9.7/xmen/analysis.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:45:25.753865 xmen-0.9.7/xmen/cli/__init__.py
+-rw-r--r--   0        0        0     7505 2023-06-18 17:41:02.552568 xmen-0.9.7/xmen/cli/cli.py
+-rw-r--r--   0        0        0     2730 2023-06-07 14:10:12.635715 xmen-0.9.7/xmen/cli/dict.py
+-rw-r--r--   0        0        0     2077 2023-06-30 08:19:17.657151 xmen-0.9.7/xmen/cli/index.py
+-rw-r--r--   0        0        0     5514 2023-06-18 17:41:02.573569 xmen-0.9.7/xmen/cli/utils.py
+-rw-r--r--   0        0        0      930 2023-06-18 17:41:05.898702 xmen-0.9.7/xmen/confhelper.py
+-rw-r--r--   0        0        0      411 2023-06-18 17:41:04.453644 xmen-0.9.7/xmen/data/__init__.py
+-rw-r--r--   0        0        0     2355 2023-05-24 13:46:51.921446 xmen-0.9.7/xmen/data/abbrevations.py
+-rw-r--r--   0        0        0      698 2023-05-24 13:46:51.965447 xmen-0.9.7/xmen/data/filter.py
+-rw-r--r--   0        0        0     2612 2023-05-15 13:45:26.087879 xmen-0.9.7/xmen/data/indexed_dataset.py
+-rw-r--r--   0        0        0     1826 2023-05-15 13:45:26.092879 xmen-0.9.7/xmen/data/integrations.py
+-rw-r--r--   0        0        0     1308 2023-05-24 13:46:51.969447 xmen-0.9.7/xmen/data/merge_concepts.py
+-rw-r--r--   0        0        0     2386 2023-05-24 13:46:51.983447 xmen-0.9.7/xmen/data/retired_cuis.py
+-rw-r--r--   0        0        0     2497 2023-05-24 13:46:52.000447 xmen-0.9.7/xmen/data/sampling.py
+-rw-r--r--   0        0        0     2093 2023-05-24 13:46:52.039448 xmen-0.9.7/xmen/data/semantic_groups.py
+-rw-r--r--   0        0        0     2577 2023-05-24 13:46:52.043448 xmen-0.9.7/xmen/data/semantic_types.py
+-rw-r--r--   0        0        0     3228 2023-05-15 13:45:26.105879 xmen-0.9.7/xmen/data/util.py
+-rw-r--r--   0        0        0    15484 2023-06-18 17:41:04.457644 xmen-0.9.7/xmen/evaluation.py
+-rw-r--r--   0        0        0    18453 2023-05-16 10:44:55.440426 xmen-0.9.7/xmen/ext/neleval/annotation.py
+-rw-r--r--   0        0        0    10874 2023-05-16 10:44:55.511428 xmen-0.9.7/xmen/ext/neleval/configs.py
+-rw-r--r--   0        0        0     5429 2023-05-16 10:45:41.591263 xmen-0.9.7/xmen/ext/neleval/document.py
+-rw-r--r--   0        0        0    10926 2023-05-16 10:44:55.603432 xmen-0.9.7/xmen/ext/neleval/evaluate.py
+-rw-r--r--   0        0        0     5788 2023-05-16 10:44:55.635434 xmen-0.9.7/xmen/ext/neleval/prepare.py
+-rw-r--r--   0        0        0     1086 2023-05-15 13:45:26.162881 xmen-0.9.7/xmen/ext/sapbert/LICENSE
+-rw-r--r--   0        0        0     4663 2023-05-15 13:45:26.179882 xmen-0.9.7/xmen/ext/sapbert/README.md
+-rw-r--r--   0        0        0      146 2023-05-15 13:45:26.202883 xmen-0.9.7/xmen/ext/sapbert/requirements.txt
+-rwxr-xr-x   0        0        0      307 2023-05-15 13:45:26.250885 xmen-0.9.7/xmen/ext/sapbert/src/__init__.py
+-rwxr-xr-x   0        0        0    11519 2023-05-16 19:26:23.559730 xmen-0.9.7/xmen/ext/sapbert/src/data_loader.py
+-rwxr-xr-x   0        0        0     4898 2023-05-15 13:45:26.277886 xmen-0.9.7/xmen/ext/sapbert/src/metric_learning.py
+-rwxr-xr-x   0        0        0     6626 2023-05-15 13:45:26.301887 xmen-0.9.7/xmen/ext/sapbert/src/model_wrapper.py
+-rw-r--r--   0        0        0      533 2023-05-15 13:45:26.317888 xmen-0.9.7/xmen/ext/sapbert/train/.gitignore
+-rwxr-xr-x   0        0        0      466 2023-05-15 13:45:26.320888 xmen-0.9.7/xmen/ext/sapbert/train/pretrain.sh
+-rwxr-xr-x   0        0        0    10943 2023-05-15 13:45:26.338889 xmen-0.9.7/xmen/ext/sapbert/train/train.py
+-rwxr-xr-x   0        0        0      522 2023-05-15 13:45:26.363890 xmen-0.9.7/xmen/ext/sapbert/train/xling_train.sh
+-rw-r--r--   0        0        0     7632 2023-05-16 11:07:29.587327 xmen-0.9.7/xmen/ext/scispacy/umls_utils.py
+-rw-r--r--   0        0        0     6255 2023-06-18 17:41:08.611811 xmen-0.9.7/xmen/kb.py
+-rw-r--r--   0        0        0     2271 2023-06-30 08:19:17.736153 xmen-0.9.7/xmen/linkers/__init__.py
+-rw-r--r--   0        0        0     6866 2023-06-30 08:19:17.767153 xmen-0.9.7/xmen/linkers/ensemble.py
+-rw-r--r--   0        0        0     8770 2023-05-15 13:45:26.488895 xmen-0.9.7/xmen/linkers/faiss_indexer.py
+-rw-r--r--   0        0        0     9721 2023-06-18 17:41:02.764576 xmen-0.9.7/xmen/linkers/sap_bert_linker.py
+-rw-r--r--   0        0        0     9442 2023-05-24 13:46:52.069449 xmen-0.9.7/xmen/linkers/tf_idf_ngram_linker.py
+-rw-r--r--   0        0        0      916 2023-05-15 13:45:26.567898 xmen-0.9.7/xmen/linkers/util.py
+-rw-r--r--   0        0        0      510 2023-05-15 13:45:26.587899 xmen-0.9.7/xmen/log.py
+-rw-r--r--   0        0        0      452 2023-05-15 13:45:26.881910 xmen-0.9.7/xmen/reranking/__init__.py
+-rw-r--r--   0        0        0    21046 2023-06-30 08:19:17.811154 xmen-0.9.7/xmen/reranking/cross_encoder.py
+-rw-r--r--   0        0        0     9852 2023-05-15 13:45:26.951913 xmen-0.9.7/xmen/reranking/list_wise.py
+-rw-r--r--   0        0        0     5179 2023-05-15 13:45:26.990915 xmen-0.9.7/xmen/reranking/multiple_choice_util.py
+-rw-r--r--   0        0        0     4914 2023-05-15 13:45:27.008916 xmen-0.9.7/xmen/reranking/ranking_util.py
+-rw-r--r--   0        0        0     1160 2023-05-15 13:45:27.045917 xmen-0.9.7/xmen/reranking/rule_based.py
+-rw-r--r--   0        0        0    14257 2023-06-30 08:19:17.865156 xmen-0.9.7/xmen/reranking/scored_cross_encoder.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:45:27.128920 xmen-0.9.7/xmen/resources/.gitkeep
+-rw-r--r--   0        0        0       70 2023-05-15 13:45:27.132920 xmen-0.9.7/xmen/resources/Readme.md
+-rw-r--r--   0        0        0     5743 2023-05-15 13:45:27.176922 xmen-0.9.7/xmen/resources/SemGroups-v03.txt
+-rw-r--r--   0        0        0     5468 2023-05-15 13:45:27.211923 xmen-0.9.7/xmen/resources/SemGroups.txt
+-rw-r--r--   0        0        0    10168 2023-05-16 20:37:32.742833 xmen-0.9.7/xmen/umls.py
+-rw-r--r--   0        0        0    10618 1970-01-01 00:00:00.000000 xmen-0.9.7/PKG-INFO
```

### Comparing `xmen-0.9.6/LICENSE` & `xmen-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/README.md` & `xmen-0.9.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -139,40 +139,32 @@
 
 xMEN provides implementations of different neural and non-neural candidate generators
 
 ### TF-IDF Weighted Character N-grams
 
 Based on the implementation from [scispaCy](https://github.com/allenai/scispacy).
 
-YAML file:
-
-```
-linker:
-  candidate_generation:
-    ngram: ~
-```
-
 Run `xmen index my_config.yaml --ngram` or `xmen index my_config.yaml --all` to create the index.
 
 To use the linker at runtime, pass the index folder as an argument:
 
 ```
 from xmen.linkers import TFIDFNGramLinker
 
 ngram_linker = TFIDFNGramLinker(index_base_path="/path/to/my/index/ngram", k=100)
 predictions = ngram_linker.predict_batch(dataset)
 ```
 
-Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
+Example usage: see [BioASQ / DisTEMIST Notebook](notebooks/examples/01_BioASQ_DisTEMIST.ipynb)
 
 ### SapBERT
 
 Dense Retrieval based on [SapBERT](https://github.com/cambridgeltl/sapbert) embeddings.
 
-YAML file:
+YAML file (optional, if you want to configure another Transformer model):
 
 ```
 linker:
   candidate_generation:
     sapbert:
       model_name: cambridgeltl/SapBERT-UMLS-2020AB-all-lang-from-XLMR
 ```
@@ -195,15 +187,15 @@
 
 ```
 sapbert_linker = SapBERTLinker(**config)
 ```
 
 By default, SapBERT assumes a CUDA device is available. If you want to disable cuda, pass `cuda=False` to the constructor.
 
-Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
+Example usage: see [BioASQ / DisTEMIST Notebook](notebooks/examples/01_BioASQ_DisTEMIST.ipynb)
 
 ### Ensemble
 
 Different candidate generators often work well for different kinds of entity mentions, and it can be helpful to combine their predictions.
 
 In xMEN, this can be easily achieved with an `EnsembleLinker`:
 
@@ -219,17 +211,15 @@
 
 Sometimes, you want to compare the ensemble performance to individual linkers and already have the candidate lists. To avoid recomputation, you can use the `reuse_preds` argument:
 
 ```
 prediction = ensemble_linker.predict_batch(dataset, 128, 100, reuse_preds={'sapbert' : predictions_sap, 'ngram' : predictions_ngram'})
 ```
 
-Note: `reuse_preds` currently does not support Hugging Face `DatasetDict` objects, so you would have to call it on each split individually.
-
-Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
+Example usage: see [BioASQ / DisTEMIST Notebook](notebooks/examples/examples/01_BioASQ_DisTEMIST.ipynb)
 
 ## 🌀 Rerankers
 
 ### Cross-Encoder Reranker
 
 When labelled training data is available, a trainable reranker can improve ranking of candidate lists a lot.
 
@@ -266,15 +256,15 @@
 # Fit the model
 rr.fit(args, cross_enc_ds['train'].dataset, cross_enc_ds['validation'].dataset)
 
 # Predict on test set
 prediction = rr.rerank_batch(candidates['test'], cross_enc_ds['test'])
 ```
 
-Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
+Example usage: see [BioASQ / DisTEMIST Notebook](notebooks/examples/01_BioASQ_DisTEMIST.ipynb)
 
 ### Rule-based Reranker
 
 TODO
 
 ## 💡 Pre- and Post-Processing
 
@@ -286,12 +276,12 @@
 - [Filtering by UMLS semantic types](xmen/data/semantic_types.py)
 - [Replacement of retired CUIS](xmen/data/retired_cuis.py)
 
 ## 📊 Evaluation
 
 xMEN provides implementations of common entity linking metrics (e.g., a wrapper for [neleval](https://github.com/wikilinks/neleval))
 
-Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
+Example usage: see [BioASQ / DisTEMIST Notebook](notebooks/examples/01_BioASQ_DisTEMIST.ipynb)
 
 ## 📈 Benchmark Results
 
 TODO
```

### Comparing `xmen-0.9.6/pyproject.toml` & `xmen-0.9.7/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xmen"
-version = "0.9.6"
+version = "0.9.7"
 description = "An extensible toolkit for Cross-lingual (x) Medical Entity Normalization."
 license = "Apache-2.0"
 authors = ["Florian Borchert <florian.borchert@hpi.de>"]
 readme = "README.md"
 repository = "https://github.com/hpi-dhc/xmen"
 
 [tool.poetry.scripts]
@@ -24,18 +24,27 @@
 langcodes = "^3.3.0"
 rich = "^12.3.0"
 torch = "^1.13.0"
 scispacy = "^0.5.2"
 sentence-transformers = "^2.2.2"
 faiss-gpu = {version = "^1.7.1", markers = 'sys_platform == "linux"'}
 faiss-cpu = {version = "^1.7.1", markers = 'sys_platform != "linux"'}
+orjson = "^3.9.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.0"
 black = "^22.12.0"
+hydra-core = "^1.3.2"
+en-core-sci-sm = {url = "https://s3-us-west-2.amazonaws.com/ai2-s2-scispacy/releases/v0.5.1/en_core_sci_sm-0.5.1.tar.gz"}
+# TODO: only needed for Mantra benchmark, as dataset is not on HF hub
+bigbio = {git = "https://github.com/bigscience-workshop/biomedical.git", branch="main"}
+
+[tool.poetry.group.dev.dependencies]
+wandb = "^0.15.4"
+hydra-submitit-launcher = "^1.2.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `xmen-0.9.6/xmen/analysis.py` & `xmen-0.9.7/xmen/analysis.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/cli/cli.py` & `xmen-0.9.7/xmen/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,26 +129,24 @@
         logger.warn("Please indicate which indicess to build with --sapbert or --ngram or --all.")
         raise typer.Exit()
 
     if os.path.exists(dict):
         logger.info(f"Dictionary found in {dict}. Attempting to build indices.")
 
         is_ngram_selected = ngram or all
-        required_key = "linker.candidate_generation.ngram"
         write_path = output / "index" / "ngrams"
-        if is_ngram_selected and has_correct_keys(cfg, required_key) and can_write(write_path, overwrite):
+        if is_ngram_selected and can_write(write_path, overwrite):
             logger.info("Building N-Gram index.")
             build_ngram(cfg, output, dict)
         else:
             logger.info("Skipping N-Gram index.")
 
         is_sapbert_selected = sapbert or all
-        required_key = "linker.candidate_generation.sapbert"
         write_path = output / "index" / "sapbert"
-        if is_sapbert_selected and has_correct_keys(cfg, required_key) and can_write(write_path, overwrite):
+        if is_sapbert_selected and can_write(write_path, overwrite):
             # check for GPUs
             if torch.cuda.is_available():
                 logger.info(f"CUDA is available. Running on GPU with ID {gpu_id}. To select another, use --gpu-id.")
             else:
                 gpu_id = -1
                 logger.warning(
                     "CUDA is not available on this system. Running on CPU. This can take considerably longer."
```

### Comparing `xmen-0.9.6/xmen/cli/dict.py` & `xmen-0.9.7/xmen/cli/dict.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/cli/index.py` & `xmen-0.9.7/xmen/cli/index.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from omegaconf import DictConfig
+from omegaconf import DictConfig, OmegaConf
 from ..log import logger
 from xmen.kb import create_flat_term_dict
 from xmen.linkers import TFIDFNGramLinker, SapBERTLinker
 from pathlib import Path
 import torch
 
 
@@ -36,18 +36,18 @@
     # ensure the index folder exists
     work_dir.parent.mkdir(exist_ok=True, parents=True)
     # SapBERT indices
     term_dict = create_flat_term_dict([dict_dir])
     logger.info(f"Number of aliases: {len(term_dict)}.")
     logger.info(f"Number of concepts: {len(term_dict.cui.unique())}.")
 
-    sapbert_cfg = cfg.linker.candidate_generation.sapbert
-    model_name = SapBERTLinker.CROSS_LINGUAL  # default model
-    if sapbert_cfg and "model_name" in sapbert_cfg:
-        model_name = sapbert_cfg.model_name
+    if cfg.get("linker", {}).get("candidate_generation", {}).get("sapbert", {}).get("model_name", {}) == {}:
+        model_name = SapBERTLinker.CROSS_LINGUAL  # default model
+    else:
+        model_name = cfg.linker.candidate_generation.sapbert.model_name
 
     cuda = False if gpu_id == -1 else True
     with torch.cuda.device(gpu_id):
         SapBERTLinker.write_index(
             work_dir / "index" / "sapbert",
             term_dict=term_dict,
             cuda=cuda,
```

### Comparing `xmen-0.9.6/xmen/cli/utils.py` & `xmen-0.9.7/xmen/cli/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -131,38 +131,14 @@
         if overwrite not in ["n", "y"]:
             logger.warn("Unhandled value. Please type `y` for yes or `n` for no.")
             overwrite = can_write(path, parent_overwrite)
 
         return True if overwrite == "y" else False
 
 
-def has_correct_keys(cfg, proper_nested_keys: str) -> bool:
-    """
-    Checks whether the provided configuration dictionary has the specified nested keys.
-
-    Args:
-    - cfg (dict): The configuration dictionary to check.
-    - proper_nested_keys (str): The required nested keys in the configuration, separated by dots.
-
-    Returns:
-    - (bool): True if the dictionary has the required keys, False otherwise.
-    """
-    nested_keys = proper_nested_keys.split(".")
-    for key in nested_keys:
-        if key not in cfg:
-            logger.error(
-                f"The command requires the key `{proper_nested_keys}` to be set in the config .yaml file (in that "
-                "specific nested structure)."
-            )
-            return False
-        cfg = cfg[key]
-    logger.info(f"Key {proper_nested_keys} correctly found in .yaml file.")
-    return True
-
-
 def get_alias_count(concept_details):
     """
     Calculates the total number of aliases in the given concept_details dictionary.
 
     Args:
     - concept_details (dict): A dictionary containing details of concepts and their aliases.
```

### Comparing `xmen-0.9.6/xmen/confhelper.py` & `xmen-0.9.7/xmen/confhelper.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,10 +17,10 @@
         configuration file with the current configuration file. The base configuration file should be a YAML file as well,
         and its path is relative to the current configuration file's directory.
 
     """
     path = Path(file_name)
     conf = OmegaConf.load(path)
     if base_config_path := conf.get("base_config", None):
-        base_conf = OmegaConf.load(path.parent / base_config_path)
+        base_conf = load_config(path.parent / base_config_path)
         conf = OmegaConf.merge(base_conf, conf)
     return conf
```

### Comparing `xmen-0.9.6/xmen/data/abbrevations.py` & `xmen-0.9.7/xmen/data/abbrevations.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/data/filter.py` & `xmen-0.9.7/xmen/data/filter.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/data/indexed_dataset.py` & `xmen-0.9.7/xmen/data/indexed_dataset.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/data/integrations.py` & `xmen-0.9.7/xmen/data/integrations.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/data/merge_concepts.py` & `xmen-0.9.7/xmen/data/merge_concepts.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/data/retired_cuis.py` & `xmen-0.9.7/xmen/data/retired_cuis.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/data/sampling.py` & `xmen-0.9.7/xmen/data/sampling.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/data/semantic_groups.py` & `xmen-0.9.7/xmen/data/semantic_groups.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/data/semantic_types.py` & `xmen-0.9.7/xmen/data/semantic_types.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/data/util.py` & `xmen-0.9.7/xmen/data/util.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/evaluation.py` & `xmen-0.9.7/xmen/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import imp
 from typing import Iterable
 from itertools import groupby
 import pandas as pd
 import warnings
 
 from .ext.neleval.prepare import SelectAlternatives
 from .ext.neleval.document import Document
```

### Comparing `xmen-0.9.6/xmen/ext/neleval/annotation.py` & `xmen-0.9.7/xmen/ext/neleval/annotation.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/ext/neleval/configs.py` & `xmen-0.9.7/xmen/ext/neleval/configs.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/ext/neleval/document.py` & `xmen-0.9.7/xmen/ext/neleval/document.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/ext/neleval/evaluate.py` & `xmen-0.9.7/xmen/ext/neleval/evaluate.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/ext/neleval/prepare.py` & `xmen-0.9.7/xmen/ext/neleval/prepare.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/ext/sapbert/LICENSE` & `xmen-0.9.7/xmen/ext/sapbert/LICENSE`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/ext/sapbert/README.md` & `xmen-0.9.7/xmen/ext/sapbert/README.md`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/ext/sapbert/src/data_loader.py` & `xmen-0.9.7/xmen/ext/sapbert/src/data_loader.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/ext/sapbert/src/metric_learning.py` & `xmen-0.9.7/xmen/ext/sapbert/src/metric_learning.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/ext/sapbert/src/model_wrapper.py` & `xmen-0.9.7/xmen/ext/sapbert/src/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/ext/sapbert/train/.gitignore` & `xmen-0.9.7/xmen/ext/sapbert/train/.gitignore`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/ext/sapbert/train/train.py` & `xmen-0.9.7/xmen/ext/sapbert/train/train.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/ext/sapbert/train/xling_train.sh` & `xmen-0.9.7/xmen/ext/sapbert/train/xling_train.sh`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/ext/scispacy/umls_utils.py` & `xmen-0.9.7/xmen/ext/scispacy/umls_utils.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/kb.py` & `xmen-0.9.7/xmen/kb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from collections import defaultdict
-import json
+import orjson
 from pathlib import Path
 from typing import List, Union
 import pandas as pd
 from scispacy.linking_utils import KnowledgeBase, Entity
 from collections.abc import Mapping
 
 
-def load_kb(file_path: Union[str, Path]):
+def load_kb(file_path: Union[str, Path]) -> KnowledgeBase:
     return CompositeKnowledgebase([file_path])
 
 
 class CompositeKnowledgebase(KnowledgeBase):
     """
     Initializes a CompositeKnowledgebase object with the given list of file paths and optional list of mappers.
 
@@ -37,37 +37,36 @@
         assert len(mappers) == len(file_paths)
         alias_to_cuis = defaultdict(set)
         self.cui_to_entity = {}
 
         for file_path, mapper in zip(file_paths, mappers):
             file_path = Path(file_path)
             assert file_path.suffix == ".jsonl"
-            raw = [json.loads(line) for line in open(file_path)]
+            raw = [orjson.loads(line) for line in open(file_path)]
 
             for entry in raw:
                 if mapper:
                     entry = mapper(entry)
                 if not entry:
                     continue
                 if type(entry) != list:
                     entry = [entry]
                 for concept in entry:
                     if type(concept["concept_id"]) == int:
                         concept["concept_id"] = str(concept["concept_id"])
+                    cui = concept["concept_id"]
                     unique_aliases = set(concept["aliases"])
                     if "canonical_name" in concept:
                         unique_aliases.add(concept["canonical_name"])
                     for alias in unique_aliases:
-                        alias_to_cuis[alias].add(concept["concept_id"])
-                    if not concept["concept_id"] in self.cui_to_entity:
-                        self.cui_to_entity[concept["concept_id"]] = Entity(**concept)
+                        alias_to_cuis[alias].add(cui)
+                    if not cui in self.cui_to_entity:
+                        self.cui_to_entity[cui] = Entity(**concept)
                     else:
-                        self.cui_to_entity[concept["concept_id"]] = _merge_entities(
-                            Entity(**concept), self.cui_to_entity[concept["concept_id"]]
-                        )
+                        self.cui_to_entity[cui] = _merge_entities(Entity(**concept), self.cui_to_entity[cui])
 
             self.alias_to_cuis = {**alias_to_cuis}
 
 
 def _merge_entities(e1: Entity, e2: Entity):
     """
     Merges two entities and returns the resulting entity. The two entities must have the same concept ID.
@@ -118,15 +117,15 @@
     term_dict = []
     if not mappers:
         mappers = [lambda x: x] * len(concept_names_jsonl)
     assert len(mappers) == len(concept_names_jsonl)
     for jsonl_file, mapper in zip(concept_names_jsonl, mappers):
         with open(jsonl_file) as f:
             for entry in f:
-                entry = json.loads(entry)
+                entry = orjson.loads(entry)
                 if mapper != None:
                     entry = mapper(entry)
                     if not entry:
                         continue
                 if type(entry) != list:
                     entry = [entry]
                 for e in entry:
```

### Comparing `xmen-0.9.6/xmen/linkers/__init__.py` & `xmen-0.9.7/xmen/linkers/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # pylint: disable=g-import-not-at-top,g-bad-import-order,wrong-import-position
 
 from abc import ABC, abstractmethod
 from datasets.arrow_dataset import Dataset
-import logging
+from pathlib import Path
+from xmen.log import logger
 
 from xmen.reranking import Reranker
 
-logger = logging.getLogger("transformers")
-
 
 class EntityLinker(ABC):
     def predict_batch(self, dataset: Dataset, batch_size: int = None) -> Dataset:
         """Naive default implementation of batch prediction.
         Should be overridden if the particular model provides an efficient way to predict in batch (e.g., on a GPU)
 
         Args:
@@ -45,7 +44,24 @@
     def predict(self, passages: list, entities: list) -> list:
         raise NotImplementedError()
 
 
 from .tf_idf_ngram_linker import TFIDFNGramLinker
 from .sap_bert_linker import SapBERTLinker
 from .ensemble import EnsembleLinker
+
+
+def default_ensemble(index_base_path, k_ngram=100, k_sapbert=1000, k_ensemble=64):
+    """
+    Creates the default ensemble candidate generator consisting of equally weighted SapBERT and TF-IDF N-Gram Linker
+    """
+    index_base_path = Path(index_base_path)
+    ngram_linker = TFIDFNGramLinker(index_base_path=index_base_path / "ngrams", k=k_ngram)
+
+    SapBERTLinker.clear()
+    sapbert_linker = SapBERTLinker(index_base_path=index_base_path / "sapbert", k=k_sapbert)
+
+    ensemble = EnsembleLinker()
+    ensemble.add_linker("ngram", ngram_linker, k=k_ngram)
+    ensemble.add_linker("sapbert", sapbert_linker, k=k_sapbert)
+
+    return ensemble
```

### Comparing `xmen-0.9.6/xmen/linkers/ensemble.py` & `xmen-0.9.7/xmen/linkers/ensemble.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Dict
 from xmen.linkers import EntityLinker
 from .util import filter_and_apply_threshold
-from datasets import Dataset, utils
-import numpy as np
+from datasets import Dataset, utils, DatasetDict
 import itertools
 
 
 class EnsembleLinker(EntityLinker):
     """
     A class for combining multiple entity linking models together into an ensemble.
 
@@ -66,27 +65,26 @@
         - top_k: an optional integer representing the number of top entities to keep per document
         - reuse_preds: an optional dictionary of precomputed predictions for each linker
 
         Returns:
         - a dictionary containing the predicted entities for each document in the dataset
         """
 
-        def merge_linkers(batch, index):
+        def merge_linkers(batch, index, reuse_preds_split=None):
             progress = utils.logging.is_progress_bar_enabled()
             try:
                 mapped = {}
                 if progress:
                     utils.logging.disable_progress_bar()
 
                 for linker_name, linker_fn in self.linkers_fn.items():
-                    if reuse_preds:
-                        linked = reuse_preds[linker_name].select(index)
+                    if reuse_preds_split:
+                        linked = reuse_preds_split[linker_name].select(index)
                     else:
                         linker = linker_fn()
-                        self.get_logger().info(f"Running{linker_name}")
                         linked = linker.predict_batch(Dataset.from_dict(batch), batch_size)
                     mapped[linker_name] = filter_and_apply_threshold(
                         linked,
                         self.linkers_k[linker_name],
                         self.linker_thresholds[linker_name],
                     )["entities"]
 
@@ -124,17 +122,33 @@
 
                     entities.append(doc)
             finally:
                 if progress:
                     utils.logging.enable_progress_bar()
             return {"entities": entities}
 
-        return dataset.map(
-            merge_linkers,
-            with_indices=True,
-            batched=True,
-            batch_size=batch_size,
-            load_from_cache_file=False,
-        )
+        if type(dataset) == DatasetDict:
+            return DatasetDict(
+                {
+                    split: dataset[split].map(
+                        lambda b, i: merge_linkers(
+                            b, i, {linker: v[split] for linker, v in reuse_preds.items()} if reuse_preds else None
+                        ),
+                        with_indices=True,
+                        batched=True,
+                        batch_size=batch_size,
+                        load_from_cache_file=False,
+                    )
+                    for split in dataset.keys()
+                }
+            )
+        else:
+            return dataset.map(
+                lambda b, i: merge_linkers(b, i, reuse_preds),
+                with_indices=True,
+                batched=True,
+                batch_size=batch_size,
+                load_from_cache_file=False,
+            )
 
     def predict(self, unit: str, entities: dict) -> dict:
         raise NotImplementedError()
```

### Comparing `xmen-0.9.6/xmen/linkers/faiss_indexer.py` & `xmen-0.9.7/xmen/linkers/faiss_indexer.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/linkers/sap_bert_linker.py` & `xmen-0.9.7/xmen/linkers/sap_bert_linker.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,14 @@
             load_from_cache_file=False,
         )
 
     def predict(self, unit: str, entities: dict) -> dict:
         raise NotImplementedError()
 
     def _get_concepts(self, mention_candidates):
-
         logger.debug(f"Calculate embeddings for {len(mention_candidates)} mentions")
         mention_dense_embeds = SapBERTLinker.model_wrapper.embed_dense(
             mention_candidates,
             show_progress=False,
             agg_mode="cls",
             use_cuda=self.cuda,
             batch_size=self.gpu_batch_size,
```

### Comparing `xmen-0.9.6/xmen/linkers/tf_idf_ngram_linker.py` & `xmen-0.9.7/xmen/linkers/tf_idf_ngram_linker.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/linkers/util.py` & `xmen-0.9.7/xmen/linkers/util.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/reranking/cross_encoder.py` & `xmen-0.9.7/xmen/reranking/cross_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
 
     def __init__(
         self,
         num_train_epochs: int,
         model_name: str = "bert-base-multilingual-cased",
         fp16: bool = True,
         label_smoothing: bool = False,
-        score_regularization: bool = False,
+        score_regularization: bool = 1.0,
         train_layers: list = None,
         softmax_loss: bool = True,
         random_seed: int = 42,
     ):
         self.args = {}
         self.args["model_name"] = model_name
         self.args["num_train_epochs"] = num_train_epochs
@@ -231,27 +231,30 @@
     Inherits from the abstract class Reranker.
     """
 
     def __init__(self, model=None):
         self.model = model
 
     @staticmethod
-    def load(checkpoint, device):
+    def load(checkpoint, device, max_length=512):
         """
         Loads a pre-trained model from a checkpoint and returns a new instance of CrossEncoderReranker.
 
         Args:
         - checkpoint: The path to the checkpoint file to load.
         - device: The device to load the model onto.
+        - max_length: Maximum input length
 
         Returns:
         - new instance of CrossEncoderReranker.
         """
         model = CrossEncoder(checkpoint)
         model.model.to(torch.device(device))
+        if not model.max_length:
+            model.max_length = max_length
         return CrossEncoderReranker(model)
 
     @staticmethod
     def prepare_data(
         candidates,
         ground_truth,
         kb,
@@ -372,15 +375,15 @@
         self.model.fit_with_scores(
             train_dataloader=train_dataloader,
             evaluator=evaluator,
             epochs=training_args["num_train_epochs"],
             loss_fct=loss_fct,
             warmup_steps=100,
             output_path=output_dir,
-            callback=callback,
+            callback=None,
             use_amp=training_args["fp16"],
             label_smoothing=training_args["label_smoothing"],
             score_regularization=training_args["score_regularization"],
             train_layers=training_args["train_layers"],
             show_progress_bar=show_progress_bar,
         )
```

### Comparing `xmen-0.9.6/xmen/reranking/list_wise.py` & `xmen-0.9.7/xmen/reranking/list_wise.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/reranking/multiple_choice_util.py` & `xmen-0.9.7/xmen/reranking/multiple_choice_util.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/reranking/ranking_util.py` & `xmen-0.9.7/xmen/reranking/ranking_util.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/reranking/rule_based.py` & `xmen-0.9.7/xmen/reranking/rule_based.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/reranking/scored_cross_encoder.py` & `xmen-0.9.7/xmen/reranking/scored_cross_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,23 +104,23 @@
         loss_fct=None,
         activation_fct=torch.nn.Identity(),
         scheduler: str = "WarmupLinear",
         warmup_steps: int = 10000,
         optimizer_class: Type[Optimizer] = torch.optim.AdamW,
         optimizer_params: Dict[str, object] = {"lr": 2e-5},
         weight_decay: float = 0.01,
-        score_regularization: bool = True,
+        score_regularization: bool = 1.0,
         train_layers: list = [],
         label_smoothing: float = 0.0,
         evaluation_steps: int = 0,
         output_path: str = None,
         save_best_model: bool = True,
         max_grad_norm: float = 1,
         use_amp: bool = False,
-        callback: Callable[[float, int, int], None] = None,
+        callback: Callable[[Dict], None] = None,
         show_progress_bar: bool = True,
     ):
         """
         Train the model with the given training objective
         Each training objective is sampled in turn for one batch.
         We sample only as many batches from each objective as there are in the smallest one
         to make sure of equal training with each dataset.
@@ -137,16 +137,14 @@
         :param weight_decay: Weight decay for model parameters
         :param evaluation_steps: If > 0, evaluate the model using evaluator after each number of training steps
         :param output_path: Storage path for the model and evaluation files
         :param save_best_model: If true, the best model (according to evaluator) is stored at output_path
         :param max_grad_norm: Used for gradient normalization.
         :param use_amp: Use Automatic Mixed Precision (AMP). Only for Pytorch >= 1.6.0
         :param callback: Callback function that is invoked after each evaluation.
-                It must accept the following three parameters in this order:
-                `score`, `epoch`, `steps`
         :param show_progress_bar: If True, output a tqdm progress bar
         """
         train_dataloader.collate_fn = self.smart_batching_collate_with_scores
 
         if use_amp:
             from torch.cuda.amp import autocast
 
@@ -203,16 +201,16 @@
                 if use_amp:
                     with autocast():
                         model_predictions = self.model(**features, return_dict=True)
                         logits = activation_fct(model_predictions.logits)
                         if self.config.num_labels == 1:
                             logits = logits.view(-1)
                         loss_value = loss_fct(logits, labels)
-                        if score_regularization:
-                            loss_value += self.score_regularizer(logits, scores)
+                        if score_regularization != 0:
+                            loss_value += score_regularization * self.score_regularizer(logits, scores)
 
                     scale_before_step = scaler.get_scale()
                     scaler.scale(loss_value).backward()
                     scaler.unscale_(optimizer)
                     torch.nn.utils.clip_grad_norm_(self.model.parameters(), max_grad_norm)
                     scaler.step(optimizer)
                     scaler.update()
@@ -220,18 +218,16 @@
                     skip_scheduler = scaler.get_scale() != scale_before_step
                 else:
                     model_predictions = self.model(**features, return_dict=True)
                     logits = activation_fct(model_predictions.logits)
                     if self.config.num_labels == 1:
                         logits = logits.view(-1)
                     loss_value = loss_fct(logits, labels)
-                    if score_regularization:
-                        # loss_value = self.score_regularizer(logits, scores)
-                        # Try next: only logits, no softmax
-                        loss_value += self.score_regularizer(logits, scores)
+                    if score_regularization != 0:
+                        loss_value += score_regularization * self.score_regularizer(logits, scores)
                     loss_value.backward()
                     torch.nn.utils.clip_grad_norm_(self.model.parameters(), max_grad_norm)
                     optimizer.step()
 
                 optimizer.zero_grad()
 
                 if not skip_scheduler:
```

### Comparing `xmen-0.9.6/xmen/resources/SemGroups-v03.txt` & `xmen-0.9.7/xmen/resources/SemGroups-v03.txt`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/resources/SemGroups.txt` & `xmen-0.9.7/xmen/resources/SemGroups.txt`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/xmen/umls.py` & `xmen-0.9.7/xmen/umls.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.6/PKG-INFO` & `xmen-0.9.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmen
-Version: 0.9.6
+Version: 0.9.7
 Summary: An extensible toolkit for Cross-lingual (x) Medical Entity Normalization.
 Home-page: https://github.com/hpi-dhc/xmen
 License: Apache-2.0
 Author: Florian Borchert
 Author-email: florian.borchert@hpi.de
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,14 +16,15 @@
 Requires-Dist: faiss-cpu (>=1.7.1,<2.0.0) ; sys_platform != "linux"
 Requires-Dist: faiss-gpu (>=1.7.1,<2.0.0) ; sys_platform == "linux"
 Requires-Dist: langcodes (>=3.3.0,<4.0.0)
 Requires-Dist: lxml (>=4.8.0,<5.0.0)
 Requires-Dist: neleval (>=3.1.1,<4.0.0)
 Requires-Dist: numpy (>=1.21,<2.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
+Requires-Dist: orjson (>=3.9.1,<4.0.0)
 Requires-Dist: protobuf (>=3.20.0,<4.0.0)
 Requires-Dist: pytorch-metric-learning (==0.9.98.dev1)
 Requires-Dist: rich (>=12.3.0,<13.0.0)
 Requires-Dist: scispacy (>=0.5.2,<0.6.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: sentencepiece (>=0.1.96,<0.2.0)
 Requires-Dist: torch (>=1.13.0,<2.0.0)
@@ -172,40 +173,32 @@
 
 xMEN provides implementations of different neural and non-neural candidate generators
 
 ### TF-IDF Weighted Character N-grams
 
 Based on the implementation from [scispaCy](https://github.com/allenai/scispacy).
 
-YAML file:
-
-```
-linker:
-  candidate_generation:
-    ngram: ~
-```
-
 Run `xmen index my_config.yaml --ngram` or `xmen index my_config.yaml --all` to create the index.
 
 To use the linker at runtime, pass the index folder as an argument:
 
 ```
 from xmen.linkers import TFIDFNGramLinker
 
 ngram_linker = TFIDFNGramLinker(index_base_path="/path/to/my/index/ngram", k=100)
 predictions = ngram_linker.predict_batch(dataset)
 ```
 
-Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
+Example usage: see [BioASQ / DisTEMIST Notebook](notebooks/examples/01_BioASQ_DisTEMIST.ipynb)
 
 ### SapBERT
 
 Dense Retrieval based on [SapBERT](https://github.com/cambridgeltl/sapbert) embeddings.
 
-YAML file:
+YAML file (optional, if you want to configure another Transformer model):
 
 ```
 linker:
   candidate_generation:
     sapbert:
       model_name: cambridgeltl/SapBERT-UMLS-2020AB-all-lang-from-XLMR
 ```
@@ -228,15 +221,15 @@
 
 ```
 sapbert_linker = SapBERTLinker(**config)
 ```
 
 By default, SapBERT assumes a CUDA device is available. If you want to disable cuda, pass `cuda=False` to the constructor.
 
-Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
+Example usage: see [BioASQ / DisTEMIST Notebook](notebooks/examples/01_BioASQ_DisTEMIST.ipynb)
 
 ### Ensemble
 
 Different candidate generators often work well for different kinds of entity mentions, and it can be helpful to combine their predictions.
 
 In xMEN, this can be easily achieved with an `EnsembleLinker`:
 
@@ -252,17 +245,15 @@
 
 Sometimes, you want to compare the ensemble performance to individual linkers and already have the candidate lists. To avoid recomputation, you can use the `reuse_preds` argument:
 
 ```
 prediction = ensemble_linker.predict_batch(dataset, 128, 100, reuse_preds={'sapbert' : predictions_sap, 'ngram' : predictions_ngram'})
 ```
 
-Note: `reuse_preds` currently does not support Hugging Face `DatasetDict` objects, so you would have to call it on each split individually.
-
-Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
+Example usage: see [BioASQ / DisTEMIST Notebook](notebooks/examples/examples/01_BioASQ_DisTEMIST.ipynb)
 
 ## 🌀 Rerankers
 
 ### Cross-Encoder Reranker
 
 When labelled training data is available, a trainable reranker can improve ranking of candidate lists a lot.
 
@@ -299,15 +290,15 @@
 # Fit the model
 rr.fit(args, cross_enc_ds['train'].dataset, cross_enc_ds['validation'].dataset)
 
 # Predict on test set
 prediction = rr.rerank_batch(candidates['test'], cross_enc_ds['test'])
 ```
 
-Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
+Example usage: see [BioASQ / DisTEMIST Notebook](notebooks/examples/01_BioASQ_DisTEMIST.ipynb)
 
 ### Rule-based Reranker
 
 TODO
 
 ## 💡 Pre- and Post-Processing
 
@@ -319,13 +310,13 @@
 - [Filtering by UMLS semantic types](xmen/data/semantic_types.py)
 - [Replacement of retired CUIS](xmen/data/retired_cuis.py)
 
 ## 📊 Evaluation
 
 xMEN provides implementations of common entity linking metrics (e.g., a wrapper for [neleval](https://github.com/wikilinks/neleval))
 
-Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
+Example usage: see [BioASQ / DisTEMIST Notebook](notebooks/examples/01_BioASQ_DisTEMIST.ipynb)
 
 ## 📈 Benchmark Results
 
 TODO
```

