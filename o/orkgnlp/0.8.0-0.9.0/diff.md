# Comparing `tmp/orkgnlp-0.8.0.tar.gz` & `tmp/orkgnlp-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orkgnlp-0.8.0.tar", max compression
+gzip compressed data, was "orkgnlp-0.9.0.tar", max compression
```

## Comparing `orkgnlp-0.8.0.tar` & `orkgnlp-0.9.0.tar`

### file list

```diff
@@ -1,44 +1,47 @@
--rw-r--r--   0        0        0     1119 2022-04-08 15:37:14.786424 orkgnlp-0.8.0/LICENSE
--rw-r--r--   0        0        0      696 2022-06-22 09:12:23.991322 orkgnlp-0.8.0/README.md
--rw-r--r--   0        0        0      429 2022-10-21 13:56:21.004660 orkgnlp-0.8.0/orkgnlp/__init__.py
--rw-r--r--   0        0        0      121 2022-06-23 12:55:48.539095 orkgnlp-0.8.0/orkgnlp/annotation/__init__.py
--rw-r--r--   0        0        0      235 2022-06-01 12:28:05.768777 orkgnlp-0.8.0/orkgnlp/annotation/csner/__init__.py
--rw-r--r--   0        0        0     3370 2022-06-23 12:55:50.099089 orkgnlp-0.8.0/orkgnlp/annotation/csner/annotator.py
--rw-r--r--   0        0        0     4537 2022-06-20 16:27:14.764325 orkgnlp-0.8.0/orkgnlp/annotation/csner/decoder.py
--rw-r--r--   0        0        0     8741 2022-06-20 16:27:14.764325 orkgnlp-0.8.0/orkgnlp/annotation/csner/encoder.py
--rw-r--r--   0        0        0       91 2022-06-15 14:59:35.316389 orkgnlp-0.8.0/orkgnlp/annotation/tdm/__init__.py
--rw-r--r--   0        0        0     1986 2022-06-20 16:27:14.764325 orkgnlp-0.8.0/orkgnlp/annotation/tdm/decoder.py
--rw-r--r--   0        0        0     5024 2022-06-20 16:27:14.764325 orkgnlp-0.8.0/orkgnlp/annotation/tdm/encoder.py
--rw-r--r--   0        0        0     2136 2022-06-23 12:55:50.099089 orkgnlp-0.8.0/orkgnlp/annotation/tdm/extractor.py
--rw-r--r--   0        0        0      157 2022-05-24 08:54:16.226536 orkgnlp-0.8.0/orkgnlp/clustering/__init__.py
--rw-r--r--   0        0        0      135 2022-06-01 12:28:05.768777 orkgnlp-0.8.0/orkgnlp/clustering/bioassays/__init__.py
--rw-r--r--   0        0        0      906 2022-06-20 16:27:14.764325 orkgnlp-0.8.0/orkgnlp/clustering/bioassays/decoder.py
--rw-r--r--   0        0        0     1675 2022-06-23 12:55:50.099089 orkgnlp-0.8.0/orkgnlp/clustering/bioassays/semantifier.py
--rw-r--r--   0        0        0     1943 2022-10-21 13:59:21.664011 orkgnlp-0.8.0/orkgnlp/clustering/encoders.py
--rw-r--r--   0        0        0      136 2022-06-01 12:28:05.768777 orkgnlp-0.8.0/orkgnlp/clustering/predicates/__init__.py
--rw-r--r--   0        0        0     1592 2022-10-21 14:15:43.586032 orkgnlp-0.8.0/orkgnlp/clustering/predicates/decoder.py
--rw-r--r--   0        0        0     1889 2022-10-21 13:55:59.068740 orkgnlp-0.8.0/orkgnlp/clustering/predicates/recommender.py
--rw-r--r--   0        0        0      130 2022-06-20 16:27:14.764325 orkgnlp-0.8.0/orkgnlp/common/__init__.py
--rw-r--r--   0        0        0      114 2022-05-24 08:54:16.230536 orkgnlp-0.8.0/orkgnlp/common/config/__init__.py
--rw-r--r--   0        0        0     1247 2022-06-23 12:55:50.099089 orkgnlp-0.8.0/orkgnlp/common/config/context.py
--rw-r--r--   0        0        0       73 2022-06-01 12:28:05.768777 orkgnlp-0.8.0/orkgnlp/common/service/__init__.py
--rw-r--r--   0        0        0    10338 2022-06-23 12:55:50.099089 orkgnlp-0.8.0/orkgnlp/common/service/base.py
--rw-r--r--   0        0        0     3506 2022-06-23 12:55:48.539095 orkgnlp-0.8.0/orkgnlp/common/service/runners.py
--rw-r--r--   0        0        0      117 2022-05-24 08:54:16.230536 orkgnlp-0.8.0/orkgnlp/common/tools/__init__.py
--rw-r--r--   0        0        0     4223 2022-06-23 12:55:50.107089 orkgnlp-0.8.0/orkgnlp/common/tools/downloader.py
--rw-r--r--   0        0        0       86 2022-05-24 08:54:16.230536 orkgnlp-0.8.0/orkgnlp/common/util/__init__.py
--rw-r--r--   0        0        0      658 2022-06-22 14:12:33.466453 orkgnlp-0.8.0/orkgnlp/common/util/datastructure.py
--rw-r--r--   0        0        0     1089 2022-08-22 14:37:02.540236 orkgnlp-0.8.0/orkgnlp/common/util/decorators.py
--rw-r--r--   0        0        0      434 2022-06-20 16:27:14.764325 orkgnlp-0.8.0/orkgnlp/common/util/exceptions.py
--rw-r--r--   0        0        0     2990 2022-06-23 12:55:48.539095 orkgnlp-0.8.0/orkgnlp/common/util/io.py
--rw-r--r--   0        0        0     2083 2022-08-22 14:37:02.540236 orkgnlp-0.8.0/orkgnlp/common/util/text.py
--rw-r--r--   0        0        0     3114 2022-10-21 13:41:25.132041 orkgnlp-0.8.0/orkgnlp/huggingface_repos.json
--rw-r--r--   0        0        0      303 2022-06-23 12:55:50.107089 orkgnlp-0.8.0/orkgnlp/huggingface_repos_schema.json
--rw-r--r--   0        0        0      107 2022-08-22 14:37:02.540236 orkgnlp-0.8.0/orkgnlp/nli/__init__.py
--rw-r--r--   0        0        0      126 2022-08-22 14:37:02.540236 orkgnlp-0.8.0/orkgnlp/nli/templates/__init__.py
--rw-r--r--   0        0        0     1536 2022-08-22 14:37:02.540236 orkgnlp-0.8.0/orkgnlp/nli/templates/decoder.py
--rw-r--r--   0        0        0     2638 2022-08-22 14:37:02.540236 orkgnlp-0.8.0/orkgnlp/nli/templates/encoder.py
--rw-r--r--   0        0        0     2040 2022-08-22 14:37:02.540236 orkgnlp-0.8.0/orkgnlp/nli/templates/recommender.py
--rw-r--r--   0        0        0     1265 2022-10-21 13:56:13.892686 orkgnlp-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2089 2022-10-21 14:15:46.148313 orkgnlp-0.8.0/setup.py
--rw-r--r--   0        0        0     1960 2022-10-21 14:15:46.148517 orkgnlp-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1119 2022-04-08 15:37:14.786424 orkgnlp-0.9.0/LICENSE
+-rw-r--r--   0        0        0      696 2022-06-22 09:12:23.991322 orkgnlp-0.9.0/README.md
+-rw-r--r--   0        0        0      429 2023-02-16 07:27:31.327759 orkgnlp-0.9.0/orkgnlp/__init__.py
+-rw-r--r--   0        0        0      168 2023-02-16 07:27:31.327759 orkgnlp-0.9.0/orkgnlp/annotation/__init__.py
+-rw-r--r--   0        0        0       84 2023-02-16 07:27:31.327759 orkgnlp-0.9.0/orkgnlp/annotation/agriner/__init__.py
+-rw-r--r--   0        0        0     1618 2023-02-16 07:27:31.327759 orkgnlp-0.9.0/orkgnlp/annotation/agriner/annotator.py
+-rw-r--r--   0        0        0     1151 2023-02-16 07:27:31.327759 orkgnlp-0.9.0/orkgnlp/annotation/agriner/decoder.py
+-rw-r--r--   0        0        0      235 2022-06-01 12:28:05.768777 orkgnlp-0.9.0/orkgnlp/annotation/csner/__init__.py
+-rw-r--r--   0        0        0     3370 2022-06-23 12:55:50.099089 orkgnlp-0.9.0/orkgnlp/annotation/csner/annotator.py
+-rw-r--r--   0        0        0     4537 2022-06-20 16:27:14.764325 orkgnlp-0.9.0/orkgnlp/annotation/csner/decoder.py
+-rw-r--r--   0        0        0     8741 2022-06-20 16:27:14.764325 orkgnlp-0.9.0/orkgnlp/annotation/csner/encoder.py
+-rw-r--r--   0        0        0       91 2022-06-15 14:59:35.316389 orkgnlp-0.9.0/orkgnlp/annotation/tdm/__init__.py
+-rw-r--r--   0        0        0     1986 2022-06-20 16:27:14.764325 orkgnlp-0.9.0/orkgnlp/annotation/tdm/decoder.py
+-rw-r--r--   0        0        0     5024 2022-06-20 16:27:14.764325 orkgnlp-0.9.0/orkgnlp/annotation/tdm/encoder.py
+-rw-r--r--   0        0        0     2136 2022-06-23 12:55:50.099089 orkgnlp-0.9.0/orkgnlp/annotation/tdm/extractor.py
+-rw-r--r--   0        0        0      157 2022-05-24 08:54:16.226536 orkgnlp-0.9.0/orkgnlp/clustering/__init__.py
+-rw-r--r--   0        0        0      135 2022-06-01 12:28:05.768777 orkgnlp-0.9.0/orkgnlp/clustering/bioassays/__init__.py
+-rw-r--r--   0        0        0      906 2022-06-20 16:27:14.764325 orkgnlp-0.9.0/orkgnlp/clustering/bioassays/decoder.py
+-rw-r--r--   0        0        0     1675 2022-06-23 12:55:50.099089 orkgnlp-0.9.0/orkgnlp/clustering/bioassays/semantifier.py
+-rw-r--r--   0        0        0     1943 2023-01-25 12:02:17.182232 orkgnlp-0.9.0/orkgnlp/clustering/encoders.py
+-rw-r--r--   0        0        0      136 2022-06-01 12:28:05.768777 orkgnlp-0.9.0/orkgnlp/clustering/predicates/__init__.py
+-rw-r--r--   0        0        0     1592 2023-01-25 12:02:17.182232 orkgnlp-0.9.0/orkgnlp/clustering/predicates/decoder.py
+-rw-r--r--   0        0        0     1889 2023-01-25 12:02:17.182232 orkgnlp-0.9.0/orkgnlp/clustering/predicates/recommender.py
+-rw-r--r--   0        0        0      130 2022-06-20 16:27:14.764325 orkgnlp-0.9.0/orkgnlp/common/__init__.py
+-rw-r--r--   0        0        0      114 2022-05-24 08:54:16.230536 orkgnlp-0.9.0/orkgnlp/common/config/__init__.py
+-rw-r--r--   0        0        0     1247 2022-06-23 12:55:50.099089 orkgnlp-0.9.0/orkgnlp/common/config/context.py
+-rw-r--r--   0        0        0       73 2022-06-01 12:28:05.768777 orkgnlp-0.9.0/orkgnlp/common/service/__init__.py
+-rw-r--r--   0        0        0    10342 2023-02-16 07:27:31.327759 orkgnlp-0.9.0/orkgnlp/common/service/base.py
+-rw-r--r--   0        0        0     3552 2023-02-16 07:27:31.327759 orkgnlp-0.9.0/orkgnlp/common/service/runners.py
+-rw-r--r--   0        0        0      117 2022-05-24 08:54:16.230536 orkgnlp-0.9.0/orkgnlp/common/tools/__init__.py
+-rw-r--r--   0        0        0     4223 2022-06-23 12:55:50.107089 orkgnlp-0.9.0/orkgnlp/common/tools/downloader.py
+-rw-r--r--   0        0        0       86 2022-05-24 08:54:16.230536 orkgnlp-0.9.0/orkgnlp/common/util/__init__.py
+-rw-r--r--   0        0        0      658 2022-06-22 14:12:33.466453 orkgnlp-0.9.0/orkgnlp/common/util/datastructure.py
+-rw-r--r--   0        0        0     1089 2022-08-22 14:37:02.540236 orkgnlp-0.9.0/orkgnlp/common/util/decorators.py
+-rw-r--r--   0        0        0      434 2022-06-20 16:27:14.764325 orkgnlp-0.9.0/orkgnlp/common/util/exceptions.py
+-rw-r--r--   0        0        0     2990 2022-06-23 12:55:48.539095 orkgnlp-0.9.0/orkgnlp/common/util/io.py
+-rw-r--r--   0        0        0     2083 2022-08-22 14:37:02.540236 orkgnlp-0.9.0/orkgnlp/common/util/text.py
+-rw-r--r--   0        0        0     3414 2023-02-16 07:27:31.327759 orkgnlp-0.9.0/orkgnlp/huggingface_repos.json
+-rw-r--r--   0        0        0      303 2022-06-23 12:55:50.107089 orkgnlp-0.9.0/orkgnlp/huggingface_repos_schema.json
+-rw-r--r--   0        0        0      107 2022-08-22 14:37:02.540236 orkgnlp-0.9.0/orkgnlp/nli/__init__.py
+-rw-r--r--   0        0        0      126 2022-08-22 14:37:02.540236 orkgnlp-0.9.0/orkgnlp/nli/templates/__init__.py
+-rw-r--r--   0        0        0     1536 2022-08-22 14:37:02.540236 orkgnlp-0.9.0/orkgnlp/nli/templates/decoder.py
+-rw-r--r--   0        0        0     2638 2022-08-22 14:37:02.540236 orkgnlp-0.9.0/orkgnlp/nli/templates/encoder.py
+-rw-r--r--   0        0        0     2040 2022-08-22 14:37:02.540236 orkgnlp-0.9.0/orkgnlp/nli/templates/recommender.py
+-rw-r--r--   0        0        0     1294 2023-02-16 07:27:31.331759 orkgnlp-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2158 1970-01-01 00:00:00.000000 orkgnlp-0.9.0/setup.py
+-rw-r--r--   0        0        0     2110 1970-01-01 00:00:00.000000 orkgnlp-0.9.0/PKG-INFO
```

### Comparing `orkgnlp-0.8.0/LICENSE` & `orkgnlp-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orkgnlp-0.8.0/README.md` & `orkgnlp-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `orkgnlp-0.8.0/orkgnlp/annotation/csner/annotator.py` & `orkgnlp-0.9.0/orkgnlp/annotation/csner/annotator.py`

 * *Files identical despite different names*

### Comparing `orkgnlp-0.8.0/orkgnlp/annotation/csner/decoder.py` & `orkgnlp-0.9.0/orkgnlp/annotation/csner/decoder.py`

 * *Files identical despite different names*

### Comparing `orkgnlp-0.8.0/orkgnlp/annotation/csner/encoder.py` & `orkgnlp-0.9.0/orkgnlp/annotation/csner/encoder.py`

 * *Files identical despite different names*

### Comparing `orkgnlp-0.8.0/orkgnlp/annotation/tdm/decoder.py` & `orkgnlp-0.9.0/orkgnlp/annotation/tdm/decoder.py`

 * *Files identical despite different names*

### Comparing `orkgnlp-0.8.0/orkgnlp/annotation/tdm/encoder.py` & `orkgnlp-0.9.0/orkgnlp/annotation/tdm/encoder.py`

 * *Files identical despite different names*

### Comparing `orkgnlp-0.8.0/orkgnlp/annotation/tdm/extractor.py` & `orkgnlp-0.9.0/orkgnlp/annotation/tdm/extractor.py`

 * *Files identical despite different names*

### Comparing `orkgnlp-0.8.0/orkgnlp/clustering/bioassays/decoder.py` & `orkgnlp-0.9.0/orkgnlp/clustering/bioassays/decoder.py`

 * *Files identical despite different names*

### Comparing `orkgnlp-0.8.0/orkgnlp/clustering/bioassays/semantifier.py` & `orkgnlp-0.9.0/orkgnlp/clustering/bioassays/semantifier.py`

 * *Files identical despite different names*

### Comparing `orkgnlp-0.8.0/orkgnlp/clustering/encoders.py` & `orkgnlp-0.9.0/orkgnlp/clustering/encoders.py`

 * *Files identical despite different names*

### Comparing `orkgnlp-0.8.0/orkgnlp/clustering/predicates/decoder.py` & `orkgnlp-0.9.0/orkgnlp/clustering/predicates/decoder.py`

 * *Files identical despite different names*

### Comparing `orkgnlp-0.8.0/orkgnlp/clustering/predicates/recommender.py` & `orkgnlp-0.9.0/orkgnlp/clustering/predicates/recommender.py`

 * *Files identical despite different names*

### Comparing `orkgnlp-0.8.0/orkgnlp/common/config/context.py` & `orkgnlp-0.9.0/orkgnlp/common/config/context.py`

 * *Files identical despite different names*

### Comparing `orkgnlp-0.8.0/orkgnlp/common/service/base.py` & `orkgnlp-0.9.0/orkgnlp/common/service/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     def encode(self, raw_input: Any, **kwargs: Any) -> Tuple[Any, Dict[str, Any]]:
         """
         Encodes the ``raw_input`` to a model-friendly format.
 
         :param raw_input: The user's input to be encoded.
         :return: The model-friendly output and kwargs.
         """
-        return raw_input, kwargs
+        return (raw_input, ), kwargs
 
 
 class ORKGNLPBaseDecoder(EnforceOverrides, PipelineExecutorComponent):
     """
     The ORKGNLPBaseDecoder is  the base decoder class. You can freely inherit this class, implement its
     ``decode(model_output, **kwargs)`` function and use it to decode your model output to a user-friendly format.
```

### Comparing `orkgnlp-0.8.0/orkgnlp/common/service/runners.py` & `orkgnlp-0.9.0/orkgnlp/common/service/runners.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,17 @@
         :param inputs: Tuple of model arguments or dict of model named arguments.
             A list of tuples or a list of dicts in case of batches.
         :param multiple_batches: Whether the model is to be executed x times for each input instance or batch, where
             x is the length of ``inputs`` list. Note that in this case the model's outputs
             will be returned as a python generator. Defaults to False.
         :return: The model output as a tuple or list of tuples, and kwargs.
         """
-        self._model.eval()
+
+        if hasattr(self._model, 'eval'):
+            self._model.eval()
 
         if not multiple_batches:
 
             if isinstance(inputs, dict):
                 output = self._model(**inputs)
             else:
                 output = self._model(*inputs)
```

### Comparing `orkgnlp-0.8.0/orkgnlp/common/tools/downloader.py` & `orkgnlp-0.9.0/orkgnlp/common/tools/downloader.py`

 * *Files identical despite different names*

### Comparing `orkgnlp-0.8.0/orkgnlp/common/util/datastructure.py` & `orkgnlp-0.9.0/orkgnlp/common/util/datastructure.py`

 * *Files identical despite different names*

### Comparing `orkgnlp-0.8.0/orkgnlp/common/util/decorators.py` & `orkgnlp-0.9.0/orkgnlp/common/util/decorators.py`

 * *Files identical despite different names*

### Comparing `orkgnlp-0.8.0/orkgnlp/common/util/io.py` & `orkgnlp-0.9.0/orkgnlp/common/util/io.py`

 * *Files identical despite different names*

### Comparing `orkgnlp-0.8.0/orkgnlp/common/util/text.py` & `orkgnlp-0.9.0/orkgnlp/common/util/text.py`

 * *Files identical despite different names*

### Comparing `orkgnlp-0.8.0/orkgnlp/huggingface_repos.json` & `orkgnlp-0.9.0/orkgnlp/huggingface_repos.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'agri-ner'": "[OrderedDict([('repo_id', 'orkg/orkgnlp-agri-ner'), ('files', "*

 * *               "[OrderedDict([('internal_name', 'model'), ('filename', 'pytorch_model.bin')]), "*

 * *               "OrderedDict([('internal_name', 'model_config'), ('filename', 'config.json')])])])]"}*

```diff
@@ -1,8 +1,23 @@
 {
+    "agri-ner": [
+        {
+            "files": [
+                {
+                    "filename": "pytorch_model.bin",
+                    "internal_name": "model"
+                },
+                {
+                    "filename": "config.json",
+                    "internal_name": "model_config"
+                }
+            ],
+            "repo_id": "orkg/orkgnlp-agri-ner"
+        }
+    ],
     "bioassays-semantification": [
         {
             "files": [
                 {
                     "filename": "orkgnlp-bioassays-kmeans-700.onnx",
                     "internal_name": "model"
                 },
```

### Comparing `orkgnlp-0.8.0/orkgnlp/nli/templates/decoder.py` & `orkgnlp-0.9.0/orkgnlp/nli/templates/decoder.py`

 * *Files identical despite different names*

### Comparing `orkgnlp-0.8.0/orkgnlp/nli/templates/encoder.py` & `orkgnlp-0.9.0/orkgnlp/nli/templates/encoder.py`

 * *Files identical despite different names*

### Comparing `orkgnlp-0.8.0/orkgnlp/nli/templates/recommender.py` & `orkgnlp-0.9.0/orkgnlp/nli/templates/recommender.py`

 * *Files identical despite different names*

### Comparing `orkgnlp-0.8.0/pyproject.toml` & `orkgnlp-0.9.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orkgnlp"
-version = "0.8.0"
+version = "0.9.0"
 description = "Python package wrapping the ORKG NLP Services."
 license = "MIT"
 authors = ["Omar Arab Oghli <omar.araboghli@outlook.com>"]
 maintainers = ["Omar Arab Oghli"]
 readme = "README.md"
 homepage = "http://orkg.org/about"
 repository = "https://gitlab.com/TIBHannover/orkg/nlp/orkg-nlp-pypi"
@@ -29,14 +29,15 @@
 torch = "1.11.0"
 spacy = "3.3.0"
 overrides = "^6.1.0"
 protobuf = "3.20.0"
 transformers = "4.19.3"
 sentencepiece = "^0.1.96"
 sentence-transformers = "2.2.2"
+typing-extensions = "^3.7.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 tox = "^3.25.0"
 virtualenv = "^20.14.1"
 
 [build-system]
```

### Comparing `orkgnlp-0.8.0/setup.py` & `orkgnlp-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['orkgnlp',
  'orkgnlp.annotation',
+ 'orkgnlp.annotation.agriner',
  'orkgnlp.annotation.csner',
  'orkgnlp.annotation.tdm',
  'orkgnlp.clustering',
  'orkgnlp.clustering.bioassays',
  'orkgnlp.clustering.predicates',
  'orkgnlp.common',
  'orkgnlp.common.config',
@@ -29,28 +30,29 @@
  'overrides>=6.1.0,<7.0.0',
  'pandas==1.3.5',
  'protobuf==3.20.0',
  'sentence-transformers==2.2.2',
  'sentencepiece>=0.1.96,<0.2.0',
  'spacy==3.3.0',
  'torch==1.11.0',
- 'transformers==4.19.3']
+ 'transformers==4.19.3',
+ 'typing-extensions>=3.7.4,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['test = tests.unittests:main']}
 
 setup_kwargs = {
     'name': 'orkgnlp',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Python package wrapping the ORKG NLP Services.',
     'long_description': '# ORKG NLP PyPI\n[![Documentation Status](https://readthedocs.org/projects/orkg-nlp-pypi/badge/?version=latest)](https://orkg-nlp-pypi.readthedocs.io/en/latest/?badge=latest)\n[![PyPI version](https://badge.fury.io/py/orkgnlp.svg)](https://badge.fury.io/py/orkgnlp)\n[![pipeline status](https://gitlab.com/TIBHannover/orkg/nlp/orkg-nlp-pypi/badges/main/pipeline.svg)](https://gitlab.com/TIBHannover/orkg/nlp/orkg-nlp-pypi/-/commits/main)\n\nPyPI package wrapping the ORKG NLP services.\n\nCheck our [Read the Docs](https://orkg-nlp-pypi.readthedocs.io/en/latest/) for more details!\n\nYour [contribution](https://orkg-nlp-pypi.readthedocs.io/en/latest/contribute.html) to `orkgnlp` will always be honored!',
     'author': 'Omar Arab Oghli',
     'author_email': 'omar.araboghli@outlook.com',
     'maintainer': 'Omar Arab Oghli',
-    'maintainer_email': None,
+    'maintainer_email': 'None',
     'url': 'http://orkg.org/about',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.7.1,<3.10',
 }
```

### Comparing `orkgnlp-0.8.0/PKG-INFO` & `orkgnlp-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: orkgnlp
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python package wrapping the ORKG NLP Services.
 Home-page: http://orkg.org/about
 License: MIT
 Keywords: ORKG,NLP,Scholarly Communication,Digital Library
 Author: Omar Arab Oghli
 Author-email: omar.araboghli@outlook.com
 Maintainer: Omar Arab Oghli
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: huggingface-hub (>=0.5.1,<0.6.0)
 Requires-Dist: nltk (==3.5)
 Requires-Dist: numpy (==1.21.6)
 Requires-Dist: onnx (==1.11.0)
@@ -23,14 +25,15 @@
 Requires-Dist: pandas (==1.3.5)
 Requires-Dist: protobuf (==3.20.0)
 Requires-Dist: sentence-transformers (==2.2.2)
 Requires-Dist: sentencepiece (>=0.1.96,<0.2.0)
 Requires-Dist: spacy (==3.3.0)
 Requires-Dist: torch (==1.11.0)
 Requires-Dist: transformers (==4.19.3)
+Requires-Dist: typing-extensions (>=3.7.4,<4.0.0)
 Project-URL: Documentation, https://orkg-nlp-pypi.readthedocs.io/en/latest/
 Project-URL: Repository, https://gitlab.com/TIBHannover/orkg/nlp/orkg-nlp-pypi
 Description-Content-Type: text/markdown
 
 # ORKG NLP PyPI
 [![Documentation Status](https://readthedocs.org/projects/orkg-nlp-pypi/badge/?version=latest)](https://orkg-nlp-pypi.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/orkgnlp.svg)](https://badge.fury.io/py/orkgnlp)
```

