# Comparing `tmp/embetter-0.4.1.tar.gz` & `tmp/embetter-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/embetter-0.4.1.tar", last modified: Fri Jun 30 08:55:01 2023, max compression
+gzip compressed data, was "dist/embetter-0.5.0.tar", last modified: Fri Jun 30 11:33:30 2023, max compression
```

## Comparing `embetter-0.4.1.tar` & `embetter-0.5.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 08:55:01.000000 embetter-0.4.1/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5227 2023-06-30 08:55:01.000000 embetter-0.4.1/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4061 2023-06-03 11:05:06.000000 embetter-0.4.1/README.md
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      185 2023-05-01 13:07:12.000000 embetter-0.4.1/embetter/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      326 2022-09-17 15:40:35.000000 embetter-0.4.1/embetter/base.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      742 2022-07-16 12:25:08.000000 embetter-0.4.1/embetter/error.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter/external/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      256 2023-02-09 16:06:49.000000 embetter-0.4.1/embetter/external/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2001 2023-02-09 16:06:49.000000 embetter-0.4.1/embetter/external/_cohere.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2356 2023-03-28 13:55:26.000000 embetter-0.4.1/embetter/external/_openai.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter/finetune/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      401 2023-03-28 13:55:26.000000 embetter-0.4.1/embetter/finetune/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5823 2023-06-30 08:54:47.000000 embetter-0.4.1/embetter/finetune/_contrastive.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2851 2023-06-03 11:05:04.000000 embetter-0.4.1/embetter/finetune/_forward.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2408 2023-06-03 11:05:04.000000 embetter-0.4.1/embetter/grab.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter/multi/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      185 2023-06-03 11:05:04.000000 embetter-0.4.1/embetter/multi/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1758 2023-06-03 11:05:04.000000 embetter-0.4.1/embetter/multi/_clip.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter/text/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      730 2023-03-28 13:55:26.000000 embetter-0.4.1/embetter/text/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3794 2023-02-09 16:06:49.000000 embetter-0.4.1/embetter/text/_bpemb.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1579 2023-03-28 13:55:22.000000 embetter-0.4.1/embetter/text/_s2v.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3179 2023-06-03 11:05:04.000000 embetter-0.4.1/embetter/text/_sbert.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2767 2023-03-28 13:55:22.000000 embetter-0.4.1/embetter/text/_spacy.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4364 2023-06-30 08:54:47.000000 embetter-0.4.1/embetter/utils.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter/vision/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      361 2023-02-09 16:06:49.000000 embetter-0.4.1/embetter/vision/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1980 2023-02-09 16:06:49.000000 embetter-0.4.1/embetter/vision/_colorhist.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2205 2023-02-09 16:06:49.000000 embetter-0.4.1/embetter/vision/_loader.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2056 2023-02-09 16:06:49.000000 embetter-0.4.1/embetter/vision/_torchvis.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5227 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      898 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1209 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       15 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter.egg-info/top_level.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2023-06-30 08:55:01.000000 embetter-0.4.1/setup.cfg
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2615 2023-06-30 08:54:47.000000 embetter-0.4.1/setup.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 08:55:01.000000 embetter-0.4.1/tests/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2021-10-31 16:15:20.000000 embetter-0.4.1/tests/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      324 2022-12-05 09:29:24.000000 embetter-0.4.1/tests/test_base.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       64 2022-07-16 12:25:08.000000 embetter-0.4.1/tests/test_default.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      910 2023-02-09 16:06:49.000000 embetter-0.4.1/tests/test_docs.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      694 2023-06-30 08:54:47.000000 embetter-0.4.1/tests/test_finetuners.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3033 2023-06-29 15:07:29.000000 embetter-0.4.1/tests/test_text.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      569 2023-06-30 08:54:47.000000 embetter-0.4.1/tests/test_utils.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      871 2022-12-05 09:29:24.000000 embetter-0.4.1/tests/test_vision.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 11:33:30.000000 embetter-0.5.0/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5272 2023-06-30 11:33:30.000000 embetter-0.5.0/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4083 2023-06-30 09:34:46.000000 embetter-0.5.0/README.md
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 11:33:30.000000 embetter-0.5.0/embetter/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      185 2023-05-01 13:07:12.000000 embetter-0.5.0/embetter/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      326 2022-09-17 15:40:35.000000 embetter-0.5.0/embetter/base.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      742 2022-07-16 12:25:08.000000 embetter-0.5.0/embetter/error.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 11:33:30.000000 embetter-0.5.0/embetter/external/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      353 2023-06-30 11:13:15.000000 embetter-0.5.0/embetter/external/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2337 2023-06-30 09:36:04.000000 embetter-0.5.0/embetter/external/_cohere.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2665 2023-06-30 11:12:57.000000 embetter-0.5.0/embetter/external/_openai.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 11:33:30.000000 embetter-0.5.0/embetter/finetune/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      401 2023-03-28 13:55:26.000000 embetter-0.5.0/embetter/finetune/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5823 2023-06-30 08:54:47.000000 embetter-0.5.0/embetter/finetune/_contrastive.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2851 2023-06-03 11:05:04.000000 embetter-0.5.0/embetter/finetune/_forward.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2408 2023-06-03 11:05:04.000000 embetter-0.5.0/embetter/grab.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 11:33:30.000000 embetter-0.5.0/embetter/multi/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      185 2023-06-03 11:05:04.000000 embetter-0.5.0/embetter/multi/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1758 2023-06-03 11:05:04.000000 embetter-0.5.0/embetter/multi/_clip.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 11:33:30.000000 embetter-0.5.0/embetter/text/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      730 2023-03-28 13:55:26.000000 embetter-0.5.0/embetter/text/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3794 2023-02-09 16:06:49.000000 embetter-0.5.0/embetter/text/_bpemb.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1579 2023-03-28 13:55:22.000000 embetter-0.5.0/embetter/text/_s2v.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3179 2023-06-03 11:05:04.000000 embetter-0.5.0/embetter/text/_sbert.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2767 2023-03-28 13:55:22.000000 embetter-0.5.0/embetter/text/_spacy.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4346 2023-06-30 08:59:35.000000 embetter-0.5.0/embetter/utils.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 11:33:30.000000 embetter-0.5.0/embetter/vision/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      361 2023-02-09 16:06:49.000000 embetter-0.5.0/embetter/vision/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1980 2023-02-09 16:06:49.000000 embetter-0.5.0/embetter/vision/_colorhist.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2205 2023-02-09 16:06:49.000000 embetter-0.5.0/embetter/vision/_loader.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2056 2023-02-09 16:06:49.000000 embetter-0.5.0/embetter/vision/_torchvis.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 11:33:30.000000 embetter-0.5.0/embetter.egg-info/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5272 2023-06-30 11:33:30.000000 embetter-0.5.0/embetter.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      898 2023-06-30 11:33:30.000000 embetter-0.5.0/embetter.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-06-30 11:33:30.000000 embetter-0.5.0/embetter.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1285 2023-06-30 11:33:30.000000 embetter-0.5.0/embetter.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       15 2023-06-30 11:33:30.000000 embetter-0.5.0/embetter.egg-info/top_level.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2023-06-30 11:33:30.000000 embetter-0.5.0/setup.cfg
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2704 2023-06-30 09:29:49.000000 embetter-0.5.0/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 11:33:30.000000 embetter-0.5.0/tests/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2021-10-31 16:15:20.000000 embetter-0.5.0/tests/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      324 2022-12-05 09:29:24.000000 embetter-0.5.0/tests/test_base.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       64 2022-07-16 12:25:08.000000 embetter-0.5.0/tests/test_default.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      910 2023-02-09 16:06:49.000000 embetter-0.5.0/tests/test_docs.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      694 2023-06-30 08:54:47.000000 embetter-0.5.0/tests/test_finetuners.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3033 2023-06-29 15:07:29.000000 embetter-0.5.0/tests/test_text.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      569 2023-06-30 08:54:47.000000 embetter-0.5.0/tests/test_utils.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      871 2022-12-05 09:29:24.000000 embetter-0.5.0/tests/test_vision.py
```

### Comparing `embetter-0.4.1/PKG-INFO` & `embetter-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embetter
-Version: 0.4.1
+Version: 0.5.0
 Summary: Just a bunch of useful embeddings to get started quickly.
 Home-page: https://koaning.github.io/embetter/
 Author: Vincent D. Warmerdam
 License: UNKNOWN
 Project-URL: Documentation, https://koaning.github.io/embetter/
 Project-URL: Source Code, https://github.com/koaning/embetter/
 Project-URL: Issue Tracker, https://github.com/koaning/embetter/issues
@@ -23,14 +23,15 @@
 Provides-Extra: sentence-tfm
 Provides-Extra: spacy
 Provides-Extra: bpemb
 Provides-Extra: text
 Provides-Extra: vision
 Provides-Extra: pytorch
 Provides-Extra: openai
+Provides-Extra: cohere
 Provides-Extra: all
 Provides-Extra: dev
 
 <img src="https://raw.githubusercontent.com/koaning/embetter/main/docs/images/icon.png" width="125" height="125" align="right" />
 
 # embetter
 
@@ -75,15 +76,15 @@
 # Representations for text
 from embetter.text import SentenceEncoder, Sense2VecEncoder, BytePairEncoder, spaCyEncoder
 
 # Representations from multi-modal models
 from embetter.multi import ClipEncoder
 
 # Finetuning components 
-from embetter.finetune import ForwardFinetuner
+from embetter.finetune import ForwardFinetuner, ContrastiveFinetuner
 
 # External embedding providers, typically needs an API key
 from embetter.external import CohereEncoder, OpenAIEncoder
 ```
 
 All of these components are scikit-learn compatible, which means that you
 can apply them as you would normally in a scikit-learn pipeline. Just be aware
```

### Comparing `embetter-0.4.1/README.md` & `embetter-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 # Representations for text
 from embetter.text import SentenceEncoder, Sense2VecEncoder, BytePairEncoder, spaCyEncoder
 
 # Representations from multi-modal models
 from embetter.multi import ClipEncoder
 
 # Finetuning components 
-from embetter.finetune import ForwardFinetuner
+from embetter.finetune import ForwardFinetuner, ContrastiveFinetuner
 
 # External embedding providers, typically needs an API key
 from embetter.external import CohereEncoder, OpenAIEncoder
 ```
 
 All of these components are scikit-learn compatible, which means that you
 can apply them as you would normally in a scikit-learn pipeline. Just be aware
```

### Comparing `embetter-0.4.1/embetter/error.py` & `embetter-0.5.0/embetter/error.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.1/embetter/external/_cohere.py` & `embetter-0.5.0/embetter/external/_cohere.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import os
 import numpy as np
 
+import cohere
 from embetter.base import EmbetterBase
 
 
 def _batch(iterable, n=1):
     len_iter = len(iterable)
     for ndx in range(0, len_iter, n):
         yield iterable[ndx : min(ndx + n, len_iter)]
@@ -11,41 +13,50 @@
 
 class CohereEncoder(EmbetterBase):
     """
     Encoder that can numerically encode sentences.
 
     Note that this is an **external** embedding provider. If their API breaks, so will this component.
 
+    This encoder will require the `COHERE_KEY` environment variable to be set.
+    If you have it defined in your `.env` file, you can use python-dotenv to load it.
+
+    You also need to install the `cohere` library beforehand.
+
+    ```
+    python -m pip install cohere
+    ```
+
     Arguments:
-        client: cohere client with key
         model: name of model, can be "small" or "large"
 
     **Usage**:
 
     ```python
     import pandas as pd
     from sklearn.pipeline import make_pipeline
     from sklearn.linear_model import LogisticRegression
 
-    from cohere import Client
     from embetter.grab import ColumnGrabber
     from embetter.external import CohereEncoder
+    from dotenv import load_dotenv
+
+    load_dotenv()  # take environment variables from .env.
 
-    client = Client("APIKEY")
     # Let's suppose this is the input dataframe
     dataf = pd.DataFrame({
         "text": ["positive sentiment", "super negative"],
         "label_col": ["pos", "neg"]
     })
 
     # This pipeline grabs the `text` column from a dataframe
     # which then get fed into Cohere's endpoint
     text_emb_pipeline = make_pipeline(
         ColumnGrabber("text"),
-        CohereEncoder(client=client, model="large")
+        CohereEncoder(model="large")
     )
     X = text_emb_pipeline.fit_transform(dataf, dataf['label_col'])
 
     # This pipeline can also be trained to make predictions, using
     # the embedded features.
     text_clf_pipeline = make_pipeline(
         text_emb_pipeline,
@@ -53,16 +64,18 @@
     )
 
     # Prediction example
     text_clf_pipeline.fit(dataf, dataf['label_col']).predict(dataf)
     ```
     """
 
-    def __init__(self, client, model="large"):
-        self.client = client
+    def __init__(self, model="large"):
+        from cohere import Client
+
+        self.client = Client(os.getenv("COHERE_KEY"))
         self.model = model
 
     def transform(self, X, y=None):
         """Transforms the text into a numeric representation."""
         result = []
         for b in _batch(X, 10):
             response = self.client.embed(b)
```

### Comparing `embetter-0.4.1/embetter/external/_openai.py` & `embetter-0.5.0/embetter/external/_openai.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import os
 import numpy as np
-import openai
 
+import openai
 from embetter.base import EmbetterBase
 
 
 def _batch(iterable, n=1):
     len_iter = len(iterable)
     for ndx in range(0, len_iter, n):
         yield iterable[ndx : min(ndx + n, len_iter)]
@@ -13,49 +14,48 @@
 class OpenAIEncoder(EmbetterBase):
     """
     Encoder that can numerically encode sentences.
 
     Note that this is an **external** embedding provider. If their API breaks, so will this component.
     We also assume that you've already importen openai upfront and ran this command:
 
-    ```python
-    import openai
+    This encoder will require the `OPENAI_ORG` and `OPENAI_KEY` environment variables to be set.
+    If you have it defined in your `.env` file, you can use python-dotenv to load it.
 
-    openai.organization = OPENAI_ORG
-    openai.api_key = OPENAI_KEY
+    You also need to install the `openai` library beforehand.
+
+    ```
+    python -m pip install openai
     ```
 
     Arguments:
         model: name of model, can be "small" or "large"
         batch_size: Batch size to send to OpenAI.
 
     **Usage**:
 
     ```python
     import pandas as pd
     from sklearn.pipeline import make_pipeline
     from sklearn.linear_model import LogisticRegression
 
     from embetter.grab import ColumnGrabber
-    from embetter.external import CohereEncoder
-
-    import openai
+    from embetter.external import OpenAIEncoder
+    from dotenv import load_dotenv
 
-    # You must run this first!
-    openai.organization = OPENAI_ORG
-    openai.api_key = OPENAI_KEY
+    load_dotenv()  # take environment variables from .env.
 
     # Let's suppose this is the input dataframe
     dataf = pd.DataFrame({
         "text": ["positive sentiment", "super negative"],
         "label_col": ["pos", "neg"]
     })
 
     # This pipeline grabs the `text` column from a dataframe
-    # which then get fed into Cohere's endpoint
+    # which then get fed into OpenAI's endpoint
     text_emb_pipeline = make_pipeline(
         ColumnGrabber("text"),
         OpenAIEncoder()
     )
     X = text_emb_pipeline.fit_transform(dataf, dataf['label_col'])
 
     # This pipeline can also be trained to make predictions, using
@@ -67,14 +67,17 @@
 
     # Prediction example
     text_clf_pipeline.fit(dataf, dataf['label_col']).predict(dataf)
     ```
     """
 
     def __init__(self, model="text-embedding-ada-002", batch_size=25):
+        # You must run this first!
+        openai.organization = os.getenv("OPENAI_ORG")
+        openai.api_key = os.getenv("OPENAI_KEY")
         self.model = model
         self.batch_size = batch_size
 
     def transform(self, X, y=None):
         """Transforms the text into a numeric representation."""
         result = []
         for b in _batch(X, self.batch_size):
```

### Comparing `embetter-0.4.1/embetter/finetune/_contrastive.py` & `embetter-0.5.0/embetter/finetune/_contrastive.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.1/embetter/finetune/_forward.py` & `embetter-0.5.0/embetter/finetune/_forward.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.1/embetter/grab.py` & `embetter-0.5.0/embetter/grab.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.1/embetter/multi/_clip.py` & `embetter-0.5.0/embetter/multi/_clip.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.1/embetter/text/__init__.py` & `embetter-0.5.0/embetter/text/__init__.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.1/embetter/text/_bpemb.py` & `embetter-0.5.0/embetter/text/_bpemb.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.1/embetter/text/_s2v.py` & `embetter-0.5.0/embetter/text/_s2v.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.1/embetter/text/_sbert.py` & `embetter-0.5.0/embetter/text/_sbert.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.1/embetter/text/_spacy.py` & `embetter-0.5.0/embetter/text/_spacy.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.1/embetter/utils.py` & `embetter-0.5.0/embetter/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,16 @@
 
 
 def batched(iterable: Iterable, n: int = 64):
     """
     Takes an iterable and turns it into a batched iterable.
 
     Arguments:
-        - iterable: the input stream
-        - n: the batch size
+        iterable: the input stream
+        n: the batch size
     """
     if n < 1:
         raise ValueError("n must be at least one")
     it = iter(iterable)
     for batch in tuple(islice(it, n)):
         yield batch
 
@@ -98,21 +98,21 @@
     Shortcut to compare a sequence of inputs to a set of anchors.
 
     The available metrics are: `cityblock`,`cosine`,`euclidean`,`haversine`,`l1`,`l2`,`manhattan` and `nan_euclidean`.
 
     You can read a verbose description of the metrics [here](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise.distance_metrics.html#sklearn.metrics.pairwise.distance_metrics).
 
     Arguments:
-        - inputs: sequence of inputs to calculate scores for
-        - anchors: set/list of anchors to compare against
-        - pipeline: the pipeline to use to calculate the embeddings
-        - anchor_pipeline: the pipeline to apply to the anchors, meant to be used if the anchors should use a different pipeline
-        - metric: the distance metric to use
-        - aggregate: you'll want to aggregate the distances to the different anchors down to a single metric, numpy functions that offer axis=1, like `np.max` and `np.mean`, can be used
-        - n_jobs: set to -1 to use all cores for calculation
+        inputs: sequence of inputs to calculate scores for
+        anchors: set/list of anchors to compare against
+        pipeline: the pipeline to use to calculate the embeddings
+        anchor_pipeline: the pipeline to apply to the anchors, meant to be used if the anchors should use a different pipeline
+        metric: the distance metric to use
+        aggregate: you'll want to aggregate the distances to the different anchors down to a single metric, numpy functions that offer axis=1, like `np.max` and `np.mean`, can be used
+        n_jobs: set to -1 to use all cores for calculation
     """
     X_input = pipeline.transform(inputs)
     if anchor_pipeline:
         X_anchors = anchor_pipeline.transform(anchors)
     else:
         X_anchors = pipeline.transform(anchors)
```

### Comparing `embetter-0.4.1/embetter/vision/_colorhist.py` & `embetter-0.5.0/embetter/vision/_colorhist.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.1/embetter/vision/_loader.py` & `embetter-0.5.0/embetter/vision/_loader.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.1/embetter/vision/_torchvis.py` & `embetter-0.5.0/embetter/vision/_torchvis.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.1/embetter.egg-info/PKG-INFO` & `embetter-0.5.0/embetter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embetter
-Version: 0.4.1
+Version: 0.5.0
 Summary: Just a bunch of useful embeddings to get started quickly.
 Home-page: https://koaning.github.io/embetter/
 Author: Vincent D. Warmerdam
 License: UNKNOWN
 Project-URL: Documentation, https://koaning.github.io/embetter/
 Project-URL: Source Code, https://github.com/koaning/embetter/
 Project-URL: Issue Tracker, https://github.com/koaning/embetter/issues
@@ -23,14 +23,15 @@
 Provides-Extra: sentence-tfm
 Provides-Extra: spacy
 Provides-Extra: bpemb
 Provides-Extra: text
 Provides-Extra: vision
 Provides-Extra: pytorch
 Provides-Extra: openai
+Provides-Extra: cohere
 Provides-Extra: all
 Provides-Extra: dev
 
 <img src="https://raw.githubusercontent.com/koaning/embetter/main/docs/images/icon.png" width="125" height="125" align="right" />
 
 # embetter
 
@@ -75,15 +76,15 @@
 # Representations for text
 from embetter.text import SentenceEncoder, Sense2VecEncoder, BytePairEncoder, spaCyEncoder
 
 # Representations from multi-modal models
 from embetter.multi import ClipEncoder
 
 # Finetuning components 
-from embetter.finetune import ForwardFinetuner
+from embetter.finetune import ForwardFinetuner, ContrastiveFinetuner
 
 # External embedding providers, typically needs an API key
 from embetter.external import CohereEncoder, OpenAIEncoder
 ```
 
 All of these components are scikit-learn compatible, which means that you
 can apply them as you would normally in a scikit-learn pipeline. Just be aware
```

### Comparing `embetter-0.4.1/embetter.egg-info/SOURCES.txt` & `embetter-0.5.0/embetter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `embetter-0.4.1/embetter.egg-info/requires.txt` & `embetter-0.5.0/embetter.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 
 [bpemb]
 bpemb>=0.3.3
 scikit-learn>=1.0.0
 pandas>=1.0.0
 diskcache>=5.6.1
 
+[cohere]
+cohere>=4.11.2
+scikit-learn>=1.0.0
+pandas>=1.0.0
+diskcache>=5.6.1
+
 [dev]
 scikit-learn>=1.0.0
 pandas>=1.0.0
 diskcache>=5.6.1
 sentence-transformers>=2.2.2
 sense2vec==2.0.0
 bpemb>=0.3.3
```

### Comparing `embetter-0.4.1/setup.py` & `embetter-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 vision_packages = ["timm>=0.6.7"]
 
 pytorch_packages = ["torch>=1.12.0"]
 
 openai_packages = ["openai>=0.25.0"]
 
+cohere_packages = ["cohere>=4.11.2"]
+
 
 docs_packages = [
     "mkdocs==1.1",
     "mkdocs-material==4.6.3",
     "mkdocstrings==0.8.0",
     "mktestdocs==0.1.2",
 ]
@@ -38,15 +40,15 @@
 
 all_packages = base_packages + text_packages + vision_packages + openai_packages
 dev_packages = all_packages + docs_packages + test_packages
 
 
 setup(
     name="embetter",
-    version="0.4.1",
+    version="0.5.0",
     author="Vincent D. Warmerdam",
     packages=find_packages(exclude=["notebooks", "docs"]),
     description="Just a bunch of useful embeddings to get started quickly.",
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     license_files=("LICENSE"),
     url="https://koaning.github.io/embetter/",
@@ -61,14 +63,15 @@
         "sentence-tfm": sentence_encoder_pkgs + base_packages,
         "spacy": spacy_packages + base_packages,
         "bpemb": bpemb_packages + base_packages,
         "text": text_packages + base_packages,
         "vision": vision_packages + base_packages,
         "pytorch": pytorch_packages + base_packages,
         "openai": openai_packages + base_packages,
+        "cohere": cohere_packages + base_packages,
         "all": all_packages,
         "dev": dev_packages,
     },
     classifiers=[
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
```

### Comparing `embetter-0.4.1/tests/test_docs.py` & `embetter-0.5.0/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.1/tests/test_finetuners.py` & `embetter-0.5.0/tests/test_finetuners.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.1/tests/test_text.py` & `embetter-0.5.0/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.1/tests/test_utils.py` & `embetter-0.5.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.1/tests/test_vision.py` & `embetter-0.5.0/tests/test_vision.py`

 * *Files identical despite different names*

